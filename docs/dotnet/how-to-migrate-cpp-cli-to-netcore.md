---
title: "How to: Migrate your C++/CLI project from .NET Framework to .NET Core"
ms.date: "07/03/2019"
helpviewer_keywords: ["upgrading Visual C++ applications, /clr:netcore compiler option", "compiling native code [C++]", "interoperability [C++], /clr:netcore compiler option", "interop [C++], /clr:netcore compiler option", "migration [C++], /clr:netcore compiler option", "/clr:netcore compiler option [C++], porting to"]
ms.assetid: 38de764b-b880-46c5-a1f3-49b144ab0520
---

# How to: Migrate your C++/CLI project from .NET Framework to .NET Core

This topic discusses how to move your C++/CLI project from .NET Framework to .NET Core and some of the issues that may arise during the process.

## Changes in your project file

To compile against .NET Core, you need to change your `/clr` switch to `/clr:netcore`. There is no supported .NET Core setting for `/clr:safe` or `/clr:pure`. Only mixed-mode C++/CLI is supported on .NET Core. Additionally, you currently need to specify paths to all assemblies that you use, including the built-in .NET Core framework. This should be fixed by the first supported release of the `/clr:netcore` switch.

### Minimum versions

C++/CLI on .NET Core requires Visual Studio 2019.3 and will run on .NET Core 3.0 or newer on Windows.

## The IJW Host

When compiling with the `/clr:netcore` switch, you may notice that there is a new `ijwhost.dll` in your output directory. This file is required to help bootstrap loading your C++/CLI assembly into the .NET Core runtime. Additionally, it resolves and loads the runtime into your application if your first usage of managed code is through a native entry-point exposed by your C++/CLI application. If the `ijwhost.dll` is not present, then your C++/CLI assembly will fail to load.

This same concept existed with the `/clr` switch; however, it was supplied by the globally-installed `mscoree.dll`, so it didn't have to travel with your application.

If you try to use a mixed-mode C++/CLI assembly compiled for .NET Framework in .NET Core, then you might end up with weird glitches, unexplained behavior, or exceptions since you may end up loading both .NET Framework and .NET Core into the same process, which is an unsupported scenario.

## C++/CLI executables

When compiling a C++/CLI executable project, you may notice that you get a DLL instead of an EXE file. This is expected behavior. In .NET Core, all assemblies are DLLs, even executables. To run the executable, you can run `dotnet MyExecutable.dll`.

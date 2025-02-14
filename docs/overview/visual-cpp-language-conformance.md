---
title: "Microsoft C++ Language Conformance Table"
ms.date: "05/20/2019"
ms.technology: "cpp-language"
ms.assetid: 475da6e9-0d78-4b4e-bd23-f41c406c4efe
author: "corob-msft"
ms.author: "corob"
---
# Microsoft C++ Language Conformance Table

This topic summarizes the ISO C++03, C++11, C++14, C++17, and C++20 language standards conformance of compiler features and Standard Library features for the Microsoft C++ compiler in Visual Studio 2019 and earlier versions. Each compiler and standard library feature name links to the ISO C++ Standard proposal paper that describes the feature, if one is available at publication time. The Supported column lists the Visual Studio version in which support for the feature first appeared.

For details on conformance improvements and other changes in Visual Studio 2017 or Visual Studio 2019, set the version selector in the upper left of this page, then see [C++ conformance improvements in Visual Studio](cpp-conformance-improvements.md) and [What's New for Visual C++ in Visual Studio](what-s-new-for-visual-cpp-in-visual-studio.md). For conformance changes in earlier versions, see [Visual C++ change history](../porting/visual-cpp-change-history-2003-2015.md) and [Visual C++ What's New 2003 through 2015](../porting/visual-cpp-what-s-new-2003-through-2015.md). For current news from the C++ team, visit the [C++ team blog](https://devblogs.microsoft.com/cppblog/).

> [!NOTE]
> There are no binary breaking changes between Visual Studio 2015, Visual Studio 2017, and Visual Studio 2019.

## Compiler Features

|Feature Area| |
|----|---|
|__C++03/11 Core Language Features__|__Supported__|
|&nbsp;&nbsp;Everything else|VS 2015 <sup>[A](#note_A)</sup>|
|&nbsp;&nbsp;Two-phase name lookup|VS 2017 15.7 <sup>[B](#note_B)</sup>|
|&nbsp;&nbsp;[N2634 Expression SFINAE](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2008/n2634.html)|VS 2017 15.7|
|&nbsp;&nbsp;[N1653 C99 preprocessor](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2004/n1653.htm)|Partial <sup>[C](#note_C)</sup>|
|__C++14 Core Language Features__|__Supported__|
|&nbsp;&nbsp;[N3323 Tweaked wording for contextual conversions](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2012/n3323.pdf)|VS 2013|
|&nbsp;&nbsp;[N3472 Binary literals](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2012/n3472.pdf)|VS 2015|
|&nbsp;&nbsp;[N3638 auto and decltype(auto) return types](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3638.html)|VS 2015|
|&nbsp;&nbsp;[N3648 init-captures](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3648.html)|VS 2015|
|&nbsp;&nbsp;[N3649 Generic lambdas](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3649.html)|VS 2015|
|&nbsp;&nbsp;[N3760 \[\[deprecated\]\] attribute](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3760.html)|VS 2015|
|&nbsp;&nbsp;[N3778 Sized deallocation](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3778.html)|VS 2015|
|&nbsp;&nbsp;[N3781 Digit separators](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3781.pdf)|VS 2015|
|&nbsp;&nbsp;[N3651 Variable templates](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3651.pdf)|VS 2015.2|
|&nbsp;&nbsp;[N3652 Extended constexpr](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3652.html)|VS 2017 15.0|
|&nbsp;&nbsp;[N3653 Default member initializers for aggregates](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3653.html)|VS 2017 15.0|
|__C++17 Core Language Features__|__Supported__|
|&nbsp;&nbsp;[N4086 Removing trigraphs](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n4086.html)|VS 2010 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[N3922 New rules for auto with braced-init-lists](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n3922.html)|VS 2015 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[N4051 typename in template template-parameters](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n4051.html)|VS 2015 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[N4266 Attributes for namespaces and enumerators](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n4266.html)|VS 2015 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[N4267 u8 character literals](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n4267.html)|VS 2015 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[N4230 Nested namespace definitions](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n4230.html)|VS 2015.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[N3928 Terse static_assert](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n3928.pdf)|VS 2017 15.0 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0184R0 Generalized range-based for-loops](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0184r0.html)|VS 2017 15.0 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0188R1 \[\[fallthrough\]\] attribute](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0188r1.pdf)|VS 2017 15.0 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0001R1 Removing the register keyword](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/p0001r1.html)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0002R1 Removing operator++ for bool](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/p0002r1.html)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0018R3 Capturing *this by value](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0018r3.html)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0028R4 Using attribute namespaces without repetition](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0028r4.html)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0061R1 \_\_has_include](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/p0061r1.html)|VS 2017 15.3 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0138R2 Direct-list-init of fixed enums from integers](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0138r2.pdf)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0170R1 constexpr lambdas](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0170r1.pdf)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0189R1 \[\[nodiscard\]\] attribute](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0189r1.pdf)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0212R1 \[\[maybe_unused\]\] attribute](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0212r1.pdf)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0217R3 Structured bindings](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0217r3.html)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0292R2 constexpr if-statements](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0292r2.html)|VS 2017 15.3 <sup>[D](#note_D)</sup>|
|&nbsp;&nbsp;[P0305R1 Selection statements with initializers](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0305r1.html)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0245R1 Hexfloat literals](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0245r1.html)|VS 2017 15.5 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[N4268 Allowing more non-type template args](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n4268.html)|VS 2017 15.5 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[N4295 Fold expressions](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n4295.html)|VS 2017 15.5 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0003R5 Removing dynamic-exception-specifications](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0003r5.html)|VS 2017 15.5 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0012R1 Adding noexcept to the type system](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/p0012r1.html)|VS 2017 15.5 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0035R4 Over-aligned dynamic memory allocation](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0035r4.html)|VS 2017 15.5 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0386R2 Inline variables](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0386r2.pdf)|VS 2017 15.5 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0522R0 Matching template template-parameters to compatible arguments](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0522r0.html)|VS 2017 15.5 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0036R0 Removing some empty unary folds](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/p0036r0.pdf)|VS 2017 15.5 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[N4261 Fixing qualification conversions](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n4261.html)|VS 2017 15.7 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0017R1 Extended aggregate initialization](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/p0017r1.html)|VS 2017 15.7 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0091R3 Template argument deduction for class templates](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0091r3.html)<br/>&nbsp;&nbsp;[P0512R0 Class template argument deduction issues](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0512r0.pdf)|VS 2017 15.7 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0127R2 Declaring non-type template parameters with auto](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0127r2.html)|VS 2017 15.7 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0135R1 Guaranteed copy elision](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0135r1.html)|VS 2017 15.6|
|&nbsp;&nbsp;[P0136R1 Rewording inheriting constructors](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/p0136r1.html)|VS 2017 15.7 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0137R1 std::launder](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0137r1.html)|VS 2017 15.7 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0145R3 Refining expression evaluation order](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0145r3.pdf)<br/>&nbsp;&nbsp;[P0400R0 Order of evaluation of function arguments](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0400r0.html)|VS 2017 15.7 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0195R2 Pack expansions in using-declarations](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0195r2.html)|VS 2017 15.7 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0283R2 Ignoring unrecognized attributes](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0283r2.html)|VS 2015 <sup>[14](#note_14)</sup>|


|Feature Area| |
|----|---|
|__C++17 Core Language Features (Defect Reports)__|__Supported__|
|&nbsp;&nbsp;[P0702R1 Fixing class template argument deduction for initializer-list ctors](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0702r1.html)|VS 2017 15.7 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0961R1 Relaxing the structured bindings customization point finding rules](http://open-std.org/JTC1/SC22/WG21/docs/papers/2018/p0961r1.html)|VS 2019 16.0 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0969R0 Allowing structured bindings to accessible members](http://open-std.org/JTC1/SC22/WG21/docs/papers/2018/p0969r0.pdf)|VS 2019 16.0 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0588R1 Simplifying implicit lambda capture](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0588r1.html)|No|
|&nbsp;&nbsp;[P0962R2 Relaxing the range-for loop customization point finding rules](http://open-std.org/JTC1/SC22/WG21/docs/papers/2018/p0962r1.html)|No|
|&nbsp;&nbsp;[P0929R2 Checking for abstract class types](https://wg21.link/P0929R2)|No|
|&nbsp;&nbsp;[P1009R2 Array size deduction in new-expressions](https://wg21.link/P1009R2)|No|
|&nbsp;&nbsp;[P1286R2 Contra CWG DR1778](https://wg21.link/P1286R2)|No|
|Feature Area| |
|----|---|
|__C++20 Core Language Features__|__Supported__|
|&nbsp;&nbsp;[P0704R1 Fixing const lvalue ref-qualified pointers to members](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0704r1.html)|VS 2015 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P1041R4 Make char16_t/char32_t string literals be UTF-16/32](https://wg21.link/P1041R4)|VS 2015 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P1330R0 Changing the active member of a union inside constexpr](https://wg21.link/P1330R0)|VS 2017 15.0 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0972R0 noexcept For \<chrono> zero(), min(), max()](https://wg21.link/P0972R0)|VS 2017 15.7 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0515R3 Three-way (spaceship) comparison operator <=>](https://wg21.link/P0515R3)|VS 2019 16.0 <sup>[20](#note_20)</sup>|
|&nbsp;&nbsp;[P1008R1 Prohibiting aggregates with user-declared constructors](https://wg21.link/P1008R1)|VS 2019 16.0 <sup>[20](#note_20)</sup>|
|&nbsp;&nbsp;[P0329R4 Designated initialization](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0329r4.pdf)|VS 2019 16.1 <sup>[20](#note_20)</sup>|
|&nbsp;&nbsp;[P0409R2 Allowing lambda-capture \[=, this\]](http://open-std.org/JTC1/SC22/WG21/docs/papers/2017/p0409r2.html)|VS 2019 16.1 <sup>[20](#note_20)</sup>|
|&nbsp;&nbsp;[P0515R3 Three-way (spaceship) comparison operator <=>](https://wg21.link/P0515R3)|VS 2019 16.0 <sup>[20](#note_20)</sup>|
|&nbsp;&nbsp;[P0941R2 Feature-test macros](https://wg21.link/P0941R2)|VS 2019 16.0 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P1008R1 Prohibiting aggregates with user-declared constructors](https://wg21.link/P1008R1)|VS 2019 16.0 <sup>[20](#note_20)</sup>|
|&nbsp;&nbsp;[P0846R0 ADL and function templates that are not visible](https://wg21.link/P0846R0)|VS 2019 16.1 <sup>[20](#note_20)</sup>|
|&nbsp;&nbsp;[P0641R2 const mismatch with defaulted copy constructor](https://wg21.link/P0641R2)|Partial|
|&nbsp;&nbsp;[P0306R4 Adding \_\_VA_OPT\_\_ for comma omission and comma deletion](https://wg21.link/P0306R4)|No|
|&nbsp;&nbsp;[P0315R4 Allowing lambdas in unevaluated contexts](https://wg21.link/P0315R4)|No|
|&nbsp;&nbsp;[P0409R2 Allowing lambda-capture \[=, this\]](https://wg21.link/P0409R2)|No|
|&nbsp;&nbsp;[P0428R2 Familiar template syntax for generic lambdas](http://www.open-std.org/jtc1/sc22/wg21/docs/pa pers/2017/p0428r2.pdf)|No|
|&nbsp;&nbsp;[P0479R5 \[\[likely\]\] and \[\[unlikely\]\] attributes](https://wg21.link/P0479R5)|No|
|&nbsp;&nbsp;[P0542R5 Contracts](https://wg21.link/P0542R5)|No|
|&nbsp;&nbsp;[P0614R1 Range-based for-loops with initializers](https://wg21.link/P0614R1)|No|
|&nbsp;&nbsp;[P0624R2 Default constructible and assignable stateless lambdas](https://wg21.link/P0624R2)|No|
|&nbsp;&nbsp;[P0634R3 Down with typename!](https://wg21.link/P0634R3)|No|
|&nbsp;&nbsp;[P0683R1 Default member initializers for bit-fields](https://wg21.link/P0683R1)|No|
|&nbsp;&nbsp;[P0692R1 Relaxing access checking on specializations](https://wg21.link/P0692R1)|No|
|&nbsp;&nbsp;[P0722R3 Efficient sized delete for variable sized classes](https://wg21.link/P0722R3)|No|
|&nbsp;&nbsp;[P0732R2 Class types in non-type template parameters](https://wg21.link/P0732R2)|No|
|&nbsp;&nbsp;[P0734R0 Concepts](https://wg21.link/P0734R0)|No|
|&nbsp;&nbsp;[P0780R2 Allowing pack expansion in lambda init-capture](https://wg21.link/P0780R2)|No|
|&nbsp;&nbsp;[P0806R2 Deprecate implicit capture of this via \[=\]](https://wg21.link/P0806R2)|No|
|&nbsp;&nbsp;[P0840R2 \[\[no_unique_address\]\] attribute](https://wg21.link/P0840R2)|No|
|&nbsp;&nbsp;[P0857R0 Fixing functionality gaps in constraints](https://wg21.link/P0857R0)|No|
|&nbsp;&nbsp;[P0892R2 Conditional explicit](https://wg21.link/P0892R2)|No|
|&nbsp;&nbsp;[P0912R5 Coroutines](https://wg21.link/P0912R5)|No|
|&nbsp;&nbsp;[P0960R3 Allow initializing aggregates from a parenthesized list of values](https://wg21.link/P0960R3)|No|
|&nbsp;&nbsp;[P1002R1 try-catch blocks in constexpr functions](https://wg21.link/P1002R1)|No|
|&nbsp;&nbsp;[P1064R0 Allowing virtual function calls in constant expressions](https://wg21.link/P1064R0)|No|
|&nbsp;&nbsp;[P1073R3 Immediate functions](https://wg21.link/P1073R3)|No|
|&nbsp;&nbsp;[P1084R2 Today's return-type-requirements are insufficient](https://wg21.link/P1084R2)|No|
|&nbsp;&nbsp;[P1091R3 Extending structured bindings to be more like variable declarations](https://wg21.link/P1091R3)|No|
|&nbsp;&nbsp;[P1094R2 Nested inline namespaces](https://wg21.link/P1094R2)|No|
|&nbsp;&nbsp;[P1103R3 Modules](https://wg21.link/P1103R3)|No|
|&nbsp;&nbsp;[P1120R0 Consistency improvements for <=> and other comparison operators](https://wg21.link/P1120R0)|No|
|&nbsp;&nbsp;[P1139R2 Address wording issues related to ISO 10646](https://wg21.link/P1139R2)|No|
|&nbsp;&nbsp;[P1141R2 Yet another approach for constrained declarations](https://wg21.link/P1141R2)|No|
|&nbsp;&nbsp;[P1185R2 \<=\> != ==](https://wg21.link/P1185R2)|No|
|&nbsp;&nbsp;[P1236R1 Signed integers are two's complement](https://wg21.link/P1236R1)|No|
|&nbsp;&nbsp;[P1289R1 Access control in contract conditions](https://wg21.link/P1289R1)|No|
|&nbsp;&nbsp;[P1323R2 Contract postconditions and return type deduction](https://wg21.link/P1323R2)|No|
|&nbsp;&nbsp;[P1327R1 Allowing dynamic_cast, polymorphic typeid in constant expressions](https://wg21.link/P1327R1)|No|
|&nbsp;&nbsp;[P1353R0 Missing feature-test macros](https://wg21.link/P1353R0)|No|
|&nbsp;&nbsp;[P1381R1 Reference capture of structured bindings](https://wg21.link/P1381R1)|No|

## Standard Library Features

|Feature Area| |
|---|---|
|__C++20 Standard Library Features__|__Supported__|
|&nbsp;&nbsp;[P0809R0 Comparing Unordered Containers](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2018/p0809r0.pdf)| VS 2010 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0858R0 Constexpr Iterator Requirements](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2018/p0858r0.html)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0777R1 Avoiding Unnecessary Decay](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0777r1.pdf)|VS 2017 15.7 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0550R2 remove_cvref](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0550r2.pdf)|VS 2019 16.0 <sup>[20](#note_20)</sup>|
|&nbsp;&nbsp;[P0318R1 unwrap_reference, unwrap_ref_decay](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2018/p0318r1.pdf)|VS 2019 16.1 <sup>[20](#note_20)</sup>|
|&nbsp;&nbsp;[P0457R2 starts_with()/ends_with() For basic_string/basic_string_view](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0457r2.html)|VS 2019 16.1 <sup>[20](#note_20)</sup>|
|&nbsp;&nbsp;[P0458R2 contains() For Ordered And Unordered Associative Containers](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2018/p0458r2.html)|VS 2019 16.1 <sup>[20](#note_20)</sup>|
|&nbsp;&nbsp;[P0646R1 list/forward_list remove()/remove_if()/unique() Return size_type](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2018/p0646r1.pdf)|VS 2019 16.1 <sup>[20](#note_20)</sup>|
|&nbsp;&nbsp;[P0769R2 shift_left(), shift_right()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2018/p0769r2.pdf)|VS 2019 16.1 <sup>[20](#note_20)</sup>|
|&nbsp;&nbsp;[P0887R1 type_identity](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2018/p0887r1.pdf)|VS 2019 16.1 <sup>[20](#note_20)</sup>|
|&nbsp;&nbsp;[P0019R8 atomic_ref](https://wg21.link/P0019R8)|No|
|&nbsp;&nbsp;[P0020R6 atomic\<float>, atomic\<double>, atomic\<long double>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0020r6.html)|No|
|&nbsp;&nbsp;[P0053R7 \<syncstream>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0053r7.pdf)<br/>&nbsp;&nbsp;[P0753R2 osyncstream Manipulators](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2018/p0753r2.pdf)|No|
|&nbsp;&nbsp;[P0122R7 \<span>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2018/p0122r7.pdf)|No|
|&nbsp;&nbsp;[P0202R3 constexpr For \<algorithm> And exchange()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0202r3.html)|No|
|&nbsp;&nbsp;[P0339R6 polymorphic_allocator<>](https://wg21.link/P0339R6)|No|
|&nbsp;&nbsp;[P0340R3 SFINAE-Friendly underlying_type](https://wg21.link/P0340R3)|No|
|&nbsp;&nbsp;[P0355R7 \<chrono> Calendars And Time Zones](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2018/p0355r7.html)|No|
|&nbsp;&nbsp;[P0356R5 bind_front()](https://wg21.link/P0356R5)|No|
|&nbsp;&nbsp;[P0357R3 Supporting Incomplete Types In reference_wrapper](https://wg21.link/P0357R3)|No|
|&nbsp;&nbsp;[P0415R1 constexpr For \<complex> (Again)](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0415r1.html)|No|
|&nbsp;&nbsp;[P0439R0 enum class memory_order](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0439r0.html)|No|
|&nbsp;&nbsp;[P0463R1 endian](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0463r1.html)|No|
|&nbsp;&nbsp;[P0475R1 Guaranteed Copy Elision For Piecewise Construction](https://wg21.link/P0475R1)|No|
|&nbsp;&nbsp;[P0476R2 <bit> bit_cast](https://wg21.link/P0476R2)|No|
|&nbsp;&nbsp;[P0482R6 char8_t: A type for UTF-8 characters and strings](https://wg21.link/P0482R6)|No|
|&nbsp;&nbsp;[P0487R1 Fixing operator>>(basic_istream&, CharT*)](https://wg21.link/P0487R1)|No|
|&nbsp;&nbsp;[P0528R3 Atomic Compare-And-Exchange With Padding Bits](https://wg21.link/P0528R3)|No|
|&nbsp;&nbsp;[P0556R3 <bit> ispow2(), ceil2(), floor2(), log2p1()](https://wg21.link/P0556R3)|No|
|&nbsp;&nbsp;[P0591R4 Utility Functions For Uses-Allocator Construction](https://wg21.link/P0591R4)|No|
|&nbsp;&nbsp;[P0600R1 \[\[nodiscard\]\] For The STL, Part 1](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0600r1.pdf)|No|
|&nbsp;&nbsp;[P0608R3 Improving variant's Converting Constructor/Assignment](https://wg21.link/P0608R3)|No|
|&nbsp;&nbsp;[P0616R0 Using move() In \<numeric>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0616r0.pdf)|No|
|&nbsp;&nbsp;[P0619R4 Removing C++17-Deprecated Features In C++20](https://wg21.link/P0619R4)|No|
|&nbsp;&nbsp;[P0653R2 to_address()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0653r2.html)|No|
|&nbsp;&nbsp;[P0655R1 visit<R>()](https://wg21.link/P0655R1)|No|
|&nbsp;&nbsp;[P0674R1 make_shared() For Arrays](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0674r1.html)|No|
|&nbsp;&nbsp;[P0718R2 atomic\<shared_ptr\<T>>, atomic\<weak_ptr\<T>>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0718r2.html)|No|
|&nbsp;&nbsp;[P0738R2 istream_iterator Cleanup](https://wg21.link/P0738R2)|No|
|&nbsp;&nbsp;[P0754R2 \<version>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2018/p0754r2.pdf)|No|
|&nbsp;&nbsp;[P0758R1 is_nothrow_convertible](https://wg21.link/P0758R1)|No|
|&nbsp;&nbsp;[P0767R1 Deprecating is_pod](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0767r1.html)|No|
|&nbsp;&nbsp;[P0768R1 Library Support For The Spaceship Comparison Operator \<=>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0768r1.pdf)|No|
|&nbsp;&nbsp;[P0771R1 noexcept For std::function's Move Constructor](https://wg21.link/P0771R1)|No|
|&nbsp;&nbsp;[P0811R3 midpoint(), lerp()](https://wg21.link/P0811R3)|No|
|&nbsp;&nbsp;[P0879R0 constexpr For Swapping Functions](https://wg21.link/P0879R0)|No|
|&nbsp;&nbsp;[P0896R4 \<ranges\>](https://wg21.link/P0896R4)|No|
|&nbsp;&nbsp;[P0898R3 Standard Library Concepts](https://wg21.link/P0898R3)|No|
|&nbsp;&nbsp;[P0912R5 Library Support For Coroutines](https://wg21.link/P0912R5)|No|
|&nbsp;&nbsp;[P0919R3 Heterogeneous Lookup For Unordered Containers](https://wg21.link/P0919R3)|No|
|&nbsp;&nbsp;[P0920R2 Precalculated Hash Value Lookup](https://wg21.link/P0920R2)|No|
|&nbsp;&nbsp;[P0935R0 Eradicating Unnecessarily Explicit Default Constructors](https://wg21.link/P0935R0)|No|
|&nbsp;&nbsp;[P0966R1 string::reserve() Should Not Shrink](https://wg21.link/P0966R1)|No|
|&nbsp;&nbsp;[P1001R2 execution::unseq](https://wg21.link/P1001R2)|No|
|&nbsp;&nbsp;[P1006R1 constexpr For pointer_traits<T*>::pointer_to()](https://wg21.link/P1006R1)|No|
|&nbsp;&nbsp;[P1007R3 assume_aligned()](https://wg21.link/P1007R3)|No|
|&nbsp;&nbsp;[P1020R1 Smart Pointer Creation With Default Initialization](https://wg21.link/P1020R1)|No|
|&nbsp;&nbsp;[P1023R0 constexpr For std::array Comparisons](https://wg21.link/P1023R0)|No|
|&nbsp;&nbsp;[P1032R1 Miscellaneous constexpr](https://wg21.link/P1032R1)|No|
|&nbsp;&nbsp;[P1165R1 Consistently Propagating Stateful Allocators In basic_string's operator+()](https://wg21.link/P1165R1)|No|
|&nbsp;&nbsp;[P1209R0 erase_if(), erase()](https://wg21.link/P1209R0)|No|
|&nbsp;&nbsp;[P1227R2 Signed std::ssize(), Unsigned span::size()](https://wg21.link/P1227R2)|No|
|&nbsp;&nbsp;[P1285R0 Improving Completeness Requirements For Type Traits](https://wg21.link/P1285R0)|No|
|&nbsp;&nbsp;[P1357R1 is_bounded_array, is_unbounded_array](https://wg21.link/P1357R1)|No|
|__C++17 Standard Library Features__|__Supported__|
|&nbsp;&nbsp;[LWG 2221 Formatted output operator for nullptr](https://cplusplus.github.io/LWG/issue2221)|VS 2019 16.1|
|&nbsp;&nbsp;[N3911 void_t](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n3911.pdf)|VS 2015 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[N4089 Safe Conversions In unique_ptr\<T[]>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n4089.pdf)|VS 2015 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[N4169 invoke()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n4169.html)|VS 2015 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[N4190 Removing auto_ptr, random_shuffle(), And Old \<functional> Stuff](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n4190.htm)|VS 2015 <sup>[rem](#note_rem)</sup>|
|&nbsp;&nbsp;[N4258 noexcept Cleanups](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n4258.pdf)|VS 2015 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[N4259 uncaught_exceptions()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n4259.pdf)|VS 2015 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[N4277 Trivially Copyable reference_wrapper](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n4277.html)|VS 2015 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[N4279 insert_or_assign()/try_emplace() For map/unordered_map](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n4279.html)|VS 2015 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[N4280 size(), empty(), data()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n4280.pdf)|VS 2015 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[N4366 Precisely Constraining unique_ptr Assignment](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/n4366.html)|VS 2015 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[N4387 Improving pair And tuple](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/n4387.html)|VS 2015.2 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[N4389 bool_constant](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/n4389.html)|VS 2015 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[N4508 shared_mutex (Untimed)](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/n4508.html)|VS 2015.2 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[N4510 Supporting Incomplete Types In vector/list/forward_list](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/n4510.html)|VS 2013 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[N4562 Library Fundamentals: \<algorithm> sample()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/n4562.html#alg.random.sample)|VS 2017 15.0|
|&nbsp;&nbsp;[N4562 Library Fundamentals: \<any>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/n4562.html#any)|VS 2017 15.0|
|&nbsp;&nbsp;[N4562 Library Fundamentals: \<memory_resource>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/n4562.html#memory.resource.synop)<br/>&nbsp;&nbsp;[P0337R0 Deleting polymorphic_allocator Assignment](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0337r0.html)|VS 2017 15.6|
|&nbsp;&nbsp;[N4562 Library Fundamentals: \<optional>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/n4562.html#optional)|VS 2017 15.0|
|&nbsp;&nbsp;[N4562 Library Fundamentals: \<string_view>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/n4562.html#string.view)|VS 2017 15.0|
|&nbsp;&nbsp;[N4562 Library Fundamentals: \<tuple> apply()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/n4562.html#tuple)|VS 2017 15.0|
|&nbsp;&nbsp;[N4562 Library Fundamentals: Boyer-Moore search()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/n4562.html#func.searchers.boyer_moore)<br/>&nbsp;&nbsp;[P0253R1 Fixing Searcher Return Types](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0253r1.pdf)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0003R5 Removing Dynamic Exception Specifications](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0003r5.html)|VS 2017 15.5 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0004R1 Removing Deprecated Iostreams Aliases](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/p0004r1.html)|VS 2015.2 <sup>[rem](#note_rem)</sup>|
|&nbsp;&nbsp;[P0005R4 not_fn()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0005r4.html)<br/>&nbsp;&nbsp;[P0358R1 Fixes For not_fn()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0358r1.html)|VS 2017 15.5 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0006R0 Variable Templates For Type Traits (is_same_v, etc.)](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/p0006r0.html)|VS 2015.2 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0007R1 as_const()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/p0007r1.html)|VS 2015.2 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0013R1 Logical Operator Type Traits (conjunction, etc.)](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/p0013r1.html)|VS 2015.2 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0024R2 Parallel Algorithms](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0024r2.html)<br/>&nbsp;&nbsp;[P0336R1 Renaming Parallel Execution Policies](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0336r1.pdf)<br/>&nbsp;&nbsp;[P0394R4 Parallel Algorithms Should terminate() For Exceptions](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0394r4.html)<br/>&nbsp;&nbsp;[P0452R1 Unifying \<numeric> Parallel Algorithms](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0452r1.html)|VS 2017 15.7|
|&nbsp;&nbsp;[P0025R1 clamp()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/p0025r1.html)|VS 2015.3|
|&nbsp;&nbsp;[P0030R1 hypot(x, y, z)](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/p0030r1.pdf)|VS 2017 15.7|
|&nbsp;&nbsp;[P0031R0 constexpr For \<array> (Again) And \<iterator>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/p0031r0.html)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0032R3 Homogeneous Interface For variant/any/optional](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0032r3.pdf)|VS 2017 15.0|
|&nbsp;&nbsp;[P0033R1 Rewording enable_shared_from_this](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0033r1.html)|VS 2017 15.5 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0040R3 Extending Memory Management Tools](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0040r3.html)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0063R3 C11 Standard Library](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0063r3.html)|VS 2015 <sup>[C11](#note_C11), [14](#note_14)</sup>|
|&nbsp;&nbsp;[P0067R5 Elementary String Conversions](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0067r5.html)|VS 2017 15.7 <sup>[charconv](#note_charconv)</sup>|
|&nbsp;&nbsp;[P0074R0 owner_less\<>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/p0074r0.html)|VS 2015.2 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0077R2 is_callable, is_nothrow_callable](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0077r2.html)|VS 2017 15.0|
|&nbsp;&nbsp;[P0083R3 Splicing Maps And Sets](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0083r3.pdf)<br/>&nbsp;&nbsp;[P0508R0 Clarifying insert_return_type](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0508r0.html)|VS 2017 15.5 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0084R2 Emplace Return Type](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0084r2.pdf)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0088R3 \<variant>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0088r3.html)|VS 2017 15.0|
|&nbsp;&nbsp;[P0092R1 \<chrono> floor(), ceil(), round(), abs()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/p0092r1.html)|VS 2015.2 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0152R1 atomic::is_always_lock_free](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0152r1.html)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0154R1 hardware_destructive_interference_size, etc.](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0154r1.html)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0156R0 Variadic lock_guard](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/p0156r0.html)|VS 2015.2 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0156R2 Renaming Variadic lock\_guard to scoped\_lock](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0156r2.html)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0163R0 shared_ptr::weak_type](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2015/p0163r0.html)|VS 2017 15.0|
|&nbsp;&nbsp;[P0174R2 Deprecating Vestigial Library Parts](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0174r2.html)|VS 2017 15.5 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0185R1 is_swappable, is_nothrow_swappable](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0185r1.html)|VS 2015.3|
|&nbsp;&nbsp;[P0209R2 make_from_tuple()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0209r2.pdf)|VS 2017 15.0|
|&nbsp;&nbsp;[P0218R1 \<filesystem>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0218r1.html)<br/>&nbsp;&nbsp;[P0219R1 Relative Paths For Filesystem](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0219r1.html)<br/>&nbsp;&nbsp;[P0317R1 Directory Entry Caching For Filesystem](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0317r1.html)<br/>&nbsp;&nbsp;[P0392R0 Supporting string_view In Filesystem Paths](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0392r0.pdf)<br/>&nbsp;&nbsp;[P0430R2 Supporting Non-POSIX Filesystems](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0430r2.pdf)<br/>&nbsp;&nbsp;[P0492R2 Resolving NB Comments for Filesystem](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0492r2.html)|VS 2017 15.7 <sup>[E](#note_E)</sup>|
|&nbsp;&nbsp;[P0220R1 Library Fundamentals V1](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0220r1.html)|VS 2017 15.6|
|&nbsp;&nbsp;[P0226R1 Mathematical Special Functions](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0226r1.pdf)|VS 2017 15.7|
|&nbsp;&nbsp;[P0254R2 Integrating string_view And std::string](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0254r2.pdf)|VS 2017 15.0|
|&nbsp;&nbsp;[P0258R2 has_unique_object_representations](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0258r2.html)|VS 2017 15.3 <sup>[G](#note_G)</sup>|
|&nbsp;&nbsp;[P0272R1 Non-const basic_string::data()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0272r1.html)|VS 2015.3|
|&nbsp;&nbsp;[P0295R0 gcd(), lcm()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0295r0.pdf)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0298R3 std::byte](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0298r3.pdf)|VS 2017 15.3 <sup>[17](#note_17),&nbsp;[byte](#note_byte)</sup>|
|&nbsp;&nbsp;[P0302R1 Removing Allocator Support In std::function](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0302r1.html)|VS 2017 15.5 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0307R2 Making Optional Greater Equal Again](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0307r2.pdf)|VS 2017 15.0|
|&nbsp;&nbsp;[P0393R3 Making Variant Greater Equal](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0393r3.html)|VS 2017 15.0|
|&nbsp;&nbsp;[P0403R1 UDLs For \<string_view> ("meow"sv, etc.)](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0403r1.html)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0414R2 shared_ptr\<T[]>, shared_ptr\<T[N]>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0414r2.html)<br/>&nbsp;&nbsp;[P0497R0 Fixing shared_ptr For Arrays](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0497r0.html)|VS 2017 15.5 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0418R2 atomic compare_exchange memory_order Requirements](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0418r2.html)|VS 2017 15.3 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0426R1 constexpr For char_traits](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0426r1.html)|VS 2017 15.7|
|&nbsp;&nbsp;[P0433R2 Integrating template deduction for class templates into the standard library](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0433r2.html)<br/>&nbsp;&nbsp;[P0739R0 Improving class template argument deduction integration into the standard library](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0739r0.html)|VS 2017 15.7|
|&nbsp;&nbsp;[P0435R1 Overhauling common_type](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0435r1.pdf)<br/>&nbsp;&nbsp;[P0548R1 Tweaking common\_type and duration](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0548r1.pdf)|VS 2017 15.3 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0504R0 Revisiting in_place_t/in_place_type_t\<T>/in_place_index_t\<I>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0504r0.html)|VS 2017 15.0|
|&nbsp;&nbsp;[P0505R0 constexpr For \<chrono> (Again)](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0505r0.html)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0510R0 Rejecting variants Of Nothing, Arrays, References, And Incomplete Types](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0510r0.html)|VS 2017 15.0|
|&nbsp;&nbsp;[P0513R0 Poisoning hash](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0513r0.pdf)<br/>&nbsp;&nbsp;[P0599R1 noexcept hash](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0599r1.pdf)|VS 2017 15.3 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0516R0 Marking shared_future Copying As noexcept](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0516r0.html)|VS 2017 15.3 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0517R0 Constructing future_error From future_errc](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0517r0.html)|VS 2017 15.3 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0521R0 Deprecating shared_ptr::unique()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0521r0.html)|VS 2017 15.5 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0558R1 Resolving atomic\<T> Named Base Class Inconsistencies](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0558r1.pdf)|VS 2017 15.3 <sup>[14](#note_14)</sup>|
|&nbsp;&nbsp;[P0595R2 std::is_constant_evaluated()](https://wg21.link/P0595R2)|No|
|&nbsp;&nbsp;[P0602R4 Propagating Copy/Move Triviality In variant/optional](https://wg21.link/P0602R4)|VS 2017 15.3<sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0604R0 Changing is\_callable/result\_of To invoke\_result, is\_invocable, is\_nothrow\_invocable](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0604r0.html)|VS 2017 15.3 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0607R0 Inline Variables for the Standard Library](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0607r0.html)|VS 2017 15.5 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0618R0 Deprecating \<codecvt>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0618r0.html)|VS 2017 15.5 <sup>[17](#note_17)</sup>|
|&nbsp;&nbsp;[P0682R1 Repairing Elementary String Conversions](https://wg21.link/P0682R1)|VS 2015 15.7 <sup>[17](#note_17)</sup>|
|__C++14 Standard Library Features__|__Supported__|
|&nbsp;&nbsp;[N3462 SFINAE-Friendly result_of](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2012/n3462.html)|VS 2015.2|
|&nbsp;&nbsp;[N3302 constexpr For \<complex>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2011/n3302.html)|VS 2015|
|&nbsp;&nbsp;[N3469 constexpr For \<chrono>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2012/n3469.html)|VS 2015|
|&nbsp;&nbsp;[N3470 constexpr For \<array>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2012/n3470.html)|VS 2015|
|&nbsp;&nbsp;[N3471 constexpr For \<initializer_list>, \<tuple>, \<utility>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2012/n3471.html)|VS 2015|
|&nbsp;&nbsp;[N3545 integral_constant::operator()()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3545.pdf)|VS 2015|
|&nbsp;&nbsp;[N3642 UDLs For \<chrono>, \<string> (1729ms, "meow"s, etc.)](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3642.pdf)|VS 2015|
|&nbsp;&nbsp;[N3644 Null Forward Iterators](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3644.pdf)|VS 2015|
|&nbsp;&nbsp;[N3654 quoted()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3654.html)|VS 2015|
|&nbsp;&nbsp;[N3657 Heterogeneous Associative Lookup](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3657.htm)|VS 2015|
|&nbsp;&nbsp;[N3658 integer_sequence](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3658.html)|VS 2015|
|&nbsp;&nbsp;[N3659 shared_mutex (Timed)](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3659.html)|VS 2015|
|&nbsp;&nbsp;[N3668 exchange()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3668.html)|VS 2015|
|&nbsp;&nbsp;[N3669 Fixing constexpr Member Functions Without const](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3669.pdf)|VS 2015|
|&nbsp;&nbsp;[N3670 get\<T>()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3670.html)|VS 2015|
|&nbsp;&nbsp;[N3671 Dual-Range equal(), is_permutation(), mismatch()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3671.html)|VS 2015|
|&nbsp;&nbsp;[N3778 Sized Deallocation](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3778.html)|VS 2015|
|&nbsp;&nbsp;[N3779 UDLs For \<complex> (3.14i, etc.)](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3779.pdf)|VS 2015|
|&nbsp;&nbsp;[N3789 constexpr For \<functional>](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3789.htm)|VS 2015|
|&nbsp;&nbsp;[N3887 tuple_element_t](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n3887.pdf)|VS 2015|
|&nbsp;&nbsp;[N3891 Renaming shared_mutex (Timed) To shared_timed_mutex](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2014/n3891.htm)|VS 2015|
|&nbsp;&nbsp;[N3346 Minimal Container Element Requirements](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2012/n3346.pdf)|VS 2013|
|&nbsp;&nbsp;[N3421 Transparent Operator Functors (less\<>, etc.)](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2012/n3421.htm)|VS 2013|
|&nbsp;&nbsp;[N3655 Alias Templates For \<type_traits> (decay_t, etc.)](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3655.pdf)|VS 2013|
|&nbsp;&nbsp;[N3656 make_unique()](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2013/n3656.htm)|VS 2013|

A group of papers listed together indicates that a feature was voted into the Standard, and then one or more papers to improve or expand that feature were also voted in. These features are implemented together.

### Supported values

__No__ means not yet implemented.<br/>
__Partial__ means the implementation is incomplete. For more details, see the Notes section.<br/>
__VS 2010__ indicates features that are supported in Visual Studio 2010.<br/>
__VS 2013__ indicates features that are supported in Visual Studio 2013.<br/>
__VS 2015__ indicates features that are supported in Visual Studio 2015 RTW.<br/>
__VS 2015.2__ and __VS 2015.3__ indicate features that are supported in Visual Studio 2015 Update 2 and Visual Studio 2015 Update 3, respectively.<br/>
__VS 2017 15.0__ indicates features that are supported in Visual Studio 2017 version 15.0 (RTW).<br/>
__VS 2017 15.3__ indicates features that are supported in Visual Studio 2017 version 15.3.<br/>
__VS 2017 15.5__ indicates features that are supported in Visual Studio 2017 version 15.5.<br/>
__VS 2017 15.7__ indicates features that are supported in Visual Studio 2017 version 15.7.<br/>
__VS 2019 16.0__ indicates features that are supported in Visual Studio 2019 version 16.0 (RTW).<br/>
__VS 2019 16.1__ indicates features that are supported in Visual Studio 2019 version 16.1.

### Notes

<a name="note_A"></a>__A__ In [/std:c++14](../build/reference/std-specify-language-standard-version.md) mode, dynamic exception specifications remain unimplemented, and `throw()` is still treated as a synonym for `__declspec(nothrow)`. In C++17, dynamic exception specifications were mostly removed by P0003R5, leaving one vestige: `throw()` is deprecated and required to behave as a synonym for `noexcept`. In [/std:c++17](../build/reference/std-specify-language-standard-version.md) mode, MSVC now conforms to the Standard by giving `throw()` the same behavior as `noexcept`, i.e. enforcement via termination.

The compiler option [/Zc:noexceptTypes](../build/reference/zc-noexcepttypes.md) requests our old behavior of `__declspec(nothrow)`. It’s likely that `throw()` will be removed in C++20. To help with migrating code in response to these changes in the Standard and our implementation, new compiler warnings for exception specification issues have been added under [/std:c++17](../build/reference/std-specify-language-standard-version.md) and [/permissive-](../build/reference/permissive-standards-conformance.md).

<a name="note_B"></a>__B__ Supported in [/permissive-](../build/reference/permissive-standards-conformance.md) mode in Visual Studio 2017 version 15.7. see [Two-phase name lookup support comes to MSVC](https://blogs.msdn.microsoft.com/vcblog/2017/09/11/two-phase-name-lookup-support-comes-to-msvc/) for more information.

<a name="note_C"></a>__C__ The compiler’s support for C99 Preprocessor rules is incomplete in Visual Studio 2017. Variadic macros are supported, but there are many bugs in the preprocessor’s behavior. We are overhauling the preprocessor, and will experimentally ship those changes under the [/permissive-](../build/reference/permissive-standards-conformance.md) mode soon.

<a name="note_D"></a>__D__ Supported under [/std:c++14](../build/reference/std-specify-language-standard-version.md) with a suppressible warning, C4984.

<a name="note_E"></a>__E__ This is a completely new implementation, incompatible with the
previous `std::experimental` version, necessitated by symlink support, bug fixes, and changes in standard-required behavior. Currently, including \<filesystem> provides the new `std::filesystem` and the previous `std::experimental::filesystem`, and including \<experimental/filesystem> provides only the old experimental implementation. The experimental implementation will be REMOVED in the next ABI-breaking release of the libraries.

<a name="note_G"></a>__G__ Supported by a compiler intrinsic.

<a name="note_14"></a>__14__ These C++17/20 features are always enabled, even when [/std:c++14](../build/reference/std-specify-language-standard-version.md) (the default) is specified. This is either because the feature was implemented before the introduction of the **/std** options, or because conditional implementation was undesirably complex.

<a name="note_17"></a>__17__ These features are enabled by the [/std:c++17](../build/reference/std-specify-language-standard-version.md) (or [/std:c++latest](../build/reference/std-specify-language-standard-version.md)) compiler option.

<a name="note_20"></a>__20__ These features are enabled by the [/std:c++latest](../build/reference/std-specify-language-standard-version.md) compiler option. When the C++20 implementation is complete, a new **/std:c++20** compiler option will be added, under which these features will also be available.

<a name="note_byte"></a>__byte__ `std::byte` is enabled by [/std:c++17](../build/reference/std-specify-language-standard-version.md) (or [/std:c++latest](../build/reference/std-specify-language-standard-version.md)), but because it can conflict with the Windows SDK headers in some cases, it has a fine-grained opt-out macro. It can be disabled by defining `_HAS_STD_BYTE` as `0`.

<a name="note_C11"></a>__C11__ The Universal CRT implemented the parts of the C11 Standard Library that are required by C++17, with the exception of C99 `strftime()` E/O alternative conversion specifiers, C11 `fopen()` exclusive mode, and C11 `aligned_alloc()`. The latter is unlikely to be implemented, because C11 specified `aligned_alloc()` in a way that's incompatible with the Microsoft implementation of `free()`, namely, that `free()` must be able to handle highly aligned allocations.

<a name="note_rem"></a>__rem__ Features removed when the [/std:c++17](../build/reference/std-specify-language-standard-version.md) (or [/std:c++latest](../build/reference/std-specify-language-standard-version.md)) compiler option is specified. These features can be re-enabled to ease the transition to newer language modes by use of these macros: `_HAS_AUTO_PTR_ETC`, `_HAS_FUNCTION_ALLOCATOR_SUPPORT`, `_HAS_OLD_IOSTREAMS_MEMBERS`, and `_HAS_UNEXPECTED`.

<a name="note_charconv"></a>__charconv__ `from_chars()` and `to_chars()` are available for integers. The timeline for floating-point `from_chars()` and floating-point `to_chars()` is as follows:
- VS 2017 15.7: Integer `from_chars()` and `to_chars()`.
- VS 2017 15.8: Floating-point `from_chars()`.
- VS 2017 15.9: Floating-point `to_chars()` overloads for shortest decimal.
- VS 2019 16.0: Floating-point `to_chars()` overloads for shortest hex and precision hex.
- VS 2019 16.2: Floating-point `to_chars()` overloads for precision fixed and precision scientific.
- Not yet implemented: The floating-point `to_chars()` overload for precision general. 

<a name ="note_parallel"></a> __parallel__ C++17’s parallel algorithms library is complete. This doesn’t mean every algorithm is parallelized in every case; the most important algorithms have been parallelized and execution policy signatures are provided even where algorithms are not parallelized. Our implementation’s central internal header, yvals_core.h, contains the following "Parallel Algorithms Notes": C++ allows an implementation to implement parallel algorithms as calls to the serial algorithms.  This implementation parallelizes several common algorithm calls, but not all.

The following algorithms are parallelized:

- `adjacent_difference`, `adjacent_find`, `all_of`, `any_of`, `count`, `count_if`, `equal`, `exclusive_scan`, `find`, `find_end`, `find_first_of`, `find_if`, `find_if_not`, `for_each`, `for_each_n`, `inclusive_scan`, `is_heap`, `is_heap_until`, `is_partitioned`, `is_sorted`, `is_sorted_until`, `mismatch`, `none_of`, `partition`, `reduce`, `remove`, `remove_if`, `replace`, `replace_if`, `search`, `search_n`, `set_difference`, `set_intersection`, `sort`, `stable_sort`, `transform`, `transform_exclusive_scan`, `transform_inclusive_scan`, `transform_reduce`

The following are not presently parallelized:

- No apparent parallelism performance improvement on target hardware; all algorithms which merely copy or permute elements with no branches are typically memory bandwidth limited:
  - `copy`, `copy_n`, `fill`, `fill_n`, `move`, `reverse`, `reverse_copy`, `rotate`, `rotate_copy`, `shift_left`, `shift_right`, `swap_ranges`
- Confusion over user parallelism requirements exists; likely in the above category anyway:
  - `generate`, `generate_n`
- Effective parallelism suspected to be infeasible:
  - `partial_sort`, `partial_sort_copy`
- Not yet evaluated; parallelism may be implemented in a future release and is suspected to be beneficial:
  - `copy_if`, `includes`, `inplace_merge`, `lexicographical_compare`, `max_element`, `merge`, `min_element`, `minmax_element`, `nth_element`, `partition_copy`, `remove_copy`, `remove_copy_if`, `replace_copy`, `replace_copy_if`, `set_symmetric_difference`, `set_union`, `stable_partition`, `unique`, `unique_copy`

## See also

[C++ Language Reference](../cpp/cpp-language-reference.md)<br/>
[C++ Standard Library](../standard-library/cpp-standard-library-reference.md)<br/>
[C++ conformance improvements in Visual Studio](cpp-conformance-improvements.md)<br/>
[What's New for Visual C++ in Visual Studio](what-s-new-for-visual-cpp-in-visual-studio.md)<br/>
[Visual C++ change history 2003 through 2015](../porting/visual-cpp-change-history-2003-2015.md)<br/>
[Visual C++ What's New 2003 through 2015](../porting/visual-cpp-what-s-new-2003-through-2015.md)<br/>
[C++ team blog](https://devblogs.microsoft.com/cppblog/)

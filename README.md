# _Your project title_

- _Saif Niaz_
- _md.niaz@uoit.net_

## About the language

> _Describe the language_
>
*Defination*

Swift is a general-purpose programming language that is specifically developed for macOS, iOS, tvOS, Linux and watchOS. The language was originally created by Apple Incorporation, with the goal of working with Cocoa Touch and their frameworks as well as a set of Objective C-Codes that have been written for the products of Apple Incorporation.

*History*
> - Some interesting features

## About the syntax

*Basic operation*

```swift
var age = 23
let constant_m = "Mr. "
var fname = "Saif"
var message = "Hello " + constant_m + fname + ", your number is " + String(age)
print(message)
print(message.count)
```
*if statement*

```swift
var grade = 75.50

if grade >= 50 && grade < 60 {
    print("Your grade is D")
}else if grade >= 60 && grade < 70{
    print("Your grade is C")
}else if grade >= 70 && grade < 80{
    print("Your grade is B")
}else if grade >= 80{
    print("Your grade is A")
}else{
    print("Sorry, your grade is F")
}
```
*For Loop*

```swift
for _ in 1...5{
    print("Hello!")
}
```

## About the tools

Along with translating Swift source code to executable machine codes, Swift complier also supports number of other tools. Some of these tools include IDE integration with syntax coloring, code completion and other conveniences. Major components of Swift compiler are:

- Parsing: Parsing is a recursive-descent parser with hand-coded lexer implemented. Its main responsibility is to generate an Abstract Syntax Tree (AST) without any semantic or type information, and creates warning for grammatical problems within the input source.

-	Semantic Analysis:  Semantic Analysis is responsible for taking the parsed AST and changing it into a fully-type-checked AST that emits warning for semantic errors in the source code. Semantic analysis specifies if it is safe to generate code upon successful type-checked AST.

-	Clang Importer: Clang importer imports Clang module and maps the APIs from C or Objective-C into corresponding Swift APIs. 

-	SIL generation: SIL stands for Swift Intermediate Language, which is suitable for further analysis and optimization on Swift code. In this phase the type-checked AST are lowered into raw SIL.

-	SIL guaranteed transformations: SIL guaranteed transformations perform further diagnostics on programs, which affects the accuracy of the programs. The result of these transformations is known as “canonical” SIL.

-	SIL Optimizations: The SIL optimizations perform specific optimizations on the program, such as Automatic Reference Counting, devirtualization and generic specialization.

-	LLVM IR Generation: IR generation takes the optimized SIL and lowers it to LLVM IR. At this point LLVM continues to optimize the program and generate machine codes.

## About the standard library

Implementation of the standard library are found in Swift repository, under the subdirectory of stdlib/public. Standard library includes a number of data types, protocols, collections that describes protocols, algorithm that operates on protocols and low-level primitives. The Swift standard library are subdivided into more components, such as:

-	Standard library core: The core library includes all types of data, protocols, functions and many more. For example: Int and Double for data types.

-	Runtime: Runtime is a layer between compiler and core standard library, which is responsible for implementing dynamic features of the language. Some of these features include casting, type metadata and memory management. Runtime is usually written in C++ or Objective-C.

-	SDK Overlays: SDK Overlay provide Swift based modification to existing Objective-C frameworks, which improves mapping the framework into Swift. Basically, overlay provides further support for interoperability with Objective-C code.


## About open source library

> *Foundation*

Foundation framework is a base layer of functionality that provides primitive classes and several paradigms, which are not supported by the language or runtime. It is designed to provide small basic utility classes. Introduces consistent conventions that enhances the process of software development. It supports internationalization and localization and provides a OS independences.

```swift
import Foundation

// Make an URLComponents instance
let swifty = URLComponents(string: "https://swift.org")!

// Print something useful about the URL
print("\(swifty.host!)")

// Output: "swift.org"
```


# Analysis of the language

> _Organize your report according to the project description
document_.

> *Advantages of using Swift*
- Rapid development process
- Provide better scalability of the product and the team
- Improved safety and performance
- Decreased memory footprint by using dynamic libraries
- Interoperability with Objective-C
- Automatic memory management which provide garbage collector functionality
- Has the ability to perform backend as well as front end
- Open Source 

> *Advantages of using Swift*
- The language is still quite young, so the programming language is still being tested
- Swift is often considered unstable
- There are limited Swift developer available
- Poor interoperability with third-party tools and IDEs
- Lack of support for earlier iOS versions

# _Your project title_

- _Saif Niaz_
- _md.niaz@uoit.net_

## About the language

> _Describe the language_
>
> - History
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

> _Give some examples of the functions and data structures
> offered by the standard library_.

## About open source library

> _Describe at least one contribution by the open source
community written in the language._

# Analysis of the language

> _Organize your report according to the project description
document_.



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

> Along with translating Swift source code to executable machine codes, Swift complier also supports number of other tools. Some of these tools include IDE integration with syntax coloring, code completion and other conveniences. Major components of Swift compiler are:

>   -   Parsing: Parsing is a recursive-descent parser with hand-coded lexer implemented. Its main responsibility is to generate an Abstract Syntax Tree (AST) without any semantic or type information, and creates warning for grammatical problems within the input source.

## About the standard library

> _Give some examples of the functions and data structures
> offered by the standard library_.

## About open source library

> _Describe at least one contribution by the open source
community written in the language._

# Analysis of the language

> _Organize your report according to the project description
document_.



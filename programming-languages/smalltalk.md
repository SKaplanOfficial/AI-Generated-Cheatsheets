# Smalltalk Cheatsheet

## Unique Features
- Object-oriented programming language
- Everything is an object, including classes and methods
- Dynamic language with a simple syntax
- Interactive development environment (IDE)

## Variables
- Local variable: `| variable |`
- Instance variable: `myVariable`
- Class variable: `MyClass classVariable`

## Functions
- Method definition: `myMethod
  "comment"
  | variable |
  variable := value.
  ^ variable`
- Method call: `self myMethod`

## Loops
- While loop: `whileTrue: [expression]`
- For loop: `1 to: 10 do: [:i | expression]`
- Each iterator: `myCollection do: [:each | expression]`

## Conditionals
- If statement: `condition ifTrue: [expression]`
- If-else statement: `condition ifTrue: [expression] ifFalse: [expression]`

## Collections
- Array: `#(item1 item2 item3)`
- Dictionary: `#{key1 -> value1. key2 -> value2}`

## Classes
- Class definition: `MyClass subclass: [superclass]`
- Class method definition: `MyClass class >> myMethod`
- Class method call: `MyClass myMethod`

## Blocks
- Block definition: `[:variable | expression]`
- Block call: `[expression] value`

## Exception Handling
- Try-catch statement: `[expression] on: Exception do: [:exception | expression]`

## Resources
- [Smalltalk Documentation](https://www.gnu.org/software/smalltalk/manual/html_node/)
- [Pharo Documentation](https://pharo.org/documentation)
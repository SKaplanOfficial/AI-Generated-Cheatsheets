# REBOL Cheatsheet

## Overview

REBOL is a high-level programming language that is designed to be easy to learn and use. It has a number of unique features that make it a powerful tool for developing applications.

## Variables

Variables in REBOL are created using the `set` function. Here's an example:

```
set my-variable 10
```

## Functions

Functions in REBOL are defined using the `function` keyword. Here's an example:

```
function [a b] [
    return a + b
]
```

## Loops

REBOL has several types of loops, including `for`, `while`, and `until`. Here's an example of a `for` loop:

```
for i 1 10 1 [
    print i
]
```

### Conditionals

REBOL has several types of conditionals, including `if`, `either`, and `case`. Here's an example of an `if` statement:

```
if x > 10 [
    print "x is greater than 10"
]
```

## File Manipulation

REBOL has built-in support for file manipulation. Here's an example of how to read a file:

```
file: read %myfile.txt
print file
```

## Resources

Here are some resources for learning more about REBOL:

- [The REBOL Programming Language](https://www.rebol.com/)
- [REBOL Tutorial](https://www.tutorialspoint.com/rebol/index.htm)
- [REBOL Cookbook](https://github.com/rebol/rebol3/wiki/Cookbook)
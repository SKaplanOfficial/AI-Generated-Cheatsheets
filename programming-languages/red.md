## Red Cheatsheet

### Overview

Red is a programming language and environment that is designed to be simple, flexible, and efficient. It is influenced by Rebol, a language created by Carl Sassenrath in the 1990s. Red is known for its concise syntax, powerful data manipulation features, and cross-platform support.

### Variables

Red variables can store a variety of data types, including integer, decimal, string, binary, and block. Variables are assigned using the `:` operator.

```red
; Integer variable
x: 42

; Decimal variable
pi: 3.14

; String variable
name: "Alice"

; Binary variable
flags: #{01010101}

; Block variable
numbers: [1 2 3 4 5]
```

### Functions

Red has a small number of built-in functions for common tasks such as string manipulation, file I/O, and GUI programming. Functions are called using a word followed by arguments in parentheses.

```red
; String manipulation
name: "Alice"
length? name  ; Returns 5

; File I/O
read %input.txt

; GUI programming
view [
    button "Click me" [print "Hello, world!"]
]
```

### Loops

Red has several types of loops, including `for`, `foreach`, `while`, and `until`. The `for` and `foreach` loops are used to iterate over a range of values or a block, while the `while` and `until` loops are used to repeat a block of code while a condition is true or false.

```red
; For loop
for i 1 10 1 [
    print i
]

; Foreach loop
numbers: [1 2 3 4 5]
foreach num numbers [
    print num
]

; While loop
i: 1
while i <= 10 [
    print i
    i: i + 1
]

; Until loop
i: 1
until i > 10 [
    print i
    i: i + 1
]
```

### Conditionals

Red has several conditional statements, including `if`, `either`, and `switch`. These statements are used to control the flow of a program based on certain conditions.

```red
; If statement
age: 30
if age >= 18 [
    print "You are an adult"
]

; Either statement
age: 15
either age >= 18 [
    print "You are an adult"
][
    print "You are a minor"
]

; Switch statement
fruit: "apple"
switch fruit [
    "apple" [print "It's an apple"]
    "banana" [print "It's a banana"]
    [print "It's something else"]
]
```

### File Manipulation

Red provides several functions for manipulating files, including `read`, `write`, `rename`, and `delete`.

```red
; Read file
data: read %data.txt

; Write file
write %data_new.txt data

; Rename file
rename %data.txt %data_old.txt

; Delete file
delete %data_old.txt
```

### Resources

- [Red documentation](https://doc.red-lang.org/)
- [Red language on GitHub](https://github.com/red/red) (source code)
- [Red Discord server](https://discord.gg/2vHJ5C6) (community forum)
- [Red by Example](https://tutorials.red/) (online tutorial)
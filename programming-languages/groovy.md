# Groovy Cheatsheet

Groovy is a dynamic programming language that is built on top of the Java Virtual Machine (JVM). It is designed to be concise and expressive, making it a popular choice for scripting, automation, and web development.

## Unique Features

- Dynamic typing
- Closures
- Optional typing
- Operator overloading
- Native syntax for lists, maps, and regular expressions
- Integration with Java libraries

## Variables

Variables in Groovy are declared using the `def` keyword. Groovy supports dynamic typing, so you don't need to specify the type of the variable.

```groovy
def name = "John"
def age = 30
def pi = 3.14
```

## Functions

Functions in Groovy are declared using the `def` keyword followed by the function name and parameters. Groovy supports closures, which are anonymous functions that can be assigned to variables and passed as arguments to other functions.

```groovy
def greet(name) {
  println "Hello, $name!"
}

greet("John")

def add = { a, b ->
  a + b
}

println add(2, 3)
```

## Loops

Groovy supports `for` and `while` loops, as well as the enhanced `for` loop, which can iterate over collections.

```groovy
def numbers = [1, 2, 3, 4, 5]

for (number in numbers) {
  println number
}

def i = 0
while (i < 5) {
  println i
  i++
}
```

## Conditionals

Groovy supports `if`, `else if`, and `else` statements, as well as the ternary operator.

```groovy
def age = 30

if (age < 18) {
  println "You are too young to vote."
} else if (age < 21) {
  println "You can vote, but not drink."
} else {
  println "You can vote and drink."
}

def result = age >= 18 ? "You are an adult" : "You are not an adult"
```

## File Manipulation

Groovy provides several ways to read and write files. You can use the `File` class to create, read, write, and delete files.

```groovy
def file = new File("example.txt")

// Write to file
file.write("Hello, world!")

// Read from file
def content = file.text
println content

// Delete file
file.delete()
```

## Resources

- [Groovy Documentation](https://groovy-lang.org/documentation.html)
- [Groovy Style Guide](https://github.com/apache/groovy/blob/master/styleguide.md)
- [Groovy Goodness](https://mrhaki.blogspot.com/search/label/Groovy%20Goodness) blog series by Hubert Klein Ikkink
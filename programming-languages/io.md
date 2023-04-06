# Io Cheatsheet

Io is a small, prototype-based programming language inspired by Smalltalk, Lisp, and Lua. It is designed to be simple, reflective, and highly extensible, making it a popular choice for domain-specific languages, scripting, and rapid prototyping.

## Unique Features

- Prototype-based object model
- Dynamic message passing
- Minimal syntax
- Concurrency primitives
- Coroutines
- Metaprogramming capabilities

## Variables

Variables in Io are declared using the `:=` operator. Io supports dynamic typing, so you don't need to specify the type of the variable.

```io
name := "John"
age := 30
pi := 3.14
```

## Functions

Functions in Io are objects that can be assigned to variables, passed as arguments to other functions, and returned as values. Io supports dynamic message passing, which means that functions can be called on any object, not just classes.

```io
greet := method(name,
  "Hello, #{name}!" print
)

greet("John")

add := method(a, b,
  a + b
)

add(2, 3) println
```

## Loops

Io supports `while` and `foreach` loops, as well as the `loop` control structure, which can be used to create infinite loops.

```io
numbers := list(1, 2, 3, 4, 5)

foreach(number, numbers,
  number println
)

i := 0
while(i < 5,
  i println
  i = i + 1
)

loop(
  "This is an infinite loop" println
)
```

## Conditionals

Io supports `if`, `else if`, and `else` statements, as well as the ternary operator.

```io
age := 30

if(age < 18, "You are too young to vote" println,
  if(age < 21, "You can vote, but not drink" println,
    "You can vote and drink" println
  )
)

result := age >= 18 ? "You are an adult" : "You are not an adult"
result println
```

## File Manipulation

Io provides several ways to read and write files. You can use the `File` object to create, read, write, and delete files.

```io
file := File with("example.txt")

// Write to file
file write("Hello, world!")

// Read from file
content := file readAll
content println

// Delete file
file delete
```

## Resources

- [Io Language Guide](http://iolanguage.org/scm/io/docs/IoGuide.html)
- [Io Reference](http://iolanguage.org/scm/io/docs/reference.html)
- [Io Playground](http://iolanguage.org/playground/)
- [Io Cookbook](https://en.wikibooks.org/wiki/Io_Programming/Cookbook)
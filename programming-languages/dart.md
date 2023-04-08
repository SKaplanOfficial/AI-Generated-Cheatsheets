# Dart Cheatsheet

This cheatsheet provides a brief overview of Dart's unique features and syntax, including code blocks for variables, functions, loops, conditionals, file manipulation, and more.

Dart is a client-optimized programming language developed by Google. It is used to build web, mobile, and desktop applications. Dart is known for its fast runtime, productivity, and scalability.

This cheatsheet is designed to serve as a quick reference guide for Dart developers of all levels. It includes examples of common syntax and programming constructs, as well as a list of resources for further learning.

## Unique Features
- Client-optimized programming language
- Developed by Google
- Used to build web, mobile, and desktop applications
- Fast runtime
- Productivity and scalability

## Variables
```dart
// declaring a variable
var variable_name = value;

// dynamic typing
dynamic variable_name = "string";
dynamic variable_name = 123;
```

## Functions
```dart
// defining a function
return_type function_name(parameter1, parameter2) {
  // function body
  return value;
}

// calling a function
function_name(argument1, argument2);
```

## Loops
```dart
// for loop
for (var i = 0; i < length; i++) {
  // loop body
}

// while loop
while (condition) {
  // loop body
}

// do-while loop
do {
  // loop body
} while (condition);
```

## Conditionals
```dart
// if statement
if (condition) {
  // if body
} else if (condition) {
  // else if body
} else {
  // else body
}

// ternary operator
condition ? true_body : false_body
```

## File Manipulation
```dart
// reading from a file
import 'dart:io';

File('filename').readAsString().then((String contents) {
  // process contents
});

// writing to a file
import 'dart:io';

File('filename').writeAsString('content').then((File file) {
  // process file
});
```

## Resources
- [Official Dart Website](https://dart.dev/)
- [Dart Documentation](https://dart.dev/guides)
- [Dart Style Guide](https://dart.dev/guides/language/effective-dart/style)
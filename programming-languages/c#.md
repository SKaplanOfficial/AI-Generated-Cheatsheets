# C# Cheatsheet

## Overview of unique features

- Object-oriented programming language
- Strongly-typed language
- Supports garbage collection
- Wide range of libraries and frameworks
- Can be used for web development, desktop applications, and game development

## Variables

```C#
// Declare a variable
int x = 42;

// Declare a constant
const int y = 10;

// Declare an array
int[] myArray = {1, 2, 3};

// Declare a string
string myString = "hello";
```

## Functions

```C#
// Declare a function
int add(int x, int y) {
  return x + y;
}

// Call a function
int result = add(3, 4);
```

## Loops

```C#
// Define a for loop
for (int i = 0; i < 10; i++) {
  // do something
}

// Define a while loop
while (condition) {
  // do something
}
```

## Conditionals

```C#
// Define an if-else statement
int max(int x, int y) {
  if (x > y) {
    return x;
  } else {
    return y;
  }
}
```

## Object-oriented programming

```C#
// Define a class
class MyClass {
  public int MyField;
  public void MyMethod() {
    // do something
  }
}

// Create an instance of a class
MyClass myInstance = new MyClass();
myInstance.MyField = 42;
myInstance.MyMethod();
```

## Resources

- [C# documentation](https://docs.microsoft.com/en-us/dotnet/csharp/)
- [C# tutorial](https://www.tutorialspoint.com/csharp/index.htm)
- [C# forum](https://stackoverflow.com/questions/tagged/c%23) for community support and troubleshooting.
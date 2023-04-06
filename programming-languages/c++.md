# C++ Cheatsheet

## Overview of unique features

- Object-oriented programming language
- Strongly-typed language
- Supports templates and generics
- Wide range of libraries and frameworks
- Can be used for system programming and game development

## Variables

```C++
// Declare a variable
int x = 42;

// Declare a constant
const int y = 10;

// Declare an array
int myArray[3] = {1, 2, 3};

// Declare a string
std::string myString = "hello";
```

## Functions

```C++
// Declare a function
int add(int x, int y) {
  return x + y;
}

// Call a function
int result = add(3, 4);
```

## Loops

```C++
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

```C++
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

```C++
// Define a class
class MyClass {
public:
  int myField;
  void myMethod() {
    // do something
  }
};

// Create an instance of a class
MyClass myInstance;
myInstance.myField = 42;
myInstance.myMethod();
```

## Resources

- [C++ documentation](https://devdocs.io/cpp/)
- [C++ tutorial](https://www.tutorialspoint.com/cplusplus/index.htm)
- [C++ forum](https://stackoverflow.com/questions/tagged/c%2B%2B) for community support and troubleshooting.
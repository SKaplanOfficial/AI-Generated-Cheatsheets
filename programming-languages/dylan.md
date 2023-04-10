# Dylan Cheatsheet

## Unique Features
- Object-oriented language
- Strongly typed with optional type inference
- Supports multiple dispatch
- Garbage collection
- Mixins for code reuse
- Syntax inspired by Lisp and C

## Variables
```dylan
define variable_name = value;
```

## Functions
```dylan
define method_name(parameter1: type1, parameter2: type2): return_type => {
  // Function body
}

method_name(argument1, argument2);
```

## Loops
```dylan
// While loop
while condition do {
  // Loop body
}

// For loop
for variable_name in range do {
  // Loop body
}

// Each loop
each(item in collection) {
  // Loop body
}
```

## Conditionals
```dylan
// If statement
if condition then {
  // Code to execute if condition is true
}

// If-else statement
if condition then {
  // Code to execute if condition is true
} else {
  // Code to execute if condition is false
}

// Case statement
case variable_name in
  value1 => {
    // Code to execute if variable_name equals value1
  }
  value2 => {
    // Code to execute if variable_name equals value2
  }
  _ => {
    // Code to execute if variable_name does not equal any of the values
  }
end;
```

## File Manipulation
```dylan
// Reading from a file
let file_contents = file.read("file_name");

// Writing to a file
file.write("file_name", "text to write");
```

## Resources
- [Dylan Programming Language](https://www.opendylan.org/)
- [Dylan Reference Manual](https://opendylan.org/books/drm/)
- [Dylan Programming](https://dylan-foundry.org/) (community site)
- [Dylan Programming: An Object-Oriented and Dynamic Language](https://www.amazon.com/Dylan-Programming-Object-Oriented-Dynamic-Language/dp/0201596140) (book)
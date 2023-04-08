# ActionScript Cheatsheet

This cheatsheet provides a brief overview of ActionScript's unique features and syntax, including code blocks for variables, functions, loops, conditionals, file manipulation, and more.

ActionScript is an object-oriented programming language used primarily for the development of Adobe Flash content. It is known for its simplicity and ease of use, making it a popular choice for web developers.

This cheatsheet is designed to serve as a quick reference guide for ActionScript developers of all levels. It includes examples of common syntax and programming constructs, as well as a list of resources for further learning.

## Unique Features
- Object-oriented programming language
- Used primarily for the development of Adobe Flash content
- Simple and easy to use
- Popular choice for web developers

## Variables
```actionscript
// declaring a variable
var variable_name:data_type = value;

// dynamic typing
var variable_name:* = "string";
var variable_name:* = 123;
```

## Functions
```actionscript
// defining a function
function function_name(parameter1:data_type, parameter2:data_type):return_type {
  // function body
  return value;
}

// calling a function
function_name(argument1, argument2);
```

## Loops
```actionscript
// for loop
for (var i:int = 0; i < length; i++) {
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
```actionscript
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
```actionscript
// reading from a file
var file:File = new File("filename");
var stream:FileStream = new FileStream();
stream.open(file, FileMode.READ);
var contents:String = stream.readUTFBytes(stream.bytesAvailable);
stream.close();

// writing to a file
var file:File = new File("filename");
var stream:FileStream = new FileStream();
stream.open(file, FileMode.WRITE);
stream.writeUTFBytes("content");
stream.close();
```

## Resources

- [Official Adobe ActionScript Website](https://www.adobe.com/products/actionscript.html)
- [ActionScript Documentation](https://help.adobe.com/en_US/FlashPlatform/reference/actionscript/3/)
- [ActionScript Style Guide](https://github.com/brandonhall/actionscript-3-style-guide)
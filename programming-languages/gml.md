# Game Maker Language (GML) Cheatsheet

This cheatsheet provides a brief overview of Game Maker Language's unique features and syntax, including code blocks for variables, functions, loops, conditionals, file manipulation, and more.

Game Maker Language (GML) is a scripting language used in the development of games using the GameMaker Studio game engine. It is known for its simplicity and ease of use, making it a popular choice for game developers.

This cheatsheet is designed to serve as a quick reference guide for GML developers of all levels. It includes examples of common syntax and programming constructs, as well as a list of resources for further learning.

## Unique Features
- Scripting language used in GameMaker Studio game engine
- Simple and easy to use
- Popular choice for game developers

## Variables
```gml
// declaring a variable
variable_name = value;

// dynamic typing
variable_name = "string";
variable_name = 123;
```

## Functions
```gml
// defining a function
function_name(parameter1, parameter2) {
  // function body
  return value;
}

// calling a function
function_name(argument1, argument2);
```

## Loops
```gml
// for loop
for (var i = start; i < end; i++) {
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
```gml
// if statement
if (condition) {
  // if body
} else if (condition) {
  // else if body
} else {
  // else body
}

// ternary operator
variable_name = (condition) ? true_body : false_body;
```

## File Manipulation
```gml
// reading from a file
file = file_text_open_read("filename");
while (!file_text_eof(file)) {
  line = file_text_readln(file);
  // process line
}
file_text_close(file);

// writing to a file
file = file_text_open_write("filename");
file_text_writeln(file, "content");
file_text_close(file);
```

## Resources
- [Official GameMaker Studio Website](https://www.yoyogames.com/gamemaker)
- [GML Documentation](https://docs2.yoyogames.com/)
- [GML Style Guide](https://forum.yoyogames.com/index.php?threads/gml-style-guide.1276/)
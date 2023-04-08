# BASIC Cheatsheet

This cheatsheet provides a brief overview of BASIC's unique features and syntax, including code blocks for variables, functions, loops, conditionals, file manipulation, and more.

BASIC (Beginner's All-purpose Symbolic Instruction Code) is a high-level programming language designed for beginners to learn programming concepts. It is known for its simplicity and ease of use, making it a popular choice for educational institutions.

This cheatsheet is designed to serve as a quick reference guide for BASIC developers of all levels. It includes examples of common syntax and programming constructs, as well as a list of resources for further learning.

## Unique Features
- High-level programming language
- Designed for beginners to learn programming concepts
- Simple and easy to use
- Popular choice for educational institutions

## Variables
```basic
' declaring a variable
DIM variable_name AS data_type

' dynamic typing
variable_name = "string"
variable_name = 123
```

## Functions
```basic
' defining a function
FUNCTION function_name(parameter1 AS data_type, parameter2 AS data_type) AS return_type
  ' function body
  RETURN value
END FUNCTION

' calling a function
variable_name = function_name(argument1, argument2)
```

## Loops
```basic
' for loop
FOR i = start TO end STEP increment
  ' loop body
NEXT i

' while loop
WHILE condition
  ' loop body
WEND

' do-while loop
DO
  ' loop body
LOOP WHILE condition
```

## Conditionals
```basic
' if statement
IF condition THEN
  ' if body
ELSEIF condition THEN
  ' else if body
ELSE
  ' else body
END IF

' ternary operator
variable_name = IIF(condition, true_body, false_body)
```

## File Manipulation
```basic
' reading from a file
OPEN "filename" FOR INPUT AS #1
WHILE NOT EOF(1) 
  LINE INPUT #1, line
  ' process line
WEND
CLOSE #1

' writing to a file
OPEN "filename" FOR OUTPUT AS #1
PRINT #1, "content"
CLOSE #1
```

## Resources
- [Official BASIC Website](https://www.basic.net/)
- [BASIC Documentation](https://www.freebasic.net/)
- [BASIC Style Guide](https://www.freebasic.net/wiki/Recommended_Coding_Style)
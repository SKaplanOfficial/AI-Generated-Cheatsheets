# Forth Cheatsheet

## Overview of unique features

- Stack-based programming language
- Uses Reverse Polish Notation (RPN)
- Supports low-level programming and embedded systems
- Can be used for boot loaders and firmware development

## Stack operations

```forth
1 2 3 .s      \ prints the stack: 1 2 3
4 swap .s     \ prints the stack: 4 2 3
drop .s       \ prints the stack: 4 2
```

## Arithmetic operations

```forth
1 2 + .       \ prints 3
3 2 - .       \ prints 1
2 3 * .       \ prints 6
6 3 / .       \ prints 2
```

## Conditionals

```forth
1 2 > IF
  ." 1 is greater than 2" CR
ELSE
  ." 2 is greater than 1" CR
THEN
```

## Loops

```forth
10 0 DO
  I .
LOOP
```

## Defining words

```forth
: MY-WORD ." Hello, world!" ;
MY-WORD      \ prints "Hello, world!"
```

## Resources

- [Forth documentation](https://www.forth.com/starting-forth/)
- [Forth tutorial](https://skilldrick.github.io/easyforth/)
- [Forth forum](https://www.forth.com/starting-forth/2-3-forth-forum/) for community support and troubleshooting.
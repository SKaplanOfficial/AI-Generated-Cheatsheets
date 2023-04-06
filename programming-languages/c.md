## C Cheatsheet

C is a general-purpose programming language that has been used for developing operating systems, embedded systems, and other applications. Here's a quick overview of its unique features and some code blocks for common tasks.

### Variables

Declare variables using the data type followed by the variable name. C is a statically typed language, so the data type of a variable cannot be changed after it is declared.

```c
int x = 10;
char c = 'a';
float f = 3.14;
```

### Functions

Functions in C are declared using the `function` keyword. They can take parameters and return values.

```c
int add(int a, int b) {
  return a + b;
}
```

### Loops

C supports `for`, `while`, and `do-while` loops for iterating over arrays or performing a task a certain number of times.

```c
int numbers[] = {1, 2, 3, 4, 5};

for (int i = 0; i < 5; i++) {
  printf("%d\n", numbers[i]);
}

int i = 0;
while (i < 5) {
  printf("%d\n", numbers[i]);
  i++;
}

i = 0;
do {
  printf("%d\n", numbers[i]);
  i++;
} while (i < 5);
```

### Conditionals

Use `if` statements to execute code based on a condition. `else if` and `else` statements can be used to handle multiple conditions.

```c
int x = 10;

if (x > 0) {
  printf("x is positive");
} else if (x < 0) {
  printf("x is negative");
} else {
  printf("x is zero");
}
```

### File Manipulation

C provides built-in support for file manipulation, including reading and writing files, and interacting with the file system.

```c
#include <stdio.h>

int main() {
  FILE *fp;
  char buffer[255];

  fp = fopen("/path/to/file.txt", "r");
  fgets(buffer, 255, fp);
  printf("%s", buffer);
  fclose(fp);

  fp = fopen("/path/to/file.txt", "w");
  fputs("New contents", fp);
  fclose(fp);

  if (remove("/path/to/file.txt") == 0) {
  printf("File deleted successfully");
  } else {
  printf("Error deleting file");
  }

  return 0;
}
```

### Resources

Here are some resources to help you learn more about C:

- [C Programming Wikibook](https://en.wikibooks.org/wiki/C_Programming)
- [C Programming Language](https://www.amazon.com/Programming-Language-2nd-Brian-Kernighan/dp/0131103628) (Book by Brian Kernighan and Dennis Ritchie)
- [Learn C.org](https://www.learn-c.org/) (Interactive C tutorial)
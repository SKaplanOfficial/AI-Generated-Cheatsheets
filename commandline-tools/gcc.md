# GCC Cheatsheet

## Overview
GCC (GNU Compiler Collection) is a collection of programming language compilers, including C, C++, Objective-C, Fortran, Ada, and others.

## Installation
- macOS: `xcode-select --install`
- Ubuntu/Debian: `sudo apt-get install build-essential`
- Windows: [MinGW-w64](http://mingw-w64.org/doku.php) or [Cygwin](https://www.cygwin.com/)

## Basic Usage
```bash
gcc file.c -o file
```
Compiles `file.c` and creates an executable named `file`.

## Flags
- `-c`: Compiles source files to object files without linking.
- `-o`: Specifies the name of the output file.
- `-Wall`: Enables all warning messages.
- `-Werror`: Treats all warnings as errors.
- `-g`: Adds debugging information to the executable.
- `-O`: Enables optimization of the code.
- `-std`: Specifies the language standard to use.
- `-I`: Adds a directory to the include path.
- `-L`: Adds a directory to the library path.
- `-l`: Links against a library.

## Examples
```bash
gcc -c file.c -o file.o          # Compile source file to object file
gcc file.o -o file         # Link object file to create executable
gcc -Wall -Werror -g file.c -o file     # Compile with warnings and debugging information
gcc -O2 file.c -o file        # Compile with optimization
gcc -std=c99 file.c -o file         # Compile with C99 standard
gcc -I include/ file.c -o file       # Add include directory to include path
gcc -L lib/ -l mylib file.c -o file      # Link against library "mylib"
```

## Resources
- [GCC website](https://gcc.gnu.org/)
- [GCC documentation](https://gcc.gnu.org/onlinedocs/)
- [GCC Wiki](https://gcc.gnu.org/wiki/)
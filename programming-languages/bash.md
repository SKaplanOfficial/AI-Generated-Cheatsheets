# Bash Cheatsheet

Bash is a Unix shell and command language used for automating tasks and interacting with the operating system. Here is an overview of its features, code blocks, and resources.

## Features

- Bash is a command language used for interacting with the Unix shell.
- It is a scripting language that can be used for automating tasks and system administration.
- Bash supports variables, loops, conditionals, functions, and file manipulation.
- Bash is highly customizable and can be extended with plugins and scripts.

## Code Blocks

### Variables

Variables are used to store data that can be used later in the script.

```bash
variableName=value
```

### Functions

Functions are code blocks that perform a specific task. They can be called by other parts of the script.

```bash
function functionName {
    # code to be executed
}
```

### Conditionals

Conditionals allow the script to make decisions based on certain conditions.

```bash
if [ condition ]; then
    # code to be executed if condition is true
elif [ otherCondition ]; then
    # code to be executed if otherCondition is true
else
    # code to be executed if neither condition is true
fi
```

### Loops

Loops allow the script to repeat a set of instructions.

```bash
for i in {1..10}; do
    # code to be executed
done
```

### File Manipulation

Bash can be used to manipulate files and folders on the file system.

```bash
# list all files in the current directory
ls

# create a new directory
mkdir directoryName

# remove a file
rm fileName
```

## Resources

Here are some resources for learning and using Bash:

- [Bash Reference Manual](https://www.gnu.org/software/bash/manual/bash.html)
- [Bash subreddit](https://www.reddit.com/r/bash/)
- [Bash Guide for Beginners](http://tldp.org/LDP/Bash-Beginners-Guide/html/)
- [Bash on Stack Overflow](https://stackoverflow.com/questions/tagged/bash)
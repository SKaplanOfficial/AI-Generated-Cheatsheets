# Python Cheatsheet

Python is a high-level programming language known for its simplicity, readability, and versatility. Here is an overview of its features, code blocks, and resources.

## Features

- Python is an interpreted language, which means that it does not need to be compiled before running.
- Python has a large standard library that provides many useful modules and functions for a wide range of tasks.
- Python is dynamically typed, which means that variables do not need to be declared before use.
- Python supports multiple programming paradigms, including procedural, object-oriented, and functional programming.
- Python is cross-platform and can run on many different operating systems.

## Code Blocks

### Variables

Variables are used to store data that can be used later in the script.

```python
variableName = value
```

### Functions

Functions are code blocks that perform a specific task. They can be called by other parts of the script.

```python
def functionName(parameter1, parameter2):
    # code to be executed
```

### Conditionals

Conditionals allow the script to make decisions based on certain conditions.

```python
if condition:
    # code to be executed if condition is true
elif otherCondition:
    # code to be executed if otherCondition is true
else:
    # code to be executed if neither condition is true
```

### Loops

Loops allow the script to repeat a set of instructions.

```python
for i in range(10):
    # code to be executed
```

### File Manipulation

Python can be used to manipulate files and folders on the file system.

```python
import os

for file in os.listdir("."):
    if file.endswith(".txt"):
   print(file)
```

### User Interface

Python can be used to create graphical user interfaces (GUIs) using libraries such as tkinter.

```python
import tkinter as tk

root = tk.Tk()
root.title("Hello, World!")
label = tk.Label(root, text="Hello, World!")
label.pack()
root.mainloop()
```

## Resources

Here are some resources for learning and using Python:

- [Python Documentation](https://docs.python.org/3/)
- [Python subreddit](https://www.reddit.com/r/Python/)
- [Real Python](https://realpython.com/)
- [Python on Stack Overflow](https://stackoverflow.com/questions/tagged/python)
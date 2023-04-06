# MATLAB Cheatsheet

MATLAB is a high-level programming language and interactive environment for numerical computation, visualization, and data analysis. It is widely used in engineering, science, and finance for tasks such as image processing, signal analysis, and machine learning.

## Unique Features

- Matrix operations
- Interactive visualization
- Built-in functions for signal processing and image analysis
- Simulink for modeling and simulation
- Toolboxes for specialized tasks
- Integration with C/C++ and Java code

## Variables

Variables in MATLAB are declared using the `=` or `:` operator. MATLAB supports dynamic typing, so you don't need to specify the type of the variable.

```matlab
name = 'John';
age = 30;
pi = 3.14;
```

## Functions

Functions in MATLAB are declared using the `function` keyword followed by the function name and parameters. MATLAB supports anonymous functions, which are functions that do not have a name and can be assigned to variables and passed as arguments to other functions.

```matlab
function greet(name)
  fprintf('Hello, %s!\n', name);
end

greet('John');

add = @(a, b) a + b;
disp(add(2, 3));
```

## Loops

MATLAB supports `for` and `while` loops, as well as the `if`, `else if`, and `else` statements.

```matlab
numbers = [1, 2, 3, 4, 5];

for number = numbers
  disp(number);
end

i = 0;
while i < 5
  disp(i);
  i = i + 1;
end
```

## Conditionals

MATLAB supports `if`, `else if`, and `else` statements, as well as the ternary operator.

```matlab
age = 30;

if age < 18
  disp('You are too young to vote.');
elseif age < 21
  disp('You can vote, but not drink.');
else
  disp('You can vote and drink.');
end

result = age >= 18 ? 'You are an adult' : 'You are not an adult';
disp(result);
```

## File Manipulation

MATLAB provides several ways to read and write files. You can use the `fopen`, `fprintf`, `fscanf`, and `fclose` functions to create, read, write, and delete files.

```matlab
file = fopen('example.txt', 'w');
fprintf(file, 'Hello, world!');
fclose(file);

file = fopen('example.txt', 'r');
content = fscanf(file, '%c');
disp(content);
fclose(file);

delete('example.txt');
```

## Resources

- [MATLAB Documentation](https://www.mathworks.com/help/matlab/)
- [MATLAB Style Guide](https://www.mathworks.com/matlabcentral/fileexchange/46056-matlab-style-guidelines-2-0)
- [MATLAB Onramp](https://www.mathworks.com/learn/tutorials/matlab-onramp.html)
- [MATLAB Central File Exchange](https://www.mathworks.com/matlabcentral/fileexchange/)
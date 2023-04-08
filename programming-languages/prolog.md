# Prolog Cheatsheet

This cheatsheet provides a brief overview of Prolog's unique features and syntax, including code blocks for variables, functions, loops, conditionals, file manipulation, and more.

Prolog is a logic programming language used in artificial intelligence, natural language processing, and expert systems. It is known for its ability to perform symbolic reasoning and pattern matching.

This cheatsheet is designed to serve as a quick reference guide for Prolog developers of all levels. It includes examples of common syntax and programming constructs, as well as a list of resources for further learning.

## Unique Features
- Logic programming language
- Used in artificial intelligence, natural language processing, and expert systems
- Ability to perform symbolic reasoning and pattern matching

## Variables
```prolog
% declaring a variable
variable_name = value.

% dynamic typing
variable_name = 'string'.
variable_name = 123.
```

## Functions
```prolog
% defining a function
function_name(parameter1, parameter2) :-
  % function body
  return value.

% calling a function
function_name(argument1, argument2).
```

## Loops
```prolog
% for loop
for(Variable, Start, End) :-
  Start =< End,
  % loop body
  Next is Start + 1,
  for(Variable, Next, End).
for(_, _, _).

% while loop
while(Condition, Body) :-
  Condition,
  Body,
  while(Condition, Body).
while(_, _).
```

## Conditionals
```prolog
% if statement
if(Condition, TrueBody, _) :-
  Condition,
  TrueBody.
if(_, _, FalseBody) :-
  FalseBody.

% ternary operator
Condition -> TrueBody ; FalseBody.
```

## File Manipulation
```prolog
% reading from a file
open('filename', read, Stream),
read_file(Stream, Lines),
close(Stream).

read_file(Stream, [Line|Lines]) :-
  read_line_to_string(Stream, Line),
  Line \= end_of_file,
  read_file(Stream, Lines).
read_file(_, []).

% writing to a file
open('filename', write, Stream),
write(Stream, 'content'),
close(Stream).
```

## Resources
- [Official Prolog Website](http://www.swi-prolog.org/)
- [Prolog Documentation](http://www.swi-prolog.org/pldoc/index.html)
- [Prolog Style Guide](https://www.metalevel.at/prolog/styleguide/)
# Ada Cheatsheet

This cheatsheet provides a brief overview of Ada's unique features and syntax, including code blocks for variables, functions, loops, conditionals, file manipulation, and more.

Ada is a high-level, strongly typed programming language that is used in safety-critical systems, such as aerospace and defense. It is known for its strong typing, modularity, and support for concurrency.

This cheatsheet is designed to serve as a quick reference guide for Ada developers of all levels. It includes examples of common syntax and programming constructs, as well as a list of resources for further learning.

## Unique Features
- High-level, strongly typed programming language
- Used in safety-critical systems, such as aerospace and defense
- Strong typing, modularity, and support for concurrency

## Variables
```ada
-- declaring a variable
variable_name : data_type := value;

-- dynamic typing
variable_name : any := "string";
variable_name : any := 123;
```

## Functions
```ada
-- defining a function
function function_name(parameter1 : data_type; parameter2 : data_type) return return_type is
  -- function body
begin
  return value;
end function;

-- calling a function
variable_name := function_name(argument1, argument2);
```

## Loops
```ada
-- for loop
for variable_name in range loop
  -- loop body
end loop;

-- while loop
while condition loop
  -- loop body
end loop;

-- loop through an array
for i in array_name'range loop
  -- loop body
end loop;
```

## Conditionals
```ada
-- if statement
if condition then
  -- if body
elsif condition then
  -- else if body
else
  -- else body
end if;

-- ternary operator
variable_name := (condition) ? true_body : false_body;
```

## File Manipulation
```ada
-- reading from a file
file_name : file_type;
line : string;
begin
  file_name := file_type("filename");
  while not end_of_file(file_name) loop
    readline(file_name, line);
    -- process line
  end loop;
  close(file_name);
end;

-- writing to a file
file_name : file_type;
begin
  file_name := file_type("filename", mode => out_file);
  put(file_name, "content");
  close(file_name);
end;
```

## Resources
- [Official Ada Website](https://www.adaic.org/)
- [Ada Documentation](https://www.adaic.org/resources/add_content/docs/95rat/RM-TTL.html)
- [Ada Style Guide](https://en.wikibooks.org/wiki/Ada_Style_Guide)
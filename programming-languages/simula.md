# Simula Cheatsheet

Simula is a programming language that is particularly well-suited for simulations and modeling. Here is an overview of some of its unique features and basic syntax.

## Variables

### Declaration
```
integer i;
real x;
boolean flag;
```

### Assignment
```
i := 42;
x := 3.14;
flag := true;
```

## Functions

### Declaration
```
procedure helloWorld();
begin
    write("Hello, world!");
end;
```

### Call
```
helloWorld();
```

## Loops

### For loop
```
for i := 1 to 10 do
begin
    write(i);
end;
```

### While loop
```
while flag do
begin
    write("Looping...");
end;
```

## Conditionals

### If statement
```
if x > 0 then
begin
    write("Positive");
end;
```

### If-else statement
```
if x > 0 then
begin
    write("Positive");
end
else
begin
    write("Non-positive");
end;
```

## File manipulation

### Reading from a file
```
textFile file;
file.open("filename.txt", "in");
while not file.eof do
begin
    file.readln(line);
    write(line);
end;
file.close();
```

### Writing to a file
```
textFile file;
file.open("filename.txt", "out");
file.writeln("Hello, world!");
file.close();
```

## Resources

- [Simula Programming Language](https://en.wikipedia.org/wiki/Simula)
- [Simula Tutorial](https://www.tutorialspoint.com/simula/index.htm)
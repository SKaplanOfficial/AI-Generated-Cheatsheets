# Computer Science Cheatsheet

## Programming Concepts

### Variables and Data Types

Variables hold data and data types define the kind of data a variable can hold.

```ruby
# variable declaration
x = 10

# data types
string = "hello"
integer = 42
float = 3.14
boolean = true
array = [1, 2, 3]
hash = { name: "John", age: 25 }
```

# Functions

Functions are reusable code blocks that take input parameters and perform a set of instructions.

```ruby
# function declaration
def greet(name)
  puts "Hello, #{name}!"
end

# function call
greet("John")
```

# Loops

Loops allow you to repeatedly execute code.

```ruby
# while loop
i = 0
while i < 5 do
  puts i
  i += 1
end

# for loop
for i in 0..4
  puts i
end

# each loop
[1, 2, 3].each do |i|
  puts i
end
```

# Conditionals

Conditionals execute code based on whether a condition is true or false.

```ruby
# if statement
x = 10
if x > 5
  puts "x is greater than 5"
end

# else statement
if x < 5
  puts "x is less than 5"
else
  puts "x is greater than or equal to 5"
end

# case statement
grade = "A"
case grade
when "A"
  puts "Great job!"
when "B"
  puts "Good job!"
else
  puts "Try harder next time!"
end
```

# File Manipulation

Reading and writing files is a common task in programming.

```ruby
# writing to a file
File.open("file.txt", "w") do |file|
  file.write("Hello, world!")
end

# reading from a file
File.open("file.txt", "r") do |file|
  puts file.read
end
```

Resources

- [Ruby Documentation](https://www.ruby-lang.org/en/documentation/)
- [Ruby on Rails](https://rubyonrails.org/)
- [Learn Ruby the Hard Way](https://learnrubythehardway.org/)
- [Ruby Monk](https://rubymonk.com/)
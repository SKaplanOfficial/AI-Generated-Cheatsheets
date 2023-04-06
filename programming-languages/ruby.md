# Ruby Cheatsheet

## Unique Features
- Dynamic, object-oriented language
- Interpreted with garbage collection
- Duck typing
- Blocks and Procs
- Mixins
- RubyGems package manager

## Variables
```ruby
# Local variable
x = 5

# Instance variable
@name = "John"

# Class variable
@@count = 0

# Global variable
$debug = true
```

## Functions
```ruby
# Method definition
def say_hello(name)
  puts "Hello, #{name}!"
end

# Method call
say_hello("Ruby")
```

## Loops
```ruby
# While loop
while x < 10 do
  puts x
  x += 1
end

# For loop
for i in 0..5
  puts i
end

# Each iterator
(1..5).each do |i|
  puts i
end
```

## Conditionals
```ruby
# If statement
if x > 5
  puts "x is greater than 5"
elsif x == 5
  puts "x is equal to 5"
else
  puts "x is less than 5"
end

# Ternary operator
x > 5 ? "x is greater than 5" : "x is less than or equal to 5"
```

## File Manipulation
```ruby
# Open file
file = File.open("filename.txt", "r")

# Read file
contents = file.read

# Close file
file.close

# Write to file
File.open("filename.txt", "w") do |file|
  file.write("Hello, world!")
end
```

## Resources
- [Ruby Documentation](https://www.ruby-lang.org/en/documentation/)
- [RubyGems](https://rubygems.org/)
- [Ruby on Rails](https://rubyonrails.org/)
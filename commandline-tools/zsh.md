# Zsh Cheatsheet

## Basic Commands

```zsh
# Listing files and directories
ls

# Changing directories
cd directory_name

# Creating a directory
mkdir directory_name

# Removing a directory (with its contents)
rm -rf directory_name

# Creating a file
touch file_name

# Removing a file
rm file_name
```

## Aliases

```zsh
# Creating an alias
alias short_name='long_command'

# Removing an alias
unalias short_name
```

## Functions

```zsh
# Defining a function
function_name() {
  # code
}

# Calling a function
function_name
```

## Variables

```zsh
# Declaring variables
variable_name=value

# Accessing variables
$variable_name

# Environment variables
$ENV_VARIABLE_NAME
```

## Loops

```zsh
# While loop
while condition; do
  # code
done

# For loop
for i in {1..5}; do
  # code
done

# Each loop
for element in "${array[@]}"; do
  # code
done
```

## Conditionals

```zsh
# If statement
if condition; then
  # code
fi

# If-else statement
if condition; then
  # code
else
  # code
fi

# Ternary operator
condition && true_case || false_case
```

## Resources

- [Zsh Reference Card](http://www.bash2zsh.com/zsh_refcard/refcard.pdf)
- [Zsh Wiki](https://zsh.sourceforge.io/Guide/)
- [Oh My Zsh](https://ohmyz.sh/)
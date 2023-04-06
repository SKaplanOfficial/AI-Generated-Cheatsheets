# Lua Cheatsheet

Lua is a lightweight, high-level programming language designed primarily for embedded systems and game development. Here is an overview of its features, code blocks, and resources.

## Features

- Lua is a scripting language that can be embedded in other programs.
- It is dynamically typed, which means that variables do not need to be declared before use.
- Lua is designed to be lightweight and efficient, making it well-suited for use in embedded systems and game development.
- Lua supports functional programming paradigms as well as procedural programming.

## Code Blocks

### Variables

Variables are used to store data that can be used later in the program.

```lua
variableName = value
```

### Functions

Functions are code blocks that perform a specific task. They can be called by other parts of the program.

```lua
function functionName(parameter1, parameter2)
    -- code to be executed
end
```

### Conditionals

Conditionals allow the program to make decisions based on certain conditions.

```lua
if condition then
    -- code to be executed if condition is true
elseif otherCondition then
    -- code to be executed if otherCondition is true
else
    -- code to be executed if neither condition is true
end
```

### Loops

Loops allow the program to repeat a set of instructions.

```lua
for i = 1, 10 do
    -- code to be executed
end
```

### Tables

Tables are a fundamental part of Lua and are used to store and manipulate data.

```lua
tableName = {key1 = value1, key2 = value2}

-- accessing values
tableName.key1
tableName["key1"]
```

## Resources

Here are some resources for learning and using Lua:

- [Lua Documentation](https://www.lua.org/docs.html)
- [Lua subreddit](https://www.reddit.com/r/lua/)
- [Lua Tutorial](https://www.lua.org/manual/5.1/)
- [Lua on Stack Overflow](
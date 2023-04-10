# APL Cheatsheet

## Unique Features
- Array-oriented language
- Uses special characters for built-in functions and operators
- Supports complex numbers and other mathematical structures
- Strongly typed
- Interactive development environment
- High degree of conciseness

## Variables
```apl
⍺ ← 2 ⋄ ⍵ ← 3 ⋄ result ← ⍺ + ⍵
```

## Functions
```apl
function_name ← { ⍝ Function definition
  ⍝ Function body
}

function_name argument1 argument2 ⍝ Function call
```

## Loops
```apl
⍳10 ⍝ For loop

{⍝ While loop
  ⍝ Loop body
}⍣(condition)
```

## Conditionals
```apl
condition ⌷(true_code; false_code) ⍝ If-else statement

condition ⍴ true_code ⍝ If statement
```

## File Manipulation
```apl
⎕NGET 'file_name' ⍝ Reading from a file

⎕NPUT 'file_name' 'text to write' ⍝ Writing to a file
```

## Resources
- [APL Wiki](https://aplwiki.com/)
- [Dyalog APL](https://www.dyalog.com/)
- [APL Orchard](https://apl.chat/home) (community forum)
- [Mastering Dyalog APL](https://www.dyalog.com/mastering-dyalog-apl.htm) (book)
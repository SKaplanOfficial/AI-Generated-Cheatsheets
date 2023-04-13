# Brainfuck Cheatsheet

## Unique Features

- Minimalist programming language
- Only eight commands
- Uses a tape instead of variables
- Turing complete

## Commands

| Command | Description |
| ------- | ----------- |
| `>`     | Move the data pointer to the right |
| `<`     | Move the data pointer to the left |
| `+`     | Increment the value at the data pointer |
| `-`     | Decrement the value at the data pointer |
| `.`     | Output the value at the data pointer |
| `,`     | Input a value and store it at the data pointer |
| `[`     | If the value at the data pointer is zero, jump to the matching `]` |
| `]`     | If the value at the data pointer is not zero, jump to the matching `[` |

## Hello World

```
++++++++[>++++[>++>+++>+++>+<<<<-]>+>+>->>+[<]<-]>>.>---.+++++++..+++.>>.<-.<.+++.------.--------.>>+.>++.
```

## Resources

- [Official Brainfuck website](https://www.muppetlabs.com/~breadbox/bf/)
- [Brainfuck interpreter](https://www.dcode.fr/brainfuck-language)
- [Brainfuck tutorial](https://gist.github.com/roachhd/dce54bec8ba55fb17d3a)
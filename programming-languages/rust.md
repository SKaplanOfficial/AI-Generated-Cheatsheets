## Rust Cheatsheet

Rust is a systems programming language that is designed for performance, safety, and concurrency. Here's a quick overview of its unique features and some code blocks for common tasks.

### Variables

Declare variables using the `let` keyword. Rust is a statically typed language, but it can infer the data type of a variable from its value.

```rust
let x = 10;
let c = 'a';
let f = 3.14;
```

### Functions

Functions in Rust are declared using the `fn` keyword. They can take parameters and return values.

```rust
fn add(a: i32, b: i32) -> i32 {
  return a + b;
}
```

### Loops

Rust supports `for`, `while`, and `loop` loops for iterating over arrays or performing a task a certain number of times.

```rust
let numbers = [1, 2, 3, 4, 5];

for number in numbers.iter() {
  println!("{}", number);
}

let mut i = 0;
while i < numbers.len() {
  println!("{}", numbers[i]);
  i += 1;
}

i = 0;
loop {
  println!("{}", numbers[i]);
  i += 1;
  if i >= numbers.len() {
 break;
  }
}
```

### Conditionals

Use `if` statements to execute code based on a condition. `else if` and `else` statements can be used to handle multiple conditions.

```rust
let x = 10;

if x > 0 {
  println!("x is positive");
} else if x < 0 {
  println!("x is negative");
} else {
  println!("x is zero");
}
```

### File Manipulation

Rust provides built-in support for file manipulation, including reading and writing files, and interacting with the file system.

```rust
use std::fs;

fn main() {
  let contents = fs::read_to_string("/path/to/file.txt")
 .expect("Something went wrong reading the file");
  println!("{}", contents);

  fs::write("/path/to/file.txt", "New contents")
 .expect("Something went wrong writing the file");

  if fs::remove_file("/path/to/file.txt").is_ok() {
 println!("File deleted successfully");
  } else {
 println!("Error deleting file");
  }
}
```

### Resources

Here are some resources to help you learn more about Rust:

- [The Rust Programming Language](https://doc.rust-lang.org/book/) (Official Rust book)
- [Rust by Example](https://doc.rust-lang.org/stable/rust-by-example/) (Interactive Rust tutorial)
- [Rust Programming Language Cheat Sheet](https://cheats.rs/)
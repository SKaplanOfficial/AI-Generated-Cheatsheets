# Swift Cheatsheet

This cheatsheet provides an overview of Swift's unique features and includes code blocks for variables, functions, loops, conditionals, file manipulation, and more. 

## Variables

Declaring a variable:

```swift
var myVariable = "Hello, world!"
```

Declaring a constant:

```swift
let myConstant = 42
```

## Functions

Declaring a function:

```swift
func greet(person: String) -> String {
    let greeting = "Hello, " + person + "!"
    return greeting
}
```

Calling a function:

```swift
print(greet(person: "John"))
```

## Loops

For loop:

```swift
for index in 1...5 {
    print("\(index) times 5 is \(index * 5)")
}
```

While loop:

```swift
var i = 0
while i < 10 {
    print(i)
    i += 1
}
```

## Conditionals

If statement:

```swift
let temperature = 70
if temperature > 65 {
    print("It's warm outside!")
} else {
    print("It's cold outside!")
}
```

Switch statement:

```swift
let planet = "Earth"
switch planet {
case "Earth":
    print("Mostly harmless")
default:
    print("Not a safe place for humans")
}
```

## File Manipulation

Reading a file:

```swift
if let contents = try? String(contentsOfFile: "/path/to/file") {
    print(contents)
}
```

Writing to a file:

```swift
let text = "Hello, world!"
if let dir = FileManager.default.urls(for: .documentDirectory, in: .userDomainMask).first {
    let fileURL = dir.appendingPathComponent("file.txt")
    do {
        try text.write(to: fileURL, atomically: false, encoding: .utf8)
    }
    catch {
        // Handle error
    }
}
```

## Resources

- [The Swift Programming Language](https://docs.swift.org/swift-book/)
- [Swift.org](https://swift.org/)
- [Swift Playgrounds](https://www.apple.com/swift/playgrounds/)
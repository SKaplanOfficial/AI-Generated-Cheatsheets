# JSON Cheatsheet

## Overview
- JSON (JavaScript Object Notation) is a lightweight data interchange format.
- It is often used for APIs, configuration files, and data exchange between languages.
- JSON files use a `.json` file extension.

## Basic Syntax
- Data is represented as key-value pairs, where the key is a string and the value can be a string, number, boolean, null, array, or object.
- Keys and strings are enclosed in double quotes.
- Arrays are enclosed in square brackets and separated by commas.
- Objects are enclosed in curly braces and contain key-value pairs separated by commas.

## Example
```json
// Example JSON file
{
  "name": "John Smith",
  "age": 30,
  "address": {
    "street": "123 Main St",
    "city": "Anytown",
    "state": "CA",
    "zip": "12345"
  },
  "skills": ["Ruby", "Python", "JavaScript"]
}
```

## Data Types
- Strings: enclosed in double quotes
- Numbers: integers or floating-point numbers
- Booleans: `true` or `false`
- Null: `null`
- Arrays: ordered collections of data
- Objects: unordered collections of key-value pairs

## Advanced Syntax
- Comments are not allowed in JSON.
- Multiline strings can be represented using escape characters (`\n` for a new line).
- JSON can be pretty-printed to make it more human-readable.

## Resources
- [Official JSON Website](https://www.json.org/)
- [JSON Syntax](https://www.json.org/json-en.html)
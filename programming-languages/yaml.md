# YAML Cheatsheet

## Overview
- YAML (YAML Ain't Markup Language) is a human-readable data serialization format.
- It is often used for configuration files, data exchange between languages, and storing data in a structured format.
- YAML files use a `.yaml` or `.yml` file extension.

## Basic Syntax
- YAML files use indentation to indicate structure.
- Data is represented as key-value pairs, where the key and value are separated by a colon.
- Lists are represented using a hyphen followed by a space.

## Example
```yaml
# Example YAML file
name: John Smith
age: 30
address:
  street: 123 Main St
  city: Anytown
  state: CA
  zip: 12345
skills:
  - Ruby
  - Python
  - JavaScript
```

## Data Types
- Scalars: strings, numbers, booleans, null
- Lists: ordered collections of data
- Maps: unordered collections of key-value pairs

## Advanced Syntax
- Comments start with a hash (`#`) and continue to the end of the line.
- Multiline strings can be represented using the pipe (`|`) character.
- Anchors (`&`) and aliases (`*`) can be used to reference the same data in multiple places.

## Resources
- [Official YAML Website](https://yaml.org/)
- [YAML Syntax](https://yaml.org/spec/1.2/spec.html)
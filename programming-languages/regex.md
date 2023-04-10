# Regular Expressions (Regex) Cheatsheet

## Overview
- Regular expressions (regex or regexp) are patterns used to match character combinations in strings.
- They are often used in programming languages for tasks such as search and replace, input validation, and parsing.
- Regex syntax can vary slightly between programming languages and tools.

## Basic Syntax
- Characters in a regex match themselves, unless they are special characters with a specific meaning.
- Special characters can be escaped using a backslash (`\`) to match the character itself.
- Character classes can be used to match a range of characters.
- Quantifiers can be used to match a specific number of characters.

## Examples
### Example 1: Matching an Email Address
```regex
// Example regex to match an email address
[\w.%+-]+@[A-Za-z0-9.-]+\.[A-Za-z]{2,}
```
This regex will match an email address in the format `username@domain.com`.

### Example 2: Matching a Phone Number
```regex
// Example regex to match a phone number
\+?\d{1,3}[-. ]?\d{3}[-. ]?\d{4}
```
This regex will match a phone number in a variety of formats, including `123-456-7890`, `123.456.7890`, and `+1 123-456-7890`.

### Example 3: Matching a URL
```regex
// Example regex to match a URL
https?://[\w\-\.]+(:\d+)?(/[\w/_\.]*)?
```
This regex will match a URL in a variety of formats, including `http://www.example.com`, `https://example.com/path/to/page.html`, and `http://www.example.com:8080/path/to/page.html`.

## Special Characters
- `.`: Matches any single character except a newline.
- `^`: Matches the start of a string.
- `$`: Matches the end of a string.
- `*`: Matches zero or more occurrences of the previous character.
- `+`: Matches one or more occurrences of the previous character.
- `?`: Matches zero or one occurrence of the previous character.
- `|`: Matches either the character on the left or the character on the right.
- `[]`: Matches any one character within the brackets.
- `()`: Groups characters together.

## Character Classes
- `\d`: Matches any digit character.
- `\w`: Matches any word character (alphanumeric and underscore).
- `\s`: Matches any whitespace character.
- `\D`: Matches any non-digit character.
- `\W`: Matches any non-word character.
- `\S`: Matches any non-whitespace character.

## Quantifiers
- `{n}`: Matches exactly n occurrences of the previous character.
- `{n,}`: Matches n or more occurrences of the previous character.
- `{n,m}`: Matches between n and m occurrences of the previous character.

## Advanced Syntax
- Lookaheads (`(?=...)`) and lookbehinds (`(?<=...)`) can be used to match characters based on what precedes or follows them.
- Backreferences (`\1`, `\2`, etc.) can be used to refer to previously matched groups.
- Flags can be used to modify the behavior of the regex (e.g. case-insensitive matching).

## Resources
- [RegexOne](https://regexone.com/) - Interactive regex tutorial
- [Regular-Expressions.info](https://www.regular-expressions.info/) - Comprehensive regex guide
- [Regex101](https://regex101.com/) - Online regex tester and debugger
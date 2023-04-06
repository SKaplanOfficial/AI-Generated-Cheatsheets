# Grep Cheatsheet

## Overview
`grep` is a command-line utility used for searching text files for specific patterns.

## Basic Usage
```bash
grep pattern file.txt
```
Searches for `pattern` in `file.txt` and prints all lines that match.

## Flags
- `-i`: Ignore case when searching
- `-v`: Invert the match, printing all lines that do not match
- `-r`: Recursively search all files in a directory
- `-n`: Print the line number for each match
- `-w`: Match whole words only
- `-c`: Print only the count of matching lines

## Regular Expressions
`grep` uses regular expressions to define search patterns. Some common regex syntax includes:
- `.`: Matches any single character
- `*`: Matches zero or more of the preceding character
- `+`: Matches one or more of the preceding character
- `?`: Matches zero or one of the preceding character
- `[]`: Matches any character within the brackets
- `^`: Matches the beginning of a line
- `$`: Matches the end of a line
- `|`: Matches either the expression before or after the pipe

## Examples
```bash
grep -i "hello" file.txt        # Search for "hello" case-insensitively
grep -v "goodbye" file.txt     # Print all lines that do not contain "goodbye"
grep -rn "error" /var/log      # Recursively search all files in /var/log for "error" and print line numbers
grep -w "the" file.txt         # Match whole words only
grep -E "foo|bar" file.txt     # Match either "foo" or "bar" using extended regex syntax
```

## Resources
- [Grep on Wikipedia](https://en.wikipedia.org/wiki/Grep)
- [Grep manual](https://www.gnu.org/software/grep/manual/grep.html)
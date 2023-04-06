# AWK Cheatsheet

## Overview of unique features

- Text processing language
- Uses pattern-action paradigm
- Built-in variables for manipulating text
- Supports regular expressions
- Can be used for data extraction and reporting

## Text processing

```awk
# Print a specific field from a file
awk '{print $1}' file.txt

# Search for a specific pattern in a file
awk '/pattern/ {print}' file.txt

# Use built-in variables to manipulate text
awk '{print toupper($0)}' file.txt
awk '{print length($1)}' file.txt
```

## Regular expressions

```awk
# Search for a regular expression in a file
awk '/[0-9]+/ {print}' file.txt

# Use regular expression to match a specific pattern
awk '/^start/,/^end/ {print}' file.txt
```

## Reporting and data extraction

```awk
# Calculate the sum of a column in a CSV file
awk -F, '{ sum += $3 } END { print sum }' file.csv

# Extract data from a log file
awk '/error/ {print $0}' log.txt
```

## Resources

- [AWK documentation](https://www.gnu.org/software/gawk/manual/gawk.html)
- [AWK tutorial](https://www.tutorialspoint.com/awk/index.htm)
- [AWK forum](https://stackoverflow.com/questions/tagged/awk) for community support and troubleshooting.
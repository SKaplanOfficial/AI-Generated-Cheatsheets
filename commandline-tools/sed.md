# sed Cheatsheet

## Overview

sed (stream editor) is a Unix utility used to perform basic text transformations on an input stream (a file or input from a pipeline). It is a powerful tool for editing files in batch mode or in a script.

## Usage

```bash
sed [options] [script] [input_file]
```

## Options

- `-n`: Suppress automatic printing of pattern space.
- `-e script`: Add the script to the commands to be executed.
- `-f script_file`: Add the commands contained in the script file to the commands to be executed.
- `-i`: Edit files in place.
- `-r`: Use extended regular expressions in the script.
- `-h`: Do not print filenames when editing files in place.
- `-V`: Display version information.
- `-h`: Display help information.

## Commands

- `s`: Replace the first occurrence of a pattern with a replacement string.
- `g`: Replace all occurrences of a pattern with a replacement string.
- `p`: Print the pattern space.
- `d`: Delete the pattern space.
- `a`: Append text to the output.
- `i`: Insert text before the output.
- `q`: Quit processing the input.
- `r file`: Append the contents of a file to the output.

## Examples

Replace the first occurrence of "foo" with "bar" in a file:

```bash
sed 's/foo/bar/' input_file.txt
```

Replace all occurrences of "foo" with "bar" in a file:

```bash
sed 's/foo/bar/g' input_file.txt
```

Delete lines that contain the word "foo" in a file:

```bash
sed '/foo/d' input_file.txt
```

Insert a line before the first line of a file:

```bash
sed '1i This is the first line.' input_file.txt
```

## Resources

- [GNU sed Manual](https://www.gnu.org/software/sed/manual/sed.html)
- [Sed - An Introduction and Tutorial](http://www.grymoire.com/Unix/Sed.html)
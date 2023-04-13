# Xargs Cheatsheet

The `xargs` command is used to execute a command with arguments read from standard input or from a file.

## Basic Syntax

```
command | xargs [options] executable
```

- `command`: The command whose output will be used as input for `xargs`.
- `executable`: The command to be executed with arguments.

## Examples

- Copy all files with a specific extension to a new directory:

  ```
  find /path/to/source -type f -name "*.txt" | xargs -I {} cp {} /path/to/destination
  ```

- Delete all files with a specific extension:

  ```
  find /path/to/directory -type f -name "*.log" -print0 | xargs -0 rm
  ```

- Find all files with a specific name and change their permissions:

  ```
  find /path/to/directory -type f -name "file.txt" -print0 | xargs -0 chmod 644
  ```

- Execute a command with arguments from a file:

  ```
  cat file.txt | xargs -I {} command {}
  ```

## Options

| Option | Description |
| ------ | ----------- |
| `-I` | Replaces occurrences of a placeholder string with the input arguments. |
| `-0` | Uses null characters as the delimiter instead of whitespace. |
| `-n` | Limits the number of arguments passed to the command. |
| `-P` | Limits the number of parallel processes. |
| `-t` | Displays the command being executed. |

## Resources

- [Official `xargs` command manual](https://man7.org/linux/man-pages/man1/xargs.1.html)
- [Linuxize `xargs` command tutorial](https://linuxize.com/post/xargs-command-in-linux/)
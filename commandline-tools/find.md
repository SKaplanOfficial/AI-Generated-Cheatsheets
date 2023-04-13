# Find Cheatsheet

The `find` command is used to search for files and directories in a specified location based on different search criteria.

## Basic Syntax

```
find [path] [expression]
```

- `path`: The directory to start the search from.
- `expression`: The search criteria.

## Examples

- Find all files with a specific name:

  ```
  find /path/to/directory -name "filename"
  ```

- Find all directories with a specific name:

  ```
  find /path/to/directory -type d -name "dirname"
  ```

- Find all files modified within the last 24 hours:

  ```
  find /path/to/directory -type f -mtime -1
  ```

- Find all files larger than a specific size:

  ```
  find /path/to/directory -type f -size +10M
  ```

- Find all empty files and directories:

  ```
  find /path/to/directory -empty
  ```

- Find all files with a specific extension:

  ```
  find /path/to/directory -type f -name "*.txt"
  ```

- Find all files owned by a specific user:

  ```
  find /path/to/directory -type f -user username
  ```

- Find all files with specific permissions:

  ```
  find /path/to/directory -type f -perm 644
  ```

## Options

| Option | Description |
| ------ | ----------- |
| `-name` | Search for files with a specific name. |
| `-type` | Search for a specific type of file (e.g., file, directory). |
| `-mtime` | Search for files modified within a specific period of time. |
| `-size` | Search for files larger or smaller than a specific size. |
| `-empty` | Search for empty files or directories. |
| `-user` | Search for files owned by a specific user. |
| `-perm` | Search for files with specific permissions. |

## Resources

- [Official `find` command manual](https://man7.org/linux/man-pages/man1/find.1.html)
- [Linuxize `find` command tutorial](https://linuxize.com/post/how-to-use-linux-find-command/)
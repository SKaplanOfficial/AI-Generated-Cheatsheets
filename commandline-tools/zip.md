# Zip Cheatsheet

The `zip` command is used to compress files and directories into a compressed archive file in a ZIP format.

## Basic Syntax

```
zip [options] archive.zip file1 file2 directory1
```

- `archive.zip`: The name of the compressed archive file to create.
- `file1`, `file2`, `directory1`: The files and directories to include in the archive.

## Examples

- Create a compressed archive file from a directory:

  ```
  zip -r archive.zip /path/to/directory
  ```

- Add files to an existing compressed archive file:

  ```
  zip archive.zip file1 file2
  ```

- Extract files from a compressed archive file:

  ```
  unzip archive.zip
  ```

- Extract files from a compressed archive file to a specific directory:

  ```
  unzip archive.zip -d /path/to/directory
  ```

## Options

| Option | Description |
| ------ | ----------- |
| `-r` | Compress directories recursively. |
| `-m` | Move the original files to the ZIP archive. |
| `-u` | Update the ZIP archive with only new or modified files. |
| `-d` | Extract files to a specific directory. |
| `-l` | List the contents of the ZIP archive. |
| `-v` | Display verbose output. |

## Resources

- [Official `zip` command website](https://infozip.sourceforge.io/)
- [Linuxize `zip` command tutorial](https://linuxize.com/post/how-to-zip-files-and-directories-in-linux/)
# Lsof Command Cheatsheet

The `lsof` command is used to display information about files and processes that are currently open or in use on a Unix-based operating system.

## Basic Syntax

```
lsof [options]
```

## Examples

- Display a list of all open files:

  ```
  lsof
  ```

- Display a list of all open files for a specific process:

  ```
  lsof -p <PID>
  ```

- Display a list of all open files for a specific user:

  ```
  lsof -u <username>
  ```

- Display a list of all open network connections:

  ```
  lsof -i
  ```

- Display a list of all open files for a specific directory:

  ```
  lsof +D /path/to/directory
  ```

## Options

| Option | Description |
| ------ | ----------- |
| `-p` | Displays information about a specific PID. |
| `-u` | Displays information about a specific user. |
| `-i` | Displays information about open network connections. |
| `+D` | Displays information about open files for a specific directory. |
| `-c` | Displays information about open files for a specific command. |
| `-t` | Displays only the PIDs of the matching processes. |
| `-h` | Displays help information. |

## Resources

- [Official `lsof` website](https://people.freebsd.org/~abe/)
- [Linuxize `lsof` command tutorial](https://linuxize.com/post/how-to-use-the-lsof-command-on-linux/)
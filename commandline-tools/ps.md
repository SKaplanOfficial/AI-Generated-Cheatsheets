# Ps Cheatsheet

The `ps` command is used to display information about running processes on a Unix-based operating system.

## Basic Syntax

```
ps [options]
```

## Examples

- Display a list of running processes for the current user:

  ```
  ps
  ```

- Display a list of running processes for all users:

  ```
  ps -ef
  ```

- Display a list of running processes with additional information:

  ```
  ps aux
  ```

- Display a list of running processes in full format:

  ```
  ps -efl
  ```

- Display a list of running processes with a specific PID:

  ```
  ps -p <PID>
  ```

- Display a list of running processes with a specific name:

  ```
  ps -C <process name>
  ```

## Options

| Option | Description |
| ------ | ----------- |
| `-e` | Displays information about all processes. |
| `-f` | Displays a full listing of processes with additional information. |
| `-l` | Displays a long listing of processes with additional information. |
| `-p` | Displays information about a specific PID. |
| `-C` | Displays information about a specific process name. |
| `-u` | Displays information about processes for a specific user. |

## Resources

- [Official `ps` command manual](https://man7.org/linux/man-pages/man1/ps.1.html)
- [Linuxize `ps` command tutorial](https://linuxize.com/post/how-to-use-ps-command-to-monitor-linux-processes/)
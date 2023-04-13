# Netcat Cheatsheet

The `netcat` command is a utility for reading from and writing to network connections using TCP or UDP protocols.

## Basic Syntax

```
nc [options] host port
```

- `host`: The hostname or IP address of the remote system.
- `port`: The port number to connect to on the remote system.

## Examples

- Connect to a remote system using TCP:

  ```
  nc host port
  ```

- Connect to a remote system using UDP:

  ```
  nc -u host port
  ```

- Listen for incoming connections on a specific port:

  ```
  nc -l port
  ```

- Transfer a file over a network:

  ```
  nc -w 3 host port < file
  ```

- Send a file to a remote system:

  ```
  nc -w 3 host port > file
  ```

## Options

| Option | Description |
| ------ | ----------- |
| `-u` | Use UDP instead of TCP. |
| `-l` | Listen for incoming connections. |
| `-p` | Specify the local port number to use. |
| `-w` | Set a timeout value. |
| `-v` | Display verbose output. |
| `-n` | Do not use DNS resolution. |

## Resources

- [Netcat Wikipedia article](https://en.wikipedia.org/wiki/Netcat)
- [Linuxize `netcat` command tutorial](https://linuxize.com/post/netcat-nc-command-with-examples/)
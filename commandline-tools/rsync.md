# Rsync Cheatsheet

The `rsync` command is used to synchronize files and directories between two locations, either on the same system or on different systems over a network.

## Basic Syntax

```
rsync [options] source destination
```

- `source`: The source directory or file to be copied.
- `destination`: The destination directory or file to be copied to.

## Examples

- Copy a file from one directory to another:

  ```
  rsync /path/to/source/file /path/to/destination/
  ```

- Copy a directory and its contents to another directory:

  ```
  rsync -r /path/to/source/directory /path/to/destination/
  ```

- Copy files and directories recursively while preserving permissions and timestamps:

  ```
  rsync -av /path/to/source/ /path/to/destination/
  ```

- Copy files and directories over SSH:

  ```
  rsync -avz -e ssh /path/to/source/ user@remote:/path/to/destination/
  ```

- Synchronize two directories, copying only the files that have changed:

  ```
  rsync -av --delete /path/to/source/ /path/to/destination/
  ```

## Options

| Option | Description |
| ------ | ----------- |
| `-r` | Copy directories recursively. |
| `-a` | Archive mode; preserves permissions, timestamps, and ownerships. |
| `-v` | Verbose mode; displays progress of the transfer. |
| `-z` | Compresses the data being transferred. |
| `-e` | Specifies the remote shell to use for SSH transfers. |
| `--delete` | Deletes files in the destination that do not exist in the source. |

## Resources

- [Official `rsync` website](https://rsync.samba.org/)
- [Linuxize `rsync` command tutorial](https://linuxize.com/post/how-to-use-rsync-for-local-and-remote-data-transfer-and-synchronization/)
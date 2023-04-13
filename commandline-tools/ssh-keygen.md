# SSH-Keygen Cheatsheet

The `ssh-keygen` command is used to generate, manage, and convert authentication keys for SSH (Secure Shell) protocol.

## Basic Syntax

```
ssh-keygen [options]
```

## Examples

- Generate a new SSH key pair:

  ```
  ssh-keygen
  ```

- Generate a new SSH key pair with a specific name:

  ```
  ssh-keygen -f /path/to/key
  ```

- Generate a new SSH key pair with a specific type and size:

  ```
  ssh-keygen -t rsa -b 4096
  ```

- Generate a new SSH key pair with a specific comment:

  ```
  ssh-keygen -C "user@host"
  ```

- Convert a SSH key to OpenSSH format:

  ```
  ssh-keygen -p -m PEM -f /path/to/key
  ```

## Options

| Option | Description |
| ------ | ----------- |
| `-t` | Specifies the type of key to create. |
| `-b` | Specifies the number of bits in the key. |
| `-f` | Specifies the filename of the key file. |
| `-C` | Adds a comment to the key. |
| `-N` | Specifies a new passphrase for the key. |
| `-p` | Changes the passphrase of the key. |
| `-m` | Specifies the key format to use for the key. |
| `-l` | Displays the fingerprint of the key. |

## Resources

- [Official `ssh-keygen` command manual](https://man7.org/linux/man-pages/man1/ssh-keygen.1.html)
- [Linuxize `ssh-keygen` command tutorial](https://linuxize.com/post/how-to-set-up-ssh-keys-on-ubuntu-20-04/)
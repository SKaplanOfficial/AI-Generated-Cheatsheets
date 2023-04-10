# SCP Cheatsheet

## Unique Features
- Secure file transfer protocol for copying files between remote hosts
- Encrypted data transfer for improved security
- Built-in to most Unix-based systems
- Can be used with SSH for authentication and encryption
- Supports copying files and directories recursively

## Copying Files
```scp
scp source_file destination_file
scp user@source_host:source_file user@destination_host:destination_file
```

## Copying Directories
```scp
scp -r source_directory destination_directory
scp -r user@source_host:source_directory user@destination_host:destination_directory
```

## Specifying Port Number
```scp
scp -P port_number source_file destination_file
scp -P port_number user@source_host:source_file user@destination_host:destination_file
```

## Preserving File Attributes
```scp
scp -p source_file destination_file
scp -p -r source_directory destination_directory
```

## Verbose Output
```scp
scp -v source_file destination_file
scp -v -r source_directory destination_directory
```

## Resources
- [SCP Command Examples](https://www.howtoforge.com/linux-scp-command/)
- [SSH and SCP: Howto, tips & tricks](https://www.ssh.com/academy/ssh/scp) (tutorial)
- [Secure Copy (SCP) on Wikipedia](https://en.wikipedia.org/wiki/Secure_copy)
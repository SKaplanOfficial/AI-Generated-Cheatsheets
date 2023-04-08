# netstat Cheatsheet

## Unique Features
* A command-line tool to display network connection information in Linux, Unix-like and Windows operating systems
* Displays active network connections, listening ports, routing tables, and network interface statistics
* Can also identify the process that initiated each connection
* Useful for troubleshooting network connectivity issues and network security auditing

## Basic Usage
* Display all active network connections: `netstat`
* Display listening ports: `netstat -l`
* Display statistics for all network interfaces: `netstat -i`
* Display routing table: `netstat -r`

## Advanced Usage
* Display active network connections for a specific protocol: `netstat -[tcp|udp]`
* Display network statistics in continuous mode: `netstat -c`
* Display process information for each connection: `netstat -p`
* Display all listening ports including those owned by processes without root access: `sudo netstat -lnptu`
* Display the status of sockets: `netstat -s`
* Display the list of network interfaces and their IP addresses: `netstat -ie`
* Display active network connections for a specific process: `netstat -p | grep [process_name]`

## Resources
* `netstat --help` or `man netstat` in your terminal
* [Linux Man Page for netstat](https://linux.die.net/man/8/netstat)
* [Microsoft Documentation on netstat](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/netstat) for Windows-based systems.

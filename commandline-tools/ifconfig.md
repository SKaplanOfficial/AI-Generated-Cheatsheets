# ifconfig Cheatsheet

## Unique Features
* A command-line tool to display network interface information in Linux and Unix-like operating systems
* Displays IP address, subnet mask, MAC address, and network interface status
* Can also configure network interfaces and set IP addresses manually
* Useful for troubleshooting network connectivity issues

## Basic Usage
* Display all network interface information: `ifconfig`
* Display information for a specific interface: `ifconfig [interface_name]`
* Enable an interface: `ifconfig [interface_name] up`
* Disable an interface: `ifconfig [interface_name] down`
* Assign an IP address to an interface: `ifconfig [interface_name] [ip_address]`
* Assign a netmask to an interface: `ifconfig [interface_name] netmask [netmask]`

## Advanced Usage
* Display only active network interfaces: `ifconfig -a`
* Display information in short format: `ifconfig -s`
* Display information in verbose format: `ifconfig -v`
* Assign a broadcast address to an interface: `ifconfig [interface_name] broadcast [broadcast_address]`
* Assign a point-to-point address to an interface: `ifconfig [interface_name] pointopoint [point_to_point_address]`
* Enable/disable promiscuous mode on an interface: `ifconfig [interface_name] [promisc|nopromisc]`

## Resources
* `ifconfig --help` or `man ifconfig` in your terminal
* [Linux Man Page for ifconfig](https://linux.die.net/man/8/ifconfig)

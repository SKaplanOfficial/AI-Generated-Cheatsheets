# ipconfig Cheatsheet

## Unique Features
* A command-line tool to display network interface information in Windows
* Displays IP address, subnet mask, default gateway, and DNS servers
* Can also release and renew DHCP leases and flush DNS resolver cache
* Useful for troubleshooting network connectivity issues

## Basic Usage
* Display all network interface information: `ipconfig`
* Display detailed information for a specific interface: `ipconfig /all`
* Release DHCP lease: `ipconfig /release`
* Renew DHCP lease: `ipconfig /renew`
* Flush DNS resolver cache: `ipconfig /flushdns`
* Display DNS resolver cache: `ipconfig /displaydns`
* Display DHCP lease information: `ipconfig /allcompartments /all`

## Advanced Usage
* Display IPv4 configuration only: `ipconfig /ipv4`
* Display IPv6 configuration only: `ipconfig /ipv6`
* Display interface information in brief: `ipconfig /brief`
* Display all interfaces with their MAC addresses: `ipconfig /allcompartments /all /physical`
* Disable/Enable an interface: `netsh interface set interface [interface_name] admin=[enable/disable]`

## Resources
* `ipconfig /?` in your Command Prompt
* [Microsoft Documentation on ipconfig](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/ipconfig)

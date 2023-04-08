# Raspberry Pi Cheatsheet

## Unique Features
* Credit-card sized single-board computer
* Low cost and low power consumption
* Runs various operating systems, including Linux and Windows 10 IoT
* Provides GPIO pins for hardware interfacing
* Supports camera and display modules
* Popular for educational and hobbyist projects

## Basic Usage
* Connect to Raspberry Pi over SSH: `ssh [username]@[ip_address]`
* Access Raspberry Pi desktop remotely: `VNC Viewer`
* Update package list: `sudo apt update`
* Upgrade installed packages: `sudo apt upgrade`
* Shutdown Raspberry Pi: `sudo shutdown now`

## GPIO Usage
* Export GPIO pin: `sudo echo [pin_number] > /sys/class/gpio/export`
* Set GPIO direction: `sudo echo [in/out] > /sys/class/gpio/gpio[pin_number]/direction`
* Read GPIO value: `sudo cat /sys/class/gpio/gpio[pin_number]/value`
* Write GPIO value: `sudo echo [0/1] > /sys/class/gpio/gpio[pin_number]/value`

## Advanced Usage
* Install software packages: `sudo apt install [package_name]`
* Configure network settings: `sudo nano /etc/dhcpcd.conf`
* Mount external storage devices: `sudo mount /dev/[device_name] [mount_point]`
* Create and run Python scripts: `nano [script_name].py && python [script_name].py`

## Resources
* [Raspberry Pi Official Website](https://www.raspberrypi.org/)
* [Raspberry Pi Documentation](https://www.raspberrypi.org/documentation/)
* [Raspberry Pi GPIO Pinout](https://pinout.xyz/)
* [MagPi Magazine](https://magpi.raspberrypi.org/)

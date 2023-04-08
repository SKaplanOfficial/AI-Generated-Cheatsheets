# Top Cheatsheet

## Unique Features
* Command-line process monitor
* Displays real-time system resource usage
* Can sort processes by various criteria
* Supports process manipulation (e.g. kill process)
* Available on most Unix-like operating systems

## Basic Usage
* Launch top: `top`
* Sort processes by CPU usage: `top -o %CPU`
* Sort processes by memory usage: `top -o %MEM`
* Filter processes by name: `top -pid [process_id]`
* Change refresh interval: `top -d [interval]`
* Show processes owned by user: `top -U [username]`

## Advanced Usage
* Renice a process: `r [process_id]`
* Kill a process: `k [process_id]`
* Change process priority: `r [process_id] -n [priority]`
* Toggle CPU time display: `1`
* Toggle thread display: `H`

## Output Options
* Save output to file: `top -b -n [number_of_samples] > [output_file]`
* Show only specific columns: `top -stats [columns]`

## Resources
* `man top` in your terminal
* [Top User Guide](https://www.booleanworld.com/guide-linux-top-command/)

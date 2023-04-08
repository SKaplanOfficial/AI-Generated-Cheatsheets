# Wget Cheatsheet

## Unique Features
* Command-line utility for downloading files from the web
* Supports recursive downloads
* Can follow links and download pages and their requisites
* Supports resuming interrupted downloads
* Can be used for mirroring entire websites
* Available on most Unix-like operating systems

## Basic Usage
* Download a single file: `wget [url]`
* Download a file with a specific name: `wget -O [filename] [url]`
* Download a file in the background: `wget -b [url]`
* Download a file with a user agent string: `wget --user-agent="[user agent]" [url]`

## Advanced Usage
* Limit download speed: `wget --limit-rate=[rate] [url]`
* Download recursively: `wget -r [url]`
* Mirror a website: `wget --mirror -p --convert-links -P [directory] [url]`
* Resume a partially downloaded file: `wget -c [url]`
* Follow links and download requisites: `wget --page-requisites [url]`
* Use a proxy server: `wget --proxy-user=[username] --proxy-password=[password] --proxy=[server] [url]`

## Output Options
* Log to a file: `wget -o [logfile] [url]`
* Verbose output: `wget -v [url]`
* No output: `wget -q [url]`

## Resources
* [Wget Manual](https://www.gnu.org/software/wget/manual/)
* [Wget Wikipedia Page](https://en.wikipedia.org/wiki/Wget)

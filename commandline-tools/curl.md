# cURL Cheatsheet

## Overview of unique features

- Command-line tool for transferring data
- Supports a wide range of protocols (HTTP, FTP, SMTP, etc.)
- Can be used for testing APIs and web services
- Can be used for web scraping and data extraction

## Basic usage

```bash
# Make a GET request
curl http://example.com

# Make a POST request with data
curl -X POST -d "param1=value1&param2=value2" http://example.com

# Make a request with headers
curl -H "Authorization: Bearer token" http://example.com

# Save response to a file
curl -o output.txt http://example.com
```

## Authentication

```bash
# Basic authentication
curl -u username:password http://example.com

# OAuth authentication
curl -H "Authorization: Bearer token" http://example.com
```

## Cookies

```bash
# Send cookies with a request
curl -b "cookie1=value1; cookie2=value2" http://example.com

# Save cookies to a file
curl -c cookies.txt http://example.com

# Load cookies from a file
curl -b cookies.txt http://example.com
```

## Advanced usage

```bash
# Follow redirects
curl -L http://example.com

# Set a custom user agent
curl -A "Mozilla/5.0" http://example.com

# Set a timeout
curl --connect-timeout 10 http://example.com

# Use a proxy
curl -x http://proxy.example.com:8080 http://example.com
```

## Resources

- [cURL documentation](https://curl.se/docs/)
- [cURL tutorial](https://curl.se/docs/httpscripting.html)
- [cURL forum](https://stackoverflow.com/questions/tagged/curl) for community support and troubleshooting.
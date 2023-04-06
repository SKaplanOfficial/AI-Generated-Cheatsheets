# dwebp Cheatsheet

## Overview

dwebp is a command-line tool used to decode images in the WebP format. It is part of the WebP image format library, developed by Google.

## Installation

dwebp is included in the WebP image format library, which can be downloaded from the [official WebP website](https://developers.google.com/speed/webp/docs/using).

## Usage

```bash
dwebp input_file.webp -o output_file.png
```

## Options

- `-quiet`: Disable verbose output.
- `-nofancy`: Disable the use of fancy YUV420-to-RGB conversion.
- `-mt`: Enable multi-threading.
- `-version`: Display version information.
- `-h`: Display help information.

## Examples

Convert a WebP image to PNG format:

```bash
dwebp input.webp -o output.png
```

Convert a WebP image to PNG format with multi-threading enabled:

```bash
dwebp -mt input.webp -o output.png
```

## Resources

- [WebP Documentation](https://developers.google.com/speed/webp/docs)
- [WebP Gallery](https://developers.google.com/speed/webp/gallery1)
# cwebp Cheatsheet

## Overview

cwebp is a command-line tool used to compress images in the WebP format. It is part of the WebP image format library, developed by Google.

## Installation

cwebp is included in the WebP image format library, which can be downloaded from the [official WebP website](https://developers.google.com/speed/webp/docs/using).

## Usage

```bash
cwebp [options] input_file -o output_file.webp
```

## Options

- `-q <float>`: Set the compression quality factor (0-100, default: 75).
- `-m <int>`: Set the maximum size of the output file (in bytes).
- `-lossless`: Enable lossless compression mode.
- `-alpha_q <int>`: Set the transparency-compression quality factor (0-100, default: 100).
- `-alpha_method <int>`: Set the transparency-compression method (0=fast, 1=default, 2=slow).
- `-h`: Display help information.

## Examples

Convert a PNG image to lossy WebP format with default settings:

```bash
cwebp input.png -o output.webp
```

Convert a PNG image to lossless WebP format with custom compression quality:

```bash
cwebp -lossless -q 90 input.png -o output.webp
```

Convert a PNG image with transparency to lossy WebP format with custom settings:

```bash
cwebp -q 80 -alpha_q 90 -alpha_method 1 input.png -o output.webp
```

## Resources

- [WebP Documentation](https://developers.google.com/speed/webp/docs)
- [WebP Gallery](https://developers.google.com/speed/webp/gallery1)
# FFmpeg Cheatsheet

## Overview
FFmpeg is a command-line tool used for recording, converting, and streaming audio and video.

## Installation
- [FFmpeg website](https://ffmpeg.org/download.html)
- macOS: `brew install ffmpeg`
- Ubuntu/Debian: `sudo apt-get install ffmpeg`
- Windows: [Download the binary](https://ffmpeg.org/download.html#build-windows)

## Basic Usage
```bash
ffmpeg -i input.mp4 output.avi
```
Converts `input.mp4` to `output.avi`.

## Input/Output
- `-i`: Specifies the input file.
- `-f`: Specifies the output format.
- `-c`: Specifies the codec to use for the output.
- `-s`: Specifies the frame size for the output.
- `-b`: Specifies the bitrate for the output.
- `-ar`: Specifies the audio sample rate for the output.
- `-ac`: Specifies the number of audio channels for the output.

## Filters
- `-vf`: Applies a video filter to the output.
- `-af`: Applies an audio filter to the output.

## Examples
```bash
ffmpeg -i input.mp4 -c:v libx264 -c:a copy output.mp4   # Convert to MP4 using H.264 video codec
ffmpeg -i input.mp4 -vf "scale=720:-1" output.mp4   # Resize video to 720p height
ffmpeg -i input.mp4 -af "volume=2" output.mp4     # Increase audio volume by 2x
ffmpeg -f avfoundation -i "default" output.mp4    # Record video from webcam on macOS
ffmpeg -i input.mp4 -f mpegts udp://127.0.0.1:1234    # Stream video over UDP
```

## Resources
- [FFmpeg website](https://ffmpeg.org/)
- [FFmpeg documentation](https://ffmpeg.org/documentation.html)
- [FFmpeg Wiki](https://trac.ffmpeg.org/wiki)
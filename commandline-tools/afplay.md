# afplay Cheatsheet

## Overview

afplay is a command-line audio player for macOS. It allows you to play audio files from the command line or from a script.

## Usage

```bash
afplay [options] audio_file
```

## Options

- `-v volume`: Set the playback volume (0.0 - 1.0).
- `-t time`: Play the audio file for a specific duration (in seconds).
- `-r rate`: Play the audio file at a specific sample rate.
- `-h`: Display help information.

## Examples

Play an audio file:

```bash
afplay audio_file.mp3
```

Play an audio file with reduced volume:

```bash
afplay -v 0.5 audio_file.mp3
```

Play an audio file for 30 seconds:

```bash
afplay -t 30 audio_file.mp3
```

## Resources

- [afplay Man Page](https://ss64.com/osx/afplay.html)
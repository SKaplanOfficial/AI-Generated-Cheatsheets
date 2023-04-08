# ImageMagick Cheatsheet

## Unique Features
* Command-line image editing tool
* Can manipulate and convert images in over 100 formats
* Supports batch processing of images
* Supports advanced image transformations and effects
* Can be used to create animations and GIFs
* Available on most operating systems

## Basic Usage
* Convert image format: `convert [input_file] [output_file]`
* Resize image: `convert [input_file] -resize [width]x[height] [output_file]`
* Crop image: `convert [input_file] -crop [width]x[height]+[x_offset]+[y_offset] [output_file]`
* Rotate image: `convert [input_file] -rotate [angle] [output_file]`
* Add border to image: `convert [input_file] -border [size] [output_file]`

## Advanced Usage
* Apply image filters and effects: `convert [input_file] -filter [filter] [output_file]`
* Compose images: `convert [input_file_1] [input_file_2] -compose [operator] -composite [output_file]`
* Create animated GIF: `convert -delay [delay_time] [input_files] [output_file]`
* Extract image frames from a video: `convert [video_file] -coalesce [output_files]`

## Output Options
* Set image quality: `convert [input_file] -quality [value] [output_file]`
* Output to stdout: `convert [input_file] -`
* Add image to clipboard: `convert [input_file] - | pbcopy`

## Resources
* [ImageMagick Documentation](https://imagemagick.org/script/command-line-tools.php)
* [ImageMagick Tutorials](https://imagemagick.org/script/index.php)

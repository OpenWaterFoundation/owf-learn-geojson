# GeoJSON Specification / File Size

GeoJSON files are text and can be comparatively larger than alternative formats.

This documetantation contains the following sections describing how to decrease file size:

* [Limit Digits in Geometry Coordinates](#limit-digits-in-geometry-coordinates)
* [Don't use Pretty Formatting](#dont-use-pretty-formatting)
* [Simplify Geometry](#simplify-geometry)
* [Compress the File](#compress-the-file)

## Limit Digits in Geometry Coordinates

GeoJSON files are often created by software that outputs a large number of digits.
This can greatly increase the size of the files, which can be problematic for large data sets,
especially when using with web mapping tools such as Leaflet.
And, such high precision does not correspond to actual measured precision.
The following resources explain coordinate precision:

* [Decimal Degrees on Wikipedia](https://en.wikipedia.org/wiki/Decimal_degrees)

The precision used when maintaining the original dataset should be considered based on the use of the dataset.
However, for many practical uses in GeoJSON files,
5 digits (~1 m precision at equator) or perhaps 6 digits (~.1 m precision at equator) is adequate.

## Don't use Pretty Formatting

GeoJSON is a specific version of JSON and 
the files can be formatted for machines (no formatting) or for humans ("pretty" formatting).
Pretty formatting introduces spaces and end of line characters that increase the file size.
If it is unlikely that humans need to read the files, don't use pretty formatting when generating the files.
Most GeoJSON software tools have options to control the output formatting.

**TODO smalers add resource links here to reformat machine version with formatted version.**

## Simplify Geometry

**TODO smalers 2017-01-07 need to discuss tools to simplify geometry by removing intervening points, etc.**

## Compress the File

Because GeoJSON files typically contain repeated text patterns, the files often will significantly compress.

**TODO smalers 2017-01-17 need to evaluate how this can be done to work with various software,
file extensions, web content, desktop GIS, etc..**

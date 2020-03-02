# GeoJSON Specification / File Size #

GeoJSON files are text and can be comparatively larger than alternative formats.

The remainder of this page contains the following sections describing how to decrease file size:

* [Limit Digits in Geometry Coordinates](#limit-digits-in-geometry-coordinates)
* [Don't use Pretty Formatting](#dont-use-pretty-formatting)
* [Simplify Geometry](#simplify-geometry)
* [Compress the File](#compress-the-file)

-----------------

## Limit Digits in Geometry Coordinates ##

GeoJSON files are often created by software that by default outputs a large number of digits in coordinates.
This can greatly increase the size of the files, which can be problematic for large data sets,
especially when using the GeoJSON file with web mapping tools.
A large number of digits also does not correspond to actual measured precision,
but is often an artifact of how the number is stored in software.
The following resources explain coordinate precision:

* [Decimal Degrees on Wikipedia](https://en.wikipedia.org/wiki/Decimal_degrees)

The precision used when maintaining the original dataset should be considered based on the use of the dataset.
However, for many practical uses in GeoJSON files,
5 digits (~1 m precision at equator) or perhaps 6 digits (~.1 m precision at equator) is adequate.
The data may not actually have this precision, in which case trailing digits may be zeros.

## Don't use Pretty Formatting ##

GeoJSON is a specific version of JSON and 
the files can be formatted for machines (no formatting) or for humans ("pretty" formatting).
Pretty formatting introduces spaces and end of line characters that increase the file size.
If it is unlikely that humans need to read the files, don't use pretty formatting when generating the files.
Most GeoJSON software tools have options to control the output formatting.

Online and command line tools are available to pretty print JSON, if necessary.

## Simplify Geometry ##

File size can be reduced by simplifying geometry, for example to remove redundant or nearby points.
GIS tools are available.  Simplification should ensure that the original data resolution is not
modified in a way that significantly alters the data or renders it inaccurate for the required use.

## Compress the File ##

Because GeoJSON files typically contain repeated text patterns, the files often will significantly compress.
Compression can be used if consuming applications know how to uncompress the files.

# GeoJSON Specification / Overview #

The GeoJSON file format is a specific JSON schema and includes geometry and properties for spatial data features.
Benefits of GeoJSON include:

* Single file, conducive to use with web services, static websites, and distributing datasets for visualization.
* Text file, so easy to view, create, parse, and manage in a version control system.
* No limits on feature attribute names (unlike Esri shapefiles)

Limitations of GeoJSON include:

* Can result in large file size, for example because property names are repeated for each feature.
* Specification does not explicitly define how to represent metadata and some geographic information system
concepts such as symbolization.
* Because the file format is free-format text, it is more difficult for software to access in asynchronous fashion by
jumping around the file.
* Because the file is JSON, comments are not allowed, unless included as data.
* Support for special values such as `null`, `NaN`, and date/times vary.
* Format specification for metadata is lacking.

See the following resources:

* [JSON specification](http://www.json.org)
* [GeoJSON.org](http://geojson.org/)
* [GeoJSON 2016 RFC 7964 specification](https://tools.ietf.org/html/rfc7946) - latest specification = **use this**
* [GeoJSON 2008 specification](http://geojson.org/geojson-spec.html) - original specification - **avoid if possible**

The following topics are covered in separate pages:

* [Comments](comments.md) - they are not directly supported by JSON, so how to implement?
* [Version](version.md) - options for indicating version
* [Metadata](metadata.md) - options for metadata
* [File Size](file-size.md) - tips for reducing file size
* [Alternatives](alternatives.md) - alternatives to GeoJSON

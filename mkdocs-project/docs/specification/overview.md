# GeoJSON Specification / Overview

The GeoJSON file format is a specific JSON schema and includes geometry and properties for spatial data features.
Benefits of GeoJSON include:

* Single file, conducive to use with web services, static websites, and distributing datasets for visualization.
* Text file, so easy to view, create, and parse.

Limitations of GeoJSON include:

* Can result in large file size, for example because property names are repeated for each feature.
* Specification does not explicitly define how to represent metadata and some geographic information system
concepts such as symbolization.
* Because the file format is free-format text, it is more difficult for software to access in asynchronous fashion by
jumping around the file.

See the following resources:

* [JSON specification](http://www.json.org)
* [GeoJSON.org](http://geojson.org/)
* [GeoJSON 2008 specification](http://geojson.org/geojson-spec.html) - current version
* [GeoJSON 2016 RFC 7964 specification](https://tools.ietf.org/html/rfc7946) - new recommendation

The following topics are covered in separate pages:

* [Comments](comments) - they are not directly supported by JSON, so how do implement?
* [Version](version) - suggestion for foreign properties for version
* [Metadata](metadata) - suggestion for foreign properties for metadata
* [File Size](file-size) - tips for reducing file size
* [Alternatives](alternatives) - alternatives to GeoJSON


# owf-learn-geojson #

This repository contains the [Open Water Foundation (OWF)](http://openwaterfoundation.org/) GeoJSON training materials,
which provides guidance for using GeoJSON open spatial data format.
The documentation is written for the layperson in order to encourage use of GeoJSON.

See the deployed [OWF / Learn GeoJSON](http://learn.openwaterfoundation.org/owf-learn-geojson/) documentation.

## Repository Contents ##

The repository contains the following:

```text
.github/              (Files specific to GitHub such as issue template)
.gitattributes        (Typicaly Git configuration file)
.gitignore            (Typicaly Git configuration file)
README.md             (This file)
build-util/           (Useful scripts to view, build, and deploy documentation)
mkdocs-project/       (Typical MkDocs project for this documentation)
  mkdocs.yml          (MkDocs configuration file for website)
  docs/               (Folder containing source Markdown and other files for website)
  site/               (Folder created by MkDocs containing the static website - ignored using .gitignore)

```

## Development Environment ##

The development environment for contributing to this project requires installation of Python, MkDocs, and Material MkDocs theme.
Python 2 has been used for development.  See the [OWF / Learn MkDocs](http://learn.openwaterfoundation.org/owf-learn-mkdocs/)
documentation for more information about MkDocs.

## License ##

The OWF Learn MkDocs website content and examples are licensed under the
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0).

## Contributing ##

Contribute to the documentation as follows:

1. Use GitHub repository issues to report minor issues.
2. Use GitHub pull requests.

## Maintainers ##

This repository is maintained by the [Open Water Foundation]((http://openwaterfoundation.org/).

## Contributors ##

Steve Malers, Open Water Foundation (@smalers)

## Release Notes ##

The following release notes indicate the update history for documentation, with GitHub repository issue indicated,
if applicable (links to issues via README.md are not cleanly supported by GitHub so use the repository issues page to find).

* 2017-10-21 [1] - switch to Material theme, update documentation based on experience.
* 2017-01-18 - initial version.

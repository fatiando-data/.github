# Guidelines and information about this project

This organization houses the curated collection of 
[FAIR data](https://www.go-fair.org/fair-principles/)
that is used in the [Fatiando a Terra](https://www.fatiando.org)
project (in tutorials and documentation).

Each repository here contains Python code to download,
preprocess, and repackage Geophysical data that is available
under permissive open licenses.
The curated data are then published as GitHub release artifacts
and on our [Zenodo community](https://zenodo.org/communities/fatiando/).

These datasets can be downloaded with [Pooch](https://github.com/fatiando/pooch)
and are the data source for the [Ensaio](https://github.com/fatiando/ensaio)
package.

## Versioning

Datasets in this collection use only a single number to denote their versions.
This is because any change to data/metadata can lead to code that relies on 
them breaking, so [semantic versioning](https://semver.org/) wouldn't make
sense. 
New releases are made when data/metadata are changed, added, or deleted.

Each data release is also assigned a unique DOI on Zenodo.

> We recommend pinning (specifying explicitly) the version of each dataset
> in your tutorial or documentation to guarantee that the same version
> is always used.

## Contributing

See our [Contributing Guidelines](CONTRIBUTING.md) for information on
proposing new datasets and making changes to existing ones.

## This repository

The `.github` repository contains configuration for GitHub 
and templates for issues and pull requests. 
Contents of this repository get shared between other repositories 
so we only have to update them in a single place.

## License

[Creative Commons Attribution 4.0 International](LICENSE.md)

<h1 align="center">👋 Welcome to the Fatiando a Terra FAIR data collection</h1>

![Banner showing small sections of some of the datasets present in the collection](https://github.com/fatiando-data/.github/raw/main/profile/readme-banner.jpg)

This organization houses the curated collection of 
[FAIR data](https://www.go-fair.org/fair-principles/)
that is used in the [Fatiando a Terra](https://github.com/fatiando)
project tutorials and documentation.

Each repository here contains Python code to download,
preprocess, and repackage geophysical data that is available
under permissive open licenses or in the public domain.
The curated data are then published as GitHub release artifacts
and on our [Zenodo community](https://zenodo.org/communities/fatiando/).

---

<div align="center">

⚡
[**Propose a new dataset**](https://github.com/fatiando-data/.github/issues/new) 
|
[**Contributing Guidelines**](https://github.com/fatiando-data/.github/blob/main/CONTRIBUTING.md) 
|
[**Code of Conduct**](https://github.com/fatiando-data/.github/blob/main/CODE_OF_CONDUCT.md)
⚡

</div>

---

<h2 align="center">Downloading the data</h2>

These datasets are the source for the [Ensaio](https://github.com/fatiando/ensaio)
package and can be easily downloaded with [Pooch](https://github.com/fatiando/pooch):

```python
import pooch
import pandas as pd

fname = pooch.retrieve(
    url="doi:10.5281/zenodo.5882430/southern-africa-gravity.csv.xz",
    known_hash="md5:1dee324a14e647855366d6eb01a1ef35",
)
data = pd.read_csv(fname)
```

You'll find the DOI, file name, and MD5 hash of each dataset in their 
respective repository.

<h2 align="center">Versioning</h2>

Datasets in this collection **use only a single number to denote their versions**.
This is because any change to data/metadata can lead to code that relies on 
them breaking, so [semantic versioning](https://semver.org/) wouldn't make
sense. 
New releases are made when data/metadata are changed, added, or deleted.
Each data release is also assigned a unique DOI on Zenodo.

> **We recommend pinning** (specifying explicitly) the version of each dataset
> in your tutorial or documentation to guarantee that the same version
> is always used.

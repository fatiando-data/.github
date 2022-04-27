---
name: Release checklist
about: 'Maintainers only: Checklist for making a new release'
title: 'Release vX'
labels: 'maintenance'
assignees: ''

---
Checklist:

- [ ] Reserve a DOI on Zenodo and save the entry (fill required information first).
- [ ] Update the DOI in the README
- [ ] Update the release number, file size, and checksums in the README
- [ ] Update the list of changes in the README
- [ ] Fill out the Zenodo metadata and description following the example other Fatiando Data publications and latest changes from the README
- [ ] Create a new release (use the template below). The release name should be the version number with a leading `v` (e.g. `v1`).
- [ ] Upload the new data file to the release
- [ ] Publish the release
- [ ] Upload the new data file to Zenodo
- [ ] Publish the Zenodo archive

GitHub release template:

```markdown
**Date:** YYYY/MM/DD

**DOI:** https://doi.org/XXXX

**Note:** This is a processed and formatted version of the source dataset below. It's mean for use in documentation and tutorials of the Fatiando a Terra project. Please cite the original authors when using this dataset.

**Data source:** [The reference](Link to the reference, preferably a DOI)

**Changes:**

* List of changes made to the data

| | Checksums |
|--:|:--|
| MD5 | `md5:XXX` |
| SHA256 | `sha256:XXX` |
```

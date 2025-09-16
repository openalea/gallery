# Installation

You must use conda environment : <https://docs.conda.io/en/latest/index.html>

## Users

### Create a new environment with gallery installed in there

```bash

mamba create -n gallery -c openalea3 -c conda-forge  openalea.gallery
mamba activate gallery
```

Install gallery in a existing environment

```bash
mamba install -c openalea3 -c conda-forge openalea.gallery
```

### (Optional) Test your installation

```bash
mamba install -c conda-forge pytest
git clone https://github.com/openalea/gallery.git
cd gallery/test; pytest
```

## Developers

### Install From source

```bash
# Install dependency with conda
mamba env create -n phm -f conda/environment.yml
mamba activate gallery

# Clone gallery and install
git clone https://github.com/openalea/gallery.git
cd gallery
pip install .

# (Optional) Test your installation
cd test; pytest
```

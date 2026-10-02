# OpenAlea notebooks for FSPM conference, October 2026, Montpellier

This repo contains a serie of notebooks chosen to illustrate some features of the OpenAlea plateform.

It is meant to be functional with OpenAlea release 3.0.0.

## Installation

To install the notebooks from this repository, simply clone it:

```bash
git clone
cd FSPM_2026
```

You then have 2 options to install OpenAlea

### Local Installation

OpenAlea packages are distributed via conda-packages. Once you have [installed conda or mamba](https://mamba.readthedocs.io/en/latest/installation/mamba-installation.html), you can thus install OpenAlea meta package (that includes all packages from release 3.0.0) by:

```bash
mamba install -n openalea -c openalea3 -c conda-forge openalea jupyterlab
mamba activate openalea
jupyter lab
```

### Using Docker (recommanded for the demo)

This approach is recommended to avoid installation step and load pre-installed docker image:

```bash
docker run -it --rm --volume $PWD:$HOME -p 8888:8888 openalea/fullstack-openalea:3.0.0 jupyter lab --ip 0.0.0.0 $HOME
```

## Contributions from OpenAlea developpers

To include your notebooks into this repo:

- clone this repo: `git clone`
- go into the directory: `cd  FSPM_2026`
- create your directory with your notebook + associated data:

```bash
openalea.mypackage/mynotebook.ipynb
openalea.mypackage/data/mydata.mtg
```

- update file `index.ipynb` with a link to your notebook + additional information if you feel like it.
- create a pull request on github repo

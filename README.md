# The FF library written by Geert Jan van Oldenborgh

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.14542887.svg)](https://doi.org/10.5281/zenodo.14542887)

## Installing

### From source

Building from source requires `make` and a Fortran compiler (assumed to be set in your environment to `FC`).
To build from source and install the library under `<install target path>` run

```
cd src/ff
make install FC=$FC FFLAGS="$FFLAGS -std=legacy -ffixed-line-length-none" DEST=<install target path>/lib --jobs
```

### From conda-forge

FF is packaged and distributed on [conda-forge](https://github.com/conda-forge/ff-feedstock/) for the following platforms:

[![Conda Version](https://img.shields.io/conda/vn/conda-forge/ff-static.svg)](https://anaconda.org/conda-forge/ff-static)
[![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/ff-static.svg)](https://anaconda.org/conda-forge/ff-static)

To install and add `ff-static` to a project with [`pixi`](https://pixi.sh/), from the project directory run

```
pixi add ff-static
```

and to install into a particular conda environment with [`conda`](https://docs.conda.io/projects/conda/), in the activated environment run

```
conda install --channel conda-forge ff-static
```

## Citation

Please cite FF if used in your work by citing the following paper:

"[New Algorithms For One Loop Integrals](https://inspirehep.net/literature/282949)."
G.J. van Oldenborgh, J.A.M. Vermaseren (NIKHEF, Amsterdam).
Published in Z.Phys.C46:425-438,1990.

The preferred BibTeX entry for citation of FF is

```
@article{vanOldenborgh:1989wn,
    author = "van Oldenborgh, G. J. and Vermaseren, J. A. M.",
    title = "{New Algorithms for One Loop Integrals}",
    reportNumber = "NIKHEF-H/89-17",
    doi = "10.1007/BF01621031",
    journal = "Z. Phys. C",
    volume = "46",
    pages = "425--438",
    year = "1990"
}
```

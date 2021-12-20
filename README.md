# Mock SZ Maps with Halo-based and Particle-based Baryon Pasting Algorithms

[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)


## Overview

This suite is composed of mock tSZ and kSZ maps generated from dark-matter only N-body simulations.
There are 108 realisations for all-sky (halo-based pasting) and flat-sky (particle-based pasting) coverage.


## Codes
We provide jupyter notebook to load the map data (`load_map.ipynb`).


## Data sets
The full data sets are found in shared Google Drive site.


## Data format
### All-sky maps
The file format is healpix.
The specifications of the maps are as follows:

* Nside: 8192
* pixel area: 0.184 arcmin^2


### Flat-sky maps
The file format is hdf5. The tSZ and kSZ maps are defined in regular grids.
The specifications of the maps are as follows:

* number of grids: 4096x4096
* angular size on a side: 5 deg
* resolution: 4.39 arcsec/pixel


## Attribution
We kindly ask those who use this suite to cite the paper:
[Osato and Nagai (2021)](https://ui.adsabs.harvard.edu).
The bibtex entry of the paper is:
```
[TBA]
```

## Copyright
Copyright 2021 Ken Osato and Daisuke Nagai

This software is made available under MIT License. Please see `LICENSE` file for details.

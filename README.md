# Mock SZ Maps with Halo-based and Particle-based Baryon Pasting Algorithms

[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)


## Overview

This suite is composed of mock tSZ and kSZ maps generated from dark-matter only N-body simulations
with baryon pasting algorithms.
There are 108 realisations for all-sky (halo-based pasting) and flat-sky (particle-based pasting) coverage.


## Codes
We provide jupyter notebook to load the map data (`load_allsky_HP_map.ipynb` and `load_flatsky_PP_map.ipynb`).


## Data sets
The full data sets are found in [Google Drive site](https://drive.google.com/drive/folders/1NNwnzYXe2vvvCOlqjedXoKmhAUjCJPYW?usp=sharing).


## Data format
### All-sky maps with halo-based pasting
The file format is healpix.
The file name is `allsky_HP_tSZ_nres13_r[real].fits` for the tSZ map
and `allsky_HP_kSZ_nres13_r[real].fits` for the kSZ map.
`[real]` denotes the realisation (000-107).
The corresponding halo catalogues are described in
[Takahashi et al. (2017)](http://cosmo.phys.hirosaki-u.ac.jp/takahasi/allsky_raytracing/nres13.html)
and data are found in [this site](http://cosmo.phys.hirosaki-u.ac.jp/takahasi/allsky_raytracing/nres13.html).

The specifications of the maps are as follows:

* Nside: 8192
* pixel area: 0.184 arcmin^2


### Flat-sky maps with particle-based pasting
The file format is hdf5.
The file name is `flatsky_PP_tSZ_r[real].fits` for the tSZ map
and `flatsky_PP_kSZ_r[real].fits` for the kSZ map.
`[real]` denotes the realisation (000-107).
We also provide "halo" and "field" separated kSZ maps:
`flatsky_PP_kSZ_halo_r[real].fits` for halo-particles only maps and
`flatsky_PP_kSZ_field_r[real].fits` for field-particles only maps.
The tSZ and kSZ maps are defined in regular grids.

The specifications of the maps are as follows:

* number of grids: 4096x4096
* angular size on a side: 5 deg
* resolution: 4.39 arcsec/pixel


## Attribution
We kindly ask those who use this suite to cite the paper:
[Osato and Nagai (2021)](https://ui.adsabs.harvard.edu).
The bibtex entry of the paper:
```
[TBA]
```

## Copyright
Copyright 2021 Ken Osato and Daisuke Nagai

This software is made available under MIT License. Please see `LICENSE` file for details.

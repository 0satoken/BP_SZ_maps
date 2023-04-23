# Mock SZ Maps with Halo-based and Particle-based Baryon Pasting

[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
[![arXiv](https://img.shields.io/badge/arXiv-2201.02632-b31b1b.svg)](https://arxiv.org/abs/2201.02632)

## Overview

This suite is composed of mock tSZ and kSZ maps generated from dark-matter only N-body simulations
with baryon pasting algorithms developed in
[Osato and Nagai (2022)](https://ui.adsabs.harvard.edu/abs/2022arXiv220102632O/abstract).
There are 108 realisations for all-sky (halo-based pasting) and flat-sky (particle-based pasting) coverage.


## Codes
We provide jupyter notebook to load the map data (`load_allsky_HP_map.ipynb` and `load_flatsky_PP_map.ipynb`).
[healpy](https://github.com/healpy/healpy) and [h5py](https://github.com/h5py/h5py)
are required for loading healpix and HDF5 maps, respectively.


## Data sets
The full data sets are found in [Google Drive site](https://drive.google.com/drive/folders/1NNwnzYXe2vvvCOlqjedXoKmhAUjCJPYW?usp=sharing).


## Data format
### All-sky maps with halo-based pasting
The file format is healpix.
The file name is `allsky_HP_tSZ_nres13_r[real].fits` for the tSZ map
and `allsky_HP_kSZ_nres13_r[real].fits` for the kSZ map.
`[real]` denotes the realisation (000-107).
The corresponding halo catalogues are described in
[Takahashi et al. (2017)](https://ui.adsabs.harvard.edu/abs/2017ApJ...850...24T/abstract)
and data are found in [this site](http://cosmo.phys.hirosaki-u.ac.jp/takahasi/allsky_raytracing/nres13.html).

The specifications of the maps are as follows:

* Nside: 8192
* pixel area: 0.184 arcmin^2


### Flat-sky maps with particle-based pasting
The file format is hdf5. The maps are pixellated in regular grids.
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
[Osato and Nagai (2023)](https://ui.adsabs.harvard.edu/abs/2023MNRAS.519.2069O/abstract).
The bibtex entry of the paper:
```
@ARTICLE{2023MNRAS.519.2069O,
       author = {{Osato}, Ken and {Nagai}, Daisuke},
        title = "{Baryon pasting algorithm: halo-based and particle-based pasting methods}",
      journal = {\mnras},
     keywords = {methods: numerical, galaxies: clusters: intracluster medium, large-scale structure of Universe, Astrophysics - Cosmology and Nongalactic Astrophysics},
         year = 2023,
        month = feb,
       volume = {519},
       number = {2},
        pages = {2069-2082},
          doi = {10.1093/mnras/stac3669},
archivePrefix = {arXiv},
       eprint = {2201.02632},
 primaryClass = {astro-ph.CO},
       adsurl = {https://ui.adsabs.harvard.edu/abs/2023MNRAS.519.2069O},
      adsnote = {Provided by the SAO/NASA Astrophysics Data System}
}
```

## Copyright
Copyright 2023 Ken Osato and Daisuke Nagai

This software is made available under MIT License. Please see `LICENSE` file for details.

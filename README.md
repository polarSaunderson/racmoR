# racmoR

**PRIVATE BRANCH OF THE pkg06_racmoR PACKAGE**

## Overview
racmoR is a personal package for interacting with and manipulating output from the RACMO regional climate model.
The package is an ongoing work in progress, is not foolproof, and is essentially a lot of syntactic wrapping around the [terra](https://rspatial.org) package to ease repeated processes.

It is necessary to separately download the RACMO data. 
The RACMO2.3p3 data that this package was initially created to handle can be accessed online at [https://doi.org/10.5281/zenodo.7639053] and was created by Christiaan van Dalum at IMAU, Utrecht University.

## Public Version
The public version of this repo can be accessed at: 
  https://github.com/polarSaunderson/racmoR

## To-Do
### 2023-08-04
- [ ] The logic of get_shelf_outline and get_basin_outline need correcting
 - [ ] They look only in their own dataset; need to look through all extents, then reduce to shelves
 - [ ] Will impact draw_antarctica(), and crop_racmo() functions;
 - [ ] check get_extent is not doing something wrong with this

### 2023-08-03 
- [ ] get_extent uses %notIn%
- [ ] think about projection order in get_coastlines()
- [ ] update examples for get_extent based on imbieBasins argument
- [X] create crop_racmo functions
- [ ] draw_antarctica and draw_racmo_axes functions
- [ ] calculate_racmoX functions
- [ ] create_racmoX_NetCDFs

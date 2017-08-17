# iri_cpt

This repository hosts a docker image that runs IRI's [Climate Predictability Tool](http://iri.columbia.edu/~awr/wiki/Downscaling/HydroOutlooks/Documents/cpttutorial_june08.html#d4e752).
Specifically, it runs the CPT version 15.5.12.

This is a new tool.
Although the CPT opens successfully, there are still some to-dos with this `Dockerfile` and any help is appreciated:
- reduce the install burden so that a lighter setup is used; the current iteration installs Ubuntu and the `build-essentials` but only `wget`, `make`, and `gfortran` are required
- copy the installed `CPT.x` and `cpt.ini` to `/bin/` (?)
- better cleanup

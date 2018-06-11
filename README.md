# singularity-mrtrix3
[![https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg](https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg)](https://singularity-hub.org/collections/729)

Singularity recipes for base-images containing mrtrix3.

 - mrtrix3 is pulled from its [github repository](https://github.com/MRtrix3/mrtrix3) and build using cmake.
 - cmake and the build dependencies are installed through the debian repositories via `apt-get install`.
 - At the end of the build process the image is cleaned up by:
    - removing cmake and build dependencies through `apt-get purge`,
    - deleting the package cache.

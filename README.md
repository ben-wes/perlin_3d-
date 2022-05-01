# perlin.3d~
3D perlin noise for Pure Data (Pd) - signal rate input/output

Install by adding a folder `perlin.3d~` with these files to one of pd's paths.
The abstraction `perlin.3d~` expects the arguments:
* number of octaves
* persistance value
* (optional) `normalize` flag if you want to ensure that the sum of all octaves will not exceed 1

Explanations on Perlin noise (and also the tutorial that this abstraction is based on):
* https://rtouti.github.io/graphics/perlin-noise-algorithm

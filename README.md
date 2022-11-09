# perlin.3d~
3D Perlin noise abstraction for Pure Data (Pd) with signal rate input/output (based on Perlin's improved version - see https://cs.nyu.edu/~perlin/noise/)

## Installation
Install by adding the downloaded folder as `perlin.3d~/` to Pd's path (e.g. in `externals` directory).

## Usage
The abstraction `perlin.3d~` requires the number of octaves as its first argument (it will default to 1 - but produce a clone error message).

Additional optional arguments:
* `normalize` flag to ensure that the sum of all octaves will not exceed 1.
* `-persistence` parameter to set persistence (values < 1 will attenuate higher octaves, values > 1 will amplify them).
* `-seed` parameter to initialize the gradient vector permutation with a given seed value. Without a value, the permutation gets reseeded randomly.
* `-offset` parameter to set initial offset for x, y and z coordinates (useful if only one axis is used for input since values along 0-coordinates create a less noisy pattern).

Inlets are:
1. x-coordinate
2. y-coordinate
3. z-coordinate
4. persistence

*See help patch for more explanations and examples*

Explanations on Perlin noise:
* https://en.wikipedia.org/wiki/Perlin_noise

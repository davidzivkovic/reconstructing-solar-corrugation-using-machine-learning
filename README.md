# Reconstructing Solar corrugation using machine learning

Here we use fits cubes obtained from MuRAM simulation of Solar atmosphere that have a shape of (9, 1536, 1536, 35). 8 physical parameters and 1 z(tau) map, 1536x1536 spatial resolution and 35 iso-z layers. The goal is to train a network on physical parameters (8, 1536, 1536, 35) to predict the z(tau) map on (1, 1536, 1536, 3), for our example we target 3 iso-z layers (0, 96, 192) km.

In this directory we have different notebooks based on used inputs.

- Notebooks are named **`cnn-iso-z-{type of patch creation}-{physical parms. used for training}.ipynb`**, e.g. `cnn-iso-z-random-tpv.ipynb`
> v implies we used vx, vy and vz. Same counts for B.


## Results
### Input T, p, vx, vy, vz

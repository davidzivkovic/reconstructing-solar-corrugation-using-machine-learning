# Reconstructing Solar Corrugation Using Machine Learning

## Data

We use FITS cubes obtained from MuRAM simulation of Solar atmosphere with shape:

| Dimension | Size | Description |
|-----------|------|-------------|
| Channels | 9 | 8 physical parameters + 1 z(tau) map |
| Spatial | 1536 × 1536 | Spatial resolution |
| Depth | 35 | Iso-z layers |

## Task

The goal is to train a network on physical parameters `(8, 1536, 1536, 35)` to predict the z(tau) map `(1, 1536, 1536, 3)`.

For our example we target 3 iso-z layers: **0, 96, 192 km**.

In this directory we have different notebooks based on used inputs.

- Notebooks are named **`cnn-iso-z-{type of patch creation}-{physical parms. used for training}.ipynb`**, e.g. `cnn-iso-z-random-tpv.ipynb`

> `v` implies we used `vx`, `vy` and `vz`. Same counts for `B`.

## Results

### Input T, p, vx, vy, vz

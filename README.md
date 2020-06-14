![tent](img/tent.gif)
# cmlnn
Learning to use spatiotemporal chaos

## Basic idea
Coupled map lattices (CMLs) exhibit robust nonlinear functional capacity with few parameters. As such they might prove a useful computational tool for deep neural networks. Currently this is just a first-pass notebook.

### Errata
- This is in Keras but must move to PyTorch:
  - I need layerwise learning rates so that dynamics can be learned slower than initialization, which Keras doesn't yet support
- Learning requires a slight modification of CML update:
  - the lattice boundaries must update independently instead of referencing neighbors.
    - visually, dynamics seem unaffected by this, but should validate further

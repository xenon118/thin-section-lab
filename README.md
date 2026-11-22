# Thin Section Lab

Version 1.0.0

An interactive viewer that builds a 3D cube of a sandstone from thin-section measurements and estimates its permeability with a Kozeny-Carman relation that includes the mud fraction.

**Open the viewer:** https://xenon118.github.io/thin-section-lab/

## How to use it

Open the link above, or download `index.html` and open it in a web browser. Nothing is installed, and no image or number leaves the computer: everything runs inside the browser.

- Load a thin-section image (blue-epoxy impregnated), or set the grain size, grain share and matrix by hand.
- Enter the measured porosity and the mud content (silt plus clay). Potassium and thorium can be entered instead of the mud content.
- The viewer builds the cube and reports the permeability with its typical error.

## What the numbers mean

The relation has one calibrated parameter, the effective particle size of the mud. It was calibrated and tested on 10 core plugs (permeability 0.23 to 396 mD, mud content 8 to 32 %). The typical error is the ratio between predicted and measured permeability over all ways of dividing the plugs into calibration and test:

| Inputs | Particle size of the mud (µm) | Typical error (factor) |
|---|---|---|
| Porosity and mud content measured | 5.92 | 2.3 |
| Porosity measured, mud content from K and Th | 3.91 | 3.4 |
| Porosity from the image, mud content from K and Th | 4.07 | 4.4 |

A loaded image is read with a quick colour method, which does not recognise grain borders. For the stated error, enter the grain size measured on the thin section.

The cube is a representation of the measurements. It is not a flow simulation: permeability comes from the relation.

## Authors

- Muhammad Risha, Texas Tech University
- Esraa Shokair, Wake Tech Community College

## How to cite

Risha, M., & Shokair, E. (2026). Thin Section Lab (Version 1.0.0) [Software]. https://github.com/xenon118/thin-section-lab

## Licence

Copyright (c) 2026 Muhammad Risha and Esraa Shokair.

Thin Section Lab is shared under the Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International licence (CC BY-NC-ND 4.0): https://creativecommons.org/licenses/by-nc-nd/4.0/

The viewer may be used and shared unchanged, with credit to the authors. It may not be used commercially, and modified versions may not be distributed.

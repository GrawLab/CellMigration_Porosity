# CellMigration_Porosity

## A cellular Potts model to simulate cell migration in porous environments ##

The provided code allows the simulation of cell migration within disordered porous environments by accounting for cell shape dynamics using the cellular Potts modelling framework. It relates to the following publication with details on the model structure and implementation:
* Würthner L., Graw F.: **Cell migration in porous environments**

## Description
The model allows simulation of cell migration within complex, porous environments and is implemented as a cellular Potts model (CPM) using Morpheus. It especially accounts for cell body deformation to capture effects of cell confinement within the porous structures, with cell motility being modelled by active Brownian motion. The model can be readily applied to various porous environments, with environments being easily interchangeable using synthetic or experimentally generated 3D tiff-images.

## Implementation & Requirements
The model is implemented within the powerful cellular Potts modelling framework Morpheus (https://morpheus.gitlab.io/), using Morpheus version 2.3.8. The xml-file of the model contains the basic code for cellular motility and active Brownian motion dynamics. Porous environments are integrated within the simulation framework as individual tiff-images. This can be synthetically generated structures, as e.g. by using the open-source python library PoreSpy, or experimentally obtained images. One example environment is provided within this repository.

# PlantSeg

PlantSeg is a deep learning-based tool specifically designed for cell segmentation in plant tissues, addressing the unique challenges of plant cell structure and morphology.

## Overview

PlantSeg combines deep learning-based boundary prediction with graph partitioning algorithms to achieve accurate cell segmentation in complex 3D plant tissues.

## Environment

**Environment**: `plantseg`

## Available Tasks

### Start PlantSeg GUI
Launch the PlantSeg graphical user interface:
```bash
pixi run plantseg-gui
```

## Features

- **Deep learning segmentation**: State-of-the-art neural networks trained on plant tissues
- **3D cell segmentation**: Specialized for volumetric plant imaging data
- **Pre-trained models**: Multiple models trained on different plant tissues and organs
- **Graph partitioning**: Advanced algorithms for separating touching cells
- **Batch processing**: Process multiple datasets efficiently
- **Custom training**: Ability to train models on your own plant data
- **Multi-scale analysis**: Handle images at different resolutions

## Supported Plant Tissues

- **Root tissues**: Specialized models for root cell segmentation
- **Leaf tissues**: Models optimized for leaf cellular structure
- **Shoot apical meristems**: Segmentation of meristematic tissues
- **Ovules**: Specialized for reproductive tissue analysis
- **General plant tissues**: Multi-purpose models for various plant organs

## Workflow Steps

1. **Image preprocessing**: Prepare your 3D microscopy data
2. **Boundary prediction**: Use neural networks to predict cell boundaries
3. **Segmentation**: Apply graph partitioning to separate individual cells
4. **Post-processing**: Refine segmentation results
5. **Analysis**: Extract quantitative measurements from segmented cells

## Getting Started

1. Make sure you have pixi installed and this repository cloned
2. Navigate to the repository directory
3. Run `pixi run plantseg-gui` to start the PlantSeg interface
4. Load your 3D plant imaging data and select appropriate models
5. Run the segmentation pipeline and analyze your results!

## Input Requirements

- **3D image stacks**: Confocal or light-sheet microscopy data
- **Supported formats**: TIFF, H5, various microscopy formats
- **Cell wall staining**: Images with clear cell boundary visualization
- **Resolution**: Isotropic or near-isotropic voxel spacing recommended

## Use Cases

- **Developmental biology**: Track cell divisions and growth in developing organs
- **Cell morphometry**: Quantify cell shape, size, and volume
- **Tissue architecture**: Analyze 3D tissue organization and structure
- **Comparative studies**: Compare cellular organization across different conditions
- **Growth analysis**: Study cell expansion and tissue growth patterns

## Resources

- [PlantSeg documentation](https://plantseg.readthedocs.io/)
- [PlantSeg paper](https://elifesciences.org/articles/57613)
- [PlantSeg GitHub repository](https://github.com/PlantSeg/PlantSeg)
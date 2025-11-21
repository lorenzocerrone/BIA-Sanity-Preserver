# Cellpose

Cellpose is a generalist algorithm for cellular segmentation that works well on diverse cell types and images without the need for model retraining or parameter adjustment.

## Overview

The Cellpose environment provides tools for 2D and 3D cell segmentation using deep learning models trained on a diverse dataset of cell images.

## Environment

**Environment**: `cellpose`

## Available Tasks

### Cellpose 2D GUI
Start the Cellpose graphical interface for 2D segmentation:
```bash
pixi run cellpose
```

### Cellpose 3D GUI
Start the Cellpose graphical interface for 3D segmentation:
```bash
pixi run cellpose-3D
```

## Features

- **2D and 3D segmentation**: Supports both 2D and 3D cell segmentation
- **Pre-trained models**: Includes several pre-trained models for different cell types
- **Custom training**: Ability to train custom models on your own data
- **GPU acceleration**: Supports GPU acceleration for faster processing
- **User-friendly GUI**: Easy-to-use graphical interface for interactive segmentation

## Getting Started

1. Make sure you have pixi installed and this repository cloned
2. Navigate to the repository directory
3. Run one of the available tasks above to start Cellpose
4. Load your images and start segmenting!

## Resources

- [Cellpose official documentation](https://cellpose.readthedocs.io/)
- [Cellpose paper](https://www.nature.com/articles/s41592-020-01018-x)
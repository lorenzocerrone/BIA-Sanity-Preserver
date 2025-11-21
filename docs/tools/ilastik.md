# ilastik

ilastik is an interactive machine learning toolkit that enables users to classify pixels, segment images, track objects, and count cells without requiring machine learning expertise.

## Overview

The ilastik environment provides a user-friendly interface for interactive machine learning-based image analysis, making advanced segmentation and classification accessible to biologists and researchers.

## Environment

**Environment**: `ilastik`

## Available Tasks

### Start ilastik GUI
Launch the ilastik graphical user interface:
```bash
pixi run ilastik
```

## Features

- **Interactive machine learning**: Train classifiers by providing examples
- **Pixel classification**: Classify pixels based on their local appearance
- **Object classification**: Classify segmented objects based on their features
- **Carving workflow**: Semi-automatic segmentation for challenging objects
- **Tracking**: Track objects across time-lapse sequences
- **Counting**: Automated object counting in images
- **Batch processing**: Process multiple images with trained classifiers
- **Feature extraction**: Comprehensive set of image features for analysis

## Workflows Available

### Pixel Classification
Train a classifier to distinguish different tissue types, cell types, or structures at the pixel level.

### Object Classification
Segment objects first, then classify them based on shape, intensity, and other features.

### Autocontext
Improve classification results by using predictions as additional input features.

### Carving
Interactive segmentation tool for separating touching or overlapping objects.

### Tracking
Track objects through time-lapse sequences with manual correction capabilities.

### Counting
Count objects in images using density estimation or detection-based approaches.

## Getting Started

1. Make sure you have pixi installed and this repository cloned
2. Navigate to the repository directory
3. Run `pixi run ilastik` to start the ilastik interface
4. Choose your desired workflow and start training your classifier!

## Use Cases

- **Cell segmentation**: Separate cells from background and from each other
- **Tissue classification**: Classify different tissue types in histological images
- **Organelle detection**: Identify and classify cellular organelles
- **Quality control**: Classify images based on quality metrics
- **Time-lapse analysis**: Track cell division, migration, and other dynamic processes

## Resources

- [ilastik documentation](https://www.ilastik.org/documentation/)
- [ilastik tutorials](https://www.ilastik.org/documentation/tutorials/)
- [ilastik paper](https://www.nature.com/articles/s41592-019-0582-9)
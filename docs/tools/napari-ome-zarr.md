# Napari with OME-Zarr Support

Napari is a fast, interactive, multi-dimensional image viewer for Python, enhanced here with full OME-Zarr support for handling large, multi-dimensional datasets.

## Overview

This environment provides napari with all necessary dependencies for OME-Zarr support, making it ideal for viewing and analyzing large-scale bio image datasets stored in the OME-Zarr format.

## Environment

**Environment**: `napari-ome-zarr`

## Available Tasks

### Start Napari
Launch the napari viewer with OME-Zarr support:
```bash
pixi run napari
```

## Plugins Included

- **napari-ome-zarr-navigator**: Navigate through OME-Zarr datasets efficiently
- **napari-ome-zarr**: Core OME-Zarr support for napari
- **napari-feature-classifier**: Classify features in your images
- **napari-feature-visualization**: Visualize extracted features
- **napari-animation**: Create animations from your multi-dimensional data

## Features

- **Multi-dimensional viewing**: Handle 2D, 3D, and higher-dimensional datasets
- **OME-Zarr native support**: Seamlessly open and navigate OME-Zarr files
- **Interactive visualization**: Real-time exploration of large datasets
- **Plugin ecosystem**: Extended functionality through the included plugins
- **Layer-based approach**: Organize different data types in separate layers
- **Annotation tools**: Built-in tools for manual annotation and measurement

## Getting Started

1. Make sure you have pixi installed and this repository cloned
2. Navigate to the repository directory
3. Run `pixi run napari` to start the napari viewer
4. Open your OME-Zarr datasets and start exploring!

## Use Cases

- **Large dataset visualization**: View multi-terabyte OME-Zarr datasets efficiently
- **Multi-channel analysis**: Analyze multi-channel fluorescence images
- **Time-series data**: Navigate through time-lapse datasets
- **3D visualization**: Explore volumetric data with interactive 3D rendering
- **Feature analysis**: Use the feature plugins for quantitative analysis

## Resources

- [Napari documentation](https://napari.org/)
- [OME-Zarr specification](https://ngff.openmicroscopy.org/latest/)
- [Napari tutorials](https://napari.org/stable/tutorials/index.html)
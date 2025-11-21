# Feature Explorer

Feature Explorer is a Python dashboard application for exploring OME-Zarr images alongside tabular data, specifically designed to work with outputs from the Fractal Image Analysis platform.

## Overview

Feature Explorer provides an interactive web-based interface for visualizing and analyzing multi-dimensional image datasets with associated quantitative measurements and metadata.

## Environment

**Environment**: `feature-explorer`

## Available Tasks

### Start Feature Explorer Dashboard
Launch the interactive Feature Explorer dashboard:
```bash
pixi run feature-explorer
```

## Features

- **Interactive visualization**: Web-based dashboard for image and data exploration
- **OME-Zarr support**: Native support for OME-Zarr image format
- **Tabular data integration**: Seamlessly combine images with measurement data
- **Multi-dimensional navigation**: Explore 2D, 3D, and time-series datasets
- **Feature analysis**: Visualize and analyze extracted quantitative features
- **Fractal integration**: Optimized for Fractal Image Analysis platform outputs
- **Real-time filtering**: Interactive filtering and selection of data points
- **Export capabilities**: Export visualizations and filtered datasets

## Supported Data Types

### Image Data
- **OME-Zarr format**: Multi-resolution, chunked image arrays
- **Multi-channel images**: Fluorescence microscopy with multiple markers
- **Time-series data**: Time-lapse imaging datasets
- **3D volumes**: Confocal and light-sheet microscopy data

### Tabular Data
- **Feature measurements**: Quantitative measurements extracted from images
- **Metadata**: Experimental conditions and sample information
- **Segmentation results**: Object properties and classifications
- **Statistical summaries**: Aggregated measurements and statistics

## Dashboard Components

### Image Viewer
- Multi-dimensional image display with zoom and pan
- Channel selection and blending
- Overlay of segmentation masks and annotations
- Real-time image updates based on data selection

### Data Explorer
- Interactive tables with sorting and filtering
- Statistical plots and histograms
- Correlation analysis and scatter plots
- Feature distribution visualization

### Analysis Tools
- Quality control metrics and visualizations
- Batch comparison tools
- Export functionality for further analysis
- Integration with downstream analysis pipelines

## Getting Started

1. Make sure you have pixi installed and this repository cloned
2. Navigate to the repository directory
3. Run `pixi run feature-explorer` to start the dashboard
4. Open your browser and navigate to the provided URL
5. Load your OME-Zarr images and associated tabular data
6. Start exploring your datasets interactively!

## Use Cases

- **Quality control**: Assess image quality and analysis results
- **Data exploration**: Discover patterns and relationships in large datasets
- **Result validation**: Validate automated analysis results
- **Comparative analysis**: Compare results across different experimental conditions
- **Visualization**: Create publication-ready figures and visualizations
- **Data filtering**: Select subsets of data for downstream analysis

## Integration with Fractal

Feature Explorer is specifically designed to work with outputs from the Fractal Image Analysis platform, providing:
- Direct loading of Fractal workflow outputs
- Visualization of processing results at each workflow step
- Quality assessment of automated analysis pipelines
- Interactive exploration of large-scale analysis results

## Resources

- [Feature Explorer documentation](https://github.com/fractal-analytics-platform/feature-explorer)
- [Fractal platform documentation](https://fractal-analytics-platform.github.io/)
- [OME-Zarr specification](https://ngff.openmicroscopy.org/latest/)
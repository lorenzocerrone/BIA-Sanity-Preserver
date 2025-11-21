# ngio

ngio is a Python library designed for working with next-generation image formats, providing efficient access to modern image storage formats commonly used in bio image analysis.

## Overview

The ngio library provides a unified interface for reading and writing modern image formats, with a focus on performance, scalability, and interoperability with the broader scientific Python ecosystem.

## Environment

**Environment**: `ngio`

## Features

- **Modern format support**: Native support for next-generation image formats
- **Efficient I/O**: Optimized reading and writing operations
- **Chunked access**: Efficient handling of large datasets through chunked access patterns
- **Metadata preservation**: Comprehensive metadata handling and preservation
- **Lazy loading**: Memory-efficient lazy loading of large image datasets
- **Multi-dimensional support**: Handle 2D, 3D, time-series, and multi-channel data
- **Integration ready**: Seamless integration with NumPy, Dask, and other scientific libraries

## Supported Formats

### OME-Zarr
- **Specification compliant**: Full support for OME-Zarr specification
- **Multi-resolution**: Handle multi-resolution image pyramids
- **Cloud storage**: Direct access to cloud-stored datasets
- **Metadata**: Rich metadata support including spatial and temporal information

### Other Next-Generation Formats
- Support for various modern image formats optimized for scientific applications
- Extensible architecture for adding new format support
- Integration with existing format libraries

## Key Capabilities

### Efficient Data Access
```python
import ngio

# Open large datasets efficiently
dataset = ngio.open('large_dataset.ome.zarr')
# Access specific regions without loading entire dataset
region = dataset[100:200, 150:250, :]
```

### Metadata Handling
```python
# Access comprehensive metadata
metadata = dataset.metadata
spatial_info = metadata.spatial_calibration
channel_info = metadata.channels
```

### Integration with Scientific Stack
```python
import numpy as np
import dask.array as da

# Convert to standard array types
numpy_array = np.array(dataset[:])
dask_array = da.from_array(dataset)
```

## Use Cases

### Large Dataset Analysis
- Efficiently work with multi-terabyte imaging datasets
- Stream data for analysis without memory constraints
- Process datasets that don't fit in memory

### Cloud-Based Workflows
- Access datasets stored in cloud storage directly
- Enable distributed analysis workflows
- Facilitate data sharing and collaboration

### Format Conversion
- Convert between different image formats
- Preserve metadata during conversion
- Batch processing of image collections

### Integration Workflows
- Bridge between acquisition software and analysis pipelines
- Enable interoperability between different analysis tools
- Standardize data access patterns across workflows

## Getting Started

1. Make sure you have pixi installed and this repository cloned
2. Navigate to the repository directory
3. Activate the ngio environment for your analysis scripts
4. Import ngio in your Python code and start working with modern image formats!

## Performance Benefits

- **Chunked storage**: Efficient access patterns for large datasets
- **Compression**: Built-in compression reduces storage requirements
- **Parallel access**: Support for parallel reading operations
- **Memory efficiency**: Lazy loading prevents memory overflow
- **Network optimization**: Efficient access to remote datasets

## Integration Examples

### With Napari
```python
import ngio
import napari

# Open dataset with ngio and view in napari
dataset = ngio.open('dataset.ome.zarr')
viewer = napari.Viewer()
viewer.add_image(dataset)
```

### With Dask for Parallel Processing
```python
import ngio
import dask.array as da

# Use dask for parallel processing
dataset = ngio.open('large_dataset.ome.zarr')
dask_array = da.from_array(dataset, chunks=(512, 512, 10))
processed = dask_array.map_blocks(your_processing_function)
result = processed.compute()
```

## Resources

- [ngio documentation](https://github.com/fractal-analytics-platform/ngio)
- [OME-Zarr specification](https://ngff.openmicroscopy.org/latest/)
- [Zarr documentation](https://zarr.readthedocs.io/)
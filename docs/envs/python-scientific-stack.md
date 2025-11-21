# Python Scientific Stack

A comprehensive Python environment with all the essential libraries for bio image analysis, providing a solid foundation for scientific computing and image processing tasks.

## Overview

The BIA-ready Python Scientific Stack includes carefully selected packages that form the backbone of most bio image analysis workflows, from basic image processing to advanced machine learning applications.

## Environment

**Environment**: `bia-sci-py-stack`

## Available Tasks

### Start JupyterLab
Launch JupyterLab for interactive analysis:
```bash
pixi run jupyterlab
```

## Included Libraries

### Core Scientific Computing
- **numpy**: Fundamental array computing library
- **scipy**: Scientific computing tools and algorithms
- **pandas**: Data manipulation and analysis library
- **scikit-learn**: Machine learning library with classification, regression, and clustering algorithms

### Image Processing
- **scikit-image**: Comprehensive image processing toolkit
- **tifffile**: Read and write TIFF files efficiently
- **zarr**: Chunked, compressed, N-dimensional arrays

### Visualization
- **matplotlib**: Comprehensive plotting library
- **seaborn**: Statistical data visualization based on matplotlib
- **plotly**: Interactive plotting library

### Interactive Development
- **jupyterlab**: Modern web-based interactive development environment
- **ipywidgets**: Interactive HTML widgets for Jupyter notebooks

### Parallel Computing
- **dask**: Parallel computing library for analytics

### Additional Tools
- Various other specialized libraries for bio image analysis workflows

## Features

- **Complete environment**: Everything needed for most bio image analysis tasks
- **Optimized versions**: Carefully selected compatible versions of all packages
- **Ready to use**: No additional setup required
- **Extensible**: Easy to add additional packages as needed
- **Reproducible**: Locked dependencies ensure consistent results

## Getting Started

1. Make sure you have pixi installed and this repository cloned
2. Navigate to the repository directory
3. Run `pixi run jupyterlab` to start JupyterLab
4. Create new notebooks or open existing ones to start your analysis!

## Common Use Cases

### Image Processing
```python
import numpy as np
import skimage
from skimage import io, filters, segmentation
import matplotlib.pyplot as plt

# Load and process images
image = io.imread('your_image.tif')
filtered = filters.gaussian(image, sigma=1.0)
segmented = segmentation.watershed(filtered)
```

### Data Analysis
```python
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt

# Analyze measurement data
df = pd.read_csv('measurements.csv')
correlation_matrix = df.corr()
sns.heatmap(correlation_matrix, annot=True)
```

### Machine Learning
```python
from sklearn.ensemble import RandomForestClassifier
from sklearn.model_selection import train_test_split
from sklearn.metrics import accuracy_score

# Train a classifier on your features
X_train, X_test, y_train, y_test = train_test_split(features, labels)
clf = RandomForestClassifier()
clf.fit(X_train, y_train)
predictions = clf.predict(X_test)
```

### Large Dataset Handling
```python
import dask.array as da
import zarr

# Handle large arrays efficiently
large_array = da.from_zarr('large_dataset.zarr')
result = large_array.sum(axis=0).compute()
```

## Advantages

- **Batteries included**: No need to hunt down compatible library versions
- **Conflict-free**: All packages tested to work together harmoniously
- **Performance optimized**: Libraries compiled with optimizations where applicable
- **Documentation ready**: All standard libraries with full documentation
- **Community supported**: All packages are widely used and well-maintained

## Resources

- [NumPy documentation](https://numpy.org/doc/)
- [SciPy documentation](https://docs.scipy.org/)
- [scikit-image documentation](https://scikit-image.org/docs/)
- [Pandas documentation](https://pandas.pydata.org/docs/)
- [JupyterLab documentation](https://jupyterlab.readthedocs.io/)
# 🔬 BIA Sanity Preserver 🧠

> Because setting up bio image analysis tools shouldn’t cost you your sanity.

Setting up bio image analysis (BIA) tools the *sane* way is hard. Requirements change. Dependencies fight. Conflicts arise. Environments grow tangled and break.

**BIA Sanity Preserver** is here to restore balance.

With it, you can install and run your favourite bio image analysis tools in **clean, isolated environments**, avoiding conflicts and keeping your workflows reproducible and drama-free.

## 🧩 The Idea

In one work, use **[pixi](https://pixi.sh/latest/)**. No containers, no complexity, just pure, isolated environments.

📦  Each tool gets its own dedicated environment.
⚡ Environments can be quickly **created**, fearlessly **modified** (thanks to pixi locks 🔒), and easily **deleted**.


## 🚀 Getting Started

All you need is:

1. **pixi** installed → [pixi](https://pixi.sh/latest/)
2. This repository cloned:

```bash
git clone TODO
```

That’s it. You’re officially on the path to BIA enlightenment.


## 🛠️ Tools Included

Run your tools with a single command and zero emotional damage:

### **Bia-ready Python Scientific Stack**
An environment with all the essentials for bio image analysis in Python, including
`numpy`, `scipy`, `pandas`, `scikit-image`, `matplotlib`, `seaborn`, `jupyterlab`, `scikit-learn`, `dask`, `zarr`, `tiff-file`, and more.

**environment**: `bia-sci-py-stack`
**task**:
* Start a notebook with:
    ```bash
    pixi run jupyterlab
    ```
### **Napari** with OME-Zarr support
An environment with `napari`, and all necessary dependencies for OME-Zarr support, included.
**environment**: `napari-ome-zarr`
**task**:
* Start Napari with:
    ```bash
    pixi run napari
    ```

### **Cellpose**
An environment with `cellpose` for 2D and 3D cell segmentation.

**environment**: `cellpose`
**tasks**:
*  Cellpose 2D Gui
    ```bash
    pixi run cellpose
    ```
* Cellpose 3D GUI
    ```bash
    pixi run cellpose-3D
    ```

### **Ilastik**
An environment with `ilastik` for interactive machine learning-based image classification and segmentation.

**environment**: `ilastik`
**task**:
* Start Ilastik GUI:
    ```bash
    pixi run ilastik
    ```

### **PlantSeg**
`PlantSeg` is a deep learning-based tool for cell segmentation in plant tissues.

**environment**: `plantseg`
**tasks**:
* Start PlantSeg GUI
    ```bash
    pixi run plantseg-gui
    ```

### **ngio**
`ngio` is a python library for working with next-generation image formats.
**environment**: `ngio`

### **feature-explorer**
`feature-explorer` a python dashboard for exploring OME-Zarr images and with 
tabular data (e.g. outputs from the Fractal Image Analysis platform).

**environment**: `feature-explorer`
**task**:
* Start Feature Explorer Dashboard:
    ```bash
    pixi run feature-explorer
    ```

## 🌠 Wish List

* StarDist
* ...

(Java-based tools are trickier to containerize with pixi, but it could be done!)

* **Fiji / ImageJ2**
  (PoC available: [pixi-fiji](https://github.com/fmi-faim/pixi-fiji))

* **QuPath**



## 🤝 Contributing

Any contributions are welcome! Here’s how you can help:

* If something's not working, **open an issue** 🐛
* If you have ideas for new tools or improvements, **open an issue** 💡
* If you want to add a tool or improve an existing setup, **submit a pull request** 🚀

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
git clone https://github.com/lorenzocerrone/BIA-Sanity-Preserver
```

That’s it. You’re officially on the path to BIA enlightenment.


## 🛠️ Tools Included

Run your tools with a single command and zero emotional damage:

* [Cellpose](https://biovisioncenter.github.io/BIA-Sanity-Preserver/stable/tools/cellpose/)
* [Napari with OME-Zarr support](https://biovisioncenter.github.io/BIA-Sanity-Preserver/stable/tools/napari-ome-zarr/)
* [ilastik](https://biovisioncenter.github.io/BIA-Sanity-Preserver/stable/tools/ilastik/)
* [Plant-seg](https://biovisioncenter.github.io/BIA-Sanity-Preserver/stable/tools/plant-seg/)
* [Feature-explorer](https://biovisioncenter.github.io/BIA-Sanity-Preserver/stable/tools/feature-explorer/)
## 🏗️ Environments

Ready-to-use environments for bio image analysis:

* [Python Scientific Stack](https://biovisioncenter.github.io/BIA-Sanity-Preserver/stable/envs/python-scientific-stack/)
* [Ngio](https://biovisioncenter.github.io/BIA-Sanity-Preserver/stable/envs/ngio/)

## 🌠 Wish List

* StarDist
* ...

(Java-based tools are trickier to containerize with pixi, but it could be done!)

* **Fiji / ImageJ2**
  (PoC available: [pixi-fiji](https://github.com/fmi-faim/pixi-fiji))

* **QuPath**

## 🤝 Contributing

Such a project can only thrive with the help of the community, to make sure that it stays up-to-date and useful for everyone. Here’s how you can contribute:

* If you have ideas for new tools or improvements, **open an issue** 💡
* If you test some tools, and had an issue let us know by **opening an issue** 🐛
* If you know your way around pixi and want to add a tool or improve an existing setup, **submit a pull request** 🚀
* If the documentation is lacking or unclear, feel free to suggest improvements via **pull requests** ✍️

## 🧪 Testing

Each environment is automatically installed on Ubuntu, macOS, and Windows using GitHub Actions to ensure cross-platform compatibility. The tools themselves are not tested beyond installation.


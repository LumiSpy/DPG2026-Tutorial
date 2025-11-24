# Hands-on Tutorial: *HyperSpy* – Multidimensional data analysis using python

> **Spectroscopy Data Analysis in Python Using [HyperSpy](https://hyperspy.org)**

Tutorial for the **[DPG Spring Meeting of the Condensed Matter Section (SKM) 2026]([https://ebeam2024.sciencesconf.org/](https://dresden26.dpg-tagungen.de/programme/tutorials))**

> Dresden, March 8, 2026 | 16:00-18:15 h

---------------

**Dear attendants of the tutorial session at DPG Dresden,**

we are happy to introduce you to data analysis using [HyperSpy](https://hyperspy.org) and its extensions [RosettaSciIO](https://hyperspy.org/rosettasciio/), [LumiSpy](https://lumispy.org), [exSPy](https://hyperspy.org/exspy) and [pyXem](https://pyxem.readthedocs.io/). 

To follow the interactive tutorials and make maximum use of the limited time available, we kindly ask you to bring your laptop and already install the **[HyperSpy-bundle](https://hyperspy.org/hyperspy-bundle/)** matching your system before coming to the tutorial. The [HyperSpy bundle](https://hyperspy.org/hyperspy-bundle/) ships a python environment including all relevant packages.

Remember to bring a fully charged battery, as there will be limited power outlets in the room

## Installing HyperSpy

Follow the [installation guide for the HyperSpy bundle](https://hyperspy.org/hyperspy-bundle/install.html). The demo notebooks have been tested to run on the HyperSpy bundle version `2025.08.07`. Some of the examples might not run with older HyperSpy versions (`<2.0.0` / bundle releases up to `2023.11.20`) and we do not guarantee for operation with newer HyperSpy versions, though the syntax/API should not change until the next major release (`v3.0.0`) will be released.

If you already have python installed on your system and prefer not installing the bundle, we recommend creating a new environment for the tutorial and installing at least the following packages using *pip* or *conda*:

``hyperspy, exspy, pyxem, lumispy, hyperspy-gui-ipywidgets, jupyter-lab, ipympl, scikit-learn, numba``

*Note that you should have at least version `1.26.4` of `numpy` installed.*

Otherwise, have a look at the full [list of packages included in the HyperSpy-bundle](https://hyperspy.org/hyperspy-bundle/index.html#included-software-and-libraries).

*(if you run into problems, come a bit early - a number of experienced colleagues can help you get started)*

## Download tutorial for local execution:

The tutorials are based on [Jupyter Notebooks](http://jupyter.org/).

**[Download the tutorial notebooks and demo data as zip file](https://github.com/LumiSpy/DPG2026-Tutorial/archive/refs/heads/main.zip)** from this repository and unpack in a local directory.

The tutorial is split in four jupyter notebooks to cater both for participants with ot without precious experience using HyperSpy:
- `DPG26_1_HyperSpy-RosettaSciIO.ipynb` - A basic introduction to get started with core functionalitie
- `DPG26_2_LumiSpy.ipynb`- for luminescence spectroscopy
- `DPG26_3_exSPY.ipynb` - for electron energy loss spectroscopy (EELS)
- `DPG26_4_pyXem.ipynb` - for crystallographic diffraction microscopy, e.g. 4D-STEM

The relevant datasets are provided in the subfolder `data`.

Please once open at least one of the notebooks and try to run the first cell in order to make sure your local installation is working and you can debug your installation beforehand.

*(if you run into problems, come a bit early - a number of experienced colleagues can help you get started)*

## Launch jupyter-lab

If possible, try to already launch `jupyter-lab` on your computer and open the first tutorial notebooks to make sure that we can directly dive into the HyperSpy usage during the tutorials.

There are multiple ways to start `jupyter-lab`, see for example the [JupyterLab User Guide](https://jupyterlab.readthedocs.io/en/stable/getting_started/starting.html) or the [Ansys JupyterLab Quick Start Guide](https://developer.ansys.com/blog/jupyterlab-quick-start).

## Introduction to python

If you are new to programming or programming with python, we recommend the [W3 schools Python Tutorial](https://www.w3schools.com/python/default.asp).


## Visualising and running the tutorials online:

Even though the preferable way is to run the notebooks locally on your computer, there is ways for an online visualization or even execution:

(Non-interactive) Visualizing the tutorial notebooks online:

[![Notebook Viewer (nbviewer)](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg?sanitize=true)](https://nbviewer.org/github/lumispy/DPG2026-Tutorial/tree/main/)

(Interactive) Running the tutorial notebooks online (may be slow!):

[![Live demos (Binder)](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/lumispy/DPG2026-Tutorial/main)

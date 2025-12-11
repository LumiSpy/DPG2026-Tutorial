# Hands-on Tutorial: [HyperSpy](https://hyperspy.org) – Multidimensional data analysis using python

Tutorial for the **[DPG Spring Meeting of the Condensed Matter Section (SKM) 2026]([https://ebeam2024.sciencesconf.org/](https://dresden26.dpg-tagungen.de/programme/tutorials))**

Dresden, March 8, 2026 | 16:00-18:15 h

**Note: This tutorial is still work in progress, the final version will be available latest on March 1, 2026**

---------------

**Dear attendants of the tutorial session at DPG Dresden,**

we are happy to introduce you to data analysis using [HyperSpy](https://hyperspy.org) and its extensions [RosettaSciIO](https://hyperspy.org/rosettasciio/), [LumiSpy](https://lumispy.org), [exSPy](https://hyperspy.org/exspy) and [pyXem](https://pyxem.readthedocs.io/). 

To follow the interactive tutorials and make maximum use of the limited time available, we kindly ask you to bring your laptop and execute the following three steps prior to arriving at the tutorial (for further details see below):

1. [Install HyperSpy](#install-hyperspy)
2. Download the example notebooks by clicking the button below and extract the Zip file to a folder on your system

> [![Download Course Files](https://img.shields.io/badge/Download_Course_Files-347d39?style=for-the-badge&logoColor=white&logo=data:image/svg%2bxml;base64,PHN2ZyB2ZXJzaW9uPSIxIiB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PHBhdGggZD0iTTExLjIgMGEuOC44IDAgMCAwLS44Ljh2MTEuNEw3LjI2IDkuNDRhLjgwMy44MDMgMCAwIDAtMS4xMy4wNzRsLTEuMDUgMS4yYS44LjggMCAwIDAgLjA3MyAxLjEzbDYuMzMgNS41NGEuNzk1Ljc5NSAwIDAgMCAxLjA1IDBsNi4zMi01LjU0YS44LjggMCAwIDAgLjA3NC0xLjEzbC0xLjA1LTEuMmEuODA0LjgwNCAwIDAgMC0xLjEzLS4wNzRsLTMuMTQgMi43NlYuOGEuOC44IDAgMCAwLS44LS44em0tOCAyMC44YS44LjggMCAwIDAtLjguOHYxLjZhLjguOCAwIDAgMCAuOC44aDE3LjZhLjguOCAwIDAgMCAuOC0uOHYtMS42YS44LjggMCAwIDAtLjgtLjh6IiBmaWxsPSIiIHN0eWxlPSJmaWxsOiNmZmZmZmY7ZmlsbC1vcGFjaXR5OjEiIC8+PC9zdmc+)](https://github.com/LumiSpy/DPG2026-Tutorial/archive/refs/heads/main.zip)

3. Verify that you can load and execute the first sample notebook

Remember to bring a fully charged battery, as there will be limited power outlets in the room.


## Install HyperSpy:

Follow the [installation guide for the HyperSpy bundle](https://hyperspy.org/hyperspy-bundle/install.html). The [HyperSpy bundle](https://hyperspy.org/hyperspy-bundle/) ships a python environment including all relevant packages. *The demo notebooks have been tested to run on the HyperSpy bundle version `2025.12.06`. Some of the examples might not run with older HyperSpy versions (`<2.0.0` / bundle releases up to `2023.11.20`) and we do not guarantee for operation with newer HyperSpy versions, though the syntax/API should not change until the next major release (`v3.0.0`) will be released.*

If you already have python installed on your system and prefer not installing the bundle, we recommend creating a new environment for the tutorial and installing at least the following packages using *pip* or *conda*:

``hyperspy, exspy, pyxem, lumispy, hyperspy-gui-ipywidgets, jupyter-lab, ipympl, scikit-learn, numba``

*Note that you should have at least version `1.26.4` of `numpy` installed.*

Otherwise, have a look at the full [list of packages included in the HyperSpy-bundle](https://hyperspy.org/hyperspy-bundle/index.html#included-software-and-libraries).


## Download tutorial files for local execution:

The tutorials are based on [Jupyter Notebooks](http://jupyter.org/).

**[Download the tutorial notebooks and demo data as zip file](https://github.com/LumiSpy/DPG2026-Tutorial/archive/refs/heads/main.zip)** from this repository and unpack in a local directory.

The tutorial is split in four jupyter notebooks to cater both for participants with ot without precious experience using HyperSpy:
- `DPG26_1_HyperSpy-RosettaSciIO.ipynb` - A basic introduction to get started with core functionalitie
- `DPG26_2_LumiSpy.ipynb`- for luminescence spectroscopy
- `DPG26_3_exSPY.ipynb` - for electron energy loss spectroscopy (EELS)
- `DPG26_4_pyXem.ipynb` - for crystallographic diffraction microscopy, e.g. 4D-STEM

The relevant datasets are provided in the subfolder `data`.


## Launch jupyter-lab:

Beforehand, please try to already launch `jupyter-lab` on your computer, open the first tutorial notebook and try to run the first cell - to ensure your local installation is working and debug your installation if needed. That way, we can directly dive into the HyperSpy usage during the tutorials.

There are multiple ways to start `jupyter-lab`, see for example the [JupyterLab User Guide](https://jupyterlab.readthedocs.io/en/stable/getting_started/starting.html) or the [Ansys JupyterLab Quick Start Guide](https://developer.ansys.com/blog/jupyterlab-quick-start). If you installed the HyperSpy bundle:
- (on Windows): you will find the "HyperSpy-bundle prompt" in your Start Menu. Open this application, and change to the directory where you unzipped the files via the [`cd` command](https://www.geeksforgeeks.org/operating-systems/cd-cmd-command/). Once in the right directory, execute the `jupyter lab` command to start Jupyter
- (on MacOS or Linux): from a terminal window, change to the directory where you unzipped the files, and execute the `jupyter` command from the `bin/` directory of the bundle installation. This will look something like: 
  - `cd /Users/username/Downloads/hyperspy_tutorial/`
  - `/Users/username/hyperspy-bundle/bin/jupyter lab`

*(if you run into problems, come a bit early - a number of experienced colleagues can help you get started)*


## Introduction to python:

If you are new to programming or programming with python, we recommend the [W3 schools Python Tutorial](https://www.w3schools.com/python/default.asp).


## Visualising and running the tutorials in your browser:

While we recommend downloading this repository and running the code locally (since that will be how you use
HyperSpy on your own data), you can use the following link to interactively run these tutorial files
in your web browser (*may be slow*):

[![Live demos (Binder)](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/lumispy/DPG2026-Tutorial/main)

(Non-interactive) Visualizing the tutorial notebooks online:

[![Notebook Viewer (nbviewer)](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg?sanitize=true)](https://nbviewer.org/github/lumispy/DPG2026-Tutorial/tree/main/)

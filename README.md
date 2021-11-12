# <img src="https://raw.githubusercontent.com/hatchet/hatchet/develop/logo-hex.png"  width="64" valign="middle" alt="hatchet"/> Hatchet Tutorial

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/hatchet/hatchet-tutorial/main)

Hatchet is a Python-based library that allows [Pandas](https://pandas.pydata.org) dataframes to be indexed by structured tree and graph data. It is intended for analyzing performance data that has a hierarchy (for example, serial or parallel profiles that represent calling context trees, call graphs, nested regions’ timers, etc.). Hatchet implements various operations to analyze a single hierarchical data set or compare multiple data sets, and its API facilitates analyzing such data programmatically.

This repository contains materials for Hatchet's hands-on tutorial. You can do
all of the exercises on your own laptop using BinderHub.


### Running the notebooks online

We use [BinderHub](https://mybinder.org) to create a shareable and interactive
environment of the notebooks within a live JupyterHub instance.

You can access the interactive environment at this
[link](https://mybinder.org/v2/gh/hatchet/hatchet-tutorial)
or by clicking the badge at the top of this file.


### Running the notebooks at NERSC

To run the notebooks on Cori, you will need to install Caliper, create a conda
environment with Hatchet and its dependencies, and install the environment so
that it can be accessed in JupyterHub.

To build and install Caliper:

    $ git clone https://github.com/hatchet/hatchet-tutorial
    $ cd hatchet-tutorial
    $ ./build_and_install_caliper

To setup your local conda environment with Hatchet and its dependencies:

    $ module load python
    $ conda create --name hatchet-sc21-env python=3.8
    $ conda install ipykernel multiproces
    $ source activate hatchet-sc21-env
    $ pip install hatchet==1.3.1a0

Lastly, we install our conda environment so we can use it in JupyterHub:

    $ python -m ipykernel install --user --name hatchet-sc21-env-jupyter

To access the notebooks, navigate to https://jupyter.nersc.gov, and switch to
kernel "hatchet-sc21-env-jupyter" in the kernel list.


### License

This repository is distributed under the terms of the MIT license.

All contributions must be made under the MIT license.  Copyrights are retained
by contributors. No copyright assignment is required to contribute to this
project.

See [LICENSE](https://github.com/hatchet/hatchet-tutorial/blob/main/LICENSE).

SPDX-License-Identifier: MIT

LLNL-CODE-741008

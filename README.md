# Introduction to Spatial Optimisation at Tartu University
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ljwolf/agile-2023-spatialopt/HEAD)

*Levi John Wolf, University of Bristol *levi.john.wolf@bristol.ac.uk*

## Setup

### Step 1: Download the workshop material

If you are comfortable with GitHub and `git`, the command-line program, you can download the workshop materials by cloning my repository:

```sh
git clone https://github.com/ljwolf/tartu-spatialopt
cd tartu-spatialopt
```

If you are not comfortable with GitHub, download the repository to your computer as a zip file from the workshop website. To do this, go to <https://github.com/ljwolf/tartu-spatialopt>, click on the green button labelled "< > Code <i class="fa-regular fa-angle-down"></i>", then click the "<i class="fa-regular fa-file-zipper"></i> Download Zip" option. 

### Step 2: Install the required Python packages

To follow along with the workshop material, it is best if you install Anaconda, a scientific python computing environment. If you do not yet have Anaconda installed, you can install miniconda
(<https://conda.io/miniconda.html>) or the (larger) Anaconda distribution (<https://www.anaconda.com/download/>). 

Using the `conda` program from your command line or within the anaconda prompt, we recommend using the following terminal commands to set up your environment: 

```bash
# we want to use only the community-distributed packages on "conda-forge" 
conda config --add channels conda-forge
conda config --set channel_priority strict
# and, we want to use the faster implementation of conda, called "mamba"
conda install mamba
# Then, we want to create our actual environment
mamba env create --file environment.yml
# and finally, activate the environment
conda activate spatialopt
```

If you are using the "Anaconda Navigator" interface, you can import the workshop environment using [the steps described in its documentation.](https://docs.anaconda.com/free/navigator/tutorials/manage-environments/#importing-an-environment)

If you would prefer not to install everything on your own computer, you can follow along with the materials online using Binder [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ljwolf/agile-2023-spatialopt/main?urlpath=lab/) to open the notebooks without having to install any software. 

### Step 3: starting Jupyter Lab

To start your analysis environment locally, you first must activate the spatialopt environment: 
```bash
conda activate spatialopt
```

And then, you must start [Juptyer Lab](https://jupyterlab.readthedocs.io/en/stable/), the next-generation user interface for Project Jupyter. The workshop code is implemented in Jupyter Notebooks, a literate and interactive programming environment for scientific computing.

```bash
jupyter lab
```
### Acknowledgements

This material was generated with help, thanks, and perspective from [`spopt` contributors](https://github.com/pysal/spopt/graphs/contributors), funding from Google Summer of Code and the Association of Geographic Information Laboratories, Europe (AGILE). 
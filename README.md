# Ichthyop Conda environments 

In order to easily install all the tools to compile and run Ichthyop, install Anaconda (https://www.anaconda.com/products/individual).

## Anaconda install

### Linux users

When downloaded, run the install script as follows:

```
bash Anaconda3-2020.11-Linux-x86_64.sh
```

**Do not allow the `git-init` command**. 

When done, add the following line to your `~/.bash_profile` and `~/.bashrc` files:

```
. $CONDA/etc/profile.d/conda.sh
```

with `$CONDA` the path of your `Anaconda` install. 

### Mac Os X users

When downloaded, double-click on the ```Anaconda3-2020.11-MacOSX-x86_64.pkg``` file. 

When done, add the following line to your `~/.bash_profile` and `~/.bashrc` files:

```
. $CONDA/etc/profile.d/conda.sh
```

with `$CONDA` the path of your `Anaconda` install.

### Windows users

Double-click on the ```Anaconda3-2020.11-Windows-x86_64.exe``` and follow the install instructions. 

## Install Ichthyop Environments

### From command line (Anaconda Prompt, Terminal)

- Open a Terminal or the Anaconda prompt, and type: `conda create -c conda-forge --name ichthyop`
- Activate the environment: `conda activate ichthyop` 
- To run and compile Ichthyop, install Maven and NetCDF4 libray by typing:
```
conda install -y maven openjdk netcdf4 
```
- To use the Python library for Ichthyop, install the additional packages:
```
conda install -y xarray dask cartopy matplotlib ffmpeg 
```
- To use spyder, install:
```
conda install -y spyder
```
- To use Jupyter Notebooks, install the following packages:
```
conda install -y jupyter jupytext ipykernel
```
- To build the documentation, install:
```
conda install -y sphinxcontrib-programoutput sphinxcontrib-bibtex ipython sphinx_rtd_theme nbsphinx
```

### From Anaconda Navigator (Windows/MacOs users)

- Open the `Anaconda Navigator`
- Click on `Environments` and on the `Create` button. Select `Python`
- In the `Channels` box, make sure that both `Defaults` and `Conda-Forge` are available.
- Select all the packages listed in the above and which are not installed yet, then click on `Apply`

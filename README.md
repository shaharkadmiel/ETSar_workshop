# Interactive hands-on session

## Sardinia Workshop, Nuoro, November 2021

**Chairs:** *[Matteo Di Giovanni (GSSI)](mailto:matteo.digiovanni@gssi.it) & [Shahar Shani-Kadmiel (KNMI)](mailto:shahar.shani.kadmiel@knmi.nl)*

## Geting ready

The majority of the session will be interactive with a lot of hands-on demonstrations and exercises purposed to enrich the learning experience. We will do this by using [Jupyter Notebooks](https://jupyter.org/), which you should install (or already have) on your laptop.

We have prepared some instructions for setting up your environment. Please follow the instructions at your earliest convenience and send us an email if you run into any difficulties that you are not able to solve yourself. These instructions work on Linux and macOS but should work for Windows machines just as well.

---
#### Step 1:

If you do not already have Anaconda or Miniconda installed on your machine (Hint: If you are unsure, go ahead and install a fresh copy), follow this link to download Miniconda and install the right package for your OS: 

https://docs.conda.io/en/latest/miniconda.html#latest-miniconda-installer-links

We recommend the 64-bit version regardless of your OS.

Follow the Installation instructions (https://conda.io/projects/conda/en/latest/user-guide/install/index.html#regular-installation).

---
#### Step 2:
(optional, if you know what you are doing you can skip this step)

Whether you just installed Miniconda or are using an already existing conda environment, we recommend you to create a new environment by typing the following command in you terminal ('Anaconda Prompt' on Windows):

```shell
conda create -n ETSWS -c conda-forge -y
```

And activate this new environment with:

```shell
conda activate ETSWS
```

---
#### Step 3:

Now install the packages needed to run the session notebooks with the following command:

```shell
conda config --add channels conda-forge && conda install -y ipython \
    jupyter notebook scipy numpy pandas gdal pyproj netcdf4 matplotlib \
    cartopy obspy xarray dask
```


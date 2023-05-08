# Next-Level Data Visualization in Python

This repository provides the materials and prerequisites for attendees at ODSC East 2023.
The session is a 90-minute tutorial, where interactive participation is optional but encouraged.
There will be a mixture of presentation content and code demo, following notebooks `Part-1` through `Part-4`.

The notebooks make use of census data, which is included in the repo in `census-data`.
Additional notebooks are included in that folder for historical reference only,
showing how the data was downloaded and processed.

## Basic prerequisites

The examples assume an existing Python installation (`3.10.10`) with JupyterLab for running the sample notebooks.
Versions used to develop the notebooks are noted, but exact version matches are likely not required.

Most of the notebook examples can be run as long as some common packages are installed:
* `pandas` (`1.5.3`)
* `numpy` (`1.24.2`)
* `matplotlib` (`3.7.1`)
* `seaborn` (`0.12.2`, used in one example only)

## Advanced prerequisites

Some of the examples and supplementary code require additional packages that are less common, and may require some work to install correctly.

These are strictly OPTIONAL for the tutorial session; please do not sink a lot of time into attempting to install them unless you are very committed to experimenting with them on your own!

The following steps worked to install these packages on MacOS 13.2.1 (Ventura), with the above basic prerequisites and Homebrew already installed.
See the documentation for [`cenpy`](https://github.com/cenpy-devs/cenpy) and [`geopandas`](https://geopandas.org/en/stable/getting_started/install.html) for more details, and other options for installation.
```
# These are prerequisites for geopandas and cenpy
pip install rtree
pip install shapely
brew install gdal
pip install fiona
# Loading and plotting the geodata examples requires geopandas
pip install geopandas
# Supplementary code for obtaining the census data used in the examples requires cenpy
pip install cenpy
# Installing python-Levenshtein silences warnings in cenpy, but is not strictly required
pip install python-Levenshtein
```

Versions used in the `census-data` notebooks are `geopandas=0.12.2` and `cenpy=1.0.1`.
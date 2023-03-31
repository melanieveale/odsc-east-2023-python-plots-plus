# Next-Level Data Visualization in Python

This repository provides the materials and prerequisites for attendees at ODSC East 2023.
The session is a 90-minute tutorial, where interactive participation is optional but encouraged.
There will be a mixture of presentation content and code demo, with notebooks added closer to the session so participants can run the demo code themselves.

## Basic prerequisites

The examples assume an existing Python installation with JupyterLab for running the sample notebooks.

Most of the notebook examples can be run as long as some common packages are installed:
* `pandas`
* `numpy`
* `matplotlib`

## Advanced prerequisites

Some of the examples and supplementary code require additional packages that are less common, and may require some work to install correctly.
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
```


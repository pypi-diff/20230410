# Comparing `tmp/goes2go-2022.8.26.tar.gz` & `tmp/goes2go-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goes2go-2022.8.26.tar", last modified: Sat Aug 27 03:04:29 2022, max compression
+gzip compressed data, was "goes2go-2023.4.0.tar", last modified: Mon Apr 10 16:52:01 2023, max compression
```

## Comparing `goes2go-2022.8.26.tar` & `goes2go-2023.4.0.tar`

### file list

```diff
@@ -1,26 +1,39 @@
-drwxrwxrwx   0        0        0        0 2022-08-27 03:04:29.204998 goes2go-2022.8.26/
--rw-rw-rw-   0        0        0     1097 2022-03-26 16:25:47.000000 goes2go-2022.8.26/LICENSE
--rw-rw-rw-   0        0        0     7193 2022-08-27 03:04:29.203358 goes2go-2022.8.26/PKG-INFO
--rw-rw-rw-   0        0        0     6309 2022-07-16 04:15:53.000000 goes2go-2022.8.26/README.md
-drwxrwxrwx   0        0        0        0 2022-08-27 03:04:29.094491 goes2go-2022.8.26/goes2go/
--rw-rw-rw-   0        0        0     8030 2022-07-16 03:14:55.000000 goes2go-2022.8.26/goes2go/NEW.py
--rw-rw-rw-   0        0        0     3195 2022-07-16 03:00:53.000000 goes2go-2022.8.26/goes2go/__init__.py
--rw-rw-rw-   0        0        0    42246 2022-03-26 16:25:56.000000 goes2go-2022.8.26/goes2go/accessors.py
--rw-rw-rw-   0        0        0    21888 2022-08-27 02:57:33.000000 goes2go-2022.8.26/goes2go/data.py
--rw-rw-rw-   0        0        0     6798 2022-05-07 17:41:57.000000 goes2go-2022.8.26/goes2go/product_table.txt
--rw-rw-rw-   0        0        0    36217 2022-03-26 16:25:56.000000 goes2go-2022.8.26/goes2go/rgb.py
--rw-rw-rw-   0        0        0     6775 2022-03-26 16:25:56.000000 goes2go-2022.8.26/goes2go/tools.py
-drwxrwxrwx   0        0        0        0 2022-08-27 03:04:29.159674 goes2go-2022.8.26/goes2go.egg-info/
--rw-rw-rw-   0        0        0     7193 2022-08-27 03:04:26.000000 goes2go-2022.8.26/goes2go.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2022-08-27 03:04:28.000000 goes2go-2022.8.26/goes2go.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-27 03:04:27.000000 goes2go-2022.8.26/goes2go.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-07-16 04:03:41.000000 goes2go-2022.8.26/goes2go.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2022-08-27 03:04:27.000000 goes2go-2022.8.26/goes2go.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-08-27 03:04:28.000000 goes2go-2022.8.26/goes2go.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-27 03:04:29.205490 goes2go-2022.8.26/setup.cfg
--rw-rw-rw-   0        0        0     2345 2022-08-27 03:04:24.000000 goes2go-2022.8.26/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-27 03:04:29.198965 goes2go-2022.8.26/tests/
--rw-rw-rw-   0        0        0        0 2022-08-27 02:57:33.000000 goes2go-2022.8.26/tests/__init__.py
--rw-rw-rw-   0        0        0      318 2022-03-26 16:25:56.000000 goes2go-2022.8.26/tests/test_abi.py
--rw-rw-rw-   0        0        0     2861 2022-08-27 02:57:33.000000 goes2go-2022.8.26/tests/test_data.py
--rw-rw-rw-   0        0        0      348 2022-03-26 16:25:56.000000 goes2go-2022.8.26/tests/test_glm.py
+drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-10 16:52:01.000000 goes2go-2023.4.0/
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)       69 2022-03-07 22:50:31.000000 goes2go-2023.4.0/.gitattributes
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     2027 2023-02-02 16:15:19.000000 goes2go-2023.4.0/.gitignore
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     1079 2023-02-02 16:12:51.000000 goes2go-2023.4.0/.readthedocs.yml
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      977 2023-04-10 16:44:33.000000 goes2go-2023.4.0/CITATION.cff
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     1076 2022-03-07 22:50:31.000000 goes2go-2023.4.0/LICENSE
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      102 2022-10-20 19:50:16.000000 goes2go-2023.4.0/MANIFEST.in
+-rw-------   0 blaylock (922916) 0381G056  (8708)     9935 2023-04-10 16:52:01.000000 goes2go-2023.4.0/PKG-INFO
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     8722 2023-02-02 16:12:51.000000 goes2go-2023.4.0/README.md
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     2393 2022-11-15 17:49:05.000000 goes2go-2023.4.0/environment-dev.yml
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      747 2022-11-15 17:45:56.000000 goes2go-2023.4.0/environment-test-conda.yml
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     1038 2022-10-20 20:22:08.000000 goes2go-2023.4.0/environment-test.yml
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     1352 2023-02-02 16:28:56.000000 goes2go-2023.4.0/environment.yml
+drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-10 16:52:01.000000 goes2go-2023.4.0/goes2go/
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     7797 2022-10-20 15:16:21.000000 goes2go-2023.4.0/goes2go/NEW.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     3105 2023-03-20 15:41:44.000000 goes2go-2023.4.0/goes2go/__init__.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      166 2023-04-10 16:51:37.000000 goes2go-2023.4.0/goes2go/_version.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)    41053 2023-03-20 15:41:44.000000 goes2go-2023.4.0/goes2go/accessors.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)    21281 2023-03-20 15:46:12.000000 goes2go-2023.4.0/goes2go/data.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     6710 2022-05-12 15:43:43.000000 goes2go-2023.4.0/goes2go/product_table.txt
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)    35108 2023-03-20 15:41:44.000000 goes2go-2023.4.0/goes2go/rgb.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     6593 2022-03-21 20:48:21.000000 goes2go-2023.4.0/goes2go/tools.py
+drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-10 16:52:01.000000 goes2go-2023.4.0/goes2go.egg-info/
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     9935 2023-04-10 16:51:37.000000 goes2go-2023.4.0/goes2go.egg-info/PKG-INFO
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      656 2023-04-10 16:52:00.000000 goes2go-2023.4.0/goes2go.egg-info/SOURCES.txt
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)        1 2023-04-10 16:51:37.000000 goes2go-2023.4.0/goes2go.egg-info/dependency_links.txt
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)        1 2021-02-22 16:48:38.000000 goes2go-2023.4.0/goes2go.egg-info/not-zip-safe
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      237 2023-04-10 16:51:37.000000 goes2go-2023.4.0/goes2go.egg-info/requires.txt
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)       14 2023-04-10 16:51:37.000000 goes2go-2023.4.0/goes2go.egg-info/top_level.txt
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      277 2022-10-20 19:33:08.000000 goes2go-2023.4.0/pyproject.toml
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      107 2022-10-20 18:27:34.000000 goes2go-2023.4.0/requirements.txt
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     1541 2023-04-10 16:52:01.000000 goes2go-2023.4.0/setup.cfg
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)       69 2022-10-20 19:32:14.000000 goes2go-2023.4.0/setup.py
+drwx------   0 blaylock (922916) 0381G056  (8708)        0 2023-04-10 16:52:01.000000 goes2go-2023.4.0/tests/
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)        0 2022-10-20 15:16:21.000000 goes2go-2023.4.0/tests/__init__.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      532 2022-11-15 17:49:05.000000 goes2go-2023.4.0/tests/test_GOES.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      302 2022-03-21 20:48:21.000000 goes2go-2023.4.0/tests/test_abi.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)     2756 2023-03-20 15:41:44.000000 goes2go-2023.4.0/tests/test_data.py
+-rw-r-----   0 blaylock (922916) 0381G056  (8708)      332 2022-03-21 20:48:21.000000 goes2go-2023.4.0/tests/test_glm.py
```

### Comparing `goes2go-2022.8.26/README.md` & `goes2go-2023.4.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,148 +1,211 @@
-<div
-  align="center"
->
-
-![](https://github.com/blaylockbk/goes2go/blob/main/docs/_static/goes2go_logo_100dpi.png?raw=true)
-
-# Download and display GOES-East and GOES-West data
-
-<!-- Badges -->
-
-[![](https://img.shields.io/pypi/v/goes2go)](https://pypi.python.org/pypi/goes2go/)
-![](https://img.shields.io/github/license/blaylockbk/goes2go)
-[![DOI](https://zenodo.org/badge/296737878.svg)](https://zenodo.org/badge/latestdoi/296737878)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-<!--[![Join the chat at https://gitter.im/blaylockbk/goes2go](https://badges.gitter.im/blaylockbk/goes2go.svg)](https://gitter.im/blaylockbk/goes2go?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)-->
-<!--(Badges)-->
-
-</div>
-
-GOES-East and GOES-West satellite data are made available on Amazon Web Services through [NOAA's Big Data Program](https://www.noaa.gov/information-technology/big-data). **GOES-2-go** is a python package that makes it easy to find and download the files you want to your local computer with some additional helpers to look at and understand the data.
-
----
-
-<br>
-
-# 📔 [GOES-2-go Documentation](https://blaylockbk.github.io/goes2go/_build/html/)
-
-<br>
-
----
-
-# Capabilities
-
-## Download Data
-
-Download GOES ABI or GLM NetCDF files to your local computer. Files can also be read with xarray.
-
-First, create a GOES object to specify the satellite, data product, and domain you are interested in. The example below downloads the Multi-Channel Cloud Moisture Imagery for CONUS.
-
-```python
-from goes2go import GOES
-
-# ABI Multi-Channel Cloud Moisture Imagry Product
-G = GOES(satellite=16, product="ABI-L2-MCMIP", domain='C')
-
-# Geostationary Lightning Mapper
-G = GOES(satellite=17, product="GLM-L2-LCFA", domain='C')
-
-# ABI Level 1b Data
-G = GOES(satellite=17, product="ABI-L1b-Rad", domain='F')
-```
-
-> A complete listing of the products available are available [here](https://github.com/blaylockbk/goes2go/blob/main/goes2go/product_table.txt).
-
-There are methods to do the following:
-
-- List the available files for a time range
-- Download data to your local drive for a specified time range
-- Read the data into an xarray Dataset for a specific time
-
-```python
-   # Produce a pandas DataFrame of the available files in a time range
-   df = G.df(start='2022-07-04 01:00', end='2022-07-04 01:30')
-```
-
-```python
-   # Download and read the data as an xarray Dataset nearest a specific time
-   ds = G.nearesttime('2022-01-01')
-```
-
-```python
-   # Download and read the latest data as an xarray Dataset
-   ds = G.latest()
-```
-
-```python
-   # Download data for a specified time range
-   G.timerange(start='2022-06-01 00:00', end='2022-06-01 01:00')
-
-   # Download recent data for a specific interval
-   G.timerange(recent='30min')
-```
-
-## RGB Recipes
-
-The `rgb` xarray accessor creates an RGB product for a GOES ABI multichannel xarray.Dataset. See the [demo](https://blaylockbk.github.io/goes2go/_build/html/user_guide/notebooks/DEMO_rgb_recipes.html#) for more examples of RGB products.
-
-```python
-import matplotlib.pyplot as plt
-ds = GOES().latest()
-ax = plt.subplot(projection=ds.rgb.crs)
-ax.imshow(ds.rgb.TrueColor(), **ds.rgb.imshow_kwargs)
-ax.coastlines()
-```
-
-![](./images/TrueColor.png)
-
-## Field of View
-
-The `FOV` xarray accessor creates shapely.Polygon objects for the ABI and GLM field of view. See notebooks for [GLM](https://blaylockbk.github.io/goes2go/_build/html/user_guide/notebooks/field-of-view_GLM.html) and [ABI](https://blaylockbk.github.io/goes2go/_build/html/user_guide/notebooks/field-of-view_ABI.html) field of view.
-
-```python
-from goes2go.data import goes_latest
-G = goes_latest()
-# Get polygons of the full disk or ABI domain field of view.
-G.FOV.full_disk
-G.FOV.domain
-# Get Cartopy coordinate reference system
-G.FOV.crs
-```
-
-GOES-West is centered over -137 W and GOES-East is centered over -75 W. When GOES was being tested, it was in a "central" position, outlined in the dashed black line. Below is the ABI field of view for the full disk:
-![field of view image](./images/ABI_field-of-view.png)
-
-The GLM field of view is slightly smaller and limited by a bounding box. Below is the approximated GLM field of view:
-![field of view image](./images/GLM_field-of-view.png)
-
-> ### Useful Links
->
-> - [🙋🏻‍♂️ Brian's AWS GOES Web Downloader](https://home.chpc.utah.edu/~u0553130/Brian_Blaylock/cgi-bin/goes16_download.cgi)
-> - [📔 GOES-R Series Data Book](https://www.goes-r.gov/downloads/resources/documents/GOES-RSeriesDataBook.pdf)
-> - [🎠 Beginner's Guide](https://www.goes-r.gov/downloads/resources/documents/Beginners_Guide_to_GOES-R_Series_Data.pdf)
-> - [🖥 Rammb Slider GOES Viewer](https://rammb-slider.cira.colostate.edu)
-> - [💾 GOES on AWS](https://registry.opendata.aws/noaa-goes/)
-> - [🐍 Unidata Plot GOES Data](https://unidata.github.io/python-training/gallery/mapping_goes16_truecolor/)
-> - [🗺 Plotting tips form geonetcast blog](https://geonetcast.wordpress.com/2019/08/02/plot-0-5-km-goes-r-full-disk-regions/)
-> - [🐍 `glmtools`](https://github.com/deeplycloudy/glmtools/)
-> - [🐍 `satpy`](https://github.com/pytroll/satpy)
-
-> ### What if I don't like the GOES-2-go or Python?
->
-> As an alternative you can use [rclone](https://rclone.org/) to download GOES files from AWS. I quite like rclone. Here is a [short rclone tutorial](https://github.com/blaylockbk/pyBKB_v3/blob/master/rclone_howto.md).
-
----
-
----
-
-I hope you find this makes GOES data easier to retrieve and display. Enjoy!
-
-\- Brian Blaylock
-
-👨🏻‍💻 [Contributing Guidelines](https://blaylockbk.github.io/goes2go/_build/html/user_guide/contribute.html)  
-💬 [GitHub Discussions](https://github.com/blaylockbk/goes2go/discussions)  
-🚑 [GitHub Issues](https://github.com/blaylockbk/goes2go/issues)  
-🌐 [Personal Webpage](http://home.chpc.utah.edu/~u0553130/Brian_Blaylock/home.html)
-
-P.S. If you like GOES-2-go, check out my [Herbie](https://github.com/blaylockbk/Herbie) package to download weather model data and [SynopticPy](https://github.com/blaylockbk/Herbie) to download mesonet data from the Synoptic API.
+<div
+  align="center"
+>
+
+![](https://github.com/blaylockbk/goes2go/blob/main/docs/_static/goes2go_logo_100dpi.png?raw=true)
+
+# Download and display GOES-East and GOES-West data
+
+<!-- Badges -->
+
+[![](https://img.shields.io/pypi/v/goes2go)](https://pypi.python.org/pypi/goes2go/)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/goes2go.svg)](https://anaconda.org/conda-forge/goes2go)
+[![DOI](https://zenodo.org/badge/296737878.svg)](https://zenodo.org/badge/latestdoi/296737878)
+
+![](https://img.shields.io/github/license/blaylockbk/goes2go)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Documentation Status](https://readthedocs.org/projects/goes2go/badge/?version=latest)](https://goes2go.readthedocs.io/?badge=latest)
+[![Python](https://img.shields.io/pypi/pyversions/goes2go.svg)](https://pypi.org/project/goes2go/)
+[![Conda Recipe](https://img.shields.io/badge/recipe-goes2go-green.svg)](https://anaconda.org/conda-forge/goes2go)
+[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/goes2go.svg)](https://anaconda.org/conda-forge/goes2go)
+[![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/goes2go.svg)](https://anaconda.org/conda-forge/goes2go)
+
+<!--(Badges)-->
+
+</div>
+
+GOES-East and GOES-West satellite data are made available on Amazon Web Services through [NOAA's Big Data Program](https://www.noaa.gov/information-technology/big-data). **GOES-2-go** is a python package that makes it easy to find and download the files you want to your local computer with some additional helpers to look at and understand the data.
+
+---
+
+<br>
+
+# 📔 [GOES-2-go Documentation](https://goes2go.readthedocs.io/)
+
+<br>
+
+---
+
+# Installation
+
+The easiest way to install `goes2go` and its dependencies is with [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) from conda-forge.
+
+```
+conda install -c conda-forge goes2go
+```
+
+You may also create the provided Conda environment, **[`environment.yml`](https://github.com/blaylockbk/goes2go/blob/main/environment.yml)**.
+
+```bash
+# Download environment file
+wget https://github.com/blaylockbk/goes2go/raw/main/environment.yml
+
+# Modify that file if you wish.
+
+# Create the environment
+conda env create -f environment.yml
+
+# Activate the environment
+conda activate goes2go
+```
+
+Alternatively, `goes2go` is published on PyPI and you can install it with pip, _but_ it requires some additional dependencies that you will have to install yourself:
+
+- Python 3.8+
+- [Cartopy](https://scitools.org.uk/cartopy/docs/latest/installing.html), which requires GEOS and Proj.
+- MetPy
+- _Optional:_ [Carpenter Workshop](https://github.com/blaylockbk/Carpenter_Workshop)
+
+When those are installed within your environment, _then_ you can install GOES-2-go with pip.
+
+```bash
+# Latest published version
+pip install goes2go
+
+# ~~ or ~~
+
+# Most recent changes
+pip install git+https://github.com/blaylockbk/goes2go.git
+```
+
+# Capabilities
+
+- [Download GOES Data](#download-data)
+- [Create RGB composites](#rgb-recipes)
+- [Get the field of view](#field-of-view)
+
+## Download Data
+
+Download GOES ABI or GLM NetCDF files to your local computer. Files can also be read with xarray.
+
+First, create a GOES object to specify the satellite, data product, and domain you are interested in. The example below downloads the Multi-Channel Cloud Moisture Imagery for CONUS.
+
+```python
+from goes2go import GOES
+
+# ABI Multi-Channel Cloud Moisture Imagry Product
+G = GOES(satellite=16, product="ABI-L2-MCMIP", domain='C')
+
+# Geostationary Lightning Mapper
+G = GOES(satellite=17, product="GLM-L2-LCFA", domain='C')
+
+# ABI Level 1b Data
+G = GOES(satellite=17, product="ABI-L1b-Rad", domain='F')
+```
+
+> A complete listing of the products available are available [here](https://github.com/blaylockbk/goes2go/blob/main/goes2go/product_table.txt).
+
+There are methods to do the following:
+
+- List the available files for a time range
+- Download data to your local drive for a specified time range
+- Read the data into an xarray Dataset for a specific time
+
+```python
+   # Produce a pandas DataFrame of the available files in a time range
+   df = G.df(start='2022-07-04 01:00', end='2022-07-04 01:30')
+```
+
+```python
+   # Download and read the data as an xarray Dataset nearest a specific time
+   ds = G.nearesttime('2022-01-01')
+```
+
+```python
+   # Download and read the latest data as an xarray Dataset
+   ds = G.latest()
+```
+
+```python
+   # Download data for a specified time range
+   G.timerange(start='2022-06-01 00:00', end='2022-06-01 01:00')
+
+   # Download recent data for a specific interval
+   G.timerange(recent='30min')
+```
+
+## RGB Recipes
+
+The `rgb` xarray accessor creates an RGB product for a GOES ABI multichannel xarray.Dataset. See the [demo](https://goes2go.readthedocs.io/en/latest/user_guide/notebooks/DEMO_rgb_recipes.html#) for more examples of RGB products.
+
+```python
+import matplotlib.pyplot as plt
+ds = GOES().latest()
+ax = plt.subplot(projection=ds.rgb.crs)
+ax.imshow(ds.rgb.TrueColor(), **ds.rgb.imshow_kwargs)
+ax.coastlines()
+```
+
+![](./images/TrueColor.png)
+
+## Field of View
+
+The `FOV` xarray accessor creates shapely.Polygon objects for the ABI and GLM field of view. See notebooks for [GLM](https://goes2go.readthedocs.io/en/latest/user_guide/notebooks/field-of-view_GLM.html) and [ABI](https://goes2go.readthedocs.io/en/latest/user_guide/notebooks/field-of-view_ABI.html) field of view.
+
+```python
+from goes2go.data import goes_latest
+G = goes_latest()
+# Get polygons of the full disk or ABI domain field of view.
+G.FOV.full_disk
+G.FOV.domain
+# Get Cartopy coordinate reference system
+G.FOV.crs
+```
+
+GOES-West is centered over -137 W and GOES-East is centered over -75 W. When GOES was being tested, it was in a "central" position, outlined in the dashed black line. Below is the ABI field of view for the full disk:
+![field of view image](./images/ABI_field-of-view.png)
+
+The GLM field of view is slightly smaller and limited by a bounding box. Below is the approximated GLM field of view:
+![field of view image](./images/GLM_field-of-view.png)
+
+# How to Cite and Acknowledge
+
+If GOES-2-go played an important role in your work, please [tell me about it](https://github.com/blaylockbk/goes2go/discussions/categories/show-and-tell)! Also, consider including a citation or acknowledgement in your article or product.
+
+**_Suggested Citation_**
+
+> Blaylock, B. K. (2022). GOES-2-go: Download and display GOES-East and GOES-West data (Version 2022.07.15) [Computer software]. https://github.com/blaylockbk/goes2go
+
+**_Suggested Acknowledgment_**
+
+> A portion of this work used code generously provided by Brian Blaylock's GOES-2-go python package (https://github.com/blaylockbk/goes2go)
+
+### What if I don't like the GOES-2-go or Python?
+
+As an alternative you can use [rclone](https://rclone.org/) to download GOES files from AWS. I quite like rclone. Here is a [short rclone tutorial](https://github.com/blaylockbk/pyBKB_v3/blob/master/rclone_howto.md).
+
+---
+
+I hope you find this makes GOES data easier to retrieve and display. Enjoy!
+
+\- Brian Blaylock
+
+👨🏻‍💻 [Contributing Guidelines](https://goes2go.readthedocs.io/en/latest/user_guide/contribute.html)  
+💬 [GitHub Discussions](https://github.com/blaylockbk/goes2go/discussions)  
+🚑 [GitHub Issues](https://github.com/blaylockbk/goes2go/issues)  
+🌐 [Personal Webpage](http://home.chpc.utah.edu/~u0553130/Brian_Blaylock/home.html)
+
+P.S. If you like GOES-2-go, check out my [Herbie](https://github.com/blaylockbk/Herbie) package to download weather model data and [SynopticPy](https://github.com/blaylockbk/Herbie) to download mesonet data from the Synoptic API.
+
+# Useful Links
+
+- [🙋🏻‍♂️ Brian's AWS GOES Web Downloader](https://home.chpc.utah.edu/~u0553130/Brian_Blaylock/cgi-bin/goes16_download.cgi)
+- [📔 GOES-R Series Data Book](https://www.goes-r.gov/downloads/resources/documents/GOES-RSeriesDataBook.pdf)
+- [🎠 Beginner's Guide](https://www.goes-r.gov/downloads/resources/documents/Beginners_Guide_to_GOES-R_Series_Data.pdf)
+- [🖥 Rammb Slider GOES Viewer](https://rammb-slider.cira.colostate.edu)
+- [💾 GOES on AWS](https://registry.opendata.aws/noaa-goes/)
+- [🐍 Unidata Plot GOES Data](https://unidata.github.io/python-training/gallery/mapping_goes16_truecolor/)
+- [🗺 Plotting tips form geonetcast blog](https://geonetcast.wordpress.com/2019/08/02/plot-0-5-km-goes-r-full-disk-regions/)
+- [🐍 `glmtools`](https://github.com/deeplycloudy/glmtools/)
+- [🐍 `satpy`](https://github.com/pytroll/satpy)
+- [🖥 CSPPGEO](http://cimss.ssec.wisc.edu/csppgeo/) | [Gridded GLM software package](https://download.ssec.wisc.edu/files/csppgeo/)
```

### Comparing `goes2go-2022.8.26/goes2go/__init__.py` & `goes2go-2023.4.0/goes2go/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,97 +1,98 @@
-## Brian Blaylock
-## July 8, 2021
-
-import warnings
-import toml
-from pathlib import Path
-import os
-
-#=======================================================================
-# Load custom xarray accessors
-# TODO: Move some of the tools.py to these accessors.
-try:
-    import goes2go.accessors
-except:
-    warnings.warn("goes2go xarray accessors could not be imported.")
-
-#=======================================================================
-# Append Path object with my custom expand method so user can use
-# environment variables in the config file (e.g., ${HOME}).
-def _expand(self):
-    """
-    Fully expand and resolve the Path with the given environment variables.
-
-    Example
-    -------
-    >>> Path('$HOME').expand()
-    >>> PosixPath('/p/home/blaylock')
-    """
-    return Path(os.path.expandvars(self)).expanduser().resolve()
-
-
-Path.expand = _expand
-
-#=======================================================================
-# goes2go configuration file
-# Configuration file is save in `~/config/goes2go/config.toml`
-_config_path = Path("~/.config/goes2go/config.toml").expand()
-_save_dir = str(Path("~/data").expand())
-
-# NOTE: The `\\` is an escape character in TOML.
-# For Windows paths "C:\\user\\"" needs to be "C:\\\\user\\\\""
-_save_dir = str(Path("~/data").expand())
-_save_dir = _save_dir.replace("\\", "\\\\")
-
-#=======================================================================
-# Default TOML Configuration
-default_toml = f"""
-["default"]
-save_dir = "{_save_dir}"
-satellite = "noaa-goes16"
-product = "ABI-L2-MCMIP"
-domain = "C"
-download = true
-return_as = "filelist"
-overwrite = false
-max_cpus = 1
-s3_refresh = true
-verbose = true
-
-["timerange"]
-s3_refresh = false
-
-["latest"]
-return_as = "xarray"
-
-["nearesttime"]
-within = "1H"
-return_as = "xarray"
-"""
-
-#=======================================================================
-# If a config file isn't found, make one
-if not _config_path.exists():
-    print(
-        f" ╭─────────────────────────────────────────────────╮\n"
-        f" │ I'm building goes2go's default config file.     │\n"
-        f" ╰╥────────────────────────────────────────────────╯\n"
-        f" 👷🏻‍♂️"
-    )
-    _config_path.parent.mkdir(parents=True, exist_ok=True)
-    with open(_config_path, "w") as f:
-        toml_string = toml.dump(toml.loads(default_toml), f)
-    print(f"⚙ Created config file [{_config_path}] with default values.")
-
-#=======================================================================
-# Read the config file
-config = toml.load(_config_path)
-
-config["default"]["save_dir"] = Path(config["default"]["save_dir"]).expand()
-
-# Merge default settings with overwrite settings for each download method
-for i in ["timerange", "latest", "nearesttime"]:
-    config[i] = {**config["default"], **config[i]}
-
-
-from goes2go.NEW import GOES
-from goes2go.data import goes_nearesttime, goes_latest, goes_timerange
+## Brian Blaylock
+## July 8, 2021
+
+import warnings
+import toml
+from pathlib import Path
+import os
+
+# =======================================================================
+# Load custom xarray accessors
+# TODO: Move some of the tools.py to these accessors.
+try:
+    import goes2go.accessors
+except:
+    warnings.warn("goes2go xarray accessors could not be imported.")
+
+
+# =======================================================================
+# Append Path object with my custom expand method so user can use
+# environment variables in the config file (e.g., ${HOME}).
+def _expand(self):
+    """
+    Fully expand and resolve the Path with the given environment variables.
+
+    Example
+    -------
+    >>> Path('$HOME').expand()
+    >>> PosixPath('/p/home/blaylock')
+    """
+    return Path(os.path.expandvars(self)).expanduser().resolve()
+
+
+Path.expand = _expand
+
+# =======================================================================
+# goes2go configuration file
+# Configuration file is save in `~/config/goes2go/config.toml`
+_config_path = Path("~/.config/goes2go/config.toml").expand()
+_save_dir = str(Path("~/data").expand())
+
+# NOTE: The `\\` is an escape character in TOML.
+# For Windows paths "C:\\user\\"" needs to be "C:\\\\user\\\\""
+_save_dir = str(Path("~/data").expand())
+_save_dir = _save_dir.replace("\\", "\\\\")
+
+# =======================================================================
+# Default TOML Configuration
+default_toml = f"""
+["default"]
+save_dir = "{_save_dir}"
+satellite = "noaa-goes16"
+product = "ABI-L2-MCMIP"
+domain = "C"
+download = true
+return_as = "filelist"
+overwrite = false
+max_cpus = 1
+s3_refresh = true
+verbose = true
+
+["timerange"]
+s3_refresh = false
+
+["latest"]
+return_as = "xarray"
+
+["nearesttime"]
+within = "1H"
+return_as = "xarray"
+"""
+
+# =======================================================================
+# If a config file isn't found, make one
+if not _config_path.exists():
+    print(
+        f" ╭─────────────────────────────────────────────────╮\n"
+        f" │ I'm building goes2go's default config file.     │\n"
+        f" ╰╥────────────────────────────────────────────────╯\n"
+        f" 👷🏻‍♂️"
+    )
+    _config_path.parent.mkdir(parents=True, exist_ok=True)
+    with open(_config_path, "w") as f:
+        toml_string = toml.dump(toml.loads(default_toml), f)
+    print(f"⚙ Created config file [{_config_path}] with default values.")
+
+# =======================================================================
+# Read the config file
+config = toml.load(_config_path)
+
+config["default"]["save_dir"] = Path(config["default"]["save_dir"]).expand()
+
+# Merge default settings with overwrite settings for each download method
+for i in ["timerange", "latest", "nearesttime"]:
+    config[i] = {**config["default"], **config[i]}
+
+
+from goes2go.NEW import GOES
+from goes2go.data import goes_nearesttime, goes_latest, goes_timerange
```

### Comparing `goes2go-2022.8.26/goes2go/accessors.py` & `goes2go-2023.4.0/goes2go/accessors.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1197 +1,1197 @@
-## Brian Blaylock
-## July 9, 2021
-
-"""
-===========
-RGB Recipes
-===========
-
-RGB Recipes for the GOES Advanced Baseline Imager.
-
-More about xarray accessors:
-http://xarray.pydata.org/en/stable/internals/extending-xarray.html?highlight=extending#
-"""
-
-import warnings
-
-import cartopy.crs as ccrs
-import numpy as np
-import xarray as xr
-from shapely.geometry import Point, Polygon
-
-
-########################
-# Image Processing Tools
-def _gamma_correction(a, gamma, verbose=False):
-    """
-    Darken or lighten an image with `gamma correction
-    <https://en.wikipedia.org/wiki/_gamma_correction>`_.
-
-    Parameters
-    ----------
-    a : array-like
-        An array of values, typically the RGB array of values in
-        an image.
-    gamma : float
-        Gamma value to decode the image by.
-        Values > 1 will lighten an image.
-        Values < 1 will darken an image.
-    """
-    if verbose:
-        if gamma > 1:
-            print("Gamma Correction: 🌔 Lighten image")
-        elif gamma < 1:
-            print("Gamma Correction: 🌒 Darken image")
-        else:
-            print("Gamma Correction: 🌓 Gamma=1. No correction made.")
-            return a
-
-    # Gamma decoding formula
-    return np.power(a, 1 / gamma)
-
-
-def _normalize(value, lower_limit, upper_limit, clip=True):
-    """
-    Normalize values between an upper and lower limit between 0 and 1.
-
-    Normalize between a lower and upper limit. In other words, it
-    converts your number to a value in the range between 0 and 1.
-    Follows `normalization formula
-    <https://stats.stackexchange.com/a/70807/220885>`_
-
-    This is the same concept as `contrast or histogram stretching
-    <https://staff.fnwi.uva.nl/r.vandenboomgaard/IPCV20162017/LectureNotes/IP/PointOperators/ImageStretching.html>`_
-
-
-    .. code:: python
-
-        _normalizedValue = (OriginalValue-LowerLimit)/(UpperLimit-LowerLimit)
-
-    Parameters
-    ----------
-    value :
-        The original value. A single value, vector, or array.
-    upper_limit :
-        The upper limit.
-    lower_limit :
-        The lower limit.
-    clip : bool
-        - True: Clips values between 0 and 1 for RGB.
-        - False: Retain the numbers that extends outside 0-1 range.
-    """
-    norm = (value - lower_limit) / (upper_limit - lower_limit)
-    if clip:
-        norm = np.clip(norm, 0, 1)
-    return norm
-
-
-@xr.register_dataset_accessor("FOV")
-class fieldOfViewAccessor:
-    """
-    Create a field-of-view polygon for the GOES data.
-
-    Based on information from the `GOES-R Series Data Book
-    <https://www.goes-r.gov/downloads/resources/documents/GOES-RSeriesDataBook.pdf>`_.
-
-    GLM lense field of view is 16 degree, or +/- 8 degrees (see page 225)
-    ABI full-disk field of view if 17.4 degrees (see page 48)
-    """
-
-    def __init__(self, xarray_obj):
-        self._obj = xarray_obj
-        self._crs = None
-        self._x = None
-        self._y = None
-        self._sat_h = self._obj.goes_imager_projection.perspective_point_height
-        self._imshow_kwargs = None
-
-    @property
-    def crs(self):
-        """Cartopy coordinate reference system for the Satellite."""
-        ds = self._obj
-        if ds.cdm_data_type == "Image":
-            globe_kwargs = dict(
-                semimajor_axis=ds.goes_imager_projection.semi_major_axis,
-                semiminor_axis=ds.goes_imager_projection.semi_minor_axis,
-                inverse_flattening=ds.goes_imager_projection.inverse_flattening,
-            )
-            sat_height = ds.goes_imager_projection.perspective_point_height
-            nadir_lon = ds.geospatial_lat_lon_extent.geospatial_lon_nadir
-            nadir_lat = ds.geospatial_lat_lon_extent.geospatial_lat_nadir
-        elif ds.cdm_data_type == "Point":
-            globe_kwargs = dict(
-                semimajor_axis=ds.goes_lat_lon_projection.semi_major_axis,
-                semiminor_axis=ds.goes_lat_lon_projection.semi_minor_axis,
-                inverse_flattening=ds.goes_lat_lon_projection.inverse_flattening,
-            )
-            sat_height = ds.nominal_satellite_height.item() * 1000
-            nadir_lon = ds.lon_field_of_view.item()
-            nadir_lat = ds.lat_field_of_view.item()
-        # Create a cartopy coordinate reference system (crs)
-        globe = ccrs.Globe(ellipse=None, **globe_kwargs)
-
-        crs = ccrs.Geostationary(
-            central_longitude=nadir_lon,
-            satellite_height=sat_height,
-            globe=globe,
-            sweep_axis="x",
-        )
-
-        return crs
-
-    @property
-    def x(self):
-        """x sweep in crs units (m); x * sat_height"""
-        if self._x is None:
-            self._x = self._obj.x * self._sat_h
-        return self._x
-
-    @property
-    def y(self):
-        """y sweep in crs units (m); x * sat_height"""
-        if self._y is None:
-            self._y = self._obj.y * self._sat_h
-        return self._y
-
-    @property
-    def imshow_kwargs(self):
-        """Key word arguments for plt.imshow for generating images.
-
-        Projection axis must be the coordinate reference system.
-        """
-        if self._imshow_kwargs is None:
-            self._imshow_kwargs = dict(
-                extent=[
-                    self.x.data.min(),
-                    self.x.data.max(),
-                    self.y.data.min(),
-                    self.y.data.max(),
-                ],
-                transform=self._crs,
-                origin="upper",
-                interpolation="none",
-            )
-        return self._imshow_kwargs
-
-    def get_latlon(self):
-        """Get lat/lon of all points"""
-        X, Y = np.meshgrid(self.x, self.y)
-        a = ccrs.PlateCarree().transform_points(self._crs, X, Y)
-        lons, lats, _ = a[:, :, 0], a[:, :, 1], a[:, :, 2]
-
-        self._obj.coords["longitude"] = (("y", "x"), lons)
-        self._obj.coords["latitude"] = (("y", "x"), lats)
-        return self._obj["latitude"], self._obj["longitude"]
-
-    @property
-    def full_disk(self):
-        """
-        Full-disk field of view for the ABI or GLM instruments.
-
-        .. image:: /_static/ABI_field-of-view.png
-
-        .. image:: /_static/GLM_field-of-view.png
-
-        Returns
-        -------
-        shapely.Polygon
-        """
-        ds = self._obj
-
-        # Create polygon of the field of view. This polygon is in
-        # the geostationary crs projection units, and is in meters.
-        # The central point is at 0,0 (not the nadir position), because
-        # we are working in the geostationary projection coordinates
-        # and the center point is 0,0 meters.
-        if ds.title.startswith("ABI"):
-            # Field of view (FOV) in degrees. Reduce just a little to
-            # get all polygon points in the projection plane so cartopy
-            # can plot it correctly.
-            # TODO: Is there a more "correct" way to handle this?
-            sat_height = ds.goes_imager_projection.perspective_point_height
-            FOV_degrees = 17.4
-            FOV_degrees -= 0.06
-            FOV_radius = np.radians(FOV_degrees / 2) * sat_height
-            FOV_polygon = Point(0, 0).buffer(FOV_radius, resolution=160)
-            return FOV_polygon
-        elif ds.title.startswith("GLM"):
-            # Field of view (FOV) of GLM is different than ABI.
-            # Do a little offset to better match boundary from
-            # Rudlosky et al. 2018
-            sat_height = ds.nominal_satellite_height.item() * 1000
-            FOV_degrees = 8 * 2
-            FOV_degrees += 0.15
-            FOV_radius = np.radians(FOV_degrees / 2) * sat_height
-            FOV_polygon = Point(0, 0).buffer(FOV_radius, resolution=160)
-
-            # I haven't found this explained in the documentation yet,
-            # but the GLM field-of-view is not exactly the full circle,
-            # there is a square area cut out of it.
-            # The square FOV width and height is about 15 degrees.
-            cutout_FOV_degrees = 15 / 2
-            cutout_FOV_length = np.radians(cutout_FOV_degrees) * sat_height
-            # Create a square with many points clockwise, starting in bottom left corner
-            side_points = np.linspace(-cutout_FOV_length, cutout_FOV_length, 300)
-            cutout_points = np.array(
-                [(-cutout_FOV_length, i) for i in side_points]
-                + [(i, cutout_FOV_length) for i in side_points]
-                + [(cutout_FOV_length, i) for i in side_points][::-1]
-                + [(i, -cutout_FOV_length) for i in side_points][::-1]
-            )
-            cutout = Polygon(cutout_points)
-            FOV_polygon = FOV_polygon.intersection(cutout)
-            return FOV_polygon
-
-    @property
-    def domain(self):
-        """
-        Field of view for the ABI domain (CONUS or MesoScale).
-
-        .. image:: /_static/ABI_field-of-view_16dom.png
-
-        .. image:: /_static/ABI_field-of-view_16M1M2.png
-
-        .. image:: /_static/ABI_field-of-view_17dom.png
-
-        Returns
-        -------
-        shapely.Polygon
-        """
-        ds = self._obj
-        assert ds.title.startswith(
-            "ABI"
-        ), "Domain polygon only available for ABI CONUS and Mesoscale files."
-        sat_height = ds.goes_imager_projection.perspective_point_height
-        # Trim out domain FOV from the full disk (this is necessary for GOES-16).
-        dom_border = np.array(
-            [(i, ds.y.data[0]) for i in ds.x.data]
-            + [(ds.x.data[-1], i) for i in ds.y.data]
-            + [(i, ds.y.data[-1]) for i in ds.x.data[::-1]]
-            + [(ds.x.data[0], i) for i in ds.y.data[::-1]]
-        )
-        FOV_domain = Polygon(dom_border * sat_height)
-        FOV_domain = FOV_domain.intersection(self.full_disk)
-        return FOV_domain
-
-
-@xr.register_dataset_accessor("rgb")
-class rgbAccessor:
-    def __init__(self, xarray_obj):
-        self._obj = xarray_obj
-        assert (
-            self._obj.title == "ABI L2 Cloud and Moisture Imagery"
-        ), "Dataset must be an ABI L2 Cloud and Moisture Imagery file."
-        self._crs = None
-        self._x = None
-        self._y = None
-        self._sat_h = self._obj.goes_imager_projection.perspective_point_height
-        self._imshow_kwargs = None
-
-    @property
-    def crs(self):
-        """Cartopy coordinate reference system"""
-        if self._crs is None:
-            # Why am I doing this? To cache the values.
-            self._crs = self._obj.FOV.crs
-        return self._crs
-
-    @property
-    def x(self):
-        """x sweep in crs units (m); x * sat_height"""
-        if self._x is None:
-            self._x = self._obj.x * self._sat_h
-        return self._x
-
-    @property
-    def y(self):
-        """y sweep in crs units (m); x * sat_height"""
-        if self._y is None:
-            self._y = self._obj.y * self._sat_h
-        return self._y
-
-    @property
-    def imshow_kwargs(self):
-        """Key word arguments for plt.imshow for generating images.
-
-        Projection axis must be the coordinate reference system.
-        """
-        if self._imshow_kwargs is None:
-            self._imshow_kwargs = dict(
-                extent=[
-                    self.x.data.min(),
-                    self.x.data.max(),
-                    self.y.data.min(),
-                    self.y.data.max(),
-                ],
-                transform=self._crs,
-                origin="upper",
-                interpolation="none",
-            )
-        return self._imshow_kwargs
-
-    def get_latlon(self):
-        """Get lat/lon of all points"""
-        X, Y = np.meshgrid(self.x, self.y)
-        a = ccrs.PlateCarree().transform_points(self._crs, X, Y)
-        lons, lats, _ = a[:, :, 0], a[:, :, 1], a[:, :, 2]
-
-        self._obj.coords["longitude"] = (("y", "x"), lons)
-        self._obj.coords["latitude"] = (("y", "x"), lats)
-        return self._obj["latitude"], self._obj["longitude"]
-
-    ####################################################################
-    # Helpers
-    def _load_RGB_channels(self, channels):
-        """
-        Return the R, G, and B arrays for the three channels requested. This
-        function will convert the data any units in Kelvin to Celsius.
-
-        Parameters
-        ----------
-        channels : tuple of size 3
-            A tuple of the channel number for each (R, G, B).
-            For example ``channel=(2, 3, 1)`` is for the true color RGB
-
-        Returns
-        -------
-        A list with three items that are used for R, G, and B.
-        >>> R, G, B = _load_RGB_channels((2,3,1))
-
-        """
-        ds = self._obj
-
-        # Units of each channel requested
-        units = [ds["CMI_C%02d" % c].units for c in channels]
-        RGB = []
-        for u, c in zip(units, channels):
-            if u == "K":
-                # Convert form Kelvin to Celsius                                ## <-- Do I REALLY want to hard-code this in?
-                RGB.append(ds["CMI_C%02d" % c].data - 273.15)
-            else:
-                RGB.append(ds["CMI_C%02d" % c].data)
-        return RGB
-
-    ####################################################################
-    # RGB Recipes
-    def TrueColor(self, gamma=2.2, pseudoGreen=True, night_IR=True):
-        """
-        True Color RGB:
-        (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_CIMSSRGB_v2.pdf>`__ for reference)
-
-        This is similar to the NaturalColor RGB, but uses a different gamma
-        correction and does not apply contrast stretching. I think these
-        images look a little "washed out" when compared to the NaturalColor
-        RGB. So, I would recommend using the NaturalColor RGB.
-
-        For more details on combing RGB and making the psedo green channel, refer to
-        `Bah et al. 2018 <https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2018EA000379>`_.
-
-        .. image:: /_static/TrueColor.png
-
-        .. image:: /_static/gamma_demo_TrueColor.png
-
-        .. image:: /_static/Color-IR_demo.png
-
-        Parameters
-        ----------
-        gamma : float
-            Darken or lighten an image with `gamma correction
-            <https://en.wikipedia.org/wiki/_gamma_correction>`_.
-            Values > 1 will lighten an image.
-            Values < 1 will darken an image.
-        pseudoGreen : bool
-            True: returns the calculated "True" green color
-            False: returns the "veggie" channel
-        night_IR : bool
-            If True, use Clean IR (channel 13) as maximum RGB value overlay
-            so that cold clouds show up at night. (Be aware that some
-            daytime clouds might appear brighter).
-
-
-        """
-        ds = self._obj
-
-        # Load the three channels into appropriate R, G, and B variables
-        R, G, B = self._load_RGB_channels((2, 3, 1))
-
-        # Apply range limits for each channel. RGB values must be between 0 and 1
-        R = np.clip(R, 0, 1)
-        G = np.clip(G, 0, 1)
-        B = np.clip(B, 0, 1)
-
-        # Apply a gamma correction to each R, G, B channel
-        R = _gamma_correction(R, gamma)
-        G = _gamma_correction(G, gamma)
-        B = _gamma_correction(B, gamma)
-
-        if pseudoGreen:
-            # Calculate the "True" Green
-            G = 0.45 * R + 0.1 * G + 0.45 * B
-            G = np.clip(G, 0, 1)
-
-        if night_IR:
-            # Load the Clean IR channel
-            IR = ds["CMI_C13"]
-            # _normalize between a range and clip
-            IR = _normalize(IR, 90, 313, clip=True)
-            # Invert colors so cold clouds are white
-            IR = 1 - IR
-            # Lessen the brightness of the coldest clouds so they don't
-            # appear so bright when we overlay it on the true color image
-            IR = IR / 1.4
-            # RGB with IR as greyscale
-            RGB = np.dstack([np.maximum(R, IR), np.maximum(G, IR), np.maximum(B, IR)])
-        else:
-            RGB = np.dstack([R, G, B])
-
-        ds["TrueColor"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["TrueColor"].attrs[
-            "Quick Guide"
-        ] = "http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_CIMSSRGB_v2.pdf"
-        ds["TrueColor"].attrs["long_name"] = "True Color"
-
-        return ds["TrueColor"]
-
-    def NaturalColor(self, gamma=0.8, pseudoGreen=True, night_IR=False):
-        """
-        Natural Color RGB based on CIMSS method. Thanks Rick Kohrs!
-        (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_CIMSSRGB_v2.pdf>`__ for reference)
-
-        Check out Rick Kohrs `merged GOES images <https://www.ssec.wisc.edu/~rickk/local-noon.html>`_.
-
-        This NaturalColor RGB is *very* similar to the TrueColor RGB but
-        uses slightly different contrast stretches and ranges.
-
-        For more details on combing RGB and making the psedo green channel, refer to
-        `Bah et al. 2018 <https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2018EA000379>`_.
-
-        .. image:: /_static/NaturalColor.png
-
-        .. image:: /_static/gamma_demo_NaturalColor-PsuedoGreen.png
-
-        .. image:: /_static/gamma_demo_NaturalColor-VeggieGreen.png
-
-        .. image:: /_static/Color-IR_demo.png
-
-        Parameters
-        ----------
-        gamma : float
-            Darken or lighten an image with `gamma correction
-            <https://en.wikipedia.org/wiki/_gamma_correction>`_.
-            Values > 1 will lighten an image.
-            Values < 1 will darken an image.
-        night_IR : bool
-            If True, use Clean IR (channel 13) as maximum RGB value overlay
-            so that cold clouds show up at night. (Be aware that some
-            daytime clouds might appear brighter).
-
-        """
-        ds = self._obj
-
-        def breakpoint_stretch(C, breakpoint):
-            """
-            Contrast stretching by break point (number provided by Rick Kohrs)
-            """
-            lower = _normalize(C, 0, 10)  # Low end
-            upper = _normalize(C, 10, 255)  # High end
-
-            # Combine the two datasets
-            # This works because if upper=1 and lower==.7, then
-            # that means the upper value was out of range and the
-            # value for the lower pass was used instead.
-            combined = np.minimum(lower, upper)
-
-            return combined
-
-        # Load the three channels into appropriate R, G, and B variables
-        R, G, B = self._load_RGB_channels((2, 3, 1))
-
-        # Apply range limits for each channel. RGB values must be between 0 and 1
-        R = np.clip(R, 0, 1)
-        G = np.clip(G, 0, 1)
-        B = np.clip(B, 0, 1)
-
-        if pseudoGreen:
-            # Derive pseudo Green channel
-            G = 0.45 * R + 0.1 * G + 0.45 * B
-            G = np.clip(G, 0, 1)
-
-        # Convert Albedo to Brightness, ranging from 0-255 K
-        # (numbers based on email from Rick Kohrs)
-        R = np.sqrt(R * 100) * 25.5
-        G = np.sqrt(G * 100) * 25.5
-        B = np.sqrt(B * 100) * 25.5
-
-        # Apply contrast stretching based on breakpoints
-        # (numbers based on email form Rick Kohrs)
-        R = breakpoint_stretch(R, 33)
-        G = breakpoint_stretch(G, 40)
-        B = breakpoint_stretch(B, 50)
-
-        if night_IR:
-            # Load the Clean IR channel
-            IR = ds["CMI_C13"]
-            # _normalize between a range and clip
-            IR = _normalize(IR, 90, 313, clip=True)
-            # Invert colors so cold clouds are white
-            IR = 1 - IR
-            # Lessen the brightness of the coldest clouds so they don't
-            # appear so bright when we overlay it on the true color image
-            IR = IR / 1.4
-            # Overlay IR channel, as greyscale image (use IR in R, G, and B)
-            RGB = np.dstack([np.maximum(R, IR), np.maximum(G, IR), np.maximum(B, IR)])
-        else:
-            RGB = np.dstack([R, G, B])
-
-        # Apply a gamma correction to the image
-        RGB = _gamma_correction(RGB, gamma)
-
-        ds["NaturalColor"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["NaturalColor"].attrs[
-            "Quick Guide"
-        ] = "http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_CIMSSRGB_v2.pdf"
-        ds["NaturalColor"].attrs["long_name"] = "Natural Color"
-
-        return ds["NaturalColor"]
-
-    def FireTemperature(self):
-        """
-        Fire Temperature RGB:
-        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Fire_Temperature_RGB.pdf>`__ for reference)
-
-        .. image:: /_static/FireTemperature.png
-
-
-        """
-        ds = self._obj
-
-        # Load the three channels into appropriate R, G, and B variables
-        R, G, B = self._load_RGB_channels((7, 6, 5))
-
-        # _normalize each channel by the appropriate range of values (clipping happens in function)
-        R = _normalize(R, 273, 333)
-        G = _normalize(G, 0, 1)
-        B = _normalize(B, 0, 0.75)
-
-        # Apply the gamma correction to Red channel.
-        #   corrected_value = value^(1/gamma)
-        gamma = 0.4
-        R = _gamma_correction(R, gamma)
-
-        # The final RGB array :)
-        RGB = np.dstack([R, G, B])
-
-        ds["FireTemperature"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["FireTemperature"].attrs[
-            "Quick Guide"
-        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/Fire_Temperature_RGB.pdf"
-        ds["FireTemperature"].attrs["long_name"] = "Fire Temperature"
-
-        return ds["FireTemperature"]
-
-    def AirMass(self):
-        """
-        Air Mass RGB:
-        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_AirMassRGB_final.pdf>`__ for reference)
-
-        .. image:: /_static/AirMass.png
-
-
-        """
-        ds = self._obj
-
-        # Load the three channels into appropriate R, G, and B variables
-        R = ds["CMI_C08"].data - ds["CMI_C10"].data
-        G = ds["CMI_C12"].data - ds["CMI_C13"].data
-        B = ds["CMI_C08"].data - 273.15  # remember to convert to Celsius
-
-        # _normalize each channel by the appropriate range of values. e.g. R = (R-minimum)/(maximum-minimum)
-        R = _normalize(R, -26.2, 0.6)
-        G = _normalize(G, -42.2, 6.7)
-        B = _normalize(B, -64.65, -29.25)
-
-        # Invert B
-        B = 1 - B
-
-        # The final RGB array :)
-        RGB = np.dstack([R, G, B])
-
-        ds["AirMass"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["AirMass"].attrs[
-            "Quick Guide"
-        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_AirMassRGB_final.pdf"
-        ds["AirMass"].attrs["long_name"] = "Air Mass"
-
-        return ds["AirMass"]
-
-    def DayCloudPhase(self):
-        """
-        Day Cloud Phase Distinction RGB:
-        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Day_Cloud_Phase_Distinction.pdf>`__ for reference)
-
-        .. image:: /_static/DayCloudPhase.png
-
-
-        """
-        ds = self._obj
-
-        # Load the three channels into appropriate R, G, and B variables
-        R, G, B = self._load_RGB_channels((13, 2, 5))
-
-        # _normalize each channel by the appropriate range of values. (Clipping happens inside function)
-        R = _normalize(R, -53.5, 7.5)
-        G = _normalize(G, 0, 0.78)
-        B = _normalize(B, 0.01, 0.59)
-
-        # Invert R
-        R = 1 - R
-
-        # The final RGB array :)
-        RGB = np.dstack([R, G, B])
-
-        ds["DayCloudPhase"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["DayCloudPhase"].attrs[
-            "Quick Guide"
-        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/Day_Cloud_Phase_Distinction.pdf"
-        ds["DayCloudPhase"].attrs["long_name"] = "Day Cloud Phase"
-
-        return ds["DayCloudPhase"]
-
-    def DayConvection(self):
-        """
-        Day Convection RGB:
-        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DayConvectionRGB_final.pdf>`__ for reference)
-
-        .. image:: /_static/DayConvection.png
-
-
-        """
-        ds = self._obj
-
-        # Load the three channels into appropriate R, G, and B variables
-        # NOTE: Each R, G, B is a channel difference.
-        R = ds["CMI_C08"].data - ds["CMI_C10"].data
-        G = ds["CMI_C07"].data - ds["CMI_C13"].data
-        B = ds["CMI_C05"].data - ds["CMI_C02"].data
-
-        # _normalize each channel by the appropriate range of values.
-        R = _normalize(R, -35, 5)
-        G = _normalize(G, -5, 60)
-        B = _normalize(B, -0.75, 0.25)
-
-        # The final RGB array :)
-        RGB = np.dstack([R, G, B])
-
-        ds["DayConvection"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["DayConvection"].attrs[
-            "Quick Guide"
-        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DayConvectionRGB_final.pdf"
-        ds["DayConvection"].attrs["long_name"] = "Day Convection"
-
-        return ds["DayConvection"]
-
-    def DayCloudConvection(self):
-        """
-        Day Cloud Convection RGB:
-        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_DayCloudConvectionRGB_final.pdf>`__ for reference)
-
-        .. image:: /_static/DayCloudConvection.png
-
-        """
-        ds = self._obj
-
-        # Load the three channels into appropriate R, G, and B variables
-        R, G, B = self._load_RGB_channels((2, 2, 13))
-
-        # _normalize each channel by the appropriate range of values.
-        R = _normalize(R, 0, 1)
-        G = _normalize(G, 0, 1)
-        B = _normalize(B, -70.15, 49.85)
-
-        # Invert B
-        B = 1 - B
-
-        # Apply the gamma correction to Red channel.
-        #   corrected_value = value^(1/gamma)
-        gamma = 1.7
-        R = _gamma_correction(R, gamma)
-        G = _gamma_correction(G, gamma)
-
-        # The final RGB array :)
-        RGB = np.dstack([R, G, B])
-
-        ds["DayCloudConvection"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["DayCloudConvection"].attrs[
-            "Quick Guide"
-        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_DayCloudConvectionRGB_final.pdf"
-        ds["DayCloudConvection"].attrs["long_name"] = "Day Cloud Convection"
-
-        return ds["DayCloudConvection"]
-
-    def DayLandCloud(self):
-        """
-        Day Land Cloud Fire RGB:
-        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_daylandcloudRGB_final.pdf>`__ for reference)
-
-        .. image:: /_static/DayLandCloud.png
-
-
-        """
-        ds = self._obj
-
-        # Load the three channels into appropriate R, G, and B variables
-        R, G, B = self._load_RGB_channels((5, 3, 2))
-
-        # _normalize each channel by the appropriate range of values  e.g. R = (R-minimum)/(maximum-minimum)
-        R = _normalize(R, 0, 0.975)
-        G = _normalize(G, 0, 1.086)
-        B = _normalize(B, 0, 1)
-
-        # The final RGB array :)
-        RGB = np.dstack([R, G, B])
-
-        ds["DayLandCloud"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["DayLandCloud"].attrs[
-            "Quick Guide"
-        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_daylandcloudRGB_final.pdf"
-        ds["DayLandCloud"].attrs["long_name"] = "Day Land Cloud"
-
-        return ds["DayLandCloud"]
-
-    def DayLandCloudFire(self):
-        """
-        Day Land Cloud Fire RGB:
-        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DayLandCloudFireRGB_final.pdf>`__ for reference)
-
-        .. image:: /_static/DayLandCloudFire.png
-
-
-        """
-        ds = self._obj
-
-        # Load the three channels into appropriate R, G, and B variables
-        R, G, B = self._load_RGB_channels((6, 3, 2))
-
-        # _normalize each channel by the appropriate range of values  e.g. R = (R-minimum)/(maximum-minimum)
-        R = _normalize(R, 0, 1)
-        G = _normalize(G, 0, 1)
-        B = _normalize(B, 0, 1)
-
-        # The final RGB array :)
-        RGB = np.dstack([R, G, B])
-
-        ds["DayLandCloudFire"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["DayLandCloudFire"].attrs[
-            "Quick Guide"
-        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DayLandCloudFireRGB_final.pdf"
-        ds["DayLandCloudFire"].attrs["long_name"] = "Day Land Cloud Fire"
-
-        return ds["DayLandCloud"]
-
-    def WaterVapor(self):
-        """
-        Simple Water Vapor RGB:
-        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Simple_Water_Vapor_RGB.pdf>`__ for reference)
-
-        .. image:: /_static/WaterVapor.png
-
-
-        """
-        ds = self._obj
-
-        # Load the three channels into appropriate R, G, and B variables.
-        R, G, B = self._load_RGB_channels((13, 8, 10))
-
-        # _normalize each channel by the appropriate range of values. e.g. R = (R-minimum)/(maximum-minimum)
-        R = _normalize(R, -70.86, 5.81)
-        G = _normalize(G, -58.49, -30.48)
-        B = _normalize(B, -28.03, -12.12)
-
-        # Invert the colors
-        R = 1 - R
-        G = 1 - G
-        B = 1 - B
-
-        # The final RGB array :)
-        RGB = np.dstack([R, G, B])
-
-        ds["WaterVapor"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["WaterVapor"].attrs[
-            "Quick Guide"
-        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/Simple_Water_Vapor_RGB.pdf"
-        ds["WaterVapor"].attrs["long_name"] = "Water Vapor"
-
-        return ds["WaterVapor"]
-
-    def DifferentialWaterVapor(self):
-        """
-        Differential Water Vapor RGB:
-        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DifferentialWaterVaporRGB_final.pdf>`__ for reference)
-
-        .. image:: /_static/DifferentialWaterVapor.png
-
-
-        """
-        ds = self._obj
-
-        # Load the three channels into appropriate R, G, and B variables.
-        R = ds["CMI_C10"].data - ds["CMI_C08"].data
-        G = ds["CMI_C10"].data - 273.15
-        B = ds["CMI_C08"].data - 273.15
-
-        # _normalize each channel by the appropriate range of values. e.g. R = (R-minimum)/(maximum-minimum)
-        R = _normalize(R, -3, 30)
-        G = _normalize(G, -60, 5)
-        B = _normalize(B, -64.65, -29.25)
-
-        # Gamma correction
-        R = _gamma_correction(R, 0.2587)
-        G = _gamma_correction(G, 0.4)
-        B = _gamma_correction(B, 0.4)
-
-        # Invert the colors
-        R = 1 - R
-        G = 1 - G
-        B = 1 - B
-
-        # The final RGB array :)
-        RGB = np.dstack([R, G, B])
-
-        ds["DifferentialWaterVapor"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["DifferentialWaterVapor"].attrs[
-            "Quick Guide"
-        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DifferentialWaterVaporRGB_final.pdf"
-        ds["DifferentialWaterVapor"].attrs["long_name"] = "Differential Water Vapor"
-
-        return ds["DifferentialWaterVapor"]
-
-    def DaySnowFog(self):
-        """
-        Day Snow-Fog RGB:
-        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_DaySnowFog.pdf>`__ for reference)
-
-        .. image:: /_static/DaySnowFog.png
-
-
-        """
-        ds = self._obj
-
-        # Load the three channels into appropriate R, G, and B variables
-        R = ds["CMI_C03"].data
-        G = ds["CMI_C05"].data
-        B = ds["CMI_C07"].data - ds["CMI_C13"].data
-
-        # _normalize values
-        R = _normalize(R, 0, 1)
-        G = _normalize(G, 0, 0.7)
-        B = _normalize(B, 0, 30)
-
-        # Apply a gamma correction to the image
-        gamma = 1.7
-        R = _gamma_correction(R, gamma)
-        G = _gamma_correction(G, gamma)
-        B = _gamma_correction(B, gamma)
-
-        # The final RGB array :)
-        RGB = np.dstack([R, G, B])
-
-        ds["DaySnowFog"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["DaySnowFog"].attrs[
-            "Quick Guide"
-        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_DaySnowFog.pdf"
-        ds["DaySnowFog"].attrs["long_name"] = "Day Snow Fog"
-
-        return ds["DaySnowFog"]
-
-    def NighttimeMicrophysics(self):
-        """
-        Nighttime Microphysics RGB:
-        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_NtMicroRGB_final.pdf>`__ for reference)
-
-        .. image:: /_static/NighttimeMicrophysics.png
-
-
-        """
-        ds = self._obj
-
-        # Load the three channels into appropriate R, G, and B variables
-        R = ds["CMI_C15"].data - ds["CMI_C13"].data
-        G = ds["CMI_C13"].data - ds["CMI_C07"].data
-        B = ds["CMI_C13"].data - 273.15
-
-        # _normalize values
-        R = _normalize(R, -6.7, 2.6)
-        G = _normalize(G, -3.1, 5.2)
-        B = _normalize(B, -29.6, 19.5)
-
-        # The final RGB array :)
-        RGB = np.dstack([R, G, B])
-
-        ds["NighttimeMicrophysics"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["NighttimeMicrophysics"].attrs[
-            "Quick Guide"
-        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_NtMicroRGB_final.pdf"
-        ds["NighttimeMicrophysics"].attrs["long_name"] = "Nighttime Microphysics"
-
-        return ds["NighttimeMicrophysics"]
-
-    def Dust(self):
-        """
-        SulfurDioxide RGB:
-        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Dust_RGB_Quick_Guide.pdf>`__ for reference)
-
-        .. image:: /_static/Dust.png
-
-
-        """
-        ds = self._obj
-
-        # Load the three channels into appropriate R, G, and B variables
-        R = ds["CMI_C15"].data - ds["CMI_C13"].data
-        G = ds["CMI_C14"].data - ds["CMI_C11"].data
-        B = ds["CMI_C13"].data - 273.15
-
-        # _normalize values
-        R = _normalize(R, -6.7, 2.6)
-        G = _normalize(G, -0.5, 20)
-        B = _normalize(B, -11.95, 15.55)
-
-        # Apply a gamma correction to the image
-        gamma = 2.5
-        G = _gamma_correction(G, gamma)
-
-        # The final RGB array :)
-        RGB = np.dstack([R, G, B])
-
-        ds["Dust"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["Dust"].attrs[
-            "Quick Guide"
-        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/Dust_RGB_Quick_Guide.pdf"
-        ds["Dust"].attrs["long_name"] = "Dust"
-
-        return ds["Dust"]
-
-    def SulfurDioxide(self):
-        """
-        SulfurDioxide RGB:
-        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Quick_Guide_SO2_RGB.pdf>`__ for reference)
-
-        .. image:: /_static/SulfurDioxide.png
-
-
-        """
-        ds = self._obj
-
-        # Load the three channels into appropriate R, G, and B variables
-        R = ds["CMI_C09"].data - ds["CMI_C10"].data
-        G = ds["CMI_C13"].data - ds["CMI_C11"].data
-        B = ds["CMI_C07"].data - 273.15
-
-        # _normalize values
-        R = _normalize(R, -4, 2)
-        G = _normalize(G, -4, 5)
-        B = _normalize(B, -30.1, 29.8)
-
-        # The final RGB array :)
-        RGB = np.dstack([R, G, B])
-
-        ds["SulfurDioxide"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["SulfurDioxide"].attrs[
-            "Quick Guide"
-        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/Quick_Guide_SO2_RGB.pdf"
-        ds["SulfurDioxide"].attrs["long_name"] = "Sulfur Dioxide"
-
-        return ds["SulfurDioxide"]
-
-    def Ash(self):
-        """
-        Ash RGB:
-        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/GOES_Ash_RGB.pdf>`__ for reference)
-
-        .. image:: /_static/Ash.png
-
-
-        """
-        ds = self._obj
-
-        # Load the three channels into appropriate R, G, and B variables
-        R = ds["CMI_C15"].data - ds["CMI_C13"].data
-        G = ds["CMI_C14"].data - ds["CMI_C11"].data
-        B = ds["CMI_C13"].data - 273.15
-
-        # _normalize values
-        R = _normalize(R, -6.7, 2.6)
-        G = _normalize(G, -6, 6.3)
-        B = _normalize(B, -29.55, 29.25)
-
-        # The final RGB array :)
-        RGB = np.dstack([R, G, B])
-
-        ds["Ash"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["Ash"].attrs[
-            "Quick Guide"
-        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/GOES_Ash_RGB.pdf"
-        ds["Ash"].attrs["long_name"] = "Ash"
-
-        return ds["Ash"]
-
-    def SplitWindowDifference(self):
-        """
-        Split Window Difference RGB (greyscale):
-        (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_SplitWindowDifference.pdf>`__ for reference)
-
-        .. image:: /_static/SplitWindowDifference.png
-
-
-        """
-        ds = self._obj
-
-        # Load the three channels into appropriate R, G, and B variables
-        data = ds["CMI_C15"].data - ds["CMI_C13"].data
-
-        # _normalize values
-        data = _normalize(data, -10, 10)
-
-        # The final RGB array :)
-        RGB = np.dstack([data, data, data])
-
-        ds["SplitWindowDifference"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["SplitWindowDifference"].attrs[
-            "Quick Guide"
-        ] = "http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_SplitWindowDifference.pdf"
-        ds["SplitWindowDifference"].attrs["long_name"] = "Split Window Difference"
-
-        return ds["SplitWindowDifference"]
-
-    def NightFogDifference(self):
-        """
-        Night Fog Difference RGB (greyscale):
-        (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_NightFogBTD.pdf>`__ for reference)
-
-        .. image:: /_static/NightFogDifference.png
-
-
-        """
-        ds = self._obj
-
-        # Load the three channels into appropriate R, G, and B variables
-        data = ds["CMI_C13"].data - ds["CMI_C07"].data
-
-        # _normalize values
-        data = _normalize(data, -90, 15)
-
-        # Invert data
-        data = 1 - data
-
-        # The final RGB array :)
-        RGB = np.dstack([data, data, data])
-
-        ds["NightFogDifference"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["NightFogDifference"].attrs[
-            "Quick Guide"
-        ] = "http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_NightFogBTD.pdf"
-        ds["NightFogDifference"].attrs["long_name"] = "NightFogDifference"
-
-        return ds["NightFogDifference"]
-
-    def RocketPlume(self, night=False):
-        """
-        Rocket Plume RGB
-
-        For identifying rocket launches.
-
-        See `this blog <https://cimss.ssec.wisc.edu/satellite-blog/archives/41335>`__ and
-        the `Quick Guide <https://cimss.ssec.wisc.edu/satellite-blog/images/2021/06/QuickGuide_Template_GOESRBanner_Rocket_Plume.pdf>`__
-        for reference
-
-        .. image:: /_static/RocketPlume.png
-
-        Parameters
-        ----------
-        night : bool
-            If the area is in night, turn this on to use a different channel
-            than the daytime application.
-
-
-        """
-        ds = self._obj
-
-        # Load the three channels into appropriate R, G, and B variables
-        R = ds["CMI_C07"].data
-        G = ds["CMI_C08"].data
-        if not night:
-            B = ds["CMI_C02"].data
-        else:
-            B = ds["CMI_C05"].data
-
-        # _normalize values
-        R = _normalize(R, 273, 338)
-        G = _normalize(G, 233, 253)
-        B = _normalize(B, 0, 0.80)
-
-        # The final RGB array :)
-        RGB = np.dstack([R, G, B])
-
-        ds["RocketPlume"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["RocketPlume"].attrs[
-            "Quick Guide"
-        ] = "https://cimss.ssec.wisc.edu/satellite-blog/images/2021/06/QuickGuide_Template_GOESRBanner_Rocket_Plume.pdf"
-        ds["RocketPlume"].attrs["long_name"] = "Rocket Plume"
-
-        return ds["RocketPlume"]
-
-    def NormalizedBurnRatio(self):
-        """
-        Normalized Burn Ratio
-
-        **THIS FUNCTION IS NOT FULLY DEVELOPED. Need more info.**
-
-        NBR= (0.86 µm – 2.2 µm)/(0.86 um + 2.2 um)
-
-
-        https://ntrs.nasa.gov/citations/20190030825
-
-        """
-        warnings.warn(
-            "THE `NormalizedBurnRatio` FUNCTION IS NOT FULLY DEVELOPED. NEED MORE INFO."
-        )
-        ds = self._obj
-
-        # Load the three channels into appropriate R, G, and B variables
-        C3 = ds["CMI_C03"].data
-        C6 = ds["CMI_C06"].data
-        data = (C3 - C6) / (C3 + C6)
-
-        # Invert data
-        # data = 1-data
-
-        # The final RGB array :)
-        RGB = np.dstack([data, data, data])
-
-        ds["NormalizedBurnRatio"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"]
-        ds["NormalizedBurnRatio"].attrs[
-            "Quick Guide"
-        ] = "https://ntrs.nasa.gov/citations/20190030825"
-        ds["NormalizedBurnRatio"].attrs["long_name"] = "Normalized Burn Ratio"
-
-        return ds["NormalizedBurnRatio"]
+## Brian Blaylock
+## July 9, 2021
+
+"""
+===========
+RGB Recipes
+===========
+
+RGB Recipes for the GOES Advanced Baseline Imager.
+
+More about xarray accessors:
+http://xarray.pydata.org/en/stable/internals/extending-xarray.html?highlight=extending#
+"""
+
+import warnings
+
+import cartopy.crs as ccrs
+import numpy as np
+import xarray as xr
+from shapely.geometry import Point, Polygon
+
+
+########################
+# Image Processing Tools
+def _gamma_correction(a, gamma, verbose=False):
+    """
+    Darken or lighten an image with `gamma correction
+    <https://en.wikipedia.org/wiki/_gamma_correction>`_.
+
+    Parameters
+    ----------
+    a : array-like
+        An array of values, typically the RGB array of values in
+        an image.
+    gamma : float
+        Gamma value to decode the image by.
+        Values > 1 will lighten an image.
+        Values < 1 will darken an image.
+    """
+    if verbose:
+        if gamma > 1:
+            print("Gamma Correction: 🌔 Lighten image")
+        elif gamma < 1:
+            print("Gamma Correction: 🌒 Darken image")
+        else:
+            print("Gamma Correction: 🌓 Gamma=1. No correction made.")
+            return a
+
+    # Gamma decoding formula
+    return np.power(a, 1 / gamma)
+
+
+def _normalize(value, lower_limit, upper_limit, clip=True):
+    """
+    Normalize values between an upper and lower limit between 0 and 1.
+
+    Normalize between a lower and upper limit. In other words, it
+    converts your number to a value in the range between 0 and 1.
+    Follows `normalization formula
+    <https://stats.stackexchange.com/a/70807/220885>`_
+
+    This is the same concept as `contrast or histogram stretching
+    <https://staff.fnwi.uva.nl/r.vandenboomgaard/IPCV20162017/LectureNotes/IP/PointOperators/ImageStretching.html>`_
+
+
+    .. code:: python
+
+        _normalizedValue = (OriginalValue-LowerLimit)/(UpperLimit-LowerLimit)
+
+    Parameters
+    ----------
+    value :
+        The original value. A single value, vector, or array.
+    upper_limit :
+        The upper limit.
+    lower_limit :
+        The lower limit.
+    clip : bool
+        - True: Clips values between 0 and 1 for RGB.
+        - False: Retain the numbers that extends outside 0-1 range.
+    """
+    norm = (value - lower_limit) / (upper_limit - lower_limit)
+    if clip:
+        norm = np.clip(norm, 0, 1)
+    return norm
+
+
+@xr.register_dataset_accessor("FOV")
+class fieldOfViewAccessor:
+    """
+    Create a field-of-view polygon for the GOES data.
+
+    Based on information from the `GOES-R Series Data Book
+    <https://www.goes-r.gov/downloads/resources/documents/GOES-RSeriesDataBook.pdf>`_.
+
+    GLM lense field of view is 16 degree, or +/- 8 degrees (see page 225)
+    ABI full-disk field of view if 17.4 degrees (see page 48)
+    """
+
+    def __init__(self, xarray_obj):
+        self._obj = xarray_obj
+        self._crs = None
+        self._x = None
+        self._y = None
+        self._sat_h = self._obj.goes_imager_projection.perspective_point_height
+        self._imshow_kwargs = None
+
+    @property
+    def crs(self):
+        """Cartopy coordinate reference system for the Satellite."""
+        ds = self._obj
+        if ds.cdm_data_type == "Image":
+            globe_kwargs = dict(
+                semimajor_axis=ds.goes_imager_projection.semi_major_axis,
+                semiminor_axis=ds.goes_imager_projection.semi_minor_axis,
+                inverse_flattening=ds.goes_imager_projection.inverse_flattening,
+            )
+            sat_height = ds.goes_imager_projection.perspective_point_height
+            nadir_lon = ds.geospatial_lat_lon_extent.geospatial_lon_nadir
+            nadir_lat = ds.geospatial_lat_lon_extent.geospatial_lat_nadir
+        elif ds.cdm_data_type == "Point":
+            globe_kwargs = dict(
+                semimajor_axis=ds.goes_lat_lon_projection.semi_major_axis,
+                semiminor_axis=ds.goes_lat_lon_projection.semi_minor_axis,
+                inverse_flattening=ds.goes_lat_lon_projection.inverse_flattening,
+            )
+            sat_height = ds.nominal_satellite_height.item() * 1000
+            nadir_lon = ds.lon_field_of_view.item()
+            nadir_lat = ds.lat_field_of_view.item()
+        # Create a cartopy coordinate reference system (crs)
+        globe = ccrs.Globe(ellipse=None, **globe_kwargs)
+
+        crs = ccrs.Geostationary(
+            central_longitude=nadir_lon,
+            satellite_height=sat_height,
+            globe=globe,
+            sweep_axis="x",
+        )
+
+        return crs
+
+    @property
+    def x(self):
+        """x sweep in crs units (m); x * sat_height"""
+        if self._x is None:
+            self._x = self._obj.x * self._sat_h
+        return self._x
+
+    @property
+    def y(self):
+        """y sweep in crs units (m); x * sat_height"""
+        if self._y is None:
+            self._y = self._obj.y * self._sat_h
+        return self._y
+
+    @property
+    def imshow_kwargs(self):
+        """Key word arguments for plt.imshow for generating images.
+
+        Projection axis must be the coordinate reference system.
+        """
+        if self._imshow_kwargs is None:
+            self._imshow_kwargs = dict(
+                extent=[
+                    self.x.data.min(),
+                    self.x.data.max(),
+                    self.y.data.min(),
+                    self.y.data.max(),
+                ],
+                transform=self._crs,
+                origin="upper",
+                interpolation="none",
+            )
+        return self._imshow_kwargs
+
+    def get_latlon(self):
+        """Get lat/lon of all points"""
+        X, Y = np.meshgrid(self.x, self.y)
+        a = ccrs.PlateCarree().transform_points(self._crs, X, Y)
+        lons, lats, _ = a[:, :, 0], a[:, :, 1], a[:, :, 2]
+
+        self._obj.coords["longitude"] = (("y", "x"), lons)
+        self._obj.coords["latitude"] = (("y", "x"), lats)
+        return self._obj["latitude"], self._obj["longitude"]
+
+    @property
+    def full_disk(self):
+        """
+        Full-disk field of view for the ABI or GLM instruments.
+
+        .. image:: /_static/ABI_field-of-view.png
+
+        .. image:: /_static/GLM_field-of-view.png
+
+        Returns
+        -------
+        shapely.Polygon
+        """
+        ds = self._obj
+
+        # Create polygon of the field of view. This polygon is in
+        # the geostationary crs projection units, and is in meters.
+        # The central point is at 0,0 (not the nadir position), because
+        # we are working in the geostationary projection coordinates
+        # and the center point is 0,0 meters.
+        if ds.title.startswith("ABI"):
+            # Field of view (FOV) in degrees. Reduce just a little to
+            # get all polygon points in the projection plane so cartopy
+            # can plot it correctly.
+            # TODO: Is there a more "correct" way to handle this?
+            sat_height = ds.goes_imager_projection.perspective_point_height
+            FOV_degrees = 17.4
+            FOV_degrees -= 0.06
+            FOV_radius = np.radians(FOV_degrees / 2) * sat_height
+            FOV_polygon = Point(0, 0).buffer(FOV_radius, resolution=160)
+            return FOV_polygon
+        elif ds.title.startswith("GLM"):
+            # Field of view (FOV) of GLM is different than ABI.
+            # Do a little offset to better match boundary from
+            # Rudlosky et al. 2018
+            sat_height = ds.nominal_satellite_height.item() * 1000
+            FOV_degrees = 8 * 2
+            FOV_degrees += 0.15
+            FOV_radius = np.radians(FOV_degrees / 2) * sat_height
+            FOV_polygon = Point(0, 0).buffer(FOV_radius, resolution=160)
+
+            # I haven't found this explained in the documentation yet,
+            # but the GLM field-of-view is not exactly the full circle,
+            # there is a square area cut out of it.
+            # The square FOV width and height is about 15 degrees.
+            cutout_FOV_degrees = 15 / 2
+            cutout_FOV_length = np.radians(cutout_FOV_degrees) * sat_height
+            # Create a square with many points clockwise, starting in bottom left corner
+            side_points = np.linspace(-cutout_FOV_length, cutout_FOV_length, 300)
+            cutout_points = np.array(
+                [(-cutout_FOV_length, i) for i in side_points]
+                + [(i, cutout_FOV_length) for i in side_points]
+                + [(cutout_FOV_length, i) for i in side_points][::-1]
+                + [(i, -cutout_FOV_length) for i in side_points][::-1]
+            )
+            cutout = Polygon(cutout_points)
+            FOV_polygon = FOV_polygon.intersection(cutout)
+            return FOV_polygon
+
+    @property
+    def domain(self):
+        """
+        Field of view for the ABI domain (CONUS or MesoScale).
+
+        .. image:: /_static/ABI_field-of-view_16dom.png
+
+        .. image:: /_static/ABI_field-of-view_16M1M2.png
+
+        .. image:: /_static/ABI_field-of-view_17dom.png
+
+        Returns
+        -------
+        shapely.Polygon
+        """
+        ds = self._obj
+        assert ds.title.startswith(
+            "ABI"
+        ), "Domain polygon only available for ABI CONUS and Mesoscale files."
+        sat_height = ds.goes_imager_projection.perspective_point_height
+        # Trim out domain FOV from the full disk (this is necessary for GOES-16).
+        dom_border = np.array(
+            [(i, ds.y.data[0]) for i in ds.x.data]
+            + [(ds.x.data[-1], i) for i in ds.y.data]
+            + [(i, ds.y.data[-1]) for i in ds.x.data[::-1]]
+            + [(ds.x.data[0], i) for i in ds.y.data[::-1]]
+        )
+        FOV_domain = Polygon(dom_border * sat_height)
+        FOV_domain = FOV_domain.intersection(self.full_disk)
+        return FOV_domain
+
+
+@xr.register_dataset_accessor("rgb")
+class rgbAccessor:
+    def __init__(self, xarray_obj):
+        self._obj = xarray_obj
+        assert (
+            self._obj.title == "ABI L2 Cloud and Moisture Imagery"
+        ), "Dataset must be an ABI L2 Cloud and Moisture Imagery file."
+        self._crs = None
+        self._x = None
+        self._y = None
+        self._sat_h = self._obj.goes_imager_projection.perspective_point_height
+        self._imshow_kwargs = None
+
+    @property
+    def crs(self):
+        """Cartopy coordinate reference system"""
+        if self._crs is None:
+            # Why am I doing this? To cache the values.
+            self._crs = self._obj.FOV.crs
+        return self._crs
+
+    @property
+    def x(self):
+        """x sweep in crs units (m); x * sat_height"""
+        if self._x is None:
+            self._x = self._obj.x * self._sat_h
+        return self._x
+
+    @property
+    def y(self):
+        """y sweep in crs units (m); x * sat_height"""
+        if self._y is None:
+            self._y = self._obj.y * self._sat_h
+        return self._y
+
+    @property
+    def imshow_kwargs(self):
+        """Key word arguments for plt.imshow for generating images.
+
+        Projection axis must be the coordinate reference system.
+        """
+        if self._imshow_kwargs is None:
+            self._imshow_kwargs = dict(
+                extent=[
+                    self.x.data.min(),
+                    self.x.data.max(),
+                    self.y.data.min(),
+                    self.y.data.max(),
+                ],
+                transform=self._crs,
+                origin="upper",
+                interpolation="none",
+            )
+        return self._imshow_kwargs
+
+    def get_latlon(self):
+        """Get lat/lon of all points"""
+        X, Y = np.meshgrid(self.x, self.y)
+        a = ccrs.PlateCarree().transform_points(self._crs, X, Y)
+        lons, lats, _ = a[:, :, 0], a[:, :, 1], a[:, :, 2]
+
+        self._obj.coords["longitude"] = (("y", "x"), lons)
+        self._obj.coords["latitude"] = (("y", "x"), lats)
+        return self._obj["latitude"], self._obj["longitude"]
+
+    ####################################################################
+    # Helpers
+    def _load_RGB_channels(self, channels):
+        """
+        Return the R, G, and B arrays for the three channels requested. This
+        function will convert the data any units in Kelvin to Celsius.
+
+        Parameters
+        ----------
+        channels : tuple of size 3
+            A tuple of the channel number for each (R, G, B).
+            For example ``channel=(2, 3, 1)`` is for the true color RGB
+
+        Returns
+        -------
+        A list with three items that are used for R, G, and B.
+        >>> R, G, B = _load_RGB_channels((2,3,1))
+
+        """
+        ds = self._obj
+
+        # Units of each channel requested
+        units = [ds["CMI_C%02d" % c].units for c in channels]
+        RGB = []
+        for u, c in zip(units, channels):
+            if u == "K":
+                # Convert form Kelvin to Celsius                                ## <-- Do I REALLY want to hard-code this in?
+                RGB.append(ds["CMI_C%02d" % c].data - 273.15)
+            else:
+                RGB.append(ds["CMI_C%02d" % c].data)
+        return RGB
+
+    ####################################################################
+    # RGB Recipes
+    def TrueColor(self, gamma=2.2, pseudoGreen=True, night_IR=True):
+        """
+        True Color RGB:
+        (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_CIMSSRGB_v2.pdf>`__ for reference)
+
+        This is similar to the NaturalColor RGB, but uses a different gamma
+        correction and does not apply contrast stretching. I think these
+        images look a little "washed out" when compared to the NaturalColor
+        RGB. So, I would recommend using the NaturalColor RGB.
+
+        For more details on combing RGB and making the psedo green channel, refer to
+        `Bah et al. 2018 <https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2018EA000379>`_.
+
+        .. image:: /_static/TrueColor.png
+
+        .. image:: /_static/gamma_demo_TrueColor.png
+
+        .. image:: /_static/Color-IR_demo.png
+
+        Parameters
+        ----------
+        gamma : float
+            Darken or lighten an image with `gamma correction
+            <https://en.wikipedia.org/wiki/_gamma_correction>`_.
+            Values > 1 will lighten an image.
+            Values < 1 will darken an image.
+        pseudoGreen : bool
+            True: returns the calculated "True" green color
+            False: returns the "veggie" channel
+        night_IR : bool
+            If True, use Clean IR (channel 13) as maximum RGB value overlay
+            so that cold clouds show up at night. (Be aware that some
+            daytime clouds might appear brighter).
+
+
+        """
+        ds = self._obj
+
+        # Load the three channels into appropriate R, G, and B variables
+        R, G, B = self._load_RGB_channels((2, 3, 1))
+
+        # Apply range limits for each channel. RGB values must be between 0 and 1
+        R = np.clip(R, 0, 1)
+        G = np.clip(G, 0, 1)
+        B = np.clip(B, 0, 1)
+
+        # Apply a gamma correction to each R, G, B channel
+        R = _gamma_correction(R, gamma)
+        G = _gamma_correction(G, gamma)
+        B = _gamma_correction(B, gamma)
+
+        if pseudoGreen:
+            # Calculate the "True" Green
+            G = 0.45 * R + 0.1 * G + 0.45 * B
+            G = np.clip(G, 0, 1)
+
+        if night_IR:
+            # Load the Clean IR channel
+            IR = ds["CMI_C13"]
+            # _normalize between a range and clip
+            IR = _normalize(IR, 90, 313, clip=True)
+            # Invert colors so cold clouds are white
+            IR = 1 - IR
+            # Lessen the brightness of the coldest clouds so they don't
+            # appear so bright when we overlay it on the true color image
+            IR = IR / 1.4
+            # RGB with IR as greyscale
+            RGB = np.dstack([np.maximum(R, IR), np.maximum(G, IR), np.maximum(B, IR)])
+        else:
+            RGB = np.dstack([R, G, B])
+
+        ds["TrueColor"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["TrueColor"].attrs[
+            "Quick Guide"
+        ] = "http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_CIMSSRGB_v2.pdf"
+        ds["TrueColor"].attrs["long_name"] = "True Color"
+
+        return ds["TrueColor"]
+
+    def NaturalColor(self, gamma=0.8, pseudoGreen=True, night_IR=False):
+        """
+        Natural Color RGB based on CIMSS method. Thanks Rick Kohrs!
+        (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_CIMSSRGB_v2.pdf>`__ for reference)
+
+        Check out Rick Kohrs `merged GOES images <https://www.ssec.wisc.edu/~rickk/local-noon.html>`_.
+
+        This NaturalColor RGB is *very* similar to the TrueColor RGB but
+        uses slightly different contrast stretches and ranges.
+
+        For more details on combing RGB and making the psedo green channel, refer to
+        `Bah et al. 2018 <https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2018EA000379>`_.
+
+        .. image:: /_static/NaturalColor.png
+
+        .. image:: /_static/gamma_demo_NaturalColor-PsuedoGreen.png
+
+        .. image:: /_static/gamma_demo_NaturalColor-VeggieGreen.png
+
+        .. image:: /_static/Color-IR_demo.png
+
+        Parameters
+        ----------
+        gamma : float
+            Darken or lighten an image with `gamma correction
+            <https://en.wikipedia.org/wiki/_gamma_correction>`_.
+            Values > 1 will lighten an image.
+            Values < 1 will darken an image.
+        night_IR : bool
+            If True, use Clean IR (channel 13) as maximum RGB value overlay
+            so that cold clouds show up at night. (Be aware that some
+            daytime clouds might appear brighter).
+
+        """
+        ds = self._obj
+
+        def breakpoint_stretch(C, breakpoint):
+            """
+            Contrast stretching by break point (number provided by Rick Kohrs)
+            """
+            lower = _normalize(C, 0, 10)  # Low end
+            upper = _normalize(C, 10, 255)  # High end
+
+            # Combine the two datasets
+            # This works because if upper=1 and lower==.7, then
+            # that means the upper value was out of range and the
+            # value for the lower pass was used instead.
+            combined = np.minimum(lower, upper)
+
+            return combined
+
+        # Load the three channels into appropriate R, G, and B variables
+        R, G, B = self._load_RGB_channels((2, 3, 1))
+
+        # Apply range limits for each channel. RGB values must be between 0 and 1
+        R = np.clip(R, 0, 1)
+        G = np.clip(G, 0, 1)
+        B = np.clip(B, 0, 1)
+
+        if pseudoGreen:
+            # Derive pseudo Green channel
+            G = 0.45 * R + 0.1 * G + 0.45 * B
+            G = np.clip(G, 0, 1)
+
+        # Convert Albedo to Brightness, ranging from 0-255 K
+        # (numbers based on email from Rick Kohrs)
+        R = np.sqrt(R * 100) * 25.5
+        G = np.sqrt(G * 100) * 25.5
+        B = np.sqrt(B * 100) * 25.5
+
+        # Apply contrast stretching based on breakpoints
+        # (numbers based on email form Rick Kohrs)
+        R = breakpoint_stretch(R, 33)
+        G = breakpoint_stretch(G, 40)
+        B = breakpoint_stretch(B, 50)
+
+        if night_IR:
+            # Load the Clean IR channel
+            IR = ds["CMI_C13"]
+            # _normalize between a range and clip
+            IR = _normalize(IR, 90, 313, clip=True)
+            # Invert colors so cold clouds are white
+            IR = 1 - IR
+            # Lessen the brightness of the coldest clouds so they don't
+            # appear so bright when we overlay it on the true color image
+            IR = IR / 1.4
+            # Overlay IR channel, as greyscale image (use IR in R, G, and B)
+            RGB = np.dstack([np.maximum(R, IR), np.maximum(G, IR), np.maximum(B, IR)])
+        else:
+            RGB = np.dstack([R, G, B])
+
+        # Apply a gamma correction to the image
+        RGB = _gamma_correction(RGB, gamma)
+
+        ds["NaturalColor"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["NaturalColor"].attrs[
+            "Quick Guide"
+        ] = "http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_CIMSSRGB_v2.pdf"
+        ds["NaturalColor"].attrs["long_name"] = "Natural Color"
+
+        return ds["NaturalColor"]
+
+    def FireTemperature(self):
+        """
+        Fire Temperature RGB:
+        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Fire_Temperature_RGB.pdf>`__ for reference)
+
+        .. image:: /_static/FireTemperature.png
+
+
+        """
+        ds = self._obj
+
+        # Load the three channels into appropriate R, G, and B variables
+        R, G, B = self._load_RGB_channels((7, 6, 5))
+
+        # _normalize each channel by the appropriate range of values (clipping happens in function)
+        R = _normalize(R, 273, 333)
+        G = _normalize(G, 0, 1)
+        B = _normalize(B, 0, 0.75)
+
+        # Apply the gamma correction to Red channel.
+        #   corrected_value = value^(1/gamma)
+        gamma = 0.4
+        R = _gamma_correction(R, gamma)
+
+        # The final RGB array :)
+        RGB = np.dstack([R, G, B])
+
+        ds["FireTemperature"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["FireTemperature"].attrs[
+            "Quick Guide"
+        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/Fire_Temperature_RGB.pdf"
+        ds["FireTemperature"].attrs["long_name"] = "Fire Temperature"
+
+        return ds["FireTemperature"]
+
+    def AirMass(self):
+        """
+        Air Mass RGB:
+        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_AirMassRGB_final.pdf>`__ for reference)
+
+        .. image:: /_static/AirMass.png
+
+
+        """
+        ds = self._obj
+
+        # Load the three channels into appropriate R, G, and B variables
+        R = ds["CMI_C08"].data - ds["CMI_C10"].data
+        G = ds["CMI_C12"].data - ds["CMI_C13"].data
+        B = ds["CMI_C08"].data - 273.15  # remember to convert to Celsius
+
+        # _normalize each channel by the appropriate range of values. e.g. R = (R-minimum)/(maximum-minimum)
+        R = _normalize(R, -26.2, 0.6)
+        G = _normalize(G, -42.2, 6.7)
+        B = _normalize(B, -64.65, -29.25)
+
+        # Invert B
+        B = 1 - B
+
+        # The final RGB array :)
+        RGB = np.dstack([R, G, B])
+
+        ds["AirMass"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["AirMass"].attrs[
+            "Quick Guide"
+        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_AirMassRGB_final.pdf"
+        ds["AirMass"].attrs["long_name"] = "Air Mass"
+
+        return ds["AirMass"]
+
+    def DayCloudPhase(self):
+        """
+        Day Cloud Phase Distinction RGB:
+        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Day_Cloud_Phase_Distinction.pdf>`__ for reference)
+
+        .. image:: /_static/DayCloudPhase.png
+
+
+        """
+        ds = self._obj
+
+        # Load the three channels into appropriate R, G, and B variables
+        R, G, B = self._load_RGB_channels((13, 2, 5))
+
+        # _normalize each channel by the appropriate range of values. (Clipping happens inside function)
+        R = _normalize(R, -53.5, 7.5)
+        G = _normalize(G, 0, 0.78)
+        B = _normalize(B, 0.01, 0.59)
+
+        # Invert R
+        R = 1 - R
+
+        # The final RGB array :)
+        RGB = np.dstack([R, G, B])
+
+        ds["DayCloudPhase"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["DayCloudPhase"].attrs[
+            "Quick Guide"
+        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/Day_Cloud_Phase_Distinction.pdf"
+        ds["DayCloudPhase"].attrs["long_name"] = "Day Cloud Phase"
+
+        return ds["DayCloudPhase"]
+
+    def DayConvection(self):
+        """
+        Day Convection RGB:
+        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DayConvectionRGB_final.pdf>`__ for reference)
+
+        .. image:: /_static/DayConvection.png
+
+
+        """
+        ds = self._obj
+
+        # Load the three channels into appropriate R, G, and B variables
+        # NOTE: Each R, G, B is a channel difference.
+        R = ds["CMI_C08"].data - ds["CMI_C10"].data
+        G = ds["CMI_C07"].data - ds["CMI_C13"].data
+        B = ds["CMI_C05"].data - ds["CMI_C02"].data
+
+        # _normalize each channel by the appropriate range of values.
+        R = _normalize(R, -35, 5)
+        G = _normalize(G, -5, 60)
+        B = _normalize(B, -0.75, 0.25)
+
+        # The final RGB array :)
+        RGB = np.dstack([R, G, B])
+
+        ds["DayConvection"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["DayConvection"].attrs[
+            "Quick Guide"
+        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DayConvectionRGB_final.pdf"
+        ds["DayConvection"].attrs["long_name"] = "Day Convection"
+
+        return ds["DayConvection"]
+
+    def DayCloudConvection(self):
+        """
+        Day Cloud Convection RGB:
+        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_DayCloudConvectionRGB_final.pdf>`__ for reference)
+
+        .. image:: /_static/DayCloudConvection.png
+
+        """
+        ds = self._obj
+
+        # Load the three channels into appropriate R, G, and B variables
+        R, G, B = self._load_RGB_channels((2, 2, 13))
+
+        # _normalize each channel by the appropriate range of values.
+        R = _normalize(R, 0, 1)
+        G = _normalize(G, 0, 1)
+        B = _normalize(B, -70.15, 49.85)
+
+        # Invert B
+        B = 1 - B
+
+        # Apply the gamma correction to Red channel.
+        #   corrected_value = value^(1/gamma)
+        gamma = 1.7
+        R = _gamma_correction(R, gamma)
+        G = _gamma_correction(G, gamma)
+
+        # The final RGB array :)
+        RGB = np.dstack([R, G, B])
+
+        ds["DayCloudConvection"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["DayCloudConvection"].attrs[
+            "Quick Guide"
+        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_DayCloudConvectionRGB_final.pdf"
+        ds["DayCloudConvection"].attrs["long_name"] = "Day Cloud Convection"
+
+        return ds["DayCloudConvection"]
+
+    def DayLandCloud(self):
+        """
+        Day Land Cloud Fire RGB:
+        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_daylandcloudRGB_final.pdf>`__ for reference)
+
+        .. image:: /_static/DayLandCloud.png
+
+
+        """
+        ds = self._obj
+
+        # Load the three channels into appropriate R, G, and B variables
+        R, G, B = self._load_RGB_channels((5, 3, 2))
+
+        # _normalize each channel by the appropriate range of values  e.g. R = (R-minimum)/(maximum-minimum)
+        R = _normalize(R, 0, 0.975)
+        G = _normalize(G, 0, 1.086)
+        B = _normalize(B, 0, 1)
+
+        # The final RGB array :)
+        RGB = np.dstack([R, G, B])
+
+        ds["DayLandCloud"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["DayLandCloud"].attrs[
+            "Quick Guide"
+        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_daylandcloudRGB_final.pdf"
+        ds["DayLandCloud"].attrs["long_name"] = "Day Land Cloud"
+
+        return ds["DayLandCloud"]
+
+    def DayLandCloudFire(self):
+        """
+        Day Land Cloud Fire RGB:
+        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DayLandCloudFireRGB_final.pdf>`__ for reference)
+
+        .. image:: /_static/DayLandCloudFire.png
+
+
+        """
+        ds = self._obj
+
+        # Load the three channels into appropriate R, G, and B variables
+        R, G, B = self._load_RGB_channels((6, 3, 2))
+
+        # _normalize each channel by the appropriate range of values  e.g. R = (R-minimum)/(maximum-minimum)
+        R = _normalize(R, 0, 1)
+        G = _normalize(G, 0, 1)
+        B = _normalize(B, 0, 1)
+
+        # The final RGB array :)
+        RGB = np.dstack([R, G, B])
+
+        ds["DayLandCloudFire"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["DayLandCloudFire"].attrs[
+            "Quick Guide"
+        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DayLandCloudFireRGB_final.pdf"
+        ds["DayLandCloudFire"].attrs["long_name"] = "Day Land Cloud Fire"
+
+        return ds["DayLandCloudFire"]
+
+    def WaterVapor(self):
+        """
+        Simple Water Vapor RGB:
+        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Simple_Water_Vapor_RGB.pdf>`__ for reference)
+
+        .. image:: /_static/WaterVapor.png
+
+
+        """
+        ds = self._obj
+
+        # Load the three channels into appropriate R, G, and B variables.
+        R, G, B = self._load_RGB_channels((13, 8, 10))
+
+        # _normalize each channel by the appropriate range of values. e.g. R = (R-minimum)/(maximum-minimum)
+        R = _normalize(R, -70.86, 5.81)
+        G = _normalize(G, -58.49, -30.48)
+        B = _normalize(B, -28.03, -12.12)
+
+        # Invert the colors
+        R = 1 - R
+        G = 1 - G
+        B = 1 - B
+
+        # The final RGB array :)
+        RGB = np.dstack([R, G, B])
+
+        ds["WaterVapor"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["WaterVapor"].attrs[
+            "Quick Guide"
+        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/Simple_Water_Vapor_RGB.pdf"
+        ds["WaterVapor"].attrs["long_name"] = "Water Vapor"
+
+        return ds["WaterVapor"]
+
+    def DifferentialWaterVapor(self):
+        """
+        Differential Water Vapor RGB:
+        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DifferentialWaterVaporRGB_final.pdf>`__ for reference)
+
+        .. image:: /_static/DifferentialWaterVapor.png
+
+
+        """
+        ds = self._obj
+
+        # Load the three channels into appropriate R, G, and B variables.
+        R = ds["CMI_C10"].data - ds["CMI_C08"].data
+        G = ds["CMI_C10"].data - 273.15
+        B = ds["CMI_C08"].data - 273.15
+
+        # _normalize each channel by the appropriate range of values. e.g. R = (R-minimum)/(maximum-minimum)
+        R = _normalize(R, -3, 30)
+        G = _normalize(G, -60, 5)
+        B = _normalize(B, -64.65, -29.25)
+
+        # Gamma correction
+        R = _gamma_correction(R, 0.2587)
+        G = _gamma_correction(G, 0.4)
+        B = _gamma_correction(B, 0.4)
+
+        # Invert the colors
+        R = 1 - R
+        G = 1 - G
+        B = 1 - B
+
+        # The final RGB array :)
+        RGB = np.dstack([R, G, B])
+
+        ds["DifferentialWaterVapor"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["DifferentialWaterVapor"].attrs[
+            "Quick Guide"
+        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DifferentialWaterVaporRGB_final.pdf"
+        ds["DifferentialWaterVapor"].attrs["long_name"] = "Differential Water Vapor"
+
+        return ds["DifferentialWaterVapor"]
+
+    def DaySnowFog(self):
+        """
+        Day Snow-Fog RGB:
+        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_DaySnowFog.pdf>`__ for reference)
+
+        .. image:: /_static/DaySnowFog.png
+
+
+        """
+        ds = self._obj
+
+        # Load the three channels into appropriate R, G, and B variables
+        R = ds["CMI_C03"].data
+        G = ds["CMI_C05"].data
+        B = ds["CMI_C07"].data - ds["CMI_C13"].data
+
+        # _normalize values
+        R = _normalize(R, 0, 1)
+        G = _normalize(G, 0, 0.7)
+        B = _normalize(B, 0, 30)
+
+        # Apply a gamma correction to the image
+        gamma = 1.7
+        R = _gamma_correction(R, gamma)
+        G = _gamma_correction(G, gamma)
+        B = _gamma_correction(B, gamma)
+
+        # The final RGB array :)
+        RGB = np.dstack([R, G, B])
+
+        ds["DaySnowFog"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["DaySnowFog"].attrs[
+            "Quick Guide"
+        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_DaySnowFog.pdf"
+        ds["DaySnowFog"].attrs["long_name"] = "Day Snow Fog"
+
+        return ds["DaySnowFog"]
+
+    def NighttimeMicrophysics(self):
+        """
+        Nighttime Microphysics RGB:
+        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_NtMicroRGB_final.pdf>`__ for reference)
+
+        .. image:: /_static/NighttimeMicrophysics.png
+
+
+        """
+        ds = self._obj
+
+        # Load the three channels into appropriate R, G, and B variables
+        R = ds["CMI_C15"].data - ds["CMI_C13"].data
+        G = ds["CMI_C13"].data - ds["CMI_C07"].data
+        B = ds["CMI_C13"].data - 273.15
+
+        # _normalize values
+        R = _normalize(R, -6.7, 2.6)
+        G = _normalize(G, -3.1, 5.2)
+        B = _normalize(B, -29.6, 19.5)
+
+        # The final RGB array :)
+        RGB = np.dstack([R, G, B])
+
+        ds["NighttimeMicrophysics"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["NighttimeMicrophysics"].attrs[
+            "Quick Guide"
+        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_NtMicroRGB_final.pdf"
+        ds["NighttimeMicrophysics"].attrs["long_name"] = "Nighttime Microphysics"
+
+        return ds["NighttimeMicrophysics"]
+
+    def Dust(self):
+        """
+        SulfurDioxide RGB:
+        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Dust_RGB_Quick_Guide.pdf>`__ for reference)
+
+        .. image:: /_static/Dust.png
+
+
+        """
+        ds = self._obj
+
+        # Load the three channels into appropriate R, G, and B variables
+        R = ds["CMI_C15"].data - ds["CMI_C13"].data
+        G = ds["CMI_C14"].data - ds["CMI_C11"].data
+        B = ds["CMI_C13"].data - 273.15
+
+        # _normalize values
+        R = _normalize(R, -6.7, 2.6)
+        G = _normalize(G, -0.5, 20)
+        B = _normalize(B, -11.95, 15.55)
+
+        # Apply a gamma correction to the image
+        gamma = 2.5
+        G = _gamma_correction(G, gamma)
+
+        # The final RGB array :)
+        RGB = np.dstack([R, G, B])
+
+        ds["Dust"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["Dust"].attrs[
+            "Quick Guide"
+        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/Dust_RGB_Quick_Guide.pdf"
+        ds["Dust"].attrs["long_name"] = "Dust"
+
+        return ds["Dust"]
+
+    def SulfurDioxide(self):
+        """
+        SulfurDioxide RGB:
+        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Quick_Guide_SO2_RGB.pdf>`__ for reference)
+
+        .. image:: /_static/SulfurDioxide.png
+
+
+        """
+        ds = self._obj
+
+        # Load the three channels into appropriate R, G, and B variables
+        R = ds["CMI_C09"].data - ds["CMI_C10"].data
+        G = ds["CMI_C13"].data - ds["CMI_C11"].data
+        B = ds["CMI_C07"].data - 273.15
+
+        # _normalize values
+        R = _normalize(R, -4, 2)
+        G = _normalize(G, -4, 5)
+        B = _normalize(B, -30.1, 29.8)
+
+        # The final RGB array :)
+        RGB = np.dstack([R, G, B])
+
+        ds["SulfurDioxide"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["SulfurDioxide"].attrs[
+            "Quick Guide"
+        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/Quick_Guide_SO2_RGB.pdf"
+        ds["SulfurDioxide"].attrs["long_name"] = "Sulfur Dioxide"
+
+        return ds["SulfurDioxide"]
+
+    def Ash(self):
+        """
+        Ash RGB:
+        (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/GOES_Ash_RGB.pdf>`__ for reference)
+
+        .. image:: /_static/Ash.png
+
+
+        """
+        ds = self._obj
+
+        # Load the three channels into appropriate R, G, and B variables
+        R = ds["CMI_C15"].data - ds["CMI_C13"].data
+        G = ds["CMI_C14"].data - ds["CMI_C11"].data
+        B = ds["CMI_C13"].data - 273.15
+
+        # _normalize values
+        R = _normalize(R, -6.7, 2.6)
+        G = _normalize(G, -6, 6.3)
+        B = _normalize(B, -29.55, 29.25)
+
+        # The final RGB array :)
+        RGB = np.dstack([R, G, B])
+
+        ds["Ash"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["Ash"].attrs[
+            "Quick Guide"
+        ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/GOES_Ash_RGB.pdf"
+        ds["Ash"].attrs["long_name"] = "Ash"
+
+        return ds["Ash"]
+
+    def SplitWindowDifference(self):
+        """
+        Split Window Difference RGB (greyscale):
+        (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_SplitWindowDifference.pdf>`__ for reference)
+
+        .. image:: /_static/SplitWindowDifference.png
+
+
+        """
+        ds = self._obj
+
+        # Load the three channels into appropriate R, G, and B variables
+        data = ds["CMI_C15"].data - ds["CMI_C13"].data
+
+        # _normalize values
+        data = _normalize(data, -10, 10)
+
+        # The final RGB array :)
+        RGB = np.dstack([data, data, data])
+
+        ds["SplitWindowDifference"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["SplitWindowDifference"].attrs[
+            "Quick Guide"
+        ] = "http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_SplitWindowDifference.pdf"
+        ds["SplitWindowDifference"].attrs["long_name"] = "Split Window Difference"
+
+        return ds["SplitWindowDifference"]
+
+    def NightFogDifference(self):
+        """
+        Night Fog Difference RGB (greyscale):
+        (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_NightFogBTD.pdf>`__ for reference)
+
+        .. image:: /_static/NightFogDifference.png
+
+
+        """
+        ds = self._obj
+
+        # Load the three channels into appropriate R, G, and B variables
+        data = ds["CMI_C13"].data - ds["CMI_C07"].data
+
+        # _normalize values
+        data = _normalize(data, -90, 15)
+
+        # Invert data
+        data = 1 - data
+
+        # The final RGB array :)
+        RGB = np.dstack([data, data, data])
+
+        ds["NightFogDifference"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["NightFogDifference"].attrs[
+            "Quick Guide"
+        ] = "http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_NightFogBTD.pdf"
+        ds["NightFogDifference"].attrs["long_name"] = "NightFogDifference"
+
+        return ds["NightFogDifference"]
+
+    def RocketPlume(self, night=False):
+        """
+        Rocket Plume RGB
+
+        For identifying rocket launches.
+
+        See `this blog <https://cimss.ssec.wisc.edu/satellite-blog/archives/41335>`__ and
+        the `Quick Guide <https://cimss.ssec.wisc.edu/satellite-blog/images/2021/06/QuickGuide_Template_GOESRBanner_Rocket_Plume.pdf>`__
+        for reference
+
+        .. image:: /_static/RocketPlume.png
+
+        Parameters
+        ----------
+        night : bool
+            If the area is in night, turn this on to use a different channel
+            than the daytime application.
+
+
+        """
+        ds = self._obj
+
+        # Load the three channels into appropriate R, G, and B variables
+        R = ds["CMI_C07"].data
+        G = ds["CMI_C08"].data
+        if not night:
+            B = ds["CMI_C02"].data
+        else:
+            B = ds["CMI_C05"].data
+
+        # _normalize values
+        R = _normalize(R, 273, 338)
+        G = _normalize(G, 233, 253)
+        B = _normalize(B, 0, 0.80)
+
+        # The final RGB array :)
+        RGB = np.dstack([R, G, B])
+
+        ds["RocketPlume"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["RocketPlume"].attrs[
+            "Quick Guide"
+        ] = "https://cimss.ssec.wisc.edu/satellite-blog/images/2021/06/QuickGuide_Template_GOESRBanner_Rocket_Plume.pdf"
+        ds["RocketPlume"].attrs["long_name"] = "Rocket Plume"
+
+        return ds["RocketPlume"]
+
+    def NormalizedBurnRatio(self):
+        """
+        Normalized Burn Ratio
+
+        **THIS FUNCTION IS NOT FULLY DEVELOPED. Need more info.**
+
+        NBR= (0.86 µm – 2.2 µm)/(0.86 um + 2.2 um)
+
+
+        https://ntrs.nasa.gov/citations/20190030825
+
+        """
+        warnings.warn(
+            "THE `NormalizedBurnRatio` FUNCTION IS NOT FULLY DEVELOPED. NEED MORE INFO."
+        )
+        ds = self._obj
+
+        # Load the three channels into appropriate R, G, and B variables
+        C3 = ds["CMI_C03"].data
+        C6 = ds["CMI_C06"].data
+        data = (C3 - C6) / (C3 + C6)
+
+        # Invert data
+        # data = 1-data
+
+        # The final RGB array :)
+        RGB = np.dstack([data, data, data])
+
+        ds["NormalizedBurnRatio"] = (("y", "x", "rgb"), RGB)
+        ds["rgb"] = ["R", "G", "B"]
+        ds["NormalizedBurnRatio"].attrs[
+            "Quick Guide"
+        ] = "https://ntrs.nasa.gov/citations/20190030825"
+        ds["NormalizedBurnRatio"].attrs["long_name"] = "Normalized Burn Ratio"
+
+        return ds["NormalizedBurnRatio"]
```

### Comparing `goes2go-2022.8.26/goes2go/data.py` & `goes2go-2023.4.0/goes2go/data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,630 +1,631 @@
-## Brian Blaylock
-## September 16, 2020
-
-"""
-=============
-Retrieve Data
-=============
-Download and read data from the R-series Geostationary Operational
-Environmental Satellite data.
-
-Data is downloaded from Amazon Web Services and can be returned
-as a file list or read as an xarray.Dataset. If the data is not
-available in a local directory, it is loaded directly into memory.
-
-https://registry.opendata.aws/noaa-goes/
-"""
-
-import multiprocessing
-from concurrent.futures import ThreadPoolExecutor, as_completed, wait
-from datetime import datetime, timedelta
-from pathlib import Path
-
-import numpy as np
-import pandas as pd
-import s3fs
-import xarray as xr
-
-# NOTE: These config dict values are retrieved from __init__ and read
-# from the file ${HOME}/.config/goes2go/config.toml
-from . import config
-
-# Connect to AWS public buckets
-fs = s3fs.S3FileSystem(anon=True)
-
-# Define parameter options and aliases
-# ------------------------------------
-_satellite = {
-    "noaa-goes16": [16, "16", "G16", "EAST", "GOES16"],
-    "noaa-goes17": [17, "17", "G17", "WEST", "GOES17"],
-    "noaa-goes18": [18, "18", "G18", "WEST", "GOES18"],
-}
-
-_domain = {
-    "C": ["CONUS"],
-    "F": ["FULL", "FULLDISK", "FULL DISK"],
-    "M": ["MESOSCALE", "M1", "M2"],
-}
-
-_product = {
-    # Assume goes17 and goes18 have same products as goes16
-    i.split("/")[-1]: []
-    for i in fs.ls(f"noaa-goes16")
-}
-_product.pop("index.html", None)
-_product["GLM-L2-LCFA"] = ["GLM"]
-_product["ABI-L2-MCMIPC"] = ["ABIC"]
-_product["ABI-L2-MCMIPF"] = ["ABIF"]
-_product["ABI-L2-MCMIPM"] = ["ABIM"]
-
-
-def _check_param_inputs(**params):
-    """
-    Checks the input parameters for correct name or alias.
-
-    Specifically, check the input for product, domain, and satellite are
-    in the list of accepted values. If not, then look if it has an alias.
-    """
-    # Kinda messy, but gets the job done.
-    params.setdefault("verbose", True)
-    satellite = params["satellite"]
-    domain = params["domain"]
-    product = params["product"]
-    verbose = params["verbose"]
-
-    ## Determine the Satellite
-    if satellite not in _satellite:
-        satellite = str(satellite).upper()
-        for key, aliases in _satellite.items():
-            if satellite in aliases:
-                satellite = key
-    assert (
-        satellite in _satellite
-    ), f"satellite must be one of {list(_satellite.keys())} or an alias {list(_satellite.values())}"
-
-    ## Determine the Domain (only needed for ABI product)
-    if product.upper().startswith("ABI"):
-        if product[-1] in _domain:
-            # If the product has the domain, this takes priority
-            domain = product[-1]
-        elif isinstance(domain, str):
-            domain = domain.upper()
-            if domain in ["M1", "M2"]:
-                product = product + "M"
-            else:
-                for key, aliases in _domain.items():
-                    if domain in aliases:
-                        domain = key
-                product = product + domain
-        assert (domain in _domain) or (
-            domain in ["M1", "M2"]
-        ), f"domain must be one of {list(_domain.keys())} or an alias {list(_domain.values())}"
-    else:
-        domain = None
-
-    ## Determine the Product
-    if product not in _product:
-        for key, aliases in _product.items():
-            if product.upper() in aliases:
-                product = key
-    assert (
-        product in _product
-    ), f"product must be one of {list(_product .keys())} or an alias {list(_product .values())}"
-
-    return satellite, product, domain
-
-
-def _goes_file_df(satellite, product, start, end, bands=None, refresh=True):
-    """
-    Get list of requested GOES files as pandas.DataFrame.
-
-    Parameters
-    ----------
-    satellite : str
-    product : str
-    start : datetime
-    end : datetime
-    band : None, int, or list
-        Specify the ABI channels to retrieve.
-    refresh : bool
-        Refresh the s3fs.S3FileSystem object when files are listed.
-        Default True will refresh and not use a cached list.
-    """
-    params = locals()
-
-    start = pd.to_datetime(start)
-    end = pd.to_datetime(end)
-
-    DATES = pd.date_range(f"{start:%Y-%m-%d %H:00}", f"{end:%Y-%m-%d %H:00}", freq="1H")
-
-    # List all files for each date
-    # ----------------------------
-    files = []
-    for DATE in DATES:
-        files += fs.ls(f"{satellite}/{product}/{DATE:%Y/%j/%H/}", refresh=refresh)
-
-    # Build a table of the files
-    # --------------------------
-    df = pd.DataFrame(files, columns=["file"])
-    df[["product_mode", "satellite", "start", "end", "creation"]] = (
-        df["file"].str.rsplit("_", expand=True, n=5).loc[:, 1:]
-    )
-
-    # Todo: this could use some clean up !
-    if product.startswith("ABI"):
-        product_mode = df.product_mode.str.rsplit("-", 1, expand=True)
-        df["product"] = product_mode[0]
-        df["mode_bands"] = product_mode[1]
-
-        mode_bands = df.mode_bands.str.split("C", expand=True)
-        df["mode"] = mode_bands[0].str[1:].astype(int)
-        try:
-            df["band"] = mode_bands[1].astype(int)
-        except:
-            # No channel data
-            df["band"] = None
-
-        # Filter files by band number
-        if bands is not None:
-            if not hasattr(bands, "__len__"):
-                bands = [bands]
-            df = df.loc[df.band.isin(bands)]
-
-    # Filter files by requested time range
-    # ------------------------------------
-    # Convert filename datetime string to datetime object
-    df["start"] = pd.to_datetime(df.start, format="s%Y%j%H%M%S%f")
-    df["end"] = pd.to_datetime(df.end, format="e%Y%j%H%M%S%f")
-    df["creation"] = pd.to_datetime(df.creation, format="c%Y%j%H%M%S%f.nc")
-
-    # Filter by files within the requested time range
-    df = df.loc[df.start >= start].loc[df.end <= end].reset_index(drop=True)
-
-    for i in params:
-        df.attrs[i] = params[i]
-
-    return df
-
-
-def _download(df, save_dir, overwrite, max_threads=10, verbose=False):
-    """Download the files from a DataFrame listing with multithreading"""
-
-    def do_download(src):
-        dst = Path(save_dir) / src
-        if not dst.parent.is_dir():
-            dst.parent.mkdir(parents=True, exist_ok=True)
-        if dst.is_file() and not overwrite:
-            if verbose:
-                print(f" 👮🏻‍♂️ File already exists. Do not overwrite: {dst}")
-        else:
-            # Downloading file from AWS
-            fs.get(src, str(dst))
-
-    ################
-    # Multithreading
-    tasks = len(df)
-    threads = min(tasks, max_threads)
-
-    with ThreadPoolExecutor(threads) as exe:
-        futures = [exe.submit(do_download, src) for src in df.file]
-
-        # nothing is returned in the list
-        this_list = [future.result() for future in as_completed(futures)]
-
-    print(
-        f"📦 Finished downloading [{len(df)}] files to [{save_dir/Path(df.file[0]).parents[3]}]."
-    )
-
-
-def _as_xarray_MP(src, save_dir, i=None, n=None, verbose=True):
-    """Open a file as a xarray.Dataset -- a multiprocessing helper"""
-
-    # File destination
-    local_copy = Path(save_dir) / src
-
-    if local_copy.is_file():
-        if verbose:
-            print(
-                f"\r📖💽 Reading ({i:,}/{n:,}) file from LOCAL COPY [{local_copy}].",
-                end=" ",
-            )
-        ds = xr.open_dataset(local_copy)
-    else:
-        if verbose:
-            print(
-                f"\r📖☁ Reading ({i:,}/{n:,}) file from AWS to MEMORY [{src}].", end=" "
-            )
-        with fs.open(src, "rb") as f:
-            ds = xr.open_dataset(f).copy(deep=True)
-
-    # Turn some attributes to coordinates so they will be preserved
-    # when we concat multiple GOES DataSets together.
-    attr2coord = [
-        "dataset_name",
-        "date_created",
-        "time_coverage_start",
-        "time_coverage_end",
-    ]
-    for i in attr2coord:
-        if i in ds.attrs:
-            ds.coords[i] = ds.attrs.pop(i)
-
-    ds["filename"] = src
-
-    return ds
-
-
-def _as_xarray(df, **params):
-    """
-    Download files in the list to the desired path.
-
-    Use multiprocessing to speed up the download process.
-
-    Parameters
-    ----------
-    df : pandas.DataFrame
-        A list of files in the GOES s3 bucket.
-        This DataFrame must have a column of "files"
-    params : dict
-        Parameters from `goes_*` function.
-    """
-    params.setdefault("max_cpus", None)
-    params.setdefault("verbose", True)
-    save_dir = params["save_dir"]
-    max_cpus = params["max_cpus"]
-    verbose = params["verbose"]
-
-    n = len(df.file)
-    if n == 0:
-        print("🛸 No data....🌌")
-    elif n == 1:
-        # If we only have one file, we don't need multiprocessing
-        ds = _as_xarray_MP(df.iloc[0].file, save_dir, 1, 1, verbose)
-    else:
-        # Use Multiprocessing to read multiple files.
-        if max_cpus is None:
-            max_cpus = multiprocessing.cpu_count()
-        cpus = np.minimum(multiprocessing.cpu_count(), max_cpus)
-        cpus = np.minimum(cpus, n)
-
-        inputs = [(src, save_dir, i, n) for i, src in enumerate(df.file, start=1)]
-
-        with multiprocessing.Pool(cpus) as p:
-            results = p.starmap(_as_xarray_MP, inputs)
-            p.close()
-            p.join()
-
-        # Need some work to concat the datasets
-        if df.attrs["product"].startswith("ABI"):
-            print("concatenate Datasets", end="")
-            ds = xr.concat(results, dim="t")
-        else:
-            ds = results
-
-    if verbose:
-        print(f"\r{'':1000}\r📚 Finished reading [{n}] files into xarray.Dataset.")
-    ds.attrs["path"] = df.file.to_list()
-    return ds
-
-
-###############################################################################
-###############################################################################
-
-
-def goes_timerange(
-    start=None,
-    end=None,
-    recent=None,
-    *,
-    satellite=config["timerange"].get("satellite"),
-    product=config["timerange"].get("product"),
-    domain=config["timerange"].get("domain"),
-    return_as=config["timerange"].get("return_as"),
-    download=config["timerange"].get("download"),
-    overwrite=config["timerange"].get("overwrite"),
-    save_dir=config["timerange"].get("save_dir"),
-    max_cpus=config["timerange"].get("max_cpus"),
-    bands=None,
-    s3_refresh=config["timerange"].get("s3_refresh"),
-    verbose=config["timerange"].get("verbose", True),
-):
-    """
-    Get GOES data for a time range.
-
-    Parameters
-    ----------
-    start, end : datetime
-        Required if recent is None.
-    recent : timedelta or pandas-parsable timedelta str
-        Required if start and end are None. If timedelta(hours=1), will
-        get the most recent files for the past hour.
-    satellite : {'goes16', 'goes17', 'goes18'}
-        Specify which GOES satellite.
-        The following alias may also be used:
-
-        - ``'goes16'``: 16, 'G16', or 'EAST'
-        - ``'goes17'``: 17, 'G17', or 'WEST'
-        - ``'goes18'``: 18, 'G18', or 'WEST'
-
-    product : {'ABI', 'GLM', other GOES product}
-        Specify the product name.
-
-        - 'ABI' is an alias for ABI-L2-MCMIP Multichannel Cloud and Moisture Imagery
-        - 'GLM' is an alias for GLM-L2-LCFA Geostationary Lightning Mapper
-
-        Others may include ``'ABI-L1b-Rad'``, ``'ABI-L2-DMW'``, etc.
-        For more available products, look at this `README
-        <https://docs.opendata.aws/noaa-goes16/cics-readme.html>`_
-    domain : {'C', 'F', 'M'}
-        ABI scan region indicator. Only required for ABI products if the
-        given product does not end with C, F, or M.
-
-        - C: Contiguous United States (alias 'CONUS')
-        - F: Full Disk (alias 'FULL')
-        - M: Mesoscale (alias 'MESOSCALE')
-
-    return_as : {'xarray', 'filelist'}
-        Return the data as an xarray.Dataset or as a list of files
-    download : bool
-        - True: Download the data to disk to the location set by :guilabel:`save_dir`
-        - False: Just load the data into memory.
-    save_dir : pathlib.Path or str
-        Path to save the data.
-    overwrite : bool
-        - True: Download the file even if it exists.
-        - False Do not download the file if it already exists
-    max_cpus : int
-    bands : None, int, or list
-        ONLY FOR L1b-Rad products; specify the bands you want
-    s3_refresh : bool
-        Refresh the s3fs.S3FileSystem object when files are listed.
-
-    """
-    # If `start`, or `end` is a string, parse with Pandas
-    if isinstance(start, str):
-        start = pd.to_datetime(start)
-    if isinstance(end, str):
-        end = pd.to_datetime(end)
-    # If `recent` is a string (like recent='1H'), parse with Pandas
-    if isinstance(recent, str):
-        recent = pd.to_timedelta(recent)
-
-    params = locals()
-    satellite, product, domain = _check_param_inputs(**params)
-    params["satellite"] = satellite
-    params["product"] = product
-    params["domain"] = domain
-
-    check1 = start is not None and end is not None
-    check2 = recent is not None
-    assert check1 or check2, "🤔 `start` and `end` *or* `recent` is required"
-
-    if check1:
-        assert hasattr(start, "second") and hasattr(
-            end, "second"
-        ), "`start` and `end` must be a datetime object"
-    elif check2:
-        assert hasattr(recent, "seconds"), "`recent` must be a timedelta object"
-
-    # Parameter Setup
-    # ---------------
-    # Create a range of directories to check. The GOES S3 bucket is
-    # organized by hour of day.
-    if recent is not None:
-        start = datetime.utcnow() - recent
-        end = datetime.utcnow()
-
-    df = _goes_file_df(satellite, product, start, end, bands=bands, refresh=s3_refresh)
-
-    if download:
-        _download(df, save_dir=save_dir, overwrite=overwrite, verbose=verbose)
-
-    if return_as == "filelist":
-        df.attrs["filePath"] = save_dir
-        return df
-    elif return_as == "xarray":
-        return _as_xarray(df, **params)
-
-
-def goes_latest(
-    *,
-    satellite=config["latest"].get("satellite"),
-    product=config["latest"].get("product"),
-    domain=config["latest"].get("domain"),
-    return_as=config["latest"].get("return_as"),
-    download=config["latest"].get("download"),
-    overwrite=config["latest"].get("overwrite"),
-    save_dir=config["latest"].get("save_dir"),
-    bands=None,
-    s3_refresh=config["latest"].get("s3_refresh"),
-    verbose=config["latest"].get("verbose", True),
-):
-    """
-    Get the latest available GOES data.
-
-    Parameters
-    ----------
-    satellite : {'goes16', 'goes17', 'goes18'}
-        Specify which GOES satellite.
-        The following alias may also be used:
-
-        - ``'goes16'``: 16, 'G16', or 'EAST'
-        - ``'goes17'``: 17, 'G17', or 'WEST'
-        - ``'goes18'``: 18, 'G18', or 'WEST'
-
-    product : {'ABI', 'GLM', other GOES product}
-        Specify the product name.
-
-        - 'ABI' is an alias for ABI-L2-MCMIP Multichannel Cloud and Moisture Imagery
-        - 'GLM' is an alias for GLM-L2-LCFA Geostationary Lightning Mapper
-
-        Others may include ``'ABI-L1b-Rad'``, ``'ABI-L2-DMW'``, etc.
-        For more available products, look at this `README
-        <https://docs.opendata.aws/noaa-goes16/cics-readme.html>`_
-    domain : {'C', 'F', 'M'}
-        ABI scan region indicator. Only required for ABI products if the
-        given product does not end with C, F, or M.
-
-        - C: Contiguous United States (alias 'CONUS')
-        - F: Full Disk (alias 'FULL')
-        - M: Mesoscale (alias 'MESOSCALE')
-
-    return_as : {'xarray', 'filelist'}
-        Return the data as an xarray.Dataset or as a list of files
-    download : bool
-        - True: Download the data to disk to the location set by :guilabel:`save_dir`
-        - False: Just load the data into memory.
-    save_dir : pathlib.Path or str
-        Path to save the data.
-    overwrite : bool
-        - True: Download the file even if it exists.
-        - False Do not download the file if it already exists
-    bands : None, int, or list
-        ONLY FOR L1b-Rad products; specify the bands you want
-    s3_refresh : bool
-        Refresh the s3fs.S3FileSystem object when files are listed.
-    """
-    params = locals()
-    satellite, product, domain = _check_param_inputs(**params)
-    params["satellite"] = satellite
-    params["product"] = product
-    params["domain"] = domain
-
-    # Parameter Setup
-    # ---------------
-    # Create a range of directories to check. The GOES S3 bucket is
-    # organized by hour of day. Look in the current hour and last hour.
-    start = datetime.utcnow() - timedelta(hours=1)
-    end = datetime.utcnow()
-
-    df = _goes_file_df(satellite, product, start, end, bands=bands, refresh=s3_refresh)
-
-    # Filter for specific mesoscale domain
-    if domain is not None and domain.upper() in ["M1", "M2"]:
-        df = df[df["file"].str.contains(f"{domain.upper()}-M")]
-
-    # Get the most recent file (latest start date)
-    df = df.loc[df.start == df.start.max()].reset_index(drop=True)
-
-    if download:
-        _download(df, save_dir=save_dir, overwrite=overwrite, verbose=verbose)
-
-    if return_as == "filelist":
-        df.attrs["filePath"] = save_dir
-        return df
-    elif return_as == "xarray":
-        return _as_xarray(df, **params)
-
-
-def goes_nearesttime(
-    attime,
-    within=pd.to_timedelta(config["nearesttime"].get("within", "1H")),
-    *,
-    satellite=config["nearesttime"].get("satellite"),
-    product=config["nearesttime"].get("product"),
-    domain=config["nearesttime"].get("domain"),
-    return_as=config["nearesttime"].get("return_as"),
-    download=config["nearesttime"].get("download"),
-    overwrite=config["nearesttime"].get("overwrite"),
-    save_dir=config["nearesttime"].get("save_dir"),
-    bands=None,
-    s3_refresh=config["nearesttime"].get("s3_refresh"),
-    verbose=config["nearesttime"].get("verbose", True),
-):
-    """
-    Get the GOES data nearest a specified time.
-
-    Parameters
-    ----------
-    attime : datetime
-        Time to find the nearest observation for.
-        May also use a pandas-interpretable datetime string.
-    within : timedelta or pandas-parsable timedelta str
-        Timerange tht the nearest observation must be.
-    satellite : {'goes16', 'goes17', 'goes18'}
-        Specify which GOES satellite.
-        The following alias may also be used:
-
-        - ``'goes16'``: 16, 'G16', or 'EAST'
-        - ``'goes17'``: 17, 'G17', or 'WEST'
-        - ``'goes18'``: 18, 'G18', or 'WEST'
-
-    product : {'ABI', 'GLM', other GOES product}
-        Specify the product name.
-
-        - 'ABI' is an alias for ABI-L2-MCMIP Multichannel Cloud and Moisture Imagery
-        - 'GLM' is an alias for GLM-L2-LCFA Geostationary Lightning Mapper
-
-        Others may include ``'ABI-L1b-Rad'``, ``'ABI-L2-DMW'``, etc.
-        For more available products, look at this `README
-        <https://docs.opendata.aws/noaa-goes16/cics-readme.html>`_
-    domain : {'C', 'F', 'M'}
-        ABI scan region indicator. Only required for ABI products if the
-        given product does not end with C, F, or M.
-
-        - C: Contiguous United States (alias 'CONUS')
-        - F: Full Disk (alias 'FULL')
-        - M: Mesoscale (alias 'MESOSCALE')
-
-    return_as : {'xarray', 'filelist'}
-        Return the data as an xarray.Dataset or as a list of files
-    download : bool
-        - True: Download the data to disk to the location set by :guilabel:`save_dir`
-        - False: Just load the data into memory.
-    save_dir : pathlib.Path or str
-        Path to save the data.
-    overwrite : bool
-        - True: Download the file even if it exists.
-        - False: Do not download the file if it already exists
-    bands : None, int, or list
-        ONLY FOR L1b-Rad products; specify the bands you want
-    s3_refresh : bool
-        Refresh the s3fs.S3FileSystem object when files are listed.
-    """
-    if isinstance(attime, str):
-        attime = pd.to_datetime(attime)
-    if isinstance(within, str):
-        within = pd.to_timedelta(within)
-
-    params = locals()
-    satellite, product, _ = _check_param_inputs(**params)
-    params["satellite"] = satellite
-    params["product"] = product
-
-    # Parameter Setup
-    # ---------------
-    # Create a range of directories to check. The GOES S3 bucket is
-    # organized by hour of day.
-    start = attime - within
-    end = attime + within
-
-    df = _goes_file_df(satellite, product, start, end, bands=bands, refresh=s3_refresh)
-
-    # return df, start, end, attime
-
-    # Filter for specific mesoscale domain
-    if domain.upper() in ["M1", "M2"]:
-        df = df[df["file"].str.contains(f"{domain.upper()}-M")]
-
-    # Get row that matches the nearest time
-    df = df.sort_values("start")
-    df = df.set_index(df.start)
-    unique_times_index = df.index.unique()
-    nearest_time_index = unique_times_index.get_indexer([attime], method='nearest')
-    nearest_time = unique_times_index[nearest_time_index]
-    df = df.loc[nearest_time]
-    df = df.reset_index(drop=True)
-
-    n = len(df.file)
-    if n == 0:
-        print("🛸 No data....🌌")
-        return None
-
-    if download:
-        _download(df, save_dir=save_dir, overwrite=overwrite, verbose=verbose)
-
-    if return_as == "filelist":
-        df.attrs["filePath"] = save_dir
-        return df
-    elif return_as == "xarray":
-        return _as_xarray(df, **params)
+## Brian Blaylock
+## September 16, 2020
+
+"""
+=============
+Retrieve Data
+=============
+Download and read data from the R-series Geostationary Operational
+Environmental Satellite data.
+
+Data is downloaded from Amazon Web Services and can be returned
+as a file list or read as an xarray.Dataset. If the data is not
+available in a local directory, it is loaded directly into memory.
+
+https://registry.opendata.aws/noaa-goes/
+"""
+
+import multiprocessing
+from concurrent.futures import ThreadPoolExecutor, as_completed, wait
+from datetime import datetime, timedelta
+from pathlib import Path
+
+import numpy as np
+import pandas as pd
+import s3fs
+import xarray as xr
+
+# NOTE: These config dict values are retrieved from __init__ and read
+# from the file ${HOME}/.config/goes2go/config.toml
+from . import config
+
+# Connect to AWS public buckets
+fs = s3fs.S3FileSystem(anon=True)
+
+# Define parameter options and aliases
+# ------------------------------------
+_satellite = {
+    "noaa-goes16": [16, "16", "G16", "EAST", "GOES16"],
+    "noaa-goes17": [17, "17", "G17", "WEST", "GOES17"],
+    "noaa-goes18": [18, "18", "G18", "WEST", "GOES18"],
+}
+
+_domain = {
+    "C": ["CONUS"],
+    "F": ["FULL", "FULLDISK", "FULL DISK"],
+    "M": ["MESOSCALE", "M1", "M2"],
+}
+
+_product = {
+    # Assume goes17 and goes18 have same products as goes16
+    i.split("/")[-1]: []
+    for i in fs.ls(f"noaa-goes16")
+}
+_product.pop("index.html", None)
+_product["GLM-L2-LCFA"] = ["GLM"]
+_product["ABI-L2-MCMIPC"] = ["ABIC"]
+_product["ABI-L2-MCMIPF"] = ["ABIF"]
+_product["ABI-L2-MCMIPM"] = ["ABIM"]
+
+
+def _check_param_inputs(**params):
+    """
+    Checks the input parameters for correct name or alias.
+
+    Specifically, check the input for product, domain, and satellite are
+    in the list of accepted values. If not, then look if it has an alias.
+    """
+    # Kinda messy, but gets the job done.
+    params.setdefault("verbose", True)
+    satellite = params["satellite"]
+    domain = params["domain"]
+    product = params["product"]
+    verbose = params["verbose"]
+
+    ## Determine the Satellite
+    if satellite not in _satellite:
+        satellite = str(satellite).upper()
+        for key, aliases in _satellite.items():
+            if satellite in aliases:
+                satellite = key
+    assert (
+        satellite in _satellite
+    ), f"satellite must be one of {list(_satellite.keys())} or an alias {list(_satellite.values())}"
+
+    ## Determine the Domain (only needed for ABI product)
+    if product.upper().startswith("ABI"):
+        if product[-1] in _domain:
+            # If the product has the domain, this takes priority
+            domain = product[-1]
+        elif isinstance(domain, str):
+            domain = domain.upper()
+            if domain in ["M1", "M2"]:
+                product = product + "M"
+            else:
+                for key, aliases in _domain.items():
+                    if domain in aliases:
+                        domain = key
+                product = product + domain
+        assert (domain in _domain) or (
+            domain in ["M1", "M2"]
+        ), f"domain must be one of {list(_domain.keys())} or an alias {list(_domain.values())}"
+    else:
+        domain = None
+
+    ## Determine the Product
+    if product not in _product:
+        for key, aliases in _product.items():
+            if product.upper() in aliases:
+                product = key
+    assert (
+        product in _product
+    ), f"product must be one of {list(_product .keys())} or an alias {list(_product .values())}"
+
+    return satellite, product, domain
+
+
+def _goes_file_df(satellite, product, start, end, bands=None, refresh=True):
+    """
+    Get list of requested GOES files as pandas.DataFrame.
+
+    Parameters
+    ----------
+    satellite : str
+    product : str
+    start : datetime
+    end : datetime
+    band : None, int, or list
+        Specify the ABI channels to retrieve.
+    refresh : bool
+        Refresh the s3fs.S3FileSystem object when files are listed.
+        Default True will refresh and not use a cached list.
+    """
+    params = locals()
+
+    start = pd.to_datetime(start)
+    end = pd.to_datetime(end)
+
+    DATES = pd.date_range(f"{start:%Y-%m-%d %H:00}", f"{end:%Y-%m-%d %H:00}", freq="1H")
+
+    # List all files for each date
+    # ----------------------------
+    files = []
+    for DATE in DATES:
+        files += fs.ls(f"{satellite}/{product}/{DATE:%Y/%j/%H/}", refresh=refresh)
+
+    # Build a table of the files
+    # --------------------------
+    df = pd.DataFrame(files, columns=["file"])
+    df[["product_mode", "satellite", "start", "end", "creation"]] = (
+        df["file"].str.rsplit("_", expand=True, n=5).loc[:, 1:]
+    )
+
+    # Todo: this could use some clean up !
+    if product.startswith("ABI"):
+        product_mode = df.product_mode.str.rsplit("-", n=1, expand=True)
+        df["product"] = product_mode[0]
+        df["mode_bands"] = product_mode[1]
+
+        mode_bands = df.mode_bands.str.split("C", expand=True)
+        df["mode"] = mode_bands[0].str[1:].astype(int)
+        try:
+            df["band"] = mode_bands[1].astype(int)
+        except:
+            # No channel data
+            df["band"] = None
+
+        # Filter files by band number
+        if bands is not None:
+            if not hasattr(bands, "__len__"):
+                bands = [bands]
+            df = df.loc[df.band.isin(bands)]
+
+    # Filter files by requested time range
+    # ------------------------------------
+    # Convert filename datetime string to datetime object
+    df["start"] = pd.to_datetime(df.start, format="s%Y%j%H%M%S%f")
+    df["end"] = pd.to_datetime(df.end, format="e%Y%j%H%M%S%f")
+    df["creation"] = pd.to_datetime(df.creation, format="c%Y%j%H%M%S%f.nc")
+
+    # Filter by files within the requested time range
+    df = df.loc[df.start >= start].loc[df.end <= end].reset_index(drop=True)
+
+    for i in params:
+        df.attrs[i] = params[i]
+
+    return df
+
+
+def _download(df, save_dir, overwrite, max_threads=10, verbose=False):
+    """Download the files from a DataFrame listing with multithreading"""
+
+    def do_download(src):
+        dst = Path(save_dir) / src
+        if not dst.parent.is_dir():
+            dst.parent.mkdir(parents=True, exist_ok=True)
+        if dst.is_file() and not overwrite:
+            if verbose:
+                print(f" 👮🏻‍♂️ File already exists. Do not overwrite: {dst}")
+        else:
+            # Downloading file from AWS
+            fs.get(src, str(dst))
+
+    ################
+    # Multithreading
+    tasks = len(df)
+    threads = min(tasks, max_threads)
+
+    with ThreadPoolExecutor(threads) as exe:
+        futures = [exe.submit(do_download, src) for src in df.file]
+
+        # nothing is returned in the list
+        this_list = [future.result() for future in as_completed(futures)]
+
+    print(
+        f"📦 Finished downloading [{len(df)}] files to [{save_dir/Path(df.file[0]).parents[3]}]."
+    )
+
+
+def _as_xarray_MP(src, save_dir, i=None, n=None, verbose=True):
+    """Open a file as a xarray.Dataset -- a multiprocessing helper"""
+
+    # File destination
+    local_copy = Path(save_dir) / src
+
+    if local_copy.is_file():
+        if verbose:
+            print(
+                f"\r📖💽 Reading ({i:,}/{n:,}) file from LOCAL COPY [{local_copy}].",
+                end=" ",
+            )
+        with open(local_copy, "rb") as f:
+            ds = xr.load_dataset(f)
+    else:
+        if verbose:
+            print(
+                f"\r📖☁ Reading ({i:,}/{n:,}) file from AWS to MEMORY [{src}].", end=" "
+            )
+        with fs.open(src, "rb") as f:
+            ds = xr.load_dataset(f)
+
+    # Turn some attributes to coordinates so they will be preserved
+    # when we concat multiple GOES DataSets together.
+    attr2coord = [
+        "dataset_name",
+        "date_created",
+        "time_coverage_start",
+        "time_coverage_end",
+    ]
+    for i in attr2coord:
+        if i in ds.attrs:
+            ds.coords[i] = ds.attrs.pop(i)
+
+    ds["filename"] = src
+
+    return ds
+
+
+def _as_xarray(df, **params):
+    """
+    Download files in the list to the desired path.
+
+    Use multiprocessing to speed up the download process.
+
+    Parameters
+    ----------
+    df : pandas.DataFrame
+        A list of files in the GOES s3 bucket.
+        This DataFrame must have a column of "files"
+    params : dict
+        Parameters from `goes_*` function.
+    """
+    params.setdefault("max_cpus", None)
+    params.setdefault("verbose", True)
+    save_dir = params["save_dir"]
+    max_cpus = params["max_cpus"]
+    verbose = params["verbose"]
+
+    n = len(df.file)
+    if n == 0:
+        print("🛸 No data....🌌")
+    elif n == 1:
+        # If we only have one file, we don't need multiprocessing
+        ds = _as_xarray_MP(df.iloc[0].file, save_dir, 1, 1, verbose)
+    else:
+        # Use Multiprocessing to read multiple files.
+        if max_cpus is None:
+            max_cpus = multiprocessing.cpu_count()
+        cpus = np.minimum(multiprocessing.cpu_count(), max_cpus)
+        cpus = np.minimum(cpus, n)
+
+        inputs = [(src, save_dir, i, n) for i, src in enumerate(df.file, start=1)]
+
+        with multiprocessing.Pool(cpus) as p:
+            results = p.starmap(_as_xarray_MP, inputs)
+            p.close()
+            p.join()
+
+        # Need some work to concat the datasets
+        if df.attrs["product"].startswith("ABI"):
+            print("concatenate Datasets", end="")
+            ds = xr.concat(results, dim="t")
+        else:
+            ds = results
+
+    if verbose:
+        print(f"\r{'':1000}\r📚 Finished reading [{n}] files into xarray.Dataset.")
+    ds.attrs["path"] = df.file.to_list()
+    return ds
+
+
+###############################################################################
+###############################################################################
+
+
+def goes_timerange(
+    start=None,
+    end=None,
+    recent=None,
+    *,
+    satellite=config["timerange"].get("satellite"),
+    product=config["timerange"].get("product"),
+    domain=config["timerange"].get("domain"),
+    return_as=config["timerange"].get("return_as"),
+    download=config["timerange"].get("download"),
+    overwrite=config["timerange"].get("overwrite"),
+    save_dir=config["timerange"].get("save_dir"),
+    max_cpus=config["timerange"].get("max_cpus"),
+    bands=None,
+    s3_refresh=config["timerange"].get("s3_refresh"),
+    verbose=config["timerange"].get("verbose", True),
+):
+    """
+    Get GOES data for a time range.
+
+    Parameters
+    ----------
+    start, end : datetime
+        Required if recent is None.
+    recent : timedelta or pandas-parsable timedelta str
+        Required if start and end are None. If timedelta(hours=1), will
+        get the most recent files for the past hour.
+    satellite : {'goes16', 'goes17', 'goes18'}
+        Specify which GOES satellite.
+        The following alias may also be used:
+
+        - ``'goes16'``: 16, 'G16', or 'EAST'
+        - ``'goes17'``: 17, 'G17', or 'WEST'
+        - ``'goes18'``: 18, 'G18', or 'WEST'
+
+    product : {'ABI', 'GLM', other GOES product}
+        Specify the product name.
+
+        - 'ABI' is an alias for ABI-L2-MCMIP Multichannel Cloud and Moisture Imagery
+        - 'GLM' is an alias for GLM-L2-LCFA Geostationary Lightning Mapper
+
+        Others may include ``'ABI-L1b-Rad'``, ``'ABI-L2-DMW'``, etc.
+        For more available products, look at this `README
+        <https://docs.opendata.aws/noaa-goes16/cics-readme.html>`_
+    domain : {'C', 'F', 'M'}
+        ABI scan region indicator. Only required for ABI products if the
+        given product does not end with C, F, or M.
+
+        - C: Contiguous United States (alias 'CONUS')
+        - F: Full Disk (alias 'FULL')
+        - M: Mesoscale (alias 'MESOSCALE')
+
+    return_as : {'xarray', 'filelist'}
+        Return the data as an xarray.Dataset or as a list of files
+    download : bool
+        - True: Download the data to disk to the location set by :guilabel:`save_dir`
+        - False: Just load the data into memory.
+    save_dir : pathlib.Path or str
+        Path to save the data.
+    overwrite : bool
+        - True: Download the file even if it exists.
+        - False Do not download the file if it already exists
+    max_cpus : int
+    bands : None, int, or list
+        ONLY FOR L1b-Rad products; specify the bands you want
+    s3_refresh : bool
+        Refresh the s3fs.S3FileSystem object when files are listed.
+
+    """
+    # If `start`, or `end` is a string, parse with Pandas
+    if isinstance(start, str):
+        start = pd.to_datetime(start)
+    if isinstance(end, str):
+        end = pd.to_datetime(end)
+    # If `recent` is a string (like recent='1H'), parse with Pandas
+    if isinstance(recent, str):
+        recent = pd.to_timedelta(recent)
+
+    params = locals()
+    satellite, product, domain = _check_param_inputs(**params)
+    params["satellite"] = satellite
+    params["product"] = product
+    params["domain"] = domain
+
+    check1 = start is not None and end is not None
+    check2 = recent is not None
+    assert check1 or check2, "🤔 `start` and `end` *or* `recent` is required"
+
+    if check1:
+        assert hasattr(start, "second") and hasattr(
+            end, "second"
+        ), "`start` and `end` must be a datetime object"
+    elif check2:
+        assert hasattr(recent, "seconds"), "`recent` must be a timedelta object"
+
+    # Parameter Setup
+    # ---------------
+    # Create a range of directories to check. The GOES S3 bucket is
+    # organized by hour of day.
+    if recent is not None:
+        start = datetime.utcnow() - recent
+        end = datetime.utcnow()
+
+    df = _goes_file_df(satellite, product, start, end, bands=bands, refresh=s3_refresh)
+
+    if download:
+        _download(df, save_dir=save_dir, overwrite=overwrite, verbose=verbose)
+
+    if return_as == "filelist":
+        df.attrs["filePath"] = save_dir
+        return df
+    elif return_as == "xarray":
+        return _as_xarray(df, **params)
+
+
+def goes_latest(
+    *,
+    satellite=config["latest"].get("satellite"),
+    product=config["latest"].get("product"),
+    domain=config["latest"].get("domain"),
+    return_as=config["latest"].get("return_as"),
+    download=config["latest"].get("download"),
+    overwrite=config["latest"].get("overwrite"),
+    save_dir=config["latest"].get("save_dir"),
+    bands=None,
+    s3_refresh=config["latest"].get("s3_refresh"),
+    verbose=config["latest"].get("verbose", True),
+):
+    """
+    Get the latest available GOES data.
+
+    Parameters
+    ----------
+    satellite : {'goes16', 'goes17', 'goes18'}
+        Specify which GOES satellite.
+        The following alias may also be used:
+
+        - ``'goes16'``: 16, 'G16', or 'EAST'
+        - ``'goes17'``: 17, 'G17', or 'WEST'
+        - ``'goes18'``: 18, 'G18', or 'WEST'
+
+    product : {'ABI', 'GLM', other GOES product}
+        Specify the product name.
+
+        - 'ABI' is an alias for ABI-L2-MCMIP Multichannel Cloud and Moisture Imagery
+        - 'GLM' is an alias for GLM-L2-LCFA Geostationary Lightning Mapper
+
+        Others may include ``'ABI-L1b-Rad'``, ``'ABI-L2-DMW'``, etc.
+        For more available products, look at this `README
+        <https://docs.opendata.aws/noaa-goes16/cics-readme.html>`_
+    domain : {'C', 'F', 'M'}
+        ABI scan region indicator. Only required for ABI products if the
+        given product does not end with C, F, or M.
+
+        - C: Contiguous United States (alias 'CONUS')
+        - F: Full Disk (alias 'FULL')
+        - M: Mesoscale (alias 'MESOSCALE')
+
+    return_as : {'xarray', 'filelist'}
+        Return the data as an xarray.Dataset or as a list of files
+    download : bool
+        - True: Download the data to disk to the location set by :guilabel:`save_dir`
+        - False: Just load the data into memory.
+    save_dir : pathlib.Path or str
+        Path to save the data.
+    overwrite : bool
+        - True: Download the file even if it exists.
+        - False Do not download the file if it already exists
+    bands : None, int, or list
+        ONLY FOR L1b-Rad products; specify the bands you want
+    s3_refresh : bool
+        Refresh the s3fs.S3FileSystem object when files are listed.
+    """
+    params = locals()
+    satellite, product, domain = _check_param_inputs(**params)
+    params["satellite"] = satellite
+    params["product"] = product
+    params["domain"] = domain
+
+    # Parameter Setup
+    # ---------------
+    # Create a range of directories to check. The GOES S3 bucket is
+    # organized by hour of day. Look in the current hour and last hour.
+    start = datetime.utcnow() - timedelta(hours=1)
+    end = datetime.utcnow()
+
+    df = _goes_file_df(satellite, product, start, end, bands=bands, refresh=s3_refresh)
+
+    # Filter for specific mesoscale domain
+    if domain is not None and domain.upper() in ["M1", "M2"]:
+        df = df[df["file"].str.contains(f"{domain.upper()}-M")]
+
+    # Get the most recent file (latest start date)
+    df = df.loc[df.start == df.start.max()].reset_index(drop=True)
+
+    if download:
+        _download(df, save_dir=save_dir, overwrite=overwrite, verbose=verbose)
+
+    if return_as == "filelist":
+        df.attrs["filePath"] = save_dir
+        return df
+    elif return_as == "xarray":
+        return _as_xarray(df, **params)
+
+
+def goes_nearesttime(
+    attime,
+    within=pd.to_timedelta(config["nearesttime"].get("within", "1H")),
+    *,
+    satellite=config["nearesttime"].get("satellite"),
+    product=config["nearesttime"].get("product"),
+    domain=config["nearesttime"].get("domain"),
+    return_as=config["nearesttime"].get("return_as"),
+    download=config["nearesttime"].get("download"),
+    overwrite=config["nearesttime"].get("overwrite"),
+    save_dir=config["nearesttime"].get("save_dir"),
+    bands=None,
+    s3_refresh=config["nearesttime"].get("s3_refresh"),
+    verbose=config["nearesttime"].get("verbose", True),
+):
+    """
+    Get the GOES data nearest a specified time.
+
+    Parameters
+    ----------
+    attime : datetime
+        Time to find the nearest observation for.
+        May also use a pandas-interpretable datetime string.
+    within : timedelta or pandas-parsable timedelta str
+        Timerange tht the nearest observation must be.
+    satellite : {'goes16', 'goes17', 'goes18'}
+        Specify which GOES satellite.
+        The following alias may also be used:
+
+        - ``'goes16'``: 16, 'G16', or 'EAST'
+        - ``'goes17'``: 17, 'G17', or 'WEST'
+        - ``'goes18'``: 18, 'G18', or 'WEST'
+
+    product : {'ABI', 'GLM', other GOES product}
+        Specify the product name.
+
+        - 'ABI' is an alias for ABI-L2-MCMIP Multichannel Cloud and Moisture Imagery
+        - 'GLM' is an alias for GLM-L2-LCFA Geostationary Lightning Mapper
+
+        Others may include ``'ABI-L1b-Rad'``, ``'ABI-L2-DMW'``, etc.
+        For more available products, look at this `README
+        <https://docs.opendata.aws/noaa-goes16/cics-readme.html>`_
+    domain : {'C', 'F', 'M'}
+        ABI scan region indicator. Only required for ABI products if the
+        given product does not end with C, F, or M.
+
+        - C: Contiguous United States (alias 'CONUS')
+        - F: Full Disk (alias 'FULL')
+        - M: Mesoscale (alias 'MESOSCALE')
+
+    return_as : {'xarray', 'filelist'}
+        Return the data as an xarray.Dataset or as a list of files
+    download : bool
+        - True: Download the data to disk to the location set by :guilabel:`save_dir`
+        - False: Just load the data into memory.
+    save_dir : pathlib.Path or str
+        Path to save the data.
+    overwrite : bool
+        - True: Download the file even if it exists.
+        - False: Do not download the file if it already exists
+    bands : None, int, or list
+        ONLY FOR L1b-Rad products; specify the bands you want
+    s3_refresh : bool
+        Refresh the s3fs.S3FileSystem object when files are listed.
+    """
+    if isinstance(attime, str):
+        attime = pd.to_datetime(attime)
+    if isinstance(within, str):
+        within = pd.to_timedelta(within)
+
+    params = locals()
+    satellite, product, _ = _check_param_inputs(**params)
+    params["satellite"] = satellite
+    params["product"] = product
+
+    # Parameter Setup
+    # ---------------
+    # Create a range of directories to check. The GOES S3 bucket is
+    # organized by hour of day.
+    start = attime - within
+    end = attime + within
+
+    df = _goes_file_df(satellite, product, start, end, bands=bands, refresh=s3_refresh)
+
+    # return df, start, end, attime
+
+    # Filter for specific mesoscale domain
+    if domain.upper() in ["M1", "M2"]:
+        df = df[df["file"].str.contains(f"{domain.upper()}-M")]
+
+    # Get row that matches the nearest time
+    df = df.sort_values("start")
+    df = df.set_index(df.start)
+    unique_times_index = df.index.unique()
+    nearest_time_index = unique_times_index.get_indexer([attime], method="nearest")
+    nearest_time = unique_times_index[nearest_time_index]
+    df = df.loc[nearest_time]
+    df = df.reset_index(drop=True)
+
+    n = len(df.file)
+    if n == 0:
+        print("🛸 No data....🌌")
+        return None
+
+    if download:
+        _download(df, save_dir=save_dir, overwrite=overwrite, verbose=verbose)
+
+    if return_as == "filelist":
+        df.attrs["filePath"] = save_dir
+        return df
+    elif return_as == "xarray":
+        return _as_xarray(df, **params)
```

### Comparing `goes2go-2022.8.26/goes2go/product_table.txt` & `goes2go-2023.4.0/goes2go/product_table.txt`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-# List of ABI products and their full description
-# From https://github.com/awslabs/open-data-docs/tree/main/docs/noaa/noaa-goes16
-ABI-L1b-RadF,   Advanced Baseline Imager Level 1b Full Disk
-ABI-L1b-RadC,   Advanced Baseline Imager Level 1b CONUS
-ABI-L1b-RadM,   Advanced Baseline Imager Level 1b Mesoscale
-ABI-L2-ACHAC,   Advanced Baseline Imager Level 2 Cloud Top Height CONUS
-ABI-L2-ACHAF,   Advanced Baseline Imager Level 2 Cloud Top Height Full Disk
-ABI-L2-ACHAM,   Advanced Baseline Imager Level 2 Cloud Top Height Mesoscale
-ABI-L2-ACHTF,   Advanced Baseline Imager Level 2 Cloud Top Temperature Full Disk
-ABI-L2-ACHTM,   Advanced Baseline Imager Level 2 Cloud Top Temperature Mesoscale
-ABI-L2-ACMC,    Advanced Baseline Imager Level 2 Clear Sky Mask CONUS
-ABI-L2-ACMF,    Advanced Baseline Imager Level 2 Clear Sky Mask Full Disk
-ABI-L2-ACMM,    Advanced Baseline Imager Level 2 Clear Sky Mask Mesoscale
-ABI-L2-ACTPC,   Advanced Baseline Imager Level 2 Cloud Top Phase CONUS
-ABI-L2-ACTPF,   Advanced Baseline Imager Level 2 Cloud Top Phase Full Disk
-ABI-L2-ACTPM,   Advanced Baseline Imager Level 2 Cloud Top Phase Mesoscale
-ABI-L2-ADPC,    Advanced Baseline Imager Level 2 Aerosol Detection CONUS
-ABI-L2-ADPF,    Advanced Baseline Imager Level 2 Aerosol Detection Full Disk
-ABI-L2-ADPM,    Advanced Baseline Imager Level 2 Aerosol Detection Mesoscale
-ABI-L2-AICEF,   Ice Concentration and Extent
-ABI-L2-AITAF,   Ice Age and Thickness
-ABI-L2-AODC,    Advanced Baseline Imager Level 2 Aerosol Optical Depth CONUS
-ABI-L2-AODF,    Advanced Baseline Imager Level 2 Aerosol Optical Depth Full Disk
-ABI-L2-BRFC,    Land Surface Bidirectional Reflectance Factor (CONUS) 2 km resolution & DQFs
-ABI-L2-BRFF,    Land Surface Bidirectional Reflectance Factor (Full Disk) 2 km resolution & DQFs
-ABI-L2-BRFM,    Land Surface Bidirectional Reflectance Factor (Mesoscale) 2 km resolution & DQFs
-ABI-L2-CMIPC,   Advanced Baseline Imager Level 2 Cloud and Moisture Imagery CONUS
-ABI-L2-CMIPF,   Advanced Baseline Imager Level 2 Cloud and Moisture Imagery Full Disk
-ABI-L2-CMIPM,   Advanced Baseline Imager Level 2 Cloud and Moisture Imagery Mesoscale
-ABI-L2-CODC,    Advanced Baseline Imager Level 2 Cloud Optical Depth CONUS
-ABI-L2-CODF,    Advanced Baseline Imager Level 2 Cloud Optical Depth Full Disk
-ABI-L2-CPSC,    Advanced Baseline Imager Level 2 Cloud Particle Size CONUS
-ABI-L2-CPSF,    Advanced Baseline Imager Level 2 Cloud Particle Size Full Disk
-ABI-L2-CPSM,    Advanced Baseline Imager Level 2 Cloud Particle Size Mesoscale
-ABI-L2-CTPC,    Advanced Baseline Imager Level 2 Cloud Top Pressure CONUS
-ABI-L2-CTPF,    Advanced Baseline Imager Level 2 Cloud Top Pressure Full Disk
-ABI-L2-DMWC,    Advanced Baseline Imager Level 2 Derived Motion Winds CONUS
-ABI-L2-DMWF,    Advanced Baseline Imager Level 2 Derived Motion Winds Full Disk
-ABI-L2-DMWM,    Advanced Baseline Imager Level 2 Derived Motion Winds Mesoscale
-ABI-L2-DMWVC,   L2+ Derived Motion Winds - Vapor CONUS
-ABI-L2-DMWVF,   L2+ Derived Motion Winds - Vapor Full Disk
-ABI-L2-DMWVM,   L2+ Derived Motion Winds - Vapor Mesoscale
-ABI-L2-DSIC,    Advanced Baseline Imager Level 2 Derived Stability Indices CONUS
-ABI-L2-DSIF,    Advanced Baseline Imager Level 2 Derived Stability Indices Full Disk
-ABI-L2-DSIM,    Advanced Baseline Imager Level 2 Derived Stability Indices Mesoscale
-ABI-L2-DSRC,    Advanced Baseline Imager Level 2 Downward Shortwave Radiation CONUS
-ABI-L2-DSRF,    Advanced Baseline Imager Level 2 Downward Shortwave Radiation Full Disk
-ABI-L2-DSRM,    Advanced Baseline Imager Level 2 Downward Shortwave Radiation Mesoscale
-ABI-L2-FDCC,    Advanced Baseline Imager Level 2 Fire (Hot Spot Characterization) CONUS
-ABI-L2-FDCF,    Advanced Baseline Imager Level 2 Fire (Hot Spot Characterization) Full Disk
-ABI-L2-FDCM,    Advanced Baseline Imager Level 2 Fire (Hot Spot Characterization) Mesoscale
-ABI-L2-LSAC,    Land Surface Albedo (CONUS) 2km resolution & DQFs
-ABI-L2-LSAF,    Land Surface Albedo (Full Disk) 2km resolution & DQFs
-ABI-L2-LSAM,    Land Surface Albedo (Mesoscale) 2km resolution & DQFs
-ABI-L2-LSTC,    Advanced Baseline Imager Level 2 Land Surface Temperature CONUS
-ABI-L2-LSTF,    Advanced Baseline Imager Level 2 Land Surface Temperature Full Disk
-ABI-L2-LSTM,    Advanced Baseline Imager Level 2 Land Surface Temperature Mesoscale
-ABI-L2-LVMPC,   Advanced Baseline Imager Level 2 Legacy Vertical Moisture Profile CONUS
-ABI-L2-LVMPF,   Advanced Baseline Imager Level 2 Legacy Vertical Moisture Profile Full Disk
-ABI-L2-LVMPM,   Advanced Baseline Imager Level 2 Legacy Vertical Moisture Profile Mesoscale
-ABI-L2-LVTPC,   Advanced Baseline Imager Level 2 Legacy Vertical Temperature Profile CONUS
-ABI-L2-LVTPF,   Advanced Baseline Imager Level 2 Legacy Vertical Temperature Profile Full Disk
-ABI-L2-LVTPM,   Advanced Baseline Imager Level 2 Legacy Vertical Temperature Profile Mesoscale
-ABI-L2-MCMIPC,  Advanced Baseline Imager Level 2 Cloud and Moisture Imagery CONUS
-ABI-L2-MCMIPF,  Advanced Baseline Imager Level 2 Cloud and Moisture Imagery Full Disk
-ABI-L2-MCMIPM,  Advanced Baseline Imager Level 2 Cloud and Moisture Imagery Mesoscale
-ABI-L2-RRQPEF,  Advanced Baseline Imager Level 2 Rainfall Rate (Quantitative Precipitation Estimate) Full Disk
-ABI-L2-RSRC,    Advanced Baseline Imager Level 2 Reflected Shortwave Radiation Top-Of-Atmosphere CONUS
-ABI-L2-RSRF,    Advanced Baseline Imager Level 2 Reflected Shortwave Radiation Top-Of-Atmosphere Full Disk
-ABI-L2-SSTF,    Advanced Baseline Imager Level 2 Sea Surface (Skin) Temperature Full Disk
-ABI-L2-TPWC,    Advanced Baseline Imager Level 2 Total Precipitable Water CONUS
-ABI-L2-TPWF,    Advanced Baseline Imager Level 2 Total Precipitable Water Full Disk
-ABI-L2-TPWM,    Advanced Baseline Imager Level 2 Total Precipitable Water Mesoscale
-ABI-L2-VAAF,    Advanced Baseline Imager Level 2 Volcanic Ash: Detection and Height Full Disk
-EXIS-L1b-SFEU,  EXIS-Solar Flux: EUV
-EXIS-L1b-SFXR,  EXIS-Solar Flux: X-Ray
-GLM-L2-LCFA,    Geostationary Lightning Mapper Level 2 Lightning Detection
-MAG-L1b-GEOF,   MAG-Geomagnetic Field
-SEIS-L1b-EHIS,  SEISS-Energetic Heavy Ions
-SEIS-L1b-MPSH,  SEISS-Mag. Electrons & Protons: Med & High Energy
-SEIS-L1b-MPSL,  SEISS-Mag. Electrons & Protons: Low Energy
-SEIS-L1b-SGPS,  SEISS-Solar & Galactic Protons
-SUVI-L1b-Fe093, Solar Ultraviolet Imager Level 1b Extreme Ultraviolet
-SUVI-L1b-Fe131, Solar Ultraviolet Imager Level 1b Extreme Ultraviolet
-SUVI-L1b-Fe171, Solar Ultraviolet Imager Level 1b Extreme Ultraviolet
-SUVI-L1b-Fe195, Solar Ultraviolet Imager Level 1b Extreme Ultraviolet
-SUVI-L1b-Fe284, Solar Ultraviolet Imager Level 1b Extreme Ultraviolet
-SUVI-L1b-He303, Solar Ultraviolet Imager Level 1b Extreme Ultraviolet
+# List of ABI products and their full description
+# From https://github.com/awslabs/open-data-docs/tree/main/docs/noaa/noaa-goes16
+ABI-L1b-RadF,   Advanced Baseline Imager Level 1b Full Disk
+ABI-L1b-RadC,   Advanced Baseline Imager Level 1b CONUS
+ABI-L1b-RadM,   Advanced Baseline Imager Level 1b Mesoscale
+ABI-L2-ACHAC,   Advanced Baseline Imager Level 2 Cloud Top Height CONUS
+ABI-L2-ACHAF,   Advanced Baseline Imager Level 2 Cloud Top Height Full Disk
+ABI-L2-ACHAM,   Advanced Baseline Imager Level 2 Cloud Top Height Mesoscale
+ABI-L2-ACHTF,   Advanced Baseline Imager Level 2 Cloud Top Temperature Full Disk
+ABI-L2-ACHTM,   Advanced Baseline Imager Level 2 Cloud Top Temperature Mesoscale
+ABI-L2-ACMC,    Advanced Baseline Imager Level 2 Clear Sky Mask CONUS
+ABI-L2-ACMF,    Advanced Baseline Imager Level 2 Clear Sky Mask Full Disk
+ABI-L2-ACMM,    Advanced Baseline Imager Level 2 Clear Sky Mask Mesoscale
+ABI-L2-ACTPC,   Advanced Baseline Imager Level 2 Cloud Top Phase CONUS
+ABI-L2-ACTPF,   Advanced Baseline Imager Level 2 Cloud Top Phase Full Disk
+ABI-L2-ACTPM,   Advanced Baseline Imager Level 2 Cloud Top Phase Mesoscale
+ABI-L2-ADPC,    Advanced Baseline Imager Level 2 Aerosol Detection CONUS
+ABI-L2-ADPF,    Advanced Baseline Imager Level 2 Aerosol Detection Full Disk
+ABI-L2-ADPM,    Advanced Baseline Imager Level 2 Aerosol Detection Mesoscale
+ABI-L2-AICEF,   Ice Concentration and Extent
+ABI-L2-AITAF,   Ice Age and Thickness
+ABI-L2-AODC,    Advanced Baseline Imager Level 2 Aerosol Optical Depth CONUS
+ABI-L2-AODF,    Advanced Baseline Imager Level 2 Aerosol Optical Depth Full Disk
+ABI-L2-BRFC,    Land Surface Bidirectional Reflectance Factor (CONUS) 2 km resolution & DQFs
+ABI-L2-BRFF,    Land Surface Bidirectional Reflectance Factor (Full Disk) 2 km resolution & DQFs
+ABI-L2-BRFM,    Land Surface Bidirectional Reflectance Factor (Mesoscale) 2 km resolution & DQFs
+ABI-L2-CMIPC,   Advanced Baseline Imager Level 2 Cloud and Moisture Imagery CONUS
+ABI-L2-CMIPF,   Advanced Baseline Imager Level 2 Cloud and Moisture Imagery Full Disk
+ABI-L2-CMIPM,   Advanced Baseline Imager Level 2 Cloud and Moisture Imagery Mesoscale
+ABI-L2-CODC,    Advanced Baseline Imager Level 2 Cloud Optical Depth CONUS
+ABI-L2-CODF,    Advanced Baseline Imager Level 2 Cloud Optical Depth Full Disk
+ABI-L2-CPSC,    Advanced Baseline Imager Level 2 Cloud Particle Size CONUS
+ABI-L2-CPSF,    Advanced Baseline Imager Level 2 Cloud Particle Size Full Disk
+ABI-L2-CPSM,    Advanced Baseline Imager Level 2 Cloud Particle Size Mesoscale
+ABI-L2-CTPC,    Advanced Baseline Imager Level 2 Cloud Top Pressure CONUS
+ABI-L2-CTPF,    Advanced Baseline Imager Level 2 Cloud Top Pressure Full Disk
+ABI-L2-DMWC,    Advanced Baseline Imager Level 2 Derived Motion Winds CONUS
+ABI-L2-DMWF,    Advanced Baseline Imager Level 2 Derived Motion Winds Full Disk
+ABI-L2-DMWM,    Advanced Baseline Imager Level 2 Derived Motion Winds Mesoscale
+ABI-L2-DMWVC,   L2+ Derived Motion Winds - Vapor CONUS
+ABI-L2-DMWVF,   L2+ Derived Motion Winds - Vapor Full Disk
+ABI-L2-DMWVM,   L2+ Derived Motion Winds - Vapor Mesoscale
+ABI-L2-DSIC,    Advanced Baseline Imager Level 2 Derived Stability Indices CONUS
+ABI-L2-DSIF,    Advanced Baseline Imager Level 2 Derived Stability Indices Full Disk
+ABI-L2-DSIM,    Advanced Baseline Imager Level 2 Derived Stability Indices Mesoscale
+ABI-L2-DSRC,    Advanced Baseline Imager Level 2 Downward Shortwave Radiation CONUS
+ABI-L2-DSRF,    Advanced Baseline Imager Level 2 Downward Shortwave Radiation Full Disk
+ABI-L2-DSRM,    Advanced Baseline Imager Level 2 Downward Shortwave Radiation Mesoscale
+ABI-L2-FDCC,    Advanced Baseline Imager Level 2 Fire (Hot Spot Characterization) CONUS
+ABI-L2-FDCF,    Advanced Baseline Imager Level 2 Fire (Hot Spot Characterization) Full Disk
+ABI-L2-FDCM,    Advanced Baseline Imager Level 2 Fire (Hot Spot Characterization) Mesoscale
+ABI-L2-LSAC,    Land Surface Albedo (CONUS) 2km resolution & DQFs
+ABI-L2-LSAF,    Land Surface Albedo (Full Disk) 2km resolution & DQFs
+ABI-L2-LSAM,    Land Surface Albedo (Mesoscale) 2km resolution & DQFs
+ABI-L2-LSTC,    Advanced Baseline Imager Level 2 Land Surface Temperature CONUS
+ABI-L2-LSTF,    Advanced Baseline Imager Level 2 Land Surface Temperature Full Disk
+ABI-L2-LSTM,    Advanced Baseline Imager Level 2 Land Surface Temperature Mesoscale
+ABI-L2-LVMPC,   Advanced Baseline Imager Level 2 Legacy Vertical Moisture Profile CONUS
+ABI-L2-LVMPF,   Advanced Baseline Imager Level 2 Legacy Vertical Moisture Profile Full Disk
+ABI-L2-LVMPM,   Advanced Baseline Imager Level 2 Legacy Vertical Moisture Profile Mesoscale
+ABI-L2-LVTPC,   Advanced Baseline Imager Level 2 Legacy Vertical Temperature Profile CONUS
+ABI-L2-LVTPF,   Advanced Baseline Imager Level 2 Legacy Vertical Temperature Profile Full Disk
+ABI-L2-LVTPM,   Advanced Baseline Imager Level 2 Legacy Vertical Temperature Profile Mesoscale
+ABI-L2-MCMIPC,  Advanced Baseline Imager Level 2 Cloud and Moisture Imagery CONUS
+ABI-L2-MCMIPF,  Advanced Baseline Imager Level 2 Cloud and Moisture Imagery Full Disk
+ABI-L2-MCMIPM,  Advanced Baseline Imager Level 2 Cloud and Moisture Imagery Mesoscale
+ABI-L2-RRQPEF,  Advanced Baseline Imager Level 2 Rainfall Rate (Quantitative Precipitation Estimate) Full Disk
+ABI-L2-RSRC,    Advanced Baseline Imager Level 2 Reflected Shortwave Radiation Top-Of-Atmosphere CONUS
+ABI-L2-RSRF,    Advanced Baseline Imager Level 2 Reflected Shortwave Radiation Top-Of-Atmosphere Full Disk
+ABI-L2-SSTF,    Advanced Baseline Imager Level 2 Sea Surface (Skin) Temperature Full Disk
+ABI-L2-TPWC,    Advanced Baseline Imager Level 2 Total Precipitable Water CONUS
+ABI-L2-TPWF,    Advanced Baseline Imager Level 2 Total Precipitable Water Full Disk
+ABI-L2-TPWM,    Advanced Baseline Imager Level 2 Total Precipitable Water Mesoscale
+ABI-L2-VAAF,    Advanced Baseline Imager Level 2 Volcanic Ash: Detection and Height Full Disk
+EXIS-L1b-SFEU,  EXIS-Solar Flux: EUV
+EXIS-L1b-SFXR,  EXIS-Solar Flux: X-Ray
+GLM-L2-LCFA,    Geostationary Lightning Mapper Level 2 Lightning Detection
+MAG-L1b-GEOF,   MAG-Geomagnetic Field
+SEIS-L1b-EHIS,  SEISS-Energetic Heavy Ions
+SEIS-L1b-MPSH,  SEISS-Mag. Electrons & Protons: Med & High Energy
+SEIS-L1b-MPSL,  SEISS-Mag. Electrons & Protons: Low Energy
+SEIS-L1b-SGPS,  SEISS-Solar & Galactic Protons
+SUVI-L1b-Fe093, Solar Ultraviolet Imager Level 1b Extreme Ultraviolet
+SUVI-L1b-Fe131, Solar Ultraviolet Imager Level 1b Extreme Ultraviolet
+SUVI-L1b-Fe171, Solar Ultraviolet Imager Level 1b Extreme Ultraviolet
+SUVI-L1b-Fe195, Solar Ultraviolet Imager Level 1b Extreme Ultraviolet
+SUVI-L1b-Fe284, Solar Ultraviolet Imager Level 1b Extreme Ultraviolet
+SUVI-L1b-He303, Solar Ultraviolet Imager Level 1b Extreme Ultraviolet
```

### Comparing `goes2go-2022.8.26/goes2go/rgb.py` & `goes2go-2023.4.0/goes2go/rgb.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,1108 +1,1107 @@
-## Brian Blaylock
-## August 8, 2019
-
-"""
-===========
-RGB Recipes
-===========
-
-.. image:: /_static/RGB_sample.png
-
-These functions take GOES-East or GOES-West multichannel data on a 
-fixed grid (files named ``ABI-L2-MCMIPC``) and generates a 3D 
-Red-Green-Blue (RGB) array for various GOES RGB products.
-
-RGB recipes are based on the `GOES Quick Guides
-<http://rammb.cira.colostate.edu/training/visit/quick_guides/>`_ 
-and include the following:
-
-    - NaturalColor
-    - TrueColor
-    - FireTemperature
-    - AirMass
-    - DayCloudPhase
-    - DayConvection
-    - DayCloudConvection
-    - DayLandCloud
-    - DayLandCloudFire
-    - WaterVapor
-    - DifferentialWaterVapor
-    - DaySnowFog
-    - NighttimeMicrophysics
-    - Dust
-    - SulfurDioxide
-    - Ash
-    - SplitWindowDifference
-    - NightFogDifference
-    - RocketPlume              ✨New - July 9, 2021
-
-The returned RGB can easily be viewed with ``plt.imshow(RGB)``. 
-
-For imshow to show an RGB image, the values must range between 0 and 1. 
-Values are normalized between the range specified in the Quick Guides. 
-This normalization is synonymous to `contrast or histogram stretching 
-<https://micro.magnet.fsu.edu/primer/java/digitalimaging/processing/histogramstretching/index.html>`_
-(`more info here
-<https://staff.fnwi.uva.nl/r.vandenboomgaard/IPCV20162017/LectureNotes/IP/PointOperators/ImageStretching.html>`_)
-and follows the formula:
-
-    .. code-block:: python 
-
-        NormalizedValue = (OriginalValue-LowerLimit)/(UpperLimit-LowerLimit)
-
-`Gamma correction <https://en.wikipedia.org/wiki/Gamma_correction>`_
-darkens or lightens an image (`more info 
-<https://www.cambridgeincolour.com/tutorials/gamma-correction.htm>`_) 
-and follows the decoding formula:
-
-    .. code-block:: python 
-        
-        R_corrected = R**(1/gamma)
-
-The input for all these functions are denoted by ``C`` for "channels" which
-represents the GOES ABI multichannel file opened with xarray. For example:
-
-    .. code-block:: python 
-        
-        FILE = 'OR_ABI-L2-MCMIPC-M6_G17_s20192201631196_e20192201633575_c20192201634109.nc'
-        C = xarray.open_dataset(FILE)
-
-All RGB products are demonstarted in the `make_RGB_Demo 
-<https://github.com/blaylockbk/goes2go/tree/master/notebooks>`_ notebook.
-
-Note: I don't have a `GeoColor <https://journals.ametsoc.org/view/journals/atot/37/3/JTECH-D-19-0134.1.xml>`_
-RGB, because it is much more involved than simply stacking RGB channels. If anyone does do
-something similar to a GeoColor image, let me know!
-
-ABI Band Reference
-------------------
-
-https://www.weather.gov/media/crp/GOES_16_Guides_FINALBIS.pdf
-http://cimss.ssec.wisc.edu/goes/GOESR_QuickGuides.html
-https://www.goes-r.gov/mission/ABI-bands-quick-info.html
-
-=============== ================== ============================================== ======================================
-ABI Band Number Central Wavelength  Name                                          Type
-=============== ================== ============================================== ======================================
-      1             0.47 μm        "Blue" Band                                    Visible
-      2             0.64 μm        "Red" Band                                     Visible
-      3             0.86 μm        "Veggie" Band                                  Near-IR
-      4             1.37 μm        "Cirrus" Band                                  Near-IR
-      5             1.6  μm        "Snow/Ice" Band                                Near-IR
-      6             2.2  μm        "Cloud Particle Size" Band                     Near-IR
-      7             3.9  μm        "Shortwave Window" Band                        IR (with reflected daytime component)
-      8             6.2  μm        "Upper-Level Tropospheric Water Vapor" Band    IR
-      9             6.9  μm        "Mid-Level Tropospheric Water Vapor" Band      IR
-      10            7.3  μm        "Lower-level Water Vapor" Band                 IR
-      11            8.4  μm        "Cloud-Top Phase" Band                         IR
-      12            9.6  μm        "Ozone Band"                                   IR
-      13            10.3 μm        "Clean" IR Longwave Window Band                IR
-      14            11.2 μm        IR Longwave Window Band                        IR
-      15            12.3 μm        "Dirty" Longwave Window Band                   IR
-      16            13.3 μm        "CO2" Longwave infrared                        IR
-=============== ================== ============================================== ======================================
-
-
-"""
-
-import numpy as np
-import matplotlib.pyplot as plt
-import cartopy.crs as ccrs
-import xarray as xr
-
-from goes2go.tools import field_of_view
-
-
-def get_imshow_kwargs(ds):
-    """
-    Help determine the ``plt.imshow`` arguments.
-
-    Parameters
-    ----------
-    ds : xarray.Dataset
-
-    Returns
-    -------
-    kwargs for the ``plt.imshow`` with the correct image extent limits.
-
-    Examples
-    --------
-
-    .. code:: python
-
-        r = TrueColor(G)
-        ax = common_features(r.crs)
-        ax.imshow(r.TrueColor, *\*\get_imshow_kwargs(r))
-
-    """
-    return dict(
-        extent=[ds.x2.data.min(), ds.x2.data.max(), ds.y2.data.min(), ds.y2.data.max()],
-        transform=ds.crs,
-        origin="upper",
-        interpolation="none",
-    )
-
-
-def rgb_as_dataset(G, RGB, description, latlon=False):
-    """
-    Assemble a dataset with the RGB array with other data from the file.
-
-    Parameters
-    ----------
-    G : xarray.Dataset
-        GOES ABI data from multispectral channel
-    RGB : array
-        A 3D array of R, G, and B values at each pixel
-    description : str
-        A description of what the RGB data represents.
-    latlon : bool
-        Derive the latitude and longitude of each pixel.
-
-    """
-    # Assemble a new xarray.Dataset for the RGB data
-    ds = xr.Dataset({description.replace(" ", ""): (["y", "x", "rgb"], RGB)})
-    ds.attrs["description"] = description
-
-    # Convert x, y points to latitude/longitude
-    _, crs = field_of_view(G)
-    sat_h = G.goes_imager_projection.perspective_point_height
-    x2 = G.x * sat_h
-    y2 = G.y * sat_h
-    ds.coords["x2"] = x2
-    ds.coords["y2"] = y2
-
-    ds["x2"].attrs["long_name"] = "x sweep in crs units (m); x * sat_height"
-    ds["y2"].attrs["long_name"] = "y sweep in crs units (m); y * sat_height"
-
-    ds.attrs["crs"] = crs
-
-    if latlon:
-        X, Y = np.meshgrid(x2, y2)
-        a = ccrs.PlateCarree().transform_points(crs, X, Y)
-        lons, lats, _ = a[:, :, 0], a[:, :, 1], a[:, :, 2]
-        ds.coords["longitude"] = (("y", "x"), lons)
-        ds.coords["latitude"] = (("y", "x"), lats)
-
-    # Copy some coordinates and attributes of interest from the original data
-    for i in ["x", "y", "t", "geospatial_lat_lon_extent"]:
-        ds.coords[i] = G[i]
-    for i in [
-        "orbital_slot",
-        "platform_ID",
-        "scene_id",
-        "spatial_resolution",
-        "instrument_type",
-        "title",
-    ]:
-        ds.attrs[i] = G.attrs[i]
-
-    ## Provide some helpers to plot with imshow
-    ds.attrs["imshow_kwargs"] = get_imshow_kwargs(ds)
-
-    ## Provide some helpers to plot with imshow and pcolormesh
-    ## Not super useful, because pcolormesh doesn't allow nans in x, y dimension
-    # pcolormesh_kwargs = dict(
-    #    color = RGB.reshape(np.shape(RGB)[0] * np.shape(RGB)[1], np.shape(RGB)[2])
-    #    shading='nearest'
-    #    )
-    # ds.attrs['pcolormesh_kwargs'] = pcolormesh_kwargs
-
-    return ds
-
-
-def load_RGB_channels(C, channels):
-    """
-    Return the R, G, and B arrays for the three channels requested. This
-    function will convert the data any units in Kelvin to Celsius.
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        The GOES multi-channel file opened with xarray.
-    channels : tuple of size 3
-        A tuple of the channel number for each (R, G, B).
-        For example ``channel=(2, 3, 1)`` is for the true color RGB
-
-    Returns
-    -------
-    A list with three items that are used for R, G, and B.
-    >>> R, G, B = load_RGB_channels(C, (2,3,1))
-
-    """
-    # Units of each channel requested
-    units = [C["CMI_C%02d" % c].units for c in channels]
-    RGB = []
-    for u, c in zip(units, channels):
-        if u == "K":
-            # Convert form Kelvin to Celsius
-            RGB.append(C["CMI_C%02d" % c].data - 273.15)
-        else:
-            RGB.append(C["CMI_C%02d" % c].data)
-    return RGB
-
-
-def gamma_correction(a, gamma, verbose=False):
-    """
-    Darken or lighten an image with `gamma correction
-    <https://en.wikipedia.org/wiki/Gamma_correction>`_.
-
-    Parameters
-    ----------
-    a : array-like
-        An array of values, typically the RGB array of values in
-        an image.
-    gamma : float
-        Gamma value to decode the image by.
-        Values > 1 will lighten an image.
-        Values < 1 will darken an image.
-    """
-    if verbose:
-        if gamma > 1:
-            print("Gamma Correction: 🌔 Lighten image")
-        elif gamma < 1:
-            print("Gamma Correction: 🌒 Darken image")
-        else:
-            print("Gamma Correction: 🌓 Gamma=1. No correction made.")
-            return a
-
-    # Gamma decoding formula
-    return np.power(a, 1 / gamma)
-
-
-def normalize(value, lower_limit, upper_limit, clip=True):
-    """
-    Normalize values between 0 and 1.
-
-    Normalize between a lower and upper limit. In other words, it
-    converts your number to a value in the range between 0 and 1.
-    Follows `normalization formula
-    <https://stats.stackexchange.com/a/70807/220885>`_
-
-    This is the same concept as `contrast or histogram stretching
-    <https://staff.fnwi.uva.nl/r.vandenboomgaard/IPCV20162017/LectureNotes/IP/PointOperators/ImageStretching.html>`_
-
-
-    .. code:: python
-
-        NormalizedValue = (OriginalValue-LowerLimit)/(UpperLimit-LowerLimit)
-
-    Parameters
-    ----------
-    value :
-        The original value. A single value, vector, or array.
-    upper_limit :
-        The upper limit.
-    lower_limit :
-        The lower limit.
-    clip : bool
-        - True: Clips values between 0 and 1 for RGB.
-        - False: Retain the numbers that extends outside 0-1 range.
-    Output:
-        Values normalized between the upper and lower limit.
-    """
-    norm = (value - lower_limit) / (upper_limit - lower_limit)
-    if clip:
-        norm = np.clip(norm, 0, 1)
-    return norm
-
-
-# ======================================================================
-# ======================================================================
-
-
-def TrueColor(C, gamma=2.2, pseudoGreen=True, night_IR=True, **kwargs):
-    """
-    True Color RGB:
-    (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_CIMSSRGB_v2.pdf>`__ for reference)
-
-    This is similar to the NaturalColor RGB, but uses a different gamma
-    correction and does not apply contrast stretching. I think these
-    images look a little "washed out" when compared to the NaturalColor
-    RGB. So, I would recommend using the NaturalColor RGB.
-
-    For more details on combing RGB and making the psedo green channel, refer to
-    `Bah et al. 2018 <https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2018EA000379>`_.
-
-    .. image:: /_static/TrueColor.png
-
-    .. image:: /_static/gamma_demo_TrueColor.png
-
-    .. image:: /_static/Color-IR_demo.png
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        A GOES ABI multichannel file opened with xarray.
-    gamma : float
-        Darken or lighten an image with `gamma correction
-        <https://en.wikipedia.org/wiki/Gamma_correction>`_.
-        Values > 1 will lighten an image.
-        Values < 1 will darken an image.
-    pseudoGreen : bool
-        True: returns the calculated "True" green color
-        False: returns the "veggie" channel
-    night_IR : bool
-        If True, use Clean IR (channel 13) as maximum RGB value overlay
-        so that cold clouds show up at night. (Be aware that some
-        daytime clouds might appear brighter).
-    \*\*kwargs :
-        Keyword arguments for ``rgb_as_dataset`` function.
-        - latlon : derive latitude and longitude of each pixel
-
-    """
-    # Load the three channels into appropriate R, G, and B variables
-    R, G, B = load_RGB_channels(C, (2, 3, 1))
-
-    # Apply range limits for each channel. RGB values must be between 0 and 1
-    R = np.clip(R, 0, 1)
-    G = np.clip(G, 0, 1)
-    B = np.clip(B, 0, 1)
-
-    # Apply a gamma correction to each R, G, B channel
-    R = gamma_correction(R, gamma)
-    G = gamma_correction(G, gamma)
-    B = gamma_correction(B, gamma)
-
-    if pseudoGreen:
-        # Calculate the "True" Green
-        G = 0.45 * R + 0.1 * G + 0.45 * B
-        G = np.clip(G, 0, 1)
-
-    if night_IR:
-        # Load the Clean IR channel
-        IR = C["CMI_C13"]
-        # Normalize between a range and clip
-        IR = normalize(IR, 90, 313, clip=True)
-        # Invert colors so cold clouds are white
-        IR = 1 - IR
-        # Lessen the brightness of the coldest clouds so they don't
-        # appear so bright when we overlay it on the true color image
-        IR = IR / 1.4
-        # RGB with IR as greyscale
-        RGB = np.dstack([np.maximum(R, IR), np.maximum(G, IR), np.maximum(B, IR)])
-    else:
-        RGB = np.dstack([R, G, B])
-
-    return rgb_as_dataset(C, RGB, "True Color", **kwargs)
-
-
-def NaturalColor(C, gamma=0.8, pseudoGreen=True, night_IR=False, **kwargs):
-    """
-    Natural Color RGB based on CIMSS method. Thanks Rick Kohrs!
-    (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_CIMSSRGB_v2.pdf>`__ for reference)
-
-    Check out Rick Kohrs `merged GOES images <https://www.ssec.wisc.edu/~rickk/local-noon.html>`_.
-
-    This NaturalColor RGB is *very* similar to the TrueColor RGB but
-    uses slightly different contrast stretches and ranges.
-
-    For more details on combing RGB and making the psedo green channel, refer to
-    `Bah et al. 2018 <https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2018EA000379>`_.
-
-    .. image:: /_static/NaturalColor.png
-
-    .. image:: /_static/gamma_demo_NaturalColor-PsuedoGreen.png
-
-    .. image:: /_static/gamma_demo_NaturalColor-VeggieGreen.png
-
-    .. image:: /_static/Color-IR_demo.png
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        A GOES ABI multichannel file opened ith xarray.
-    gamma : float
-        Darken or lighten an image with `gamma correction
-        <https://en.wikipedia.org/wiki/Gamma_correction>`_.
-        Values > 1 will lighten an image.
-        Values < 1 will darken an image.
-    night_IR : bool
-        If True, use Clean IR (channel 13) as maximum RGB value overlay
-        so that cold clouds show up at night. (Be aware that some
-        daytime clouds might appear brighter).
-    \*\*kwargs :
-        Keyword arguments for ``rgb_as_dataset`` function.
-        - latlon : derive latitude and longitude of each pixel
-    """
-
-    def breakpoint_stretch(C, breakpoint):
-        """
-        Contrast stretching by break point (number provided by Rick Kohrs)
-        """
-        lower = normalize(C, 0, 10)  # Low end
-        upper = normalize(C, 10, 255)  # High end
-
-        # Combine the two datasets
-        # This works because if upper=1 and lower==.7, then
-        # that means the upper value was out of range and the
-        # value for the lower pass was used instead.
-        combined = np.minimum(lower, upper)
-
-        return combined
-
-    # Load the three channels into appropriate R, G, and B variables
-    R, G, B = load_RGB_channels(C, (2, 3, 1))
-
-    # Apply range limits for each channel. RGB values must be between 0 and 1
-    R = np.clip(R, 0, 1)
-    G = np.clip(G, 0, 1)
-    B = np.clip(B, 0, 1)
-
-    if pseudoGreen:
-        # Derive pseudo Green channel
-        G = 0.45 * R + 0.1 * G + 0.45 * B
-        G = np.clip(G, 0, 1)
-
-    # Convert Albedo to Brightness, ranging from 0-255 K
-    # (numbers based on email from Rick Kohrs)
-    R = np.sqrt(R * 100) * 25.5
-    G = np.sqrt(G * 100) * 25.5
-    B = np.sqrt(B * 100) * 25.5
-
-    # Apply contrast stretching based on breakpoints
-    # (numbers based on email form Rick Kohrs)
-    R = breakpoint_stretch(R, 33)
-    G = breakpoint_stretch(G, 40)
-    B = breakpoint_stretch(B, 50)
-
-    if night_IR:
-        # Load the Clean IR channel
-        IR = C["CMI_C13"]
-        # Normalize between a range and clip
-        IR = normalize(IR, 90, 313, clip=True)
-        # Invert colors so cold clouds are white
-        IR = 1 - IR
-        # Lessen the brightness of the coldest clouds so they don't
-        # appear so bright when we overlay it on the true color image
-        IR = IR / 1.4
-        # Overlay IR channel, as greyscale image (use IR in R, G, and B)
-        RGB = np.dstack([np.maximum(R, IR), np.maximum(G, IR), np.maximum(B, IR)])
-    else:
-        RGB = np.dstack([R, G, B])
-
-    # Apply a gamma correction to the image
-    RGB = gamma_correction(RGB, gamma)
-
-    return rgb_as_dataset(C, RGB, "Natural Color", **kwargs)
-
-
-def FireTemperature(C, **kwargs):
-    """
-    Fire Temperature RGB:
-    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Fire_Temperature_RGB.pdf>`__ for reference)
-
-    .. image:: /_static/FireTemperature.png
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        A GOES ABI multichannel file opened with xarray.
-    \*\*kwargs :
-        Keyword arguments for ``rgb_as_dataset`` function.
-        - latlon : derive latitude and longitude of each pixel
-
-    """
-    # Load the three channels into appropriate R, G, and B variables
-    R, G, B = load_RGB_channels(C, (7, 6, 5))
-
-    # Normalize each channel by the appropriate range of values (clipping happens in function)
-    R = normalize(R, 273, 333)
-    G = normalize(G, 0, 1)
-    B = normalize(B, 0, 0.75)
-
-    # Apply the gamma correction to Red channel.
-    #   corrected_value = value^(1/gamma)
-    gamma = 0.4
-    R = gamma_correction(R, gamma)
-
-    # The final RGB array :)
-    RGB = np.dstack([R, G, B])
-
-    return rgb_as_dataset(C, RGB, "Fire Temperature", **kwargs)
-
-
-def AirMass(C, **kwargs):
-    """
-    Air Mass RGB:
-    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_AirMassRGB_final.pdf>`__ for reference)
-
-    .. image:: /_static/AirMass.png
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        A GOES ABI multichannel file opened with xarray.
-    \*\*kwargs :
-        Keyword arguments for ``rgb_as_dataset`` function.
-        - latlon : derive latitude and longitude of each pixel
-
-    """
-    # Load the three channels into appropriate R, G, and B variables
-    R = C["CMI_C08"].data - C["CMI_C10"].data
-    G = C["CMI_C12"].data - C["CMI_C13"].data
-    B = C["CMI_C08"].data - 273.15  # remember to convert to Celsius
-
-    # Normalize each channel by the appropriate range of values. e.g. R = (R-minimum)/(maximum-minimum)
-    R = normalize(R, -26.2, 0.6)
-    G = normalize(G, -42.2, 6.7)
-    B = normalize(B, -64.65, -29.25)
-
-    # Invert B
-    B = 1 - B
-
-    # The final RGB array :)
-    RGB = np.dstack([R, G, B])
-
-    return rgb_as_dataset(C, RGB, "Air Mass", **kwargs)
-
-
-def DayCloudPhase(C, **kwargs):
-    """
-    Day Cloud Phase Distinction RGB:
-    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Day_Cloud_Phase_Distinction.pdf>`__ for reference)
-
-    .. image:: /_static/DayCloudPhase.png
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        A GOES ABI multichannel file opened with xarray.
-    \*\*kwargs :
-        Keyword arguments for ``rgb_as_dataset`` function.
-        - latlon : derive latitude and longitude of each pixel
-
-    """
-    # Load the three channels into appropriate R, G, and B variables
-    R, G, B = load_RGB_channels(C, (13, 2, 5))
-
-    # Normalize each channel by the appropriate range of values. (Clipping happens inside function)
-    R = normalize(R, -53.5, 7.5)
-    G = normalize(G, 0, 0.78)
-    B = normalize(B, 0.01, 0.59)
-
-    # Invert R
-    R = 1 - R
-
-    # The final RGB array :)
-    RGB = np.dstack([R, G, B])
-
-    return rgb_as_dataset(C, RGB, "Day Cloud Phase", **kwargs)
-
-
-def DayConvection(C, **kwargs):
-    """
-    Day Convection RGB:
-    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DayConvectionRGB_final.pdf>`__ for reference)
-
-    .. image:: /_static/DayConvection.png
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        A GOES ABI multichannel file opened with xarray.
-    \*\*kwargs :
-        Keyword arguments for ``rgb_as_dataset`` function.
-        - latlon : derive latitude and longitude of each pixel
-
-    """
-    # Load the three channels into appropriate R, G, and B variables
-    # NOTE: Each R, G, B is a channel difference.
-    R = C["CMI_C08"].data - C["CMI_C10"].data
-    G = C["CMI_C07"].data - C["CMI_C13"].data
-    B = C["CMI_C05"].data - C["CMI_C02"].data
-
-    # Normalize each channel by the appropriate range of values.
-    R = normalize(R, -35, 5)
-    G = normalize(G, -5, 60)
-    B = normalize(B, -0.75, 0.25)
-
-    # The final RGB array :)
-    RGB = np.dstack([R, G, B])
-
-    return rgb_as_dataset(C, RGB, "Day Convection", **kwargs)
-
-
-def DayCloudConvection(C, **kwargs):
-    """
-    Day Cloud Convection RGB:
-    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_DayCloudConvectionRGB_final.pdf>`__ for reference)
-
-    .. image:: /_static/DayCloudConvection.png
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        A GOES ABI multichannel file opened with xarray.
-    \*\*kwargs :
-        Keyword arguments for ``rgb_as_dataset`` function.
-        - latlon : derive latitude and longitude of each pixel
-
-    """
-    # Load the three channels into appropriate R, G, and B variables
-    R, G, B = load_RGB_channels(C, (2, 2, 13))
-
-    # Normalize each channel by the appropriate range of values.
-    R = normalize(R, 0, 1)
-    G = normalize(G, 0, 1)
-    B = normalize(B, -70.15, 49.85)
-
-    # Invert B
-    B = 1 - B
-
-    # Apply the gamma correction to Red channel.
-    #   corrected_value = value^(1/gamma)
-    gamma = 1.7
-    R = gamma_correction(R, gamma)
-    G = gamma_correction(G, gamma)
-
-    # The final RGB array :)
-    RGB = np.dstack([R, G, B])
-
-    return rgb_as_dataset(C, RGB, "Day Cloud Convection", **kwargs)
-
-
-def DayLandCloud(C, **kwargs):
-    """
-    Day Land Cloud Fire RGB:
-    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_daylandcloudRGB_final.pdf>`__ for reference)
-
-    .. image:: /_static/DayLandCloud.png
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        A GOES ABI multichannel file opened with xarray.
-    \*\*kwargs :
-        Keyword arguments for ``rgb_as_dataset`` function.
-        - latlon : derive latitude and longitude of each pixel
-
-    """
-    # Load the three channels into appropriate R, G, and B variables
-    R, G, B = load_RGB_channels(C, (5, 3, 2))
-
-    # Normalize each channel by the appropriate range of values  e.g. R = (R-minimum)/(maximum-minimum)
-    R = normalize(R, 0, 0.975)
-    G = normalize(G, 0, 1.086)
-    B = normalize(B, 0, 1)
-
-    # The final RGB array :)
-    RGB = np.dstack([R, G, B])
-
-    return rgb_as_dataset(C, RGB, "Day Land Cloud", **kwargs)
-
-
-def DayLandCloudFire(C, **kwargs):
-    """
-    Day Land Cloud Fire RGB:
-    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DayLandCloudFireRGB_final.pdf>`__ for reference)
-
-    .. image:: /_static/DayLandCloudFire.png
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        A GOES ABI multichannel file opened with xarray.
-    \*\*kwargs :
-        Keyword arguments for ``rgb_as_dataset`` function.
-        - latlon : derive latitude and longitude of each pixel
-
-    """
-    # Load the three channels into appropriate R, G, and B variables
-    R, G, B = load_RGB_channels(C, (6, 3, 2))
-
-    # Normalize each channel by the appropriate range of values  e.g. R = (R-minimum)/(maximum-minimum)
-    R = normalize(R, 0, 1)
-    G = normalize(G, 0, 1)
-    B = normalize(B, 0, 1)
-
-    # The final RGB array :)
-    RGB = np.dstack([R, G, B])
-
-    return rgb_as_dataset(C, RGB, "Day Land Cloud Fire", **kwargs)
-
-
-def WaterVapor(C, **kwargs):
-    """
-    Simple Water Vapor RGB:
-    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Simple_Water_Vapor_RGB.pdf>`__ for reference)
-
-    .. image:: /_static/WaterVapor.png
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        A GOES ABI multichannel file opened with xarray.
-    \*\*kwargs :
-        Keyword arguments for ``rgb_as_dataset`` function.
-        - latlon : derive latitude and longitude of each pixel
-
-    """
-    # Load the three channels into appropriate R, G, and B variables.
-    R, G, B = load_RGB_channels(C, (13, 8, 10))
-
-    # Normalize each channel by the appropriate range of values. e.g. R = (R-minimum)/(maximum-minimum)
-    R = normalize(R, -70.86, 5.81)
-    G = normalize(G, -58.49, -30.48)
-    B = normalize(B, -28.03, -12.12)
-
-    # Invert the colors
-    R = 1 - R
-    G = 1 - G
-    B = 1 - B
-
-    # The final RGB array :)
-    RGB = np.dstack([R, G, B])
-
-    return rgb_as_dataset(C, RGB, "Water Vapor", **kwargs)
-
-
-def DifferentialWaterVapor(C, **kwargs):
-    """
-    Differential Water Vapor RGB:
-    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DifferentialWaterVaporRGB_final.pdf>`__ for reference)
-
-    .. image:: /_static/DifferentialWaterVapor.png
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        A GOES ABI multichannel file opened with xarray.
-    \*\*kwargs :
-        Keyword arguments for ``rgb_as_dataset`` function.
-        - latlon : derive latitude and longitude of each pixel
-
-    """
-    # Load the three channels into appropriate R, G, and B variables.
-    R = C["CMI_C10"].data - C["CMI_C08"].data
-    G = C["CMI_C10"].data - 273.15
-    B = C["CMI_C08"].data - 273.15
-
-    # Normalize each channel by the appropriate range of values. e.g. R = (R-minimum)/(maximum-minimum)
-    R = normalize(R, -3, 30)
-    G = normalize(G, -60, 5)
-    B = normalize(B, -64.65, -29.25)
-
-    # Gamma correction
-    R = gamma_correction(R, 0.2587)
-    G = gamma_correction(G, 0.4)
-    B = gamma_correction(B, 0.4)
-
-    # Invert the colors
-    R = 1 - R
-    G = 1 - G
-    B = 1 - B
-
-    # The final RGB array :)
-    RGB = np.dstack([R, G, B])
-
-    return rgb_as_dataset(C, RGB, "Differenctial Water Vapor", **kwargs)
-
-
-def DaySnowFog(C, **kwargs):
-    """
-    Day Snow-Fog RGB:
-    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_DaySnowFog.pdf>`__ for reference)
-
-    .. image:: /_static/DaySnowFog.png
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        A GOES ABI multichannel file opened with xarray.
-    \*\*kwargs :
-        Keyword arguments for ``rgb_as_dataset`` function.
-        - latlon : derive latitude and longitude of each pixel
-
-    """
-    # Load the three channels into appropriate R, G, and B variables
-    R = C["CMI_C03"].data
-    G = C["CMI_C05"].data
-    B = C["CMI_C07"].data - C["CMI_C13"].data
-
-    # Normalize values
-    R = normalize(R, 0, 1)
-    G = normalize(G, 0, 0.7)
-    B = normalize(B, 0, 30)
-
-    # Apply a gamma correction to the image
-    gamma = 1.7
-    R = gamma_correction(R, gamma)
-    G = gamma_correction(G, gamma)
-    B = gamma_correction(B, gamma)
-
-    # The final RGB array :)
-    RGB = np.dstack([R, G, B])
-
-    return rgb_as_dataset(C, RGB, "Day Snow Fog", **kwargs)
-
-
-def NighttimeMicrophysics(C, **kwargs):
-    """
-    Nighttime Microphysics RGB:
-    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_NtMicroRGB_final.pdf>`__ for reference)
-
-    .. image:: /_static/NighttimeMicrophysics.png
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        A GOES ABI multichannel file opened with xarray.
-    \*\*kwargs :
-        Keyword arguments for ``rgb_as_dataset`` function.
-        - latlon : derive latitude and longitude of each pixel
-
-    """
-    # Load the three channels into appropriate R, G, and B variables
-    R = C["CMI_C15"].data - C["CMI_C13"].data
-    G = C["CMI_C13"].data - C["CMI_C07"].data
-    B = C["CMI_C13"].data - 273.15
-
-    # Normalize values
-    R = normalize(R, -6.7, 2.6)
-    G = normalize(G, -3.1, 5.2)
-    B = normalize(B, -29.6, 19.5)
-
-    # The final RGB array :)
-    RGB = np.dstack([R, G, B])
-
-    return rgb_as_dataset(C, RGB, "Nighttime Microphysics", **kwargs)
-
-
-def Dust(C, **kwargs):
-    """
-    SulfurDioxide RGB:
-    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Dust_RGB_Quick_Guide.pdf>`__ for reference)
-
-    .. image:: /_static/Dust.png
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        A GOES ABI multichannel file opened with xarray.
-    \*\*kwargs :
-        Keyword arguments for ``rgb_as_dataset`` function.
-        - latlon : derive latitude and longitude of each pixel
-
-    """
-    # Load the three channels into appropriate R, G, and B variables
-    R = C["CMI_C15"].data - C["CMI_C13"].data
-    G = C["CMI_C14"].data - C["CMI_C11"].data
-    B = C["CMI_C13"].data - 273.15
-
-    # Normalize values
-    R = normalize(R, -6.7, 2.6)
-    G = normalize(G, -0.5, 20)
-    B = normalize(B, -11.95, 15.55)
-
-    # Apply a gamma correction to the image
-    gamma = 2.5
-    G = gamma_correction(G, gamma)
-
-    # The final RGB array :)
-    RGB = np.dstack([R, G, B])
-
-    return rgb_as_dataset(C, RGB, "Dust", **kwargs)
-
-
-def SulfurDioxide(C, **kwargs):
-    """
-    SulfurDioxide RGB:
-    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Quick_Guide_SO2_RGB.pdf>`__ for reference)
-
-    .. image:: /_static/SulfurDioxide.png
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        A GOES ABI multichannel file opened with xarray.
-    \*\*kwargs :
-        Keyword arguments for ``rgb_as_dataset`` function.
-        - latlon : derive latitude and longitude of each pixel
-
-    """
-    # Load the three channels into appropriate R, G, and B variables
-    R = C["CMI_C09"].data - C["CMI_C10"].data
-    G = C["CMI_C13"].data - C["CMI_C11"].data
-    B = C["CMI_C07"].data - 273.15
-
-    # Normalize values
-    R = normalize(R, -4, 2)
-    G = normalize(G, -4, 5)
-    B = normalize(B, -30.1, 29.8)
-
-    # The final RGB array :)
-    RGB = np.dstack([R, G, B])
-
-    return rgb_as_dataset(C, RGB, "Sulfur Dioxide", **kwargs)
-
-
-def Ash(C, **kwargs):
-    """
-    Ash RGB:
-    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/GOES_Ash_RGB.pdf>`__ for reference)
-
-    .. image:: /_static/Ash.png
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        A GOES ABI multichannel file opened with xarray.
-    \*\*kwargs :
-        Keyword arguments for ``rgb_as_dataset`` function.
-        - latlon : derive latitude and longitude of each pixel
-
-    """
-    # Load the three channels into appropriate R, G, and B variables
-    R = C["CMI_C15"].data - C["CMI_C13"].data
-    G = C["CMI_C14"].data - C["CMI_C11"].data
-    B = C["CMI_C13"].data - 273.15
-
-    # Normalize values
-    R = normalize(R, -6.7, 2.6)
-    G = normalize(G, -6, 6.3)
-    B = normalize(B, -29.55, 29.25)
-
-    # The final RGB array :)
-    RGB = np.dstack([R, G, B])
-
-    return rgb_as_dataset(C, RGB, "Ash", **kwargs)
-
-
-def SplitWindowDifference(C, **kwargs):
-    """
-    Split Window Difference RGB (greyscale):
-    (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_SplitWindowDifference.pdf>`__ for reference)
-
-    .. image:: /_static/SplitWindowDifference.png
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        A GOES ABI multichannel file opened with xarray.
-    \*\*kwargs :
-        Keyword arguments for ``rgb_as_dataset`` function.
-        - latlon : derive latitude and longitude of each pixel
-
-    """
-    # Load the three channels into appropriate R, G, and B variables
-    data = C["CMI_C15"].data - C["CMI_C13"].data
-
-    # Normalize values
-    data = normalize(data, -10, 10)
-
-    # The final RGB array :)
-    RGB = np.dstack([data, data, data])
-
-    return rgb_as_dataset(C, RGB, "Split Window Difference", **kwargs)
-
-
-def NightFogDifference(C, **kwargs):
-    """
-    Night Fog Difference RGB (greyscale):
-    (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_NightFogBTD.pdf>`__ for reference)
-
-    .. image:: /_static/NightFogDifference.png
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        A GOES ABI multichannel file opened with xarray.
-    \*\*kwargs :
-        Keyword arguments for ``rgb_as_dataset`` function.
-        - latlon : derive latitude and longitude of each pixel
-
-    """
-    # Load the three channels into appropriate R, G, and B variables
-    data = C["CMI_C13"].data - C["CMI_C07"].data
-
-    # Normalize values
-    data = normalize(data, -90, 15)
-
-    # Invert data
-    data = 1 - data
-
-    # The final RGB array :)
-    RGB = np.dstack([data, data, data])
-
-    return rgb_as_dataset(C, RGB, "Night Fog Difference", **kwargs)
-
-
-def RocketPlume(C, night=False, **kwargs):
-    """
-    Rocket Plume RGB
-
-    For identifying rocket launches.
-
-    See `this blog <https://cimss.ssec.wisc.edu/satellite-blog/archives/41335>`__ and
-    the `Quick Guide <https://cimss.ssec.wisc.edu/satellite-blog/images/2021/06/QuickGuide_Template_GOESRBanner_Rocket_Plume.pdf>`__
-    for reference
-
-    .. image:: /_static/RocketPlume.png
-
-    Parameters
-    ----------
-    C : xarray.Dataset
-        A GOES ABI multichannel file opened with xarray.
-    night : bool
-        If the area is in night, turn this on to use a different channel
-        than the daytime application.
-    \*\*kwargs :
-        Keyword arguments for ``rgb_as_dataset`` function.
-        - latlon : derive latitude and longitude of each pixel
-
-    """
-    # Load the three channels into appropriate R, G, and B variables
-    R = C["CMI_C07"].data
-    G = C["CMI_C08"].data
-    if not night:
-        B = C["CMI_C02"].data
-    else:
-        B = C["CMI_C05"].data
-
-    # Normalize values
-    R = normalize(R, 273, 338)
-    G = normalize(G, 233, 253)
-    B = normalize(B, 0, 0.80)
-
-    # The final RGB array :)
-    RGB = np.dstack([R, G, B])
-
-    return rgb_as_dataset(C, RGB, "RocketPlume", **kwargs)
-
-
-#######################
-# 🚧 Construction Zone
-#######################
-def NormalizedBurnRatio(C, **kwargs):
-    """
-    Normalized Burn Ratio
-
-    **THIS FUNCTION IS NOT FULLY DEVELOPED. Need more info.**
-
-    NBR= (0.86 µm – 2.2 µm)/(0.86 um + 2.2 um)
-
-
-    https://ntrs.nasa.gov/citations/20190030825
-
-    Parameters
-    ----------
-
-    """
-    # Load the three channels into appropriate R, G, and B variables
-    C3 = C["CMI_C03"].data
-    C6 = C["CMI_C06"].data
-    data = (C3 - C6) / (C3 + C6)
-
-    # Invert data
-    # data = 1-data
-
-    # The final RGB array :)
-    RGB = np.dstack([data, data, data])
-
-    return rgb_as_dataset(C, RGB, "Normalized Burn Ratio", **kwargs)
-
-
-if __name__ == "__main__":
-
-    # Create images of each for Docs
-    print("nothing here for now")
+## Brian Blaylock
+## August 8, 2019
+
+"""
+===========
+RGB Recipes
+===========
+
+.. image:: /_static/RGB_sample.png
+
+These functions take GOES-East or GOES-West multichannel data on a 
+fixed grid (files named ``ABI-L2-MCMIPC``) and generates a 3D 
+Red-Green-Blue (RGB) array for various GOES RGB products.
+
+RGB recipes are based on the `GOES Quick Guides
+<http://rammb.cira.colostate.edu/training/visit/quick_guides/>`_ 
+and include the following:
+
+    - NaturalColor
+    - TrueColor
+    - FireTemperature
+    - AirMass
+    - DayCloudPhase
+    - DayConvection
+    - DayCloudConvection
+    - DayLandCloud
+    - DayLandCloudFire
+    - WaterVapor
+    - DifferentialWaterVapor
+    - DaySnowFog
+    - NighttimeMicrophysics
+    - Dust
+    - SulfurDioxide
+    - Ash
+    - SplitWindowDifference
+    - NightFogDifference
+    - RocketPlume              ✨New - July 9, 2021
+
+The returned RGB can easily be viewed with ``plt.imshow(RGB)``. 
+
+For imshow to show an RGB image, the values must range between 0 and 1. 
+Values are normalized between the range specified in the Quick Guides. 
+This normalization is synonymous to `contrast or histogram stretching 
+<https://micro.magnet.fsu.edu/primer/java/digitalimaging/processing/histogramstretching/index.html>`_
+(`more info here
+<https://staff.fnwi.uva.nl/r.vandenboomgaard/IPCV20162017/LectureNotes/IP/PointOperators/ImageStretching.html>`_)
+and follows the formula:
+
+    .. code-block:: python 
+
+        NormalizedValue = (OriginalValue-LowerLimit)/(UpperLimit-LowerLimit)
+
+`Gamma correction <https://en.wikipedia.org/wiki/Gamma_correction>`_
+darkens or lightens an image (`more info 
+<https://www.cambridgeincolour.com/tutorials/gamma-correction.htm>`_) 
+and follows the decoding formula:
+
+    .. code-block:: python 
+        
+        R_corrected = R**(1/gamma)
+
+The input for all these functions are denoted by ``C`` for "channels" which
+represents the GOES ABI multichannel file opened with xarray. For example:
+
+    .. code-block:: python 
+        
+        FILE = 'OR_ABI-L2-MCMIPC-M6_G17_s20192201631196_e20192201633575_c20192201634109.nc'
+        C = xarray.open_dataset(FILE)
+
+All RGB products are demonstarted in the `make_RGB_Demo 
+<https://github.com/blaylockbk/goes2go/tree/master/notebooks>`_ notebook.
+
+Note: I don't have a `GeoColor <https://journals.ametsoc.org/view/journals/atot/37/3/JTECH-D-19-0134.1.xml>`_
+RGB, because it is much more involved than simply stacking RGB channels. If anyone does do
+something similar to a GeoColor image, let me know!
+
+ABI Band Reference
+------------------
+
+https://www.weather.gov/media/crp/GOES_16_Guides_FINALBIS.pdf
+http://cimss.ssec.wisc.edu/goes/GOESR_QuickGuides.html
+https://www.goes-r.gov/mission/ABI-bands-quick-info.html
+
+=============== ================== ============================================== ======================================
+ABI Band Number Central Wavelength  Name                                          Type
+=============== ================== ============================================== ======================================
+      1             0.47 μm        "Blue" Band                                    Visible
+      2             0.64 μm        "Red" Band                                     Visible
+      3             0.86 μm        "Veggie" Band                                  Near-IR
+      4             1.37 μm        "Cirrus" Band                                  Near-IR
+      5             1.6  μm        "Snow/Ice" Band                                Near-IR
+      6             2.2  μm        "Cloud Particle Size" Band                     Near-IR
+      7             3.9  μm        "Shortwave Window" Band                        IR (with reflected daytime component)
+      8             6.2  μm        "Upper-Level Tropospheric Water Vapor" Band    IR
+      9             6.9  μm        "Mid-Level Tropospheric Water Vapor" Band      IR
+      10            7.3  μm        "Lower-level Water Vapor" Band                 IR
+      11            8.4  μm        "Cloud-Top Phase" Band                         IR
+      12            9.6  μm        "Ozone Band"                                   IR
+      13            10.3 μm        "Clean" IR Longwave Window Band                IR
+      14            11.2 μm        IR Longwave Window Band                        IR
+      15            12.3 μm        "Dirty" Longwave Window Band                   IR
+      16            13.3 μm        "CO2" Longwave infrared                        IR
+=============== ================== ============================================== ======================================
+
+
+"""
+
+import numpy as np
+import matplotlib.pyplot as plt
+import cartopy.crs as ccrs
+import xarray as xr
+
+from goes2go.tools import field_of_view
+
+
+def get_imshow_kwargs(ds):
+    """
+    Help determine the ``plt.imshow`` arguments.
+
+    Parameters
+    ----------
+    ds : xarray.Dataset
+
+    Returns
+    -------
+    kwargs for the ``plt.imshow`` with the correct image extent limits.
+
+    Examples
+    --------
+
+    .. code:: python
+
+        r = TrueColor(G)
+        ax = common_features(r.crs)
+        ax.imshow(r.TrueColor, *\*\get_imshow_kwargs(r))
+
+    """
+    return dict(
+        extent=[ds.x2.data.min(), ds.x2.data.max(), ds.y2.data.min(), ds.y2.data.max()],
+        transform=ds.crs,
+        origin="upper",
+        interpolation="none",
+    )
+
+
+def rgb_as_dataset(G, RGB, description, latlon=False):
+    """
+    Assemble a dataset with the RGB array with other data from the file.
+
+    Parameters
+    ----------
+    G : xarray.Dataset
+        GOES ABI data from multispectral channel
+    RGB : array
+        A 3D array of R, G, and B values at each pixel
+    description : str
+        A description of what the RGB data represents.
+    latlon : bool
+        Derive the latitude and longitude of each pixel.
+
+    """
+    # Assemble a new xarray.Dataset for the RGB data
+    ds = xr.Dataset({description.replace(" ", ""): (["y", "x", "rgb"], RGB)})
+    ds.attrs["description"] = description
+
+    # Convert x, y points to latitude/longitude
+    _, crs = field_of_view(G)
+    sat_h = G.goes_imager_projection.perspective_point_height
+    x2 = G.x * sat_h
+    y2 = G.y * sat_h
+    ds.coords["x2"] = x2
+    ds.coords["y2"] = y2
+
+    ds["x2"].attrs["long_name"] = "x sweep in crs units (m); x * sat_height"
+    ds["y2"].attrs["long_name"] = "y sweep in crs units (m); y * sat_height"
+
+    ds.attrs["crs"] = crs
+
+    if latlon:
+        X, Y = np.meshgrid(x2, y2)
+        a = ccrs.PlateCarree().transform_points(crs, X, Y)
+        lons, lats, _ = a[:, :, 0], a[:, :, 1], a[:, :, 2]
+        ds.coords["longitude"] = (("y", "x"), lons)
+        ds.coords["latitude"] = (("y", "x"), lats)
+
+    # Copy some coordinates and attributes of interest from the original data
+    for i in ["x", "y", "t", "geospatial_lat_lon_extent"]:
+        ds.coords[i] = G[i]
+    for i in [
+        "orbital_slot",
+        "platform_ID",
+        "scene_id",
+        "spatial_resolution",
+        "instrument_type",
+        "title",
+    ]:
+        ds.attrs[i] = G.attrs[i]
+
+    ## Provide some helpers to plot with imshow
+    ds.attrs["imshow_kwargs"] = get_imshow_kwargs(ds)
+
+    ## Provide some helpers to plot with imshow and pcolormesh
+    ## Not super useful, because pcolormesh doesn't allow nans in x, y dimension
+    # pcolormesh_kwargs = dict(
+    #    color = RGB.reshape(np.shape(RGB)[0] * np.shape(RGB)[1], np.shape(RGB)[2])
+    #    shading='nearest'
+    #    )
+    # ds.attrs['pcolormesh_kwargs'] = pcolormesh_kwargs
+
+    return ds
+
+
+def load_RGB_channels(C, channels):
+    """
+    Return the R, G, and B arrays for the three channels requested. This
+    function will convert the data any units in Kelvin to Celsius.
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        The GOES multi-channel file opened with xarray.
+    channels : tuple of size 3
+        A tuple of the channel number for each (R, G, B).
+        For example ``channel=(2, 3, 1)`` is for the true color RGB
+
+    Returns
+    -------
+    A list with three items that are used for R, G, and B.
+    >>> R, G, B = load_RGB_channels(C, (2,3,1))
+
+    """
+    # Units of each channel requested
+    units = [C["CMI_C%02d" % c].units for c in channels]
+    RGB = []
+    for u, c in zip(units, channels):
+        if u == "K":
+            # Convert form Kelvin to Celsius
+            RGB.append(C["CMI_C%02d" % c].data - 273.15)
+        else:
+            RGB.append(C["CMI_C%02d" % c].data)
+    return RGB
+
+
+def gamma_correction(a, gamma, verbose=False):
+    """
+    Darken or lighten an image with `gamma correction
+    <https://en.wikipedia.org/wiki/Gamma_correction>`_.
+
+    Parameters
+    ----------
+    a : array-like
+        An array of values, typically the RGB array of values in
+        an image.
+    gamma : float
+        Gamma value to decode the image by.
+        Values > 1 will lighten an image.
+        Values < 1 will darken an image.
+    """
+    if verbose:
+        if gamma > 1:
+            print("Gamma Correction: 🌔 Lighten image")
+        elif gamma < 1:
+            print("Gamma Correction: 🌒 Darken image")
+        else:
+            print("Gamma Correction: 🌓 Gamma=1. No correction made.")
+            return a
+
+    # Gamma decoding formula
+    return np.power(a, 1 / gamma)
+
+
+def normalize(value, lower_limit, upper_limit, clip=True):
+    """
+    Normalize values between 0 and 1.
+
+    Normalize between a lower and upper limit. In other words, it
+    converts your number to a value in the range between 0 and 1.
+    Follows `normalization formula
+    <https://stats.stackexchange.com/a/70807/220885>`_
+
+    This is the same concept as `contrast or histogram stretching
+    <https://staff.fnwi.uva.nl/r.vandenboomgaard/IPCV20162017/LectureNotes/IP/PointOperators/ImageStretching.html>`_
+
+
+    .. code:: python
+
+        NormalizedValue = (OriginalValue-LowerLimit)/(UpperLimit-LowerLimit)
+
+    Parameters
+    ----------
+    value :
+        The original value. A single value, vector, or array.
+    upper_limit :
+        The upper limit.
+    lower_limit :
+        The lower limit.
+    clip : bool
+        - True: Clips values between 0 and 1 for RGB.
+        - False: Retain the numbers that extends outside 0-1 range.
+    Output:
+        Values normalized between the upper and lower limit.
+    """
+    norm = (value - lower_limit) / (upper_limit - lower_limit)
+    if clip:
+        norm = np.clip(norm, 0, 1)
+    return norm
+
+
+# ======================================================================
+# ======================================================================
+
+
+def TrueColor(C, gamma=2.2, pseudoGreen=True, night_IR=True, **kwargs):
+    """
+    True Color RGB:
+    (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_CIMSSRGB_v2.pdf>`__ for reference)
+
+    This is similar to the NaturalColor RGB, but uses a different gamma
+    correction and does not apply contrast stretching. I think these
+    images look a little "washed out" when compared to the NaturalColor
+    RGB. So, I would recommend using the NaturalColor RGB.
+
+    For more details on combing RGB and making the psedo green channel, refer to
+    `Bah et al. 2018 <https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2018EA000379>`_.
+
+    .. image:: /_static/TrueColor.png
+
+    .. image:: /_static/gamma_demo_TrueColor.png
+
+    .. image:: /_static/Color-IR_demo.png
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        A GOES ABI multichannel file opened with xarray.
+    gamma : float
+        Darken or lighten an image with `gamma correction
+        <https://en.wikipedia.org/wiki/Gamma_correction>`_.
+        Values > 1 will lighten an image.
+        Values < 1 will darken an image.
+    pseudoGreen : bool
+        True: returns the calculated "True" green color
+        False: returns the "veggie" channel
+    night_IR : bool
+        If True, use Clean IR (channel 13) as maximum RGB value overlay
+        so that cold clouds show up at night. (Be aware that some
+        daytime clouds might appear brighter).
+    \*\*kwargs :
+        Keyword arguments for ``rgb_as_dataset`` function.
+        - latlon : derive latitude and longitude of each pixel
+
+    """
+    # Load the three channels into appropriate R, G, and B variables
+    R, G, B = load_RGB_channels(C, (2, 3, 1))
+
+    # Apply range limits for each channel. RGB values must be between 0 and 1
+    R = np.clip(R, 0, 1)
+    G = np.clip(G, 0, 1)
+    B = np.clip(B, 0, 1)
+
+    # Apply a gamma correction to each R, G, B channel
+    R = gamma_correction(R, gamma)
+    G = gamma_correction(G, gamma)
+    B = gamma_correction(B, gamma)
+
+    if pseudoGreen:
+        # Calculate the "True" Green
+        G = 0.45 * R + 0.1 * G + 0.45 * B
+        G = np.clip(G, 0, 1)
+
+    if night_IR:
+        # Load the Clean IR channel
+        IR = C["CMI_C13"]
+        # Normalize between a range and clip
+        IR = normalize(IR, 90, 313, clip=True)
+        # Invert colors so cold clouds are white
+        IR = 1 - IR
+        # Lessen the brightness of the coldest clouds so they don't
+        # appear so bright when we overlay it on the true color image
+        IR = IR / 1.4
+        # RGB with IR as greyscale
+        RGB = np.dstack([np.maximum(R, IR), np.maximum(G, IR), np.maximum(B, IR)])
+    else:
+        RGB = np.dstack([R, G, B])
+
+    return rgb_as_dataset(C, RGB, "True Color", **kwargs)
+
+
+def NaturalColor(C, gamma=0.8, pseudoGreen=True, night_IR=False, **kwargs):
+    """
+    Natural Color RGB based on CIMSS method. Thanks Rick Kohrs!
+    (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_CIMSSRGB_v2.pdf>`__ for reference)
+
+    Check out Rick Kohrs `merged GOES images <https://www.ssec.wisc.edu/~rickk/local-noon.html>`_.
+
+    This NaturalColor RGB is *very* similar to the TrueColor RGB but
+    uses slightly different contrast stretches and ranges.
+
+    For more details on combing RGB and making the psedo green channel, refer to
+    `Bah et al. 2018 <https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2018EA000379>`_.
+
+    .. image:: /_static/NaturalColor.png
+
+    .. image:: /_static/gamma_demo_NaturalColor-PsuedoGreen.png
+
+    .. image:: /_static/gamma_demo_NaturalColor-VeggieGreen.png
+
+    .. image:: /_static/Color-IR_demo.png
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        A GOES ABI multichannel file opened ith xarray.
+    gamma : float
+        Darken or lighten an image with `gamma correction
+        <https://en.wikipedia.org/wiki/Gamma_correction>`_.
+        Values > 1 will lighten an image.
+        Values < 1 will darken an image.
+    night_IR : bool
+        If True, use Clean IR (channel 13) as maximum RGB value overlay
+        so that cold clouds show up at night. (Be aware that some
+        daytime clouds might appear brighter).
+    \*\*kwargs :
+        Keyword arguments for ``rgb_as_dataset`` function.
+        - latlon : derive latitude and longitude of each pixel
+    """
+
+    def breakpoint_stretch(C, breakpoint):
+        """
+        Contrast stretching by break point (number provided by Rick Kohrs)
+        """
+        lower = normalize(C, 0, 10)  # Low end
+        upper = normalize(C, 10, 255)  # High end
+
+        # Combine the two datasets
+        # This works because if upper=1 and lower==.7, then
+        # that means the upper value was out of range and the
+        # value for the lower pass was used instead.
+        combined = np.minimum(lower, upper)
+
+        return combined
+
+    # Load the three channels into appropriate R, G, and B variables
+    R, G, B = load_RGB_channels(C, (2, 3, 1))
+
+    # Apply range limits for each channel. RGB values must be between 0 and 1
+    R = np.clip(R, 0, 1)
+    G = np.clip(G, 0, 1)
+    B = np.clip(B, 0, 1)
+
+    if pseudoGreen:
+        # Derive pseudo Green channel
+        G = 0.45 * R + 0.1 * G + 0.45 * B
+        G = np.clip(G, 0, 1)
+
+    # Convert Albedo to Brightness, ranging from 0-255 K
+    # (numbers based on email from Rick Kohrs)
+    R = np.sqrt(R * 100) * 25.5
+    G = np.sqrt(G * 100) * 25.5
+    B = np.sqrt(B * 100) * 25.5
+
+    # Apply contrast stretching based on breakpoints
+    # (numbers based on email form Rick Kohrs)
+    R = breakpoint_stretch(R, 33)
+    G = breakpoint_stretch(G, 40)
+    B = breakpoint_stretch(B, 50)
+
+    if night_IR:
+        # Load the Clean IR channel
+        IR = C["CMI_C13"]
+        # Normalize between a range and clip
+        IR = normalize(IR, 90, 313, clip=True)
+        # Invert colors so cold clouds are white
+        IR = 1 - IR
+        # Lessen the brightness of the coldest clouds so they don't
+        # appear so bright when we overlay it on the true color image
+        IR = IR / 1.4
+        # Overlay IR channel, as greyscale image (use IR in R, G, and B)
+        RGB = np.dstack([np.maximum(R, IR), np.maximum(G, IR), np.maximum(B, IR)])
+    else:
+        RGB = np.dstack([R, G, B])
+
+    # Apply a gamma correction to the image
+    RGB = gamma_correction(RGB, gamma)
+
+    return rgb_as_dataset(C, RGB, "Natural Color", **kwargs)
+
+
+def FireTemperature(C, **kwargs):
+    """
+    Fire Temperature RGB:
+    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Fire_Temperature_RGB.pdf>`__ for reference)
+
+    .. image:: /_static/FireTemperature.png
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        A GOES ABI multichannel file opened with xarray.
+    \*\*kwargs :
+        Keyword arguments for ``rgb_as_dataset`` function.
+        - latlon : derive latitude and longitude of each pixel
+
+    """
+    # Load the three channels into appropriate R, G, and B variables
+    R, G, B = load_RGB_channels(C, (7, 6, 5))
+
+    # Normalize each channel by the appropriate range of values (clipping happens in function)
+    R = normalize(R, 273, 333)
+    G = normalize(G, 0, 1)
+    B = normalize(B, 0, 0.75)
+
+    # Apply the gamma correction to Red channel.
+    #   corrected_value = value^(1/gamma)
+    gamma = 0.4
+    R = gamma_correction(R, gamma)
+
+    # The final RGB array :)
+    RGB = np.dstack([R, G, B])
+
+    return rgb_as_dataset(C, RGB, "Fire Temperature", **kwargs)
+
+
+def AirMass(C, **kwargs):
+    """
+    Air Mass RGB:
+    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_AirMassRGB_final.pdf>`__ for reference)
+
+    .. image:: /_static/AirMass.png
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        A GOES ABI multichannel file opened with xarray.
+    \*\*kwargs :
+        Keyword arguments for ``rgb_as_dataset`` function.
+        - latlon : derive latitude and longitude of each pixel
+
+    """
+    # Load the three channels into appropriate R, G, and B variables
+    R = C["CMI_C08"].data - C["CMI_C10"].data
+    G = C["CMI_C12"].data - C["CMI_C13"].data
+    B = C["CMI_C08"].data - 273.15  # remember to convert to Celsius
+
+    # Normalize each channel by the appropriate range of values. e.g. R = (R-minimum)/(maximum-minimum)
+    R = normalize(R, -26.2, 0.6)
+    G = normalize(G, -42.2, 6.7)
+    B = normalize(B, -64.65, -29.25)
+
+    # Invert B
+    B = 1 - B
+
+    # The final RGB array :)
+    RGB = np.dstack([R, G, B])
+
+    return rgb_as_dataset(C, RGB, "Air Mass", **kwargs)
+
+
+def DayCloudPhase(C, **kwargs):
+    """
+    Day Cloud Phase Distinction RGB:
+    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Day_Cloud_Phase_Distinction.pdf>`__ for reference)
+
+    .. image:: /_static/DayCloudPhase.png
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        A GOES ABI multichannel file opened with xarray.
+    \*\*kwargs :
+        Keyword arguments for ``rgb_as_dataset`` function.
+        - latlon : derive latitude and longitude of each pixel
+
+    """
+    # Load the three channels into appropriate R, G, and B variables
+    R, G, B = load_RGB_channels(C, (13, 2, 5))
+
+    # Normalize each channel by the appropriate range of values. (Clipping happens inside function)
+    R = normalize(R, -53.5, 7.5)
+    G = normalize(G, 0, 0.78)
+    B = normalize(B, 0.01, 0.59)
+
+    # Invert R
+    R = 1 - R
+
+    # The final RGB array :)
+    RGB = np.dstack([R, G, B])
+
+    return rgb_as_dataset(C, RGB, "Day Cloud Phase", **kwargs)
+
+
+def DayConvection(C, **kwargs):
+    """
+    Day Convection RGB:
+    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DayConvectionRGB_final.pdf>`__ for reference)
+
+    .. image:: /_static/DayConvection.png
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        A GOES ABI multichannel file opened with xarray.
+    \*\*kwargs :
+        Keyword arguments for ``rgb_as_dataset`` function.
+        - latlon : derive latitude and longitude of each pixel
+
+    """
+    # Load the three channels into appropriate R, G, and B variables
+    # NOTE: Each R, G, B is a channel difference.
+    R = C["CMI_C08"].data - C["CMI_C10"].data
+    G = C["CMI_C07"].data - C["CMI_C13"].data
+    B = C["CMI_C05"].data - C["CMI_C02"].data
+
+    # Normalize each channel by the appropriate range of values.
+    R = normalize(R, -35, 5)
+    G = normalize(G, -5, 60)
+    B = normalize(B, -0.75, 0.25)
+
+    # The final RGB array :)
+    RGB = np.dstack([R, G, B])
+
+    return rgb_as_dataset(C, RGB, "Day Convection", **kwargs)
+
+
+def DayCloudConvection(C, **kwargs):
+    """
+    Day Cloud Convection RGB:
+    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_DayCloudConvectionRGB_final.pdf>`__ for reference)
+
+    .. image:: /_static/DayCloudConvection.png
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        A GOES ABI multichannel file opened with xarray.
+    \*\*kwargs :
+        Keyword arguments for ``rgb_as_dataset`` function.
+        - latlon : derive latitude and longitude of each pixel
+
+    """
+    # Load the three channels into appropriate R, G, and B variables
+    R, G, B = load_RGB_channels(C, (2, 2, 13))
+
+    # Normalize each channel by the appropriate range of values.
+    R = normalize(R, 0, 1)
+    G = normalize(G, 0, 1)
+    B = normalize(B, -70.15, 49.85)
+
+    # Invert B
+    B = 1 - B
+
+    # Apply the gamma correction to Red channel.
+    #   corrected_value = value^(1/gamma)
+    gamma = 1.7
+    R = gamma_correction(R, gamma)
+    G = gamma_correction(G, gamma)
+
+    # The final RGB array :)
+    RGB = np.dstack([R, G, B])
+
+    return rgb_as_dataset(C, RGB, "Day Cloud Convection", **kwargs)
+
+
+def DayLandCloud(C, **kwargs):
+    """
+    Day Land Cloud Fire RGB:
+    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_daylandcloudRGB_final.pdf>`__ for reference)
+
+    .. image:: /_static/DayLandCloud.png
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        A GOES ABI multichannel file opened with xarray.
+    \*\*kwargs :
+        Keyword arguments for ``rgb_as_dataset`` function.
+        - latlon : derive latitude and longitude of each pixel
+
+    """
+    # Load the three channels into appropriate R, G, and B variables
+    R, G, B = load_RGB_channels(C, (5, 3, 2))
+
+    # Normalize each channel by the appropriate range of values  e.g. R = (R-minimum)/(maximum-minimum)
+    R = normalize(R, 0, 0.975)
+    G = normalize(G, 0, 1.086)
+    B = normalize(B, 0, 1)
+
+    # The final RGB array :)
+    RGB = np.dstack([R, G, B])
+
+    return rgb_as_dataset(C, RGB, "Day Land Cloud", **kwargs)
+
+
+def DayLandCloudFire(C, **kwargs):
+    """
+    Day Land Cloud Fire RGB:
+    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DayLandCloudFireRGB_final.pdf>`__ for reference)
+
+    .. image:: /_static/DayLandCloudFire.png
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        A GOES ABI multichannel file opened with xarray.
+    \*\*kwargs :
+        Keyword arguments for ``rgb_as_dataset`` function.
+        - latlon : derive latitude and longitude of each pixel
+
+    """
+    # Load the three channels into appropriate R, G, and B variables
+    R, G, B = load_RGB_channels(C, (6, 3, 2))
+
+    # Normalize each channel by the appropriate range of values  e.g. R = (R-minimum)/(maximum-minimum)
+    R = normalize(R, 0, 1)
+    G = normalize(G, 0, 1)
+    B = normalize(B, 0, 1)
+
+    # The final RGB array :)
+    RGB = np.dstack([R, G, B])
+
+    return rgb_as_dataset(C, RGB, "Day Land Cloud Fire", **kwargs)
+
+
+def WaterVapor(C, **kwargs):
+    """
+    Simple Water Vapor RGB:
+    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Simple_Water_Vapor_RGB.pdf>`__ for reference)
+
+    .. image:: /_static/WaterVapor.png
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        A GOES ABI multichannel file opened with xarray.
+    \*\*kwargs :
+        Keyword arguments for ``rgb_as_dataset`` function.
+        - latlon : derive latitude and longitude of each pixel
+
+    """
+    # Load the three channels into appropriate R, G, and B variables.
+    R, G, B = load_RGB_channels(C, (13, 8, 10))
+
+    # Normalize each channel by the appropriate range of values. e.g. R = (R-minimum)/(maximum-minimum)
+    R = normalize(R, -70.86, 5.81)
+    G = normalize(G, -58.49, -30.48)
+    B = normalize(B, -28.03, -12.12)
+
+    # Invert the colors
+    R = 1 - R
+    G = 1 - G
+    B = 1 - B
+
+    # The final RGB array :)
+    RGB = np.dstack([R, G, B])
+
+    return rgb_as_dataset(C, RGB, "Water Vapor", **kwargs)
+
+
+def DifferentialWaterVapor(C, **kwargs):
+    """
+    Differential Water Vapor RGB:
+    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DifferentialWaterVaporRGB_final.pdf>`__ for reference)
+
+    .. image:: /_static/DifferentialWaterVapor.png
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        A GOES ABI multichannel file opened with xarray.
+    \*\*kwargs :
+        Keyword arguments for ``rgb_as_dataset`` function.
+        - latlon : derive latitude and longitude of each pixel
+
+    """
+    # Load the three channels into appropriate R, G, and B variables.
+    R = C["CMI_C10"].data - C["CMI_C08"].data
+    G = C["CMI_C10"].data - 273.15
+    B = C["CMI_C08"].data - 273.15
+
+    # Normalize each channel by the appropriate range of values. e.g. R = (R-minimum)/(maximum-minimum)
+    R = normalize(R, -3, 30)
+    G = normalize(G, -60, 5)
+    B = normalize(B, -64.65, -29.25)
+
+    # Gamma correction
+    R = gamma_correction(R, 0.2587)
+    G = gamma_correction(G, 0.4)
+    B = gamma_correction(B, 0.4)
+
+    # Invert the colors
+    R = 1 - R
+    G = 1 - G
+    B = 1 - B
+
+    # The final RGB array :)
+    RGB = np.dstack([R, G, B])
+
+    return rgb_as_dataset(C, RGB, "Differenctial Water Vapor", **kwargs)
+
+
+def DaySnowFog(C, **kwargs):
+    """
+    Day Snow-Fog RGB:
+    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_DaySnowFog.pdf>`__ for reference)
+
+    .. image:: /_static/DaySnowFog.png
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        A GOES ABI multichannel file opened with xarray.
+    \*\*kwargs :
+        Keyword arguments for ``rgb_as_dataset`` function.
+        - latlon : derive latitude and longitude of each pixel
+
+    """
+    # Load the three channels into appropriate R, G, and B variables
+    R = C["CMI_C03"].data
+    G = C["CMI_C05"].data
+    B = C["CMI_C07"].data - C["CMI_C13"].data
+
+    # Normalize values
+    R = normalize(R, 0, 1)
+    G = normalize(G, 0, 0.7)
+    B = normalize(B, 0, 30)
+
+    # Apply a gamma correction to the image
+    gamma = 1.7
+    R = gamma_correction(R, gamma)
+    G = gamma_correction(G, gamma)
+    B = gamma_correction(B, gamma)
+
+    # The final RGB array :)
+    RGB = np.dstack([R, G, B])
+
+    return rgb_as_dataset(C, RGB, "Day Snow Fog", **kwargs)
+
+
+def NighttimeMicrophysics(C, **kwargs):
+    """
+    Nighttime Microphysics RGB:
+    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_NtMicroRGB_final.pdf>`__ for reference)
+
+    .. image:: /_static/NighttimeMicrophysics.png
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        A GOES ABI multichannel file opened with xarray.
+    \*\*kwargs :
+        Keyword arguments for ``rgb_as_dataset`` function.
+        - latlon : derive latitude and longitude of each pixel
+
+    """
+    # Load the three channels into appropriate R, G, and B variables
+    R = C["CMI_C15"].data - C["CMI_C13"].data
+    G = C["CMI_C13"].data - C["CMI_C07"].data
+    B = C["CMI_C13"].data - 273.15
+
+    # Normalize values
+    R = normalize(R, -6.7, 2.6)
+    G = normalize(G, -3.1, 5.2)
+    B = normalize(B, -29.6, 19.5)
+
+    # The final RGB array :)
+    RGB = np.dstack([R, G, B])
+
+    return rgb_as_dataset(C, RGB, "Nighttime Microphysics", **kwargs)
+
+
+def Dust(C, **kwargs):
+    """
+    SulfurDioxide RGB:
+    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Dust_RGB_Quick_Guide.pdf>`__ for reference)
+
+    .. image:: /_static/Dust.png
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        A GOES ABI multichannel file opened with xarray.
+    \*\*kwargs :
+        Keyword arguments for ``rgb_as_dataset`` function.
+        - latlon : derive latitude and longitude of each pixel
+
+    """
+    # Load the three channels into appropriate R, G, and B variables
+    R = C["CMI_C15"].data - C["CMI_C13"].data
+    G = C["CMI_C14"].data - C["CMI_C11"].data
+    B = C["CMI_C13"].data - 273.15
+
+    # Normalize values
+    R = normalize(R, -6.7, 2.6)
+    G = normalize(G, -0.5, 20)
+    B = normalize(B, -11.95, 15.55)
+
+    # Apply a gamma correction to the image
+    gamma = 2.5
+    G = gamma_correction(G, gamma)
+
+    # The final RGB array :)
+    RGB = np.dstack([R, G, B])
+
+    return rgb_as_dataset(C, RGB, "Dust", **kwargs)
+
+
+def SulfurDioxide(C, **kwargs):
+    """
+    SulfurDioxide RGB:
+    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Quick_Guide_SO2_RGB.pdf>`__ for reference)
+
+    .. image:: /_static/SulfurDioxide.png
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        A GOES ABI multichannel file opened with xarray.
+    \*\*kwargs :
+        Keyword arguments for ``rgb_as_dataset`` function.
+        - latlon : derive latitude and longitude of each pixel
+
+    """
+    # Load the three channels into appropriate R, G, and B variables
+    R = C["CMI_C09"].data - C["CMI_C10"].data
+    G = C["CMI_C13"].data - C["CMI_C11"].data
+    B = C["CMI_C07"].data - 273.15
+
+    # Normalize values
+    R = normalize(R, -4, 2)
+    G = normalize(G, -4, 5)
+    B = normalize(B, -30.1, 29.8)
+
+    # The final RGB array :)
+    RGB = np.dstack([R, G, B])
+
+    return rgb_as_dataset(C, RGB, "Sulfur Dioxide", **kwargs)
+
+
+def Ash(C, **kwargs):
+    """
+    Ash RGB:
+    (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/GOES_Ash_RGB.pdf>`__ for reference)
+
+    .. image:: /_static/Ash.png
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        A GOES ABI multichannel file opened with xarray.
+    \*\*kwargs :
+        Keyword arguments for ``rgb_as_dataset`` function.
+        - latlon : derive latitude and longitude of each pixel
+
+    """
+    # Load the three channels into appropriate R, G, and B variables
+    R = C["CMI_C15"].data - C["CMI_C13"].data
+    G = C["CMI_C14"].data - C["CMI_C11"].data
+    B = C["CMI_C13"].data - 273.15
+
+    # Normalize values
+    R = normalize(R, -6.7, 2.6)
+    G = normalize(G, -6, 6.3)
+    B = normalize(B, -29.55, 29.25)
+
+    # The final RGB array :)
+    RGB = np.dstack([R, G, B])
+
+    return rgb_as_dataset(C, RGB, "Ash", **kwargs)
+
+
+def SplitWindowDifference(C, **kwargs):
+    """
+    Split Window Difference RGB (greyscale):
+    (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_SplitWindowDifference.pdf>`__ for reference)
+
+    .. image:: /_static/SplitWindowDifference.png
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        A GOES ABI multichannel file opened with xarray.
+    \*\*kwargs :
+        Keyword arguments for ``rgb_as_dataset`` function.
+        - latlon : derive latitude and longitude of each pixel
+
+    """
+    # Load the three channels into appropriate R, G, and B variables
+    data = C["CMI_C15"].data - C["CMI_C13"].data
+
+    # Normalize values
+    data = normalize(data, -10, 10)
+
+    # The final RGB array :)
+    RGB = np.dstack([data, data, data])
+
+    return rgb_as_dataset(C, RGB, "Split Window Difference", **kwargs)
+
+
+def NightFogDifference(C, **kwargs):
+    """
+    Night Fog Difference RGB (greyscale):
+    (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_NightFogBTD.pdf>`__ for reference)
+
+    .. image:: /_static/NightFogDifference.png
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        A GOES ABI multichannel file opened with xarray.
+    \*\*kwargs :
+        Keyword arguments for ``rgb_as_dataset`` function.
+        - latlon : derive latitude and longitude of each pixel
+
+    """
+    # Load the three channels into appropriate R, G, and B variables
+    data = C["CMI_C13"].data - C["CMI_C07"].data
+
+    # Normalize values
+    data = normalize(data, -90, 15)
+
+    # Invert data
+    data = 1 - data
+
+    # The final RGB array :)
+    RGB = np.dstack([data, data, data])
+
+    return rgb_as_dataset(C, RGB, "Night Fog Difference", **kwargs)
+
+
+def RocketPlume(C, night=False, **kwargs):
+    """
+    Rocket Plume RGB
+
+    For identifying rocket launches.
+
+    See `this blog <https://cimss.ssec.wisc.edu/satellite-blog/archives/41335>`__ and
+    the `Quick Guide <https://cimss.ssec.wisc.edu/satellite-blog/images/2021/06/QuickGuide_Template_GOESRBanner_Rocket_Plume.pdf>`__
+    for reference
+
+    .. image:: /_static/RocketPlume.png
+
+    Parameters
+    ----------
+    C : xarray.Dataset
+        A GOES ABI multichannel file opened with xarray.
+    night : bool
+        If the area is in night, turn this on to use a different channel
+        than the daytime application.
+    \*\*kwargs :
+        Keyword arguments for ``rgb_as_dataset`` function.
+        - latlon : derive latitude and longitude of each pixel
+
+    """
+    # Load the three channels into appropriate R, G, and B variables
+    R = C["CMI_C07"].data
+    G = C["CMI_C08"].data
+    if not night:
+        B = C["CMI_C02"].data
+    else:
+        B = C["CMI_C05"].data
+
+    # Normalize values
+    R = normalize(R, 273, 338)
+    G = normalize(G, 233, 253)
+    B = normalize(B, 0, 0.80)
+
+    # The final RGB array :)
+    RGB = np.dstack([R, G, B])
+
+    return rgb_as_dataset(C, RGB, "RocketPlume", **kwargs)
+
+
+#######################
+# 🚧 Construction Zone
+#######################
+def NormalizedBurnRatio(C, **kwargs):
+    """
+    Normalized Burn Ratio
+
+    **THIS FUNCTION IS NOT FULLY DEVELOPED. Need more info.**
+
+    NBR= (0.86 µm – 2.2 µm)/(0.86 um + 2.2 um)
+
+
+    https://ntrs.nasa.gov/citations/20190030825
+
+    Parameters
+    ----------
+
+    """
+    # Load the three channels into appropriate R, G, and B variables
+    C3 = C["CMI_C03"].data
+    C6 = C["CMI_C06"].data
+    data = (C3 - C6) / (C3 + C6)
+
+    # Invert data
+    # data = 1-data
+
+    # The final RGB array :)
+    RGB = np.dstack([data, data, data])
+
+    return rgb_as_dataset(C, RGB, "Normalized Burn Ratio", **kwargs)
+
+
+if __name__ == "__main__":
+    # Create images of each for Docs
+    print("nothing here for now")
```

### Comparing `goes2go-2022.8.26/goes2go/tools.py` & `goes2go-2023.4.0/goes2go/tools.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-## Brian Blaylock
-## September 22, 2020
-
-"""
-===========
-Other Tools
-===========
-Other tools for handeling NOAA GOES data files.
-"""
-
-import numpy as np
-import cartopy.crs as ccrs
-import warnings
-
-try:
-    import metpy  # Need accessors to get projection info.
-except:
-    # Not sure why sphinx can't import metpy??
-    warnings.warn("Metpy not imported.")
-from shapely.geometry import Point, Polygon
-
-
-def field_of_view(G, resolution=60, reduce_abi_fov=0.06):
-    """
-    Create a field-of-view polygon for the GOES data.
-
-    Based on information from the `GOES-R Series Data Book
-    <https://www.goes-r.gov/downloads/resources/documents/GOES-RSeriesDataBook.pdf>`_.
-
-    GLM lense field of view is 16 degree, or +/- 8 degrees (see page 225)
-    ABI full-disk field of view if 17.4 degrees (see page 48)
-
-    To plot the field of view on the cartopy axes, do the following:
-
-    .. code:: python
-
-        FOV, geo = field_of_view(G)
-        ax = plt.subplot(projection=geo)
-        ax.add_geometries([FOV], crs=geo)
-
-    Parameters
-    ----------
-    G : xarray.Dataset
-        The GOES NetCDF file opened with xarray. A file is required
-        because we get info from the file to define the projection.
-    resolution : int
-        Resolution of polygon shapes
-    reduce_abi_fov : float or int
-        Since the globe isn't a perfect ellipse, reduce the field of
-        view just slightly to get all the points to be on the projection
-        plane. If this number is less than the default, the polygon
-        will not be calculated correctly because edge points will lie
-        off the projection globe.
-    """
-    warnings.warn(
-        "DEPRECIATION. Use the FOV accessor instead `G.FOV.full_disk` or `G.FOV.domain`"
-    )
-    if G.title.startswith("ABI"):
-        globe_kwargs = dict(
-            semimajor_axis=G.goes_imager_projection.semi_major_axis,
-            semiminor_axis=G.goes_imager_projection.semi_minor_axis,
-            inverse_flattening=G.goes_imager_projection.inverse_flattening,
-        )
-        sat_height = G.goes_imager_projection.perspective_point_height
-        nadir_lon = G.geospatial_lat_lon_extent.geospatial_lon_nadir
-        nadir_lat = G.geospatial_lat_lon_extent.geospatial_lat_nadir
-        # Field of view in degrees
-        FOV = 17.4
-        FOV -= reduce_abi_fov  # little less to account for imprecise ellipsoid
-    elif G.title.startswith("GLM"):
-        globe_kwargs = dict(
-            semimajor_axis=G.goes_lat_lon_projection.semi_major_axis,
-            semiminor_axis=G.goes_lat_lon_projection.semi_minor_axis,
-            inverse_flattening=G.goes_lat_lon_projection.inverse_flattening,
-        )
-        sat_height = G.nominal_satellite_height.item() * 1000
-        nadir_lon = G.lon_field_of_view.item()
-        nadir_lat = G.lat_field_of_view.item()
-        FOV = 8 * 2
-        FOV += 0.15  # Little offset to better match boundary from Rudlosky et al. 2018
-
-    # Create a cartopy coordinate reference system for the data
-
-    # These numbers are from the `goes_imager_projection` variable
-    globe = ccrs.Globe(ellipse=None, **globe_kwargs)
-
-    crs = ccrs.Geostationary(
-        central_longitude=nadir_lon,
-        satellite_height=sat_height,
-        globe=globe,
-        sweep_axis="x",
-    )
-
-    # Create polygon of the field of view. This polygon is in
-    # the geostationary crs projection units, and is in meters.
-    # The central point is at 0,0 (not the nadir position), because
-    # we are working in the geostationary projection coordinates
-    # and the center point is 0,0 meters.
-    FOV_radius = np.radians(FOV / 2) * sat_height
-    FOV_poly = Point(0, 0).buffer(FOV_radius, resolution=resolution)
-
-    ## GLM is a bit funny. I haven't found this in the documentation
-    ## anywhere, yet, but the GLM field-of-view is not exactly
-    ## the full circle, there is a square area cut out of it.
-    ## The square FOV is ~ 15 degrees
-    if G.title.startswith("GLM"):
-        FOV_square = 15 / 2
-        # FOV_square += .1 # offset to match Rudlosky et al. 2018
-        FOV_radius = np.radians(FOV_square) * sat_height
-        # Create a square with many points clockwise, starting in bottom left corner
-        side1x, side1y = (
-            np.ones(resolution) * -FOV_radius,
-            np.linspace(-FOV_radius, FOV_radius, resolution),
-        )
-        side2x, side2y = (
-            np.linspace(-FOV_radius, FOV_radius, resolution),
-            np.ones(resolution) * FOV_radius,
-        )
-        side3x, side3y = (
-            np.ones(resolution) * FOV_radius,
-            np.linspace(FOV_radius, -FOV_radius, resolution),
-        )
-        side4x, side4y = (
-            np.linspace(FOV_radius, -FOV_radius, resolution),
-            np.ones(resolution) * -FOV_radius,
-        )
-        x = np.hstack([side1x, side2x, side3x, side4x])
-        y = np.hstack([side1y, side2y, side3y, side4y])
-        square_FOV = Polygon(zip(x, y))
-        FOV_poly = FOV_poly.intersection(square_FOV)
-
-        return FOV_poly, crs
-
-    if G.title.startswith("ABI"):
-        # We have the global field of view
-        # now we need the domain field of view
-        dom_border = np.array(
-            [(i, G.y.data[0]) for i in G.x.data]
-            + [(G.x.data[-1], i) for i in G.y.data]
-            + [(i, G.y.data[-1]) for i in G.x.data[::-1]]
-            + [(G.x.data[0], i) for i in G.y.data[::-1]]
-        )
-        FOV_dom = Polygon(dom_border * sat_height)
-        FOV_dom = FOV_dom.intersection(FOV_poly)
-        return FOV_poly, FOV_dom, crs
-
-
-def abi_crs(G, reference_variable="CMI_C01"):
-    """
-    Get coordinate reference system for the Advanced Baseline Imager (ABI).
-
-    Parameters
-    ----------
-    G : xarray.Dataset
-        An xarray.Dataset to derive the coordinate reference system.
-    reference_variable : str
-        A variable in the xarray.Dataset to use to parse projection from.
-
-    Returns
-    -------
-    Three objects are returned
-        1. cartopy coordinate reference system
-        2. data projection coordinates in x direction
-        3. data projection coordinates in y direction
-
-    """
-    # We'll use the `CMI_C01` variable as a 'hook' to get the CF metadata.
-    dat = G.metpy.parse_cf(reference_variable)
-
-    crs = dat.metpy.cartopy_crs
-
-    # We also need the x (north/south) and y (east/west) axis sweep of the ABI data
-    x, y = (dat.x, dat.y)
-
-    return crs, x, y
-
-
-def glm_crs(G, reference_variable="flash_lat"):
-    """Not too useful, because it's just lat/lon coordinates"""
-    dat = G.metpy.parse_cf("flash_lat")
-    crs = dat.metpy.cartopy_crs
-    return crs
+## Brian Blaylock
+## September 22, 2020
+
+"""
+===========
+Other Tools
+===========
+Other tools for handeling NOAA GOES data files.
+"""
+
+import numpy as np
+import cartopy.crs as ccrs
+import warnings
+
+try:
+    import metpy  # Need accessors to get projection info.
+except:
+    # Not sure why sphinx can't import metpy??
+    warnings.warn("Metpy not imported.")
+from shapely.geometry import Point, Polygon
+
+
+def field_of_view(G, resolution=60, reduce_abi_fov=0.06):
+    """
+    Create a field-of-view polygon for the GOES data.
+
+    Based on information from the `GOES-R Series Data Book
+    <https://www.goes-r.gov/downloads/resources/documents/GOES-RSeriesDataBook.pdf>`_.
+
+    GLM lense field of view is 16 degree, or +/- 8 degrees (see page 225)
+    ABI full-disk field of view if 17.4 degrees (see page 48)
+
+    To plot the field of view on the cartopy axes, do the following:
+
+    .. code:: python
+
+        FOV, geo = field_of_view(G)
+        ax = plt.subplot(projection=geo)
+        ax.add_geometries([FOV], crs=geo)
+
+    Parameters
+    ----------
+    G : xarray.Dataset
+        The GOES NetCDF file opened with xarray. A file is required
+        because we get info from the file to define the projection.
+    resolution : int
+        Resolution of polygon shapes
+    reduce_abi_fov : float or int
+        Since the globe isn't a perfect ellipse, reduce the field of
+        view just slightly to get all the points to be on the projection
+        plane. If this number is less than the default, the polygon
+        will not be calculated correctly because edge points will lie
+        off the projection globe.
+    """
+    warnings.warn(
+        "DEPRECIATION. Use the FOV accessor instead `G.FOV.full_disk` or `G.FOV.domain`"
+    )
+    if G.title.startswith("ABI"):
+        globe_kwargs = dict(
+            semimajor_axis=G.goes_imager_projection.semi_major_axis,
+            semiminor_axis=G.goes_imager_projection.semi_minor_axis,
+            inverse_flattening=G.goes_imager_projection.inverse_flattening,
+        )
+        sat_height = G.goes_imager_projection.perspective_point_height
+        nadir_lon = G.geospatial_lat_lon_extent.geospatial_lon_nadir
+        nadir_lat = G.geospatial_lat_lon_extent.geospatial_lat_nadir
+        # Field of view in degrees
+        FOV = 17.4
+        FOV -= reduce_abi_fov  # little less to account for imprecise ellipsoid
+    elif G.title.startswith("GLM"):
+        globe_kwargs = dict(
+            semimajor_axis=G.goes_lat_lon_projection.semi_major_axis,
+            semiminor_axis=G.goes_lat_lon_projection.semi_minor_axis,
+            inverse_flattening=G.goes_lat_lon_projection.inverse_flattening,
+        )
+        sat_height = G.nominal_satellite_height.item() * 1000
+        nadir_lon = G.lon_field_of_view.item()
+        nadir_lat = G.lat_field_of_view.item()
+        FOV = 8 * 2
+        FOV += 0.15  # Little offset to better match boundary from Rudlosky et al. 2018
+
+    # Create a cartopy coordinate reference system for the data
+
+    # These numbers are from the `goes_imager_projection` variable
+    globe = ccrs.Globe(ellipse=None, **globe_kwargs)
+
+    crs = ccrs.Geostationary(
+        central_longitude=nadir_lon,
+        satellite_height=sat_height,
+        globe=globe,
+        sweep_axis="x",
+    )
+
+    # Create polygon of the field of view. This polygon is in
+    # the geostationary crs projection units, and is in meters.
+    # The central point is at 0,0 (not the nadir position), because
+    # we are working in the geostationary projection coordinates
+    # and the center point is 0,0 meters.
+    FOV_radius = np.radians(FOV / 2) * sat_height
+    FOV_poly = Point(0, 0).buffer(FOV_radius, resolution=resolution)
+
+    ## GLM is a bit funny. I haven't found this in the documentation
+    ## anywhere, yet, but the GLM field-of-view is not exactly
+    ## the full circle, there is a square area cut out of it.
+    ## The square FOV is ~ 15 degrees
+    if G.title.startswith("GLM"):
+        FOV_square = 15 / 2
+        # FOV_square += .1 # offset to match Rudlosky et al. 2018
+        FOV_radius = np.radians(FOV_square) * sat_height
+        # Create a square with many points clockwise, starting in bottom left corner
+        side1x, side1y = (
+            np.ones(resolution) * -FOV_radius,
+            np.linspace(-FOV_radius, FOV_radius, resolution),
+        )
+        side2x, side2y = (
+            np.linspace(-FOV_radius, FOV_radius, resolution),
+            np.ones(resolution) * FOV_radius,
+        )
+        side3x, side3y = (
+            np.ones(resolution) * FOV_radius,
+            np.linspace(FOV_radius, -FOV_radius, resolution),
+        )
+        side4x, side4y = (
+            np.linspace(FOV_radius, -FOV_radius, resolution),
+            np.ones(resolution) * -FOV_radius,
+        )
+        x = np.hstack([side1x, side2x, side3x, side4x])
+        y = np.hstack([side1y, side2y, side3y, side4y])
+        square_FOV = Polygon(zip(x, y))
+        FOV_poly = FOV_poly.intersection(square_FOV)
+
+        return FOV_poly, crs
+
+    if G.title.startswith("ABI"):
+        # We have the global field of view
+        # now we need the domain field of view
+        dom_border = np.array(
+            [(i, G.y.data[0]) for i in G.x.data]
+            + [(G.x.data[-1], i) for i in G.y.data]
+            + [(i, G.y.data[-1]) for i in G.x.data[::-1]]
+            + [(G.x.data[0], i) for i in G.y.data[::-1]]
+        )
+        FOV_dom = Polygon(dom_border * sat_height)
+        FOV_dom = FOV_dom.intersection(FOV_poly)
+        return FOV_poly, FOV_dom, crs
+
+
+def abi_crs(G, reference_variable="CMI_C01"):
+    """
+    Get coordinate reference system for the Advanced Baseline Imager (ABI).
+
+    Parameters
+    ----------
+    G : xarray.Dataset
+        An xarray.Dataset to derive the coordinate reference system.
+    reference_variable : str
+        A variable in the xarray.Dataset to use to parse projection from.
+
+    Returns
+    -------
+    Three objects are returned
+        1. cartopy coordinate reference system
+        2. data projection coordinates in x direction
+        3. data projection coordinates in y direction
+
+    """
+    # We'll use the `CMI_C01` variable as a 'hook' to get the CF metadata.
+    dat = G.metpy.parse_cf(reference_variable)
+
+    crs = dat.metpy.cartopy_crs
+
+    # We also need the x (north/south) and y (east/west) axis sweep of the ABI data
+    x, y = (dat.x, dat.y)
+
+    return crs, x, y
+
+
+def glm_crs(G, reference_variable="flash_lat"):
+    """Not too useful, because it's just lat/lon coordinates"""
+    dat = G.metpy.parse_cf("flash_lat")
+    crs = dat.metpy.cartopy_crs
+    return crs
```

### Comparing `goes2go-2022.8.26/tests/test_data.py` & `goes2go-2023.4.0/tests/test_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,95 @@
-from datetime import datetime, timedelta
-import unittest
-from unittest.mock import patch
-from venv import create
-
-import pandas as pd
-
-from goes2go.data import goes_nearesttime
-
-
-def _test_row(
-    satellite="G17",
-    product="ABI-L1b-RadC",
-    start=datetime(2021, 1, 1, 17, 0, 0),
-    band=1,
-    mode=6,
-):
-
-    return {
-        "file": "fname",
-        "product_mode": "pmode",
-        "satellite": satellite,
-        "start": start,
-        "end": start + timedelta(seconds=60),
-        "creation": start + timedelta(seconds=90),
-        "product": product,
-        "mode": mode,
-        "band": band,
-    }
-
-
-class TestData(unittest.TestCase):
-    def test_goes_nearesttime_singleband(self):
-
-        t = datetime(2021, 1, 1, 17, 0, 0)
-
-        with patch("goes2go.data._goes_file_df") as _goes_file_df_patched:
-
-            test_df = pd.DataFrame([_test_row(start=t)])
-            _goes_file_df_patched.return_value = test_df
-
-            res = goes_nearesttime(
-                t,
-                satellite=17,
-                product="ABI-L1b-Rad",
-                return_as="filelist",
-                bands=[1],
-                download=False,
-                domain="C",
-            )
-            self.assertEqual(len(res), 1)
-
-    def test_goes_nearesttime_multiband(self):
-
-        t = datetime(2021, 1, 1, 17, 0, 0)
-
-        with patch("goes2go.data._goes_file_df") as _goes_file_df_patched:
-
-            # test case where both have the same time, 2 res expected
-            test_df = pd.DataFrame(
-                [
-                    _test_row(start=t, band=1),
-                    _test_row(start=t, band=2),
-                ]
-            )
-            _goes_file_df_patched.return_value = test_df
-            res = goes_nearesttime(
-                t,
-                satellite=17,
-                product="ABI-L1b-Rad",
-                return_as="filelist",
-                bands=[1, 2],
-                download=False,
-                domain="C",
-            )
-            self.assertEqual(len(res), 2)
-
-            # test case where both have different time, 1 res expected
-            test_df = pd.DataFrame(
-                [
-                    _test_row(start=t, band=1),
-                    _test_row(start=t + timedelta(days=1), band=2),
-                ]
-            )
-            _goes_file_df_patched.return_value = test_df
-            res = goes_nearesttime(
-                t,
-                satellite=17,
-                product="ABI-L1b-Rad",
-                return_as="filelist",
-                bands=[1, 2],
-                download=False,
-                domain="C",
-            )
-            self.assertEqual(len(res), 1)
-            self.assertEqual(res.start[0], t)
-
-
-if __name__ == "__main__":
-    unittest.main()
+from datetime import datetime, timedelta
+import unittest
+from unittest.mock import patch
+from venv import create
+
+import pandas as pd
+
+from goes2go.data import goes_nearesttime
+
+
+def _test_row(
+    satellite="G17",
+    product="ABI-L1b-RadC",
+    start=datetime(2021, 1, 1, 17, 0, 0),
+    band=1,
+    mode=6,
+):
+    return {
+        "file": "fname",
+        "product_mode": "pmode",
+        "satellite": satellite,
+        "start": start,
+        "end": start + timedelta(seconds=60),
+        "creation": start + timedelta(seconds=90),
+        "product": product,
+        "mode": mode,
+        "band": band,
+    }
+
+
+class TestData(unittest.TestCase):
+    def test_goes_nearesttime_singleband(self):
+        t = datetime(2021, 1, 1, 17, 0, 0)
+
+        with patch("goes2go.data._goes_file_df") as _goes_file_df_patched:
+            test_df = pd.DataFrame([_test_row(start=t)])
+            _goes_file_df_patched.return_value = test_df
+
+            res = goes_nearesttime(
+                t,
+                satellite=17,
+                product="ABI-L1b-Rad",
+                return_as="filelist",
+                bands=[1],
+                download=False,
+                domain="C",
+            )
+            self.assertEqual(len(res), 1)
+
+    def test_goes_nearesttime_multiband(self):
+        t = datetime(2021, 1, 1, 17, 0, 0)
+
+        with patch("goes2go.data._goes_file_df") as _goes_file_df_patched:
+            # test case where both have the same time, 2 res expected
+            test_df = pd.DataFrame(
+                [
+                    _test_row(start=t, band=1),
+                    _test_row(start=t, band=2),
+                ]
+            )
+            _goes_file_df_patched.return_value = test_df
+            res = goes_nearesttime(
+                t,
+                satellite=17,
+                product="ABI-L1b-Rad",
+                return_as="filelist",
+                bands=[1, 2],
+                download=False,
+                domain="C",
+            )
+            self.assertEqual(len(res), 2)
+
+            # test case where both have different time, 1 res expected
+            test_df = pd.DataFrame(
+                [
+                    _test_row(start=t, band=1),
+                    _test_row(start=t + timedelta(days=1), band=2),
+                ]
+            )
+            _goes_file_df_patched.return_value = test_df
+            res = goes_nearesttime(
+                t,
+                satellite=17,
+                product="ABI-L1b-Rad",
+                return_as="filelist",
+                bands=[1, 2],
+                download=False,
+                domain="C",
+            )
+            self.assertEqual(len(res), 1)
+            self.assertEqual(res.start[0], t)
+
+
+if __name__ == "__main__":
+    unittest.main()
```


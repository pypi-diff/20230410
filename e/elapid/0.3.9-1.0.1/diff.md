# Comparing `tmp/elapid-0.3.9.tar.gz` & `tmp/elapid-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elapid-0.3.9.tar", last modified: Fri Sep  9 16:38:01 2022, max compression
+gzip compressed data, was "elapid-1.0.1.tar", last modified: Mon Apr 10 08:12:49 2023, max compression
```

## Comparing `elapid-0.3.9.tar` & `elapid-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 cba       (1000) cba       (1000)        0 2022-09-09 16:38:01.030368 elapid-0.3.9/
--rw-r--r--   0 cba       (1000) cba       (1000)     1077 2021-06-26 05:24:58.000000 elapid-0.3.9/LICENSE
--rw-r--r--   0 cba       (1000) cba       (1000)      121 2022-09-09 06:53:10.000000 elapid-0.3.9/MANIFEST.in
--rw-r--r--   0 cba       (1000) cba       (1000)     5595 2022-09-09 16:38:01.030368 elapid-0.3.9/PKG-INFO
--rw-r--r--   0 cba       (1000) cba       (1000)     5051 2022-09-06 17:30:49.000000 elapid-0.3.9/README.md
-drwxr-xr-x   0 cba       (1000) cba       (1000)        0 2022-09-09 16:38:01.026366 elapid-0.3.9/elapid/
--rw-r--r--   0 cba       (1000) cba       (1000)      401 2022-05-02 20:10:05.000000 elapid-0.3.9/elapid/__init__.py
--rw-r--r--   0 cba       (1000) cba       (1000)        8 2022-09-09 06:28:12.000000 elapid-0.3.9/elapid/__version__.py
--rw-r--r--   0 cba       (1000) cba       (1000)     1863 2022-09-09 01:11:05.000000 elapid-0.3.9/elapid/config.py
--rw-r--r--   0 cba       (1000) cba       (1000)    27535 2022-09-08 04:45:29.000000 elapid-0.3.9/elapid/features.py
--rw-r--r--   0 cba       (1000) cba       (1000)    26446 2022-09-08 04:45:29.000000 elapid-0.3.9/elapid/geo.py
--rw-r--r--   0 cba       (1000) cba       (1000)    24197 2022-09-09 06:53:10.000000 elapid-0.3.9/elapid/models.py
--rw-r--r--   0 cba       (1000) cba       (1000)     3689 2022-04-29 18:45:43.000000 elapid-0.3.9/elapid/stats.py
--rw-r--r--   0 cba       (1000) cba       (1000)     3171 2022-05-10 23:20:30.000000 elapid-0.3.9/elapid/types.py
--rw-r--r--   0 cba       (1000) cba       (1000)     7778 2022-09-09 06:11:01.000000 elapid-0.3.9/elapid/utils.py
-drwxr-xr-x   0 cba       (1000) cba       (1000)        0 2022-09-09 16:38:01.029368 elapid-0.3.9/elapid.egg-info/
--rw-r--r--   0 cba       (1000) cba       (1000)     5595 2022-09-09 16:38:00.000000 elapid-0.3.9/elapid.egg-info/PKG-INFO
--rw-r--r--   0 cba       (1000) cba       (1000)      360 2022-09-09 16:38:00.000000 elapid-0.3.9/elapid.egg-info/SOURCES.txt
--rw-r--r--   0 cba       (1000) cba       (1000)        1 2022-09-09 16:38:00.000000 elapid-0.3.9/elapid.egg-info/dependency_links.txt
--rw-r--r--   0 cba       (1000) cba       (1000)      170 2022-09-09 16:38:00.000000 elapid-0.3.9/elapid.egg-info/requires.txt
--rw-r--r--   0 cba       (1000) cba       (1000)        7 2022-09-09 16:38:00.000000 elapid-0.3.9/elapid.egg-info/top_level.txt
--rw-r--r--   0 cba       (1000) cba       (1000)      164 2022-09-09 06:53:10.000000 elapid-0.3.9/requirements.txt
--rw-r--r--   0 cba       (1000) cba       (1000)       38 2022-09-09 16:38:01.030368 elapid-0.3.9/setup.cfg
--rw-r--r--   0 cba       (1000) cba       (1000)     1458 2022-09-09 06:53:10.000000 elapid-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:12:49.799788 elapid-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-10 08:12:11.000000 elapid-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-10 08:12:11.000000 elapid-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-04-10 08:12:49.799788 elapid-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-04-10 08:12:11.000000 elapid-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:12:49.795788 elapid-1.0.1/elapid/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-10 08:12:11.000000 elapid-1.0.1/elapid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 08:12:11.000000 elapid-1.0.1/elapid/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-10 08:12:11.000000 elapid-1.0.1/elapid/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:12:49.799788 elapid-1.0.1/elapid/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20715 2023-04-10 08:12:11.000000 elapid-1.0.1/elapid/data/bradypus.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    27603 2023-04-10 08:12:11.000000 elapid-1.0.1/elapid/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32123 2023-04-10 08:12:11.000000 elapid-1.0.1/elapid/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32802 2023-04-10 08:12:11.000000 elapid-1.0.1/elapid/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-10 08:12:11.000000 elapid-1.0.1/elapid/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-10 08:12:11.000000 elapid-1.0.1/elapid/train_test_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-10 08:12:11.000000 elapid-1.0.1/elapid/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-04-10 08:12:11.000000 elapid-1.0.1/elapid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:12:49.799788 elapid-1.0.1/elapid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-04-10 08:12:49.000000 elapid-1.0.1/elapid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-10 08:12:49.000000 elapid-1.0.1/elapid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:12:49.000000 elapid-1.0.1/elapid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-10 08:12:49.000000 elapid-1.0.1/elapid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 08:12:49.000000 elapid-1.0.1/elapid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-10 08:12:11.000000 elapid-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 08:12:49.799788 elapid-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-10 08:12:11.000000 elapid-1.0.1/setup.py
```

### Comparing `elapid-0.3.9/LICENSE` & `elapid-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elapid-0.3.9/PKG-INFO` & `elapid-1.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,115 +1,106 @@
-Metadata-Version: 2.1
-Name: elapid
-Version: 0.3.9
-Summary: Species distribution modeling support tools
-Home-page: https://elapid.org
-Author: Christopher Anderson
-Author-email: cbanders@stanford.edu
-License: MIT
-Keywords: biogeography,ecology,conservation,SDM,species distribution modeling,maxent
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # elapid
 
 <img src="https://earth-chris.github.io/elapid/img/amazon.jpg" alt="the amazon"/>
 
 <p align="center">
   <em>Contemporary species distribution modeling tools for python.</em>
 </p>
 
 ![GitHub](https://img.shields.io/github/license/earth-chris/elapid)
-![PyPI](https://img.shields.io/pypi/v/elapid)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/earth-chris/elapid/docs)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/elapid)
+![PyPI version](https://img.shields.io/pypi/v/elapid)
+![Anaconda version](https://anaconda.org/conda-forge/elapid/badges/version.svg)
+![PyPI downloads](https://img.shields.io/pypi/dm/elapid)
 ![GitHub last commit](https://img.shields.io/github/last-commit/earth-chris/elapid)
-![Lines of code](https://img.shields.io/tokei/lines/github/earth-chris/elapid)
+[![JOSS manuscript status](https://joss.theoj.org/papers/ac415a024261efb3b397a1bad6f9cde6/status.svg)](https://earth-chris.github.io/elapid/paper/draft-paper.pdf)
 
 ---
 
 **Documentation**: [earth-chris.github.io/elapid](https://earth-chris.github.io/elapid)
 
 **Source code**: [earth-chris/elapid](https://github.com/earth-chris/elapid)
 
 ---
 
 ## :snake: Introduction
 
-`elapid` provides python support for species distribution modeling. This includes a custom implementation of [Maxent][home-maxent] and a suite of tools to simplify working with biogeography data.
+`elapid` is a series of species distribution modeling tools for python. This includes a custom implementation of [Maxent][home-maxent] and a suite of methods to simplify working with biogeography data.
 
 The name is an homage to *A Biogeographic Analysis of Australian Elapid Snakes* (H.A. Nix, 1986), the paper widely credited with defining the essential bioclimatic variables to use in species distribution modeling. It's also a snake pun (a python wrapper for mapping snake biogeography).
 
 ---
 
 ## :seedling: Installation
 
-```bash
-pip install elapid
-```
-
-This should suffice for most linux/mac users, as there are available unix builds of the underlying python dependencies (`numpy`, `sklearn`, `glmnet`, `rasterio`, etc.).
+`pip install elapid` or `conda install -c conda-forge elapid`
 
-Windows installs are more challenging. [glmnet][glmnet] has to compile some fortran code on install, meaning you need to have a fortran compiler running (like [MinGW-w64][mingw] or [Cygwin](https://www.cygwin.com/)).
+Installing `glmnet` is optional, but recommended. This can be done with `pip install elapid[glmnet]` or `conda install -c conda-forge elapid glmnet`. For more support, and for information on why this package is recommended, see [this page](https://elapid.org/install#installing-glmnet).
 
-You can review Windows install instructions with slightly more detail, or contribute a better solution, at [this issue][fortran-issue].
+The `conda` install is recommended for Windows users. While there is a `pip` distribution, you may experience some challenges. The easiest way to overcome them is to use [Windows Subsystem for Linux (WSL)](https://docs.microsoft.com/en-us/windows/wsl/about). Otherwise, see [this page](https://elapid.org/install) for support.
 
 ---
 
-## :deciduous_tree: Package design
+## :deciduous_tree: Why use elapid?
 
 The amount and quality of bioegeographic data has increased dramatically over the past decade, as have cloud-based tools for working with it. `elapid` was designed to provide a set of modern, python-based tools for working with species occurrence records and environmental covariates to map different dimensions of a species' niche.
 
 `elapid` supports working with modern geospatial data formats and uses contemporary approaches to training statistical models. It uses `sklearn` conventions to fit and apply models, `rasterio` to handle raster operations, `geopandas` for vector operations, and processes data under the hood with `numpy`.
 
+This makes it easier to do things like fit/apply models to multi-temporal and multi-scale data, fit geographically-weighted models, create ensembles, precisely define background point distributions, and summarize model predictions.
+
 It does the following things reasonably well:
 
 :globe_with_meridians: **Point sampling**
 
-Select random geographic point samples (aka background or pseudoabsence points) within polygons or rasters, handling `nodata` locations, as well as sampling from bias maps (using `elapid.sample_geoseries()`, `elapid.sample_raster()`, or `elapid.sample_bias_file()`).
+Select random geographic point samples (aka background or pseudoabsence points) within polygons or rasters, handling `nodata` locations, as well as sampling from bias maps (using `elapid.sample_raster()`, `elapid.sample_vector()`, or `elapid.sample_bias_file()`).
 
 :chart_with_upwards_trend: **Vector annotation**
 
-Annotate point data with coincident raster data, creating `GeoDataFrames` with sample locations and co-aligned covariate values (using `elapid.annotate()`).
+Extract and annotate point data from rasters, creating `GeoDataFrames` with sample locations and their matching covariate values (using `elapid.annotate()`). On-the-fly reprojection, dropping nodata, multi-band inputs and multi-file inputs are all supported.
 
 :bar_chart: **Zonal statistics**
 
 Calculate zonal statistics from multi-band, multi-raster data into a single `GeoDataFrame` from one command (using `elapid.zonal_stats()`).
 
 :bug: **Feature transformations**
 
-Transform covariate data into derivative `features` to expand data dimensionality (primarily the `elapid.MaxentFeatureTransformer()`, but see others under `elapid.features`)
+Transform covariate data into derivative `features` to expand data dimensionality and improve prediction accuracy (like `elapid.ProductTransformer()`, `elapid.HingeTransformer()`, or the all-in-one `elapid.MaxentFeatureTransformer()`).
 
 :bird: **Species distribution modeling**
 
-Train and apply generic species distribution models (like `elapid.MaxentModel()` and `elapid.NicheEnvelopeModel()`).
+Train and apply species distribution models based on annotated point data, configured with sensible defaults (like `elapid.MaxentModel()` and `elapid.NicheEnvelopeModel()`).
+
+:satellite: **Training spatially-aware models**
+
+Compute spatially-explicit sample weights, checkerboard train/test splits, or geographically-clustered cross-validation splits to reduce spatial autocorellation effects (with `elapid.distance_weights()`, `elapid.checkerboard_split()` and `elapid.GeographicKFold()`).
 
 :earth_asia: **Applying models to rasters**
 
-Apply pixel-based models with a `.predict()` method to rasters (like training a `RandomForestClassifier()` and applying with `elapid.apply_model_to_rasters()`).
+Apply any pixel-based model with a `.predict()` method to raster data to easily create prediction probability maps (like training a `RandomForestClassifier()` and applying with `elapid.apply_model_to_rasters()`).
 
 :cloud: **Cloud-native geo support**
 
-Work with cloud- or web-hosted raster/vector data (on `https://`, `gs://`, `s3://`, etc.).
+Work with cloud- or web-hosted raster/vector data (on `https://`, `gs://`, `s3://`, etc.) to keep your disk free of temporary files.
+
+Check out some example code snippets and workflows on the [Working with Geospatial Data](https://elapid.org/examples/WorkingWithGeospatialData/) page.
 
 ---
 
-:snake: `elapid` requires some effort on the user's part to draw samples and extract covariate data. This is by design. Selecting background samples, splitting train/test data, and specifying model parameters are all critical modeling choices that have profound effects on model prediction and interpretation. This extra flexibility provides more control over the seemingly black-box approach of Maxent's java implementation, and enabling users to better tune and evaluate their models.
+:snake: `elapid` requires some effort on the user's part to draw samples and extract covariate data. This is by design.
+
+Selecting background samples, computing sample weights, splitting train/test data, and specifying training parameters are all critical modeling choices that have profound effects on inference and interpretation.
+
+The extra flexibility provided by `elapid` enables more control over the seemingly black-box approach of Maxent, enabling users to better tune and evaluate their models.
 
 ---
 
-## Contact
+## Developed by
 
-<a href="https://twitter.com/earth_chris">![Twitter Follow](https://img.shields.io/twitter/follow/earth_chris)</a>
-<a href="https://twitter.com/forestobs">![Twitter Follow](https://img.shields.io/twitter/follow/forestobs)</a>
+[Christopher Anderson](https://cbanderson.info)[^1] [^2]
 
+<a href="https://twitter.com/earth_chris">![Twitter Follow](https://img.shields.io/twitter/follow/earth_chris)</a>
+<a href="https://github.com/earth-chris">![GitHub Stars](https://img.shields.io/github/stars/earth-chris?affiliations=OWNER%2CCOLLABORATOR&style=social)</a>
 
 [home-maxent]: https://biodiversityinformatics.amnh.org/open_source/maxent/
 [r-maxnet]: https://github.com/mrmaxent/maxnet
-[glmnet]: https://github.com/civisanalytics/python-glmnet/
-[fortran-issue]: https://github.com/earth-chris/elapid/issues/9
-[mingw]: https://www.mingw-w64.org/
+[^1]: [EO Lab, Planet Labs PBC](https://www.planet.com)
+[^2]: [Center for Conservation Biology, Stanford University](https://ccb.stanford.edu)
```

### Comparing `elapid-0.3.9/elapid/config.py` & `elapid-1.0.1/elapid/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,31 +25,38 @@
     n_threshold_features: int = 10
 
     # model training metric (from `sklearn.metrics`)
     scorer: str = "roc_auc"
 
     # species prevalence scalar
     tau: float = 0.5
+    transform: str = "cloglog"
 
     # model convergence tolerance threshold
-    tolerance: float = 1e-7
+    tolerance: float = 2e-6
 
     # elasticnet lambda type to use ('best' or 'last')
     use_lambdas: str = "best"
     n_lambdas: int = 100
 
     # method for weighting presence samples
-    class_weights: Union[str, float] = "balanced"
+    # set to "balanced" for nomalizing weights based on sample density
+    class_weights: Union[str, float] = 100
 
 
 # maxent default regularization parameters (from the maxnet R package)
 class RegularizationConfig:
     linear: list = [[0, 10, 30, 100], [1, 1, 0.2, 0.05]]
     quadratic: list = [[0, 10, 17, 30, 100], [1.3, 0.8, 0.5, 0.25, 0.05]]
     product: list = [[0, 10, 17, 30, 100], [2.6, 1.6, 0.9, 0.55, 0.05]]
     hinge: list = [[0, 1], [0.5, 0.5]]
     threshold: list = [[0, 100], [2, 1]]
     categorical: list = [[0, 10, 17], [0.65, 0.5, 0.25]]
 
 
 class NicheEnvelopeConfig:
     percentile_range: Tuple[float, float] = [2.5, 97.5]
+    overlay: str = "average"
+
+
+class EnsembleConfig:
+    reducer: str = "mean"
```

### Comparing `elapid-0.3.9/elapid/features.py` & `elapid-1.0.1/elapid/features.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,65 +1,130 @@
 """Functions to transform covariate data into complex model features."""
 
 from typing import Any, List, Tuple, Union
 
 import numpy as np
 import pandas as pd
-from sklearn.base import BaseEstimator
+from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.preprocessing import MinMaxScaler, OneHotEncoder, QuantileTransformer
 
 from elapid.config import MaxentConfig, RegularizationConfig
 from elapid.types import ArrayLike, validate_boolean, validate_feature_types, validate_numeric_scalar
 from elapid.utils import make_band_labels, repeat_array
 
 
+class FeaturesMixin:
+    """Methods for formatting x data and labels"""
+
+    def _format_covariate_data(self, x: ArrayLike) -> Tuple[np.array, np.array]:
+        """Reads input x data and formats it to consistent array dtypes.
+
+        Args:
+            x: array-like of shape (n_samples, n_features)
+
+        Returns:
+            (continuous, categorical) tuple of ndarrays with continuous and
+                categorical covariate data.
+        """
+        if isinstance(x, np.ndarray):
+            if self.categorical_ is None:
+                con = x
+                cat = None
+            else:
+                con = x[:, self.continuous_]
+                cat = x[:, self.categorical_]
+
+        elif isinstance(x, pd.DataFrame):
+            con = x[self.continuous_pd_].to_numpy()
+            if len(self.categorical_pd_) > 0:
+                cat = x[self.categorical_pd_].to_numpy()
+            else:
+                cat = None
+
+        else:
+            raise TypeError(f"Unsupported x dtype: {type(x)}. Must be pd.DataFrame or np.array")
+
+        return con, cat
+
+    def _format_labels_and_dtypes(self, x: ArrayLike, categorical: list = None, labels: list = None) -> None:
+        """Read input x data and lists of categorical data indices and band
+            labels to format and store this info for later indexing.
+
+        Args:
+            s: array-like of shape (n_samples, n_features)
+            categorical: indices indicating which x columns are categorical
+            labels: covariate column labels. ignored if x is a pandas DataFrame
+        """
+        if isinstance(x, np.ndarray):
+            nrows, ncols = x.shape
+            if categorical is None:
+                continuous = list(range(ncols))
+            else:
+                continuous = list(set(range(ncols)).difference(set(categorical)))
+            self.labels_ = labels or make_band_labels(ncols)
+            self.categorical_ = categorical
+            self.continuous_ = continuous
+
+        elif isinstance(x, pd.DataFrame):
+            x.drop(["geometry"], axis=1, errors="ignore", inplace=True)
+            self.labels_ = labels or list(x.columns)
+
+            # store both pandas and numpy indexing of these values
+            self.continuous_pd_ = list(x.select_dtypes(exclude="category").columns)
+            self.categorical_pd_ = list(x.select_dtypes(include="category").columns)
+
+            all_columns = list(x.columns)
+            self.continuous_ = [all_columns.index(item) for item in self.continuous_pd_ if item in all_columns]
+            if len(self.categorical_pd_) != 0:
+                self.categorical_ = [all_columns.index(item) for item in self.categorical_pd_ if item in all_columns]
+            else:
+                self.categorical_ = None
+
+
 class LinearTransformer(MinMaxScaler):
     """Applies linear feature transformations to rescale features from 0-1."""
 
-    clamp: bool = None
-    feature_range: None
-
     def __init__(
         self,
         clamp: bool = MaxentConfig.clamp,
         feature_range: Tuple[float, float] = (0.0, 1.0),
     ):
         self.clamp = clamp
         self.feature_range = feature_range
         super().__init__(clip=clamp, feature_range=feature_range)
 
 
-class QuadraticTransformer(BaseEstimator):
+class QuadraticTransformer(BaseEstimator, TransformerMixin):
     """Applies quadtratic feature transformations and rescales features from 0-1."""
 
-    clamp: bool = None
-    feature_range: Tuple[float, float] = None
-    estimator: BaseEstimator = None
-
     def __init__(
         self,
         clamp: bool = MaxentConfig.clamp,
         feature_range: Tuple[float, float] = (0.0, 1.0),
     ):
         self.clamp = clamp
         self.feature_range = feature_range
-        self.estimator = MinMaxScaler(clip=self.clamp, feature_range=self.feature_range)
+        self.estimator = None
 
-    def fit(self, x: ArrayLike) -> None:
+    def fit(self, x: ArrayLike) -> "QuadraticTransformer":
         """Compute the minimum and maximum for scaling.
 
         Args:
             x: array-like of shape (n_samples, n_features)
                 The data used to compute the per-feature minimum and maximum
                 used for later scaling along the features axis.
+
         Returns:
-            None. Updates the transformer with feature fitting parameters.
+            self. Returns the transformer with fitted parameters.
         """
+        self.estimator = MinMaxScaler(clip=self.clamp, feature_range=self.feature_range)
         self.estimator.fit(np.array(x) ** 2)
 
+        return self
+
     def transform(self, x: ArrayLike) -> np.ndarray:
         """Scale covariates according to the feature range.
 
         Args:
             x: array-like of shape (n_samples, n_features)
                 Input data that will be transformed.
 
@@ -90,42 +155,42 @@
 
         Returns:
             ndarray with unscaled covariate values.
         """
         return self.estimator.inverse_transform(np.array(x)) ** 0.5
 
 
-class ProductTransformer(BaseEstimator):
+class ProductTransformer(BaseEstimator, TransformerMixin):
     """Computes the column-wise product of an array of input features, rescaling from 0-1."""
 
-    clamp: bool = None
-    feature_range: Tuple[float, float] = None
-    estimator: BaseEstimator = None
-
     def __init__(
         self,
         clamp: bool = MaxentConfig.clamp,
         feature_range: Tuple[float, float] = (0.0, 1.0),
     ):
         self.clamp = clamp
         self.feature_range = feature_range
-        self.estimator = MinMaxScaler(clip=self.clamp, feature_range=self.feature_range)
+        self.estimator = None
 
-    def fit(self, x: ArrayLike) -> None:
+    def fit(self, x: ArrayLike) -> "ProductTransformer":
         """Compute the minimum and maximum for scaling.
 
         Args:
             x: array-like of shape (n_samples, n_features)
                 The data used to compute the per-feature minimum and maximum
                 used for later scaling along the features axis.
+
         Returns:
-            None. Updates the transformer with feature fitting parameters.
+            self. Returns the transformer with fitted parameters.
         """
+        self.estimator = MinMaxScaler(clip=self.clamp, feature_range=self.feature_range)
         self.estimator.fit(column_product(np.array(x)))
 
+        return self
+
     def transform(self, x: ArrayLike) -> np.ndarray:
         """Scale covariates according to the feature range.
 
         Args:
             x: array-like of shape (n_samples, n_features)
                 Input data that will be transformed.
 
@@ -144,40 +209,40 @@
         Returns:
             ndarray with transformed data.
         """
         self.fit(x)
         return self.transform(x)
 
 
-class ThresholdTransformer(BaseEstimator):
-    """Applies binary thresholds to each covariate based on n evenly-spaced
-    thresholds across it's min/max range."""
-
-    n_thresholds_: int = None
-    mins_: np.ndarray = None
-    maxs_: np.ndarray = None
-    threshold_indices_: np.ndarray = None
+class ThresholdTransformer(BaseEstimator, TransformerMixin):
+    """Apply binary thresholds across evenly-spaced bins for each covariate."""
 
     def __init__(self, n_thresholds: int = MaxentConfig.n_threshold_features):
-        self.n_thresholds_ = n_thresholds
+        self.n_thresholds = n_thresholds
+        self.mins_ = None
+        self.maxs_ = None
+        self.threshold_indices_ = None
 
-    def fit(self, x: ArrayLike) -> None:
+    def fit(self, x: ArrayLike) -> "ThresholdTransformer":
         """Compute the minimum and maximum for scaling.
 
         Args:
             x: array-like of shape (n_samples, n_features)
                 The data used to compute the per-feature minimum and maximum
                 used for later scaling along the features axis.
+
         Returns:
-            None. Updates the transformer with feature fitting parameters.
+            self. Returns the transformer with fitted parameters.
         """
         x = np.array(x)
         self.mins_ = x.min(axis=0)
         self.maxs_ = x.max(axis=0)
-        self.threshold_indices_ = np.linspace(self.mins_, self.maxs_, self.n_thresholds_)
+        self.threshold_indices_ = np.linspace(self.mins_, self.maxs_, self.n_thresholds)
+
+        return self
 
     def transform(self, x: ArrayLike) -> np.ndarray:
         """Scale covariates according to the feature range.
 
         Args:
             x: array-like of shape (n_samples, n_features)
                 Input data that will be transformed.
@@ -201,52 +266,53 @@
         Returns:
             ndarray with transformed data.
         """
         self.fit(x)
         return self.transform(x)
 
 
-class HingeTransformer(BaseEstimator):
+class HingeTransformer(BaseEstimator, TransformerMixin):
     """Fits hinge transformations to an array of covariates."""
 
-    n_hinges_: int = None
-    mins_: np.ndarray = None
-    maxs_: np.ndarray = None
-    hinge_indices_: np.ndarray = None
-
     def __init__(self, n_hinges: int = MaxentConfig.n_hinge_features):
-        self.n_hinges_ = n_hinges
+        self.n_hinges = n_hinges
+        self.mins_ = None
+        self.maxs_ = None
+        self.hinge_indices_ = None
 
-    def fit(self, x: ArrayLike) -> None:
+    def fit(self, x: ArrayLike) -> "HingeTransformer":
         """Compute the minimum and maximum for scaling.
 
         Args:
             x: array-like of shape (n_samples, n_features)
                 The data used to compute the per-feature minimum and maximum
                 used for later scaling along the features axis.
+
         Returns:
-            None. Updates the transformer with feature fitting parameters.
+            self. Updatesd transformer with fitted parameters.
         """
         x = np.array(x)
         self.mins_ = x.min(axis=0)
         self.maxs_ = x.max(axis=0)
-        self.hinge_indices_ = np.linspace(self.mins_, self.maxs_, self.n_hinges_)
+        self.hinge_indices_ = np.linspace(self.mins_, self.maxs_, self.n_hinges)
+
+        return self
 
     def transform(self, x: ArrayLike) -> np.ndarray:
         """Scale covariates according to the feature range.
 
         Args:
             x: array-like of shape (n_samples, n_features)
                 Input data that will be transformed.
 
         Returns:
             ndarray with transformed data.
         """
         x = np.array(x)
-        xarr = repeat_array(x, self.n_hinges_ - 1, axis=-1)
+        xarr = repeat_array(x, self.n_hinges - 1, axis=-1)
         lharr = repeat_array(self.hinge_indices_[:-1].transpose(), len(x), axis=0)
         rharr = repeat_array(self.hinge_indices_[1:].transpose(), len(x), axis=0)
         lh = left_hinge(xarr, lharr, self.maxs_)
         rh = right_hinge(xarr, self.mins_, rharr)
         return np.concatenate((lh, rh), axis=2).reshape(x.shape[0], -1)
 
     def fit_transform(self, x: ArrayLike) -> np.ndarray:
@@ -259,44 +325,45 @@
         Returns:
             ndarray with transformed data.
         """
         self.fit(x)
         return self.transform(x)
 
 
-class CategoricalTransformer(BaseEstimator):
+class CategoricalTransformer(BaseEstimator, TransformerMixin):
     """Applies one-hot encoding to categorical covariate datasets."""
 
-    estimators_: list = None
-
     def __init__(self):
-        pass
+        self.estimators_ = None
 
-    def fit(self, x: ArrayLike) -> None:
+    def fit(self, x: ArrayLike) -> "CategoricalTransformer":
         """Compute the minimum and maximum for scaling.
 
         Args:
             x: array-like of shape (n_samples, n_features)
                 The data used to compute the per-feature minimum and maximum
                 used for later scaling along the features axis.
+
         Returns:
-            None. Updates the transformer with feature fitting parameters.
+            self. Returns the transformer with fitted parameters.
         """
         self.estimators_ = []
         x = np.array(x)
         if x.ndim == 1:
             estimator = OneHotEncoder(dtype=np.uint8, sparse=False)
             self.estimators_.append(estimator.fit(x.reshape(-1, 1)))
         else:
             nrows, ncols = x.shape
             for col in range(ncols):
                 xsub = x[:, col].reshape(-1, 1)
                 estimator = OneHotEncoder(dtype=np.uint8, sparse=False)
                 self.estimators_.append(estimator.fit(xsub))
 
+        return self
+
     def transform(self, x: ArrayLike) -> np.ndarray:
         """Scale covariates according to the feature range.
 
         Args:
             x: array-like of shape (n_samples, n_features)
                 Input data that will be transformed.
 
@@ -333,205 +400,141 @@
 class CumulativeTransformer(QuantileTransformer):
     """Applies a percentile-based transform to estimate cumulative suitability."""
 
     def __init__(self):
         super().__init__(n_quantiles=100, output_distribution="uniform")
 
 
-class MaxentFeatureTransformer(BaseEstimator):
+class MaxentFeatureTransformer(BaseEstimator, TransformerMixin, FeaturesMixin):
     """Transforms covariate data into maxent-format feature data."""
 
-    feature_types_: list = None
-    clamp_: bool = None
-    n_hinge_features_: int = None
-    n_threshold_features_: int = None
-    categorical_: list = None
-    continuous_: list = None
-    categorical_pd_: list = None
-    continuous_pd_: list = None
-    labels_: list = None
-    estimators_: dict = {
-        "linear": None,
-        "quadratic": None,
-        "product": None,
-        "threshold": None,
-        "hinge": None,
-        "categorical": None,
-    }
-    feature_names_: list = None
-
     def __init__(
         self,
         feature_types: Union[str, list] = MaxentConfig.feature_types,
         clamp: bool = MaxentConfig.clamp,
         n_hinge_features: int = MaxentConfig.n_hinge_features,
         n_threshold_features: int = MaxentConfig.n_threshold_features,
     ):
         """Computes features based on the maxent feature types specified (like linear, quadratic, hinge).
 
-        Implemented using sklearn conventions (with `.fit()` and `.transform()` functions.
-
         Args:
             feature_types: list of maxent features to generate.
             clamp: set feature values to global mins/maxs during prediction
             n_hinge_features: number of hinge knots to generate
             n_threshold_features: nuber of threshold features to generate
         """
-        self.feature_types_ = validate_feature_types(feature_types)
-        self.clamp_ = validate_boolean(clamp)
-        self.n_hinge_features_ = validate_numeric_scalar(n_hinge_features)
-        self.n_threshold_features_ = validate_numeric_scalar(n_threshold_features)
-
-    def _format_covariate_data(self, x: ArrayLike) -> Tuple[np.array, np.array]:
-        """Reads input x data and formats it to consistent array dtypes.
-
-        Args:
-            x: array-like of shape (n_samples, n_features)
-
-        Returns:
-            (continuous, categorical) tuple of ndarrays with continuous and
-                categorical covariate data.
-        """
-        if isinstance(x, np.ndarray):
-            if self.categorical_ is None:
-                con = x
-                cat = None
-            else:
-                con = x[:, self.continuous_]
-                cat = x[:, self.categorical_]
-
-        elif isinstance(x, pd.DataFrame):
-            con = x[self.continuous_pd_].to_numpy()
-            if len(self.categorical_pd_) > 0:
-                cat = x[self.categorical_pd_].to_numpy()
-            else:
-                cat = None
-
-        else:
-            raise TypeError(f"Unsupported x dtype: {type(x)}. Must be pd.DataFrame or np.array")
-
-        return con, cat
-
-    def _format_labels_and_dtypes(self, x: ArrayLike, categorical: list = None, labels: list = None) -> None:
-        """Read input x data and lists of categorical data indices and band
-            labels to format and store this info for later indexing.
-
-        Args:
-            s: array-like of shape (n_samples, n_features)
-            categorical: indices indicating which x columns are categorical
-            labels: covariate column labels. ignored if x is a pandas DataFrame
-        """
-        if isinstance(x, np.ndarray):
-            nrows, ncols = x.shape
-            if categorical is None:
-                continuous = list(range(ncols))
-            else:
-                continuous = list(set(range(ncols)).difference(set(categorical)))
-            self.labels_ = labels or make_band_labels(ncols)
-            self.categorical_ = categorical
-            self.continuous_ = continuous
-
-        elif isinstance(x, pd.DataFrame):
-            x.drop(["geometry"], axis=1, errors="ignore", inplace=True)
-            self.labels_ = labels or list(x.columns)
-
-            # store both pandas and numpy indexing of these values
-            self.continuous_pd_ = list(x.select_dtypes(exclude="category").columns)
-            self.categorical_pd_ = list(x.select_dtypes(include="category").columns)
-
-            all_columns = list(x.columns)
-            self.continuous_ = [all_columns.index(item) for item in self.continuous_pd_ if item in all_columns]
-            if len(self.categorical_pd_) != 0:
-                self.categorical_ = [all_columns.index(item) for item in self.categorical_pd_ if item in all_columns]
-            else:
-                self.categorical_ = None
+        self.feature_types = feature_types
+        self.clamp = clamp
+        self.n_hinge_features = n_hinge_features
+        self.n_threshold_features = n_threshold_features
+        self.categorical_ = None
+        self.continuous_ = None
+        self.categorical_pd_ = None
+        self.continuous_pd_ = None
+        self.labels_ = None
+        self.feature_names_ = None
+        self.estimators_ = {
+            "linear": None,
+            "quadratic": None,
+            "product": None,
+            "threshold": None,
+            "hinge": None,
+            "categorical": None,
+        }
 
-    def fit(self, x: ArrayLike, categorical: list = None, labels: list = None) -> None:
+    def fit(self, x: ArrayLike, categorical: list = None, labels: list = None) -> "MaxentFeatureTransformer":
         """Compute the minimum and maximum for scaling.
 
         Args:
             x: array-like of shape (n_samples, n_features)
                 The data used to compute the per-feature minimum and maximum
                 used for later scaling along the features axis.
             categorical: indices indicating which x columns are categorical
             labels: covariate column labels. ignored if x is a pandas DataFrame
 
         Returns:
-            None. Updates the transformer with feature fitting parameters.
+            self. Returns the transformer with fitted parameters.
         """
+        self.feature_types = validate_feature_types(self.feature_types)
+        self.clamp = validate_boolean(self.clamp)
+        self.n_hinge_features = validate_numeric_scalar(self.n_hinge_features)
+        self.n_threshold_features = validate_numeric_scalar(self.n_threshold_features)
+
         self._format_labels_and_dtypes(x, categorical=categorical, labels=labels)
         con, cat = self._format_covariate_data(x)
         nrows, ncols = con.shape
 
         feature_names = []
-        if "linear" in self.feature_types_:
-            estimator = LinearTransformer(clamp=self.clamp_)
+        if "linear" in self.feature_types:
+            estimator = LinearTransformer(clamp=self.clamp)
             estimator.fit(con)
             self.estimators_["linear"] = estimator
             feature_names += ["linear"] * estimator.n_features_in_
 
-        if "quadratic" in self.feature_types_:
-            estimator = QuadraticTransformer(clamp=self.clamp_)
+        if "quadratic" in self.feature_types:
+            estimator = QuadraticTransformer(clamp=self.clamp)
             estimator.fit(con)
             self.estimators_["quadratic"] = estimator
             feature_names += ["quadratic"] * estimator.estimator.n_features_in_
 
-        if "product" in self.feature_types_:
-            estimator = ProductTransformer(clamp=self.clamp_)
+        if "product" in self.feature_types:
+            estimator = ProductTransformer(clamp=self.clamp)
             estimator.fit(con)
             self.estimators_["product"] = estimator
             feature_names += ["product"] * estimator.estimator.n_features_in_
 
-        if "threshold" in self.feature_types_:
-            estimator = ThresholdTransformer(n_thresholds=self.n_threshold_features_)
+        if "threshold" in self.feature_types:
+            estimator = ThresholdTransformer(n_thresholds=self.n_threshold_features)
             estimator.fit(con)
             self.estimators_["threshold"] = estimator
-            feature_names += ["threshold"] * (estimator.n_thresholds_ * ncols)
+            feature_names += ["threshold"] * (estimator.n_thresholds * ncols)
 
-        if "hinge" in self.feature_types_:
-            estimator = HingeTransformer(n_hinges=self.n_hinge_features_)
+        if "hinge" in self.feature_types:
+            estimator = HingeTransformer(n_hinges=self.n_hinge_features)
             estimator.fit(con)
             self.estimators_["hinge"] = estimator
-            feature_names += ["hinge"] * ((estimator.n_hinges_ - 1) * 2 * ncols)
+            feature_names += ["hinge"] * ((estimator.n_hinges - 1) * 2 * ncols)
 
         if cat is not None:
             estimator = CategoricalTransformer()
             estimator.fit(cat)
             self.estimators_["categorical"] = estimator
             for est in estimator.estimators_:
                 feature_names += ["categorical"] * len(est.categories_[0])
 
         self.feature_names_ = feature_names
 
+        return self
+
     def transform(self, x: ArrayLike) -> np.ndarray:
         """Scale covariates according to the feature range.
 
         Args:
             x: array-like of shape (n_samples, n_features)
                 Input data that will be transformed.
 
         Returns:
             ndarray with transformed data.
         """
         con, cat = self._format_covariate_data(x)
         features = []
 
-        if "linear" in self.feature_types_:
+        if "linear" in self.feature_types:
             features.append(self.estimators_["linear"].transform(con))
 
-        if "quadratic" in self.feature_types_:
+        if "quadratic" in self.feature_types:
             features.append(self.estimators_["quadratic"].transform(con))
 
-        if "product" in self.feature_types_:
+        if "product" in self.feature_types:
             features.append(self.estimators_["product"].transform(con))
 
-        if "threshold" in self.feature_types_:
+        if "threshold" in self.feature_types:
             features.append(self.estimators_["threshold"].transform(con))
 
-        if "hinge" in self.feature_types_:
+        if "hinge" in self.feature_types:
             features.append(self.estimators_["hinge"].transform(con))
 
         if cat is not None:
             features.append(self.estimators_["categorical"].transform(cat))
 
         return np.concatenate(features, axis=1)
```

### Comparing `elapid-0.3.9/elapid/geo.py` & `elapid-1.0.1/elapid/geo.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,37 +6,38 @@
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import pyproj
 import rasterio as rio
 from rasterio.features import geometry_mask
+from scipy.spatial import KDTree
 from shapely.geometry import MultiPoint, MultiPolygon, Point, Polygon
 from sklearn.base import BaseEstimator
 
-from elapid.stats import get_raster_stats_methods
-from elapid.types import CRSType, to_iterable
+from elapid.stats import get_raster_stats_methods, normalize_sample_probabilities
+from elapid.types import CRSType, Vector, to_iterable
 from elapid.utils import (
     NoDataException,
     check_raster_alignment,
     create_output_raster_profile,
     format_band_labels,
     get_raster_band_indexes,
     get_tqdm,
     n_digits,
+    tqdm_opts,
 )
 
 tqdm = get_tqdm()
-tqdm_opts = {"bar_format": "{l_bar}{bar:20}{r_bar}{bar:-20b}"}
 
 # sampling tools
 
 
 def xy_to_geoseries(
-    x: Union[float, list, np.ndarray], y: Union[float, list, np.ndarray], crs: CRSType = "epsg:4236"
+    x: Union[float, list, np.ndarray], y: Union[float, list, np.ndarray], crs: CRSType = "epsg:4326"
 ) -> gpd.GeoSeries:
     """Converts x/y data into a geopandas geoseries.
 
     Args:
         x: 1-D array-like of x location values
         y: 1-D array-like of y location values
         crs: coordinate reference system. accepts pyproj.CRS / rio.crs.CRS objects
@@ -51,37 +52,104 @@
 
     points = [Point(x, y) for x, y in zip(x, y)]
     gs = gpd.GeoSeries(points, crs=crs)
 
     return gs
 
 
-def sample_raster(raster_path: str, count: int, ignore_mask: bool = False) -> gpd.GeoSeries:
-    """Creates a random geographic sampling of points based on a raster's extent.
+def stack_geodataframes(
+    presence: Vector, background: Vector, add_class_label: bool = False, target_crs: str = "presence"
+) -> gpd.GeoDataFrame:
+    """Concatenate geometries from two GeoSeries/GeoDataFrames.
+
+    Args:
+        presence: presence geometry (y=1) locations
+        background: background geometry (y=0) locations
+        add_class_label: add a column labeling the y value for each point
+        target_crs: if reprojection is necessary, use this variable's crs.
+            valid options are "presence" and "background"
+
+    Returns:
+        merged GeoDataFrame with all geometries projected to the same crs.
+    """
+    validate_gpd(presence)
+    validate_gpd(background)
+
+    # cast to geodataframes
+    if isinstance(presence, gpd.GeoSeries):
+        presence = presence.to_frame("geometry")
+    if isinstance(background, gpd.GeoSeries):
+        background = background.to_frame("geometry")
+
+    # handle projection mismatch
+    crs = presence.crs
+    if crs_match(presence.crs, background.crs):
+        # explicitly set the two to exactly matching crs as geopandas
+        # throws errors if there's any mismatch at all
+        background.crs = presence.crs
+    else:
+        if target_crs.lower() == "presence":
+            background.to_crs(crs, inplace=True)
+        elif target_crs.lower() == "background":
+            crs = background.crs
+            presence.to_crs(crs, inplace=True)
+        else:
+            raise NameError(f"Unrecognized target_crs option: {target_crs}")
+
+    if add_class_label:
+        presence["class"] = 1
+        background["class"] = 0
+
+    matching = [col for col in presence.columns if col in background.columns]
+    assert len(matching) > 0, "no matching columns found between data frames"
+
+    merged = pd.concat((presence[matching], background[matching]), axis=0, ignore_index=True)
+    gdf = gpd.GeoDataFrame(merged, crs=crs)
+
+    return gdf
+
+
+def sample_raster(raster_path: str, count: int, nodata: float = None, ignore_mask: bool = False) -> gpd.GeoSeries:
+    """Create a random geographic sample of points based on a raster's extent.
 
     Selects from unmasked locations if the rasters nodata value is set.
 
     Args:
         raster_path: raster file path to sample locations from
         count: number of samples to generate
+        nodata: add pixels with this value to the nodata mask
         ignore_mask: sample from the full extent of the raster instead of unmasked areas only
 
     Returns:
         points: Point geometry geoseries
     """
     # handle masked vs unmasked data differently
     with rio.open(raster_path) as src:
-
         if src.nodata is None or ignore_mask:
-            xmin, ymin, xmax, ymax = src.bounds
-            xy = np.random.uniform((xmin, ymin), (xmax, ymax), (count, 2))
+            if nodata is None:
+                xmin, ymin, xmax, ymax = src.bounds
+                xy = np.random.uniform((xmin, ymin), (xmax, ymax), (count, 2))
+            else:
+                data = src.read(1)
+                mask = data != nodata
+                rows, cols = np.where(mask)
+                samples = np.random.randint(0, len(rows), count)
+                xy = np.zeros((count, 2))
+                for i, sample in enumerate(samples):
+                    xy[i] = src.xy(rows[sample], cols[sample])
 
         else:
-            masked = src.read_masks(1)
-            rows, cols = np.where(masked == 255)
+            if nodata is None:
+                masked = src.read_masks(1)
+                rows, cols = np.where(masked == 255)
+            else:
+                data = src.read(1, masked=True)
+                data.mask += data.data == nodata
+                rows, cols = np.where(~data.mask)
+
             samples = np.random.randint(0, len(rows), count)
             xy = np.zeros((count, 2))
             for i, sample in enumerate(samples):
                 xy[i] = src.xy(rows[sample], cols[sample])
 
         points = xy_to_geoseries(xy[:, 0], xy[:, 1], crs=src.crs)
         return points
@@ -96,27 +164,26 @@
         count: total number of samples to generate
         ignore_mask: sample from the full extent of the raster instead of unmasked areas only
 
     Returns:
         points: Point geometry geoseries
     """
     with rio.open(raster_path) as src:
-
         if src.nodata is None or ignore_mask:
             data = src.read(1)
             rows, cols = np.where(data)
             values = data.flatten()
-            probabilities = (values - values.min()) / (values - values.min()).sum()
+            probabilities = normalize_sample_probabilities(values)
             samples = np.random.choice(len(rows), size=count, p=probabilities)
 
         else:
             data = src.read(1, masked=True)
             rows, cols = np.where(~data.mask)
             values = data[rows, cols]
-            probabilities = (values - values.min()) / (values - values.min()).sum()
+            probabilities = normalize_sample_probabilities(values)
             samples = np.random.choice(len(rows), size=count, p=probabilities)
 
         xy = np.zeros((count, 2))
         for i, sample in enumerate(samples):
             xy[i] = src.xy(rows[sample], cols[sample])
 
         points = xy_to_geoseries(xy[:, 0], xy[:, 1], crs=src.crs)
@@ -237,178 +304,189 @@
 
     return matches
 
 
 # raster reading tools
 
 
-def _read_pixel_value(point: gpd.GeoSeries, source: rio.io.DatasetReader) -> np.ndarray:
-    """Reads raster value from an open rasterio dataset.
-
-    Designed to be run using a `geodataframe.apply()` function.
-
-    Args:
-        point: a row from gdf.apply() or gdf.iterrows()
-        source: an open rasterio data source
-
-    Returns:
-        values: 1-d n-length array with the pixel values of each raster band.
-    """
-    row, col = source.index(point.geometry.x, point.geometry.y)
-    window = rio.windows.Window(col, row, 1, 1)
-    values = source.read(window=window, boundless=True)
-    return np.squeeze(values)
-
-
 def annotate(
     points: Union[str, gpd.GeoSeries, gpd.GeoDataFrame],
     raster_paths: Union[str, list],
     labels: list = None,
     drop_na: bool = True,
-):
+    quiet: bool = False,
+) -> gpd.GeoDataFrame:
     """Read raster values for each point in a vector and append as new columns.
 
     Args:
         points: path to a point-format vector, OR
             GeoDataFrame with point locations, OR
             GeoSeries (e.g., gdf['geometry']) with point locations
         raster_paths: raster paths to extract pixel values from.
         labels: band name labels. number of labels should match the
             total number of bands across all raster_paths.
         drop_na: drop all records with no-data values.
+        quiet: silence progress bar output.
 
     Returns:
-        gdf: GeoDataFrame annotated with the pixel values from each raster
+        GeoDataFrame annotated with the pixel values from each raster
     """
     # format the inputs
     raster_paths = to_iterable(raster_paths)
     labels = format_band_labels(raster_paths, labels)
 
     # read raster values based on the points dtype
     if isinstance(points, gpd.GeoSeries):
+        points = points.reset_index(drop=True)
         gdf = annotate_geoseries(
             points,
             raster_paths,
             labels=labels,
             drop_na=drop_na,
+            quiet=quiet,
         )
 
     elif isinstance(points, gpd.GeoDataFrame) or isinstance(points, pd.DataFrame):
+        points = points.reset_index(drop=True)
         gdf = annotate_geoseries(
             points.geometry,
             raster_paths,
             labels=labels,
             drop_na=drop_na,
+            quiet=quiet,
         )
 
         # append annotations to the input dataframe
         gdf = pd.concat([points, gdf.drop(["geometry"], axis=1, errors="ignore")], axis=1)
 
     elif os.path.isfile(points):
-        gdf = annotate_vector(points, raster_paths, labels=labels, drop_na=drop_na)
+        gdf = annotate_vector(points, raster_paths, labels=labels, drop_na=drop_na, quiet=quiet)
 
     else:
         raise TypeError("points arg must be a valid path, GeoDataFrame, or GeoSeries")
 
+    if drop_na:
+        try:
+            valid = gdf["valid"] == 1
+            gdf = gdf[valid].drop(columns="valid").dropna().reset_index(drop=True)
+        except KeyError:
+            pass
+
     return gdf
 
 
 def annotate_vector(
     vector_path: str,
     raster_paths: list,
     labels: list = None,
     drop_na: bool = True,
+    quiet: bool = False,
 ) -> gpd.GeoDataFrame:
     """Reads and stores pixel values from rasters using a point-format vector file.
 
     Args:
         vector_path: path to a vector file (shp, geojson, etc)
         raster_paths: raster paths to extract pixel values from
         labels: band name labels. should match the total number of bands across all raster_paths
         drop_na: drop all records with no-data values
+        quiet: silence progress bar output.
 
     Returns:
         gdf: GeoDataFrame annotated with the pixel values from each raster
     """
     # format the inputs
     raster_paths = to_iterable(raster_paths)
     labels = format_band_labels(raster_paths, labels)
 
     gdf = gpd.read_file(vector_path)
     raster_df = annotate_geoseries(gdf.geometry, raster_paths, labels, drop_na)
     gdf = pd.concat([gdf, raster_df.drop(["geometry"], axis=1, errors="ignore")], axis=1)
+
     return gdf
 
 
 def annotate_geoseries(
-    points: gpd.GeoSeries, raster_paths: list, labels: list = None, drop_na: bool = True, dtype: str = None
-) -> gpd.GeoDataFrame:
+    points: gpd.GeoSeries,
+    raster_paths: list,
+    labels: list = None,
+    drop_na: bool = True,
+    dtype: str = None,
+    quiet: bool = False,
+) -> (gpd.GeoDataFrame, np.ndarray):
     """Reads and stores pixel values from rasters using point locations.
 
     Args:
         points: GeoSeries with point locations.
         raster_paths: rasters to extract pixel values from.
         labels: band labels. must match the total number of bands for all raster_paths.
         drop_na: drop records with no-data values.
         dtype: output column data type. uses the first raster's dtype by default.
+        quiet: silence progress bar output.
 
     Returns:
         gdf: GeoDataFrame annotated with the pixel values from each raster
     """
     # format the inputs
     raster_paths = to_iterable(raster_paths)
     labels = format_band_labels(raster_paths, labels)
 
     # get the dataset dimensions
     n_rasters = len(raster_paths)
-    n_points = len(points)
 
     # create arrays and flags for updating
     raster_values = []
     valid_idxs = []
     nodata_flag = False
 
     # annotate each point with the pixel values for each raster
-    for raster_idx, raster_path in tqdm(enumerate(raster_paths), desc="Raster", total=n_rasters, **tqdm_opts):
+    for raster_idx, raster_path in tqdm(
+        enumerate(raster_paths), desc="Raster", total=n_rasters, disable=quiet, **tqdm_opts
+    ):
         with rio.open(raster_path, "r") as src:
-
             # reproject points to match raster and convert to a dataframe
             if not crs_match(points.crs, src.crs):
                 points = points.to_crs(src.crs)
 
             # use the first rasters dtype for the output array if not set
             if raster_idx == 0 and dtype is None:
                 dtype = src.dtypes[0]
 
             # get the raster row/col indices for each point and the respective read windows
             xys = [(point.x, point.y) for point in points]
 
             # read each pixel value
-            samples = src.sample(xys, masked=False)
-
-            # assign to an output array
-            outarr = np.zeros((n_points, src.count), dtype=dtype)
-            for idx, sample in enumerate(samples):
-                outarr[idx] = sample
+            n_points = len(points)
+            samples_iter = list(
+                tqdm(
+                    src.sample(xys, masked=False),
+                    desc="Sample",
+                    total=n_points,
+                    leave=False,
+                    disable=quiet,
+                    **tqdm_opts,
+                )
+            )
+            samples = np.array(samples_iter, dtype=dtype)
+            raster_values.append(samples)
 
             # identify nodata points to remove later
             if drop_na and src.nodata is not None:
                 nodata_flag = True
-                valid_idxs.append(outarr[:, 0] != src.nodata)
-
-            raster_values.append(outarr)
+                valid_idxs.append(samples[:, 0] != src.nodata)
 
     # merge the arrays from each raster
     values = np.concatenate(raster_values, axis=1, dtype=dtype)
 
     if nodata_flag:
-        valid = np.max(valid_idxs, axis=0)
-        values = values[valid, :]
-        points = points.iloc[valid]
-        points.index = range(valid.sum())
+        valid = np.all(valid_idxs, axis=0).reshape(-1, 1)
+        values = np.concatenate([values, valid], axis=1, dtype=dtype)
+        labels.append("valid")
+        # values = values[valid, :]
+        # points = points.iloc[valid]
+        # points.index = range(valid.sum())
 
     # convert to a geodataframe
     gdf = gpd.GeoDataFrame(values, geometry=points.geometry, columns=labels)
 
     return gdf
 
 
@@ -433,16 +511,15 @@
         model: object with a `model.predict()` function
         array: array of shape (nbands, nrows, ncols) with pixel values
         nodata: numeric nodata value to apply to the output array
         nodata_idx: array of bools with shape (nbands, nrows, ncols) containing nodata locations
         count: number of bands in the prediction output
         dtype: prediction array dtype
         predict_proba: use model.predict_proba() instead of model.predict()
-        **kwargs: additonal keywords to pass to model.predict().
-            For MaxentModels, this would include transform="logistic"
+        **kwargs: additonal keywords to pass to model.predict()
 
     Returns:
         ypred_window: Array of shape (nrows, ncols) with model predictions
     """
     # only apply to valid pixels
     valid = ~nodata_idx.any(axis=0)
     covariates = array[:, valid].transpose()
@@ -467,14 +544,15 @@
     driver: str = "GTiff",
     compress: str = "deflate",
     bigtiff: bool = True,
     template_idx: int = 0,
     windowed: bool = True,
     predict_proba: bool = False,
     ignore_sklearn: bool = True,
+    quiet: bool = False,
     **kwargs,
 ) -> None:
     """Applies a trained model to a list of raster datasets.
 
     The list and band order of the rasters must match the order of the covariates
     used to train the model. It reads each dataset block-by-block, applies
     the model, and writes gridded predictions. If the raster datasets are not
@@ -497,16 +575,16 @@
         bigtiff: specify the output file as a bigtiff (for rasters > 2GB)
         template_idx: index of the raster file to use as a template.
             template_idx=0 sets the first raster as template
         windowed: apply the model using windowed read/write
             slower, but more memory efficient
         predict_proba: use model.predict_proba() instead of model.predict()
         ignore_sklearn: silence sklearn warning messages
+        quiet: silence progress bar output
         **kwargs: additonal keywords to pass to model.predict()
-            For MaxentModels, this would include transform="logistic"
 
     Returns:
         None: saves model predictions to disk.
     """
     # make sure the raster_paths are iterable
     raster_paths = to_iterable(raster_paths)
 
@@ -548,16 +626,15 @@
             "height": dst_profile["height"],
             "width": dst_profile["width"],
         }
         srcs = [rio.vrt.WarpedVRT(src, **vrt_options) for src in srcs]
 
     # read and reproject blocks from each data source and write predictions to disk
     with rio.open(output_path, "w", **dst_profile) as dst:
-        for window in tqdm(windows, desc="Window", **tqdm_opts):
-
+        for window in tqdm(windows, desc="Window", disable=quiet, **tqdm_opts):
             # create stacked arrays to handle multi-raster, multi-band inputs
             # that may have different nodata locations
             covariates = np.zeros((nbands, window.height, window.width), dtype=np.float32)
             nodata_idx = np.ones_like(covariates, dtype=bool)
 
             try:
                 for i, src in enumerate(srcs):
@@ -581,28 +658,28 @@
                 )
                 dst.write(predictions, window=window)
 
             except NoDataException:
                 continue
 
 
-def validate_gpd(geo: Union[gpd.GeoSeries, gpd.GeoDataFrame]) -> None:
+def validate_gpd(geo: Vector) -> None:
     """Validates whether an input is a GeoDataFrame or a GeoSeries.
 
     Args:
         geo: an input variable that should be in GeoPandas format
 
     Raises:
         TypeError: geo is not a GeoPandas dataframe or series
     """
     if not (isinstance(geo, gpd.GeoDataFrame) or isinstance(geo, gpd.GeoSeries)):
         raise TypeError("Input must be a GeoDataFrame or GeoSeries")
 
 
-def validate_polygons(geometry: Union[gpd.GeoSeries, gpd.GeoDataFrame]) -> pd.Index:
+def validate_polygons(geometry: Vector) -> pd.Index:
     """Iterate over a geoseries to find rows with invalid geometry types.
 
     Args:
         geometry: a GeoSeries or GeoDataFrame with polygon geometries
 
     Returns:
         an index of rows with valid polygon types
@@ -648,42 +725,44 @@
     # update the mask
     data[:, poly_mask] = np.ma.masked
 
     return data
 
 
 def zonal_stats(
-    polygons: Union[gpd.GeoSeries, gpd.GeoDataFrame],
+    polygons: Vector,
     raster_paths: list,
     labels: list = None,
     all_touched: bool = True,
     mean: bool = True,
     stdv: bool = True,
     min: bool = False,
     max: bool = False,
     count: bool = False,
     sum: bool = False,
     skew: bool = False,
     kurtosis: bool = False,
     mode: bool = False,
     all: bool = False,
     percentiles: list = [],
+    quiet: bool = False,
 ) -> gpd.GeoDataFrame:
     """Compute raster summary stats for each polygon in a GeoSeries or GeoDataFrame.
 
     Args:
         polygons: GeoSeries or GeoDataFrame with polygon geometries.
         raster_paths: list of paths to rasters to summarize
         labels: band labels. must match the total number of bands for all raster_paths.
         all_touched: include all pixels that touch a polygon.
             set to False to only include pixels whose centers intersect the polygon
         mean, min, max, count, sum, stdv, skew, kurtosis, mode:
             set to True to compute these stats
         all: compute all of the above stats
         percentiles: list of 0-100 percentile ranges to compute
+        quiet: silence progress bar output
 
     Returns:
         GeoDataFrame with zonal stats for each raster band in new columns.
             If `polygons` is a GeoDataFrame, the zonal stats columns are appended
             to the original input.
     """
     # format the input geometries
@@ -715,38 +794,38 @@
         all=all,
     )
 
     # create dataframes for each raster and concatenate at the end
     raster_dfs = []
 
     # run zonal stats raster-by-raster (instead of iterating first over geometries)
-    for r, raster in tqdm(enumerate(raster_paths), total=len(raster_paths), desc="Raster", **tqdm_opts):
-
+    for r, raster in tqdm(enumerate(raster_paths), total=len(raster_paths), desc="Raster", disable=quiet, **tqdm_opts):
         # format the band labels
         band_labels = labels[band_idx[r] : band_idx[r + 1]]
         n_raster_bands = band_idx[r + 1] - band_idx[r]
         stats_labels = []
         for method in stats_methods:
             stats_labels.append([f"{band}_{method.name}" for band in band_labels])
 
         # open the raster for reading
         with rio.open(raster, "r") as src:
-
             # reproject the polygon data as necessary
             if not crs_match(polys.crs, src.crs):
                 polys = polys.to_crs(src.crs)
 
             # create output arrays to store each stat's output
             stats_arrays = []
             for method in stats_methods:
                 dtype = method.dtype or src.dtypes[0]
                 stats_arrays.append(np.zeros((len(polys), n_raster_bands), dtype=dtype))
 
             # iterate over each geometry to read data and compute stats
-            for p, poly in tqdm(enumerate(polys), total=len(polys), desc="Polygon", leave=False, **tqdm_opts):
+            for p, poly in tqdm(
+                enumerate(polys), total=len(polys), desc="Polygon", leave=False, disable=quiet, **tqdm_opts
+            ):
                 data = read_raster_from_polygon(src, poly)
                 for method, array in zip(stats_methods, stats_arrays):
                     array[p, :] = method.reduce(data)
 
         # convert each stat's array into dataframes and merge them together
         stats_dfs = [pd.DataFrame(array, columns=labels) for array, labels in zip(stats_arrays, stats_labels)]
         raster_dfs.append(pd.concat(stats_dfs, axis=1))
@@ -754,7 +833,87 @@
     # merge the outputs from each raster
     if is_df:
         merged = gpd.GeoDataFrame(pd.concat([polygons] + raster_dfs, axis=1), crs=polygons.crs)
     else:
         merged = gpd.GeoDataFrame(pd.concat(raster_dfs, axis=1), geometry=polygons, crs=polygons.crs)
 
     return merged
+
+
+# sample weighting methods
+
+
+def nearest_point_distance(
+    points1: Vector, points2: Vector = None, n_neighbors: int = 1, cpu_count: int = -1
+) -> np.ndarray:
+    """Compute the average euclidean distance to the nearest point in a series.
+
+    Args:
+        points1: return the closest distance *from* these points
+        points2: return the closest distance *to* these points
+            if None, compute the distance to the nearest points
+            in the points1 series
+        n_neighbors: compute the average distance to the nearest n_neighbors.
+            set to -1 to compute the distance to all neighbors.
+        cpu_count: number of cpus to use for estimation.
+            -1 uses all cores
+
+    Returns:
+        array of shape (len(points),) with the distance to
+            each point's nearest neighbor
+    """
+    if points1.crs.is_geographic:
+        warnings.warn("Computing distances using geographic coordinates is bad")
+
+    pta1 = np.array(list(zip(points1.geometry.x, points1.geometry.y)))
+    k_offset = 1
+
+    if points2 is None:
+        pta2 = pta1
+        k_offset += 1
+
+    else:
+        pta2 = np.array(list(zip(points2.geometry.x, points2.geometry.y)))
+        if not crs_match(points1.crs, points2.crs):
+            warnings.warn("CRS mismatch between points")
+
+    if n_neighbors < 1:
+        n_neighbors = len(pta2) - k_offset
+
+    tree = KDTree(pta1)
+    k = np.arange(n_neighbors) + k_offset
+    distance, idx = tree.query(pta2, k=k, workers=cpu_count)
+
+    return distance.mean(axis=1)
+
+
+def distance_weights(points: Vector, n_neighbors: int = -1, center: str = "median", cpu_count: int = -1) -> np.ndarray:
+    """Compute sample weights based on the distance between points.
+
+    Assigns higher scores to isolated points, lower scores to clustered points.
+
+    Args:
+        points: point-format GeoSeries or GeoDataFrame
+        n_neighbors: compute weights based on average distance to the nearest n_neighbors
+            set to -1 to compute the distance to all neighbors.
+        center: rescale the weights to center the mean or median of the array on 1
+            accepts either 'mean' or 'median' as input.
+            pass None to ignore.
+        cpu_count: number of cpus to use for estimation.
+            -1 uses all cores
+
+    Returns:
+        array of shape (len(points),) with scaled sample weights. Scaling
+            is performed by dividing by the maximum value, preserving the
+            relative scale of differences between the min and max distance.
+    """
+    distances = nearest_point_distance(points, n_neighbors=n_neighbors, cpu_count=cpu_count)
+    weights = distances / distances.max()
+
+    if center is not None:
+        if center.lower() == "mean":
+            weights /= weights.mean()
+
+        elif center.lower() == "median":
+            weights /= np.median(weights)
+
+    return weights
```

### Comparing `elapid-0.3.9/elapid/models.py` & `elapid-1.0.1/elapid/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,263 @@
 """Classes for training species distribution models."""
 from typing import List, Tuple, Union
-from warnings import warn
 
+import matplotlib.pyplot as plt
 import numpy as np
-import pandas as pd
+from scipy import stats as scistats
 from sklearn.base import BaseEstimator
 from sklearn.exceptions import NotFittedError
+from sklearn.inspection import partial_dependence, permutation_importance
 from sklearn.linear_model import LogisticRegression
+from sklearn.metrics import roc_auc_score
 
-from elapid import features as _features
-from elapid.config import MaxentConfig, NicheEnvelopeConfig
-from elapid.types import ArrayLike, Number, validate_feature_types
-from elapid.utils import NCPUS, make_band_labels
+from elapid.config import EnsembleConfig, MaxentConfig, NicheEnvelopeConfig
+from elapid.features import (
+    CategoricalTransformer,
+    FeaturesMixin,
+    MaxentFeatureTransformer,
+    compute_lambdas,
+    compute_regularization,
+    compute_weights,
+)
+from elapid.types import ArrayLike, validate_feature_types
+from elapid.utils import NCPUS, make_band_labels, square_factor
 
 # handle windows systems without functioning gfortran compilers
 FORCE_SKLEARN = False
 try:
     from glmnet.logistic import LogitNet
 
 except ModuleNotFoundError:
-    warn(
-        "Failed to import glmnet: using sklearn for Maxent. Interpret results with caution.",
-        category=RuntimeWarning,
-    )
     FORCE_SKLEARN = True
 
 
-class MaxentModel(BaseEstimator):
-    """Model estimator for Maxent-style species distribution models."""
+class SDMMixin:
+    """Mixin class for SDM classifiers."""
+
+    _estimator_type = "classifier"
+    classes_ = [0, 1]
+
+    def score(self, x: ArrayLike, y: ArrayLike, sample_weight: ArrayLike = None) -> float:
+        """Return the mean AUC score on the given test data and labels.
+
+        Args:
+            x: test samples. array-like of shape (n_samples, n_features).
+            y: presence/absence labels. array-like of shape (n_samples,).
+            sample_weight: array-like of shape (n_samples,)
+
+        Returns:
+            AUC score of `self.predict(x)` w.r.t. `y`.
+        """
+        return roc_auc_score(y, self.predict(x), sample_weight=sample_weight)
+
+    def _more_tags(self):
+        return {"requires_y": True}
+
+    def permutation_importance_scores(
+        self,
+        x: ArrayLike,
+        y: ArrayLike,
+        sample_weight: ArrayLike = None,
+        n_repeats: int = 10,
+        n_jobs: int = -1,
+    ) -> np.ndarray:
+        """Compute a generic feature importance score by modifying feature values
+            and computing the relative change in model performance.
+
+        Permutation importance measures how much a model score decreases when a
+            single feature value is randomly shuffled. This score doesn't reflect
+            the intrinsic predictive value of a feature by itself, but how important
+            feature is for a particular model.
+
+        Args:
+            x: test samples. array-like of shape (n_samples, n_features).
+            y: presence/absence labels. array-like of shape (n_samples,).
+            sample_weight: array-like of shape (n_samples,)
+            n_repeats: number of permutation iterations.
+            n_jobs: number of parallel compute tasks. set to -1 for all cpus.
+
+        Returns:
+            importances: an array of shape (n_features, n_repeats).
+        """
+        pi = permutation_importance(self, x, y, sample_weight=sample_weight, n_jobs=n_jobs, n_repeats=n_repeats)
+
+        return pi.importances
+
+    def permutation_importance_plot(
+        self,
+        x: ArrayLike,
+        y: ArrayLike,
+        sample_weight: ArrayLike = None,
+        n_repeats: int = 10,
+        labels: list = None,
+        **kwargs,
+    ) -> Tuple[plt.Figure, plt.Axes]:
+        """Create a box plot with bootstrapped permutation importance scores for each covariate.
+
+        Permutation importance measures how much a model score decreases when a
+            single feature value is randomly shuffled. This score doesn't reflect
+            the intrinsic predictive value of a feature by itself, but how important
+            feature is for a particular model.
+
+        It is often appropriate to compute permuation importance scores using both
+            training and validation sets. Large differences between the two may
+            indicate overfitting.
+
+        This implementation does not necessarily match the implementation in Maxent.
+            These scores may be difficult to interpret if there is a high degree
+            of covariance between features or if the model estimator includes any
+            non-linear feature transformations (e.g. 'hinge' features).
+
+        Reference:
+            https://scikit-learn.org/stable/modules/permutation_importance.html
+
+        Args:
+            x: evaluation features. array-like of shape (n_samples, n_features).
+            y: presence/absence labels. array-like of shape (n_samples,).
+            sample_weight: array-like of shape (n_samples,)
+            n_repeats: number of permutation iterations.
+            labels: list of band names to label the plots.
+            **kwargs: additional arguments to pass to `plt.subplots()`.
+
+        Returns:
+            fig, ax: matplotlib subplot figure and axes.
+        """
+        importance = self.permutation_importance_scores(x, y, sample_weight=sample_weight, n_repeats=n_repeats)
+        rank_order = importance.mean(axis=-1).argsort()
+
+        if labels is None:
+            try:
+                labels = x.columns.tolist()
+            except AttributeError:
+                labels = make_band_labels(x.shape[-1])
+        labels = [labels[idx] for idx in rank_order]
+
+        plot_defaults = {"dpi": 150, "figsize": (5, 4)}
+        plot_defaults.update(**kwargs)
+        fig, ax = plt.subplots(**plot_defaults)
+        ax.boxplot(
+            importance[rank_order].T,
+            vert=False,
+            labels=labels,
+        )
+        fig.tight_layout()
+
+        return fig, ax
+
+    def partial_dependence_scores(
+        self,
+        x: ArrayLike,
+        percentiles: tuple = (0.025, 0.975),
+        n_bins: int = 100,
+        categorical_features: tuple = [None],
+    ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+        """Compute partial dependence scores for each feature.
+
+        Args:
+            x: evaluation features. array-like of shape (n_samples, n_features).
+                used to constrain the range of values to evaluate for each feature.
+            percentiles: lower and upper percentiles used to set the range to plot.
+            n_bins: the number of bins spanning the lower-upper percentile range.
+            categorical_features: a 0-based index of which features are categorical.
+
+        Returns:
+            bins, mean, stdv: the binned feature values and the mean/stdv of responses.
+        """
+        ncols = x.shape[1]
+        mean = np.zeros((ncols, n_bins))
+        stdv = np.zeros_like(mean)
+        bins = np.zeros_like(mean)
+
+        for idx in range(ncols):
+            if idx in categorical_features:
+                continue
+            pd = partial_dependence(
+                self,
+                x,
+                [idx],
+                percentiles=percentiles,
+                grid_resolution=n_bins,
+                kind="individual",
+            )
+            mean[idx] = pd["individual"][0].mean(axis=0)
+            stdv[idx] = pd["individual"][0].std(axis=0)
+            bins[idx] = pd["values"][0]
+
+        return bins, mean, stdv
+
+    def partial_dependence_plot(
+        self,
+        x: ArrayLike,
+        percentiles: tuple = (0.025, 0.975),
+        n_bins: int = 50,
+        categorical_features: tuple = None,
+        labels: list = None,
+        **kwargs,
+    ) -> Tuple[plt.Figure, plt.Axes]:
+        """Plot the response of an estimator across the range of feature values.
+
+        Args:
+            x: evaluation features. array-like of shape (n_samples, n_features).
+                used to constrain the range of values to evaluate for each feature.
+            percentiles: lower and upper percentiles used to set the range to plot.
+            n_bins: the number of bins spanning the lower-upper percentile range.
+            categorical_features: a 0-based index of which features are categorical.
+            labels: list of band names to label the plots.
+            **kwargs: additional arguments to pass to `plt.subplots()`.
+
+        Returns:
+            fig, ax: matplotlib subplot figure and axes.
+        """
+        # skip categorical features for now
+        if categorical_features is None:
+            try:
+                categorical_features = self.transformer.categorical_ or [None]
+            except AttributeError:
+                categorical_features = [None]
+
+        bins, mean, stdv = self.partial_dependence_scores(
+            x, percentiles=percentiles, n_bins=n_bins, categorical_features=categorical_features
+        )
+
+        if labels is None:
+            try:
+                labels = x.columns.tolist()
+            except AttributeError:
+                labels = make_band_labels(x.shape[-1])
+
+        ncols = x.shape[1]
+        figx = int(np.ceil(np.sqrt(ncols)))
+        figy = int(np.ceil(ncols / figx))
+        fig, ax = plt.subplots(figx, figy, **kwargs)
+        ax = ax.flatten()
+
+        for idx in range(ncols):
+            ax[idx].fill_between(bins[idx], mean[idx] - stdv[idx], mean[idx] + stdv[idx], alpha=0.25)
+            ax[idx].plot(bins[idx], mean[idx])
+            ax[idx].set_title(labels[idx])
+
+        # turn off empty plots
+        for axi in ax:
+            if not axi.lines:
+                axi.set_visible(False)
 
-    # passed to __init__
-    feature_types: list = MaxentConfig.feature_types
-    tau: float = MaxentConfig.tau
-    clamp: bool = MaxentConfig.clamp
-    scorer: str = MaxentConfig.scorer
-    beta_multiplier: float = MaxentConfig.beta_multiplier
-    beta_hinge: float = MaxentConfig.beta_hinge
-    beta_lqp: float = MaxentConfig.beta_lqp
-    beta_threshold: float = MaxentConfig.beta_threshold
-    beta_categorical: float = MaxentConfig.beta_categorical
-    n_hinge_features: int = MaxentConfig.n_hinge_features
-    n_threshold_features: int = MaxentConfig.n_threshold_features
-    convergence_tolerance: float = MaxentConfig.tolerance
-    use_lambdas: str = MaxentConfig.use_lambdas
-    n_lambdas: str = MaxentConfig.n_lambdas
-    class_weights: Union[str, float] = None
-    n_cpus: int = NCPUS
-    use_sklearn: bool = False
-
-    # computed during model fitting
-    initialized_: bool = False
-    estimator: BaseEstimator = None
-    preprocessor: BaseEstimator = None
-    transformer: BaseEstimator = None
-    regularization_: np.ndarray = None
-    sample_weights_: np.ndarray = None
-    lambdas_: np.ndarray = None
-    beta_scores_: np.array = None
-    entropy_: float = 0.0
-    alpha_: float = 0.0
+        fig.tight_layout()
+
+        return fig, ax
+
+
+class MaxentModel(BaseEstimator, SDMMixin):
+    """Model estimator for Maxent-style species distribution models."""
 
     def __init__(
         self,
         feature_types: Union[list, str] = MaxentConfig.feature_types,
         tau: float = MaxentConfig.tau,
+        transform: float = MaxentConfig.transform,
         clamp: bool = MaxentConfig.clamp,
         scorer: str = MaxentConfig.scorer,
         beta_multiplier: float = MaxentConfig.beta_multiplier,
         beta_lqp: float = MaxentConfig.beta_lqp,
         beta_hinge: float = MaxentConfig.beta_hinge,
         beta_threshold: float = MaxentConfig.beta_lqp,
         beta_categorical: float = MaxentConfig.beta_categorical,
@@ -82,39 +272,43 @@
     ):
         """Create a maxent model object.
 
         Args:
             feature_types: maxent feature types to fit. must be in string "lqphta" or
                 list ["linear", "quadratic", "product", "hinge", "threshold", "auto"]
             tau: maxent prevalence value for scaling logistic output
+            transform: maxent model transformation type. select from
+                ["raw", "logistic", "cloglog"].
             clamp: set features to min/max range from training during prediction
             scorer: sklearn scoring function for model training
             beta_multiplier: scaler for all regularization parameters.
                 higher values drop more coeffiecients
             beta_lqp: linear, quadratic and product feature regularization scaler
             beta_hinge: hinge feature regularization scaler
             beta_threshold: threshold feature regularization scaler
             beta_categorical: categorical feature regularization scaler
             n_hinge_features: the number of hinge features to fit in feature transformation
             n_threshold_features: the number of thresholds to fit in feature transformation
             convergence_tolerance: model convergence tolerance level
             use_lambdas: guide for which model lambdas to select (either "best" or "last")
             n_lambdas: number of lamba values to fit models with
             class_weights: strategy for weighting presence samples.
-                pass "balance" to compute the ratio based on sample frequency
+                pass "balanced" to compute the ratio based on sample frequency
                 or pass a float for the presence:background weight ratio
-                the R `maxnet` package uses a value of 100 as default
+                the R `maxnet` package uses a value of 100 as default.
+                set to None to ignore.
             n_cpus: threads to use during model training
             use_sklearn: force using `sklearn` for fitting logistic regression.
                 turned off by default to use `glmnet` for fitting.
                 this feature was turned on to support Windows users
                 who install the package without a fortran compiler.
         """
-        self.feature_types = validate_feature_types(feature_types)
+        self.feature_types = feature_types
         self.tau = tau
+        self.transform = transform
         self.clamp = clamp
         self.scorer = scorer
         self.beta_multiplier = beta_multiplier
         self.beta_hinge = beta_hinge
         self.beta_lqp = beta_lqp
         self.beta_threshold = beta_threshold
         self.beta_categorical = beta_categorical
@@ -123,27 +317,42 @@
         self.convergence_tolerance = convergence_tolerance
         self.n_cpus = n_cpus
         self.use_lambdas = use_lambdas
         self.n_lambdas = n_lambdas
         self.class_weights = class_weights
         self.use_sklearn = use_sklearn
 
+        # computed during model fitting
+        self.initialized_ = False
+        self.estimator = None
+        self.preprocessor = None
+        self.transformer = None
+        self.regularization_ = None
+        self.lambdas_ = None
+        self.beta_scores_ = None
+        self.entropy_ = 0.0
+        self.alpha_ = 0.0
+
     def fit(
         self,
         x: ArrayLike,
         y: ArrayLike,
+        sample_weight: ArrayLike = None,
         categorical: List[int] = None,
         labels: list = None,
         preprocessor: BaseEstimator = None,
     ) -> None:
         """Trains a maxent model using a set of covariates and presence/background points.
 
         Args:
-            x: array-like of shape (n_samples, n_features) with covariate data
-            y: array-like of shape (n_samples,) with binary presence/background (1/0) values
+            x: array of shape (n_samples, n_features) with covariate data
+            y: array of shape (n_samples,) with binary presence/background (1/0) values
+            sample_weight: array of weights assigned to each sample with shape (n_samples,).
+                this is modified by the `class_weights` model parameter unless
+                you set `class_weights=None`.
             categorical: indices for which columns are categorical
             labels: covariate labels. ignored if x is a pandas DataFrame
             preprocessor: an `sklearn` transformer with a .transform() and/or
                 a .fit_transform() method. Some examples include a PCA() object or a
                 RobustScaler().
         """
         # clear state variables
@@ -158,87 +367,96 @@
             self.preprocessor = preprocessor
             try:
                 x = self.preprocessor.transform(x)
             except NotFittedError:
                 x = self.preprocessor.fit_transform(x)
 
         # fit the feature transformer
-        self.transformer = _features.MaxentFeatureTransformer(
+        self.feature_types = validate_feature_types(self.feature_types)
+        self.transformer = MaxentFeatureTransformer(
             feature_types=self.feature_types,
             clamp=self.clamp,
             n_hinge_features=self.n_hinge_features,
             n_threshold_features=self.n_threshold_features,
         )
         features = self.transformer.fit_transform(x, categorical=categorical, labels=labels)
         feature_labels = self.transformer.feature_names_
 
-        # compute sample weights
-        pbr = len(y) / y.sum() if self.class_weights == "balanced" else self.class_weights
-        self.sample_weights_ = _features.compute_weights(y, pbr=pbr)
+        # compute class weights
+        if self.class_weights is not None:
+            pbr = len(y) / y.sum() if self.class_weights == "balanced" else self.class_weights
+            class_weight = compute_weights(y, pbr=pbr)
+
+            # scale the sample weight
+            if sample_weight is None:
+                sample_weight = class_weight
+            else:
+                sample_weight *= class_weight
 
         # model fitting with sklearn
         if self.use_sklearn:
             C = estimate_C_from_betas(self.beta_multiplier)
             self.initialize_sklearn_model(C)
-            self.estimator.fit(features, y, sample_weight=self.sample_weights_)
+            self.estimator.fit(features, y, sample_weight=sample_weight)
             self.beta_scores_ = self.estimator.coef_[0]
 
         # model fitting with glmnet
         else:
             # set feature regularization parameters
-            self.regularization_ = _features.compute_regularization(
+            self.regularization_ = compute_regularization(
                 y,
                 features,
                 feature_labels=feature_labels,
                 beta_multiplier=self.beta_multiplier,
                 beta_lqp=self.beta_lqp,
                 beta_threshold=self.beta_threshold,
                 beta_hinge=self.beta_hinge,
                 beta_categorical=self.beta_categorical,
             )
 
             # get model lambda scores to initialize the glm
-            self.lambdas_ = _features.compute_lambdas(
-                y, self.sample_weights_, self.regularization_, n_lambdas=self.n_lambdas
-            )
+            self.lambdas_ = compute_lambdas(y, sample_weight, self.regularization_, n_lambdas=self.n_lambdas)
 
             # model fitting
             self.initialize_glmnet_model(lambdas=self.lambdas_)
             self.estimator.fit(
                 features,
                 y,
-                sample_weight=self.sample_weights_,
+                sample_weight=sample_weight,
                 relative_penalties=self.regularization_,
             )
 
             # get the beta values based on which lambda selection method to use
             if self.use_lambdas == "last":
                 self.beta_scores_ = self.estimator.coef_path_[0, :, -1]
             elif self.use_lambdas == "best":
                 self.beta_scores_ = self.estimator.coef_path_[0, :, self.estimator.lambda_max_inx_]
 
         # store initialization state
         self.initialized_ = True
 
         # apply maxent-specific transformations
-        raw = self.predict(x[y == 0], transform="raw")
+        class_transform = self.get_params()["transform"]
+        self.set_params(transform="raw")
+        raw = self.predict(x[y == 0])
+        self.set_params(transform=class_transform)
 
         # alpha is a normalizing constant that ensures that f1(z) integrates (sums) to 1
         self.alpha_ = maxent_alpha(raw)
 
         # the distance from f(z) is the relative entropy of f1(z) WRT f(z)
         self.entropy_ = maxent_entropy(raw)
 
-    def predict(self, x: ArrayLike, transform: str = "cloglog") -> ArrayLike:
-        """Applies a model to a set of covariates or features. Requires that a model has been fit.
+        return self
+
+    def predict(self, x: ArrayLike) -> ArrayLike:
+        """Apply a model to a set of covariates or features. Requires that a model has been fit.
 
         Args:
             x: array-like of shape (n_samples, n_features) with covariate data
-            transform: maxent model transformation type. select from
-                ["raw", "logistic", "cloglog"].
 
         Returns:
             predictions: array-like of shape (n_samples,) with model predictions
         """
         if not self.initialized_:
             raise NotFittedError("Model must be fit first")
 
@@ -246,50 +464,61 @@
         x = x if self.preprocessor is None else self.preprocessor.transform(x)
         features = x if self.transformer is None else self.transformer.transform(x)
 
         # apply the model
         engma = np.matmul(features, self.beta_scores_) + self.alpha_
 
         # scale based on the transform type
-        if transform == "raw":
+        if self.transform == "raw":
             return maxent_raw_transform(engma)
 
-        elif transform == "logistic":
+        elif self.transform == "logistic":
             return maxent_logistic_transform(engma, self.entropy_, self.tau)
 
-        elif transform == "cloglog":
+        elif self.transform == "cloglog":
             return maxent_cloglog_transform(engma, self.entropy_)
 
+    def predict_proba(self, x: ArrayLike) -> ArrayLike:
+        """Compute prediction probability scores for the 0/1 classes.
+
+        Args:
+            x: array-like of shape (n_samples, n_features) with covariate data
+
+        Returns:
+            predictions: array-like of shape (n_samples, 2) with model predictions
+        """
+        ypred = self.predict(x).reshape(-1, 1)
+        predictions = np.hstack((1 - ypred, ypred))
+
+        return predictions
+
     def fit_predict(
         self,
         x: ArrayLike,
         y: ArrayLike,
         categorical: list = None,
         labels: list = None,
         preprocessor: BaseEstimator = None,
-        transform: str = "cloglog",
     ) -> ArrayLike:
         """Trains and applies a model to x/y data.
 
         Args:
             x: array-like of shape (n_samples, n_features) with covariate data
             y: array-like of shape (n_samples,) with binary presence/background (1/0) values
             categorical: column indices indicating which columns are categorical
             labels: Covariate labels. Ignored if x is a pandas DataFrame
             preprocessor: an `sklearn` transformer with a .transform() and/or
                 a .fit_transform() method. Some examples include a PCA() object or a
                 RobustScaler().
-            transform: maxent model transformation type. select from
-                ["raw", "logistic", "cloglog"].
 
         Returns:
             predictions: Array-like of shape (n_samples,) with model predictions
         """
         self.fit(x, y, categorical=categorical, labels=labels, preprocessor=preprocessor)
-        predictions = self.predict(x, transform=transform)
+        predictions = self.predict(x)
 
         return predictions
 
     def initialize_glmnet_model(
         self,
         lambdas: np.array,
         alpha: float = 1,
@@ -327,102 +556,42 @@
             penalty="l1",
             solver="liblinear",
             tol=self.convergence_tolerance,
             max_iter=self.n_lambdas,
         )
 
 
-class NicheEnvelopeModel(BaseEstimator):
+class NicheEnvelopeModel(BaseEstimator, SDMMixin, FeaturesMixin):
     """Model estimator for niche envelope-style models."""
 
-    percentile_range: Tuple[float, float] = None
-    feature_mins_: np.ndarray = None
-    feature_maxs_: np.ndarray = None
-    categorical_estimator: BaseEstimator = None
-    categorical_: list = None
-    continuous_: list = None
-    categorical_pd_: list = None
-    continuous_pd_: list = None
-    in_categorical_: np.ndarray = None
-
-    def __init__(self, percentile_range: Tuple[float, float] = NicheEnvelopeConfig.percentile_range):
+    def __init__(
+        self,
+        percentile_range: Tuple[float, float] = NicheEnvelopeConfig.percentile_range,
+        overlay: str = NicheEnvelopeConfig.overlay,
+    ):
         """Create a niche envelope model estimator.
 
         Args:
             percentile_range: covariate values within this range are flagged as suitable habitat
                 using a narrow range like [10, 90] drops more areas from suitability maps
                 while [0, 100] creates an envelope around the full range of observed
                 covariates at all y==1 locations.
+            overlay: niche envelope overlap type.
+                select from ["average", "intersection", "union"]
         """
         self.percentile_range = percentile_range
-        self.categorical_estimator = _features.CategoricalTransformer()
-
-    def _format_covariate_data(self, x: ArrayLike) -> Tuple[np.array, np.array]:
-        """Reads input x data and formats it to consistent array dtypes.
-
-        Args:
-            x: array-like of shape (n_samples, n_features)
-
-        Returns:
-            (continuous, categorical) tuple of ndarrays with continuous and
-                categorical covariate data.
-        """
-        if isinstance(x, np.ndarray):
-            if self.categorical_ is None:
-                con = x
-                cat = None
-            else:
-                con = x[:, self.continuous_]
-                cat = x[:, self.categorical_]
-
-        elif isinstance(x, pd.DataFrame):
-            con = x[self.continuous_pd_].to_numpy()
-            if len(self.categorical_pd_) > 0:
-                cat = x[self.categorical_pd_].to_numpy()
-            else:
-                cat = None
-
-        else:
-            raise TypeError(f"Unsupported x dtype: {type(x)}. Must be pd.DataFrame or np.array")
-
-        return con, cat
-
-    def _format_labels_and_dtypes(self, x: ArrayLike, categorical: list = None, labels: list = None) -> None:
-        """Read input x data and lists of categorical data indices and band
-            labels to format and store this info for later indexing.
-
-        Args:
-            s: array-like of shape (n_samples, n_features)
-            categorical: indices indicating which x columns are categorical
-            labels: covariate column labels. ignored if x is a pandas DataFrame
-        """
-        if isinstance(x, np.ndarray):
-            nrows, ncols = x.shape
-            if categorical is None:
-                continuous = list(range(ncols))
-            else:
-                continuous = list(set(range(ncols)).difference(set(categorical)))
-            self.labels_ = labels or make_band_labels(ncols)
-            self.categorical_ = categorical
-            self.continuous_ = continuous
-
-        elif isinstance(x, pd.DataFrame):
-            x.drop(["geometry"], axis=1, errors="ignore", inplace=True)
-            self.labels_ = labels or list(x.columns)
-
-            # store both pandas and numpy indexing of these values
-            self.continuous_pd_ = list(x.select_dtypes(exclude="category").columns)
-            self.categorical_pd_ = list(x.select_dtypes(include="category").columns)
-
-            all_columns = list(x.columns)
-            self.continuous_ = [all_columns.index(item) for item in self.continuous_pd_ if item in all_columns]
-            if len(self.categorical_pd_) != 0:
-                self.categorical_ = [all_columns.index(item) for item in self.categorical_pd_ if item in all_columns]
-            else:
-                self.categorical_ = None
+        self.overlay = overlay
+        self.feature_mins_ = None
+        self.feature_maxs_ = None
+        self.categorical_estimator = None
+        self.categorical_ = None
+        self.continuous_ = None
+        self.categorical_pd_ = None
+        self.continuous_pd_ = None
+        self.in_categorical_ = None
 
     def fit(self, x: ArrayLike, y: ArrayLike, categorical: list = None, labels: list = None) -> None:
         """Fits a niche envelope model using a set of covariates and presence/background points.
 
         Args:
             x: array-like of shape (n_samples, n_features) with covariate data
             y: array-like of shape (n_samples,) with binary presence/background (1/0) values
@@ -436,29 +605,30 @@
 
         # estimate the feature range of the continuous data
         self.feature_mins_ = np.percentile(con[y == 1], self.percentile_range[0], axis=0)
         self.feature_maxs_ = np.percentile(con[y == 1], self.percentile_range[1], axis=0)
 
         # one-hot encode the categorical data and label the classes with
         if cat is not None:
+            self.categorical_estimator = CategoricalTransformer()
             ohe = self.categorical_estimator.fit_transform(cat)
             self.in_categorical_ = np.any(ohe[y == 1], axis=0)
 
-    def predict(self, x: ArrayLike, overlay: str = "average") -> np.ndarray:
+        return self
+
+    def predict(self, x: ArrayLike) -> np.ndarray:
         """Applies a model to a set of covariates or features. Requires that a model has been fit.
 
         Args:
             x: array-like of shape (n_samples, n_features) with covariate data
-            overlay: niche envelope overlap type.
-                select from ["average", "intersection", "union"]
 
         Returns:
             array-like of shape (n_samples,) with model predictions
         """
-        overlay = overlay.lower()
+        overlay = self.overlay.lower()
         overlay_options = ["average", "intersection", "union"]
         assert overlay in overlay_options, f"overlay must be one of {', '.join(overlay_options)}"
 
         # format the input data
         con, cat = self._format_covariate_data(x)
         nrows, ncols = x.shape
 
@@ -480,32 +650,113 @@
             ypred = np.all(in_range, axis=1).astype("uint8")
 
         elif overlay == "union":
             ypred = np.any(in_range, axis=1).astype("uint8")
 
         return ypred
 
-    def fit_predict(
-        self, x: ArrayLike, y: ArrayLike, categorical: list = None, labels: list = None, overlay: str = "average"
-    ) -> np.ndarray:
+    def predict_proba(self, x: ArrayLike) -> ArrayLike:
+        """Compute prediction probability scores for the 0/1 classes.
+
+        Args:
+            x: array-like of shape (n_samples, n_features) with covariate data
+
+        Returns:
+            predictions: array-like of shape (n_samples, 2) with model predictions
+        """
+        ypred = self.predict(x).reshape(-1, 1)
+        predictions = np.hstack((1 - ypred, ypred))
+
+        return predictions
+
+    def fit_predict(self, x: ArrayLike, y: ArrayLike, categorical: list = None, labels: list = None) -> np.ndarray:
         """Trains and applies a model to x/y data.
 
         Args:
             x: array-like of shape (n_samples, n_features) with covariate data
             y: array-like of shape (n_samples,) with binary presence/background (1/0) values
             categorical: column indices indicating which columns are categorical
             labels: Covariate labels. Ignored if x is a pandas DataFrame
-            overlay: maxent model transformation type.
-                select from ["average", "intersection", "union"]
 
         Returns:
             array-like of shape (n_samples,) with model predictions
         """
         self.fit(x, y, categorical=categorical, labels=labels)
-        return self.predict(x, overlay=overlay)
+        return self.predict(x)
+
+
+class EnsembleModel(BaseEstimator, SDMMixin):
+    """Barebones estimator for ensembling multiple model predictions."""
+
+    models: list = None
+    reducer: str = None
+
+    def __init__(self, models: List[BaseEstimator], reducer: str = EnsembleConfig.reducer):
+        """Create a model ensemble from a set of trained models.
+
+        Args:
+            models: iterable of models with `.predict()` and/or `.predict_proba()` methods
+            reducer: method for reducing/ensembling each model's predictions.
+                select from ['mean', 'median', 'mode']
+        """
+        self.models = models
+        self.reducer = reducer
+
+    def reduce(self, preds: List[np.ndarray]) -> np.ndarray:
+        """Reduce multiple model predictions into ensemble prediction/probability scores.
+
+        Args:
+            preds: list of model predictions from .predict() or .predict_proba()
+
+        Returns:
+            array-like of shape (n_samples, n_classes) with model predictions
+        """
+        reducer = self.reducer.lower()
+
+        if reducer == "mean":
+            reduced = np.nanmean(preds, axis=0)
+
+        elif reducer == "median":
+            reduced = np.nanmedian(preds, axis=0)
+
+        elif reducer == "mode":
+            try:
+                summary = scistats.mode(preds, axis=0, nan_policy="omit", keepdims=False)
+                reduced = summary.mode
+            except TypeError:
+                summary = scistats.mode(preds, axis=0, nan_policy="omit")
+                reduced = np.squeeze(summary.mode)
+
+        return reduced
+
+    def predict(self, x: ArrayLike) -> np.ndarray:
+        """Applies models to a set of covariates or features. Requires each model has been fit.
+
+        Args:
+            x: array-like of shape (n_samples, n_features) with covariate data
+
+        Returns:
+            array-like of shape (n_samples,) with model predictions
+        """
+        preds = [model.predict(x) for model in self.models]
+        ensemble = self.reduce(preds)
+        return ensemble
+
+    def predict_proba(self, x: ArrayLike) -> np.ndarray:
+        """Compute prediction probability scores for each class.
+
+        Args:
+            x: array-like of shape (n_samples, n_features) with covariate data
+
+        Returns:
+            array-like of shape (n_samples, n_classes) with model predictions
+        """
+        probas = [model.predict_proba(x) for model in self.models]
+        ensemble = self.reduce(probas)
+        return ensemble
 
 
 def maxent_alpha(raw: np.ndarray) -> float:
     """Compute the sum-to-one alpha maxent model parameter.
 
     Args:
         raw: uncalibrated maxent raw (exponential) model output
```

### Comparing `elapid-0.3.9/elapid/stats.py` & `elapid-1.0.1/elapid/stats.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-"""Utilities for calculating zonal statistics"""
+"""Utilities for calculating zonal stats and other transformations"""
 
 from typing import Callable, List
 
 import numpy as np
 from scipy import stats as scistats
 
+from elapid.types import ArrayLike
+
 
 class RasterStat:
     """Utility class to iterate over and apply reductions to multiband arrays"""
 
-    name: str = None
-    method: Callable = None
-    dtype: str = None
-    kwargs: dict = None
-
     def __init__(self, name: str, method: Callable, dtype: str = None, **kwargs):
         """Create a RasterStat object
 
         Args:
             name: the label to prepend to the output column
             method: function to reduce a 2d ndarray to an (nbands,) shape array
             dtype: the output array data type
@@ -83,19 +80,28 @@
 
 
 def raster_kurtosis(x):
     return scistats.kurtosis(x, axis=1, nan_policy="omit")
 
 
 def raster_mode(x):
-    summary = scistats.mode(x, axis=1, nan_policy="omit")
-    return summary.mode.flatten()
+    try:
+        summary = scistats.mode(x, axis=1, nan_policy="omit", keepdims=False)
+        mode = summary.mode
+    except TypeError:
+        summary = scistats.mode(x, axis=1, nan_policy="omit")
+        mode = summary.mode.flatten()
+
+    return mode
 
 
 def raster_percentile(x, pctile):
+    if isinstance(x, np.ma.masked_array):
+        valid = ~x.mask[0, ::]
+        x = np.array(x[:, valid])
     return np.nanpercentile(x, pctile, axis=1)
 
 
 def get_raster_stats_methods(
     mean: bool = True,
     min: bool = False,
     max: bool = False,
@@ -139,7 +145,25 @@
         methods.append(RasterStat(name="mode", method=raster_mode))
 
     if len(percentiles) > 0:
         for percentile in percentiles:
             methods.append(RasterStat(name=f"{percentile}pct", method=raster_percentile, pctile=percentile))
 
     return methods
+
+
+def normalize_sample_probabilities(values: ArrayLike) -> np.ndarray:
+    """Compute scaled probability scores for an array of samples.
+
+    These normalized probabilities sum to 1.0 and are designed to be used
+        as the `p` parameter for determining sample probabilities in
+        np.random.choice
+
+    Args:
+        values: numeric array to be treated as sample probabilities.
+            probabilities will be scaled linearly based on the input range.
+            setting `values = np.array([2, 1, 1])` returns (0.5, 0.25, 0.25)
+
+    Returns:
+        sample probabiility scores
+    """
+    return values / np.linalg.norm(values, ord=1)
```

### Comparing `elapid-0.3.9/elapid/types.py` & `elapid-1.0.1/elapid/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Custom maxent and typing data types."""
 from typing import Any, Union
 
+import geopandas as gpd
 import numpy as np
 import pandas as pd
 import pyproj
 
 # typing
 Number = Union[int, float]
 ArrayLike = Union[np.ndarray, pd.DataFrame]
 CRSType = Union[pyproj.CRS, str]
+Vector = Union[gpd.GeoSeries, gpd.GeoDataFrame]
 
 
 # maxent feature transformations
 def get_feature_types(return_string: bool = False) -> Union[list, str]:
     feature_types = "lqpht" if return_string else ["linear", "quadratic", "product", "hinge", "threshold"]
     return feature_types
```

### Comparing `elapid-0.3.9/elapid/utils.py` & `elapid-1.0.1/elapid/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """Backend helper and convenience functions."""
 
 import gzip
 import multiprocessing as mp
 import os
 import pickle
 import sys
-from typing import Any, Callable, Dict, Iterable, Tuple, Union
+from typing import Any, Callable, Dict, Iterable, List, Tuple, Union
+from urllib import request
 
+import geopandas as gpd
 import numpy as np
 import pandas as pd
 import rasterio as rio
 
 from elapid.types import Number
 
 NCPUS = mp.cpu_count()
+tqdm_opts = {"bar_format": "{l_bar}{bar:30}{r_bar}{bar:-30b}"}
 
 
 class NoDataException(Exception):
     pass
 
 
 def repeat_array(x: np.array, length: int = 1, axis: int = 0) -> np.ndarray:
@@ -30,36 +33,86 @@
 
     Returns:
         An n+1 dimensional numpy array
     """
     return np.expand_dims(x, axis=axis).repeat(length, axis=axis)
 
 
-def load_sample_data(name: str = "bradypus") -> Tuple[pd.DataFrame, pd.DataFrame]:
+def load_sample_data(name: str = "ariolimax", drop_geometry: bool = False) -> Tuple[pd.DataFrame, pd.DataFrame]:
     """Loads example species presence/background and covariate data.
 
     Args:
-        name: the sample dataset to load. options currently include ["bradypus"], from the R 'maxnet' package
+        name: the sample dataset to load. options include:
+            "ariolimax" button's banana slug dataset
+            "bradypus" from the R 'maxnet' package
 
     Returns:
         (x, y): a tuple of dataframes containing covariate and response data, respectively
     """
-    assert name.lower() in ["bradypus"], "Invalid sample data requested"
+    name = str.lower(name)
+    assert name in ["bradypus", "ariolimax"], "Invalid sample data requested"
 
     package_path = os.path.realpath(__file__)
     package_dir = os.path.dirname(package_path)
 
-    if name.lower() == "bradypus":
-
+    if name == "bradypus":
         file_path = os.path.join(package_dir, "data", "bradypus.csv.gz")
+        assert os.path.exists(file_path), "sample data missing from install path."
         df = pd.read_csv(file_path, compression="gzip").astype("int64")
         y = df["presence"].astype("int8")
         x = df.drop(columns=["presence"]).astype({"ecoreg": "category"})
         return x, y
 
+    if name == "ariolimax":
+        file_path = os.path.join(package_dir, "data", "ariolimax.gpkg")
+        assert os.path.exists(file_path), "sample data missing from install path."
+        df = gpd.read_file(file_path)
+        columns_to_drop = ["presence"]
+        if drop_geometry:
+            columns_to_drop.append("geometry")
+        x = df.drop(columns=columns_to_drop)
+        y = df["presence"].astype("int8")
+        return x, y
+
+
+def download_sample_data(dir: str, name: str = "ariolimax", quiet: bool = False) -> None:
+    """Downloads sample raster and vector files from a web server.
+
+    Args:
+        dir: the directory to download the data to
+        name: the sample dataset to download. options include:
+            "ariolimax" button's banana slug dataset
+        quiet: disable the progress bar
+
+    Returns:
+        None. Downloads files to `dir`
+    """
+    name = str.lower(name)
+    https = "https://earth-chris.github.io/images/research"
+
+    if name == "ariolimax":
+        fnames = [
+            "ariolimax-ca.gpkg",
+            "ca-cloudcover-mean.tif",
+            "ca-cloudcover-stdv.tif",
+            "ca-leafareaindex-mean.tif",
+            "ca-leafareaindex-stdv.tif",
+            "ca-surfacetemp-mean.tif",
+            "ca-surfacetemp-stdv.tif",
+        ]
+
+    try:
+        os.mkdir(dir)
+    except FileExistsError:
+        pass
+
+    tqdm = get_tqdm()
+    for fname in tqdm(fnames, disable=quiet, **tqdm_opts):
+        request.urlretrieve(f"{https}/{fname}", os.path.join(dir, fname))
+
 
 def save_object(obj: object, path: str, compress: bool = True) -> None:
     """Writes a python object to disk for later access.
 
     Args:
         obj: a python object or variable to be saved (e.g., a MaxentModel() instance)
         path: the output file path
@@ -251,23 +304,43 @@
     """
     n_zeros = n_digits(n_bands)
     labels = ["b{band_number:0{n_zeros}d}".format(band_number=i + 1, n_zeros=n_zeros) for i in range(n_bands)]
 
     return labels
 
 
-def format_band_labels(raster_paths: list, labels: list = None):
-    """Verifies whether a list of band labels matches the band count,
-        or creates labels when none are passed.
+def format_band_labels(raster_paths: list, labels: List[str] = None):
+    """Verify the number of labels matches the band count, create labels if none passed.
 
     Args:
-        raster_paths:
+        raster_paths: count the total number of bands in these rasters.
+        labels: a list of band labels.
+
+    Returns:
+        labels: creates default band labels if none are passed.
     """
     n_bands = count_raster_bands(raster_paths)
 
     if labels is None:
         labels = make_band_labels(n_bands)
 
     n_labels = len(labels)
     assert n_labels == n_bands, f"number of band labels ({n_labels}) != n_bands ({n_bands})"
 
-    return labels
+    return labels.copy()
+
+
+def square_factor(n: int) -> tuple:
+    """Compute a square form-factor to fit `n` items.
+
+    Args:
+        n: the number of items to fit into a square.
+
+    Returns:
+        (x, y) tuple of the square dimensions.
+    """
+    val = np.ceil(np.sqrt(n))
+    val2 = int(n / val)
+    while val2 * val != float(n):
+        val -= 1
+        val2 = int(n / val)
+    return int(val), int(val2)
```

### Comparing `elapid-0.3.9/setup.py` & `elapid-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,18 +4,14 @@
 from setuptools import setup
 
 this_dir, this_path = os.path.split(os.path.abspath(__file__))
 version = open(os.path.join(this_dir, "elapid", "__version__.py")).read().strip('"\n')
 long_description = open(os.path.join(this_dir, "README.md"), "r", encoding="utf-8").read()
 requirements = open(os.path.join(this_dir, "requirements.txt"), "r", encoding="utf-8").read().strip().split()
 
-# remove glmnet requirement for windows installs
-if platform.system() != "Linux":
-    [requirements.pop(idx) for idx, pkg in enumerate(requirements) if "glmnet" in pkg]
-
 setup_args = {
     "name": "elapid",
     "version": version,
     "url": "https://elapid.org",
     "license": "MIT",
     "author": "Christopher Anderson",
     "author_email": "cbanders@stanford.edu",
@@ -28,15 +24,19 @@
         "conservation",
         "SDM",
         "species distribution modeling",
         "maxent",
     ],
     "packages": ["elapid"],
     "include_package_data": True,
+    "data_files": [("elapid", ["elapid/data/bradypus.csv.gz"])],
     "install_requires": requirements,
+    "extras_require": {
+        "glmnet": "glmnet",
+    },
     "python_requires": ">=3.7.0",
     "platforms": "any",
     "classifiers": [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```


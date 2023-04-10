# Comparing `tmp/ts2vg-1.2.1.tar.gz` & `tmp/ts2vg-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts2vg-1.2.1.tar", last modified: Thu Feb  9 23:09:35 2023, max compression
+gzip compressed data, was "ts2vg-1.2.2.tar", last modified: Mon Apr 10 18:20:30 2023, max compression
```

## Comparing `ts2vg-1.2.1.tar` & `ts2vg-1.2.2.tar`

### file list

```diff
@@ -1,39 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 23:09:35.302219 ts2vg-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-09 23:09:12.000000 ts2vg-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-02-09 23:09:35.302219 ts2vg-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-02-09 23:09:12.000000 ts2vg-1.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-02-09 23:09:12.000000 ts2vg-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-02-09 23:09:35.302219 ts2vg-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-02-09 23:09:12.000000 ts2vg-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 23:09:35.294219 ts2vg-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-02-09 23:09:12.000000 ts2vg-1.2.1/tests/test_horizontal.py
--rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-02-09 23:09:12.000000 ts2vg-1.2.1/tests/test_horizontal_penetrable.py
--rw-r--r--   0 runner    (1001) docker     (123)    13804 2023-02-09 23:09:12.000000 ts2vg-1.2.1/tests/test_natural.py
--rw-r--r--   0 runner    (1001) docker     (123)    19767 2023-02-09 23:09:12.000000 ts2vg-1.2.1/tests/test_natural_penetrable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-02-09 23:09:12.000000 ts2vg-1.2.1/tests/test_parametric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 23:09:35.294219 ts2vg-1.2.1/ts2vg/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-02-09 23:09:12.000000 ts2vg-1.2.1/ts2vg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-09 23:09:12.000000 ts2vg-1.2.1/ts2vg/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-02-09 23:09:12.000000 ts2vg-1.2.1/ts2vg/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 23:09:35.302219 ts2vg-1.2.1/ts2vg/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 23:09:12.000000 ts2vg-1.2.1/ts2vg/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   878536 2023-02-09 23:09:29.000000 ts2vg-1.2.1/ts2vg/graph/_base.c
--rw-r--r--   0 runner    (1001) docker     (123)   968676 2023-02-09 23:09:30.000000 ts2vg-1.2.1/ts2vg/graph/_horizontal.c
--rw-r--r--   0 runner    (1001) docker     (123)   977489 2023-02-09 23:09:32.000000 ts2vg-1.2.1/ts2vg/graph/_horizontal_penetrable.c
--rw-r--r--   0 runner    (1001) docker     (123)   974801 2023-02-09 23:09:33.000000 ts2vg-1.2.1/ts2vg/graph/_natural.c
--rw-r--r--   0 runner    (1001) docker     (123)   979882 2023-02-09 23:09:34.000000 ts2vg-1.2.1/ts2vg/graph/_natural_penetrable.c
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-02-09 23:09:12.000000 ts2vg-1.2.1/ts2vg/graph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-02-09 23:09:12.000000 ts2vg-1.2.1/ts2vg/graph/horizontal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-02-09 23:09:12.000000 ts2vg-1.2.1/ts2vg/graph/natural.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-02-09 23:09:12.000000 ts2vg-1.2.1/ts2vg/graph/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 23:09:35.302219 ts2vg-1.2.1/ts2vg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 23:09:12.000000 ts2vg-1.2.1/ts2vg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   166788 2023-02-09 23:09:34.000000 ts2vg-1.2.1/ts2vg/utils/pairqueue.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 23:09:35.294219 ts2vg-1.2.1/ts2vg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-02-09 23:09:35.000000 ts2vg-1.2.1/ts2vg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-02-09 23:09:35.000000 ts2vg-1.2.1/ts2vg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 23:09:35.000000 ts2vg-1.2.1/ts2vg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-09 23:09:35.000000 ts2vg-1.2.1/ts2vg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 23:09:34.000000 ts2vg-1.2.1/ts2vg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-09 23:09:35.000000 ts2vg-1.2.1/ts2vg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-09 23:09:35.000000 ts2vg-1.2.1/ts2vg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:20:30.906321 ts2vg-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-10 18:20:09.000000 ts2vg-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-04-10 18:20:30.906321 ts2vg-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-04-10 18:20:09.000000 ts2vg-1.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-10 18:20:09.000000 ts2vg-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-10 18:20:30.906321 ts2vg-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-10 18:20:09.000000 ts2vg-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:20:30.898321 ts2vg-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10053 2023-04-10 18:20:09.000000 ts2vg-1.2.2/tests/test_horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21022 2023-04-10 18:20:09.000000 ts2vg-1.2.2/tests/test_horizontal_penetrable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-04-10 18:20:09.000000 ts2vg-1.2.2/tests/test_natural.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-04-10 18:20:09.000000 ts2vg-1.2.2/tests/test_natural_penetrable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-10 18:20:09.000000 ts2vg-1.2.2/tests/test_parametric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:20:30.898321 ts2vg-1.2.2/ts2vg/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-10 18:20:09.000000 ts2vg-1.2.2/ts2vg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 18:20:09.000000 ts2vg-1.2.2/ts2vg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-04-10 18:20:09.000000 ts2vg-1.2.2/ts2vg/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:20:30.906321 ts2vg-1.2.2/ts2vg/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 18:20:09.000000 ts2vg-1.2.2/ts2vg/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   880190 2023-04-10 18:20:25.000000 ts2vg-1.2.2/ts2vg/graph/_base.c
+-rw-r--r--   0 runner    (1001) docker     (123)   968528 2023-04-10 18:20:26.000000 ts2vg-1.2.2/ts2vg/graph/_horizontal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   978801 2023-04-10 18:20:27.000000 ts2vg-1.2.2/ts2vg/graph/_horizontal_penetrable.c
+-rw-r--r--   0 runner    (1001) docker     (123)   974624 2023-04-10 18:20:28.000000 ts2vg-1.2.2/ts2vg/graph/_natural.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   981194 2023-04-10 18:20:30.000000 ts2vg-1.2.2/ts2vg/graph/_natural_penetrable.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13856 2023-04-10 18:20:09.000000 ts2vg-1.2.2/ts2vg/graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-10 18:20:09.000000 ts2vg-1.2.2/ts2vg/graph/horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-10 18:20:09.000000 ts2vg-1.2.2/ts2vg/graph/natural.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-10 18:20:09.000000 ts2vg-1.2.2/ts2vg/graph/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:20:30.898321 ts2vg-1.2.2/ts2vg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-04-10 18:20:30.000000 ts2vg-1.2.2/ts2vg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-10 18:20:30.000000 ts2vg-1.2.2/ts2vg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:20:30.000000 ts2vg-1.2.2/ts2vg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-10 18:20:30.000000 ts2vg-1.2.2/ts2vg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:20:30.000000 ts2vg-1.2.2/ts2vg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 18:20:30.000000 ts2vg-1.2.2/ts2vg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 18:20:30.000000 ts2vg-1.2.2/ts2vg.egg-info/top_level.txt
```

### Comparing `ts2vg-1.2.1/LICENSE` & `ts2vg-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ts2vg-1.2.1/PKG-INFO` & `ts2vg-1.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts2vg
-Version: 1.2.1
+Version: 1.2.2
 Summary: Build visibility graphs from time series data.
 Home-page: https://github.com/CarlosBergillos/ts2vg
 Author: Carlos Bergillos
 Author-email: c.bergillos.v@gmail.com
 License: MIT
 Project-URL: Documentation, https://carlosbergillos.github.io/ts2vg
 Project-URL: Source Code, https://github.com/CarlosBergillos/ts2vg
@@ -59,30 +59,22 @@
    :target: https://pypi.python.org/pypi/ts2vg
 
 |cover|
 
 |
 
 The Python |ts2vg| package provides high-performance algorithm
-implementations to build visibility graphs from time series data.
+implementations to build visibility graphs from time series data,
+as first introduced by Lucas Lacasa et al. in 2008 [#Lacasa2008]_.
 
 The visibility graphs and some of their properties (e.g. degree
 distributions) are computed quickly and efficiently even for time
 series with millions of observations.
-
-The visibility graphs are provided according to the
-mathematical definitions presented in:
-
--  Lucas Lacasa et al., "*From time series to complex networks: The visibility graph*", 2008.
--  Lucas Lacasa et al., "*Horizontal visibility graphs: exact results for random time series*", 2009.
-
-An efficient divide-and-conquer algorithm is used to compute the graphs,
-as described in:
-
--  Xin Lan et al., "*Fast transformation from time series to visibility graphs*", 2015.
+An efficient divide-and-conquer algorithm is used to compute the graphs
+whenever possible [#Lan2015]_.
 
    
 Installation
 ------------
 
 The latest released |ts2vg| version is available at the `Python Package Index (PyPI)`_
 and can be easily installed by running:
@@ -96,24 +88,24 @@
 
 Supported graph types
 ---------------------
 
 Root graph types
 ~~~~~~~~~~~~~~~~
 
-- Natural Visibility Graphs (NVG) (``ts2vg.NaturalVG``)
-- Horizontal Visibility Graphs (HVG) (``ts2vg.HorizontalVG``)
+- Natural Visibility Graphs (NVG) [#Lacasa2008]_ (``ts2vg.NaturalVG``)
+- Horizontal Visibility Graphs (HVG) [#Lacasa2009]_ (``ts2vg.HorizontalVG``)
 
 Available variations
 ~~~~~~~~~~~~~~~~~~~~
 
 - Weighted Visibility Graphs (via the ``weighted`` parameter)
 - Directed Visibility Graphs (via the ``directed`` parameter)
-- Parametric Visibility Graphs (via the ``min_weight`` and ``max_weight`` parameters)
-- Limited Penetrable Visibility Graphs (LPVG) (via the ``penetrable_limit`` parameter)
+- Parametric Visibility Graphs [#Bezsudnov2014]_ (via the ``min_weight`` and ``max_weight`` parameters)
+- Limited Penetrable Visibility Graphs (LPVG) [#Zhou2012]_ [#Xuan2021]_ (via the ``penetrable_limit`` parameter)
 
 .. - Dual Perspective Visibility Graph [*planned, not implemented yet*]
 
 Note that multiple graph variations can be combined and used simultaneously.
 
 
 Documentation
@@ -121,96 +113,81 @@
 
 Usage and reference documentation for |ts2vg| can be found at `carlosbergillos.github.io/ts2vg`_.
 
 
 Basic usage
 -----------
 
-Visibility graph
-~~~~~~~~~~~~~~~~
-
-To build a visibility graph:
+To build a visibility graph from a time series do:
 
 .. code:: python
 
    from ts2vg import NaturalVG
 
    ts = [1.0, 0.5, 0.3, 0.7, 1.0, 0.5, 0.3, 0.8]
 
-   g = NaturalVG()
-   g.build(ts)
+   vg = NaturalVG()
+   vg.build(ts)
+
+   edges = vg.edges
 
-   edges = g.edges
 
 The time series passed (``ts``) can be any one-dimensional iterable, such as a list or a ``numpy`` 1D array.
 
 By default, the input observations are assumed to be equally spaced in time.
 Alternatively, a second 1D iterable (``xs``) can be provided for unevenly spaced time series.
 
 
-Horizontal visibility graph
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
 Horizontal visibility graphs can be obtained in a very similar way:
 
 .. code:: python
 
    from ts2vg import HorizontalVG
 
    ts = [1.0, 0.5, 0.3, 0.7, 1.0, 0.5, 0.3, 0.8]
 
-   g = HorizontalVG()
-   g.build(ts)
-
-   edges = g.edges
+   vg = HorizontalVG()
+   vg.build(ts)
 
+   edges = vg.edges
 
-Degree distribution
-~~~~~~~~~~~~~~~~~~~
 
 If we are only interested in the degree distribution of the visibility graph
 we can pass ``only_degrees=True`` to the ``build`` method.
 This will be more efficient in time and memory than storing the whole graph.
 
 .. code:: python
 
-   g = NaturalVG()
-   g.build(ts, only_degrees=True)
+   vg = NaturalVG()
+   vg.build(ts, only_degrees=True)
 
-   ks, ps = g.degree_distribution
+   ks, ps = vg.degree_distribution
 
 
-Directed visibility graph
-~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Directed graphs can be obtained by using the ``directed`` parameter.
-See the reference documentation for the different available options.
+Directed graphs can be obtained by using the ``directed`` parameter
+and weighted graphs can be obtained by using the ``weighted`` parameter:
 
 .. code:: python
 
-   g = NaturalVG(directed='left_to_right')
-   g.build(ts)
-
+   vg1 = NaturalVG(directed="left_to_right")
+   vg1.build(ts)
 
-Weighted visibility graph
-~~~~~~~~~~~~~~~~~~~~~~~~~
+   vg2 = NaturalVG(weighted="distance")
+   vg2.build(ts)
 
-Weighted graphs can be obtained by using the ``weighted`` parameter.
-See the reference documentation for the different available options.
-
-.. code:: python
+   vg3 = NaturalVG(directed="left_to_right", weighted="distance")
+   vg3.build(ts)
 
-   g = NaturalVG(weighted='distance')
-   g.build(ts)
+   vg4 = HorizontalVG(directed="left_to_right", weighted="h_distance")
+   vg4.build(ts)
 
-|
 
 .. **For more information and options see:** :ref:`Examples` and :ref:`API Reference`.
 
-**For more information and options see:** `Examples`_ and `API Reference`_.
+For more information and options see: `Examples`_ and `API Reference`_.
 
 
 Interoperability with other libraries
 -------------------------------------
 
 The graphs obtained can be easily converted to graph objects
 from other common Python graph libraries such as `igraph`_, `NetworkX`_ and `SNAP`_
@@ -226,18 +203,18 @@
 -  ``as_networkx()``
 -  ``as_snap()``
 
 For example:
 
 .. code:: python
 
-   g = NaturalVG()
-   g.build(ts)
+   vg = NaturalVG()
+   vg.build(ts)
    
-   nx_g = g.as_networkx()
+   g = vg.as_networkx()
 
 
 Command line interface
 ----------------------
 
 |ts2vg| can also be used as a command line program directly from the console:
 
@@ -269,7 +246,18 @@
 .. _Python Package Index (PyPI): https://pypi.org/project/ts2vg
 .. _igraph: https://igraph.org/python/
 .. _NetworkX: https://networkx.github.io/
 .. _SNAP: https://snap.stanford.edu/snappy/
 .. _on GitHub: https://github.com/CarlosBergillos/ts2vg
 .. _MIT License: https://github.com/CarlosBergillos/ts2vg/blob/main/LICENSE
 .. _carlosbergillos.github.io/ts2vg: https://carlosbergillos.github.io/ts2vg/
+
+
+References
+----------
+
+.. [#Lacasa2008] Lucas Lacasa et al., "*From time series to complex networks: The visibility graph*", 2008.
+.. [#Lacasa2009] Lucas Lacasa et al., "*Horizontal visibility graphs: exact results for random time series*", 2009.
+.. [#Lan2015] Xin Lan et al., "*Fast transformation from time series to visibility graphs*", 2015.
+.. [#Zhou2012] T.T Zhou et al., "*Limited penetrable visibility graph for establishing complex network from time series*", 2012.
+.. [#Bezsudnov2014] I.V. Bezsudnov et al., "*From the time series to the complex networks: The parametric natural visibility graph*", 2014
+.. [#Xuan2021] Qi Xuan et al., "*CLPVG: Circular limited penetrable visibility graph as a new network model for time series*", 2021
```

### Comparing `ts2vg-1.2.1/README.rst` & `ts2vg-1.2.2/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -28,30 +28,22 @@
    :target: https://pypi.python.org/pypi/ts2vg
 
 |cover|
 
 |
 
 The Python |ts2vg| package provides high-performance algorithm
-implementations to build visibility graphs from time series data.
+implementations to build visibility graphs from time series data,
+as first introduced by Lucas Lacasa et al. in 2008 [#Lacasa2008]_.
 
 The visibility graphs and some of their properties (e.g. degree
 distributions) are computed quickly and efficiently even for time
 series with millions of observations.
-
-The visibility graphs are provided according to the
-mathematical definitions presented in:
-
--  Lucas Lacasa et al., "*From time series to complex networks: The visibility graph*", 2008.
--  Lucas Lacasa et al., "*Horizontal visibility graphs: exact results for random time series*", 2009.
-
-An efficient divide-and-conquer algorithm is used to compute the graphs,
-as described in:
-
--  Xin Lan et al., "*Fast transformation from time series to visibility graphs*", 2015.
+An efficient divide-and-conquer algorithm is used to compute the graphs
+whenever possible [#Lan2015]_.
 
    
 Installation
 ------------
 
 The latest released |ts2vg| version is available at the `Python Package Index (PyPI)`_
 and can be easily installed by running:
@@ -65,24 +57,24 @@
 
 Supported graph types
 ---------------------
 
 Root graph types
 ~~~~~~~~~~~~~~~~
 
-- Natural Visibility Graphs (NVG) (``ts2vg.NaturalVG``)
-- Horizontal Visibility Graphs (HVG) (``ts2vg.HorizontalVG``)
+- Natural Visibility Graphs (NVG) [#Lacasa2008]_ (``ts2vg.NaturalVG``)
+- Horizontal Visibility Graphs (HVG) [#Lacasa2009]_ (``ts2vg.HorizontalVG``)
 
 Available variations
 ~~~~~~~~~~~~~~~~~~~~
 
 - Weighted Visibility Graphs (via the ``weighted`` parameter)
 - Directed Visibility Graphs (via the ``directed`` parameter)
-- Parametric Visibility Graphs (via the ``min_weight`` and ``max_weight`` parameters)
-- Limited Penetrable Visibility Graphs (LPVG) (via the ``penetrable_limit`` parameter)
+- Parametric Visibility Graphs [#Bezsudnov2014]_ (via the ``min_weight`` and ``max_weight`` parameters)
+- Limited Penetrable Visibility Graphs (LPVG) [#Zhou2012]_ [#Xuan2021]_ (via the ``penetrable_limit`` parameter)
 
 .. - Dual Perspective Visibility Graph [*planned, not implemented yet*]
 
 Note that multiple graph variations can be combined and used simultaneously.
 
 
 Documentation
@@ -90,96 +82,81 @@
 
 Usage and reference documentation for |ts2vg| can be found at `carlosbergillos.github.io/ts2vg`_.
 
 
 Basic usage
 -----------
 
-Visibility graph
-~~~~~~~~~~~~~~~~
-
-To build a visibility graph:
+To build a visibility graph from a time series do:
 
 .. code:: python
 
    from ts2vg import NaturalVG
 
    ts = [1.0, 0.5, 0.3, 0.7, 1.0, 0.5, 0.3, 0.8]
 
-   g = NaturalVG()
-   g.build(ts)
+   vg = NaturalVG()
+   vg.build(ts)
+
+   edges = vg.edges
 
-   edges = g.edges
 
 The time series passed (``ts``) can be any one-dimensional iterable, such as a list or a ``numpy`` 1D array.
 
 By default, the input observations are assumed to be equally spaced in time.
 Alternatively, a second 1D iterable (``xs``) can be provided for unevenly spaced time series.
 
 
-Horizontal visibility graph
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
 Horizontal visibility graphs can be obtained in a very similar way:
 
 .. code:: python
 
    from ts2vg import HorizontalVG
 
    ts = [1.0, 0.5, 0.3, 0.7, 1.0, 0.5, 0.3, 0.8]
 
-   g = HorizontalVG()
-   g.build(ts)
-
-   edges = g.edges
+   vg = HorizontalVG()
+   vg.build(ts)
 
+   edges = vg.edges
 
-Degree distribution
-~~~~~~~~~~~~~~~~~~~
 
 If we are only interested in the degree distribution of the visibility graph
 we can pass ``only_degrees=True`` to the ``build`` method.
 This will be more efficient in time and memory than storing the whole graph.
 
 .. code:: python
 
-   g = NaturalVG()
-   g.build(ts, only_degrees=True)
+   vg = NaturalVG()
+   vg.build(ts, only_degrees=True)
 
-   ks, ps = g.degree_distribution
+   ks, ps = vg.degree_distribution
 
 
-Directed visibility graph
-~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Directed graphs can be obtained by using the ``directed`` parameter.
-See the reference documentation for the different available options.
+Directed graphs can be obtained by using the ``directed`` parameter
+and weighted graphs can be obtained by using the ``weighted`` parameter:
 
 .. code:: python
 
-   g = NaturalVG(directed='left_to_right')
-   g.build(ts)
-
+   vg1 = NaturalVG(directed="left_to_right")
+   vg1.build(ts)
 
-Weighted visibility graph
-~~~~~~~~~~~~~~~~~~~~~~~~~
+   vg2 = NaturalVG(weighted="distance")
+   vg2.build(ts)
 
-Weighted graphs can be obtained by using the ``weighted`` parameter.
-See the reference documentation for the different available options.
-
-.. code:: python
+   vg3 = NaturalVG(directed="left_to_right", weighted="distance")
+   vg3.build(ts)
 
-   g = NaturalVG(weighted='distance')
-   g.build(ts)
+   vg4 = HorizontalVG(directed="left_to_right", weighted="h_distance")
+   vg4.build(ts)
 
-|
 
 .. **For more information and options see:** :ref:`Examples` and :ref:`API Reference`.
 
-**For more information and options see:** `Examples`_ and `API Reference`_.
+For more information and options see: `Examples`_ and `API Reference`_.
 
 
 Interoperability with other libraries
 -------------------------------------
 
 The graphs obtained can be easily converted to graph objects
 from other common Python graph libraries such as `igraph`_, `NetworkX`_ and `SNAP`_
@@ -195,18 +172,18 @@
 -  ``as_networkx()``
 -  ``as_snap()``
 
 For example:
 
 .. code:: python
 
-   g = NaturalVG()
-   g.build(ts)
+   vg = NaturalVG()
+   vg.build(ts)
    
-   nx_g = g.as_networkx()
+   g = vg.as_networkx()
 
 
 Command line interface
 ----------------------
 
 |ts2vg| can also be used as a command line program directly from the console:
 
@@ -238,7 +215,18 @@
 .. _Python Package Index (PyPI): https://pypi.org/project/ts2vg
 .. _igraph: https://igraph.org/python/
 .. _NetworkX: https://networkx.github.io/
 .. _SNAP: https://snap.stanford.edu/snappy/
 .. _on GitHub: https://github.com/CarlosBergillos/ts2vg
 .. _MIT License: https://github.com/CarlosBergillos/ts2vg/blob/main/LICENSE
 .. _carlosbergillos.github.io/ts2vg: https://carlosbergillos.github.io/ts2vg/
+
+
+References
+----------
+
+.. [#Lacasa2008] Lucas Lacasa et al., "*From time series to complex networks: The visibility graph*", 2008.
+.. [#Lacasa2009] Lucas Lacasa et al., "*Horizontal visibility graphs: exact results for random time series*", 2009.
+.. [#Lan2015] Xin Lan et al., "*Fast transformation from time series to visibility graphs*", 2015.
+.. [#Zhou2012] T.T Zhou et al., "*Limited penetrable visibility graph for establishing complex network from time series*", 2012.
+.. [#Bezsudnov2014] I.V. Bezsudnov et al., "*From the time series to the complex networks: The parametric natural visibility graph*", 2014
+.. [#Xuan2021] Qi Xuan et al., "*CLPVG: Circular limited penetrable visibility graph as a new network model for time series*", 2021
```

### Comparing `ts2vg-1.2.1/pyproject.toml` & `ts2vg-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ts2vg-1.2.1/setup.cfg` & `ts2vg-1.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ts2vg-1.2.1/setup.py` & `ts2vg-1.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 
 def main():
     include_dirs = [get_np_include()]
     define_macros = [("NPY_NO_DEPRECATED_API", "NPY_1_7_API_VERSION")]
 
     # fmt: off
     extensions = [
-        Extension('ts2vg.utils.pairqueue',
-                  [f'ts2vg/utils/pairqueue.pyx']),
-
         Extension('ts2vg.graph._base',
                   [f'ts2vg/graph/_base.pyx'],
                   include_dirs=include_dirs,
                   define_macros=define_macros),
 
         Extension('ts2vg.graph._natural',
                   [f'ts2vg/graph/_natural.pyx'],
```

### Comparing `ts2vg-1.2.1/tests/test_horizontal.py` & `ts2vg-1.2.2/tests/test_horizontal.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from math import atan, sqrt
 
 import numpy as np
 import pytest
 from pytest import approx
 
+from fixtures import *
 import ts2vg
-from fixtures import empty_ts, flat_ts, sample_ts, sample_ts_2
+from naive_implementations import horizontal_visibility_graph as naive_hvg
 
 
 def test_basic(sample_ts):
     out_got = ts2vg.HorizontalVG().build(sample_ts).edges
 
     out_truth = [
         (0, 1),
@@ -40,14 +41,36 @@
         (7, 8),
         (8, 9),
     ]
 
     assert sorted(sorted(e) for e in out_got) == sorted(sorted(e) for e in out_truth)
 
 
+def test_white_noise(white_noise_ts):
+    ts = white_noise_ts
+    xs = list(range(len(ts)))
+
+    out_got = ts2vg.HorizontalVG().build(ts, xs).edges
+
+    out_truth = naive_hvg(ts, xs)
+
+    assert sorted(sorted(e) for e in out_got) == sorted(sorted(e) for e in out_truth)
+
+
+def test_brownian_motion_ts(brownian_motion_ts):
+    ts = brownian_motion_ts
+    xs = list(range(len(ts)))
+
+    out_got = ts2vg.HorizontalVG().build(ts, xs).edges
+
+    out_truth = naive_hvg(ts, xs)
+
+    assert sorted(sorted(e) for e in out_got) == sorted(sorted(e) for e in out_truth)
+
+
 def test_left_to_right(sample_ts):
     out_got = ts2vg.HorizontalVG(directed="left_to_right").build(sample_ts).edges
 
     out_truth = [
         (0, 1),
         (1, 2),
         (2, 3),
```

### Comparing `ts2vg-1.2.1/tests/test_horizontal_penetrable.py` & `ts2vg-1.2.2/tests/test_horizontal_penetrable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 from math import atan, sqrt
 
 import numpy as np
 import pytest
 from pytest import approx
 
+from fixtures import *
 import ts2vg
-from fixtures import (
-    empty_ts,
-    flat_ts,
-    sample_ts,
-    sample_ts_2,
-    linear_ts_small,
-    linear_ts_large,
-    linear_ts_large_negative,
-)
+from naive_implementations import horizontal_visibility_graph as naive_hvg
 
 
 def test_negative_parametric(sample_ts):
     with pytest.raises(ValueError):
         ts2vg.HorizontalVG(penetrable_limit=-1).build(sample_ts)
 
 
@@ -113,14 +106,67 @@
         (1, 3),
         (2, 3),
     ]
 
     assert sorted(sorted(e) for e in out_got) == sorted(sorted(e) for e in out_truth)
 
 
+
+def test_penetrable_1_white_noise(white_noise_ts):
+    ts = white_noise_ts
+    xs = list(range(len(ts)))
+
+    vg = ts2vg.HorizontalVG(penetrable_limit=1)
+
+    out_got = vg.build(ts, xs).edges
+
+    out_truth = naive_hvg(ts, xs, penetrable_limit=1)
+
+    assert sorted(sorted(e) for e in out_got) == sorted(sorted(e) for e in out_truth)
+
+
+def test_penetrable_3_white_noise(white_noise_ts):
+    ts = white_noise_ts
+    xs = list(range(len(ts)))
+
+    vg = ts2vg.HorizontalVG(penetrable_limit=3)
+
+    out_got = vg.build(ts, xs).edges
+
+    out_truth = naive_hvg(ts, xs, penetrable_limit=3)
+
+    assert sorted(sorted(e) for e in out_got) == sorted(sorted(e) for e in out_truth)
+
+
+def test_penetrable_1_brownian_motion(brownian_motion_ts):
+    ts = brownian_motion_ts
+    xs = list(range(len(ts)))
+
+    vg = ts2vg.HorizontalVG(penetrable_limit=1)
+
+    out_got = vg.build(ts, xs).edges
+
+    out_truth = naive_hvg(ts, xs, penetrable_limit=1)
+
+    assert sorted(sorted(e) for e in out_got) == sorted(sorted(e) for e in out_truth)
+
+
+def test_penetrable_3_brownian_motion(brownian_motion_ts):
+    ts = brownian_motion_ts
+    xs = list(range(len(ts)))
+
+    vg = ts2vg.HorizontalVG(penetrable_limit=3)
+
+    out_got = vg.build(ts, xs).edges
+
+    out_truth = naive_hvg(ts, xs, penetrable_limit=3)
+
+    assert sorted(sorted(e) for e in out_got) == sorted(sorted(e) for e in out_truth)
+
+
 def test_penetrable_1_ltr(sample_ts):
     vg = ts2vg.HorizontalVG(directed="left_to_right", penetrable_limit=1)
     out_got = vg.build(sample_ts).edges
 
     out_truth = [
         (0, 1),
         (0, 2),
```

### Comparing `ts2vg-1.2.1/tests/test_natural.py` & `ts2vg-1.2.2/tests/test_natural.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 from math import atan, sqrt
 
 import numpy as np
 import pytest
 from pytest import approx
 
+from fixtures import *
 import ts2vg
-from fixtures import (
-    empty_ts,
-    flat_ts,
-    sample_ts,
-    sample_ts_2,
-    linear_ts_small,
-    linear_ts_large,
-    linear_ts_large_negative,
-)
+from naive_implementations import natural_visibility_graph as naive_nvg
 
 
 def test_basic(sample_ts):
     out_got = ts2vg.NaturalVG().build(sample_ts).edges
 
     out_truth = [
         (0, 1),
@@ -57,14 +50,36 @@
         (7, 8),
         (8, 9),
     ]
 
     assert sorted(sorted(e) for e in out_got) == sorted(sorted(e) for e in out_truth)
 
 
+def test_white_noise(white_noise_ts):
+    ts = white_noise_ts
+    xs = list(range(len(ts)))
+
+    out_got = ts2vg.NaturalVG().build(ts, xs).edges
+
+    out_truth = naive_nvg(ts, xs)
+
+    assert sorted(sorted(e) for e in out_got) == sorted(sorted(e) for e in out_truth)
+
+
+def test_brownian_motion_ts(brownian_motion_ts):
+    ts = brownian_motion_ts
+    xs = list(range(len(ts)))
+
+    out_got = ts2vg.NaturalVG().build(ts, xs).edges
+
+    out_truth = naive_nvg(ts, xs)
+
+    assert sorted(sorted(e) for e in out_got) == sorted(sorted(e) for e in out_truth)
+
+
 def test_left_to_right(sample_ts):
     out_got = ts2vg.NaturalVG(directed="left_to_right").build(sample_ts).edges
 
     out_truth = [
         (0, 1),
         (1, 2),
         (1, 3),
```

### Comparing `ts2vg-1.2.1/tests/test_natural_penetrable.py` & `ts2vg-1.2.2/tests/test_natural_penetrable.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 from math import atan, sqrt
 
 import numpy as np
 import pytest
 from pytest import approx
 
+from fixtures import *
 import ts2vg
-from fixtures import (
-    empty_ts,
-    flat_ts,
-    sample_ts,
-    sample_ts_2,
-    linear_ts_small,
-    linear_ts_large,
-    linear_ts_large_negative,
-)
+from naive_implementations import natural_visibility_graph as naive_nvg
 
 
 def test_negative_parametric(sample_ts):
     with pytest.raises(ValueError):
         ts2vg.NaturalVG(penetrable_limit=-1).build(sample_ts)
 
 
@@ -124,14 +117,66 @@
         (1, 3),
         (2, 3),
     ]
 
     assert sorted(sorted(e) for e in out_got) == sorted(sorted(e) for e in out_truth)
 
 
+def test_penetrable_1_white_noise(white_noise_ts):
+    ts = white_noise_ts
+    xs = list(range(len(ts)))
+
+    vg = ts2vg.NaturalVG(penetrable_limit=1)
+
+    out_got = vg.build(ts, xs).edges
+
+    out_truth = naive_nvg(ts, xs, penetrable_limit=1)
+
+    assert sorted(sorted(e) for e in out_got) == sorted(sorted(e) for e in out_truth)
+
+
+def test_penetrable_3_white_noise(white_noise_ts):
+    ts = white_noise_ts
+    xs = list(range(len(ts)))
+
+    vg = ts2vg.NaturalVG(penetrable_limit=3)
+
+    out_got = vg.build(ts, xs).edges
+
+    out_truth = naive_nvg(ts, xs, penetrable_limit=3)
+
+    assert sorted(sorted(e) for e in out_got) == sorted(sorted(e) for e in out_truth)
+
+
+def test_penetrable_1_brownian_motion(brownian_motion_ts):
+    ts = brownian_motion_ts
+    xs = list(range(len(ts)))
+
+    vg = ts2vg.NaturalVG(penetrable_limit=1)
+
+    out_got = vg.build(ts, xs).edges
+
+    out_truth = naive_nvg(ts, xs, penetrable_limit=1)
+
+    assert sorted(sorted(e) for e in out_got) == sorted(sorted(e) for e in out_truth)
+
+
+def test_penetrable_3_brownian_motion(brownian_motion_ts):
+    ts = brownian_motion_ts
+    xs = list(range(len(ts)))
+
+    vg = ts2vg.NaturalVG(penetrable_limit=3)
+
+    out_got = vg.build(ts, xs).edges
+
+    out_truth = naive_nvg(ts, xs, penetrable_limit=3)
+
+    assert sorted(sorted(e) for e in out_got) == sorted(sorted(e) for e in out_truth)
+
+
 def test_penetrable_1_ltr(sample_ts):
     vg = ts2vg.NaturalVG(directed="left_to_right", penetrable_limit=1)
     out_got = vg.build(sample_ts).edges
 
     out_truth = [
         (0, 1),
         (0, 2),
```

### Comparing `ts2vg-1.2.1/tests/test_parametric.py` & `ts2vg-1.2.2/tests/test_parametric.py`

 * *Files identical despite different names*

### Comparing `ts2vg-1.2.1/ts2vg/graph/_base.c` & `ts2vg-1.2.2/ts2vg/graph/_base.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include"
         ],
         "name": "ts2vg.graph._base",
         "sources": [
             "ts2vg/graph/_base.pyx"
         ]
     },
     "module_name": "ts2vg.graph._base"
@@ -33,16 +33,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -227,15 +227,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -266,15 +266,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1120,195 +1120,195 @@
   Py_ssize_t shape[8];
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1348,42 +1348,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2000,20 +2000,28 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* DictGetItem.proto */
 #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
 static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
 #define __Pyx_PyObject_Dict_GetItem(obj, name)\
     (likely(PyDict_CheckExact(obj)) ?\
@@ -3882,15 +3890,15 @@
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3899,29 +3907,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3932,15 +3940,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3949,29 +3957,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3982,15 +3990,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3999,29 +4007,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4032,15 +4040,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4049,29 +4057,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4082,15 +4090,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4099,29 +4107,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4132,212 +4140,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4353,15 +4361,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4369,53 +4377,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -4423,30 +4431,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4461,15 +4469,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4485,15 +4493,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4501,53 +4509,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -4555,30 +4563,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4593,15 +4601,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4617,15 +4625,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4633,53 +4641,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -4687,30 +4695,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4725,176 +4733,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -18836,26 +18844,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
@@ -19261,52 +19269,67 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -20311,28 +20334,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -21720,44 +21743,62 @@
     return ret;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `ts2vg-1.2.1/ts2vg/graph/_horizontal.c` & `ts2vg-1.2.2/ts2vg/graph/_horizontal.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include"
         ],
+        "language": "c++",
         "name": "ts2vg.graph._horizontal",
         "sources": [
             "ts2vg/graph/_horizontal.pyx"
         ]
     },
     "module_name": "ts2vg.graph._horizontal"
 }
@@ -33,16 +34,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -227,15 +228,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -266,15 +267,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -375,27 +376,41 @@
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
 
+#ifndef __cplusplus
+  #error "Cython files generated with the C++ option must be compiled with a C++ compiler."
+#endif
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
-  #elif defined(__GNUC__)
-    #define CYTHON_INLINE __inline__
-  #elif defined(_MSC_VER)
-    #define CYTHON_INLINE __inline
-  #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
-    #define CYTHON_INLINE inline
   #else
-    #define CYTHON_INLINE
+    #define CYTHON_INLINE inline
   #endif
 #endif
+template<typename T>
+void __Pyx_call_destructor(T& x) {
+    x.~T();
+}
+template<typename T>
+class __Pyx_FakeReference {
+  public:
+    __Pyx_FakeReference() : ptr(NULL) { }
+    __Pyx_FakeReference(const T& ref) : ptr(const_cast<T*>(&ref)) { }
+    T *operator->() { return ptr; }
+    T *operator&() { return ptr; }
+    operator T&() { return *ptr; }
+    template<typename U> bool operator ==(U other) { return *ptr == other; }
+    template<typename U> bool operator !=(U other) { return *ptr != other; }
+  private:
+    T *ptr;
+};
 
 #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
   #define Py_OptimizeFlag 0
 #endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
@@ -776,16 +791,34 @@
 #include "numpy/ndarraytypes.h"
 #include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
 
     /* NumPy API declarations from "numpy/__init__.pxd" */
     
 #include <math.h>
-#include <stdlib.h>
+#include "ios"
+#include "new"
+#include "stdexcept"
+#include "typeinfo"
+#include <queue>
+#include <utility>
+
+    #if __cplusplus >= 201103L || (defined(_MSC_VER) && _MSC_VER >= 1600)
+    // move should be defined for these versions of MSVC, but __cplusplus isn't set usefully
+    #include <type_traits>
+
+    namespace cython_std {
+    template <typename T> typename std::remove_reference<T>::type&& move(T& t) noexcept { return std::move(t); }
+    template <typename T> typename std::remove_reference<T>::type&& move(T&& t) noexcept { return std::move(t); }
+    }
+
+    #endif
+    
 #include "pythread.h"
+#include <stdlib.h>
 #include "pystate.h"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
@@ -1014,15 +1047,14 @@
 
 
 static const char *__pyx_f[] = {
   "ts2vg/graph/_horizontal.pyx",
   "__init__.pxd",
   "stringsource",
   "type.pxd",
-  "ts2vg/utils/pairqueue.pxd",
 };
 /* MemviewSliceStruct.proto */
 struct __pyx_memoryview_obj;
 typedef struct {
   struct __pyx_memoryview_obj *memview;
   char *data;
   Py_ssize_t shape[8];
@@ -1121,195 +1153,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1319,20 +1351,20 @@
  * 
  * ctypedef unsigned int uint             # <<<<<<<<<<<<<<
  * ctypedef double (*weight_func_type)(double x_a, double x_b, double y_a, double y_b, double slope)
  * 
  */
 typedef unsigned int __pyx_t_5ts2vg_5graph_5_base_uint;
 
-/* "ts2vg/graph/_horizontal.pyx":12
+/* "ts2vg/graph/_horizontal.pyx":14
  * from ts2vg.graph._base cimport _argmax, _get_weight_func, weight_func_type
  * 
  * ctypedef unsigned int uint             # <<<<<<<<<<<<<<
+ * ctypedef cpair[uint, uint] uint_pair
  * 
- * cdef uint _DIRECTED_LEFT_TO_RIGHT = _DIRECTED_OPTIONS['left_to_right']
  */
 typedef unsigned int __pyx_t_5ts2vg_5graph_11_horizontal_uint;
 /* Declarations.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     typedef ::std::complex< float > __pyx_t_float_complex;
   #else
@@ -1353,122 +1385,75 @@
 #else
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
-struct __pyx_obj_5ts2vg_5utils_9pairqueue_PairQueue;
 struct __pyx_obj_5ts2vg_5graph_11_horizontal___pyx_scope_struct___compute_graph;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
-struct __pyx_t_5ts2vg_5utils_9pairqueue_QueueEntry;
-struct __pyx_t_5ts2vg_5utils_9pairqueue_Queue;
-struct __pyx_ctuple_unsigned__space_int__and_unsigned__space_int;
-typedef struct __pyx_ctuple_unsigned__space_int__and_unsigned__space_int __pyx_ctuple_unsigned__space_int__and_unsigned__space_int;
-
-/* "ts2vg/utils/pairqueue.pxd":5
- * from libc.stdlib cimport malloc, free
- * 
- * cdef struct QueueEntry:             # <<<<<<<<<<<<<<
- *     unsigned int a;
- *     unsigned int b;
- */
-struct __pyx_t_5ts2vg_5utils_9pairqueue_QueueEntry {
-  unsigned int a;
-  unsigned int b;
-  struct __pyx_t_5ts2vg_5utils_9pairqueue_QueueEntry *next;
-};
-
-/* "ts2vg/utils/pairqueue.pxd":11
- *     QueueEntry *next;
- * 
- * cdef struct Queue:             # <<<<<<<<<<<<<<
- *     QueueEntry *head;
- *     QueueEntry *tail;
- */
-struct __pyx_t_5ts2vg_5utils_9pairqueue_Queue {
-  struct __pyx_t_5ts2vg_5utils_9pairqueue_QueueEntry *head;
-  struct __pyx_t_5ts2vg_5utils_9pairqueue_QueueEntry *tail;
-};
-
-/* "ts2vg/utils/pairqueue.pxd":18
- *     cdef Queue *queue
- * 
- *     cdef void push(self, (unsigned int, unsigned int) values)             # <<<<<<<<<<<<<<
- *     cdef (unsigned int, unsigned int) pop(self)
- *     cdef bint is_empty(self)
- */
-struct __pyx_ctuple_unsigned__space_int__and_unsigned__space_int {
-  unsigned int f0;
-  unsigned int f1;
-};
 
 /* "ts2vg/graph/_base.pxd":6
  * 
  * ctypedef unsigned int uint
  * ctypedef double (*weight_func_type)(double x_a, double x_b, double y_a, double y_b, double slope)             # <<<<<<<<<<<<<<
  * 
  * cdef bint _greater(double a, double b, double tolerance)
  */
 typedef double (*__pyx_t_5ts2vg_5graph_5_base_weight_func_type)(double, double, double, double, double);
 
-/* "ts2vg/utils/pairqueue.pxd":15
- *     QueueEntry *tail;
+/* "ts2vg/graph/_horizontal.pyx":15
  * 
- * cdef class PairQueue:             # <<<<<<<<<<<<<<
- *     cdef Queue *queue
+ * ctypedef unsigned int uint
+ * ctypedef cpair[uint, uint] uint_pair             # <<<<<<<<<<<<<<
  * 
+ * cdef uint _DIRECTED_LEFT_TO_RIGHT = _DIRECTED_OPTIONS['left_to_right']
  */
-struct __pyx_obj_5ts2vg_5utils_9pairqueue_PairQueue {
-  PyObject_HEAD
-  struct __pyx_vtabstruct_5ts2vg_5utils_9pairqueue_PairQueue *__pyx_vtab;
-  struct __pyx_t_5ts2vg_5utils_9pairqueue_Queue *queue;
-};
-
+typedef std::pair<unsigned int,unsigned int>  __pyx_t_5ts2vg_5graph_11_horizontal_uint_pair;
 
-/* "ts2vg/graph/_horizontal.pyx":21
+/* "ts2vg/graph/_horizontal.pyx":24
  * @cython.wraparound(False)
  * @cython.cdivision(True)
  * def _compute_graph(np.float64_t[:] ts, np.float64_t[:] xs, uint directed, uint weighted, bint only_degrees, double min_weight, double max_weight):             # <<<<<<<<<<<<<<
  *     """
  *     Computes the horizontal visibility graph of a time series
  */
 struct __pyx_obj_5ts2vg_5graph_11_horizontal___pyx_scope_struct___compute_graph {
@@ -1558,31 +1543,14 @@
   PyObject *from_object;
   PyObject *(*to_object_func)(char *);
   int (*to_dtype_func)(char *, PyObject *);
 };
 
 
 
-/* "ts2vg/utils/pairqueue.pxd":15
- *     QueueEntry *tail;
- * 
- * cdef class PairQueue:             # <<<<<<<<<<<<<<
- *     cdef Queue *queue
- * 
- */
-
-struct __pyx_vtabstruct_5ts2vg_5utils_9pairqueue_PairQueue {
-  void (*push)(struct __pyx_obj_5ts2vg_5utils_9pairqueue_PairQueue *, __pyx_ctuple_unsigned__space_int__and_unsigned__space_int);
-  __pyx_ctuple_unsigned__space_int__and_unsigned__space_int (*pop)(struct __pyx_obj_5ts2vg_5utils_9pairqueue_PairQueue *);
-  int (*is_empty)(struct __pyx_obj_5ts2vg_5utils_9pairqueue_PairQueue *);
-  void (*free)(struct __pyx_obj_5ts2vg_5utils_9pairqueue_PairQueue *);
-};
-static struct __pyx_vtabstruct_5ts2vg_5utils_9pairqueue_PairQueue *__pyx_vtabptr_5ts2vg_5utils_9pairqueue_PairQueue;
-
-
 /* "View.MemoryView":106
  * 
  * @cname("__pyx_array")
  * cdef class array:             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
@@ -1782,57 +1750,14 @@
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
 #endif
 
-/* PyFunctionFastCall.proto */
-#if CYTHON_FAST_PYCALL
-#define __Pyx_PyFunction_FastCall(func, args, nargs)\
-    __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
-#if 1 || PY_VERSION_HEX < 0x030600B1
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
-#else
-#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
-#endif
-#define __Pyx_BUILD_ASSERT_EXPR(cond)\
-    (sizeof(char [1 - 2*!(cond)]) - 1)
-#ifndef Py_MEMBER_SIZE
-#define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
-#endif
-#if CYTHON_FAST_PYCALL
-  static size_t __pyx_pyframe_localsplus_offset = 0;
-  #include "frameobject.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
-  #define __Pxy_PyFrame_Initialize_Offsets()\
-    ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
-     (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
-  #define __Pyx_PyFrame_GetLocalsplus(frame)\
-    (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
-#endif // CYTHON_FAST_PYCALL
-#endif
-
-/* PyObjectCallMethO.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
-#endif
-
-/* PyObjectCallNoArg.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
-#else
-#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
-#endif
-
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 
 /* CythonFunctionShared.proto */
 #define __Pyx_CyFunction_USED 1
 #define __Pyx_CYFUNCTION_STATICMETHOD  0x01
 #define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
@@ -1998,17 +1923,53 @@
 /* PyCFunctionFastCall.proto */
 #if CYTHON_FAST_PYCCALL
 static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
 #else
 #define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
 #endif
 
+/* PyFunctionFastCall.proto */
+#if CYTHON_FAST_PYCALL
+#define __Pyx_PyFunction_FastCall(func, args, nargs)\
+    __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
+#if 1 || PY_VERSION_HEX < 0x030600B1
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
+#else
+#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
+#endif
+#define __Pyx_BUILD_ASSERT_EXPR(cond)\
+    (sizeof(char [1 - 2*!(cond)]) - 1)
+#ifndef Py_MEMBER_SIZE
+#define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
+#endif
+#if CYTHON_FAST_PYCALL
+  static size_t __pyx_pyframe_localsplus_offset = 0;
+  #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+  #define __Pxy_PyFrame_Initialize_Offsets()\
+    ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
+     (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
+  #define __Pyx_PyFrame_GetLocalsplus(frame)\
+    (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
+#endif
+
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
+/* PyObjectCallMethO.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
+#endif
+
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
 /* IncludeStringH.proto */
 #include <string.h>
 
 /* BytesEquals.proto */
@@ -2203,25 +2164,30 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
-/* GetVTable.proto */
-static void* __Pyx_GetVtable(PyObject *dict);
-
 /* DictGetItem.proto */
 #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
 static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
 #define __Pyx_PyObject_Dict_GetItem(obj, name)\
     (likely(PyDict_CheckExact(obj)) ?\
      __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
 #else
@@ -2323,14 +2289,56 @@
 /* MemviewDtypeToObject.proto */
 static CYTHON_INLINE PyObject *__pyx_memview_get_nn___pyx_t_5numpy_float64_t(const char *itemp);
 static CYTHON_INLINE int __pyx_memview_set_nn___pyx_t_5numpy_float64_t(const char *itemp, PyObject *obj);
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(PyObject *, int writable_flag);
 
+/* CppExceptionConversion.proto */
+#ifndef __Pyx_CppExn2PyErr
+#include <new>
+#include <typeinfo>
+#include <stdexcept>
+#include <ios>
+static void __Pyx_CppExn2PyErr() {
+  try {
+    if (PyErr_Occurred())
+      ; // let the latest Python exn pass through and ignore the current one
+    else
+      throw;
+  } catch (const std::bad_alloc& exn) {
+    PyErr_SetString(PyExc_MemoryError, exn.what());
+  } catch (const std::bad_cast& exn) {
+    PyErr_SetString(PyExc_TypeError, exn.what());
+  } catch (const std::bad_typeid& exn) {
+    PyErr_SetString(PyExc_TypeError, exn.what());
+  } catch (const std::domain_error& exn) {
+    PyErr_SetString(PyExc_ValueError, exn.what());
+  } catch (const std::invalid_argument& exn) {
+    PyErr_SetString(PyExc_ValueError, exn.what());
+  } catch (const std::ios_base::failure& exn) {
+    PyErr_SetString(PyExc_IOError, exn.what());
+  } catch (const std::out_of_range& exn) {
+    PyErr_SetString(PyExc_IndexError, exn.what());
+  } catch (const std::overflow_error& exn) {
+    PyErr_SetString(PyExc_OverflowError, exn.what());
+  } catch (const std::range_error& exn) {
+    PyErr_SetString(PyExc_ArithmeticError, exn.what());
+  } catch (const std::underflow_error& exn) {
+    PyErr_SetString(PyExc_ArithmeticError, exn.what());
+  } catch (const std::exception& exn) {
+    PyErr_SetString(PyExc_RuntimeError, exn.what());
+  }
+  catch (...)
+  {
+    PyErr_SetString(PyExc_RuntimeError, "Unknown exception");
+  }
+}
+#endif
+
 /* MemviewDtypeToObject.proto */
 static CYTHON_INLINE PyObject *__pyx_memview_get_nn___pyx_t_5numpy_uint32_t(const char *itemp);
 static CYTHON_INLINE int __pyx_memview_set_nn___pyx_t_5numpy_uint32_t(const char *itemp, PyObject *obj);
 
 /* RealImag.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
@@ -2523,18 +2531,19 @@
 static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
 static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'libc.math' */
 
-/* Module declarations from 'libc.stdlib' */
+/* Module declarations from 'libcpp.queue' */
 
-/* Module declarations from 'ts2vg.utils.pairqueue' */
-static PyTypeObject *__pyx_ptype_5ts2vg_5utils_9pairqueue_PairQueue = 0;
+/* Module declarations from 'libcpp.utility' */
+
+/* Module declarations from 'libcpp.pair' */
 
 /* Module declarations from 'ts2vg.graph._base' */
 static __pyx_t_5ts2vg_5graph_5_base_uint (*__pyx_f_5ts2vg_5graph_5_base__argmax)(__Pyx_memviewslice, __pyx_t_5ts2vg_5graph_5_base_uint, __pyx_t_5ts2vg_5graph_5_base_uint); /*proto*/
 static __pyx_t_5ts2vg_5graph_5_base_weight_func_type (*__pyx_f_5ts2vg_5graph_5_base__get_weight_func)(__pyx_t_5ts2vg_5graph_5_base_uint); /*proto*/
 
 /* Module declarations from 'ts2vg.graph._horizontal' */
 static PyTypeObject *__pyx_ptype_5ts2vg_5graph_11_horizontal___pyx_scope_struct___compute_graph = 0;
@@ -2626,14 +2635,15 @@
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_left[] = "left";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_mode[] = "mode";
 static const char __pyx_k_name[] = "name";
 static const char __pyx_k_ndim[] = "ndim";
 static const char __pyx_k_pack[] = "pack";
+static const char __pyx_k_pair[] = "pair";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_step[] = "step";
 static const char __pyx_k_stop[] = "stop";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_ASCII[] = "ASCII";
 static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_dtype[] = "dtype";
@@ -2809,14 +2819,15 @@
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_obj;
 static PyObject *__pyx_n_s_only_degrees;
 static PyObject *__pyx_n_s_pack;
+static PyObject *__pyx_n_s_pair;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_getbuffer;
 static PyObject *__pyx_n_s_pyx_result;
 static PyObject *__pyx_n_s_pyx_state;
 static PyObject *__pyx_n_s_pyx_type;
@@ -2949,15 +2960,15 @@
 static PyObject *__pyx_tuple__30;
 static PyObject *__pyx_tuple__31;
 static PyObject *__pyx_codeobj__2;
 static PyObject *__pyx_codeobj__25;
 static PyObject *__pyx_codeobj__32;
 /* Late includes */
 
-/* "ts2vg/graph/_horizontal.pyx":21
+/* "ts2vg/graph/_horizontal.pyx":24
  * @cython.wraparound(False)
  * @cython.cdivision(True)
  * def _compute_graph(np.float64_t[:] ts, np.float64_t[:] xs, uint directed, uint weighted, bint only_degrees, double min_weight, double max_weight):             # <<<<<<<<<<<<<<
  *     """
  *     Computes the horizontal visibility graph of a time series
  */
 
@@ -3008,86 +3019,86 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ts)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_xs)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 1); __PYX_ERR(0, 21, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 1); __PYX_ERR(0, 24, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_directed)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 2); __PYX_ERR(0, 21, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 2); __PYX_ERR(0, 24, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_weighted)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 3); __PYX_ERR(0, 21, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 3); __PYX_ERR(0, 24, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_only_degrees)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 4); __PYX_ERR(0, 21, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 4); __PYX_ERR(0, 24, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_min_weight)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 5); __PYX_ERR(0, 21, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 5); __PYX_ERR(0, 24, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_max_weight)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 6); __PYX_ERR(0, 21, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 6); __PYX_ERR(0, 24, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_compute_graph") < 0)) __PYX_ERR(0, 21, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_compute_graph") < 0)) __PYX_ERR(0, 24, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 7) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
       values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
     }
-    __pyx_v_ts = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_ts.memview)) __PYX_ERR(0, 21, __pyx_L3_error)
-    __pyx_v_xs = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_xs.memview)) __PYX_ERR(0, 21, __pyx_L3_error)
-    __pyx_v_directed = __Pyx_PyInt_As_unsigned_int(values[2]); if (unlikely((__pyx_v_directed == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 21, __pyx_L3_error)
-    __pyx_v_weighted = __Pyx_PyInt_As_unsigned_int(values[3]); if (unlikely((__pyx_v_weighted == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 21, __pyx_L3_error)
-    __pyx_v_only_degrees = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_only_degrees == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 21, __pyx_L3_error)
-    __pyx_v_min_weight = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_min_weight == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 21, __pyx_L3_error)
-    __pyx_v_max_weight = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_max_weight == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 21, __pyx_L3_error)
+    __pyx_v_ts = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_ts.memview)) __PYX_ERR(0, 24, __pyx_L3_error)
+    __pyx_v_xs = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_xs.memview)) __PYX_ERR(0, 24, __pyx_L3_error)
+    __pyx_v_directed = __Pyx_PyInt_As_unsigned_int(values[2]); if (unlikely((__pyx_v_directed == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 24, __pyx_L3_error)
+    __pyx_v_weighted = __Pyx_PyInt_As_unsigned_int(values[3]); if (unlikely((__pyx_v_weighted == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 24, __pyx_L3_error)
+    __pyx_v_only_degrees = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_only_degrees == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 24, __pyx_L3_error)
+    __pyx_v_min_weight = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_min_weight == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 24, __pyx_L3_error)
+    __pyx_v_max_weight = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_max_weight == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 24, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 21, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 24, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ts2vg.graph._horizontal._compute_graph", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5ts2vg_5graph_11_horizontal__compute_graph(__pyx_self, __pyx_v_ts, __pyx_v_xs, __pyx_v_directed, __pyx_v_weighted, __pyx_v_only_degrees, __pyx_v_min_weight, __pyx_v_max_weight);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ts2vg/graph/_horizontal.pyx":40
- *     queue.push((0, n))
+/* "ts2vg/graph/_horizontal.pyx":43
+ *     queue.push(uint_pair(0, n))
  * 
  *     def add_edge(uint i1, uint i2, double x1, double x2, double y1, double y2):             # <<<<<<<<<<<<<<
  *         w = weight_func(x1, x2, y1, y2, NAN)
  * 
  */
 
 /* Python wrapper */
@@ -3133,64 +3144,64 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_i1)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_i2)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 6, 6, 1); __PYX_ERR(0, 40, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 6, 6, 1); __PYX_ERR(0, 43, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_x1)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 6, 6, 2); __PYX_ERR(0, 40, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 6, 6, 2); __PYX_ERR(0, 43, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_x2)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 6, 6, 3); __PYX_ERR(0, 40, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 6, 6, 3); __PYX_ERR(0, 43, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_y1)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 6, 6, 4); __PYX_ERR(0, 40, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 6, 6, 4); __PYX_ERR(0, 43, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_y2)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 6, 6, 5); __PYX_ERR(0, 40, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 6, 6, 5); __PYX_ERR(0, 43, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "add_edge") < 0)) __PYX_ERR(0, 40, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "add_edge") < 0)) __PYX_ERR(0, 43, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 6) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
     }
-    __pyx_v_i1 = __Pyx_PyInt_As_unsigned_int(values[0]); if (unlikely((__pyx_v_i1 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 40, __pyx_L3_error)
-    __pyx_v_i2 = __Pyx_PyInt_As_unsigned_int(values[1]); if (unlikely((__pyx_v_i2 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 40, __pyx_L3_error)
-    __pyx_v_x1 = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_x1 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 40, __pyx_L3_error)
-    __pyx_v_x2 = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_x2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 40, __pyx_L3_error)
-    __pyx_v_y1 = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_y1 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 40, __pyx_L3_error)
-    __pyx_v_y2 = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_y2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 40, __pyx_L3_error)
+    __pyx_v_i1 = __Pyx_PyInt_As_unsigned_int(values[0]); if (unlikely((__pyx_v_i1 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 43, __pyx_L3_error)
+    __pyx_v_i2 = __Pyx_PyInt_As_unsigned_int(values[1]); if (unlikely((__pyx_v_i2 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 43, __pyx_L3_error)
+    __pyx_v_x1 = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_x1 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 43, __pyx_L3_error)
+    __pyx_v_x2 = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_x2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 43, __pyx_L3_error)
+    __pyx_v_y1 = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_y1 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 43, __pyx_L3_error)
+    __pyx_v_y2 = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_y2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 43, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("add_edge", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 40, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("add_edge", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 43, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ts2vg.graph._horizontal._compute_graph.add_edge", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5ts2vg_5graph_11_horizontal_14_compute_graph_add_edge(__pyx_self, __pyx_v_i1, __pyx_v_i2, __pyx_v_x1, __pyx_v_x2, __pyx_v_y1, __pyx_v_y2);
 
@@ -3216,24 +3227,24 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_edge", 0);
   __pyx_outer_scope = (struct __pyx_obj_5ts2vg_5graph_11_horizontal___pyx_scope_struct___compute_graph *) __Pyx_CyFunction_GetClosure(__pyx_self);
   __pyx_cur_scope = __pyx_outer_scope;
 
-  /* "ts2vg/graph/_horizontal.pyx":41
+  /* "ts2vg/graph/_horizontal.pyx":44
  * 
  *     def add_edge(uint i1, uint i2, double x1, double x2, double y1, double y2):
  *         w = weight_func(x1, x2, y1, y2, NAN)             # <<<<<<<<<<<<<<
  * 
  *         if w <= min_weight or w >= max_weight:
  */
   __pyx_v_w = __pyx_cur_scope->__pyx_v_weight_func(__pyx_v_x1, __pyx_v_x2, __pyx_v_y1, __pyx_v_y2, NAN);
 
-  /* "ts2vg/graph/_horizontal.pyx":43
+  /* "ts2vg/graph/_horizontal.pyx":46
  *         w = weight_func(x1, x2, y1, y2, NAN)
  * 
  *         if w <= min_weight or w >= max_weight:             # <<<<<<<<<<<<<<
  *             return
  * 
  */
   __pyx_t_2 = ((__pyx_v_w <= __pyx_cur_scope->__pyx_v_min_weight) != 0);
@@ -3243,159 +3254,159 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = ((__pyx_v_w >= __pyx_cur_scope->__pyx_v_max_weight) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "ts2vg/graph/_horizontal.pyx":44
+    /* "ts2vg/graph/_horizontal.pyx":47
  * 
  *         if w <= min_weight or w >= max_weight:
  *             return             # <<<<<<<<<<<<<<
  * 
  *         degrees_out[i1] += 1
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "ts2vg/graph/_horizontal.pyx":43
+    /* "ts2vg/graph/_horizontal.pyx":46
  *         w = weight_func(x1, x2, y1, y2, NAN)
  * 
  *         if w <= min_weight or w >= max_weight:             # <<<<<<<<<<<<<<
  *             return
  * 
  */
   }
 
-  /* "ts2vg/graph/_horizontal.pyx":46
+  /* "ts2vg/graph/_horizontal.pyx":49
  *             return
  * 
  *         degrees_out[i1] += 1             # <<<<<<<<<<<<<<
  *         degrees_in[i2] += 1
  * 
  */
-  if (unlikely(!__pyx_cur_scope->__pyx_v_degrees_out.memview)) { __Pyx_RaiseClosureNameError("degrees_out"); __PYX_ERR(0, 46, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_v_degrees_out.memview)) { __Pyx_RaiseClosureNameError("degrees_out"); __PYX_ERR(0, 49, __pyx_L1_error) }
   __pyx_t_3 = __pyx_v_i1;
   *((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_cur_scope->__pyx_v_degrees_out.data + __pyx_t_3 * __pyx_cur_scope->__pyx_v_degrees_out.strides[0]) )) += 1;
 
-  /* "ts2vg/graph/_horizontal.pyx":47
+  /* "ts2vg/graph/_horizontal.pyx":50
  * 
  *         degrees_out[i1] += 1
  *         degrees_in[i2] += 1             # <<<<<<<<<<<<<<
  * 
  *         if not only_degrees:
  */
-  if (unlikely(!__pyx_cur_scope->__pyx_v_degrees_in.memview)) { __Pyx_RaiseClosureNameError("degrees_in"); __PYX_ERR(0, 47, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_v_degrees_in.memview)) { __Pyx_RaiseClosureNameError("degrees_in"); __PYX_ERR(0, 50, __pyx_L1_error) }
   __pyx_t_3 = __pyx_v_i2;
   *((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_cur_scope->__pyx_v_degrees_in.data + __pyx_t_3 * __pyx_cur_scope->__pyx_v_degrees_in.strides[0]) )) += 1;
 
-  /* "ts2vg/graph/_horizontal.pyx":49
+  /* "ts2vg/graph/_horizontal.pyx":52
  *         degrees_in[i2] += 1
  * 
  *         if not only_degrees:             # <<<<<<<<<<<<<<
  *             if weighted > 0:
  *                 edges.append((i1, i2, w))
  */
   __pyx_t_1 = ((!(__pyx_cur_scope->__pyx_v_only_degrees != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "ts2vg/graph/_horizontal.pyx":50
+    /* "ts2vg/graph/_horizontal.pyx":53
  * 
  *         if not only_degrees:
  *             if weighted > 0:             # <<<<<<<<<<<<<<
  *                 edges.append((i1, i2, w))
  *             else:
  */
     __pyx_t_1 = ((__pyx_cur_scope->__pyx_v_weighted > 0) != 0);
     if (__pyx_t_1) {
 
-      /* "ts2vg/graph/_horizontal.pyx":51
+      /* "ts2vg/graph/_horizontal.pyx":54
  *         if not only_degrees:
  *             if weighted > 0:
  *                 edges.append((i1, i2, w))             # <<<<<<<<<<<<<<
  *             else:
  *                 edges.append((i1, i2))
  */
-      if (unlikely(!__pyx_cur_scope->__pyx_v_edges)) { __Pyx_RaiseClosureNameError("edges"); __PYX_ERR(0, 51, __pyx_L1_error) }
+      if (unlikely(!__pyx_cur_scope->__pyx_v_edges)) { __Pyx_RaiseClosureNameError("edges"); __PYX_ERR(0, 54, __pyx_L1_error) }
       if (unlikely(__pyx_cur_scope->__pyx_v_edges == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "append");
-        __PYX_ERR(0, 51, __pyx_L1_error)
+        __PYX_ERR(0, 54, __pyx_L1_error)
       }
-      __pyx_t_4 = __Pyx_PyInt_From_unsigned_int(__pyx_v_i1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 51, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_unsigned_int(__pyx_v_i1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyInt_From_unsigned_int(__pyx_v_i2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 51, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_unsigned_int(__pyx_v_i2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 54, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = PyFloat_FromDouble(__pyx_v_w); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 51, __pyx_L1_error)
+      __pyx_t_6 = PyFloat_FromDouble(__pyx_v_w); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 54, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 51, __pyx_L1_error)
+      __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 54, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_t_6);
       __pyx_t_4 = 0;
       __pyx_t_5 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_8 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_edges, __pyx_t_7); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 51, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_edges, __pyx_t_7); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 54, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "ts2vg/graph/_horizontal.pyx":50
+      /* "ts2vg/graph/_horizontal.pyx":53
  * 
  *         if not only_degrees:
  *             if weighted > 0:             # <<<<<<<<<<<<<<
  *                 edges.append((i1, i2, w))
  *             else:
  */
       goto __pyx_L7;
     }
 
-    /* "ts2vg/graph/_horizontal.pyx":53
+    /* "ts2vg/graph/_horizontal.pyx":56
  *                 edges.append((i1, i2, w))
  *             else:
  *                 edges.append((i1, i2))             # <<<<<<<<<<<<<<
  * 
  * 
  */
     /*else*/ {
-      if (unlikely(!__pyx_cur_scope->__pyx_v_edges)) { __Pyx_RaiseClosureNameError("edges"); __PYX_ERR(0, 53, __pyx_L1_error) }
+      if (unlikely(!__pyx_cur_scope->__pyx_v_edges)) { __Pyx_RaiseClosureNameError("edges"); __PYX_ERR(0, 56, __pyx_L1_error) }
       if (unlikely(__pyx_cur_scope->__pyx_v_edges == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "append");
-        __PYX_ERR(0, 53, __pyx_L1_error)
+        __PYX_ERR(0, 56, __pyx_L1_error)
       }
-      __pyx_t_7 = __Pyx_PyInt_From_unsigned_int(__pyx_v_i1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 53, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_From_unsigned_int(__pyx_v_i1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 56, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_6 = __Pyx_PyInt_From_unsigned_int(__pyx_v_i2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 53, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_From_unsigned_int(__pyx_v_i2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 56, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_7);
       PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_7);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_6);
       __pyx_t_7 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_8 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_edges, __pyx_t_5); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 53, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_edges, __pyx_t_5); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 56, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __pyx_L7:;
 
-    /* "ts2vg/graph/_horizontal.pyx":49
+    /* "ts2vg/graph/_horizontal.pyx":52
  *         degrees_in[i2] += 1
  * 
  *         if not only_degrees:             # <<<<<<<<<<<<<<
  *             if weighted > 0:
  *                 edges.append((i1, i2, w))
  */
   }
 
-  /* "ts2vg/graph/_horizontal.pyx":40
- *     queue.push((0, n))
+  /* "ts2vg/graph/_horizontal.pyx":43
+ *     queue.push(uint_pair(0, n))
  * 
  *     def add_edge(uint i1, uint i2, double x1, double x2, double y1, double y2):             # <<<<<<<<<<<<<<
  *         w = weight_func(x1, x2, y1, y2, NAN)
  * 
  */
 
   /* function exit code */
@@ -3410,15 +3421,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ts2vg/graph/_horizontal.pyx":21
+/* "ts2vg/graph/_horizontal.pyx":24
  * @cython.wraparound(False)
  * @cython.cdivision(True)
  * def _compute_graph(np.float64_t[:] ts, np.float64_t[:] xs, uint directed, uint weighted, bint only_degrees, double min_weight, double max_weight):             # <<<<<<<<<<<<<<
  *     """
  *     Computes the horizontal visibility graph of a time series
  */
 
@@ -3430,26 +3441,27 @@
   __pyx_t_5ts2vg_5graph_11_horizontal_uint __pyx_v_i;
   __pyx_t_5ts2vg_5graph_11_horizontal_uint __pyx_v_d;
   double __pyx_v_x_a;
   double __pyx_v_x_b;
   double __pyx_v_y_a;
   double __pyx_v_y_b;
   double __pyx_v_max_y;
-  struct __pyx_obj_5ts2vg_5utils_9pairqueue_PairQueue *__pyx_v_queue = 0;
+  std::queue<__pyx_t_5ts2vg_5graph_11_horizontal_uint_pair>  __pyx_v_queue;
   PyObject *__pyx_v_add_edge = 0;
+  __pyx_t_5ts2vg_5graph_11_horizontal_uint_pair __pyx_v_pair;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   __pyx_t_5ts2vg_5graph_11_horizontal_uint __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   __Pyx_memviewslice __pyx_t_7 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  __pyx_ctuple_unsigned__space_int__and_unsigned__space_int __pyx_t_8;
+  __pyx_t_5ts2vg_5graph_11_horizontal_uint_pair __pyx_t_8;
   int __pyx_t_9;
   unsigned int __pyx_t_10;
   unsigned int __pyx_t_11;
   size_t __pyx_t_12;
   long __pyx_t_13;
   long __pyx_t_14;
   __pyx_t_5ts2vg_5graph_11_horizontal_uint __pyx_t_15;
@@ -3459,539 +3471,556 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_compute_graph", 0);
   __pyx_cur_scope = (struct __pyx_obj_5ts2vg_5graph_11_horizontal___pyx_scope_struct___compute_graph *)__pyx_tp_new_5ts2vg_5graph_11_horizontal___pyx_scope_struct___compute_graph(__pyx_ptype_5ts2vg_5graph_11_horizontal___pyx_scope_struct___compute_graph, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_5ts2vg_5graph_11_horizontal___pyx_scope_struct___compute_graph *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 21, __pyx_L1_error)
+    __PYX_ERR(0, 24, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_weighted = __pyx_v_weighted;
   __pyx_cur_scope->__pyx_v_only_degrees = __pyx_v_only_degrees;
   __pyx_cur_scope->__pyx_v_min_weight = __pyx_v_min_weight;
   __pyx_cur_scope->__pyx_v_max_weight = __pyx_v_max_weight;
 
-  /* "ts2vg/graph/_horizontal.pyx":26
+  /* "ts2vg/graph/_horizontal.pyx":29
  *     using a divide-and-conquer strategy.
  *     """
  *     cdef uint n = ts.size             # <<<<<<<<<<<<<<
  *     cdef list edges = []
  *     cdef np.uint32_t[:] degrees_in = np.zeros(n, dtype=np.uint32)
  */
-  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_ts, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_float64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_float64_t, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_ts, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_float64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_float64_t, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyInt_As_unsigned_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_unsigned_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_n = __pyx_t_3;
 
-  /* "ts2vg/graph/_horizontal.pyx":27
+  /* "ts2vg/graph/_horizontal.pyx":30
  *     """
  *     cdef uint n = ts.size
  *     cdef list edges = []             # <<<<<<<<<<<<<<
  *     cdef np.uint32_t[:] degrees_in = np.zeros(n, dtype=np.uint32)
  *     cdef np.uint32_t[:] degrees_out = np.zeros(n, dtype=np.uint32)
  */
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_cur_scope->__pyx_v_edges = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "ts2vg/graph/_horizontal.pyx":28
+  /* "ts2vg/graph/_horizontal.pyx":31
  *     cdef uint n = ts.size
  *     cdef list edges = []
  *     cdef np.uint32_t[:] degrees_in = np.zeros(n, dtype=np.uint32)             # <<<<<<<<<<<<<<
  *     cdef np.uint32_t[:] degrees_out = np.zeros(n, dtype=np.uint32)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uint32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uint32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_t_6, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_t_6, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_cur_scope->__pyx_v_degrees_in = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
-  /* "ts2vg/graph/_horizontal.pyx":29
+  /* "ts2vg/graph/_horizontal.pyx":32
  *     cdef list edges = []
  *     cdef np.uint32_t[:] degrees_in = np.zeros(n, dtype=np.uint32)
  *     cdef np.uint32_t[:] degrees_out = np.zeros(n, dtype=np.uint32)             # <<<<<<<<<<<<<<
  * 
  *     cdef uint left, right, i, d
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyInt_From_unsigned_int(__pyx_v_n); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_unsigned_int(__pyx_v_n); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_cur_scope->__pyx_v_degrees_out = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
-  /* "ts2vg/graph/_horizontal.pyx":35
+  /* "ts2vg/graph/_horizontal.pyx":38
  *     cdef double max_y, w
  * 
  *     cdef weight_func_type weight_func = _get_weight_func(weighted)             # <<<<<<<<<<<<<<
  * 
- *     cdef PairQueue queue = PairQueue()
+ *     cdef cqueue[uint_pair] queue
  */
   __pyx_cur_scope->__pyx_v_weight_func = __pyx_f_5ts2vg_5graph_5_base__get_weight_func(__pyx_cur_scope->__pyx_v_weighted);
 
-  /* "ts2vg/graph/_horizontal.pyx":37
- *     cdef weight_func_type weight_func = _get_weight_func(weighted)
- * 
- *     cdef PairQueue queue = PairQueue()             # <<<<<<<<<<<<<<
- *     queue.push((0, n))
- * 
- */
-  __pyx_t_5 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_5ts2vg_5utils_9pairqueue_PairQueue)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 37, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_v_queue = ((struct __pyx_obj_5ts2vg_5utils_9pairqueue_PairQueue *)__pyx_t_5);
-  __pyx_t_5 = 0;
-
-  /* "ts2vg/graph/_horizontal.pyx":38
+  /* "ts2vg/graph/_horizontal.pyx":41
  * 
- *     cdef PairQueue queue = PairQueue()
- *     queue.push((0, n))             # <<<<<<<<<<<<<<
+ *     cdef cqueue[uint_pair] queue
+ *     queue.push(uint_pair(0, n))             # <<<<<<<<<<<<<<
  * 
  *     def add_edge(uint i1, uint i2, double x1, double x2, double y1, double y2):
  */
-  __pyx_t_8.f0 = 0;
-  __pyx_t_8.f1 = __pyx_v_n;
-  ((struct __pyx_vtabstruct_5ts2vg_5utils_9pairqueue_PairQueue *)__pyx_v_queue->__pyx_vtab)->push(__pyx_v_queue, __pyx_t_8);
+  try {
+    __pyx_t_8 = __pyx_t_5ts2vg_5graph_11_horizontal_uint_pair(0, __pyx_v_n);
+  } catch(...) {
+    __Pyx_CppExn2PyErr();
+    __PYX_ERR(0, 41, __pyx_L1_error)
+  }
+  __pyx_v_queue.push(__pyx_t_8);
 
-  /* "ts2vg/graph/_horizontal.pyx":40
- *     queue.push((0, n))
+  /* "ts2vg/graph/_horizontal.pyx":43
+ *     queue.push(uint_pair(0, n))
  * 
  *     def add_edge(uint i1, uint i2, double x1, double x2, double y1, double y2):             # <<<<<<<<<<<<<<
  *         w = weight_func(x1, x2, y1, y2, NAN)
  * 
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_5ts2vg_5graph_11_horizontal_14_compute_graph_1add_edge, 0, __pyx_n_s_compute_graph_locals_add_edge, ((PyObject*)__pyx_cur_scope), __pyx_n_s_ts2vg_graph__horizontal, __pyx_d, ((PyObject *)__pyx_codeobj__2)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_5ts2vg_5graph_11_horizontal_14_compute_graph_1add_edge, 0, __pyx_n_s_compute_graph_locals_add_edge, ((PyObject*)__pyx_cur_scope), __pyx_n_s_ts2vg_graph__horizontal, __pyx_d, ((PyObject *)__pyx_codeobj__2)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_v_add_edge = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "ts2vg/graph/_horizontal.pyx":56
+  /* "ts2vg/graph/_horizontal.pyx":59
  * 
  * 
- *     while not queue.is_empty():             # <<<<<<<<<<<<<<
- *         (left, right) = queue.pop()
- * 
+ *     while not queue.empty():             # <<<<<<<<<<<<<<
+ *         pair = queue.front()
+ *         left, right = pair.first, pair.second
  */
   while (1) {
-    __pyx_t_9 = ((!(((struct __pyx_vtabstruct_5ts2vg_5utils_9pairqueue_PairQueue *)__pyx_v_queue->__pyx_vtab)->is_empty(__pyx_v_queue) != 0)) != 0);
+    __pyx_t_9 = ((!(__pyx_v_queue.empty() != 0)) != 0);
     if (!__pyx_t_9) break;
 
-    /* "ts2vg/graph/_horizontal.pyx":57
+    /* "ts2vg/graph/_horizontal.pyx":60
  * 
- *     while not queue.is_empty():
- *         (left, right) = queue.pop()             # <<<<<<<<<<<<<<
+ *     while not queue.empty():
+ *         pair = queue.front()             # <<<<<<<<<<<<<<
+ *         left, right = pair.first, pair.second
+ *         queue.pop()
+ */
+    __pyx_v_pair = __pyx_v_queue.front();
+
+    /* "ts2vg/graph/_horizontal.pyx":61
+ *     while not queue.empty():
+ *         pair = queue.front()
+ *         left, right = pair.first, pair.second             # <<<<<<<<<<<<<<
+ *         queue.pop()
  * 
- *         if left+1 < right:
  */
-    __pyx_t_8 = ((struct __pyx_vtabstruct_5ts2vg_5utils_9pairqueue_PairQueue *)__pyx_v_queue->__pyx_vtab)->pop(__pyx_v_queue);
-    __pyx_t_10 = __pyx_t_8.f0;
-    __pyx_t_11 = __pyx_t_8.f1;
+    __pyx_t_10 = __pyx_v_pair.first;
+    __pyx_t_11 = __pyx_v_pair.second;
     __pyx_v_left = __pyx_t_10;
     __pyx_v_right = __pyx_t_11;
 
-    /* "ts2vg/graph/_horizontal.pyx":59
- *         (left, right) = queue.pop()
+    /* "ts2vg/graph/_horizontal.pyx":62
+ *         pair = queue.front()
+ *         left, right = pair.first, pair.second
+ *         queue.pop()             # <<<<<<<<<<<<<<
+ * 
+ *         if left+1 < right:
+ */
+    __pyx_v_queue.pop();
+
+    /* "ts2vg/graph/_horizontal.pyx":64
+ *         queue.pop()
  * 
  *         if left+1 < right:             # <<<<<<<<<<<<<<
  *             i = _argmax(ts, left, right)
  *             x_a = xs[i]
  */
     __pyx_t_9 = (((__pyx_v_left + 1) < __pyx_v_right) != 0);
     if (__pyx_t_9) {
 
-      /* "ts2vg/graph/_horizontal.pyx":60
+      /* "ts2vg/graph/_horizontal.pyx":65
  * 
  *         if left+1 < right:
  *             i = _argmax(ts, left, right)             # <<<<<<<<<<<<<<
  *             x_a = xs[i]
  *             y_a = ts[i]
  */
       __pyx_v_i = __pyx_f_5ts2vg_5graph_5_base__argmax(__pyx_v_ts, __pyx_v_left, __pyx_v_right);
 
-      /* "ts2vg/graph/_horizontal.pyx":61
+      /* "ts2vg/graph/_horizontal.pyx":66
  *         if left+1 < right:
  *             i = _argmax(ts, left, right)
  *             x_a = xs[i]             # <<<<<<<<<<<<<<
  *             y_a = ts[i]
  * 
  */
       __pyx_t_12 = __pyx_v_i;
       __pyx_v_x_a = (*((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_xs.data + __pyx_t_12 * __pyx_v_xs.strides[0]) )));
 
-      /* "ts2vg/graph/_horizontal.pyx":62
+      /* "ts2vg/graph/_horizontal.pyx":67
  *             i = _argmax(ts, left, right)
  *             x_a = xs[i]
  *             y_a = ts[i]             # <<<<<<<<<<<<<<
  * 
  *             # sweep from i towards the left
  */
       __pyx_t_12 = __pyx_v_i;
       __pyx_v_y_a = (*((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_ts.data + __pyx_t_12 * __pyx_v_ts.strides[0]) )));
 
-      /* "ts2vg/graph/_horizontal.pyx":65
+      /* "ts2vg/graph/_horizontal.pyx":70
  * 
  *             # sweep from i towards the left
  *             max_y = -INFINITY             # <<<<<<<<<<<<<<
  *             for d in range(1, i-left+1):
  *                 x_b = xs[i-d]
  */
       __pyx_v_max_y = (-INFINITY);
 
-      /* "ts2vg/graph/_horizontal.pyx":66
+      /* "ts2vg/graph/_horizontal.pyx":71
  *             # sweep from i towards the left
  *             max_y = -INFINITY
  *             for d in range(1, i-left+1):             # <<<<<<<<<<<<<<
  *                 x_b = xs[i-d]
  *                 y_b = ts[i-d]
  */
       __pyx_t_13 = ((__pyx_v_i - __pyx_v_left) + 1);
       __pyx_t_14 = __pyx_t_13;
       for (__pyx_t_3 = 1; __pyx_t_3 < __pyx_t_14; __pyx_t_3+=1) {
         __pyx_v_d = __pyx_t_3;
 
-        /* "ts2vg/graph/_horizontal.pyx":67
+        /* "ts2vg/graph/_horizontal.pyx":72
  *             max_y = -INFINITY
  *             for d in range(1, i-left+1):
  *                 x_b = xs[i-d]             # <<<<<<<<<<<<<<
  *                 y_b = ts[i-d]
  * 
  */
         __pyx_t_12 = (__pyx_v_i - __pyx_v_d);
         __pyx_v_x_b = (*((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_xs.data + __pyx_t_12 * __pyx_v_xs.strides[0]) )));
 
-        /* "ts2vg/graph/_horizontal.pyx":68
+        /* "ts2vg/graph/_horizontal.pyx":73
  *             for d in range(1, i-left+1):
  *                 x_b = xs[i-d]
  *                 y_b = ts[i-d]             # <<<<<<<<<<<<<<
  * 
  *                 if y_b > max_y:
  */
         __pyx_t_12 = (__pyx_v_i - __pyx_v_d);
         __pyx_v_y_b = (*((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_ts.data + __pyx_t_12 * __pyx_v_ts.strides[0]) )));
 
-        /* "ts2vg/graph/_horizontal.pyx":70
+        /* "ts2vg/graph/_horizontal.pyx":75
  *                 y_b = ts[i-d]
  * 
  *                 if y_b > max_y:             # <<<<<<<<<<<<<<
  *                     if directed == _DIRECTED_TOP_TO_BOTTOM:
  *                         add_edge(i, i-d, x_a, x_b, y_a, y_b)
  */
         __pyx_t_9 = ((__pyx_v_y_b > __pyx_v_max_y) != 0);
         if (__pyx_t_9) {
 
-          /* "ts2vg/graph/_horizontal.pyx":71
+          /* "ts2vg/graph/_horizontal.pyx":76
  * 
  *                 if y_b > max_y:
  *                     if directed == _DIRECTED_TOP_TO_BOTTOM:             # <<<<<<<<<<<<<<
  *                         add_edge(i, i-d, x_a, x_b, y_a, y_b)
  *                     else:  # left_to_right
  */
           __pyx_t_9 = ((__pyx_v_directed == __pyx_v_5ts2vg_5graph_11_horizontal__DIRECTED_TOP_TO_BOTTOM) != 0);
           if (__pyx_t_9) {
 
-            /* "ts2vg/graph/_horizontal.pyx":72
+            /* "ts2vg/graph/_horizontal.pyx":77
  *                 if y_b > max_y:
  *                     if directed == _DIRECTED_TOP_TO_BOTTOM:
  *                         add_edge(i, i-d, x_a, x_b, y_a, y_b)             # <<<<<<<<<<<<<<
  *                     else:  # left_to_right
  *                         add_edge(i-d, i, x_b, x_a, y_b, y_a)
  */
-            __pyx_t_5 = __pyx_pf_5ts2vg_5graph_11_horizontal_14_compute_graph_add_edge(__pyx_v_add_edge, __pyx_v_i, (__pyx_v_i - __pyx_v_d), __pyx_v_x_a, __pyx_v_x_b, __pyx_v_y_a, __pyx_v_y_b); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 72, __pyx_L1_error)
+            __pyx_t_5 = __pyx_pf_5ts2vg_5graph_11_horizontal_14_compute_graph_add_edge(__pyx_v_add_edge, __pyx_v_i, (__pyx_v_i - __pyx_v_d), __pyx_v_x_a, __pyx_v_x_b, __pyx_v_y_a, __pyx_v_y_b); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 77, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_5);
             __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-            /* "ts2vg/graph/_horizontal.pyx":71
+            /* "ts2vg/graph/_horizontal.pyx":76
  * 
  *                 if y_b > max_y:
  *                     if directed == _DIRECTED_TOP_TO_BOTTOM:             # <<<<<<<<<<<<<<
  *                         add_edge(i, i-d, x_a, x_b, y_a, y_b)
  *                     else:  # left_to_right
  */
             goto __pyx_L9;
           }
 
-          /* "ts2vg/graph/_horizontal.pyx":74
+          /* "ts2vg/graph/_horizontal.pyx":79
  *                         add_edge(i, i-d, x_a, x_b, y_a, y_b)
  *                     else:  # left_to_right
  *                         add_edge(i-d, i, x_b, x_a, y_b, y_a)             # <<<<<<<<<<<<<<
  * 
  *                     max_y = y_b
  */
           /*else*/ {
-            __pyx_t_5 = __pyx_pf_5ts2vg_5graph_11_horizontal_14_compute_graph_add_edge(__pyx_v_add_edge, (__pyx_v_i - __pyx_v_d), __pyx_v_i, __pyx_v_x_b, __pyx_v_x_a, __pyx_v_y_b, __pyx_v_y_a); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 74, __pyx_L1_error)
+            __pyx_t_5 = __pyx_pf_5ts2vg_5graph_11_horizontal_14_compute_graph_add_edge(__pyx_v_add_edge, (__pyx_v_i - __pyx_v_d), __pyx_v_i, __pyx_v_x_b, __pyx_v_x_a, __pyx_v_y_b, __pyx_v_y_a); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 79, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_5);
             __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           }
           __pyx_L9:;
 
-          /* "ts2vg/graph/_horizontal.pyx":76
+          /* "ts2vg/graph/_horizontal.pyx":81
  *                         add_edge(i-d, i, x_b, x_a, y_b, y_a)
  * 
  *                     max_y = y_b             # <<<<<<<<<<<<<<
  * 
  *             # sweep from i towards the right
  */
           __pyx_v_max_y = __pyx_v_y_b;
 
-          /* "ts2vg/graph/_horizontal.pyx":70
+          /* "ts2vg/graph/_horizontal.pyx":75
  *                 y_b = ts[i-d]
  * 
  *                 if y_b > max_y:             # <<<<<<<<<<<<<<
  *                     if directed == _DIRECTED_TOP_TO_BOTTOM:
  *                         add_edge(i, i-d, x_a, x_b, y_a, y_b)
  */
         }
       }
 
-      /* "ts2vg/graph/_horizontal.pyx":79
+      /* "ts2vg/graph/_horizontal.pyx":84
  * 
  *             # sweep from i towards the right
  *             max_y = -INFINITY             # <<<<<<<<<<<<<<
  *             for d in range(1, right-i):
  *                 x_b = xs[i+d]
  */
       __pyx_v_max_y = (-INFINITY);
 
-      /* "ts2vg/graph/_horizontal.pyx":80
+      /* "ts2vg/graph/_horizontal.pyx":85
  *             # sweep from i towards the right
  *             max_y = -INFINITY
  *             for d in range(1, right-i):             # <<<<<<<<<<<<<<
  *                 x_b = xs[i+d]
  *                 y_b = ts[i+d]
  */
       __pyx_t_3 = (__pyx_v_right - __pyx_v_i);
       __pyx_t_15 = __pyx_t_3;
       for (__pyx_t_16 = 1; __pyx_t_16 < __pyx_t_15; __pyx_t_16+=1) {
         __pyx_v_d = __pyx_t_16;
 
-        /* "ts2vg/graph/_horizontal.pyx":81
+        /* "ts2vg/graph/_horizontal.pyx":86
  *             max_y = -INFINITY
  *             for d in range(1, right-i):
  *                 x_b = xs[i+d]             # <<<<<<<<<<<<<<
  *                 y_b = ts[i+d]
  * 
  */
         __pyx_t_12 = (__pyx_v_i + __pyx_v_d);
         __pyx_v_x_b = (*((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_xs.data + __pyx_t_12 * __pyx_v_xs.strides[0]) )));
 
-        /* "ts2vg/graph/_horizontal.pyx":82
+        /* "ts2vg/graph/_horizontal.pyx":87
  *             for d in range(1, right-i):
  *                 x_b = xs[i+d]
  *                 y_b = ts[i+d]             # <<<<<<<<<<<<<<
  * 
  *                 if y_b > max_y:
  */
         __pyx_t_12 = (__pyx_v_i + __pyx_v_d);
         __pyx_v_y_b = (*((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_ts.data + __pyx_t_12 * __pyx_v_ts.strides[0]) )));
 
-        /* "ts2vg/graph/_horizontal.pyx":84
+        /* "ts2vg/graph/_horizontal.pyx":89
  *                 y_b = ts[i+d]
  * 
  *                 if y_b > max_y:             # <<<<<<<<<<<<<<
  *                     # note, single case works for both top_to_bottom and left_to_right orders
  *                     add_edge(i, i+d, x_a, x_b, y_a, y_b)
  */
         __pyx_t_9 = ((__pyx_v_y_b > __pyx_v_max_y) != 0);
         if (__pyx_t_9) {
 
-          /* "ts2vg/graph/_horizontal.pyx":86
+          /* "ts2vg/graph/_horizontal.pyx":91
  *                 if y_b > max_y:
  *                     # note, single case works for both top_to_bottom and left_to_right orders
  *                     add_edge(i, i+d, x_a, x_b, y_a, y_b)             # <<<<<<<<<<<<<<
  * 
  *                     max_y = y_b
  */
-          __pyx_t_5 = __pyx_pf_5ts2vg_5graph_11_horizontal_14_compute_graph_add_edge(__pyx_v_add_edge, __pyx_v_i, (__pyx_v_i + __pyx_v_d), __pyx_v_x_a, __pyx_v_x_b, __pyx_v_y_a, __pyx_v_y_b); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 86, __pyx_L1_error)
+          __pyx_t_5 = __pyx_pf_5ts2vg_5graph_11_horizontal_14_compute_graph_add_edge(__pyx_v_add_edge, __pyx_v_i, (__pyx_v_i + __pyx_v_d), __pyx_v_x_a, __pyx_v_x_b, __pyx_v_y_a, __pyx_v_y_b); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-          /* "ts2vg/graph/_horizontal.pyx":88
+          /* "ts2vg/graph/_horizontal.pyx":93
  *                     add_edge(i, i+d, x_a, x_b, y_a, y_b)
  * 
  *                     max_y = y_b             # <<<<<<<<<<<<<<
  * 
- *             queue.push((left, i))
+ *             queue.push(uint_pair(left, i))
  */
           __pyx_v_max_y = __pyx_v_y_b;
 
-          /* "ts2vg/graph/_horizontal.pyx":84
+          /* "ts2vg/graph/_horizontal.pyx":89
  *                 y_b = ts[i+d]
  * 
  *                 if y_b > max_y:             # <<<<<<<<<<<<<<
  *                     # note, single case works for both top_to_bottom and left_to_right orders
  *                     add_edge(i, i+d, x_a, x_b, y_a, y_b)
  */
         }
       }
 
-      /* "ts2vg/graph/_horizontal.pyx":90
+      /* "ts2vg/graph/_horizontal.pyx":95
  *                     max_y = y_b
  * 
- *             queue.push((left, i))             # <<<<<<<<<<<<<<
- *             queue.push((i+1, right))
+ *             queue.push(uint_pair(left, i))             # <<<<<<<<<<<<<<
+ *             queue.push(uint_pair(i+1, right))
  * 
  */
-      __pyx_t_8.f0 = __pyx_v_left;
-      __pyx_t_8.f1 = __pyx_v_i;
-      ((struct __pyx_vtabstruct_5ts2vg_5utils_9pairqueue_PairQueue *)__pyx_v_queue->__pyx_vtab)->push(__pyx_v_queue, __pyx_t_8);
+      try {
+        __pyx_t_8 = __pyx_t_5ts2vg_5graph_11_horizontal_uint_pair(__pyx_v_left, __pyx_v_i);
+      } catch(...) {
+        __Pyx_CppExn2PyErr();
+        __PYX_ERR(0, 95, __pyx_L1_error)
+      }
+      __pyx_v_queue.push(__pyx_t_8);
 
-      /* "ts2vg/graph/_horizontal.pyx":91
+      /* "ts2vg/graph/_horizontal.pyx":96
  * 
- *             queue.push((left, i))
- *             queue.push((i+1, right))             # <<<<<<<<<<<<<<
+ *             queue.push(uint_pair(left, i))
+ *             queue.push(uint_pair(i+1, right))             # <<<<<<<<<<<<<<
  * 
  *     return edges, np.asarray(degrees_in, dtype=np.uint32), np.asarray(degrees_out, dtype=np.uint32)
  */
-      __pyx_t_8.f0 = (__pyx_v_i + 1);
-      __pyx_t_8.f1 = __pyx_v_right;
-      ((struct __pyx_vtabstruct_5ts2vg_5utils_9pairqueue_PairQueue *)__pyx_v_queue->__pyx_vtab)->push(__pyx_v_queue, __pyx_t_8);
+      try {
+        __pyx_t_8 = __pyx_t_5ts2vg_5graph_11_horizontal_uint_pair((__pyx_v_i + 1), __pyx_v_right);
+      } catch(...) {
+        __Pyx_CppExn2PyErr();
+        __PYX_ERR(0, 96, __pyx_L1_error)
+      }
+      __pyx_v_queue.push(__pyx_t_8);
 
-      /* "ts2vg/graph/_horizontal.pyx":59
- *         (left, right) = queue.pop()
+      /* "ts2vg/graph/_horizontal.pyx":64
+ *         queue.pop()
  * 
  *         if left+1 < right:             # <<<<<<<<<<<<<<
  *             i = _argmax(ts, left, right)
  *             x_a = xs[i]
  */
     }
   }
 
-  /* "ts2vg/graph/_horizontal.pyx":93
- *             queue.push((i+1, right))
+  /* "ts2vg/graph/_horizontal.pyx":98
+ *             queue.push(uint_pair(i+1, right))
  * 
  *     return edges, np.asarray(degrees_in, dtype=np.uint32), np.asarray(degrees_out, dtype=np.uint32)             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_asarray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_asarray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __pyx_memoryview_fromslice(__pyx_cur_scope->__pyx_v_degrees_in, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint32_t, 0);; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_5 = __pyx_memoryview_fromslice(__pyx_cur_scope->__pyx_v_degrees_in, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint32_t, 0);; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_asarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_asarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __pyx_memoryview_fromslice(__pyx_cur_scope->__pyx_v_degrees_out, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint32_t, 0);; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_5 = __pyx_memoryview_fromslice(__pyx_cur_scope->__pyx_v_degrees_out, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint32_t, 0);; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_17 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint32); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_17 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint32); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_17) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_17) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-  __pyx_t_17 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_17 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_edges);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_edges);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_cur_scope->__pyx_v_edges);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_17);
   PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_17);
   __pyx_t_1 = 0;
   __pyx_t_17 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "ts2vg/graph/_horizontal.pyx":21
+  /* "ts2vg/graph/_horizontal.pyx":24
  * @cython.wraparound(False)
  * @cython.cdivision(True)
  * def _compute_graph(np.float64_t[:] ts, np.float64_t[:] xs, uint directed, uint weighted, bint only_degrees, double min_weight, double max_weight):             # <<<<<<<<<<<<<<
  *     """
  *     Computes the horizontal visibility graph of a time series
  */
 
@@ -4003,25 +4032,24 @@
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __PYX_XDEC_MEMVIEW(&__pyx_t_7, 1);
   __Pyx_XDECREF(__pyx_t_17);
   __Pyx_AddTraceback("ts2vg.graph._horizontal._compute_graph", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_queue);
   __Pyx_XDECREF(__pyx_v_add_edge);
   __PYX_XDEC_MEMVIEW(&__pyx_v_ts, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_xs, 1);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4030,29 +4058,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4063,15 +4091,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4080,29 +4108,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4113,15 +4141,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4130,29 +4158,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4163,15 +4191,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4180,29 +4208,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4213,15 +4241,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4230,29 +4258,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4263,212 +4291,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4484,15 +4512,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4500,53 +4528,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -4554,30 +4582,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4592,15 +4620,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4616,15 +4644,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4632,53 +4660,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -4686,30 +4714,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4724,15 +4752,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4748,15 +4776,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4764,53 +4792,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -4818,30 +4846,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4856,176 +4884,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19052,14 +19080,15 @@
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
   {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
   {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
   {&__pyx_n_s_only_degrees, __pyx_k_only_degrees, sizeof(__pyx_k_only_degrees), 0, 0, 1, 1},
   {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
+  {&__pyx_n_s_pair, __pyx_k_pair, sizeof(__pyx_k_pair), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_getbuffer, __pyx_k_pyx_getbuffer, sizeof(__pyx_k_pyx_getbuffer), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
@@ -19106,15 +19135,15 @@
   {&__pyx_n_s_y2, __pyx_k_y2, sizeof(__pyx_k_y2), 0, 0, 1, 1},
   {&__pyx_n_s_y_a, __pyx_k_y_a, sizeof(__pyx_k_y_a), 0, 0, 1, 1},
   {&__pyx_n_s_y_b, __pyx_k_y_b, sizeof(__pyx_k_y_b), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 71, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 134, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 152, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 615, __pyx_L1_error)
@@ -19124,38 +19153,38 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "ts2vg/graph/_horizontal.pyx":40
- *     queue.push((0, n))
+  /* "ts2vg/graph/_horizontal.pyx":43
+ *     queue.push(uint_pair(0, n))
  * 
  *     def add_edge(uint i1, uint i2, double x1, double x2, double y1, double y2):             # <<<<<<<<<<<<<<
  *         w = weight_func(x1, x2, y1, y2, NAN)
  * 
  */
-  __pyx_tuple_ = PyTuple_Pack(7, __pyx_n_s_i1, __pyx_n_s_i2, __pyx_n_s_x1, __pyx_n_s_x2, __pyx_n_s_y1, __pyx_n_s_y2, __pyx_n_s_w); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(7, __pyx_n_s_i1, __pyx_n_s_i2, __pyx_n_s_x1, __pyx_n_s_x2, __pyx_n_s_y1, __pyx_n_s_y2, __pyx_n_s_w); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
-  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(6, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ts2vg_graph__horizontal_pyx, __pyx_n_s_add_edge, 40, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(6, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ts2vg_graph__horizontal_pyx, __pyx_n_s_add_edge, 43, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 43, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 950, __pyx_L1_error)
@@ -19353,25 +19382,25 @@
   __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
   __pyx_tuple__23 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
 
-  /* "ts2vg/graph/_horizontal.pyx":21
+  /* "ts2vg/graph/_horizontal.pyx":24
  * @cython.wraparound(False)
  * @cython.cdivision(True)
  * def _compute_graph(np.float64_t[:] ts, np.float64_t[:] xs, uint directed, uint weighted, bint only_degrees, double min_weight, double max_weight):             # <<<<<<<<<<<<<<
  *     """
  *     Computes the horizontal visibility graph of a time series
  */
-  __pyx_tuple__24 = PyTuple_Pack(25, __pyx_n_s_ts, __pyx_n_s_xs, __pyx_n_s_directed, __pyx_n_s_weighted, __pyx_n_s_only_degrees, __pyx_n_s_min_weight, __pyx_n_s_max_weight, __pyx_n_s_n, __pyx_n_s_edges, __pyx_n_s_degrees_in, __pyx_n_s_degrees_out, __pyx_n_s_left, __pyx_n_s_right, __pyx_n_s_i, __pyx_n_s_d, __pyx_n_s_x_a, __pyx_n_s_x_b, __pyx_n_s_y_a, __pyx_n_s_y_b, __pyx_n_s_max_y, __pyx_n_s_w, __pyx_n_s_weight_func, __pyx_n_s_queue, __pyx_n_s_add_edge, __pyx_n_s_add_edge); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(26, __pyx_n_s_ts, __pyx_n_s_xs, __pyx_n_s_directed, __pyx_n_s_weighted, __pyx_n_s_only_degrees, __pyx_n_s_min_weight, __pyx_n_s_max_weight, __pyx_n_s_n, __pyx_n_s_edges, __pyx_n_s_degrees_in, __pyx_n_s_degrees_out, __pyx_n_s_left, __pyx_n_s_right, __pyx_n_s_i, __pyx_n_s_d, __pyx_n_s_x_a, __pyx_n_s_x_b, __pyx_n_s_y_a, __pyx_n_s_y_b, __pyx_n_s_max_y, __pyx_n_s_w, __pyx_n_s_weight_func, __pyx_n_s_queue, __pyx_n_s_add_edge, __pyx_n_s_add_edge, __pyx_n_s_pair); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(7, 0, 25, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ts2vg_graph__horizontal_pyx, __pyx_n_s_compute_graph, 21, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(7, 0, 26, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ts2vg_graph__horizontal_pyx, __pyx_n_s_compute_graph, 24, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 24, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
@@ -19493,15 +19522,15 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_5ts2vg_5graph_11_horizontal___pyx_scope_struct___compute_graph) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_5ts2vg_5graph_11_horizontal___pyx_scope_struct___compute_graph) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_5ts2vg_5graph_11_horizontal___pyx_scope_struct___compute_graph.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_5ts2vg_5graph_11_horizontal___pyx_scope_struct___compute_graph.tp_dictoffset && __pyx_type_5ts2vg_5graph_11_horizontal___pyx_scope_struct___compute_graph.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_5ts2vg_5graph_11_horizontal___pyx_scope_struct___compute_graph.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_5ts2vg_5graph_11_horizontal___pyx_scope_struct___compute_graph = &__pyx_type_5ts2vg_5graph_11_horizontal___pyx_scope_struct___compute_graph;
@@ -19571,60 +19600,69 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("ts2vg.utils.pairqueue"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 15, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5ts2vg_5utils_9pairqueue_PairQueue = __Pyx_ImportType(__pyx_t_1, "ts2vg.utils.pairqueue", "PairQueue", sizeof(struct __pyx_obj_5ts2vg_5utils_9pairqueue_PairQueue), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5ts2vg_5utils_9pairqueue_PairQueue) __PYX_ERR(4, 15, __pyx_L1_error)
-  __pyx_vtabptr_5ts2vg_5utils_9pairqueue_PairQueue = (struct __pyx_vtabstruct_5ts2vg_5utils_9pairqueue_PairQueue*)__Pyx_GetVtable(__pyx_ptype_5ts2vg_5utils_9pairqueue_PairQueue->tp_dict); if (unlikely(!__pyx_vtabptr_5ts2vg_5utils_9pairqueue_PairQueue)) __PYX_ERR(4, 15, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -19857,95 +19895,95 @@
   (void)__Pyx_modinit_variable_import_code();
   if (unlikely(__Pyx_modinit_function_import_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "ts2vg/graph/_horizontal.pyx":4
+  /* "ts2vg/graph/_horizontal.pyx":5
  * 
  * cimport cython
  * import numpy as np             # <<<<<<<<<<<<<<
  * cimport numpy as np
  * from libc.math cimport INFINITY, NAN
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "ts2vg/graph/_horizontal.pyx":9
+  /* "ts2vg/graph/_horizontal.pyx":11
+ * from libcpp.pair cimport pair as cpair
  * 
- * from ts2vg.utils.pairqueue cimport PairQueue
  * from ts2vg.graph.base import _DIRECTED_OPTIONS             # <<<<<<<<<<<<<<
  * from ts2vg.graph._base cimport _argmax, _get_weight_func, weight_func_type
  * 
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_DIRECTED_OPTIONS);
   __Pyx_GIVEREF(__pyx_n_s_DIRECTED_OPTIONS);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_DIRECTED_OPTIONS);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_ts2vg_graph_base, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_ts2vg_graph_base, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_DIRECTED_OPTIONS); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_DIRECTED_OPTIONS); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_DIRECTED_OPTIONS, __pyx_t_1) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_DIRECTED_OPTIONS, __pyx_t_1) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "ts2vg/graph/_horizontal.pyx":14
- * ctypedef unsigned int uint
+  /* "ts2vg/graph/_horizontal.pyx":17
+ * ctypedef cpair[uint, uint] uint_pair
  * 
  * cdef uint _DIRECTED_LEFT_TO_RIGHT = _DIRECTED_OPTIONS['left_to_right']             # <<<<<<<<<<<<<<
  * cdef uint _DIRECTED_TOP_TO_BOTTOM = _DIRECTED_OPTIONS['top_to_bottom']
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DIRECTED_OPTIONS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DIRECTED_OPTIONS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_2, __pyx_n_u_left_to_right); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_2, __pyx_n_u_left_to_right); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __Pyx_PyInt_As_unsigned_int(__pyx_t_1); if (unlikely((__pyx_t_3 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_unsigned_int(__pyx_t_1); if (unlikely((__pyx_t_3 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_5ts2vg_5graph_11_horizontal__DIRECTED_LEFT_TO_RIGHT = __pyx_t_3;
 
-  /* "ts2vg/graph/_horizontal.pyx":15
+  /* "ts2vg/graph/_horizontal.pyx":18
  * 
  * cdef uint _DIRECTED_LEFT_TO_RIGHT = _DIRECTED_OPTIONS['left_to_right']
  * cdef uint _DIRECTED_TOP_TO_BOTTOM = _DIRECTED_OPTIONS['top_to_bottom']             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DIRECTED_OPTIONS); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DIRECTED_OPTIONS); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_top_to_bottom); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_top_to_bottom); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyInt_As_unsigned_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_unsigned_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_5ts2vg_5graph_11_horizontal__DIRECTED_TOP_TO_BOTTOM = __pyx_t_3;
 
-  /* "ts2vg/graph/_horizontal.pyx":21
+  /* "ts2vg/graph/_horizontal.pyx":24
  * @cython.wraparound(False)
  * @cython.cdivision(True)
  * def _compute_graph(np.float64_t[:] ts, np.float64_t[:] xs, uint directed, uint weighted, bint only_degrees, double min_weight, double max_weight):             # <<<<<<<<<<<<<<
  *     """
  *     Computes the horizontal visibility graph of a time series
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5ts2vg_5graph_11_horizontal_1_compute_graph, NULL, __pyx_n_s_ts2vg_graph__horizontal); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5ts2vg_5graph_11_horizontal_1_compute_graph, NULL, __pyx_n_s_ts2vg_graph__horizontal); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compute_graph, __pyx_t_2) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compute_graph, __pyx_t_2) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "ts2vg/graph/_horizontal.pyx":1
  * #cython: language_level=3             # <<<<<<<<<<<<<<
+ * #distutils: language=c++
  * 
- * cimport cython
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "View.MemoryView":210
@@ -20396,175 +20434,14 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
-/* PyFunctionFastCall */
-#if CYTHON_FAST_PYCALL
-static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
-                                               PyObject *globals) {
-    PyFrameObject *f;
-    PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject **fastlocals;
-    Py_ssize_t i;
-    PyObject *result;
-    assert(globals != NULL);
-    /* XXX Perhaps we should create a specialized
-       PyFrame_New() that doesn't take locals, but does
-       take builtins without sanity checking them.
-       */
-    assert(tstate != NULL);
-    f = PyFrame_New(tstate, co, globals, NULL);
-    if (f == NULL) {
-        return NULL;
-    }
-    fastlocals = __Pyx_PyFrame_GetLocalsplus(f);
-    for (i = 0; i < na; i++) {
-        Py_INCREF(*args);
-        fastlocals[i] = *args++;
-    }
-    result = PyEval_EvalFrameEx(f,0);
-    ++tstate->recursion_depth;
-    Py_DECREF(f);
-    --tstate->recursion_depth;
-    return result;
-}
-#if 1 || PY_VERSION_HEX < 0x030600B1
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
-    PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
-    PyObject *globals = PyFunction_GET_GLOBALS(func);
-    PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
-    PyObject *closure;
-#if PY_MAJOR_VERSION >= 3
-    PyObject *kwdefs;
-#endif
-    PyObject *kwtuple, **k;
-    PyObject **d;
-    Py_ssize_t nd;
-    Py_ssize_t nk;
-    PyObject *result;
-    assert(kwargs == NULL || PyDict_Check(kwargs));
-    nk = kwargs ? PyDict_Size(kwargs) : 0;
-    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
-        return NULL;
-    }
-    if (
-#if PY_MAJOR_VERSION >= 3
-            co->co_kwonlyargcount == 0 &&
-#endif
-            likely(kwargs == NULL || nk == 0) &&
-            co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
-        if (argdefs == NULL && co->co_argcount == nargs) {
-            result = __Pyx_PyFunction_FastCallNoKw(co, args, nargs, globals);
-            goto done;
-        }
-        else if (nargs == 0 && argdefs != NULL
-                 && co->co_argcount == Py_SIZE(argdefs)) {
-            /* function called with no arguments, but all parameters have
-               a default value: use default values as arguments .*/
-            args = &PyTuple_GET_ITEM(argdefs, 0);
-            result =__Pyx_PyFunction_FastCallNoKw(co, args, Py_SIZE(argdefs), globals);
-            goto done;
-        }
-    }
-    if (kwargs != NULL) {
-        Py_ssize_t pos, i;
-        kwtuple = PyTuple_New(2 * nk);
-        if (kwtuple == NULL) {
-            result = NULL;
-            goto done;
-        }
-        k = &PyTuple_GET_ITEM(kwtuple, 0);
-        pos = i = 0;
-        while (PyDict_Next(kwargs, &pos, &k[i], &k[i+1])) {
-            Py_INCREF(k[i]);
-            Py_INCREF(k[i+1]);
-            i += 2;
-        }
-        nk = i / 2;
-    }
-    else {
-        kwtuple = NULL;
-        k = NULL;
-    }
-    closure = PyFunction_GET_CLOSURE(func);
-#if PY_MAJOR_VERSION >= 3
-    kwdefs = PyFunction_GET_KW_DEFAULTS(func);
-#endif
-    if (argdefs != NULL) {
-        d = &PyTuple_GET_ITEM(argdefs, 0);
-        nd = Py_SIZE(argdefs);
-    }
-    else {
-        d = NULL;
-        nd = 0;
-    }
-#if PY_MAJOR_VERSION >= 3
-    result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
-                               args, (int)nargs,
-                               k, (int)nk,
-                               d, (int)nd, kwdefs, closure);
-#else
-    result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
-                               args, (int)nargs,
-                               k, (int)nk,
-                               d, (int)nd, closure);
-#endif
-    Py_XDECREF(kwtuple);
-done:
-    Py_LeaveRecursiveCall();
-    return result;
-}
-#endif
-#endif
-
-/* PyObjectCallMethO */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
-    PyObject *self, *result;
-    PyCFunction cfunc;
-    cfunc = PyCFunction_GET_FUNCTION(func);
-    self = PyCFunction_GET_SELF(func);
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    result = cfunc(self, arg);
-    Py_LeaveRecursiveCall();
-    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
-        PyErr_SetString(
-            PyExc_SystemError,
-            "NULL result without error in PyObject_Call");
-    }
-    return result;
-}
-#endif
-
-/* PyObjectCallNoArg */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, NULL, 0);
-    }
-#endif
-#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
-    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
-#else
-    if (likely(PyCFunction_Check(func)))
-#endif
-    {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-            return __Pyx_PyObject_CallMethO(func, NULL);
-        }
-    }
-    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
-}
-#endif
-
 /* FetchCommonType */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
     PyObject* fake_module;
     PyTypeObject* cached_type = NULL;
     fake_module = PyImport_AddModule((char*) "_cython_" CYTHON_ABI);
     if (!fake_module) return NULL;
     Py_INCREF(fake_module);
@@ -21673,28 +21550,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -21739,14 +21616,133 @@
         return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
     } else {
         return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
     }
 }
 #endif
 
+/* PyFunctionFastCall */
+#if CYTHON_FAST_PYCALL
+static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
+                                               PyObject *globals) {
+    PyFrameObject *f;
+    PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject **fastlocals;
+    Py_ssize_t i;
+    PyObject *result;
+    assert(globals != NULL);
+    /* XXX Perhaps we should create a specialized
+       PyFrame_New() that doesn't take locals, but does
+       take builtins without sanity checking them.
+       */
+    assert(tstate != NULL);
+    f = PyFrame_New(tstate, co, globals, NULL);
+    if (f == NULL) {
+        return NULL;
+    }
+    fastlocals = __Pyx_PyFrame_GetLocalsplus(f);
+    for (i = 0; i < na; i++) {
+        Py_INCREF(*args);
+        fastlocals[i] = *args++;
+    }
+    result = PyEval_EvalFrameEx(f,0);
+    ++tstate->recursion_depth;
+    Py_DECREF(f);
+    --tstate->recursion_depth;
+    return result;
+}
+#if 1 || PY_VERSION_HEX < 0x030600B1
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
+    PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
+    PyObject *globals = PyFunction_GET_GLOBALS(func);
+    PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
+    PyObject *closure;
+#if PY_MAJOR_VERSION >= 3
+    PyObject *kwdefs;
+#endif
+    PyObject *kwtuple, **k;
+    PyObject **d;
+    Py_ssize_t nd;
+    Py_ssize_t nk;
+    PyObject *result;
+    assert(kwargs == NULL || PyDict_Check(kwargs));
+    nk = kwargs ? PyDict_Size(kwargs) : 0;
+    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
+        return NULL;
+    }
+    if (
+#if PY_MAJOR_VERSION >= 3
+            co->co_kwonlyargcount == 0 &&
+#endif
+            likely(kwargs == NULL || nk == 0) &&
+            co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
+        if (argdefs == NULL && co->co_argcount == nargs) {
+            result = __Pyx_PyFunction_FastCallNoKw(co, args, nargs, globals);
+            goto done;
+        }
+        else if (nargs == 0 && argdefs != NULL
+                 && co->co_argcount == Py_SIZE(argdefs)) {
+            /* function called with no arguments, but all parameters have
+               a default value: use default values as arguments .*/
+            args = &PyTuple_GET_ITEM(argdefs, 0);
+            result =__Pyx_PyFunction_FastCallNoKw(co, args, Py_SIZE(argdefs), globals);
+            goto done;
+        }
+    }
+    if (kwargs != NULL) {
+        Py_ssize_t pos, i;
+        kwtuple = PyTuple_New(2 * nk);
+        if (kwtuple == NULL) {
+            result = NULL;
+            goto done;
+        }
+        k = &PyTuple_GET_ITEM(kwtuple, 0);
+        pos = i = 0;
+        while (PyDict_Next(kwargs, &pos, &k[i], &k[i+1])) {
+            Py_INCREF(k[i]);
+            Py_INCREF(k[i+1]);
+            i += 2;
+        }
+        nk = i / 2;
+    }
+    else {
+        kwtuple = NULL;
+        k = NULL;
+    }
+    closure = PyFunction_GET_CLOSURE(func);
+#if PY_MAJOR_VERSION >= 3
+    kwdefs = PyFunction_GET_KW_DEFAULTS(func);
+#endif
+    if (argdefs != NULL) {
+        d = &PyTuple_GET_ITEM(argdefs, 0);
+        nd = Py_SIZE(argdefs);
+    }
+    else {
+        d = NULL;
+        nd = 0;
+    }
+#if PY_MAJOR_VERSION >= 3
+    result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
+                               args, (int)nargs,
+                               k, (int)nk,
+                               d, (int)nd, kwdefs, closure);
+#else
+    result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
+                               args, (int)nargs,
+                               k, (int)nk,
+                               d, (int)nd, closure);
+#endif
+    Py_XDECREF(kwtuple);
+done:
+    Py_LeaveRecursiveCall();
+    return result;
+}
+#endif
+#endif
+
 /* PyObjectCall2Args */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
     PyObject *args, *result = NULL;
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(function)) {
         PyObject *args[2] = {arg1, arg2};
         return __Pyx_PyFunction_FastCall(function, args, 2);
@@ -21768,14 +21764,34 @@
     result = __Pyx_PyObject_Call(function, args, NULL);
     Py_DECREF(args);
     Py_DECREF(function);
 done:
     return result;
 }
 
+/* PyObjectCallMethO */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
+    PyObject *self, *result;
+    PyCFunction cfunc;
+    cfunc = PyCFunction_GET_FUNCTION(func);
+    self = PyCFunction_GET_SELF(func);
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    result = cfunc(self, arg);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
+    }
+    return result;
+}
+#endif
+
 /* PyObjectCallOneArg */
 #if CYTHON_COMPILING_IN_CPYTHON
 static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
     PyObject *result;
     PyObject *args = PyTuple_New(1);
     if (unlikely(!args)) return NULL;
     Py_INCREF(arg);
@@ -22740,44 +22756,62 @@
     return ret;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
@@ -22797,34 +22831,14 @@
     return (PyTypeObject *)result;
 bad:
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
-/* GetVTable */
-static void* __Pyx_GetVtable(PyObject *dict) {
-    void* ptr;
-    PyObject *ob = PyObject_GetItem(dict, __pyx_n_s_pyx_vtable);
-    if (!ob)
-        goto bad;
-#if PY_VERSION_HEX >= 0x02070000
-    ptr = PyCapsule_GetPointer(ob, 0);
-#else
-    ptr = PyCObject_AsVoidPtr(ob);
-#endif
-    if (!ptr && !PyErr_Occurred())
-        PyErr_SetString(PyExc_RuntimeError, "invalid vtable found for imported type");
-    Py_DECREF(ob);
-    return ptr;
-bad:
-    Py_XDECREF(ob);
-    return NULL;
-}
-
 /* DictGetItem */
 #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
 static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
     PyObject *value;
     value = PyDict_GetItemWithError(d, key);
     if (unlikely(!value)) {
         if (!PyErr_Occurred()) {
```

### Comparing `ts2vg-1.2.1/ts2vg/graph/_horizontal_penetrable.c` & `ts2vg-1.2.2/ts2vg/graph/_horizontal_penetrable.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include"
         ],
         "name": "ts2vg.graph._horizontal_penetrable",
         "sources": [
             "ts2vg/graph/_horizontal_penetrable.pyx"
         ]
     },
     "module_name": "ts2vg.graph._horizontal_penetrable"
@@ -33,16 +33,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -227,15 +227,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -266,15 +266,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1120,195 +1120,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1358,42 +1358,42 @@
 /*--- Type declarations ---*/
 struct __pyx_obj_5ts2vg_5graph_22_horizontal_penetrable___pyx_scope_struct___compute_graph;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2122,20 +2122,28 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* DictGetItem.proto */
 #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
 static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
 #define __Pyx_PyObject_Dict_GetItem(obj, name)\
     (likely(PyDict_CheckExact(obj)) ?\
@@ -2535,15 +2543,14 @@
 static const char __pyx_k_x_a[] = "x_a";
 static const char __pyx_k_x_b[] = "x_b";
 static const char __pyx_k_y_a[] = "y_a";
 static const char __pyx_k_y_b[] = "y_b";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_full[] = "full";
-static const char __pyx_k_left[] = "left";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_mode[] = "mode";
 static const char __pyx_k_name[] = "name";
 static const char __pyx_k_ndim[] = "ndim";
 static const char __pyx_k_pack[] = "pack";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_step[] = "step";
@@ -2553,15 +2560,14 @@
 static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_edges[] = "edges";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_flags[] = "flags";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_range[] = "range";
-static const char __pyx_k_right[] = "right";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_zeros[] = "zeros";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_max_ys[] = "max_ys";
@@ -2714,15 +2720,14 @@
 static PyObject *__pyx_n_s_i_b;
 static PyObject *__pyx_n_s_id;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_itemsize;
 static PyObject *__pyx_kp_s_itemsize_0_for_cython_array;
 static PyObject *__pyx_n_s_j;
 static PyObject *__pyx_n_s_known_w;
-static PyObject *__pyx_n_s_left;
 static PyObject *__pyx_n_u_left_to_right;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_max_weight;
 static PyObject *__pyx_n_s_max_ys;
 static PyObject *__pyx_n_s_memview;
 static PyObject *__pyx_n_s_min_weight;
 static PyObject *__pyx_n_s_mode;
@@ -2750,15 +2755,14 @@
 static PyObject *__pyx_n_s_pyx_type;
 static PyObject *__pyx_n_s_pyx_unpickle_Enum;
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
-static PyObject *__pyx_n_s_right;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_shape;
 static PyObject *__pyx_n_s_size;
 static PyObject *__pyx_n_s_start;
 static PyObject *__pyx_n_s_step;
 static PyObject *__pyx_n_s_stop;
@@ -3529,15 +3533,15 @@
   __pyx_t_7.data = NULL;
 
   /* "ts2vg/graph/_horizontal_penetrable.pyx":34
  *     cdef list edges = []
  *     cdef np.uint32_t[:] degrees_in = np.zeros(n, dtype=np.uint32)
  *     cdef np.uint32_t[:] degrees_out = np.zeros(n, dtype=np.uint32)             # <<<<<<<<<<<<<<
  * 
- *     cdef uint left, right, i_a, i_b
+ *     cdef uint i_a, i_b
  */
   __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = __Pyx_PyInt_From_unsigned_int(__pyx_v_n); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 34, __pyx_L1_error)
@@ -4077,15 +4081,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_xs, 1);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4094,29 +4098,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4127,15 +4131,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4144,29 +4148,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4177,15 +4181,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4194,29 +4198,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4227,15 +4231,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4244,29 +4248,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4277,15 +4281,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4294,29 +4298,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4327,212 +4331,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4548,15 +4552,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4564,53 +4568,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -4618,30 +4622,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4656,15 +4660,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4680,15 +4684,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4696,53 +4700,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -4750,30 +4754,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4788,15 +4792,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4812,15 +4816,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4828,53 +4832,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -4882,30 +4886,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4920,176 +4924,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19100,15 +19104,14 @@
   {&__pyx_n_s_i_b, __pyx_k_i_b, sizeof(__pyx_k_i_b), 0, 0, 1, 1},
   {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_itemsize, __pyx_k_itemsize, sizeof(__pyx_k_itemsize), 0, 0, 1, 1},
   {&__pyx_kp_s_itemsize_0_for_cython_array, __pyx_k_itemsize_0_for_cython_array, sizeof(__pyx_k_itemsize_0_for_cython_array), 0, 0, 1, 0},
   {&__pyx_n_s_j, __pyx_k_j, sizeof(__pyx_k_j), 0, 0, 1, 1},
   {&__pyx_n_s_known_w, __pyx_k_known_w, sizeof(__pyx_k_known_w), 0, 0, 1, 1},
-  {&__pyx_n_s_left, __pyx_k_left, sizeof(__pyx_k_left), 0, 0, 1, 1},
   {&__pyx_n_u_left_to_right, __pyx_k_left_to_right, sizeof(__pyx_k_left_to_right), 0, 1, 0, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_max_weight, __pyx_k_max_weight, sizeof(__pyx_k_max_weight), 0, 0, 1, 1},
   {&__pyx_n_s_max_ys, __pyx_k_max_ys, sizeof(__pyx_k_max_ys), 0, 0, 1, 1},
   {&__pyx_n_s_memview, __pyx_k_memview, sizeof(__pyx_k_memview), 0, 0, 1, 1},
   {&__pyx_n_s_min_weight, __pyx_k_min_weight, sizeof(__pyx_k_min_weight), 0, 0, 1, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
@@ -19136,15 +19139,14 @@
   {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_Enum, __pyx_k_pyx_unpickle_Enum, sizeof(__pyx_k_pyx_unpickle_Enum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
-  {&__pyx_n_s_right, __pyx_k_right, sizeof(__pyx_k_right), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
   {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
   {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
   {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
   {&__pyx_n_s_stop, __pyx_k_stop, sizeof(__pyx_k_stop), 0, 0, 1, 1},
@@ -19208,26 +19210,26 @@
  *             w = weight_func(x1, x2, y1, y2, NAN)
  */
   __pyx_tuple_ = PyTuple_Pack(8, __pyx_n_s_i1, __pyx_n_s_i2, __pyx_n_s_x1, __pyx_n_s_x2, __pyx_n_s_y1, __pyx_n_s_y2, __pyx_n_s_known_w, __pyx_n_s_w); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
   __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(7, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ts2vg_graph__horizontal_penetrab, __pyx_n_s_add_edge, 45, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 45, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 950, __pyx_L1_error)
@@ -19432,18 +19434,18 @@
   /* "ts2vg/graph/_horizontal_penetrable.pyx":21
  * @cython.wraparound(False)
  * @cython.cdivision(True)
  * def _compute_graph(np.float64_t[:] ts, np.float64_t[:] xs, uint directed, uint weighted, bint only_degrees, double min_weight, double max_weight, uint penetrable_limit):             # <<<<<<<<<<<<<<
  *     """
  *     Computes the limited penetrable horizontal visibility graph of a time series.
  */
-  __pyx_tuple__24 = PyTuple_Pack(28, __pyx_n_s_ts, __pyx_n_s_xs, __pyx_n_s_directed, __pyx_n_s_weighted, __pyx_n_s_only_degrees, __pyx_n_s_min_weight, __pyx_n_s_max_weight, __pyx_n_s_penetrable_limit, __pyx_n_s_n, __pyx_n_s_edges, __pyx_n_s_degrees_in, __pyx_n_s_degrees_out, __pyx_n_s_left, __pyx_n_s_right, __pyx_n_s_i_a, __pyx_n_s_i_b, __pyx_n_s_x_a, __pyx_n_s_x_b, __pyx_n_s_y_a, __pyx_n_s_y_b, __pyx_n_s_w, __pyx_n_s_max_ys, __pyx_n_s_threshold_y_idx, __pyx_n_s_threshold_y, __pyx_n_s_weight_func, __pyx_n_s_add_edge, __pyx_n_s_add_edge, __pyx_n_s_j); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(26, __pyx_n_s_ts, __pyx_n_s_xs, __pyx_n_s_directed, __pyx_n_s_weighted, __pyx_n_s_only_degrees, __pyx_n_s_min_weight, __pyx_n_s_max_weight, __pyx_n_s_penetrable_limit, __pyx_n_s_n, __pyx_n_s_edges, __pyx_n_s_degrees_in, __pyx_n_s_degrees_out, __pyx_n_s_i_a, __pyx_n_s_i_b, __pyx_n_s_x_a, __pyx_n_s_x_b, __pyx_n_s_y_a, __pyx_n_s_y_b, __pyx_n_s_w, __pyx_n_s_max_ys, __pyx_n_s_threshold_y_idx, __pyx_n_s_threshold_y, __pyx_n_s_weight_func, __pyx_n_s_add_edge, __pyx_n_s_add_edge, __pyx_n_s_j); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(8, 0, 28, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ts2vg_graph__horizontal_penetrab, __pyx_n_s_compute_graph, 21, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(8, 0, 26, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ts2vg_graph__horizontal_penetrab, __pyx_n_s_compute_graph, 21, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 21, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
@@ -19643,52 +19645,67 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -21602,28 +21619,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -22808,44 +22825,62 @@
     return ret;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `ts2vg-1.2.1/ts2vg/graph/_natural.c` & `ts2vg-1.2.2/ts2vg/graph/_natural.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include"
         ],
+        "language": "c++",
         "name": "ts2vg.graph._natural",
         "sources": [
             "ts2vg/graph/_natural.pyx"
         ]
     },
     "module_name": "ts2vg.graph._natural"
 }
@@ -33,16 +34,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -227,15 +228,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -266,15 +267,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -375,27 +376,41 @@
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
 
+#ifndef __cplusplus
+  #error "Cython files generated with the C++ option must be compiled with a C++ compiler."
+#endif
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
-  #elif defined(__GNUC__)
-    #define CYTHON_INLINE __inline__
-  #elif defined(_MSC_VER)
-    #define CYTHON_INLINE __inline
-  #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
-    #define CYTHON_INLINE inline
   #else
-    #define CYTHON_INLINE
+    #define CYTHON_INLINE inline
   #endif
 #endif
+template<typename T>
+void __Pyx_call_destructor(T& x) {
+    x.~T();
+}
+template<typename T>
+class __Pyx_FakeReference {
+  public:
+    __Pyx_FakeReference() : ptr(NULL) { }
+    __Pyx_FakeReference(const T& ref) : ptr(const_cast<T*>(&ref)) { }
+    T *operator->() { return ptr; }
+    T *operator&() { return ptr; }
+    operator T&() { return *ptr; }
+    template<typename U> bool operator ==(U other) { return *ptr == other; }
+    template<typename U> bool operator !=(U other) { return *ptr != other; }
+  private:
+    T *ptr;
+};
 
 #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
   #define Py_OptimizeFlag 0
 #endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
@@ -776,16 +791,34 @@
 #include "numpy/ndarraytypes.h"
 #include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
 
     /* NumPy API declarations from "numpy/__init__.pxd" */
     
 #include <math.h>
-#include <stdlib.h>
+#include "ios"
+#include "new"
+#include "stdexcept"
+#include "typeinfo"
+#include <queue>
+#include <utility>
+
+    #if __cplusplus >= 201103L || (defined(_MSC_VER) && _MSC_VER >= 1600)
+    // move should be defined for these versions of MSVC, but __cplusplus isn't set usefully
+    #include <type_traits>
+
+    namespace cython_std {
+    template <typename T> typename std::remove_reference<T>::type&& move(T& t) noexcept { return std::move(t); }
+    template <typename T> typename std::remove_reference<T>::type&& move(T&& t) noexcept { return std::move(t); }
+    }
+
+    #endif
+    
 #include "pythread.h"
+#include <stdlib.h>
 #include "pystate.h"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
@@ -1014,15 +1047,14 @@
 
 
 static const char *__pyx_f[] = {
   "ts2vg/graph/_natural.pyx",
   "__init__.pxd",
   "stringsource",
   "type.pxd",
-  "ts2vg/utils/pairqueue.pxd",
 };
 /* MemviewSliceStruct.proto */
 struct __pyx_memoryview_obj;
 typedef struct {
   struct __pyx_memoryview_obj *memview;
   char *data;
   Py_ssize_t shape[8];
@@ -1121,195 +1153,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1319,20 +1351,20 @@
  * 
  * ctypedef unsigned int uint             # <<<<<<<<<<<<<<
  * ctypedef double (*weight_func_type)(double x_a, double x_b, double y_a, double y_b, double slope)
  * 
  */
 typedef unsigned int __pyx_t_5ts2vg_5graph_5_base_uint;
 
-/* "ts2vg/graph/_natural.pyx":12
+/* "ts2vg/graph/_natural.pyx":14
  * from ts2vg.graph._base cimport _greater, _argmax, _get_weight_func, weight_func_type
  * 
  * ctypedef unsigned int uint             # <<<<<<<<<<<<<<
+ * ctypedef cpair[uint, uint] uint_pair
  * 
- * cdef double ABS_TOL = 1e-14
  */
 typedef unsigned int __pyx_t_5ts2vg_5graph_8_natural_uint;
 /* Declarations.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     typedef ::std::complex< float > __pyx_t_float_complex;
   #else
@@ -1353,122 +1385,75 @@
 #else
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
-struct __pyx_obj_5ts2vg_5utils_9pairqueue_PairQueue;
 struct __pyx_obj_5ts2vg_5graph_8_natural___pyx_scope_struct___compute_graph;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
-struct __pyx_t_5ts2vg_5utils_9pairqueue_QueueEntry;
-struct __pyx_t_5ts2vg_5utils_9pairqueue_Queue;
-struct __pyx_ctuple_unsigned__space_int__and_unsigned__space_int;
-typedef struct __pyx_ctuple_unsigned__space_int__and_unsigned__space_int __pyx_ctuple_unsigned__space_int__and_unsigned__space_int;
-
-/* "ts2vg/utils/pairqueue.pxd":5
- * from libc.stdlib cimport malloc, free
- * 
- * cdef struct QueueEntry:             # <<<<<<<<<<<<<<
- *     unsigned int a;
- *     unsigned int b;
- */
-struct __pyx_t_5ts2vg_5utils_9pairqueue_QueueEntry {
-  unsigned int a;
-  unsigned int b;
-  struct __pyx_t_5ts2vg_5utils_9pairqueue_QueueEntry *next;
-};
-
-/* "ts2vg/utils/pairqueue.pxd":11
- *     QueueEntry *next;
- * 
- * cdef struct Queue:             # <<<<<<<<<<<<<<
- *     QueueEntry *head;
- *     QueueEntry *tail;
- */
-struct __pyx_t_5ts2vg_5utils_9pairqueue_Queue {
-  struct __pyx_t_5ts2vg_5utils_9pairqueue_QueueEntry *head;
-  struct __pyx_t_5ts2vg_5utils_9pairqueue_QueueEntry *tail;
-};
-
-/* "ts2vg/utils/pairqueue.pxd":18
- *     cdef Queue *queue
- * 
- *     cdef void push(self, (unsigned int, unsigned int) values)             # <<<<<<<<<<<<<<
- *     cdef (unsigned int, unsigned int) pop(self)
- *     cdef bint is_empty(self)
- */
-struct __pyx_ctuple_unsigned__space_int__and_unsigned__space_int {
-  unsigned int f0;
-  unsigned int f1;
-};
 
 /* "ts2vg/graph/_base.pxd":6
  * 
  * ctypedef unsigned int uint
  * ctypedef double (*weight_func_type)(double x_a, double x_b, double y_a, double y_b, double slope)             # <<<<<<<<<<<<<<
  * 
  * cdef bint _greater(double a, double b, double tolerance)
  */
 typedef double (*__pyx_t_5ts2vg_5graph_5_base_weight_func_type)(double, double, double, double, double);
 
-/* "ts2vg/utils/pairqueue.pxd":15
- *     QueueEntry *tail;
+/* "ts2vg/graph/_natural.pyx":15
  * 
- * cdef class PairQueue:             # <<<<<<<<<<<<<<
- *     cdef Queue *queue
+ * ctypedef unsigned int uint
+ * ctypedef cpair[uint, uint] uint_pair             # <<<<<<<<<<<<<<
  * 
+ * cdef double ABS_TOL = 1e-14
  */
-struct __pyx_obj_5ts2vg_5utils_9pairqueue_PairQueue {
-  PyObject_HEAD
-  struct __pyx_vtabstruct_5ts2vg_5utils_9pairqueue_PairQueue *__pyx_vtab;
-  struct __pyx_t_5ts2vg_5utils_9pairqueue_Queue *queue;
-};
-
+typedef std::pair<unsigned int,unsigned int>  __pyx_t_5ts2vg_5graph_8_natural_uint_pair;
 
-/* "ts2vg/graph/_natural.pyx":23
+/* "ts2vg/graph/_natural.pyx":26
  * @cython.wraparound(False)
  * @cython.cdivision(True)
  * def _compute_graph(np.float64_t[:] ts, np.float64_t[:] xs, uint directed, uint weighted, bint only_degrees, double min_weight, double max_weight):             # <<<<<<<<<<<<<<
  *     """
  *     Computes the visibility graph of a time series
  */
 struct __pyx_obj_5ts2vg_5graph_8_natural___pyx_scope_struct___compute_graph {
@@ -1558,31 +1543,14 @@
   PyObject *from_object;
   PyObject *(*to_object_func)(char *);
   int (*to_dtype_func)(char *, PyObject *);
 };
 
 
 
-/* "ts2vg/utils/pairqueue.pxd":15
- *     QueueEntry *tail;
- * 
- * cdef class PairQueue:             # <<<<<<<<<<<<<<
- *     cdef Queue *queue
- * 
- */
-
-struct __pyx_vtabstruct_5ts2vg_5utils_9pairqueue_PairQueue {
-  void (*push)(struct __pyx_obj_5ts2vg_5utils_9pairqueue_PairQueue *, __pyx_ctuple_unsigned__space_int__and_unsigned__space_int);
-  __pyx_ctuple_unsigned__space_int__and_unsigned__space_int (*pop)(struct __pyx_obj_5ts2vg_5utils_9pairqueue_PairQueue *);
-  int (*is_empty)(struct __pyx_obj_5ts2vg_5utils_9pairqueue_PairQueue *);
-  void (*free)(struct __pyx_obj_5ts2vg_5utils_9pairqueue_PairQueue *);
-};
-static struct __pyx_vtabstruct_5ts2vg_5utils_9pairqueue_PairQueue *__pyx_vtabptr_5ts2vg_5utils_9pairqueue_PairQueue;
-
-
 /* "View.MemoryView":106
  * 
  * @cname("__pyx_array")
  * cdef class array:             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
@@ -1782,57 +1750,14 @@
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
 #endif
 
-/* PyFunctionFastCall.proto */
-#if CYTHON_FAST_PYCALL
-#define __Pyx_PyFunction_FastCall(func, args, nargs)\
-    __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
-#if 1 || PY_VERSION_HEX < 0x030600B1
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
-#else
-#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
-#endif
-#define __Pyx_BUILD_ASSERT_EXPR(cond)\
-    (sizeof(char [1 - 2*!(cond)]) - 1)
-#ifndef Py_MEMBER_SIZE
-#define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
-#endif
-#if CYTHON_FAST_PYCALL
-  static size_t __pyx_pyframe_localsplus_offset = 0;
-  #include "frameobject.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
-  #define __Pxy_PyFrame_Initialize_Offsets()\
-    ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
-     (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
-  #define __Pyx_PyFrame_GetLocalsplus(frame)\
-    (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
-#endif // CYTHON_FAST_PYCALL
-#endif
-
-/* PyObjectCallMethO.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
-#endif
-
-/* PyObjectCallNoArg.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
-#else
-#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
-#endif
-
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 
 /* CythonFunctionShared.proto */
 #define __Pyx_CyFunction_USED 1
 #define __Pyx_CYFUNCTION_STATICMETHOD  0x01
 #define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
@@ -1998,17 +1923,53 @@
 /* PyCFunctionFastCall.proto */
 #if CYTHON_FAST_PYCCALL
 static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
 #else
 #define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
 #endif
 
+/* PyFunctionFastCall.proto */
+#if CYTHON_FAST_PYCALL
+#define __Pyx_PyFunction_FastCall(func, args, nargs)\
+    __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
+#if 1 || PY_VERSION_HEX < 0x030600B1
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
+#else
+#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
+#endif
+#define __Pyx_BUILD_ASSERT_EXPR(cond)\
+    (sizeof(char [1 - 2*!(cond)]) - 1)
+#ifndef Py_MEMBER_SIZE
+#define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
+#endif
+#if CYTHON_FAST_PYCALL
+  static size_t __pyx_pyframe_localsplus_offset = 0;
+  #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+  #define __Pxy_PyFrame_Initialize_Offsets()\
+    ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
+     (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
+  #define __Pyx_PyFrame_GetLocalsplus(frame)\
+    (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
+#endif
+
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
+/* PyObjectCallMethO.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
+#endif
+
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
 /* IncludeStringH.proto */
 #include <string.h>
 
 /* BytesEquals.proto */
@@ -2203,25 +2164,30 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
-/* GetVTable.proto */
-static void* __Pyx_GetVtable(PyObject *dict);
-
 /* DictGetItem.proto */
 #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
 static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
 #define __Pyx_PyObject_Dict_GetItem(obj, name)\
     (likely(PyDict_CheckExact(obj)) ?\
      __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
 #else
@@ -2323,14 +2289,56 @@
 /* MemviewDtypeToObject.proto */
 static CYTHON_INLINE PyObject *__pyx_memview_get_nn___pyx_t_5numpy_float64_t(const char *itemp);
 static CYTHON_INLINE int __pyx_memview_set_nn___pyx_t_5numpy_float64_t(const char *itemp, PyObject *obj);
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(PyObject *, int writable_flag);
 
+/* CppExceptionConversion.proto */
+#ifndef __Pyx_CppExn2PyErr
+#include <new>
+#include <typeinfo>
+#include <stdexcept>
+#include <ios>
+static void __Pyx_CppExn2PyErr() {
+  try {
+    if (PyErr_Occurred())
+      ; // let the latest Python exn pass through and ignore the current one
+    else
+      throw;
+  } catch (const std::bad_alloc& exn) {
+    PyErr_SetString(PyExc_MemoryError, exn.what());
+  } catch (const std::bad_cast& exn) {
+    PyErr_SetString(PyExc_TypeError, exn.what());
+  } catch (const std::bad_typeid& exn) {
+    PyErr_SetString(PyExc_TypeError, exn.what());
+  } catch (const std::domain_error& exn) {
+    PyErr_SetString(PyExc_ValueError, exn.what());
+  } catch (const std::invalid_argument& exn) {
+    PyErr_SetString(PyExc_ValueError, exn.what());
+  } catch (const std::ios_base::failure& exn) {
+    PyErr_SetString(PyExc_IOError, exn.what());
+  } catch (const std::out_of_range& exn) {
+    PyErr_SetString(PyExc_IndexError, exn.what());
+  } catch (const std::overflow_error& exn) {
+    PyErr_SetString(PyExc_OverflowError, exn.what());
+  } catch (const std::range_error& exn) {
+    PyErr_SetString(PyExc_ArithmeticError, exn.what());
+  } catch (const std::underflow_error& exn) {
+    PyErr_SetString(PyExc_ArithmeticError, exn.what());
+  } catch (const std::exception& exn) {
+    PyErr_SetString(PyExc_RuntimeError, exn.what());
+  }
+  catch (...)
+  {
+    PyErr_SetString(PyExc_RuntimeError, "Unknown exception");
+  }
+}
+#endif
+
 /* MemviewDtypeToObject.proto */
 static CYTHON_INLINE PyObject *__pyx_memview_get_nn___pyx_t_5numpy_uint32_t(const char *itemp);
 static CYTHON_INLINE int __pyx_memview_set_nn___pyx_t_5numpy_uint32_t(const char *itemp, PyObject *obj);
 
 /* RealImag.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
@@ -2523,18 +2531,19 @@
 static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
 static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'libc.math' */
 
-/* Module declarations from 'libc.stdlib' */
+/* Module declarations from 'libcpp.queue' */
 
-/* Module declarations from 'ts2vg.utils.pairqueue' */
-static PyTypeObject *__pyx_ptype_5ts2vg_5utils_9pairqueue_PairQueue = 0;
+/* Module declarations from 'libcpp.utility' */
+
+/* Module declarations from 'libcpp.pair' */
 
 /* Module declarations from 'ts2vg.graph._base' */
 static int (*__pyx_f_5ts2vg_5graph_5_base__greater)(double, double, double); /*proto*/
 static __pyx_t_5ts2vg_5graph_5_base_uint (*__pyx_f_5ts2vg_5graph_5_base__argmax)(__Pyx_memviewslice, __pyx_t_5ts2vg_5graph_5_base_uint, __pyx_t_5ts2vg_5graph_5_base_uint); /*proto*/
 static __pyx_t_5ts2vg_5graph_5_base_weight_func_type (*__pyx_f_5ts2vg_5graph_5_base__get_weight_func)(__pyx_t_5ts2vg_5graph_5_base_uint); /*proto*/
 
 /* Module declarations from 'ts2vg.graph._natural' */
@@ -2630,14 +2639,15 @@
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_left[] = "left";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_mode[] = "mode";
 static const char __pyx_k_name[] = "name";
 static const char __pyx_k_ndim[] = "ndim";
 static const char __pyx_k_pack[] = "pack";
+static const char __pyx_k_pair[] = "pair";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_step[] = "step";
 static const char __pyx_k_stop[] = "stop";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_ASCII[] = "ASCII";
 static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_dtype[] = "dtype";
@@ -2814,14 +2824,15 @@
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_obj;
 static PyObject *__pyx_n_s_only_degrees;
 static PyObject *__pyx_n_s_pack;
+static PyObject *__pyx_n_s_pair;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_getbuffer;
 static PyObject *__pyx_n_s_pyx_result;
 static PyObject *__pyx_n_s_pyx_state;
 static PyObject *__pyx_n_s_pyx_type;
@@ -2956,15 +2967,15 @@
 static PyObject *__pyx_tuple__30;
 static PyObject *__pyx_tuple__31;
 static PyObject *__pyx_codeobj__2;
 static PyObject *__pyx_codeobj__25;
 static PyObject *__pyx_codeobj__32;
 /* Late includes */
 
-/* "ts2vg/graph/_natural.pyx":23
+/* "ts2vg/graph/_natural.pyx":26
  * @cython.wraparound(False)
  * @cython.cdivision(True)
  * def _compute_graph(np.float64_t[:] ts, np.float64_t[:] xs, uint directed, uint weighted, bint only_degrees, double min_weight, double max_weight):             # <<<<<<<<<<<<<<
  *     """
  *     Computes the visibility graph of a time series
  */
 
@@ -3015,86 +3026,86 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ts)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_xs)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 1); __PYX_ERR(0, 23, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 1); __PYX_ERR(0, 26, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_directed)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 2); __PYX_ERR(0, 23, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 2); __PYX_ERR(0, 26, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_weighted)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 3); __PYX_ERR(0, 23, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 3); __PYX_ERR(0, 26, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_only_degrees)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 4); __PYX_ERR(0, 23, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 4); __PYX_ERR(0, 26, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_min_weight)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 5); __PYX_ERR(0, 23, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 5); __PYX_ERR(0, 26, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_max_weight)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 6); __PYX_ERR(0, 23, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, 6); __PYX_ERR(0, 26, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_compute_graph") < 0)) __PYX_ERR(0, 23, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_compute_graph") < 0)) __PYX_ERR(0, 26, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 7) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
       values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
     }
-    __pyx_v_ts = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_ts.memview)) __PYX_ERR(0, 23, __pyx_L3_error)
-    __pyx_v_xs = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_xs.memview)) __PYX_ERR(0, 23, __pyx_L3_error)
-    __pyx_v_directed = __Pyx_PyInt_As_unsigned_int(values[2]); if (unlikely((__pyx_v_directed == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 23, __pyx_L3_error)
-    __pyx_v_weighted = __Pyx_PyInt_As_unsigned_int(values[3]); if (unlikely((__pyx_v_weighted == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 23, __pyx_L3_error)
-    __pyx_v_only_degrees = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_only_degrees == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 23, __pyx_L3_error)
-    __pyx_v_min_weight = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_min_weight == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 23, __pyx_L3_error)
-    __pyx_v_max_weight = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_max_weight == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 23, __pyx_L3_error)
+    __pyx_v_ts = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_ts.memview)) __PYX_ERR(0, 26, __pyx_L3_error)
+    __pyx_v_xs = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_float64_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_xs.memview)) __PYX_ERR(0, 26, __pyx_L3_error)
+    __pyx_v_directed = __Pyx_PyInt_As_unsigned_int(values[2]); if (unlikely((__pyx_v_directed == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L3_error)
+    __pyx_v_weighted = __Pyx_PyInt_As_unsigned_int(values[3]); if (unlikely((__pyx_v_weighted == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L3_error)
+    __pyx_v_only_degrees = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_only_degrees == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L3_error)
+    __pyx_v_min_weight = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_min_weight == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L3_error)
+    __pyx_v_max_weight = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_max_weight == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 26, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 23, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_compute_graph", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 26, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ts2vg.graph._natural._compute_graph", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5ts2vg_5graph_8_natural__compute_graph(__pyx_self, __pyx_v_ts, __pyx_v_xs, __pyx_v_directed, __pyx_v_weighted, __pyx_v_only_degrees, __pyx_v_min_weight, __pyx_v_max_weight);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ts2vg/graph/_natural.pyx":42
- *     queue.push((0, n))
+/* "ts2vg/graph/_natural.pyx":45
+ *     queue.push(uint_pair(0, n))
  * 
  *     def add_edge(uint i1, uint i2, double x1, double x2, double y1, double y2, double slope):             # <<<<<<<<<<<<<<
  *         w = weight_func(x1, x2, y1, y2, slope)
  * 
  */
 
 /* Python wrapper */
@@ -3143,72 +3154,72 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_i1)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_i2)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 7, 7, 1); __PYX_ERR(0, 42, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 7, 7, 1); __PYX_ERR(0, 45, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_x1)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 7, 7, 2); __PYX_ERR(0, 42, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 7, 7, 2); __PYX_ERR(0, 45, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_x2)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 7, 7, 3); __PYX_ERR(0, 42, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 7, 7, 3); __PYX_ERR(0, 45, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_y1)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 7, 7, 4); __PYX_ERR(0, 42, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 7, 7, 4); __PYX_ERR(0, 45, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_y2)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 7, 7, 5); __PYX_ERR(0, 42, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 7, 7, 5); __PYX_ERR(0, 45, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_slope)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 7, 7, 6); __PYX_ERR(0, 42, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_edge", 1, 7, 7, 6); __PYX_ERR(0, 45, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "add_edge") < 0)) __PYX_ERR(0, 42, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "add_edge") < 0)) __PYX_ERR(0, 45, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 7) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
       values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
     }
-    __pyx_v_i1 = __Pyx_PyInt_As_unsigned_int(values[0]); if (unlikely((__pyx_v_i1 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 42, __pyx_L3_error)
-    __pyx_v_i2 = __Pyx_PyInt_As_unsigned_int(values[1]); if (unlikely((__pyx_v_i2 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 42, __pyx_L3_error)
-    __pyx_v_x1 = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_x1 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 42, __pyx_L3_error)
-    __pyx_v_x2 = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_x2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 42, __pyx_L3_error)
-    __pyx_v_y1 = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_y1 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 42, __pyx_L3_error)
-    __pyx_v_y2 = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_y2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 42, __pyx_L3_error)
-    __pyx_v_slope = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_slope == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 42, __pyx_L3_error)
+    __pyx_v_i1 = __Pyx_PyInt_As_unsigned_int(values[0]); if (unlikely((__pyx_v_i1 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L3_error)
+    __pyx_v_i2 = __Pyx_PyInt_As_unsigned_int(values[1]); if (unlikely((__pyx_v_i2 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L3_error)
+    __pyx_v_x1 = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_x1 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L3_error)
+    __pyx_v_x2 = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_x2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L3_error)
+    __pyx_v_y1 = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_y1 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L3_error)
+    __pyx_v_y2 = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_y2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L3_error)
+    __pyx_v_slope = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_slope == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("add_edge", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 42, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("add_edge", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 45, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ts2vg.graph._natural._compute_graph.add_edge", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5ts2vg_5graph_8_natural_14_compute_graph_add_edge(__pyx_self, __pyx_v_i1, __pyx_v_i2, __pyx_v_x1, __pyx_v_x2, __pyx_v_y1, __pyx_v_y2, __pyx_v_slope);
 
@@ -3234,24 +3245,24 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_edge", 0);
   __pyx_outer_scope = (struct __pyx_obj_5ts2vg_5graph_8_natural___pyx_scope_struct___compute_graph *) __Pyx_CyFunction_GetClosure(__pyx_self);
   __pyx_cur_scope = __pyx_outer_scope;
 
-  /* "ts2vg/graph/_natural.pyx":43
+  /* "ts2vg/graph/_natural.pyx":46
  * 
  *     def add_edge(uint i1, uint i2, double x1, double x2, double y1, double y2, double slope):
  *         w = weight_func(x1, x2, y1, y2, slope)             # <<<<<<<<<<<<<<
  * 
  *         if w <= min_weight or w >= max_weight:
  */
   __pyx_v_w = __pyx_cur_scope->__pyx_v_weight_func(__pyx_v_x1, __pyx_v_x2, __pyx_v_y1, __pyx_v_y2, __pyx_v_slope);
 
-  /* "ts2vg/graph/_natural.pyx":45
+  /* "ts2vg/graph/_natural.pyx":48
  *         w = weight_func(x1, x2, y1, y2, slope)
  * 
  *         if w <= min_weight or w >= max_weight:             # <<<<<<<<<<<<<<
  *             return
  * 
  */
   __pyx_t_2 = ((__pyx_v_w <= __pyx_cur_scope->__pyx_v_min_weight) != 0);
@@ -3261,159 +3272,159 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = ((__pyx_v_w >= __pyx_cur_scope->__pyx_v_max_weight) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "ts2vg/graph/_natural.pyx":46
+    /* "ts2vg/graph/_natural.pyx":49
  * 
  *         if w <= min_weight or w >= max_weight:
  *             return             # <<<<<<<<<<<<<<
  * 
  *         degrees_out[i1] += 1
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "ts2vg/graph/_natural.pyx":45
+    /* "ts2vg/graph/_natural.pyx":48
  *         w = weight_func(x1, x2, y1, y2, slope)
  * 
  *         if w <= min_weight or w >= max_weight:             # <<<<<<<<<<<<<<
  *             return
  * 
  */
   }
 
-  /* "ts2vg/graph/_natural.pyx":48
+  /* "ts2vg/graph/_natural.pyx":51
  *             return
  * 
  *         degrees_out[i1] += 1             # <<<<<<<<<<<<<<
  *         degrees_in[i2] += 1
  * 
  */
-  if (unlikely(!__pyx_cur_scope->__pyx_v_degrees_out.memview)) { __Pyx_RaiseClosureNameError("degrees_out"); __PYX_ERR(0, 48, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_v_degrees_out.memview)) { __Pyx_RaiseClosureNameError("degrees_out"); __PYX_ERR(0, 51, __pyx_L1_error) }
   __pyx_t_3 = __pyx_v_i1;
   *((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_cur_scope->__pyx_v_degrees_out.data + __pyx_t_3 * __pyx_cur_scope->__pyx_v_degrees_out.strides[0]) )) += 1;
 
-  /* "ts2vg/graph/_natural.pyx":49
+  /* "ts2vg/graph/_natural.pyx":52
  * 
  *         degrees_out[i1] += 1
  *         degrees_in[i2] += 1             # <<<<<<<<<<<<<<
  * 
  *         if not only_degrees:
  */
-  if (unlikely(!__pyx_cur_scope->__pyx_v_degrees_in.memview)) { __Pyx_RaiseClosureNameError("degrees_in"); __PYX_ERR(0, 49, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_v_degrees_in.memview)) { __Pyx_RaiseClosureNameError("degrees_in"); __PYX_ERR(0, 52, __pyx_L1_error) }
   __pyx_t_3 = __pyx_v_i2;
   *((__pyx_t_5numpy_uint32_t *) ( /* dim=0 */ (__pyx_cur_scope->__pyx_v_degrees_in.data + __pyx_t_3 * __pyx_cur_scope->__pyx_v_degrees_in.strides[0]) )) += 1;
 
-  /* "ts2vg/graph/_natural.pyx":51
+  /* "ts2vg/graph/_natural.pyx":54
  *         degrees_in[i2] += 1
  * 
  *         if not only_degrees:             # <<<<<<<<<<<<<<
  *             if weighted > 0:
  *                 edges.append((i1, i2, w))
  */
   __pyx_t_1 = ((!(__pyx_cur_scope->__pyx_v_only_degrees != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "ts2vg/graph/_natural.pyx":52
+    /* "ts2vg/graph/_natural.pyx":55
  * 
  *         if not only_degrees:
  *             if weighted > 0:             # <<<<<<<<<<<<<<
  *                 edges.append((i1, i2, w))
  *             else:
  */
     __pyx_t_1 = ((__pyx_cur_scope->__pyx_v_weighted > 0) != 0);
     if (__pyx_t_1) {
 
-      /* "ts2vg/graph/_natural.pyx":53
+      /* "ts2vg/graph/_natural.pyx":56
  *         if not only_degrees:
  *             if weighted > 0:
  *                 edges.append((i1, i2, w))             # <<<<<<<<<<<<<<
  *             else:
  *                 edges.append((i1, i2))
  */
-      if (unlikely(!__pyx_cur_scope->__pyx_v_edges)) { __Pyx_RaiseClosureNameError("edges"); __PYX_ERR(0, 53, __pyx_L1_error) }
+      if (unlikely(!__pyx_cur_scope->__pyx_v_edges)) { __Pyx_RaiseClosureNameError("edges"); __PYX_ERR(0, 56, __pyx_L1_error) }
       if (unlikely(__pyx_cur_scope->__pyx_v_edges == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "append");
-        __PYX_ERR(0, 53, __pyx_L1_error)
+        __PYX_ERR(0, 56, __pyx_L1_error)
       }
-      __pyx_t_4 = __Pyx_PyInt_From_unsigned_int(__pyx_v_i1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_unsigned_int(__pyx_v_i1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 56, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyInt_From_unsigned_int(__pyx_v_i2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_unsigned_int(__pyx_v_i2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = PyFloat_FromDouble(__pyx_v_w); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 53, __pyx_L1_error)
+      __pyx_t_6 = PyFloat_FromDouble(__pyx_v_w); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 56, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 53, __pyx_L1_error)
+      __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 56, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_t_6);
       __pyx_t_4 = 0;
       __pyx_t_5 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_8 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_edges, __pyx_t_7); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 53, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_edges, __pyx_t_7); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 56, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "ts2vg/graph/_natural.pyx":52
+      /* "ts2vg/graph/_natural.pyx":55
  * 
  *         if not only_degrees:
  *             if weighted > 0:             # <<<<<<<<<<<<<<
  *                 edges.append((i1, i2, w))
  *             else:
  */
       goto __pyx_L7;
     }
 
-    /* "ts2vg/graph/_natural.pyx":55
+    /* "ts2vg/graph/_natural.pyx":58
  *                 edges.append((i1, i2, w))
  *             else:
  *                 edges.append((i1, i2))             # <<<<<<<<<<<<<<
  * 
  * 
  */
     /*else*/ {
-      if (unlikely(!__pyx_cur_scope->__pyx_v_edges)) { __Pyx_RaiseClosureNameError("edges"); __PYX_ERR(0, 55, __pyx_L1_error) }
+      if (unlikely(!__pyx_cur_scope->__pyx_v_edges)) { __Pyx_RaiseClosureNameError("edges"); __PYX_ERR(0, 58, __pyx_L1_error) }
       if (unlikely(__pyx_cur_scope->__pyx_v_edges == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "append");
-        __PYX_ERR(0, 55, __pyx_L1_error)
+        __PYX_ERR(0, 58, __pyx_L1_error)
       }
-      __pyx_t_7 = __Pyx_PyInt_From_unsigned_int(__pyx_v_i1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 55, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_From_unsigned_int(__pyx_v_i1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 58, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_6 = __Pyx_PyInt_From_unsigned_int(__pyx_v_i2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 55, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_From_unsigned_int(__pyx_v_i2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 58, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 55, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_7);
       PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_7);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_6);
       __pyx_t_7 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_8 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_edges, __pyx_t_5); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 55, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyList_Append(__pyx_cur_scope->__pyx_v_edges, __pyx_t_5); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 58, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __pyx_L7:;
 
-    /* "ts2vg/graph/_natural.pyx":51
+    /* "ts2vg/graph/_natural.pyx":54
  *         degrees_in[i2] += 1
  * 
  *         if not only_degrees:             # <<<<<<<<<<<<<<
  *             if weighted > 0:
  *                 edges.append((i1, i2, w))
  */
   }
 
-  /* "ts2vg/graph/_natural.pyx":42
- *     queue.push((0, n))
+  /* "ts2vg/graph/_natural.pyx":45
+ *     queue.push(uint_pair(0, n))
  * 
  *     def add_edge(uint i1, uint i2, double x1, double x2, double y1, double y2, double slope):             # <<<<<<<<<<<<<<
  *         w = weight_func(x1, x2, y1, y2, slope)
  * 
  */
 
   /* function exit code */
@@ -3428,15 +3439,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ts2vg/graph/_natural.pyx":23
+/* "ts2vg/graph/_natural.pyx":26
  * @cython.wraparound(False)
  * @cython.cdivision(True)
  * def _compute_graph(np.float64_t[:] ts, np.float64_t[:] xs, uint directed, uint weighted, bint only_degrees, double min_weight, double max_weight):             # <<<<<<<<<<<<<<
  *     """
  *     Computes the visibility graph of a time series
  */
 
@@ -3449,27 +3460,28 @@
   __pyx_t_5ts2vg_5graph_8_natural_uint __pyx_v_d;
   double __pyx_v_x_a;
   double __pyx_v_x_b;
   double __pyx_v_y_a;
   double __pyx_v_y_b;
   double __pyx_v_slope;
   double __pyx_v_max_slope;
-  struct __pyx_obj_5ts2vg_5utils_9pairqueue_PairQueue *__pyx_v_queue = 0;
+  std::queue<__pyx_t_5ts2vg_5graph_8_natural_uint_pair>  __pyx_v_queue;
   PyObject *__pyx_v_add_edge = 0;
+  __pyx_t_5ts2vg_5graph_8_natural_uint_pair __pyx_v_pair;
   double __pyx_v_tol;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   __pyx_t_5ts2vg_5graph_8_natural_uint __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   __Pyx_memviewslice __pyx_t_7 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  __pyx_ctuple_unsigned__space_int__and_unsigned__space_int __pyx_t_8;
+  __pyx_t_5ts2vg_5graph_8_natural_uint_pair __pyx_t_8;
   int __pyx_t_9;
   unsigned int __pyx_t_10;
   unsigned int __pyx_t_11;
   size_t __pyx_t_12;
   long __pyx_t_13;
   long __pyx_t_14;
   double __pyx_t_15;
@@ -3484,288 +3496,297 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_compute_graph", 0);
   __pyx_cur_scope = (struct __pyx_obj_5ts2vg_5graph_8_natural___pyx_scope_struct___compute_graph *)__pyx_tp_new_5ts2vg_5graph_8_natural___pyx_scope_struct___compute_graph(__pyx_ptype_5ts2vg_5graph_8_natural___pyx_scope_struct___compute_graph, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_5ts2vg_5graph_8_natural___pyx_scope_struct___compute_graph *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 23, __pyx_L1_error)
+    __PYX_ERR(0, 26, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_weighted = __pyx_v_weighted;
   __pyx_cur_scope->__pyx_v_only_degrees = __pyx_v_only_degrees;
   __pyx_cur_scope->__pyx_v_min_weight = __pyx_v_min_weight;
   __pyx_cur_scope->__pyx_v_max_weight = __pyx_v_max_weight;
 
-  /* "ts2vg/graph/_natural.pyx":28
+  /* "ts2vg/graph/_natural.pyx":31
  *     using a divide-and-conquer strategy.
  *     """
  *     cdef uint n = ts.size             # <<<<<<<<<<<<<<
  *     cdef list edges = []
  *     cdef np.uint32_t[:] degrees_in = np.zeros(n, dtype=np.uint32)
  */
-  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_ts, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_float64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_float64_t, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_ts, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_float64_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_float64_t, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyInt_As_unsigned_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_unsigned_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_n = __pyx_t_3;
 
-  /* "ts2vg/graph/_natural.pyx":29
+  /* "ts2vg/graph/_natural.pyx":32
  *     """
  *     cdef uint n = ts.size
  *     cdef list edges = []             # <<<<<<<<<<<<<<
  *     cdef np.uint32_t[:] degrees_in = np.zeros(n, dtype=np.uint32)
  *     cdef np.uint32_t[:] degrees_out = np.zeros(n, dtype=np.uint32)
  */
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_cur_scope->__pyx_v_edges = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "ts2vg/graph/_natural.pyx":30
+  /* "ts2vg/graph/_natural.pyx":33
  *     cdef uint n = ts.size
  *     cdef list edges = []
  *     cdef np.uint32_t[:] degrees_in = np.zeros(n, dtype=np.uint32)             # <<<<<<<<<<<<<<
  *     cdef np.uint32_t[:] degrees_out = np.zeros(n, dtype=np.uint32)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uint32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uint32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_t_6, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_t_6, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_cur_scope->__pyx_v_degrees_in = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
-  /* "ts2vg/graph/_natural.pyx":31
+  /* "ts2vg/graph/_natural.pyx":34
  *     cdef list edges = []
  *     cdef np.uint32_t[:] degrees_in = np.zeros(n, dtype=np.uint32)
  *     cdef np.uint32_t[:] degrees_out = np.zeros(n, dtype=np.uint32)             # <<<<<<<<<<<<<<
  * 
  *     cdef uint left, right, i, d
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyInt_From_unsigned_int(__pyx_v_n); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_unsigned_int(__pyx_v_n); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_uint32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_5numpy_uint32_t(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_cur_scope->__pyx_v_degrees_out = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
-  /* "ts2vg/graph/_natural.pyx":37
+  /* "ts2vg/graph/_natural.pyx":40
  *     cdef double slope, max_slope, w
  * 
  *     cdef weight_func_type weight_func = _get_weight_func(weighted)             # <<<<<<<<<<<<<<
  * 
- *     cdef PairQueue queue = PairQueue()
+ *     cdef cqueue[uint_pair] queue
  */
   __pyx_cur_scope->__pyx_v_weight_func = __pyx_f_5ts2vg_5graph_5_base__get_weight_func(__pyx_cur_scope->__pyx_v_weighted);
 
-  /* "ts2vg/graph/_natural.pyx":39
- *     cdef weight_func_type weight_func = _get_weight_func(weighted)
- * 
- *     cdef PairQueue queue = PairQueue()             # <<<<<<<<<<<<<<
- *     queue.push((0, n))
- * 
- */
-  __pyx_t_5 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_5ts2vg_5utils_9pairqueue_PairQueue)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 39, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_v_queue = ((struct __pyx_obj_5ts2vg_5utils_9pairqueue_PairQueue *)__pyx_t_5);
-  __pyx_t_5 = 0;
-
-  /* "ts2vg/graph/_natural.pyx":40
+  /* "ts2vg/graph/_natural.pyx":43
  * 
- *     cdef PairQueue queue = PairQueue()
- *     queue.push((0, n))             # <<<<<<<<<<<<<<
+ *     cdef cqueue[uint_pair] queue
+ *     queue.push(uint_pair(0, n))             # <<<<<<<<<<<<<<
  * 
  *     def add_edge(uint i1, uint i2, double x1, double x2, double y1, double y2, double slope):
  */
-  __pyx_t_8.f0 = 0;
-  __pyx_t_8.f1 = __pyx_v_n;
-  ((struct __pyx_vtabstruct_5ts2vg_5utils_9pairqueue_PairQueue *)__pyx_v_queue->__pyx_vtab)->push(__pyx_v_queue, __pyx_t_8);
+  try {
+    __pyx_t_8 = __pyx_t_5ts2vg_5graph_8_natural_uint_pair(0, __pyx_v_n);
+  } catch(...) {
+    __Pyx_CppExn2PyErr();
+    __PYX_ERR(0, 43, __pyx_L1_error)
+  }
+  __pyx_v_queue.push(__pyx_t_8);
 
-  /* "ts2vg/graph/_natural.pyx":42
- *     queue.push((0, n))
+  /* "ts2vg/graph/_natural.pyx":45
+ *     queue.push(uint_pair(0, n))
  * 
  *     def add_edge(uint i1, uint i2, double x1, double x2, double y1, double y2, double slope):             # <<<<<<<<<<<<<<
  *         w = weight_func(x1, x2, y1, y2, slope)
  * 
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_5ts2vg_5graph_8_natural_14_compute_graph_1add_edge, 0, __pyx_n_s_compute_graph_locals_add_edge, ((PyObject*)__pyx_cur_scope), __pyx_n_s_ts2vg_graph__natural, __pyx_d, ((PyObject *)__pyx_codeobj__2)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_5ts2vg_5graph_8_natural_14_compute_graph_1add_edge, 0, __pyx_n_s_compute_graph_locals_add_edge, ((PyObject*)__pyx_cur_scope), __pyx_n_s_ts2vg_graph__natural, __pyx_d, ((PyObject *)__pyx_codeobj__2)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_v_add_edge = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "ts2vg/graph/_natural.pyx":58
+  /* "ts2vg/graph/_natural.pyx":61
  * 
  * 
- *     while not queue.is_empty():             # <<<<<<<<<<<<<<
- *         (left, right) = queue.pop()
- * 
+ *     while not queue.empty():             # <<<<<<<<<<<<<<
+ *         pair = queue.front()
+ *         left, right = pair.first, pair.second
  */
   while (1) {
-    __pyx_t_9 = ((!(((struct __pyx_vtabstruct_5ts2vg_5utils_9pairqueue_PairQueue *)__pyx_v_queue->__pyx_vtab)->is_empty(__pyx_v_queue) != 0)) != 0);
+    __pyx_t_9 = ((!(__pyx_v_queue.empty() != 0)) != 0);
     if (!__pyx_t_9) break;
 
-    /* "ts2vg/graph/_natural.pyx":59
+    /* "ts2vg/graph/_natural.pyx":62
  * 
- *     while not queue.is_empty():
- *         (left, right) = queue.pop()             # <<<<<<<<<<<<<<
+ *     while not queue.empty():
+ *         pair = queue.front()             # <<<<<<<<<<<<<<
+ *         left, right = pair.first, pair.second
+ *         queue.pop()
+ */
+    __pyx_v_pair = __pyx_v_queue.front();
+
+    /* "ts2vg/graph/_natural.pyx":63
+ *     while not queue.empty():
+ *         pair = queue.front()
+ *         left, right = pair.first, pair.second             # <<<<<<<<<<<<<<
+ *         queue.pop()
  * 
- *         if left+1 < right:
  */
-    __pyx_t_8 = ((struct __pyx_vtabstruct_5ts2vg_5utils_9pairqueue_PairQueue *)__pyx_v_queue->__pyx_vtab)->pop(__pyx_v_queue);
-    __pyx_t_10 = __pyx_t_8.f0;
-    __pyx_t_11 = __pyx_t_8.f1;
+    __pyx_t_10 = __pyx_v_pair.first;
+    __pyx_t_11 = __pyx_v_pair.second;
     __pyx_v_left = __pyx_t_10;
     __pyx_v_right = __pyx_t_11;
 
-    /* "ts2vg/graph/_natural.pyx":61
- *         (left, right) = queue.pop()
+    /* "ts2vg/graph/_natural.pyx":64
+ *         pair = queue.front()
+ *         left, right = pair.first, pair.second
+ *         queue.pop()             # <<<<<<<<<<<<<<
+ * 
+ *         if left+1 < right:
+ */
+    __pyx_v_queue.pop();
+
+    /* "ts2vg/graph/_natural.pyx":66
+ *         queue.pop()
  * 
  *         if left+1 < right:             # <<<<<<<<<<<<<<
  *             i = _argmax(ts, left, right)
  *             x_a = xs[i]
  */
     __pyx_t_9 = (((__pyx_v_left + 1) < __pyx_v_right) != 0);
     if (__pyx_t_9) {
 
-      /* "ts2vg/graph/_natural.pyx":62
+      /* "ts2vg/graph/_natural.pyx":67
  * 
  *         if left+1 < right:
  *             i = _argmax(ts, left, right)             # <<<<<<<<<<<<<<
  *             x_a = xs[i]
  *             y_a = ts[i]
  */
       __pyx_v_i = __pyx_f_5ts2vg_5graph_5_base__argmax(__pyx_v_ts, __pyx_v_left, __pyx_v_right);
 
-      /* "ts2vg/graph/_natural.pyx":63
+      /* "ts2vg/graph/_natural.pyx":68
  *         if left+1 < right:
  *             i = _argmax(ts, left, right)
  *             x_a = xs[i]             # <<<<<<<<<<<<<<
  *             y_a = ts[i]
  * 
  */
       __pyx_t_12 = __pyx_v_i;
       __pyx_v_x_a = (*((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_xs.data + __pyx_t_12 * __pyx_v_xs.strides[0]) )));
 
-      /* "ts2vg/graph/_natural.pyx":64
+      /* "ts2vg/graph/_natural.pyx":69
  *             i = _argmax(ts, left, right)
  *             x_a = xs[i]
  *             y_a = ts[i]             # <<<<<<<<<<<<<<
  * 
  *             # sweep from i towards the left
  */
       __pyx_t_12 = __pyx_v_i;
       __pyx_v_y_a = (*((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_ts.data + __pyx_t_12 * __pyx_v_ts.strides[0]) )));
 
-      /* "ts2vg/graph/_natural.pyx":67
+      /* "ts2vg/graph/_natural.pyx":72
  * 
  *             # sweep from i towards the left
  *             max_slope = -INFINITY             # <<<<<<<<<<<<<<
  *             for d in range(1, i-left+1):
  *                 x_b = xs[i-d]
  */
       __pyx_v_max_slope = (-INFINITY);
 
-      /* "ts2vg/graph/_natural.pyx":68
+      /* "ts2vg/graph/_natural.pyx":73
  *             # sweep from i towards the left
  *             max_slope = -INFINITY
  *             for d in range(1, i-left+1):             # <<<<<<<<<<<<<<
  *                 x_b = xs[i-d]
  *                 y_b = ts[i-d]
  */
       __pyx_t_13 = ((__pyx_v_i - __pyx_v_left) + 1);
       __pyx_t_14 = __pyx_t_13;
       for (__pyx_t_3 = 1; __pyx_t_3 < __pyx_t_14; __pyx_t_3+=1) {
         __pyx_v_d = __pyx_t_3;
 
-        /* "ts2vg/graph/_natural.pyx":69
+        /* "ts2vg/graph/_natural.pyx":74
  *             max_slope = -INFINITY
  *             for d in range(1, i-left+1):
  *                 x_b = xs[i-d]             # <<<<<<<<<<<<<<
  *                 y_b = ts[i-d]
  *                 slope = (y_b-y_a) / -(x_b-x_a)  # note: x-axis reversed because sweeping from left to right
  */
         __pyx_t_12 = (__pyx_v_i - __pyx_v_d);
         __pyx_v_x_b = (*((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_xs.data + __pyx_t_12 * __pyx_v_xs.strides[0]) )));
 
-        /* "ts2vg/graph/_natural.pyx":70
+        /* "ts2vg/graph/_natural.pyx":75
  *             for d in range(1, i-left+1):
  *                 x_b = xs[i-d]
  *                 y_b = ts[i-d]             # <<<<<<<<<<<<<<
  *                 slope = (y_b-y_a) / -(x_b-x_a)  # note: x-axis reversed because sweeping from left to right
  *                 tol = max(ABS_TOL, REL_TOL * max(fabs(x_a), fabs(x_b), fabs(y_a), fabs(y_b)))
  */
         __pyx_t_12 = (__pyx_v_i - __pyx_v_d);
         __pyx_v_y_b = (*((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_ts.data + __pyx_t_12 * __pyx_v_ts.strides[0]) )));
 
-        /* "ts2vg/graph/_natural.pyx":71
+        /* "ts2vg/graph/_natural.pyx":76
  *                 x_b = xs[i-d]
  *                 y_b = ts[i-d]
  *                 slope = (y_b-y_a) / -(x_b-x_a)  # note: x-axis reversed because sweeping from left to right             # <<<<<<<<<<<<<<
  *                 tol = max(ABS_TOL, REL_TOL * max(fabs(x_a), fabs(x_b), fabs(y_a), fabs(y_b)))
  * 
  */
         __pyx_v_slope = ((__pyx_v_y_b - __pyx_v_y_a) / (-(__pyx_v_x_b - __pyx_v_x_a)));
 
-        /* "ts2vg/graph/_natural.pyx":72
+        /* "ts2vg/graph/_natural.pyx":77
  *                 y_b = ts[i-d]
  *                 slope = (y_b-y_a) / -(x_b-x_a)  # note: x-axis reversed because sweeping from left to right
  *                 tol = max(ABS_TOL, REL_TOL * max(fabs(x_a), fabs(x_b), fabs(y_a), fabs(y_b)))             # <<<<<<<<<<<<<<
  * 
  *                 if _greater(slope, max_slope, tol):
  */
         __pyx_t_15 = fabs(__pyx_v_x_b);
@@ -3794,139 +3815,139 @@
         if (((__pyx_t_15 > __pyx_t_19) != 0)) {
           __pyx_t_16 = __pyx_t_15;
         } else {
           __pyx_t_16 = __pyx_t_19;
         }
         __pyx_v_tol = __pyx_t_16;
 
-        /* "ts2vg/graph/_natural.pyx":74
+        /* "ts2vg/graph/_natural.pyx":79
  *                 tol = max(ABS_TOL, REL_TOL * max(fabs(x_a), fabs(x_b), fabs(y_a), fabs(y_b)))
  * 
  *                 if _greater(slope, max_slope, tol):             # <<<<<<<<<<<<<<
  *                     if directed == _DIRECTED_TOP_TO_BOTTOM:
  *                         add_edge(i, i-d, x_a, x_b, y_a, y_b, -slope)
  */
         __pyx_t_9 = (__pyx_f_5ts2vg_5graph_5_base__greater(__pyx_v_slope, __pyx_v_max_slope, __pyx_v_tol) != 0);
         if (__pyx_t_9) {
 
-          /* "ts2vg/graph/_natural.pyx":75
+          /* "ts2vg/graph/_natural.pyx":80
  * 
  *                 if _greater(slope, max_slope, tol):
  *                     if directed == _DIRECTED_TOP_TO_BOTTOM:             # <<<<<<<<<<<<<<
  *                         add_edge(i, i-d, x_a, x_b, y_a, y_b, -slope)
  *                     else:  # left_to_right
  */
           __pyx_t_9 = ((__pyx_v_directed == __pyx_v_5ts2vg_5graph_8_natural__DIRECTED_TOP_TO_BOTTOM) != 0);
           if (__pyx_t_9) {
 
-            /* "ts2vg/graph/_natural.pyx":76
+            /* "ts2vg/graph/_natural.pyx":81
  *                 if _greater(slope, max_slope, tol):
  *                     if directed == _DIRECTED_TOP_TO_BOTTOM:
  *                         add_edge(i, i-d, x_a, x_b, y_a, y_b, -slope)             # <<<<<<<<<<<<<<
  *                     else:  # left_to_right
  *                         add_edge(i-d, i, x_b, x_a, y_b, y_a, -slope)
  */
-            __pyx_t_5 = __pyx_pf_5ts2vg_5graph_8_natural_14_compute_graph_add_edge(__pyx_v_add_edge, __pyx_v_i, (__pyx_v_i - __pyx_v_d), __pyx_v_x_a, __pyx_v_x_b, __pyx_v_y_a, __pyx_v_y_b, (-__pyx_v_slope)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 76, __pyx_L1_error)
+            __pyx_t_5 = __pyx_pf_5ts2vg_5graph_8_natural_14_compute_graph_add_edge(__pyx_v_add_edge, __pyx_v_i, (__pyx_v_i - __pyx_v_d), __pyx_v_x_a, __pyx_v_x_b, __pyx_v_y_a, __pyx_v_y_b, (-__pyx_v_slope)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 81, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_5);
             __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-            /* "ts2vg/graph/_natural.pyx":75
+            /* "ts2vg/graph/_natural.pyx":80
  * 
  *                 if _greater(slope, max_slope, tol):
  *                     if directed == _DIRECTED_TOP_TO_BOTTOM:             # <<<<<<<<<<<<<<
  *                         add_edge(i, i-d, x_a, x_b, y_a, y_b, -slope)
  *                     else:  # left_to_right
  */
             goto __pyx_L9;
           }
 
-          /* "ts2vg/graph/_natural.pyx":78
+          /* "ts2vg/graph/_natural.pyx":83
  *                         add_edge(i, i-d, x_a, x_b, y_a, y_b, -slope)
  *                     else:  # left_to_right
  *                         add_edge(i-d, i, x_b, x_a, y_b, y_a, -slope)             # <<<<<<<<<<<<<<
  * 
  *                     max_slope = slope
  */
           /*else*/ {
-            __pyx_t_5 = __pyx_pf_5ts2vg_5graph_8_natural_14_compute_graph_add_edge(__pyx_v_add_edge, (__pyx_v_i - __pyx_v_d), __pyx_v_i, __pyx_v_x_b, __pyx_v_x_a, __pyx_v_y_b, __pyx_v_y_a, (-__pyx_v_slope)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 78, __pyx_L1_error)
+            __pyx_t_5 = __pyx_pf_5ts2vg_5graph_8_natural_14_compute_graph_add_edge(__pyx_v_add_edge, (__pyx_v_i - __pyx_v_d), __pyx_v_i, __pyx_v_x_b, __pyx_v_x_a, __pyx_v_y_b, __pyx_v_y_a, (-__pyx_v_slope)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 83, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_5);
             __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           }
           __pyx_L9:;
 
-          /* "ts2vg/graph/_natural.pyx":80
+          /* "ts2vg/graph/_natural.pyx":85
  *                         add_edge(i-d, i, x_b, x_a, y_b, y_a, -slope)
  * 
  *                     max_slope = slope             # <<<<<<<<<<<<<<
  * 
  * 
  */
           __pyx_v_max_slope = __pyx_v_slope;
 
-          /* "ts2vg/graph/_natural.pyx":74
+          /* "ts2vg/graph/_natural.pyx":79
  *                 tol = max(ABS_TOL, REL_TOL * max(fabs(x_a), fabs(x_b), fabs(y_a), fabs(y_b)))
  * 
  *                 if _greater(slope, max_slope, tol):             # <<<<<<<<<<<<<<
  *                     if directed == _DIRECTED_TOP_TO_BOTTOM:
  *                         add_edge(i, i-d, x_a, x_b, y_a, y_b, -slope)
  */
         }
       }
 
-      /* "ts2vg/graph/_natural.pyx":84
+      /* "ts2vg/graph/_natural.pyx":89
  * 
  *             # sweep from i towards the right
  *             max_slope = -INFINITY             # <<<<<<<<<<<<<<
  *             for d in range(1, right-i):
  *                 x_b = xs[i+d]
  */
       __pyx_v_max_slope = (-INFINITY);
 
-      /* "ts2vg/graph/_natural.pyx":85
+      /* "ts2vg/graph/_natural.pyx":90
  *             # sweep from i towards the right
  *             max_slope = -INFINITY
  *             for d in range(1, right-i):             # <<<<<<<<<<<<<<
  *                 x_b = xs[i+d]
  *                 y_b = ts[i+d]
  */
       __pyx_t_3 = (__pyx_v_right - __pyx_v_i);
       __pyx_t_20 = __pyx_t_3;
       for (__pyx_t_21 = 1; __pyx_t_21 < __pyx_t_20; __pyx_t_21+=1) {
         __pyx_v_d = __pyx_t_21;
 
-        /* "ts2vg/graph/_natural.pyx":86
+        /* "ts2vg/graph/_natural.pyx":91
  *             max_slope = -INFINITY
  *             for d in range(1, right-i):
  *                 x_b = xs[i+d]             # <<<<<<<<<<<<<<
  *                 y_b = ts[i+d]
  *                 slope = (y_b-y_a) / (x_b-x_a)
  */
         __pyx_t_12 = (__pyx_v_i + __pyx_v_d);
         __pyx_v_x_b = (*((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_xs.data + __pyx_t_12 * __pyx_v_xs.strides[0]) )));
 
-        /* "ts2vg/graph/_natural.pyx":87
+        /* "ts2vg/graph/_natural.pyx":92
  *             for d in range(1, right-i):
  *                 x_b = xs[i+d]
  *                 y_b = ts[i+d]             # <<<<<<<<<<<<<<
  *                 slope = (y_b-y_a) / (x_b-x_a)
  *                 tol = max(ABS_TOL, REL_TOL * max(fabs(x_a), fabs(x_b), fabs(y_a), fabs(y_b)))
  */
         __pyx_t_12 = (__pyx_v_i + __pyx_v_d);
         __pyx_v_y_b = (*((__pyx_t_5numpy_float64_t *) ( /* dim=0 */ (__pyx_v_ts.data + __pyx_t_12 * __pyx_v_ts.strides[0]) )));
 
-        /* "ts2vg/graph/_natural.pyx":88
+        /* "ts2vg/graph/_natural.pyx":93
  *                 x_b = xs[i+d]
  *                 y_b = ts[i+d]
  *                 slope = (y_b-y_a) / (x_b-x_a)             # <<<<<<<<<<<<<<
  *                 tol = max(ABS_TOL, REL_TOL * max(fabs(x_a), fabs(x_b), fabs(y_a), fabs(y_b)))
  * 
  */
         __pyx_v_slope = ((__pyx_v_y_b - __pyx_v_y_a) / (__pyx_v_x_b - __pyx_v_x_a));
 
-        /* "ts2vg/graph/_natural.pyx":89
+        /* "ts2vg/graph/_natural.pyx":94
  *                 y_b = ts[i+d]
  *                 slope = (y_b-y_a) / (x_b-x_a)
  *                 tol = max(ABS_TOL, REL_TOL * max(fabs(x_a), fabs(x_b), fabs(y_a), fabs(y_b)))             # <<<<<<<<<<<<<<
  * 
  *                 if _greater(slope, max_slope, tol):
  */
         __pyx_t_16 = fabs(__pyx_v_x_b);
@@ -3955,160 +3976,168 @@
         if (((__pyx_t_16 > __pyx_t_18) != 0)) {
           __pyx_t_15 = __pyx_t_16;
         } else {
           __pyx_t_15 = __pyx_t_18;
         }
         __pyx_v_tol = __pyx_t_15;
 
-        /* "ts2vg/graph/_natural.pyx":91
+        /* "ts2vg/graph/_natural.pyx":96
  *                 tol = max(ABS_TOL, REL_TOL * max(fabs(x_a), fabs(x_b), fabs(y_a), fabs(y_b)))
  * 
  *                 if _greater(slope, max_slope, tol):             # <<<<<<<<<<<<<<
  *                     # note, single case works for both top_to_bottom and left_to_right orders
  *                     add_edge(i, i+d, x_a, x_b, y_a, y_b, slope)
  */
         __pyx_t_9 = (__pyx_f_5ts2vg_5graph_5_base__greater(__pyx_v_slope, __pyx_v_max_slope, __pyx_v_tol) != 0);
         if (__pyx_t_9) {
 
-          /* "ts2vg/graph/_natural.pyx":93
+          /* "ts2vg/graph/_natural.pyx":98
  *                 if _greater(slope, max_slope, tol):
  *                     # note, single case works for both top_to_bottom and left_to_right orders
  *                     add_edge(i, i+d, x_a, x_b, y_a, y_b, slope)             # <<<<<<<<<<<<<<
  * 
  *                     max_slope = slope
  */
-          __pyx_t_5 = __pyx_pf_5ts2vg_5graph_8_natural_14_compute_graph_add_edge(__pyx_v_add_edge, __pyx_v_i, (__pyx_v_i + __pyx_v_d), __pyx_v_x_a, __pyx_v_x_b, __pyx_v_y_a, __pyx_v_y_b, __pyx_v_slope); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L1_error)
+          __pyx_t_5 = __pyx_pf_5ts2vg_5graph_8_natural_14_compute_graph_add_edge(__pyx_v_add_edge, __pyx_v_i, (__pyx_v_i + __pyx_v_d), __pyx_v_x_a, __pyx_v_x_b, __pyx_v_y_a, __pyx_v_y_b, __pyx_v_slope); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 98, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-          /* "ts2vg/graph/_natural.pyx":95
+          /* "ts2vg/graph/_natural.pyx":100
  *                     add_edge(i, i+d, x_a, x_b, y_a, y_b, slope)
  * 
  *                     max_slope = slope             # <<<<<<<<<<<<<<
  * 
- *             queue.push((left, i))
+ *             queue.push(uint_pair(left, i))
  */
           __pyx_v_max_slope = __pyx_v_slope;
 
-          /* "ts2vg/graph/_natural.pyx":91
+          /* "ts2vg/graph/_natural.pyx":96
  *                 tol = max(ABS_TOL, REL_TOL * max(fabs(x_a), fabs(x_b), fabs(y_a), fabs(y_b)))
  * 
  *                 if _greater(slope, max_slope, tol):             # <<<<<<<<<<<<<<
  *                     # note, single case works for both top_to_bottom and left_to_right orders
  *                     add_edge(i, i+d, x_a, x_b, y_a, y_b, slope)
  */
         }
       }
 
-      /* "ts2vg/graph/_natural.pyx":97
+      /* "ts2vg/graph/_natural.pyx":102
  *                     max_slope = slope
  * 
- *             queue.push((left, i))             # <<<<<<<<<<<<<<
- *             queue.push((i+1, right))
+ *             queue.push(uint_pair(left, i))             # <<<<<<<<<<<<<<
+ *             queue.push(uint_pair(i+1, right))
  * 
  */
-      __pyx_t_8.f0 = __pyx_v_left;
-      __pyx_t_8.f1 = __pyx_v_i;
-      ((struct __pyx_vtabstruct_5ts2vg_5utils_9pairqueue_PairQueue *)__pyx_v_queue->__pyx_vtab)->push(__pyx_v_queue, __pyx_t_8);
+      try {
+        __pyx_t_8 = __pyx_t_5ts2vg_5graph_8_natural_uint_pair(__pyx_v_left, __pyx_v_i);
+      } catch(...) {
+        __Pyx_CppExn2PyErr();
+        __PYX_ERR(0, 102, __pyx_L1_error)
+      }
+      __pyx_v_queue.push(__pyx_t_8);
 
-      /* "ts2vg/graph/_natural.pyx":98
+      /* "ts2vg/graph/_natural.pyx":103
  * 
- *             queue.push((left, i))
- *             queue.push((i+1, right))             # <<<<<<<<<<<<<<
+ *             queue.push(uint_pair(left, i))
+ *             queue.push(uint_pair(i+1, right))             # <<<<<<<<<<<<<<
  * 
  *     return edges, np.asarray(degrees_in, dtype=np.uint32), np.asarray(degrees_out, dtype=np.uint32)
  */
-      __pyx_t_8.f0 = (__pyx_v_i + 1);
-      __pyx_t_8.f1 = __pyx_v_right;
-      ((struct __pyx_vtabstruct_5ts2vg_5utils_9pairqueue_PairQueue *)__pyx_v_queue->__pyx_vtab)->push(__pyx_v_queue, __pyx_t_8);
+      try {
+        __pyx_t_8 = __pyx_t_5ts2vg_5graph_8_natural_uint_pair((__pyx_v_i + 1), __pyx_v_right);
+      } catch(...) {
+        __Pyx_CppExn2PyErr();
+        __PYX_ERR(0, 103, __pyx_L1_error)
+      }
+      __pyx_v_queue.push(__pyx_t_8);
 
-      /* "ts2vg/graph/_natural.pyx":61
- *         (left, right) = queue.pop()
+      /* "ts2vg/graph/_natural.pyx":66
+ *         queue.pop()
  * 
  *         if left+1 < right:             # <<<<<<<<<<<<<<
  *             i = _argmax(ts, left, right)
  *             x_a = xs[i]
  */
     }
   }
 
-  /* "ts2vg/graph/_natural.pyx":100
- *             queue.push((i+1, right))
+  /* "ts2vg/graph/_natural.pyx":105
+ *             queue.push(uint_pair(i+1, right))
  * 
  *     return edges, np.asarray(degrees_in, dtype=np.uint32), np.asarray(degrees_out, dtype=np.uint32)             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_asarray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_asarray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __pyx_memoryview_fromslice(__pyx_cur_scope->__pyx_v_degrees_in, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint32_t, 0);; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_5 = __pyx_memoryview_fromslice(__pyx_cur_scope->__pyx_v_degrees_in, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint32_t, 0);; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 100, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_asarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_asarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __pyx_memoryview_fromslice(__pyx_cur_scope->__pyx_v_degrees_out, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint32_t, 0);; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_5 = __pyx_memoryview_fromslice(__pyx_cur_scope->__pyx_v_degrees_out, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_5numpy_uint32_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_5numpy_uint32_t, 0);; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint32); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_uint32); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_22);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_22) < 0) __PYX_ERR(0, 100, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_22) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-  __pyx_t_22 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_22 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_22);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_edges);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_edges);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_cur_scope->__pyx_v_edges);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_22);
   PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_22);
   __pyx_t_1 = 0;
   __pyx_t_22 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "ts2vg/graph/_natural.pyx":23
+  /* "ts2vg/graph/_natural.pyx":26
  * @cython.wraparound(False)
  * @cython.cdivision(True)
  * def _compute_graph(np.float64_t[:] ts, np.float64_t[:] xs, uint directed, uint weighted, bint only_degrees, double min_weight, double max_weight):             # <<<<<<<<<<<<<<
  *     """
  *     Computes the visibility graph of a time series
  */
 
@@ -4120,25 +4149,24 @@
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __PYX_XDEC_MEMVIEW(&__pyx_t_7, 1);
   __Pyx_XDECREF(__pyx_t_22);
   __Pyx_AddTraceback("ts2vg.graph._natural._compute_graph", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_queue);
   __Pyx_XDECREF(__pyx_v_add_edge);
   __PYX_XDEC_MEMVIEW(&__pyx_v_ts, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_xs, 1);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4147,29 +4175,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4180,15 +4208,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4197,29 +4225,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4230,15 +4258,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4247,29 +4275,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4280,15 +4308,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4297,29 +4325,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4330,15 +4358,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4347,29 +4375,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4380,212 +4408,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4601,15 +4629,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4617,53 +4645,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -4671,30 +4699,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4709,15 +4737,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4733,15 +4761,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4749,53 +4777,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -4803,30 +4831,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4841,15 +4869,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4865,15 +4893,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4881,53 +4909,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -4935,30 +4963,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4973,176 +5001,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19169,14 +19197,15 @@
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
   {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
   {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
   {&__pyx_n_s_only_degrees, __pyx_k_only_degrees, sizeof(__pyx_k_only_degrees), 0, 0, 1, 1},
   {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
+  {&__pyx_n_s_pair, __pyx_k_pair, sizeof(__pyx_k_pair), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_getbuffer, __pyx_k_pyx_getbuffer, sizeof(__pyx_k_pyx_getbuffer), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
@@ -19225,15 +19254,15 @@
   {&__pyx_n_s_y2, __pyx_k_y2, sizeof(__pyx_k_y2), 0, 0, 1, 1},
   {&__pyx_n_s_y_a, __pyx_k_y_a, sizeof(__pyx_k_y_a), 0, 0, 1, 1},
   {&__pyx_n_s_y_b, __pyx_k_y_b, sizeof(__pyx_k_y_b), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 73, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 134, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 152, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 615, __pyx_L1_error)
@@ -19243,38 +19272,38 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "ts2vg/graph/_natural.pyx":42
- *     queue.push((0, n))
+  /* "ts2vg/graph/_natural.pyx":45
+ *     queue.push(uint_pair(0, n))
  * 
  *     def add_edge(uint i1, uint i2, double x1, double x2, double y1, double y2, double slope):             # <<<<<<<<<<<<<<
  *         w = weight_func(x1, x2, y1, y2, slope)
  * 
  */
-  __pyx_tuple_ = PyTuple_Pack(8, __pyx_n_s_i1, __pyx_n_s_i2, __pyx_n_s_x1, __pyx_n_s_x2, __pyx_n_s_y1, __pyx_n_s_y2, __pyx_n_s_slope, __pyx_n_s_w); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(8, __pyx_n_s_i1, __pyx_n_s_i2, __pyx_n_s_x1, __pyx_n_s_x2, __pyx_n_s_y1, __pyx_n_s_y2, __pyx_n_s_slope, __pyx_n_s_w); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
-  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(7, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ts2vg_graph__natural_pyx, __pyx_n_s_add_edge, 42, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(7, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ts2vg_graph__natural_pyx, __pyx_n_s_add_edge, 45, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 45, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 950, __pyx_L1_error)
@@ -19472,25 +19501,25 @@
   __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
   __pyx_tuple__23 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
 
-  /* "ts2vg/graph/_natural.pyx":23
+  /* "ts2vg/graph/_natural.pyx":26
  * @cython.wraparound(False)
  * @cython.cdivision(True)
  * def _compute_graph(np.float64_t[:] ts, np.float64_t[:] xs, uint directed, uint weighted, bint only_degrees, double min_weight, double max_weight):             # <<<<<<<<<<<<<<
  *     """
  *     Computes the visibility graph of a time series
  */
-  __pyx_tuple__24 = PyTuple_Pack(27, __pyx_n_s_ts, __pyx_n_s_xs, __pyx_n_s_directed, __pyx_n_s_weighted, __pyx_n_s_only_degrees, __pyx_n_s_min_weight, __pyx_n_s_max_weight, __pyx_n_s_n, __pyx_n_s_edges, __pyx_n_s_degrees_in, __pyx_n_s_degrees_out, __pyx_n_s_left, __pyx_n_s_right, __pyx_n_s_i, __pyx_n_s_d, __pyx_n_s_x_a, __pyx_n_s_x_b, __pyx_n_s_y_a, __pyx_n_s_y_b, __pyx_n_s_slope, __pyx_n_s_max_slope, __pyx_n_s_w, __pyx_n_s_weight_func, __pyx_n_s_queue, __pyx_n_s_add_edge, __pyx_n_s_add_edge, __pyx_n_s_tol); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(28, __pyx_n_s_ts, __pyx_n_s_xs, __pyx_n_s_directed, __pyx_n_s_weighted, __pyx_n_s_only_degrees, __pyx_n_s_min_weight, __pyx_n_s_max_weight, __pyx_n_s_n, __pyx_n_s_edges, __pyx_n_s_degrees_in, __pyx_n_s_degrees_out, __pyx_n_s_left, __pyx_n_s_right, __pyx_n_s_i, __pyx_n_s_d, __pyx_n_s_x_a, __pyx_n_s_x_b, __pyx_n_s_y_a, __pyx_n_s_y_b, __pyx_n_s_slope, __pyx_n_s_max_slope, __pyx_n_s_w, __pyx_n_s_weight_func, __pyx_n_s_queue, __pyx_n_s_add_edge, __pyx_n_s_add_edge, __pyx_n_s_pair, __pyx_n_s_tol); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(7, 0, 27, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ts2vg_graph__natural_pyx, __pyx_n_s_compute_graph, 23, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(7, 0, 28, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ts2vg_graph__natural_pyx, __pyx_n_s_compute_graph, 26, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 26, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
@@ -19612,15 +19641,15 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_5ts2vg_5graph_8_natural___pyx_scope_struct___compute_graph) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_5ts2vg_5graph_8_natural___pyx_scope_struct___compute_graph) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_5ts2vg_5graph_8_natural___pyx_scope_struct___compute_graph.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_5ts2vg_5graph_8_natural___pyx_scope_struct___compute_graph.tp_dictoffset && __pyx_type_5ts2vg_5graph_8_natural___pyx_scope_struct___compute_graph.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_5ts2vg_5graph_8_natural___pyx_scope_struct___compute_graph.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_5ts2vg_5graph_8_natural___pyx_scope_struct___compute_graph = &__pyx_type_5ts2vg_5graph_8_natural___pyx_scope_struct___compute_graph;
@@ -19690,60 +19719,69 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("ts2vg.utils.pairqueue"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 15, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5ts2vg_5utils_9pairqueue_PairQueue = __Pyx_ImportType(__pyx_t_1, "ts2vg.utils.pairqueue", "PairQueue", sizeof(struct __pyx_obj_5ts2vg_5utils_9pairqueue_PairQueue), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5ts2vg_5utils_9pairqueue_PairQueue) __PYX_ERR(4, 15, __pyx_L1_error)
-  __pyx_vtabptr_5ts2vg_5utils_9pairqueue_PairQueue = (struct __pyx_vtabstruct_5ts2vg_5utils_9pairqueue_PairQueue*)__Pyx_GetVtable(__pyx_ptype_5ts2vg_5utils_9pairqueue_PairQueue->tp_dict); if (unlikely(!__pyx_vtabptr_5ts2vg_5utils_9pairqueue_PairQueue)) __PYX_ERR(4, 15, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -19977,113 +20015,113 @@
   (void)__Pyx_modinit_variable_import_code();
   if (unlikely(__Pyx_modinit_function_import_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "ts2vg/graph/_natural.pyx":4
+  /* "ts2vg/graph/_natural.pyx":5
  * 
  * cimport cython
  * import numpy as np             # <<<<<<<<<<<<<<
  * cimport numpy as np
  * from libc.math cimport fabs, INFINITY
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "ts2vg/graph/_natural.pyx":9
+  /* "ts2vg/graph/_natural.pyx":11
+ * from libcpp.pair cimport pair as cpair
  * 
- * from ts2vg.utils.pairqueue cimport PairQueue
  * from ts2vg.graph.base import _DIRECTED_OPTIONS             # <<<<<<<<<<<<<<
  * from ts2vg.graph._base cimport _greater, _argmax, _get_weight_func, weight_func_type
  * 
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_DIRECTED_OPTIONS);
   __Pyx_GIVEREF(__pyx_n_s_DIRECTED_OPTIONS);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_DIRECTED_OPTIONS);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_ts2vg_graph_base, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_ts2vg_graph_base, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_DIRECTED_OPTIONS); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_DIRECTED_OPTIONS); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_DIRECTED_OPTIONS, __pyx_t_1) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_DIRECTED_OPTIONS, __pyx_t_1) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "ts2vg/graph/_natural.pyx":14
- * ctypedef unsigned int uint
+  /* "ts2vg/graph/_natural.pyx":17
+ * ctypedef cpair[uint, uint] uint_pair
  * 
  * cdef double ABS_TOL = 1e-14             # <<<<<<<<<<<<<<
  * cdef double REL_TOL = 1e-14
  * cdef uint _DIRECTED_LEFT_TO_RIGHT = _DIRECTED_OPTIONS['left_to_right']
  */
   __pyx_v_5ts2vg_5graph_8_natural_ABS_TOL = 1e-14;
 
-  /* "ts2vg/graph/_natural.pyx":15
+  /* "ts2vg/graph/_natural.pyx":18
  * 
  * cdef double ABS_TOL = 1e-14
  * cdef double REL_TOL = 1e-14             # <<<<<<<<<<<<<<
  * cdef uint _DIRECTED_LEFT_TO_RIGHT = _DIRECTED_OPTIONS['left_to_right']
  * cdef uint _DIRECTED_TOP_TO_BOTTOM = _DIRECTED_OPTIONS['top_to_bottom']
  */
   __pyx_v_5ts2vg_5graph_8_natural_REL_TOL = 1e-14;
 
-  /* "ts2vg/graph/_natural.pyx":16
+  /* "ts2vg/graph/_natural.pyx":19
  * cdef double ABS_TOL = 1e-14
  * cdef double REL_TOL = 1e-14
  * cdef uint _DIRECTED_LEFT_TO_RIGHT = _DIRECTED_OPTIONS['left_to_right']             # <<<<<<<<<<<<<<
  * cdef uint _DIRECTED_TOP_TO_BOTTOM = _DIRECTED_OPTIONS['top_to_bottom']
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DIRECTED_OPTIONS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DIRECTED_OPTIONS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_2, __pyx_n_u_left_to_right); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_2, __pyx_n_u_left_to_right); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __Pyx_PyInt_As_unsigned_int(__pyx_t_1); if (unlikely((__pyx_t_3 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_unsigned_int(__pyx_t_1); if (unlikely((__pyx_t_3 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_5ts2vg_5graph_8_natural__DIRECTED_LEFT_TO_RIGHT = __pyx_t_3;
 
-  /* "ts2vg/graph/_natural.pyx":17
+  /* "ts2vg/graph/_natural.pyx":20
  * cdef double REL_TOL = 1e-14
  * cdef uint _DIRECTED_LEFT_TO_RIGHT = _DIRECTED_OPTIONS['left_to_right']
  * cdef uint _DIRECTED_TOP_TO_BOTTOM = _DIRECTED_OPTIONS['top_to_bottom']             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DIRECTED_OPTIONS); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DIRECTED_OPTIONS); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_top_to_bottom); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_top_to_bottom); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyInt_As_unsigned_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_unsigned_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_5ts2vg_5graph_8_natural__DIRECTED_TOP_TO_BOTTOM = __pyx_t_3;
 
-  /* "ts2vg/graph/_natural.pyx":23
+  /* "ts2vg/graph/_natural.pyx":26
  * @cython.wraparound(False)
  * @cython.cdivision(True)
  * def _compute_graph(np.float64_t[:] ts, np.float64_t[:] xs, uint directed, uint weighted, bint only_degrees, double min_weight, double max_weight):             # <<<<<<<<<<<<<<
  *     """
  *     Computes the visibility graph of a time series
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5ts2vg_5graph_8_natural_1_compute_graph, NULL, __pyx_n_s_ts2vg_graph__natural); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5ts2vg_5graph_8_natural_1_compute_graph, NULL, __pyx_n_s_ts2vg_graph__natural); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compute_graph, __pyx_t_2) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compute_graph, __pyx_t_2) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "ts2vg/graph/_natural.pyx":1
  * #cython: language_level=3             # <<<<<<<<<<<<<<
+ * #distutils: language=c++
  * 
- * cimport cython
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "View.MemoryView":210
@@ -20534,175 +20572,14 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
-/* PyFunctionFastCall */
-#if CYTHON_FAST_PYCALL
-static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
-                                               PyObject *globals) {
-    PyFrameObject *f;
-    PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject **fastlocals;
-    Py_ssize_t i;
-    PyObject *result;
-    assert(globals != NULL);
-    /* XXX Perhaps we should create a specialized
-       PyFrame_New() that doesn't take locals, but does
-       take builtins without sanity checking them.
-       */
-    assert(tstate != NULL);
-    f = PyFrame_New(tstate, co, globals, NULL);
-    if (f == NULL) {
-        return NULL;
-    }
-    fastlocals = __Pyx_PyFrame_GetLocalsplus(f);
-    for (i = 0; i < na; i++) {
-        Py_INCREF(*args);
-        fastlocals[i] = *args++;
-    }
-    result = PyEval_EvalFrameEx(f,0);
-    ++tstate->recursion_depth;
-    Py_DECREF(f);
-    --tstate->recursion_depth;
-    return result;
-}
-#if 1 || PY_VERSION_HEX < 0x030600B1
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
-    PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
-    PyObject *globals = PyFunction_GET_GLOBALS(func);
-    PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
-    PyObject *closure;
-#if PY_MAJOR_VERSION >= 3
-    PyObject *kwdefs;
-#endif
-    PyObject *kwtuple, **k;
-    PyObject **d;
-    Py_ssize_t nd;
-    Py_ssize_t nk;
-    PyObject *result;
-    assert(kwargs == NULL || PyDict_Check(kwargs));
-    nk = kwargs ? PyDict_Size(kwargs) : 0;
-    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
-        return NULL;
-    }
-    if (
-#if PY_MAJOR_VERSION >= 3
-            co->co_kwonlyargcount == 0 &&
-#endif
-            likely(kwargs == NULL || nk == 0) &&
-            co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
-        if (argdefs == NULL && co->co_argcount == nargs) {
-            result = __Pyx_PyFunction_FastCallNoKw(co, args, nargs, globals);
-            goto done;
-        }
-        else if (nargs == 0 && argdefs != NULL
-                 && co->co_argcount == Py_SIZE(argdefs)) {
-            /* function called with no arguments, but all parameters have
-               a default value: use default values as arguments .*/
-            args = &PyTuple_GET_ITEM(argdefs, 0);
-            result =__Pyx_PyFunction_FastCallNoKw(co, args, Py_SIZE(argdefs), globals);
-            goto done;
-        }
-    }
-    if (kwargs != NULL) {
-        Py_ssize_t pos, i;
-        kwtuple = PyTuple_New(2 * nk);
-        if (kwtuple == NULL) {
-            result = NULL;
-            goto done;
-        }
-        k = &PyTuple_GET_ITEM(kwtuple, 0);
-        pos = i = 0;
-        while (PyDict_Next(kwargs, &pos, &k[i], &k[i+1])) {
-            Py_INCREF(k[i]);
-            Py_INCREF(k[i+1]);
-            i += 2;
-        }
-        nk = i / 2;
-    }
-    else {
-        kwtuple = NULL;
-        k = NULL;
-    }
-    closure = PyFunction_GET_CLOSURE(func);
-#if PY_MAJOR_VERSION >= 3
-    kwdefs = PyFunction_GET_KW_DEFAULTS(func);
-#endif
-    if (argdefs != NULL) {
-        d = &PyTuple_GET_ITEM(argdefs, 0);
-        nd = Py_SIZE(argdefs);
-    }
-    else {
-        d = NULL;
-        nd = 0;
-    }
-#if PY_MAJOR_VERSION >= 3
-    result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
-                               args, (int)nargs,
-                               k, (int)nk,
-                               d, (int)nd, kwdefs, closure);
-#else
-    result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
-                               args, (int)nargs,
-                               k, (int)nk,
-                               d, (int)nd, closure);
-#endif
-    Py_XDECREF(kwtuple);
-done:
-    Py_LeaveRecursiveCall();
-    return result;
-}
-#endif
-#endif
-
-/* PyObjectCallMethO */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
-    PyObject *self, *result;
-    PyCFunction cfunc;
-    cfunc = PyCFunction_GET_FUNCTION(func);
-    self = PyCFunction_GET_SELF(func);
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    result = cfunc(self, arg);
-    Py_LeaveRecursiveCall();
-    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
-        PyErr_SetString(
-            PyExc_SystemError,
-            "NULL result without error in PyObject_Call");
-    }
-    return result;
-}
-#endif
-
-/* PyObjectCallNoArg */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, NULL, 0);
-    }
-#endif
-#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
-    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
-#else
-    if (likely(PyCFunction_Check(func)))
-#endif
-    {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-            return __Pyx_PyObject_CallMethO(func, NULL);
-        }
-    }
-    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
-}
-#endif
-
 /* FetchCommonType */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
     PyObject* fake_module;
     PyTypeObject* cached_type = NULL;
     fake_module = PyImport_AddModule((char*) "_cython_" CYTHON_ABI);
     if (!fake_module) return NULL;
     Py_INCREF(fake_module);
@@ -21811,28 +21688,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -21877,14 +21754,133 @@
         return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
     } else {
         return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
     }
 }
 #endif
 
+/* PyFunctionFastCall */
+#if CYTHON_FAST_PYCALL
+static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
+                                               PyObject *globals) {
+    PyFrameObject *f;
+    PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject **fastlocals;
+    Py_ssize_t i;
+    PyObject *result;
+    assert(globals != NULL);
+    /* XXX Perhaps we should create a specialized
+       PyFrame_New() that doesn't take locals, but does
+       take builtins without sanity checking them.
+       */
+    assert(tstate != NULL);
+    f = PyFrame_New(tstate, co, globals, NULL);
+    if (f == NULL) {
+        return NULL;
+    }
+    fastlocals = __Pyx_PyFrame_GetLocalsplus(f);
+    for (i = 0; i < na; i++) {
+        Py_INCREF(*args);
+        fastlocals[i] = *args++;
+    }
+    result = PyEval_EvalFrameEx(f,0);
+    ++tstate->recursion_depth;
+    Py_DECREF(f);
+    --tstate->recursion_depth;
+    return result;
+}
+#if 1 || PY_VERSION_HEX < 0x030600B1
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
+    PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
+    PyObject *globals = PyFunction_GET_GLOBALS(func);
+    PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
+    PyObject *closure;
+#if PY_MAJOR_VERSION >= 3
+    PyObject *kwdefs;
+#endif
+    PyObject *kwtuple, **k;
+    PyObject **d;
+    Py_ssize_t nd;
+    Py_ssize_t nk;
+    PyObject *result;
+    assert(kwargs == NULL || PyDict_Check(kwargs));
+    nk = kwargs ? PyDict_Size(kwargs) : 0;
+    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
+        return NULL;
+    }
+    if (
+#if PY_MAJOR_VERSION >= 3
+            co->co_kwonlyargcount == 0 &&
+#endif
+            likely(kwargs == NULL || nk == 0) &&
+            co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
+        if (argdefs == NULL && co->co_argcount == nargs) {
+            result = __Pyx_PyFunction_FastCallNoKw(co, args, nargs, globals);
+            goto done;
+        }
+        else if (nargs == 0 && argdefs != NULL
+                 && co->co_argcount == Py_SIZE(argdefs)) {
+            /* function called with no arguments, but all parameters have
+               a default value: use default values as arguments .*/
+            args = &PyTuple_GET_ITEM(argdefs, 0);
+            result =__Pyx_PyFunction_FastCallNoKw(co, args, Py_SIZE(argdefs), globals);
+            goto done;
+        }
+    }
+    if (kwargs != NULL) {
+        Py_ssize_t pos, i;
+        kwtuple = PyTuple_New(2 * nk);
+        if (kwtuple == NULL) {
+            result = NULL;
+            goto done;
+        }
+        k = &PyTuple_GET_ITEM(kwtuple, 0);
+        pos = i = 0;
+        while (PyDict_Next(kwargs, &pos, &k[i], &k[i+1])) {
+            Py_INCREF(k[i]);
+            Py_INCREF(k[i+1]);
+            i += 2;
+        }
+        nk = i / 2;
+    }
+    else {
+        kwtuple = NULL;
+        k = NULL;
+    }
+    closure = PyFunction_GET_CLOSURE(func);
+#if PY_MAJOR_VERSION >= 3
+    kwdefs = PyFunction_GET_KW_DEFAULTS(func);
+#endif
+    if (argdefs != NULL) {
+        d = &PyTuple_GET_ITEM(argdefs, 0);
+        nd = Py_SIZE(argdefs);
+    }
+    else {
+        d = NULL;
+        nd = 0;
+    }
+#if PY_MAJOR_VERSION >= 3
+    result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
+                               args, (int)nargs,
+                               k, (int)nk,
+                               d, (int)nd, kwdefs, closure);
+#else
+    result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
+                               args, (int)nargs,
+                               k, (int)nk,
+                               d, (int)nd, closure);
+#endif
+    Py_XDECREF(kwtuple);
+done:
+    Py_LeaveRecursiveCall();
+    return result;
+}
+#endif
+#endif
+
 /* PyObjectCall2Args */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
     PyObject *args, *result = NULL;
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(function)) {
         PyObject *args[2] = {arg1, arg2};
         return __Pyx_PyFunction_FastCall(function, args, 2);
@@ -21906,14 +21902,34 @@
     result = __Pyx_PyObject_Call(function, args, NULL);
     Py_DECREF(args);
     Py_DECREF(function);
 done:
     return result;
 }
 
+/* PyObjectCallMethO */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
+    PyObject *self, *result;
+    PyCFunction cfunc;
+    cfunc = PyCFunction_GET_FUNCTION(func);
+    self = PyCFunction_GET_SELF(func);
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    result = cfunc(self, arg);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
+    }
+    return result;
+}
+#endif
+
 /* PyObjectCallOneArg */
 #if CYTHON_COMPILING_IN_CPYTHON
 static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
     PyObject *result;
     PyObject *args = PyTuple_New(1);
     if (unlikely(!args)) return NULL;
     Py_INCREF(arg);
@@ -22878,44 +22894,62 @@
     return ret;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
@@ -22935,34 +22969,14 @@
     return (PyTypeObject *)result;
 bad:
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
-/* GetVTable */
-static void* __Pyx_GetVtable(PyObject *dict) {
-    void* ptr;
-    PyObject *ob = PyObject_GetItem(dict, __pyx_n_s_pyx_vtable);
-    if (!ob)
-        goto bad;
-#if PY_VERSION_HEX >= 0x02070000
-    ptr = PyCapsule_GetPointer(ob, 0);
-#else
-    ptr = PyCObject_AsVoidPtr(ob);
-#endif
-    if (!ptr && !PyErr_Occurred())
-        PyErr_SetString(PyExc_RuntimeError, "invalid vtable found for imported type");
-    Py_DECREF(ob);
-    return ptr;
-bad:
-    Py_XDECREF(ob);
-    return NULL;
-}
-
 /* DictGetItem */
 #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
 static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
     PyObject *value;
     value = PyDict_GetItemWithError(d, key);
     if (unlikely(!value)) {
         if (!PyErr_Occurred()) {
```

### Comparing `ts2vg-1.2.1/ts2vg/graph/_natural_penetrable.c` & `ts2vg-1.2.2/ts2vg/graph/_natural_penetrable.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/core/include"
         ],
         "name": "ts2vg.graph._natural_penetrable",
         "sources": [
             "ts2vg/graph/_natural_penetrable.pyx"
         ]
     },
     "module_name": "ts2vg.graph._natural_penetrable"
@@ -33,16 +33,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -227,15 +227,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -266,15 +266,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1120,195 +1120,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1358,42 +1358,42 @@
 /*--- Type declarations ---*/
 struct __pyx_obj_5ts2vg_5graph_19_natural_penetrable___pyx_scope_struct___compute_graph;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2122,20 +2122,28 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* DictGetItem.proto */
 #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
 static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
 #define __Pyx_PyObject_Dict_GetItem(obj, name)\
     (likely(PyDict_CheckExact(obj)) ?\
@@ -2539,15 +2547,14 @@
 static const char __pyx_k_x_a[] = "x_a";
 static const char __pyx_k_x_b[] = "x_b";
 static const char __pyx_k_y_a[] = "y_a";
 static const char __pyx_k_y_b[] = "y_b";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_full[] = "full";
-static const char __pyx_k_left[] = "left";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_mode[] = "mode";
 static const char __pyx_k_name[] = "name";
 static const char __pyx_k_ndim[] = "ndim";
 static const char __pyx_k_pack[] = "pack";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_step[] = "step";
@@ -2557,15 +2564,14 @@
 static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_edges[] = "edges";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_flags[] = "flags";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_range[] = "range";
-static const char __pyx_k_right[] = "right";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_slope[] = "slope";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_zeros[] = "zeros";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
@@ -2719,15 +2725,14 @@
 static PyObject *__pyx_n_s_i_b;
 static PyObject *__pyx_n_s_id;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_itemsize;
 static PyObject *__pyx_kp_s_itemsize_0_for_cython_array;
 static PyObject *__pyx_n_s_j;
 static PyObject *__pyx_n_s_known_w;
-static PyObject *__pyx_n_s_left;
 static PyObject *__pyx_n_u_left_to_right;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_max_slopes;
 static PyObject *__pyx_n_s_max_weight;
 static PyObject *__pyx_n_s_memview;
 static PyObject *__pyx_n_s_min_weight;
 static PyObject *__pyx_n_s_mode;
@@ -2755,15 +2760,14 @@
 static PyObject *__pyx_n_s_pyx_type;
 static PyObject *__pyx_n_s_pyx_unpickle_Enum;
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
-static PyObject *__pyx_n_s_right;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_shape;
 static PyObject *__pyx_n_s_size;
 static PyObject *__pyx_n_s_slope;
 static PyObject *__pyx_n_s_start;
 static PyObject *__pyx_n_s_step;
@@ -3554,15 +3558,15 @@
   __pyx_t_7.data = NULL;
 
   /* "ts2vg/graph/_natural_penetrable.pyx":41
  *     cdef list edges = []
  *     cdef np.uint32_t[:] degrees_in = np.zeros(n, dtype=np.uint32)
  *     cdef np.uint32_t[:] degrees_out = np.zeros(n, dtype=np.uint32)             # <<<<<<<<<<<<<<
  * 
- *     cdef uint left, right, i_a, i_b
+ *     cdef uint i_a, i_b
  */
   __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = __Pyx_PyInt_From_unsigned_int(__pyx_v_n); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 41, __pyx_L1_error)
@@ -4102,15 +4106,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_xs, 1);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4119,29 +4123,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4152,15 +4156,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4169,29 +4173,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4202,15 +4206,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4219,29 +4223,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4252,15 +4256,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4269,29 +4273,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4302,15 +4306,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4319,29 +4323,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4352,212 +4356,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4573,15 +4577,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4589,53 +4593,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -4643,30 +4647,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4681,15 +4685,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4705,15 +4709,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4721,53 +4725,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -4775,30 +4779,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4813,15 +4817,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4837,15 +4841,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4853,53 +4857,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -4907,30 +4911,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4945,176 +4949,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19125,15 +19129,14 @@
   {&__pyx_n_s_i_b, __pyx_k_i_b, sizeof(__pyx_k_i_b), 0, 0, 1, 1},
   {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_itemsize, __pyx_k_itemsize, sizeof(__pyx_k_itemsize), 0, 0, 1, 1},
   {&__pyx_kp_s_itemsize_0_for_cython_array, __pyx_k_itemsize_0_for_cython_array, sizeof(__pyx_k_itemsize_0_for_cython_array), 0, 0, 1, 0},
   {&__pyx_n_s_j, __pyx_k_j, sizeof(__pyx_k_j), 0, 0, 1, 1},
   {&__pyx_n_s_known_w, __pyx_k_known_w, sizeof(__pyx_k_known_w), 0, 0, 1, 1},
-  {&__pyx_n_s_left, __pyx_k_left, sizeof(__pyx_k_left), 0, 0, 1, 1},
   {&__pyx_n_u_left_to_right, __pyx_k_left_to_right, sizeof(__pyx_k_left_to_right), 0, 1, 0, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_max_slopes, __pyx_k_max_slopes, sizeof(__pyx_k_max_slopes), 0, 0, 1, 1},
   {&__pyx_n_s_max_weight, __pyx_k_max_weight, sizeof(__pyx_k_max_weight), 0, 0, 1, 1},
   {&__pyx_n_s_memview, __pyx_k_memview, sizeof(__pyx_k_memview), 0, 0, 1, 1},
   {&__pyx_n_s_min_weight, __pyx_k_min_weight, sizeof(__pyx_k_min_weight), 0, 0, 1, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
@@ -19161,15 +19164,14 @@
   {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_Enum, __pyx_k_pyx_unpickle_Enum, sizeof(__pyx_k_pyx_unpickle_Enum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
-  {&__pyx_n_s_right, __pyx_k_right, sizeof(__pyx_k_right), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
   {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
   {&__pyx_n_s_slope, __pyx_k_slope, sizeof(__pyx_k_slope), 0, 0, 1, 1},
   {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
   {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
@@ -19235,26 +19237,26 @@
  *             w = weight_func(x1, x2, y1, y2, slope)
  */
   __pyx_tuple_ = PyTuple_Pack(9, __pyx_n_s_i1, __pyx_n_s_i2, __pyx_n_s_x1, __pyx_n_s_x2, __pyx_n_s_y1, __pyx_n_s_y2, __pyx_n_s_slope, __pyx_n_s_known_w, __pyx_n_s_w); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
   __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(8, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ts2vg_graph__natural_penetrable, __pyx_n_s_add_edge, 52, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 52, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../../../../tmp/build-env-p_kxnkmt/lib/python3.8/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-k4a3migh/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 950, __pyx_L1_error)
@@ -19459,18 +19461,18 @@
   /* "ts2vg/graph/_natural_penetrable.pyx":23
  * @cython.wraparound(False)
  * @cython.cdivision(True)
  * def _compute_graph(np.float64_t[:] ts, np.float64_t[:] xs, uint directed, uint weighted, bint only_degrees, double min_weight, double max_weight, uint penetrable_limit):             # <<<<<<<<<<<<<<
  *     """
  *     Computes the limited penetrable visibility graph of a time series.
  */
-  __pyx_tuple__24 = PyTuple_Pack(30, __pyx_n_s_ts, __pyx_n_s_xs, __pyx_n_s_directed, __pyx_n_s_weighted, __pyx_n_s_only_degrees, __pyx_n_s_min_weight, __pyx_n_s_max_weight, __pyx_n_s_penetrable_limit, __pyx_n_s_n, __pyx_n_s_edges, __pyx_n_s_degrees_in, __pyx_n_s_degrees_out, __pyx_n_s_left, __pyx_n_s_right, __pyx_n_s_i_a, __pyx_n_s_i_b, __pyx_n_s_x_a, __pyx_n_s_x_b, __pyx_n_s_y_a, __pyx_n_s_y_b, __pyx_n_s_slope, __pyx_n_s_w, __pyx_n_s_max_slopes, __pyx_n_s_threshold_slope_idx, __pyx_n_s_threshold_slope, __pyx_n_s_weight_func, __pyx_n_s_add_edge, __pyx_n_s_add_edge, __pyx_n_s_tol, __pyx_n_s_j); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(28, __pyx_n_s_ts, __pyx_n_s_xs, __pyx_n_s_directed, __pyx_n_s_weighted, __pyx_n_s_only_degrees, __pyx_n_s_min_weight, __pyx_n_s_max_weight, __pyx_n_s_penetrable_limit, __pyx_n_s_n, __pyx_n_s_edges, __pyx_n_s_degrees_in, __pyx_n_s_degrees_out, __pyx_n_s_i_a, __pyx_n_s_i_b, __pyx_n_s_x_a, __pyx_n_s_x_b, __pyx_n_s_y_a, __pyx_n_s_y_b, __pyx_n_s_slope, __pyx_n_s_w, __pyx_n_s_max_slopes, __pyx_n_s_threshold_slope_idx, __pyx_n_s_threshold_slope, __pyx_n_s_weight_func, __pyx_n_s_add_edge, __pyx_n_s_add_edge, __pyx_n_s_tol, __pyx_n_s_j); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(8, 0, 30, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ts2vg_graph__natural_penetrable, __pyx_n_s_compute_graph, 23, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(8, 0, 28, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ts2vg_graph__natural_penetrable, __pyx_n_s_compute_graph, 23, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 23, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
@@ -19670,52 +19672,67 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -21648,28 +21665,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -22854,44 +22871,62 @@
     return ret;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `ts2vg-1.2.1/ts2vg/graph/base.py` & `ts2vg-1.2.2/ts2vg/graph/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,15 +399,15 @@
         The ``snap`` package is required.
         """
         self._validate_is_built()
 
         from snap import TUNGraph, TNGraph
 
         if self.is_weighted:
-            raise ValueError("SNAP weighted graphs not currently supported.")
+            raise NotImplementedError("SNAP weighted graphs not currently supported.")
 
         if self.is_directed:
             g = TNGraph.New(self.n_vertices, self.n_edges)
         else:
             g = TUNGraph.New(self.n_vertices, self.n_edges)
 
         for i in range(self.n_vertices):
```

### Comparing `ts2vg-1.2.1/ts2vg/graph/horizontal.py` & `ts2vg-1.2.2/ts2vg/graph/horizontal.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 from ts2vg.graph.base import VG
 
 
 class HorizontalVG(VG):
     r"""
     Horizontal Visibility Graph.
 
-    Transform a time series to a Horizontal Visibility Graph.
+    Used to transform a time series to a Horizontal Visibility Graph.
 
     Parameters
     ----------
     directed : str, None
         If ``None`` make an undirected graph, otherwise, a directed graph by using one of the following values:
-        ``left_to_right``, ``top_to_bottom``.
+        ``'left_to_right'``, ``'top_to_bottom'``.
         See :ref:`Directed graphs` for more information.
         Default ``None``.
 
     weighted : str, None
         If ``None`` make an unweighted graph, otherwise, a weighted graph by using one of the following values:
-        ``distance``, ``sq_distance``, ``v_distance``, ``abs_v_distance``, ``h_distance``, ``abs_h_distance``,
-        ``slope``, ``abs_slope``, ``angle``, ``abs_angle``.
+        ``'distance'``, ``'sq_distance'``, ``'v_distance'``, ``'abs_v_distance'``, ``'h_distance'``, ``'abs_h_distance'``,
+        ``'slope'``, ``'abs_slope'``, ``'angle'``, ``'abs_angle'``, ``'num_penetrations'``.
         See :ref:`Weighted graphs` for more information.
         Default ``None``.
 
     min_weight : float, None
         If provided, only edges with a weight higher than ``min_weight`` (non inclusive) will be included in the final graph.
         The graph must be weighted and the values used for weight will depend on the ``weighted`` parameter.
         This acts as a generalization of parametric visibility graphs.
```

### Comparing `ts2vg-1.2.1/ts2vg/graph/natural.py` & `ts2vg-1.2.2/ts2vg/graph/natural.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 from ts2vg.graph.base import VG
 
 
 class NaturalVG(VG):
     r"""
     Natural Visibility Graph.
 
-    Transform a time series to a Natural Visibility Graph.
+    Used to transform a time series to a Natural Visibility Graph.
 
     Parameters
     ----------
     directed : str, None
         If ``None`` make an undirected graph, otherwise, a directed graph by using one of the following values:
-        ``left_to_right``, ``top_to_bottom``.
+        ``'left_to_right'``, ``'top_to_bottom'``.
         See :ref:`Directed graphs` for more information.
         Default ``None``.
 
     weighted : str, None
         If ``None`` make an unweighted graph, otherwise, a weighted graph by using one of the following values:
-        ``distance``, ``sq_distance``, ``v_distance``, ``abs_v_distance``, ``h_distance``, ``abs_h_distance``,
-        ``slope``, ``abs_slope``, ``angle``, ``abs_angle``.
+        ``'distance'``, ``'sq_distance'``, ``'v_distance'``, ``'abs_v_distance'``, ``'h_distance'``, ``'abs_h_distance'``,
+        ``'slope'``, ``'abs_slope'``, ``'angle'``, ``'abs_angle'``, ``'num_penetrations'``.
         See :ref:`Weighted graphs` for more information.
         Default ``None``.
 
     min_weight : float, None
         If provided, only edges with a weight higher than ``min_weight`` (non inclusive) will be included in the final graph.
         The graph must be weighted and the values used for weight will depend on the ``weighted`` parameter.
         This acts as a generalization of parametric visibility graphs.
```

### Comparing `ts2vg-1.2.1/ts2vg/graph/summary.py` & `ts2vg-1.2.2/ts2vg/graph/summary.py`

 * *Files identical despite different names*

### Comparing `ts2vg-1.2.1/ts2vg.egg-info/PKG-INFO` & `ts2vg-1.2.2/ts2vg.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts2vg
-Version: 1.2.1
+Version: 1.2.2
 Summary: Build visibility graphs from time series data.
 Home-page: https://github.com/CarlosBergillos/ts2vg
 Author: Carlos Bergillos
 Author-email: c.bergillos.v@gmail.com
 License: MIT
 Project-URL: Documentation, https://carlosbergillos.github.io/ts2vg
 Project-URL: Source Code, https://github.com/CarlosBergillos/ts2vg
@@ -59,30 +59,22 @@
    :target: https://pypi.python.org/pypi/ts2vg
 
 |cover|
 
 |
 
 The Python |ts2vg| package provides high-performance algorithm
-implementations to build visibility graphs from time series data.
+implementations to build visibility graphs from time series data,
+as first introduced by Lucas Lacasa et al. in 2008 [#Lacasa2008]_.
 
 The visibility graphs and some of their properties (e.g. degree
 distributions) are computed quickly and efficiently even for time
 series with millions of observations.
-
-The visibility graphs are provided according to the
-mathematical definitions presented in:
-
--  Lucas Lacasa et al., "*From time series to complex networks: The visibility graph*", 2008.
--  Lucas Lacasa et al., "*Horizontal visibility graphs: exact results for random time series*", 2009.
-
-An efficient divide-and-conquer algorithm is used to compute the graphs,
-as described in:
-
--  Xin Lan et al., "*Fast transformation from time series to visibility graphs*", 2015.
+An efficient divide-and-conquer algorithm is used to compute the graphs
+whenever possible [#Lan2015]_.
 
    
 Installation
 ------------
 
 The latest released |ts2vg| version is available at the `Python Package Index (PyPI)`_
 and can be easily installed by running:
@@ -96,24 +88,24 @@
 
 Supported graph types
 ---------------------
 
 Root graph types
 ~~~~~~~~~~~~~~~~
 
-- Natural Visibility Graphs (NVG) (``ts2vg.NaturalVG``)
-- Horizontal Visibility Graphs (HVG) (``ts2vg.HorizontalVG``)
+- Natural Visibility Graphs (NVG) [#Lacasa2008]_ (``ts2vg.NaturalVG``)
+- Horizontal Visibility Graphs (HVG) [#Lacasa2009]_ (``ts2vg.HorizontalVG``)
 
 Available variations
 ~~~~~~~~~~~~~~~~~~~~
 
 - Weighted Visibility Graphs (via the ``weighted`` parameter)
 - Directed Visibility Graphs (via the ``directed`` parameter)
-- Parametric Visibility Graphs (via the ``min_weight`` and ``max_weight`` parameters)
-- Limited Penetrable Visibility Graphs (LPVG) (via the ``penetrable_limit`` parameter)
+- Parametric Visibility Graphs [#Bezsudnov2014]_ (via the ``min_weight`` and ``max_weight`` parameters)
+- Limited Penetrable Visibility Graphs (LPVG) [#Zhou2012]_ [#Xuan2021]_ (via the ``penetrable_limit`` parameter)
 
 .. - Dual Perspective Visibility Graph [*planned, not implemented yet*]
 
 Note that multiple graph variations can be combined and used simultaneously.
 
 
 Documentation
@@ -121,96 +113,81 @@
 
 Usage and reference documentation for |ts2vg| can be found at `carlosbergillos.github.io/ts2vg`_.
 
 
 Basic usage
 -----------
 
-Visibility graph
-~~~~~~~~~~~~~~~~
-
-To build a visibility graph:
+To build a visibility graph from a time series do:
 
 .. code:: python
 
    from ts2vg import NaturalVG
 
    ts = [1.0, 0.5, 0.3, 0.7, 1.0, 0.5, 0.3, 0.8]
 
-   g = NaturalVG()
-   g.build(ts)
+   vg = NaturalVG()
+   vg.build(ts)
+
+   edges = vg.edges
 
-   edges = g.edges
 
 The time series passed (``ts``) can be any one-dimensional iterable, such as a list or a ``numpy`` 1D array.
 
 By default, the input observations are assumed to be equally spaced in time.
 Alternatively, a second 1D iterable (``xs``) can be provided for unevenly spaced time series.
 
 
-Horizontal visibility graph
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
 Horizontal visibility graphs can be obtained in a very similar way:
 
 .. code:: python
 
    from ts2vg import HorizontalVG
 
    ts = [1.0, 0.5, 0.3, 0.7, 1.0, 0.5, 0.3, 0.8]
 
-   g = HorizontalVG()
-   g.build(ts)
-
-   edges = g.edges
+   vg = HorizontalVG()
+   vg.build(ts)
 
+   edges = vg.edges
 
-Degree distribution
-~~~~~~~~~~~~~~~~~~~
 
 If we are only interested in the degree distribution of the visibility graph
 we can pass ``only_degrees=True`` to the ``build`` method.
 This will be more efficient in time and memory than storing the whole graph.
 
 .. code:: python
 
-   g = NaturalVG()
-   g.build(ts, only_degrees=True)
+   vg = NaturalVG()
+   vg.build(ts, only_degrees=True)
 
-   ks, ps = g.degree_distribution
+   ks, ps = vg.degree_distribution
 
 
-Directed visibility graph
-~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Directed graphs can be obtained by using the ``directed`` parameter.
-See the reference documentation for the different available options.
+Directed graphs can be obtained by using the ``directed`` parameter
+and weighted graphs can be obtained by using the ``weighted`` parameter:
 
 .. code:: python
 
-   g = NaturalVG(directed='left_to_right')
-   g.build(ts)
-
+   vg1 = NaturalVG(directed="left_to_right")
+   vg1.build(ts)
 
-Weighted visibility graph
-~~~~~~~~~~~~~~~~~~~~~~~~~
+   vg2 = NaturalVG(weighted="distance")
+   vg2.build(ts)
 
-Weighted graphs can be obtained by using the ``weighted`` parameter.
-See the reference documentation for the different available options.
-
-.. code:: python
+   vg3 = NaturalVG(directed="left_to_right", weighted="distance")
+   vg3.build(ts)
 
-   g = NaturalVG(weighted='distance')
-   g.build(ts)
+   vg4 = HorizontalVG(directed="left_to_right", weighted="h_distance")
+   vg4.build(ts)
 
-|
 
 .. **For more information and options see:** :ref:`Examples` and :ref:`API Reference`.
 
-**For more information and options see:** `Examples`_ and `API Reference`_.
+For more information and options see: `Examples`_ and `API Reference`_.
 
 
 Interoperability with other libraries
 -------------------------------------
 
 The graphs obtained can be easily converted to graph objects
 from other common Python graph libraries such as `igraph`_, `NetworkX`_ and `SNAP`_
@@ -226,18 +203,18 @@
 -  ``as_networkx()``
 -  ``as_snap()``
 
 For example:
 
 .. code:: python
 
-   g = NaturalVG()
-   g.build(ts)
+   vg = NaturalVG()
+   vg.build(ts)
    
-   nx_g = g.as_networkx()
+   g = vg.as_networkx()
 
 
 Command line interface
 ----------------------
 
 |ts2vg| can also be used as a command line program directly from the console:
 
@@ -269,7 +246,18 @@
 .. _Python Package Index (PyPI): https://pypi.org/project/ts2vg
 .. _igraph: https://igraph.org/python/
 .. _NetworkX: https://networkx.github.io/
 .. _SNAP: https://snap.stanford.edu/snappy/
 .. _on GitHub: https://github.com/CarlosBergillos/ts2vg
 .. _MIT License: https://github.com/CarlosBergillos/ts2vg/blob/main/LICENSE
 .. _carlosbergillos.github.io/ts2vg: https://carlosbergillos.github.io/ts2vg/
+
+
+References
+----------
+
+.. [#Lacasa2008] Lucas Lacasa et al., "*From time series to complex networks: The visibility graph*", 2008.
+.. [#Lacasa2009] Lucas Lacasa et al., "*Horizontal visibility graphs: exact results for random time series*", 2009.
+.. [#Lan2015] Xin Lan et al., "*Fast transformation from time series to visibility graphs*", 2015.
+.. [#Zhou2012] T.T Zhou et al., "*Limited penetrable visibility graph for establishing complex network from time series*", 2012.
+.. [#Bezsudnov2014] I.V. Bezsudnov et al., "*From the time series to the complex networks: The parametric natural visibility graph*", 2014
+.. [#Xuan2021] Qi Xuan et al., "*CLPVG: Circular limited penetrable visibility graph as a new network model for time series*", 2021
```

### Comparing `ts2vg-1.2.1/ts2vg.egg-info/SOURCES.txt` & `ts2vg-1.2.2/ts2vg.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 ts2vg.egg-info/dependency_links.txt
 ts2vg.egg-info/entry_points.txt
 ts2vg.egg-info/not-zip-safe
 ts2vg.egg-info/requires.txt
 ts2vg.egg-info/top_level.txt
 ts2vg/graph/__init__.py
 ts2vg/graph/_base.c
-ts2vg/graph/_horizontal.c
+ts2vg/graph/_horizontal.cpp
 ts2vg/graph/_horizontal_penetrable.c
-ts2vg/graph/_natural.c
+ts2vg/graph/_natural.cpp
 ts2vg/graph/_natural_penetrable.c
 ts2vg/graph/base.py
 ts2vg/graph/horizontal.py
 ts2vg/graph/natural.py
-ts2vg/graph/summary.py
-ts2vg/utils/__init__.py
-ts2vg/utils/pairqueue.c
+ts2vg/graph/summary.py
```


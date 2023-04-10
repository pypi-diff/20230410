# Comparing `tmp/sphoin-2.0.8.tar.gz` & `tmp/sphoin-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/desac/Documents/my-python-packages/sphoin/dist/.tmp-0hlpb7hc/sphoin-2.0.8.tar", last modified: Wed Apr  5 09:43:47 2023, max compression
+gzip compressed data, was "/Users/desac/Documents/my-python-packages/sphoin/dist/.tmp-ju7hbpak/sphoin-2.0.9.tar", last modified: Mon Apr 10 07:51:42 2023, max compression
```

## Comparing `sphoin-2.0.8.tar` & `sphoin-2.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-05 09:43:47.000000 sphoin-2.0.8/
--rw-r--r--   0 desac      (501) staff       (20)     1093 2023-03-20 18:40:36.000000 sphoin-2.0.8/LICENSE
--rw-r--r--   0 desac      (501) staff       (20)       53 2022-11-24 19:48:58.000000 sphoin-2.0.8/MANIFEST.in
--rw-r--r--   0 desac      (501) staff       (20)     3746 2023-04-05 09:43:47.000000 sphoin-2.0.8/PKG-INFO
--rw-r--r--   0 desac      (501) staff       (20)     2943 2023-04-05 08:40:24.000000 sphoin-2.0.8/README.md
--rw-r--r--   0 desac      (501) staff       (20)      138 2023-04-05 08:41:06.000000 sphoin-2.0.8/config.yaml
--rw-r--r--   0 desac      (501) staff       (20)       38 2023-04-05 09:43:47.000000 sphoin-2.0.8/setup.cfg
--rw-r--r--   0 desac      (501) staff       (20)     1565 2023-04-05 09:43:10.000000 sphoin-2.0.8/setup.py
-drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-05 09:43:47.000000 sphoin-2.0.8/sphoin/
--rw-r--r--   0 desac      (501) staff       (20)      226 2023-04-05 09:43:09.000000 sphoin-2.0.8/sphoin/__init__.py
--rw-r--r--   0 desac      (501) staff       (20)     6992 2023-04-05 09:43:09.000000 sphoin-2.0.8/sphoin/app.py
--rw-r--r--   0 desac      (501) staff       (20)     2629 2023-04-05 09:43:08.000000 sphoin-2.0.8/sphoin/cli.py
-drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-05 09:43:47.000000 sphoin-2.0.8/sphoin/models/
--rw-r--r--   0 desac      (501) staff       (20)     1148 2023-04-05 09:43:08.000000 sphoin-2.0.8/sphoin/models/__init__.py
--rw-r--r--   0 desac      (501) staff       (20)     2693 2023-03-24 21:51:25.000000 sphoin-2.0.8/sphoin/models/_indicator.py
--rw-r--r--   0 desac      (501) staff       (20)      546 2023-03-24 21:51:28.000000 sphoin-2.0.8/sphoin/models/_ohlcv.py
--rw-r--r--   0 desac      (501) staff       (20)     1716 2023-03-31 11:05:42.000000 sphoin-2.0.8/sphoin/models/_study.py
-drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-05 09:43:47.000000 sphoin-2.0.8/sphoin/plot/
--rw-r--r--   0 desac      (501) staff       (20)     2696 2023-04-05 09:43:06.000000 sphoin-2.0.8/sphoin/plot/__init__.py
--rw-r--r--   0 desac      (501) staff       (20)    17078 2023-04-04 17:12:59.000000 sphoin-2.0.8/sphoin/plot/_plot.py
-drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-05 09:43:47.000000 sphoin-2.0.8/sphoin/tui/
--rw-r--r--   0 desac      (501) staff       (20)     4052 2023-04-05 09:43:05.000000 sphoin-2.0.8/sphoin/tui/__init__.py
-drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-05 09:43:47.000000 sphoin-2.0.8/sphoin/tui/widgets/
--rw-r--r--   0 desac      (501) staff       (20)      783 2023-04-05 09:43:04.000000 sphoin-2.0.8/sphoin/tui/widgets/__init__.py
--rw-r--r--   0 desac      (501) staff       (20)     3853 2023-04-03 18:15:59.000000 sphoin-2.0.8/sphoin/tui/widgets/_footer.py
--rw-r--r--   0 desac      (501) staff       (20)     3429 2023-03-31 08:29:54.000000 sphoin-2.0.8/sphoin/tui/widgets/_graph.py
--rw-r--r--   0 desac      (501) staff       (20)     2965 2023-04-05 08:41:04.000000 sphoin-2.0.8/sphoin/tui/widgets/_help.py
--rw-r--r--   0 desac      (501) staff       (20)     1312 2023-03-30 18:53:28.000000 sphoin-2.0.8/sphoin/tui/widgets/_time.py
-drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-05 09:43:47.000000 sphoin-2.0.8/sphoin/utils/
--rw-r--r--   0 desac      (501) staff       (20)     2710 2023-03-30 19:19:01.000000 sphoin-2.0.8/sphoin/utils/__init__.py
-drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-05 09:43:47.000000 sphoin-2.0.8/sphoin.egg-info/
--rw-r--r--   0 desac      (501) staff       (20)     3746 2023-04-05 09:43:47.000000 sphoin-2.0.8/sphoin.egg-info/PKG-INFO
--rw-r--r--   0 desac      (501) staff       (20)      645 2023-04-05 09:43:47.000000 sphoin-2.0.8/sphoin.egg-info/SOURCES.txt
--rw-r--r--   0 desac      (501) staff       (20)        1 2023-04-05 09:43:47.000000 sphoin-2.0.8/sphoin.egg-info/dependency_links.txt
--rw-r--r--   0 desac      (501) staff       (20)       74 2023-04-05 09:43:47.000000 sphoin-2.0.8/sphoin.egg-info/entry_points.txt
--rw-r--r--   0 desac      (501) staff       (20)      102 2023-04-05 09:43:47.000000 sphoin-2.0.8/sphoin.egg-info/requires.txt
--rw-r--r--   0 desac      (501) staff       (20)        7 2023-04-05 09:43:47.000000 sphoin-2.0.8/sphoin.egg-info/top_level.txt
--rw-r--r--   0 desac      (501) staff       (20)        1 2020-06-05 22:31:20.000000 sphoin-2.0.8/sphoin.egg-info/zip-safe
+drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-10 07:51:42.000000 sphoin-2.0.9/
+-rw-r--r--   0 desac      (501) staff       (20)     1093 2023-03-20 18:40:36.000000 sphoin-2.0.9/LICENSE
+-rw-r--r--   0 desac      (501) staff       (20)       53 2022-11-24 19:48:58.000000 sphoin-2.0.9/MANIFEST.in
+-rw-r--r--   0 desac      (501) staff       (20)     3823 2023-04-10 07:51:42.000000 sphoin-2.0.9/PKG-INFO
+-rw-r--r--   0 desac      (501) staff       (20)     3020 2023-04-05 13:27:35.000000 sphoin-2.0.9/README.md
+-rw-r--r--   0 desac      (501) staff       (20)      138 2023-04-05 08:41:06.000000 sphoin-2.0.9/config.yaml
+-rw-r--r--   0 desac      (501) staff       (20)       38 2023-04-10 07:51:42.000000 sphoin-2.0.9/setup.cfg
+-rw-r--r--   0 desac      (501) staff       (20)     1565 2023-04-10 07:50:40.000000 sphoin-2.0.9/setup.py
+drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-10 07:51:42.000000 sphoin-2.0.9/sphoin/
+-rw-r--r--   0 desac      (501) staff       (20)      226 2023-04-10 07:50:39.000000 sphoin-2.0.9/sphoin/__init__.py
+-rw-r--r--   0 desac      (501) staff       (20)     6992 2023-04-10 07:50:38.000000 sphoin-2.0.9/sphoin/app.py
+-rw-r--r--   0 desac      (501) staff       (20)     2629 2023-04-10 07:50:38.000000 sphoin-2.0.9/sphoin/cli.py
+drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-10 07:51:42.000000 sphoin-2.0.9/sphoin/models/
+-rw-r--r--   0 desac      (501) staff       (20)     1148 2023-04-10 07:50:36.000000 sphoin-2.0.9/sphoin/models/__init__.py
+-rw-r--r--   0 desac      (501) staff       (20)     2693 2023-03-24 21:51:25.000000 sphoin-2.0.9/sphoin/models/_indicator.py
+-rw-r--r--   0 desac      (501) staff       (20)      546 2023-03-24 21:51:28.000000 sphoin-2.0.9/sphoin/models/_ohlcv.py
+-rw-r--r--   0 desac      (501) staff       (20)     1716 2023-03-31 11:05:42.000000 sphoin-2.0.9/sphoin/models/_study.py
+drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-10 07:51:42.000000 sphoin-2.0.9/sphoin/plot/
+-rw-r--r--   0 desac      (501) staff       (20)     2696 2023-04-10 07:50:34.000000 sphoin-2.0.9/sphoin/plot/__init__.py
+-rw-r--r--   0 desac      (501) staff       (20)    17082 2023-04-10 07:48:44.000000 sphoin-2.0.9/sphoin/plot/_plot.py
+drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-10 07:51:42.000000 sphoin-2.0.9/sphoin/tui/
+-rw-r--r--   0 desac      (501) staff       (20)     4052 2023-04-10 07:50:33.000000 sphoin-2.0.9/sphoin/tui/__init__.py
+drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-10 07:51:42.000000 sphoin-2.0.9/sphoin/tui/widgets/
+-rw-r--r--   0 desac      (501) staff       (20)      783 2023-04-10 07:50:32.000000 sphoin-2.0.9/sphoin/tui/widgets/__init__.py
+-rw-r--r--   0 desac      (501) staff       (20)     3853 2023-04-03 18:15:59.000000 sphoin-2.0.9/sphoin/tui/widgets/_footer.py
+-rw-r--r--   0 desac      (501) staff       (20)     3429 2023-03-31 08:29:54.000000 sphoin-2.0.9/sphoin/tui/widgets/_graph.py
+-rw-r--r--   0 desac      (501) staff       (20)     2965 2023-04-05 08:41:04.000000 sphoin-2.0.9/sphoin/tui/widgets/_help.py
+-rw-r--r--   0 desac      (501) staff       (20)     1312 2023-03-30 18:53:28.000000 sphoin-2.0.9/sphoin/tui/widgets/_time.py
+drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-10 07:51:42.000000 sphoin-2.0.9/sphoin/utils/
+-rw-r--r--   0 desac      (501) staff       (20)     2710 2023-03-30 19:19:01.000000 sphoin-2.0.9/sphoin/utils/__init__.py
+drwxr-xr-x   0 desac      (501) staff       (20)        0 2023-04-10 07:51:42.000000 sphoin-2.0.9/sphoin.egg-info/
+-rw-r--r--   0 desac      (501) staff       (20)     3823 2023-04-10 07:51:42.000000 sphoin-2.0.9/sphoin.egg-info/PKG-INFO
+-rw-r--r--   0 desac      (501) staff       (20)      645 2023-04-10 07:51:42.000000 sphoin-2.0.9/sphoin.egg-info/SOURCES.txt
+-rw-r--r--   0 desac      (501) staff       (20)        1 2023-04-10 07:51:42.000000 sphoin-2.0.9/sphoin.egg-info/dependency_links.txt
+-rw-r--r--   0 desac      (501) staff       (20)       74 2023-04-10 07:51:42.000000 sphoin-2.0.9/sphoin.egg-info/entry_points.txt
+-rw-r--r--   0 desac      (501) staff       (20)      102 2023-04-10 07:51:42.000000 sphoin-2.0.9/sphoin.egg-info/requires.txt
+-rw-r--r--   0 desac      (501) staff       (20)        7 2023-04-10 07:51:42.000000 sphoin-2.0.9/sphoin.egg-info/top_level.txt
+-rw-r--r--   0 desac      (501) staff       (20)        1 2020-06-05 22:31:20.000000 sphoin-2.0.9/sphoin.egg-info/zip-safe
```

### Comparing `sphoin-2.0.8/LICENSE` & `sphoin-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sphoin-2.0.8/PKG-INFO` & `sphoin-2.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphoin
-Version: 2.0.8
+Version: 2.0.9
 Summary: Connect to sphoin.app Pro Slots
 Home-page: https://github.com/Parsecom/sphoin
 Author: P.O.M.
 Author-email: office@parsecom.ro
 License: MIT license
 Keywords: sphoin
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,17 +21,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 
 # <img  src="https://api.sphoin.app/logo"  alt="drawing"  width="100"/>
 
-<img  src="https://img.shields.io/pypi/v/sphoin.svg"/><img  src="https://img.shields.io/pypi/pyversions/sphoin.svg"/> 
-
-
+[![PyPI](https://img.shields.io/pypi/v/sphoin.svg)](https://pypi.org/project/sphoin/) [![PyPI](https://img.shields.io/pypi/pyversions/sphoin.svg)](https://img.shields.io/pypi/pyversions/sphoin.svg)
 
 Connect to [sphoin.app](https://www.sphoin.app) Pro Slots.
 
 <img  src="https://firebasestorage.googleapis.com/v0/b/sphoin-545ba.appspot.com/o/tui.png?alt=media&token=99083efe-74eb-4418-b7f9-abdca46d573f"  alt="drawing" width="100%" />
 
 # Installation
```

### Comparing `sphoin-2.0.8/README.md` & `sphoin-2.0.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 
 
 # <img  src="https://api.sphoin.app/logo"  alt="drawing"  width="100"/>
 
-<img  src="https://img.shields.io/pypi/v/sphoin.svg"/><img  src="https://img.shields.io/pypi/pyversions/sphoin.svg"/> 
-
-
+[![PyPI](https://img.shields.io/pypi/v/sphoin.svg)](https://pypi.org/project/sphoin/) [![PyPI](https://img.shields.io/pypi/pyversions/sphoin.svg)](https://img.shields.io/pypi/pyversions/sphoin.svg)
 
 Connect to [sphoin.app](https://www.sphoin.app) Pro Slots.
 
 <img  src="https://firebasestorage.googleapis.com/v0/b/sphoin-545ba.appspot.com/o/tui.png?alt=media&token=99083efe-74eb-4418-b7f9-abdca46d573f"  alt="drawing" width="100%" />
 
 # Installation
```

### Comparing `sphoin-2.0.8/setup.py` & `sphoin-2.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 __author__ = "pom11"
 __copyright__ = "Copyright 2023, Parsec Original Mastercraft S.R.L."
 __license__ = "MIT"
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 __maintainer__ = "pom11"
 __email__ = "office@parsecom.ro"
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
@@ -48,10 +48,10 @@
 	long_description_content_type="text/markdown",
 	include_package_data=True,
 	keywords='sphoin',
 	name='sphoin',
 	packages=find_packages(include=['sphoin', 'sphoin.*']),
 	setup_requires=setup_requirements,
 	url='https://github.com/Parsecom/sphoin',
-	version='2.0.8',
+	version='2.0.9',
 	zip_safe=True,
 )
```

### Comparing `sphoin-2.0.8/sphoin/app.py` & `sphoin-2.0.9/sphoin/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Main module."""
 
 __author__ = "pom11"
 __copyright__ = "Copyright 2023, Parsec Original Mastercraft S.R.L."
 __license__ = "MIT"
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 __maintainer__ = "pom11"
 __email__ = "office@parsecom.ro"
 
 import requests
 import json
 import yaml
 import time
```

### Comparing `sphoin-2.0.8/sphoin/cli.py` & `sphoin-2.0.9/sphoin/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Console script for sphoin."""
 
 __author__ = "pom11"
 __copyright__ = "Copyright 2023, Parsec Original Mastercraft S.R.L."
 __license__ = "MIT"
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 __maintainer__ = "pom11"
 __email__ = "office@parsecom.ro"
 
 import argparse
 import sys
 from .app import Slot
 from .plot import test
```

### Comparing `sphoin-2.0.8/sphoin/models/__init__.py` & `sphoin-2.0.9/sphoin/models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Models module."""
 
 __author__ = "pom11"
 __copyright__ = "Copyright 2023, Parsec Original Mastercraft S.R.L."
 __license__ = "MIT"
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 __maintainer__ = "pom11"
 __email__ = "office@parsecom.ro"
 
 import typing
 from importlib import import_module
 
 if typing.TYPE_CHECKING:
```

### Comparing `sphoin-2.0.8/sphoin/models/_indicator.py` & `sphoin-2.0.9/sphoin/models/_indicator.py`

 * *Files identical despite different names*

### Comparing `sphoin-2.0.8/sphoin/models/_ohlcv.py` & `sphoin-2.0.9/sphoin/models/_ohlcv.py`

 * *Files identical despite different names*

### Comparing `sphoin-2.0.8/sphoin/models/_study.py` & `sphoin-2.0.9/sphoin/models/_study.py`

 * *Files identical despite different names*

### Comparing `sphoin-2.0.8/sphoin/plot/__init__.py` & `sphoin-2.0.9/sphoin/plot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Plot module."""
 
 __author__ = "pom11"
 __copyright__ = "Copyright 2023, Parsec Original Mastercraft S.R.L."
 __license__ = "MIT"
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 __maintainer__ = "pom11"
 __email__ = "office@parsecom.ro"
 
 import typing
 from importlib import import_module
 from rich.text import Text
```

### Comparing `sphoin-2.0.8/sphoin/plot/_plot.py` & `sphoin-2.0.9/sphoin/plot/_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 		max_flag: int = 0,
 		color1: str = 'magenta', 
 		color2: str = 'cyan',
 		sizeY: int = 200, 
 		sizeX: int = 50,
 		signal_as_line: bool = False,
 		dark_theme: bool = True,
-		brightness: bool = True,
+		brightness: bool = False,
 		as_ansi: bool = False) -> str:
 		"""
 Generate an ascii chart for a series
 
 Parameters
 ----------
 series : list
@@ -336,15 +336,15 @@
 
 	def study_bar(
 		study: Study,
 		color1: str = 'magenta', 
 		color2: str = 'cyan', 
 		sizeX: int = 50,
 		dark_theme: bool = True,
-		brightness: bool = True,
+		brightness: bool = False,
 		as_ansi: bool = False) -> Text:
 		"""
 Generate an ascii bar chart for Sphoin Slot Study
 
 Parameters
 ----------
 study : Study
@@ -366,15 +366,15 @@
 	Contraints
 		min : 50
 		max : 500
 dark_theme : bool
 	Theme of chart plot
 	Default : True
 brightness : bool
-	Default : True
+	Default : False
 as_ansi : bool
 	Default : False
 Returns
 ------
 rich Text
 	Ansi chart
 		"""
@@ -409,15 +409,15 @@
 			ret = capture.get()
 		return ret
 
 	def time_bar(
 		slot: Slot, 
 		sizeX: int = 50,
 		dark_theme: bool = True,
-		brightness: bool = True,
+		brightness: bool = False,
 		as_ansi: bool = False) -> str:
 		"""
 Generate an ascii time bar for a Sphoin Slot
 
 Parameters
 ----------
 slot : Slot
```

### Comparing `sphoin-2.0.8/sphoin/tui/__init__.py` & `sphoin-2.0.9/sphoin/tui/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "pom11"
 __copyright__ = "Copyright 2023, Parsec Original Mastercraft S.R.L."
 __license__ = "MIT"
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 __maintainer__ = "pom11"
 __email__ = "office@parsecom.ro"
 
 from textual.app import App, ComposeResult
 from textual.containers import Container, Vertical
 from textual.widgets import Static
 from rich.color import Color
```

### Comparing `sphoin-2.0.8/sphoin/tui/widgets/__init__.py` & `sphoin-2.0.9/sphoin/tui/widgets/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "pom11"
 __copyright__ = "Copyright 2023, Parsec Original Mastercraft S.R.L."
 __license__ = "MIT"
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 __maintainer__ = "pom11"
 __email__ = "office@parsecom.ro"
 
 import typing
 from importlib import import_module
 
 if typing.TYPE_CHECKING:
```

### Comparing `sphoin-2.0.8/sphoin/tui/widgets/_footer.py` & `sphoin-2.0.9/sphoin/tui/widgets/_footer.py`

 * *Files identical despite different names*

### Comparing `sphoin-2.0.8/sphoin/tui/widgets/_graph.py` & `sphoin-2.0.9/sphoin/tui/widgets/_graph.py`

 * *Files identical despite different names*

### Comparing `sphoin-2.0.8/sphoin/tui/widgets/_help.py` & `sphoin-2.0.9/sphoin/tui/widgets/_help.py`

 * *Files identical despite different names*

### Comparing `sphoin-2.0.8/sphoin/tui/widgets/_time.py` & `sphoin-2.0.9/sphoin/tui/widgets/_time.py`

 * *Files identical despite different names*

### Comparing `sphoin-2.0.8/sphoin/utils/__init__.py` & `sphoin-2.0.9/sphoin/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sphoin-2.0.8/sphoin.egg-info/PKG-INFO` & `sphoin-2.0.9/sphoin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphoin
-Version: 2.0.8
+Version: 2.0.9
 Summary: Connect to sphoin.app Pro Slots
 Home-page: https://github.com/Parsecom/sphoin
 Author: P.O.M.
 Author-email: office@parsecom.ro
 License: MIT license
 Keywords: sphoin
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,17 +21,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 
 # <img  src="https://api.sphoin.app/logo"  alt="drawing"  width="100"/>
 
-<img  src="https://img.shields.io/pypi/v/sphoin.svg"/><img  src="https://img.shields.io/pypi/pyversions/sphoin.svg"/> 
-
-
+[![PyPI](https://img.shields.io/pypi/v/sphoin.svg)](https://pypi.org/project/sphoin/) [![PyPI](https://img.shields.io/pypi/pyversions/sphoin.svg)](https://img.shields.io/pypi/pyversions/sphoin.svg)
 
 Connect to [sphoin.app](https://www.sphoin.app) Pro Slots.
 
 <img  src="https://firebasestorage.googleapis.com/v0/b/sphoin-545ba.appspot.com/o/tui.png?alt=media&token=99083efe-74eb-4418-b7f9-abdca46d573f"  alt="drawing" width="100%" />
 
 # Installation
```

### Comparing `sphoin-2.0.8/sphoin.egg-info/SOURCES.txt` & `sphoin-2.0.9/sphoin.egg-info/SOURCES.txt`

 * *Files identical despite different names*


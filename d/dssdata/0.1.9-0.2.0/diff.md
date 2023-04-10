# Comparing `tmp/dssdata-0.1.9.tar.gz` & `tmp/dssdata-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dssdata-0.1.9.tar", max compression
+gzip compressed data, was "dssdata-0.2.0.tar", max compression
```

## Comparing `dssdata-0.1.9.tar` & `dssdata-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1091 2023-03-22 14:08:27.907392 dssdata-0.1.9/LICENSE
--rw-r--r--   0        0        0     2471 2023-03-22 14:08:27.907392 dssdata-0.1.9/README.md
--rw-r--r--   0        0        0     5628 2023-03-22 14:08:27.911392 dssdata-0.1.9/dssdata/__init__.py
--rw-r--r--   0        0        0     2468 2023-03-22 14:08:27.911392 dssdata-0.1.9/dssdata/_formatters.py
--rw-r--r--   0        0        0      852 2023-03-22 14:08:27.911392 dssdata-0.1.9/dssdata/_tools.py
--rw-r--r--   0        0        0     1188 2023-03-22 14:08:27.911392 dssdata-0.1.9/dssdata/decorators/__init__.py
--rw-r--r--   0        0        0     3030 2023-03-22 14:08:27.911392 dssdata-0.1.9/dssdata/pfmodes/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 14:08:27.911392 dssdata-0.1.9/dssdata/reductions/__init__.py
--rw-r--r--   0        0        0     1149 2023-03-22 14:08:27.911392 dssdata-0.1.9/dssdata/reductions/regs/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 14:08:27.911392 dssdata-0.1.9/dssdata/tools/__init__.py
--rw-r--r--   0        0        0     5388 2023-03-22 14:08:27.911392 dssdata-0.1.9/dssdata/tools/lines/__init__.py
--rw-r--r--   0        0        0     8636 2023-03-22 14:08:27.911392 dssdata-0.1.9/dssdata/tools/losses/__init__.py
--rw-r--r--   0        0        0     1136 2023-03-22 14:08:27.911392 dssdata-0.1.9/dssdata/tools/regs/__init__.py
--rw-r--r--   0        0        0     2541 2023-03-22 14:08:27.911392 dssdata-0.1.9/dssdata/tools/voltages/__init__.py
--rw-r--r--   0        0        0      880 2023-03-22 14:08:27.911392 dssdata-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 dssdata-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-10 12:46:13.902691 dssdata-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3835 2023-04-10 12:46:13.902691 dssdata-0.2.0/README.md
+-rw-r--r--   0        0        0     5626 2023-04-10 12:46:13.906691 dssdata-0.2.0/dssdata/__init__.py
+-rw-r--r--   0        0        0     2468 2023-04-10 12:46:13.906691 dssdata-0.2.0/dssdata/_formatters.py
+-rw-r--r--   0        0        0      852 2023-04-10 12:46:13.906691 dssdata-0.2.0/dssdata/_tools.py
+-rw-r--r--   0        0        0     1188 2023-04-10 12:46:13.906691 dssdata-0.2.0/dssdata/decorators/__init__.py
+-rw-r--r--   0        0        0     3030 2023-04-10 12:46:13.906691 dssdata-0.2.0/dssdata/pfmodes/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 12:46:13.906691 dssdata-0.2.0/dssdata/reductions/__init__.py
+-rw-r--r--   0        0        0     1149 2023-04-10 12:46:13.906691 dssdata-0.2.0/dssdata/reductions/regs/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 12:46:13.906691 dssdata-0.2.0/dssdata/tools/__init__.py
+-rw-r--r--   0        0        0     5388 2023-04-10 12:46:13.906691 dssdata-0.2.0/dssdata/tools/lines/__init__.py
+-rw-r--r--   0        0        0     8636 2023-04-10 12:46:13.906691 dssdata-0.2.0/dssdata/tools/losses/__init__.py
+-rw-r--r--   0        0        0     1136 2023-04-10 12:46:13.906691 dssdata-0.2.0/dssdata/tools/regs/__init__.py
+-rw-r--r--   0        0        0     2541 2023-04-10 12:46:13.906691 dssdata-0.2.0/dssdata/tools/voltages/__init__.py
+-rw-r--r--   0        0        0      880 2023-04-10 12:46:13.906691 dssdata-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4759 1970-01-01 00:00:00.000000 dssdata-0.2.0/PKG-INFO
```

### Comparing `dssdata-0.1.9/LICENSE` & `dssdata-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dssdata-0.1.9/dssdata/__init__.py` & `dssdata-0.2.0/dssdata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from os import getcwd, chdir
 from os import path as pathfunc
 from typing import Iterable, List
 
-__version__ = "0.1.8"
+__version__ = "0.2"
 
 
 def _redirect_handler(path) -> List[str]:
     """
     If a redirect command is found, call the function recursively
     Args:
         path: The path to the file.
```

### Comparing `dssdata-0.1.9/dssdata/_formatters.py` & `dssdata-0.2.0/dssdata/_formatters.py`

 * *Files identical despite different names*

### Comparing `dssdata-0.1.9/dssdata/_tools.py` & `dssdata-0.2.0/dssdata/_tools.py`

 * *Files identical despite different names*

### Comparing `dssdata-0.1.9/dssdata/decorators/__init__.py` & `dssdata-0.2.0/dssdata/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dssdata-0.1.9/dssdata/pfmodes/__init__.py` & `dssdata-0.2.0/dssdata/pfmodes/__init__.py`

 * *Files identical despite different names*

### Comparing `dssdata-0.1.9/dssdata/reductions/regs/__init__.py` & `dssdata-0.2.0/dssdata/reductions/regs/__init__.py`

 * *Files identical despite different names*

### Comparing `dssdata-0.1.9/dssdata/tools/lines/__init__.py` & `dssdata-0.2.0/dssdata/tools/lines/__init__.py`

 * *Files identical despite different names*

### Comparing `dssdata-0.1.9/dssdata/tools/losses/__init__.py` & `dssdata-0.2.0/dssdata/tools/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `dssdata-0.1.9/dssdata/tools/regs/__init__.py` & `dssdata-0.2.0/dssdata/tools/regs/__init__.py`

 * *Files identical despite different names*

### Comparing `dssdata-0.1.9/dssdata/tools/voltages/__init__.py` & `dssdata-0.2.0/dssdata/tools/voltages/__init__.py`

 * *Files identical despite different names*

### Comparing `dssdata-0.1.9/pyproject.toml` & `dssdata-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dssdata"
-version = "0.1.9"
+version = "0.2.0"
 description = "Organizing OpenDSS data"
 authors = ["Felipe M. S. Monteiro <fmarkson@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://felipemarkson.github.io/dssdata/"
 repository = "https://github.com/felipemarkson/dssdata"
 classifiers = [
@@ -12,15 +12,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Intended Audience :: Science/Research",
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
-"OpenDSSDirect.py" = "0.7.*"
+"OpenDSSDirect.py" = "0.8.*"
 pandas = "1.*"
 
 
 [tool.poetry.dev-dependencies]
 flake8 = "*"
 black = "*"
 matplotlib = "*"
```

### Comparing `dssdata-0.1.9/PKG-INFO` & `dssdata-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: dssdata
-Version: 0.1.9
+Version: 0.2.0
 Summary: Organizing OpenDSS data
 Home-page: https://github.com/felipemarkson/dssdata
 License: MIT
 Author: Felipe M. S. Monteiro
 Author-email: fmarkson@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: OpenDSSDirect.py (>=0.7.0,<0.8.0)
+Requires-Dist: OpenDSSDirect.py (>=0.8.0,<0.9.0)
 Requires-Dist: pandas (>=1.0.0,<2.0.0)
 Project-URL: Documentation, https://felipemarkson.github.io/dssdata/
 Project-URL: Repository, https://github.com/felipemarkson/dssdata
 Description-Content-Type: text/markdown
 
 # DSSData
 
@@ -45,34 +45,68 @@
 
 ### Easy to simulate
 
 We built the DSSData for you just write what you want in a simple function, plugin on a power flow mode, and run. 
 
 You don't need anymore write a routine to run each power flow per time. 
 
-## Documentation
-
-See [DSSData Documentation](https://felipemarkson.github.io/dssdata).
-
-## Installation
+## Quick Start
+### Installation
 
 We strongly recommend the use of virtual environments manager.
 
-### Using pip
-
 ```console
 pip install dssdata
 ```
 
-### Using poetry
+### Static Power Flow (Snapshot)
 
-```console
-poetry add dssdata
+First, comment any `solve`, output command (e.g: `show`), or solve configurations (e.g: `set mode=Snap`) from your `.dss` file.
+
+_**NOTE**: Any `Monitor` is needed to get the data._
+
+Supposing that you file is in the path `master.dss`:
+
+```python
+from dssdata import SystemClass
+from dssdata.pfmodes import run_static_pf
+from dssdata.tools import voltages
+
+distSys = SystemClass(path="master.dss", kV=[13.8, 0.230], loadmult=1.0)
+
+[voltageDataFrame] = run_static_pf(distSys, tools=[voltages.get_all])
+print(voltageDataFrame)
 ```
 
+### Time series Power Flow
+
+First, comment any `solve`, output command (e.g: `show`), or solve configurations (e.g: `set mode=daily stepsize=5m time=...`) from your `.dss` file.
+
+_**NOTE**: Any `Monitor` is needed to get the data._
+
+_**NOTE**: The `Loadshape` must be defined in the `.dss` file_
+
+Supposing that you file is in the path `master.dss`:
+
+```python
+from dssdata import SystemClass
+from dssdata.pfmodes import cfg_tspf, run_tspf
+from dssdata.tools import lines, voltages
+
+distSys = SystemClass(path="master.dss", kV=[13.8], loadmult=1.2)
+cfg_tspf(distSys, step_size="5m", initial_time=(0, 0))
+
+[voltageDataFrame] = run_tspf(distSys, tools=[voltages.get_all], num_steps=288)
+print(voltageDataFrame)
+```
+
+## Documentation
+
+We provide an full API documentation and examples in the [DSSData Documentation](https://felipemarkson.github.io/dssdata).
+
 ## Citing
 
 If you find DSSData useful in your work, we kindly request that you cite it as below: 
 ```bibtex
 @software{Monteiro_felipemarkson_dssdata_v0_1_7_2022,
   author = {Monteiro, Felipe},
   doi = {10.5281/zenodo.6784238},
@@ -83,14 +117,13 @@
   version = {0.1.7},
   year = {2022}
 }
 ```
 
 ## Help us to improve DSSData
 
-See our [Issue](https://github.com/felipemarkson/dssdata/issues) section!
-
+See our [Issue](https://github.com/felipemarkson/dssdata/issues) section, our [Development Guidelines](DEV.md), and our [Code of conduct](CODE_OF_CONDUCT.md).
 
-## Contributors: 
+### Contributors: 
 
 - [JonasVil](https://github.com/felipemarkson/power-flow-analysis/commits?author=JonasVil)
```


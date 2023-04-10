# Comparing `tmp/h5-0.8.7.tar.gz` & `tmp/h5-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5-0.8.7.tar", max compression
+gzip compressed data, was "h5-0.8.8.tar", max compression
```

## Comparing `h5-0.8.7.tar` & `h5-0.8.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2987 2023-04-05 20:11:35.022106 h5-0.8.7/h5/__init__.py
--rw-r--r--   0        0        0     1048 2023-04-05 20:11:35.022106 h5-0.8.7/h5/__main__.py
--rw-r--r--   0        0        0      184 2023-04-06 18:10:36.897192 h5-0.8.7/h5/_meta.py
--rw-r--r--   0        0        0    12195 2023-04-06 18:09:53.633081 h5-0.8.7/h5/cli.py
--rw-r--r--   0        0        0    15743 2023-04-05 20:11:35.022106 h5-0.8.7/h5/core.py
--rw-r--r--   0        0        0    14738 2023-04-05 20:11:35.022106 h5-0.8.7/h5/dev.py
--rw-r--r--   0        0        0     2935 2023-03-31 17:46:06.860725 h5-0.8.7/h5/legacy.py
--rw-r--r--   0        0        0        0 2022-02-01 22:06:04.805953 h5-0.8.7/h5/py.typed
--rw-r--r--   0        0        0     4457 2023-04-05 20:11:35.027132 h5-0.8.7/h5/testing.py
--rw-r--r--   0        0        0     1056 2022-02-17 22:17:07.419494 h5-0.8.7/LICENSE
--rw-r--r--   0        0        0     1890 2023-04-06 18:10:26.228534 h5-0.8.7/pyproject.toml
--rw-r--r--   0        0        0      739 2022-09-19 18:35:16.982212 h5-0.8.7/README.md
--rw-r--r--   0        0        0     1752 1970-01-01 00:00:00.000000 h5-0.8.7/setup.py
--rw-r--r--   0        0        0     2042 1970-01-01 00:00:00.000000 h5-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0     2987 2023-04-10 16:39:46.706848 h5-0.8.8/h5/__init__.py
+-rw-r--r--   0        0        0     1048 2023-04-10 16:39:46.707849 h5-0.8.8/h5/__main__.py
+-rw-r--r--   0        0        0      184 2023-04-10 16:41:57.348070 h5-0.8.8/h5/_meta.py
+-rw-r--r--   0        0        0    12195 2023-04-10 16:39:46.707849 h5-0.8.8/h5/cli.py
+-rw-r--r--   0        0        0    15743 2023-04-10 16:39:46.708848 h5-0.8.8/h5/core.py
+-rw-r--r--   0        0        0    14738 2023-04-10 16:39:46.708848 h5-0.8.8/h5/dev.py
+-rw-r--r--   0        0        0     2935 2023-03-31 17:44:54.413796 h5-0.8.8/h5/legacy.py
+-rw-r--r--   0        0        0        0 2022-02-01 20:37:20.150020 h5-0.8.8/h5/py.typed
+-rw-r--r--   0        0        0     4457 2023-04-10 16:39:46.708848 h5-0.8.8/h5/testing.py
+-rw-r--r--   0        0        0     1056 2022-02-11 23:27:58.156814 h5-0.8.8/LICENSE
+-rw-r--r--   0        0        0     1891 2023-04-10 16:45:29.557162 h5-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0      739 2022-12-12 16:24:11.593604 h5-0.8.8/README.md
+-rw-r--r--   0        0        0     1745 1970-01-01 00:00:00.000000 h5-0.8.8/setup.py
+-rw-r--r--   0        0        0     2035 1970-01-01 00:00:00.000000 h5-0.8.8/PKG-INFO
```

### Comparing `h5-0.8.7/h5/__init__.py` & `h5-0.8.8/h5/__init__.py`

 * *Files identical despite different names*

### Comparing `h5-0.8.7/h5/__main__.py` & `h5-0.8.8/h5/__main__.py`

 * *Files identical despite different names*

### Comparing `h5-0.8.7/h5/cli.py` & `h5-0.8.8/h5/cli.py`

 * *Files identical despite different names*

### Comparing `h5-0.8.7/h5/core.py` & `h5-0.8.8/h5/core.py`

 * *Files identical despite different names*

### Comparing `h5-0.8.7/h5/dev.py` & `h5-0.8.8/h5/dev.py`

 * *Files identical despite different names*

### Comparing `h5-0.8.7/h5/legacy.py` & `h5-0.8.8/h5/legacy.py`

 * *Files identical despite different names*

### Comparing `h5-0.8.7/h5/testing.py` & `h5-0.8.8/h5/testing.py`

 * *Files identical despite different names*

### Comparing `h5-0.8.7/LICENSE` & `h5-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `h5-0.8.7/pyproject.toml` & `h5-0.8.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "h5"
-version = "0.8.7"
+version = "0.8.8"
 description = "H5py utils"
 license = "MIT"
 authors = ["jesse <jesse@dgi.com>"]
 repository = "https://github.com/dynamic-graphics-inc/dgpy-libs"
 homepage = "https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/h5"
 readme = 'README.md'
 packages = [
@@ -26,26 +26,26 @@
   "h5",
   "numpy",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.0"
 h5py = ">=3.7.0"
-numpy = "^1.24.2"
+numpy = ">=1.23.2"
 typing-extensions = "^4.5.0"
 click = { version = "^8.1.3", optional = true }
 rich = { version = "^13.3.3", optional = true }
 globsters = { version = "^0.0.2", optional = true }
 
 [tool.poetry.extras]
 cli = ["click", "rich", "globsters"]
 
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.2"
+pytest = "^7.3.0"
 
 # coverage config
 # [tool.coverage.run]
 # omit = ["*/tests/*", "*/__init__.py", "h5/__main__.py",]
 [tool.poetry.scripts]
 h5 = "h5.cli:main"
```

### Comparing `h5-0.8.7/README.md` & `h5-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `h5-0.8.7/setup.py` & `h5-0.8.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 packages = \
 ['h5']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['h5py>=3.7.0', 'numpy>=1.24.2,<2.0.0', 'typing-extensions>=4.5.0,<5.0.0']
+['h5py>=3.7.0', 'numpy>=1.23.2', 'typing-extensions>=4.5.0,<5.0.0']
 
 extras_require = \
 {'cli': ['click>=8.1.3,<9.0.0',
          'rich>=13.3.3,<14.0.0',
          'globsters>=0.0.2,<0.0.3']}
 
 entry_points = \
 {'console_scripts': ['h5 = h5.cli:main']}
 
 setup_kwargs = {
     'name': 'h5',
-    'version': '0.8.7',
+    'version': '0.8.8',
     'description': 'H5py utils',
     'long_description': '<a href="https://github.com/dynamic-graphics-inc/dgpy-libs">\n<img align="right" src="https://github.com/dynamic-graphics-inc/dgpy-libs/blob/main/docs/images/dgpy_banner.svg?raw=true" alt="drawing" height="120" width="300"/>\n</a>\n\n# h5\n\n[![Wheel](https://img.shields.io/pypi/wheel/h5.svg)](https://img.shields.io/pypi/wheel/h5.svg)\n[![Version](https://img.shields.io/pypi/v/h5.svg)](https://img.shields.io/pypi/v/h5.svg)\n[![py_versions](https://img.shields.io/pypi/pyversions/h5.svg)](https://img.shields.io/pypi/pyversions/h5.svg)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n**Install:** `pip install h5`\n\n---\n\nUtil functions for h5py and home of recursive generators!\n',
     'author': 'jesse',
     'author_email': 'jesse@dgi.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/h5',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'': '.'}
 packages = \ ['h5'] package_data = \ {'': ['*']} install_requires = \
-['h5py>=3.7.0', 'numpy>=1.24.2,<2.0.0', 'typing-extensions>=4.5.0,<5.0.0']
+['h5py>=3.7.0', 'numpy>=1.23.2', 'typing-extensions>=4.5.0,<5.0.0']
 extras_require = \ {'cli': ['click>=8.1.3,<9.0.0', 'rich>=13.3.3,<14.0.0',
 'globsters>=0.0.2,<0.0.3']} entry_points = \ {'console_scripts': ['h5 = h5.cli:
-main']} setup_kwargs = { 'name': 'h5', 'version': '0.8.7', 'description': 'H5py
+main']} setup_kwargs = { 'name': 'h5', 'version': '0.8.8', 'description': 'H5py
 utils', 'long_description': '\n[drawing]\n\n\n# h5\n\n[![Wheel](https://
 img.shields.io/pypi/wheel/h5.svg)](https://img.shields.io/pypi/wheel/h5.svg)\n
 [![Version](https://img.shields.io/pypi/v/h5.svg)](https://img.shields.io/pypi/
 v/h5.svg)\n[![py_versions](https://img.shields.io/pypi/pyversions/h5.svg)]
 (https://img.shields.io/pypi/pyversions/h5.svg)\n[![Code style: black](https://
 img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
 black)\n\n**Install:** `pip install h5`\n\n---\n\nUtil functions for h5py and
```

### Comparing `h5-0.8.7/PKG-INFO` & `h5-0.8.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5
-Version: 0.8.7
+Version: 0.8.8
 Summary: H5py utils
 Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/h5
 License: MIT
 Keywords: hdf5,h5py,h5,numpy
 Author: jesse
 Author-email: jesse@dgi.com
 Requires-Python: >=3.8.0
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Provides-Extra: cli
 Requires-Dist: click (>=8.1.3,<9.0.0) ; extra == "cli"
 Requires-Dist: globsters (>=0.0.2,<0.0.3) ; extra == "cli"
 Requires-Dist: h5py (>=3.7.0)
-Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: numpy (>=1.23.2)
 Requires-Dist: rich (>=13.3.3,<14.0.0) ; extra == "cli"
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/dynamic-graphics-inc/dgpy-libs
 Description-Content-Type: text/markdown
 
 <a href="https://github.com/dynamic-graphics-inc/dgpy-libs">
 <img align="right" src="https://github.com/dynamic-graphics-inc/dgpy-libs/blob/main/docs/images/dgpy_banner.svg?raw=true" alt="drawing" height="120" width="300"/>
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: h5 Version: 0.8.7 Summary: H5py utils Home-page:
+Metadata-Version: 2.1 Name: h5 Version: 0.8.8 Summary: H5py utils Home-page:
 https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/h5 License:
 MIT Keywords: hdf5,h5py,h5,numpy Author: jesse Author-email: jesse@dgi.com
 Requires-Python: >=3.8.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Typing :: Typed Provides-Extra: cli Requires-Dist:
 click (>=8.1.3,<9.0.0) ; extra == "cli" Requires-Dist: globsters
 (>=0.0.2,<0.0.3) ; extra == "cli" Requires-Dist: h5py (>=3.7.0) Requires-Dist:
-numpy (>=1.24.2,<2.0.0) Requires-Dist: rich (>=13.3.3,<14.0.0) ; extra == "cli"
+numpy (>=1.23.2) Requires-Dist: rich (>=13.3.3,<14.0.0) ; extra == "cli"
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) Project-URL: Repository,
 https://github.com/dynamic-graphics-inc/dgpy-libs Description-Content-Type:
 text/markdown [drawing] # h5 [![Wheel](https://img.shields.io/pypi/wheel/
 h5.svg)](https://img.shields.io/pypi/wheel/h5.svg) [![Version](https://
 img.shields.io/pypi/v/h5.svg)](https://img.shields.io/pypi/v/h5.svg) [!
 [py_versions](https://img.shields.io/pypi/pyversions/h5.svg)](https://
 img.shields.io/pypi/pyversions/h5.svg) [![Code style: black](https://
```


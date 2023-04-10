# Comparing `tmp/edgetest-2022.7.0.tar.gz` & `tmp/edgetest-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgetest-2022.7.0.tar", last modified: Fri Jul 15 15:35:18 2022, max compression
+gzip compressed data, was "edgetest-2023.4.0.tar", last modified: Mon Apr 10 19:37:55 2023, max compression
```

## Comparing `edgetest-2022.7.0.tar` & `edgetest-2023.4.0.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 15:35:18.210664 edgetest-2022.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-07-15 15:34:45.000000 edgetest-2022.7.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-07-15 15:34:45.000000 edgetest-2022.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-07-15 15:34:45.000000 edgetest-2022.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5285 2022-07-15 15:35:18.210664 edgetest-2022.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4145 2022-07-15 15:34:45.000000 edgetest-2022.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 15:35:18.206664 edgetest-2022.7.0/edgetest/
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-07-15 15:34:45.000000 edgetest-2022.7.0/edgetest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5220 2022-07-15 15:34:45.000000 edgetest-2022.7.0/edgetest/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     2838 2022-07-15 15:34:45.000000 edgetest-2022.7.0/edgetest/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5506 2022-07-15 15:34:45.000000 edgetest-2022.7.0/edgetest/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     2051 2022-07-15 15:34:45.000000 edgetest-2022.7.0/edgetest/lib.py
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-07-15 15:34:45.000000 edgetest-2022.7.0/edgetest/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-07-15 15:34:45.000000 edgetest-2022.7.0/edgetest/report.py
--rw-r--r--   0 runner    (1001) docker     (121)     3230 2022-07-15 15:34:45.000000 edgetest-2022.7.0/edgetest/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     9751 2022-07-15 15:34:45.000000 edgetest-2022.7.0/edgetest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 15:35:18.206664 edgetest-2022.7.0/edgetest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5285 2022-07-15 15:35:18.000000 edgetest-2022.7.0/edgetest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-07-15 15:35:18.000000 edgetest-2022.7.0/edgetest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-15 15:35:18.000000 edgetest-2022.7.0/edgetest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-07-15 15:35:18.000000 edgetest-2022.7.0/edgetest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-15 15:35:12.000000 edgetest-2022.7.0/edgetest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-07-15 15:35:18.000000 edgetest-2022.7.0/edgetest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-07-15 15:35:18.000000 edgetest-2022.7.0/edgetest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-07-15 15:34:45.000000 edgetest-2022.7.0/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-07-15 15:34:45.000000 edgetest-2022.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2944 2022-07-15 15:35:18.210664 edgetest-2022.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-07-15 15:34:45.000000 edgetest-2022.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 15:35:18.210664 edgetest-2022.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 15:34:45.000000 edgetest-2022.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-07-15 15:34:45.000000 edgetest-2022.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     5352 2022-07-15 15:34:45.000000 edgetest-2022.7.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)     4144 2022-07-15 15:34:45.000000 edgetest-2022.7.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)    12621 2022-07-15 15:34:45.000000 edgetest-2022.7.0/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-07-15 15:34:45.000000 edgetest-2022.7.0/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-07-15 15:34:45.000000 edgetest-2022.7.0/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-07-15 15:34:45.000000 edgetest-2022.7.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     5150 2022-07-15 15:34:45.000000 edgetest-2022.7.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:37:55.486532 edgetest-2023.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 19:37:17.000000 edgetest-2023.4.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 19:37:17.000000 edgetest-2023.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 19:37:17.000000 edgetest-2023.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-04-10 19:37:55.486532 edgetest-2023.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-10 19:37:17.000000 edgetest-2023.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:37:55.482532 edgetest-2023.4.0/edgetest/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-10 19:37:17.000000 edgetest-2023.4.0/edgetest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-10 19:37:17.000000 edgetest-2023.4.0/edgetest/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-10 19:37:17.000000 edgetest-2023.4.0/edgetest/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-04-10 19:37:17.000000 edgetest-2023.4.0/edgetest/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-10 19:37:17.000000 edgetest-2023.4.0/edgetest/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-10 19:37:17.000000 edgetest-2023.4.0/edgetest/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-10 19:37:17.000000 edgetest-2023.4.0/edgetest/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-10 19:37:17.000000 edgetest-2023.4.0/edgetest/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-04-10 19:37:17.000000 edgetest-2023.4.0/edgetest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:37:55.486532 edgetest-2023.4.0/edgetest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-04-10 19:37:55.000000 edgetest-2023.4.0/edgetest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-10 19:37:55.000000 edgetest-2023.4.0/edgetest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:37:55.000000 edgetest-2023.4.0/edgetest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 19:37:55.000000 edgetest-2023.4.0/edgetest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:37:47.000000 edgetest-2023.4.0/edgetest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-10 19:37:55.000000 edgetest-2023.4.0/edgetest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-10 19:37:55.000000 edgetest-2023.4.0/edgetest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-10 19:37:17.000000 edgetest-2023.4.0/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-10 19:37:17.000000 edgetest-2023.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-10 19:37:55.490532 edgetest-2023.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-10 19:37:17.000000 edgetest-2023.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:37:55.486532 edgetest-2023.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/test_integration_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/test_integration_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/test_interface_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/test_interface_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-04-10 19:37:17.000000 edgetest-2023.4.0/tests/test_utils.py
```

### Comparing `edgetest-2022.7.0/LICENSE` & `edgetest-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgetest-2022.7.0/PKG-INFO` & `edgetest-2023.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgetest
-Version: 2022.7.0
+Version: 2023.4.0
 Summary: Bleeding edge dependency testing
 Home-page: https://github.com/capitalone/edgetest
 Author: Akshay Gupta
 Author-email: akshay.gupta2@capitalone.com
 Maintainer: Akshay Gupta
 Maintainer-email: akshay.gupta2@capitalone.com
 License: Apache Software License
@@ -16,14 +16,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: qa
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
@@ -31,28 +32,37 @@
 
 # Bleeding edge dependency testing
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edgetest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![PyPI version](https://badge.fury.io/py/edgetest.svg)](https://badge.fury.io/py/edgetest)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/edgetest/badges/version.svg)](https://anaconda.org/conda-forge/edgetest)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/edgetest)
 
 [Full Documentation](https://capitalone.github.io/edgetest/)
 
-`edgetest` is a `tox`-inspired python library that will loop through your project's dependencies, and check if your 
+`edgetest` is a `tox`-inspired python library that will loop through your project's dependencies, and check if your
 project is compatible with the latest version of each dependency. It does this by:
 
 * creating a virtual environment,
 * installing your local package into the environment,
 * upgrading specified dependency package(s), and
 * running your test command.
 
 For example, if you depend on ``pandas>=0.25.1,<=1.0.0``, ``edgetest`` will test your project against the most current
 pandas version (say ``1.3.4``), so you know if you can safely update your dependency to ``pandas>=0.25.1,<=1.3.4`` or not.
 
+
+`edgetest` works with the following types of projects:
+
+- `pyproject.toml`
+- `setup.cfg`
+- and `requirements.txt`
+
+
 Table Of Contents
 -----------------
 
 - [Install](#install)
 - [Getting Started](#getting-started)
 - [Options](#options)
 - [Plugins](#plugins)
@@ -74,15 +84,16 @@
 ```console
 $ conda install -c conda-forge edgetest
 ```
 
 Getting Started
 ---------------
 
-``edgetest`` allows multi-package, bleeding edge dependency testing. Suppose you have a package, ``mypackage``, with the following ``requirements.txt``:
+``edgetest`` allows multi-package, bleeding edge dependency testing. Suppose you have a package, ``mypackage``, with
+the following ``requirements.txt``:
 
 ```
 pandas>=0.25.1,<=1.0.0
 ...
 ```
 
 ``edgetest`` allows you to test your package against the latest version of ``pandas``. If you run
@@ -145,8 +156,7 @@
 Apache-2.0
 
 
 Roadmap
 -------
 
 Roadmap details can be found [here](https://capitalone.github.io/edgetest/roadmap.html).
-
```

### Comparing `edgetest-2022.7.0/README.md` & `edgetest-2023.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 # Bleeding edge dependency testing
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edgetest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![PyPI version](https://badge.fury.io/py/edgetest.svg)](https://badge.fury.io/py/edgetest)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/edgetest/badges/version.svg)](https://anaconda.org/conda-forge/edgetest)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/edgetest)
 
 [Full Documentation](https://capitalone.github.io/edgetest/)
 
-`edgetest` is a `tox`-inspired python library that will loop through your project's dependencies, and check if your 
+`edgetest` is a `tox`-inspired python library that will loop through your project's dependencies, and check if your
 project is compatible with the latest version of each dependency. It does this by:
 
 * creating a virtual environment,
 * installing your local package into the environment,
 * upgrading specified dependency package(s), and
 * running your test command.
 
 For example, if you depend on ``pandas>=0.25.1,<=1.0.0``, ``edgetest`` will test your project against the most current
 pandas version (say ``1.3.4``), so you know if you can safely update your dependency to ``pandas>=0.25.1,<=1.3.4`` or not.
 
+
+`edgetest` works with the following types of projects:
+
+- `pyproject.toml`
+- `setup.cfg`
+- and `requirements.txt`
+
+
 Table Of Contents
 -----------------
 
 - [Install](#install)
 - [Getting Started](#getting-started)
 - [Options](#options)
 - [Plugins](#plugins)
@@ -43,15 +52,16 @@
 ```console
 $ conda install -c conda-forge edgetest
 ```
 
 Getting Started
 ---------------
 
-``edgetest`` allows multi-package, bleeding edge dependency testing. Suppose you have a package, ``mypackage``, with the following ``requirements.txt``:
+``edgetest`` allows multi-package, bleeding edge dependency testing. Suppose you have a package, ``mypackage``, with
+the following ``requirements.txt``:
 
 ```
 pandas>=0.25.1,<=1.0.0
 ...
 ```
 
 ``edgetest`` allows you to test your package against the latest version of ``pandas``. If you run
@@ -114,8 +124,7 @@
 Apache-2.0
 
 
 Roadmap
 -------
 
 Roadmap details can be found [here](https://capitalone.github.io/edgetest/roadmap.html).
-
```

### Comparing `edgetest-2022.7.0/edgetest/core.py` & `edgetest-2023.4.0/edgetest/core.py`

 * *Files identical despite different names*

### Comparing `edgetest-2022.7.0/edgetest/hookspecs.py` & `edgetest-2023.4.0/edgetest/hookspecs.py`

 * *Files identical despite different names*

### Comparing `edgetest-2022.7.0/edgetest/interface.py` & `edgetest-2023.4.0/edgetest/interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """Command-line interface."""
 
 from pathlib import Path
 from typing import List
 
 import click
 import pluggy
+from tomlkit import dumps
 
 from . import hookspecs, lib
 from .core import TestPackage
 from .logger import get_logger
 from .report import gen_report
 from .schema import EdgetestValidator, Schema
 from .utils import (
     gen_requirements_config,
     parse_cfg,
+    parse_toml,
+    upgrade_pyproject_toml,
     upgrade_requirements,
     upgrade_setup_cfg,
 )
 
 LOG = get_logger(__name__)
 
 
@@ -105,31 +108,32 @@
     extras,
     deps,
     command,
     export,
 ):
     """Create the environments and test.
 
-    If you do not supply a YAML configuration file, this package will search for a
+    If you do not supply a configuration file, this package will search for a
     ``requirements.txt`` file and create a conda environment for each package in that file.
     """
     # Get the hooks
     pm = get_plugin_manager()
-    if config:
+    if config and Path(config).suffix == ".cfg":
         conf = parse_cfg(filename=config, requirements=requirements)
+    elif config and Path(config).suffix == ".toml":
+        conf = parse_toml(filename=config, requirements=requirements)
     else:
         # Find the path to the local directory using the requirements file
         conf = gen_requirements_config(
             fname_or_buf=requirements,
             extras=extras,
             deps=deps,
             command=command,
             package_dir=str(Path(requirements).parent),
         )
-
     # Validate the configuration file
     docstructure = Schema()
     pm.hook.addoption(schema=docstructure)
     validator = EdgetestValidator(schema=docstructure.schema)
     if not validator.validate(conf):
         click.echo("Unable to validate configuration file.")
         raise ValueError("Unable to validate configuration file.")
@@ -178,14 +182,32 @@
                     f"{requirements}"
                 )
                 upgraded = upgrade_requirements(
                     fname_or_buf=requirements,
                     upgraded_packages=testers[-1].upgraded_packages(),
                 )
                 with open(requirements, "w") as outfile:
+                    outfile.write(upgraded)
+        elif config is not None and Path(config).name == "pyproject.toml":
+            parser = upgrade_pyproject_toml(
+                upgraded_packages=testers[-1].upgraded_packages(),
+                filename=config,
+            )
+            with open(config, "w") as outfile:
+                outfile.write(dumps(parser))
+            if "project" not in parser or not parser.get("project").get("dependencies"):
+                click.echo(
+                    "No dependencies in ``pyproject.toml`` to update. Updating "
+                    f"{requirements}"
+                )
+                upgraded = upgrade_requirements(
+                    fname_or_buf=requirements,
+                    upgraded_packages=testers[-1].upgraded_packages(),
+                )
+                with open(requirements, "w") as outfile:
                     outfile.write(upgraded)
         else:
             click.echo(f"Overwriting the requirements file {requirements}...")
             upgraded = upgrade_requirements(
                 fname_or_buf=requirements,
                 upgraded_packages=testers[-1].upgraded_packages(),
             )
```

### Comparing `edgetest-2022.7.0/edgetest/lib.py` & `edgetest-2023.4.0/edgetest/lib.py`

 * *Files identical despite different names*

### Comparing `edgetest-2022.7.0/edgetest/logger.py` & `edgetest-2023.4.0/edgetest/logger.py`

 * *Files identical despite different names*

### Comparing `edgetest-2022.7.0/edgetest/report.py` & `edgetest-2023.4.0/edgetest/report.py`

 * *Files identical despite different names*

### Comparing `edgetest-2022.7.0/edgetest/schema.py` & `edgetest-2023.4.0/edgetest/schema.py`

 * *Files identical despite different names*

### Comparing `edgetest-2022.7.0/edgetest.egg-info/PKG-INFO` & `edgetest-2023.4.0/edgetest.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgetest
-Version: 2022.7.0
+Version: 2023.4.0
 Summary: Bleeding edge dependency testing
 Home-page: https://github.com/capitalone/edgetest
 Author: Akshay Gupta
 Author-email: akshay.gupta2@capitalone.com
 Maintainer: Akshay Gupta
 Maintainer-email: akshay.gupta2@capitalone.com
 License: Apache Software License
@@ -16,14 +16,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: qa
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
@@ -31,28 +32,37 @@
 
 # Bleeding edge dependency testing
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edgetest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![PyPI version](https://badge.fury.io/py/edgetest.svg)](https://badge.fury.io/py/edgetest)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/edgetest/badges/version.svg)](https://anaconda.org/conda-forge/edgetest)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/edgetest)
 
 [Full Documentation](https://capitalone.github.io/edgetest/)
 
-`edgetest` is a `tox`-inspired python library that will loop through your project's dependencies, and check if your 
+`edgetest` is a `tox`-inspired python library that will loop through your project's dependencies, and check if your
 project is compatible with the latest version of each dependency. It does this by:
 
 * creating a virtual environment,
 * installing your local package into the environment,
 * upgrading specified dependency package(s), and
 * running your test command.
 
 For example, if you depend on ``pandas>=0.25.1,<=1.0.0``, ``edgetest`` will test your project against the most current
 pandas version (say ``1.3.4``), so you know if you can safely update your dependency to ``pandas>=0.25.1,<=1.3.4`` or not.
 
+
+`edgetest` works with the following types of projects:
+
+- `pyproject.toml`
+- `setup.cfg`
+- and `requirements.txt`
+
+
 Table Of Contents
 -----------------
 
 - [Install](#install)
 - [Getting Started](#getting-started)
 - [Options](#options)
 - [Plugins](#plugins)
@@ -74,15 +84,16 @@
 ```console
 $ conda install -c conda-forge edgetest
 ```
 
 Getting Started
 ---------------
 
-``edgetest`` allows multi-package, bleeding edge dependency testing. Suppose you have a package, ``mypackage``, with the following ``requirements.txt``:
+``edgetest`` allows multi-package, bleeding edge dependency testing. Suppose you have a package, ``mypackage``, with
+the following ``requirements.txt``:
 
 ```
 pandas>=0.25.1,<=1.0.0
 ...
 ```
 
 ``edgetest`` allows you to test your package against the latest version of ``pandas``. If you run
@@ -145,8 +156,7 @@
 Apache-2.0
 
 
 Roadmap
 -------
 
 Roadmap details can be found [here](https://capitalone.github.io/edgetest/roadmap.html).
-
```

### Comparing `edgetest-2022.7.0/edgetest.egg-info/requires.txt` & `edgetest-2023.4.0/edgetest.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Cerberus<=1.3.4,>=1.3.0
 click<=8.1.3,>=7.0
 pluggy<=1.0.0,>=1.0.0
-tabulate<=0.8.10,>=0.8.9
-packaging<=21.3,>20.6
+tabulate<=0.9.0,>=0.8.9
+packaging<=23.0,>20.6
+tomlkit<=0.11.4,>=0.11.4
 
 [build]
 build
 twine
 wheel
 bumpver
```

### Comparing `edgetest-2022.7.0/pull_request_template.md` & `edgetest-2023.4.0/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `edgetest-2022.7.0/setup.cfg` & `edgetest-2023.4.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -22,25 +22,27 @@
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
 	Cerberus<=1.3.4,>=1.3.0
 	click<=8.1.3,>=7.0
 	pluggy<=1.0.0,>=1.0.0
-	tabulate<=0.8.10,>=0.8.9
-	packaging<=21.3,>20.6
+	tabulate<=0.9.0,>=0.8.9
+	packaging<=23.0,>20.6
+	tomlkit<=0.11.4,>=0.11.4
 
 [options.extras_require]
 docs = 
 	furo
 	sphinx
 	sphinx-copybutton
 	sphinx-tabs
@@ -94,15 +96,15 @@
 	bumpver
 
 [options.entry_points]
 console_scripts = 
 	edgetest = edgetest.interface:cli
 
 [bumpver]
-current_version = "2022.7.0"
+current_version = "2023.4.0"
 version_pattern = "YYYY.MM.INC0"
 commit_message = "Bump {old_version} to {new_version}"
 commit = True
 
 [bumpver:file_patterns]
 docs/source/conf.py = 
 	version = "{version}"
@@ -127,19 +129,20 @@
 multi_line_output = 3
 include_trailing_comma = True
 force_grid_wrap = 0
 use_parentheses = True
 line_length = 88
 
 [mypy]
-python_version = 3.7
+python_version = 3.9
 warn_return_any = True
 warn_unused_configs = True
 ignore_missing_imports = True
 allow_redefinition = True
+disable_error_code = empty-body
 
 [pylint]
 pylint_minimum_score = 9.5
 
 [tool:pytest]
 markers = 
 	unit: mark unit tests that do not require external interfaces and use mocking
```

### Comparing `edgetest-2022.7.0/tests/conftest.py` & `edgetest-2023.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `edgetest-2022.7.0/tests/test_core.py` & `edgetest-2023.4.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `edgetest-2022.7.0/tests/test_integration.py` & `edgetest-2023.4.0/tests/test_integration_cfg.py`

 * *Files identical despite different names*

### Comparing `edgetest-2022.7.0/tests/test_interface.py` & `edgetest-2023.4.0/tests/test_interface_cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         )
     ]
 
     assert result.output == TABLE_OUTPUT
 
 
 @patch("edgetest.lib.EnvBuilder", autospec=True)
-@patch("edgetest.core.Popen", autospect=True)
+@patch("edgetest.core.Popen", autospec=True)
 @patch("edgetest.utils.Popen", autospec=True)
 def test_cli_reqs(mock_popen, mock_cpopen, mock_builder):
     """Test running tests based on the requirements file."""
     mock_popen.return_value.communicate.return_value = (PIP_LIST, "error")
     type(mock_popen.return_value).returncode = PropertyMock(return_value=0)
     mock_cpopen.return_value.communicate.return_value = ("output", "error")
     type(mock_cpopen.return_value).returncode = PropertyMock(return_value=0)
@@ -266,15 +266,15 @@
         ),
     ]
 
     assert result.output == TABLE_OUTPUT_REQS
 
 
 @patch("edgetest.lib.EnvBuilder", autospec=True)
-@patch("edgetest.core.Popen", autospect=True)
+@patch("edgetest.core.Popen", autospec=True)
 @patch("edgetest.utils.Popen", autospec=True)
 def test_cli_setup_reqs_update(mock_popen, mock_cpopen, mock_builder):
     """Test running tests and updating requirements in a ``setup.cfg`` file."""
     mock_popen.return_value.communicate.return_value = (PIP_LIST, "error")
     type(mock_popen.return_value).returncode = PropertyMock(return_value=0)
     mock_cpopen.return_value.communicate.return_value = ("output", "error")
     type(mock_cpopen.return_value).returncode = PropertyMock(return_value=0)
@@ -292,15 +292,15 @@
 
     assert result.exit_code == 0
 
     assert out == SETUP_CFG_REQS_UPGRADE
 
 
 @patch("edgetest.lib.EnvBuilder", autospec=True)
-@patch("edgetest.core.Popen", autospect=True)
+@patch("edgetest.core.Popen", autospec=True)
 @patch("edgetest.utils.Popen", autospec=True)
 def test_cli_setup_extras_update(mock_popen, mock_cpopen, mock_builder):
     """Test running tests and updating extra installation requirements in a ``setup.cfg`` file."""
     mock_popen.return_value.communicate.return_value = (PIP_LIST, "error")
     type(mock_popen.return_value).returncode = PropertyMock(return_value=0)
     mock_cpopen.return_value.communicate.return_value = ("output", "error")
     type(mock_cpopen.return_value).returncode = PropertyMock(return_value=0)
@@ -319,15 +319,15 @@
             out = infile.read()
 
     assert result.exit_code == 0
 
     assert out == SETUP_CFG_EXTRAS_UPGRADE
 
 
-@patch("edgetest.core.Popen", autospect=True)
+@patch("edgetest.core.Popen", autospec=True)
 @patch("edgetest.utils.Popen", autospec=True)
 def test_cli_nosetup(mock_popen, mock_cpopen):
     """Test creating a basic environment."""
     mock_popen.return_value.communicate.return_value = (PIP_LIST, "error")
     type(mock_popen.return_value).returncode = PropertyMock(return_value=0)
     mock_cpopen.return_value.communicate.return_value = ("output", "error")
     type(mock_cpopen.return_value).returncode = PropertyMock(return_value=0)
```

### Comparing `edgetest-2022.7.0/tests/test_lib.py` & `edgetest-2023.4.0/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `edgetest-2022.7.0/tests/test_report.py` & `edgetest-2023.4.0/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `edgetest-2022.7.0/tests/test_schema.py` & `edgetest-2023.4.0/tests/test_schema.py`

 * *Files identical despite different names*


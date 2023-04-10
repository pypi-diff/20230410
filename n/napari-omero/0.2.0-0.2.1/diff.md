# Comparing `tmp/napari_omero-0.2.0.tar.gz` & `tmp/napari_omero-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_omero-0.2.0.tar", last modified: Sun May 22 23:26:56 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `napari_omero-0.2.0.tar` & `napari_omero-0.2.1.tar`

### file list

```diff
@@ -1,47 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 23:26:56.943984 napari_omero-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 23:26:56.931984 napari_omero-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 23:26:56.943984 napari_omero-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2524 2022-05-22 23:26:38.000000 napari_omero-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-05-22 23:26:38.000000 napari_omero-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-05-22 23:26:38.000000 napari_omero-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-05-22 23:26:38.000000 napari_omero-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6775 2022-05-22 23:26:56.943984 napari_omero-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5025 2022-05-22 23:26:38.000000 napari_omero-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121) 10477702 2022-05-22 23:26:38.000000 napari_omero-0.2.0/demo.gif
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-05-22 23:26:38.000000 napari_omero-0.2.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-05-22 23:26:38.000000 napari_omero-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2127 2022-05-22 23:26:56.943984 napari_omero-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 23:26:56.931984 napari_omero-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 23:26:56.943984 napari_omero-0.2.0/src/napari_omero/
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-05-22 23:26:38.000000 napari_omero-0.2.0/src/napari_omero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-05-22 23:26:38.000000 napari_omero-0.2.0/src/napari_omero/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-05-22 23:26:55.000000 napari_omero-0.2.0/src/napari_omero/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-05-22 23:26:38.000000 napari_omero-0.2.0/src/napari_omero/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 23:26:56.943984 napari_omero-0.2.0/src/napari_omero/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-22 23:26:38.000000 napari_omero-0.2.0/src/napari_omero/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-05-22 23:26:38.000000 napari_omero-0.2.0/src/napari_omero/plugins/_napari.py
--rw-r--r--   0 runner    (1001) docker     (121)     3931 2022-05-22 23:26:38.000000 napari_omero-0.2.0/src/napari_omero/plugins/loaders.py
--rw-r--r--   0 runner    (1001) docker     (121)     1812 2022-05-22 23:26:38.000000 napari_omero-0.2.0/src/napari_omero/plugins/masks.py
--rw-r--r--   0 runner    (1001) docker     (121)     9811 2022-05-22 23:26:38.000000 napari_omero-0.2.0/src/napari_omero/plugins/omero.py
--rw-r--r--   0 runner    (1001) docker     (121)     2469 2022-05-22 23:26:38.000000 napari_omero-0.2.0/src/napari_omero/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 23:26:56.943984 napari_omero-0.2.0/src/napari_omero/widgets/
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-05-22 23:26:38.000000 napari_omero-0.2.0/src/napari_omero/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6091 2022-05-22 23:26:38.000000 napari_omero-0.2.0/src/napari_omero/widgets/gateway.py
--rw-r--r--   0 runner    (1001) docker     (121)     2582 2022-05-22 23:26:38.000000 napari_omero-0.2.0/src/napari_omero/widgets/login.py
--rw-r--r--   0 runner    (1001) docker     (121)     3045 2022-05-22 23:26:38.000000 napari_omero-0.2.0/src/napari_omero/widgets/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     2767 2022-05-22 23:26:38.000000 napari_omero-0.2.0/src/napari_omero/widgets/thumb_grid.py
--rw-r--r--   0 runner    (1001) docker     (121)     3709 2022-05-22 23:26:38.000000 napari_omero-0.2.0/src/napari_omero/widgets/tree_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 23:26:56.943984 napari_omero-0.2.0/src/napari_omero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6775 2022-05-22 23:26:56.000000 napari_omero-0.2.0/src/napari_omero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-05-22 23:26:56.000000 napari_omero-0.2.0/src/napari_omero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-22 23:26:56.000000 napari_omero-0.2.0/src/napari_omero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-05-22 23:26:56.000000 napari_omero-0.2.0/src/napari_omero.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-05-22 23:26:56.000000 napari_omero-0.2.0/src/napari_omero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-05-22 23:26:56.000000 napari_omero-0.2.0/src/napari_omero.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 23:26:56.931984 napari_omero-0.2.0/src/omero/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 23:26:56.943984 napari_omero-0.2.0/src/omero/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-05-22 23:26:38.000000 napari_omero-0.2.0/src/omero/plugins/napari.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-22 23:26:56.943984 napari_omero-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-05-22 23:26:38.000000 napari_omero-0.2.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-05-22 23:26:38.000000 napari_omero-0.2.0/tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-05-22 23:26:38.000000 napari_omero-0.2.0/tox.ini
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 napari_omero-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0 10477702 2020-02-02 00:00:00.000000 napari_omero-0.2.1/demo.gif
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 napari_omero-0.2.1/tox.ini
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 napari_omero-0.2.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 napari_omero-0.2.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 napari_omero-0.2.1/src/napari_omero/__init__.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 napari_omero-0.2.1/src/napari_omero/__main__.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 napari_omero-0.2.1/src/napari_omero/napari.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 napari_omero-0.2.1/src/napari_omero/py.typed
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 napari_omero-0.2.1/src/napari_omero/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 napari_omero-0.2.1/src/napari_omero/plugins/__init__.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 napari_omero-0.2.1/src/napari_omero/plugins/_napari.py
+-rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 napari_omero-0.2.1/src/napari_omero/plugins/loaders.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 napari_omero-0.2.1/src/napari_omero/plugins/masks.py
+-rw-r--r--   0        0        0     9799 2020-02-02 00:00:00.000000 napari_omero-0.2.1/src/napari_omero/plugins/omero.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 napari_omero-0.2.1/src/napari_omero/widgets/__init__.py
+-rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 napari_omero-0.2.1/src/napari_omero/widgets/gateway.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 napari_omero-0.2.1/src/napari_omero/widgets/login.py
+-rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 napari_omero-0.2.1/src/napari_omero/widgets/main.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 napari_omero-0.2.1/src/napari_omero/widgets/thumb_grid.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 napari_omero-0.2.1/src/napari_omero/widgets/tree_model.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 napari_omero-0.2.1/src/omero/plugins/napari.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 napari_omero-0.2.1/tests/test_utils.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 napari_omero-0.2.1/tests/test_widget.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 napari_omero-0.2.1/.gitignore
+-rw-r--r--   0        0        0    15144 2020-02-02 00:00:00.000000 napari_omero-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 napari_omero-0.2.1/README.md
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 napari_omero-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 napari_omero-0.2.1/PKG-INFO
```

### Comparing `napari_omero-0.2.0/.github/workflows/ci.yml` & `napari_omero-0.2.1/.github/workflows/ci.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 name: CI
 
-on: 
+on:
   push:
     branches:
       - main
     tags:
       - "v*" # Push events to matching v*, i.e. v1.0, v20.15.10
   pull_request:
     branches:
       - main
   workflow_dispatch:
 
 jobs:
+  check-manifest:
+    # check-manifest is a tool that checks that all files in version control are
+    # included in the sdist (unless explicitly excluded)
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+      - run: pipx run check-manifest
 
   test:
     name: ${{ matrix.platform }} ${{ matrix.python-version }}
     runs-on: ${{ matrix.platform }}
     defaults:
       run:
         shell: bash -l {0}
     strategy:
       fail-fast: false
       matrix:
         platform: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: [3.8, 3.9, '3.10']
+        python-version: ["3.8", "3.9", "3.10"]
         backend: [pyqt5]
         include:
           - platform: ubuntu-latest
             python-version: 3.7
             backend: pyqt5
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - uses: conda-incubator/setup-miniconda@v2
         with:
           miniconda-version: "latest"
           channels: conda-forge
           channel-priority: strict
           python-version: ${{ matrix.python-version }}
 
@@ -49,37 +56,37 @@
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install --upgrade setuptools tox tox-conda tox-gh-actions
 
       - name: Test with tox
-        run: tox
+        uses: aganders3/headless-gui@v1.2
+        with:
+          shell: bash -el {0}
+          run: python -m tox
         env:
           PLATFORM: ${{ matrix.platform }}
           PYTHON: ${{ matrix.python-version }}
           PYVISTA_OFF_SCREEN: True
           BACKEND: ${{ matrix.backend }}
 
       - name: Codecov
-        uses: codecov/codecov-action@v2
-        with:
-          fail_ci_if_error: true
-
+        uses: codecov/codecov-action@v3
 
   deploy:
     # this will run when you have tagged a commit, starting with "v*"
-    # and requires that you have put your twine API key in your 
+    # and requires that you have put your twine API key in your
     needs: [test]
     if: github.repository == 'tlambert03/napari-omero' && contains(github.ref, 'tags')
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -U build twine
       - name: Build and publish
```

### Comparing `napari_omero-0.2.0/.gitignore` & `napari_omero-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_omero-0.2.0/PKG-INFO` & `napari_omero-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,70 @@
 Metadata-Version: 2.1
-Name: napari_omero
-Version: 0.2.0
+Name: napari-omero
+Version: 0.2.1
 Summary: napari/OMERO interoperability
-Home-page: https://github.com/tlambert03/napari-omero
-Author: The Open Microscopy and napari teams
-Author-email: talley.lambert@gmail.com
-License: BSD-3-Clause
-Project-URL: Bug Tracker, https://github.com/tlambert03/napari-omero/issues
-Project-URL: Source Code, https://github.com/tlambert03/napari-omero
-Keywords: OMERO.CLI plugin napari napari-plugin
-Platform: any
+Project-URL: homepage, https://github.com/tlambert03/napari-omero
+Project-URL: repository, https://github.com/tlambert03/napari-omero
+Author: Will Moore
+Author-email: Talley Lambert <talley.lambert@gmail.com>
+License: GPL-2.0-or-later
+License-File: LICENSE
+Keywords: OMERO.CLI,napari,napari-plugin,plugin
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Requires-Dist: importlib-metadata; python_version < '3.8'
+Requires-Dist: napari>=0.4.13
+Requires-Dist: omero-py
+Requires-Dist: omero-rois
 Provides-Extra: all
+Requires-Dist: napari[all]; extra == 'all'
 Provides-Extra: dev
-Provides-Extra: tests
-License-File: LICENSE
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: ipython; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: pdbpp; extra == 'dev'
+Requires-Dist: rich; extra == 'dev'
+Requires-Dist: ruff; extra == 'dev'
+Provides-Extra: test
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: pytest-qt; extra == 'test'
+Requires-Dist: pytest-regressions; extra == 'test'
+Requires-Dist: pywin32; sys_platform == 'win32' and extra == 'test'
+Description-Content-Type: text/markdown
 
 # napari-omero
 
-[![License](https://img.shields.io/github/license/tlambert03/napari-omero)](LICENSE)
-[![Version](https://img.shields.io/pypi/v/napari-omero.svg)](https://pypi.python.org/pypi/napari-omero)
-[![Python Version](https://img.shields.io/pypi/pyversions/napari-omero.svg)](https://python.org)
-[![CI](https://github.com/tlambert03/napari-omero/workflows/CI/badge.svg)](https://github.com/tlambert03/napari-omero/actions)
-<!-- [![conda-forge](https://img.shields.io/conda/vn/conda-forge/napari-omero)](https://anaconda.org/conda-forge/napari-omero) -->
+[![License](https://img.shields.io/pypi/l/napari-omero.svg?color=green)](https://github.com/tlambert03/napari-omero/raw/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/napari-omero.svg?color=green)](https://pypi.org/project/napari-omero)
+[![Python Version](https://img.shields.io/pypi/pyversions/napari-omero.svg?color=green)](https://python.org)
+[![CI](https://github.com/tlambert03/napari-omero/actions/workflows/ci.yml/badge.svg)](https://github.com/tlambert03/napari-omero/actions/workflows/ci.yml)
+[![codecov](https://codecov.io/gh/tlambert03/napari-omero/branch/main/graph/badge.svg)](https://codecov.io/gh/tlambert03/napari-omero)
+[![conda-forge](https://img.shields.io/conda/vn/conda-forge/napari-omero)](https://anaconda.org/conda-forge/napari-omero)
 
 This package provides interoperability between the
 [OMERO](https://www.openmicroscopy.org/omero/) image management platform, and
 [napari](https://github.com/napari/napari): a fast, multi-dimensional image
 viewer for python.
 
 It provides a GUI interface for browsing an OMERO instance from within napari,
```

### Comparing `napari_omero-0.2.0/README.md` & `napari_omero-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # napari-omero
 
-[![License](https://img.shields.io/github/license/tlambert03/napari-omero)](LICENSE)
-[![Version](https://img.shields.io/pypi/v/napari-omero.svg)](https://pypi.python.org/pypi/napari-omero)
-[![Python Version](https://img.shields.io/pypi/pyversions/napari-omero.svg)](https://python.org)
-[![CI](https://github.com/tlambert03/napari-omero/workflows/CI/badge.svg)](https://github.com/tlambert03/napari-omero/actions)
-<!-- [![conda-forge](https://img.shields.io/conda/vn/conda-forge/napari-omero)](https://anaconda.org/conda-forge/napari-omero) -->
+[![License](https://img.shields.io/pypi/l/napari-omero.svg?color=green)](https://github.com/tlambert03/napari-omero/raw/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/napari-omero.svg?color=green)](https://pypi.org/project/napari-omero)
+[![Python Version](https://img.shields.io/pypi/pyversions/napari-omero.svg?color=green)](https://python.org)
+[![CI](https://github.com/tlambert03/napari-omero/actions/workflows/ci.yml/badge.svg)](https://github.com/tlambert03/napari-omero/actions/workflows/ci.yml)
+[![codecov](https://codecov.io/gh/tlambert03/napari-omero/branch/main/graph/badge.svg)](https://codecov.io/gh/tlambert03/napari-omero)
+[![conda-forge](https://img.shields.io/conda/vn/conda-forge/napari-omero)](https://anaconda.org/conda-forge/napari-omero)
 
 This package provides interoperability between the
 [OMERO](https://www.openmicroscopy.org/omero/) image management platform, and
 [napari](https://github.com/napari/napari): a fast, multi-dimensional image
 viewer for python.
 
 It provides a GUI interface for browsing an OMERO instance from within napari,
```

### Comparing `napari_omero-0.2.0/demo.gif` & `napari_omero-0.2.1/demo.gif`

 * *Files identical despite different names*

### Comparing `napari_omero-0.2.0/src/napari_omero/plugins/_napari.py` & `napari_omero-0.2.1/src/napari_omero/plugins/_napari.py`

 * *Files identical despite different names*

### Comparing `napari_omero-0.2.0/src/napari_omero/plugins/loaders.py` & `napari_omero-0.2.1/src/napari_omero/plugins/loaders.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Dict, List
+from typing import Dict, List, Optional
 
 import dask.array as da
-from dask import delayed
+from dask.delayed import delayed
 from napari.types import LayerData
 from omero.cli import ProxyStringType
 from omero.gateway import BlitzGateway, ImageWrapper
 from omero.model import IObject
 from vispy.color import Colormap
 
 from ..utils import PIXEL_TYPES, lookup_obj, parse_omero_url, timer
 from ..widgets import QGateWay
 
 
-@timer
-def get_gateway(path: str, host: str = None) -> BlitzGateway:
+# @timer
+def get_gateway(path: str, host: Optional[str] = None) -> BlitzGateway:
     gateway = QGateWay()
     if host:
         if host != gateway.host:
             gateway.close()
         gateway.host = host
 
     if gateway.isConnected():
@@ -45,17 +45,17 @@
             gateway, ProxyStringType("Image")(f"Image:{match.get('id')}")
         )
         if isinstance(wrapper, ImageWrapper):
             return load_image_wrapper(wrapper)
     return []
 
 
-@timer
+# @timer
 def omero_proxy_reader(
-    path: str, proxy_obj: IObject = None
+    path: str, proxy_obj: Optional[IObject] = None
 ) -> List[LayerData]:
     gateway = get_gateway(path)
 
     if proxy_obj.__class__.__name__.startswith("Image"):
         wrapper = lookup_obj(gateway, proxy_obj)
         if isinstance(wrapper, ImageWrapper):
             return load_image_wrapper(wrapper)
@@ -78,49 +78,47 @@
     colors = []
     for ch in channels:
         # use current rendering settings from OMERO
         color = ch.getColor().getRGB()
         color = [r / 256 for r in color]
         colors.append(Colormap([[0, 0, 0], color]))
 
-    contrast_limits = [
-        [ch.getWindowStart(), ch.getWindowEnd()] for ch in channels
-    ]
+    contrast_limits = [[ch.getWindowStart(), ch.getWindowEnd()] for ch in channels]
 
     visibles = [ch.isActive() for ch in channels]
     names = [ch.getLabel() for ch in channels]
 
     scale = None
     # Setting z-scale causes issues with Z-slider.
     # See https://github.com/tlambert03/napari-omero/pull/15
     # if image.getSizeZ() > 1:
     #     size_x = image.getPixelSizeX()
     #     size_z = image.getPixelSizeZ()
     #     if size_x is not None and size_z is not None:
     #         scale = [1, size_z / size_x, 1, 1]
 
     return {
-        'channel_axis': 1,
-        'colormap': colors,
-        'contrast_limits': contrast_limits,
-        'name': names,
-        'visible': visibles,
-        'scale': scale,
+        "channel_axis": 1,
+        "colormap": colors,
+        "contrast_limits": contrast_limits,
+        "name": names,
+        "visible": visibles,
+        "scale": scale,
     }
 
 
-@timer
+# @timer
 def get_data_lazy(image: ImageWrapper) -> da.Array:
     """Get 5D dask array, with delayed reading from OMERO image."""
-    nt, nc, nz, ny, nx = [getattr(image, f'getSize{x}')() for x in 'TCZYX']
+    nt, nc, nz, ny, nx = (getattr(image, f"getSize{x}")() for x in "TCZYX")
     pixels = image.getPrimaryPixels()
     dtype = PIXEL_TYPES.get(pixels.getPixelsType().value, None)
     get_plane = delayed(timer(lambda idx: pixels.getPlane(*idx)))
 
-    def get_lazy_plane(zct):
+    def get_lazy_plane(zct: tuple[int, ...]):
         return da.from_delayed(get_plane(zct), shape=(ny, nx), dtype=dtype)
 
     # 5D stack: TCZXY
     t_stacks = []
     for t in range(nt):
         c_stacks = []
         for c in range(nc):
```

### Comparing `napari_omero-0.2.0/src/napari_omero/plugins/masks.py` & `napari_omero-0.2.1/src/napari_omero/plugins/masks.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         roi.addShape(shape)
     # Save the ROI (saves any linked shapes too)
     return updateService.saveAndReturnObject(roi)
 
 
 def save_labels(layer, image: ImageWrapper) -> List[RoiI]:
     """
-    Saves masks from a 5D image (no C dimension)
+    Saves masks from a 5D image (no C dimension).
 
     Each non-zero value in the labels data
     is used to create an ROI in OMERO with a
     Shape Mask created for each Z/T plane of
     the mask.
     """
     # for each label value, check if we have any masks
@@ -36,15 +36,15 @@
             rgba = [round(r * 255) for r in rgba]
             rgba[3] = layer.opacity * 256
             rois.append(save_label(masks_4d == v, image, rgba))
     return rois
 
 
 def save_label(bool_4d: np.ndarray, image: ImageWrapper, rgba) -> RoiI:
-    """Turns a boolean array of shape (t, z, y, x) into OMERO Roi"""
+    """Turns a boolean array of shape (t, z, y, x) into OMERO Roi."""
     size_t = bool_4d.shape[0]
     size_z = bool_4d.shape[1]
     # Create an ROI with a shape for each Z/T that has some mask
     mask_shapes = []
     for z in range(0, size_z):
         for t in range(0, size_t):
             masks_2d = bool_4d[t][z]
```

### Comparing `napari_omero-0.2.0/src/napari_omero/plugins/omero.py` & `napari_omero-0.2.1/src/napari_omero/plugins/omero.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from functools import wraps
 
 import napari
 import numpy
-import omero.clients  # noqa
+import omero.clients
 from napari.layers.labels.labels import Labels as labels_layer
 from napari.layers.points.points import Points as points_layer
 from napari.layers.shapes.shapes import Shapes as shapes_layer
 from omero.cli import CLI, BaseControl, ProxyStringType
 from omero.gateway import BlitzGateway, PixelsWrapper
 from omero.model import (
     EllipseI,
@@ -49,15 +49,14 @@
                 self.gateway = None
                 self.client = None
 
     return _wrapper
 
 
 class NapariControl(BaseControl):
-
     gateway = None
     client = None
 
     def _configure(self, parser):
         parser.add_login_arguments()
         sub = parser.sub()
         view = parser.add(sub, self.view, VIEW_HELP)
@@ -72,55 +71,52 @@
                 "Use eager loading to load all planes immediately instead"
                 "of lazy-loading each plane when needed"
             ),
         )
 
     @gateway_required
     def view(self, args):
-
         if isinstance(args.object, ImageI):
             try:
                 img = lookup_obj(self.gateway, args.object)
             except NameError:
                 self.ctx.die(110, f"No such {type}: {args.object.id}")
 
             self.ctx.out(f"View image: {img.name}")
 
-            viewer = napari.Viewer()
+            viewer = napari.Viewer()  # type: ignore
 
             add_buttons(viewer, img)
 
             viewer.open(
-                f'omero://{obj_to_proxy_string(args.object)}',
+                f"omero://{obj_to_proxy_string(args.object)}",
                 plugin="napari-omero",
             )
             set_dims_defaults(viewer, img)
             set_dims_labels(viewer, img)
 
             # add 'conn' and 'omero_image' to the viewer console
             viewer.update_console({"conn": self.gateway, "omero_image": img})
-            napari.run()
+            napari.run()  # type: ignore
 
 
 def add_buttons(viewer, img):
-    """
-    Add custom buttons to the viewer UI
-    """
+    """Add custom buttons to the viewer UI."""
 
     def handle_save_rois():
         save_rois(viewer, img)
 
     button = QPushButton("Save ROIs to OMERO")
     button.clicked.connect(handle_save_rois)
     viewer.window.add_dock_widget(button, name="Save OMERO", area="left")
 
 
 def get_data(img, c=0):
     """
-    Get 4D numpy array of pixel data, shape = (size_t, size_z, size_y, size_x)
+    Get 4D numpy array of pixel data, shape = (size_t, size_z, size_y, size_x).
 
     :param  img:        omero.gateway.ImageWrapper
     :c      int:        Channel index
     """
     size_z = img.getSizeZ()
     size_t = img.getSizeT()
     # get all planes we need in a single generator
@@ -134,30 +130,30 @@
         t_stacks.append(numpy.array(z_stack))
     return numpy.array(t_stacks)
 
 
 def set_dims_labels(viewer, image):
     """
     Set labels on napari viewer dims, based on
-    dimensions of OMERO image
+    dimensions of OMERO image.
 
     :param  viewer:     napari viewer instance
     :param  image:      omero.gateway.ImageWrapper
     """
     # dims (t, z, y, x) for 5D image
     dims = "TZ"
 
     for idx, label in enumerate(dims):
         viewer.dims.set_axis_label(idx, label)
 
 
 def set_dims_defaults(viewer, image):
     """
     Set Z/T slider index on napari viewer, according
-    to default Z/T indecies of the OMERO image
+    to default Z/T indecies of the OMERO image.
 
     :param  viewer:     napari viewer instance
     :param  image:      omero.gateway.ImageWrapper
     """
     # dims (t, z, y, x) for 5D image
     if image.getSizeT() > 1:
         viewer.dims.set_point(0, image.getDefaultT())
@@ -165,32 +161,30 @@
         viewer.dims.set_point(1, image.getDefaultZ())
 
 
 def save_rois(viewer, image):
     """
     Usage: In napari, open console...
     >>> from napari_omero import *
-    >>> save_rois(viewer, omero_image)
+    >>> save_rois(viewer, omero_image).
     """
     conn = image._conn
 
     for layer in viewer.layers:
         if type(layer) == points_layer:
             for p in layer.data:
                 point = create_omero_point(p)
                 roi = create_roi(conn, image.id, [point])
                 print(f"Created ROI: {roi.id.val}")
         elif type(layer) == shapes_layer:
             if len(layer.data) == 0 or len(layer.shape_type) == 0:
                 continue
             shape_types = layer.shape_type
             if isinstance(shape_types, str):
-                shape_types = [
-                    layer.shape_type for _ in range(len(layer.data))
-                ]
+                shape_types = [layer.shape_type for _ in range(len(layer.data))]
             for shape_type, data in zip(shape_types, layer.data):
                 shape = create_omero_shape(shape_type, data)
                 if shape is not None:
                     roi = create_roi(conn, image.id, [shape])
                     print(f"Created ROI: {roi.id.val}")
         elif type(layer) == labels_layer:
             print("Saving Labels...")
@@ -258,16 +252,16 @@
                 shape.x = rdouble(x1)
                 shape.y = rdouble(y1)
                 shape.width = rdouble(x3 - x1)
                 shape.height = rdouble(y2 - y1)
             else:
                 # Rotated Rectangle - save as Polygon
                 shape = PolygonI()
-                points = f"{x1},{y1}, {x2},{y2}, {x3},{y3}, {x4},{y4}"
-                shape.points = rstring(points)
+                points_str = f"{x1},{y1}, {x2},{y2}, {x3},{y3}, {x4},{y4}"
+                shape.points = rstring(points_str)
         elif shape_type == "ellipse":
             # Ellipse not rotated (ignore floating point rouding)
             if int(x1) == int(x2):
                 shape = EllipseI()
                 shape.x = rdouble((x1 + x3) / 2)
                 shape.y = rdouble((y1 + y2) / 2)
                 shape.radiusX = rdouble(abs(x3 - x1) / 2)
@@ -292,15 +286,15 @@
 
 
 class NonCachedPixelsWrapper(PixelsWrapper):
     """Extend gateway.PixelWrapper to override _prepareRawPixelsStore."""
 
     def _prepareRawPixelsStore(self):
         """
-        Creates RawPixelsStore and sets the id etc
+        Creates RawPixelsStore and sets the id etc.
 
         This overrides the superclass behaviour to make sure that
         we don't re-use RawPixelStore in multiple processes since
         the Store may be closed in 1 process while still needed elsewhere.
         This is needed when napari requests may planes simultaneously,
         e.g. when switching to 3D view.
         """
```

### Comparing `napari_omero-0.2.0/src/napari_omero/utils.py` & `napari_omero-0.2.1/src/napari_omero/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,57 +27,56 @@
     ProxyStringType("Image"),
     ProxyStringType("Dataset"),
     ProxyStringType("Project"),
 )
 
 
 def timer(func):
-    """Print the runtime of the decorated function"""
+    """Print the runtime of the decorated function."""
 
     @functools.wraps(func)
     def wrapper_timer(*args, **kwargs):
         start_time = time.perf_counter()  # 1
         value = func(*args, **kwargs)
         end_time = time.perf_counter()  # 2
         run_time = end_time - start_time  # 3
         logger.debug(f"Finished {func.__name__!r} in {run_time:.4f} secs")
         return value
 
     return wrapper_timer
 
 
-@timer
+# @timer
 def lookup_obj(conn: BlitzGateway, iobj: IObject) -> BlitzObjectWrapper:
     """Find object of type by ID."""
     conn.SERVICE_OPTS.setOmeroGroup("-1")
     type_ = iobj.__class__.__name__.rstrip("I")
     obj = conn.getObject(type_, iobj.id)
     if not obj:
         raise NameError(f"No such {type_}: {iobj.id}")
 
     return obj
 
 
 omero_url_pattern = re.compile(
-    r"https?://(?P<host>[^/]+).*/webclient"
-    r"/\?show=(?P<type>[a-z]+)-(?P<id>[0-9]+)"
+    r"https?://(?P<host>[^/]+).*/webclient" r"/\?show=(?P<type>[a-z]+)-(?P<id>[0-9]+)"
 )
 
 omero_object_pattern = re.compile(
     r"(?P<protocol>omero://)?(?P<type>(Image|Dataset|Project)):(?P<id>[0-9]+)"
 )
 
 
 def parse_omero_url(url: str) -> Optional[Dict[str, str]]:
     match = omero_url_pattern.search(url)
     return match.groupdict() if match else None
 
 
 def get_proxy_obj(path: str) -> Optional[IObject]:
-    """If path ends with e.g. Image:ID return proxy obj"""
+    """If path ends with e.g. Image:ID return proxy obj."""
     if path.startswith("omero://"):
         path = path[8:]
     match = omero_object_pattern.search(path)
     if match is None:
         return None
     d = match.groupdict()
     _path = f'{d["type"]}:{d["id"]}'
```

### Comparing `napari_omero-0.2.0/src/napari_omero/widgets/gateway.py` & `napari_omero-0.2.1/src/napari_omero/widgets/gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     _user: Optional[str] = None
 
     def __init__(self, parent=None):
         super().__init__(parent)
         self.store = SessionsStore()
         self.destroyed.connect(self.close)
         atexit.register(self.close)
-        self.worker: Optional['WorkerBase'] = None
-        self._next_worker: Optional['WorkerBase'] = None
+        self.worker: Optional["WorkerBase"] = None
+        self._next_worker: Optional["WorkerBase"] = None
 
     @property
     def conn(self):
         return QGateWay._conn
 
     @conn.setter
     def conn(self, val):
@@ -94,17 +94,15 @@
         if self._next_worker is not None:
             self.worker = self._next_worker
             self._next_worker = None
             self.worker.start()
         else:
             self.worker = None
 
-    def _submit(
-        self, func: Callable, *args, _wait=True, **kwargs
-    ) -> 'WorkerBase':
+    def _submit(self, func: Callable, *args, _wait=True, **kwargs) -> "WorkerBase":
         from napari.qt.threading import create_worker
 
         new_worker = create_worker(func, *args, _start_thread=False, **kwargs)
         new_worker.finished.connect(self._start_next_worker)
 
         if self.worker and self.worker.is_running:
             self._next_worker = new_worker
@@ -129,32 +127,26 @@
                 session = self.store.attach(host, username, uuid)
                 return self._on_new_session(session)
             except Exception as e:
                 self.status.emit("Error")
                 self.error.emit(e)
         return None
 
-    def create_session(
-        self, host: str, port: str, username: str, password: str
-    ):
-        return self._submit(
-            self._create_session, host, port, username, password
-        )
-
-    def _create_session(
-        self, host: str, port: str, username: str, password: str
-    ):
+    def create_session(self, host: str, port: str, username: str, password: str):
+        return self._submit(self._create_session, host, port, username, password)
+
+    def _create_session(self, host: str, port: str, username: str, password: str):
         self.status.emit("connecting...")
         try:
             props = {
                 "omero.host": host,
                 "omero.user": username,
             }
             if port:
-                props['omero.port'] = port
+                props["omero.port"] = port
             session = self.store.create(username, password, props)
             return self._on_new_session(session)
         except Exception as e:
             self.status.emit("Error")
             self.error.emit(e)
 
     def _on_new_session(self, session: SessionStats):
@@ -179,15 +171,15 @@
 
 
 class NonCachedPixelsWrapper(PixelsWrapper):
     """Extend gateway.PixelWrapper to override _prepareRawPixelsStore."""
 
     def _prepareRawPixelsStore(self):
         """
-        Creates RawPixelsStore and sets the id etc
+        Creates RawPixelsStore and sets the id etc.
 
         This overrides the superclass behaviour to make sure that
         we don't re-use RawPixelStore in multiple processes since
         the Store may be closed in 1 process while still needed elsewhere.
         This is needed when napari requests may planes simultaneously,
         e.g. when switching to 3D view.
         """
```

### Comparing `napari_omero-0.2.0/src/napari_omero/widgets/login.py` & `napari_omero-0.2.1/src/napari_omero/widgets/login.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     def __init__(self, gateway: QGateWay, parent=None):
         super().__init__(parent)
         self.gateway = gateway
         self.setup_ui()
         self.gateway.status.connect(self.status.setText)
         self.gateway.error.connect(self._on_gateway_error)
         self.gateway.connected.connect(self.hide)
+        self.gateway.disconnected.connect(self.show)
         self.gateway.try_restore_session()
 
     def setup_ui(self):
         self.host = QLineEdit(self)
         self.host.setMinimumWidth(170)
         self.port = QLineEdit(self)
         self.port.setValidator(QIntValidator(0, 99999, self))
```

### Comparing `napari_omero-0.2.0/src/napari_omero/widgets/main.py` & `napari_omero-0.2.1/src/napari_omero/widgets/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,58 +2,62 @@
 from qtpy.QtCore import (
     QCoreApplication,
     QItemSelection,
     QItemSelectionModel,
     QModelIndex,
     Qt,
 )
-from qtpy.QtWidgets import QLabel, QSplitter, QTreeView, QVBoxLayout, QWidget
+from qtpy.QtWidgets import (
+    QLabel,
+    QPushButton,
+    QSplitter,
+    QTreeView,
+    QVBoxLayout,
+    QWidget,
+)
 
 from .gateway import QGateWay
 from .login import LoginForm
 from .thumb_grid import ThumbGrid
 from .tree_model import OMEROTreeModel
 
 
 class OMEROWidget(QWidget):
     def __init__(self):
         super().__init__()
         self.gateway = QGateWay(self)
         self.tree = QTreeView(self)
         self.tree.setHeaderHidden(True)
         # self.tree.setSelectionMode(QTreeView.MultiSelection)
-        self.model = OMEROTreeModel(self.gateway, self)
         self.thumb_grid = ThumbGrid(self.gateway, self)
         self.thumb_grid.hide()
         self.login = LoginForm(self.gateway, self)
         self.login.setWindowFlags(self.login.windowFlags() & ~Qt.Dialog)
 
-        self.tree.setModel(self.model)
-        self.tree.selectionModel().selectionChanged.connect(
-            self._on_tree_selection
-        )
-        self.thumb_grid.itemSelectionChanged.connect(
-            self._on_thumbnail_selected
-        )
+        self._setup_tree()
+
+        self.thumb_grid.itemSelectionChanged.connect(self._on_thumbnail_selected)
         layout = QVBoxLayout(self)
         self.splitter = QSplitter(Qt.Vertical, self)
         self.status = QLabel(self)
         self.status.hide()
         self.status.setAlignment(Qt.AlignCenter)
         self.status.setStyleSheet("QLabel{color: #AAA;}")
+        self.disconnect_button = QPushButton("Disconnect")
+        self.disconnect_button.hide()
+
         layout.addWidget(self.status)
         layout.addWidget(self.splitter)
+
         self.splitter.addWidget(self.login)
         self.splitter.addWidget(self.tree)
         self.splitter.addWidget(self.thumb_grid)
-        self.gateway.connected.connect(self._show_connection_label)
-
-    def _show_connection_label(self):
-        self.status.setText(f"{self.gateway._user}@{self.gateway._host}")
-        self.status.show()
+        self.splitter.addWidget(self.disconnect_button)
+        self.gateway.connected.connect(self._on_connect)
+        self.disconnect_button.clicked.connect(self._on_disconnect)
 
     @property
     def viewer(self):
         from napari.utils._magicgui import find_viewer_ancestor
 
         return find_viewer_ancestor(self)
 
@@ -65,17 +69,38 @@
         if index:
             self.tree.selectionModel().select(
                 index,
                 QItemSelectionModel.ClearAndSelect | QItemSelectionModel.Rows,
             )
         self.load_image(wrapper)
 
-    def _on_tree_selection(
-        self, selected: QItemSelection, deselected: QItemSelection
-    ):
+    def _setup_tree(self):
+        """Set up QTreeView with a fresh tree model."""
+        self.model = OMEROTreeModel(self.gateway, self)
+        self.tree.setModel(self.model)
+        self.tree.selectionModel().selectionChanged.connect(self._on_tree_selection)
+
+    def _on_disconnect(self):
+        """Hide project widgets (tree, thumb grid) and disconnect button."""
+        self.status.setText("Not connected")
+        self.gateway.close()
+        self.disconnect_button.hide()
+        self.tree.hide()
+        self.thumb_grid.hide()
+
+        self._setup_tree()
+
+    def _on_connect(self):
+        """Show project tree and disconnect button."""
+        self.status.setText(f"{self.gateway._user}@{self.gateway._host}")
+        self.status.show()
+        self.tree.show()
+        self.disconnect_button.show()
+
+    def _on_tree_selection(self, selected: QItemSelection, deselected: QItemSelection):
         item = self.model.itemFromIndex(selected.indexes()[0])
         self.thumb_grid.set_item(item)
 
         if item.isImage():
             QCoreApplication.processEvents()
             self.load_image(item.wrapper)
```

### Comparing `napari_omero-0.2.0/src/napari_omero/widgets/thumb_grid.py` & `napari_omero-0.2.1/src/napari_omero/widgets/thumb_grid.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,35 +41,34 @@
         if dataset:
             self.set_dataset(dataset)
             self.show()
         if item.isImage():
             self.select_image()
 
     def select_image(self):
-        wrapper = self._current_item.wrapper
-        item = self._item_map.get(wrapper.getId())
-        if item:
-            self.setCurrentItem(item)
+        if self._current_item is not None:
+            wrapper = self._current_item.wrapper
+            item = self._item_map.get(wrapper.getId())
+            if item:
+                self.setCurrentItem(item)
 
     def set_dataset(self, item):
         if not self.gateway.isConnected():
             return
 
         if item == self._current_dataset:
             return
 
         self._current_dataset = item
 
         def yield_thumbs(conn):
             self.clear()
             self._item_map.clear()
             for img in item.wrapper.listChildren():
-                for byte in conn.getThumbnailSet(
-                    [img.getId()], THUMBSIZE
-                ).values():
+                for byte in conn.getThumbnailSet([img.getId()], THUMBSIZE).values():
                     yield byte, img
 
         return self.gateway._submit(
             yield_thumbs,
             self.gateway.conn,
             _wait=False,
             _connect={"yielded": self.add_thumb_bytes},
@@ -78,15 +77,17 @@
     def add_thumb_bytes(self, result):
         bytes_, wrapper = result
         img = QImage()
         img.loadFromData(bytes_)
         icon = QIcon(QPixmap.fromImage(img))
         name = wrapper.getName()
         if len(name) > 18:
-            name = name[:15] + "..."
+            name = f"{name[:15]}..."
         item = QListWidgetItem(icon, name)
-        item.setTextAlignment(Qt.AlignHCenter | Qt.AlignBottom)
+        item.setTextAlignment(
+            Qt.AlignmentFlag.AlignHCenter | Qt.AlignmentFlag.AlignBottom
+        )
         item.wrapper = wrapper
         self._item_map[wrapper.getId()] = item
         self.addItem(item)
-        if self._current_item.isImage():
+        if self._current_item is not None and self._current_item.isImage():
             self.select_image()
```

### Comparing `napari_omero-0.2.0/src/napari_omero/widgets/tree_model.py` & `napari_omero-0.2.1/src/napari_omero/widgets/tree_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,40 +21,40 @@
         return not self._has_fetched and self.hasChildren()
 
     def yieldChildren(self):
         yield from self.wrapper._conn.getObjects(
             self.child_type,
             opts={
                 self.wrapper_type.lower(): self.wrapper.id,
-                'order_by': 'obj.name',
+                "order_by": "obj.name",
             },
         )
 
     def hasChildren(self) -> bool:
         return bool(self.child_type and self.n_children > 0)
 
     @property
     def child_type(self) -> Optional[str]:
-        kls = self.wrapper.CHILD_WRAPPER_CLASS or ''
+        kls = self.wrapper.CHILD_WRAPPER_CLASS or ""
         kls = kls if isinstance(kls, str) else kls.__name__
         return kls.lstrip("_").replace("Wrapper", "") if kls else None
 
     @property
     def wrapper_type(self) -> str:
         return self.wrapper.OMERO_CLASS
 
     @property
     def parent_type(self) -> Optional[str]:
-        kls = self.wrapper.PARENT_WRAPPER_CLASS or ''
+        kls = self.wrapper.PARENT_WRAPPER_CLASS or ""
         kls = kls if isinstance(kls, str) else kls.__name__
         return kls.lstrip("_").replace("Wrapper", "") if kls else None
 
     @property
     def n_children(self) -> int:
-        if not hasattr(self, '_n_children'):
+        if not hasattr(self, "_n_children"):
             self._n_children = self.wrapper.countChildren()
         return self._n_children
 
     def isDataset(self) -> bool:
         return isinstance(self.wrapper, _DatasetWrapper)
 
     def isImage(self) -> bool:
@@ -63,25 +63,23 @@
 
 class OMEROTreeModel(QStandardItemModel):
     def __init__(self, gateway: QGateWay, parent=None):
         super().__init__(parent)
         self.gateway = gateway
         self.gateway.connected.connect(
             lambda g: self.gateway._submit(
-                self._get_projects, _connect={'returned': self._add_projects}
+                self._get_projects, _connect={"returned": self._add_projects}
             )
         )
         self._wrapper_map: Dict[BlitzObjectWrapper, QModelIndex] = {}
 
     def _get_projects(self):
         root = self.invisibleRootItem()
-        root.appendRow(QStandardItem('loading...'))
-        return self.gateway.getObjects(
-            "Project", opts={'order_by': 'obj.name'}
-        )
+        root.appendRow(QStandardItem("loading..."))
+        return self.gateway.getObjects("Project", opts={"order_by": "obj.name"})
 
     def _add_projects(self, projects):
         root = self.invisibleRootItem()
         root.removeRow(0)
         for project in projects:
             item = OMEROTreeItem(project)
             root.appendRow(item)
```

### Comparing `napari_omero-0.2.0/src/omero/plugins/napari.py` & `napari_omero-0.2.1/src/omero/plugins/napari.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 # Copyright (C) 2019 University of Dundee & Open Microscopy Environment.
 # All rights reserved.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 2 of the License, or
```


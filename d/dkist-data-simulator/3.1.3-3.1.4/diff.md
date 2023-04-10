# Comparing `tmp/dkist_data_simulator-3.1.3.tar.gz` & `tmp/dkist_data_simulator-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_data_simulator-3.1.3.tar", last modified: Tue Mar  7 15:47:54 2023, max compression
+gzip compressed data, was "dkist_data_simulator-3.1.4.tar", last modified: Mon Apr 10 19:27:20 2023, max compression
```

## Comparing `dkist_data_simulator-3.1.3.tar` & `dkist_data_simulator-3.1.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-07 15:47:54.260866 dkist_data_simulator-3.1.3/
--rw-rw-rw-   0 root         (0) root         (0)     3308 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     4986 2023-03-07 15:47:54.260866 dkist_data_simulator-3.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4650 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      651 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-07 15:47:54.256866 dkist_data_simulator-3.1.3/dkist_data_simulator/
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-07 15:47:54.256866 dkist_data_simulator-3.1.3/dkist_data_simulator/data/
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/data/README.rst
--rw-rw-rw-   0 root         (0) root         (0)    16806 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/dataset.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-07 15:47:54.256866 dkist_data_simulator-3.1.3/dkist_data_simulator/examples/
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3370 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/examples/vtf_crisp_5d.py
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/expansions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    10932 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/schemas.py
--rw-rw-rw-   0 root         (0) root         (0)     7180 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/spec122.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-07 15:47:54.256866 dkist_data_simulator-3.1.3/dkist_data_simulator/spec214/
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/spec214/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26675 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/spec214/core.py
--rw-rw-rw-   0 root         (0) root         (0)    11480 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/spec214/cryo.py
--rw-rw-rw-   0 root         (0) root         (0)     3446 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/spec214/dlnirsp.py
--rw-rw-rw-   0 root         (0) root         (0)     7627 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/spec214/vbi.py
--rw-rw-rw-   0 root         (0) root         (0)     6602 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/spec214/visp.py
--rw-rw-rw-   0 root         (0) root         (0)     3585 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/spec214/vtf.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-07 15:47:54.260866 dkist_data_simulator-3.1.3/dkist_data_simulator/tests/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1012 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/tests/test_122.py
--rw-rw-rw-   0 root         (0) root         (0)     8380 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/tests/test_214.py
--rw-rw-rw-   0 root         (0) root         (0)     4450 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/tests/test_214_inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     5458 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/tests/test_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2689 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/util.py
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-03-07 15:47:54.000000 dkist_data_simulator-3.1.3/dkist_data_simulator/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-07 15:47:54.256866 dkist_data_simulator-3.1.3/dkist_data_simulator.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4986 2023-03-07 15:47:54.000000 dkist_data_simulator-3.1.3/dkist_data_simulator.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1429 2023-03-07 15:47:54.000000 dkist_data_simulator-3.1.3/dkist_data_simulator.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-07 15:47:54.000000 dkist_data_simulator-3.1.3/dkist_data_simulator.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-07 15:47:54.000000 dkist_data_simulator-3.1.3/dkist_data_simulator.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      242 2023-03-07 15:47:54.000000 dkist_data_simulator-3.1.3/dkist_data_simulator.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-03-07 15:47:54.000000 dkist_data_simulator-3.1.3/dkist_data_simulator.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-07 15:47:54.260866 dkist_data_simulator-3.1.3/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     2618 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/docs/make.bat
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-07 15:47:54.260866 dkist_data_simulator-3.1.3/examples/
--rwxrwxrwx   0 root         (0) root         (0)      908 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/examples/vtf_crisp_5d.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-07 15:47:54.260866 dkist_data_simulator-3.1.3/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/licenses/TEMPLATE_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2656 2023-03-07 15:47:54.260866 dkist_data_simulator-3.1.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      607 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1315 2023-03-07 15:47:27.000000 dkist_data_simulator-3.1.3/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.480412 dkist_data_simulator-3.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)     3308 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     4986 2023-04-10 19:27:20.480412 dkist_data_simulator-3.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4650 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      651 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.476412 dkist_data_simulator-3.1.4/dkist_data_simulator/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.476412 dkist_data_simulator-3.1.4/dkist_data_simulator/data/
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/data/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)    16806 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/dataset.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.476412 dkist_data_simulator-3.1.4/dkist_data_simulator/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3370 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/examples/vtf_crisp_5d.py
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/expansions.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    10932 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)     7180 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/spec122.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.476412 dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26874 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    11480 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/cryo.py
+-rw-rw-rw-   0 root         (0) root         (0)     3446 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/dlnirsp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7627 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/vbi.py
+-rw-rw-rw-   0 root         (0) root         (0)     6602 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/visp.py
+-rw-rw-rw-   0 root         (0) root         (0)     3585 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/vtf.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.480412 dkist_data_simulator-3.1.4/dkist_data_simulator/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/tests/test_122.py
+-rw-rw-rw-   0 root         (0) root         (0)     8380 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/tests/test_214.py
+-rw-rw-rw-   0 root         (0) root         (0)     4450 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/tests/test_214_inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5458 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/tests/test_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2689 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/util.py
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-04-10 19:27:20.000000 dkist_data_simulator-3.1.4/dkist_data_simulator/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.476412 dkist_data_simulator-3.1.4/dkist_data_simulator.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4986 2023-04-10 19:27:20.000000 dkist_data_simulator-3.1.4/dkist_data_simulator.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1429 2023-04-10 19:27:20.000000 dkist_data_simulator-3.1.4/dkist_data_simulator.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-10 19:27:20.000000 dkist_data_simulator-3.1.4/dkist_data_simulator.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-10 19:27:20.000000 dkist_data_simulator-3.1.4/dkist_data_simulator.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      242 2023-04-10 19:27:20.000000 dkist_data_simulator-3.1.4/dkist_data_simulator.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-10 19:27:20.000000 dkist_data_simulator-3.1.4/dkist_data_simulator.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.480412 dkist_data_simulator-3.1.4/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     2618 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/docs/make.bat
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.480412 dkist_data_simulator-3.1.4/examples/
+-rwxrwxrwx   0 root         (0) root         (0)      908 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/examples/vtf_crisp_5d.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 19:27:20.480412 dkist_data_simulator-3.1.4/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2656 2023-04-10 19:27:20.480412 dkist_data_simulator-3.1.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      607 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1315 2023-04-10 19:26:58.000000 dkist_data_simulator-3.1.4/tox.ini
```

### Comparing `dkist_data_simulator-3.1.3/.gitignore` & `dkist_data_simulator-3.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/.pre-commit-config.yaml` & `dkist_data_simulator-3.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/PKG-INFO` & `dkist_data_simulator-3.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_data_simulator
-Version: 3.1.3
+Version: 3.1.4
 Summary: A header generator and FITS file creator for DKIST data.
 Home-page: 
 Author: AURA / NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.9
 Provides-Extra: all
```

### Comparing `dkist_data_simulator-3.1.3/README.rst` & `dkist_data_simulator-3.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/bitbucket-pipelines.yml` & `dkist_data_simulator-3.1.4/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/dkist_data_simulator/dataset.py` & `dkist_data_simulator-3.1.4/dkist_data_simulator/dataset.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/dkist_data_simulator/examples/vtf_crisp_5d.py` & `dkist_data_simulator-3.1.4/dkist_data_simulator/examples/vtf_crisp_5d.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/dkist_data_simulator/expansions.py` & `dkist_data_simulator-3.1.4/dkist_data_simulator/expansions.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/dkist_data_simulator/schemas.py` & `dkist_data_simulator-3.1.4/dkist_data_simulator/schemas.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/dkist_data_simulator/spec122.py` & `dkist_data_simulator-3.1.4/dkist_data_simulator/spec122.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/dkist_data_simulator/spec214/core.py` & `dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,18 @@
         self.add_constant_key("WKFLVERS", "WORKFLOWVERSION")
         self.add_constant_key("HLSVERS", "HLSVERSION")
         self.add_constant_key("IDSPARID", 1)
         self.add_constant_key("IDSOBSID", 2)
         self.add_constant_key("IDSCALID", 3)
         self.add_constant_key("OBSPR_ID", "OPID")
         self.add_constant_key("IP_ID", "IPID")
+        self.add_constant_key("NSPECLNS", 3)
+        self.add_constant_key("SPECLN01", "Ca II")
+        self.add_constant_key("SPECLN02", "H alpha")
+        self.add_constant_key("SPECLN03", "Fe I")
         self.add_constant_key("HEADVERS", "HEADERVERSION")
         self.add_constant_key("HEAD_URL", "HEADERURL")
         self.add_constant_key("INFO_URL", "INFOURL")
         self.add_constant_key("CAL_URL", "CALURL")
 
         hashids = Hashids()
         dsetid = hashids.encode(self.random.integers(0, 1000000))
```

### Comparing `dkist_data_simulator-3.1.3/dkist_data_simulator/spec214/cryo.py` & `dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/cryo.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/dkist_data_simulator/spec214/dlnirsp.py` & `dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/dlnirsp.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/dkist_data_simulator/spec214/vbi.py` & `dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/vbi.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/dkist_data_simulator/spec214/visp.py` & `dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/visp.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/dkist_data_simulator/spec214/vtf.py` & `dkist_data_simulator-3.1.4/dkist_data_simulator/spec214/vtf.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/dkist_data_simulator/tests/conftest.py` & `dkist_data_simulator-3.1.4/dkist_data_simulator/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/dkist_data_simulator/tests/test_122.py` & `dkist_data_simulator-3.1.4/dkist_data_simulator/tests/test_122.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/dkist_data_simulator/tests/test_214.py` & `dkist_data_simulator-3.1.4/dkist_data_simulator/tests/test_214.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/dkist_data_simulator/tests/test_214_inventory.py` & `dkist_data_simulator-3.1.4/dkist_data_simulator/tests/test_214_inventory.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/dkist_data_simulator/tests/test_dataset.py` & `dkist_data_simulator-3.1.4/dkist_data_simulator/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/dkist_data_simulator/util.py` & `dkist_data_simulator-3.1.4/dkist_data_simulator/util.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/dkist_data_simulator.egg-info/PKG-INFO` & `dkist_data_simulator-3.1.4/dkist_data_simulator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-data-simulator
-Version: 3.1.3
+Version: 3.1.4
 Summary: A header generator and FITS file creator for DKIST data.
 Home-page: 
 Author: AURA / NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.9
 Provides-Extra: all
```

### Comparing `dkist_data_simulator-3.1.3/dkist_data_simulator.egg-info/SOURCES.txt` & `dkist_data_simulator-3.1.4/dkist_data_simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/docs/Makefile` & `dkist_data_simulator-3.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/docs/conf.py` & `dkist_data_simulator-3.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/docs/make.bat` & `dkist_data_simulator-3.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/examples/vtf_crisp_5d.py` & `dkist_data_simulator-3.1.4/examples/vtf_crisp_5d.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/licenses/LICENSE.rst` & `dkist_data_simulator-3.1.4/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/licenses/TEMPLATE_LICENSE.rst` & `dkist_data_simulator-3.1.4/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/setup.cfg` & `dkist_data_simulator-3.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/setup.py` & `dkist_data_simulator-3.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `dkist_data_simulator-3.1.3/tox.ini` & `dkist_data_simulator-3.1.4/tox.ini`

 * *Files identical despite different names*


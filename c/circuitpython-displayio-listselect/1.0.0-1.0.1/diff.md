# Comparing `tmp/circuitpython-displayio-listselect-1.0.0.tar.gz` & `tmp/circuitpython-displayio-listselect-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-displayio-listselect-1.0.0.tar", last modified: Mon Apr 10 14:57:17 2023, max compression
+gzip compressed data, was "circuitpython-displayio-listselect-1.0.1.tar", last modified: Mon Apr 10 15:15:51 2023, max compression
```

## Comparing `circuitpython-displayio-listselect-1.0.0.tar` & `circuitpython-displayio-listselect-1.0.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:57:17.285776 circuitpython-displayio-listselect-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:57:17.281776 circuitpython-displayio-listselect-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:57:17.281776 circuitpython-displayio-listselect-1.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:57:17.285776 circuitpython-displayio-listselect-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:57:17.285776 circuitpython-displayio-listselect-1.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-10 14:57:17.285776 circuitpython-displayio-listselect-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:57:17.285776 circuitpython-displayio-listselect-1.0.0/circuitpython_displayio_listselect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-10 14:57:17.000000 circuitpython-displayio-listselect-1.0.0/circuitpython_displayio_listselect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-10 14:57:17.000000 circuitpython-displayio-listselect-1.0.0/circuitpython_displayio_listselect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 14:57:17.000000 circuitpython-displayio-listselect-1.0.0/circuitpython_displayio_listselect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-10 14:57:17.000000 circuitpython-displayio-listselect-1.0.0/circuitpython_displayio_listselect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-10 14:57:17.000000 circuitpython-displayio-listselect-1.0.0/circuitpython_displayio_listselect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-04-10 14:57:09.000000 circuitpython-displayio-listselect-1.0.0/displayio_listselect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:57:17.285776 circuitpython-displayio-listselect-1.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:57:17.285776 circuitpython-displayio-listselect-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:57:17.285776 circuitpython-displayio-listselect-1.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-10 14:57:09.000000 circuitpython-displayio-listselect-1.0.0/examples/displayio_listselect_funhouse_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-10 14:57:09.000000 circuitpython-displayio-listselect-1.0.0/examples/displayio_listselect_joystick.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-10 14:57:09.000000 circuitpython-displayio-listselect-1.0.0/examples/displayio_listselect_pygamedisplay_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-10 14:57:09.000000 circuitpython-displayio-listselect-1.0.0/examples/displayio_listselect_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-10 14:57:09.000000 circuitpython-displayio-listselect-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-10 14:56:57.000000 circuitpython-displayio-listselect-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 14:57:17.285776 circuitpython-displayio-listselect-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:15:51.649086 circuitpython-displayio-listselect-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:15:51.641086 circuitpython-displayio-listselect-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:15:51.645086 circuitpython-displayio-listselect-1.0.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:15:51.645086 circuitpython-displayio-listselect-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:15:51.645086 circuitpython-displayio-listselect-1.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-04-10 15:15:51.649086 circuitpython-displayio-listselect-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:15:51.649086 circuitpython-displayio-listselect-1.0.1/circuitpython_displayio_listselect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-04-10 15:15:51.000000 circuitpython-displayio-listselect-1.0.1/circuitpython_displayio_listselect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-10 15:15:51.000000 circuitpython-displayio-listselect-1.0.1/circuitpython_displayio_listselect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:15:51.000000 circuitpython-displayio-listselect-1.0.1/circuitpython_displayio_listselect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-10 15:15:51.000000 circuitpython-displayio-listselect-1.0.1/circuitpython_displayio_listselect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-10 15:15:51.000000 circuitpython-displayio-listselect-1.0.1/circuitpython_displayio_listselect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-04-10 15:15:41.000000 circuitpython-displayio-listselect-1.0.1/displayio_listselect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:15:51.649086 circuitpython-displayio-listselect-1.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:15:51.649086 circuitpython-displayio-listselect-1.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:15:51.649086 circuitpython-displayio-listselect-1.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-10 15:15:41.000000 circuitpython-displayio-listselect-1.0.1/examples/displayio_listselect_funhouse_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-10 15:15:41.000000 circuitpython-displayio-listselect-1.0.1/examples/displayio_listselect_joystick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-10 15:15:41.000000 circuitpython-displayio-listselect-1.0.1/examples/displayio_listselect_pygamedisplay_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-10 15:15:41.000000 circuitpython-displayio-listselect-1.0.1/examples/displayio_listselect_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-10 15:15:41.000000 circuitpython-displayio-listselect-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-10 15:15:27.000000 circuitpython-displayio-listselect-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:15:51.649086 circuitpython-displayio-listselect-1.0.1/setup.cfg
```

### Comparing `circuitpython-displayio-listselect-1.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-displayio-listselect-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-displayio-listselect-1.0.0/.github/workflows/release_gh.yml` & `circuitpython-displayio-listselect-1.0.1/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-displayio-listselect-1.0.0/.gitignore` & `circuitpython-displayio-listselect-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-displayio-listselect-1.0.0/.pre-commit-config.yaml` & `circuitpython-displayio-listselect-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-displayio-listselect-1.0.0/.pylintrc` & `circuitpython-displayio-listselect-1.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-displayio-listselect-1.0.0/CODE_OF_CONDUCT.md` & `circuitpython-displayio-listselect-1.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-displayio-listselect-1.0.0/LICENSE` & `circuitpython-displayio-listselect-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-displayio-listselect-1.0.0/LICENSES/CC-BY-4.0.txt` & `circuitpython-displayio-listselect-1.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-displayio-listselect-1.0.0/LICENSES/MIT.txt` & `circuitpython-displayio-listselect-1.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-displayio-listselect-1.0.0/LICENSES/Unlicense.txt` & `circuitpython-displayio-listselect-1.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-displayio-listselect-1.0.0/PKG-INFO` & `circuitpython-displayio-listselect-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-displayio-listselect
-Version: 1.0.0
+Version: 1.0.1
 Summary: ListSelect widget for circuitpython displayio. Display a list of strings with a selection indicator allow user to move selection up and down.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/foamyguy/CircuitPython_DisplayIO_ListSelect
 Keywords: adafruit,blinka,circuitpython,micropython,displayio_listselect,list,select,listselect,dropdown,choice,choose,chooser,options,menu
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -110,18 +110,16 @@
 .. code-block:: python
 
     import time
     import displayio
     import board
     from displayio_listselect import ListSelect
 
-    # Make the display context. Change size if you want
     display = board.DISPLAY
 
-    # Make the display context
     main_group = displayio.Group()
     display.show(main_group)
 
     items = ["First", "Second", "Third", "Fourth"]
 
     list_select = ListSelect(scale=2, items=items)
```

### Comparing `circuitpython-displayio-listselect-1.0.0/README.rst` & `circuitpython-displayio-listselect-1.0.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -92,18 +92,16 @@
 .. code-block:: python
 
     import time
     import displayio
     import board
     from displayio_listselect import ListSelect
 
-    # Make the display context. Change size if you want
     display = board.DISPLAY
 
-    # Make the display context
     main_group = displayio.Group()
     display.show(main_group)
 
     items = ["First", "Second", "Third", "Fourth"]
 
     list_select = ListSelect(scale=2, items=items)
```

### Comparing `circuitpython-displayio-listselect-1.0.0/circuitpython_displayio_listselect.egg-info/PKG-INFO` & `circuitpython-displayio-listselect-1.0.1/circuitpython_displayio_listselect.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-displayio-listselect
-Version: 1.0.0
+Version: 1.0.1
 Summary: ListSelect widget for circuitpython displayio. Display a list of strings with a selection indicator allow user to move selection up and down.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/foamyguy/CircuitPython_DisplayIO_ListSelect
 Keywords: adafruit,blinka,circuitpython,micropython,displayio_listselect,list,select,listselect,dropdown,choice,choose,chooser,options,menu
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -110,18 +110,16 @@
 .. code-block:: python
 
     import time
     import displayio
     import board
     from displayio_listselect import ListSelect
 
-    # Make the display context. Change size if you want
     display = board.DISPLAY
 
-    # Make the display context
     main_group = displayio.Group()
     display.show(main_group)
 
     items = ["First", "Second", "Third", "Fourth"]
 
     list_select = ListSelect(scale=2, items=items)
```

### Comparing `circuitpython-displayio-listselect-1.0.0/circuitpython_displayio_listselect.egg-info/SOURCES.txt` & `circuitpython-displayio-listselect-1.0.1/circuitpython_displayio_listselect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-displayio-listselect-1.0.0/displayio_listselect.py` & `circuitpython-displayio-listselect-1.0.1/displayio_listselect.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 """
 
 import terminalio
 from adafruit_display_text.bitmap_label import Label
 from displayio import Group
 
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __repo__ = "https://github.com/foamyguy/CircuitPython_DisplayIO_ListSelect.git"
 
 
 class ListSelect(Group):
     """
     ListSelect widget for CircuitPython DisplayIO.
     Display a list of strings with a selection indicator allow
```

### Comparing `circuitpython-displayio-listselect-1.0.0/docs/_static/favicon.ico` & `circuitpython-displayio-listselect-1.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-displayio-listselect-1.0.0/docs/conf.py` & `circuitpython-displayio-listselect-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-displayio-listselect-1.0.0/docs/index.rst` & `circuitpython-displayio-listselect-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-displayio-listselect-1.0.0/examples/displayio_listselect_funhouse_test.py` & `circuitpython-displayio-listselect-1.0.1/examples/displayio_listselect_funhouse_test.py`

 * *Files identical despite different names*

### Comparing `circuitpython-displayio-listselect-1.0.0/examples/displayio_listselect_joystick.py` & `circuitpython-displayio-listselect-1.0.1/examples/displayio_listselect_joystick.py`

 * *Files identical despite different names*

### Comparing `circuitpython-displayio-listselect-1.0.0/examples/displayio_listselect_pygamedisplay_simpletest.py` & `circuitpython-displayio-listselect-1.0.1/examples/displayio_listselect_pygamedisplay_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-displayio-listselect-1.0.0/examples/displayio_listselect_simpletest.py` & `circuitpython-displayio-listselect-1.0.1/examples/displayio_listselect_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-displayio-listselect-1.0.0/pyproject.toml` & `circuitpython-displayio-listselect-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-displayio-listselect"
 description = "ListSelect widget for circuitpython displayio. Display a list of strings with a selection indicator allow user to move selection up and down."
-version = "1.0.0"
+version = "1.0.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/foamyguy/CircuitPython_DisplayIO_ListSelect"}
 keywords = [
     "adafruit",
```


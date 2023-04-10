# Comparing `tmp/adafruit-circuitpython-wii-classic-1.0.0.tar.gz` & `tmp/adafruit-circuitpython-wii-classic-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-wii-classic-1.0.0.tar", last modified: Tue Apr  4 20:55:29 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-wii-classic-1.0.1.tar", last modified: Mon Apr 10 14:22:39 2023, max compression
```

## Comparing `adafruit-circuitpython-wii-classic-1.0.0.tar` & `adafruit-circuitpython-wii-classic-1.0.1.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:55:29.879840 adafruit-circuitpython-wii-classic-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:55:29.871840 adafruit-circuitpython-wii-classic-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:55:29.875840 adafruit-circuitpython-wii-classic-1.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:55:29.875840 adafruit-circuitpython-wii-classic-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:55:29.875840 adafruit-circuitpython-wii-classic-1.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-04 20:55:29.875840 adafruit-circuitpython-wii-classic-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:55:29.875840 adafruit-circuitpython-wii-classic-1.0.0/adafruit_circuitpython_wii_classic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-04 20:55:29.000000 adafruit-circuitpython-wii-classic-1.0.0/adafruit_circuitpython_wii_classic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-04 20:55:29.000000 adafruit-circuitpython-wii-classic-1.0.0/adafruit_circuitpython_wii_classic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 20:55:29.000000 adafruit-circuitpython-wii-classic-1.0.0/adafruit_circuitpython_wii_classic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-04 20:55:29.000000 adafruit-circuitpython-wii-classic-1.0.0/adafruit_circuitpython_wii_classic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-04 20:55:29.000000 adafruit-circuitpython-wii-classic-1.0.0/adafruit_circuitpython_wii_classic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-04 20:55:22.000000 adafruit-circuitpython-wii-classic-1.0.0/adafruit_wii_classic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:55:29.875840 adafruit-circuitpython-wii-classic-1.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:55:29.875840 adafruit-circuitpython-wii-classic-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:55:29.875840 adafruit-circuitpython-wii-classic-1.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-04 20:55:22.000000 adafruit-circuitpython-wii-classic-1.0.0/examples/wii_classic_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-04 20:55:22.000000 adafruit-circuitpython-wii-classic-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-04 20:55:12.000000 adafruit-circuitpython-wii-classic-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 20:55:29.879840 adafruit-circuitpython-wii-classic-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:22:39.295741 adafruit-circuitpython-wii-classic-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:22:39.291741 adafruit-circuitpython-wii-classic-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:22:39.291741 adafruit-circuitpython-wii-classic-1.0.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:22:39.295741 adafruit-circuitpython-wii-classic-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:22:39.295741 adafruit-circuitpython-wii-classic-1.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-10 14:22:39.295741 adafruit-circuitpython-wii-classic-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:22:39.295741 adafruit-circuitpython-wii-classic-1.0.1/adafruit_circuitpython_wii_classic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-10 14:22:39.000000 adafruit-circuitpython-wii-classic-1.0.1/adafruit_circuitpython_wii_classic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-10 14:22:39.000000 adafruit-circuitpython-wii-classic-1.0.1/adafruit_circuitpython_wii_classic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 14:22:39.000000 adafruit-circuitpython-wii-classic-1.0.1/adafruit_circuitpython_wii_classic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-10 14:22:39.000000 adafruit-circuitpython-wii-classic-1.0.1/adafruit_circuitpython_wii_classic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-10 14:22:39.000000 adafruit-circuitpython-wii-classic-1.0.1/adafruit_circuitpython_wii_classic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-10 14:22:30.000000 adafruit-circuitpython-wii-classic-1.0.1/adafruit_wii_classic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:22:39.295741 adafruit-circuitpython-wii-classic-1.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:22:39.295741 adafruit-circuitpython-wii-classic-1.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:22:39.295741 adafruit-circuitpython-wii-classic-1.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    77052 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/examples/wii_classic.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/examples/wii_classic.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-04-10 14:22:30.000000 adafruit-circuitpython-wii-classic-1.0.1/examples/wii_classic_displayio_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-10 14:22:30.000000 adafruit-circuitpython-wii-classic-1.0.1/examples/wii_classic_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-10 14:22:30.000000 adafruit-circuitpython-wii-classic-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 14:22:39.295741 adafruit-circuitpython-wii-classic-1.0.1/setup.cfg
```

### Comparing `adafruit-circuitpython-wii-classic-1.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-wii-classic-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.0/.gitignore` & `adafruit-circuitpython-wii-classic-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.0/.pre-commit-config.yaml` & `adafruit-circuitpython-wii-classic-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.0/.pylintrc` & `adafruit-circuitpython-wii-classic-1.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-wii-classic-1.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.0/LICENSE` & `adafruit-circuitpython-wii-classic-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-wii-classic-1.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.0/LICENSES/MIT.txt` & `adafruit-circuitpython-wii-classic-1.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-wii-classic-1.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.0/PKG-INFO` & `adafruit-circuitpython-wii-classic-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wii-classic
-Version: 1.0.0
+Version: 1.0.1
 Summary: CircuitPython library for Nintendo Wii Classic controllers.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wii_Classic
 Keywords: adafruit,blinka,circuitpython,micropython,wii_classic,wii,classic,remote,control
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -119,26 +119,26 @@
 
 	i2c = board.STEMMA_I2C()
 	ctrl_pad = adafruit_wii_classic.Wii_Classic(i2c)
 
 	while True:
 		left_x, left_y = ctrl_pad.joystick_l
 		right_x, right_y = ctrl_pad.joystick_r
-		left_pressure = ctrl_pad.l_shoulder
-		right_pressure = ctrl_pad.r_shoulder
+		left_pressure = ctrl_pad.l_shoulder.LEFT_FORCE
+		right_pressure = ctrl_pad.r_shoulder.RIGHT_FORCE
 		print("joystick_l = {},{}".format(left_x, left_y))
 		print("joystick_r = {},{}".format(right_X, left_y))
 		print("left shoulder = {}".format(left_pressure))
 		print("right shoulder = {}".format(right_pressure))
 		if ctrl_pad.buttons.A:
 			print("button A")
 		if ctrl_pad.buttons.B:
 			print("button B")
 		if ctrl_pad.d_pad.UP:
-			print("button Up")
+			print("d_pad Up")
 		time.sleep(0.5)
 
 Documentation
 =============
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/wii_classic/en/latest/>`_.
 
 For information on building library documentation, please check out
```

### Comparing `adafruit-circuitpython-wii-classic-1.0.0/README.rst` & `adafruit-circuitpython-wii-classic-1.0.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -101,26 +101,26 @@
 
 	i2c = board.STEMMA_I2C()
 	ctrl_pad = adafruit_wii_classic.Wii_Classic(i2c)
 
 	while True:
 		left_x, left_y = ctrl_pad.joystick_l
 		right_x, right_y = ctrl_pad.joystick_r
-		left_pressure = ctrl_pad.l_shoulder
-		right_pressure = ctrl_pad.r_shoulder
+		left_pressure = ctrl_pad.l_shoulder.LEFT_FORCE
+		right_pressure = ctrl_pad.r_shoulder.RIGHT_FORCE
 		print("joystick_l = {},{}".format(left_x, left_y))
 		print("joystick_r = {},{}".format(right_X, left_y))
 		print("left shoulder = {}".format(left_pressure))
 		print("right shoulder = {}".format(right_pressure))
 		if ctrl_pad.buttons.A:
 			print("button A")
 		if ctrl_pad.buttons.B:
 			print("button B")
 		if ctrl_pad.d_pad.UP:
-			print("button Up")
+			print("d_pad Up")
 		time.sleep(0.5)
 
 Documentation
 =============
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/wii_classic/en/latest/>`_.
 
 For information on building library documentation, please check out
```

### Comparing `adafruit-circuitpython-wii-classic-1.0.0/adafruit_circuitpython_wii_classic.egg-info/PKG-INFO` & `adafruit-circuitpython-wii-classic-1.0.1/adafruit_circuitpython_wii_classic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wii-classic
-Version: 1.0.0
+Version: 1.0.1
 Summary: CircuitPython library for Nintendo Wii Classic controllers.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wii_Classic
 Keywords: adafruit,blinka,circuitpython,micropython,wii_classic,wii,classic,remote,control
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -119,26 +119,26 @@
 
 	i2c = board.STEMMA_I2C()
 	ctrl_pad = adafruit_wii_classic.Wii_Classic(i2c)
 
 	while True:
 		left_x, left_y = ctrl_pad.joystick_l
 		right_x, right_y = ctrl_pad.joystick_r
-		left_pressure = ctrl_pad.l_shoulder
-		right_pressure = ctrl_pad.r_shoulder
+		left_pressure = ctrl_pad.l_shoulder.LEFT_FORCE
+		right_pressure = ctrl_pad.r_shoulder.RIGHT_FORCE
 		print("joystick_l = {},{}".format(left_x, left_y))
 		print("joystick_r = {},{}".format(right_X, left_y))
 		print("left shoulder = {}".format(left_pressure))
 		print("right shoulder = {}".format(right_pressure))
 		if ctrl_pad.buttons.A:
 			print("button A")
 		if ctrl_pad.buttons.B:
 			print("button B")
 		if ctrl_pad.d_pad.UP:
-			print("button Up")
+			print("d_pad Up")
 		time.sleep(0.5)
 
 Documentation
 =============
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/wii_classic/en/latest/>`_.
 
 For information on building library documentation, please check out
```

### Comparing `adafruit-circuitpython-wii-classic-1.0.0/adafruit_circuitpython_wii_classic.egg-info/SOURCES.txt` & `adafruit-circuitpython-wii-classic-1.0.1/adafruit_circuitpython_wii_classic.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -29,8 +29,11 @@
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
+examples/wii_classic.bmp
+examples/wii_classic.bmp.license
+examples/wii_classic_displayio_visualizer.py
 examples/wii_classic_simpletest.py
```

### Comparing `adafruit-circuitpython-wii-classic-1.0.0/adafruit_wii_classic.py` & `adafruit-circuitpython-wii-classic-1.0.1/adafruit_wii_classic.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 try:
     import typing  # pylint: disable=unused-import
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Wii_Classic.git"
 
 _I2C_INIT_DELAY = 0.1
 
 
 class Wii_Classic:
     """Class which provides interface to Nintendo Wii Classic controller.
```

### Comparing `adafruit-circuitpython-wii-classic-1.0.0/docs/_static/favicon.ico` & `adafruit-circuitpython-wii-classic-1.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.0/docs/conf.py` & `adafruit-circuitpython-wii-classic-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.0/docs/index.rst` & `adafruit-circuitpython-wii-classic-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.0/pyproject.toml` & `adafruit-circuitpython-wii-classic-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-wii-classic"
 description = "CircuitPython library for Nintendo Wii Classic controllers."
-version = "1.0.0"
+version = "1.0.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Wii_Classic"}
 keywords = [
     "adafruit",
```


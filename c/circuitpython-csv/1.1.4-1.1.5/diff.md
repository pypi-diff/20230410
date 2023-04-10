# Comparing `tmp/circuitpython-csv-1.1.4.tar.gz` & `tmp/circuitpython-csv-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-csv-1.1.4.tar", last modified: Fri Feb 17 17:30:30 2023, max compression
+gzip compressed data, was "circuitpython-csv-1.1.5.tar", last modified: Mon Apr 10 16:54:04 2023, max compression
```

## Comparing `circuitpython-csv-1.1.4.tar` & `circuitpython-csv-1.1.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 17:30:30.452414 circuitpython-csv-1.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 17:30:30.448414 circuitpython-csv-1.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 17:30:30.448414 circuitpython-csv-1.1.4/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 17:30:30.448414 circuitpython-csv-1.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20709 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 17:30:30.448414 circuitpython-csv-1.1.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/LICENSES/0BSD.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/LICENSES/PSF-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-02-17 17:30:30.452414 circuitpython-csv-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 17:30:30.448414 circuitpython-csv-1.1.4/circuitpython_csv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-02-17 17:30:30.000000 circuitpython-csv-1.1.4/circuitpython_csv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-02-17 17:30:30.000000 circuitpython-csv-1.1.4/circuitpython_csv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 17:30:30.000000 circuitpython-csv-1.1.4/circuitpython_csv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 17:30:30.000000 circuitpython-csv-1.1.4/circuitpython_csv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-17 17:30:30.000000 circuitpython-csv-1.1.4/circuitpython_csv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-02-17 17:30:19.000000 circuitpython-csv-1.1.4/circuitpython_csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 17:30:30.452414 circuitpython-csv-1.1.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 17:30:30.452414 circuitpython-csv-1.1.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 17:30:30.452414 circuitpython-csv-1.1.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-02-17 17:30:19.000000 circuitpython-csv-1.1.4/examples/csv_dictwritertest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-02-17 17:30:19.000000 circuitpython-csv-1.1.4/examples/csv_disklogger.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-02-17 17:30:19.000000 circuitpython-csv-1.1.4/examples/csv_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-02-17 17:30:19.000000 circuitpython-csv-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-17 17:29:58.000000 circuitpython-csv-1.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 17:30:30.452414 circuitpython-csv-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:54:04.890569 circuitpython-csv-1.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:54:04.886569 circuitpython-csv-1.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:54:04.886569 circuitpython-csv-1.1.5/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:54:04.886569 circuitpython-csv-1.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20709 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:54:04.890569 circuitpython-csv-1.1.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/LICENSES/0BSD.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/LICENSES/PSF-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-04-10 16:54:04.890569 circuitpython-csv-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:54:04.890569 circuitpython-csv-1.1.5/circuitpython_csv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-04-10 16:54:04.000000 circuitpython-csv-1.1.5/circuitpython_csv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-10 16:54:04.000000 circuitpython-csv-1.1.5/circuitpython_csv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:54:04.000000 circuitpython-csv-1.1.5/circuitpython_csv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 16:54:04.000000 circuitpython-csv-1.1.5/circuitpython_csv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 16:54:04.000000 circuitpython-csv-1.1.5/circuitpython_csv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-04-10 16:53:56.000000 circuitpython-csv-1.1.5/circuitpython_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:54:04.890569 circuitpython-csv-1.1.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:54:04.890569 circuitpython-csv-1.1.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:54:04.890569 circuitpython-csv-1.1.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-10 16:53:56.000000 circuitpython-csv-1.1.5/examples/csv_dictwritertest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-10 16:53:56.000000 circuitpython-csv-1.1.5/examples/csv_disklogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-10 16:53:56.000000 circuitpython-csv-1.1.5/examples/csv_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-10 16:53:56.000000 circuitpython-csv-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-10 16:53:46.000000 circuitpython-csv-1.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 16:54:04.890569 circuitpython-csv-1.1.5/setup.cfg
```

### Comparing `circuitpython-csv-1.1.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-csv-1.1.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-csv-1.1.4/.pre-commit-config.yaml` & `circuitpython-csv-1.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-csv-1.1.4/.pylintrc` & `circuitpython-csv-1.1.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-csv-1.1.4/CODE_OF_CONDUCT.md` & `circuitpython-csv-1.1.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-csv-1.1.4/LICENSE` & `circuitpython-csv-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-csv-1.1.4/LICENSES/0BSD.txt` & `circuitpython-csv-1.1.5/LICENSES/0BSD.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-csv-1.1.4/LICENSES/CC-BY-4.0.txt` & `circuitpython-csv-1.1.5/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-csv-1.1.4/LICENSES/MIT.txt` & `circuitpython-csv-1.1.5/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-csv-1.1.4/LICENSES/PSF-2.0.txt` & `circuitpython-csv-1.1.5/LICENSES/PSF-2.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-csv-1.1.4/LICENSES/Unlicense.txt` & `circuitpython-csv-1.1.5/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-csv-1.1.4/PKG-INFO` & `circuitpython-csv-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-csv
-Version: 1.1.4
+Version: 1.1.5
 Summary: CircuitPython helper library for working with CSV files
 Author-email: Alec Delaney <tekktrik@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/tekktrik/CircuitPython_CSV
 Keywords: adafruit,csv,data,files,embedded,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -56,15 +56,15 @@
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
 * `MicroPython's regular expression library (re) <https://circuitpython.readthedocs.io/en/latest/docs/library/re.html>`_
 
-You can find which Adafruit boards have the re library `here <https://circuitpython.readthedocs.io/en/latest/shared-bindings/support_matrix.html>`_
+You can find which Adafruit boards have the ``re`` library `here <https://circuitpython.readthedocs.io/en/latest/shared-bindings/support_matrix.html>`_.
 
 Please ensure all dependencies are available on the CircuitPython filesystem.
 This is easily achieved by downloading
 `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
 or individual libraries can be installed using
 `circup <https://github.com/adafruit/circup>`_.
```

### Comparing `circuitpython-csv-1.1.4/README.rst` & `circuitpython-csv-1.1.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
 * `MicroPython's regular expression library (re) <https://circuitpython.readthedocs.io/en/latest/docs/library/re.html>`_
 
-You can find which Adafruit boards have the re library `here <https://circuitpython.readthedocs.io/en/latest/shared-bindings/support_matrix.html>`_
+You can find which Adafruit boards have the ``re`` library `here <https://circuitpython.readthedocs.io/en/latest/shared-bindings/support_matrix.html>`_.
 
 Please ensure all dependencies are available on the CircuitPython filesystem.
 This is easily achieved by downloading
 `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
 or individual libraries can be installed using
 `circup <https://github.com/adafruit/circup>`_.
```

### Comparing `circuitpython-csv-1.1.4/circuitpython_csv.egg-info/PKG-INFO` & `circuitpython-csv-1.1.5/circuitpython_csv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-csv
-Version: 1.1.4
+Version: 1.1.5
 Summary: CircuitPython helper library for working with CSV files
 Author-email: Alec Delaney <tekktrik@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/tekktrik/CircuitPython_CSV
 Keywords: adafruit,csv,data,files,embedded,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -56,15 +56,15 @@
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
 * `MicroPython's regular expression library (re) <https://circuitpython.readthedocs.io/en/latest/docs/library/re.html>`_
 
-You can find which Adafruit boards have the re library `here <https://circuitpython.readthedocs.io/en/latest/shared-bindings/support_matrix.html>`_
+You can find which Adafruit boards have the ``re`` library `here <https://circuitpython.readthedocs.io/en/latest/shared-bindings/support_matrix.html>`_.
 
 Please ensure all dependencies are available on the CircuitPython filesystem.
 This is easily achieved by downloading
 `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
 or individual libraries can be installed using
 `circup <https://github.com/adafruit/circup>`_.
```

### Comparing `circuitpython-csv-1.1.4/circuitpython_csv.egg-info/SOURCES.txt` & `circuitpython-csv-1.1.5/circuitpython_csv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-csv-1.1.4/circuitpython_csv.py` & `circuitpython-csv-1.1.5/circuitpython_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
-__version__ = "1.1.4"
+__version__ = "1.1.5"
 __repo__ = "https://github.com/tekktrik/CircuitPython_CSV.git"
 
 import re
 
 try:
     from typing import List, Optional, Any, Dict, Iterable, Sequence, Tuple
     import io
```

### Comparing `circuitpython-csv-1.1.4/docs/_static/favicon.ico` & `circuitpython-csv-1.1.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-csv-1.1.4/docs/conf.py` & `circuitpython-csv-1.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-csv-1.1.4/docs/examples.rst` & `circuitpython-csv-1.1.5/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-csv-1.1.4/docs/index.rst` & `circuitpython-csv-1.1.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-csv-1.1.4/examples/csv_dictwritertest.py` & `circuitpython-csv-1.1.5/examples/csv_dictwritertest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-csv-1.1.4/examples/csv_disklogger.py` & `circuitpython-csv-1.1.5/examples/csv_disklogger.py`

 * *Files identical despite different names*

### Comparing `circuitpython-csv-1.1.4/examples/csv_simpletest.py` & `circuitpython-csv-1.1.5/examples/csv_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-csv-1.1.4/pyproject.toml` & `circuitpython-csv-1.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-csv"
 description = "CircuitPython helper library for working with CSV files"
-version = "1.1.4"
+version = "1.1.5"
 readme = "README.rst"
 authors = [
     {name = "Alec Delaney", email = "tekktrik@gmail.com"}
 ]
 urls = {Homepage = "https://github.com/tekktrik/CircuitPython_CSV"}
 keywords = [
     "adafruit",
```


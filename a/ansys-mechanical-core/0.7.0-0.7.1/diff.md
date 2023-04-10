# Comparing `tmp/ansys-mechanical-core-0.7.0.tar.gz` & `tmp/ansys-mechanical-core-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-mechanical-core-0.7.0.tar", last modified: Thu Apr  6 06:17:40 2023, max compression
+gzip compressed data, was "ansys-mechanical-core-0.7.1.tar", last modified: Mon Apr 10 12:41:59 2023, max compression
```

## Comparing `ansys-mechanical-core-0.7.0.tar` & `ansys-mechanical-core-0.7.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1089 2023-04-06 06:17:23.718088 ansys-mechanical-core-0.7.0/LICENSE
--rw-r--r--   0        0        0    11020 2023-04-06 06:17:23.718088 ansys-mechanical-core-0.7.0/README.rst
--rw-r--r--   0        0        0     3894 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1242 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/__init__.py
--rw-r--r--   0        0        0      536 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/_version.py
--rw-r--r--   0        0        0      167 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/embedding/__init__.py
--rw-r--r--   0        0        0     4811 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/embedding/app.py
--rw-r--r--   0        0        0     1392 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/embedding/config.py
--rw-r--r--   0        0        0      819 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/embedding/imports.py
--rw-r--r--   0        0        0     1344 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/embedding/initializer.py
--rw-r--r--   0        0        0     1958 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/embedding/loader.py
--rw-r--r--   0        0        0     2022 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/embedding/logging.py
--rw-r--r--   0        0        0      852 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/embedding/resolver.py
--rw-r--r--   0        0        0     1287 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/embedding/runtime.py
--rw-r--r--   0        0        0      703 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/embedding/shims.py
--rw-r--r--   0        0        0     3312 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/errors.py
--rw-r--r--   0        0        0      113 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/examples/__init__.py
--rw-r--r--   0        0        0     2992 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/examples/downloads.py
--rw-r--r--   0        0        0     5505 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/launcher.py
--rw-r--r--   0        0        0    23658 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/logging.py
--rw-r--r--   0        0        0    83310 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/mechanical.py
--rw-r--r--   0        0        0     4215 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/misc.py
--rw-r--r--   0        0        0    25079 2023-04-06 06:17:23.730090 ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/pool.py
--rw-r--r--   0        0        0    13689 1970-01-01 00:00:00.000000 ansys-mechanical-core-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-10 12:41:47.449289 ansys-mechanical-core-0.7.1/LICENSE
+-rw-r--r--   0        0        0     5456 2023-04-10 12:41:47.449289 ansys-mechanical-core-0.7.1/README.rst
+-rw-r--r--   0        0        0     3922 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1242 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/__init__.py
+-rw-r--r--   0        0        0      536 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/_version.py
+-rw-r--r--   0        0        0      167 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/__init__.py
+-rw-r--r--   0        0        0     4811 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/app.py
+-rw-r--r--   0        0        0     1392 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/config.py
+-rw-r--r--   0        0        0      819 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/imports.py
+-rw-r--r--   0        0        0     1344 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/initializer.py
+-rw-r--r--   0        0        0     1958 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/loader.py
+-rw-r--r--   0        0        0     2022 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/logging.py
+-rw-r--r--   0        0        0      852 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/resolver.py
+-rw-r--r--   0        0        0     1287 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/runtime.py
+-rw-r--r--   0        0        0      703 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/shims.py
+-rw-r--r--   0        0        0     3312 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/errors.py
+-rw-r--r--   0        0        0      113 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/examples/__init__.py
+-rw-r--r--   0        0        0     2992 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/examples/downloads.py
+-rw-r--r--   0        0        0     5505 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/launcher.py
+-rw-r--r--   0        0        0    23658 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/logging.py
+-rw-r--r--   0        0        0    83310 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/mechanical.py
+-rw-r--r--   0        0        0     4215 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/misc.py
+-rw-r--r--   0        0        0    25079 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/pool.py
+-rw-r--r--   0        0        0     8178 1970-01-01 00:00:00.000000 ansys-mechanical-core-0.7.1/PKG-INFO
```

### Comparing `ansys-mechanical-core-0.7.0/LICENSE` & `ansys-mechanical-core-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.0/pyproject.toml` & `ansys-mechanical-core-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-mechanical-core"
-version = "0.7.0"
+version = "0.7.1"
 description = "A python wrapper for Ansys Mechanical"
 readme = "README.rst"
 requires-python = ">=3.7,<4.0"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -66,14 +66,15 @@
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
     "pythreejs==2.4.2",
     "pyvista==0.38.5",
     "sphinx-autobuild==2021.3.14",
     "sphinx-autodoc-typehints==1.22",
     "sphinx-copybutton==0.5.1",
+    "sphinx_design==0.3.0",
     "sphinx-gallery==0.12.2",
     "sphinx-notfound-page==0.8.3",
     "sphinxcontrib-websupport==1.2.4",
     "sphinxemoji==0.2.0",
 ]
 
 [tool.flit.module]
```

### Comparing `ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/__init__.py` & `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/_version.py` & `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/_version.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/embedding/app.py` & `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/app.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/embedding/config.py` & `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/config.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/embedding/imports.py` & `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/imports.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/embedding/initializer.py` & `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/initializer.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/embedding/loader.py` & `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/loader.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/embedding/logging.py` & `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/logging.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/embedding/resolver.py` & `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/resolver.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/embedding/runtime.py` & `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/runtime.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/embedding/shims.py` & `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/shims.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/errors.py` & `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/examples/downloads.py` & `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/launcher.py` & `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/launcher.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/logging.py` & `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/logging.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/mechanical.py` & `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/mechanical.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/misc.py` & `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/misc.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.0/src/ansys/mechanical/core/pool.py` & `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/pool.py`

 * *Files identical despite different names*


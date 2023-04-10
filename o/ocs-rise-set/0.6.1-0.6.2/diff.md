# Comparing `tmp/ocs_rise_set-0.6.1.tar.gz` & `tmp/ocs_rise_set-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocs_rise_set-0.6.1.tar", max compression
+gzip compressed data, was "ocs_rise_set-0.6.2.tar", max compression
```

## Comparing `ocs_rise_set-0.6.1.tar` & `ocs_rise_set-0.6.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    35147 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/LICENSE
--rw-r--r--   0        0        0     2043 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/README.md
--rw-r--r--   0        0        0      702 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/__init__.py
--rw-r--r--   0        0        0     5078 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/angle.py
--rw-r--r--   0        0        0    52413 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/astrometry.py
--rw-r--r--   0        0        0     1189 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/exceptions.py
--rw-r--r--   0        0        0      745 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/logging.conf
--rw-r--r--   0        0        0    13677 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/moving_objects.py
--rw-r--r--   0        0        0     2425 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/rates.py
--rw-r--r--   0        0        0     1940 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/sky_coordinates.py
--rw-r--r--   0        0        0    27911 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/transits.py
--rw-r--r--   0        0        0     4128 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/utils.py
--rw-r--r--   0        0        0    29825 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/visibility.py
--rw-r--r--   0        0        0     2742 1970-01-01 00:00:00.000000 ocs_rise_set-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-04-10 16:54:11.102429 ocs_rise_set-0.6.2/LICENSE
+-rw-r--r--   0        0        0     2058 2023-04-10 16:54:11.102429 ocs_rise_set-0.6.2/README.md
+-rw-r--r--   0        0        0      720 2023-04-10 16:54:11.102429 ocs_rise_set-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 16:54:11.102429 ocs_rise_set-0.6.2/rise_set/__init__.py
+-rw-r--r--   0        0        0     5078 2023-04-10 16:54:11.102429 ocs_rise_set-0.6.2/rise_set/angle.py
+-rw-r--r--   0        0        0    52413 2023-04-10 16:54:11.102429 ocs_rise_set-0.6.2/rise_set/astrometry.py
+-rw-r--r--   0        0        0     1189 2023-04-10 16:54:11.102429 ocs_rise_set-0.6.2/rise_set/exceptions.py
+-rw-r--r--   0        0        0      745 2023-04-10 16:54:11.102429 ocs_rise_set-0.6.2/rise_set/logging.conf
+-rw-r--r--   0        0        0    13677 2023-04-10 16:54:11.102429 ocs_rise_set-0.6.2/rise_set/moving_objects.py
+-rw-r--r--   0        0        0     2425 2023-04-10 16:54:11.102429 ocs_rise_set-0.6.2/rise_set/rates.py
+-rw-r--r--   0        0        0     1940 2023-04-10 16:54:11.102429 ocs_rise_set-0.6.2/rise_set/sky_coordinates.py
+-rw-r--r--   0        0        0    27911 2023-04-10 16:54:11.102429 ocs_rise_set-0.6.2/rise_set/transits.py
+-rw-r--r--   0        0        0     4128 2023-04-10 16:54:11.102429 ocs_rise_set-0.6.2/rise_set/utils.py
+-rw-r--r--   0        0        0    29825 2023-04-10 16:54:11.102429 ocs_rise_set-0.6.2/rise_set/visibility.py
+-rw-r--r--   0        0        0     2808 1970-01-01 00:00:00.000000 ocs_rise_set-0.6.2/PKG-INFO
```

### Comparing `ocs_rise_set-0.6.1/LICENSE` & `ocs_rise_set-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ocs_rise_set-0.6.1/README.md` & `ocs_rise_set-0.6.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -28,10 +28,11 @@
 ## For Developers
 
 ### Running the Tests
 
 The unit tests are currently using nosetests, so there are a few tests dependencies to install. After cloning this project, from the project root and inside your virtual environment (using Poetry):
 
 ```bash
-$ poetry env use python3.9
-$ poetry run nosetests
+$ poetry env use python3.10
+$ poetry install
+$ poetry run pytest
 ```
```

### Comparing `ocs_rise_set-0.6.1/rise_set/angle.py` & `ocs_rise_set-0.6.2/rise_set/angle.py`

 * *Files identical despite different names*

### Comparing `ocs_rise_set-0.6.1/rise_set/astrometry.py` & `ocs_rise_set-0.6.2/rise_set/astrometry.py`

 * *Files identical despite different names*

### Comparing `ocs_rise_set-0.6.1/rise_set/exceptions.py` & `ocs_rise_set-0.6.2/rise_set/exceptions.py`

 * *Files identical despite different names*

### Comparing `ocs_rise_set-0.6.1/rise_set/logging.conf` & `ocs_rise_set-0.6.2/rise_set/logging.conf`

 * *Files identical despite different names*

### Comparing `ocs_rise_set-0.6.1/rise_set/moving_objects.py` & `ocs_rise_set-0.6.2/rise_set/moving_objects.py`

 * *Files identical despite different names*

### Comparing `ocs_rise_set-0.6.1/rise_set/rates.py` & `ocs_rise_set-0.6.2/rise_set/rates.py`

 * *Files identical despite different names*

### Comparing `ocs_rise_set-0.6.1/rise_set/sky_coordinates.py` & `ocs_rise_set-0.6.2/rise_set/sky_coordinates.py`

 * *Files identical despite different names*

### Comparing `ocs_rise_set-0.6.1/rise_set/transits.py` & `ocs_rise_set-0.6.2/rise_set/transits.py`

 * *Files identical despite different names*

### Comparing `ocs_rise_set-0.6.1/rise_set/utils.py` & `ocs_rise_set-0.6.2/rise_set/utils.py`

 * *Files identical despite different names*

### Comparing `ocs_rise_set-0.6.1/rise_set/visibility.py` & `ocs_rise_set-0.6.2/rise_set/visibility.py`

 * *Files identical despite different names*

### Comparing `ocs_rise_set-0.6.1/PKG-INFO` & `ocs_rise_set-0.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: ocs-rise-set
-Version: 0.6.1
+Version: 0.6.2
 Summary: Routines for accurate rise/set/transit calculations
 Author: Eric Saunders
 Author-email: esaunders@lcogt.net
-Requires-Python: >=3.7,<3.10
+Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Dist: future (>=0.18.3,<0.19.0)
 Requires-Dist: pyslalib (==1.0.6)
 Description-Content-Type: text/markdown
 
 # Rise-set Library
@@ -46,11 +47,12 @@
 ## For Developers
 
 ### Running the Tests
 
 The unit tests are currently using nosetests, so there are a few tests dependencies to install. After cloning this project, from the project root and inside your virtual environment (using Poetry):
 
 ```bash
-$ poetry env use python3.9
-$ poetry run nosetests
+$ poetry env use python3.10
+$ poetry install
+$ poetry run pytest
 ```
```


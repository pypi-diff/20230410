# Comparing `tmp/lf-0.1.8.tar.gz` & `tmp/lf-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lf-0.1.8.tar", last modified: Fri Jul 22 17:34:57 2022, max compression
+gzip compressed data, was "lf-0.1.9.tar", last modified: Mon Apr 10 20:26:03 2023, max compression
```

## Comparing `lf-0.1.8.tar` & `lf-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 drichardson42  (1000) drichardson42  (1000)        0 2022-07-22 17:34:57.572930 lf-0.1.8/
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)    35149 2022-07-22 16:44:04.000000 lf-0.1.8/LICENSE
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)       16 2022-07-22 16:44:04.000000 lf-0.1.8/MANIFEST.in
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)     1567 2022-07-22 17:34:57.568929 lf-0.1.8/PKG-INFO
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)      905 2022-07-22 16:44:04.000000 lf-0.1.8/README.md
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)       38 2022-07-22 17:34:57.572930 lf-0.1.8/setup.cfg
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)     1171 2022-07-22 17:27:45.000000 lf-0.1.8/setup.py
-drwxrwxr-x   0 drichardson42  (1000) drichardson42  (1000)        0 2022-07-22 17:34:57.564926 lf-0.1.8/src/
-drwxrwxr-x   0 drichardson42  (1000) drichardson42  (1000)        0 2022-07-22 17:34:57.568929 lf-0.1.8/src/lf/
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)      244 2022-07-22 16:44:04.000000 lf-0.1.8/src/lf/__init__.py
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)     4779 2022-07-22 16:44:04.000000 lf-0.1.8/src/lf/calibration.py
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)     1923 2022-07-22 16:44:04.000000 lf-0.1.8/src/lf/calibration_lut.py
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)     3266 2022-07-22 16:44:04.000000 lf-0.1.8/src/lf/crawler.py
-drwxrwxr-x   0 drichardson42  (1000) drichardson42  (1000)        0 2022-07-22 17:34:57.568929 lf-0.1.8/src/lf/data/
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)      100 2022-07-22 16:44:04.000000 lf-0.1.8/src/lf/data/__init__.py
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)    24208 2022-07-22 17:24:03.000000 lf-0.1.8/src/lf/data/rx.py
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)    13890 2022-07-22 16:44:04.000000 lf-0.1.8/src/lf/data/rxquality.py
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)     7379 2022-07-22 16:44:04.000000 lf-0.1.8/src/lf/data/table.py
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)     1898 2022-07-22 16:44:04.000000 lf-0.1.8/src/lf/txrx.py
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)     4296 2022-07-22 16:44:04.000000 lf-0.1.8/src/lf/utils.py
-drwxrwxr-x   0 drichardson42  (1000) drichardson42  (1000)        0 2022-07-22 17:34:57.568929 lf-0.1.8/src/lf.egg-info/
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)     1567 2022-07-22 17:34:55.000000 lf-0.1.8/src/lf.egg-info/PKG-INFO
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)      391 2022-07-22 17:34:57.000000 lf-0.1.8/src/lf.egg-info/SOURCES.txt
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)        1 2022-07-22 17:34:56.000000 lf-0.1.8/src/lf.egg-info/dependency_links.txt
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)      123 2022-07-22 17:34:57.000000 lf-0.1.8/src/lf.egg-info/requires.txt
--rw-rw-r--   0 drichardson42  (1000) drichardson42  (1000)        3 2022-07-22 17:34:57.000000 lf-0.1.8/src/lf.egg-info/top_level.txt
+drwxr-xr-x   0 drichardson42  (1000) drichardson42  (1000)        0 2023-04-10 20:26:03.687575 lf-0.1.9/
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)    35149 2023-03-06 17:20:07.000000 lf-0.1.9/LICENSE
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)       16 2023-03-06 17:20:07.000000 lf-0.1.9/MANIFEST.in
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)     1567 2023-04-10 20:26:03.686575 lf-0.1.9/PKG-INFO
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)      905 2023-03-06 17:20:07.000000 lf-0.1.9/README.md
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)       38 2023-04-10 20:26:03.687575 lf-0.1.9/setup.cfg
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)     1176 2023-04-10 20:15:48.000000 lf-0.1.9/setup.py
+drwxr-xr-x   0 drichardson42  (1000) drichardson42  (1000)        0 2023-04-10 20:26:03.574576 lf-0.1.9/src/
+drwxr-xr-x   0 drichardson42  (1000) drichardson42  (1000)        0 2023-04-10 20:26:03.648575 lf-0.1.9/src/lf/
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)      244 2023-03-06 17:20:07.000000 lf-0.1.9/src/lf/__init__.py
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)     4779 2023-03-06 17:20:07.000000 lf-0.1.9/src/lf/calibration.py
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)     1923 2023-03-06 17:20:07.000000 lf-0.1.9/src/lf/calibration_lut.py
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)     3266 2023-03-06 17:20:07.000000 lf-0.1.9/src/lf/crawler.py
+drwxr-xr-x   0 drichardson42  (1000) drichardson42  (1000)        0 2023-04-10 20:26:03.675575 lf-0.1.9/src/lf/data/
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)      100 2023-03-06 17:20:07.000000 lf-0.1.9/src/lf/data/__init__.py
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)    24208 2023-04-10 20:12:59.000000 lf-0.1.9/src/lf/data/rx.py
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)    13890 2023-03-06 17:20:07.000000 lf-0.1.9/src/lf/data/rxquality.py
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)     7379 2023-03-06 17:20:07.000000 lf-0.1.9/src/lf/data/table.py
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)     1898 2023-03-06 17:20:07.000000 lf-0.1.9/src/lf/txrx.py
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)     4296 2023-03-06 17:20:07.000000 lf-0.1.9/src/lf/utils.py
+drwxr-xr-x   0 drichardson42  (1000) drichardson42  (1000)        0 2023-04-10 20:26:03.654575 lf-0.1.9/src/lf.egg-info/
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)     1567 2023-04-10 20:26:02.000000 lf-0.1.9/src/lf.egg-info/PKG-INFO
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)      391 2023-04-10 20:26:02.000000 lf-0.1.9/src/lf.egg-info/SOURCES.txt
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)        1 2023-04-10 20:26:02.000000 lf-0.1.9/src/lf.egg-info/dependency_links.txt
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)      128 2023-04-10 20:26:02.000000 lf-0.1.9/src/lf.egg-info/requires.txt
+-rw-r--r--   0 drichardson42  (1000) drichardson42  (1000)        3 2023-04-10 20:26:02.000000 lf-0.1.9/src/lf.egg-info/top_level.txt
```

### Comparing `lf-0.1.8/LICENSE` & `lf-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lf-0.1.8/PKG-INFO` & `lf-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lf
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for interacting with GT's LF AWESOME Receiver data
 Home-page: https://github.gatech.edu/LF-Group/lfdata
 Author: David Richardson
 Author-email: drichardson42@gatech.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `lf-0.1.8/README.md` & `lf-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lf-0.1.8/setup.py` & `lf-0.1.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lf",
-    version="0.1.8",
+    version="0.1.9",
     description="Tools for interacting with GT's LF AWESOME Receiver data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="David Richardson",
     author_email="drichardson42@gatech.edu",
     url="https://github.gatech.edu/LF-Group/lfdata",
     packages=find_packages(where="src"),
@@ -21,15 +21,15 @@
         "License :: OSI Approved :: GNU General Public License v3 or later " "(GPLv3+)",
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
     ],
     install_requires=[
         "scipy",
         "numpy",
-        "sklearn",
+        "scikit-learn",
         "geographiclib",
         "pandas",
         "pysolar>=0.8",
         "matplotlib",
         "datetime",
     ],
     extras_require={
```

### Comparing `lf-0.1.8/src/lf/calibration.py` & `lf-0.1.9/src/lf/calibration.py`

 * *Files identical despite different names*

### Comparing `lf-0.1.8/src/lf/calibration_lut.py` & `lf-0.1.9/src/lf/calibration_lut.py`

 * *Files identical despite different names*

### Comparing `lf-0.1.8/src/lf/crawler.py` & `lf-0.1.9/src/lf/crawler.py`

 * *Files identical despite different names*

### Comparing `lf-0.1.8/src/lf/data/rx.py` & `lf-0.1.9/src/lf/data/rx.py`

 * *Files identical despite different names*

### Comparing `lf-0.1.8/src/lf/data/rxquality.py` & `lf-0.1.9/src/lf/data/rxquality.py`

 * *Files identical despite different names*

### Comparing `lf-0.1.8/src/lf/data/table.py` & `lf-0.1.9/src/lf/data/table.py`

 * *Files identical despite different names*

### Comparing `lf-0.1.8/src/lf/txrx.py` & `lf-0.1.9/src/lf/txrx.py`

 * *Files identical despite different names*

### Comparing `lf-0.1.8/src/lf/utils.py` & `lf-0.1.9/src/lf/utils.py`

 * *Files identical despite different names*

### Comparing `lf-0.1.8/src/lf.egg-info/PKG-INFO` & `lf-0.1.9/src/lf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lf
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for interacting with GT's LF AWESOME Receiver data
 Home-page: https://github.gatech.edu/LF-Group/lfdata
 Author: David Richardson
 Author-email: drichardson42@gatech.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```


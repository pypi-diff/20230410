# Comparing `tmp/tmart-1.3.2.tar.gz` & `tmp/tmart-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmart-1.3.2.tar", last modified: Sat Apr  8 22:51:28 2023, max compression
+gzip compressed data, was "tmart-1.3.3.tar", last modified: Mon Apr 10 04:22:56 2023, max compression
```

## Comparing `tmart-1.3.2.tar` & `tmart-1.3.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-08 22:51:28.385299 tmart-1.3.2/
--rw-r--r--   0 yw         (501) staff       (20)       45 2022-09-20 16:15:46.000000 tmart-1.3.2/MANIFEST.in
--rw-r--r--   0 yw         (501) staff       (20)     3803 2023-04-08 22:51:28.385064 tmart-1.3.2/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)     3181 2023-04-03 04:04:03.000000 tmart-1.3.2/README.md
--rw-r--r--   0 yw         (501) staff       (20)       38 2023-04-08 22:51:28.385380 tmart-1.3.2/setup.cfg
--rw-r--r--   0 yw         (501) staff       (20)     1966 2023-04-08 22:46:54.000000 tmart-1.3.2/setup.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-08 22:51:28.370787 tmart-1.3.2/tests/
--rw-r--r--   0 yw         (501) staff       (20)      246 2023-03-29 21:18:48.000000 tmart-1.3.2/tests/test_AEC.py
--rw-r--r--   0 yw         (501) staff       (20)     3048 2023-01-03 02:43:30.000000 tmart-1.3.2/tests/test_E_diffuse.py
--rw-r--r--   0 yw         (501) staff       (20)     2310 2023-01-03 03:48:03.000000 tmart-1.3.2/tests/test_L_sky.py
--rw-r--r--   0 yw         (501) staff       (20)     1827 2023-03-25 22:34:08.000000 tmart-1.3.2/tests/test_basic.py
--rw-r--r--   0 yw         (501) staff       (20)     1327 2022-09-21 16:59:26.000000 tmart-1.3.2/tests/test_basic_import.py
--rw-r--r--   0 yw         (501) staff       (20)     3197 2022-09-17 14:43:02.000000 tmart-1.3.2/tests/test_calcref.py
--rw-r--r--   0 yw         (501) staff       (20)     2993 2023-03-25 22:34:08.000000 tmart-1.3.2/tests/test_quickstart.py
--rw-r--r--   0 yw         (501) staff       (20)     3113 2022-09-26 04:25:24.000000 tmart-1.3.2/tests/test_specular_contribution.py
--rw-r--r--   0 yw         (501) staff       (20)     3228 2022-09-27 15:07:16.000000 tmart-1.3.2/tests/test_typical_ocean.py
--rw-r--r--   0 yw         (501) staff       (20)     3021 2022-10-03 05:42:50.000000 tmart-1.3.2/tests/test_whales_SR.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-08 22:51:28.372704 tmart-1.3.2/tmart/
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-08 22:51:28.373771 tmart-1.3.2/tmart/AEC/
--rw-r--r--   0 yw         (501) staff       (20)      382 2023-04-08 19:19:35.000000 tmart-1.3.2/tmart/AEC/__init__.py
--rw-r--r--   0 yw         (501) staff       (20)     5531 2023-04-08 22:45:49.000000 tmart-1.3.2/tmart/AEC/get_parameters.py
--rw-r--r--   0 yw         (501) staff       (20)     2753 2023-04-08 21:44:12.000000 tmart-1.3.2/tmart/AEC/reflectance_correction.py
--rw-r--r--   0 yw         (501) staff       (20)     2320 2023-04-08 22:49:14.000000 tmart-1.3.2/tmart/Aerosol.py
--rw-r--r--   0 yw         (501) staff       (20)    10526 2023-04-08 22:49:20.000000 tmart-1.3.2/tmart/Atmosphere.py
--rw-r--r--   0 yw         (501) staff       (20)    10104 2023-04-08 22:49:24.000000 tmart-1.3.2/tmart/Surface.py
--rw-r--r--   0 yw         (501) staff       (20)    13619 2023-04-08 22:50:39.000000 tmart-1.3.2/tmart/Tmart.py
--rw-r--r--   0 yw         (501) staff       (20)    41660 2023-04-08 22:50:38.000000 tmart-1.3.2/tmart/Tmart2.py
--rw-r--r--   0 yw         (501) staff       (20)      522 2023-04-08 22:49:15.000000 tmart-1.3.2/tmart/__init__.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-08 22:51:28.376500 tmart-1.3.2/tmart/ancillary/
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-08 22:51:28.383610 tmart-1.3.2/tmart/ancillary/aerosolSPF/
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:20:25.000000 tmart-1.3.2/tmart/ancillary/aerosolSPF/BiomassBurning.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:49:56.000000 tmart-1.3.2/tmart/ancillary/aerosolSPF/Continental.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:55:10.000000 tmart-1.3.2/tmart/ancillary/aerosolSPF/Desert.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 16:59:28.000000 tmart-1.3.2/tmart/ancillary/aerosolSPF/Maritime.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:21:44.000000 tmart-1.3.2/tmart/ancillary/aerosolSPF/Stratospheric.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:53:59.000000 tmart-1.3.2/tmart/ancillary/aerosolSPF/Urban.csv
--rw-r--r--   0 yw         (501) staff       (20)     1763 2022-12-14 22:44:42.000000 tmart-1.3.2/tmart/ancillary/conifer_forest.csv
--rw-r--r--   0 yw         (501) staff       (20)      838 2022-12-14 22:45:12.000000 tmart-1.3.2/tmart/ancillary/dry_beach_sand.csv
--rw-r--r--   0 yw         (501) staff       (20)     1618 2022-12-14 22:45:48.000000 tmart-1.3.2/tmart/ancillary/lawn_grass.csv
--rw-r--r--   0 yw         (501) staff       (20)      794 2021-08-03 20:21:41.000000 tmart-1.3.2/tmart/ancillary/soil.csv
--rw-r--r--   0 yw         (501) staff       (20)     1190 2021-08-03 20:22:22.000000 tmart-1.3.2/tmart/ancillary/vegetation.csv
--rw-r--r--   0 yw         (501) staff       (20)      284 2021-08-03 20:21:58.000000 tmart-1.3.2/tmart/ancillary/water.csv
--rw-r--r--   0 yw         (501) staff       (20)      707 2022-02-08 17:04:47.000000 tmart-1.3.2/tmart/ancillary/water_chl1.csv
--rw-r--r--   0 yw         (501) staff       (20)     1015 2022-12-14 22:46:19.000000 tmart-1.3.2/tmart/ancillary/wet_beach_sand.csv
--rw-r--r--   0 yw         (501) staff       (20)      181 2023-03-31 22:46:09.000000 tmart-1.3.2/tmart/ancillary/whitecap_factor.csv
--rw-r--r--   0 yw         (501) staff       (20)     2684 2023-04-08 22:50:41.000000 tmart-1.3.2/tmart/tm_OT.py
--rw-r--r--   0 yw         (501) staff       (20)    11784 2023-04-08 22:49:35.000000 tmart-1.3.2/tmart/tm_calcref.py
--rw-r--r--   0 yw         (501) staff       (20)     4094 2023-04-08 22:49:45.000000 tmart-1.3.2/tmart/tm_geometry.py
--rw-r--r--   0 yw         (501) staff       (20)    19399 2023-04-08 22:49:52.000000 tmart-1.3.2/tmart/tm_intersect.py
--rw-r--r--   0 yw         (501) staff       (20)    11289 2023-04-08 22:50:00.000000 tmart-1.3.2/tmart/tm_move.py
--rw-r--r--   0 yw         (501) staff       (20)     8649 2023-04-08 22:50:40.000000 tmart-1.3.2/tmart/tm_sampling.py
--rw-r--r--   0 yw         (501) staff       (20)    20018 2023-04-08 22:50:39.000000 tmart-1.3.2/tmart/tm_water.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-08 22:51:28.373372 tmart-1.3.2/tmart.egg-info/
--rw-r--r--   0 yw         (501) staff       (20)     3803 2023-04-08 22:51:28.000000 tmart-1.3.2/tmart.egg-info/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)     1275 2023-04-08 22:51:28.000000 tmart-1.3.2/tmart.egg-info/SOURCES.txt
--rw-r--r--   0 yw         (501) staff       (20)        1 2023-04-08 22:51:28.000000 tmart-1.3.2/tmart.egg-info/dependency_links.txt
--rw-r--r--   0 yw         (501) staff       (20)       50 2023-04-08 22:51:28.000000 tmart-1.3.2/tmart.egg-info/requires.txt
--rw-r--r--   0 yw         (501) staff       (20)        6 2023-04-08 22:51:28.000000 tmart-1.3.2/tmart.egg-info/top_level.txt
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-10 04:22:56.718859 tmart-1.3.3/
+-rw-r--r--   0 yw         (501) staff       (20)       45 2022-09-20 16:15:46.000000 tmart-1.3.3/MANIFEST.in
+-rw-r--r--   0 yw         (501) staff       (20)     3803 2023-04-10 04:22:56.718645 tmart-1.3.3/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)     3181 2023-04-03 04:04:03.000000 tmart-1.3.3/README.md
+-rw-r--r--   0 yw         (501) staff       (20)       38 2023-04-10 04:22:56.718929 tmart-1.3.3/setup.cfg
+-rw-r--r--   0 yw         (501) staff       (20)     1966 2023-04-10 04:22:07.000000 tmart-1.3.3/setup.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-10 04:22:56.703521 tmart-1.3.3/tests/
+-rw-r--r--   0 yw         (501) staff       (20)      246 2023-03-29 21:18:48.000000 tmart-1.3.3/tests/test_AEC.py
+-rw-r--r--   0 yw         (501) staff       (20)     3048 2023-01-03 02:43:30.000000 tmart-1.3.3/tests/test_E_diffuse.py
+-rw-r--r--   0 yw         (501) staff       (20)     2310 2023-01-03 03:48:03.000000 tmart-1.3.3/tests/test_L_sky.py
+-rw-r--r--   0 yw         (501) staff       (20)     1827 2023-03-25 22:34:08.000000 tmart-1.3.3/tests/test_basic.py
+-rw-r--r--   0 yw         (501) staff       (20)     1327 2022-09-21 16:59:26.000000 tmart-1.3.3/tests/test_basic_import.py
+-rw-r--r--   0 yw         (501) staff       (20)     3197 2022-09-17 14:43:02.000000 tmart-1.3.3/tests/test_calcref.py
+-rw-r--r--   0 yw         (501) staff       (20)     2993 2023-03-25 22:34:08.000000 tmart-1.3.3/tests/test_quickstart.py
+-rw-r--r--   0 yw         (501) staff       (20)     3113 2022-09-26 04:25:24.000000 tmart-1.3.3/tests/test_specular_contribution.py
+-rw-r--r--   0 yw         (501) staff       (20)     3228 2022-09-27 15:07:16.000000 tmart-1.3.3/tests/test_typical_ocean.py
+-rw-r--r--   0 yw         (501) staff       (20)     3021 2022-10-03 05:42:50.000000 tmart-1.3.3/tests/test_whales_SR.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-10 04:22:56.705925 tmart-1.3.3/tmart/
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-10 04:22:56.707344 tmart-1.3.3/tmart/AEC/
+-rw-r--r--   0 yw         (501) staff       (20)      382 2023-04-08 19:19:35.000000 tmart-1.3.3/tmart/AEC/__init__.py
+-rw-r--r--   0 yw         (501) staff       (20)     5614 2023-04-09 15:01:43.000000 tmart-1.3.3/tmart/AEC/get_parameters.py
+-rw-r--r--   0 yw         (501) staff       (20)     2727 2023-04-09 23:00:04.000000 tmart-1.3.3/tmart/AEC/reflectance_correction.py
+-rw-r--r--   0 yw         (501) staff       (20)     2320 2023-04-08 22:49:14.000000 tmart-1.3.3/tmart/Aerosol.py
+-rw-r--r--   0 yw         (501) staff       (20)    10526 2023-04-08 22:49:20.000000 tmart-1.3.3/tmart/Atmosphere.py
+-rw-r--r--   0 yw         (501) staff       (20)    10104 2023-04-08 22:49:24.000000 tmart-1.3.3/tmart/Surface.py
+-rw-r--r--   0 yw         (501) staff       (20)    13619 2023-04-08 22:50:39.000000 tmart-1.3.3/tmart/Tmart.py
+-rw-r--r--   0 yw         (501) staff       (20)    41660 2023-04-08 22:50:38.000000 tmart-1.3.3/tmart/Tmart2.py
+-rw-r--r--   0 yw         (501) staff       (20)      522 2023-04-08 22:49:15.000000 tmart-1.3.3/tmart/__init__.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-10 04:22:56.710465 tmart-1.3.3/tmart/ancillary/
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-10 04:22:56.717321 tmart-1.3.3/tmart/ancillary/aerosolSPF/
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:20:25.000000 tmart-1.3.3/tmart/ancillary/aerosolSPF/BiomassBurning.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:49:56.000000 tmart-1.3.3/tmart/ancillary/aerosolSPF/Continental.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:55:10.000000 tmart-1.3.3/tmart/ancillary/aerosolSPF/Desert.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 16:59:28.000000 tmart-1.3.3/tmart/ancillary/aerosolSPF/Maritime.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:21:44.000000 tmart-1.3.3/tmart/ancillary/aerosolSPF/Stratospheric.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:53:59.000000 tmart-1.3.3/tmart/ancillary/aerosolSPF/Urban.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1763 2022-12-14 22:44:42.000000 tmart-1.3.3/tmart/ancillary/conifer_forest.csv
+-rw-r--r--   0 yw         (501) staff       (20)      838 2022-12-14 22:45:12.000000 tmart-1.3.3/tmart/ancillary/dry_beach_sand.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1618 2022-12-14 22:45:48.000000 tmart-1.3.3/tmart/ancillary/lawn_grass.csv
+-rw-r--r--   0 yw         (501) staff       (20)      794 2021-08-03 20:21:41.000000 tmart-1.3.3/tmart/ancillary/soil.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1190 2021-08-03 20:22:22.000000 tmart-1.3.3/tmart/ancillary/vegetation.csv
+-rw-r--r--   0 yw         (501) staff       (20)      284 2021-08-03 20:21:58.000000 tmart-1.3.3/tmart/ancillary/water.csv
+-rw-r--r--   0 yw         (501) staff       (20)      707 2022-02-08 17:04:47.000000 tmart-1.3.3/tmart/ancillary/water_chl1.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1015 2022-12-14 22:46:19.000000 tmart-1.3.3/tmart/ancillary/wet_beach_sand.csv
+-rw-r--r--   0 yw         (501) staff       (20)      181 2023-03-31 22:46:09.000000 tmart-1.3.3/tmart/ancillary/whitecap_factor.csv
+-rw-r--r--   0 yw         (501) staff       (20)     2684 2023-04-08 22:50:41.000000 tmart-1.3.3/tmart/tm_OT.py
+-rw-r--r--   0 yw         (501) staff       (20)    11784 2023-04-08 22:49:35.000000 tmart-1.3.3/tmart/tm_calcref.py
+-rw-r--r--   0 yw         (501) staff       (20)     4094 2023-04-08 22:49:45.000000 tmart-1.3.3/tmart/tm_geometry.py
+-rw-r--r--   0 yw         (501) staff       (20)    19399 2023-04-08 22:49:52.000000 tmart-1.3.3/tmart/tm_intersect.py
+-rw-r--r--   0 yw         (501) staff       (20)    11289 2023-04-08 22:50:00.000000 tmart-1.3.3/tmart/tm_move.py
+-rw-r--r--   0 yw         (501) staff       (20)     8649 2023-04-08 22:50:40.000000 tmart-1.3.3/tmart/tm_sampling.py
+-rw-r--r--   0 yw         (501) staff       (20)    20018 2023-04-08 22:50:39.000000 tmart-1.3.3/tmart/tm_water.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-10 04:22:56.706662 tmart-1.3.3/tmart.egg-info/
+-rw-r--r--   0 yw         (501) staff       (20)     3803 2023-04-10 04:22:56.000000 tmart-1.3.3/tmart.egg-info/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)     1275 2023-04-10 04:22:56.000000 tmart-1.3.3/tmart.egg-info/SOURCES.txt
+-rw-r--r--   0 yw         (501) staff       (20)        1 2023-04-10 04:22:56.000000 tmart-1.3.3/tmart.egg-info/dependency_links.txt
+-rw-r--r--   0 yw         (501) staff       (20)       50 2023-04-10 04:22:56.000000 tmart-1.3.3/tmart.egg-info/requires.txt
+-rw-r--r--   0 yw         (501) staff       (20)        6 2023-04-10 04:22:56.000000 tmart-1.3.3/tmart.egg-info/top_level.txt
```

### Comparing `tmart-1.3.2/PKG-INFO` & `tmart-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmart
-Version: 1.3.2
+Version: 1.3.3
 Summary: Radiative transfer modelling for aquatic remote sensing
 Author: Yulun Wu
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tmart Version: 1.3.2 Summary: Radiative transfer
+Metadata-Version: 2.1 Name: tmart Version: 1.3.3 Summary: Radiative transfer
 modelling for aquatic remote sensing Author: Yulun Wu Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering ::
 Atmospheric Science Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
```

### Comparing `tmart-1.3.2/README.md` & `tmart-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/setup.py` & `tmart-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tmart",                     # This is the name of the package
-    version="1.3.2",                       
+    version="1.3.3",                       
     author="Yulun Wu",                     # Full name of the author
     description="Radiative transfer modelling for aquatic remote sensing",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     # packages=setuptools.find_packages(),    # List of all python modules to be installed
     packages = ['tmart','tmart.AEC','tmart.ancillary','tmart.ancillary.aerosolSPF'],
     include_package_data=True,
```

### Comparing `tmart-1.3.2/tests/test_E_diffuse.py` & `tmart-1.3.3/tests/test_E_diffuse.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tests/test_L_sky.py` & `tmart-1.3.3/tests/test_L_sky.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tests/test_basic.py` & `tmart-1.3.3/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tests/test_basic_import.py` & `tmart-1.3.3/tests/test_basic_import.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tests/test_calcref.py` & `tmart-1.3.3/tests/test_calcref.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tests/test_quickstart.py` & `tmart-1.3.3/tests/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tests/test_specular_contribution.py` & `tmart-1.3.3/tests/test_specular_contribution.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tests/test_typical_ocean.py` & `tmart-1.3.3/tests/test_typical_ocean.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tests/test_whales_SR.py` & `tmart-1.3.3/tests/test_whales_SR.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/AEC/get_parameters.py` & `tmart-1.3.3/tmart/AEC/get_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,34 +108,39 @@
             'F_correction': F_correction,
             'F_captured': F_captured,
             'R_atm': R['R_atm']}
 
 
 
 
-'''
+
 
 if __name__ == "__main__":
    
     import Py6S
+    import sys
+    
+    sys.path.append('/Users/yw/Desktop/tmart')
     import tmart
 
-    wl = 833
-    band = Py6S.Wavelength(Py6S.PredefinedWavelengths.S2A_MSI_08)
-    aerosol_type = 'Continental'
-    aot550 = 0.28
+    wl = 433
+    # band = Py6S.Wavelength(Py6S.PredefinedWavelengths.S2A_MSI_08)
+    aerosol_type = 'Maritime'
+    aot550 = 0.05
     
-    test = tmart.AEC.get_parameters(wl = wl, band = band,
+    test = tmart.AEC.get_parameters(wl = wl, SR_avg=1 ,n_photon = 100_000,
                                     aerosol_type = aerosol_type, aot550 = aot550,
                                     cell_size = 200,
                                     window_size=5)
     
-    print(test)
-    test2 = test['conv_window_1']
-    
+    # print(test)
+    test1 = test['conv_window_1']
+
+
+'''
 
 ### Test AEC
 
 # image_test = image_reflectance.copy()
 
 image_test = np.full((window_size_x, window_size_y), 0.39378) # unitless
```

### Comparing `tmart-1.3.2/tmart/AEC/reflectance_correction.py` & `tmart-1.3.3/tmart/AEC/reflectance_correction.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         s.atmos_profile = AtmosProfile.PredefinedType(AtmosProfile.MidlatitudeSummer)
     else: 
         s.atmos_profile = AtmosProfile.UserWaterAndOzone(atm_profile[0], atm_profile[1])
      
     # Aerosol 
     if aerosol_type == 'Maritime':
         aerosol_profile = s.aero_profile = AeroProfile.PredefinedType(AeroProfile.Maritime)
-    elif aeaerosol_type == 'Continental':
+    elif aerosol_type == 'Continental':
         aerosol_profile = s.aero_profile = AeroProfile.PredefinedType(AeroProfile.Continental)
     else:
         sys.exit('Unrecgnized aerosol type')
         
     s.aot550 = aot550
     
     s.altitudes.set_sensor_satellite_level()
@@ -83,15 +83,15 @@
     
     
     image_out = image * correction
     
     max_correction = correction.min()
     max_correction_percent = str(round((1 - max_correction)*100, 2))
     
-    print('Reflectance correction, maximum change: ' + max_correction_percent + '%')
+    print('Maximum change: ' + max_correction_percent + '%')
     
     
     return image_out
```

### Comparing `tmart-1.3.2/tmart/Aerosol.py` & `tmart-1.3.3/tmart/Aerosol.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/Atmosphere.py` & `tmart-1.3.3/tmart/Atmosphere.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/Surface.py` & `tmart-1.3.3/tmart/Surface.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/Tmart.py` & `tmart-1.3.3/tmart/Tmart.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/Tmart2.py` & `tmart-1.3.3/tmart/Tmart2.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/__init__.py` & `tmart-1.3.3/tmart/__init__.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/ancillary/aerosolSPF/BiomassBurning.csv` & `tmart-1.3.3/tmart/ancillary/aerosolSPF/BiomassBurning.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/ancillary/aerosolSPF/Continental.csv` & `tmart-1.3.3/tmart/ancillary/aerosolSPF/Continental.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/ancillary/aerosolSPF/Desert.csv` & `tmart-1.3.3/tmart/ancillary/aerosolSPF/Desert.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/ancillary/aerosolSPF/Maritime.csv` & `tmart-1.3.3/tmart/ancillary/aerosolSPF/Maritime.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/ancillary/aerosolSPF/Stratospheric.csv` & `tmart-1.3.3/tmart/ancillary/aerosolSPF/Stratospheric.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/ancillary/aerosolSPF/Urban.csv` & `tmart-1.3.3/tmart/ancillary/aerosolSPF/Urban.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/ancillary/conifer_forest.csv` & `tmart-1.3.3/tmart/ancillary/conifer_forest.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/ancillary/dry_beach_sand.csv` & `tmart-1.3.3/tmart/ancillary/dry_beach_sand.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/ancillary/lawn_grass.csv` & `tmart-1.3.3/tmart/ancillary/lawn_grass.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/ancillary/soil.csv` & `tmart-1.3.3/tmart/ancillary/soil.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/ancillary/vegetation.csv` & `tmart-1.3.3/tmart/ancillary/vegetation.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/ancillary/water_chl1.csv` & `tmart-1.3.3/tmart/ancillary/water_chl1.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/ancillary/wet_beach_sand.csv` & `tmart-1.3.3/tmart/ancillary/wet_beach_sand.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/tm_OT.py` & `tmart-1.3.3/tmart/tm_OT.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/tm_calcref.py` & `tmart-1.3.3/tmart/tm_calcref.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/tm_geometry.py` & `tmart-1.3.3/tmart/tm_geometry.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/tm_intersect.py` & `tmart-1.3.3/tmart/tm_intersect.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/tm_move.py` & `tmart-1.3.3/tmart/tm_move.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/tm_sampling.py` & `tmart-1.3.3/tmart/tm_sampling.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart/tm_water.py` & `tmart-1.3.3/tmart/tm_water.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.2/tmart.egg-info/PKG-INFO` & `tmart-1.3.3/tmart.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmart
-Version: 1.3.2
+Version: 1.3.3
 Summary: Radiative transfer modelling for aquatic remote sensing
 Author: Yulun Wu
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tmart Version: 1.3.2 Summary: Radiative transfer
+Metadata-Version: 2.1 Name: tmart Version: 1.3.3 Summary: Radiative transfer
 modelling for aquatic remote sensing Author: Yulun Wu Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering ::
 Atmospheric Science Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
```

### Comparing `tmart-1.3.2/tmart.egg-info/SOURCES.txt` & `tmart-1.3.3/tmart.egg-info/SOURCES.txt`

 * *Files identical despite different names*


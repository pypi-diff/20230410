# Comparing `tmp/voltage_imaging_analysis-0.1.6.tar.gz` & `tmp/voltage_imaging_analysis-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voltage_imaging_analysis-0.1.6.tar", last modified: Mon Apr 10 18:48:52 2023, max compression
+gzip compressed data, was "voltage_imaging_analysis-0.1.7.tar", last modified: Mon Apr 10 18:51:56 2023, max compression
```

## Comparing `voltage_imaging_analysis-0.1.6.tar` & `voltage_imaging_analysis-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:48:52.518086 voltage_imaging_analysis-0.1.6/
--rw-r--r--   0 rrsims     (501) staff       (20)     6148 2023-04-10 18:39:58.000000 voltage_imaging_analysis-0.1.6/.DS_Store
--rw-r--r--   0 rrsims     (501) staff       (20)      498 2023-04-10 18:48:52.517889 voltage_imaging_analysis-0.1.6/PKG-INFO
--rw-r--r--   0 rrsims     (501) staff       (20)      101 2023-02-07 14:38:32.000000 voltage_imaging_analysis-0.1.6/README.md
-drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:48:52.516270 voltage_imaging_analysis-0.1.6/dist/
--rw-r--r--   0 rrsims     (501) staff       (20)     9000 2023-04-10 18:40:06.000000 voltage_imaging_analysis-0.1.6/dist/voltage_imaging_analysis-0.1.0.tar.gz
--rw-r--r--   0 rrsims     (501) staff       (20)    23089 2023-04-10 18:42:27.000000 voltage_imaging_analysis-0.1.6/dist/voltage_imaging_analysis-0.1.5.tar.gz
--rw-r--r--   0 rrsims     (501) staff       (20)       38 2023-04-10 18:48:52.518139 voltage_imaging_analysis-0.1.6/setup.cfg
--rw-r--r--   0 rrsims     (501) staff       (20)      697 2023-04-10 18:48:40.000000 voltage_imaging_analysis-0.1.6/setup.py
-drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:48:52.516673 voltage_imaging_analysis-0.1.6/voltage_imaging_analysis/
--rw-r--r--   0 rrsims     (501) staff       (20)      125 2023-04-10 18:39:53.000000 voltage_imaging_analysis-0.1.6/voltage_imaging_analysis/__init__.py
-drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:48:52.517535 voltage_imaging_analysis-0.1.6/voltage_imaging_analysis/__pycache__/
--rw-r--r--   0 rrsims     (501) staff       (20)      321 2023-02-07 14:49:20.000000 voltage_imaging_analysis-0.1.6/voltage_imaging_analysis/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rrsims     (501) staff       (20)     6024 2023-04-10 18:48:11.000000 voltage_imaging_analysis-0.1.6/voltage_imaging_analysis/test_1p_analysis.py
--rw-r--r--   0 rrsims     (501) staff       (20)    29744 2023-04-10 18:48:11.000000 voltage_imaging_analysis-0.1.6/voltage_imaging_analysis/voltage_imaging_analysis_fcts.py
-drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:48:52.517375 voltage_imaging_analysis-0.1.6/voltage_imaging_analysis.egg-info/
--rw-r--r--   0 rrsims     (501) staff       (20)      498 2023-04-10 18:48:52.000000 voltage_imaging_analysis-0.1.6/voltage_imaging_analysis.egg-info/PKG-INFO
--rw-r--r--   0 rrsims     (501) staff       (20)      554 2023-04-10 18:48:52.000000 voltage_imaging_analysis-0.1.6/voltage_imaging_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 rrsims     (501) staff       (20)        1 2023-04-10 18:48:52.000000 voltage_imaging_analysis-0.1.6/voltage_imaging_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 rrsims     (501) staff       (20)        6 2023-04-10 18:48:52.000000 voltage_imaging_analysis-0.1.6/voltage_imaging_analysis.egg-info/requires.txt
--rw-r--r--   0 rrsims     (501) staff       (20)       25 2023-04-10 18:48:52.000000 voltage_imaging_analysis-0.1.6/voltage_imaging_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:51:56.126758 voltage_imaging_analysis-0.1.7/
+-rw-r--r--   0 rrsims     (501) staff       (20)     6148 2023-04-10 18:39:58.000000 voltage_imaging_analysis-0.1.7/.DS_Store
+-rw-r--r--   0 rrsims     (501) staff       (20)      498 2023-04-10 18:51:56.126564 voltage_imaging_analysis-0.1.7/PKG-INFO
+-rw-r--r--   0 rrsims     (501) staff       (20)      101 2023-02-07 14:38:32.000000 voltage_imaging_analysis-0.1.7/README.md
+drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:51:56.124503 voltage_imaging_analysis-0.1.7/dist/
+-rw-r--r--   0 rrsims     (501) staff       (20)     9000 2023-04-10 18:40:06.000000 voltage_imaging_analysis-0.1.7/dist/voltage_imaging_analysis-0.1.0.tar.gz
+-rw-r--r--   0 rrsims     (501) staff       (20)    23089 2023-04-10 18:42:27.000000 voltage_imaging_analysis-0.1.7/dist/voltage_imaging_analysis-0.1.5.tar.gz
+-rw-r--r--   0 rrsims     (501) staff       (20)    44357 2023-04-10 18:48:52.000000 voltage_imaging_analysis-0.1.7/dist/voltage_imaging_analysis-0.1.6.tar.gz
+-rw-r--r--   0 rrsims     (501) staff       (20)       38 2023-04-10 18:51:56.126810 voltage_imaging_analysis-0.1.7/setup.cfg
+-rw-r--r--   0 rrsims     (501) staff       (20)      697 2023-04-10 18:51:52.000000 voltage_imaging_analysis-0.1.7/setup.py
+drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:51:56.125333 voltage_imaging_analysis-0.1.7/voltage_imaging_analysis/
+-rw-r--r--   0 rrsims     (501) staff       (20)      125 2023-04-10 18:39:53.000000 voltage_imaging_analysis-0.1.7/voltage_imaging_analysis/__init__.py
+drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:51:56.126209 voltage_imaging_analysis-0.1.7/voltage_imaging_analysis/__pycache__/
+-rw-r--r--   0 rrsims     (501) staff       (20)      321 2023-02-07 14:49:20.000000 voltage_imaging_analysis-0.1.7/voltage_imaging_analysis/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rrsims     (501) staff       (20)     5998 2023-04-10 18:51:38.000000 voltage_imaging_analysis-0.1.7/voltage_imaging_analysis/test_1p_analysis.py
+-rw-r--r--   0 rrsims     (501) staff       (20)    29791 2023-04-10 18:51:38.000000 voltage_imaging_analysis-0.1.7/voltage_imaging_analysis/voltage_imaging_analysis_fcts.py
+drwxr-xr-x   0 rrsims     (501) staff       (20)        0 2023-04-10 18:51:56.126087 voltage_imaging_analysis-0.1.7/voltage_imaging_analysis.egg-info/
+-rw-r--r--   0 rrsims     (501) staff       (20)      498 2023-04-10 18:51:55.000000 voltage_imaging_analysis-0.1.7/voltage_imaging_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 rrsims     (501) staff       (20)      597 2023-04-10 18:51:56.000000 voltage_imaging_analysis-0.1.7/voltage_imaging_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 rrsims     (501) staff       (20)        1 2023-04-10 18:51:55.000000 voltage_imaging_analysis-0.1.7/voltage_imaging_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 rrsims     (501) staff       (20)        6 2023-04-10 18:51:55.000000 voltage_imaging_analysis-0.1.7/voltage_imaging_analysis.egg-info/requires.txt
+-rw-r--r--   0 rrsims     (501) staff       (20)       25 2023-04-10 18:51:55.000000 voltage_imaging_analysis-0.1.7/voltage_imaging_analysis.egg-info/top_level.txt
```

### Comparing `voltage_imaging_analysis-0.1.6/.DS_Store` & `voltage_imaging_analysis-0.1.7/.DS_Store`

 * *Files identical despite different names*

### Comparing `voltage_imaging_analysis-0.1.6/dist/voltage_imaging_analysis-0.1.0.tar.gz` & `voltage_imaging_analysis-0.1.7/dist/voltage_imaging_analysis-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `voltage_imaging_analysis-0.1.6/dist/voltage_imaging_analysis-0.1.5.tar.gz` & `voltage_imaging_analysis-0.1.7/dist/voltage_imaging_analysis-0.1.5.tar.gz`

 * *Files identical despite different names*

### Comparing `voltage_imaging_analysis-0.1.6/setup.py` & `voltage_imaging_analysis-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='voltage_imaging_analysis',
-    version='0.1.6',    
+    version='0.1.7',    
     description='Python package used for analysing voltage imaging data.',
     url='https://github.com/rrsims21/voltage_imaging_analysis/',
     author='Ruth Sims',
     author_email='ruth.sims@inserm.fr',
     license='BSD 2-clause',
     packages=['voltage_imaging_analysis'],
     install_requires=[
```

### Comparing `voltage_imaging_analysis-0.1.6/voltage_imaging_analysis/test_1p_analysis.py` & `voltage_imaging_analysis-0.1.7/voltage_imaging_analysis/test_1p_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from voltage_imaging_analysis import voltage_imaging_analysis_fcts as voltage_imaging_fcts
 import timeit
 import tifffile
 import scipy
 import cv2
 from matplotlib import pyplot as plt
 import skimage
-from numpy.lib.stride_tricks import as_strided
 
 blocksize_x1x2 = 10
 blocksize_x3 = 10
 
 fname = r"H:/1p_data_for_tests/1p_field_stim_no_stim_2/1p_field_stim_no_stim_2_MMStack_Pos0.ome.tif"
 
 print("Loading " + fname + "...")
@@ -62,15 +61,15 @@
 # print(np.max(S))
 
 # tifffile.imsave(r"C:/Users/photonics-voltage/Desktop/lowrank_test.tif", S.astype(np.uint16))
 
 # all_resized_S = []
 
 # for x in np.arange(S.shape[0]):
-#     all_resized_S.append(tile_array(S[x, :, :], no_tiles[1], no_tiles[2]))
+#     all_resized_S.append(voltage_imaging_fcts.tile_array(S[x, :, :], no_tiles[1], no_tiles[2]))
 
 # all_resized_S = np.array(all_resized_S)
 
 # # get rid of artefacts from "block_reduce"
 # pix_to_crop = np.array(all_resized_S.shape) - np.array(data.shape) 
 
 # all_resized_S = all_resized_S[:, :-pix_to_crop[1], :-pix_to_crop[2]]
```

### Comparing `voltage_imaging_analysis-0.1.6/voltage_imaging_analysis/voltage_imaging_analysis_fcts.py` & `voltage_imaging_analysis-0.1.7/voltage_imaging_analysis/voltage_imaging_analysis_fcts.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import skimage
 from sklearn import linear_model
 from matplotlib import pyplot as plt
 import sys
 from scipy import stats
 import statistics
 from scipy.spatial import distance
+from numpy.lib.stride_tricks import as_strided
 
 # timings analysis:
     # generate timeseries from stack 
     # segmentation
     # ... 
     # take a long time
```

### Comparing `voltage_imaging_analysis-0.1.6/voltage_imaging_analysis.egg-info/SOURCES.txt` & `voltage_imaging_analysis-0.1.7/voltage_imaging_analysis.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .DS_Store
 README.md
 setup.py
 dist/voltage_imaging_analysis-0.1.0.tar.gz
 dist/voltage_imaging_analysis-0.1.5.tar.gz
+dist/voltage_imaging_analysis-0.1.6.tar.gz
 voltage_imaging_analysis/__init__.py
 voltage_imaging_analysis/test_1p_analysis.py
 voltage_imaging_analysis/voltage_imaging_analysis_fcts.py
 voltage_imaging_analysis.egg-info/PKG-INFO
 voltage_imaging_analysis.egg-info/SOURCES.txt
 voltage_imaging_analysis.egg-info/dependency_links.txt
 voltage_imaging_analysis.egg-info/requires.txt
```


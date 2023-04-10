# Comparing `tmp/aafitrans-0.0.5.tar.gz` & `tmp/aafitrans-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aafitrans-0.0.5.tar", last modified: Mon Apr  3 12:41:33 2023, max compression
+gzip compressed data, was "aafitrans-0.0.6.tar", last modified: Mon Apr 10 17:43:39 2023, max compression
```

## Comparing `aafitrans-0.0.5.tar` & `aafitrans-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-03 12:41:33.894954 aafitrans-0.0.5/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1103 2023-04-02 07:47:45.000000 aafitrans-0.0.5/LICENSE.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1434 2023-04-03 12:41:33.893954 aafitrans-0.0.5/PKG-INFO
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)      931 2023-04-02 08:55:45.000000 aafitrans-0.0.5/README.md
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)      741 2023-04-03 06:04:32.000000 aafitrans-0.0.5/pyproject.toml
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       38 2023-04-03 12:41:33.894954 aafitrans-0.0.5/setup.cfg
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-03 12:41:33.889954 aafitrans-0.0.5/src/
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-03 12:41:33.892954 aafitrans-0.0.5/src/aafitrans/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       51 2023-04-03 06:42:21.000000 aafitrans-0.0.5/src/aafitrans/__init__.py
--rwxrwx---   0 prajwel   (1000) prajwel   (1000)    14769 2023-04-03 12:13:21.000000 aafitrans-0.0.5/src/aafitrans/aafitrans.py
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-03 12:41:33.893954 aafitrans-0.0.5/src/aafitrans.egg-info/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1434 2023-04-03 12:41:33.000000 aafitrans-0.0.5/src/aafitrans.egg-info/PKG-INFO
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)      273 2023-04-03 12:41:33.000000 aafitrans-0.0.5/src/aafitrans.egg-info/SOURCES.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)        1 2023-04-03 12:41:33.000000 aafitrans-0.0.5/src/aafitrans.egg-info/dependency_links.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       25 2023-04-03 12:41:33.000000 aafitrans-0.0.5/src/aafitrans.egg-info/requires.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       10 2023-04-03 12:41:33.000000 aafitrans-0.0.5/src/aafitrans.egg-info/top_level.txt
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-10 17:43:39.099627 aafitrans-0.0.6/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1103 2023-04-02 07:47:45.000000 aafitrans-0.0.6/LICENSE.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1434 2023-04-10 17:43:39.099627 aafitrans-0.0.6/PKG-INFO
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      931 2023-04-02 08:55:45.000000 aafitrans-0.0.6/README.md
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      741 2023-04-03 06:04:32.000000 aafitrans-0.0.6/pyproject.toml
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       38 2023-04-10 17:43:39.099627 aafitrans-0.0.6/setup.cfg
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-10 17:43:39.096627 aafitrans-0.0.6/src/
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-10 17:43:39.097627 aafitrans-0.0.6/src/aafitrans/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       51 2023-04-03 06:42:21.000000 aafitrans-0.0.6/src/aafitrans/__init__.py
+-rwxrwx---   0 prajwel   (1000) prajwel   (1000)    15508 2023-04-10 17:31:40.000000 aafitrans-0.0.6/src/aafitrans/aafitrans.py
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-10 17:43:39.098626 aafitrans-0.0.6/src/aafitrans.egg-info/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1434 2023-04-10 17:43:39.000000 aafitrans-0.0.6/src/aafitrans.egg-info/PKG-INFO
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      273 2023-04-10 17:43:39.000000 aafitrans-0.0.6/src/aafitrans.egg-info/SOURCES.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)        1 2023-04-10 17:43:39.000000 aafitrans-0.0.6/src/aafitrans.egg-info/dependency_links.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       25 2023-04-10 17:43:39.000000 aafitrans-0.0.6/src/aafitrans.egg-info/requires.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       10 2023-04-10 17:43:39.000000 aafitrans-0.0.6/src/aafitrans.egg-info/top_level.txt
```

### Comparing `aafitrans-0.0.5/LICENSE.txt` & `aafitrans-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aafitrans-0.0.5/PKG-INFO` & `aafitrans-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aafitrans
-Version: 0.0.5
+Version: 0.0.6
 Summary: match coordinate lists
 Author-email: Prajwel Joseph <prajwel.pj@gmail.com>
 Project-URL: Homepage, https://github.com/prajwel/aafitrans
 Project-URL: Bug Tracker, https://github.com/prajwel/aafitrans/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aafitrans-0.0.5/README.md` & `aafitrans-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aafitrans-0.0.5/pyproject.toml` & `aafitrans-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aafitrans-0.0.5/src/aafitrans/aafitrans.py` & `aafitrans-0.0.6/src/aafitrans/aafitrans.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from scipy.spatial import KDTree
 from itertools import combinations
 from functools import partial
 from collections import Counter
 from skimage import transform
 
 
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 
 class _MatchTransform:
     def __init__(self, source, target, ttype):
         self.source = source
         self.target = target
         self.ttype = ttype
 
@@ -71,14 +71,21 @@
         s, d = data.reshape(d1 * d2, d3).T
         resid = approx_t.residuals(self.source[s], self.target[d]).reshape(
             d1, d2
         )
         error = resid.max(axis=1)
         return error
     
+    def get_total_error(self, data, approx_t):
+        d1, d2, d3 = data.shape
+        s, d = data.reshape(d1 * d2, d3).T
+        resid = approx_t.residuals(self.source[s], self.target[d])
+        total_error = np.sqrt(np.sum(np.square(resid)) / (len(resid) * 3))    
+        return total_error       
+    
     
 def _invariantfeatures(x1, x2, x3):
     """Given 3 points x1, x2, x3, return the invariant features for the set."""
     sides = np.sort(
         [
             np.linalg.norm(x1 - x2),
             np.linalg.norm(x2 - x3),
@@ -160,18 +167,19 @@
     return inv_uniq, triang_vrtx_uniq
 
 
 def find_transform(source, target, 
                    max_control_points=50, 
                    ttype='similarity', 
                    pixel_tolerance=2, 
-                   min_matches=10, 
-                   num_nearest_neighbors=10,
-                   kdtree_search_radius = 0.001,
+                   min_matches=4, 
+                   num_nearest_neighbors=8,
+                   kdtree_search_radius = 0.02,
                    n_samples = 1,
+                   get_best_fit = True,
                    seed = None):
     """Estimate the transform between ``source`` and ``target``.
 
     Return a GeometricTransform object ``T`` that maps pixel x, y indices from
     the source image s = (x, y) into the target (destination) image t = (x, y).
     T contains parameters of the tranformation.
 
@@ -189,19 +197,20 @@
             The maximum residual error for the estimated tranform.            
         min_matches
             The minimum number of matches to be found.
         num_nearest_neighbors
             The number of nearest neighbors of a given star (including itself) 
             to construct the triangle invariants.                      
         kdtree_search_radius
-            The default is 0.001. I recommend to keep it 10 times the 
-            (pixel_tolerance / image size). For example, if your tolerance is 2 
-            image size is 1024, keep the value as (10 * 2 / 1024).  
+            The default is 0.02. This radius is used to find nearest neighbours
+            while conducting a KD tree search of invariant features. 
         n_samples
-            The minimum number of data points to fit the model to.            
+            The minimum number of data points to fit the model to.
+        get_best_fit
+            Whether to minimise the total error.                          
         seed
             Seed value for Numpy Random Generator.       
             
     Returns
     -------
         T, (source_pos_array, target_pos_array)
             The transformation object and a tuple of corresponding star positions
@@ -273,24 +282,27 @@
         inlier_ind = np.arange(len(matches))  # All of the indices
     else:
         best_t, inlier_ind = _ransac(matches, 
                                      inv_model, 
                                      pixel_tolerance, 
                                      min_matches, 
                                      n_samples, 
+                                     get_best_fit,
                                      seed)
         
     triangle_inliers = matches[inlier_ind]
     d1, d2, d3 = triangle_inliers.shape
     inl_arr = triangle_inliers.reshape(d1 * d2, d3)
     inl_arr_unique = np.unique(inl_arr, axis=0)
     s, t = inl_arr_unique.T
 
     return best_t, (source_controlp[s], target_controlp[t])
 
+
+
 # Copyright (c) 2004-2007, Andrew D. Straw. All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are
 # met:
 
 #     * Redistributions of source code must retain the above copyright
@@ -323,46 +335,47 @@
 
 
 class MaxIterError(RuntimeError):
     """Raise if maximum iterations reached."""
     pass
 
 
-def _ransac(data, model, thresh, min_matches, n_samples = 1, seed = None):
+def _ransac(data, model, thresh, min_matches, n_samples = 1, get_best_fit = True, seed = None):
     """Fit model parameters to data using the RANSAC algorithm.
 
-    This implementation written from pseudocode found at
-    http://en.wikipedia.org/w/index.php?title=RANSAC&oldid=116358182
-
     Parameters
     ----------
         data
             A set of data points
         model
             A model that can be fitted to data points
         thresh
             A threshold value to determine when a data point fits a model
         min_matches
             The min number of matches required to assert that a model
             fits well to data
         n_samples
             The minimum number of data points to fit the model to.
+        get_best_fit
+            Whether to minimise the total error.            
         seed
             Seed value for Numpy Random Generator.     
     Returns
     -------
         bestfit: model parameters which best fit the data (or nil if no good
                   model is found)
     """
     good_fit = None
     n_data = data.shape[0]
     all_idxs = np.arange(n_data)
     rng = np.random.default_rng(seed)
     rng.shuffle(all_idxs)
-
+    best_error = np.inf
+    improve_error_counter = 0
+    
     for iter_i in range(n_data):
         # Partition indices into two random subsets
         maybe_idxs = all_idxs[iter_i : iter_i + n_samples]
         test_idxs = np.concatenate([all_idxs[:iter_i], 
                                     all_idxs[iter_i + n_samples:]])        
         maybeinliers = data[maybe_idxs, :]
         test_points = data[test_idxs, :]
@@ -370,29 +383,35 @@
         test_err = model.get_error(test_points, maybemodel)
         # select indices of rows with accepted points
         also_idxs = test_idxs[test_err < thresh]
         alsoinliers = data[also_idxs, :]
         if len(alsoinliers) >= min_matches:
             good_data = np.concatenate((maybeinliers, alsoinliers))
             good_fit = model.fit(good_data)
-            break
+            total_error = model.get_total_error(good_data, good_fit)
+            if get_best_fit and total_error < best_error:
+                best_error = total_error
+                best_fit = good_fit 
+                improve_error_counter += 1
+                if improve_error_counter == 100:
+                    break
+            else:
+                best_fit = good_fit
 
-    if good_fit is None:
+    if best_fit is None:
         raise MaxIterError(
             "List of matching triangles exhausted before an acceptable "
             "transformation was found"
         )
 
-    better_fit = good_fit
-    previous_fit = good_fit.params + 1
+    better_fit = best_fit
+    previous_fit = best_fit.params + 1
     for i in range(100):
         test_err = model.get_error(data, better_fit)
         better_inlier_idxs = np.arange(n_data)[test_err < thresh]
         better_data = data[better_inlier_idxs]
         better_fit = model.fit(better_data)
         if np.all((previous_fit == better_fit.params)):
             break
         previous_fit = better_fit.params
 
-    best_fit = better_fit
-    best_inlier_idxs = better_inlier_idxs
-    return best_fit, best_inlier_idxs
+    return better_fit, better_inlier_idxs
```

### Comparing `aafitrans-0.0.5/src/aafitrans.egg-info/PKG-INFO` & `aafitrans-0.0.6/src/aafitrans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aafitrans
-Version: 0.0.5
+Version: 0.0.6
 Summary: match coordinate lists
 Author-email: Prajwel Joseph <prajwel.pj@gmail.com>
 Project-URL: Homepage, https://github.com/prajwel/aafitrans
 Project-URL: Bug Tracker, https://github.com/prajwel/aafitrans/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


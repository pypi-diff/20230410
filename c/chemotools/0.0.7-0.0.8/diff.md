# Comparing `tmp/chemotools-0.0.7.tar.gz` & `tmp/chemotools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemotools-0.0.7.tar", last modified: Mon Apr 10 14:29:02 2023, max compression
+gzip compressed data, was "chemotools-0.0.8.tar", last modified: Mon Apr 10 15:18:14 2023, max compression
```

## Comparing `chemotools-0.0.7.tar` & `chemotools-0.0.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:29:02.614383 chemotools-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-10 14:28:52.000000 chemotools-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-10 14:29:02.614383 chemotools-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-10 14:28:52.000000 chemotools-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:29:02.606383 chemotools-0.0.7/chemotools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:29:02.606383 chemotools-0.0.7/chemotools/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/baseline/air_pls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/baseline/cubic_spline_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/baseline/linear_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/baseline/non_negative.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/baseline/polynomial_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:29:02.606383 chemotools-0.0.7/chemotools/derivative/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/derivative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/derivative/norris_william.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/derivative/savitzky_golay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:29:02.610383 chemotools-0.0.7/chemotools/normalize/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/normalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/normalize/l_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/normalize/min_max_normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:29:02.610383 chemotools-0.0.7/chemotools/scattering/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/scattering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/scattering/extended_multiplicative_scatter_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/scattering/multiplicative_scatter_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/scattering/standard_normal_variate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:29:02.610383 chemotools-0.0.7/chemotools/smoothing/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/smoothing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/smoothing/mean_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/smoothing/median_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/smoothing/savitzky_golay_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/smoothing/whittaker_smooth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:29:02.610383 chemotools-0.0.7/chemotools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-10 14:28:52.000000 chemotools-0.0.7/chemotools/utils/check_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:29:02.614383 chemotools-0.0.7/chemotools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-10 14:29:02.000000 chemotools-0.0.7/chemotools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-10 14:29:02.000000 chemotools-0.0.7/chemotools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 14:29:02.000000 chemotools-0.0.7/chemotools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 14:29:02.000000 chemotools-0.0.7/chemotools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-10 14:29:02.000000 chemotools-0.0.7/chemotools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 14:28:52.000000 chemotools-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 14:29:02.614383 chemotools-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-10 14:28:52.000000 chemotools-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:29:02.614383 chemotools-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 14:28:52.000000 chemotools-0.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-10 14:28:52.000000 chemotools-0.0.7/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-04-10 14:28:52.000000 chemotools-0.0.7/tests/test_functionality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-10 14:28:52.000000 chemotools-0.0.7/tests/test_sklearn_compliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.922122 chemotools-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-10 15:17:51.000000 chemotools-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-10 15:18:14.922122 chemotools-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-10 15:17:51.000000 chemotools-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.914122 chemotools-0.0.8/chemotools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.918122 chemotools-0.0.8/chemotools/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/baseline/air_pls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/baseline/cubic_spline_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/baseline/linear_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/baseline/non_negative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/baseline/polynomial_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.918122 chemotools-0.0.8/chemotools/derivative/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/derivative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/derivative/norris_william.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/derivative/savitzky_golay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.918122 chemotools-0.0.8/chemotools/normalize/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/normalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/normalize/l_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/normalize/min_max_normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.918122 chemotools-0.0.8/chemotools/scattering/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/scattering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/scattering/extended_multiplicative_scatter_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/scattering/multiplicative_scatter_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/scattering/standard_normal_variate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.918122 chemotools-0.0.8/chemotools/smoothing/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/smoothing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/smoothing/mean_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/smoothing/median_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/smoothing/savitzky_golay_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/smoothing/whittaker_smooth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.918122 chemotools-0.0.8/chemotools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-10 15:17:51.000000 chemotools-0.0.8/chemotools/utils/check_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.922122 chemotools-0.0.8/chemotools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-10 15:18:14.000000 chemotools-0.0.8/chemotools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-10 15:18:14.000000 chemotools-0.0.8/chemotools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:18:14.000000 chemotools-0.0.8/chemotools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 15:18:14.000000 chemotools-0.0.8/chemotools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-10 15:18:14.000000 chemotools-0.0.8/chemotools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 15:17:51.000000 chemotools-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:18:14.922122 chemotools-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-10 15:17:51.000000 chemotools-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:14.922122 chemotools-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:17:51.000000 chemotools-0.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-10 15:17:51.000000 chemotools-0.0.8/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-04-10 15:17:51.000000 chemotools-0.0.8/tests/test_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-10 15:17:51.000000 chemotools-0.0.8/tests/test_sklearn_compliance.py
```

### Comparing `chemotools-0.0.7/LICENSE` & `chemotools-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.7/PKG-INFO` & `chemotools-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemotools
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package to integrate chemometrics in scikit-learn pipelines
 Home-page: https://github.com/paucablop/chemotools
 Author: Pau Cabaneros Lopez
 Author-email: pau.cabaneros@gmail.com
 Project-URL: Bug Tracker, https://github.com/paucablop/chemotools/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chemotools-0.0.7/chemotools/baseline/air_pls.py` & `chemotools-0.0.8/chemotools/baseline/air_pls.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.7/chemotools/baseline/cubic_spline_correction.py` & `chemotools-0.0.8/chemotools/baseline/polynomial_correction.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,45 @@
 import numpy as np
-from scipy.interpolate import CubicSpline
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_is_fitted
 
 from chemotools.utils.check_inputs import check_input
 
-class CubicSplineCorrection(BaseEstimator, TransformerMixin):
-    def __init__(self, indices: tuple = None) -> None:
+class PolynomialCorrection(BaseEstimator, TransformerMixin):
+    def __init__(self, order: int = 1, indices: tuple = (0, -1)) -> None:
+        self.order = order
         self.indices = indices
 
-    def fit(self, X: np.ndarray, y=None) -> "CubicSplineCorrection":
+    def fit(self, X: np.ndarray, y=None) -> "PolynomialCorrection":
         # Check that X is a 2D array and has only finite values
         X = check_input(X)
 
         # Set the number of features
         self.n_features_in_ = X.shape[1]
 
         # Set the fitted attribute to True
         self._is_fitted = True
 
         return self
-
-    def transform(self, X: np.ndarray, y=None, copy=True):
+    
+    def transform(self, X: np.ndarray, y=0, copy=True) -> np.ndarray:
         # Check that the estimator is fitted
         check_is_fitted(self, "_is_fitted")
 
         # Check that X is a 2D array and has only finite values
         X = check_input(X)
         X_ = X.copy()
 
         # Check that the number of features is the same as the fitted data
         if X_.shape[1] != self.n_features_in_:
             raise ValueError(f"Expected {self.n_features_in_} features but got {X_.shape[1]}")
 
-        # Calculate spline baseline correction
+        # Calculate polynomial baseline correction
         for i, x in enumerate(X_):
-            X_[i] = self._spline_baseline_correct(x)
+            X_[i] = self._baseline_correct_spectrum(x)
         return X_.reshape(-1, 1) if X_.ndim == 1 else X_
-
-    def _spline_baseline_correct(self, x: np.ndarray) -> np.ndarray:
-        if self.indices is None:
-            indices = [0, len(x) - 1]
-        else:
-            indices = self.indices
-
-        intensity = x[indices]  
-        spl = CubicSpline(indices, intensity)
-        baseline = spl(range(len(x)))      
+    
+    def _baseline_correct_spectrum(self, x: np.ndarray) -> np.ndarray:
+        intensity = x[list(self.indices)]
+        poly = np.polyfit(self.indices, intensity, self.order)
+        baseline = [np.polyval(poly, i) for i in range(0, len(x))]      
         return x - baseline
```

### Comparing `chemotools-0.0.7/chemotools/baseline/linear_correction.py` & `chemotools-0.0.8/chemotools/baseline/linear_correction.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.7/chemotools/baseline/non_negative.py` & `chemotools-0.0.8/chemotools/baseline/non_negative.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.7/chemotools/baseline/polynomial_correction.py` & `chemotools-0.0.8/chemotools/smoothing/median_filter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 import numpy as np
+from scipy.ndimage import median_filter
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_is_fitted
 
 from chemotools.utils.check_inputs import check_input
 
-class PolynomialCorrection(BaseEstimator, TransformerMixin):
-    def __init__(self, order: int = 1, indices: tuple = (0, -1)) -> None:
-        self.order = order
-        self.indices = indices
 
-    def fit(self, X: np.ndarray, y=None) -> "PolynomialCorrection":
+class MedianFilter(BaseEstimator, TransformerMixin):
+    def __init__(self, window_size: int = 3, mode: str = 'nearest') -> None:
+        self.window_size = window_size
+        self.mode = mode
+
+    def fit(self, X: np.ndarray, y=None) -> "MedianFilter":
         # Check that X is a 2D array and has only finite values
         X = check_input(X)
 
         # Set the number of features
         self.n_features_in_ = X.shape[1]
 
         # Set the fitted attribute to True
         self._is_fitted = True
 
         return self
-    
-    def transform(self, X: np.ndarray, y=0, copy=True) -> np.ndarray:
+
+    def transform(self, X: np.ndarray, y=None) -> np.ndarray:
         # Check that the estimator is fitted
         check_is_fitted(self, "_is_fitted")
 
         # Check that X is a 2D array and has only finite values
         X = check_input(X)
         X_ = X.copy()
 
-        # Check that the number of features is the same as the fitted data
         if X_.shape[1] != self.n_features_in_:
-            raise ValueError(f"Expected {self.n_features_in_} features but got {X_.shape[1]}")
+            raise ValueError(
+                f"Expected {self.n_features_in_} features but got {X_.shape[1]}"
+            )
 
-        # Calculate polynomial baseline correction
+        # Mean filter the data
         for i, x in enumerate(X_):
-            X_[i] = self._baseline_correct_spectrum(x)
+            X_[i] = median_filter(x, size=self.window_size, mode=self.mode)
         return X_.reshape(-1, 1) if X_.ndim == 1 else X_
-    
-    def _baseline_correct_spectrum(self, x: np.ndarray) -> np.ndarray:
-        intensity = x[list(self.indices)]
-        poly = np.polyfit(self.indices, intensity, self.order)
-        baseline = [np.polyval(poly, i) for i in range(0, len(x))]      
-        return x - baseline
```

### Comparing `chemotools-0.0.7/chemotools/derivative/norris_william.py` & `chemotools-0.0.8/chemotools/derivative/norris_william.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.7/chemotools/derivative/savitzky_golay.py` & `chemotools-0.0.8/chemotools/derivative/savitzky_golay.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.7/chemotools/normalize/l_normalize.py` & `chemotools-0.0.8/chemotools/normalize/l_normalize.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.7/chemotools/normalize/min_max_normalize.py` & `chemotools-0.0.8/chemotools/normalize/min_max_normalize.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.7/chemotools/scattering/extended_multiplicative_scatter_correction.py` & `chemotools-0.0.8/chemotools/scattering/extended_multiplicative_scatter_correction.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.7/chemotools/scattering/multiplicative_scatter_correction.py` & `chemotools-0.0.8/chemotools/scattering/multiplicative_scatter_correction.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.7/chemotools/scattering/standard_normal_variate.py` & `chemotools-0.0.8/chemotools/scattering/standard_normal_variate.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.7/chemotools/smoothing/mean_filter.py` & `chemotools-0.0.8/chemotools/smoothing/mean_filter.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.7/chemotools/smoothing/median_filter.py` & `chemotools-0.0.8/chemotools/smoothing/savitzky_golay_filter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import numpy as np
-from scipy.ndimage import median_filter
+from scipy.signal import savgol_filter
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_is_fitted
 
 from chemotools.utils.check_inputs import check_input
 
 
-class MedianFilter(BaseEstimator, TransformerMixin):
-    def __init__(self, window_size: int = 3, mode: str = 'nearest') -> None:
+class SavitzkyGolayFilter(BaseEstimator, TransformerMixin):
+    def __init__(
+        self, window_size: int = 3, polynomial_order: int = 1, mode: str = "nearest"
+    ) -> None:
         self.window_size = window_size
+        self.polynomial_order = polynomial_order
         self.mode = mode
 
-    def fit(self, X: np.ndarray, y=None) -> "MedianFilter":
+    def fit(self, X: np.ndarray, y=None) -> "SavitzkyGolayFilter":
         # Check that X is a 2D array and has only finite values
         X = check_input(X)
 
         # Set the number of features
         self.n_features_in_ = X.shape[1]
 
         # Set the fitted attribute to True
@@ -32,11 +35,22 @@
         X_ = X.copy()
 
         if X_.shape[1] != self.n_features_in_:
             raise ValueError(
                 f"Expected {self.n_features_in_} features but got {X_.shape[1]}"
             )
 
-        # Mean filter the data
+        # Calculate the standard normal variate
         for i, x in enumerate(X_):
-            X_[i] = median_filter(x, size=self.window_size, mode=self.mode)
+            X_[i] = self._calculate_smoothing(x)
+
         return X_.reshape(-1, 1) if X_.ndim == 1 else X_
+
+    def _calculate_smoothing(self, x) -> np.ndarray:
+        return savgol_filter(
+            x,
+            self.window_size,
+            self.polynomial_order,
+            deriv=0,
+            axis=0,
+            mode=self.mode,
+        )
```

### Comparing `chemotools-0.0.7/chemotools/smoothing/savitzky_golay_filter.py` & `chemotools-0.0.8/chemotools/smoothing/whittaker_smooth.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import numpy as np
-from scipy.signal import savgol_filter
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_is_fitted
 
 from chemotools.utils.check_inputs import check_input
 
 
-class SavitzkyGolayFilter(BaseEstimator, TransformerMixin):
+class WhittakerSmooth(BaseEstimator, TransformerMixin):
     def __init__(
-        self, window_size: int = 3, polynomial_order: int = 1, mode: str = "nearest"
-    ) -> None:
-        self.window_size = window_size
-        self.polynomial_order = polynomial_order
-        self.mode = mode
+        self,
+        lam: float = 1e2,
+        differences: int = 1,
+    ):
+        self.lam = lam
+        self.differences = differences
 
-    def fit(self, X: np.ndarray, y=None) -> "SavitzkyGolayFilter":
+    def fit(self, X: np.ndarray, y=None) -> "WhittakerSmooth":
         # Check that X is a 2D array and has only finite values
         X = check_input(X)
 
         # Set the number of features
         self.n_features_in_ = X.shape[1]
 
         # Set the fitted attribute to True
@@ -30,27 +30,28 @@
         # Check that the estimator is fitted
         check_is_fitted(self, "_is_fitted")
 
         # Check that X is a 2D array and has only finite values
         X = check_input(X)
         X_ = X.copy()
 
+        # Check that the number of features is the same as the fitted data
         if X_.shape[1] != self.n_features_in_:
-            raise ValueError(
-                f"Expected {self.n_features_in_} features but got {X_.shape[1]}"
-            )
+            raise ValueError(f"Expected {self.n_features_in_} features but got {X_.shape[1]}")
 
-        # Calculate the standard normal variate
+        # Calculate the whittaker smooth
         for i, x in enumerate(X_):
-            X_[i] = self._calculate_smoothing(x)
-
+            X_[i] = self._calculate_whittaker_smooth(x)
+            
         return X_.reshape(-1, 1) if X_.ndim == 1 else X_
 
-    def _calculate_smoothing(self, x) -> np.ndarray:
-        return savgol_filter(
-            x,
-            self.window_size,
-            self.polynomial_order,
-            deriv=0,
-            axis=0,
-            mode=self.mode,
-        )
+    def _calculate_whittaker_smooth(self, x):
+        x = np.asarray(x)
+        n = len(x)
+        D = np.diff(np.eye(n), self.differences)
+        w = np.ones(n)
+        for i in range(self.differences+1):
+            W = np.diag(w) + 1e-8*np.eye(n)
+            Z = W + self.lam * np.dot(D, D.T)
+            z = np.linalg.solve(Z, w * x)
+            w = np.sqrt(np.maximum(z, 0))
+        return z
```

### Comparing `chemotools-0.0.7/chemotools/smoothing/whittaker_smooth.py` & `chemotools-0.0.8/chemotools/baseline/cubic_spline_correction.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,50 @@
 import numpy as np
+from scipy.interpolate import CubicSpline
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_is_fitted
 
 from chemotools.utils.check_inputs import check_input
 
+class CubicSplineCorrection(BaseEstimator, TransformerMixin):
+    def __init__(self, indices: tuple = None) -> None:
+        self.indices = indices
 
-class WhittakerSmooth(BaseEstimator, TransformerMixin):
-    def __init__(
-        self,
-        lam: float = 1e2,
-        differences: int = 1,
-    ):
-        self.lam = lam
-        self.differences = differences
-
-    def fit(self, X: np.ndarray, y=None) -> "WhittakerSmooth":
+    def fit(self, X: np.ndarray, y=None) -> "CubicSplineCorrection":
         # Check that X is a 2D array and has only finite values
         X = check_input(X)
 
         # Set the number of features
         self.n_features_in_ = X.shape[1]
 
         # Set the fitted attribute to True
         self._is_fitted = True
 
         return self
 
-    def transform(self, X: np.ndarray, y=None) -> np.ndarray:
+    def transform(self, X: np.ndarray, y=None, copy=True):
         # Check that the estimator is fitted
         check_is_fitted(self, "_is_fitted")
 
         # Check that X is a 2D array and has only finite values
         X = check_input(X)
         X_ = X.copy()
 
         # Check that the number of features is the same as the fitted data
         if X_.shape[1] != self.n_features_in_:
             raise ValueError(f"Expected {self.n_features_in_} features but got {X_.shape[1]}")
 
-        # Calculate the whittaker smooth
+        # Calculate spline baseline correction
         for i, x in enumerate(X_):
-            X_[i] = self._calculate_whittaker_smooth(x)
-            
+            X_[i] = self._spline_baseline_correct(x)
         return X_.reshape(-1, 1) if X_.ndim == 1 else X_
 
-    def _calculate_whittaker_smooth(self, x):
-        x = np.asarray(x)
-        n = len(x)
-        D = np.diff(np.eye(n), self.differences)
-        w = np.ones(n)
-        for i in range(self.differences+1):
-            W = np.diag(w) + 1e-8*np.eye(n)
-            Z = W + self.lam * np.dot(D, D.T)
-            z = np.linalg.solve(Z, w * x)
-            w = np.sqrt(np.maximum(z, 0))
-        return z
+    def _spline_baseline_correct(self, x: np.ndarray) -> np.ndarray:
+        if self.indices is None:
+            indices = [0, len(x) - 1]
+        else:
+            indices = list(self.indices)
+
+        intensity = x[indices]  
+        spl = CubicSpline(indices, intensity)
+        baseline = spl(range(len(x)))      
+        return x - baseline
```

### Comparing `chemotools-0.0.7/chemotools/utils/check_inputs.py` & `chemotools-0.0.8/chemotools/utils/check_inputs.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.7/chemotools.egg-info/PKG-INFO` & `chemotools-0.0.8/chemotools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemotools
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package to integrate chemometrics in scikit-learn pipelines
 Home-page: https://github.com/paucablop/chemotools
 Author: Pau Cabaneros Lopez
 Author-email: pau.cabaneros@gmail.com
 Project-URL: Bug Tracker, https://github.com/paucablop/chemotools/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chemotools-0.0.7/chemotools.egg-info/SOURCES.txt` & `chemotools-0.0.8/chemotools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.7/setup.py` & `chemotools-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.7/tests/fixtures.py` & `chemotools-0.0.8/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.7/tests/test_functionality.py` & `chemotools-0.0.8/tests/test_functionality.py`

 * *Files identical despite different names*

### Comparing `chemotools-0.0.7/tests/test_sklearn_compliance.py` & `chemotools-0.0.8/tests/test_sklearn_compliance.py`

 * *Files identical despite different names*


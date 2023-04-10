# Comparing `tmp/statinf-1.2.1.tar.gz` & `tmp/statinf-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statinf-1.2.1.tar", last modified: Sun Apr  9 11:19:11 2023, max compression
+gzip compressed data, was "statinf-1.2.2.tar", last modified: Mon Apr 10 12:25:05 2023, max compression
```

## Comparing `statinf-1.2.1.tar` & `statinf-1.2.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-09 11:19:11.321976 statinf-1.2.1/
--rw-r--r--   0 florian   (1000) florian   (1000)     1070 2020-10-01 18:31:13.000000 statinf-1.2.1/LICENSE
--rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-04-09 11:19:11.321976 statinf-1.2.1/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     8337 2020-10-01 18:31:13.000000 statinf-1.2.1/README.md
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-04-09 11:19:11.321976 statinf-1.2.1/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)      781 2020-10-01 18:31:13.000000 statinf-1.2.1/setup.py
--rw-r--r--   0 florian   (1000) florian   (1000)      889 2023-04-09 11:19:10.000000 statinf-1.2.1/setup_new.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-09 11:19:11.301976 statinf-1.2.1/statinf/
--rw-r--r--   0 florian   (1000) florian   (1000)       22 2023-04-09 11:19:10.000000 statinf-1.2.1/statinf/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-09 11:19:11.311976 statinf-1.2.1/statinf/data/
--rw-r--r--   0 florian   (1000) florian   (1000)     2701 2023-02-03 18:48:52.000000 statinf-1.2.1/statinf/data/GenerateData.py
--rw-r--r--   0 florian   (1000) florian   (1000)    27132 2021-03-24 14:33:31.000000 statinf-1.2.1/statinf/data/ProcessData.py
--rw-r--r--   0 florian   (1000) florian   (1000)       55 2020-10-01 18:31:13.000000 statinf-1.2.1/statinf/data/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-09 11:19:11.311976 statinf-1.2.1/statinf/distributions/
--rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-02-03 18:27:09.000000 statinf-1.2.1/statinf/distributions/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    22095 2023-04-09 10:59:39.000000 statinf-1.2.1/statinf/distributions/discrete.py
--rw-r--r--   0 florian   (1000) florian   (1000)       26 2021-06-27 12:48:10.000000 statinf-1.2.1/statinf/init_template.py
--rw-r--r--   0 florian   (1000) florian   (1000)     5107 2021-06-27 13:22:48.000000 statinf-1.2.1/statinf/misc.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-09 11:19:11.311976 statinf-1.2.1/statinf/ml/
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2020-10-01 18:31:13.000000 statinf-1.2.1/statinf/ml/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2522 2021-03-07 06:24:49.000000 statinf-1.2.1/statinf/ml/activations.py
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2020-10-17 16:20:51.000000 statinf-1.2.1/statinf/ml/generative.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2892 2021-03-07 06:09:35.000000 statinf-1.2.1/statinf/ml/initializations.py
--rw-r--r--   0 florian   (1000) florian   (1000)     3152 2021-03-07 06:45:42.000000 statinf-1.2.1/statinf/ml/losses.py
--rw-r--r--   0 florian   (1000) florian   (1000)    16863 2022-08-21 10:47:32.000000 statinf-1.2.1/statinf/ml/neuralnetwork.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11152 2021-03-07 08:40:43.000000 statinf-1.2.1/statinf/ml/optimizers.py
--rw-r--r--   0 florian   (1000) florian   (1000)     6141 2021-06-27 13:22:59.000000 statinf-1.2.1/statinf/ml/performance.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-09 11:19:11.311976 statinf-1.2.1/statinf/nonparametrics/
--rw-r--r--   0 florian   (1000) florian   (1000)       23 2020-11-01 11:38:35.000000 statinf-1.2.1/statinf/nonparametrics/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)      842 2020-11-01 18:05:22.000000 statinf-1.2.1/statinf/nonparametrics/kernels.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-09 11:19:11.311976 statinf-1.2.1/statinf/regressions/
--rw-r--r--   0 florian   (1000) florian   (1000)    19249 2021-03-24 15:58:55.000000 statinf-1.2.1/statinf/regressions/LinearModels.py
--rw-r--r--   0 florian   (1000) florian   (1000)       51 2023-02-03 18:26:31.000000 statinf-1.2.1/statinf/regressions/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    18168 2021-03-24 15:54:37.000000 statinf-1.2.1/statinf/regressions/glm.py
--rw-r--r--   0 florian   (1000) florian   (1000)     7060 2020-10-01 18:31:13.000000 statinf-1.2.1/statinf/regressions/glm_test.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-09 11:19:11.321976 statinf-1.2.1/statinf/stats/
--rw-r--r--   0 florian   (1000) florian   (1000)      126 2020-11-01 12:20:16.000000 statinf-1.2.1/statinf/stats/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     6950 2020-11-01 18:03:36.000000 statinf-1.2.1/statinf/stats/bayesian.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4185 2020-10-01 18:31:13.000000 statinf-1.2.1/statinf/stats/descriptive.py
--rw-r--r--   0 florian   (1000) florian   (1000)    21520 2023-02-03 18:58:48.000000 statinf-1.2.1/statinf/stats/tests.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11524 2020-10-27 02:35:31.000000 statinf-1.2.1/statinf/stats/timeseries.py
--rw-r--r--   0 florian   (1000) florian   (1000)    10469 2020-11-01 18:02:58.000000 statinf-1.2.1/statinf/stats/unsupervised.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-09 11:19:11.311976 statinf-1.2.1/statinf.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-04-09 11:19:11.000000 statinf-1.2.1/statinf.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      966 2023-04-09 11:19:11.000000 statinf-1.2.1/statinf.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-04-09 11:19:11.000000 statinf-1.2.1/statinf.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      101 2023-04-09 11:19:11.000000 statinf-1.2.1/statinf.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-04-09 11:19:11.000000 statinf-1.2.1/statinf.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-10 12:25:05.507358 statinf-1.2.2/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1070 2020-10-01 18:31:13.000000 statinf-1.2.2/LICENSE
+-rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-04-10 12:25:05.507358 statinf-1.2.2/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     8337 2020-10-01 18:31:13.000000 statinf-1.2.2/README.md
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-04-10 12:25:05.507358 statinf-1.2.2/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)      781 2020-10-01 18:31:13.000000 statinf-1.2.2/setup.py
+-rw-r--r--   0 florian   (1000) florian   (1000)      889 2023-04-10 12:25:05.000000 statinf-1.2.2/setup_new.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-10 12:25:05.487358 statinf-1.2.2/statinf/
+-rw-r--r--   0 florian   (1000) florian   (1000)       22 2023-04-10 12:25:05.000000 statinf-1.2.2/statinf/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-10 12:25:05.497358 statinf-1.2.2/statinf/data/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2701 2023-02-03 18:48:52.000000 statinf-1.2.2/statinf/data/GenerateData.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    27132 2021-03-24 14:33:31.000000 statinf-1.2.2/statinf/data/ProcessData.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       55 2020-10-01 18:31:13.000000 statinf-1.2.2/statinf/data/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-10 12:25:05.497358 statinf-1.2.2/statinf/distributions/
+-rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-02-03 18:27:09.000000 statinf-1.2.2/statinf/distributions/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    22636 2023-04-10 12:16:43.000000 statinf-1.2.2/statinf/distributions/discrete.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       26 2021-06-27 12:48:10.000000 statinf-1.2.2/statinf/init_template.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     5107 2021-06-27 13:22:48.000000 statinf-1.2.2/statinf/misc.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-10 12:25:05.497358 statinf-1.2.2/statinf/ml/
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2020-10-01 18:31:13.000000 statinf-1.2.2/statinf/ml/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2522 2021-03-07 06:24:49.000000 statinf-1.2.2/statinf/ml/activations.py
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2020-10-17 16:20:51.000000 statinf-1.2.2/statinf/ml/generative.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2892 2021-03-07 06:09:35.000000 statinf-1.2.2/statinf/ml/initializations.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     3152 2021-03-07 06:45:42.000000 statinf-1.2.2/statinf/ml/losses.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    16863 2022-08-21 10:47:32.000000 statinf-1.2.2/statinf/ml/neuralnetwork.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11152 2021-03-07 08:40:43.000000 statinf-1.2.2/statinf/ml/optimizers.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     6141 2021-06-27 13:22:59.000000 statinf-1.2.2/statinf/ml/performance.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-10 12:25:05.497358 statinf-1.2.2/statinf/nonparametrics/
+-rw-r--r--   0 florian   (1000) florian   (1000)       23 2020-11-01 11:38:35.000000 statinf-1.2.2/statinf/nonparametrics/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)      842 2020-11-01 18:05:22.000000 statinf-1.2.2/statinf/nonparametrics/kernels.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-10 12:25:05.507358 statinf-1.2.2/statinf/regressions/
+-rw-r--r--   0 florian   (1000) florian   (1000)    19249 2021-03-24 15:58:55.000000 statinf-1.2.2/statinf/regressions/LinearModels.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       51 2023-02-03 18:26:31.000000 statinf-1.2.2/statinf/regressions/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    18168 2021-03-24 15:54:37.000000 statinf-1.2.2/statinf/regressions/glm.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     7060 2020-10-01 18:31:13.000000 statinf-1.2.2/statinf/regressions/glm_test.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-10 12:25:05.507358 statinf-1.2.2/statinf/stats/
+-rw-r--r--   0 florian   (1000) florian   (1000)      126 2020-11-01 12:20:16.000000 statinf-1.2.2/statinf/stats/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     6950 2020-11-01 18:03:36.000000 statinf-1.2.2/statinf/stats/bayesian.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4185 2020-10-01 18:31:13.000000 statinf-1.2.2/statinf/stats/descriptive.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    21520 2023-02-03 18:58:48.000000 statinf-1.2.2/statinf/stats/tests.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11524 2020-10-27 02:35:31.000000 statinf-1.2.2/statinf/stats/timeseries.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    10469 2020-11-01 18:02:58.000000 statinf-1.2.2/statinf/stats/unsupervised.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-10 12:25:05.497358 statinf-1.2.2/statinf.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-04-10 12:25:05.000000 statinf-1.2.2/statinf.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      966 2023-04-10 12:25:05.000000 statinf-1.2.2/statinf.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-04-10 12:25:05.000000 statinf-1.2.2/statinf.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      101 2023-04-10 12:25:05.000000 statinf-1.2.2/statinf.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-04-10 12:25:05.000000 statinf-1.2.2/statinf.egg-info/top_level.txt
```

### Comparing `statinf-1.2.1/LICENSE` & `statinf-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/PKG-INFO` & `statinf-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statinf
-Version: 1.2.1
+Version: 1.2.2
 Summary: A library for statistics and causal inference
 Home-page: https://www.florianfelice.com/statinf
 Author: Florian Felice
 Author-email: florian.felice@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `statinf-1.2.1/README.md` & `statinf-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/setup.py` & `statinf-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/setup_new.py` & `statinf-1.2.2/setup_new.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="statinf",
-    version="1.2.1",
+    version="1.2.2",
     author="Florian Felice",
     author_email="florian.felice@outlook.com",
     description="A library for statistics and causal inference",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.florianfelice.com/statinf",
     packages=setuptools.find_packages(),
```

### Comparing `statinf-1.2.1/statinf/data/GenerateData.py` & `statinf-1.2.2/statinf/data/GenerateData.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/statinf/data/ProcessData.py` & `statinf-1.2.2/statinf/data/ProcessData.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/statinf/distributions/discrete.py` & `statinf-1.2.2/statinf/distributions/discrete.py`

 * *Files 8% similar despite different names*

```diff
@@ -306,20 +306,20 @@
 
         self._Z = None
 
         if (self.lambda_ is not None) & (self.nu_ is not None):
             assert self.lambda_ >= 0, ValueError('Value for parameter lambda must be strictly greater to 0 (lambda_ > 0)')
             assert self.nu_ >= 0, ValueError('Value for parameter nu must be greater or equal to 0 (nu_ >= 0)')
             warnings.filterwarnings("error")
-            self._Z = self.Z()
+            self._Z = self.Z(lambda_=self.lambda_, nu_=self.nu_, j=self.j, approx=True)
             warnings.resetwarnings()
 
-        self.nll_fun = lambda params, data, j: self.nloglike(params=params, data=data, j=j)
+        self.nll_fun = lambda params, data, j, approx: self.nloglike(params=params, data=data, j=j, approx=approx, Z=self.Z)
 
-    def Z(self, j=None) -> float:
+    def Z(self, lambda_, nu_, j=None, approx=False, log=False) -> float:
         """Compute the :math:`Z` factor, normalizing constant.
 
         The factor :math:`Z(\\lambda, \\nu)` serves as a normalizing constant such that the distribution satisfies the basic probability axioms (i.e. the probability mass function sums up to 1).
 
         .. math::
 
             Z(\\lambda, \\nu) = \\sum_{j=0}^{\\infty} \\dfrac{\\lambda^{j}}{(j!)^{\\nu}}
@@ -327,52 +327,98 @@
         .. note::
 
             For implementation purposes, the length of the sum cannot be infinity.
             The parameter :obj:`j` is chosen to be suficiently large so that the value of the sum converges to its asymptotic value.
             Note that too large values for :obj:`j` will imply longer computation time and potential errors
             (:math:`j!` may become too large and might not fit in memory).
 
+        :param lambda\\_: First parameter :math:`\\lambda > 0` of the distribution
+        :type lambda\\_: :obj:`float`, optional
+        :param nu\\_: Second parameter :math:`\\nu > 0` of the distribution
+        :type nu\\_: :obj:`float`, optional
         :param j: Length of the sum for the normalizing constant, if :obj:`None` then we use the value from the :obj:`__init__` method, defaults to None
         :type j: :obj:`int`, optional
+        :param approx: Use approximation form for computing :math:`Z(\\lambda, \\nu)`, defaults to False
+        :type approx: :obj:`bool`
+        :param approx: Compute :math:`Z(\\lambda, \\nu)`, defaults to False
+        :type approx: :obj:`bool`
 
         :return: Z factor
         :rtype: :obj:`float`
         """
         j = j if j else self.j
-        z_i = 0
-        for i in range(j):
-            _dec = False
-            # We use a decimal placeholder variable in case we encounter overflow errors (number is too long).
-            # We don't use decimal as a default but only in case of error because it slows down computations,
-            # therefore, by default we use light and simple format and call Decimal when needed.
-            # For instances where we need Decimal, we will transform back the ratio of decimals to float as
-            # the value will be of reasonable size and not too long for a classical float.
 
-            # Compute the denominator
+        if (nu_ > 1 - self.eps) & (nu_ < 1 + self.eps):
+            # ## Poisson distribution
+            # When nu = 1, then we have a Poisson distribution
+            z_i = math.exp(lambda_)
+        elif (nu_ > 0) & (nu_ < 0 + self.eps):
+            # ## Geometric distribution
+            # When nu = 0, then we have a geometric distribution
+            z_i = 1 / (1 - lambda_)
+        elif (approx) & ((nu_ < 1 + self.eps) or (lambda_ > (10 ** nu_))):
+            # ## Approximation
+            # If we want the approximation and it verifies the assumptions (for nu > 1 and lambda > 10^nu), we use approximation
+            _dec = False
+            # Compute numerator
             try:
-                _denom = math.factorial(i) ** self.nu_
-            except OverflowError:
-                # If overflow error (i.e. output is too long), use Decimal format
-                _denom = Decimal(math.factorial(i)) ** Decimal(self.nu_)
+                _num = math.exp(nu_ * (lambda_ ** (1 / nu_)))
+            except RuntimeWarning:
+                # If runtime warning it is similar to overflow error (i.e. output is too long), use Decimal format
+                _pow = Decimal(lambda_) ** Decimal(1 / nu_)
+                _num = Decimal(math.exp(Decimal(nu_) * _pow))
                 _dec = True
-            # Compute the numerator
+
+            # Compute denominator
             try:
-                _num = self.lambda_ ** i
+                _denom = lambda_ ** ((nu_ - 1) / (2 * nu_))
+                _denom *= (2 * math.pi) ** ((nu_ - 1) / 2)
+                _denom *= math.sqrt(nu_)
+                _o_lambda = 1 / (lambda_ ** (1 / nu_))
             except RuntimeWarning:
-                # If runtime warning it is similar to overflow error (i.e. output is too long), use Decimal format
-                _num = Decimal(self.lambda_) ** Decimal(i)
+                _denom = Decimal(lambda_) ** Decimal((nu_ - 1) / (2 * nu_))
+                _denom *= Decimal(2 * math.pi) ** Decimal((nu_ - 1) / 2)
+                _denom *= Decimal(math.sqrt(nu_))
+                _o_lambda = Decimal(1) / (Decimal(lambda_) ** Decimal(1 / nu_))
                 _dec = True
 
             if _dec:
                 _denom = Decimal(_denom)
                 _num = Decimal(_num)
-            z_i += float(_num / _denom)
+                _o_lambda = Decimal(_o_lambda)
+
+            # Compute the ratio
+            z_i = float(_num / _denom) * (1 + float(_o_lambda))
+        else:
+            # ## Almost exact form
+            z_i = - np.inf
+            z_last = 0
+            current_j = 0
+
+            while (np.abs(z_i - z_last) > self.eps) & (current_j < j):
+                z_last = z_i
+                _log_fact = np.sum(np.log(range(1, current_j)))
+                z_i = self.log_sum(z_i, current_j * math.log(lambda_) - nu_ * _log_fact)
+                current_j += 1
+
+            if not log:
+                z_i = math.exp(z_i)
 
         return float(np.sum(z_i))
 
+    def log_sum(self, x, y):
+        if x == -np.inf:
+            return y
+        elif y == -np.inf:
+            return x
+        elif x > y:
+            return x + math.log(1 + math.exp(y - x))
+        else:
+            return y + math.log(1 + math.exp(x - y))
+
     def pmf(self, x) -> float:
         """Computes the probability mass function for selected value :obj:`x`.
 
         :formula: The probability mass function (pmf) is computed by
 
             .. math:: \\mathbb{P}(X = x | \\lambda, \\nu) = \\dfrac{\\lambda^{x}}{(x!)^{\\nu}} \\dfrac{1}{Z(\\lambda, \\nu)}
 
@@ -404,78 +450,45 @@
             # If decimal was used for power calculations, we have to use the same for factorial
             _fact = [Decimal(p) for p in _fact]
 
         a = np.array([float(p / f) for p, f in zip(_pow, _fact)])
         return a * (1 / self._Z)
 
     @staticmethod
-    def nloglike(params, data, j=100) -> float:
+    def nloglike(params, data, Z, j=100, approx=False) -> float:
         """Static method to estumate the negative likelihood (used in :meth:`statinf.distributions.discrete.CMPoisson.fit` method).
 
         :formula: The log-likelihood function :math:`l` is defined by
 
             .. math:: \\mathcal{l}(x_1, ..., x_n | \\lambda, \\nu) = \\log (\\lambda) \\sum_{i}^{n} {x_i} - \\nu \\sum_{i}^{n} {\\log (x_i!)} - n \\log (Z(\\lambda, \\nu))
 
         :param params: List of parameters :math:`\\lambda` and :math:`\\nu`
         :type params: :obj:`list`
         :param data: Data to evaluate the netative log-likelihood on
         :type data: :obj:`numpy.array` or :obj:`list` or :obj:`pandas.Series`
         :param j: Length of the inifinite sum for the normalizing factor :math:`Z`, defaults to 100
         :type j: :obj:`int`, optional
+        :param approx: Use approximation form for computing :math:`Z(\\lambda, \\nu)`, defaults to False
+        :type approx: :obj:`bool`
 
         :return: Negative log-likelihood
         :rtype: :obj:`float`
         """
         lambda_ = params[0]
         nu_ = params[1]
         X = np.asarray(data)
 
-        z_i = 0
-        for i in range(j):
-            _dec = False
-            # We use a decimal placeholder variable in case we encounter overflow errors (number is too long).
-            # We don't use decimal as a default but only in case of error because it slows down computations,
-            # therefore, by default we use light and simple format and call Decimal when needed.
-            # For instances where we need Decimal, we will transform back the ratio of decimals to float as
-            # the value will be of reasonable size and not too long for a classical float.
-
-            # Compute denominator
-            try:
-                # Try normal formula
-                _denom = math.factorial(i) ** nu_
-            except OverflowError:
-                # If overflow error (i.e. output is too long), use Decimal format
-                _denom = Decimal(math.factorial(i)) ** Decimal(nu_)
-                _dec = True
-
-            # Compute numerator
-            try:
-                _num = lambda_ ** i
-            except RuntimeWarning:
-                # If runtime warning it is similar to overflow error (i.e. output is too long), use Decimal format
-                _num = Decimal(lambda_) ** Decimal(i)
-                _dec = True
-
-            # If decimal was used
-            if _dec:
-                # If decimal was used for one of denominator or denominator, we apply decimal to all (for format consistency)
-                _denom = Decimal(_denom)
-                _num = Decimal(_num)
-
-            # Then compute the ratio and transform to float (whether decimal was used or not)
-            z_i += float(_num / _denom)
-
         # Compute log(Z)
-        log_Z = np.log(z_i)
+        log_Z = Z(lambda_=lambda_, nu_=nu_, j=j, approx=approx, log=True)
 
         _log_fact = np.asarray([math.log(math.factorial(_x)) for _x in X])
         ll = (math.log(lambda_) * np.sum(X)) - (nu_ * np.sum(_log_fact)) - (len(X) * log_Z)
         return -ll
 
-    def fit(self, data, method='L-BFGS-B', init_params=np.array([1., 1.]), j=None) -> dict:
+    def fit(self, data, method='L-BFGS-B', init_params=np.array([1., 1.]), j=None, approx=False) -> dict:
         """Estimates the parameters :math:`\\lambda` and :math:`\\nu` of the distribution from empirical data based on Maximum Likelihood Estimation.
 
         .. note::
 
             There is no close form to estimate the parameters nor a direct relation between the empirical moments (:math:`\\bar{X}`) and the theoretical ones.
             Therefore, only MLE is available (no fast method).
 
@@ -486,23 +499,23 @@
         :param init_params: Initial parameters for the optimization method, defaults to obj:`np.array([1., 1.])`
         :type init_params: obj:`numpy.array`, optional
 
         :return: Estimated parameters
         :rtype: obj:`dict`
         """
         # We transform warnings as error (for overflow) to handle in try / except: https://stackoverflow.com/questions/5644836/
-        warnings.filterwarnings("error")
         j = j if j else self.j
         bounds = [(self.eps, None), (self.eps, None)]
 
-        res = self._fit(data=data, bounds=bounds, method=method, init_params=init_params, args=(j,))
+        res = self._fit(data=data, bounds=bounds, method=method, init_params=init_params, args=(j, approx))
         self.lambda_ = res.x[0]
         self.nu_ = res.x[1]
-        self._Z = self.Z()
+        warnings.filterwarnings("error")
+        self._Z = self.Z(lambda_=self.lambda_, nu_=self.nu_, j=j, approx=approx)
         warnings.resetwarnings()
 
-        out = {'lambda_': self.lambda_, 'nu_': self.nu_}
+        out = {'lambda_': self.lambda_, 'nu_': self.nu_, 'convergence': res.success}
 
         if method in scipy_methods:
             out.update({'nll': self.nll})
 
         return out
```

### Comparing `statinf-1.2.1/statinf/misc.py` & `statinf-1.2.2/statinf/misc.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/statinf/ml/activations.py` & `statinf-1.2.2/statinf/ml/activations.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/statinf/ml/initializations.py` & `statinf-1.2.2/statinf/ml/initializations.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/statinf/ml/losses.py` & `statinf-1.2.2/statinf/ml/losses.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/statinf/ml/neuralnetwork.py` & `statinf-1.2.2/statinf/ml/neuralnetwork.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/statinf/ml/optimizers.py` & `statinf-1.2.2/statinf/ml/optimizers.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/statinf/ml/performance.py` & `statinf-1.2.2/statinf/ml/performance.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/statinf/nonparametrics/kernels.py` & `statinf-1.2.2/statinf/nonparametrics/kernels.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/statinf/regressions/LinearModels.py` & `statinf-1.2.2/statinf/regressions/LinearModels.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/statinf/regressions/glm.py` & `statinf-1.2.2/statinf/regressions/glm.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/statinf/regressions/glm_test.py` & `statinf-1.2.2/statinf/regressions/glm_test.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/statinf/stats/bayesian.py` & `statinf-1.2.2/statinf/stats/bayesian.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/statinf/stats/descriptive.py` & `statinf-1.2.2/statinf/stats/descriptive.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/statinf/stats/tests.py` & `statinf-1.2.2/statinf/stats/tests.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/statinf/stats/timeseries.py` & `statinf-1.2.2/statinf/stats/timeseries.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/statinf/stats/unsupervised.py` & `statinf-1.2.2/statinf/stats/unsupervised.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.1/statinf.egg-info/PKG-INFO` & `statinf-1.2.2/statinf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statinf
-Version: 1.2.1
+Version: 1.2.2
 Summary: A library for statistics and causal inference
 Home-page: https://www.florianfelice.com/statinf
 Author: Florian Felice
 Author-email: florian.felice@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `statinf-1.2.1/statinf.egg-info/SOURCES.txt` & `statinf-1.2.2/statinf.egg-info/SOURCES.txt`

 * *Files identical despite different names*


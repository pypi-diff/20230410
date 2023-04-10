# Comparing `tmp/inFairness-0.2.2.tar.gz` & `tmp/inFairness-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inFairness-0.2.2.tar", last modified: Tue Sep  6 19:57:21 2022, max compression
+gzip compressed data, was "inFairness-0.2.3.tar", last modified: Mon Apr 10 19:16:10 2023, max compression
```

## Comparing `inFairness-0.2.2.tar` & `inFairness-0.2.3.tar`

### file list

```diff
@@ -1,48 +1,52 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-09-06 19:57:21.081925 inFairness-0.2.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2022-09-06 19:54:49.000000 inFairness-0.2.2/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     7712 2022-09-06 19:57:21.081925 inFairness-0.2.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     7232 2022-09-06 19:54:49.000000 inFairness-0.2.2/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-09-06 19:57:21.057922 inFairness-0.2.2/inFairness/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-09-06 19:57:21.057922 inFairness-0.2.2/inFairness/auditor/
--rw-rw-r--   0 travis    (2000) travis    (2000)      233 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/auditor/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4199 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/auditor/auditor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      342 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/auditor/datainterface.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5904 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/auditor/sensei_auditor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5871 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/auditor/sensr_auditor.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-09-06 19:57:21.065923 inFairness-0.2.2/inFairness/distances/
--rw-rw-r--   0 travis    (2000) travis    (2000)      717 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/distances/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      695 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/distances/distance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2193 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/distances/euclidean_dists.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4155 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/distances/explore_distance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7716 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/distances/logistic_sensitive_subspace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5129 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/distances/mahalanobis_distance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5490 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/distances/sensitive_subspace_dist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1924 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/distances/wasserstein_distance.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-09-06 19:57:21.069923 inFairness-0.2.2/inFairness/fairalgo/
--rw-rw-r--   0 travis    (2000) travis    (2000)      223 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/fairalgo/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      212 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/fairalgo/datainterfaces.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3743 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/fairalgo/sensei.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3534 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/fairalgo/sensr.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-09-06 19:57:21.069923 inFairness-0.2.2/inFairness/postprocessing/
--rw-rw-r--   0 travis    (2000) travis    (2000)      206 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/postprocessing/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2253 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/postprocessing/base_postprocessing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2843 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/postprocessing/data_ds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      256 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/postprocessing/datainterfaces.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1604 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/postprocessing/distance_ds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11440 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/postprocessing/glif.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-09-06 19:57:21.069923 inFairness-0.2.2/inFairness/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4492 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/utils/datautils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      953 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/utils/misc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      475 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/utils/params.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2900 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/utils/postprocessing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      475 2022-09-06 19:54:49.000000 inFairness-0.2.2/inFairness/utils/validationutils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-09-06 19:57:21.069923 inFairness-0.2.2/inFairness.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7712 2022-09-06 19:57:20.000000 inFairness-0.2.2/inFairness.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1349 2022-09-06 19:57:21.000000 inFairness-0.2.2/inFairness.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-09-06 19:57:20.000000 inFairness-0.2.2/inFairness.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      104 2022-09-06 19:57:20.000000 inFairness-0.2.2/inFairness.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2022-09-06 19:57:20.000000 inFairness-0.2.2/inFairness.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       79 2022-09-06 19:57:21.081925 inFairness-0.2.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1060 2022-09-06 19:54:49.000000 inFairness-0.2.2/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-10 19:16:10.101023 inFairness-0.2.3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2023-04-10 19:13:21.000000 inFairness-0.2.3/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7893 2023-04-10 19:16:10.101023 inFairness-0.2.3/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7413 2023-04-10 19:13:21.000000 inFairness-0.2.3/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-10 19:16:10.093022 inFairness-0.2.3/inFairness/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-10 19:16:10.093022 inFairness-0.2.3/inFairness/auditor/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      295 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/auditor/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4199 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/auditor/auditor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      342 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/auditor/datainterface.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5904 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/auditor/sensei_auditor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5871 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/auditor/sensr_auditor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4386 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/auditor/senstir_auditor.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-10 19:16:10.097023 inFairness-0.2.3/inFairness/distances/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      717 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/distances/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1196 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/distances/distance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2264 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/distances/euclidean_dists.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4287 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/distances/explore_distance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8395 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/distances/logistic_sensitive_subspace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5180 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/distances/mahalanobis_distance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5490 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/distances/sensitive_subspace_dist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1924 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/distances/wasserstein_distance.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-10 19:16:10.097023 inFairness-0.2.3/inFairness/fairalgo/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      271 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/fairalgo/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      212 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/fairalgo/datainterfaces.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3743 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/fairalgo/sensei.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3534 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/fairalgo/sensr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5938 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/fairalgo/senstir.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-10 19:16:10.101023 inFairness-0.2.3/inFairness/postprocessing/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      206 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/postprocessing/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2253 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/postprocessing/base_postprocessing.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2843 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/postprocessing/data_ds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      256 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/postprocessing/datainterfaces.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1604 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/postprocessing/distance_ds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11440 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/postprocessing/glif.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-10 19:16:10.101023 inFairness-0.2.3/inFairness/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4492 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/utils/datautils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      953 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/utils/misc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1822 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/utils/ndcg.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      475 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/utils/params.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5646 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/utils/plackett_luce.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2900 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/utils/postprocessing.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      475 2023-04-10 19:13:21.000000 inFairness-0.2.3/inFairness/utils/validationutils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-10 19:16:10.101023 inFairness-0.2.3/inFairness.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7893 2023-04-10 19:16:10.000000 inFairness-0.2.3/inFairness.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1485 2023-04-10 19:16:10.000000 inFairness-0.2.3/inFairness.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-10 19:16:10.000000 inFairness-0.2.3/inFairness.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       87 2023-04-10 19:16:10.000000 inFairness-0.2.3/inFairness.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2023-04-10 19:16:10.000000 inFairness-0.2.3/inFairness.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       79 2023-04-10 19:16:10.101023 inFairness-0.2.3/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1031 2023-04-10 19:13:21.000000 inFairness-0.2.3/setup.py
```

### Comparing `inFairness-0.2.2/LICENSE` & `inFairness-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `inFairness-0.2.2/PKG-INFO` & `inFairness-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inFairness
-Version: 0.2.2
+Version: 0.2.3
 Summary: inFairness is a Python package to train and audit individually fair PyTorch models
 Home-page: https://github.com/IBM/inFairness
 Author: IBM Research
 Author-email: mayank.agarwal@ibm.com, aldo.pareja@ibm.com, onkarbhardwaj@ibm.com, mikhail.yurochkin@ibm.com
 Keywords: individual fairness,ai fairness,trustworthy ai,machine learning
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -16,17 +16,18 @@
    </a>
 </p>
 
 <p align="center">
    <a href="https://pypi.org/project/infairness"><img src="https://img.shields.io/pypi/v/infairness?color=important&label=pypi%20package&logo=PyPy"></a>
    <a href="./examples"><img src="https://img.shields.io/badge/example-notebooks-red?logo=jupyter"></a>
    <a href="https://ibm.github.io/inFairness"><img src="https://img.shields.io/badge/documentation-up-green?logo=GitBook"></a>
+   <a href="https://fairbert.vizhub.ai"><img src="https://img.shields.io/badge/fairness-demonstration-yellow?logo=ibm-watson"></a>
    <br/>
    <a href="https://app.travis-ci.com/IBM/inFairness"><img src="https://app.travis-ci.com/IBM/inFairness.svg?branch=main"></a>
-   <a href="https://pepy.tech/project/infairness"><img src="https://pepy.tech/badge/infairness"></a>
+   <a href="https://pypistats.org/packages/infairness"><img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/inFairness?color=blue"></a>
    <a href="https://www.python.org/"><img src="https://img.shields.io/badge/python-3.7+-blue?logo=python"></a>
    <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/license-Apache-yellow"></a>
    <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 
 ## Individual Fairness and inFairness
@@ -35,15 +36,15 @@
 
 $$ d_y (h(x_1), h(x_2)) \leq L d_x(x_1, x_2) \quad \forall \quad x_1, x_2 \in X $$
 
 Here, $h: X \rightarrow Y$ is a ML model, where $X$ and $Y$ are input and output spaces; $d_x$ and $d_y$ are metrics on the input and output spaces, and $L \geq 0$ is a Lipchitz constant. This constrained optimization equation states that the distance between the model predictions for inputs $x_1$ and $x_2$ is upper-bounded by the fair distance between the inputs $x_1$ and $x_2$. Here, the fair metric $d_x$ encodes our intuition of which samples should be treated similarly by the ML model, and in designing so, we ensure that for input samples considered similar by the fair metric $d_x$, the model outputs will be similar as well.
 
 inFairness is a PyTorch package that supports auditing, training, and post-processing ML models for individual fairness. At its core, the library implements the key components of individual fairness pipeline: $d_x$ - distance in the input space, $d_y$ - distance in the output space, and the learning algorithms to optimize for the equation above.
 
-For an in-depth tutorial of Individual Fairness and the inFairness package, please watch this tutorial. Also, take a look at the [examples](./examples/) folder for illustrative use-cases. For more group fairness examples see [AIF360](https://aif360.mybluemix.net/).
+For an in-depth tutorial of Individual Fairness and the inFairness package, please watch this tutorial. Also, take a look at the [examples](./examples/) folder for illustrative use-cases and try the [Fairness Playground demo](https://fairbert.vizhub.ai). For more group fairness examples see [AIF360](https://aif360.mybluemix.net/).
 
 <p align="center">
   <a href="https://video.ibm.com/recorded/131932983" target="_blank"><img width="700" alt="Watch the tutorial" src="https://user-images.githubusercontent.com/991913/178768336-2bfa5958-487f-4f14-a156-03dacfd68263.png"></a>
 </p>
 
 ## Installation
 
@@ -68,20 +69,15 @@
 
 inFairness currently supports:
 
 1. Learning individually fair metrics : [[Docs]](https://ibm.github.io/inFairness/reference/distances.html)
 2. Training of individually fair models : [[Docs]](https://ibm.github.io/inFairness/reference/algorithms.html)
 3. Auditing pre-trained ML models for individual fairness : [[Docs]](https://ibm.github.io/inFairness/reference/auditors.html)
 4. Post-processing for Individual Fairness : [[Docs]](https://ibm.github.io/inFairness/reference/postprocessing.html)
-
-
-### Coming soon
-
-We plan to extend the package by integrating the following features:
-1. Individually fair ranking : [[Paper]](https://arxiv.org/abs/2103.11023)
+5. Individually fair ranking : [[Docs]](https://ibm.github.io/inFairness/reference/algorithms.html)
 
 
 ## Contributing
 
 We welcome contributions from the community in any form - whether it is through the contribution of a new fair algorithm, fair metric, a new use-case, or simply reporting an issue or enhancement in the package. To contribute code to the package, please follow the following steps:
 
 1. Clone this git repository to your local system
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: inFairness Version: 0.2.2 Summary: inFairness is a
+Metadata-Version: 2.1 Name: inFairness Version: 0.2.3 Summary: inFairness is a
 Python package to train and audit individually fair PyTorch models Home-page:
 https://github.com/IBM/inFairness Author: IBM Research Author-email:
 mayank.agarwal@ibm.com, aldo.pareja@ibm.com, onkarbhardwaj@ibm.com,
 mikhail.yurochkin@ibm.com Keywords: individual fairness,ai fairness,trustworthy
 ai,machine learning Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE
         [https://ibm.github.io/inFairness/_static/infairness-logo.png]
                         [https://img.shields.io/pypi/v/
      infairness?color=important&label=pypi%20package&logo=PyPy] [https://
       img.shields.io/badge/example-notebooks-red?logo=jupyter] [https://
-          img.shields.io/badge/documentation-up-green?logo=GitBook]
-[https://app.travis-ci.com/IBM/inFairness.svg?branch=main] [https://pepy.tech/
-badge/infairness] [https://img.shields.io/badge/python-3.7+-blue?logo=python]
- [https://img.shields.io/badge/license-Apache-yellow] [https://img.shields.io/
-                     badge/code%20style-black-000000.svg]
+      img.shields.io/badge/documentation-up-green?logo=GitBook] [https://
+     img.shields.io/badge/fairness-demonstration-yellow?logo=ibm-watson]
+[https://app.travis-ci.com/IBM/inFairness.svg?branch=main] [PyPI_-_Downloads]
+     [https://img.shields.io/badge/python-3.7+-blue?logo=python] [https://
+  img.shields.io/badge/license-Apache-yellow] [https://img.shields.io/badge/
+                        code%20style-black-000000.svg]
 ## Individual Fairness and inFairness Intuitively, an individually fair Machine
 Learning (ML) model treats similar inputs similarly. Formally, the leading
 notion of individual fairness is metric fairness [(Dwork et al., 2011)](https:/
 /dl.acm.org/doi/abs/10.1145/2090236.2090255); it requires: $$ d_y (h(x_1), h
 (x_2)) \leq L d_x(x_1, x_2) \quad \forall \quad x_1, x_2 \in X $$ Here, $h: X
 \rightarrow Y$ is a ML model, where $X$ and $Y$ are input and output spaces;
 $d_x$ and $d_y$ are metrics on the input and output spaces, and $L \geq 0$ is a
@@ -30,37 +31,36 @@
 as well. inFairness is a PyTorch package that supports auditing, training, and
 post-processing ML models for individual fairness. At its core, the library
 implements the key components of individual fairness pipeline: $d_x$ - distance
 in the input space, $d_y$ - distance in the output space, and the learning
 algorithms to optimize for the equation above. For an in-depth tutorial of
 Individual Fairness and the inFairness package, please watch this tutorial.
 Also, take a look at the [examples](./examples/) folder for illustrative use-
-cases. For more group fairness examples see [AIF360](https://
-aif360.mybluemix.net/).
+cases and try the [Fairness Playground demo](https://fairbert.vizhub.ai). For
+more group fairness examples see [AIF360](https://aif360.mybluemix.net/).
                              [Watch_the_tutorial]
 ## Installation inFairness can be installed using `pip`: ``` pip install
 inFairness ``` Alternatively, if you wish to install the latest development
 version, you can install directly by cloning this repository: ``` git clone  cd
 inFairness pip install -e . ``` ## Features inFairness currently supports: 1.
 Learning individually fair metrics : [[Docs]](https://ibm.github.io/inFairness/
 reference/distances.html) 2. Training of individually fair models : [[Docs]]
 (https://ibm.github.io/inFairness/reference/algorithms.html) 3. Auditing pre-
 trained ML models for individual fairness : [[Docs]](https://ibm.github.io/
 inFairness/reference/auditors.html) 4. Post-processing for Individual Fairness
-: [[Docs]](https://ibm.github.io/inFairness/reference/postprocessing.html) ###
-Coming soon We plan to extend the package by integrating the following
-features: 1. Individually fair ranking : [[Paper]](https://arxiv.org/abs/
-2103.11023) ## Contributing We welcome contributions from the community in any
-form - whether it is through the contribution of a new fair algorithm, fair
-metric, a new use-case, or simply reporting an issue or enhancement in the
-package. To contribute code to the package, please follow the following steps:
-1. Clone this git repository to your local system 2. Setup your system by
-installing dependencies as: `pip3 install -r requirements.txt` and `pip3
-install -r build_requirements.txt` 3. Add your code contribution to the
-package. Please refer to the [`inFairness`](./inFairness) folder for an
+: [[Docs]](https://ibm.github.io/inFairness/reference/postprocessing.html) 5.
+Individually fair ranking : [[Docs]](https://ibm.github.io/inFairness/
+reference/algorithms.html) ## Contributing We welcome contributions from the
+community in any form - whether it is through the contribution of a new fair
+algorithm, fair metric, a new use-case, or simply reporting an issue or
+enhancement in the package. To contribute code to the package, please follow
+the following steps: 1. Clone this git repository to your local system 2. Setup
+your system by installing dependencies as: `pip3 install -r requirements.txt`
+and `pip3 install -r build_requirements.txt` 3. Add your code contribution to
+the package. Please refer to the [`inFairness`](./inFairness) folder for an
 overview of the directory structure 4. Add appropriate unit tests in the
 [`tests`](./tests) folder 5. Once you are ready to commit code, check for the
 following: 1. Coding style compliance using: `flake8 inFairness/`. This command
 will list all stylistic violations found in the code. Please try to fix as much
 as you can 2. Ensure all the test cases pass using: `coverage run --source
 inFairness -m pytest tests/`. All unit tests need to pass to be able merge code
 in the package. 6. Finally, commit your code and raise a Pull Request. ##
```

### Comparing `inFairness-0.2.2/README.md` & `inFairness-0.2.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,18 @@
    </a>
 </p>
 
 <p align="center">
    <a href="https://pypi.org/project/infairness"><img src="https://img.shields.io/pypi/v/infairness?color=important&label=pypi%20package&logo=PyPy"></a>
    <a href="./examples"><img src="https://img.shields.io/badge/example-notebooks-red?logo=jupyter"></a>
    <a href="https://ibm.github.io/inFairness"><img src="https://img.shields.io/badge/documentation-up-green?logo=GitBook"></a>
+   <a href="https://fairbert.vizhub.ai"><img src="https://img.shields.io/badge/fairness-demonstration-yellow?logo=ibm-watson"></a>
    <br/>
    <a href="https://app.travis-ci.com/IBM/inFairness"><img src="https://app.travis-ci.com/IBM/inFairness.svg?branch=main"></a>
-   <a href="https://pepy.tech/project/infairness"><img src="https://pepy.tech/badge/infairness"></a>
+   <a href="https://pypistats.org/packages/infairness"><img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/inFairness?color=blue"></a>
    <a href="https://www.python.org/"><img src="https://img.shields.io/badge/python-3.7+-blue?logo=python"></a>
    <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/license-Apache-yellow"></a>
    <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 
 ## Individual Fairness and inFairness
@@ -23,15 +24,15 @@
 
 $$ d_y (h(x_1), h(x_2)) \leq L d_x(x_1, x_2) \quad \forall \quad x_1, x_2 \in X $$
 
 Here, $h: X \rightarrow Y$ is a ML model, where $X$ and $Y$ are input and output spaces; $d_x$ and $d_y$ are metrics on the input and output spaces, and $L \geq 0$ is a Lipchitz constant. This constrained optimization equation states that the distance between the model predictions for inputs $x_1$ and $x_2$ is upper-bounded by the fair distance between the inputs $x_1$ and $x_2$. Here, the fair metric $d_x$ encodes our intuition of which samples should be treated similarly by the ML model, and in designing so, we ensure that for input samples considered similar by the fair metric $d_x$, the model outputs will be similar as well.
 
 inFairness is a PyTorch package that supports auditing, training, and post-processing ML models for individual fairness. At its core, the library implements the key components of individual fairness pipeline: $d_x$ - distance in the input space, $d_y$ - distance in the output space, and the learning algorithms to optimize for the equation above.
 
-For an in-depth tutorial of Individual Fairness and the inFairness package, please watch this tutorial. Also, take a look at the [examples](./examples/) folder for illustrative use-cases. For more group fairness examples see [AIF360](https://aif360.mybluemix.net/).
+For an in-depth tutorial of Individual Fairness and the inFairness package, please watch this tutorial. Also, take a look at the [examples](./examples/) folder for illustrative use-cases and try the [Fairness Playground demo](https://fairbert.vizhub.ai). For more group fairness examples see [AIF360](https://aif360.mybluemix.net/).
 
 <p align="center">
   <a href="https://video.ibm.com/recorded/131932983" target="_blank"><img width="700" alt="Watch the tutorial" src="https://user-images.githubusercontent.com/991913/178768336-2bfa5958-487f-4f14-a156-03dacfd68263.png"></a>
 </p>
 
 ## Installation
 
@@ -56,20 +57,15 @@
 
 inFairness currently supports:
 
 1. Learning individually fair metrics : [[Docs]](https://ibm.github.io/inFairness/reference/distances.html)
 2. Training of individually fair models : [[Docs]](https://ibm.github.io/inFairness/reference/algorithms.html)
 3. Auditing pre-trained ML models for individual fairness : [[Docs]](https://ibm.github.io/inFairness/reference/auditors.html)
 4. Post-processing for Individual Fairness : [[Docs]](https://ibm.github.io/inFairness/reference/postprocessing.html)
-
-
-### Coming soon
-
-We plan to extend the package by integrating the following features:
-1. Individually fair ranking : [[Paper]](https://arxiv.org/abs/2103.11023)
+5. Individually fair ranking : [[Docs]](https://ibm.github.io/inFairness/reference/algorithms.html)
 
 
 ## Contributing
 
 We welcome contributions from the community in any form - whether it is through the contribution of a new fair algorithm, fair metric, a new use-case, or simply reporting an issue or enhancement in the package. To contribute code to the package, please follow the following steps:
 
 1. Clone this git repository to your local system
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
         [https://ibm.github.io/inFairness/_static/infairness-logo.png]
                         [https://img.shields.io/pypi/v/
      infairness?color=important&label=pypi%20package&logo=PyPy] [https://
       img.shields.io/badge/example-notebooks-red?logo=jupyter] [https://
-          img.shields.io/badge/documentation-up-green?logo=GitBook]
-[https://app.travis-ci.com/IBM/inFairness.svg?branch=main] [https://pepy.tech/
-badge/infairness] [https://img.shields.io/badge/python-3.7+-blue?logo=python]
- [https://img.shields.io/badge/license-Apache-yellow] [https://img.shields.io/
-                     badge/code%20style-black-000000.svg]
+      img.shields.io/badge/documentation-up-green?logo=GitBook] [https://
+     img.shields.io/badge/fairness-demonstration-yellow?logo=ibm-watson]
+[https://app.travis-ci.com/IBM/inFairness.svg?branch=main] [PyPI_-_Downloads]
+     [https://img.shields.io/badge/python-3.7+-blue?logo=python] [https://
+  img.shields.io/badge/license-Apache-yellow] [https://img.shields.io/badge/
+                        code%20style-black-000000.svg]
 ## Individual Fairness and inFairness Intuitively, an individually fair Machine
 Learning (ML) model treats similar inputs similarly. Formally, the leading
 notion of individual fairness is metric fairness [(Dwork et al., 2011)](https:/
 /dl.acm.org/doi/abs/10.1145/2090236.2090255); it requires: $$ d_y (h(x_1), h
 (x_2)) \leq L d_x(x_1, x_2) \quad \forall \quad x_1, x_2 \in X $$ Here, $h: X
 \rightarrow Y$ is a ML model, where $X$ and $Y$ are input and output spaces;
 $d_x$ and $d_y$ are metrics on the input and output spaces, and $L \geq 0$ is a
@@ -23,37 +24,36 @@
 as well. inFairness is a PyTorch package that supports auditing, training, and
 post-processing ML models for individual fairness. At its core, the library
 implements the key components of individual fairness pipeline: $d_x$ - distance
 in the input space, $d_y$ - distance in the output space, and the learning
 algorithms to optimize for the equation above. For an in-depth tutorial of
 Individual Fairness and the inFairness package, please watch this tutorial.
 Also, take a look at the [examples](./examples/) folder for illustrative use-
-cases. For more group fairness examples see [AIF360](https://
-aif360.mybluemix.net/).
+cases and try the [Fairness Playground demo](https://fairbert.vizhub.ai). For
+more group fairness examples see [AIF360](https://aif360.mybluemix.net/).
                              [Watch_the_tutorial]
 ## Installation inFairness can be installed using `pip`: ``` pip install
 inFairness ``` Alternatively, if you wish to install the latest development
 version, you can install directly by cloning this repository: ``` git clone  cd
 inFairness pip install -e . ``` ## Features inFairness currently supports: 1.
 Learning individually fair metrics : [[Docs]](https://ibm.github.io/inFairness/
 reference/distances.html) 2. Training of individually fair models : [[Docs]]
 (https://ibm.github.io/inFairness/reference/algorithms.html) 3. Auditing pre-
 trained ML models for individual fairness : [[Docs]](https://ibm.github.io/
 inFairness/reference/auditors.html) 4. Post-processing for Individual Fairness
-: [[Docs]](https://ibm.github.io/inFairness/reference/postprocessing.html) ###
-Coming soon We plan to extend the package by integrating the following
-features: 1. Individually fair ranking : [[Paper]](https://arxiv.org/abs/
-2103.11023) ## Contributing We welcome contributions from the community in any
-form - whether it is through the contribution of a new fair algorithm, fair
-metric, a new use-case, or simply reporting an issue or enhancement in the
-package. To contribute code to the package, please follow the following steps:
-1. Clone this git repository to your local system 2. Setup your system by
-installing dependencies as: `pip3 install -r requirements.txt` and `pip3
-install -r build_requirements.txt` 3. Add your code contribution to the
-package. Please refer to the [`inFairness`](./inFairness) folder for an
+: [[Docs]](https://ibm.github.io/inFairness/reference/postprocessing.html) 5.
+Individually fair ranking : [[Docs]](https://ibm.github.io/inFairness/
+reference/algorithms.html) ## Contributing We welcome contributions from the
+community in any form - whether it is through the contribution of a new fair
+algorithm, fair metric, a new use-case, or simply reporting an issue or
+enhancement in the package. To contribute code to the package, please follow
+the following steps: 1. Clone this git repository to your local system 2. Setup
+your system by installing dependencies as: `pip3 install -r requirements.txt`
+and `pip3 install -r build_requirements.txt` 3. Add your code contribution to
+the package. Please refer to the [`inFairness`](./inFairness) folder for an
 overview of the directory structure 4. Add appropriate unit tests in the
 [`tests`](./tests) folder 5. Once you are ready to commit code, check for the
 following: 1. Coding style compliance using: `flake8 inFairness/`. This command
 will list all stylistic violations found in the code. Please try to fix as much
 as you can 2. Ensure all the test cases pass using: `coverage run --source
 inFairness -m pytest tests/`. All unit tests need to pass to be able merge code
 in the package. 6. Finally, commit your code and raise a Pull Request. ##
```

### Comparing `inFairness-0.2.2/inFairness/auditor/auditor.py` & `inFairness-0.2.3/inFairness/auditor/auditor.py`

 * *Files identical despite different names*

### Comparing `inFairness-0.2.2/inFairness/auditor/sensei_auditor.py` & `inFairness-0.2.3/inFairness/auditor/sensei_auditor.py`

 * *Files identical despite different names*

### Comparing `inFairness-0.2.2/inFairness/auditor/sensr_auditor.py` & `inFairness-0.2.3/inFairness/auditor/sensr_auditor.py`

 * *Files identical despite different names*

### Comparing `inFairness-0.2.2/inFairness/distances/__init__.py` & `inFairness-0.2.3/inFairness/distances/__init__.py`

 * *Files identical despite different names*

### Comparing `inFairness-0.2.2/inFairness/distances/euclidean_dists.py` & `inFairness-0.2.3/inFairness/distances/euclidean_dists.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 
 class ProtectedEuclideanDistance(Distance):
     def __init__(self):
         super().__init__()
 
         self._protected_attributes = None
         self._num_attributes = None
-        self.protected_vector = None
+        self.register_buffer("protected_vector", torch.Tensor())
 
     def to(self, device):
         """Moves distance metric to a particular device
 
         Parameters
         ------------
             device: torch.device
         """
 
         assert (
-            self.protected_vector is not None
+            self.protected_vector is not None and len(self.protected_vector.size()) != 0
         ), "Please fit the metric before moving parameters to device"
 
         self.device = device
         self.protected_vector = self.protected_vector.to(self.device)
 
     def fit(self, protected_attributes, num_attributes):
         """Fit Protected Euclidean Distance metric
```

### Comparing `inFairness-0.2.2/inFairness/distances/explore_distance.py` & `inFairness-0.2.3/inFairness/distances/explore_distance.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,17 @@
             autoinfer_device: bool
                 Should the distance metric be automatically moved to an appropriate
                 device (CPU / GPU) or not? If set to True, it moves the metric
                 to the same device `X1` is on. If set to False, keeps the metric
                 on CPU.
         """
 
+        assert (
+            X1.shape[0] == X2.shape[0] == Y.shape[0]
+        ), "Number of elements in X1, X2, and Y do not match"
         X = datautils.convert_tensor_to_numpy(X1 - X2)
         Y = datautils.convert_tensor_to_numpy(Y)
         sigma = self.compute_sigma(X, Y, iters, batchsize)
         super().fit(sigma)
 
         if autoinfer_device:
             device = datautils.get_device(X1)
```

### Comparing `inFairness-0.2.2/inFairness/distances/logistic_sensitive_subspace.py` & `inFairness-0.2.3/inFairness/distances/logistic_sensitive_subspace.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,24 @@
         `Yurochkin, Mikhail, Amanda Bower, and Yuekai Sun. "Training individually fair
         ML models with sensitive subspace robustness." arXiv preprint arXiv:1907.00020 (2019).`
     """
 
     def __init__(self):
         super().__init__()
         self.basis_vectors_ = None
+        self._logreg_models = None
+
+    @property
+    def logistic_regression_models(self):
+        """Logistic Regression models trained by the metric to predict each sensitive attribute
+        given inputs. The property is a list of logistic regression models each corresponding to
+        :math:`\mathbb{P}(K_i = l\\mid X_i)`. This property can be used to measure the performance
+        of the logistic regression models.
+        """
+        return self._logreg_models
 
     def fit(
         self,
         data_X: torch.Tensor,
         data_SensitiveAttrs: torch.Tensor = None,
         protected_idxs: Iterable[int] = None,
         keep_protected_idxs: bool = True,
@@ -111,19 +121,23 @@
         protected_idxs = sorted(protected_idxs)
         free_idxs = [idx for idx in range(num_attr) if idx not in protected_idxs]
         X_train = data[:, free_idxs]
         Y_train = data[:, protected_idxs]
 
         self.__assert_sensitiveattrs_binary__(Y_train)
 
+        self._logreg_models = [
+            LogisticRegression(solver="liblinear", penalty="l1")
+            .fit(X_train, Y_train[:, idx])
+            for idx in range(len(protected_idxs))
+        ]
+
         coefs = np.array(
             [
-                LogisticRegression(solver="liblinear", penalty="l1")
-                .fit(X_train, Y_train[:, idx])
-                .coef_.squeeze()
+                self._logreg_models[idx].coef_.squeeze()
                 for idx in range(len(protected_idxs))
             ]
         )  # ( |protected_idxs|, |free_idxs| )
 
         if keep_protected_idxs:
             # To keep protected indices, we add two basis vectors
             # First, with logistic regression coefficients with 0 in
@@ -162,19 +176,23 @@
         y_train = datautils.convert_tensor_to_numpy(y_train)
 
         self.__assert_sensitiveattrs_binary__(y_train)
 
         basis_vectors_ = []
         outdim = y_train.shape[-1]
 
+        self._logreg_models = [
+            LogisticRegression(solver="liblinear", penalty="l1")
+            .fit(X_train, y_train[:, idx])
+            for idx in range(outdim)
+        ]
+
         basis_vectors_ = np.array(
             [
-                LogisticRegression(solver="liblinear", penalty="l1")
-                .fit(X_train, y_train[:, idx])
-                .coef_.squeeze()
+                self._logreg_models[idx].coef_.squeeze()
                 for idx in range(outdim)
             ]
         )
 
         basis_vectors_ = torch.tensor(basis_vectors_, dtype=dtype).T
         basis_vectors_ = basis_vectors_.detach()
```

### Comparing `inFairness-0.2.2/inFairness/distances/mahalanobis_distance.py` & `inFairness-0.2.3/inFairness/distances/mahalanobis_distance.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,29 +12,28 @@
 
     .. math:: \\text{dist}(X_1, X_2) = (X_1 - X_2) \\Sigma (X_1 - X_2)^{T}
     """
 
     def __init__(self):
         super().__init__()
 
-        self.sigma = None
         self.device = torch.device("cpu")
         self._vectorized_dist = None
-        
+        self.register_buffer("sigma", torch.Tensor())
 
     def to(self, device):
         """Moves distance metric to a particular device
 
         Parameters
         ------------
             device: torch.device
         """
 
         assert (
-            self.sigma is not None
+            self.sigma is not None and len(self.sigma.size()) != 0
         ), "Please fit the metric before moving parameters to device"
 
         self.device = device
         self.sigma = self.sigma.to(self.device)
 
     def fit(self, sigma):
         """Fit Mahalanobis Distance metric
```

### Comparing `inFairness-0.2.2/inFairness/distances/sensitive_subspace_dist.py` & `inFairness-0.2.3/inFairness/distances/sensitive_subspace_dist.py`

 * *Files identical despite different names*

### Comparing `inFairness-0.2.2/inFairness/distances/wasserstein_distance.py` & `inFairness-0.2.3/inFairness/distances/wasserstein_distance.py`

 * *Files identical despite different names*

### Comparing `inFairness-0.2.2/inFairness/fairalgo/sensei.py` & `inFairness-0.2.3/inFairness/fairalgo/sensei.py`

 * *Files identical despite different names*

### Comparing `inFairness-0.2.2/inFairness/fairalgo/sensr.py` & `inFairness-0.2.3/inFairness/fairalgo/sensr.py`

 * *Files identical despite different names*

### Comparing `inFairness-0.2.2/inFairness/postprocessing/base_postprocessing.py` & `inFairness-0.2.3/inFairness/postprocessing/base_postprocessing.py`

 * *Files identical despite different names*

### Comparing `inFairness-0.2.2/inFairness/postprocessing/data_ds.py` & `inFairness-0.2.3/inFairness/postprocessing/data_ds.py`

 * *Files identical despite different names*

### Comparing `inFairness-0.2.2/inFairness/postprocessing/distance_ds.py` & `inFairness-0.2.3/inFairness/postprocessing/distance_ds.py`

 * *Files identical despite different names*

### Comparing `inFairness-0.2.2/inFairness/postprocessing/glif.py` & `inFairness-0.2.3/inFairness/postprocessing/glif.py`

 * *Files identical despite different names*

### Comparing `inFairness-0.2.2/inFairness/utils/datautils.py` & `inFairness-0.2.3/inFairness/utils/datautils.py`

 * *Files identical despite different names*

### Comparing `inFairness-0.2.2/inFairness/utils/misc.py` & `inFairness-0.2.3/inFairness/utils/misc.py`

 * *Files identical despite different names*

### Comparing `inFairness-0.2.2/inFairness/utils/postprocessing.py` & `inFairness-0.2.3/inFairness/utils/postprocessing.py`

 * *Files identical despite different names*

### Comparing `inFairness-0.2.2/inFairness.egg-info/PKG-INFO` & `inFairness-0.2.3/inFairness.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inFairness
-Version: 0.2.2
+Version: 0.2.3
 Summary: inFairness is a Python package to train and audit individually fair PyTorch models
 Home-page: https://github.com/IBM/inFairness
 Author: IBM Research
 Author-email: mayank.agarwal@ibm.com, aldo.pareja@ibm.com, onkarbhardwaj@ibm.com, mikhail.yurochkin@ibm.com
 Keywords: individual fairness,ai fairness,trustworthy ai,machine learning
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -16,17 +16,18 @@
    </a>
 </p>
 
 <p align="center">
    <a href="https://pypi.org/project/infairness"><img src="https://img.shields.io/pypi/v/infairness?color=important&label=pypi%20package&logo=PyPy"></a>
    <a href="./examples"><img src="https://img.shields.io/badge/example-notebooks-red?logo=jupyter"></a>
    <a href="https://ibm.github.io/inFairness"><img src="https://img.shields.io/badge/documentation-up-green?logo=GitBook"></a>
+   <a href="https://fairbert.vizhub.ai"><img src="https://img.shields.io/badge/fairness-demonstration-yellow?logo=ibm-watson"></a>
    <br/>
    <a href="https://app.travis-ci.com/IBM/inFairness"><img src="https://app.travis-ci.com/IBM/inFairness.svg?branch=main"></a>
-   <a href="https://pepy.tech/project/infairness"><img src="https://pepy.tech/badge/infairness"></a>
+   <a href="https://pypistats.org/packages/infairness"><img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/inFairness?color=blue"></a>
    <a href="https://www.python.org/"><img src="https://img.shields.io/badge/python-3.7+-blue?logo=python"></a>
    <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/license-Apache-yellow"></a>
    <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 
 ## Individual Fairness and inFairness
@@ -35,15 +36,15 @@
 
 $$ d_y (h(x_1), h(x_2)) \leq L d_x(x_1, x_2) \quad \forall \quad x_1, x_2 \in X $$
 
 Here, $h: X \rightarrow Y$ is a ML model, where $X$ and $Y$ are input and output spaces; $d_x$ and $d_y$ are metrics on the input and output spaces, and $L \geq 0$ is a Lipchitz constant. This constrained optimization equation states that the distance between the model predictions for inputs $x_1$ and $x_2$ is upper-bounded by the fair distance between the inputs $x_1$ and $x_2$. Here, the fair metric $d_x$ encodes our intuition of which samples should be treated similarly by the ML model, and in designing so, we ensure that for input samples considered similar by the fair metric $d_x$, the model outputs will be similar as well.
 
 inFairness is a PyTorch package that supports auditing, training, and post-processing ML models for individual fairness. At its core, the library implements the key components of individual fairness pipeline: $d_x$ - distance in the input space, $d_y$ - distance in the output space, and the learning algorithms to optimize for the equation above.
 
-For an in-depth tutorial of Individual Fairness and the inFairness package, please watch this tutorial. Also, take a look at the [examples](./examples/) folder for illustrative use-cases. For more group fairness examples see [AIF360](https://aif360.mybluemix.net/).
+For an in-depth tutorial of Individual Fairness and the inFairness package, please watch this tutorial. Also, take a look at the [examples](./examples/) folder for illustrative use-cases and try the [Fairness Playground demo](https://fairbert.vizhub.ai). For more group fairness examples see [AIF360](https://aif360.mybluemix.net/).
 
 <p align="center">
   <a href="https://video.ibm.com/recorded/131932983" target="_blank"><img width="700" alt="Watch the tutorial" src="https://user-images.githubusercontent.com/991913/178768336-2bfa5958-487f-4f14-a156-03dacfd68263.png"></a>
 </p>
 
 ## Installation
 
@@ -68,20 +69,15 @@
 
 inFairness currently supports:
 
 1. Learning individually fair metrics : [[Docs]](https://ibm.github.io/inFairness/reference/distances.html)
 2. Training of individually fair models : [[Docs]](https://ibm.github.io/inFairness/reference/algorithms.html)
 3. Auditing pre-trained ML models for individual fairness : [[Docs]](https://ibm.github.io/inFairness/reference/auditors.html)
 4. Post-processing for Individual Fairness : [[Docs]](https://ibm.github.io/inFairness/reference/postprocessing.html)
-
-
-### Coming soon
-
-We plan to extend the package by integrating the following features:
-1. Individually fair ranking : [[Paper]](https://arxiv.org/abs/2103.11023)
+5. Individually fair ranking : [[Docs]](https://ibm.github.io/inFairness/reference/algorithms.html)
 
 
 ## Contributing
 
 We welcome contributions from the community in any form - whether it is through the contribution of a new fair algorithm, fair metric, a new use-case, or simply reporting an issue or enhancement in the package. To contribute code to the package, please follow the following steps:
 
 1. Clone this git repository to your local system
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: inFairness Version: 0.2.2 Summary: inFairness is a
+Metadata-Version: 2.1 Name: inFairness Version: 0.2.3 Summary: inFairness is a
 Python package to train and audit individually fair PyTorch models Home-page:
 https://github.com/IBM/inFairness Author: IBM Research Author-email:
 mayank.agarwal@ibm.com, aldo.pareja@ibm.com, onkarbhardwaj@ibm.com,
 mikhail.yurochkin@ibm.com Keywords: individual fairness,ai fairness,trustworthy
 ai,machine learning Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE
         [https://ibm.github.io/inFairness/_static/infairness-logo.png]
                         [https://img.shields.io/pypi/v/
      infairness?color=important&label=pypi%20package&logo=PyPy] [https://
       img.shields.io/badge/example-notebooks-red?logo=jupyter] [https://
-          img.shields.io/badge/documentation-up-green?logo=GitBook]
-[https://app.travis-ci.com/IBM/inFairness.svg?branch=main] [https://pepy.tech/
-badge/infairness] [https://img.shields.io/badge/python-3.7+-blue?logo=python]
- [https://img.shields.io/badge/license-Apache-yellow] [https://img.shields.io/
-                     badge/code%20style-black-000000.svg]
+      img.shields.io/badge/documentation-up-green?logo=GitBook] [https://
+     img.shields.io/badge/fairness-demonstration-yellow?logo=ibm-watson]
+[https://app.travis-ci.com/IBM/inFairness.svg?branch=main] [PyPI_-_Downloads]
+     [https://img.shields.io/badge/python-3.7+-blue?logo=python] [https://
+  img.shields.io/badge/license-Apache-yellow] [https://img.shields.io/badge/
+                        code%20style-black-000000.svg]
 ## Individual Fairness and inFairness Intuitively, an individually fair Machine
 Learning (ML) model treats similar inputs similarly. Formally, the leading
 notion of individual fairness is metric fairness [(Dwork et al., 2011)](https:/
 /dl.acm.org/doi/abs/10.1145/2090236.2090255); it requires: $$ d_y (h(x_1), h
 (x_2)) \leq L d_x(x_1, x_2) \quad \forall \quad x_1, x_2 \in X $$ Here, $h: X
 \rightarrow Y$ is a ML model, where $X$ and $Y$ are input and output spaces;
 $d_x$ and $d_y$ are metrics on the input and output spaces, and $L \geq 0$ is a
@@ -30,37 +31,36 @@
 as well. inFairness is a PyTorch package that supports auditing, training, and
 post-processing ML models for individual fairness. At its core, the library
 implements the key components of individual fairness pipeline: $d_x$ - distance
 in the input space, $d_y$ - distance in the output space, and the learning
 algorithms to optimize for the equation above. For an in-depth tutorial of
 Individual Fairness and the inFairness package, please watch this tutorial.
 Also, take a look at the [examples](./examples/) folder for illustrative use-
-cases. For more group fairness examples see [AIF360](https://
-aif360.mybluemix.net/).
+cases and try the [Fairness Playground demo](https://fairbert.vizhub.ai). For
+more group fairness examples see [AIF360](https://aif360.mybluemix.net/).
                              [Watch_the_tutorial]
 ## Installation inFairness can be installed using `pip`: ``` pip install
 inFairness ``` Alternatively, if you wish to install the latest development
 version, you can install directly by cloning this repository: ``` git clone  cd
 inFairness pip install -e . ``` ## Features inFairness currently supports: 1.
 Learning individually fair metrics : [[Docs]](https://ibm.github.io/inFairness/
 reference/distances.html) 2. Training of individually fair models : [[Docs]]
 (https://ibm.github.io/inFairness/reference/algorithms.html) 3. Auditing pre-
 trained ML models for individual fairness : [[Docs]](https://ibm.github.io/
 inFairness/reference/auditors.html) 4. Post-processing for Individual Fairness
-: [[Docs]](https://ibm.github.io/inFairness/reference/postprocessing.html) ###
-Coming soon We plan to extend the package by integrating the following
-features: 1. Individually fair ranking : [[Paper]](https://arxiv.org/abs/
-2103.11023) ## Contributing We welcome contributions from the community in any
-form - whether it is through the contribution of a new fair algorithm, fair
-metric, a new use-case, or simply reporting an issue or enhancement in the
-package. To contribute code to the package, please follow the following steps:
-1. Clone this git repository to your local system 2. Setup your system by
-installing dependencies as: `pip3 install -r requirements.txt` and `pip3
-install -r build_requirements.txt` 3. Add your code contribution to the
-package. Please refer to the [`inFairness`](./inFairness) folder for an
+: [[Docs]](https://ibm.github.io/inFairness/reference/postprocessing.html) 5.
+Individually fair ranking : [[Docs]](https://ibm.github.io/inFairness/
+reference/algorithms.html) ## Contributing We welcome contributions from the
+community in any form - whether it is through the contribution of a new fair
+algorithm, fair metric, a new use-case, or simply reporting an issue or
+enhancement in the package. To contribute code to the package, please follow
+the following steps: 1. Clone this git repository to your local system 2. Setup
+your system by installing dependencies as: `pip3 install -r requirements.txt`
+and `pip3 install -r build_requirements.txt` 3. Add your code contribution to
+the package. Please refer to the [`inFairness`](./inFairness) folder for an
 overview of the directory structure 4. Add appropriate unit tests in the
 [`tests`](./tests) folder 5. Once you are ready to commit code, check for the
 following: 1. Coding style compliance using: `flake8 inFairness/`. This command
 will list all stylistic violations found in the code. Please try to fix as much
 as you can 2. Ensure all the test cases pass using: `coverage run --source
 inFairness -m pytest tests/`. All unit tests need to pass to be able merge code
 in the package. 6. Finally, commit your code and raise a Pull Request. ##
```

### Comparing `inFairness-0.2.2/inFairness.egg-info/SOURCES.txt` & `inFairness-0.2.3/inFairness.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,36 +4,40 @@
 setup.py
 ./inFairness/__init__.py
 ./inFairness/auditor/__init__.py
 ./inFairness/auditor/auditor.py
 ./inFairness/auditor/datainterface.py
 ./inFairness/auditor/sensei_auditor.py
 ./inFairness/auditor/sensr_auditor.py
+./inFairness/auditor/senstir_auditor.py
 ./inFairness/distances/__init__.py
 ./inFairness/distances/distance.py
 ./inFairness/distances/euclidean_dists.py
 ./inFairness/distances/explore_distance.py
 ./inFairness/distances/logistic_sensitive_subspace.py
 ./inFairness/distances/mahalanobis_distance.py
 ./inFairness/distances/sensitive_subspace_dist.py
 ./inFairness/distances/wasserstein_distance.py
 ./inFairness/fairalgo/__init__.py
 ./inFairness/fairalgo/datainterfaces.py
 ./inFairness/fairalgo/sensei.py
 ./inFairness/fairalgo/sensr.py
+./inFairness/fairalgo/senstir.py
 ./inFairness/postprocessing/__init__.py
 ./inFairness/postprocessing/base_postprocessing.py
 ./inFairness/postprocessing/data_ds.py
 ./inFairness/postprocessing/datainterfaces.py
 ./inFairness/postprocessing/distance_ds.py
 ./inFairness/postprocessing/glif.py
 ./inFairness/utils/__init__.py
 ./inFairness/utils/datautils.py
 ./inFairness/utils/misc.py
+./inFairness/utils/ndcg.py
 ./inFairness/utils/params.py
+./inFairness/utils/plackett_luce.py
 ./inFairness/utils/postprocessing.py
 ./inFairness/utils/validationutils.py
 inFairness.egg-info/PKG-INFO
 inFairness.egg-info/SOURCES.txt
 inFairness.egg-info/dependency_links.txt
 inFairness.egg-info/requires.txt
 inFairness.egg-info/top_level.txt
```

### Comparing `inFairness-0.2.2/setup.py` & `inFairness-0.2.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,26 +7,25 @@
     name="inFairness",
     packages=[
         "inFairness",
         *["inFairness." + p for p in find_packages(where="./inFairness")],
     ],
     package_dir={"": ".",},
     install_requires=[
-        "functorch~=0.1.1",
         "numpy>=1.21.6",
         "pandas>=1.3.5",
         "POT>=0.8.0",
         "scikit-learn>=0.24.2",
         "scipy>=1.5.4",
-        "torch>=1.11.0",
+        "torch>=1.13.0"
     ],
     description="inFairness is a Python package to train and audit individually fair PyTorch models",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.2.2",
+    version="0.2.3",
     url="https://github.com/IBM/inFairness",
     author="IBM Research",
     author_email="mayank.agarwal@ibm.com, aldo.pareja@ibm.com, onkarbhardwaj@ibm.com, mikhail.yurochkin@ibm.com",
     keywords=[
         "individual fairness",
         "ai fairness",
         "trustworthy ai",
```


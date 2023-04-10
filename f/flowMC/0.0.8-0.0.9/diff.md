# Comparing `tmp/flowMC-0.0.8.tar.gz` & `tmp/flowMC-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowMC-0.0.8.tar", last modified: Tue Nov 15 14:16:12 2022, max compression
+gzip compressed data, was "flowMC-0.0.9.tar", last modified: Thu Nov 17 07:06:46 2022, max compression
```

## Comparing `flowMC-0.0.8.tar` & `flowMC-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-15 14:16:12.596961 flowMC-0.0.8/
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     1080 2022-11-02 23:17:49.000000 flowMC-0.0.8/LICENSE
--rw-rw-r--   0 kaze      (1001) kaze      (1001)      351 2022-11-15 14:16:12.596961 flowMC-0.0.8/PKG-INFO
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     2448 2022-11-10 08:16:30.000000 flowMC-0.0.8/README.md
--rw-rw-r--   0 kaze      (1001) kaze      (1001)       88 2022-11-02 23:17:49.000000 flowMC-0.0.8/pyproject.toml
--rw-rw-r--   0 kaze      (1001) kaze      (1001)      510 2022-11-15 14:16:12.596961 flowMC-0.0.8/setup.cfg
-drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-15 14:16:12.588961 flowMC-0.0.8/src/
-drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-15 14:16:12.592961 flowMC-0.0.8/src/flowMC/
--rw-rw-r--   0 kaze      (1001) kaze      (1001)        0 2022-11-02 23:17:49.000000 flowMC-0.0.8/src/flowMC/__init__.py
-drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-15 14:16:12.592961 flowMC-0.0.8/src/flowMC/nfmodel/
--rw-rw-r--   0 kaze      (1001) kaze      (1001)        0 2022-11-02 23:17:49.000000 flowMC-0.0.8/src/flowMC/nfmodel/__init__.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     5429 2022-11-15 08:25:19.000000 flowMC-0.0.8/src/flowMC/nfmodel/realNVP.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     5230 2022-11-02 23:17:49.000000 flowMC-0.0.8/src/flowMC/nfmodel/rqSpline.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     3009 2022-11-02 23:17:49.000000 flowMC-0.0.8/src/flowMC/nfmodel/utils.py
-drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-15 14:16:12.596961 flowMC-0.0.8/src/flowMC/sampler/
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     2695 2022-11-15 14:15:36.000000 flowMC-0.0.8/src/flowMC/sampler/Gaussian_random_walk.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     6256 2022-11-15 14:15:36.000000 flowMC-0.0.8/src/flowMC/sampler/HMC.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)      558 2022-11-15 14:15:36.000000 flowMC-0.0.8/src/flowMC/sampler/LocalSampler_Base.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     5302 2022-11-15 14:15:36.000000 flowMC-0.0.8/src/flowMC/sampler/MALA.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     8150 2022-11-02 23:17:49.000000 flowMC-0.0.8/src/flowMC/sampler/NF_proposal.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)    15627 2022-11-15 14:15:36.000000 flowMC-0.0.8/src/flowMC/sampler/Sampler.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)        0 2022-11-02 23:17:49.000000 flowMC-0.0.8/src/flowMC/sampler/__init__.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     5996 2022-11-02 23:17:49.000000 flowMC-0.0.8/src/flowMC/sampler/mMALA.py
-drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-15 14:16:12.596961 flowMC-0.0.8/src/flowMC/utils/
--rw-rw-r--   0 kaze      (1001) kaze      (1001)      988 2022-11-02 23:17:49.000000 flowMC-0.0.8/src/flowMC/utils/PRNG_keys.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     3910 2022-11-02 23:17:49.000000 flowMC-0.0.8/src/flowMC/utils/PythonFunctionWrap.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)        0 2022-11-02 23:17:49.000000 flowMC-0.0.8/src/flowMC/utils/__init__.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     2700 2022-11-02 23:17:49.000000 flowMC-0.0.8/src/flowMC/utils/progressBar.py
-drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-15 14:16:12.592961 flowMC-0.0.8/src/flowMC.egg-info/
--rw-rw-r--   0 kaze      (1001) kaze      (1001)      351 2022-11-15 14:16:12.000000 flowMC-0.0.8/src/flowMC.egg-info/PKG-INFO
--rw-rw-r--   0 kaze      (1001) kaze      (1001)      851 2022-11-15 14:16:12.000000 flowMC-0.0.8/src/flowMC.egg-info/SOURCES.txt
--rw-rw-r--   0 kaze      (1001) kaze      (1001)        1 2022-11-15 14:16:12.000000 flowMC-0.0.8/src/flowMC.egg-info/dependency_links.txt
--rw-rw-r--   0 kaze      (1001) kaze      (1001)       29 2022-11-15 14:16:12.000000 flowMC-0.0.8/src/flowMC.egg-info/requires.txt
--rw-rw-r--   0 kaze      (1001) kaze      (1001)        7 2022-11-15 14:16:12.000000 flowMC-0.0.8/src/flowMC.egg-info/top_level.txt
-drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-15 14:16:12.596961 flowMC-0.0.8/test/
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     2367 2022-11-15 14:15:36.000000 flowMC-0.0.8/test/test_HMC.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     2433 2022-11-15 14:15:36.000000 flowMC-0.0.8/test/test_MALA.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     2244 2022-11-15 14:15:36.000000 flowMC-0.0.8/test/test_RWMCMC.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     2626 2022-11-02 23:17:49.000000 flowMC-0.0.8/test/test_normalizingFlow.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)      804 2022-11-02 23:17:49.000000 flowMC-0.0.8/test/test_quickstart.py
+drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-17 07:06:46.882324 flowMC-0.0.9/
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)     1080 2022-11-02 23:17:49.000000 flowMC-0.0.9/LICENSE
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)      351 2022-11-17 07:06:46.882324 flowMC-0.0.9/PKG-INFO
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)     2448 2022-11-10 08:16:30.000000 flowMC-0.0.9/README.md
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)       88 2022-11-02 23:17:49.000000 flowMC-0.0.9/pyproject.toml
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)      510 2022-11-17 07:06:46.882324 flowMC-0.0.9/setup.cfg
+drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-17 07:06:46.874323 flowMC-0.0.9/src/
+drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-17 07:06:46.878323 flowMC-0.0.9/src/flowMC/
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)        0 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/__init__.py
+drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-17 07:06:46.882324 flowMC-0.0.9/src/flowMC/nfmodel/
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)        0 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/nfmodel/__init__.py
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)     5429 2022-11-15 08:25:19.000000 flowMC-0.0.9/src/flowMC/nfmodel/realNVP.py
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)     5230 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/nfmodel/rqSpline.py
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)     3009 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/nfmodel/utils.py
+drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-17 07:06:46.882324 flowMC-0.0.9/src/flowMC/sampler/
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)     2695 2022-11-15 14:15:36.000000 flowMC-0.0.9/src/flowMC/sampler/Gaussian_random_walk.py
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)     6256 2022-11-15 14:15:36.000000 flowMC-0.0.9/src/flowMC/sampler/HMC.py
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)      558 2022-11-15 14:15:36.000000 flowMC-0.0.9/src/flowMC/sampler/LocalSampler_Base.py
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)     5302 2022-11-15 14:15:36.000000 flowMC-0.0.9/src/flowMC/sampler/MALA.py
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)     8150 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/sampler/NF_proposal.py
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)    15627 2022-11-15 14:15:36.000000 flowMC-0.0.9/src/flowMC/sampler/Sampler.py
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)        0 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/sampler/__init__.py
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)     5996 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/sampler/mMALA.py
+drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-17 07:06:46.882324 flowMC-0.0.9/src/flowMC/utils/
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)      988 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/utils/PRNG_keys.py
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)     3910 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/utils/PythonFunctionWrap.py
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)        0 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/utils/__init__.py
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)     2700 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/utils/progressBar.py
+drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-17 07:06:46.878323 flowMC-0.0.9/src/flowMC.egg-info/
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)      351 2022-11-17 07:06:46.000000 flowMC-0.0.9/src/flowMC.egg-info/PKG-INFO
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)      851 2022-11-17 07:06:46.000000 flowMC-0.0.9/src/flowMC.egg-info/SOURCES.txt
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)        1 2022-11-17 07:06:46.000000 flowMC-0.0.9/src/flowMC.egg-info/dependency_links.txt
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)       29 2022-11-17 07:06:46.000000 flowMC-0.0.9/src/flowMC.egg-info/requires.txt
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)        7 2022-11-17 07:06:46.000000 flowMC-0.0.9/src/flowMC.egg-info/top_level.txt
+drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-17 07:06:46.882324 flowMC-0.0.9/test/
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)     2367 2022-11-15 14:15:36.000000 flowMC-0.0.9/test/test_HMC.py
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)     2433 2022-11-15 14:15:36.000000 flowMC-0.0.9/test/test_MALA.py
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)     2244 2022-11-15 14:15:36.000000 flowMC-0.0.9/test/test_RWMCMC.py
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)     2626 2022-11-02 23:17:49.000000 flowMC-0.0.9/test/test_normalizingFlow.py
+-rw-rw-r--   0 kaze      (1001) kaze      (1001)      804 2022-11-02 23:17:49.000000 flowMC-0.0.9/test/test_quickstart.py
```

### Comparing `flowMC-0.0.8/LICENSE` & `flowMC-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/README.md` & `flowMC-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/src/flowMC/nfmodel/realNVP.py` & `flowMC-0.0.9/src/flowMC/nfmodel/realNVP.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/src/flowMC/nfmodel/rqSpline.py` & `flowMC-0.0.9/src/flowMC/nfmodel/rqSpline.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/src/flowMC/nfmodel/utils.py` & `flowMC-0.0.9/src/flowMC/nfmodel/utils.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/src/flowMC/sampler/Gaussian_random_walk.py` & `flowMC-0.0.9/src/flowMC/sampler/Gaussian_random_walk.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/src/flowMC/sampler/HMC.py` & `flowMC-0.0.9/src/flowMC/sampler/HMC.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/src/flowMC/sampler/LocalSampler_Base.py` & `flowMC-0.0.9/src/flowMC/sampler/LocalSampler_Base.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/src/flowMC/sampler/MALA.py` & `flowMC-0.0.9/src/flowMC/sampler/MALA.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/src/flowMC/sampler/NF_proposal.py` & `flowMC-0.0.9/src/flowMC/sampler/NF_proposal.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/src/flowMC/sampler/Sampler.py` & `flowMC-0.0.9/src/flowMC/sampler/Sampler.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/src/flowMC/sampler/mMALA.py` & `flowMC-0.0.9/src/flowMC/sampler/mMALA.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/src/flowMC/utils/PRNG_keys.py` & `flowMC-0.0.9/src/flowMC/utils/PRNG_keys.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/src/flowMC/utils/PythonFunctionWrap.py` & `flowMC-0.0.9/src/flowMC/utils/PythonFunctionWrap.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/src/flowMC/utils/progressBar.py` & `flowMC-0.0.9/src/flowMC/utils/progressBar.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/src/flowMC.egg-info/SOURCES.txt` & `flowMC-0.0.9/src/flowMC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/test/test_HMC.py` & `flowMC-0.0.9/test/test_HMC.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/test/test_MALA.py` & `flowMC-0.0.9/test/test_MALA.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/test/test_RWMCMC.py` & `flowMC-0.0.9/test/test_RWMCMC.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/test/test_normalizingFlow.py` & `flowMC-0.0.9/test/test_normalizingFlow.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.8/test/test_quickstart.py` & `flowMC-0.0.9/test/test_quickstart.py`

 * *Files identical despite different names*


# Comparing `tmp/jimGW-0.0.4.4.tar.gz` & `tmp/jimGW-0.0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jimGW-0.0.4.4.tar", last modified: Mon Apr 10 20:24:10 2023, max compression
+gzip compressed data, was "jimGW-0.0.4.5.tar", last modified: Mon Apr 10 20:29:20 2023, max compression
```

## Comparing `jimGW-0.0.4.4.tar` & `jimGW-0.0.4.5.tar`

### file list

```diff
@@ -1,19 +1,31 @@
-drwxrwxr-x   0 wwong     (1568) wwong     (1568)        0 2023-04-10 20:24:10.597065 jimGW-0.0.4.4/
--rw-rw-r--   0 wwong     (1568) wwong     (1568)     1066 2023-03-30 17:56:57.000000 jimGW-0.0.4.4/LICENSE
--rw-rw-r--   0 wwong     (1568) wwong     (1568)      342 2023-04-10 20:24:10.598128 jimGW-0.0.4.4/PKG-INFO
--rw-rw-r--   0 wwong     (1568) wwong     (1568)     2180 2023-03-30 18:12:50.000000 jimGW-0.0.4.4/README.md
--rw-rw-r--   0 wwong     (1568) wwong     (1568)       88 2023-03-30 17:56:57.000000 jimGW-0.0.4.4/pyproject.toml
--rw-rw-r--   0 wwong     (1568) wwong     (1568)      539 2023-04-10 20:24:10.602540 jimGW-0.0.4.4/setup.cfg
-drwxrwxr-x   0 wwong     (1568) wwong     (1568)        0 2023-04-10 20:24:10.524463 jimGW-0.0.4.4/src/
-drwxrwxr-x   0 wwong     (1568) wwong     (1568)        0 2023-04-10 20:24:10.567312 jimGW-0.0.4.4/src/jimGW.egg-info/
--rw-rw-r--   0 wwong     (1568) wwong     (1568)      342 2023-04-10 20:24:10.000000 jimGW-0.0.4.4/src/jimGW.egg-info/PKG-INFO
--rw-rw-r--   0 wwong     (1568) wwong     (1568)      334 2023-04-10 20:24:10.000000 jimGW-0.0.4.4/src/jimGW.egg-info/SOURCES.txt
--rw-rw-r--   0 wwong     (1568) wwong     (1568)        1 2023-04-10 20:24:10.000000 jimGW-0.0.4.4/src/jimGW.egg-info/dependency_links.txt
--rw-rw-r--   0 wwong     (1568) wwong     (1568)       65 2023-04-10 20:24:10.000000 jimGW-0.0.4.4/src/jimGW.egg-info/requires.txt
--rw-rw-r--   0 wwong     (1568) wwong     (1568)        1 2023-04-10 20:24:10.000000 jimGW-0.0.4.4/src/jimGW.egg-info/top_level.txt
-drwxrwxr-x   0 wwong     (1568) wwong     (1568)        0 2023-04-10 20:24:10.592321 jimGW-0.0.4.4/test/
--rw-rw-r--   0 wwong     (1568) wwong     (1568)      794 2023-03-30 17:56:58.000000 jimGW-0.0.4.4/test/test_IMRPhenomC.py
--rw-rw-r--   0 wwong     (1568) wwong     (1568)     1739 2023-03-30 17:56:58.000000 jimGW-0.0.4.4/test/test_TaylorF2.py
--rw-rw-r--   0 wwong     (1568) wwong     (1568)      879 2023-03-30 17:56:58.000000 jimGW-0.0.4.4/test/test_interferometer.py
--rw-rw-r--   0 wwong     (1568) wwong     (1568)     4243 2023-03-30 17:56:58.000000 jimGW-0.0.4.4/test/test_likelihood.py
--rw-rw-r--   0 wwong     (1568) wwong     (1568)    10696 2023-03-30 17:56:58.000000 jimGW-0.0.4.4/test/test_likelihood_bilby.py
+drwxrwxr-x   0 wwong     (1568) wwong     (1568)        0 2023-04-10 20:29:20.315119 jimGW-0.0.4.5/
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)     1066 2023-03-30 17:56:57.000000 jimGW-0.0.4.5/LICENSE
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)      342 2023-04-10 20:29:20.316237 jimGW-0.0.4.5/PKG-INFO
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)     2180 2023-03-30 18:12:50.000000 jimGW-0.0.4.5/README.md
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)       88 2023-03-30 17:56:57.000000 jimGW-0.0.4.5/pyproject.toml
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)      539 2023-04-10 20:29:20.320726 jimGW-0.0.4.5/setup.cfg
+drwxrwxr-x   0 wwong     (1568) wwong     (1568)        0 2023-04-10 20:29:20.152189 jimGW-0.0.4.5/src/
+drwxrwxr-x   0 wwong     (1568) wwong     (1568)        0 2023-04-10 20:29:20.198779 jimGW-0.0.4.5/src/jimGW.egg-info/
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)      342 2023-04-10 20:29:20.000000 jimGW-0.0.4.5/src/jimGW.egg-info/PKG-INFO
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)      635 2023-04-10 20:29:20.000000 jimGW-0.0.4.5/src/jimGW.egg-info/SOURCES.txt
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)        1 2023-04-10 20:29:20.000000 jimGW-0.0.4.5/src/jimGW.egg-info/dependency_links.txt
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)       65 2023-04-10 20:29:20.000000 jimGW-0.0.4.5/src/jimGW.egg-info/requires.txt
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)        6 2023-04-10 20:29:20.000000 jimGW-0.0.4.5/src/jimGW.egg-info/top_level.txt
+drwxrwxr-x   0 wwong     (1568) wwong     (1568)        0 2023-04-10 20:29:20.203585 jimGW-0.0.4.5/src/jimgw/
+drwxrwxr-x   0 wwong     (1568) wwong     (1568)        0 2023-04-10 20:29:20.283643 jimGW-0.0.4.5/src/jimgw/PE/
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)        1 2023-04-10 20:28:20.000000 jimGW-0.0.4.5/src/jimgw/PE/__init__.py
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)      318 2023-03-30 18:12:50.000000 jimGW-0.0.4.5/src/jimgw/PE/constants.py
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)     2655 2023-03-30 18:12:50.000000 jimGW-0.0.4.5/src/jimgw/PE/detector_preset.py
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)     6385 2023-03-30 18:12:50.000000 jimGW-0.0.4.5/src/jimgw/PE/detector_projection.py
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)     1866 2023-03-30 18:12:50.000000 jimGW-0.0.4.5/src/jimgw/PE/generate_noise.py
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)     5556 2023-03-30 18:12:50.000000 jimGW-0.0.4.5/src/jimgw/PE/heterodyneLikelihood.py
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)      504 2023-03-30 18:12:50.000000 jimGW-0.0.4.5/src/jimgw/PE/single_event_likelihood.py
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)     1537 2023-03-30 18:12:50.000000 jimGW-0.0.4.5/src/jimgw/PE/time_and_date.py
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)     1098 2023-03-30 18:12:50.000000 jimGW-0.0.4.5/src/jimgw/PE/utils.py
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)        1 2023-04-10 20:28:27.000000 jimGW-0.0.4.5/src/jimgw/__init__.py
+drwxrwxr-x   0 wwong     (1568) wwong     (1568)        0 2023-04-10 20:29:20.310143 jimGW-0.0.4.5/test/
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)      794 2023-03-30 17:56:58.000000 jimGW-0.0.4.5/test/test_IMRPhenomC.py
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)     1739 2023-03-30 17:56:58.000000 jimGW-0.0.4.5/test/test_TaylorF2.py
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)      879 2023-03-30 17:56:58.000000 jimGW-0.0.4.5/test/test_interferometer.py
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)     4243 2023-03-30 17:56:58.000000 jimGW-0.0.4.5/test/test_likelihood.py
+-rw-rw-r--   0 wwong     (1568) wwong     (1568)    10696 2023-03-30 17:56:58.000000 jimGW-0.0.4.5/test/test_likelihood_bilby.py
```

### Comparing `jimGW-0.0.4.4/LICENSE` & `jimGW-0.0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jimGW-0.0.4.4/README.md` & `jimGW-0.0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `jimGW-0.0.4.4/setup.cfg` & `jimGW-0.0.4.5/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jimGW
-version = 0.0.4.4
+version = 0.0.4.5
 author = Kaze Wong
 author_email = kazewong.physics@gmail.com
 url = https://github.com/kazewong/jim
 description = Gravitatioanl wave data analysis tool in Jax
 keywords = sampling, inference, machine learning, normalizing, autodiff, jax
 license = MIT
```

### Comparing `jimGW-0.0.4.4/test/test_IMRPhenomC.py` & `jimGW-0.0.4.5/test/test_IMRPhenomC.py`

 * *Files identical despite different names*

### Comparing `jimGW-0.0.4.4/test/test_TaylorF2.py` & `jimGW-0.0.4.5/test/test_TaylorF2.py`

 * *Files identical despite different names*

### Comparing `jimGW-0.0.4.4/test/test_interferometer.py` & `jimGW-0.0.4.5/test/test_interferometer.py`

 * *Files identical despite different names*

### Comparing `jimGW-0.0.4.4/test/test_likelihood.py` & `jimGW-0.0.4.5/test/test_likelihood.py`

 * *Files identical despite different names*

### Comparing `jimGW-0.0.4.4/test/test_likelihood_bilby.py` & `jimGW-0.0.4.5/test/test_likelihood_bilby.py`

 * *Files identical despite different names*


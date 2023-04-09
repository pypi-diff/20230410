# Comparing `tmp/deepdog-0.6.5.tar.gz` & `tmp/deepdog-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdog-0.6.5.tar", max compression
+gzip compressed data, was "deepdog-0.6.6.tar", max compression
```

## Comparing `deepdog-0.6.5.tar` & `deepdog-0.6.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      501 2023-04-09 22:42:35.584677 deepdog-0.6.5/deepdog/__init__.py
--rw-r--r--   0        0        0     8197 2023-04-09 22:42:35.584677 deepdog-0.6.5/deepdog/bayes_run.py
--rw-r--r--   0        0        0    11705 2023-04-09 22:42:35.584677 deepdog-0.6.5/deepdog/bayes_run_simulpairs.py
--rw-r--r--   0        0        0       73 2023-04-09 22:42:35.584677 deepdog-0.6.5/deepdog/meta.py
--rw-r--r--   0        0        0     6655 2023-04-09 22:42:35.584677 deepdog-0.6.5/deepdog/real_spectrum_run.py
--rw-r--r--   0        0        0     6681 2023-04-09 22:42:35.584677 deepdog-0.6.5/deepdog/temp_aware_real_spectrum_run.py
--rw-r--r--   0        0        0      895 2023-04-09 22:42:35.588678 deepdog-0.6.5/pyproject.toml
--rw-r--r--   0        0        0      630 2023-04-09 22:43:50.177066 deepdog-0.6.5/setup.py
--rw-r--r--   0        0        0      408 2023-04-09 22:43:50.177417 deepdog-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0      501 2023-04-09 23:13:34.475057 deepdog-0.6.6/deepdog/__init__.py
+-rw-r--r--   0        0        0     8197 2023-04-09 23:13:34.475057 deepdog-0.6.6/deepdog/bayes_run.py
+-rw-r--r--   0        0        0    11705 2023-04-09 23:13:34.475057 deepdog-0.6.6/deepdog/bayes_run_simulpairs.py
+-rw-r--r--   0        0        0       73 2023-04-09 23:13:34.475057 deepdog-0.6.6/deepdog/meta.py
+-rw-r--r--   0        0        0     6655 2023-04-09 23:13:34.475057 deepdog-0.6.6/deepdog/real_spectrum_run.py
+-rw-r--r--   0        0        0     6576 2023-04-09 23:13:34.475057 deepdog-0.6.6/deepdog/temp_aware_real_spectrum_run.py
+-rw-r--r--   0        0        0      895 2023-04-09 23:13:34.479057 deepdog-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0      630 2023-04-09 23:15:03.630427 deepdog-0.6.6/setup.py
+-rw-r--r--   0        0        0      408 2023-04-09 23:15:03.630786 deepdog-0.6.6/PKG-INFO
```

### Comparing `deepdog-0.6.5/deepdog/bayes_run.py` & `deepdog-0.6.6/deepdog/bayes_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.6.5/deepdog/bayes_run_simulpairs.py` & `deepdog-0.6.6/deepdog/bayes_run_simulpairs.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.6.5/deepdog/real_spectrum_run.py` & `deepdog-0.6.6/deepdog/real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.6.5/deepdog/temp_aware_real_spectrum_run.py` & `deepdog-0.6.6/deepdog/temp_aware_real_spectrum_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,14 @@
 		monte_carlo_count, None, rng_to_use=rng
 	)
 
 	current_sample = sample_dipoles
 	for temp in dot_inputs_dict.keys():
 		dot_inputs = dot_inputs_dict[temp]
 		lows, highs = low_high_dict[temp]
-		_logger.info(f"current sample length: {len(current_sample)}")
-		_logger.info(f"workng on temp {temp}")
 		for di, low, high in zip(dot_inputs, lows, highs):
 
 			if len(current_sample) < 1:
 				break
 			vals = pdme.util.fast_v_calc.fast_vs_for_asymmetric_dipoleses(
 				numpy.array([di]), current_sample, temp
 			)
```

### Comparing `deepdog-0.6.5/pyproject.toml` & `deepdog-0.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepdog"
-version = "0.6.5"
+version = "0.6.6"
 description = ""
 authors = ["Deepak Mallubhotla <dmallubhotla+github@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.10"
 pdme = "^0.8.6"
 numpy = "1.22.3"
```

### Comparing `deepdog-0.6.5/setup.py` & `deepdog-0.6.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy==1.22.3', 'pdme>=0.8.6,<0.9.0', 'scipy==1.10']
 
 setup_kwargs = {
     'name': 'deepdog',
-    'version': '0.6.5',
+    'version': '0.6.6',
     'description': '',
     'long_description': None,
     'author': 'Deepak Mallubhotla',
     'author_email': 'dmallubhotla+github@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```


# Comparing `tmp/deepdog-0.6.4.tar.gz` & `tmp/deepdog-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdog-0.6.4.tar", max compression
+gzip compressed data, was "deepdog-0.6.5.tar", max compression
```

## Comparing `deepdog-0.6.4.tar` & `deepdog-0.6.5.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      398 2022-08-13 20:52:26.304298 deepdog-0.6.4/deepdog/__init__.py
--rw-r--r--   0        0        0     8197 2022-08-13 20:52:26.304298 deepdog-0.6.4/deepdog/bayes_run.py
--rw-r--r--   0        0        0    11705 2022-08-13 20:52:26.304298 deepdog-0.6.4/deepdog/bayes_run_simulpairs.py
--rw-r--r--   0        0        0       73 2022-08-13 20:52:26.304298 deepdog-0.6.4/deepdog/meta.py
--rw-r--r--   0        0        0     6655 2022-08-13 20:52:26.304298 deepdog-0.6.4/deepdog/real_spectrum_run.py
--rw-r--r--   0        0        0      896 2022-08-13 20:52:26.304298 deepdog-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      631 2022-08-13 20:54:17.076424 deepdog-0.6.4/setup.py
--rw-r--r--   0        0        0      409 2022-08-13 20:54:17.076827 deepdog-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0      501 2023-04-09 22:42:35.584677 deepdog-0.6.5/deepdog/__init__.py
+-rw-r--r--   0        0        0     8197 2023-04-09 22:42:35.584677 deepdog-0.6.5/deepdog/bayes_run.py
+-rw-r--r--   0        0        0    11705 2023-04-09 22:42:35.584677 deepdog-0.6.5/deepdog/bayes_run_simulpairs.py
+-rw-r--r--   0        0        0       73 2023-04-09 22:42:35.584677 deepdog-0.6.5/deepdog/meta.py
+-rw-r--r--   0        0        0     6655 2023-04-09 22:42:35.584677 deepdog-0.6.5/deepdog/real_spectrum_run.py
+-rw-r--r--   0        0        0     6681 2023-04-09 22:42:35.584677 deepdog-0.6.5/deepdog/temp_aware_real_spectrum_run.py
+-rw-r--r--   0        0        0      895 2023-04-09 22:42:35.588678 deepdog-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      630 2023-04-09 22:43:50.177066 deepdog-0.6.5/setup.py
+-rw-r--r--   0        0        0      408 2023-04-09 22:43:50.177417 deepdog-0.6.5/PKG-INFO
```

### Comparing `deepdog-0.6.4/deepdog/bayes_run.py` & `deepdog-0.6.5/deepdog/bayes_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.6.4/deepdog/bayes_run_simulpairs.py` & `deepdog-0.6.5/deepdog/bayes_run_simulpairs.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.6.4/deepdog/real_spectrum_run.py` & `deepdog-0.6.5/deepdog/real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.6.4/pyproject.toml` & `deepdog-0.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "deepdog"
-version = "0.6.4"
+version = "0.6.5"
 description = ""
 authors = ["Deepak Mallubhotla <dmallubhotla+github@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.10"
 pdme = "^0.8.6"
 numpy = "1.22.3"
-scipy = "1.8.0"
+scipy = "1.10"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6"
 flake8 = "^4.0.1"
 pytest-cov = "^3.0.0"
 mypy = "^0.971"
 python-semantic-release = "^7.24.0"
```

### Comparing `deepdog-0.6.4/setup.py` & `deepdog-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['deepdog']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy==1.22.3', 'pdme>=0.8.6,<0.9.0', 'scipy==1.8.0']
+['numpy==1.22.3', 'pdme>=0.8.6,<0.9.0', 'scipy==1.10']
 
 setup_kwargs = {
     'name': 'deepdog',
-    'version': '0.6.4',
+    'version': '0.6.5',
     'description': '',
     'long_description': None,
     'author': 'Deepak Mallubhotla',
     'author_email': 'dmallubhotla+github@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```


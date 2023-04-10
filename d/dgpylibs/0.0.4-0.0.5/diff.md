# Comparing `tmp/dgpylibs-0.0.4.tar.gz` & `tmp/dgpylibs-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgpylibs-0.0.4.tar", max compression
+gzip compressed data, was "dgpylibs-0.0.5.tar", max compression
```

## Comparing `dgpylibs-0.0.4.tar` & `dgpylibs-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     5409 2022-09-30 17:11:16.160479 dgpylibs-0.0.4/dgpylibs/__init__.py
--rw-r--r--   0        0        0      656 2022-09-29 01:53:26.534391 dgpylibs-0.0.4/dgpylibs/__main__.py
--rw-r--r--   0        0        0      214 2022-09-29 01:53:26.534527 dgpylibs-0.0.4/dgpylibs/_meta.py
--rw-r--r--   0        0        0       49 2022-09-29 01:11:55.780099 dgpylibs-0.0.4/dgpylibs/dev/__init__.py
--rw-r--r--   0        0        0        0 2022-09-29 01:11:55.780099 dgpylibs-0.0.4/dgpylibs/py.typed
--rw-r--r--   0        0        0     1757 2022-09-30 17:11:16.160479 dgpylibs-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 dgpylibs-0.0.4/setup.py
--rw-r--r--   0        0        0     1275 1970-01-01 00:00:00.000000 dgpylibs-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     8525 2023-03-24 22:14:11.921866 dgpylibs-0.0.5/dgpylibs/__init__.py
+-rw-r--r--   0        0        0      580 2023-03-24 22:14:11.922878 dgpylibs-0.0.5/dgpylibs/__main__.py
+-rw-r--r--   0        0        0      214 2023-04-10 21:38:22.349978 dgpylibs-0.0.5/dgpylibs/_meta.py
+-rw-r--r--   0        0        0       49 2022-09-29 01:11:55.780099 dgpylibs-0.0.5/dgpylibs/dev/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-29 01:11:55.780099 dgpylibs-0.0.5/dgpylibs/py.typed
+-rw-r--r--   0        0        0     1797 2023-04-10 21:38:09.592968 dgpylibs-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      858 1970-01-01 00:00:00.000000 dgpylibs-0.0.5/setup.py
+-rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 dgpylibs-0.0.5/PKG-INFO
```

### Comparing `dgpylibs-0.0.4/pyproject.toml` & `dgpylibs-0.0.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,38 @@
 [tool.poetry]
 name = "dgpylibs"
-version = "0.0.4"
+version = "0.0.5"
 description = "Dynamic Graphics Python libraries"
 authors = ["jessekrubin <jesse@dgi.com>"]
 license = "MIT"
 repository = "https://github.com/dynamic-graphics-inc/dgpy-libs"
 homepage = "https://github.com/dynamic-graphics-inc/dgpy-libs"
-packages = [
-  { include = "dgpylibs", from = "." },
-]
+packages = [{ include = "dgpylibs", from = "." }]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
+  "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Typing :: Typed",
 ]
-keywords = [
-  "dgpy",
-  "dgi",
-  "typed",
-  "python3",
-]
+keywords = ["dgpy", "dgi", "typed", "python3"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 aiopen = "*"
 asyncify = "*"
 fmts = "*"
 funkify = "*"
-h5 = "*"
+h5 = ">=0.8.8"
 jsonbourne = "*"
-lager = "*"
+lager = ">=0.17.0"
 listless = "*"
 requires = "*"
 shellfish = "*"
 xtyping = "*"
 
 [tool.poetry.dev-dependencies]
 xdoctest = ">=0.15.10"
@@ -52,7 +45,10 @@
 # /\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/
 # =============================================================================
 #  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\
 # /  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \
 # =============================================================================
 # \/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\
 # =============================================================================
+
+[tool.ruff]
+extend = "../../pyproject.toml"
```

### Comparing `dgpylibs-0.0.4/setup.py` & `dgpylibs-0.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,34 +11,34 @@
 {'': ['*']}
 
 install_requires = \
 ['aiopen',
  'asyncify',
  'fmts',
  'funkify',
- 'h5',
+ 'h5>=0.8.8',
  'jsonbourne',
- 'lager',
+ 'lager>=0.17.0',
  'listless',
  'requires',
  'shellfish',
  'xtyping']
 
 setup_kwargs = {
     'name': 'dgpylibs',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Dynamic Graphics Python libraries',
     'long_description': 'None',
     'author': 'jessekrubin',
     'author_email': 'jesse@dgi.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/dynamic-graphics-inc/dgpy-libs',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `dgpylibs-0.0.4/PKG-INFO` & `dgpylibs-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: dgpylibs
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dynamic Graphics Python libraries
 Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs
 License: MIT
 Keywords: dgpy,dgi,typed,python3
 Author: jessekrubin
 Author-email: jesse@dgi.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Requires-Dist: aiopen
 Requires-Dist: asyncify
 Requires-Dist: fmts
 Requires-Dist: funkify
-Requires-Dist: h5
+Requires-Dist: h5 (>=0.8.8)
 Requires-Dist: jsonbourne
-Requires-Dist: lager
+Requires-Dist: lager (>=0.17.0)
 Requires-Dist: listless
 Requires-Dist: requires
 Requires-Dist: shellfish
 Requires-Dist: xtyping
 Project-URL: Repository, https://github.com/dynamic-graphics-inc/dgpy-libs
```


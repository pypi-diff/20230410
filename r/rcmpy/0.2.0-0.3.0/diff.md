# Comparing `tmp/rcmpy-0.2.0.tar.gz` & `tmp/rcmpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcmpy-0.2.0.tar", last modified: Tue Apr  4 05:54:57 2023, max compression
+gzip compressed data, was "rcmpy-0.3.0.tar", last modified: Mon Apr 10 05:45:40 2023, max compression
```

## Comparing `rcmpy-0.2.0.tar` & `rcmpy-0.3.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:54:57.939086 rcmpy-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-04 05:53:53.000000 rcmpy-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-04 05:54:57.939086 rcmpy-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-04 05:53:53.000000 rcmpy-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-04 05:53:53.000000 rcmpy-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:54:57.935086 rcmpy-0.2.0/rcmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:54:57.935086 rcmpy-0.2.0/rcmpy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/commands/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/commands/use.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/commands/variant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/commands/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:54:57.935086 rcmpy-0.2.0/rcmpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:54:57.931086 rcmpy-0.2.0/rcmpy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:54:57.935086 rcmpy-0.2.0/rcmpy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/data/schemas/ManagedFile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/data/schemas/State.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:54:57.935086 rcmpy-0.2.0/rcmpy/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/environment/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:54:57.935086 rcmpy-0.2.0/rcmpy/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:54:57.935086 rcmpy-0.2.0/rcmpy/state/
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:54:57.935086 rcmpy-0.2.0/rcmpy/xdg/
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-04 05:53:53.000000 rcmpy-0.2.0/rcmpy/xdg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:54:57.935086 rcmpy-0.2.0/rcmpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-04 05:54:57.000000 rcmpy-0.2.0/rcmpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-04 05:54:57.000000 rcmpy-0.2.0/rcmpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 05:54:57.000000 rcmpy-0.2.0/rcmpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-04 05:54:57.000000 rcmpy-0.2.0/rcmpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-04 05:54:57.000000 rcmpy-0.2.0/rcmpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-04 05:54:57.000000 rcmpy-0.2.0/rcmpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 05:54:57.939086 rcmpy-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-04 05:53:53.000000 rcmpy-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 05:54:57.939086 rcmpy-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-04 05:53:53.000000 rcmpy-0.2.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-04 05:53:53.000000 rcmpy-0.2.0/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-04 05:53:53.000000 rcmpy-0.2.0/tests/test_xdg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.713079 rcmpy-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-10 05:44:36.000000 rcmpy-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-10 05:45:40.713079 rcmpy-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-10 05:44:36.000000 rcmpy-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-10 05:44:36.000000 rcmpy-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.709079 rcmpy-0.3.0/rcmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.713079 rcmpy-0.3.0/rcmpy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/commands/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/commands/use.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/commands/variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/commands/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.713079 rcmpy-0.3.0/rcmpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.709079 rcmpy-0.3.0/rcmpy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.713079 rcmpy-0.3.0/rcmpy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/data/schemas/ManagedFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/data/schemas/State.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.713079 rcmpy-0.3.0/rcmpy/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/environment/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.713079 rcmpy-0.3.0/rcmpy/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.713079 rcmpy-0.3.0/rcmpy/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.713079 rcmpy-0.3.0/rcmpy/xdg/
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/xdg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.709079 rcmpy-0.3.0/rcmpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-10 05:45:40.000000 rcmpy-0.3.0/rcmpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-10 05:45:40.000000 rcmpy-0.3.0/rcmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 05:45:40.000000 rcmpy-0.3.0/rcmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 05:45:40.000000 rcmpy-0.3.0/rcmpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-10 05:45:40.000000 rcmpy-0.3.0/rcmpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 05:45:40.000000 rcmpy-0.3.0/rcmpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 05:45:40.713079 rcmpy-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-10 05:44:36.000000 rcmpy-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.713079 rcmpy-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-10 05:44:36.000000 rcmpy-0.3.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-10 05:44:36.000000 rcmpy-0.3.0/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-10 05:44:36.000000 rcmpy-0.3.0/tests/test_xdg.py
```

### Comparing `rcmpy-0.2.0/LICENSE` & `rcmpy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rcmpy-0.2.0/PKG-INFO` & `rcmpy-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 0.2.0
+Version: 0.3.0
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=e6c457784db73e957b3b0da662d10294
+    hash=96aa8923f1d36b7eddcfda3f7e4d8171
     =====================================
 -->
 
-# rcmpy ([0.2.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([0.3.0](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
```

### Comparing `rcmpy-0.2.0/README.md` & `rcmpy-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=e6c457784db73e957b3b0da662d10294
+    hash=96aa8923f1d36b7eddcfda3f7e4d8171
     =====================================
 -->
 
-# rcmpy ([0.2.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([0.3.0](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
```

### Comparing `rcmpy-0.2.0/pyproject.toml` & `rcmpy-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "rcmpy"
-version = "0.2.0"
+version = "0.3.0"
 description = "A configuration-file management system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
@@ -29,18 +29,18 @@
 ]
 dynamic = ["dependencies"]
 
 [project.optional-dependencies]
 test = [
   "pylint",
   "flake8",
-  "pytest",
-  "pytest-cov",
-  "mypy",
   "black",
+  "ruff",
+  "mypy",
   "isort",
+  "yamllint",
   "setuptools-wrapper",
   "types-setuptools"
 ]
 
 [project.scripts]
 rcmpy = "rcmpy.entry:main"
```

### Comparing `rcmpy-0.2.0/rcmpy/app.py` & `rcmpy-0.3.0/rcmpy/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # =====================================
 # generator=datazen
 # version=3.1.2
-# hash=20b145df60dffa371c92ff46f777d771
+# hash=0cb0fd902b7216726825ed86f95176e5
 # =====================================
 
 """
 This package's command-line entry-point application.
 """
 
 # built-in
 from argparse import ArgumentParser as _ArgumentParser
 from argparse import Namespace as _Namespace
+from typing import Optional as _Optional
 
 # third-party
 from vcorelib.args import CommandFunction as _CommandFunction
 from vcorelib.args import app_args as _app_args
 
 # internal
 from rcmpy.commands.all import commands
 
-COMMAND: _CommandFunction = lambda _: 1
+COMMAND: _Optional[_CommandFunction] = None
 
 
 def entry(args: _Namespace) -> int:
     """Execute the requested task."""
+
+    assert COMMAND is not None
     return COMMAND(args)
 
 
 def add_app_args(parser: _ArgumentParser) -> None:
     """Add application-specific arguments to the command-line parser."""
     global COMMAND  # pylint: disable=global-statement
     add, COMMAND = _app_args(commands, {})
```

### Comparing `rcmpy-0.2.0/rcmpy/commands/all.py` & `rcmpy-0.3.0/rcmpy/commands/all.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.2.0/rcmpy/commands/use.py` & `rcmpy-0.3.0/rcmpy/commands/use.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.2.0/rcmpy/commands/variant.py` & `rcmpy-0.3.0/rcmpy/commands/variant.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.2.0/rcmpy/commands/watch.py` & `rcmpy-0.3.0/rcmpy/commands/watch.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.2.0/rcmpy/entry.py` & `rcmpy-0.3.0/rcmpy/entry.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.2.0/rcmpy/environment/__init__.py` & `rcmpy-0.3.0/rcmpy/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.2.0/rcmpy/environment/base.py` & `rcmpy-0.3.0/rcmpy/environment/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,31 +5,37 @@
 # built-in
 from contextlib import ExitStack
 from typing import Optional
 
 # third-party
 from vcorelib.io.types import FileExtension
 from vcorelib.logging import LoggerMixin
+from vcorelib.paths import rel
 
 # internal
 from rcmpy import PKG_NAME
 from rcmpy.config import Config
+from rcmpy.paths import default_cache_directory
 from rcmpy.state import State
 
 
 class BaseEnvironment(LoggerMixin):
     """A class implementing this package's base runtime environment."""
 
     def __init__(self, state: State, stack: ExitStack) -> None:
         """Initialize this instance."""
 
         super().__init__()
         self.state = state
         self.stack = stack
         self._config: Optional[Config] = None
+        self._cache = default_cache_directory()
+
+        self._build = state.directory.joinpath("build")
+        self._build.mkdir(exist_ok=True)
 
         config_base = state.directory.joinpath(PKG_NAME)
 
         config_candidates = list(
             FileExtension.data_candidates(config_base, exists_only=True)
         )
 
@@ -38,20 +44,35 @@
                 "No config found: %s.",
                 list(
                     str(x) for x in FileExtension.data_candidates(config_base)
                 ),
             )
         else:
             assert len(config_candidates) == 1, config_candidates
-            self._config = Config.decode(config_candidates[0])
-            self.logger.info("Loaded config '%s'.", config_candidates[0])
-            self._init_loaded()
+            self._config = Config.decode(
+                config_candidates[0], includes_key="includes"
+            )
+            self.logger.info("Loaded config '%s'.", rel(config_candidates[0]))
+
+            # Ensure that any relative paths called out are relative to the
+            # root directory of the data repository.
+            self._config.update_root(state.directory)
+
+            # Consider the config not loaded if initialization fails.
+            #
+            # **Add this back in if initialization can actually fail.**
+            #
+            # if not self._init_loaded():
+            #     self.logger.info("Initialization failed!")
+            #     self._config = None
+            assert self._init_loaded()
 
-    def _init_loaded(self) -> None:
+    def _init_loaded(self) -> bool:
         """Called during initialization if a valid configuration is loaded."""
+        return True
 
     @property
     def config_loaded(self) -> bool:
         """Determine if this environment has loaded a config."""
         return self._config is not None
 
     @property
```

### Comparing `rcmpy-0.2.0/rcmpy/paths/__init__.py` & `rcmpy-0.3.0/rcmpy/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.2.0/rcmpy/schemas.py` & `rcmpy-0.3.0/rcmpy/schemas.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.2.0/rcmpy/state/__init__.py` & `rcmpy-0.3.0/rcmpy/state/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from logging import getLogger
 from pathlib import Path
 from typing import Iterator, cast
 
 # third-party
 from vcorelib.dict.cache import FileCache
 from vcorelib.io.types import JsonObject as _JsonObject
-from vcorelib.paths import Pathlike, normalize
+from vcorelib.paths import Pathlike, normalize, rel
 
 # internal
 from rcmpy.paths import default_config_directory, default_state_directory
 from rcmpy.schemas import RcmpyDictCodec as _RcmpyDictCodec
 
 LOG = getLogger(__name__)
 
@@ -32,31 +32,33 @@
 
         self.logger = LOG
 
         self.directory = normalize(
             cast(str, data.get("directory", default_config_directory()))
         ).resolve()
 
-        self.logger.info("Using directory '%s'.", self.directory)
+        self.logger.info("Using directory '%s'.", rel(self.directory))
 
         self.variant: str = cast(str, data["variant"])
         if self.variant:
             self.logger.info("Using variant '%s'.", self.variant)
 
     def set_directory(self, path: Pathlike) -> None:
         """Set a new directory to use as the data repository."""
 
         new_dir = normalize(path).resolve()
 
         if new_dir == self.directory:
-            self.logger.info("New directory '%s' same as current.", new_dir)
+            self.logger.info(
+                "New directory '%s' same as current.", rel(new_dir)
+            )
             return
 
         self.directory = new_dir
-        self.logger.info("Set directory to '%s'.", new_dir)
+        self.logger.info("Set directory to '%s'.", rel(new_dir))
 
     def set_variant(self, variant: str = None) -> None:
         """Set a new variant value."""
 
         if not variant:
             self.logger.info("Current variant: '%s'.", self.variant)
         elif variant != self.variant:
```

### Comparing `rcmpy-0.2.0/rcmpy/xdg/__init__.py` & `rcmpy-0.3.0/rcmpy/xdg/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.2.0/rcmpy.egg-info/PKG-INFO` & `rcmpy-0.3.0/rcmpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 0.2.0
+Version: 0.3.0
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=e6c457784db73e957b3b0da662d10294
+    hash=96aa8923f1d36b7eddcfda3f7e4d8171
     =====================================
 -->
 
-# rcmpy ([0.2.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([0.3.0](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
```

### Comparing `rcmpy-0.2.0/rcmpy.egg-info/SOURCES.txt` & `rcmpy-0.3.0/rcmpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcmpy-0.2.0/setup.py` & `rcmpy-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.2.0/tests/test_entry.py` & `rcmpy-0.3.0/tests/test_entry.py`

 * *Files identical despite different names*


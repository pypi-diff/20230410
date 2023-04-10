# Comparing `tmp/preface-0.1.3.tar.gz` & `tmp/preface-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preface-0.1.3.tar", last modified: Thu Sep 15 04:17:38 2022, max compression
+gzip compressed data, was "preface-0.1.4.tar", last modified: Mon Apr 10 16:52:42 2023, max compression
```

## Comparing `preface-0.1.3.tar` & `preface-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      113 2022-04-25 00:17:32.200013 preface-0.1.3/.gitignore
--rw-r--r--   0        0        0     1081 2022-04-24 14:38:11.593494 preface-0.1.3/LICENSE
--rw-r--r--   0        0        0      449 2022-04-24 23:26:31.091106 preface-0.1.3/README.rst
--rw-r--r--   0        0        0     3990 2022-09-15 04:17:36.209796 preface-0.1.3/preface/__init__.py
--rw-r--r--   0        0        0     2306 2022-09-15 04:02:14.210990 preface-0.1.3/preface/dict.py
--rw-r--r--   0        0        0        0 2022-04-24 17:49:39.575358 preface-0.1.3/preface/py.typed
--rw-r--r--   0        0        0      509 2022-09-15 04:14:08.661744 preface-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      139 2022-09-15 04:13:57.648274 preface-0.1.3/requirements/dev.txt
--rw-r--r--   0        0        0       38 2022-04-25 00:15:06.344814 preface-0.1.3/requirements/docs.txt
--rw-r--r--   0        0        0       43 2022-09-15 04:13:47.071786 preface-0.1.3/setup.cfg
--rw-r--r--   0        0        0        0 2021-02-19 13:45:03.243430 preface-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0      862 2022-09-15 04:04:41.365117 preface-0.1.3/tests/test_dict.py
--rw-r--r--   0        0        0     1374 2022-09-15 04:06:30.474925 preface-0.1.3/tests/test_preface.py
--rw-r--r--   0        0        0      360 2022-04-24 23:23:11.033293 preface-0.1.3/tox.ini
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 preface-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      120 2023-04-10 16:52:08.131901 preface-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1081 2022-04-24 14:38:11.593494 preface-0.1.4/LICENSE
+-rw-r--r--   0        0        0      449 2022-04-24 23:26:31.091106 preface-0.1.4/README.rst
+-rw-r--r--   0        0        0     3973 2023-04-10 16:51:19.662901 preface-0.1.4/preface/__init__.py
+-rw-r--r--   0        0        0     1149 2023-04-10 16:48:04.934428 preface-0.1.4/preface/concurrency.py
+-rw-r--r--   0        0        0     2306 2022-09-15 04:02:14.210990 preface-0.1.4/preface/dict.py
+-rw-r--r--   0        0        0        0 2022-04-24 17:49:39.575358 preface-0.1.4/preface/py.typed
+-rw-r--r--   0        0        0      509 2022-09-15 04:14:08.661744 preface-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-04-10 16:51:54.101456 preface-0.1.4/requirements/dev.txt
+-rw-r--r--   0        0        0       38 2022-04-25 00:15:06.344814 preface-0.1.4/requirements/docs.txt
+-rw-r--r--   0        0        0       43 2022-09-15 04:13:47.071786 preface-0.1.4/setup.cfg
+-rw-r--r--   0        0        0        0 2021-02-19 13:45:03.243430 preface-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      862 2022-09-15 04:04:41.365117 preface-0.1.4/tests/test_dict.py
+-rw-r--r--   0        0        0     1374 2022-09-15 04:06:30.474925 preface-0.1.4/tests/test_preface.py
+-rw-r--r--   0        0        0      377 2023-04-10 16:49:00.924969 preface-0.1.4/tox.ini
+-rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 preface-0.1.4/PKG-INFO
```

### Comparing `preface-0.1.3/LICENSE` & `preface-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `preface-0.1.3/preface/__init__.py` & `preface-0.1.4/preface/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Some helper functions and classes that I want in nearly every project."""
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 import enum
 import sys
 from typing import (
     Iterable,
     Iterator,
     List,
@@ -144,17 +144,14 @@
     """
     rows = [things[i:] for i in range(size)]
 
     return zip(*rows)
 
 
 def unwrap(maybe: Result[T]) -> T:
-    """
-
-    """
     if isinstance(maybe, Exception):
         raise maybe
 
     return maybe
 
 
 def never(value: NoReturn) -> NoReturn:
```

### Comparing `preface-0.1.3/preface/dict.py` & `preface-0.1.4/preface/dict.py`

 * *Files identical despite different names*

### Comparing `preface-0.1.3/tests/test_dict.py` & `preface-0.1.4/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `preface-0.1.3/tests/test_preface.py` & `preface-0.1.4/tests/test_preface.py`

 * *Files identical despite different names*

### Comparing `preface-0.1.3/PKG-INFO` & `preface-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preface
-Version: 0.1.3
+Version: 0.1.4
 Summary: Some helper functions and classes that I want in nearly every project.
 Author-email: Samuel Stevens <samuel.robert.stevens@gmail.com>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/samuelstevens/preface
 
 Python Preface
```


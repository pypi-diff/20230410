# Comparing `tmp/replit-3.2.5.tar.gz` & `tmp/replit-3.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit-3.2.5.tar", max compression
+gzip compressed data, was "replit-3.2.6.tar", max compression
```

## Comparing `replit-3.2.5.tar` & `replit-3.2.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      720 2022-10-21 17:43:10.441261 replit-3.2.5/LICENSE
--rw-r--r--   0        0        0      673 2022-10-21 17:43:10.441261 replit-3.2.5/README.md
--rw-r--r--   0        0        0     1272 2022-10-21 17:43:10.449261 replit-3.2.5/pyproject.toml
--rw-r--r--   0        0        0      410 2022-10-21 17:43:10.449261 replit-3.2.5/src/replit/__init__.py
--rw-r--r--   0        0        0     2868 2022-10-21 17:43:10.449261 replit-3.2.5/src/replit/__main__.py
--rw-r--r--   0        0        0      171 2022-10-21 17:43:10.449261 replit-3.2.5/src/replit/audio/Makefile
--rw-r--r--   0        0        0    13226 2022-10-21 17:43:10.449261 replit-3.2.5/src/replit/audio/__init__.py
--rw-r--r--   0        0        0     1848 2022-10-21 17:43:10.449261 replit-3.2.5/src/replit/audio/test.py
--rw-r--r--   0        0        0     3687 2022-10-21 17:43:10.449261 replit-3.2.5/src/replit/audio/types.py
--rw-r--r--   0        0        0      426 2022-10-21 17:43:10.449261 replit-3.2.5/src/replit/database/__init__.py
--rw-r--r--   0        0        0    18096 2022-10-21 17:43:10.449261 replit-3.2.5/src/replit/database/database.py
--rw-r--r--   0        0        0      314 2022-10-21 17:43:10.449261 replit-3.2.5/src/replit/database/default_db.py
--rw-r--r--   0        0        0     2239 2022-10-21 17:43:10.449261 replit-3.2.5/src/replit/database/server.py
--rw-r--r--   0        0        0       33 2022-10-21 17:43:10.449261 replit-3.2.5/src/replit/goval/__init__.py
--rw-r--r--   0        0        0        0 2022-10-21 17:43:10.449261 replit-3.2.5/src/replit/goval/api/__init__.py
--rw-r--r--   0        0        0     5198 2022-10-21 17:43:10.449261 replit-3.2.5/src/replit/goval/api/client_pb2.py
--rw-r--r--   0        0        0        0 2022-10-21 17:43:10.449261 replit-3.2.5/src/replit/goval/api/features/__init__.py
--rw-r--r--   0        0        0     1516 2022-10-21 17:43:10.449261 replit-3.2.5/src/replit/goval/api/features/features_pb2.py
--rw-r--r--   0        0        0        0 2022-10-21 17:43:10.449261 replit-3.2.5/src/replit/goval/api/repl/__init__.py
--rw-r--r--   0        0        0     3031 2022-10-21 17:43:10.449261 replit-3.2.5/src/replit/goval/api/repl/repl_pb2.py
--rw-r--r--   0        0        0     3563 2022-10-21 17:43:10.449261 replit-3.2.5/src/replit/goval/api/signing_pb2.py
--rw-r--r--   0        0        0      135 2022-10-21 17:43:10.449261 replit-3.2.5/src/replit/identity/__init__.py
--rw-r--r--   0        0        0      159 2022-10-21 17:43:10.453261 replit-3.2.5/src/replit/identity/exceptions.py
--rw-r--r--   0        0        0     9156 2022-10-21 17:43:10.453261 replit-3.2.5/src/replit/identity/verify.py
--rw-r--r--   0        0        0     2466 2022-10-21 17:43:10.453261 replit-3.2.5/src/replit/info.py
--rw-r--r--   0        0        0      352 2022-10-21 17:43:10.453261 replit-3.2.5/src/replit/web/__init__.py
--rw-r--r--   0        0        0     2589 2022-10-21 17:43:10.453261 replit-3.2.5/src/replit/web/app.py
--rw-r--r--   0        0        0     3329 2022-10-21 17:43:10.453261 replit-3.2.5/src/replit/web/user.py
--rw-r--r--   0        0        0     8552 2022-10-21 17:43:10.453261 replit-3.2.5/src/replit/web/utils.py
--rw-r--r--   0        0        0     1847 1970-01-01 00:00:00.000000 replit-3.2.5/setup.py
--rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 replit-3.2.5/PKG-INFO
+-rw-r--r--   0        0        0      720 2023-04-07 15:30:56.391990 replit-3.2.6/LICENSE
+-rw-r--r--   0        0        0      673 2023-04-07 15:30:56.391990 replit-3.2.6/README.md
+-rw-r--r--   0        0        0     1272 2023-04-10 20:11:04.049856 replit-3.2.6/pyproject.toml
+-rw-r--r--   0        0        0      410 2023-04-07 15:30:56.397991 replit-3.2.6/src/replit/__init__.py
+-rw-r--r--   0        0        0     2868 2023-04-07 15:30:56.397991 replit-3.2.6/src/replit/__main__.py
+-rw-r--r--   0        0        0      171 2023-04-07 15:30:56.397991 replit-3.2.6/src/replit/audio/Makefile
+-rw-r--r--   0        0        0    13226 2023-04-07 15:30:56.397991 replit-3.2.6/src/replit/audio/__init__.py
+-rw-r--r--   0        0        0     1848 2023-04-07 15:30:56.397991 replit-3.2.6/src/replit/audio/test.py
+-rw-r--r--   0        0        0     3687 2023-04-07 15:30:56.397991 replit-3.2.6/src/replit/audio/types.py
+-rw-r--r--   0        0        0      426 2023-04-07 15:30:56.397991 replit-3.2.6/src/replit/database/__init__.py
+-rw-r--r--   0        0        0    18106 2023-04-10 18:56:39.411937 replit-3.2.6/src/replit/database/database.py
+-rw-r--r--   0        0        0      508 2023-04-10 19:13:25.023719 replit-3.2.6/src/replit/database/default_db.py
+-rw-r--r--   0        0        0     2239 2023-04-07 15:30:56.397991 replit-3.2.6/src/replit/database/server.py
+-rw-r--r--   0        0        0       33 2023-04-07 15:30:56.398991 replit-3.2.6/src/replit/goval/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-07 15:30:56.398991 replit-3.2.6/src/replit/goval/api/__init__.py
+-rw-r--r--   0        0        0     5198 2023-04-07 15:30:56.398991 replit-3.2.6/src/replit/goval/api/client_pb2.py
+-rw-r--r--   0        0        0        0 2023-04-07 15:30:56.398991 replit-3.2.6/src/replit/goval/api/features/__init__.py
+-rw-r--r--   0        0        0     1516 2023-04-07 15:30:56.398991 replit-3.2.6/src/replit/goval/api/features/features_pb2.py
+-rw-r--r--   0        0        0        0 2023-04-07 15:30:56.398991 replit-3.2.6/src/replit/goval/api/repl/__init__.py
+-rw-r--r--   0        0        0     3031 2023-04-07 15:30:56.398991 replit-3.2.6/src/replit/goval/api/repl/repl_pb2.py
+-rw-r--r--   0        0        0     3563 2023-04-07 15:30:56.398991 replit-3.2.6/src/replit/goval/api/signing_pb2.py
+-rw-r--r--   0        0        0      135 2023-04-07 15:30:56.398991 replit-3.2.6/src/replit/identity/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-07 15:30:56.398991 replit-3.2.6/src/replit/identity/exceptions.py
+-rw-r--r--   0        0        0     9156 2023-04-07 15:30:56.398991 replit-3.2.6/src/replit/identity/verify.py
+-rw-r--r--   0        0        0     2466 2023-04-07 15:30:56.398991 replit-3.2.6/src/replit/info.py
+-rw-r--r--   0        0        0      352 2023-04-07 15:30:56.398991 replit-3.2.6/src/replit/web/__init__.py
+-rw-r--r--   0        0        0     2589 2023-04-07 15:30:56.398991 replit-3.2.6/src/replit/web/app.py
+-rw-r--r--   0        0        0     3329 2023-04-07 15:30:56.398991 replit-3.2.6/src/replit/web/user.py
+-rw-r--r--   0        0        0     8552 2023-04-07 15:30:56.398991 replit-3.2.6/src/replit/web/utils.py
+-rw-r--r--   0        0        0     1843 2023-04-10 20:11:25.269858 replit-3.2.6/setup.py
+-rw-r--r--   0        0        0     1611 2023-04-10 20:11:25.270225 replit-3.2.6/PKG-INFO
```

### Comparing `replit-3.2.5/LICENSE` & `replit-3.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `replit-3.2.5/README.md` & `replit-3.2.6/README.md`

 * *Files identical despite different names*

### Comparing `replit-3.2.5/pyproject.toml` & `replit-3.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "replit"
-version = "3.2.5"
+version = "3.2.6"
 description = "A library for interacting with features of repl.it"
 authors = ["Repl.it <contact@repl.it>", "mat <pypi@matdoes.dev>", "kennethreitz <me@kennethreitz.org>", "Scoder12 <pypi@scoder12.ml>", "AllAwesome497", ]
 license = "ISC"
 readme = "README.md"
 repository = "https://github.com/replit/replit-py"
 homepage = "https://github.com/replit/replit-py"
 documentation = "https://replit-py.readthedocs.org/"
```

### Comparing `replit-3.2.5/src/replit/__main__.py` & `replit-3.2.6/src/replit/__main__.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.5/src/replit/audio/__init__.py` & `replit-3.2.6/src/replit/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.5/src/replit/audio/test.py` & `replit-3.2.6/src/replit/audio/test.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.5/src/replit/audio/types.py` & `replit-3.2.6/src/replit/audio/types.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.5/src/replit/database/database.py` & `replit-3.2.6/src/replit/database/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Async and dict-like interfaces for interacting with Repl.it Database."""
 
 from collections import abc
 import json
+import os
 from typing import (
     AbstractSet,
     Any,
     Callable,
     Dict,
     Iterator,
     List,
```

### Comparing `replit-3.2.5/src/replit/database/server.py` & `replit-3.2.6/src/replit/database/server.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.5/src/replit/goval/api/client_pb2.py` & `replit-3.2.6/src/replit/goval/api/client_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.5/src/replit/goval/api/features/features_pb2.py` & `replit-3.2.6/src/replit/goval/api/features/features_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.5/src/replit/goval/api/repl/repl_pb2.py` & `replit-3.2.6/src/replit/goval/api/repl/repl_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.5/src/replit/goval/api/signing_pb2.py` & `replit-3.2.6/src/replit/goval/api/signing_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.5/src/replit/identity/verify.py` & `replit-3.2.6/src/replit/identity/verify.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.5/src/replit/info.py` & `replit-3.2.6/src/replit/info.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.5/src/replit/web/app.py` & `replit-3.2.6/src/replit/web/app.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.5/src/replit/web/user.py` & `replit-3.2.6/src/replit/web/user.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.5/src/replit/web/utils.py` & `replit-3.2.6/src/replit/web/utils.py`

 * *Files identical despite different names*

### Comparing `replit-3.2.5/setup.py` & `replit-3.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,21 +28,21 @@
  'typing_extensions>=3.7.4,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['replit = replit.__main__:cli']}
 
 setup_kwargs = {
     'name': 'replit',
-    'version': '3.2.5',
+    'version': '3.2.6',
     'description': 'A library for interacting with features of repl.it',
     'long_description': '### `>>> import replit`\n\n![compute](https://github.com/kennethreitz42/replit-py/blob/kr-cleanup/ext/readme.gif?raw=true)\n\nThis repository is the home for the `replit` Python package, which provides:\n\n- A fully-featured database client for [Replit DB](https://docs.repl.it/misc/database).\n- A Flask–based application framework for accelerating development on the platform.\n- Replit user profile metadata retrieval (more coming here!).\n- A simple audio library that can play tones and audio files!\n\n### Open Source License\n\nThis library is licensed under the [ISC License](https://en.wikipedia.org/wiki/ISC_license) and is free for you to use, change, or even profit from!\n',
     'author': 'Repl.it',
     'author_email': 'contact@repl.it',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
+    'maintainer': None,
+    'maintainer_email': None,
     'url': 'https://github.com/replit/replit-py',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<4.0',
```

### Comparing `replit-3.2.5/PKG-INFO` & `replit-3.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: replit
-Version: 3.2.5
+Version: 3.2.6
 Summary: A library for interacting with features of repl.it
 Home-page: https://github.com/replit/replit-py
 License: ISC
 Author: Repl.it
 Author-email: contact@repl.it
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Flask (>=2.0.0,<3.0.0)
 Requires-Dist: Werkzeug (>=2.0.0,<3.0.0)
 Requires-Dist: aiohttp (>=3.6.2,<4.0.0)
 Requires-Dist: protobuf (>=4.21.8,<5.0.0)
 Requires-Dist: pyseto (>=1.6.11,<2.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: typing_extensions (>=3.7.4,<4.0.0)
```


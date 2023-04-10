# Comparing `tmp/stoppy-1.0.4.tar.gz` & `tmp/stoppy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stoppy-1.0.4.tar", max compression
+gzip compressed data, was "stoppy-1.0.5.tar", max compression
```

## Comparing `stoppy-1.0.4.tar` & `stoppy-1.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1112 2022-12-05 09:33:37.873099 stoppy-1.0.4/README.md
--rw-r--r--   0        0        0      539 2022-12-05 09:34:32.337764 stoppy-1.0.4/pyproject.toml
--rw-r--r--   0        0        0       39 2022-12-05 08:08:57.177104 stoppy-1.0.4/stoppy/__init__.py
--rw-r--r--   0        0        0     1830 2022-12-05 09:27:50.017917 stoppy-1.0.4/stoppy/stopwatch.py
--rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 stoppy-1.0.4/setup.py
--rw-r--r--   0        0        0     1624 1970-01-01 00:00:00.000000 stoppy-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-10 10:15:12.822170 stoppy-1.0.5/LICENSE
+-rw-r--r--   0        0        0     1112 2023-02-19 06:24:32.190389 stoppy-1.0.5/README.md
+-rw-r--r--   0        0        0      538 2023-04-10 10:15:12.827497 stoppy-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-02-19 06:24:32.190951 stoppy-1.0.5/stoppy/__init__.py
+-rw-r--r--   0        0        0     1830 2023-02-19 06:24:32.191075 stoppy-1.0.5/stoppy/stopwatch.py
+-rw-r--r--   0        0        0     1773 1970-01-01 00:00:00.000000 stoppy-1.0.5/PKG-INFO
```

### Comparing `stoppy-1.0.4/README.md` & `stoppy-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `stoppy-1.0.4/pyproject.toml` & `stoppy-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "stoppy"
-version = "1.0.4"
+version = "1.0.5"
 description = "A precise and lightweight stopwatch built on top of `perf_counter`, which can be used as a replacement for `perf_counter` that returns absolute time starting from zero."
 authors = ["morefigs"]
 homepage = "https://github.com/morefigs/stoppy"
 readme = "README.md"
 packages = [{include = "stoppy"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.7"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `stoppy-1.0.4/stoppy/stopwatch.py` & `stoppy-1.0.5/stoppy/stopwatch.py`

 * *Files identical despite different names*

### Comparing `stoppy-1.0.4/setup.py` & `stoppy-1.0.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,56 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: stoppy
+Version: 1.0.5
+Summary: A precise and lightweight stopwatch built on top of `perf_counter`, which can be used as a replacement for `perf_counter` that returns absolute time starting from zero.
+Home-page: https://github.com/morefigs/stoppy
+Author: morefigs
+Requires-Python: >=3.7,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
 
-packages = \
-['stoppy']
+# stoppy ⏱
 
-package_data = \
-{'': ['*']}
+A precise and lightweight stopwatch built on top of `perf_counter`, which can be used as a replacement for `perf_counter` that returns absolute time starting from zero.
 
-setup_kwargs = {
-    'name': 'stoppy',
-    'version': '1.0.4',
-    'description': 'A precise and lightweight stopwatch built on top of `perf_counter`, which can be used as a replacement for `perf_counter` that returns absolute time starting from zero.',
-    'long_description': '# stoppy ⏱\n\nA precise and lightweight stopwatch built on top of `perf_counter`, which can be used as a replacement for `perf_counter` that returns absolute time starting from zero.\n\nThe stopwatch can optionally be started automatically by calling `time(True)` instead of `start()`, which can streamline usage when polling the time repeatedly.\n\n## Installation\n\nInstall from [PyPI](https://pypi.org/project/stoppy/) via:\n\n```shell\npip install stoppy\n```\n\n## Usage\n\nBasic usage is as follows:\n\n```python\nfrom time import sleep\nfrom stoppy import Stopwatch\n\nwith Stopwatch(start=True) as stopwatch:\n    sleep(0.1)\n    stopwatch.stop()\n    print(stopwatch.time())\n    stopwatch.reset()\n```\n\nIt can also be used as a direct replacement for `perf_counter` that returns absolute time starting from zero:\n\n```python\nfrom stoppy import Stopwatch\n\nwith Stopwatch() as stopwatch:\n    # Calling `stopwatch.time(True)` is equivalent to calling `perf_counter()`, but starts from exactly zero\n    print(stopwatch.time(True))\n```\n\nFor all usage examples see [examples/](https://github.com/morefigs/stoppy/tree/main/examples).\n',
-    'author': 'morefigs',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/morefigs/stoppy',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.10,<4.0',
-}
+The stopwatch can optionally be started automatically by calling `time(True)` instead of `start()`, which can streamline usage when polling the time repeatedly.
 
+## Installation
+
+Install from [PyPI](https://pypi.org/project/stoppy/) via:
+
+```shell
+pip install stoppy
+```
+
+## Usage
+
+Basic usage is as follows:
+
+```python
+from time import sleep
+from stoppy import Stopwatch
+
+with Stopwatch(start=True) as stopwatch:
+    sleep(0.1)
+    stopwatch.stop()
+    print(stopwatch.time())
+    stopwatch.reset()
+```
+
+It can also be used as a direct replacement for `perf_counter` that returns absolute time starting from zero:
+
+```python
+from stoppy import Stopwatch
+
+with Stopwatch() as stopwatch:
+    # Calling `stopwatch.time(True)` is equivalent to calling `perf_counter()`, but starts from exactly zero
+    print(stopwatch.time(True))
+```
+
+For all usage examples see [examples/](https://github.com/morefigs/stoppy/tree/main/examples).
 
-setup(**setup_kwargs)
```


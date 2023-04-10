# Comparing `tmp/retry_extended-0.2.0.tar.gz` & `tmp/retry_extended-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retry_extended-0.2.0.tar", max compression
+gzip compressed data, was "retry_extended-0.2.1.tar", max compression
```

## Comparing `retry_extended-0.2.0.tar` & `retry_extended-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-04-10 18:28:57.429966 retry_extended-0.2.0/LICENSE
--rw-r--r--   0        0        0     1219 2023-04-10 18:28:57.429966 retry_extended-0.2.0/README.md
--rw-r--r--   0        0        0     1172 2023-04-10 18:28:57.429966 retry_extended-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      252 2023-04-10 18:28:57.429966 retry_extended-0.2.0/retry/__init__.py
--rw-r--r--   0        0        0     7264 2023-04-10 18:28:57.429966 retry_extended-0.2.0/retry/api.py
--rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 retry_extended-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-10 19:08:56.975862 retry_extended-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1232 2023-04-10 19:08:56.975862 retry_extended-0.2.1/README.md
+-rw-r--r--   0        0        0     1172 2023-04-10 19:09:11.368620 retry_extended-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      252 2023-04-10 19:08:56.975862 retry_extended-0.2.1/retry/__init__.py
+-rw-r--r--   0        0        0     7280 2023-04-10 19:08:56.975862 retry_extended-0.2.1/retry/api.py
+-rw-r--r--   0        0        0     2429 1970-01-01 00:00:00.000000 retry_extended-0.2.1/PKG-INFO
```

### Comparing `retry_extended-0.2.0/LICENSE` & `retry_extended-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `retry_extended-0.2.0/README.md` & `retry_extended-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Retry Extended
-[![Lint](https://github.com/strollby/retry-extended/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/strollby/retry-extended/actions/workflows/lint.yml) [![Test Package](https://github.com/strollby/retry-extended/actions/workflows/test.yml/badge.svg)](https://github.com/strollby/retry-extended/actions/workflows/test.yml) [![Build Package](https://github.com/strollby/retry-extended/actions/workflows/build-main.yml/badge.svg?branch=main)](https://github.com/strollby/retry-extended/actions/workflows/build-main.yml) [![Publish to PyPI](https://github.com/strollby/retry-extended/actions/workflows/publish-release.yml/badge.svg)](https://github.com/strollby/retry-extended/actions/workflows/publish-release.yml) 
+[![Lint](https://github.com/strollby/retry-extended/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/strollby/retry-extended/actions/workflows/lint.yml) [![Test Package](https://github.com/strollby/retry-extended/actions/workflows/test.yml/badge.svg)](https://github.com/strollby/retry-extended/actions/workflows/test.yml) [![Build Package](https://github.com/strollby/retry-extended/actions/workflows/build-main.yml/badge.svg?branch=main)](https://github.com/strollby/retry-extended/actions/workflows/build-main.yml) [![Publish to PyPI](https://github.com/strollby/retry-extended/actions/workflows/publish-release.yml/badge.svg?event=release)](https://github.com/strollby/retry-extended/actions/workflows/publish-release.yml)
 
 
 
 Retry API compatible maintained project
 
 This package had been developed on top of the original python [retry](https://github.com/invl/retry) package, and is intended to develop on top of it without implementing any breaking API changes and keeping the simplicity of the package.
```

### Comparing `retry_extended-0.2.0/pyproject.toml` & `retry_extended-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "retry-extended"
-version = "0.2.0"
+version = "0.2.1"
 description = "Retry API compatible extended library"
 authors = ["Strollby Developers <backend.developers@strollby.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/strollby/retry-extended"
 repository = "https://github.com/strollby/retry-extended"
 documentation = "https://github.com/strollby/retry-extended"
```

### Comparing `retry_extended-0.2.0/retry/api.py` & `retry_extended-0.2.1/retry/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import inspect
 import logging
 import random
 import time
 
 from typing import Callable, Optional, Any
 
 
@@ -108,15 +107,15 @@
             default: retry.DEFAULT_LOGGER. if None, logging is disabled.
     Returns:
         Result of the f function.
     """
     _tries, _delay = tries, delay
     while _tries:
         try:
-            return await f(*args, *kwargs)
+            return await f(*args, **kwargs)
         except exceptions as e:
             _tries -= 1
             if not _tries:
                 raise
 
             if logger is not None:
                 logger.warning("%s, retrying in %s seconds...", e, _delay)
@@ -169,19 +168,22 @@
     """
 
     def retry_decorator(func):
         def wrapper(*args: dict, **kwargs: dict) -> Any:
             return __retry_internal(func, args, kwargs, exceptions, tries, delay, max_delay, backoff, jitter, logger)
 
         async def wrapper_async(*args: dict, **kwargs: dict) -> Any:
-            return await __retry_internal_async(func, args, kwargs, exceptions, tries, delay, max_delay, backoff, jitter, logger)
+            return await __retry_internal_async(
+                func, args, kwargs, exceptions, tries, delay, max_delay, backoff, jitter, logger
+            )
 
         if asyncio.iscoroutinefunction(func):
             return wrapper_async
         return wrapper
+
     return retry_decorator
 
 
 def retry_call(
     f,
     fargs: tuple = None,
     fkwargs: dict = None,
@@ -225,8 +227,7 @@
     """
     args = fargs if fargs else tuple()
     kwargs = fkwargs if fkwargs else dict()
 
     if asyncio.iscoroutinefunction(f):
         return __retry_internal_async(f, args, kwargs, exceptions, tries, delay, max_delay, backoff, jitter, logger)
     return __retry_internal(f, args, kwargs, exceptions, tries, delay, max_delay, backoff, jitter, logger)
-
```

### Comparing `retry_extended-0.2.0/PKG-INFO` & `retry_extended-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retry-extended
-Version: 0.2.0
+Version: 0.2.1
 Summary: Retry API compatible extended library
 Home-page: https://github.com/strollby/retry-extended
 License: Apache-2.0
 Keywords: retry,retry-extended,python-retry
 Author: Strollby Developers
 Author-email: backend.developers@strollby.com
 Requires-Python: >=3.7,<4.0
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Project-URL: Bug Tracker, https://github.com/strollby/retry-extended/issues
 Project-URL: Documentation, https://github.com/strollby/retry-extended
 Project-URL: Repository, https://github.com/strollby/retry-extended
 Description-Content-Type: text/markdown
 
 # Retry Extended
-[![Lint](https://github.com/strollby/retry-extended/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/strollby/retry-extended/actions/workflows/lint.yml) [![Test Package](https://github.com/strollby/retry-extended/actions/workflows/test.yml/badge.svg)](https://github.com/strollby/retry-extended/actions/workflows/test.yml) [![Build Package](https://github.com/strollby/retry-extended/actions/workflows/build-main.yml/badge.svg?branch=main)](https://github.com/strollby/retry-extended/actions/workflows/build-main.yml) [![Publish to PyPI](https://github.com/strollby/retry-extended/actions/workflows/publish-release.yml/badge.svg)](https://github.com/strollby/retry-extended/actions/workflows/publish-release.yml) 
+[![Lint](https://github.com/strollby/retry-extended/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/strollby/retry-extended/actions/workflows/lint.yml) [![Test Package](https://github.com/strollby/retry-extended/actions/workflows/test.yml/badge.svg)](https://github.com/strollby/retry-extended/actions/workflows/test.yml) [![Build Package](https://github.com/strollby/retry-extended/actions/workflows/build-main.yml/badge.svg?branch=main)](https://github.com/strollby/retry-extended/actions/workflows/build-main.yml) [![Publish to PyPI](https://github.com/strollby/retry-extended/actions/workflows/publish-release.yml/badge.svg?event=release)](https://github.com/strollby/retry-extended/actions/workflows/publish-release.yml)
 
 
 
 Retry API compatible maintained project
 
 This package had been developed on top of the original python [retry](https://github.com/invl/retry) package, and is intended to develop on top of it without implementing any breaking API changes and keeping the simplicity of the package.
```


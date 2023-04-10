# Comparing `tmp/toolrack-3.1.0.tar.gz` & `tmp/toolrack-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolrack-3.1.0.tar", last modified: Thu Mar  2 20:06:40 2023, max compression
+gzip compressed data, was "toolrack-4.0.0.tar", last modified: Mon Apr 10 07:52:25 2023, max compression
```

## Comparing `toolrack-3.1.0.tar` & `toolrack-4.0.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-03-02 20:06:40.810263 toolrack-3.1.0/
--rw-r--r--   0 ack       (1000) ack       (1000)     7651 2017-03-04 10:38:59.000000 toolrack-3.1.0/LICENSE.txt
--rw-rw-r--   0 ack       (1000) ack       (1000)    11695 2023-03-02 20:06:40.810263 toolrack-3.1.0/PKG-INFO
--rw-rw-r--   0 ack       (1000) ack       (1000)     1536 2021-11-21 17:00:15.000000 toolrack-3.1.0/README.rst
--rw-rw-r--   0 ack       (1000) ack       (1000)     2315 2023-03-02 19:51:35.000000 toolrack-3.1.0/pyproject.toml
--rw-rw-r--   0 ack       (1000) ack       (1000)       38 2023-03-02 20:06:40.810263 toolrack-3.1.0/setup.cfg
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-03-02 20:06:40.810263 toolrack-3.1.0/toolrack/
--rw-rw-r--   0 ack       (1000) ack       (1000)       90 2023-03-02 20:03:49.000000 toolrack-3.1.0/toolrack/__init__.py
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-03-02 20:06:40.810263 toolrack-3.1.0/toolrack/aio/
--rw-r--r--   0 ack       (1000) ack       (1000)      353 2020-05-10 07:50:32.000000 toolrack-3.1.0/toolrack/aio/__init__.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     3994 2023-03-02 19:51:35.000000 toolrack-3.1.0/toolrack/aio/periodic.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     3924 2023-03-02 19:51:35.000000 toolrack-3.1.0/toolrack/aio/process.py
--rw-rw-r--   0 ack       (1000) ack       (1000)      882 2023-03-02 19:51:35.000000 toolrack-3.1.0/toolrack/certificate.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     2954 2023-03-02 19:51:35.000000 toolrack-3.1.0/toolrack/collect.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     4900 2023-03-02 19:51:35.000000 toolrack-3.1.0/toolrack/config.py
--rw-r--r--   0 ack       (1000) ack       (1000)      926 2019-12-01 08:21:52.000000 toolrack-3.1.0/toolrack/convert.py
--rw-r--r--   0 ack       (1000) ack       (1000)     2704 2019-12-01 08:21:52.000000 toolrack-3.1.0/toolrack/fsmap.py
--rw-r--r--   0 ack       (1000) ack       (1000)      921 2019-12-01 08:21:52.000000 toolrack-3.1.0/toolrack/iterate.py
--rw-r--r--   0 ack       (1000) ack       (1000)      719 2019-12-01 08:21:52.000000 toolrack-3.1.0/toolrack/json_util.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     1491 2023-03-02 19:51:35.000000 toolrack-3.1.0/toolrack/log.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     2086 2023-03-02 19:51:35.000000 toolrack-3.1.0/toolrack/password.py
--rw-r--r--   0 ack       (1000) ack       (1000)      717 2019-12-01 08:21:52.000000 toolrack-3.1.0/toolrack/path.py
--rw-rw-r--   0 ack       (1000) ack       (1000)      528 2023-03-02 19:43:11.000000 toolrack-3.1.0/toolrack/property.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     3366 2023-03-02 19:51:35.000000 toolrack-3.1.0/toolrack/script.py
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-03-02 20:06:40.810263 toolrack-3.1.0/toolrack/scripts/
--rw-r--r--   0 ack       (1000) ack       (1000)       29 2018-03-10 11:52:14.000000 toolrack-3.1.0/toolrack/scripts/__init__.py
--rw-r--r--   0 ack       (1000) ack       (1000)     1211 2019-12-01 08:21:52.000000 toolrack-3.1.0/toolrack/scripts/certinfo.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     2283 2023-03-02 19:51:35.000000 toolrack-3.1.0/toolrack/scripts/password_generator.py
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-03-02 20:06:40.810263 toolrack-3.1.0/toolrack/testing/
--rw-r--r--   0 ack       (1000) ack       (1000)      105 2019-12-01 08:21:52.000000 toolrack-3.1.0/toolrack/testing/__init__.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     5093 2023-03-02 19:51:35.000000 toolrack-3.1.0/toolrack/testing/fixtures.py
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-03-02 20:06:40.810263 toolrack-3.1.0/toolrack/testing/tests/
--rw-r--r--   0 ack       (1000) ack       (1000)        0 2017-02-14 09:36:59.000000 toolrack-3.1.0/toolrack/testing/tests/__init__.py
--rw-r--r--   0 ack       (1000) ack       (1000)     1463 2019-12-01 08:21:52.000000 toolrack-3.1.0/toolrack/threading.py
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-03-02 20:06:40.810263 toolrack-3.1.0/toolrack.egg-info/
--rw-rw-r--   0 ack       (1000) ack       (1000)    11695 2023-03-02 20:06:40.000000 toolrack-3.1.0/toolrack.egg-info/PKG-INFO
--rw-rw-r--   0 ack       (1000) ack       (1000)      775 2023-03-02 20:06:40.000000 toolrack-3.1.0/toolrack.egg-info/SOURCES.txt
--rw-rw-r--   0 ack       (1000) ack       (1000)        1 2023-03-02 20:06:40.000000 toolrack-3.1.0/toolrack.egg-info/dependency_links.txt
--rw-rw-r--   0 ack       (1000) ack       (1000)      127 2023-03-02 20:06:40.000000 toolrack-3.1.0/toolrack.egg-info/entry_points.txt
--rw-rw-r--   0 ack       (1000) ack       (1000)       45 2023-03-02 20:06:40.000000 toolrack-3.1.0/toolrack.egg-info/requires.txt
--rw-rw-r--   0 ack       (1000) ack       (1000)        9 2023-03-02 20:06:40.000000 toolrack-3.1.0/toolrack.egg-info/top_level.txt
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-04-10 07:52:24.996296 toolrack-4.0.0/
+-rw-r--r--   0 ack       (1000) ack       (1000)     7651 2017-03-04 10:38:59.000000 toolrack-4.0.0/LICENSE.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)    11323 2023-04-10 07:52:24.996296 toolrack-4.0.0/PKG-INFO
+-rw-rw-r--   0 ack       (1000) ack       (1000)     1164 2023-04-10 07:43:55.000000 toolrack-4.0.0/README.rst
+-rw-rw-r--   0 ack       (1000) ack       (1000)     2310 2023-04-10 07:41:50.000000 toolrack-4.0.0/pyproject.toml
+-rw-rw-r--   0 ack       (1000) ack       (1000)       38 2023-04-10 07:52:24.996296 toolrack-4.0.0/setup.cfg
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-04-10 07:52:24.996296 toolrack-4.0.0/toolrack/
+-rw-rw-r--   0 ack       (1000) ack       (1000)       90 2023-04-10 07:43:26.000000 toolrack-4.0.0/toolrack/__init__.py
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-04-10 07:52:24.996296 toolrack-4.0.0/toolrack/aio/
+-rw-r--r--   0 ack       (1000) ack       (1000)      353 2020-05-10 07:50:32.000000 toolrack-4.0.0/toolrack/aio/__init__.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     4016 2023-04-10 07:41:32.000000 toolrack-4.0.0/toolrack/aio/periodic.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     4362 2023-03-25 19:26:19.000000 toolrack-4.0.0/toolrack/aio/process.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)      887 2023-03-11 23:49:28.000000 toolrack-4.0.0/toolrack/certificate.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     2954 2023-03-10 16:26:52.000000 toolrack-4.0.0/toolrack/collect.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     5032 2023-04-10 07:41:32.000000 toolrack-4.0.0/toolrack/config.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)      965 2023-04-10 07:41:32.000000 toolrack-4.0.0/toolrack/convert.py
+-rw-r--r--   0 ack       (1000) ack       (1000)     2704 2019-12-01 08:21:52.000000 toolrack-4.0.0/toolrack/fsmap.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     1012 2023-04-10 07:41:32.000000 toolrack-4.0.0/toolrack/iterate.py
+-rw-r--r--   0 ack       (1000) ack       (1000)      733 2023-03-11 23:49:28.000000 toolrack-4.0.0/toolrack/json_util.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     1491 2023-03-10 16:26:52.000000 toolrack-4.0.0/toolrack/log.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     2086 2023-03-10 16:26:52.000000 toolrack-4.0.0/toolrack/password.py
+-rw-r--r--   0 ack       (1000) ack       (1000)      717 2019-12-01 08:21:52.000000 toolrack-4.0.0/toolrack/path.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)      622 2023-04-10 07:41:32.000000 toolrack-4.0.0/toolrack/property.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     3303 2023-04-10 07:41:50.000000 toolrack-4.0.0/toolrack/script.py
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-04-10 07:52:24.996296 toolrack-4.0.0/toolrack/scripts/
+-rw-r--r--   0 ack       (1000) ack       (1000)       29 2018-03-10 11:52:14.000000 toolrack-4.0.0/toolrack/scripts/__init__.py
+-rw-r--r--   0 ack       (1000) ack       (1000)     1246 2023-03-11 23:49:28.000000 toolrack-4.0.0/toolrack/scripts/certinfo.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     2483 2023-04-10 07:41:50.000000 toolrack-4.0.0/toolrack/scripts/password_generator.py
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-04-10 07:52:24.996296 toolrack-4.0.0/toolrack/testing/
+-rw-r--r--   0 ack       (1000) ack       (1000)      105 2019-12-01 08:21:52.000000 toolrack-4.0.0/toolrack/testing/__init__.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     5482 2023-04-10 07:41:50.000000 toolrack-4.0.0/toolrack/testing/fixtures.py
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-04-10 07:52:24.996296 toolrack-4.0.0/toolrack/testing/tests/
+-rw-r--r--   0 ack       (1000) ack       (1000)        0 2017-02-14 09:36:59.000000 toolrack-4.0.0/toolrack/testing/tests/__init__.py
+-rw-r--r--   0 ack       (1000) ack       (1000)     1463 2019-12-01 08:21:52.000000 toolrack-4.0.0/toolrack/threading.py
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-04-10 07:52:24.996296 toolrack-4.0.0/toolrack.egg-info/
+-rw-rw-r--   0 ack       (1000) ack       (1000)    11323 2023-04-10 07:52:24.000000 toolrack-4.0.0/toolrack.egg-info/PKG-INFO
+-rw-rw-r--   0 ack       (1000) ack       (1000)      775 2023-04-10 07:52:24.000000 toolrack-4.0.0/toolrack.egg-info/SOURCES.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)        1 2023-04-10 07:52:24.000000 toolrack-4.0.0/toolrack.egg-info/dependency_links.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)      127 2023-04-10 07:52:24.000000 toolrack-4.0.0/toolrack.egg-info/entry_points.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)       45 2023-04-10 07:52:24.000000 toolrack-4.0.0/toolrack.egg-info/requires.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)        9 2023-04-10 07:52:24.000000 toolrack-4.0.0/toolrack.egg-info/top_level.txt
```

### Comparing `toolrack-3.1.0/LICENSE.txt` & `toolrack-4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `toolrack-3.1.0/PKG-INFO` & `toolrack-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolrack
-Version: 3.1.0
+Version: 4.0.0
 Summary: A collection of miscellaneous utility functions and classes
 Author-email: Alberto Donato <alberto.donato@gmail.com>
 Maintainer-email: Alberto Donato <alberto.donato@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -190,16 +190,15 @@
 License-File: LICENSE.txt
 
 ToolRack
 ========
 
 |Latest Version| |Build Status| |Coverage Status| |Documentation|
 
-A collection of utility functions and classes, and a few scripts too.
-
+A collection of miscellaneous utility functions and classes, and a few scripts.
 
 Documentation
 -------------
 
 API docs are available on ReadTheDocs_.
 
 
@@ -211,33 +210,14 @@
 As a user run:
 
 .. code:: bash
 
   $ pip install toolrack
 
 
-Development installation
-------------------------
-
-The source tree is available available at
-`<https://github.com/albertodonato/toolrack>`_.
-
-Development setup can be done via Virtualenv.
-
-As a user run:
-
-.. code:: bash
-
-  $ python3 -m venv <target-dir>
-  $ . <target-dir>/bin/activate
-  $ git clone https://github.com/albertodonato/toolrack
-  $ cd toolrack
-  $ pip install -e .
-
-
 .. _ReadTheDocs: https://toolrack.readthedocs.io/en/latest/
 .. _PyPI: https://pypi.python.org/
 
 .. |Latest Version| image:: https://img.shields.io/pypi/v/toolrack.svg
    :alt: Latest Version
    :target: https://pypi.python.org/pypi/toolrack
 .. |Build Status| image:: https://github.com/albertodonato/toolrack/workflows/CI/badge.svg
```

### Comparing `toolrack-3.1.0/README.rst` & `toolrack-4.0.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 ToolRack
 ========
 
 |Latest Version| |Build Status| |Coverage Status| |Documentation|
 
-A collection of utility functions and classes, and a few scripts too.
-
+A collection of miscellaneous utility functions and classes, and a few scripts.
 
 Documentation
 -------------
 
 API docs are available on ReadTheDocs_.
 
 
@@ -20,33 +19,14 @@
 As a user run:
 
 .. code:: bash
 
   $ pip install toolrack
 
 
-Development installation
-------------------------
-
-The source tree is available available at
-`<https://github.com/albertodonato/toolrack>`_.
-
-Development setup can be done via Virtualenv.
-
-As a user run:
-
-.. code:: bash
-
-  $ python3 -m venv <target-dir>
-  $ . <target-dir>/bin/activate
-  $ git clone https://github.com/albertodonato/toolrack
-  $ cd toolrack
-  $ pip install -e .
-
-
 .. _ReadTheDocs: https://toolrack.readthedocs.io/en/latest/
 .. _PyPI: https://pypi.python.org/
 
 .. |Latest Version| image:: https://img.shields.io/pypi/v/toolrack.svg
    :alt: Latest Version
    :target: https://pypi.python.org/pypi/toolrack
 .. |Build Status| image:: https://github.com/albertodonato/toolrack/workflows/CI/badge.svg
```

### Comparing `toolrack-3.1.0/pyproject.toml` & `toolrack-4.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 password-generator = "toolrack.scripts.password_generator:script"
 
 [tool.setuptools.packages.find]
 include = ["toolrack*"]
 [tool.setuptools.dynamic]
 version = {attr = "toolrack.__version__"}
 
+[tool.black]
+line-length = 79
+
 [tool.isort]
 combine_as_imports = true
 force_grid_wrap = 2
 force_sort_within_sections = true
 from_first = false
 include_trailing_comma = true
 multi_line_output = 3
@@ -84,9 +87,8 @@
 source = ["toolrack"]
 omit = ["toolrack/scripts/*"]
 
 [tool.mypy]
 ignore_missing_imports = true
 install_types = true
 non_interactive = true
-warn_return_any = true
-warn_unused_configs = true
+strict = true
```

### Comparing `toolrack-3.1.0/toolrack/aio/periodic.py` & `toolrack-4.0.0/toolrack/aio/periodic.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,35 +12,32 @@
     Task,
 )
 from collections.abc import (
     Callable,
     Iterator,
 )
 from functools import partial
-from typing import (
-    cast,
-    Union,
-)
+from typing import cast
 
 
 class AlreadyRunning(Exception):
     """The TimedCall is already running."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__("Timed call is already running")
 
 
 class NotRunning(Exception):
     """The TimedCall is not running."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__("Timed call is not running")
 
 
-TimesIterator = Iterator[Union[float, int]]
+TimesIterator = Iterator[float | int]
 
 
 class TimedCall:
     """Call a function based on a timer.
 
     The class takes a function with optional arguments. Upon
     :meth:`start()`, the function is scheduled at specified times
@@ -48,15 +45,15 @@
 
     :param func: the function to call periodically.
     :param args: arguments to pass to the function.
     :param kwargs: keyword arguments to pass to the function.
 
     """
 
-    def __init__(self, func: Callable, *args, **kwargs):
+    def __init__(self, func: Callable, *args, **kwargs) -> None:
         self._func = self._wrap_func(func, *args, **kwargs)
         self._loop = get_event_loop()
         self._handle: Handle | None = None
         self._task: Task | None = None
 
     @property
     def running(self) -> bool:
@@ -72,32 +69,32 @@
 
         """
         if self.running:
             raise AlreadyRunning()
 
         self._run(times_iter, do_call=False)
 
-    async def stop(self):
+    async def stop(self) -> None:
         """Stop calling the function periodically."""
         if not self.running:
             raise NotRunning()
 
         if self._handle:
             self._handle.cancel()
             self._handle = None
         if self._task:
             await self._task
             self._task = None
 
-    def _run(self, times_iter: TimesIterator, do_call: bool = True):
+    def _run(self, times_iter: TimesIterator, do_call: bool = True) -> None:
         if do_call:
             self._task = self._loop.create_task(self._func())
         self._schedule_next_run(times_iter)
 
-    def _schedule_next_run(self, times_iter: TimesIterator):
+    def _schedule_next_run(self, times_iter: TimesIterator) -> None:
         delay = self._get_run_delay(times_iter)
         if delay is None:
             self._handle = None
         else:
             self._handle = self._loop.call_later(delay, self._run, times_iter)
 
     def _get_run_delay(self, times_iter: TimesIterator) -> float | None:
```

### Comparing `toolrack-3.1.0/toolrack/aio/process.py` & `toolrack-4.0.0/toolrack/aio/process.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,126 +1,142 @@
 """Protocol class for collecting a process stdout/stderr."""
 
 from asyncio import (
     Future,
+    get_event_loop,
     SubprocessProtocol,
 )
 from collections.abc import Callable
 from io import StringIO
-from locale import getpreferredencoding
-from typing import (
-    cast,
-    IO,
-)
+from typing import cast
 
 
 class ProcessParserProtocol(SubprocessProtocol):
     """Collect process stdout and stderr.
 
-    Line parser functions can be passed for stdout and stderr, and they are
-    called on each full line of output.
+    If parser functions are be passed for stdout and/or stderr, they are called
+    on each full line of output.
+
+    If no parser function is passed, the full output content is returned when
+    the process terminates via the ``done`` :class:`Future`.  This returns a
+    tuple with the full stdout and stderr. Each tuple element is ``None`` if a
+    parser is passed for that stream.
 
-    When the process ends, the ``future`` returns a tuple with the full stdout
-    and stderr. Each tuple element is ``None`` if a parser is passed for that
-    stream.
-
-    :param asyncio.Future future: a Future called with a tuple with
-        (stdout, stderr) from the process once it it exits.
-    :param callable out_parser: an optional parser for the process standard
-        output.
-    :param callable err_parser: an optional parser for the process standard
-        error.
+    :param out_parser: an optional parser for the process standard output.
+    :param err_parser: an optional parser for the process standard error.
 
     """
 
-    def __init__(self, future: Future, out_parser=None, err_parser=None):
-        self.future = future
-        self._outputs = {
-            fd: StreamHelper(callback=parser)
-            for fd, parser in enumerate((out_parser, err_parser), 1)
+    done: Future
+
+    def __init__(self, out_parser=None, err_parser=None):
+        self.done = get_event_loop().create_future()
+        self._streams = {
+            1: StreamHelper(callback=out_parser),
+            2: StreamHelper(callback=err_parser),
         }
+        self._data = [None, None]  # hold stdout/stderr data
+        self._exception = None
+        self._process_exited = False
 
     def pipe_data_received(self, fd, data):
-        stream = self._outputs[fd]
-        data = data.decode(getpreferredencoding(False))
-        stream.receive_data(data)
-
-    def connection_lost(self, exc):
-        self._outputs[1].flush_partial()
-        self._outputs[2].flush_partial()
-        stdout = self._outputs[1].get_data()
-        stderr = self._outputs[2].get_data()
+        stream = self._streams.get(fd)
+        if stream:
+            stream.receive_data(data.decode())
+
+    def pipe_connection_lost(self, fd, exc):
+        stream = self._streams.pop(fd, None)
+        if not stream:
+            return
+
+        stream.flush_partial()
+        self._data[fd - 1] = stream.get_data()
         if exc:
-            self.future.set_exception(exc)
+            self._exception = exc
+        self._maybe_done()
+
+    def process_exited(self):
+        self._process_exited = True
+        self._maybe_done()
+
+    def _maybe_done(self):
+        if not self._process_exited or self._streams:
+            return
+
+        if self._exception:
+            self.done.set_exception(self._exception)
         else:
-            self.future.set_result((stdout, stderr))
+            self.done.set_result(tuple(self._data))
 
 
 class StreamHelper:
     """Helper to cache data until full lines of text are received.
 
     This is useful to collect data from a stream and process them when full
     lines are received.
     For example::
 
-      stream = StreamHelper(callback)
+      stream = StreamHelper(callback=callback)
       stream.receive_data('line one\\nline two')
       stream.receive_data('continues here\\n')
 
     would call ``callback`` twice, one with ``'line one'`` and one with
     ``'line two continues here'``
 
     :param callable callback: an optional function which is called with full
         lines of text from the stream.
     :param str separator: the line separator
 
     """
 
     def __init__(
-        self, callback: Callable[[str], None] | None = None, separator: str = "\n"
+        self,
+        callback: Callable[[str], None] | None = None,
+        separator: str = "\n",
     ):
         self.separator = separator
         self._callback = callback
-        self._buffer = StringIO() if not callback else None
+        self._buffer = StringIO()
         self._partial = StringIO()
 
     def receive_data(self, data: str):
         """Receive data and process them.
 
         If a ``callback`` has been passed to the class, it's called for each
         full line of text.
 
         """
         if self._callback:
             self._parse_data(data)
         else:
-            cast(IO, self._buffer).write(data)
+            self._buffer.write(data)
 
-    def get_data(self):
-        """Return the full content of the stream."""
-        if not self._buffer:
-            return
+    def get_data(self) -> str | None:
+        """Return the full content of the stream if no callback is defined."""
+        if self._callback:
+            return None
         return self._buffer.getvalue() + self._partial.getvalue()
 
     def flush_partial(self):
         """Flush and process pending data from a partial line."""
         if not self._callback:
             return
         partial = self._partial.getvalue()
         if partial:
             self._callback(partial)
 
     def _parse_data(self, data: str):
         """Process data parsing full lines."""
         lines = data.split(self.separator)
-        lines[0] = self._pop_partial() + lines[0]
+        if len(lines) > 1:  # at least one full line
+            lines[0] = self._pop_partial() + lines[0]
+        # might be empty if data ended with separator
         self._partial.write(lines.pop())
-        # Call the callback on full lines
+        # call the callback on full lines
         for line in lines:
-            if line:
-                cast(Callable, self._callback)(line)
+            cast(Callable, self._callback)(line)
 
     def _pop_partial(self):
         """Return the current partial line and reset it."""
         line = self._partial.getvalue()
-        self._partial.truncate()
+        self._partial.truncate(0)
         return line
```

### Comparing `toolrack-3.1.0/toolrack/certificate.py` & `toolrack-4.0.0/toolrack/certificate.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from collections.abc import Callable
 from ssl import get_server_certificate
 from urllib.parse import urlsplit
 
 
 def get_host_certificate(
-    uri: str, get_func: Callable[[tuple[str, int]], str] = get_server_certificate
+    uri: str,
+    get_func: Callable[[tuple[str, int]], str] = get_server_certificate,
 ) -> str:
     """Return a string with the host certificate.
 
     :param str uri: the host URI, in the form :data:`[scheme://]host[:port]`.
         The scheme is optional (and ignored), and port defaults to 443.
 
     """
```

### Comparing `toolrack-3.1.0/toolrack/collect.py` & `toolrack-4.0.0/toolrack/collect.py`

 * *Files identical despite different names*

### Comparing `toolrack-3.1.0/toolrack/config.py` & `toolrack-4.0.0/toolrack/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,38 +38,40 @@
     """Collection of type converters for ConfigKeys."""
 
     # Base types
     _type_int = int
     _type_float = float
     _type_str = str
 
-    def get_converter(self, _type: str) -> Callable:
+    def get_converter(self, _type: str) -> Callable[[Any], Any]:
         """Return the converter method for the specified type."""
         if _type.endswith("[]"):
             _type = _type.strip("[]")
             elem_converter = self.get_converter(_type)
             converter = partial(self._type_list, elem_converter)
         else:
             try:
                 converter = getattr(self, f"_type_{_type}")
             except AttributeError:
                 raise TypeError(_type)
 
         return converter
 
-    def _type_bool(self, value) -> bool:
+    def _type_bool(self, value: Any) -> bool:
         """Convert to boolean.
 
         Accepted values for True are 'true', 'yes' and '1', case insensitive.
         """
         if isinstance(value, str):
             return value.lower() in ("true", "yes", "1")
         return bool(value)
 
-    def _type_list(self, converter: Callable, value) -> list:
+    def _type_list(
+        self, converter: Callable[[Any], Any], value: Any
+    ) -> list[Any]:
         """Convert to list."""
         if isinstance(value, str):
             value = value.split()
         return [converter(item) for item in value]
 
 
 class ConfigKey:
@@ -89,57 +91,56 @@
         self.description = description
         self.required = required
         self.default = default
         self.validator = validator
         self.description
         self._config_types = ConfigKeyTypes()
 
-    def parse(self, value):
+    def parse(self, value: Any) -> Any:
         """Convert and validate a value."""
         try:
             value = self._convert(value)
             self._validate(value)
         except ValueError:
             raise InvalidConfigValue(self.name)
         return value
 
-    def validate(self, value):
+    def validate(self, value: Any) -> None:
         """Validate a value based for the key.
 
         Can be overridden by subclasses. It should raise a ValueError if the
         value is invalid.
         """
-        pass
 
-    def _validate(self, value):
+    def _validate(self, value: Any) -> None:
         """Call the type validator."""
         self.validate(value)
         if self.validator is not None:
             self.validator(value)
 
-    def _convert(self, value):
+    def _convert(self, value: Any) -> Any:
         """Convert the value to the proper type."""
         converter = self._config_types.get_converter(self.type)
         return converter(value)
 
 
 class Config:
     """Parse a configuration dictionary.
 
     A configuration has a set of keys of specific types.
     """
 
     def __init__(self, *keys: ConfigKey):
         self._config_keys = {key.name: key for key in keys}
 
-    def keys(self):
+    def keys(self) -> list[ConfigKey]:
         """Return ConfigKeys sorted by name alphabetically."""
         return sorted(self._config_keys.values(), key=attrgetter("name"))
 
-    def extend(self, *keys):
+    def extend(self, *keys: ConfigKey) -> "Config":
         """Return a new Config with additional keys."""
         all_keys = self._config_keys.copy()
         all_keys.update((key.name, key) for key in keys)
         return Config(*all_keys.values())
 
     def parse(self, config: dict[str, Any] | None) -> dict[str, Any]:
         """Parse the provided configuration dict.
```

### Comparing `toolrack-3.1.0/toolrack/convert.py` & `toolrack-4.0.0/toolrack/convert.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """Utilities for unit conversion."""
 
 #: Binary byte multipliers
 BYTE_SUFFIXES = (None, "kib", "mib", "gib", "tib", "pib", "eib", "zib", "yib")
 
 
-def convert_bbyte(value, suffix=None, to=None):
+def convert_bbyte(
+    value: int, suffix: str | None = None, to: str | None = None
+) -> int:
     """Convert a binary byte value across multipliers.
 
-    :param int value: the current value.
-    :param str suffix: the current multiplier for the value (:data:`None`
+    :param value: the current value.
+    :param suffix: the current multiplier for the value (:data:`None`
         for bytes).
-    :param str to: the target multiplier (:data:`None` for bytes).
+    :param to: the target multiplier (:data:`None` for bytes).
 
     """
     if suffix:
         suffix = suffix.lower()
     if suffix not in BYTE_SUFFIXES:
         raise ValueError("Unknown multiplier suffix")
     if to not in BYTE_SUFFIXES:
         raise ValueError("Unknown target multiplier")
-    multiplier = 2 ** (10 * BYTE_SUFFIXES.index(suffix))
+    multiplier: int = 2 ** (10 * BYTE_SUFFIXES.index(suffix))
     converted = value * multiplier
     if to:
         to = to.lower()
         divider = 2 ** (10 * BYTE_SUFFIXES.index(to))
         converted = converted / divider
     return converted
```

### Comparing `toolrack-3.1.0/toolrack/fsmap.py` & `toolrack-4.0.0/toolrack/fsmap.py`

 * *Files identical despite different names*

### Comparing `toolrack-3.1.0/toolrack/json_util.py` & `toolrack-4.0.0/toolrack/json_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,9 +16,11 @@
     :param out_fd: output file descriptor.
     :param int indent: number of spaces used for indentation.
     :param bool ensure_ascii: passed to the JSON serializer, if specified,
         non-ASCII characters are escaped.
 
     """
     data = load(in_fd)
-    dump(data, out_fd, sort_keys=True, ensure_ascii=ensure_ascii, indent=indent)
+    dump(
+        data, out_fd, sort_keys=True, ensure_ascii=ensure_ascii, indent=indent
+    )
     out_fd.write("\n")
```

### Comparing `toolrack-3.1.0/toolrack/log.py` & `toolrack-4.0.0/toolrack/log.py`

 * *Files identical despite different names*

### Comparing `toolrack-3.1.0/toolrack/password.py` & `toolrack-4.0.0/toolrack/password.py`

 * *Files identical despite different names*

### Comparing `toolrack-3.1.0/toolrack/path.py` & `toolrack-4.0.0/toolrack/path.py`

 * *Files identical despite different names*

### Comparing `toolrack-3.1.0/toolrack/script.py` & `toolrack-4.0.0/toolrack/script.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     """Raised to exit the process with the specified message and exit code.
 
     :param message: the error message.
     :param code: the script exit code.
 
     """
 
-    def __init__(self, message: str, code: int = 1):
+    def __init__(self, message: str, code: int = 1) -> None:
         self.message = message
         self.code = code
 
 
 class Script:
     """Wraps a python script handling argument parsing.
 
@@ -56,62 +56,61 @@
     the message outputted to standard error.
 
     Script instances are callable, and can be passed the argument list (which
     defaults to :data:`sys.argv` if not provided).
 
     """
 
-    def __init__(self, stdout: IO | None = None, stderr: IO | None = None):
+    def __init__(
+        self, stdout: IO | None = None, stderr: IO | None = None
+    ) -> None:
         self._stdout = stdout or sys.stdout
         self._stderr = stderr or sys.stderr
 
     def get_parser(self) -> ArgumentParser:
         """Return a configured :class:`argparse.ArgumentParser` instance.
 
         .. note::
             Subclasses must implement this method.
 
         """
         raise NotImplementedError()
 
-    def main(self, args: Namespace):
+    def main(self, args: Namespace) -> int | None:
         """The body of the script.
 
         It gets called with the :class:`argparse.Namespace` instance returned
         by :func:`get_parser`.
 
         :param args: command line arguments.
 
         .. note::
             Subclasses must implement this method.
 
         """
         raise NotImplementedError()
 
-    def exit(self, code: int = 0):
+    def exit(self, code: int = 0) -> None:
         """Exit with the specified return code."""
         sys.exit(code)
 
     def handle_keyboard_interrupt(self, interrupt: KeyboardInterrupt):
         """Called when a :class:`KeyboardInterrupt` is raised.
 
         By default it just traps the exception and exits with success.
         It can be overridden to perform additional cleanups.
 
         """
         self.exit()
 
-    def __call__(self, args: list[str] | None = None):
+    def __call__(self, args: list[str] | None = None) -> int:
         """Call the script, passing :data:`sys.argv` by default."""
         parser = self.get_parser()
         parsed_args = parser.parse_args(args=args)
         try:
-            self.main(parsed_args)
+            return self.main(parsed_args) or 0
         except KeyboardInterrupt as interrupt:
             self.handle_keyboard_interrupt(interrupt)
         except ErrorExitMessage as error:
-            self._error_exit(error)
-
-    def _error_exit(self, error: ErrorExitMessage):
-        """Terminate with the specified :class:`ErrorExitMessage`."""
-        self._stderr.write(f"{error.message}\n")
-        self.exit(error.code)
+            self._stderr.write(f"{error.message}\n")
+            self.exit(error.code)
+        return 0
```

### Comparing `toolrack-3.1.0/toolrack/scripts/certinfo.py` & `toolrack-4.0.0/toolrack/scripts/certinfo.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,25 +9,28 @@
 )
 
 
 class CertInfo(Script):
     """Get information about SSL certificates."""
 
     def get_parser(self):
-        parser = ArgumentParser(description="Get information about SSL certificates.")
+        parser = ArgumentParser(
+            description="Get information about SSL certificates."
+        )
         subparsers = parser.add_subparsers(
             metavar="ACTION", dest="action", help="action to perform"
         )
         subparsers.required = True
 
         get_cert_parser = subparsers.add_parser(
             "get-cert", help="get certificate for a host"
         )
         get_cert_parser.add_argument(
-            "hostname", help="hostname in the host[:port] format. Port defaults to 443"
+            "hostname",
+            help="hostname in the host[:port] format. Port defaults to 443",
         )
         return parser
 
     def main(self, args):
         action = args.action.replace("-", "_")
         method = getattr(self, "action_" + action)
         method(args)
```

### Comparing `toolrack-3.1.0/toolrack/scripts/password_generator.py` & `toolrack-4.0.0/toolrack/scripts/password_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """Generate random passwords."""
 
-from argparse import ArgumentParser
+from argparse import (
+    ArgumentParser,
+    Namespace,
+)
 from collections import OrderedDict
 
 from ..password import (
     DEFAULT_LENGTH,
     PasswordProfile,
 )
 from ..script import Script
@@ -16,40 +19,50 @@
     ]
 )
 
 
 class PasswordGenerator(Script):
     """Script to generate random passwords."""
 
-    def get_parser(self):
+    def get_parser(self) -> ArgumentParser:
         parser = ArgumentParser(description="Generate random passwords")
         parser.add_argument(
             "-n", type=int, default=1, help="number of passwords to generate"
         )
         parser.add_argument(
-            "-l", "--length", type=int, default=DEFAULT_LENGTH, help="password length"
+            "-l",
+            "--length",
+            type=int,
+            default=DEFAULT_LENGTH,
+            help="password length",
         )
         parser.add_argument(
             "-p",
             "--profile",
             default="default",
             help=(
                 "profile to use. Can be the name of a defined profile or a "
                 "sequence of character definitions."
             ),
         )
         parser.add_argument(
-            "-L", "--list-profiles", action="store_true", help="list available profiles"
+            "-L",
+            "--list-profiles",
+            action="store_true",
+            help="list available profiles",
         )
         parser.add_argument(
-            "-d", "--list-defs", action="store_true", help="list characters definitions"
+            "-d",
+            "--list-defs",
+            action="store_true",
+            help="list characters definitions",
         )
         return parser
 
-    def main(self, args):
+    def main(self, args: Namespace) -> None:
         if args.list_profiles:
             self._list_profiles()
             self.exit()
 
         if args.list_defs:
             self._list_definitions()
             self.exit()
@@ -59,20 +72,20 @@
         else:
             profile = PasswordProfile(args.profile)
 
         for _ in range(args.n):
             password = profile.generate(length=args.length)
             print(password)
 
-    def _list_profiles(self):
+    def _list_profiles(self) -> None:
         """List available profiles."""
         for name, profile in PROFILES.items():
             message = "{}:\n  definition: {}\n  characters: {}"
             print(message.format(name, profile.definition, profile.chars))
 
-    def _list_definitions(self):
+    def _list_definitions(self) -> None:
         """List available character set definitions."""
         for tag, chars in PasswordProfile.CHAR_DEFS.items():
             print(f"{tag}: {chars!r}")
 
 
 script = PasswordGenerator()
```

### Comparing `toolrack-3.1.0/toolrack/testing/fixtures.py` & `toolrack-4.0.0/toolrack/testing/fixtures.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,44 +19,49 @@
 class Dir:
     """A helper for creating files and directories under a base directory.
 
     This is meant to be used for test fixtures.
 
     """
 
-    def __init__(self, path: Path):
-        self.path = path
+    def __init__(self, path: str | Path):
+        self.path = Path(path)
 
-    def __truediv__(self, other):
+    def __truediv__(self, other: Path) -> Path:
         """Append to the path."""
         return self.path / other
 
-    def __str__(self):
+    def __str__(self) -> str:
         """The path as string."""
         return str(self.path)
 
-    def join(self, *paths):
+    def join(self, *paths: str | Path) -> Path:
         """Join the specified path fragments with directory prefix."""
         return self.path.joinpath(*paths)
 
-    def mkdir(self, path=None):
+    def mkdir(self, path: str | None = None) -> Path:
         """Create a temporary directory and return the :class:`pathlib.Path`.
 
         By default, a random name is chosen.
 
         :param path: if specified, it's appended to the base directory and all
             intermiediate directories are created too.
             A relative path *must* be specified.
             A tuple of strings can be also passed, in which case elements are
             joined using :func:`os.path.sep`.
 
         """
         return self._mkpath(path, mkdtemp, os.mkdir)
 
-    def mkfile(self, path=None, content="", mode=None):
+    def mkfile(
+        self,
+        path: str | Path | None = None,
+        content: str = "",
+        mode: int | None = None,
+    ) -> Path:
         """Create a temporary file and return the :class:`pathlib.Path`.
 
         By default, a random name is chosen.
 
         :param path: if specified, it's appended to the base directory and all
             intermiediate directories are created too.
             A relative path *must* be specified.
@@ -71,15 +76,17 @@
         if content:
             path.write_text(content)
 
         if mode is not None:
             path.chmod(mode)
         return path
 
-    def mksymlink(self, target, path=None):
+    def mksymlink(
+        self, target: str | Path, path: str | Path | None = None
+    ) -> Path:
         """Create a symbolic link and return the :class:`pathlib.Path`.
 
         By default, a random name is chosen.
 
         :param target: path of the symlink target.
         :param path: if specified, it's appended to the base directory and all
             intermiediate directories are created too.
@@ -90,15 +97,20 @@
         """
         return self._mkpath(
             path,
             partial(self._mkstemp_symlink, target),
             lambda p: Path(p).symlink_to(target),
         )
 
-    def _mkpath(self, path, create_temp, create_func):
+    def _mkpath(
+        self,
+        path: str | Path | tuple[str | Path] | None,
+        create_temp,
+        create_func,
+    ) -> Path:
         if path is None:
             return Path(create_temp(dir=str(self.path)))
 
         if isinstance(path, tuple):
             path = Path().joinpath(*path)
         else:
             path = Path(path)
@@ -107,20 +119,22 @@
 
         path = self.path / path
         # ensure parent exists
         path.parent.mkdir(parents=True, exist_ok=True)
         create_func(str(path))
         return path
 
-    def _mkstemp(self, dir=None):
+    def _mkstemp(self, dir: str | Path | None = None) -> Path:
         fd, path = mkstemp(dir=dir)
         os.close(fd)
         return Path(path)
 
-    def _mkstemp_symlink(self, target, dir=None):
+    def _mkstemp_symlink(
+        self, target: str | Path, dir: str | Path | None = None
+    ) -> Path:
         path = self._mkstemp(dir=dir)
         path.unlink()
         path.symlink_to(target)
         return path
 
 
 @pytest.fixture
```

### Comparing `toolrack-3.1.0/toolrack/threading.py` & `toolrack-4.0.0/toolrack/threading.py`

 * *Files identical despite different names*

### Comparing `toolrack-3.1.0/toolrack.egg-info/PKG-INFO` & `toolrack-4.0.0/toolrack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolrack
-Version: 3.1.0
+Version: 4.0.0
 Summary: A collection of miscellaneous utility functions and classes
 Author-email: Alberto Donato <alberto.donato@gmail.com>
 Maintainer-email: Alberto Donato <alberto.donato@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -190,16 +190,15 @@
 License-File: LICENSE.txt
 
 ToolRack
 ========
 
 |Latest Version| |Build Status| |Coverage Status| |Documentation|
 
-A collection of utility functions and classes, and a few scripts too.
-
+A collection of miscellaneous utility functions and classes, and a few scripts.
 
 Documentation
 -------------
 
 API docs are available on ReadTheDocs_.
 
 
@@ -211,33 +210,14 @@
 As a user run:
 
 .. code:: bash
 
   $ pip install toolrack
 
 
-Development installation
-------------------------
-
-The source tree is available available at
-`<https://github.com/albertodonato/toolrack>`_.
-
-Development setup can be done via Virtualenv.
-
-As a user run:
-
-.. code:: bash
-
-  $ python3 -m venv <target-dir>
-  $ . <target-dir>/bin/activate
-  $ git clone https://github.com/albertodonato/toolrack
-  $ cd toolrack
-  $ pip install -e .
-
-
 .. _ReadTheDocs: https://toolrack.readthedocs.io/en/latest/
 .. _PyPI: https://pypi.python.org/
 
 .. |Latest Version| image:: https://img.shields.io/pypi/v/toolrack.svg
    :alt: Latest Version
    :target: https://pypi.python.org/pypi/toolrack
 .. |Build Status| image:: https://github.com/albertodonato/toolrack/workflows/CI/badge.svg
```

### Comparing `toolrack-3.1.0/toolrack.egg-info/SOURCES.txt` & `toolrack-4.0.0/toolrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/adaptive_scheduler-1.7.0.tar.gz` & `tmp/adaptive_scheduler-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptive_scheduler-1.7.0.tar", last modified: Tue Mar 28 16:38:17 2023, max compression
+gzip compressed data, was "adaptive_scheduler-1.8.0.tar", last modified: Mon Apr 10 19:35:50 2023, max compression
```

## Comparing `adaptive_scheduler-1.7.0.tar` & `adaptive_scheduler-1.8.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:38:17.477740 adaptive_scheduler-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-28 16:38:04.000000 adaptive_scheduler-1.7.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-03-28 16:38:04.000000 adaptive_scheduler-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-28 16:38:04.000000 adaptive_scheduler-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-03-28 16:38:17.477740 adaptive_scheduler-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-03-28 16:38:04.000000 adaptive_scheduler-1.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:38:17.477740 adaptive_scheduler-1.7.0/adaptive_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-28 16:38:04.000000 adaptive_scheduler-1.7.0/adaptive_scheduler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6835 2023-03-28 16:38:04.000000 adaptive_scheduler-1.7.0/adaptive_scheduler/_mock_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-28 16:38:17.477740 adaptive_scheduler-1.7.0/adaptive_scheduler/_static_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-03-28 16:38:04.000000 adaptive_scheduler-1.7.0/adaptive_scheduler/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-03-28 16:38:04.000000 adaptive_scheduler-1.7.0/adaptive_scheduler/client_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-03-28 16:38:04.000000 adaptive_scheduler-1.7.0/adaptive_scheduler/run_script.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)    33523 2023-03-28 16:38:04.000000 adaptive_scheduler-1.7.0/adaptive_scheduler/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-03-28 16:38:04.000000 adaptive_scheduler-1.7.0/adaptive_scheduler/sequence_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    51548 2023-03-28 16:38:04.000000 adaptive_scheduler-1.7.0/adaptive_scheduler/server_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    27698 2023-03-28 16:38:04.000000 adaptive_scheduler-1.7.0/adaptive_scheduler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-03-28 16:38:04.000000 adaptive_scheduler-1.7.0/adaptive_scheduler/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:38:17.477740 adaptive_scheduler-1.7.0/adaptive_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-03-28 16:38:17.000000 adaptive_scheduler-1.7.0/adaptive_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-28 16:38:17.000000 adaptive_scheduler-1.7.0/adaptive_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 16:38:17.000000 adaptive_scheduler-1.7.0/adaptive_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-28 16:38:17.000000 adaptive_scheduler-1.7.0/adaptive_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-28 16:38:17.000000 adaptive_scheduler-1.7.0/adaptive_scheduler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-28 16:38:04.000000 adaptive_scheduler-1.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-28 16:38:17.477740 adaptive_scheduler-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-28 16:38:04.000000 adaptive_scheduler-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:35:50.799599 adaptive_scheduler-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-04-10 19:35:50.799599 adaptive_scheduler-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:35:50.803598 adaptive_scheduler-1.8.0/adaptive_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6835 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/_mock_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 19:35:50.803598 adaptive_scheduler-1.8.0/adaptive_scheduler/_static_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/client_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/run_script.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    33523 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/sequence_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51548 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/server_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27703 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:35:50.799599 adaptive_scheduler-1.8.0/adaptive_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-04-10 19:35:50.000000 adaptive_scheduler-1.8.0/adaptive_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-10 19:35:50.000000 adaptive_scheduler-1.8.0/adaptive_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:35:50.000000 adaptive_scheduler-1.8.0/adaptive_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-10 19:35:50.000000 adaptive_scheduler-1.8.0/adaptive_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 19:35:50.000000 adaptive_scheduler-1.8.0/adaptive_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-10 19:35:50.803598 adaptive_scheduler-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/setup.py
```

### Comparing `adaptive_scheduler-1.7.0/LICENSE` & `adaptive_scheduler-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-1.7.0/PKG-INFO` & `adaptive_scheduler-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive_scheduler
-Version: 1.7.0
+Version: 1.8.0
 Summary: Run many `adaptive.Learner`s on many cores (>10k) using `mpi4py.futures`, `ipyparallel`, `dask-mpi`, or `process-pool`.
 Home-page: https://github.com/basnijholt/adaptive-scheduler
 Download-URL: https://pypi.python.org/pypi/adaptive_scheduler
 Maintainer: Bas Nijholt
 Maintainer-email: bas@nijho.lt
 License: BSD-3
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `adaptive_scheduler-1.7.0/README.rst` & `adaptive_scheduler-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-1.7.0/adaptive_scheduler/_mock_scheduler.py` & `adaptive_scheduler-1.8.0/adaptive_scheduler/_mock_scheduler.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-1.7.0/adaptive_scheduler/_version.py` & `adaptive_scheduler-1.8.0/adaptive_scheduler/_version.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-1.7.0/adaptive_scheduler/client_support.py` & `adaptive_scheduler-1.8.0/adaptive_scheduler/client_support.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-1.7.0/adaptive_scheduler/run_script.py.j2` & `adaptive_scheduler-1.8.0/adaptive_scheduler/run_script.py.j2`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-1.7.0/adaptive_scheduler/scheduler.py` & `adaptive_scheduler-1.8.0/adaptive_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-1.7.0/adaptive_scheduler/sequence_learner.py` & `adaptive_scheduler-1.8.0/adaptive_scheduler/sequence_learner.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-1.7.0/adaptive_scheduler/server_support.py` & `adaptive_scheduler-1.8.0/adaptive_scheduler/server_support.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-1.7.0/adaptive_scheduler/utils.py` & `adaptive_scheduler-1.8.0/adaptive_scheduler/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 import adaptive
 import cloudpickle
 import numpy as np
 import pandas as pd
 import toolz
 from adaptive.notebook_integration import in_ipynb
-from ipyparallel import Client
 from rich.console import Console
 from tqdm import tqdm, tqdm_notebook
 
 console = Console()
 
 MAX_LINE_LENGTH = 100
 _NONE_RETURN_STR = "__ReturnsNone__"
@@ -503,14 +502,16 @@
         Folder that is added to the path of the engines, e.g. ``"~/Work/my_current_project"``.
 
     Returns
     -------
     client : `ipyparallel.Client` object
         An IPyparallel client.
     """
+    from ipyparallel import Client
+
     client = Client(profile=profile, **(client_kwargs or {}))
     dview = _wait_for_successful_ipyparallel_client_start(client, n, timeout)
     dview.use_dill()
 
     if folder is not None:
         console.print(f"Adding {folder} to path.")
         cmd = f"import sys, os; sys.path.append(os.path.expanduser('{folder}'))"
```

### Comparing `adaptive_scheduler-1.7.0/adaptive_scheduler/widgets.py` & `adaptive_scheduler-1.8.0/adaptive_scheduler/widgets.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-1.7.0/adaptive_scheduler.egg-info/PKG-INFO` & `adaptive_scheduler-1.8.0/adaptive_scheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive-scheduler
-Version: 1.7.0
+Version: 1.8.0
 Summary: Run many `adaptive.Learner`s on many cores (>10k) using `mpi4py.futures`, `ipyparallel`, `dask-mpi`, or `process-pool`.
 Home-page: https://github.com/basnijholt/adaptive-scheduler
 Download-URL: https://pypi.python.org/pypi/adaptive_scheduler
 Maintainer: Bas Nijholt
 Maintainer-email: bas@nijho.lt
 License: BSD-3
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `adaptive_scheduler-1.7.0/adaptive_scheduler.egg-info/SOURCES.txt` & `adaptive_scheduler-1.8.0/adaptive_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-1.7.0/setup.py` & `adaptive_scheduler-1.8.0/setup.py`

 * *Files identical despite different names*


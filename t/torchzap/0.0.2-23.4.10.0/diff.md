# Comparing `tmp/torchzap-0.0.2.tar.gz` & `tmp/torchzap-23.4.10.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchzap-0.0.2.tar", last modified: Fri Mar 31 09:52:05 2023, max compression
+gzip compressed data, was "torchzap-23.4.10.0.tar", last modified: Mon Apr 10 00:21:46 2023, max compression
```

## Comparing `torchzap-0.0.2.tar` & `torchzap-23.4.10.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-03-31 09:52:05.886428 torchzap-0.0.2/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      354 2023-03-31 09:52:05.886428 torchzap-0.0.2/PKG-INFO
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        5 2023-03-31 07:38:53.000000 torchzap-0.0.2/README.md
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       38 2023-03-31 09:52:05.886428 torchzap-0.0.2/setup.cfg
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      728 2023-03-31 09:10:55.000000 torchzap-0.0.2/setup.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-03-31 09:52:05.886428 torchzap-0.0.2/torchzap/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-03-31 07:41:48.000000 torchzap-0.0.2/torchzap/__init__.py
--rwxr-xr-x   0 gaoang    (1001) gaoang    (1001)      638 2023-03-31 07:55:32.000000 torchzap-0.0.2/torchzap/preprocessing.py
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     6222 2023-03-31 07:40:01.000000 torchzap-0.0.2/torchzap/trainer.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-03-31 09:52:05.886428 torchzap-0.0.2/torchzap.egg-info/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      354 2023-03-31 09:52:05.000000 torchzap-0.0.2/torchzap.egg-info/PKG-INFO
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      244 2023-03-31 09:52:05.000000 torchzap-0.0.2/torchzap.egg-info/SOURCES.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        1 2023-03-31 09:52:05.000000 torchzap-0.0.2/torchzap.egg-info/dependency_links.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       61 2023-03-31 09:52:05.000000 torchzap-0.0.2/torchzap.egg-info/requires.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        9 2023-03-31 09:52:05.000000 torchzap-0.0.2/torchzap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:21:46.882202 torchzap-23.4.10.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-10 00:21:46.882202 torchzap-23.4.10.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 00:21:29.000000 torchzap-23.4.10.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 00:21:46.882202 torchzap-23.4.10.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-10 00:21:29.000000 torchzap-23.4.10.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:21:46.882202 torchzap-23.4.10.0/torchzap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 00:21:29.000000 torchzap-23.4.10.0/torchzap/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-04-10 00:21:29.000000 torchzap-23.4.10.0/torchzap/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-04-10 00:21:29.000000 torchzap-23.4.10.0/torchzap/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:21:46.882202 torchzap-23.4.10.0/torchzap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-10 00:21:46.000000 torchzap-23.4.10.0/torchzap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-10 00:21:46.000000 torchzap-23.4.10.0/torchzap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 00:21:46.000000 torchzap-23.4.10.0/torchzap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-10 00:21:46.000000 torchzap-23.4.10.0/torchzap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 00:21:46.000000 torchzap-23.4.10.0/torchzap.egg-info/top_level.txt
```

### Comparing `torchzap-0.0.2/setup.py` & `torchzap-23.4.10.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import setuptools
+import codefast as cf 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="torchzap",
-    version="0.0.2",  # Latest version .
+    version=cf.generate_version(),
     author="tompz",
     author_email="mailto@gmail.com",
     description="PyTorch Zap",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/private_repo/",
     packages=setuptools.find_packages(),
```

### Comparing `torchzap-0.0.2/torchzap/preprocessing.py` & `torchzap-23.4.10.0/torchzap/preprocessing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 
-from typing import List
-
 import codefast as cf
 
+from typing import List, Union, Callable, Set, Dict, Tuple, Optional, Any
+
 
 class LabelEncoder(object):
 
     def __init__(self, labels: List[str] = None):
         self.label2id = {}
         self.id2label = {}
         if labels:
```

### Comparing `torchzap-0.0.2/torchzap/trainer.py` & `torchzap-23.4.10.0/torchzap/trainer.py`

 * *Files identical despite different names*


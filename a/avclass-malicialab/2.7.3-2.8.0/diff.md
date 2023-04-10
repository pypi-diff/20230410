# Comparing `tmp/avclass-malicialab-2.7.3.tar.gz` & `tmp/avclass-malicialab-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avclass-malicialab-2.7.3.tar", last modified: Thu Mar 23 08:32:13 2023, max compression
+gzip compressed data, was "avclass-malicialab-2.8.0.tar", last modified: Mon Apr 10 14:58:13 2023, max compression
```

## Comparing `avclass-malicialab-2.7.3.tar` & `avclass-malicialab-2.8.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-03-23 08:32:13.533906 avclass-malicialab-2.7.3/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)     1100 2020-09-01 17:16:19.000000 avclass-malicialab-2.7.3/LICENSE
--rw-rw-r--   0 juanca    (1000) juanca    (1000)       23 2023-02-23 10:39:34.000000 avclass-malicialab-2.7.3/MANIFEST.in
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    17096 2023-03-23 08:32:13.533906 avclass-malicialab-2.7.3/PKG-INFO
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    15296 2023-02-27 10:51:14.000000 avclass-malicialab-2.7.3/README.md
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-03-23 08:32:13.533906 avclass-malicialab-2.7.3/avclass/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      401 2023-02-23 10:09:56.000000 avclass-malicialab-2.7.3/avclass/__init__.py
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    20210 2023-03-23 08:28:38.000000 avclass-malicialab-2.7.3/avclass/common.py
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-03-23 08:32:13.533906 avclass-malicialab-2.7.3/avclass/data/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)     6823 2023-02-23 10:09:56.000000 avclass-malicialab-2.7.3/avclass/data/andropup.expansion
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      308 2023-02-26 20:25:08.000000 avclass-malicialab-2.7.3/avclass/data/default.expansion
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    24120 2023-02-26 20:25:08.000000 avclass-malicialab-2.7.3/avclass/data/default.tagging
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    15901 2023-02-26 20:25:08.000000 avclass-malicialab-2.7.3/avclass/data/default.taxonomy
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)     4202 2023-02-26 07:44:35.000000 avclass-malicialab-2.7.3/avclass/evaluate.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)    23606 2023-02-27 10:51:54.000000 avclass-malicialab-2.7.3/avclass/labeler.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)     3996 2023-03-04 13:05:26.000000 avclass-malicialab-2.7.3/avclass/misp.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)     1704 2023-02-26 07:00:49.000000 avclass-malicialab-2.7.3/avclass/normalize.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)    17636 2023-02-23 10:26:36.000000 avclass-malicialab-2.7.3/avclass/update.py
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-03-23 08:32:13.533906 avclass-malicialab-2.7.3/avclass_malicialab.egg-info/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    17096 2023-03-23 08:32:13.000000 avclass-malicialab-2.7.3/avclass_malicialab.egg-info/PKG-INFO
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      511 2023-03-23 08:32:13.000000 avclass-malicialab-2.7.3/avclass_malicialab.egg-info/SOURCES.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)        1 2023-03-23 08:32:13.000000 avclass-malicialab-2.7.3/avclass_malicialab.egg-info/dependency_links.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      162 2023-03-23 08:32:13.000000 avclass-malicialab-2.7.3/avclass_malicialab.egg-info/entry_points.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)        8 2023-03-23 08:32:13.000000 avclass-malicialab-2.7.3/avclass_malicialab.egg-info/top_level.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      831 2023-03-23 08:29:41.000000 avclass-malicialab-2.7.3/pyproject.toml
--rw-rw-r--   0 juanca    (1000) juanca    (1000)       38 2023-03-23 08:32:13.533906 avclass-malicialab-2.7.3/setup.cfg
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-04-10 14:58:13.194088 avclass-malicialab-2.8.0/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)     1100 2020-09-01 17:16:19.000000 avclass-malicialab-2.8.0/LICENSE
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)       23 2023-02-23 10:39:34.000000 avclass-malicialab-2.8.0/MANIFEST.in
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-04-10 14:58:13.194088 avclass-malicialab-2.8.0/PKG-INFO
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    15317 2023-04-10 14:11:52.000000 avclass-malicialab-2.8.0/README.md
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-04-10 14:58:13.194088 avclass-malicialab-2.8.0/avclass/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      401 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.0/avclass/__init__.py
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    20210 2023-03-23 08:28:38.000000 avclass-malicialab-2.8.0/avclass/common.py
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-04-10 14:58:13.194088 avclass-malicialab-2.8.0/avclass/data/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)     6823 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.0/avclass/data/andropup.expansion
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      308 2023-04-10 14:08:05.000000 avclass-malicialab-2.8.0/avclass/data/default.expansion
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    56429 2023-04-10 14:08:05.000000 avclass-malicialab-2.8.0/avclass/data/default.tagging
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    41254 2023-04-10 14:08:05.000000 avclass-malicialab-2.8.0/avclass/data/default.taxonomy
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)     4202 2023-02-26 07:44:35.000000 avclass-malicialab-2.8.0/avclass/evaluate.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)    23606 2023-02-27 10:51:54.000000 avclass-malicialab-2.8.0/avclass/labeler.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)     3996 2023-03-04 13:05:26.000000 avclass-malicialab-2.8.0/avclass/misp.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)     1704 2023-02-26 07:00:49.000000 avclass-malicialab-2.8.0/avclass/normalize.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)    17636 2023-02-23 10:26:36.000000 avclass-malicialab-2.8.0/avclass/update.py
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-04-10 14:58:13.194088 avclass-malicialab-2.8.0/avclass_malicialab.egg-info/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-04-10 14:58:13.000000 avclass-malicialab-2.8.0/avclass_malicialab.egg-info/PKG-INFO
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      511 2023-04-10 14:58:13.000000 avclass-malicialab-2.8.0/avclass_malicialab.egg-info/SOURCES.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)        1 2023-04-10 14:58:13.000000 avclass-malicialab-2.8.0/avclass_malicialab.egg-info/dependency_links.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      162 2023-04-10 14:58:13.000000 avclass-malicialab-2.8.0/avclass_malicialab.egg-info/entry_points.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)        8 2023-04-10 14:58:13.000000 avclass-malicialab-2.8.0/avclass_malicialab.egg-info/top_level.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      831 2023-04-10 14:09:05.000000 avclass-malicialab-2.8.0/pyproject.toml
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)       38 2023-04-10 14:58:13.194088 avclass-malicialab-2.8.0/setup.cfg
```

### Comparing `avclass-malicialab-2.7.3/LICENSE` & `avclass-malicialab-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.7.3/PKG-INFO` & `avclass-malicialab-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avclass-malicialab
-Version: 2.7.3
+Version: 2.8.0
 Summary: AVClass is a Python package and command line tool to tag / label malware samples.
 Author: MaliciaLab
 License: MIT License
         
         Copyright (c) 2016-2020 MaliciaLab @ IMDEA Software Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -470,13 +470,13 @@
 
 ## Contributors
 
 Several members of the MaliciaLab at the
 [IMDEA Software Institute](http://software.imdea.org)
 have contributed to AVClass:
 Marcos Sebastián, Richard Rivera, Platon Kotzias, Srdjan Matic,
-Silvia Sebastián, and Juan Caballero.
+Silvia Sebastián, Kevin van Liebergen, and Juan Caballero.
 
 GitHub users with significant contributions to AVClass include
 (let us know if you believe you should be listed here):
 [eljeffeg](https://github.com/eljeffeg)
```

### Comparing `avclass-malicialab-2.7.3/README.md` & `avclass-malicialab-2.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -433,13 +433,13 @@
 
 ## Contributors
 
 Several members of the MaliciaLab at the
 [IMDEA Software Institute](http://software.imdea.org)
 have contributed to AVClass:
 Marcos Sebastián, Richard Rivera, Platon Kotzias, Srdjan Matic,
-Silvia Sebastián, and Juan Caballero.
+Silvia Sebastián, Kevin van Liebergen, and Juan Caballero.
 
 GitHub users with significant contributions to AVClass include
 (let us know if you believe you should be listed here):
 [eljeffeg](https://github.com/eljeffeg)
```

### Comparing `avclass-malicialab-2.7.3/avclass/common.py` & `avclass-malicialab-2.8.0/avclass/common.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.7.3/avclass/data/andropup.expansion` & `avclass-malicialab-2.8.0/avclass/data/andropup.expansion`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.7.3/avclass/evaluate.py` & `avclass-malicialab-2.8.0/avclass/evaluate.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.7.3/avclass/labeler.py` & `avclass-malicialab-2.8.0/avclass/labeler.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.7.3/avclass/misp.py` & `avclass-malicialab-2.8.0/avclass/misp.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.7.3/avclass/normalize.py` & `avclass-malicialab-2.8.0/avclass/normalize.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.7.3/avclass/update.py` & `avclass-malicialab-2.8.0/avclass/update.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.7.3/avclass_malicialab.egg-info/PKG-INFO` & `avclass-malicialab-2.8.0/avclass_malicialab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avclass-malicialab
-Version: 2.7.3
+Version: 2.8.0
 Summary: AVClass is a Python package and command line tool to tag / label malware samples.
 Author: MaliciaLab
 License: MIT License
         
         Copyright (c) 2016-2020 MaliciaLab @ IMDEA Software Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -470,13 +470,13 @@
 
 ## Contributors
 
 Several members of the MaliciaLab at the
 [IMDEA Software Institute](http://software.imdea.org)
 have contributed to AVClass:
 Marcos Sebastián, Richard Rivera, Platon Kotzias, Srdjan Matic,
-Silvia Sebastián, and Juan Caballero.
+Silvia Sebastián, Kevin van Liebergen, and Juan Caballero.
 
 GitHub users with significant contributions to AVClass include
 (let us know if you believe you should be listed here):
 [eljeffeg](https://github.com/eljeffeg)
```

### Comparing `avclass-malicialab-2.7.3/pyproject.toml` & `avclass-malicialab-2.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "avclass-malicialab"
-version = "2.7.3"
+version = "2.8.0"
 description = "AVClass is a Python package and command line tool to tag / label malware samples."
 readme = "README.md"
 authors = [{ name = "MaliciaLab" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```


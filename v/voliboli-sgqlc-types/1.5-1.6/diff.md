# Comparing `tmp/voliboli_sgqlc_types-1.5.tar.gz` & `tmp/voliboli_sgqlc_types-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voliboli_sgqlc_types-1.5.tar", last modified: Mon Apr 10 08:37:19 2023, max compression
+gzip compressed data, was "voliboli_sgqlc_types-1.6.tar", last modified: Mon Apr 10 08:56:15 2023, max compression
```

## Comparing `voliboli_sgqlc_types-1.5.tar` & `voliboli_sgqlc_types-1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 08:37:19.200287 voliboli_sgqlc_types-1.5/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      796 2023-04-10 08:37:19.200287 voliboli_sgqlc_types-1.5/PKG-INFO
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      433 2023-04-10 08:36:59.000000 voliboli_sgqlc_types-1.5/README.md
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      496 2023-04-10 08:37:19.200287 voliboli_sgqlc_types-1.5/setup.cfg
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      304 2023-04-10 08:35:40.000000 voliboli_sgqlc_types-1.5/setup.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 08:37:19.196287 voliboli_sgqlc_types-1.5/src/
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 08:37:19.200287 voliboli_sgqlc_types-1.5/src/voliboli_sgqlc_types.egg-info/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      796 2023-04-10 08:37:19.000000 voliboli_sgqlc_types-1.5/src/voliboli_sgqlc_types.egg-info/PKG-INFO
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      267 2023-04-10 08:37:19.000000 voliboli_sgqlc_types-1.5/src/voliboli_sgqlc_types.egg-info/SOURCES.txt
--rw-rw-r--   0 dorka     (1000) dorka     (1000)        1 2023-04-10 08:37:19.000000 voliboli_sgqlc_types-1.5/src/voliboli_sgqlc_types.egg-info/dependency_links.txt
--rw-rw-r--   0 dorka     (1000) dorka     (1000)        6 2023-04-10 08:37:19.000000 voliboli_sgqlc_types-1.5/src/voliboli_sgqlc_types.egg-info/requires.txt
--rw-rw-r--   0 dorka     (1000) dorka     (1000)        1 2023-04-10 08:37:19.000000 voliboli_sgqlc_types-1.5/src/voliboli_sgqlc_types.egg-info/top_level.txt
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 08:56:15.832749 voliboli_sgqlc_types-1.6/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      796 2023-04-10 08:56:15.832749 voliboli_sgqlc_types-1.6/PKG-INFO
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      433 2023-04-10 08:36:59.000000 voliboli_sgqlc_types-1.6/README.md
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      496 2023-04-10 08:56:15.832749 voliboli_sgqlc_types-1.6/setup.cfg
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      303 2023-04-10 08:56:09.000000 voliboli_sgqlc_types-1.6/setup.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 08:56:15.832749 voliboli_sgqlc_types-1.6/src/
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 08:56:15.832749 voliboli_sgqlc_types-1.6/src/voliboli_sgqlc_types.egg-info/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      796 2023-04-10 08:56:15.000000 voliboli_sgqlc_types-1.6/src/voliboli_sgqlc_types.egg-info/PKG-INFO
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      267 2023-04-10 08:56:15.000000 voliboli_sgqlc_types-1.6/src/voliboli_sgqlc_types.egg-info/SOURCES.txt
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)        1 2023-04-10 08:56:15.000000 voliboli_sgqlc_types-1.6/src/voliboli_sgqlc_types.egg-info/dependency_links.txt
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)        6 2023-04-10 08:56:15.000000 voliboli_sgqlc_types-1.6/src/voliboli_sgqlc_types.egg-info/requires.txt
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)        1 2023-04-10 08:56:15.000000 voliboli_sgqlc_types-1.6/src/voliboli_sgqlc_types.egg-info/top_level.txt
```

### Comparing `voliboli_sgqlc_types-1.5/PKG-INFO` & `voliboli_sgqlc_types-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voliboli_sgqlc_types
-Version: 1.5
+Version: 1.6
 Summary: Voliboli SGQLC Types
 Author: Teodor Janez Podobnik
 Author-email: teo.podobnik1234@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `voliboli_sgqlc_types-1.5/src/voliboli_sgqlc_types.egg-info/PKG-INFO` & `voliboli_sgqlc_types-1.6/src/voliboli_sgqlc_types.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voliboli-sgqlc-types
-Version: 1.5
+Version: 1.6
 Summary: Voliboli SGQLC Types
 Author: Teodor Janez Podobnik
 Author-email: teo.podobnik1234@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


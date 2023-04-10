# Comparing `tmp/voliboli_sgqlc_types-1.7.tar.gz` & `tmp/voliboli_sgqlc_types-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voliboli_sgqlc_types-1.7.tar", last modified: Mon Apr 10 09:00:54 2023, max compression
+gzip compressed data, was "voliboli_sgqlc_types-1.8.tar", last modified: Mon Apr 10 09:04:15 2023, max compression
```

## Comparing `voliboli_sgqlc_types-1.7.tar` & `voliboli_sgqlc_types-1.8.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 09:00:54.317947 voliboli_sgqlc_types-1.7/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      796 2023-04-10 09:00:54.317947 voliboli_sgqlc_types-1.7/PKG-INFO
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      433 2023-04-10 08:36:59.000000 voliboli_sgqlc_types-1.7/README.md
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      496 2023-04-10 09:00:54.317947 voliboli_sgqlc_types-1.7/setup.cfg
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      303 2023-04-10 09:00:50.000000 voliboli_sgqlc_types-1.7/setup.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 09:00:54.317947 voliboli_sgqlc_types-1.7/src/
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 09:00:54.317947 voliboli_sgqlc_types-1.7/src/voliboli_sgqlc_types.egg-info/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      796 2023-04-10 09:00:54.000000 voliboli_sgqlc_types-1.7/src/voliboli_sgqlc_types.egg-info/PKG-INFO
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      267 2023-04-10 09:00:54.000000 voliboli_sgqlc_types-1.7/src/voliboli_sgqlc_types.egg-info/SOURCES.txt
--rw-rw-r--   0 dorka     (1000) dorka     (1000)        1 2023-04-10 09:00:54.000000 voliboli_sgqlc_types-1.7/src/voliboli_sgqlc_types.egg-info/dependency_links.txt
--rw-rw-r--   0 dorka     (1000) dorka     (1000)        6 2023-04-10 09:00:54.000000 voliboli_sgqlc_types-1.7/src/voliboli_sgqlc_types.egg-info/requires.txt
--rw-rw-r--   0 dorka     (1000) dorka     (1000)        1 2023-04-10 09:00:54.000000 voliboli_sgqlc_types-1.7/src/voliboli_sgqlc_types.egg-info/top_level.txt
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 09:04:15.722710 voliboli_sgqlc_types-1.8/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      796 2023-04-10 09:04:15.722710 voliboli_sgqlc_types-1.8/PKG-INFO
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      433 2023-04-10 08:36:59.000000 voliboli_sgqlc_types-1.8/README.md
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      496 2023-04-10 09:04:15.722710 voliboli_sgqlc_types-1.8/setup.cfg
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      303 2023-04-10 09:04:11.000000 voliboli_sgqlc_types-1.8/setup.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 09:04:15.722710 voliboli_sgqlc_types-1.8/src/
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 09:04:15.722710 voliboli_sgqlc_types-1.8/src/voliboli_sgqlc_types/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)        0 2023-04-10 09:03:42.000000 voliboli_sgqlc_types-1.8/src/voliboli_sgqlc_types/__init__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2854 2023-04-10 08:33:20.000000 voliboli_sgqlc_types-1.8/src/voliboli_sgqlc_types/main.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 09:04:15.722710 voliboli_sgqlc_types-1.8/src/voliboli_sgqlc_types.egg-info/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      796 2023-04-10 09:04:15.000000 voliboli_sgqlc_types-1.8/src/voliboli_sgqlc_types.egg-info/PKG-INFO
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      337 2023-04-10 09:04:15.000000 voliboli_sgqlc_types-1.8/src/voliboli_sgqlc_types.egg-info/SOURCES.txt
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)        1 2023-04-10 09:04:15.000000 voliboli_sgqlc_types-1.8/src/voliboli_sgqlc_types.egg-info/dependency_links.txt
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)        6 2023-04-10 09:04:15.000000 voliboli_sgqlc_types-1.8/src/voliboli_sgqlc_types.egg-info/requires.txt
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)       21 2023-04-10 09:04:15.000000 voliboli_sgqlc_types-1.8/src/voliboli_sgqlc_types.egg-info/top_level.txt
```

### Comparing `voliboli_sgqlc_types-1.7/PKG-INFO` & `voliboli_sgqlc_types-1.8/src/voliboli_sgqlc_types.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: voliboli_sgqlc_types
-Version: 1.7
+Name: voliboli-sgqlc-types
+Version: 1.8
 Summary: Voliboli SGQLC Types
 Author: Teodor Janez Podobnik
 Author-email: teo.podobnik1234@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `voliboli_sgqlc_types-1.7/src/voliboli_sgqlc_types.egg-info/PKG-INFO` & `voliboli_sgqlc_types-1.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: voliboli-sgqlc-types
-Version: 1.7
+Name: voliboli_sgqlc_types
+Version: 1.8
 Summary: Voliboli SGQLC Types
 Author: Teodor Janez Podobnik
 Author-email: teo.podobnik1234@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


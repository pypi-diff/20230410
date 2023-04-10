# Comparing `tmp/doppkit-0.1.1.tar.gz` & `tmp/doppkit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doppkit-0.1.1.tar", last modified: Mon Apr 10 17:56:28 2023, max compression
+gzip compressed data, was "doppkit-0.1.2.tar", last modified: Mon Apr 10 18:11:18 2023, max compression
```

## Comparing `doppkit-0.1.1.tar` & `doppkit-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:56:28.982736 doppkit-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 17:56:14.000000 doppkit-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-04-10 17:56:28.982736 doppkit-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-10 17:56:14.000000 doppkit-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-10 17:56:14.000000 doppkit-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 17:56:28.982736 doppkit-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:56:28.978736 doppkit-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:56:28.978736 doppkit-0.1.1/src/doppkit/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 17:56:14.000000 doppkit-0.1.1/src/doppkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-10 17:56:14.000000 doppkit-0.1.1/src/doppkit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-10 17:56:14.000000 doppkit-0.1.1/src/doppkit/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-10 17:56:14.000000 doppkit-0.1.1/src/doppkit/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-10 17:56:14.000000 doppkit-0.1.1/src/doppkit/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-10 17:56:14.000000 doppkit-0.1.1/src/doppkit/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-10 17:56:14.000000 doppkit-0.1.1/src/doppkit/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:56:28.982736 doppkit-0.1.1/src/doppkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-04-10 17:56:28.000000 doppkit-0.1.1/src/doppkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-10 17:56:28.000000 doppkit-0.1.1/src/doppkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:56:28.000000 doppkit-0.1.1/src/doppkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-10 17:56:28.000000 doppkit-0.1.1/src/doppkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:56:28.000000 doppkit-0.1.1/src/doppkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-10 17:56:28.000000 doppkit-0.1.1/src/doppkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 17:56:28.000000 doppkit-0.1.1/src/doppkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:11:18.626577 doppkit-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 18:11:02.000000 doppkit-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-04-10 18:11:18.626577 doppkit-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-10 18:11:02.000000 doppkit-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-10 18:11:02.000000 doppkit-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:11:18.626577 doppkit-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:11:18.622577 doppkit-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:11:18.622577 doppkit-0.1.2/src/doppkit/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 18:11:02.000000 doppkit-0.1.2/src/doppkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-10 18:11:02.000000 doppkit-0.1.2/src/doppkit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-10 18:11:02.000000 doppkit-0.1.2/src/doppkit/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-10 18:11:02.000000 doppkit-0.1.2/src/doppkit/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-10 18:11:02.000000 doppkit-0.1.2/src/doppkit/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-10 18:11:02.000000 doppkit-0.1.2/src/doppkit/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-10 18:11:02.000000 doppkit-0.1.2/src/doppkit/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:11:18.626577 doppkit-0.1.2/src/doppkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-04-10 18:11:18.000000 doppkit-0.1.2/src/doppkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-10 18:11:18.000000 doppkit-0.1.2/src/doppkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:11:18.000000 doppkit-0.1.2/src/doppkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-10 18:11:18.000000 doppkit-0.1.2/src/doppkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:11:18.000000 doppkit-0.1.2/src/doppkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-10 18:11:18.000000 doppkit-0.1.2/src/doppkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 18:11:18.000000 doppkit-0.1.2/src/doppkit.egg-info/top_level.txt
```

### Comparing `doppkit-0.1.1/LICENSE` & `doppkit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.1/PKG-INFO` & `doppkit-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>, Howard Butler <howard@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `doppkit-0.1.1/pyproject.toml` & `doppkit-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.1/src/doppkit/app.py` & `doppkit-0.1.2/src/doppkit/app.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.1/src/doppkit/cache.py` & `doppkit-0.1.2/src/doppkit/cache.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.1/src/doppkit/grid.py` & `doppkit-0.1.2/src/doppkit/grid.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.1/src/doppkit/list.py` & `doppkit-0.1.2/src/doppkit/list.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.1/src/doppkit/sync.py` & `doppkit-0.1.2/src/doppkit/sync.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.1/src/doppkit.egg-info/PKG-INFO` & `doppkit-0.1.2/src/doppkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>, Howard Butler <howard@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```


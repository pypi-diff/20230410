# Comparing `tmp/doppkit-0.1.3.tar.gz` & `tmp/doppkit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doppkit-0.1.3.tar", last modified: Mon Apr 10 18:19:40 2023, max compression
+gzip compressed data, was "doppkit-0.1.4.tar", last modified: Mon Apr 10 18:28:19 2023, max compression
```

## Comparing `doppkit-0.1.3.tar` & `doppkit-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:40.655334 doppkit-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 18:19:25.000000 doppkit-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-04-10 18:19:40.655334 doppkit-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-10 18:19:25.000000 doppkit-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-10 18:19:25.000000 doppkit-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:19:40.655334 doppkit-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:40.651334 doppkit-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:40.651334 doppkit-0.1.3/src/doppkit/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 18:19:25.000000 doppkit-0.1.3/src/doppkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-10 18:19:25.000000 doppkit-0.1.3/src/doppkit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-10 18:19:25.000000 doppkit-0.1.3/src/doppkit/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-10 18:19:25.000000 doppkit-0.1.3/src/doppkit/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-10 18:19:25.000000 doppkit-0.1.3/src/doppkit/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-10 18:19:25.000000 doppkit-0.1.3/src/doppkit/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-10 18:19:25.000000 doppkit-0.1.3/src/doppkit/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:40.655334 doppkit-0.1.3/src/doppkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-04-10 18:19:40.000000 doppkit-0.1.3/src/doppkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-10 18:19:40.000000 doppkit-0.1.3/src/doppkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:19:40.000000 doppkit-0.1.3/src/doppkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-10 18:19:40.000000 doppkit-0.1.3/src/doppkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:19:40.000000 doppkit-0.1.3/src/doppkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-10 18:19:40.000000 doppkit-0.1.3/src/doppkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 18:19:40.000000 doppkit-0.1.3/src/doppkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:28:19.686774 doppkit-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 18:27:58.000000 doppkit-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-04-10 18:28:19.686774 doppkit-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-10 18:27:58.000000 doppkit-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-10 18:27:58.000000 doppkit-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:28:19.686774 doppkit-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:28:19.682774 doppkit-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:28:19.682774 doppkit-0.1.4/src/doppkit/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 18:27:58.000000 doppkit-0.1.4/src/doppkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-10 18:27:58.000000 doppkit-0.1.4/src/doppkit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-10 18:27:58.000000 doppkit-0.1.4/src/doppkit/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-10 18:27:58.000000 doppkit-0.1.4/src/doppkit/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-10 18:27:58.000000 doppkit-0.1.4/src/doppkit/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-10 18:27:58.000000 doppkit-0.1.4/src/doppkit/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-10 18:27:58.000000 doppkit-0.1.4/src/doppkit/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:28:19.682774 doppkit-0.1.4/src/doppkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-04-10 18:28:19.000000 doppkit-0.1.4/src/doppkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-10 18:28:19.000000 doppkit-0.1.4/src/doppkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:28:19.000000 doppkit-0.1.4/src/doppkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-10 18:28:19.000000 doppkit-0.1.4/src/doppkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:28:19.000000 doppkit-0.1.4/src/doppkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-10 18:28:19.000000 doppkit-0.1.4/src/doppkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 18:28:19.000000 doppkit-0.1.4/src/doppkit.egg-info/top_level.txt
```

### Comparing `doppkit-0.1.3/LICENSE` & `doppkit-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.3/PKG-INFO` & `doppkit-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>, Howard Butler <howard@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `doppkit-0.1.3/pyproject.toml` & `doppkit-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.3/src/doppkit/app.py` & `doppkit-0.1.4/src/doppkit/app.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.3/src/doppkit/cache.py` & `doppkit-0.1.4/src/doppkit/cache.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.3/src/doppkit/grid.py` & `doppkit-0.1.4/src/doppkit/grid.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.3/src/doppkit/list.py` & `doppkit-0.1.4/src/doppkit/list.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.3/src/doppkit/sync.py` & `doppkit-0.1.4/src/doppkit/sync.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.1.3/src/doppkit.egg-info/PKG-INFO` & `doppkit-0.1.4/src/doppkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>, Howard Butler <howard@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```


# Comparing `tmp/tarn-0.4.0.tar.gz` & `tmp/tarn-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarn-0.4.0.tar", last modified: Sat Apr  8 16:41:43 2023, max compression
+gzip compressed data, was "tarn-0.4.1.tar", last modified: Mon Apr 10 11:10:29 2023, max compression
```

## Comparing `tarn-0.4.0.tar` & `tarn-0.4.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-04-08 16:41:38.000000 tarn-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-08 16:41:38.000000 tarn-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-08 16:41:43.769901 tarn-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-08 16:41:38.000000 tarn-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-08 16:41:38.000000 tarn-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-08 16:41:38.000000 tarn-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 16:41:43.773902 tarn-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-08 16:41:38.000000 tarn-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/tarn/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/tarn/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/cache/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/cache/index.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/cache/pickler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/cache/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/cache/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/tarn/local/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/local/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/tarn/location/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/location/disk_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/location/fanout.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/location/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/location/levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/location/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/location/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/tarn/pickler/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/pickler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/pickler/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/pickler/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/tarn/pool/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/pool/hash_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/pool/pickle_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/tarn/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/remote/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/remote/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/tarn/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/tools/locker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/tools/size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/tools/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/tarn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-08 16:41:43.000000 tarn-0.4.0/tarn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-08 16:41:43.000000 tarn-0.4.0/tarn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 16:41:43.000000 tarn-0.4.0/tarn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-08 16:41:43.000000 tarn-0.4.0/tarn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-08 16:41:43.000000 tarn-0.4.0/tarn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:10:29.126998 tarn-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-04-10 11:10:24.000000 tarn-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-10 11:10:24.000000 tarn-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-10 11:10:29.126998 tarn-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-10 11:10:24.000000 tarn-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-10 11:10:24.000000 tarn-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-10 11:10:24.000000 tarn-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 11:10:29.126998 tarn-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-10 11:10:24.000000 tarn-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:10:29.122998 tarn-0.4.1/tarn/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:10:29.126998 tarn-0.4.1/tarn/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/cache/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/cache/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/cache/pickler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/cache/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/cache/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:10:29.126998 tarn-0.4.1/tarn/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/local/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:10:29.126998 tarn-0.4.1/tarn/location/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/location/disk_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/location/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/location/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/location/levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/location/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/location/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:10:29.126998 tarn-0.4.1/tarn/pickler/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/pickler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/pickler/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/pickler/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:10:29.126998 tarn-0.4.1/tarn/pool/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/pool/hash_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/pool/pickle_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:10:29.126998 tarn-0.4.1/tarn/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/remote/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/remote/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:10:29.126998 tarn-0.4.1/tarn/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/tools/locker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/tools/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/tools/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-10 11:10:24.000000 tarn-0.4.1/tarn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:10:29.122998 tarn-0.4.1/tarn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-10 11:10:29.000000 tarn-0.4.1/tarn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-10 11:10:29.000000 tarn-0.4.1/tarn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 11:10:29.000000 tarn-0.4.1/tarn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-10 11:10:29.000000 tarn-0.4.1/tarn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 11:10:29.000000 tarn-0.4.1/tarn.egg-info/top_level.txt
```

### Comparing `tarn-0.4.0/LICENSE` & `tarn-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/PKG-INFO` & `tarn-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.4.0
+Version: 0.4.1
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.4.0.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.4.1.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.4.0/README.md` & `tarn-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/pyproject.toml` & `tarn-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/setup.py` & `tarn-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/tarn/cache/storage.py` & `tarn-0.4.1/tarn/cache/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/tarn/compat.py` & `tarn-0.4.1/tarn/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/tarn/config.py` & `tarn-0.4.1/tarn/config.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/tarn/digest.py` & `tarn-0.4.1/tarn/digest.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/tarn/interface.py` & `tarn-0.4.1/tarn/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/tarn/local/storage.py` & `tarn-0.4.1/tarn/local/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/tarn/location/disk_dict.py` & `tarn-0.4.1/tarn/location/disk_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         self.levels = config.levels
         self.hash = config.hash.build()
         assert self.hash().digest_size == sum(self.levels)
 
         self.root = root
         self.permissions, self.group = root_params(self.root)
         usage_folder = self.root / 'tools/usage'
+        # FIXME: race condition
         create_folders(usage_folder, self.permissions, self.group)
 
         self.locker: Locker = config.make_locker()
         self.size_tracker: SizeTracker = config.make_size()
         self.usage_tracker: UsageTracker = config.make_usage(usage_folder)
         self.min_free_size = config.free_disk_size
         self.max_size = config.max_size
```

### Comparing `tarn-0.4.0/tarn/location/fanout.py` & `tarn-0.4.1/tarn/location/fanout.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/tarn/location/interface.py` & `tarn-0.4.1/tarn/location/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/tarn/location/levels.py` & `tarn-0.4.1/tarn/location/levels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/tarn/location/nginx.py` & `tarn-0.4.1/tarn/location/nginx.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/tarn/location/scp.py` & `tarn-0.4.1/tarn/location/scp.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/tarn/pickler/compat.py` & `tarn-0.4.1/tarn/pickler/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/tarn/pickler/interface.py` & `tarn-0.4.1/tarn/pickler/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/tarn/pool/hash_key.py` & `tarn-0.4.1/tarn/pool/hash_key.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/tarn/pool/pickle_key.py` & `tarn-0.4.1/tarn/pool/pickle_key.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/tarn/serializers.py` & `tarn-0.4.1/tarn/serializers.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/tarn/tools/locker.py` & `tarn-0.4.1/tarn/tools/locker.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/tarn/tools/size.py` & `tarn-0.4.1/tarn/tools/size.py`

 * *Files identical despite different names*

### Comparing `tarn-0.4.0/tarn/tools/usage.py` & `tarn-0.4.1/tarn/tools/usage.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from datetime import datetime
 from pathlib import Path
 from typing import Optional
 
 from ..compat import get_path_group, remove_file, set_path_attrs
 from ..digest import key_to_relative
 from ..interface import Key
+from ..utils import create_folders
 
 __all__ = 'UsageTracker', 'DummyUsage', 'StatUsage'
 
 
 class UsageTracker(ABC):
     def __init__(self, root: Path):
         self.root = root
@@ -38,25 +39,25 @@
         pass
 
 
 class StatUsage(UsageTracker):
     def update(self, key: Key, path: Path):
         mark = self._mark(key)
         missing = not mark.exists()
+        group = get_path_group(path)
+        create_folders(mark.parent, 0o777, group)
         mark.touch(exist_ok=True)
         if missing:
-            set_path_attrs(mark, 0o777, get_path_group(path))
+            set_path_attrs(mark, 0o777, group)
 
     def delete(self, key: Key):
         mark = self._mark(key)
         if mark.exists():
             remove_file(mark)
 
     def get(self, key: Key, path: Path) -> Optional[datetime]:
         mark = self._mark(key)
         if mark.exists():
             return datetime.fromtimestamp(mark.stat().st_mtime)
 
     def _mark(self, key):
-        mark = self.root / key_to_relative(key, (1, len(key) - 1))
-        mark.parent.mkdir(parents=True, exist_ok=True)
-        return mark
+        return self.root / key_to_relative(key, (1, len(key) - 1))
```

### Comparing `tarn-0.4.0/tarn/utils.py` & `tarn-0.4.1/tarn/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     path.mkdir(parents=parents, exist_ok=exist_ok)
     set_path_attrs(path, permissions, group)
 
 
 def create_folders(path: Path, permissions, group):
     if not path.exists():
         create_folders(path.parent, permissions, group)
-        mkdir(path, permissions, group)
+        mkdir(path, permissions, group, exist_ok=True)
 
 
 # TODO: need functions that return bool
 
 def match_files(first: Path, second: Path):
     if not filecmp.cmp(first, second, shallow=False):
         raise ValueError(f'Files do not match: {first} vs {second}')
```

### Comparing `tarn-0.4.0/tarn.egg-info/PKG-INFO` & `tarn-0.4.1/tarn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.4.0
+Version: 0.4.1
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.4.0.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.4.1.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.4.0/tarn.egg-info/SOURCES.txt` & `tarn-0.4.1/tarn.egg-info/SOURCES.txt`

 * *Files identical despite different names*


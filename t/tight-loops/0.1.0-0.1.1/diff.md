# Comparing `tmp/tight_loops-0.1.0.tar.gz` & `tmp/tight_loops-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tight_loops-0.1.0.tar", last modified: Thu Mar 30 15:02:29 2023, max compression
+gzip compressed data, was "tight_loops-0.1.1.tar", last modified: Mon Apr 10 17:47:00 2023, max compression
```

## Comparing `tight_loops-0.1.0.tar` & `tight_loops-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:02:29.513305 tight_loops-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-30 15:02:19.000000 tight_loops-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-30 15:02:19.000000 tight_loops-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-03-30 15:02:29.513305 tight_loops-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-30 15:02:19.000000 tight_loops-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-30 15:02:19.000000 tight_loops-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-30 15:02:29.513305 tight_loops-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-03-30 15:02:19.000000 tight_loops-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:02:29.509305 tight_loops-0.1.0/tight_loops/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-30 15:02:19.000000 tight_loops-0.1.0/tight_loops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-30 15:02:19.000000 tight_loops-0.1.0/tight_loops/tight_loops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:02:29.513305 tight_loops-0.1.0/tight_loops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-03-30 15:02:29.000000 tight_loops-0.1.0/tight_loops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-30 15:02:29.000000 tight_loops-0.1.0/tight_loops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-30 15:02:29.000000 tight_loops-0.1.0/tight_loops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 15:02:29.000000 tight_loops-0.1.0/tight_loops.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-30 15:02:29.000000 tight_loops-0.1.0/tight_loops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-30 15:02:29.000000 tight_loops-0.1.0/tight_loops.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:47:00.628458 tight_loops-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-10 17:46:50.000000 tight_loops-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-10 17:46:50.000000 tight_loops-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-10 17:47:00.628458 tight_loops-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-10 17:46:50.000000 tight_loops-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-10 17:46:50.000000 tight_loops-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-10 17:47:00.632458 tight_loops-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-10 17:46:50.000000 tight_loops-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:47:00.628458 tight_loops-0.1.1/tight_loops/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-10 17:46:50.000000 tight_loops-0.1.1/tight_loops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-10 17:46:50.000000 tight_loops-0.1.1/tight_loops/tight_loops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:47:00.628458 tight_loops-0.1.1/tight_loops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-10 17:47:00.000000 tight_loops-0.1.1/tight_loops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-10 17:47:00.000000 tight_loops-0.1.1/tight_loops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 17:47:00.000000 tight_loops-0.1.1/tight_loops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:47:00.000000 tight_loops-0.1.1/tight_loops.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 17:47:00.000000 tight_loops-0.1.1/tight_loops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 17:47:00.000000 tight_loops-0.1.1/tight_loops.egg-info/top_level.txt
```

### Comparing `tight_loops-0.1.0/LICENSE` & `tight_loops-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tight_loops-0.1.0/PKG-INFO` & `tight_loops-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tight_loops
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is a demo python package for UTK GEOG510
 Home-page: https://github.com/wnelso18/tight_loops
 Author: Will Nelson
 Author-email: wnelso18@vols.utk.edu
 License: MIT license
 Keywords: tight_loops
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `tight_loops-0.1.0/README.md` & `tight_loops-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tight_loops-0.1.0/setup.py` & `tight_loops-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='tight_loops',
     name='tight_loops',
     packages=find_packages(include=['tight_loops', 'tight_loops.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/wnelso18/tight_loops',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

### Comparing `tight_loops-0.1.0/tight_loops.egg-info/PKG-INFO` & `tight_loops-0.1.1/tight_loops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tight-loops
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is a demo python package for UTK GEOG510
 Home-page: https://github.com/wnelso18/tight_loops
 Author: Will Nelson
 Author-email: wnelso18@vols.utk.edu
 License: MIT license
 Keywords: tight_loops
 Classifier: Development Status :: 2 - Pre-Alpha
```


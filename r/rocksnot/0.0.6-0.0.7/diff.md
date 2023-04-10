# Comparing `tmp/rocksnot-0.0.6.tar.gz` & `tmp/rocksnot-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocksnot-0.0.6.tar", last modified: Thu Mar 23 14:54:42 2023, max compression
+gzip compressed data, was "rocksnot-0.0.7.tar", last modified: Mon Apr 10 17:48:24 2023, max compression
```

## Comparing `rocksnot-0.0.6.tar` & `rocksnot-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:54:42.146186 rocksnot-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-23 14:54:31.000000 rocksnot-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-23 14:54:31.000000 rocksnot-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-23 14:54:42.146186 rocksnot-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-23 14:54:31.000000 rocksnot-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:54:31.000000 rocksnot-0.0.6/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:54:42.146186 rocksnot-0.0.6/rocksnot/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-23 14:54:31.000000 rocksnot-0.0.6/rocksnot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-23 14:54:31.000000 rocksnot-0.0.6/rocksnot/rocksnot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:54:42.146186 rocksnot-0.0.6/rocksnot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-23 14:54:42.000000 rocksnot-0.0.6/rocksnot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-23 14:54:42.000000 rocksnot-0.0.6/rocksnot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 14:54:42.000000 rocksnot-0.0.6/rocksnot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 14:54:42.000000 rocksnot-0.0.6/rocksnot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-23 14:54:42.000000 rocksnot-0.0.6/rocksnot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-23 14:54:42.146186 rocksnot-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-23 14:54:31.000000 rocksnot-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:48:24.225576 rocksnot-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 17:48:16.000000 rocksnot-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-10 17:48:16.000000 rocksnot-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-10 17:48:24.229576 rocksnot-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-10 17:48:16.000000 rocksnot-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-10 17:48:16.000000 rocksnot-0.0.7/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:48:24.225576 rocksnot-0.0.7/rocksnot/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-10 17:48:16.000000 rocksnot-0.0.7/rocksnot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-04-10 17:48:16.000000 rocksnot-0.0.7/rocksnot/rocksnot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:48:24.225576 rocksnot-0.0.7/rocksnot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-10 17:48:24.000000 rocksnot-0.0.7/rocksnot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-10 17:48:24.000000 rocksnot-0.0.7/rocksnot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 17:48:24.000000 rocksnot-0.0.7/rocksnot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:48:24.000000 rocksnot-0.0.7/rocksnot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 17:48:24.000000 rocksnot-0.0.7/rocksnot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 17:48:24.000000 rocksnot-0.0.7/rocksnot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-10 17:48:24.229576 rocksnot-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-10 17:48:16.000000 rocksnot-0.0.7/setup.py
```

### Comparing `rocksnot-0.0.6/LICENSE` & `rocksnot-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rocksnot-0.0.6/PKG-INFO` & `rocksnot-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocksnot
-Version: 0.0.6
+Version: 0.0.7
 Summary: python package
 Home-page: https://github.com/rlape28/rocksnot
 Author: Robby Lape
 Author-email: robby.lape@gmail.com
 License: MIT license
 Keywords: rocksnot
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `rocksnot-0.0.6/README.md` & `rocksnot-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `rocksnot-0.0.6/rocksnot.egg-info/PKG-INFO` & `rocksnot-0.0.7/rocksnot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocksnot
-Version: 0.0.6
+Version: 0.0.7
 Summary: python package
 Home-page: https://github.com/rlape28/rocksnot
 Author: Robby Lape
 Author-email: robby.lape@gmail.com
 License: MIT license
 Keywords: rocksnot
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `rocksnot-0.0.6/setup.py` & `rocksnot-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='rocksnot',
     name='rocksnot',
     packages=find_packages(include=['rocksnot', 'rocksnot.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/rlape28/rocksnot',
-    version='0.0.6',
+    version='0.0.7',
     zip_safe=False,
 )
```


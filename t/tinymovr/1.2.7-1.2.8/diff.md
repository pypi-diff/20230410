# Comparing `tmp/tinymovr-1.2.7.tar.gz` & `tmp/tinymovr-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinymovr-1.2.7.tar", last modified: Mon Apr 10 19:05:14 2023, max compression
+gzip compressed data, was "tinymovr-1.2.8.tar", last modified: Mon Apr 10 19:15:29 2023, max compression
```

## Comparing `tinymovr-1.2.7.tar` & `tinymovr-1.2.8.tar`

### file list

```diff
@@ -1,31 +1,36 @@
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:05:14.320796 tinymovr-1.2.7/
--rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-10 19:05:14.320414 tinymovr-1.2.7/PKG-INFO
--rw-r--r--   0 yanconst   (501) staff       (20)     1689 2023-04-08 07:47:15.000000 tinymovr-1.2.7/README.md
--rw-r--r--   0 yanconst   (501) staff       (20)       38 2023-04-10 19:05:14.320946 tinymovr-1.2.7/setup.cfg
--rw-r--r--   0 yanconst   (501) staff       (20)     2369 2023-04-10 19:03:18.000000 tinymovr-1.2.7/setup.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:05:14.312111 tinymovr-1.2.7/tinymovr/
--rw-r--r--   0 yanconst   (501) staff       (20)       55 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3529 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/channel.py
--rw-r--r--   0 yanconst   (501) staff       (20)     2882 2023-04-10 19:03:18.000000 tinymovr-1.2.7/tinymovr/cli.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:05:14.316466 tinymovr-1.2.7/tinymovr/codec/
--rw-r--r--   0 yanconst   (501) staff       (20)       65 2022-02-09 17:27:03.000000 tinymovr-1.2.7/tinymovr/codec/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     2944 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/codec/codec.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:05:14.317284 tinymovr-1.2.7/tinymovr/config/
--rw-r--r--   0 yanconst   (501) staff       (20)      160 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/config/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3358 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/config/config.py
--rw-r--r--   0 yanconst   (501) staff       (20)     1075 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/constants.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3292 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/discovery.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:05:14.319799 tinymovr-1.2.7/tinymovr/gui/
--rw-r--r--   0 yanconst   (501) staff       (20)      411 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/gui/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     1718 2023-04-10 19:03:18.000000 tinymovr-1.2.7/tinymovr/gui/gui.py
--rw-r--r--   0 yanconst   (501) staff       (20)     8904 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/gui/helpers.py
--rw-r--r--   0 yanconst   (501) staff       (20)    12186 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/gui/window.py
--rw-r--r--   0 yanconst   (501) staff       (20)     4472 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/gui/worker.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3088 2023-04-08 07:47:15.000000 tinymovr-1.2.7/tinymovr/tee.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:05:14.315380 tinymovr-1.2.7/tinymovr.egg-info/
--rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-10 19:05:14.000000 tinymovr-1.2.7/tinymovr.egg-info/PKG-INFO
--rw-r--r--   0 yanconst   (501) staff       (20)      549 2023-04-10 19:05:14.000000 tinymovr-1.2.7/tinymovr.egg-info/SOURCES.txt
--rw-r--r--   0 yanconst   (501) staff       (20)        1 2023-04-10 19:05:14.000000 tinymovr-1.2.7/tinymovr.egg-info/dependency_links.txt
--rw-r--r--   0 yanconst   (501) staff       (20)       82 2023-04-10 19:05:14.000000 tinymovr-1.2.7/tinymovr.egg-info/entry_points.txt
--rw-r--r--   0 yanconst   (501) staff       (20)      158 2023-04-10 19:05:14.000000 tinymovr-1.2.7/tinymovr.egg-info/requires.txt
--rw-r--r--   0 yanconst   (501) staff       (20)        9 2023-04-10 19:05:14.000000 tinymovr-1.2.7/tinymovr.egg-info/top_level.txt
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:15:29.511173 tinymovr-1.2.8/
+-rw-r--r--   0 yanconst   (501) staff       (20)       87 2023-04-10 19:14:46.000000 tinymovr-1.2.8/MANIFEST.in
+-rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-10 19:15:29.510793 tinymovr-1.2.8/PKG-INFO
+-rw-r--r--   0 yanconst   (501) staff       (20)     1689 2023-04-08 07:47:15.000000 tinymovr-1.2.8/README.md
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:15:29.489743 tinymovr-1.2.8/resources/
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:15:29.494096 tinymovr-1.2.8/resources/icons/
+-rw-r--r--   0 yanconst   (501) staff       (20)     3184 2023-04-08 07:47:15.000000 tinymovr-1.2.8/resources/icons/call.png
+-rw-r--r--   0 yanconst   (501) staff       (20)       38 2023-04-10 19:15:29.511263 tinymovr-1.2.8/setup.cfg
+-rw-r--r--   0 yanconst   (501) staff       (20)     2326 2023-04-10 19:14:46.000000 tinymovr-1.2.8/setup.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:15:29.498489 tinymovr-1.2.8/tinymovr/
+-rw-r--r--   0 yanconst   (501) staff       (20)       55 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3529 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/channel.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     2882 2023-04-10 19:03:18.000000 tinymovr-1.2.8/tinymovr/cli.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:15:29.504777 tinymovr-1.2.8/tinymovr/codec/
+-rw-r--r--   0 yanconst   (501) staff       (20)       65 2022-02-09 17:27:03.000000 tinymovr-1.2.8/tinymovr/codec/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     2944 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/codec/codec.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:15:29.506866 tinymovr-1.2.8/tinymovr/config/
+-rw-r--r--   0 yanconst   (501) staff       (20)      160 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/config/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3358 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/config/config.py
+-rw-r--r--   0 yanconst   (501) staff       (20)    15484 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/config/device.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)     1075 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/constants.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3292 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/discovery.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:15:29.510094 tinymovr-1.2.8/tinymovr/gui/
+-rw-r--r--   0 yanconst   (501) staff       (20)      411 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/gui/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1718 2023-04-10 19:03:18.000000 tinymovr-1.2.8/tinymovr/gui/gui.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     8904 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/gui/helpers.py
+-rw-r--r--   0 yanconst   (501) staff       (20)    12186 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/gui/window.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     4472 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/gui/worker.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3088 2023-04-08 07:47:15.000000 tinymovr-1.2.8/tinymovr/tee.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-10 19:15:29.503719 tinymovr-1.2.8/tinymovr.egg-info/
+-rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-10 19:15:29.000000 tinymovr-1.2.8/tinymovr.egg-info/PKG-INFO
+-rw-r--r--   0 yanconst   (501) staff       (20)      614 2023-04-10 19:15:29.000000 tinymovr-1.2.8/tinymovr.egg-info/SOURCES.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)        1 2023-04-10 19:15:29.000000 tinymovr-1.2.8/tinymovr.egg-info/dependency_links.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)       82 2023-04-10 19:15:29.000000 tinymovr-1.2.8/tinymovr.egg-info/entry_points.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)      158 2023-04-10 19:15:29.000000 tinymovr-1.2.8/tinymovr.egg-info/requires.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)        9 2023-04-10 19:15:29.000000 tinymovr-1.2.8/tinymovr.egg-info/top_level.txt
```

### Comparing `tinymovr-1.2.7/PKG-INFO` & `tinymovr-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinymovr
-Version: 1.2.7
+Version: 1.2.8
 Summary: Tinymovr Studio
 Home-page: https://github.com/yconst/Tinymovr
 Author: Yannis Chatzikonstantinou
 Author-email: info@tinymovr.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `tinymovr-1.2.7/README.md` & `tinymovr-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.7/setup.py` & `tinymovr-1.2.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     author="Yannis Chatzikonstantinou",
     author_email="info@tinymovr.com",
     description="Tinymovr Studio",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/yconst/Tinymovr",
     packages=find_packages(include=["tinymovr", "tinymovr.*"]),
-    package_data={'tinymovr': ['*.yaml']},
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9",
```

### Comparing `tinymovr-1.2.7/tinymovr/channel.py` & `tinymovr-1.2.8/tinymovr/channel.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.7/tinymovr/cli.py` & `tinymovr-1.2.8/tinymovr/cli.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.7/tinymovr/codec/codec.py` & `tinymovr-1.2.8/tinymovr/codec/codec.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.7/tinymovr/config/config.py` & `tinymovr-1.2.8/tinymovr/config/config.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.7/tinymovr/constants.py` & `tinymovr-1.2.8/tinymovr/constants.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.7/tinymovr/discovery.py` & `tinymovr-1.2.8/tinymovr/discovery.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.7/tinymovr/gui/gui.py` & `tinymovr-1.2.8/tinymovr/gui/gui.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.7/tinymovr/gui/helpers.py` & `tinymovr-1.2.8/tinymovr/gui/helpers.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.7/tinymovr/gui/window.py` & `tinymovr-1.2.8/tinymovr/gui/window.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.7/tinymovr/gui/worker.py` & `tinymovr-1.2.8/tinymovr/gui/worker.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.7/tinymovr/tee.py` & `tinymovr-1.2.8/tinymovr/tee.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.2.7/tinymovr.egg-info/PKG-INFO` & `tinymovr-1.2.8/tinymovr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinymovr
-Version: 1.2.7
+Version: 1.2.8
 Summary: Tinymovr Studio
 Home-page: https://github.com/yconst/Tinymovr
 Author: Yannis Chatzikonstantinou
 Author-email: info@tinymovr.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `tinymovr-1.2.7/tinymovr.egg-info/SOURCES.txt` & `tinymovr-1.2.8/tinymovr.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+MANIFEST.in
 README.md
 setup.py
+resources/icons/call.png
 tinymovr/__init__.py
 tinymovr/channel.py
 tinymovr/cli.py
 tinymovr/constants.py
 tinymovr/discovery.py
 tinymovr/tee.py
 tinymovr.egg-info/PKG-INFO
@@ -12,12 +14,13 @@
 tinymovr.egg-info/entry_points.txt
 tinymovr.egg-info/requires.txt
 tinymovr.egg-info/top_level.txt
 tinymovr/codec/__init__.py
 tinymovr/codec/codec.py
 tinymovr/config/__init__.py
 tinymovr/config/config.py
+tinymovr/config/device.yaml
 tinymovr/gui/__init__.py
 tinymovr/gui/gui.py
 tinymovr/gui/helpers.py
 tinymovr/gui/window.py
 tinymovr/gui/worker.py
```


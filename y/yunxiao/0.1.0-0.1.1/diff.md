# Comparing `tmp/yunxiao-0.1.0.tar.gz` & `tmp/yunxiao-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.1.0.tar", last modified: Sun Apr  9 14:40:32 2023, max compression
+gzip compressed data, was "yunxiao-0.1.1.tar", last modified: Sun Apr  9 22:12:19 2023, max compression
```

## Comparing `yunxiao-0.1.0.tar` & `yunxiao-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 14:40:32.055618 yunxiao-0.1.0/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      940 2023-04-09 14:40:32.054616 yunxiao-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      451 2023-04-09 14:22:29.000000 yunxiao-0.1.0/README.md
--rw-rw-rw-   0        0        0      616 2023-04-09 14:40:18.000000 yunxiao-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-09 14:40:32.055618 yunxiao-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-09 14:40:32.033710 yunxiao-0.1.0/yunxiao/
--rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.1.0/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    18695 2023-04-09 13:02:30.000000 yunxiao-0.1.0/yunxiao/app.py
--rw-rw-rw-   0        0        0     5985 2023-04-09 13:04:42.000000 yunxiao-0.1.0/yunxiao/web.py
--rw-rw-rw-   0        0        0     6516 2023-04-08 20:37:39.000000 yunxiao-0.1.0/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-04-09 14:40:32.053616 yunxiao-0.1.0/yunxiao.egg-info/
--rw-rw-rw-   0        0        0      940 2023-04-09 14:40:32.000000 yunxiao-0.1.0/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-04-09 14:40:32.000000 yunxiao-0.1.0/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 14:40:32.000000 yunxiao-0.1.0/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-09 14:40:32.000000 yunxiao-0.1.0/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-09 14:40:32.000000 yunxiao-0.1.0/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 22:12:19.753275 yunxiao-0.1.1/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      940 2023-04-09 22:12:19.738166 yunxiao-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      451 2023-04-09 14:22:29.000000 yunxiao-0.1.1/README.md
+-rw-rw-rw-   0        0        0      587 2023-04-09 22:11:57.000000 yunxiao-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-09 22:12:19.753275 yunxiao-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-09 22:12:19.731159 yunxiao-0.1.1/yunxiao/
+-rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.1.1/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    18695 2023-04-09 13:02:30.000000 yunxiao-0.1.1/yunxiao/app.py
+-rw-rw-rw-   0        0        0     5985 2023-04-09 13:04:42.000000 yunxiao-0.1.1/yunxiao/web.py
+-rw-rw-rw-   0        0        0     6516 2023-04-08 20:37:39.000000 yunxiao-0.1.1/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-04-09 22:12:19.737165 yunxiao-0.1.1/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0      940 2023-04-09 22:12:19.000000 yunxiao-0.1.1/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-04-09 22:12:19.000000 yunxiao-0.1.1/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 22:12:19.000000 yunxiao-0.1.1/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-09 22:12:19.000000 yunxiao-0.1.1/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-09 22:12:19.000000 yunxiao-0.1.1/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.1.0/LICENSE` & `yunxiao-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.0/PKG-INFO` & `yunxiao-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.1.0
+Version: 0.1.1
 Summary: An API tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yunxiao-0.1.0/pyproject.toml` & `yunxiao-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.1.0"
+version = "0.1.1"
 description = "An API tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "requests",
-    "time",
-    "datetime",
-    "logging"
+    "datetime"
 ]
```

### Comparing `yunxiao-0.1.0/yunxiao/app.py` & `yunxiao-0.1.1/yunxiao/app.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.0/yunxiao/web.py` & `yunxiao-0.1.1/yunxiao/web.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.0/yunxiao/yunxiao.py` & `yunxiao-0.1.1/yunxiao/yunxiao.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.0/yunxiao.egg-info/PKG-INFO` & `yunxiao-0.1.1/yunxiao.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.1.0
+Version: 0.1.1
 Summary: An API tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```


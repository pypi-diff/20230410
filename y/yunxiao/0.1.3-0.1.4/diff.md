# Comparing `tmp/yunxiao-0.1.3.tar.gz` & `tmp/yunxiao-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.1.3.tar", last modified: Mon Apr 10 14:57:27 2023, max compression
+gzip compressed data, was "yunxiao-0.1.4.tar", last modified: Mon Apr 10 15:05:55 2023, max compression
```

## Comparing `yunxiao-0.1.3.tar` & `yunxiao-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 14:57:27.007994 yunxiao-0.1.3/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     7017 2023-04-10 14:57:27.007307 yunxiao-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6530 2023-04-10 01:07:24.000000 yunxiao-0.1.3/README.md
--rw-rw-rw-   0        0        0      587 2023-04-10 14:57:10.000000 yunxiao-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-10 14:57:27.007994 yunxiao-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-10 14:57:26.982764 yunxiao-0.1.3/yunxiao/
--rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.1.3/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    18394 2023-04-10 14:56:31.000000 yunxiao-0.1.3/yunxiao/app.py
--rw-rw-rw-   0        0        0     8911 2023-04-10 01:47:54.000000 yunxiao-0.1.3/yunxiao/web.py
--rw-rw-rw-   0        0        0     6516 2023-04-08 20:37:39.000000 yunxiao-0.1.3/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:57:27.005746 yunxiao-0.1.3/yunxiao.egg-info/
--rw-rw-rw-   0        0        0     7017 2023-04-10 14:57:26.000000 yunxiao-0.1.3/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-04-10 14:57:26.000000 yunxiao-0.1.3/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 14:57:26.000000 yunxiao-0.1.3/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-10 14:57:26.000000 yunxiao-0.1.3/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-10 14:57:26.000000 yunxiao-0.1.3/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 15:05:55.242483 yunxiao-0.1.4/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     7017 2023-04-10 15:05:55.240961 yunxiao-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6530 2023-04-10 01:07:24.000000 yunxiao-0.1.4/README.md
+-rw-rw-rw-   0        0        0      587 2023-04-10 15:05:39.000000 yunxiao-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-10 15:05:55.242483 yunxiao-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 15:05:55.233441 yunxiao-0.1.4/yunxiao/
+-rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.1.4/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    18394 2023-04-10 14:56:31.000000 yunxiao-0.1.4/yunxiao/app.py
+-rw-rw-rw-   0        0        0     8912 2023-04-10 15:04:42.000000 yunxiao-0.1.4/yunxiao/web.py
+-rw-rw-rw-   0        0        0     6516 2023-04-08 20:37:39.000000 yunxiao-0.1.4/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-04-10 15:05:55.238958 yunxiao-0.1.4/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0     7017 2023-04-10 15:05:55.000000 yunxiao-0.1.4/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-04-10 15:05:55.000000 yunxiao-0.1.4/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 15:05:55.000000 yunxiao-0.1.4/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-10 15:05:55.000000 yunxiao-0.1.4/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-10 15:05:55.000000 yunxiao-0.1.4/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.1.3/LICENSE` & `yunxiao-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.3/PKG-INFO` & `yunxiao-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.1.3
+Version: 0.1.4
 Summary: An API tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yunxiao-0.1.3/README.md` & `yunxiao-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.3/pyproject.toml` & `yunxiao-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.1.3"
+version = "0.1.4"
 description = "An API tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
```

### Comparing `yunxiao-0.1.3/yunxiao/app.py` & `yunxiao-0.1.4/yunxiao/app.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.3/yunxiao/web.py` & `yunxiao-0.1.4/yunxiao/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from yunxiao import WebOAuth, UsedTime
+from .yunxiao import WebOAuth, UsedTime
 
 
 class Web(WebOAuth):
     def __init__(self, userphone: str, password: str, campus: list =None):
         super().__init__(userphone, password)
         if campus is None:
             self.campus = []
```

### Comparing `yunxiao-0.1.3/yunxiao/yunxiao.py` & `yunxiao-0.1.4/yunxiao/yunxiao.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.3/yunxiao.egg-info/PKG-INFO` & `yunxiao-0.1.4/yunxiao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.1.3
+Version: 0.1.4
 Summary: An API tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```


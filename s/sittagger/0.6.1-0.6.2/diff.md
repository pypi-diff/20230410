# Comparing `tmp/sittagger-0.6.1.tar.gz` & `tmp/sittagger-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sittagger-0.6.1.tar", last modified: Sun Aug  7 18:20:40 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `sittagger-0.6.1.tar` & `sittagger-0.6.2.tar`

### file list

```diff
@@ -1,35 +1,25 @@
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2022-08-07 18:20:40.477259 sittagger-0.6.1/
--rw-r--r--   0 ntome     (1000) ntome     (1000)      484 2022-08-07 18:20:37.000000 sittagger-0.6.1/COPYING.WTFPL
--rw-r--r--   0 ntome     (1000) ntome     (1000)       23 2022-08-07 18:20:37.000000 sittagger-0.6.1/MANIFEST.in
--rw-r--r--   0 ntome     (1000) ntome     (1000)     2333 2022-08-07 18:20:40.477259 sittagger-0.6.1/PKG-INFO
--rw-r--r--   0 ntome     (1000) ntome     (1000)     1325 2022-08-07 18:20:37.000000 sittagger-0.6.1/README.rst
--rw-r--r--   0 ntome     (1000) ntome     (1000)     1332 2022-08-07 18:20:40.477259 sittagger-0.6.1/setup.cfg
--rwxr-xr-x   0 ntome     (1000) ntome     (1000)      165 2022-08-07 18:20:37.000000 sittagger-0.6.1/setup.py
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2022-08-07 18:20:40.477259 sittagger-0.6.1/sittagger/
--rw-r--r--   0 ntome     (1000) ntome     (1000)       56 2022-08-07 18:20:37.000000 sittagger-0.6.1/sittagger/__init__.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)       64 2022-08-07 18:20:37.000000 sittagger-0.6.1/sittagger/__main__.py
--rwxr-xr-x   0 ntome     (1000) ntome     (1000)     4769 2022-08-07 18:20:37.000000 sittagger-0.6.1/sittagger/app.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)     2955 2022-08-07 18:20:37.000000 sittagger-0.6.1/sittagger/canvas.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)     3967 2022-08-07 18:20:37.000000 sittagger-0.6.1/sittagger/cli.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)     4428 2022-08-07 18:20:37.000000 sittagger-0.6.1/sittagger/dbtag.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)     5304 2022-08-07 18:20:37.000000 sittagger-0.6.1/sittagger/dirwidgets.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)      890 2022-08-07 18:20:37.000000 sittagger-0.6.1/sittagger/fileoperationdialog.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)     1952 2022-08-07 18:20:37.000000 sittagger-0.6.1/sittagger/fm_interop.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)     5104 2022-08-07 18:20:37.000000 sittagger-0.6.1/sittagger/fsops.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)    10051 2022-08-07 18:20:37.000000 sittagger-0.6.1/sittagger/fullscreenviewer.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)    11804 2022-08-07 18:20:37.000000 sittagger-0.6.1/sittagger/imagewidgets.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)     7585 2022-08-07 18:20:37.000000 sittagger-0.6.1/sittagger/mainwindow.ui
--rw-r--r--   0 ntome     (1000) ntome     (1000)     5086 2022-08-07 18:20:37.000000 sittagger-0.6.1/sittagger/tagwidgets.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)     1406 2022-08-07 18:20:37.000000 sittagger-0.6.1/sittagger/thumbnailmaker.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)     2810 2022-08-07 18:20:37.000000 sittagger-0.6.1/sittagger/videogrid.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)     8647 2022-08-07 18:20:37.000000 sittagger-0.6.1/sittagger/videowidgets.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)      617 2022-08-07 18:20:37.000000 sittagger-0.6.1/sittagger.desktop
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2022-08-07 18:20:40.477259 sittagger-0.6.1/sittagger.egg-info/
--rw-r--r--   0 ntome     (1000) ntome     (1000)     2333 2022-08-07 18:20:40.000000 sittagger-0.6.1/sittagger.egg-info/PKG-INFO
--rw-r--r--   0 ntome     (1000) ntome     (1000)      713 2022-08-07 18:20:40.000000 sittagger-0.6.1/sittagger.egg-info/SOURCES.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)        1 2022-08-07 18:20:40.000000 sittagger-0.6.1/sittagger.egg-info/dependency_links.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)      101 2022-08-07 18:20:40.000000 sittagger-0.6.1/sittagger.egg-info/entry_points.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)       21 2022-08-07 18:20:40.000000 sittagger-0.6.1/sittagger.egg-info/requires.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)       10 2022-08-07 18:20:40.000000 sittagger-0.6.1/sittagger.egg-info/top_level.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)        1 2022-08-07 18:20:40.000000 sittagger-0.6.1/sittagger.egg-info/zip-safe
--rw-r--r--   0 ntome     (1000) ntome     (1000)     4853 2022-08-07 18:20:37.000000 sittagger-0.6.1/sittagger.png
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger.desktop
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger.png
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/__main__.py
+-rwxr-xr-x   0        0        0     4769 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/app.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/birdeye.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/canvas.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/cli.py
+-rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/dbtag.py
+-rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/dirwidgets.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/fileoperationdialog.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/fm_interop.py
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/fsops.py
+-rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/fullscreenviewer.py
+-rw-r--r--   0        0        0    11804 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/imagewidgets.py
+-rw-r--r--   0        0        0     7585 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/mainwindow.ui
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/tagwidgets.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/thumbnailmaker.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/videogrid.py
+-rw-r--r--   0        0        0     8647 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/videowidgets.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 sittagger-0.6.2/.gitignore
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 sittagger-0.6.2/COPYING.WTFPL
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 sittagger-0.6.2/README.rst
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 sittagger-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 sittagger-0.6.2/PKG-INFO
```

### Comparing `sittagger-0.6.1/PKG-INFO` & `sittagger-0.6.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 Metadata-Version: 2.1
 Name: sittagger
-Version: 0.6.1
+Version: 0.6.2
 Summary: Image viewer with user-labels tag database
-Home-page: https://github.com/hydrargyrum/sit-tagger
-Author: Hg
-Author-email: dev@indigo.re
-License: WTFPLv2
-Keywords: image,photo,viewer,browser,database,tagging,tag,label,labelling,python
+Project-URL: Homepage, https://indigo.re/sit-tagger/
+Project-URL: Project, https://github.com/hydrargyrum/sit-tagger
+Project-URL: PyPI, https://pypi.org/project/sittagger/
+Author-email: Hg <dev@indigo.re>
+License-Expression: WTFPL
+License-File: COPYING.WTFPL
+Keywords: browser,database,image,label,labelling,photo,python,tag,tagging,viewer
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: Public Domain
-Classifier: Topic :: Desktop Environment :: File Managers
-Classifier: Topic :: Multimedia :: Graphics :: Viewers
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Desktop Environment :: File Managers
+Classifier: Topic :: Multimedia :: Graphics :: Viewers
 Requires-Python: >=3.4
-License-File: COPYING.WTFPL
+Requires-Dist: pyqt5
+Requires-Dist: pyxdg
+Requires-Dist: vignette
+Description-Content-Type: text/x-rst
 
 SIT-Tagger
 ==========
 
 SIT-Tagger is an app for browsing tagged files.
 
 For now, it consists in an image browser app, that allows to set custom text tags
@@ -78,7 +86,13 @@
     % sit-tagger-cli list-files
     /tmp/some/file.jpg
 
 Remove all tags from a file::
 
     sit-tagger-cli untrack-files some/file.jpg
 
+Install
+-------
+
+Using ``pip install sittagger``.
+
+<https://pypi.org/project/sittagger/>
```

### Comparing `sittagger-0.6.1/README.rst` & `sittagger-0.6.2/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -53,7 +53,13 @@
     % sit-tagger-cli list-files
     /tmp/some/file.jpg
 
 Remove all tags from a file::
 
     sit-tagger-cli untrack-files some/file.jpg
 
+Install
+-------
+
+Using ``pip install sittagger``.
+
+<https://pypi.org/project/sittagger/>
```

### Comparing `sittagger-0.6.1/sittagger/app.py` & `sittagger-0.6.2/sittagger/app.py`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.1/sittagger/canvas.py` & `sittagger-0.6.2/sittagger/canvas.py`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.1/sittagger/cli.py` & `sittagger-0.6.2/sittagger/cli.py`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.1/sittagger/dbtag.py` & `sittagger-0.6.2/sittagger/dbtag.py`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.1/sittagger/dirwidgets.py` & `sittagger-0.6.2/sittagger/dirwidgets.py`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.1/sittagger/fileoperationdialog.py` & `sittagger-0.6.2/sittagger/fileoperationdialog.py`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.1/sittagger/fm_interop.py` & `sittagger-0.6.2/sittagger/fm_interop.py`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.1/sittagger/fsops.py` & `sittagger-0.6.2/sittagger/fsops.py`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.1/sittagger/fullscreenviewer.py` & `sittagger-0.6.2/sittagger/fullscreenviewer.py`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.1/sittagger/imagewidgets.py` & `sittagger-0.6.2/sittagger/imagewidgets.py`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.1/sittagger/mainwindow.ui` & `sittagger-0.6.2/sittagger/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.1/sittagger/tagwidgets.py` & `sittagger-0.6.2/sittagger/tagwidgets.py`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.1/sittagger/thumbnailmaker.py` & `sittagger-0.6.2/sittagger/thumbnailmaker.py`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.1/sittagger/videogrid.py` & `sittagger-0.6.2/sittagger/videogrid.py`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.1/sittagger/videowidgets.py` & `sittagger-0.6.2/sittagger/videowidgets.py`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.1/sittagger.desktop` & `sittagger-0.6.2/sittagger.desktop`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.1/sittagger.png` & `sittagger-0.6.2/sittagger.png`

 * *Files identical despite different names*


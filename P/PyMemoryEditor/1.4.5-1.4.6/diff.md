# Comparing `tmp/PyMemoryEditor-1.4.5.tar.gz` & `tmp/PyMemoryEditor-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMemoryEditor-1.4.5.tar", last modified: Mon Apr 10 00:47:52 2023, max compression
+gzip compressed data, was "PyMemoryEditor-1.4.6.tar", last modified: Mon Apr 10 00:56:32 2023, max compression
```

## Comparing `PyMemoryEditor-1.4.5.tar` & `PyMemoryEditor-1.4.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 00:47:52.754123 PyMemoryEditor-1.4.5/
--rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.4.5/LICENSE
--rw-rw-rw-   0        0        0     3857 2023-04-10 00:47:52.754123 PyMemoryEditor-1.4.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 00:47:52.722895 PyMemoryEditor-1.4.5/PyMemoryEditor/
--rw-rw-rw-   0        0        0      430 2023-04-10 00:47:26.000000 PyMemoryEditor-1.4.5/PyMemoryEditor/__init__.py
--rw-rw-rw-   0        0        0     5049 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.5/PyMemoryEditor/open_process.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:47:52.754123 PyMemoryEditor-1.4.5/PyMemoryEditor/process/
--rw-rw-rw-   0        0        0     1676 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.5/PyMemoryEditor/process/__init__.py
--rw-rw-rw-   0        0        0      717 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.5/PyMemoryEditor/process/errors.py
--rw-rw-rw-   0        0        0      746 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.5/PyMemoryEditor/process/util.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:47:52.754123 PyMemoryEditor-1.4.5/PyMemoryEditor/win32/
--rw-rw-rw-   0        0        0     7619 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.5/PyMemoryEditor/win32/functions.py
--rw-rw-rw-   0        0        0     1791 2023-04-09 16:56:11.000000 PyMemoryEditor-1.4.5/PyMemoryEditor/win32/types.py
--rw-rw-rw-   0        0        0      928 2023-04-09 16:07:32.000000 PyMemoryEditor-1.4.5/PyMemoryEditor/win32/util.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:47:52.754123 PyMemoryEditor-1.4.5/PyMemoryEditor.egg-info/
--rw-rw-rw-   0        0        0     3857 2023-04-10 00:47:52.000000 PyMemoryEditor-1.4.5/PyMemoryEditor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2023-04-10 00:47:52.000000 PyMemoryEditor-1.4.5/PyMemoryEditor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 00:47:52.000000 PyMemoryEditor-1.4.5/PyMemoryEditor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-10 00:47:52.000000 PyMemoryEditor-1.4.5/PyMemoryEditor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-10 00:47:52.000000 PyMemoryEditor-1.4.5/PyMemoryEditor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2640 2023-04-09 22:47:34.000000 PyMemoryEditor-1.4.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-10 00:47:52.754123 PyMemoryEditor-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1602 2023-04-10 00:47:46.000000 PyMemoryEditor-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:56:32.460086 PyMemoryEditor-1.4.6/
+-rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.4.6/LICENSE
+-rw-rw-rw-   0        0        0     3909 2023-04-10 00:56:32.459476 PyMemoryEditor-1.4.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 00:56:32.439775 PyMemoryEditor-1.4.6/PyMemoryEditor/
+-rw-rw-rw-   0        0        0      430 2023-04-10 00:56:03.000000 PyMemoryEditor-1.4.6/PyMemoryEditor/__init__.py
+-rw-rw-rw-   0        0        0     5049 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.6/PyMemoryEditor/open_process.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:56:32.450697 PyMemoryEditor-1.4.6/PyMemoryEditor/process/
+-rw-rw-rw-   0        0        0     1676 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.6/PyMemoryEditor/process/__init__.py
+-rw-rw-rw-   0        0        0      717 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.6/PyMemoryEditor/process/errors.py
+-rw-rw-rw-   0        0        0      746 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.6/PyMemoryEditor/process/util.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:56:32.457816 PyMemoryEditor-1.4.6/PyMemoryEditor/win32/
+-rw-rw-rw-   0        0        0     7619 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.6/PyMemoryEditor/win32/functions.py
+-rw-rw-rw-   0        0        0     1791 2023-04-09 16:56:11.000000 PyMemoryEditor-1.4.6/PyMemoryEditor/win32/types.py
+-rw-rw-rw-   0        0        0      928 2023-04-09 16:07:32.000000 PyMemoryEditor-1.4.6/PyMemoryEditor/win32/util.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:56:32.450697 PyMemoryEditor-1.4.6/PyMemoryEditor.egg-info/
+-rw-rw-rw-   0        0        0     3909 2023-04-10 00:56:32.000000 PyMemoryEditor-1.4.6/PyMemoryEditor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-04-10 00:56:32.000000 PyMemoryEditor-1.4.6/PyMemoryEditor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 00:56:32.000000 PyMemoryEditor-1.4.6/PyMemoryEditor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-10 00:56:32.000000 PyMemoryEditor-1.4.6/PyMemoryEditor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-10 00:56:32.000000 PyMemoryEditor-1.4.6/PyMemoryEditor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2640 2023-04-09 22:47:34.000000 PyMemoryEditor-1.4.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 00:56:32.460086 PyMemoryEditor-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1654 2023-04-10 00:55:41.000000 PyMemoryEditor-1.4.6/setup.py
```

### Comparing `PyMemoryEditor-1.4.5/LICENSE` & `PyMemoryEditor-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.5/PKG-INFO` & `PyMemoryEditor-1.4.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.4.5
-Summary: Process memory reader and writer.
+Version: 1.4.6
+Summary: A Python library to edit and track memory of Windows processes (32 bits and 64 bits).
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: memory virtual writer reader read write override address pointer edit editor process win32 api cheat scan scanner debug trainer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `PyMemoryEditor-1.4.5/PyMemoryEditor/open_process.py` & `PyMemoryEditor-1.4.6/PyMemoryEditor/open_process.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.5/PyMemoryEditor/process/__init__.py` & `PyMemoryEditor-1.4.6/PyMemoryEditor/process/__init__.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.5/PyMemoryEditor/process/errors.py` & `PyMemoryEditor-1.4.6/PyMemoryEditor/process/errors.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.5/PyMemoryEditor/process/util.py` & `PyMemoryEditor-1.4.6/PyMemoryEditor/process/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.5/PyMemoryEditor/win32/functions.py` & `PyMemoryEditor-1.4.6/PyMemoryEditor/win32/functions.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.5/PyMemoryEditor/win32/types.py` & `PyMemoryEditor-1.4.6/PyMemoryEditor/win32/types.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.5/PyMemoryEditor/win32/util.py` & `PyMemoryEditor-1.4.6/PyMemoryEditor/win32/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.5/PyMemoryEditor.egg-info/PKG-INFO` & `PyMemoryEditor-1.4.6/PyMemoryEditor.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.4.5
-Summary: Process memory reader and writer.
+Version: 1.4.6
+Summary: A Python library to edit and track memory of Windows processes (32 bits and 64 bits).
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: memory virtual writer reader read write override address pointer edit editor process win32 api cheat scan scanner debug trainer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `PyMemoryEditor-1.4.5/README.md` & `PyMemoryEditor-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.5/setup.py` & `PyMemoryEditor-1.4.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("README.md") as file:
     README = file.read()
 
 setup(
     name = "PyMemoryEditor",
     version = __version__,
-    description = "Process memory reader and writer.",
+    description = "A Python library to edit and track memory of Windows processes (32 bits and 64 bits).",
     long_description = README,
     long_description_content_type = "text/markdown",
     author = "Jean Loui Bernard Silva de Jesus",
     url = "https://github.com/JeanExtreme002/PyMemoryEditor",
     license = "MIT",
     keywords = "memory virtual writer reader read write override address pointer edit editor process win32 api cheat scan scanner debug trainer",
     packages = ["PyMemoryEditor", "PyMemoryEditor.process", "PyMemoryEditor.win32"],
```


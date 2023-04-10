# Comparing `tmp/PyMemoryEditor-1.4.6.tar.gz` & `tmp/PyMemoryEditor-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMemoryEditor-1.4.6.tar", last modified: Mon Apr 10 00:56:32 2023, max compression
+gzip compressed data, was "PyMemoryEditor-1.4.7.tar", last modified: Mon Apr 10 01:36:22 2023, max compression
```

## Comparing `PyMemoryEditor-1.4.6.tar` & `PyMemoryEditor-1.4.7.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 00:56:32.460086 PyMemoryEditor-1.4.6/
--rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.4.6/LICENSE
--rw-rw-rw-   0        0        0     3909 2023-04-10 00:56:32.459476 PyMemoryEditor-1.4.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 00:56:32.439775 PyMemoryEditor-1.4.6/PyMemoryEditor/
--rw-rw-rw-   0        0        0      430 2023-04-10 00:56:03.000000 PyMemoryEditor-1.4.6/PyMemoryEditor/__init__.py
--rw-rw-rw-   0        0        0     5049 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.6/PyMemoryEditor/open_process.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:56:32.450697 PyMemoryEditor-1.4.6/PyMemoryEditor/process/
--rw-rw-rw-   0        0        0     1676 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.6/PyMemoryEditor/process/__init__.py
--rw-rw-rw-   0        0        0      717 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.6/PyMemoryEditor/process/errors.py
--rw-rw-rw-   0        0        0      746 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.6/PyMemoryEditor/process/util.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:56:32.457816 PyMemoryEditor-1.4.6/PyMemoryEditor/win32/
--rw-rw-rw-   0        0        0     7619 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.6/PyMemoryEditor/win32/functions.py
--rw-rw-rw-   0        0        0     1791 2023-04-09 16:56:11.000000 PyMemoryEditor-1.4.6/PyMemoryEditor/win32/types.py
--rw-rw-rw-   0        0        0      928 2023-04-09 16:07:32.000000 PyMemoryEditor-1.4.6/PyMemoryEditor/win32/util.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:56:32.450697 PyMemoryEditor-1.4.6/PyMemoryEditor.egg-info/
--rw-rw-rw-   0        0        0     3909 2023-04-10 00:56:32.000000 PyMemoryEditor-1.4.6/PyMemoryEditor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2023-04-10 00:56:32.000000 PyMemoryEditor-1.4.6/PyMemoryEditor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 00:56:32.000000 PyMemoryEditor-1.4.6/PyMemoryEditor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-10 00:56:32.000000 PyMemoryEditor-1.4.6/PyMemoryEditor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-10 00:56:32.000000 PyMemoryEditor-1.4.6/PyMemoryEditor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2640 2023-04-09 22:47:34.000000 PyMemoryEditor-1.4.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-10 00:56:32.460086 PyMemoryEditor-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1654 2023-04-10 00:55:41.000000 PyMemoryEditor-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:36:22.342990 PyMemoryEditor-1.4.7/
+-rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.4.7/LICENSE
+-rw-rw-rw-   0        0        0     3909 2023-04-10 01:36:22.342990 PyMemoryEditor-1.4.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 01:36:22.327367 PyMemoryEditor-1.4.7/PyMemoryEditor/
+-rw-rw-rw-   0        0        0      430 2023-04-10 01:35:55.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/__init__.py
+-rw-rw-rw-   0        0        0     5049 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/open_process.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:36:22.342990 PyMemoryEditor-1.4.7/PyMemoryEditor/process/
+-rw-rw-rw-   0        0        0     1676 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/process/__init__.py
+-rw-rw-rw-   0        0        0      717 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/process/errors.py
+-rw-rw-rw-   0        0        0      746 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/process/util.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:36:22.342990 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/
+drwxrwxrwx   0        0        0        0 2023-04-10 01:36:22.342990 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/enums/
+-rw-rw-rw-   0        0        0      281 2023-04-09 23:43:15.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/enums/__init__.py
+-rw-rw-rw-   0        0        0     2449 2023-04-09 23:42:16.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/enums/memory_allocation_states.py
+-rw-rw-rw-   0        0        0     6600 2023-04-09 23:42:16.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/enums/memory_protections.py
+-rw-rw-rw-   0        0        0      537 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/enums/memory_types.py
+-rw-rw-rw-   0        0        0     2681 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/enums/process_operations.py
+-rw-rw-rw-   0        0        0      977 2023-04-09 23:41:45.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/enums/standard_access_rights.py
+-rw-rw-rw-   0        0        0     7619 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/functions.py
+-rw-rw-rw-   0        0        0     1791 2023-04-09 16:56:11.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/types.py
+-rw-rw-rw-   0        0        0      928 2023-04-09 16:07:32.000000 PyMemoryEditor-1.4.7/PyMemoryEditor/win32/util.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:36:22.342990 PyMemoryEditor-1.4.7/PyMemoryEditor.egg-info/
+-rw-rw-rw-   0        0        0     3909 2023-04-10 01:36:22.000000 PyMemoryEditor-1.4.7/PyMemoryEditor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      753 2023-04-10 01:36:22.000000 PyMemoryEditor-1.4.7/PyMemoryEditor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 01:36:22.000000 PyMemoryEditor-1.4.7/PyMemoryEditor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-10 01:36:22.000000 PyMemoryEditor-1.4.7/PyMemoryEditor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-10 01:36:22.000000 PyMemoryEditor-1.4.7/PyMemoryEditor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2640 2023-04-09 22:47:34.000000 PyMemoryEditor-1.4.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 01:36:22.342990 PyMemoryEditor-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1727 2023-04-10 01:35:30.000000 PyMemoryEditor-1.4.7/setup.py
```

### Comparing `PyMemoryEditor-1.4.6/LICENSE` & `PyMemoryEditor-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.6/PKG-INFO` & `PyMemoryEditor-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.4.6
+Version: 1.4.7
 Summary: A Python library to edit and track memory of Windows processes (32 bits and 64 bits).
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: memory virtual writer reader read write override address pointer edit editor process win32 api cheat scan scanner debug trainer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `PyMemoryEditor-1.4.6/PyMemoryEditor/open_process.py` & `PyMemoryEditor-1.4.7/PyMemoryEditor/open_process.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.6/PyMemoryEditor/process/__init__.py` & `PyMemoryEditor-1.4.7/PyMemoryEditor/process/__init__.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.6/PyMemoryEditor/process/errors.py` & `PyMemoryEditor-1.4.7/PyMemoryEditor/process/errors.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.6/PyMemoryEditor/process/util.py` & `PyMemoryEditor-1.4.7/PyMemoryEditor/process/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.6/PyMemoryEditor/win32/functions.py` & `PyMemoryEditor-1.4.7/PyMemoryEditor/win32/functions.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.6/PyMemoryEditor/win32/types.py` & `PyMemoryEditor-1.4.7/PyMemoryEditor/win32/types.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.6/PyMemoryEditor/win32/util.py` & `PyMemoryEditor-1.4.7/PyMemoryEditor/win32/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.6/PyMemoryEditor.egg-info/PKG-INFO` & `PyMemoryEditor-1.4.7/PyMemoryEditor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.4.6
+Version: 1.4.7
 Summary: A Python library to edit and track memory of Windows processes (32 bits and 64 bits).
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: memory virtual writer reader read write override address pointer edit editor process win32 api cheat scan scanner debug trainer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `PyMemoryEditor-1.4.6/README.md` & `PyMemoryEditor-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.6/setup.py` & `PyMemoryEditor-1.4.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,20 @@
     description = "A Python library to edit and track memory of Windows processes (32 bits and 64 bits).",
     long_description = README,
     long_description_content_type = "text/markdown",
     author = "Jean Loui Bernard Silva de Jesus",
     url = "https://github.com/JeanExtreme002/PyMemoryEditor",
     license = "MIT",
     keywords = "memory virtual writer reader read write override address pointer edit editor process win32 api cheat scan scanner debug trainer",
-    packages = ["PyMemoryEditor", "PyMemoryEditor.process", "PyMemoryEditor.win32"],
+    packages = [
+        "PyMemoryEditor",
+        "PyMemoryEditor.process",
+        "PyMemoryEditor.win32",
+        "PyMemoryEditor.win32.enums"
+    ],
     install_requires = ["pywin32", "psutil"],
     classifiers = [
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
         "Environment :: Win32 (MS Windows)",
```


# Comparing `tmp/PyMemoryEditor-1.4.4.tar.gz` & `tmp/PyMemoryEditor-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMemoryEditor-1.4.4.tar", last modified: Mon Apr 10 00:03:51 2023, max compression
+gzip compressed data, was "PyMemoryEditor-1.4.5.tar", last modified: Mon Apr 10 00:47:52 2023, max compression
```

## Comparing `PyMemoryEditor-1.4.4.tar` & `PyMemoryEditor-1.4.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 00:03:51.235187 PyMemoryEditor-1.4.4/
--rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.4.4/LICENSE
--rw-rw-rw-   0        0        0     3591 2023-04-10 00:03:51.235187 PyMemoryEditor-1.4.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 00:03:51.217617 PyMemoryEditor-1.4.4/PyMemoryEditor/
--rw-rw-rw-   0        0        0      430 2023-04-09 23:45:50.000000 PyMemoryEditor-1.4.4/PyMemoryEditor/__init__.py
--rw-rw-rw-   0        0        0     5049 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.4/PyMemoryEditor/open_process.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:03:51.232686 PyMemoryEditor-1.4.4/PyMemoryEditor/process/
--rw-rw-rw-   0        0        0     1676 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.4/PyMemoryEditor/process/__init__.py
--rw-rw-rw-   0        0        0      717 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.4/PyMemoryEditor/process/errors.py
--rw-rw-rw-   0        0        0      746 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.4/PyMemoryEditor/process/util.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:03:51.233683 PyMemoryEditor-1.4.4/PyMemoryEditor/win32/
--rw-rw-rw-   0        0        0     7619 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.4/PyMemoryEditor/win32/functions.py
--rw-rw-rw-   0        0        0     1791 2023-04-09 16:56:11.000000 PyMemoryEditor-1.4.4/PyMemoryEditor/win32/types.py
--rw-rw-rw-   0        0        0      928 2023-04-09 16:07:32.000000 PyMemoryEditor-1.4.4/PyMemoryEditor/win32/util.py
-drwxrwxrwx   0        0        0        0 2023-04-10 00:03:51.230684 PyMemoryEditor-1.4.4/PyMemoryEditor.egg-info/
--rw-rw-rw-   0        0        0     3591 2023-04-10 00:03:51.000000 PyMemoryEditor-1.4.4/PyMemoryEditor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2023-04-10 00:03:51.000000 PyMemoryEditor-1.4.4/PyMemoryEditor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 00:03:51.000000 PyMemoryEditor-1.4.4/PyMemoryEditor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-10 00:03:51.000000 PyMemoryEditor-1.4.4/PyMemoryEditor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-10 00:03:51.000000 PyMemoryEditor-1.4.4/PyMemoryEditor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2640 2023-04-09 22:47:34.000000 PyMemoryEditor-1.4.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-10 00:03:51.235705 PyMemoryEditor-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1341 2023-04-03 13:26:23.000000 PyMemoryEditor-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:47:52.754123 PyMemoryEditor-1.4.5/
+-rw-rw-rw-   0        0        0     1110 2023-04-03 04:22:57.000000 PyMemoryEditor-1.4.5/LICENSE
+-rw-rw-rw-   0        0        0     3857 2023-04-10 00:47:52.754123 PyMemoryEditor-1.4.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 00:47:52.722895 PyMemoryEditor-1.4.5/PyMemoryEditor/
+-rw-rw-rw-   0        0        0      430 2023-04-10 00:47:26.000000 PyMemoryEditor-1.4.5/PyMemoryEditor/__init__.py
+-rw-rw-rw-   0        0        0     5049 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.5/PyMemoryEditor/open_process.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:47:52.754123 PyMemoryEditor-1.4.5/PyMemoryEditor/process/
+-rw-rw-rw-   0        0        0     1676 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.5/PyMemoryEditor/process/__init__.py
+-rw-rw-rw-   0        0        0      717 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.5/PyMemoryEditor/process/errors.py
+-rw-rw-rw-   0        0        0      746 2023-04-09 03:16:07.000000 PyMemoryEditor-1.4.5/PyMemoryEditor/process/util.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:47:52.754123 PyMemoryEditor-1.4.5/PyMemoryEditor/win32/
+-rw-rw-rw-   0        0        0     7619 2023-04-09 23:42:46.000000 PyMemoryEditor-1.4.5/PyMemoryEditor/win32/functions.py
+-rw-rw-rw-   0        0        0     1791 2023-04-09 16:56:11.000000 PyMemoryEditor-1.4.5/PyMemoryEditor/win32/types.py
+-rw-rw-rw-   0        0        0      928 2023-04-09 16:07:32.000000 PyMemoryEditor-1.4.5/PyMemoryEditor/win32/util.py
+drwxrwxrwx   0        0        0        0 2023-04-10 00:47:52.754123 PyMemoryEditor-1.4.5/PyMemoryEditor.egg-info/
+-rw-rw-rw-   0        0        0     3857 2023-04-10 00:47:52.000000 PyMemoryEditor-1.4.5/PyMemoryEditor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-04-10 00:47:52.000000 PyMemoryEditor-1.4.5/PyMemoryEditor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 00:47:52.000000 PyMemoryEditor-1.4.5/PyMemoryEditor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-10 00:47:52.000000 PyMemoryEditor-1.4.5/PyMemoryEditor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-10 00:47:52.000000 PyMemoryEditor-1.4.5/PyMemoryEditor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2640 2023-04-09 22:47:34.000000 PyMemoryEditor-1.4.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 00:47:52.754123 PyMemoryEditor-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1602 2023-04-10 00:47:46.000000 PyMemoryEditor-1.4.5/setup.py
```

### Comparing `PyMemoryEditor-1.4.4/LICENSE` & `PyMemoryEditor-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.4/PKG-INFO` & `PyMemoryEditor-1.4.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.4.4
+Version: 1.4.5
 Summary: Process memory reader and writer.
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
-Keywords: memory writer write reader read override address pointer peditor process win32 api cheat
+Keywords: memory virtual writer reader read write override address pointer edit editor process win32 api cheat scan scanner debug trainer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Security
+Classifier: Topic :: System :: Monitoring
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyMemoryEditor
 
 A Python library developed with [ctypes](https://docs.python.org/3/library/ctypes.html) to manipulate Windows processes (32 bits and 64 bits), <br>
 reading and writing values in the process memory.
```

### Comparing `PyMemoryEditor-1.4.4/PyMemoryEditor/open_process.py` & `PyMemoryEditor-1.4.5/PyMemoryEditor/open_process.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.4/PyMemoryEditor/process/__init__.py` & `PyMemoryEditor-1.4.5/PyMemoryEditor/process/__init__.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.4/PyMemoryEditor/process/errors.py` & `PyMemoryEditor-1.4.5/PyMemoryEditor/process/errors.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.4/PyMemoryEditor/process/util.py` & `PyMemoryEditor-1.4.5/PyMemoryEditor/process/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.4/PyMemoryEditor/win32/functions.py` & `PyMemoryEditor-1.4.5/PyMemoryEditor/win32/functions.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.4/PyMemoryEditor/win32/types.py` & `PyMemoryEditor-1.4.5/PyMemoryEditor/win32/types.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.4/PyMemoryEditor/win32/util.py` & `PyMemoryEditor-1.4.5/PyMemoryEditor/win32/util.py`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.4/PyMemoryEditor.egg-info/PKG-INFO` & `PyMemoryEditor-1.4.5/PyMemoryEditor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.4.4
+Version: 1.4.5
 Summary: Process memory reader and writer.
 Home-page: https://github.com/JeanExtreme002/PyMemoryEditor
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
-Keywords: memory writer write reader read override address pointer peditor process win32 api cheat
+Keywords: memory virtual writer reader read write override address pointer edit editor process win32 api cheat scan scanner debug trainer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Security
+Classifier: Topic :: System :: Monitoring
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyMemoryEditor
 
 A Python library developed with [ctypes](https://docs.python.org/3/library/ctypes.html) to manipulate Windows processes (32 bits and 64 bits), <br>
 reading and writing values in the process memory.
```

### Comparing `PyMemoryEditor-1.4.4/README.md` & `PyMemoryEditor-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `PyMemoryEditor-1.4.4/setup.py` & `PyMemoryEditor-1.4.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,24 +11,29 @@
     version = __version__,
     description = "Process memory reader and writer.",
     long_description = README,
     long_description_content_type = "text/markdown",
     author = "Jean Loui Bernard Silva de Jesus",
     url = "https://github.com/JeanExtreme002/PyMemoryEditor",
     license = "MIT",
-    keywords = "memory writer write reader read override address pointer peditor process win32 api cheat",
+    keywords = "memory virtual writer reader read write override address pointer edit editor process win32 api cheat scan scanner debug trainer",
     packages = ["PyMemoryEditor", "PyMemoryEditor.process", "PyMemoryEditor.win32"],
     install_requires = ["pywin32", "psutil"],
     classifiers = [
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
+        "Intended Audience :: Information Technology",
+        "Intended Audience :: Science/Research",
         "Environment :: Win32 (MS Windows)",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11"
+        "Programming Language :: Python :: 3.11",
+        "Topic :: Scientific/Engineering",
+        "Topic :: Security",
+        "Topic :: System :: Monitoring"
     ]
 )
```


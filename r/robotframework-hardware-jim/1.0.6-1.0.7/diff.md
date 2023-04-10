# Comparing `tmp/robotframework-hardware-jim-1.0.6.tar.gz` & `tmp/robotframework-hardware-jim-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-hardware-jim-1.0.6.tar", last modified: Mon Apr 10 03:11:47 2023, max compression
+gzip compressed data, was "robotframework-hardware-jim-1.0.7.tar", last modified: Mon Apr 10 05:13:38 2023, max compression
```

## Comparing `robotframework-hardware-jim-1.0.6.tar` & `robotframework-hardware-jim-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 03:11:47.485203 robotframework-hardware-jim-1.0.6/
--rw-rw-rw-   0        0        0     1094 2023-04-10 01:06:46.000000 robotframework-hardware-jim-1.0.6/LICENSE
--rw-rw-rw-   0        0        0       24 2023-04-07 07:14:30.000000 robotframework-hardware-jim-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      867 2023-04-10 03:11:47.483235 robotframework-hardware-jim-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       76 2023-04-10 02:25:02.000000 robotframework-hardware-jim-1.0.6/README.md
--rw-rw-rw-   0        0        0     3267 2023-04-10 02:21:45.000000 robotframework-hardware-jim-1.0.6/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 03:11:47.409197 robotframework-hardware-jim-1.0.6/robotframework_hardware_jim.egg-info/
--rw-rw-rw-   0        0        0      867 2023-04-10 03:11:47.000000 robotframework-hardware-jim-1.0.6/robotframework_hardware_jim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-04-10 03:11:47.000000 robotframework-hardware-jim-1.0.6/robotframework_hardware_jim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 03:11:47.000000 robotframework-hardware-jim-1.0.6/robotframework_hardware_jim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3096 2023-04-10 03:11:47.000000 robotframework-hardware-jim-1.0.6/robotframework_hardware_jim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-10 03:11:47.000000 robotframework-hardware-jim-1.0.6/robotframework_hardware_jim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 03:11:47.485203 robotframework-hardware-jim-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1951 2023-04-10 02:59:29.000000 robotframework-hardware-jim-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:11:47.348196 robotframework-hardware-jim-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-10 03:11:47.423205 robotframework-hardware-jim-1.0.6/src/HardwareLibrary/
--rw-rw-rw-   0        0        0     1556 2023-04-10 02:31:32.000000 robotframework-hardware-jim-1.0.6/src/HardwareLibrary/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:11:47.477196 robotframework-hardware-jim-1.0.6/src/HardwareLibrary/keywords/
--rw-rw-rw-   0        0        0       66 2023-04-10 02:29:54.000000 robotframework-hardware-jim-1.0.6/src/HardwareLibrary/keywords/__init__.py
--rw-rw-rw-   0        0        0     2979 2023-04-10 03:07:32.000000 robotframework-hardware-jim-1.0.6/src/HardwareLibrary/keywords/file.py
--rw-rw-rw-   0        0        0     1011 2023-04-10 03:07:44.000000 robotframework-hardware-jim-1.0.6/src/HardwareLibrary/keywords/system.py
--rw-rw-rw-   0        0        0       17 2023-04-10 03:11:01.000000 robotframework-hardware-jim-1.0.6/src/HardwareLibrary/version.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:13:38.143560 robotframework-hardware-jim-1.0.7/
+-rw-rw-rw-   0        0        0     1094 2023-04-10 01:06:46.000000 robotframework-hardware-jim-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-04-07 07:14:30.000000 robotframework-hardware-jim-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      867 2023-04-10 05:13:38.139561 robotframework-hardware-jim-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       76 2023-04-10 02:25:02.000000 robotframework-hardware-jim-1.0.7/README.md
+-rw-rw-rw-   0        0        0     3267 2023-04-10 02:21:45.000000 robotframework-hardware-jim-1.0.7/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 05:13:38.014562 robotframework-hardware-jim-1.0.7/robotframework_hardware_jim.egg-info/
+-rw-rw-rw-   0        0        0      867 2023-04-10 05:13:37.000000 robotframework-hardware-jim-1.0.7/robotframework_hardware_jim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      719 2023-04-10 05:13:37.000000 robotframework-hardware-jim-1.0.7/robotframework_hardware_jim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 05:13:37.000000 robotframework-hardware-jim-1.0.7/robotframework_hardware_jim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3096 2023-04-10 05:13:37.000000 robotframework-hardware-jim-1.0.7/robotframework_hardware_jim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-10 05:13:37.000000 robotframework-hardware-jim-1.0.7/robotframework_hardware_jim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 05:13:38.144559 robotframework-hardware-jim-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1951 2023-04-10 02:59:29.000000 robotframework-hardware-jim-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:13:37.948560 robotframework-hardware-jim-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:13:38.028560 robotframework-hardware-jim-1.0.7/src/HardwareLibrary/
+-rw-rw-rw-   0        0        0     1556 2023-04-10 02:31:32.000000 robotframework-hardware-jim-1.0.7/src/HardwareLibrary/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:13:38.038562 robotframework-hardware-jim-1.0.7/src/HardwareLibrary/hardware/
+-rw-rw-rw-   0        0        0        0 2023-04-10 05:11:32.000000 robotframework-hardware-jim-1.0.7/src/HardwareLibrary/hardware/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:13:38.050583 robotframework-hardware-jim-1.0.7/src/HardwareLibrary/hardware/interface/
+-rw-rw-rw-   0        0        0        0 2023-04-10 05:12:19.000000 robotframework-hardware-jim-1.0.7/src/HardwareLibrary/hardware/interface/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:13:38.114560 robotframework-hardware-jim-1.0.7/src/HardwareLibrary/hardware/moudle/
+-rw-rw-rw-   0        0        0      102 2023-04-10 03:10:23.000000 robotframework-hardware-jim-1.0.7/src/HardwareLibrary/hardware/moudle/__init__.py
+-rw-rw-rw-   0        0        0     6272 2023-04-10 03:00:11.000000 robotframework-hardware-jim-1.0.7/src/HardwareLibrary/hardware/moudle/file.py
+-rw-rw-rw-   0        0        0      593 2023-04-10 03:00:18.000000 robotframework-hardware-jim-1.0.7/src/HardwareLibrary/hardware/moudle/system.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:13:38.134561 robotframework-hardware-jim-1.0.7/src/HardwareLibrary/keywords/
+-rw-rw-rw-   0        0        0       66 2023-04-10 02:29:54.000000 robotframework-hardware-jim-1.0.7/src/HardwareLibrary/keywords/__init__.py
+-rw-rw-rw-   0        0        0     2979 2023-04-10 03:07:32.000000 robotframework-hardware-jim-1.0.7/src/HardwareLibrary/keywords/file.py
+-rw-rw-rw-   0        0        0     1011 2023-04-10 03:07:44.000000 robotframework-hardware-jim-1.0.7/src/HardwareLibrary/keywords/system.py
+-rw-rw-rw-   0        0        0       17 2023-04-10 05:13:02.000000 robotframework-hardware-jim-1.0.7/src/HardwareLibrary/version.py
```

### Comparing `robotframework-hardware-jim-1.0.6/LICENSE` & `robotframework-hardware-jim-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.6/PKG-INFO` & `robotframework-hardware-jim-1.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-hardware-jim
-Version: 1.0.6
+Version: 1.0.7
 Summary: Support Command and GUI operation for Windows
 Home-page: https://github.com/JimRevolutionist/robotframework-hardware
 Author: HP
 Author-email: jim.tang@hp.com
 License: MIT
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-hardware-jim-1.0.6/requirements.txt` & `robotframework-hardware-jim-1.0.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.6/robotframework_hardware_jim.egg-info/PKG-INFO` & `robotframework-hardware-jim-1.0.7/robotframework_hardware_jim.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-hardware-jim
-Version: 1.0.6
+Version: 1.0.7
 Summary: Support Command and GUI operation for Windows
 Home-page: https://github.com/JimRevolutionist/robotframework-hardware
 Author: HP
 Author-email: jim.tang@hp.com
 License: MIT
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-hardware-jim-1.0.6/robotframework_hardware_jim.egg-info/requires.txt` & `robotframework-hardware-jim-1.0.7/robotframework_hardware_jim.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.6/setup.py` & `robotframework-hardware-jim-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.6/src/HardwareLibrary/__init__.py` & `robotframework-hardware-jim-1.0.7/src/HardwareLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.6/src/HardwareLibrary/keywords/file.py` & `robotframework-hardware-jim-1.0.7/src/HardwareLibrary/keywords/file.py`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.6/src/HardwareLibrary/keywords/system.py` & `robotframework-hardware-jim-1.0.7/src/HardwareLibrary/keywords/system.py`

 * *Files identical despite different names*


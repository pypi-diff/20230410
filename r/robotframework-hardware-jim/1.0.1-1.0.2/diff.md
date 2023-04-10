# Comparing `tmp/robotframework-hardware-jim-1.0.1.tar.gz` & `tmp/robotframework-hardware-jim-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-hardware-jim-1.0.1.tar", last modified: Mon Apr 10 02:33:24 2023, max compression
+gzip compressed data, was "robotframework-hardware-jim-1.0.2.tar", last modified: Mon Apr 10 02:45:12 2023, max compression
```

## Comparing `robotframework-hardware-jim-1.0.1.tar` & `robotframework-hardware-jim-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 02:33:24.532751 robotframework-hardware-jim-1.0.1/
--rw-rw-rw-   0        0        0     1094 2023-04-10 01:06:46.000000 robotframework-hardware-jim-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       24 2023-04-07 07:14:30.000000 robotframework-hardware-jim-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      867 2023-04-10 02:33:24.530752 robotframework-hardware-jim-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       76 2023-04-10 02:25:02.000000 robotframework-hardware-jim-1.0.1/README.md
--rw-rw-rw-   0        0        0     3267 2023-04-10 02:21:45.000000 robotframework-hardware-jim-1.0.1/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 02:33:24.462753 robotframework-hardware-jim-1.0.1/robotframework_hardware_jim.egg-info/
--rw-rw-rw-   0        0        0      867 2023-04-10 02:33:24.000000 robotframework-hardware-jim-1.0.1/robotframework_hardware_jim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-04-10 02:33:24.000000 robotframework-hardware-jim-1.0.1/robotframework_hardware_jim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 02:33:24.000000 robotframework-hardware-jim-1.0.1/robotframework_hardware_jim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3096 2023-04-10 02:33:24.000000 robotframework-hardware-jim-1.0.1/robotframework_hardware_jim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-10 02:33:24.000000 robotframework-hardware-jim-1.0.1/robotframework_hardware_jim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 02:33:24.533751 robotframework-hardware-jim-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2002 2023-04-10 02:24:53.000000 robotframework-hardware-jim-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 02:33:24.400749 robotframework-hardware-jim-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-10 02:33:24.488748 robotframework-hardware-jim-1.0.1/src/HardwareLibrary/
--rw-rw-rw-   0        0        0     1556 2023-04-10 02:31:32.000000 robotframework-hardware-jim-1.0.1/src/HardwareLibrary/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 02:33:24.521778 robotframework-hardware-jim-1.0.1/src/HardwareLibrary/keywords/
--rw-rw-rw-   0        0        0       66 2023-04-10 02:29:54.000000 robotframework-hardware-jim-1.0.1/src/HardwareLibrary/keywords/__init__.py
--rw-rw-rw-   0        0        0     3056 2023-04-10 02:06:37.000000 robotframework-hardware-jim-1.0.1/src/HardwareLibrary/keywords/file.py
--rw-rw-rw-   0        0        0     1077 2023-04-10 02:11:39.000000 robotframework-hardware-jim-1.0.1/src/HardwareLibrary/keywords/system.py
--rw-rw-rw-   0        0        0       17 2023-04-10 02:32:01.000000 robotframework-hardware-jim-1.0.1/src/HardwareLibrary/version.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:45:12.289930 robotframework-hardware-jim-1.0.2/
+-rw-rw-rw-   0        0        0     1094 2023-04-10 01:06:46.000000 robotframework-hardware-jim-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-04-07 07:14:30.000000 robotframework-hardware-jim-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      867 2023-04-10 02:45:12.287874 robotframework-hardware-jim-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       76 2023-04-10 02:25:02.000000 robotframework-hardware-jim-1.0.2/README.md
+-rw-rw-rw-   0        0        0     3267 2023-04-10 02:21:45.000000 robotframework-hardware-jim-1.0.2/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 02:45:12.191218 robotframework-hardware-jim-1.0.2/robotframework_hardware_jim.egg-info/
+-rw-rw-rw-   0        0        0      867 2023-04-10 02:45:11.000000 robotframework-hardware-jim-1.0.2/robotframework_hardware_jim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-04-10 02:45:11.000000 robotframework-hardware-jim-1.0.2/robotframework_hardware_jim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 02:45:11.000000 robotframework-hardware-jim-1.0.2/robotframework_hardware_jim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3096 2023-04-10 02:45:11.000000 robotframework-hardware-jim-1.0.2/robotframework_hardware_jim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-10 02:45:11.000000 robotframework-hardware-jim-1.0.2/robotframework_hardware_jim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 02:45:12.295308 robotframework-hardware-jim-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2002 2023-04-10 02:24:53.000000 robotframework-hardware-jim-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:45:12.082026 robotframework-hardware-jim-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-10 02:45:12.218813 robotframework-hardware-jim-1.0.2/src/HardwareLibrary/
+-rw-rw-rw-   0        0        0     1556 2023-04-10 02:31:32.000000 robotframework-hardware-jim-1.0.2/src/HardwareLibrary/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:45:12.270736 robotframework-hardware-jim-1.0.2/src/HardwareLibrary/keywords/
+-rw-rw-rw-   0        0        0       66 2023-04-10 02:29:54.000000 robotframework-hardware-jim-1.0.2/src/HardwareLibrary/keywords/__init__.py
+-rw-rw-rw-   0        0        0     3056 2023-04-10 02:06:37.000000 robotframework-hardware-jim-1.0.2/src/HardwareLibrary/keywords/file.py
+-rw-rw-rw-   0        0        0     1077 2023-04-10 02:11:39.000000 robotframework-hardware-jim-1.0.2/src/HardwareLibrary/keywords/system.py
+-rw-rw-rw-   0        0        0       17 2023-04-10 02:40:25.000000 robotframework-hardware-jim-1.0.2/src/HardwareLibrary/version.py
```

### Comparing `robotframework-hardware-jim-1.0.1/LICENSE` & `robotframework-hardware-jim-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.1/PKG-INFO` & `robotframework-hardware-jim-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-hardware-jim
-Version: 1.0.1
+Version: 1.0.2
 Summary: Support Command and GUI operation for Windows
 Home-page: https://github.com/JimRevolutionist/robotframework-hardware
 Author: HP
 Author-email: jim.tang@hp.com
 License: MIT
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-hardware-jim-1.0.1/requirements.txt` & `robotframework-hardware-jim-1.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.1/robotframework_hardware_jim.egg-info/PKG-INFO` & `robotframework-hardware-jim-1.0.2/robotframework_hardware_jim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-hardware-jim
-Version: 1.0.1
+Version: 1.0.2
 Summary: Support Command and GUI operation for Windows
 Home-page: https://github.com/JimRevolutionist/robotframework-hardware
 Author: HP
 Author-email: jim.tang@hp.com
 License: MIT
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-hardware-jim-1.0.1/robotframework_hardware_jim.egg-info/requires.txt` & `robotframework-hardware-jim-1.0.2/robotframework_hardware_jim.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.1/setup.py` & `robotframework-hardware-jim-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.1/src/HardwareLibrary/__init__.py` & `robotframework-hardware-jim-1.0.2/src/HardwareLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.1/src/HardwareLibrary/keywords/file.py` & `robotframework-hardware-jim-1.0.2/src/HardwareLibrary/keywords/file.py`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.1/src/HardwareLibrary/keywords/system.py` & `robotframework-hardware-jim-1.0.2/src/HardwareLibrary/keywords/system.py`

 * *Files identical despite different names*


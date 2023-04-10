# Comparing `tmp/robotframework-hardware-jim-1.0.4.tar.gz` & `tmp/robotframework-hardware-jim-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-hardware-jim-1.0.4.tar", last modified: Mon Apr 10 02:54:52 2023, max compression
+gzip compressed data, was "robotframework-hardware-jim-1.0.5.tar", last modified: Mon Apr 10 03:01:19 2023, max compression
```

## Comparing `robotframework-hardware-jim-1.0.4.tar` & `robotframework-hardware-jim-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 02:54:52.962405 robotframework-hardware-jim-1.0.4/
--rw-rw-rw-   0        0        0     1094 2023-04-10 01:06:46.000000 robotframework-hardware-jim-1.0.4/LICENSE
--rw-rw-rw-   0        0        0       24 2023-04-07 07:14:30.000000 robotframework-hardware-jim-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      867 2023-04-10 02:54:52.956349 robotframework-hardware-jim-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       76 2023-04-10 02:25:02.000000 robotframework-hardware-jim-1.0.4/README.md
--rw-rw-rw-   0        0        0     3267 2023-04-10 02:21:45.000000 robotframework-hardware-jim-1.0.4/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 02:54:52.912347 robotframework-hardware-jim-1.0.4/robotframework_hardware_jim.egg-info/
--rw-rw-rw-   0        0        0      867 2023-04-10 02:54:52.000000 robotframework-hardware-jim-1.0.4/robotframework_hardware_jim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-04-10 02:54:52.000000 robotframework-hardware-jim-1.0.4/robotframework_hardware_jim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 02:54:52.000000 robotframework-hardware-jim-1.0.4/robotframework_hardware_jim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3096 2023-04-10 02:54:52.000000 robotframework-hardware-jim-1.0.4/robotframework_hardware_jim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-10 02:54:52.000000 robotframework-hardware-jim-1.0.4/robotframework_hardware_jim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 02:54:52.964349 robotframework-hardware-jim-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2002 2023-04-10 02:24:53.000000 robotframework-hardware-jim-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 02:54:52.847344 robotframework-hardware-jim-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-10 02:54:52.925343 robotframework-hardware-jim-1.0.4/src/HardwareLibrary/
--rw-rw-rw-   0        0        0     1556 2023-04-10 02:31:32.000000 robotframework-hardware-jim-1.0.4/src/HardwareLibrary/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 02:54:52.948344 robotframework-hardware-jim-1.0.4/src/HardwareLibrary/keywords/
--rw-rw-rw-   0        0        0       66 2023-04-10 02:29:54.000000 robotframework-hardware-jim-1.0.4/src/HardwareLibrary/keywords/__init__.py
--rw-rw-rw-   0        0        0     3048 2023-04-10 02:53:21.000000 robotframework-hardware-jim-1.0.4/src/HardwareLibrary/keywords/file.py
--rw-rw-rw-   0        0        0     1073 2023-04-10 02:48:03.000000 robotframework-hardware-jim-1.0.4/src/HardwareLibrary/keywords/system.py
--rw-rw-rw-   0        0        0       17 2023-04-10 02:54:50.000000 robotframework-hardware-jim-1.0.4/src/HardwareLibrary/version.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:01:19.391124 robotframework-hardware-jim-1.0.5/
+-rw-rw-rw-   0        0        0     1094 2023-04-10 01:06:46.000000 robotframework-hardware-jim-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-04-07 07:14:30.000000 robotframework-hardware-jim-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      867 2023-04-10 03:01:19.387118 robotframework-hardware-jim-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       76 2023-04-10 02:25:02.000000 robotframework-hardware-jim-1.0.5/README.md
+-rw-rw-rw-   0        0        0     3267 2023-04-10 02:21:45.000000 robotframework-hardware-jim-1.0.5/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 03:01:19.303120 robotframework-hardware-jim-1.0.5/robotframework_hardware_jim.egg-info/
+-rw-rw-rw-   0        0        0      867 2023-04-10 03:01:18.000000 robotframework-hardware-jim-1.0.5/robotframework_hardware_jim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-04-10 03:01:19.000000 robotframework-hardware-jim-1.0.5/robotframework_hardware_jim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 03:01:18.000000 robotframework-hardware-jim-1.0.5/robotframework_hardware_jim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3096 2023-04-10 03:01:18.000000 robotframework-hardware-jim-1.0.5/robotframework_hardware_jim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-10 03:01:18.000000 robotframework-hardware-jim-1.0.5/robotframework_hardware_jim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 03:01:19.393125 robotframework-hardware-jim-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1951 2023-04-10 02:59:29.000000 robotframework-hardware-jim-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:01:19.230163 robotframework-hardware-jim-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-10 03:01:19.323124 robotframework-hardware-jim-1.0.5/src/HardwareLibrary/
+-rw-rw-rw-   0        0        0     1556 2023-04-10 02:31:32.000000 robotframework-hardware-jim-1.0.5/src/HardwareLibrary/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:01:19.382125 robotframework-hardware-jim-1.0.5/src/HardwareLibrary/keywords/
+-rw-rw-rw-   0        0        0       66 2023-04-10 02:29:54.000000 robotframework-hardware-jim-1.0.5/src/HardwareLibrary/keywords/__init__.py
+-rw-rw-rw-   0        0        0     3018 2023-04-10 02:59:08.000000 robotframework-hardware-jim-1.0.5/src/HardwareLibrary/keywords/file.py
+-rw-rw-rw-   0        0        0     1043 2023-04-10 03:00:01.000000 robotframework-hardware-jim-1.0.5/src/HardwareLibrary/keywords/system.py
+-rw-rw-rw-   0        0        0       17 2023-04-10 03:00:24.000000 robotframework-hardware-jim-1.0.5/src/HardwareLibrary/version.py
```

### Comparing `robotframework-hardware-jim-1.0.4/LICENSE` & `robotframework-hardware-jim-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.4/PKG-INFO` & `robotframework-hardware-jim-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-hardware-jim
-Version: 1.0.4
+Version: 1.0.5
 Summary: Support Command and GUI operation for Windows
 Home-page: https://github.com/JimRevolutionist/robotframework-hardware
 Author: HP
 Author-email: jim.tang@hp.com
 License: MIT
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-hardware-jim-1.0.4/requirements.txt` & `robotframework-hardware-jim-1.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.4/robotframework_hardware_jim.egg-info/PKG-INFO` & `robotframework-hardware-jim-1.0.5/robotframework_hardware_jim.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-hardware-jim
-Version: 1.0.4
+Version: 1.0.5
 Summary: Support Command and GUI operation for Windows
 Home-page: https://github.com/JimRevolutionist/robotframework-hardware
 Author: HP
 Author-email: jim.tang@hp.com
 License: MIT
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-hardware-jim-1.0.4/robotframework_hardware_jim.egg-info/requires.txt` & `robotframework-hardware-jim-1.0.5/robotframework_hardware_jim.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.4/setup.py` & `robotframework-hardware-jim-1.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import sys
-import os
-sys.path.append(os.getcwd())
+
 from setuptools import setup, find_packages, Distribution
 
 
 class BinaryDistribution(Distribution):
     """Distribution which always forces a binary package with platform name"""
 
     # pylint: disable=no-self-use
```

### Comparing `robotframework-hardware-jim-1.0.4/src/HardwareLibrary/__init__.py` & `robotframework-hardware-jim-1.0.5/src/HardwareLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.4/src/HardwareLibrary/keywords/file.py` & `robotframework-hardware-jim-1.0.5/src/HardwareLibrary/keywords/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import sys
 import os
-sys.path.append(os.getcwd())
 from robotlibcore import keyword
 from HardwareLibrary.hardware.moudle.file import FTPUtils
 from HardwareLibrary.hardware.moudle.system import SystemBase
 
 
 LOCAL_DOWNLOAD_PATH = os.path.join(os.path.expanduser('~'), "Downloads")
```

### Comparing `robotframework-hardware-jim-1.0.4/src/HardwareLibrary/keywords/system.py` & `robotframework-hardware-jim-1.0.5/src/HardwareLibrary/keywords/system.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import sys
 import os
-sys.path.append(os.getcwd())
 from robotlibcore import keyword
 from HardwareLibrary.hardware.moudle.system import SystemBase
 
 
 system_base = SystemBase()
 
 class SystemKeywords():
```


# Comparing `tmp/robotframework-hardware-jim-1.0.3.tar.gz` & `tmp/robotframework-hardware-jim-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-hardware-jim-1.0.3.tar", last modified: Mon Apr 10 02:49:03 2023, max compression
+gzip compressed data, was "robotframework-hardware-jim-1.0.4.tar", last modified: Mon Apr 10 02:54:52 2023, max compression
```

## Comparing `robotframework-hardware-jim-1.0.3.tar` & `robotframework-hardware-jim-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 02:49:03.408377 robotframework-hardware-jim-1.0.3/
--rw-rw-rw-   0        0        0     1094 2023-04-10 01:06:46.000000 robotframework-hardware-jim-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       24 2023-04-07 07:14:30.000000 robotframework-hardware-jim-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      867 2023-04-10 02:49:03.406377 robotframework-hardware-jim-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       76 2023-04-10 02:25:02.000000 robotframework-hardware-jim-1.0.3/README.md
--rw-rw-rw-   0        0        0     3267 2023-04-10 02:21:45.000000 robotframework-hardware-jim-1.0.3/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 02:49:03.357397 robotframework-hardware-jim-1.0.3/robotframework_hardware_jim.egg-info/
--rw-rw-rw-   0        0        0      867 2023-04-10 02:49:02.000000 robotframework-hardware-jim-1.0.3/robotframework_hardware_jim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-04-10 02:49:03.000000 robotframework-hardware-jim-1.0.3/robotframework_hardware_jim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 02:49:02.000000 robotframework-hardware-jim-1.0.3/robotframework_hardware_jim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3096 2023-04-10 02:49:02.000000 robotframework-hardware-jim-1.0.3/robotframework_hardware_jim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-10 02:49:02.000000 robotframework-hardware-jim-1.0.3/robotframework_hardware_jim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 02:49:03.410380 robotframework-hardware-jim-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2002 2023-04-10 02:24:53.000000 robotframework-hardware-jim-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 02:49:03.251004 robotframework-hardware-jim-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-10 02:49:03.371377 robotframework-hardware-jim-1.0.3/src/HardwareLibrary/
--rw-rw-rw-   0        0        0     1556 2023-04-10 02:31:32.000000 robotframework-hardware-jim-1.0.3/src/HardwareLibrary/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 02:49:03.396374 robotframework-hardware-jim-1.0.3/src/HardwareLibrary/keywords/
--rw-rw-rw-   0        0        0       66 2023-04-10 02:29:54.000000 robotframework-hardware-jim-1.0.3/src/HardwareLibrary/keywords/__init__.py
--rw-rw-rw-   0        0        0     1073 2023-04-10 02:48:03.000000 robotframework-hardware-jim-1.0.3/src/HardwareLibrary/keywords/system.py
--rw-rw-rw-   0        0        0       17 2023-04-10 02:48:10.000000 robotframework-hardware-jim-1.0.3/src/HardwareLibrary/version.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:54:52.962405 robotframework-hardware-jim-1.0.4/
+-rw-rw-rw-   0        0        0     1094 2023-04-10 01:06:46.000000 robotframework-hardware-jim-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-04-07 07:14:30.000000 robotframework-hardware-jim-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      867 2023-04-10 02:54:52.956349 robotframework-hardware-jim-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       76 2023-04-10 02:25:02.000000 robotframework-hardware-jim-1.0.4/README.md
+-rw-rw-rw-   0        0        0     3267 2023-04-10 02:21:45.000000 robotframework-hardware-jim-1.0.4/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 02:54:52.912347 robotframework-hardware-jim-1.0.4/robotframework_hardware_jim.egg-info/
+-rw-rw-rw-   0        0        0      867 2023-04-10 02:54:52.000000 robotframework-hardware-jim-1.0.4/robotframework_hardware_jim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-04-10 02:54:52.000000 robotframework-hardware-jim-1.0.4/robotframework_hardware_jim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 02:54:52.000000 robotframework-hardware-jim-1.0.4/robotframework_hardware_jim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3096 2023-04-10 02:54:52.000000 robotframework-hardware-jim-1.0.4/robotframework_hardware_jim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-10 02:54:52.000000 robotframework-hardware-jim-1.0.4/robotframework_hardware_jim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 02:54:52.964349 robotframework-hardware-jim-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2002 2023-04-10 02:24:53.000000 robotframework-hardware-jim-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:54:52.847344 robotframework-hardware-jim-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-10 02:54:52.925343 robotframework-hardware-jim-1.0.4/src/HardwareLibrary/
+-rw-rw-rw-   0        0        0     1556 2023-04-10 02:31:32.000000 robotframework-hardware-jim-1.0.4/src/HardwareLibrary/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:54:52.948344 robotframework-hardware-jim-1.0.4/src/HardwareLibrary/keywords/
+-rw-rw-rw-   0        0        0       66 2023-04-10 02:29:54.000000 robotframework-hardware-jim-1.0.4/src/HardwareLibrary/keywords/__init__.py
+-rw-rw-rw-   0        0        0     3048 2023-04-10 02:53:21.000000 robotframework-hardware-jim-1.0.4/src/HardwareLibrary/keywords/file.py
+-rw-rw-rw-   0        0        0     1073 2023-04-10 02:48:03.000000 robotframework-hardware-jim-1.0.4/src/HardwareLibrary/keywords/system.py
+-rw-rw-rw-   0        0        0       17 2023-04-10 02:54:50.000000 robotframework-hardware-jim-1.0.4/src/HardwareLibrary/version.py
```

### Comparing `robotframework-hardware-jim-1.0.3/LICENSE` & `robotframework-hardware-jim-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.3/PKG-INFO` & `robotframework-hardware-jim-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-hardware-jim
-Version: 1.0.3
+Version: 1.0.4
 Summary: Support Command and GUI operation for Windows
 Home-page: https://github.com/JimRevolutionist/robotframework-hardware
 Author: HP
 Author-email: jim.tang@hp.com
 License: MIT
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-hardware-jim-1.0.3/requirements.txt` & `robotframework-hardware-jim-1.0.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.3/robotframework_hardware_jim.egg-info/PKG-INFO` & `robotframework-hardware-jim-1.0.4/robotframework_hardware_jim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-hardware-jim
-Version: 1.0.3
+Version: 1.0.4
 Summary: Support Command and GUI operation for Windows
 Home-page: https://github.com/JimRevolutionist/robotframework-hardware
 Author: HP
 Author-email: jim.tang@hp.com
 License: MIT
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-hardware-jim-1.0.3/robotframework_hardware_jim.egg-info/requires.txt` & `robotframework-hardware-jim-1.0.4/robotframework_hardware_jim.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.3/setup.py` & `robotframework-hardware-jim-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.3/src/HardwareLibrary/__init__.py` & `robotframework-hardware-jim-1.0.4/src/HardwareLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.3/src/HardwareLibrary/keywords/system.py` & `robotframework-hardware-jim-1.0.4/src/HardwareLibrary/keywords/system.py`

 * *Files identical despite different names*


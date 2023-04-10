# Comparing `tmp/robotframework-hardware-jim-1.0.5.tar.gz` & `tmp/robotframework-hardware-jim-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-hardware-jim-1.0.5.tar", last modified: Mon Apr 10 03:01:19 2023, max compression
+gzip compressed data, was "robotframework-hardware-jim-1.0.6.tar", last modified: Mon Apr 10 03:11:47 2023, max compression
```

## Comparing `robotframework-hardware-jim-1.0.5.tar` & `robotframework-hardware-jim-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 03:01:19.391124 robotframework-hardware-jim-1.0.5/
--rw-rw-rw-   0        0        0     1094 2023-04-10 01:06:46.000000 robotframework-hardware-jim-1.0.5/LICENSE
--rw-rw-rw-   0        0        0       24 2023-04-07 07:14:30.000000 robotframework-hardware-jim-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      867 2023-04-10 03:01:19.387118 robotframework-hardware-jim-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       76 2023-04-10 02:25:02.000000 robotframework-hardware-jim-1.0.5/README.md
--rw-rw-rw-   0        0        0     3267 2023-04-10 02:21:45.000000 robotframework-hardware-jim-1.0.5/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 03:01:19.303120 robotframework-hardware-jim-1.0.5/robotframework_hardware_jim.egg-info/
--rw-rw-rw-   0        0        0      867 2023-04-10 03:01:18.000000 robotframework-hardware-jim-1.0.5/robotframework_hardware_jim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-04-10 03:01:19.000000 robotframework-hardware-jim-1.0.5/robotframework_hardware_jim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 03:01:18.000000 robotframework-hardware-jim-1.0.5/robotframework_hardware_jim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3096 2023-04-10 03:01:18.000000 robotframework-hardware-jim-1.0.5/robotframework_hardware_jim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-10 03:01:18.000000 robotframework-hardware-jim-1.0.5/robotframework_hardware_jim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 03:01:19.393125 robotframework-hardware-jim-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1951 2023-04-10 02:59:29.000000 robotframework-hardware-jim-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:01:19.230163 robotframework-hardware-jim-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-10 03:01:19.323124 robotframework-hardware-jim-1.0.5/src/HardwareLibrary/
--rw-rw-rw-   0        0        0     1556 2023-04-10 02:31:32.000000 robotframework-hardware-jim-1.0.5/src/HardwareLibrary/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:01:19.382125 robotframework-hardware-jim-1.0.5/src/HardwareLibrary/keywords/
--rw-rw-rw-   0        0        0       66 2023-04-10 02:29:54.000000 robotframework-hardware-jim-1.0.5/src/HardwareLibrary/keywords/__init__.py
--rw-rw-rw-   0        0        0     3018 2023-04-10 02:59:08.000000 robotframework-hardware-jim-1.0.5/src/HardwareLibrary/keywords/file.py
--rw-rw-rw-   0        0        0     1043 2023-04-10 03:00:01.000000 robotframework-hardware-jim-1.0.5/src/HardwareLibrary/keywords/system.py
--rw-rw-rw-   0        0        0       17 2023-04-10 03:00:24.000000 robotframework-hardware-jim-1.0.5/src/HardwareLibrary/version.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:11:47.485203 robotframework-hardware-jim-1.0.6/
+-rw-rw-rw-   0        0        0     1094 2023-04-10 01:06:46.000000 robotframework-hardware-jim-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-04-07 07:14:30.000000 robotframework-hardware-jim-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      867 2023-04-10 03:11:47.483235 robotframework-hardware-jim-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       76 2023-04-10 02:25:02.000000 robotframework-hardware-jim-1.0.6/README.md
+-rw-rw-rw-   0        0        0     3267 2023-04-10 02:21:45.000000 robotframework-hardware-jim-1.0.6/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 03:11:47.409197 robotframework-hardware-jim-1.0.6/robotframework_hardware_jim.egg-info/
+-rw-rw-rw-   0        0        0      867 2023-04-10 03:11:47.000000 robotframework-hardware-jim-1.0.6/robotframework_hardware_jim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-04-10 03:11:47.000000 robotframework-hardware-jim-1.0.6/robotframework_hardware_jim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 03:11:47.000000 robotframework-hardware-jim-1.0.6/robotframework_hardware_jim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3096 2023-04-10 03:11:47.000000 robotframework-hardware-jim-1.0.6/robotframework_hardware_jim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-10 03:11:47.000000 robotframework-hardware-jim-1.0.6/robotframework_hardware_jim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 03:11:47.485203 robotframework-hardware-jim-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1951 2023-04-10 02:59:29.000000 robotframework-hardware-jim-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:11:47.348196 robotframework-hardware-jim-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-10 03:11:47.423205 robotframework-hardware-jim-1.0.6/src/HardwareLibrary/
+-rw-rw-rw-   0        0        0     1556 2023-04-10 02:31:32.000000 robotframework-hardware-jim-1.0.6/src/HardwareLibrary/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:11:47.477196 robotframework-hardware-jim-1.0.6/src/HardwareLibrary/keywords/
+-rw-rw-rw-   0        0        0       66 2023-04-10 02:29:54.000000 robotframework-hardware-jim-1.0.6/src/HardwareLibrary/keywords/__init__.py
+-rw-rw-rw-   0        0        0     2979 2023-04-10 03:07:32.000000 robotframework-hardware-jim-1.0.6/src/HardwareLibrary/keywords/file.py
+-rw-rw-rw-   0        0        0     1011 2023-04-10 03:07:44.000000 robotframework-hardware-jim-1.0.6/src/HardwareLibrary/keywords/system.py
+-rw-rw-rw-   0        0        0       17 2023-04-10 03:11:01.000000 robotframework-hardware-jim-1.0.6/src/HardwareLibrary/version.py
```

### Comparing `robotframework-hardware-jim-1.0.5/LICENSE` & `robotframework-hardware-jim-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.5/PKG-INFO` & `robotframework-hardware-jim-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-hardware-jim
-Version: 1.0.5
+Version: 1.0.6
 Summary: Support Command and GUI operation for Windows
 Home-page: https://github.com/JimRevolutionist/robotframework-hardware
 Author: HP
 Author-email: jim.tang@hp.com
 License: MIT
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-hardware-jim-1.0.5/requirements.txt` & `robotframework-hardware-jim-1.0.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.5/robotframework_hardware_jim.egg-info/PKG-INFO` & `robotframework-hardware-jim-1.0.6/robotframework_hardware_jim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-hardware-jim
-Version: 1.0.5
+Version: 1.0.6
 Summary: Support Command and GUI operation for Windows
 Home-page: https://github.com/JimRevolutionist/robotframework-hardware
 Author: HP
 Author-email: jim.tang@hp.com
 License: MIT
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-hardware-jim-1.0.5/robotframework_hardware_jim.egg-info/requires.txt` & `robotframework-hardware-jim-1.0.6/robotframework_hardware_jim.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.5/setup.py` & `robotframework-hardware-jim-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.5/src/HardwareLibrary/__init__.py` & `robotframework-hardware-jim-1.0.6/src/HardwareLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-hardware-jim-1.0.5/src/HardwareLibrary/keywords/file.py` & `robotframework-hardware-jim-1.0.6/src/HardwareLibrary/keywords/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from HardwareLibrary.hardware.moudle.file import FTPUtils
 from HardwareLibrary.hardware.moudle.system import SystemBase
 
 
 LOCAL_DOWNLOAD_PATH = os.path.join(os.path.expanduser('~'), "Downloads")
    
    
-class FileKeywords():
+class FileKeywords:
     """
     Interface implementation from robotframework usage for file keywords.
     """
     
     def __init__(self):
         pass
     
@@ -74,9 +74,8 @@
 
         Examples:
         | Install Thinupdate Package  <package>  <local_path>                  |
         """
         
         # install ThinUpdate package
         local_package = os.path.join(local_path, package)
-        system_base = SystemBase()
-        system_base.run_powershell(["msiexec", f"/i {local_package}", "/qb"])
+        SystemBase.run_powershell(["msiexec", f"/i {local_package}", "/qb"])
```

### Comparing `robotframework-hardware-jim-1.0.5/src/HardwareLibrary/keywords/system.py` & `robotframework-hardware-jim-1.0.6/src/HardwareLibrary/keywords/system.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import sys
 import os
 from robotlibcore import keyword
 from HardwareLibrary.hardware.moudle.system import SystemBase
 
 
-system_base = SystemBase()
 
-class SystemKeywords():
+class SystemKeywords:
     """
     Interface implementation from robotframework usage for file keywords.
     """
     
     def __init__(self):
         pass
     
@@ -24,21 +23,21 @@
 
         language = ["zh-CN", "en-US"]
         
         Examples:
         | Set Regional Format  <language>  |
         
         """
-        system_base.run_powershell(["Set-Culture", language])
+        SystemBase.run_powershell(["Set-Culture", language])
         
     
     @keyword
     def get_regional_format(self):
         """get_regional_format
 
         Examples:
         | Get Regional Format  |
         
         """
         
-        return system_base.run_powershell(["Get-Culture"])
+        return SystemBase.run_powershell(["Get-Culture"])
```


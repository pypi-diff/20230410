# Comparing `tmp/weekdaytime-0.0.10.tar.gz` & `tmp/weekdaytime-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\weekdaytime-0.0.10.tar", last modified: Mon Apr 10 11:35:22 2023, max compression
+gzip compressed data, was "dist\weekdaytime-0.0.9.tar", last modified: Mon Apr 10 10:57:09 2023, max compression
```

## Comparing `weekdaytime-0.0.10.tar` & `weekdaytime-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:22.000000 weekdaytime-0.0.10/
--rw-rw-rw-   0        0        0     1091 2023-04-05 09:07:45.000000 weekdaytime-0.0.10/LICENSE
--rw-rw-rw-   0        0        0       34 2023-04-10 10:38:24.000000 weekdaytime-0.0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     4850 2023-04-10 11:35:22.000000 weekdaytime-0.0.10/PKG-INFO
--rw-rw-rw-   0        0        0     4520 2023-04-10 11:34:39.000000 weekdaytime-0.0.10/README.md
--rw-rw-rw-   0        0        0      148 2023-04-10 11:35:22.000000 weekdaytime-0.0.10/setup.cfg
--rw-rw-rw-   0        0        0      516 2023-04-10 11:35:08.000000 weekdaytime-0.0.10/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:22.000000 weekdaytime-0.0.10/weekdaytime/
--rw-rw-rw-   0        0        0     7096 2023-04-10 09:20:43.000000 weekdaytime-0.0.10/weekdaytime/period.py
--rw-rw-rw-   0        0        0     2345 2023-04-08 14:41:13.000000 weekdaytime-0.0.10/weekdaytime/weekdaytime.py
--rw-rw-rw-   0        0        0       90 2023-04-10 11:35:12.000000 weekdaytime-0.0.10/weekdaytime/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:22.000000 weekdaytime-0.0.10/weekdaytime.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-10 11:35:22.000000 weekdaytime-0.0.10/weekdaytime.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-10 10:57:09.000000 weekdaytime-0.0.10/weekdaytime.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4850 2023-04-10 11:35:22.000000 weekdaytime-0.0.10/weekdaytime.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-04-10 11:35:22.000000 weekdaytime-0.0.10/weekdaytime.egg-info/requires.txt
--rw-rw-rw-   0        0        0      329 2023-04-10 11:35:22.000000 weekdaytime-0.0.10/weekdaytime.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2023-04-10 11:35:22.000000 weekdaytime-0.0.10/weekdaytime.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-04-05 09:07:45.000000 weekdaytime-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-04-10 10:38:24.000000 weekdaytime-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5018 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4689 2023-04-10 10:50:15.000000 weekdaytime-0.0.9/README.md
+-rw-rw-rw-   0        0        0      148 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      515 2023-04-10 10:50:49.000000 weekdaytime-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime/
+-rw-rw-rw-   0        0        0     7096 2023-04-10 09:20:43.000000 weekdaytime-0.0.9/weekdaytime/period.py
+-rw-rw-rw-   0        0        0     2345 2023-04-08 14:41:13.000000 weekdaytime-0.0.9/weekdaytime/weekdaytime.py
+-rw-rw-rw-   0        0        0       89 2023-04-10 10:50:53.000000 weekdaytime-0.0.9/weekdaytime/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     5018 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      329 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/top_level.txt
```

### Comparing `weekdaytime-0.0.10/LICENSE` & `weekdaytime-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `weekdaytime-0.0.10/PKG-INFO` & `weekdaytime-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: weekdaytime
-Version: 0.0.10
-Summary: Python library that models available periods in a week
-Home-page: https://github.com/AaronTHCheung/weekdaytime
-Author: Aaron Cheung
-License: MIT
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # weekdaytime: modelling availability within a week
 This library includes Python classes for modelling available periods within a week.
 
 ## Key features
 - Simple checking of whether visiting period is within an available period. The expression
     ```
     visit_period in available_period
@@ -21,18 +9,23 @@
     evaluates to True if and only if ```visit_period``` is within ```available_period```.
 - Manipulate period objects with bitwise operators (```|, &, ~, ^```)
 - Convert period string into a period object, and vise versa (e.g., `'09:00~15:00,17:00~21:00;15:00~02:00(Fri,Sat)'`)
 
 ## Installation
 1. Python version must not be less than 3.6.
 2. The dependent library `bitarray` requires Microsoft Visual C++ 14.0. Get it with "Microsoft Visual C++ Build Tools": https://visualstudio.microsoft.com/downloads/
-3. Install with pip using the command
-    ```
-    pip install weekdaytime
-    ```
+3. 
+    - Install with pip using the command
+        ```
+        pip install weekdaytime
+        ```
+    - Alternatively, the library can also be installed with anaconda using the command
+        ```
+        conda install weekdaytime
+        ```
 
 ## Usage
 ### weekdaytime class
 A weekdaytime instance specifies a point in time in a week.
 ```
 from weekdaytime import weekdaytime as wdt
 
@@ -129,9 +122,8 @@
 p = period.strpperiod(avail_string)
 print(p)  # '09:00~15:00,17:00~21:00(Mon,Tue,Thu);00:00~02:00,09:00~21:00(Sun);12:00~24:00(Fri);00:00~02:00,12:00~24:00(Sat)'
 
 # Specifying all opening weekdays, the effect is the same
 avail_string = '09:00~15:00,17:00~21:00(Mon,Tue,Thu);12:00~02:00(Fri,Sat);09:00~21:00(Sun)'
 p = period.strpperiod(avail_string)
 print(p)  # '09:00~15:00,17:00~21:00(Mon,Tue,Thu);00:00~02:00,09:00~21:00(Sun);12:00~24:00(Fri);00:00~02:00,12:00~24:00(Sat)'
-```
-
+```
```

### Comparing `weekdaytime-0.0.10/README.md` & `weekdaytime-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: weekdaytime
+Version: 0.0.9
+Summary: Python library that models available periods in a week
+Home-page: https://github.com/AaronTHCheung/weekdaytime
+Author: Aaron Cheung
+License: MIT
+Platform: UNKNOWN
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # weekdaytime: modelling availability within a week
 This library includes Python classes for modelling available periods within a week.
 
 ## Key features
 - Simple checking of whether visiting period is within an available period. The expression
     ```
     visit_period in available_period
@@ -9,18 +21,23 @@
     evaluates to True if and only if ```visit_period``` is within ```available_period```.
 - Manipulate period objects with bitwise operators (```|, &, ~, ^```)
 - Convert period string into a period object, and vise versa (e.g., `'09:00~15:00,17:00~21:00;15:00~02:00(Fri,Sat)'`)
 
 ## Installation
 1. Python version must not be less than 3.6.
 2. The dependent library `bitarray` requires Microsoft Visual C++ 14.0. Get it with "Microsoft Visual C++ Build Tools": https://visualstudio.microsoft.com/downloads/
-3. Install with pip using the command
-    ```
-    pip install weekdaytime
-    ```
+3. 
+    - Install with pip using the command
+        ```
+        pip install weekdaytime
+        ```
+    - Alternatively, the library can also be installed with anaconda using the command
+        ```
+        conda install weekdaytime
+        ```
 
 ## Usage
 ### weekdaytime class
 A weekdaytime instance specifies a point in time in a week.
 ```
 from weekdaytime import weekdaytime as wdt
 
@@ -117,8 +134,9 @@
 p = period.strpperiod(avail_string)
 print(p)  # '09:00~15:00,17:00~21:00(Mon,Tue,Thu);00:00~02:00,09:00~21:00(Sun);12:00~24:00(Fri);00:00~02:00,12:00~24:00(Sat)'
 
 # Specifying all opening weekdays, the effect is the same
 avail_string = '09:00~15:00,17:00~21:00(Mon,Tue,Thu);12:00~02:00(Fri,Sat);09:00~21:00(Sun)'
 p = period.strpperiod(avail_string)
 print(p)  # '09:00~15:00,17:00~21:00(Mon,Tue,Thu);00:00~02:00,09:00~21:00(Sun);12:00~24:00(Fri);00:00~02:00,12:00~24:00(Sat)'
-```
+```
+
```

### Comparing `weekdaytime-0.0.10/setup.py` & `weekdaytime-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 from pathlib import Path
 
 long_description = (Path(__file__).parent/'README.md').read_text()
 setup(
     name='weekdaytime',
-    version='0.0.10',
+    version='0.0.9',
     description='Python library that models available periods in a week',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Aaron Cheung',
     packages=['weekdaytime'],
     python_requires='>=3.6',
     install_requires=[
```

### Comparing `weekdaytime-0.0.10/weekdaytime/period.py` & `weekdaytime-0.0.9/weekdaytime/period.py`

 * *Files identical despite different names*

### Comparing `weekdaytime-0.0.10/weekdaytime/weekdaytime.py` & `weekdaytime-0.0.9/weekdaytime/weekdaytime.py`

 * *Files identical despite different names*

### Comparing `weekdaytime-0.0.10/weekdaytime.egg-info/PKG-INFO` & `weekdaytime-0.0.9/weekdaytime.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weekdaytime
-Version: 0.0.10
+Version: 0.0.9
 Summary: Python library that models available periods in a week
 Home-page: https://github.com/AaronTHCheung/weekdaytime
 Author: Aaron Cheung
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -21,18 +21,23 @@
     evaluates to True if and only if ```visit_period``` is within ```available_period```.
 - Manipulate period objects with bitwise operators (```|, &, ~, ^```)
 - Convert period string into a period object, and vise versa (e.g., `'09:00~15:00,17:00~21:00;15:00~02:00(Fri,Sat)'`)
 
 ## Installation
 1. Python version must not be less than 3.6.
 2. The dependent library `bitarray` requires Microsoft Visual C++ 14.0. Get it with "Microsoft Visual C++ Build Tools": https://visualstudio.microsoft.com/downloads/
-3. Install with pip using the command
-    ```
-    pip install weekdaytime
-    ```
+3. 
+    - Install with pip using the command
+        ```
+        pip install weekdaytime
+        ```
+    - Alternatively, the library can also be installed with anaconda using the command
+        ```
+        conda install weekdaytime
+        ```
 
 ## Usage
 ### weekdaytime class
 A weekdaytime instance specifies a point in time in a week.
 ```
 from weekdaytime import weekdaytime as wdt
```


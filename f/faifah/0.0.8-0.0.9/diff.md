# Comparing `tmp/faifah-0.0.8.tar.gz` & `tmp/faifah-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faifah-0.0.8.tar", last modified: Mon Jan 16 03:53:22 2023, max compression
+gzip compressed data, was "faifah-0.0.9.tar", last modified: Mon Jan 16 04:30:12 2023, max compression
```

## Comparing `faifah-0.0.8.tar` & `faifah-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-01-16 03:53:22.963848 faifah-0.0.8/
--rw-rw-rw-   0        0        0     1063 2023-01-16 02:27:57.000000 faifah-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      651 2023-01-16 03:53:22.963848 faifah-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      151 2023-01-16 02:49:27.000000 faifah-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-16 03:53:22.935844 faifah-0.0.8/faifah/
--rw-rw-rw-   0        0        0    43851 2023-01-16 03:16:46.000000 faifah-0.0.8/faifah/__init__.py
--rw-rw-rw-   0        0        0    11078 2023-01-16 02:49:27.000000 faifah-0.0.8/faifah/ieee_test_system.py
--rw-rw-rw-   0        0        0      551 2023-01-16 02:49:27.000000 faifah-0.0.8/faifah/lumache.py
--rw-rw-rw-   0        0        0      618 2023-01-16 02:49:27.000000 faifah-0.0.8/faifah/test.py
-drwxrwxrwx   0        0        0        0 2023-01-16 03:53:22.962917 faifah-0.0.8/faifah.egg-info/
--rw-rw-rw-   0        0        0      651 2023-01-16 03:53:22.000000 faifah-0.0.8/faifah.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-01-16 03:53:22.000000 faifah-0.0.8/faifah.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-16 03:53:22.000000 faifah-0.0.8/faifah.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-01-16 03:53:22.000000 faifah-0.0.8/faifah.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-01-16 03:53:22.000000 faifah-0.0.8/faifah.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-01-16 03:45:42.000000 faifah-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-16 03:53:22.965844 faifah-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      995 2023-01-16 03:39:44.000000 faifah-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-16 04:30:12.483109 faifah-0.0.9/
+-rw-rw-rw-   0        0        0     1063 2023-01-16 02:27:57.000000 faifah-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      651 2023-01-16 04:30:12.484104 faifah-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      151 2023-01-16 02:49:27.000000 faifah-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-01-16 04:30:12.464102 faifah-0.0.9/faifah/
+-rw-rw-rw-   0        0        0    44193 2023-01-16 04:28:05.000000 faifah-0.0.9/faifah/__init__.py
+-rw-rw-rw-   0        0        0    11078 2023-01-16 02:49:27.000000 faifah-0.0.9/faifah/ieee_test_system.py
+-rw-rw-rw-   0        0        0      454 2023-01-16 04:22:49.000000 faifah-0.0.9/faifah/load_profile.py
+-rw-rw-rw-   0        0        0      551 2023-01-16 02:49:27.000000 faifah-0.0.9/faifah/lumache.py
+drwxrwxrwx   0        0        0        0 2023-01-16 04:30:12.482150 faifah-0.0.9/faifah.egg-info/
+-rw-rw-rw-   0        0        0      651 2023-01-16 04:30:12.000000 faifah-0.0.9/faifah.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-01-16 04:30:12.000000 faifah-0.0.9/faifah.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-16 04:30:12.000000 faifah-0.0.9/faifah.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-01-16 04:30:12.000000 faifah-0.0.9/faifah.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-01-16 04:30:12.000000 faifah-0.0.9/faifah.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-01-16 03:45:42.000000 faifah-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-01-16 04:30:12.485146 faifah-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      995 2023-01-16 04:30:04.000000 faifah-0.0.9/setup.py
```

### Comparing `faifah-0.0.8/LICENSE` & `faifah-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `faifah-0.0.8/PKG-INFO` & `faifah-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faifah
-Version: 0.0.8
+Version: 0.0.9
 Summary: DESCRIPTION
 Author: AKANIT KWANGKAEW
 Author-email: <akanitk84@gmail.com>
 Keywords: python,power system,voltage stability
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `faifah-0.0.8/faifah/__init__.py` & `faifah-0.0.9/faifah/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,22 @@
 from numpy import genfromtxt
 from colorama import Fore, Back, Style
 from termcolor import colored
 
 # from <FOLDER NAME> import <NAME of .py>
 #For PYPI
 from faifah import ieee_test_system
+from faifah import load_profile as lp
+
 
 #For local run
 # import ieee_test_system
+# import load_profile as lp
+
+
 
 
 # Require :
 # - numpy
 # - pandas
 
 # - linopy 
@@ -1117,14 +1122,22 @@
     MVA_base = 100.0 # Defining the Base-MVA
     KV_base = 100 #KV 
     nBus = 5
     SLACK_POS = 1
 
     IEEE5 = Grid( nBus, NETWORK_, '', '', MVA_base ,  KV_base, SLACK_POS )
     IEEE5.Report()
+    import os
+
+    # print(loadProfile_2017.csv loadProfile_2017.csv)
+    # print('File name :    ', os.path.basename( "loadProfile_2017.csv"))
+    # print('Directory Name:     ', os.path.dirname("loadProfile_2017.csv"))
+    print(lp.df_loadProfile.head() )
+
+
 
     # print( IEEE5.line_data )
     # print( IEEE5.load_data )
```

### Comparing `faifah-0.0.8/faifah/ieee_test_system.py` & `faifah-0.0.9/faifah/ieee_test_system.py`

 * *Files identical despite different names*

### Comparing `faifah-0.0.8/faifah/lumache.py` & `faifah-0.0.9/faifah/lumache.py`

 * *Files identical despite different names*

### Comparing `faifah-0.0.8/faifah.egg-info/PKG-INFO` & `faifah-0.0.9/faifah.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faifah
-Version: 0.0.8
+Version: 0.0.9
 Summary: DESCRIPTION
 Author: AKANIT KWANGKAEW
 Author-email: <akanitk84@gmail.com>
 Keywords: python,power system,voltage stability
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `faifah-0.0.8/setup.py` & `faifah-0.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'DESCRIPTION'
 LONG_DESCRIPTION = 'Open source for analysing electric power distribution system'
 
 # Setting up
 setup(
     name="faifah",
     version=VERSION,
```


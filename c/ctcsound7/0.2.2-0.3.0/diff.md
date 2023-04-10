# Comparing `tmp/ctcsound7-0.2.2.tar.gz` & `tmp/ctcsound7-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctcsound7-0.2.2.tar", last modified: Mon Apr  3 20:59:21 2023, max compression
+gzip compressed data, was "ctcsound7-0.3.0.tar", last modified: Mon Apr 10 10:43:54 2023, max compression
```

## Comparing `ctcsound7-0.2.2.tar` & `ctcsound7-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-03 20:59:21.448829 ctcsound7-0.2.2/
--rw-rw-r--   0 em        (1000) em        (1000)    26461 2018-10-07 17:31:50.000000 ctcsound7-0.2.2/LICENSE
--rw-rw-r--   0 em        (1000) em        (1000)      801 2023-04-03 20:59:21.449828 ctcsound7-0.2.2/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      319 2023-04-03 14:41:44.000000 ctcsound7-0.2.2/README.rst
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-03 20:59:21.448829 ctcsound7-0.2.2/ctcsound7.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)      801 2023-04-03 20:59:21.000000 ctcsound7-0.2.2/ctcsound7.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      246 2023-04-03 20:59:21.000000 ctcsound7-0.2.2/ctcsound7.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-03 20:59:21.000000 ctcsound7-0.2.2/ctcsound7.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-03 08:25:36.000000 ctcsound7-0.2.2/ctcsound7.egg-info/not-zip-safe
--rw-rw-r--   0 em        (1000) em        (1000)       12 2023-04-03 20:59:21.000000 ctcsound7-0.2.2/ctcsound7.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)       10 2023-04-03 20:59:21.000000 ctcsound7-0.2.2/ctcsound7.egg-info/top_level.txt
--rw-rw-r--   0 em        (1000) em        (1000)   123583 2023-04-03 20:59:09.000000 ctcsound7-0.2.2/ctcsound7.py
--rw-rw-r--   0 em        (1000) em        (1000)      524 2023-04-03 20:59:21.449828 ctcsound7-0.2.2/setup.cfg
--rwxrwxr-x   0 em        (1000) em        (1000)      531 2023-04-03 20:59:17.000000 ctcsound7-0.2.2/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-10 10:43:54.595877 ctcsound7-0.3.0/
+-rw-rw-r--   0 em        (1000) em        (1000)    26461 2018-10-07 17:31:50.000000 ctcsound7-0.3.0/LICENSE
+-rw-rw-r--   0 em        (1000) em        (1000)      821 2023-04-10 10:43:54.595877 ctcsound7-0.3.0/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      319 2023-04-03 14:41:44.000000 ctcsound7-0.3.0/README.rst
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-10 10:43:54.595877 ctcsound7-0.3.0/ctcsound7.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)      821 2023-04-10 10:43:54.000000 ctcsound7-0.3.0/ctcsound7.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      246 2023-04-10 10:43:54.000000 ctcsound7-0.3.0/ctcsound7.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-10 10:43:54.000000 ctcsound7-0.3.0/ctcsound7.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-03 08:25:36.000000 ctcsound7-0.3.0/ctcsound7.egg-info/not-zip-safe
+-rw-rw-r--   0 em        (1000) em        (1000)       12 2023-04-10 10:43:54.000000 ctcsound7-0.3.0/ctcsound7.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       10 2023-04-10 10:43:54.000000 ctcsound7-0.3.0/ctcsound7.egg-info/top_level.txt
+-rw-rw-r--   0 em        (1000) em        (1000)   123618 2023-04-10 10:41:39.000000 ctcsound7-0.3.0/ctcsound7.py
+-rw-rw-r--   0 em        (1000) em        (1000)      524 2023-04-10 10:43:54.596877 ctcsound7-0.3.0/setup.cfg
+-rwxrwxr-x   0 em        (1000) em        (1000)      531 2023-04-10 10:41:53.000000 ctcsound7-0.3.0/setup.py
```

### Comparing `ctcsound7-0.2.2/LICENSE` & `ctcsound7-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ctcsound7-0.2.2/PKG-INFO` & `ctcsound7-0.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: ctcsound7
-Version: 0.2.2
+Version: 0.3.0
 Summary: Python bindings to the Csound API using ctypes
 Home-page: https://github.com/csound-plugins/ctcsound7
 Author: Eduardo Moguillansky, Francois Pinot
 Author-email: eduardo.moguillansky@gmail.com
 License: BSD-3-Clause
 Keywords: csound
+Platform: UNKNOWN
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 License-File: LICENSE
 
 
@@ -30,7 +31,9 @@
 Csound needs to be installed in the system.
 
 
 .. code::
 
 	pip install ctcsound7
 
+
+
```

### Comparing `ctcsound7-0.2.2/ctcsound7.egg-info/PKG-INFO` & `ctcsound7-0.3.0/ctcsound7.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: ctcsound7
-Version: 0.2.2
+Version: 0.3.0
 Summary: Python bindings to the Csound API using ctypes
 Home-page: https://github.com/csound-plugins/ctcsound7
 Author: Eduardo Moguillansky, Francois Pinot
 Author-email: eduardo.moguillansky@gmail.com
 License: BSD-3-Clause
 Keywords: csound
+Platform: UNKNOWN
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 License-File: LICENSE
 
 
@@ -30,7 +31,9 @@
 Csound needs to be installed in the system.
 
 
 .. code::
 
 	pip install ctcsound7
 
+
+
```

### Comparing `ctcsound7-0.2.2/ctcsound7.py` & `ctcsound7-0.3.0/ctcsound7.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,16 +40,18 @@
 elif np.__version__ < '1.16':
     sys.exit("ctcsound won't work with numpy 1.15.x. Please revert numpy" +
         " to an older version or update numpy to a version >= 1.16")
 else:
     arrFromPointer = lambda p : p.contents
 
 if sys.platform.startswith('linux'):
-    libcsound = ct.CDLL(ctypes.util.find_library('csound64'))
-    # libcsound = ct.CDLL("libcsound64.so")
+    try:
+        libcsound = ct.CDLL("libcsound64.so")
+    except OSError:
+        libcsound = ct.CDLL(ctypes.util.find_library('csound64'))
 elif sys.platform.startswith('win'):
     if sys.version_info.major <=3 and sys.version_info.minor < 8:
         libcsound = ct.cdll.csound64
     else:
         libcsound = ct.CDLL(ctypes.util.find_library("csound64"))
 elif sys.platform.startswith('darwin'):
     libcsound = ct.CDLL(ctypes.util.find_library("CsoundLib64"))
```

### Comparing `ctcsound7-0.2.2/setup.cfg` & `ctcsound7-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ctcsound7-0.2.2/setup.py` & `ctcsound7-0.3.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 classifiers = """
 Topic :: Multimedia :: Sound/Audio
 Programming Language :: Python :: 2
 Programming Language :: Python :: 3
 """
 
 setup(name='ctcsound7',
-      version='0.2.2',
+      version='0.3.0',
       url='https://github.com/csound-plugins/ctcsound7',
       description='Python bindings to the Csound API using ctypes', 
       long_description=open('README.rst').read(),
       classifiers=filter(None, classifiers.split('\n')),
       py_modules=['ctcsound7'],
       install_requires=[
         'numpy>=1.16'
```


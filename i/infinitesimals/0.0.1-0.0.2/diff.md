# Comparing `tmp/infinitesimals-0.0.1.tar.gz` & `tmp/infinitesimals-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infinitesimals-0.0.1.tar", last modified: Mon Apr 10 20:45:31 2023, max compression
+gzip compressed data, was "infinitesimals-0.0.2.tar", last modified: Mon Apr 10 21:01:36 2023, max compression
```

## Comparing `infinitesimals-0.0.1.tar` & `infinitesimals-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 20:45:31.452575 infinitesimals-0.0.1/
--rw-rw-rw-   0        0        0       63 2023-04-10 19:05:04.000000 infinitesimals-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 infinitesimals-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-10 19:18:21.000000 infinitesimals-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      808 2023-04-10 20:45:31.451578 infinitesimals-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      100 2023-04-10 19:05:04.000000 infinitesimals-0.0.1/README.txt
--rw-rw-rw-   0        0        0    10188 2023-04-10 20:45:12.000000 infinitesimals-0.0.1/__init__.py
--rw-rw-rw-   0        0        0     3282 2023-04-10 20:33:46.000000 infinitesimals-0.0.1/example.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:45:31.449584 infinitesimals-0.0.1/infinitesimals.egg-info/
--rw-rw-rw-   0        0        0      808 2023-04-10 20:45:31.000000 infinitesimals-0.0.1/infinitesimals.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-04-10 20:45:31.000000 infinitesimals-0.0.1/infinitesimals.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 20:45:31.000000 infinitesimals-0.0.1/infinitesimals.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-10 20:45:31.000000 infinitesimals-0.0.1/infinitesimals.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 20:45:31.000000 infinitesimals-0.0.1/infinitesimals.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 20:45:31.452575 infinitesimals-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      906 2023-04-10 20:45:12.000000 infinitesimals-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:45:31.450580 infinitesimals-0.0.1/src/
--rw-rw-rw-   0        0        0    10014 2023-04-10 19:01:36.000000 infinitesimals-0.0.1/src/infinitesimals.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:01:36.725828 infinitesimals-0.0.2/
+-rw-rw-rw-   0        0        0      112 2023-04-10 21:01:14.000000 infinitesimals-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 infinitesimals-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-10 19:18:21.000000 infinitesimals-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      857 2023-04-10 21:01:36.725828 infinitesimals-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      100 2023-04-10 19:05:04.000000 infinitesimals-0.0.2/README.txt
+-rw-rw-rw-   0        0        0    10188 2023-04-10 20:45:12.000000 infinitesimals-0.0.2/__init__.py
+-rw-rw-rw-   0        0        0     3282 2023-04-10 20:33:46.000000 infinitesimals-0.0.2/example.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:01:36.722837 infinitesimals-0.0.2/infinitesimals.egg-info/
+-rw-rw-rw-   0        0        0      857 2023-04-10 21:01:36.000000 infinitesimals-0.0.2/infinitesimals.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-04-10 21:01:36.000000 infinitesimals-0.0.2/infinitesimals.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 21:01:36.000000 infinitesimals-0.0.2/infinitesimals.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-10 21:01:36.000000 infinitesimals-0.0.2/infinitesimals.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 21:01:36.000000 infinitesimals-0.0.2/infinitesimals.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 21:01:36.726825 infinitesimals-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      893 2023-04-10 21:01:19.000000 infinitesimals-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:01:36.723833 infinitesimals-0.0.2/src/
+-rw-rw-rw-   0        0        0    10014 2023-04-10 19:01:36.000000 infinitesimals-0.0.2/src/infinitesimals.py
```

### Comparing `infinitesimals-0.0.1/LICENSE.txt` & `infinitesimals-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `infinitesimals-0.0.1/PKG-INFO` & `infinitesimals-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infinitesimals
-Version: 0.0.1
+Version: 0.0.2
 Summary: A capable HyperReal class and related methods for work with infinitesimals and nonstandard analysis.
 Home-page: 
 Author: Lyam Boylan
 Author-email: lyamboylan@gmail.com
 License: MIT
 Keywords: math,infinitesimal,infinitesimals,hyperreal,analysis,nonstandard analysis
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,12 +13,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
 
 A capable HyperReal class and related methods for work with infinitesimals and nonstandard analysis.
 
 Change Log
-= = =
+===
 
 0.0.1 (10/04/2023)
-- - -
+---
 - First Release
+
+0.0.2 (10/04/2023)
+---
+- Fixed install_requires
```

### Comparing `infinitesimals-0.0.1/__init__.py` & `infinitesimals-0.0.2/__init__.py`

 * *Files identical despite different names*

### Comparing `infinitesimals-0.0.1/example.py` & `infinitesimals-0.0.2/example.py`

 * *Files identical despite different names*

### Comparing `infinitesimals-0.0.1/infinitesimals.egg-info/PKG-INFO` & `infinitesimals-0.0.2/infinitesimals.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infinitesimals
-Version: 0.0.1
+Version: 0.0.2
 Summary: A capable HyperReal class and related methods for work with infinitesimals and nonstandard analysis.
 Home-page: 
 Author: Lyam Boylan
 Author-email: lyamboylan@gmail.com
 License: MIT
 Keywords: math,infinitesimal,infinitesimals,hyperreal,analysis,nonstandard analysis
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,12 +13,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
 
 A capable HyperReal class and related methods for work with infinitesimals and nonstandard analysis.
 
 Change Log
-= = =
+===
 
 0.0.1 (10/04/2023)
-- - -
+---
 - First Release
+
+0.0.2 (10/04/2023)
+---
+- Fixed install_requires
```

### Comparing `infinitesimals-0.0.1/setup.py` & `infinitesimals-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,19 +6,19 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='infinitesimals',
-    version='0.0.1',
+    version='0.0.2',
     description='A capable HyperReal class and related methods for work with infinitesimals and nonstandard analysis.',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Lyam Boylan',
     author_email='lyamboylan@gmail.com',
     license='MIT',
     keywords=['math', 'infinitesimal', 'infinitesimals', 'hyperreal', 'analysis', 'nonstandard analysis'],
     classifiers=classifiers,
     packages=find_packages(),
-    install_requires=['itertools', 'numpy', 'scipy']
+    install_requires=['numpy', 'scipy']
 )
```

### Comparing `infinitesimals-0.0.1/src/infinitesimals.py` & `infinitesimals-0.0.2/src/infinitesimals.py`

 * *Files identical despite different names*


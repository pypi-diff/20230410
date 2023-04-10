# Comparing `tmp/webtypy-0.1.4.tar.gz` & `tmp/webtypy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webtypy-0.1.4.tar", last modified: Sun Apr  9 10:07:25 2023, max compression
+gzip compressed data, was "webtypy-0.1.5.tar", last modified: Mon Apr 10 06:50:57 2023, max compression
```

## Comparing `webtypy-0.1.4.tar` & `webtypy-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-09 10:07:25.116009 webtypy-0.1.4/
--rw-rw-r--   0 simone    (1000) simone    (1000)     1891 2023-04-09 10:07:25.116009 webtypy-0.1.4/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)     1445 2023-04-09 06:17:24.000000 webtypy-0.1.4/README.md
--rw-rw-r--   0 simone    (1000) simone    (1000)       90 2023-04-07 08:23:05.000000 webtypy-0.1.4/pyproject.toml
--rw-rw-r--   0 simone    (1000) simone    (1000)      780 2023-04-09 10:07:25.116009 webtypy-0.1.4/setup.cfg
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-09 10:07:25.116009 webtypy-0.1.4/src/
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-09 10:07:25.116009 webtypy-0.1.4/src/js/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-04-09 07:53:45.000000 webtypy-0.1.4/src/js/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)   536425 2023-04-09 10:06:30.000000 webtypy-0.1.4/src/js/__init__.pyi
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-09 10:07:25.116009 webtypy-0.1.4/src/webtypy.egg-info/
--rw-rw-r--   0 simone    (1000) simone    (1000)     1891 2023-04-09 10:07:25.000000 webtypy-0.1.4/src/webtypy.egg-info/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)      281 2023-04-09 10:07:25.000000 webtypy-0.1.4/src/webtypy.egg-info/SOURCES.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-09 10:07:25.000000 webtypy-0.1.4/src/webtypy.egg-info/dependency_links.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-07 08:59:42.000000 webtypy-0.1.4/src/webtypy.egg-info/not-zip-safe
--rw-rw-r--   0 simone    (1000) simone    (1000)       53 2023-04-09 10:07:25.000000 webtypy-0.1.4/src/webtypy.egg-info/requires.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        3 2023-04-09 10:07:25.000000 webtypy-0.1.4/src/webtypy.egg-info/top_level.txt
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-10 06:50:57.738555 webtypy-0.1.5/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1891 2023-04-10 06:50:57.738555 webtypy-0.1.5/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1445 2023-04-09 06:17:24.000000 webtypy-0.1.5/README.md
+-rw-rw-r--   0 simone    (1000) simone    (1000)       90 2023-04-07 08:23:05.000000 webtypy-0.1.5/pyproject.toml
+-rw-rw-r--   0 simone    (1000) simone    (1000)      783 2023-04-10 06:50:57.738555 webtypy-0.1.5/setup.cfg
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-10 06:50:57.738555 webtypy-0.1.5/src/
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-10 06:50:57.738555 webtypy-0.1.5/src/js-stubs/
+-rw-rw-r--   0 simone    (1000) simone    (1000)   536425 2023-04-09 10:06:30.000000 webtypy-0.1.5/src/js-stubs/__init__.pyi
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-04-10 06:50:57.738555 webtypy-0.1.5/src/webtypy.egg-info/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1891 2023-04-10 06:50:57.000000 webtypy-0.1.5/src/webtypy.egg-info/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)      268 2023-04-10 06:50:57.000000 webtypy-0.1.5/src/webtypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-10 06:50:57.000000 webtypy-0.1.5/src/webtypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-07 08:59:42.000000 webtypy-0.1.5/src/webtypy.egg-info/not-zip-safe
+-rw-rw-r--   0 simone    (1000) simone    (1000)       53 2023-04-10 06:50:57.000000 webtypy-0.1.5/src/webtypy.egg-info/requires.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        9 2023-04-10 06:50:57.000000 webtypy-0.1.5/src/webtypy.egg-info/top_level.txt
```

### Comparing `webtypy-0.1.4/PKG-INFO` & `webtypy-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webtypy
-Version: 0.1.4
+Version: 0.1.5
 Summary: This module contains the DOM types for the majority of the web APIs used in a web browser. These can be used by an IDE to give type hinting and completion during the development using DOM apis.
 Home-page: https://github.com/pyodide/webtypy
 Author: Simone Giacomelli
 Author-email: simone.giacomelli@gmail.com
 License: MPL 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `webtypy-0.1.4/README.md` & `webtypy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `webtypy-0.1.4/setup.cfg` & `webtypy-0.1.5/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = webtypy
 url = https://github.com/pyodide/webtypy
-version = 0.1.4
+version = 0.1.5
 license = MPL 2.0
 license_files = LICENCE
 description = This module contains the DOM types for the majority of the web APIs used in a web browser. These can be used by an IDE to give type hinting and completion during the development using DOM apis.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Simone Giacomelli
 author_email = simone.giacomelli@gmail.com
@@ -15,15 +15,15 @@
 	build==0.6.0.post1
 	twine==3.4.2
 	wheel==0.37.0
 
 [options]
 package_dir = 
 	=src
-packages = find:
+packages = js-stubs
 zip_safe = False
 include_package_data = True
 
 [options.package_data]
 * = py.typed, *.pyi
 
 [options.packages.find]
```

### Comparing `webtypy-0.1.4/src/js/__init__.pyi` & `webtypy-0.1.5/src/js-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `webtypy-0.1.4/src/webtypy.egg-info/PKG-INFO` & `webtypy-0.1.5/src/webtypy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webtypy
-Version: 0.1.4
+Version: 0.1.5
 Summary: This module contains the DOM types for the majority of the web APIs used in a web browser. These can be used by an IDE to give type hinting and completion during the development using DOM apis.
 Home-page: https://github.com/pyodide/webtypy
 Author: Simone Giacomelli
 Author-email: simone.giacomelli@gmail.com
 License: MPL 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```


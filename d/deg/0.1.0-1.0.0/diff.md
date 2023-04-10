# Comparing `tmp/deg-0.1.0.tar.gz` & `tmp/deg-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deg-0.1.0.tar", last modified: Wed Mar 29 03:27:07 2023, max compression
+gzip compressed data, was "deg-1.0.0.tar", last modified: Mon Apr 10 10:45:01 2023, max compression
```

## Comparing `deg-0.1.0.tar` & `deg-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-29 03:27:07.410861 deg-0.1.0/
--rwxrwxrwx   0 root         (0) root         (0)    11350 2023-03-29 03:10:59.000000 deg-0.1.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)    13470 2023-03-29 03:27:07.411145 deg-0.1.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       72 2023-03-29 01:50:59.000000 deg-0.1.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-29 03:27:07.386922 deg-0.1.0/deg/
--rwxrwxrwx   0 root         (0) root         (0)     3898 2023-03-29 03:07:21.000000 deg-0.1.0/deg/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-29 03:27:07.410439 deg-0.1.0/deg.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)    13470 2023-03-29 03:27:07.000000 deg-0.1.0/deg.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      208 2023-03-29 03:27:07.000000 deg-0.1.0/deg.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-03-29 03:27:07.000000 deg-0.1.0/deg.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       20 2023-03-29 03:27:07.000000 deg-0.1.0/deg.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        4 2023-03-29 03:27:07.000000 deg-0.1.0/deg.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-03-29 03:27:07.000000 deg-0.1.0/deg.egg-info/zip-safe
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-03-29 03:27:07.411595 deg-0.1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1211 2023-03-29 03:26:13.000000 deg-0.1.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 10:45:01.117124 deg-1.0.0/
+-rwxrwxrwx   0 root         (0) root         (0)    11350 2023-03-29 03:10:59.000000 deg-1.0.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)    13470 2023-04-10 10:45:01.117539 deg-1.0.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       72 2023-03-29 01:50:59.000000 deg-1.0.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 10:45:01.113948 deg-1.0.0/deg/
+-rwxrwxrwx   0 root         (0) root         (0)     5172 2023-04-10 10:43:25.000000 deg-1.0.0/deg/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 10:45:01.116777 deg-1.0.0/deg.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)    13470 2023-04-10 10:45:00.000000 deg-1.0.0/deg.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      208 2023-04-10 10:45:01.000000 deg-1.0.0/deg.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-10 10:45:00.000000 deg-1.0.0/deg.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       20 2023-04-10 10:45:00.000000 deg-1.0.0/deg.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        4 2023-04-10 10:45:00.000000 deg-1.0.0/deg.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-10 10:45:00.000000 deg-1.0.0/deg.egg-info/zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-10 10:45:01.118024 deg-1.0.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1211 2023-04-10 10:44:57.000000 deg-1.0.0/setup.py
```

### Comparing `deg-0.1.0/LICENSE` & `deg-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deg-0.1.0/PKG-INFO` & `deg-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deg
-Version: 0.1.0
+Version: 1.0.0
 Summary: A Graph library to manage inheritance rules
 Home-page: https://github.com/supratikchatterjee16/deg
 Author: Supratik Chatterjee
 Author-email: supratikdevm96@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `deg-0.1.0/deg.egg-info/PKG-INFO` & `deg-1.0.0/deg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deg
-Version: 0.1.0
+Version: 1.0.0
 Summary: A Graph library to manage inheritance rules
 Home-page: https://github.com/supratikchatterjee16/deg
 Author: Supratik Chatterjee
 Author-email: supratikdevm96@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `deg-0.1.0/setup.py` & `deg-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 requirements_noversion = [
 	'networkx',
     'matplotlib'
 ]
 setup(
 	# Meta information
 	name				= 'deg',
-	version				= '0.1.0',
+	version				= '1.0.0',
 	author				= 'Supratik Chatterjee',
 	author_email			= 'supratikdevm96@gmail.com',
 	url				= 'https://github.com/supratikchatterjee16/deg',
 	description			= 'A Graph library to manage inheritance rules',
 	keywords			= ['graph', 'visualize', 'dependency', 'inheritance'],
 	install_requires		= requirements_noversion,
 	# build information
```


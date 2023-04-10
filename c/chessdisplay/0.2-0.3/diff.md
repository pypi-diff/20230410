# Comparing `tmp/chessdisplay-0.2.tar.gz` & `tmp/chessdisplay-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chessdisplay-0.2.tar", last modified: Mon Apr 10 20:49:39 2023, max compression
+gzip compressed data, was "chessdisplay-0.3.tar", last modified: Mon Apr 10 20:57:49 2023, max compression
```

## Comparing `chessdisplay-0.2.tar` & `chessdisplay-0.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 20:49:39.827741 chessdisplay-0.2/
--rw-rw-rw-   0        0        0    35821 2023-04-10 20:26:00.000000 chessdisplay-0.2/LICENSE
--rw-rw-rw-   0        0        0     1093 2023-04-10 20:49:39.827741 chessdisplay-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-04-10 20:29:31.000000 chessdisplay-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 20:49:39.794719 chessdisplay-0.2/chessdisplay/
--rw-rw-rw-   0        0        0       27 2023-04-10 19:20:49.000000 chessdisplay-0.2/chessdisplay/__init__.py
--rw-rw-rw-   0        0        0     7774 2023-04-10 20:14:42.000000 chessdisplay-0.2/chessdisplay/display.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:49:39.825739 chessdisplay-0.2/chessdisplay.egg-info/
--rw-rw-rw-   0        0        0     1093 2023-04-10 20:49:39.000000 chessdisplay-0.2/chessdisplay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-04-10 20:49:39.000000 chessdisplay-0.2/chessdisplay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 20:49:39.000000 chessdisplay-0.2/chessdisplay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 20:49:39.000000 chessdisplay-0.2/chessdisplay.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 20:49:39.000000 chessdisplay-0.2/chessdisplay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      139 2023-04-10 20:49:39.834745 chessdisplay-0.2/setup.cfg
--rw-rw-rw-   0        0        0      894 2023-04-10 20:49:24.000000 chessdisplay-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:57:49.479628 chessdisplay-0.3/
+-rw-rw-rw-   0        0        0    35821 2023-04-10 20:26:00.000000 chessdisplay-0.3/LICENSE
+-rw-rw-rw-   0        0        0     1093 2023-04-10 20:57:49.479628 chessdisplay-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-04-10 20:29:31.000000 chessdisplay-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 20:57:49.460399 chessdisplay-0.3/chessdisplay/
+-rw-rw-rw-   0        0        0     7774 2023-04-10 20:55:23.000000 chessdisplay-0.3/chessdisplay/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:57:49.478410 chessdisplay-0.3/chessdisplay.egg-info/
+-rw-rw-rw-   0        0        0     1093 2023-04-10 20:57:49.000000 chessdisplay-0.3/chessdisplay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-04-10 20:57:49.000000 chessdisplay-0.3/chessdisplay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 20:57:49.000000 chessdisplay-0.3/chessdisplay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 20:57:49.000000 chessdisplay-0.3/chessdisplay.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 20:57:49.000000 chessdisplay-0.3/chessdisplay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      139 2023-04-10 20:57:49.486632 chessdisplay-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      894 2023-04-10 20:57:23.000000 chessdisplay-0.3/setup.py
```

### Comparing `chessdisplay-0.2/LICENSE` & `chessdisplay-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chessdisplay-0.2/PKG-INFO` & `chessdisplay-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chessdisplay
-Version: 0.2
+Version: 0.3
 Summary: A fully customizable chess board.
 Home-page: https://github.com/emanuelVINI01/chessdisplay
 Author: emanuel
 Author-email: emanueltdcsd@gmail.com
 License: UNKNOWN
 Description: # chessdisplay
```

### Comparing `chessdisplay-0.2/chessdisplay/display.py` & `chessdisplay-0.3/chessdisplay/__init__.py`

 * *Files identical despite different names*

### Comparing `chessdisplay-0.2/chessdisplay.egg-info/PKG-INFO` & `chessdisplay-0.3/chessdisplay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chessdisplay
-Version: 0.2
+Version: 0.3
 Summary: A fully customizable chess board.
 Home-page: https://github.com/emanuelVINI01/chessdisplay
 Author: emanuel
 Author-email: emanueltdcsd@gmail.com
 License: UNKNOWN
 Description: # chessdisplay
```

### Comparing `chessdisplay-0.2/setup.py` & `chessdisplay-0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 from setuptools import setup
 
 setup(
   name = 'chessdisplay',        
   packages = ['chessdisplay'], 
-  version = '0.2',           
+  version = '0.3',           
   description = 'A fully customizable chess board.',  
   long_description=long_description,
   long_description_content_type='text/markdown', 
   author = 'emanuel',                   
   author_email = 'emanueltdcsd@gmail.com',      
   url = 'https://github.com/emanuelVINI01/chessdisplay',   
   keywords = ['chess', 'chessdisplay', 'chessboard', 'pygamechess'],
```


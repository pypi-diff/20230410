# Comparing `tmp/epubcrush-2.0.1.tar.gz` & `tmp/epubcrush-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epubcrush-2.0.1.tar", last modified: Fri Feb 17 03:12:27 2023, max compression
+gzip compressed data, was "epubcrush-2.0.2.tar", last modified: Sun Apr  9 22:09:03 2023, max compression
```

## Comparing `epubcrush-2.0.1.tar` & `epubcrush-2.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-02-17 03:12:27.755822 epubcrush-2.0.1/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     2827 2023-02-17 03:12:27.755822 epubcrush-2.0.1/PKG-INFO
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-02-17 03:12:27.755822 epubcrush-2.0.1/epubcrush/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       59 2022-11-20 10:14:49.000000 epubcrush-2.0.1/epubcrush/__init__.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7737 2023-02-17 03:11:04.000000 epubcrush-2.0.1/epubcrush/epubcrush.py
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-02-17 03:12:27.755822 epubcrush-2.0.1/epubcrush.egg-info/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     2827 2023-02-17 03:12:27.000000 epubcrush-2.0.1/epubcrush.egg-info/PKG-INFO
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      221 2023-02-17 03:12:27.000000 epubcrush-2.0.1/epubcrush.egg-info/SOURCES.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-02-17 03:12:27.000000 epubcrush-2.0.1/epubcrush.egg-info/dependency_links.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       46 2023-02-17 03:12:27.000000 epubcrush-2.0.1/epubcrush.egg-info/entry_points.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       10 2023-02-17 03:12:27.000000 epubcrush-2.0.1/epubcrush.egg-info/top_level.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-02-17 03:12:27.755822 epubcrush-2.0.1/setup.cfg
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      761 2023-02-17 03:11:59.000000 epubcrush-2.0.1/setup.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-04-09 22:09:03.625120 epubcrush-2.0.2/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     2827 2023-04-09 22:09:03.625120 epubcrush-2.0.2/PKG-INFO
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-04-09 22:09:03.621120 epubcrush-2.0.2/epubcrush/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       59 2022-11-20 10:14:49.000000 epubcrush-2.0.2/epubcrush/__init__.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7560 2023-04-09 22:06:42.000000 epubcrush-2.0.2/epubcrush/epubcrush.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-04-09 22:09:03.625120 epubcrush-2.0.2/epubcrush.egg-info/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     2827 2023-04-09 22:09:03.000000 epubcrush-2.0.2/epubcrush.egg-info/PKG-INFO
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      221 2023-04-09 22:09:03.000000 epubcrush-2.0.2/epubcrush.egg-info/SOURCES.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-04-09 22:09:03.000000 epubcrush-2.0.2/epubcrush.egg-info/dependency_links.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       46 2023-04-09 22:09:03.000000 epubcrush-2.0.2/epubcrush.egg-info/entry_points.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       10 2023-04-09 22:09:03.000000 epubcrush-2.0.2/epubcrush.egg-info/top_level.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-04-09 22:09:03.625120 epubcrush-2.0.2/setup.cfg
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      761 2023-04-09 21:46:05.000000 epubcrush-2.0.2/setup.py
```

### Comparing `epubcrush-2.0.1/PKG-INFO` & `epubcrush-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epubcrush
-Version: 2.0.1
+Version: 2.0.2
 Summary: Compress EPUB files
 Home-page: https://github.com/jncraton/epubcrush
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: EPUB Crush
         ==========
```

### Comparing `epubcrush-2.0.1/epubcrush/epubcrush.py` & `epubcrush-2.0.2/epubcrush/epubcrush.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     >>> clean_xml('<html><svg></svg></html>')
     '<html xmlns="http://www.w3.org/1999/xhtml"></html>'
 
     >>> clean_xml('<html><p class="a">test</p></html>')
     '<html xmlns="http://www.w3.org/1999/xhtml"><p>test</p></html>'
 
     >>> clean_xml('<html><img src="" alt="test"/></html>')
-    '<html xmlns="http://www.w3.org/1999/xhtml"><p>test</p></html>'
+    '<html xmlns="http://www.w3.org/1999/xhtml"></html>'
 
     >>> clean_xml('<html><img src="" alt="Image"/></html>')
     '<html xmlns="http://www.w3.org/1999/xhtml"></html>'
 
     >>> clean_xml('<html><img src="" alt=""/></html>')
     '<html xmlns="http://www.w3.org/1999/xhtml"></html>'
 
@@ -175,18 +175,14 @@
         exclude_tags=exclude_tags,
         exclude_attrs=exclude_attrs,
     )
     # Ensure correct namespace definition
     xml = re.sub(r"<html", '<html xmlns="http://www.w3.org/1999/xhtml"', xml)
 
     if not images:
-        # Replace images with their alt text
-        xml = re.sub(
-            r'<img.* alt="(?!image)([^"]+?)".*></img>', r"<p>\g<1></p>", xml, flags=re.I
-        )
         xml = re.sub(r"<img.*>.*?</img>", "", xml)
 
     return xml
 
 
 def repack(filename: str) -> None:
     run(["advzip", "-z", "-4", filename])
```

### Comparing `epubcrush-2.0.1/epubcrush.egg-info/PKG-INFO` & `epubcrush-2.0.2/epubcrush.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epubcrush
-Version: 2.0.1
+Version: 2.0.2
 Summary: Compress EPUB files
 Home-page: https://github.com/jncraton/epubcrush
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: EPUB Crush
         ==========
```

### Comparing `epubcrush-2.0.1/setup.py` & `epubcrush-2.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="epubcrush",
-    version="2.0.1",
+    version="2.0.2",
     author="Jon Craton",
     author_email="jon@joncraton.com",
     description="Compress EPUB files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jncraton/epubcrush",
     packages=setuptools.find_packages(),
```


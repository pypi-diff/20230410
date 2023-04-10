# Comparing `tmp/epubcrush-2.0.2.tar.gz` & `tmp/epubcrush-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epubcrush-2.0.2.tar", last modified: Sun Apr  9 22:09:03 2023, max compression
+gzip compressed data, was "epubcrush-2.0.3.tar", last modified: Mon Apr 10 02:18:42 2023, max compression
```

## Comparing `epubcrush-2.0.2.tar` & `epubcrush-2.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-04-09 22:09:03.625120 epubcrush-2.0.2/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     2827 2023-04-09 22:09:03.625120 epubcrush-2.0.2/PKG-INFO
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-04-09 22:09:03.621120 epubcrush-2.0.2/epubcrush/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       59 2022-11-20 10:14:49.000000 epubcrush-2.0.2/epubcrush/__init__.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7560 2023-04-09 22:06:42.000000 epubcrush-2.0.2/epubcrush/epubcrush.py
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-04-09 22:09:03.625120 epubcrush-2.0.2/epubcrush.egg-info/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     2827 2023-04-09 22:09:03.000000 epubcrush-2.0.2/epubcrush.egg-info/PKG-INFO
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      221 2023-04-09 22:09:03.000000 epubcrush-2.0.2/epubcrush.egg-info/SOURCES.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-04-09 22:09:03.000000 epubcrush-2.0.2/epubcrush.egg-info/dependency_links.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       46 2023-04-09 22:09:03.000000 epubcrush-2.0.2/epubcrush.egg-info/entry_points.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       10 2023-04-09 22:09:03.000000 epubcrush-2.0.2/epubcrush.egg-info/top_level.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-04-09 22:09:03.625120 epubcrush-2.0.2/setup.cfg
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      761 2023-04-09 21:46:05.000000 epubcrush-2.0.2/setup.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-04-10 02:18:42.682225 epubcrush-2.0.3/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     2827 2023-04-10 02:18:42.682225 epubcrush-2.0.3/PKG-INFO
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-04-10 02:18:42.682225 epubcrush-2.0.3/epubcrush/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       59 2022-11-20 10:14:49.000000 epubcrush-2.0.3/epubcrush/__init__.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     9445 2023-04-10 02:16:55.000000 epubcrush-2.0.3/epubcrush/epubcrush.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-04-10 02:18:42.682225 epubcrush-2.0.3/epubcrush.egg-info/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     2827 2023-04-10 02:18:42.000000 epubcrush-2.0.3/epubcrush.egg-info/PKG-INFO
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      221 2023-04-10 02:18:42.000000 epubcrush-2.0.3/epubcrush.egg-info/SOURCES.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-04-10 02:18:42.000000 epubcrush-2.0.3/epubcrush.egg-info/dependency_links.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       46 2023-04-10 02:18:42.000000 epubcrush-2.0.3/epubcrush.egg-info/entry_points.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       10 2023-04-10 02:18:42.000000 epubcrush-2.0.3/epubcrush.egg-info/top_level.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-04-10 02:18:42.686225 epubcrush-2.0.3/setup.cfg
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      761 2023-04-10 02:17:28.000000 epubcrush-2.0.3/setup.py
```

### Comparing `epubcrush-2.0.2/PKG-INFO` & `epubcrush-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epubcrush
-Version: 2.0.2
+Version: 2.0.3
 Summary: Compress EPUB files
 Home-page: https://github.com/jncraton/epubcrush
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: EPUB Crush
         ==========
```

### Comparing `epubcrush-2.0.2/epubcrush/epubcrush.py` & `epubcrush-2.0.3/epubcrush/epubcrush.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,68 @@
 from subprocess import run
 import re
 from xml.etree import ElementTree
 import argparse
 import os
 
 
+def modernize_childrens(text):
+    """
+    >>> modernize_childrens("You are queer.")
+    'You are strange.'
+    >>> modernize_childrens("I am a queer boy.")
+    'I am a strange boy.'
+    >>> modernize_childrens("She was feeling gay.")
+    'She was feeling happy.'
+    >>> modernize_childrens("Gay children played.")
+    'Happy children played.'
+    >>> modernize_childrens("Children played, gaily!")
+    'Children played, happily!'
+    >>> modernize_childrens("Queerer things have happened.")
+    'Stranger things have happened.'
+    >>> modernize_childrens("We could do with a bit more queerness.")
+    'We could do with a bit more strangeness.'
+    """
+
+    word_updates = [
+        ("queer", "strange"),
+        ("queerer", "stranger"),
+        ("queerest", "strangest"),
+        ("queerness", "strangeness"),
+        ("gaily", "happily"),
+        ("gay", "happy"),
+        ("midget", "little person"),
+        ("policeman", "police officer"),
+        ("policemen", "police officers"),
+        ("mailman", "mail carrier"),
+        ("mailmen", "mail carriers"),
+        ("fireman", "fire fighter"),
+        ("firemen", "fire fighters"),
+    ]
+
+    tokens = []
+
+    def modernize_token(token):
+        for orig, new in word_updates:
+            if token == orig:
+                token = new
+            elif token == orig.title():
+                token = new.title()
+            elif token == orig.upper():
+                token = new.upper()
+
+        return token
+
+    tokens = [modernize_token(t) for t in re.findall(r"([\w]+|[^\w]+)", text)]
+
+    return "".join(tokens)
+
+
 def crush_epub(
-    filename: str, images=False, quality=100, styles=False, fonts=False
+    filename: str, images=False, quality=100, styles=False, fonts=False, modernize=False
 ) -> None:
     allowed_files = [
         "mimetype",
         "ncx",
         "opf",
         "xml",
         "xhtml",
@@ -38,14 +90,17 @@
             for file in epub.namelist():
                 if re.match(file_allow, file, flags=re.I):
                     if file.endswith("html") or file.endswith("htm"):
                         xml = epub.open(file).read().decode("utf8")
 
                         xml = clean_xml(xml, images, styles)
 
+                        if modernize:
+                            xml = modernize_childrens(xml)
+
                         newepub.writestr(file, xml)
                     elif file.endswith("opf"):
                         xml = epub.open(file).read().decode("utf8")
 
                         xml = ElementTree.canonicalize(xml)
 
                         xml = re.sub(
@@ -165,15 +220,15 @@
 
     if not styles:
         exclude_tags += ["style", "link"]
         exclude_attrs += ["style", "class"]
 
     # Remove the default namespace definition
     xml = re.sub(r'\sxmlns="[^"]+"', "", xml, count=1)
-    xml = xml.replace('&nbsp;', ' ')
+    xml = xml.replace("&nbsp;", " ")
     xml = ElementTree.canonicalize(
         xml,
         exclude_tags=exclude_tags,
         exclude_attrs=exclude_attrs,
     )
     # Ensure correct namespace definition
     xml = re.sub(r"<html", '<html xmlns="http://www.w3.org/1999/xhtml"', xml)
@@ -193,14 +248,19 @@
     ap.add_argument("files", nargs="+", help="List of EPUB files")
     ap.add_argument(
         "--fast",
         action="store_true",
         help="Run faster. Do not recompress using advcomp",
     )
     ap.add_argument(
+        "--modernize",
+        action="store_true",
+        help="Attempt to modernize language of older children's literature",
+    )
+    ap.add_argument(
         "--images",
         "-i",
         action="store_true",
         help="Keep images in output",
     )
     ap.add_argument(
         "--styles",
@@ -227,14 +287,15 @@
     for filename in args.files:
         crush_epub(
             filename,
             images=args.images,
             styles=args.styles,
             quality=args.quality,
             fonts=args.fonts,
+            modernize=args.modernize,
         )
         if not args.fast:
             repack(filename)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `epubcrush-2.0.2/epubcrush.egg-info/PKG-INFO` & `epubcrush-2.0.3/epubcrush.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epubcrush
-Version: 2.0.2
+Version: 2.0.3
 Summary: Compress EPUB files
 Home-page: https://github.com/jncraton/epubcrush
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: EPUB Crush
         ==========
```

### Comparing `epubcrush-2.0.2/setup.py` & `epubcrush-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="epubcrush",
-    version="2.0.2",
+    version="2.0.3",
     author="Jon Craton",
     author_email="jon@joncraton.com",
     description="Compress EPUB files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jncraton/epubcrush",
     packages=setuptools.find_packages(),
```


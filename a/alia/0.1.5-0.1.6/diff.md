# Comparing `tmp/alia-0.1.5.tar.gz` & `tmp/alia-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alia-0.1.5.tar", last modified: Wed Apr  5 19:26:17 2023, max compression
+gzip compressed data, was "alia-0.1.6.tar", last modified: Mon Apr 10 19:00:52 2023, max compression
```

## Comparing `alia-0.1.5.tar` & `alia-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-05 19:26:17.787201 alia-0.1.5/
--rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.1.5/LICENSE
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-05 19:26:17.786863 alia-0.1.5/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 19:00:09.000000 alia-0.1.5/README.md
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-05 19:26:17.783195 alia-0.1.5/alia/
--rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.1.5/alia/__init__.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    14246 2023-03-23 19:42:40.000000 alia-0.1.5/alia/colors.py
--rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.1.5/alia/df_tools.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    24521 2023-03-24 19:01:25.000000 alia-0.1.5/alia/tools.py
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-05 19:26:17.786449 alia-0.1.5/alia.egg-info/
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-05 19:26:17.000000 alia-0.1.5/alia.egg-info/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-04-05 19:26:17.000000 alia-0.1.5/alia.egg-info/SOURCES.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-04-05 19:26:17.000000 alia-0.1.5/alia.egg-info/dependency_links.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       74 2023-04-05 19:26:17.000000 alia-0.1.5/alia.egg-info/requires.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-04-05 19:26:17.000000 alia-0.1.5/alia.egg-info/top_level.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-04-05 19:26:17.787338 alia-0.1.5/setup.cfg
--rw-r--r--   0 aliavictor   (502) staff       (20)      884 2023-04-05 19:22:56.000000 alia-0.1.5/setup.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-10 19:00:52.189440 alia-0.1.6/
+-rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.1.6/LICENSE
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-10 19:00:52.188971 alia-0.1.6/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 19:00:09.000000 alia-0.1.6/README.md
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-10 19:00:52.186562 alia-0.1.6/alia/
+-rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.1.6/alia/__init__.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    14246 2023-03-23 19:42:40.000000 alia-0.1.6/alia/colors.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.1.6/alia/df_tools.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    24886 2023-04-10 19:00:16.000000 alia-0.1.6/alia/tools.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-10 19:00:52.188545 alia-0.1.6/alia.egg-info/
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-10 19:00:52.000000 alia-0.1.6/alia.egg-info/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-04-10 19:00:52.000000 alia-0.1.6/alia.egg-info/SOURCES.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-04-10 19:00:52.000000 alia-0.1.6/alia.egg-info/dependency_links.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       74 2023-04-10 19:00:52.000000 alia-0.1.6/alia.egg-info/requires.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-04-10 19:00:52.000000 alia-0.1.6/alia.egg-info/top_level.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-04-10 19:00:52.189572 alia-0.1.6/setup.cfg
+-rw-r--r--   0 aliavictor   (502) staff       (20)      884 2023-04-10 19:00:43.000000 alia-0.1.6/setup.py
```

### Comparing `alia-0.1.5/LICENSE` & `alia-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alia-0.1.5/PKG-INFO` & `alia-0.1.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alia
-Version: 0.1.5
+Version: 0.1.6
 Summary: A collection of random helper tools to make life easier
 Home-page: https://github.com/aliavictor/alia
 Author: Alia
 Author-email: alia.jo.victor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alia-0.1.5/alia/colors.py` & `alia-0.1.6/alia/colors.py`

 * *Files identical despite different names*

### Comparing `alia-0.1.5/alia/df_tools.py` & `alia-0.1.6/alia/df_tools.py`

 * *Files identical despite different names*

### Comparing `alia-0.1.5/alia/tools.py` & `alia-0.1.6/alia/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -456,14 +456,30 @@
         A string of the output of the passed regex."""
     if type(pattern) == str:
         return re.search(pattern, string).group(1)
     else:
         return pattern.search(string).group(1)
 
 
+def str_dedupe(txt):
+    """Removes duplicate substrings from a string.
+
+    Args:
+        txt (str): String to dedupe
+
+    Returns:
+        A string with unique substrings."""
+    words = txt.strip().split()
+    unique_words = []
+    for word in words:
+        if word not in unique_words:
+            unique_words.append(word)
+
+    return " ".join(unique_words)
+
 def str_remove(txt, rplc_strs):
     """Removes passed strings from a string.
 
     Args:
         txt (str): String to clean
         rplc_strs (list): Strings to remove from the passed txt string
```

### Comparing `alia-0.1.5/alia.egg-info/PKG-INFO` & `alia-0.1.6/alia.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alia
-Version: 0.1.5
+Version: 0.1.6
 Summary: A collection of random helper tools to make life easier
 Home-page: https://github.com/aliavictor/alia
 Author: Alia
 Author-email: alia.jo.victor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alia-0.1.5/setup.py` & `alia-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="alia",
-    version="0.1.5",
+    version="0.1.6",
     description="A collection of random helper tools to make life easier",
     author="Alia",
     author_email="alia.jo.victor@gmail.com",
     url="https://github.com/aliavictor/alia",
     packages=find_packages(),
     install_requires=[
         # i.e. 'numpy>=1.18.0'
```


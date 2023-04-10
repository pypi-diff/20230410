# Comparing `tmp/B0tHe1Per_test_api-0.2.tar.gz` & `tmp/B0tHe1Per_test_api-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "B0tHe1Per_test_api-0.2.tar", last modified: Mon Apr 10 11:42:58 2023, max compression
+gzip compressed data, was "B0tHe1Per_test_api-0.3.tar", last modified: Mon Apr 10 12:24:40 2023, max compression
```

## Comparing `B0tHe1Per_test_api-0.2.tar` & `B0tHe1Per_test_api-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 11:42:58.247443 B0tHe1Per_test_api-0.2/
-drwxrwxrwx   0        0        0        0 2023-04-10 11:42:58.191509 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/
--rw-rw-rw-   0        0        0      396 2023-03-24 20:35:35.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/__init__.py
--rw-rw-rw-   0        0        0     5001 2023-03-21 21:40:18.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/address_book.py
--rw-rw-rw-   0        0        0     6057 2023-03-24 21:42:15.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/bot_interface.py
--rw-rw-rw-   0        0        0     3726 2023-03-21 21:40:18.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/file_sorter.py
--rw-rw-rw-   0        0        0     2390 2023-03-21 21:40:19.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/notes_classes.py
--rw-rw-rw-   0        0        0     2777 2023-03-21 21:40:19.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/notes_main.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:42:58.244402 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api.egg-info/
--rw-rw-rw-   0        0        0      208 2023-04-10 11:42:56.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      436 2023-04-10 11:42:57.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 11:42:56.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-04-10 11:42:56.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-04-10 11:42:56.000000 B0tHe1Per_test_api-0.2/B0tHe1Per_test_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      208 2023-04-10 11:42:58.248391 B0tHe1Per_test_api-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-04-10 11:42:58.252375 B0tHe1Per_test_api-0.2/setup.cfg
--rw-rw-rw-   0        0        0      468 2023-04-10 11:39:30.000000 B0tHe1Per_test_api-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:24:40.741814 B0tHe1Per_test_api-0.3/
+drwxrwxrwx   0        0        0        0 2023-04-10 12:24:40.717973 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/
+-rw-rw-rw-   0        0        0      396 2023-03-24 20:35:35.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/__init__.py
+-rw-rw-rw-   0        0        0     5001 2023-03-21 21:40:18.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/address_book.py
+-rw-rw-rw-   0        0        0     6076 2023-04-10 12:17:10.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/bot_interface.py
+-rw-rw-rw-   0        0        0     3726 2023-03-21 21:40:18.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/file_sorter.py
+-rw-rw-rw-   0        0        0     2390 2023-03-21 21:40:19.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/notes_classes.py
+-rw-rw-rw-   0        0        0     2777 2023-03-21 21:40:19.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/notes_main.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:24:40.738833 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api.egg-info/
+-rw-rw-rw-   0        0        0      208 2023-04-10 12:24:40.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      436 2023-04-10 12:24:40.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 12:24:40.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-04-10 12:24:40.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-10 12:24:40.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      208 2023-04-10 12:24:40.742806 B0tHe1Per_test_api-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-04-10 12:24:40.745786 B0tHe1Per_test_api-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      562 2023-04-10 12:24:23.000000 B0tHe1Per_test_api-0.3/setup.py
```

### Comparing `B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/address_book.py` & `B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/address_book.py`

 * *Files identical despite different names*

### Comparing `B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/bot_interface.py` & `B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/bot_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import tkinter as tk
-from file_sorter import FileSorter
+from B0tHe1Per_test_api.file_sorter import FileSorter
 import subprocess
 
 current_process = None
 
 class BotInterface:
     def __init__(self):
         self.root = tk.Tk()
```

### Comparing `B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/file_sorter.py` & `B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/file_sorter.py`

 * *Files identical despite different names*

### Comparing `B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/notes_classes.py` & `B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/notes_classes.py`

 * *Files identical despite different names*

### Comparing `B0tHe1Per_test_api-0.2/B0tHe1Per_test_api/notes_main.py` & `B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/notes_main.py`

 * *Files identical despite different names*


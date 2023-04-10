# Comparing `tmp/B0tHe1Per_test_api-0.3.tar.gz` & `tmp/B0tHe1Per_test_api-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "B0tHe1Per_test_api-0.3.tar", last modified: Mon Apr 10 12:24:40 2023, max compression
+gzip compressed data, was "B0tHe1Per_test_api-0.4.tar", last modified: Mon Apr 10 12:36:28 2023, max compression
```

## Comparing `B0tHe1Per_test_api-0.3.tar` & `B0tHe1Per_test_api-0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 12:24:40.741814 B0tHe1Per_test_api-0.3/
-drwxrwxrwx   0        0        0        0 2023-04-10 12:24:40.717973 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/
--rw-rw-rw-   0        0        0      396 2023-03-24 20:35:35.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/__init__.py
--rw-rw-rw-   0        0        0     5001 2023-03-21 21:40:18.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/address_book.py
--rw-rw-rw-   0        0        0     6076 2023-04-10 12:17:10.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/bot_interface.py
--rw-rw-rw-   0        0        0     3726 2023-03-21 21:40:18.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/file_sorter.py
--rw-rw-rw-   0        0        0     2390 2023-03-21 21:40:19.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/notes_classes.py
--rw-rw-rw-   0        0        0     2777 2023-03-21 21:40:19.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/notes_main.py
-drwxrwxrwx   0        0        0        0 2023-04-10 12:24:40.738833 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api.egg-info/
--rw-rw-rw-   0        0        0      208 2023-04-10 12:24:40.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      436 2023-04-10 12:24:40.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 12:24:40.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-04-10 12:24:40.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-04-10 12:24:40.000000 B0tHe1Per_test_api-0.3/B0tHe1Per_test_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      208 2023-04-10 12:24:40.742806 B0tHe1Per_test_api-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-04-10 12:24:40.745786 B0tHe1Per_test_api-0.3/setup.cfg
--rw-rw-rw-   0        0        0      562 2023-04-10 12:24:23.000000 B0tHe1Per_test_api-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:36:28.431802 B0tHe1Per_test_api-0.4/
+drwxrwxrwx   0        0        0        0 2023-04-10 12:36:28.362698 B0tHe1Per_test_api-0.4/B0tHe1Per_test_api/
+-rw-rw-rw-   0        0        0      396 2023-03-24 20:35:35.000000 B0tHe1Per_test_api-0.4/B0tHe1Per_test_api/__init__.py
+-rw-rw-rw-   0        0        0     5001 2023-03-21 21:40:18.000000 B0tHe1Per_test_api-0.4/B0tHe1Per_test_api/address_book.py
+-rw-rw-rw-   0        0        0     6076 2023-04-10 12:17:10.000000 B0tHe1Per_test_api-0.4/B0tHe1Per_test_api/bot_interface.py
+-rw-rw-rw-   0        0        0     3726 2023-03-21 21:40:18.000000 B0tHe1Per_test_api-0.4/B0tHe1Per_test_api/file_sorter.py
+-rw-rw-rw-   0        0        0     2390 2023-03-21 21:40:19.000000 B0tHe1Per_test_api-0.4/B0tHe1Per_test_api/notes_classes.py
+-rw-rw-rw-   0        0        0     2796 2023-04-10 12:31:45.000000 B0tHe1Per_test_api-0.4/B0tHe1Per_test_api/notes_main.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:36:28.428824 B0tHe1Per_test_api-0.4/B0tHe1Per_test_api.egg-info/
+-rw-rw-rw-   0        0        0      208 2023-04-10 12:36:28.000000 B0tHe1Per_test_api-0.4/B0tHe1Per_test_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      436 2023-04-10 12:36:28.000000 B0tHe1Per_test_api-0.4/B0tHe1Per_test_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 12:36:28.000000 B0tHe1Per_test_api-0.4/B0tHe1Per_test_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-04-10 12:36:28.000000 B0tHe1Per_test_api-0.4/B0tHe1Per_test_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-10 12:36:28.000000 B0tHe1Per_test_api-0.4/B0tHe1Per_test_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      208 2023-04-10 12:36:28.432848 B0tHe1Per_test_api-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-04-10 12:36:28.435776 B0tHe1Per_test_api-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      582 2023-04-10 12:33:46.000000 B0tHe1Per_test_api-0.4/setup.py
```

### Comparing `B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/address_book.py` & `B0tHe1Per_test_api-0.4/B0tHe1Per_test_api/address_book.py`

 * *Files identical despite different names*

### Comparing `B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/bot_interface.py` & `B0tHe1Per_test_api-0.4/B0tHe1Per_test_api/bot_interface.py`

 * *Files identical despite different names*

### Comparing `B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/file_sorter.py` & `B0tHe1Per_test_api-0.4/B0tHe1Per_test_api/file_sorter.py`

 * *Files identical despite different names*

### Comparing `B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/notes_classes.py` & `B0tHe1Per_test_api-0.4/B0tHe1Per_test_api/notes_classes.py`

 * *Files identical despite different names*

### Comparing `B0tHe1Per_test_api-0.3/B0tHe1Per_test_api/notes_main.py` & `B0tHe1Per_test_api-0.4/B0tHe1Per_test_api/notes_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from notes_classes import *
+from B0tHe1Per_test_api.notes_classes import *
 
 MENU = """---Note Book Menu---
 1. Add note.
 2. Read note.
 3. Edit note.
 4. Delete note.
 5. Display all notes.
```

### Comparing `B0tHe1Per_test_api-0.3/setup.py` & `B0tHe1Per_test_api-0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name="B0tHe1Per_test_api",
-    version="0.3",
+    version="0.4",
     author="Serj",
     author_email="buda_serj@yahoo.com",
     description="Test API for Bot Helper project",
     url='https://github.com/serjbuda/B0tHe1Per.git',
     packages=find_packages(),
     install_requires=[],
     entry_points={
         'console_scripts': [
             'bot_helper = B0tHe1Per_test_api.bot_interface:main'
         ]
     },
-    package_data={'B0tHe1Per_test_api': ['file_sorter.py']},
+    package_data={'B0tHe1Per_test_api': ['file_sorter.py', 'notes_classes.py']},
     include_package_data=True
 )
```


# Comparing `tmp/goodreadsscraper-0.2.tar.gz` & `tmp/goodreadsscraper-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodreadsscraper-0.2.tar", last modified: Mon Apr 10 16:25:32 2023, max compression
+gzip compressed data, was "goodreadsscraper-0.3.tar", last modified: Mon Apr 10 16:28:32 2023, max compression
```

## Comparing `goodreadsscraper-0.2.tar` & `goodreadsscraper-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0     1098 2023-04-02 18:42:33.763559 goodreadsscraper-0.2/LICENSE
--rwxr-xr-x   0        0        0    27708 2023-04-05 14:39:21.394653 goodreadsscraper-0.2/geckodriver.log
--rwxr-xr-x   0        0        0    25305 2023-04-10 16:25:26.113828 goodreadsscraper-0.2/goodreadsscraper/__init__.py
--rwxr-xr-x   0        0        0     3660 2023-04-02 22:30:15.644596 goodreadsscraper-0.2/goodreadsscraper/author.py
--rwxr-xr-x   0        0        0     2876 2023-04-02 18:42:33.769060 goodreadsscraper-0.2/goodreadsscraper/book.py
--rwxr-xr-x   0        0        0     2152 2023-04-10 15:25:43.633380 goodreadsscraper-0.2/goodreadsscraper/review.py
--rwxr-xr-x   0        0        0        0 2023-04-05 21:14:32.340995 goodreadsscraper-0.2/goodreadsscraper/test/debug.html
--rwxr-xr-x   0        0        0    12709 2023-04-10 16:22:02.668138 goodreadsscraper-0.2/goodreadsscraper/utils.py
--rwxr-xr-x   0        0        0      530 2023-04-10 15:25:43.647381 goodreadsscraper-0.2/pyproject.toml
--rwxr-xr-x   0        0        0     8669 2023-04-10 16:22:02.675136 goodreadsscraper-0.2/readme.md
--rwxr-xr-x   0        0        0     1996 2023-04-10 15:25:43.652881 goodreadsscraper-0.2/reviewanalyser/__init__.py
--rwxr-xr-x   0        0        0  5329000 2023-04-10 15:25:43.697879 goodreadsscraper-0.2/reviewanalyser/model/review_analyser.h5
--rwxr-xr-x   0        0        0   138845 2023-04-10 15:25:43.705879 goodreadsscraper-0.2/reviewanalyser/model/tv_layer.pkl
--rw-r--r--   0        0        0      356 1970-01-01 00:00:00.000000 goodreadsscraper-0.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1098 2023-04-02 18:42:33.763559 goodreadsscraper-0.3/LICENSE
+-rwxr-xr-x   0        0        0    27708 2023-04-05 14:39:21.394653 goodreadsscraper-0.3/geckodriver.log
+-rwxr-xr-x   0        0        0    25305 2023-04-10 16:28:27.508161 goodreadsscraper-0.3/goodreadsscraper/__init__.py
+-rwxr-xr-x   0        0        0     3660 2023-04-02 22:30:15.644596 goodreadsscraper-0.3/goodreadsscraper/author.py
+-rwxr-xr-x   0        0        0     2876 2023-04-02 18:42:33.769060 goodreadsscraper-0.3/goodreadsscraper/book.py
+-rwxr-xr-x   0        0        0     2152 2023-04-10 15:25:43.633380 goodreadsscraper-0.3/goodreadsscraper/review.py
+-rwxr-xr-x   0        0        0        0 2023-04-05 21:14:32.340995 goodreadsscraper-0.3/goodreadsscraper/test/debug.html
+-rwxr-xr-x   0        0        0    12709 2023-04-10 16:22:02.668138 goodreadsscraper-0.3/goodreadsscraper/utils.py
+-rwxr-xr-x   0        0        0      550 2023-04-10 16:28:29.238615 goodreadsscraper-0.3/pyproject.toml
+-rwxr-xr-x   0        0        0     8669 2023-04-10 16:28:22.834903 goodreadsscraper-0.3/readme.md
+-rwxr-xr-x   0        0        0     1996 2023-04-10 15:25:43.652881 goodreadsscraper-0.3/reviewanalyser/__init__.py
+-rwxr-xr-x   0        0        0  5329000 2023-04-10 15:25:43.697879 goodreadsscraper-0.3/reviewanalyser/model/review_analyser.h5
+-rwxr-xr-x   0        0        0   138845 2023-04-10 15:25:43.705879 goodreadsscraper-0.3/reviewanalyser/model/tv_layer.pkl
+-rw-r--r--   0        0        0     8848 1970-01-01 00:00:00.000000 goodreadsscraper-0.3/PKG-INFO
```

### Comparing `goodreadsscraper-0.2/LICENSE` & `goodreadsscraper-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `goodreadsscraper-0.2/geckodriver.log` & `goodreadsscraper-0.3/geckodriver.log`

 * *Files identical despite different names*

### Comparing `goodreadsscraper-0.2/goodreadsscraper/__init__.py` & `goodreadsscraper-0.3/goodreadsscraper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python3
 """Module to scrap book information from goodreads
 """
 
-__version__ = '0.2'
+__version__ = '0.3'
 
 __description__ = 'Module to scrap book information from goodreads'
 
 import os
 import time
 import re
 import json
```

### Comparing `goodreadsscraper-0.2/goodreadsscraper/author.py` & `goodreadsscraper-0.3/goodreadsscraper/author.py`

 * *Files identical despite different names*

### Comparing `goodreadsscraper-0.2/goodreadsscraper/book.py` & `goodreadsscraper-0.3/goodreadsscraper/book.py`

 * *Files identical despite different names*

### Comparing `goodreadsscraper-0.2/goodreadsscraper/review.py` & `goodreadsscraper-0.3/goodreadsscraper/review.py`

 * *Files identical despite different names*

### Comparing `goodreadsscraper-0.2/goodreadsscraper/utils.py` & `goodreadsscraper-0.3/goodreadsscraper/utils.py`

 * *Files identical despite different names*

### Comparing `goodreadsscraper-0.2/pyproject.toml` & `goodreadsscraper-0.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -5,13 +5,13 @@
 [project]
 name = "goodreadsscraper"
 authors = [{name = "brazafonso", email = "a93178@uminho.pt"},{name = "Tiago Silva", email = "a93277@uminho.pt"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 dependencies = ["jellyfish","pandas","bs4","selenium","argparse"]
-
+readme = "readme.md"
 
 
 [project.scripts]
 grs = "goodreadsscraper:goodreadsscraper"
```

### Comparing `goodreadsscraper-0.2/readme.md` & `goodreadsscraper-0.3/readme.md`

 * *Files identical despite different names*

### Comparing `goodreadsscraper-0.2/reviewanalyser/__init__.py` & `goodreadsscraper-0.3/reviewanalyser/__init__.py`

 * *Files identical despite different names*

### Comparing `goodreadsscraper-0.2/reviewanalyser/model/review_analyser.h5` & `goodreadsscraper-0.3/reviewanalyser/model/review_analyser.h5`

 * *Files identical despite different names*

### Comparing `goodreadsscraper-0.2/reviewanalyser/model/tv_layer.pkl` & `goodreadsscraper-0.3/reviewanalyser/model/tv_layer.pkl`

 * *Files identical despite different names*


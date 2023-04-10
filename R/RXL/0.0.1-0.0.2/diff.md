# Comparing `tmp/RXL-0.0.1.tar.gz` & `tmp/RXL-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RXL-0.0.1.tar", last modified: Tue Mar 28 20:29:19 2023, max compression
+gzip compressed data, was "RXL-0.0.2.tar", last modified: Mon Apr 10 19:45:53 2023, max compression
```

## Comparing `RXL-0.0.1.tar` & `RXL-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 20:29:19.470437 RXL-0.0.1/
--rw-rw-rw-   0        0        0     7815 2022-12-20 17:30:11.000000 RXL-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      352 2023-03-28 20:29:19.468443 RXL-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-03-28 20:27:46.000000 RXL-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-28 20:29:19.455503 RXL-0.0.1/RXL/
--rw-rw-rw-   0        0        0     6121 2023-03-28 20:21:21.000000 RXL-0.0.1/RXL/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 20:29:19.466448 RXL-0.0.1/RXL.egg-info/
--rw-rw-rw-   0        0        0      352 2023-03-28 20:29:19.000000 RXL-0.0.1/RXL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2023-03-28 20:29:19.000000 RXL-0.0.1/RXL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 20:29:19.000000 RXL-0.0.1/RXL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-03-28 20:29:19.000000 RXL-0.0.1/RXL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-28 20:29:19.470437 RXL-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      628 2023-03-28 20:28:50.000000 RXL-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 19:45:53.077176 RXL-0.0.2/
+-rw-rw-rw-   0        0        0     7815 2022-12-20 17:30:11.000000 RXL-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      350 2023-04-10 19:45:53.074614 RXL-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-10 19:45:27.000000 RXL-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 19:45:53.063930 RXL-0.0.2/RXL/
+-rw-rw-rw-   0        0        0     3629 2023-04-09 19:38:27.000000 RXL-0.0.2/RXL/Errors.py
+-rw-rw-rw-   0        0        0    32483 2023-04-09 19:38:27.000000 RXL-0.0.2/RXL/Grammar.py
+-rw-rw-rw-   0        0        0    19597 2023-04-09 19:38:27.000000 RXL-0.0.2/RXL/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 19:45:53.073617 RXL-0.0.2/RXL.egg-info/
+-rw-rw-rw-   0        0        0      350 2023-04-10 19:45:52.000000 RXL-0.0.2/RXL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2023-04-10 19:45:52.000000 RXL-0.0.2/RXL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 19:45:52.000000 RXL-0.0.2/RXL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-04-10 19:45:52.000000 RXL-0.0.2/RXL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 19:45:53.077176 RXL-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      649 2023-04-10 19:45:01.000000 RXL-0.0.2/setup.py
```

### Comparing `RXL-0.0.1/LICENSE` & `RXL-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `RXL-0.0.1/setup.py` & `RXL-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup,find_packages
 
 with open("README.md", "r") as fh:
     long_descriptions = fh.read()
 
 s = setup(
     name = "RXL",
-    version = "0.0.1",
+    version = "0.0.2",
     license = "LGPL",
     description = "RXL Features",
-    url = "https://github.com/Ramin-RX7/RX7-Lib",
+    url = "https://github.com/Ramin-RX7/RX-Language/tree/master/RXL/",
     packages = find_packages(),
     install_requires = [],
     python_requires = ">= 3.8",
     author = "Ramin RX7",
     author_email = "rawmin.rx@gmail.com",
     classifiers = [
         'Programming Language :: Python :: 3',
```


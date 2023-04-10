# Comparing `tmp/enprog-0.0.1.tar.gz` & `tmp/enprog-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\enprog-0.0.1.tar", last modified: Mon Apr 10 01:07:29 2023, max compression
+gzip compressed data, was "dist\enprog-0.0.2.tar", last modified: Mon Apr 10 02:33:14 2023, max compression
```

## Comparing `enprog-0.0.1.tar` & `enprog-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 01:07:29.840000 enprog-0.0.1/
--rw-rw-rw-   0        0        0      295 2023-04-10 01:07:30.000000 enprog-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 01:07:29.850000 enprog-0.0.1/enprog.egg-info/
--rw-rw-rw-   0        0        0      295 2023-04-10 01:07:30.000000 enprog-0.0.1/enprog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      161 2023-04-10 01:07:30.000000 enprog-0.0.1/enprog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 01:07:30.000000 enprog-0.0.1/enprog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-10 01:07:30.000000 enprog-0.0.1/enprog.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 01:07:30.000000 enprog-0.0.1/enprog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 01:07:30.000000 enprog-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      548 2023-04-10 01:07:28.000000 enprog-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 02:33:14.510000 enprog-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-04-10 02:33:14.520000 enprog-0.0.2/ENPROG/
+-rw-rw-rw-   0        0        0       45 2023-04-06 16:08:10.000000 enprog-0.0.2/ENPROG/__init__.py
+-rw-rw-rw-   0        0        0      750 2023-04-10 00:56:34.000000 enprog-0.0.2/ENPROG/__main__.py
+-rw-rw-rw-   0        0        0       22 2023-04-06 06:13:38.000000 enprog-0.0.2/ENPROG/code.enprog
+-rw-rw-rw-   0        0        0     8520 2023-04-10 00:42:52.000000 enprog-0.0.2/ENPROG/enprog.py
+-rw-rw-rw-   0        0        0      280 2023-04-06 15:10:38.000000 enprog-0.0.2/ENPROG/example.py
+-rw-rw-rw-   0        0        0      173 2023-04-09 16:36:18.000000 enprog-0.0.2/ENPROG/examplescript.ep
+-rw-rw-rw-   0        0        0       39 2023-04-10 02:10:18.000000 enprog-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      295 2023-04-10 02:33:16.000000 enprog-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-04-10 01:56:18.000000 enprog-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 02:33:14.530000 enprog-0.0.2/enprog.egg-info/
+-rw-rw-rw-   0        0        0      295 2023-04-10 02:33:16.000000 enprog-0.0.2/enprog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-04-10 02:33:16.000000 enprog-0.0.2/enprog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 02:33:16.000000 enprog-0.0.2/enprog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-10 02:33:16.000000 enprog-0.0.2/enprog.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-10 02:33:16.000000 enprog-0.0.2/enprog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 02:33:16.000000 enprog-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      548 2023-04-10 02:18:40.000000 enprog-0.0.2/setup.py
```

### Comparing `enprog-0.0.1/setup.py` & `enprog-0.0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="enprog",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "enprog=ENPROG.__main__:main",
         ]
     },
     python_requires=">=3.9, <=3.9.6",
```


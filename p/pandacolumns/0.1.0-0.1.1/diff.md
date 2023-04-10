# Comparing `tmp/pandacolumns-0.1.0.tar.gz` & `tmp/pandacolumns-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandacolumns-0.1.0.tar", last modified: Mon Apr 10 19:36:28 2023, max compression
+gzip compressed data, was "pandacolumns-0.1.1.tar", last modified: Mon Apr 10 19:44:29 2023, max compression
```

## Comparing `pandacolumns-0.1.0.tar` & `pandacolumns-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 19:36:28.604020 pandacolumns-0.1.0/
--rw-rw-rw-   0        0        0      171 2023-04-10 19:36:28.604020 pandacolumns-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 19:36:28.584526 pandacolumns-0.1.0/pandacolumns/
--rw-rw-rw-   0        0        0        0 2023-04-10 19:36:18.000000 pandacolumns-0.1.0/pandacolumns/__init__.py
--rw-rw-rw-   0        0        0     2024 2023-04-10 19:20:41.000000 pandacolumns-0.1.0/pandacolumns/pandacolumns.py
-drwxrwxrwx   0        0        0        0 2023-04-10 19:36:28.603028 pandacolumns-0.1.0/pandacolumns.egg-info/
--rw-rw-rw-   0        0        0      171 2023-04-10 19:36:28.000000 pandacolumns-0.1.0/pandacolumns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-04-10 19:36:28.000000 pandacolumns-0.1.0/pandacolumns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 19:36:28.000000 pandacolumns-0.1.0/pandacolumns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-10 19:36:28.000000 pandacolumns-0.1.0/pandacolumns.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 19:36:28.000000 pandacolumns-0.1.0/pandacolumns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 19:36:28.604020 pandacolumns-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      332 2023-04-10 19:24:45.000000 pandacolumns-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 19:44:29.673259 pandacolumns-0.1.1/
+-rw-rw-rw-   0        0        0      171 2023-04-10 19:44:29.673259 pandacolumns-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 19:44:29.658687 pandacolumns-0.1.1/pandacolumns/
+-rw-rw-rw-   0        0        0        0 2023-04-10 19:36:18.000000 pandacolumns-0.1.1/pandacolumns/__init__.py
+-rw-rw-rw-   0        0        0     2024 2023-04-10 19:20:41.000000 pandacolumns-0.1.1/pandacolumns/pandacolumns.py
+drwxrwxrwx   0        0        0        0 2023-04-10 19:44:29.672412 pandacolumns-0.1.1/pandacolumns.egg-info/
+-rw-rw-rw-   0        0        0      171 2023-04-10 19:44:29.000000 pandacolumns-0.1.1/pandacolumns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-04-10 19:44:29.000000 pandacolumns-0.1.1/pandacolumns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 19:44:29.000000 pandacolumns-0.1.1/pandacolumns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-10 19:44:29.000000 pandacolumns-0.1.1/pandacolumns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 19:44:29.000000 pandacolumns-0.1.1/pandacolumns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 19:44:29.673259 pandacolumns-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-04-10 19:44:06.000000 pandacolumns-0.1.1/setup.py
```

### Comparing `pandacolumns-0.1.0/pandacolumns/pandacolumns.py` & `pandacolumns-0.1.1/pandacolumns/pandacolumns.py`

 * *Files identical despite different names*


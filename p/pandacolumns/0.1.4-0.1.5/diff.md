# Comparing `tmp/pandacolumns-0.1.4.tar.gz` & `tmp/pandacolumns-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandacolumns-0.1.4.tar", last modified: Mon Apr 10 21:36:12 2023, max compression
+gzip compressed data, was "pandacolumns-0.1.5.tar", last modified: Mon Apr 10 21:44:48 2023, max compression
```

## Comparing `pandacolumns-0.1.4.tar` & `pandacolumns-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 21:36:12.382493 pandacolumns-0.1.4/
--rw-rw-rw-   0        0        0      171 2023-04-10 21:36:12.382493 pandacolumns-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 21:36:12.371948 pandacolumns-0.1.4/pandacolumns/
--rw-rw-rw-   0        0        0     2111 2023-04-10 19:52:41.000000 pandacolumns-0.1.4/pandacolumns/PandaDrop.py
--rw-rw-rw-   0        0        0       34 2023-04-10 21:35:27.000000 pandacolumns-0.1.4/pandacolumns/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 21:36:12.382493 pandacolumns-0.1.4/pandacolumns.egg-info/
--rw-rw-rw-   0        0        0      171 2023-04-10 21:36:12.000000 pandacolumns-0.1.4/pandacolumns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-04-10 21:36:12.000000 pandacolumns-0.1.4/pandacolumns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 21:36:12.000000 pandacolumns-0.1.4/pandacolumns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-10 21:36:12.000000 pandacolumns-0.1.4/pandacolumns.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 21:36:12.000000 pandacolumns-0.1.4/pandacolumns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 21:36:12.383759 pandacolumns-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-04-10 21:35:44.000000 pandacolumns-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:44:48.377612 pandacolumns-0.1.5/
+-rw-rw-rw-   0        0        0      171 2023-04-10 21:44:48.376613 pandacolumns-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 21:44:48.358149 pandacolumns-0.1.5/pandacolumns/
+-rw-rw-rw-   0        0        0     2111 2023-04-10 19:52:41.000000 pandacolumns-0.1.5/pandacolumns/PandaDrop.py
+-rw-rw-rw-   0        0        0       33 2023-04-10 21:44:27.000000 pandacolumns-0.1.5/pandacolumns/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:44:48.376613 pandacolumns-0.1.5/pandacolumns.egg-info/
+-rw-rw-rw-   0        0        0      171 2023-04-10 21:44:48.000000 pandacolumns-0.1.5/pandacolumns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-04-10 21:44:48.000000 pandacolumns-0.1.5/pandacolumns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 21:44:48.000000 pandacolumns-0.1.5/pandacolumns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-10 21:44:48.000000 pandacolumns-0.1.5/pandacolumns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 21:44:48.000000 pandacolumns-0.1.5/pandacolumns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 21:44:48.377612 pandacolumns-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-04-10 21:44:38.000000 pandacolumns-0.1.5/setup.py
```

### Comparing `pandacolumns-0.1.4/pandacolumns/PandaDrop.py` & `pandacolumns-0.1.5/pandacolumns/PandaDrop.py`

 * *Files identical despite different names*


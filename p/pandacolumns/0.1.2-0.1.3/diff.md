# Comparing `tmp/pandacolumns-0.1.2.tar.gz` & `tmp/pandacolumns-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandacolumns-0.1.2.tar", last modified: Mon Apr 10 19:53:20 2023, max compression
+gzip compressed data, was "pandacolumns-0.1.3.tar", last modified: Mon Apr 10 21:30:33 2023, max compression
```

## Comparing `pandacolumns-0.1.2.tar` & `pandacolumns-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 19:53:20.738822 pandacolumns-0.1.2/
--rw-rw-rw-   0        0        0      171 2023-04-10 19:53:20.738822 pandacolumns-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 19:53:20.727636 pandacolumns-0.1.2/pandacolumns/
--rw-rw-rw-   0        0        0        0 2023-04-10 19:36:18.000000 pandacolumns-0.1.2/pandacolumns/__init__.py
--rw-rw-rw-   0        0        0     2111 2023-04-10 19:52:41.000000 pandacolumns-0.1.2/pandacolumns/pandacolumns.py
-drwxrwxrwx   0        0        0        0 2023-04-10 19:53:20.737817 pandacolumns-0.1.2/pandacolumns.egg-info/
--rw-rw-rw-   0        0        0      171 2023-04-10 19:53:20.000000 pandacolumns-0.1.2/pandacolumns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-04-10 19:53:20.000000 pandacolumns-0.1.2/pandacolumns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 19:53:20.000000 pandacolumns-0.1.2/pandacolumns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-10 19:53:20.000000 pandacolumns-0.1.2/pandacolumns.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 19:53:20.000000 pandacolumns-0.1.2/pandacolumns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 19:53:20.738822 pandacolumns-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-04-10 19:52:59.000000 pandacolumns-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:30:33.902674 pandacolumns-0.1.3/
+-rw-rw-rw-   0        0        0      171 2023-04-10 21:30:33.901670 pandacolumns-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 21:30:33.886437 pandacolumns-0.1.3/pandacolumns/
+-rw-rw-rw-   0        0        0     2111 2023-04-10 19:52:41.000000 pandacolumns-0.1.3/pandacolumns/PandaDrop.py
+-rw-rw-rw-   0        0        0       34 2023-04-10 20:09:33.000000 pandacolumns-0.1.3/pandacolumns/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:30:33.900668 pandacolumns-0.1.3/pandacolumns.egg-info/
+-rw-rw-rw-   0        0        0      171 2023-04-10 21:30:33.000000 pandacolumns-0.1.3/pandacolumns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-04-10 21:30:33.000000 pandacolumns-0.1.3/pandacolumns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 21:30:33.000000 pandacolumns-0.1.3/pandacolumns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-10 21:30:33.000000 pandacolumns-0.1.3/pandacolumns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 21:30:33.000000 pandacolumns-0.1.3/pandacolumns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 21:30:33.902674 pandacolumns-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-04-10 21:30:24.000000 pandacolumns-0.1.3/setup.py
```

### Comparing `pandacolumns-0.1.2/pandacolumns/pandacolumns.py` & `pandacolumns-0.1.3/pandacolumns/PandaDrop.py`

 * *Files identical despite different names*


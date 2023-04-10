# Comparing `tmp/pandacolumns-0.1.1.tar.gz` & `tmp/pandacolumns-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandacolumns-0.1.1.tar", last modified: Mon Apr 10 19:44:29 2023, max compression
+gzip compressed data, was "pandacolumns-0.1.2.tar", last modified: Mon Apr 10 19:53:20 2023, max compression
```

## Comparing `pandacolumns-0.1.1.tar` & `pandacolumns-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 19:44:29.673259 pandacolumns-0.1.1/
--rw-rw-rw-   0        0        0      171 2023-04-10 19:44:29.673259 pandacolumns-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 19:44:29.658687 pandacolumns-0.1.1/pandacolumns/
--rw-rw-rw-   0        0        0        0 2023-04-10 19:36:18.000000 pandacolumns-0.1.1/pandacolumns/__init__.py
--rw-rw-rw-   0        0        0     2024 2023-04-10 19:20:41.000000 pandacolumns-0.1.1/pandacolumns/pandacolumns.py
-drwxrwxrwx   0        0        0        0 2023-04-10 19:44:29.672412 pandacolumns-0.1.1/pandacolumns.egg-info/
--rw-rw-rw-   0        0        0      171 2023-04-10 19:44:29.000000 pandacolumns-0.1.1/pandacolumns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-04-10 19:44:29.000000 pandacolumns-0.1.1/pandacolumns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 19:44:29.000000 pandacolumns-0.1.1/pandacolumns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-10 19:44:29.000000 pandacolumns-0.1.1/pandacolumns.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 19:44:29.000000 pandacolumns-0.1.1/pandacolumns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 19:44:29.673259 pandacolumns-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-04-10 19:44:06.000000 pandacolumns-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 19:53:20.738822 pandacolumns-0.1.2/
+-rw-rw-rw-   0        0        0      171 2023-04-10 19:53:20.738822 pandacolumns-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 19:53:20.727636 pandacolumns-0.1.2/pandacolumns/
+-rw-rw-rw-   0        0        0        0 2023-04-10 19:36:18.000000 pandacolumns-0.1.2/pandacolumns/__init__.py
+-rw-rw-rw-   0        0        0     2111 2023-04-10 19:52:41.000000 pandacolumns-0.1.2/pandacolumns/pandacolumns.py
+drwxrwxrwx   0        0        0        0 2023-04-10 19:53:20.737817 pandacolumns-0.1.2/pandacolumns.egg-info/
+-rw-rw-rw-   0        0        0      171 2023-04-10 19:53:20.000000 pandacolumns-0.1.2/pandacolumns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-04-10 19:53:20.000000 pandacolumns-0.1.2/pandacolumns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 19:53:20.000000 pandacolumns-0.1.2/pandacolumns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-10 19:53:20.000000 pandacolumns-0.1.2/pandacolumns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 19:53:20.000000 pandacolumns-0.1.2/pandacolumns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 19:53:20.738822 pandacolumns-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-04-10 19:52:59.000000 pandacolumns-0.1.2/setup.py
```

### Comparing `pandacolumns-0.1.1/pandacolumns/pandacolumns.py` & `pandacolumns-0.1.2/pandacolumns/pandacolumns.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-def pandacolumns(df):
+import pandas as pd
+import ipywidgets as widgets
+from IPython.display import display
+
+def PandaDrop(df):
   checkboxes = [widgets.Checkbox(value=False, description=column) for column in df.columns]
 
   for checkbox in checkboxes:
       checkbox.layout.width = 'auto'
       #checkbox.layout.margin = '10px'
       checkbox.style.description_width = 'initial'
       checkbox.style.font_weight = 'bold'
```


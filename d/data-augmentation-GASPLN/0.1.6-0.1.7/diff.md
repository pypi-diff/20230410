# Comparing `tmp/data_augmentation_GASPLN-0.1.6.tar.gz` & `tmp/data_augmentation_GASPLN-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_augmentation_GASPLN-0.1.6.tar", last modified: Sat Apr  8 17:00:08 2023, max compression
+gzip compressed data, was "data_augmentation_GASPLN-0.1.7.tar", last modified: Mon Apr 10 14:56:57 2023, max compression
```

## Comparing `data_augmentation_GASPLN-0.1.6.tar` & `data_augmentation_GASPLN-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 17:00:08.488831 data_augmentation_GASPLN-0.1.6/
--rw-rw-rw-   0        0        0    35823 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       24 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      217 2023-04-08 17:00:08.488831 data_augmentation_GASPLN-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2462 2023-04-08 16:59:37.000000 data_augmentation_GASPLN-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 17:00:08.467715 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN/
--rw-rw-rw-   0        0        0        0 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:00:08.474717 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN/data/
--rw-rw-rw-   0        0        0  7024004 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet
--rw-rw-rw-   0        0        0     3141 2023-04-08 16:34:07.000000 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN/data_augmentation.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:00:08.474717 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN.egg-info/
--rw-rw-rw-   0        0        0      217 2023-04-08 17:00:08.000000 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      423 2023-04-08 17:00:08.000000 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 17:00:08.000000 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-08 17:00:08.000000 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-04-08 17:00:08.000000 data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-08 17:00:08.489831 data_augmentation_GASPLN-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      553 2023-04-08 16:59:32.000000 data_augmentation_GASPLN-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:56:57.767888 data_augmentation_GASPLN-0.1.7/
+-rw-rw-rw-   0        0        0    35823 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      217 2023-04-10 14:56:57.768888 data_augmentation_GASPLN-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5226 2023-04-09 23:28:39.000000 data_augmentation_GASPLN-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 14:56:57.698629 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN/
+-rw-rw-rw-   0        0        0        0 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:56:57.753888 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN/data/
+-rw-rw-rw-   0        0        0  7024004 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet
+-rw-rw-rw-   0        0        0     6150 2023-04-09 23:26:15.000000 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN/data_augmentation.py
+drwxrwxrwx   0        0        0        0 2023-04-10 14:56:57.752890 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN.egg-info/
+-rw-rw-rw-   0        0        0      217 2023-04-10 14:56:57.000000 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      423 2023-04-10 14:56:57.000000 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 14:56:57.000000 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-10 14:56:57.000000 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-04-10 14:56:57.000000 data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-10 14:56:57.769890 data_augmentation_GASPLN-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      553 2023-04-10 14:56:51.000000 data_augmentation_GASPLN-0.1.7/setup.py
```

### Comparing `data_augmentation_GASPLN-0.1.6/LICENSE` & `data_augmentation_GASPLN-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `data_augmentation_GASPLN-0.1.6/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet` & `data_augmentation_GASPLN-0.1.7/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet`

 * *Files identical despite different names*

### Comparing `data_augmentation_GASPLN-0.1.6/setup.py` & `data_augmentation_GASPLN-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='data_augmentation_GASPLN',
-    version='0.1.6',
+    version='0.1.7',
     author='Artur Melchiori Cerri',
     author_email='arturmelchiori@gmail.com',
     description='Data augmentation for Portuguese language',
     install_requires=[
         "spacy",
         "nltk",
         "pandas",
```


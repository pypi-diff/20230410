# Comparing `tmp/Postprocessing and POSEA-1.0.tar.gz` & `tmp/Postprocessing and POSEA-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Postprocessing and POSEA-1.0.tar", last modified: Mon Apr 10 03:46:21 2023, max compression
+gzip compressed data, was "Postprocessing and POSEA-1.1.tar", last modified: Mon Apr 10 11:16:12 2023, max compression
```

## Comparing `Postprocessing and POSEA-1.0.tar` & `Postprocessing and POSEA-1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 03:46:21.198743 Postprocessing and POSEA-1.0/
--rw-rw-rw-   0        0        0     1461 2023-04-10 02:00:18.000000 Postprocessing and POSEA-1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      651 2023-04-10 03:46:21.199741 Postprocessing and POSEA-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 03:46:21.197746 Postprocessing and POSEA-1.0/Postprocessing_and_POSEA.egg-info/
--rw-rw-rw-   0        0        0      651 2023-04-10 03:46:20.000000 Postprocessing and POSEA-1.0/Postprocessing_and_POSEA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-04-10 03:46:21.000000 Postprocessing and POSEA-1.0/Postprocessing_and_POSEA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 03:46:20.000000 Postprocessing and POSEA-1.0/Postprocessing_and_POSEA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-10 03:46:20.000000 Postprocessing and POSEA-1.0/Postprocessing_and_POSEA.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 03:46:21.000000 Postprocessing and POSEA-1.0/Postprocessing_and_POSEA.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      966 2023-04-10 02:35:58.000000 Postprocessing and POSEA-1.0/README.txt
--rw-rw-rw-   0        0        0       86 2023-04-10 03:46:21.199741 Postprocessing and POSEA-1.0/setup.cfg
--rw-rw-rw-   0        0        0      967 2023-04-10 03:46:13.000000 Postprocessing and POSEA-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 11:16:12.885162 Postprocessing and POSEA-1.1/
+-rw-rw-rw-   0        0        0     1461 2023-04-10 02:00:18.000000 Postprocessing and POSEA-1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      909 2023-04-10 11:16:12.885162 Postprocessing and POSEA-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 11:16:12.884164 Postprocessing and POSEA-1.1/Postprocessing_and_POSEA.egg-info/
+-rw-rw-rw-   0        0        0      909 2023-04-10 11:16:12.000000 Postprocessing and POSEA-1.1/Postprocessing_and_POSEA.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-04-10 11:16:12.000000 Postprocessing and POSEA-1.1/Postprocessing_and_POSEA.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 11:16:12.000000 Postprocessing and POSEA-1.1/Postprocessing_and_POSEA.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-10 11:16:12.000000 Postprocessing and POSEA-1.1/Postprocessing_and_POSEA.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 11:16:12.000000 Postprocessing and POSEA-1.1/Postprocessing_and_POSEA.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      966 2023-04-10 02:35:58.000000 Postprocessing and POSEA-1.1/README.txt
+-rw-rw-rw-   0        0        0       86 2023-04-10 11:16:12.886159 Postprocessing and POSEA-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1200 2023-04-10 11:13:49.000000 Postprocessing and POSEA-1.1/setup.py
```

### Comparing `Postprocessing and POSEA-1.0/LICENSE.txt` & `Postprocessing and POSEA-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Postprocessing and POSEA-1.0/README.txt` & `Postprocessing and POSEA-1.1/README.txt`

 * *Files identical despite different names*


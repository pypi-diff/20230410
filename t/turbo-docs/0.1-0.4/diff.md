# Comparing `tmp/turbo_docs-0.1.tar.gz` & `tmp/turbo_docs-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\turbo_docs-0.1.tar", last modified: Sun Apr  9 17:22:33 2023, max compression
+gzip compressed data, was "dist\turbo_docs-0.4.tar", last modified: Sun Apr  9 23:17:47 2023, max compression
```

## Comparing `turbo_docs-0.1.tar` & `turbo_docs-0.4.tar`

### file list

```diff
@@ -1,12 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 17:22:33.228967 turbo_docs-0.1/
--rw-rw-rw-   0        0        0      450 2023-04-09 17:22:33.227969 turbo_docs-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1142 2023-04-09 16:47:21.000000 turbo_docs-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-09 17:22:33.228967 turbo_docs-0.1/setup.cfg
--rw-rw-rw-   0        0        0      782 2023-04-09 17:22:30.000000 turbo_docs-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 17:22:33.225968 turbo_docs-0.1/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0      450 2023-04-09 17:22:33.000000 turbo_docs-0.1/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-04-09 17:22:33.000000 turbo_docs-0.1/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 17:22:33.000000 turbo_docs-0.1/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-09 17:22:33.000000 turbo_docs-0.1/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-04-09 17:22:33.000000 turbo_docs-0.1/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 17:22:33.000000 turbo_docs-0.1/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 23:17:47.434260 turbo_docs-0.4/
+-rw-rw-rw-   0        0        0      450 2023-04-09 23:17:47.433260 turbo_docs-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1142 2023-04-09 16:47:21.000000 turbo_docs-0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-09 23:17:47.434260 turbo_docs-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      782 2023-04-09 23:15:13.000000 turbo_docs-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 23:17:47.414359 turbo_docs-0.4/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-09 17:13:17.000000 turbo_docs-0.4/turbo_docs/__init__.py
+-rw-rw-rw-   0        0        0     1133 2023-04-09 16:45:58.000000 turbo_docs-0.4/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-04-09 23:17:47.431260 turbo_docs-0.4/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-09 17:33:26.000000 turbo_docs-0.4/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0      487 2023-04-09 16:37:59.000000 turbo_docs-0.4/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     2155 2023-04-09 16:35:50.000000 turbo_docs-0.4/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0      686 2023-04-09 16:35:50.000000 turbo_docs-0.4/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-04-09 23:17:47.424253 turbo_docs-0.4/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0      450 2023-04-09 23:17:47.000000 turbo_docs-0.4/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-04-09 23:17:47.000000 turbo_docs-0.4/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 23:17:47.000000 turbo_docs-0.4/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-09 23:17:47.000000 turbo_docs-0.4/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-04-09 23:17:47.000000 turbo_docs-0.4/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-09 23:17:47.000000 turbo_docs-0.4/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.1/README.md` & `turbo_docs-0.4/README.md`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.1/setup.py` & `turbo_docs-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="turbo_docs",
-    version="0.1",
+    version="0.4",
     packages=find_packages(),
     install_requires=[
         "requests",
         "openai",
         "click",
         "pyperclip",
     ],
```


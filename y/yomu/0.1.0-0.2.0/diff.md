# Comparing `tmp/yomu-0.1.0.tar.gz` & `tmp/yomu-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yomu-0.1.0.tar", last modified: Sun Aug  8 22:55:34 2021, max compression
+gzip compressed data, was "yomu-0.2.0.tar", last modified: Mon Apr 10 18:54:08 2023, max compression
```

## Comparing `yomu-0.1.0.tar` & `yomu-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 22:55:34.172216 yomu-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-08-08 22:55:21.000000 yomu-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      643 2021-08-08 22:55:34.172216 yomu-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-08-08 22:55:21.000000 yomu-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-08 22:55:34.172216 yomu-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      941 2021-08-08 22:55:21.000000 yomu-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 22:55:34.172216 yomu-0.1.0/yomu/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-08-08 22:55:21.000000 yomu-0.1.0/yomu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5486 2021-08-08 22:55:21.000000 yomu-0.1.0/yomu/readme.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-08 22:55:34.172216 yomu-0.1.0/yomu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      643 2021-08-08 22:55:34.000000 yomu-0.1.0/yomu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-08-08 22:55:34.000000 yomu-0.1.0/yomu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-08 22:55:34.000000 yomu-0.1.0/yomu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-08-08 22:55:34.000000 yomu-0.1.0/yomu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-08-08 22:55:34.000000 yomu-0.1.0/yomu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-08-08 22:55:34.000000 yomu-0.1.0/yomu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:54:08.693479 yomu-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-10 18:53:56.000000 yomu-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-10 18:54:08.693479 yomu-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-10 18:53:56.000000 yomu-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:54:08.693479 yomu-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-10 18:53:56.000000 yomu-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:54:08.689479 yomu-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-10 18:53:56.000000 yomu-0.2.0/tests/test_readme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:54:08.693479 yomu-0.2.0/yomu/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 18:53:56.000000 yomu-0.2.0/yomu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-04-10 18:53:56.000000 yomu-0.2.0/yomu/readme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:54:08.693479 yomu-0.2.0/yomu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-10 18:54:08.000000 yomu-0.2.0/yomu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-10 18:54:08.000000 yomu-0.2.0/yomu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:54:08.000000 yomu-0.2.0/yomu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-10 18:54:08.000000 yomu-0.2.0/yomu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 18:54:08.000000 yomu-0.2.0/yomu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 18:54:08.000000 yomu-0.2.0/yomu.egg-info/top_level.txt
```

### Comparing `yomu-0.1.0/LICENSE` & `yomu-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yomu-0.1.0/setup.py` & `yomu-0.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yomu",
-    version="0.1.0",
+    version="0.2.0",
     author="The Renegade Coder",
     author_email="jeremy.grifski@therenegadecoder.com",
     description="Generates the README for the 'How to Python Code' repo",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TheRenegadeCoder/how-to-python-readme",
     packages=setuptools.find_packages(),
     install_requires=[
         "feedparser>=6",
         "beautifulsoup4>=4",
-        "SnakeMD>=0"
+        "SnakeMD>=2"
     ],
     entry_points={
         "console_scripts": [
             'yomu = yomu.readme:main'
         ],
     },
     classifiers=(
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License"
     ),
 )
```


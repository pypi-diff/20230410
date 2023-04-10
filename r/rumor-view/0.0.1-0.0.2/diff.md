# Comparing `tmp/rumor_view-0.0.1.tar.gz` & `tmp/rumor_view-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rumor_view-0.0.1.tar", last modified: Thu Apr  6 05:05:03 2023, max compression
+gzip compressed data, was "rumor_view-0.0.2.tar", last modified: Mon Apr 10 02:40:43 2023, max compression
```

## Comparing `rumor_view-0.0.1.tar` & `rumor_view-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-04-06 05:05:03.950771 rumor_view-0.0.1/
--rw-r--r--   0 neo       (1000) neo       (1000)      514 2023-04-06 05:05:03.950771 rumor_view-0.0.1/PKG-INFO
--rwxr-xr-x   0 neo       (1000) neo       (1000)       82 2023-04-06 05:04:55.000000 rumor_view-0.0.1/README.md
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-04-06 05:05:03.950771 rumor_view-0.0.1/rumor_view/
--rwxr-xr-x   0 neo       (1000) neo       (1000)       28 2023-04-06 04:35:16.000000 rumor_view-0.0.1/rumor_view/__init__.py
--rwxr-xr-x   0 neo       (1000) neo       (1000)      498 2023-04-06 00:32:35.000000 rumor_view-0.0.1/rumor_view/categoricalization.py
--rwxr-xr-x   0 neo       (1000) neo       (1000)     5831 2023-04-06 04:42:50.000000 rumor_view-0.0.1/rumor_view/view.py
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-04-06 05:05:03.950771 rumor_view-0.0.1/rumor_view.egg-info/
--rw-r--r--   0 neo       (1000) neo       (1000)      514 2023-04-06 05:05:03.000000 rumor_view-0.0.1/rumor_view.egg-info/PKG-INFO
--rw-r--r--   0 neo       (1000) neo       (1000)      262 2023-04-06 05:05:03.000000 rumor_view-0.0.1/rumor_view.egg-info/SOURCES.txt
--rw-r--r--   0 neo       (1000) neo       (1000)        1 2023-04-06 05:05:03.000000 rumor_view-0.0.1/rumor_view.egg-info/dependency_links.txt
--rw-r--r--   0 neo       (1000) neo       (1000)       34 2023-04-06 05:05:03.000000 rumor_view-0.0.1/rumor_view.egg-info/requires.txt
--rw-r--r--   0 neo       (1000) neo       (1000)       11 2023-04-06 05:05:03.000000 rumor_view-0.0.1/rumor_view.egg-info/top_level.txt
--rw-r--r--   0 neo       (1000) neo       (1000)       38 2023-04-06 05:05:03.950771 rumor_view-0.0.1/setup.cfg
--rwxr-xr-x   0 neo       (1000) neo       (1000)      862 2023-04-06 04:57:51.000000 rumor_view-0.0.1/setup.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-04-10 02:40:43.102229 rumor_view-0.0.2/
+-rw-r--r--   0 neo       (1000) neo       (1000)     1658 2023-04-10 02:40:43.102229 rumor_view-0.0.2/PKG-INFO
+-rwxr-xr-x   0 neo       (1000) neo       (1000)     1226 2023-04-10 02:40:06.000000 rumor_view-0.0.2/README.md
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-04-10 02:40:43.102229 rumor_view-0.0.2/rumor_view/
+-rwxr-xr-x   0 neo       (1000) neo       (1000)       28 2023-04-06 04:35:16.000000 rumor_view-0.0.2/rumor_view/__init__.py
+-rwxr-xr-x   0 neo       (1000) neo       (1000)      498 2023-04-06 00:32:35.000000 rumor_view-0.0.2/rumor_view/categoricalization.py
+-rwxr-xr-x   0 neo       (1000) neo       (1000)     7439 2023-04-10 02:39:47.000000 rumor_view-0.0.2/rumor_view/view.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-04-10 02:40:43.102229 rumor_view-0.0.2/rumor_view.egg-info/
+-rw-r--r--   0 neo       (1000) neo       (1000)     1658 2023-04-10 02:40:43.000000 rumor_view-0.0.2/rumor_view.egg-info/PKG-INFO
+-rw-r--r--   0 neo       (1000) neo       (1000)      281 2023-04-10 02:40:43.000000 rumor_view-0.0.2/rumor_view.egg-info/SOURCES.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)        1 2023-04-10 02:40:43.000000 rumor_view-0.0.2/rumor_view.egg-info/dependency_links.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)       34 2023-04-10 02:40:43.000000 rumor_view-0.0.2/rumor_view.egg-info/requires.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)       11 2023-04-10 02:40:43.000000 rumor_view-0.0.2/rumor_view.egg-info/top_level.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)       38 2023-04-10 02:40:43.102229 rumor_view-0.0.2/setup.cfg
+-rwxr-xr-x   0 neo       (1000) neo       (1000)      862 2023-04-10 02:40:28.000000 rumor_view-0.0.2/setup.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-04-10 02:40:43.102229 rumor_view-0.0.2/tests/
+-rwxr-xr-x   0 neo       (1000) neo       (1000)     3175 2023-04-10 02:16:20.000000 rumor_view-0.0.2/tests/test_view.py
```

### Comparing `rumor_view-0.0.1/setup.py` & `rumor_view-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requirements = [str(req) for req in pkg_resources.parse_requirements(f)]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rumor_view",
-    version="0.0.1",
+    version="0.0.2",
     author="@not-so-fat",
     author_email="conjurer.not.so.fat@gmail.com",
     description="Visualization of column value relationship",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/not-so-fat/rumor_view",
     install_requires=requirements,
```


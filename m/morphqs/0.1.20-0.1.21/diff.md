# Comparing `tmp/morphqs-0.1.20.tar.gz` & `tmp/morphqs-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphqs-0.1.20.tar", last modified: Fri Apr  7 16:35:11 2023, max compression
+gzip compressed data, was "morphqs-0.1.21.tar", last modified: Mon Apr 10 14:03:02 2023, max compression
```

## Comparing `morphqs-0.1.20.tar` & `morphqs-0.1.21.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-07 16:35:11.641857 morphqs-0.1.20/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1072 2023-03-29 01:49:10.000000 morphqs-0.1.20/LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      925 2023-04-07 16:35:11.640033 morphqs-0.1.20/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      206 2023-03-29 01:54:53.000000 morphqs-0.1.20/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-07 16:35:11.574946 morphqs-0.1.20/morphqs/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      201 2023-04-07 16:34:53.000000 morphqs-0.1.20/morphqs/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-07 16:35:11.626335 morphqs-0.1.20/morphqs/components/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-29 02:36:46.000000 morphqs-0.1.20/morphqs/components/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1253 2023-04-07 14:03:43.000000 morphqs-0.1.20/morphqs/components/ansible.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3444 2023-04-07 16:04:30.000000 morphqs-0.1.20/morphqs/components/integrations.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6366 2023-04-05 12:30:10.000000 morphqs-0.1.20/morphqs/components/uchigheredmsp.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8969 2023-04-07 16:15:46.000000 morphqs-0.1.20/morphqs/components/usecasedeployment.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-07 16:35:11.634766 morphqs-0.1.20/morphqs/logging/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-28 19:26:20.000000 morphqs-0.1.20/morphqs/logging/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1959 2023-03-28 19:26:20.000000 morphqs-0.1.20/morphqs/logging/loghandler.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3034 2023-03-28 19:51:08.000000 morphqs-0.1.20/morphqs/morphclass.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-07 16:35:11.605394 morphqs-0.1.20/morphqs.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      925 2023-04-07 16:35:11.000000 morphqs-0.1.20/morphqs.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      456 2023-04-07 16:35:11.000000 morphqs-0.1.20/morphqs.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-07 16:35:11.000000 morphqs-0.1.20/morphqs.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-04-07 16:35:11.000000 morphqs-0.1.20/morphqs.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-04-07 16:35:11.000000 morphqs-0.1.20/morphqs.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-07 16:35:11.642900 morphqs-0.1.20/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1025 2023-04-07 16:35:09.000000 morphqs-0.1.20/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-10 14:03:02.774863 morphqs-0.1.21/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1072 2023-03-29 01:49:10.000000 morphqs-0.1.21/LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      925 2023-04-10 14:03:02.773687 morphqs-0.1.21/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      206 2023-03-29 01:54:53.000000 morphqs-0.1.21/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-10 14:03:02.711048 morphqs-0.1.21/morphqs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      201 2023-04-07 16:34:53.000000 morphqs-0.1.21/morphqs/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-10 14:03:02.762024 morphqs-0.1.21/morphqs/components/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-29 02:36:46.000000 morphqs-0.1.21/morphqs/components/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1253 2023-04-07 14:03:43.000000 morphqs-0.1.21/morphqs/components/ansible.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3444 2023-04-07 16:04:30.000000 morphqs-0.1.21/morphqs/components/integrations.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6366 2023-04-05 12:30:10.000000 morphqs-0.1.21/morphqs/components/uchigheredmsp.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8969 2023-04-07 16:15:46.000000 morphqs-0.1.21/morphqs/components/usecasedeployment.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-10 14:03:02.770171 morphqs-0.1.21/morphqs/logging/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-28 19:26:20.000000 morphqs-0.1.21/morphqs/logging/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1959 2023-03-28 19:26:20.000000 morphqs-0.1.21/morphqs/logging/loghandler.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3034 2023-03-28 19:51:08.000000 morphqs-0.1.21/morphqs/morphclass.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-10 14:03:02.736952 morphqs-0.1.21/morphqs.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      925 2023-04-10 14:03:02.000000 morphqs-0.1.21/morphqs.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      456 2023-04-10 14:03:02.000000 morphqs-0.1.21/morphqs.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-10 14:03:02.000000 morphqs-0.1.21/morphqs.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-04-10 14:03:02.000000 morphqs-0.1.21/morphqs.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-04-10 14:03:02.000000 morphqs-0.1.21/morphqs.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-10 14:03:02.775505 morphqs-0.1.21/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1025 2023-04-10 14:03:00.000000 morphqs-0.1.21/setup.py
```

### Comparing `morphqs-0.1.20/LICENSE.txt` & `morphqs-0.1.21/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.20/PKG-INFO` & `morphqs-0.1.21/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphqs
-Version: 0.1.20
+Version: 0.1.21
 Summary: Tool utilized to deploy some basic concepts for the Morpheus Data Platform
 Home-page: https://gitlab.com/jaredlutgen/morphqs
 Author: Jared Lutgen
 Author-email: jlutgen@morpheusdata.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `morphqs-0.1.20/morphqs/components/ansible.py` & `morphqs-0.1.21/morphqs/components/ansible.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.20/morphqs/components/integrations.py` & `morphqs-0.1.21/morphqs/components/integrations.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.20/morphqs/components/uchigheredmsp.py` & `morphqs-0.1.21/morphqs/components/uchigheredmsp.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.20/morphqs/components/usecasedeployment.py` & `morphqs-0.1.21/morphqs/components/usecasedeployment.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.20/morphqs/logging/loghandler.py` & `morphqs-0.1.21/morphqs/logging/loghandler.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.20/morphqs/morphclass.py` & `morphqs-0.1.21/morphqs/morphclass.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.20/morphqs.egg-info/PKG-INFO` & `morphqs-0.1.21/morphqs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphqs
-Version: 0.1.20
+Version: 0.1.21
 Summary: Tool utilized to deploy some basic concepts for the Morpheus Data Platform
 Home-page: https://gitlab.com/jaredlutgen/morphqs
 Author: Jared Lutgen
 Author-email: jlutgen@morpheusdata.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `morphqs-0.1.20/setup.py` & `morphqs-0.1.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setuptools.setup(
     author="Jared Lutgen",
     author_email="jlutgen@morpheusdata.com",
     name='morphqs',
     license="MIT",
     description='Tool utilized to deploy some basic concepts for the Morpheus Data Platform',
-    version='v0.1.20',
+    version='v0.1.21',
     long_description=README,
     url='https://gitlab.com/jaredlutgen/morphqs',
     packages=setuptools.find_packages(),
     python_requires=">=3.5",
     install_requires=['requests'],
     classifiers=[
         # Trove classifiers
```


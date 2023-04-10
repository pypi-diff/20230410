# Comparing `tmp/NikeCA-0.1.51.tar.gz` & `tmp/NikeCA-0.1.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.51.tar", last modified: Wed Apr  5 20:54:21 2023, max compression
+gzip compressed data, was "NikeCA-0.1.52.tar", last modified: Mon Apr 10 17:23:51 2023, max compression
```

## Comparing `NikeCA-0.1.51.tar` & `NikeCA-0.1.52.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-05 20:54:21.320851 NikeCA-0.1.51/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-02-18 07:46:56.000000 NikeCA-0.1.51/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-05 20:54:21.320574 NikeCA-0.1.51/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-03-15 23:26:31.000000 NikeCA-0.1.51/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-05 20:54:21.320928 NikeCA-0.1.51/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2236 2023-04-05 20:53:28.000000 NikeCA-0.1.51/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-05 20:54:21.318355 NikeCA-0.1.51/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-05 20:54:21.320105 NikeCA-0.1.51/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-05 20:54:21.000000 NikeCA-0.1.51/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      406 2023-04-05 20:54:21.000000 NikeCA-0.1.51/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-05 20:54:21.000000 NikeCA-0.1.51/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-05 20:54:21.000000 NikeCA-0.1.51/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      134 2023-04-05 20:54:21.000000 NikeCA-0.1.51/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)       92 2023-04-05 17:14:16.000000 NikeCA-0.1.51/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     9133 2023-04-05 17:14:16.000000 NikeCA-0.1.51/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    19846 2023-04-05 17:14:16.000000 NikeCA-0.1.51/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-05 17:14:16.000000 NikeCA-0.1.51/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     8728 2023-04-05 17:14:16.000000 NikeCA-0.1.51/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3710 2023-04-05 17:14:16.000000 NikeCA-0.1.51/src/_IMPSummaryDashboard.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-05 17:14:16.000000 NikeCA-0.1.51/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13952 2023-04-05 17:14:16.000000 NikeCA-0.1.51/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     6490 2023-04-05 17:14:16.000000 NikeCA-0.1.51/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7240 2023-04-05 17:14:16.000000 NikeCA-0.1.51/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-05 17:14:16.000000 NikeCA-0.1.51/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-10 17:23:51.698516 NikeCA-0.1.52/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-02-18 07:46:56.000000 NikeCA-0.1.52/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-10 17:23:51.697898 NikeCA-0.1.52/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-03-15 23:26:31.000000 NikeCA-0.1.52/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-10 17:23:51.698633 NikeCA-0.1.52/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2254 2023-04-10 17:23:20.000000 NikeCA-0.1.52/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-10 17:23:51.694941 NikeCA-0.1.52/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-10 17:23:51.697240 NikeCA-0.1.52/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-10 17:23:51.000000 NikeCA-0.1.52/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      426 2023-04-10 17:23:51.000000 NikeCA-0.1.52/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-10 17:23:51.000000 NikeCA-0.1.52/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-10 17:23:51.000000 NikeCA-0.1.52/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      147 2023-04-10 17:23:51.000000 NikeCA-0.1.52/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)       92 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    19846 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3710 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/_IMPSummaryDashboard.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3205 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13952 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6490 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7240 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/__init__.py
```

### Comparing `NikeCA-0.1.51/LICENSE` & `NikeCA-0.1.52/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.51/PKG-INFO` & `NikeCA-0.1.52/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.51
+Version: 0.1.52
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.51/README.md` & `NikeCA-0.1.52/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.51/setup.py` & `NikeCA-0.1.52/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.51',
+	version='0.1.52',
 	description='Standardize and Automate processes utilized by the DAMs at Nike in CA',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"_IMPSummaryDashboard",
+		"_SearchFiles",
 		"_SnowflakeDependencies",
 		"_SnowflakePull",
 		"NikeQA",
 		"_QA",
 		"_GitHub",
 		"NikeCA"
 	],
```

### Comparing `NikeCA-0.1.51/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.52/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.51
+Version: 0.1.52
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.51/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.52/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.51/src/NikeSF.py` & `NikeCA-0.1.52/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.51/src/_BuildSearchQuery.py` & `NikeCA-0.1.52/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.51/src/_IMPSummaryDashboard.py` & `NikeCA-0.1.52/src/_IMPSummaryDashboard.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.51/src/_QA.py` & `NikeCA-0.1.52/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.51/src/_SnowflakeData.py` & `NikeCA-0.1.52/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.51/src/_SnowflakeDependencies.py` & `NikeCA-0.1.52/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.51/src/_SnowflakePull.py` & `NikeCA-0.1.52/src/_SnowflakePull.py`

 * *Files identical despite different names*


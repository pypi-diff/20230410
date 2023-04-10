# Comparing `tmp/lightapi-0.0.17.tar.gz` & `tmp/lightapi-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightapi-0.0.17.tar", last modified: Wed Apr  5 06:28:00 2023, max compression
+gzip compressed data, was "lightapi-0.0.18.tar", last modified: Mon Apr 10 03:49:55 2023, max compression
```

## Comparing `lightapi-0.0.17.tar` & `lightapi-0.0.18.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 jordanplows   (501) staff       (20)        0 2023-04-05 06:28:00.349828 lightapi-0.0.17/
-drwxr-xr-x   0 jordanplows   (501) staff       (20)        0 2023-04-05 06:28:00.349426 lightapi-0.0.17/LightAPI.egg-info/
--rw-r--r--   0 jordanplows   (501) staff       (20)     1533 2023-04-05 06:28:00.000000 lightapi-0.0.17/LightAPI.egg-info/PKG-INFO
--rw-r--r--   0 jordanplows   (501) staff       (20)      280 2023-04-05 06:28:00.000000 lightapi-0.0.17/LightAPI.egg-info/SOURCES.txt
--rw-r--r--   0 jordanplows   (501) staff       (20)        1 2023-04-05 06:28:00.000000 lightapi-0.0.17/LightAPI.egg-info/dependency_links.txt
--rw-r--r--   0 jordanplows   (501) staff       (20)        4 2023-04-05 06:28:00.000000 lightapi-0.0.17/LightAPI.egg-info/top_level.txt
--rw-r--r--   0 jordanplows   (501) staff       (20)     1533 2023-04-05 06:28:00.349721 lightapi-0.0.17/PKG-INFO
--rw-r--r--   0 jordanplows   (501) staff       (20)     1318 2023-04-05 06:26:30.000000 lightapi-0.0.17/README.md
--rw-r--r--   0 jordanplows   (501) staff       (20)      323 2023-04-05 06:27:16.000000 lightapi-0.0.17/pyproject.toml
--rw-r--r--   0 jordanplows   (501) staff       (20)       38 2023-04-05 06:28:00.349861 lightapi-0.0.17/setup.cfg
+drwxr-xr-x   0 jordanplows   (501) staff       (20)        0 2023-04-10 03:49:55.335903 lightapi-0.0.18/
+drwxr-xr-x   0 jordanplows   (501) staff       (20)        0 2023-04-10 03:49:55.335460 lightapi-0.0.18/LightAPI.egg-info/
+-rw-r--r--   0 jordanplows   (501) staff       (20)     1537 2023-04-10 03:49:55.000000 lightapi-0.0.18/LightAPI.egg-info/PKG-INFO
+-rw-r--r--   0 jordanplows   (501) staff       (20)      280 2023-04-10 03:49:55.000000 lightapi-0.0.18/LightAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 jordanplows   (501) staff       (20)        1 2023-04-10 03:49:55.000000 lightapi-0.0.18/LightAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 jordanplows   (501) staff       (20)        1 2023-04-10 03:49:55.000000 lightapi-0.0.18/LightAPI.egg-info/top_level.txt
+-rw-r--r--   0 jordanplows   (501) staff       (20)     1537 2023-04-10 03:49:55.335772 lightapi-0.0.18/PKG-INFO
+-rw-r--r--   0 jordanplows   (501) staff       (20)     1318 2023-04-05 06:26:30.000000 lightapi-0.0.18/README.md
+-rw-r--r--   0 jordanplows   (501) staff       (20)      358 2023-04-10 03:49:48.000000 lightapi-0.0.18/pyproject.toml
+-rw-r--r--   0 jordanplows   (501) staff       (20)       38 2023-04-10 03:49:55.335951 lightapi-0.0.18/setup.cfg
```

### Comparing `lightapi-0.0.17/LightAPI.egg-info/PKG-INFO` & `lightapi-0.0.18/LightAPI.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lightapi
-Version: 0.0.17
+Version: 0.0.18
 Summary: Light API turns LLMs into Autonomous Agents
-Author-email: Light AI <jordan@lightapi.com>
+Author-email: Jordan Plows <jordan@lightapi.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 ## Introduction
 
 Light Assistant powered by LightAI is an AI-powered application designed to help you streamline your work and free up time for more important tasks. It can handle a wide range of tasks, from organizing files to managing your email inbox, scheduling meetings, and much more.
```

### Comparing `lightapi-0.0.17/PKG-INFO` & `lightapi-0.0.18/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lightapi
-Version: 0.0.17
+Version: 0.0.18
 Summary: Light API turns LLMs into Autonomous Agents
-Author-email: Light AI <jordan@lightapi.com>
+Author-email: Jordan Plows <jordan@lightapi.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 ## Introduction
 
 Light Assistant powered by LightAI is an AI-powered application designed to help you streamline your work and free up time for more important tasks. It can handle a wide range of tasks, from organizing files to managing your email inbox, scheduling meetings, and much more.
```

### Comparing `lightapi-0.0.17/README.md` & `lightapi-0.0.18/README.md`

 * *Files identical despite different names*


# Comparing `tmp/abcd_seth-1.0.3.dev0.tar.gz` & `tmp/abcd_seth-1.0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/abcd_seth-1.0.3.dev0.tar", last modified: Mon Apr 10 11:52:08 2023, max compression
+gzip compressed data, was "dist/abcd_seth-1.0.4.dev0.tar", last modified: Mon Apr 10 11:54:40 2023, max compression
```

## Comparing `abcd_seth-1.0.3.dev0.tar` & `abcd_seth-1.0.4.dev0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 daniyarauezkhan   (501) staff       (20)        0 2023-04-10 11:52:08.000000 abcd_seth-1.0.3.dev0/
--rw-r--r--   0 daniyarauezkhan   (501) staff       (20)      449 2023-04-10 11:52:08.000000 abcd_seth-1.0.3.dev0/PKG-INFO
-drwxr-xr-x   0 daniyarauezkhan   (501) staff       (20)        0 2023-04-10 11:52:08.000000 abcd_seth-1.0.3.dev0/abcd_seth/
--rw-r--r--   0 daniyarauezkhan   (501) staff       (20)       57 2023-04-10 11:42:30.000000 abcd_seth-1.0.3.dev0/abcd_seth/__init__.py
-drwxr-xr-x   0 daniyarauezkhan   (501) staff       (20)        0 2023-04-10 11:52:08.000000 abcd_seth-1.0.3.dev0/abcd_seth/dto/
--rw-r--r--   0 daniyarauezkhan   (501) staff       (20)        0 2023-04-10 08:11:11.000000 abcd_seth-1.0.3.dev0/abcd_seth/dto/__init__.py
-drwxr-xr-x   0 daniyarauezkhan   (501) staff       (20)        0 2023-04-10 11:52:08.000000 abcd_seth-1.0.3.dev0/abcd_seth/models/
--rw-r--r--   0 daniyarauezkhan   (501) staff       (20)       57 2023-04-10 11:44:44.000000 abcd_seth-1.0.3.dev0/abcd_seth/models/__init__.py
-drwxr-xr-x   0 daniyarauezkhan   (501) staff       (20)        0 2023-04-10 11:52:08.000000 abcd_seth-1.0.3.dev0/abcd_seth/models/django/
--rw-r--r--   0 daniyarauezkhan   (501) staff       (20)        0 2023-04-10 09:18:22.000000 abcd_seth-1.0.3.dev0/abcd_seth/models/django/__init__.py
--rw-r--r--   0 daniyarauezkhan   (501) staff       (20)     2092 2023-04-10 08:57:29.000000 abcd_seth-1.0.3.dev0/abcd_seth/models/django/user_model.py
-drwxr-xr-x   0 daniyarauezkhan   (501) staff       (20)        0 2023-04-10 11:52:08.000000 abcd_seth-1.0.3.dev0/abcd_seth/models/domain/
--rw-r--r--   0 daniyarauezkhan   (501) staff       (20)       29 2023-04-10 08:14:27.000000 abcd_seth-1.0.3.dev0/abcd_seth/models/domain/__init__.py
--rw-r--r--   0 daniyarauezkhan   (501) staff       (20)      236 2023-04-10 08:11:52.000000 abcd_seth-1.0.3.dev0/abcd_seth/models/domain/user_model.py
-drwxr-xr-x   0 daniyarauezkhan   (501) staff       (20)        0 2023-04-10 11:52:08.000000 abcd_seth-1.0.3.dev0/abcd_seth.egg-info/
--rw-r--r--   0 daniyarauezkhan   (501) staff       (20)      449 2023-04-10 11:52:08.000000 abcd_seth-1.0.3.dev0/abcd_seth.egg-info/PKG-INFO
--rw-r--r--   0 daniyarauezkhan   (501) staff       (20)      365 2023-04-10 11:52:08.000000 abcd_seth-1.0.3.dev0/abcd_seth.egg-info/SOURCES.txt
--rw-r--r--   0 daniyarauezkhan   (501) staff       (20)        1 2023-04-10 11:52:08.000000 abcd_seth-1.0.3.dev0/abcd_seth.egg-info/dependency_links.txt
--rw-r--r--   0 daniyarauezkhan   (501) staff       (20)       10 2023-04-10 11:52:08.000000 abcd_seth-1.0.3.dev0/abcd_seth.egg-info/top_level.txt
--rw-r--r--   0 daniyarauezkhan   (501) staff       (20)       38 2023-04-10 11:52:08.000000 abcd_seth-1.0.3.dev0/setup.cfg
--rw-r--r--   0 daniyarauezkhan   (501) staff       (20)      612 2023-04-10 11:52:07.000000 abcd_seth-1.0.3.dev0/setup.py
+drwxr-xr-x   0 daniyarauezkhan   (501) staff       (20)        0 2023-04-10 11:54:40.000000 abcd_seth-1.0.4.dev0/
+-rw-r--r--   0 daniyarauezkhan   (501) staff       (20)      449 2023-04-10 11:54:40.000000 abcd_seth-1.0.4.dev0/PKG-INFO
+drwxr-xr-x   0 daniyarauezkhan   (501) staff       (20)        0 2023-04-10 11:54:40.000000 abcd_seth-1.0.4.dev0/abcd_seth/
+-rw-r--r--   0 daniyarauezkhan   (501) staff       (20)       57 2023-04-10 11:42:30.000000 abcd_seth-1.0.4.dev0/abcd_seth/__init__.py
+drwxr-xr-x   0 daniyarauezkhan   (501) staff       (20)        0 2023-04-10 11:54:40.000000 abcd_seth-1.0.4.dev0/abcd_seth/dto/
+-rw-r--r--   0 daniyarauezkhan   (501) staff       (20)        0 2023-04-10 08:11:11.000000 abcd_seth-1.0.4.dev0/abcd_seth/dto/__init__.py
+drwxr-xr-x   0 daniyarauezkhan   (501) staff       (20)        0 2023-04-10 11:54:40.000000 abcd_seth-1.0.4.dev0/abcd_seth/models/
+-rw-r--r--   0 daniyarauezkhan   (501) staff       (20)       50 2023-04-10 11:53:50.000000 abcd_seth-1.0.4.dev0/abcd_seth/models/__init__.py
+drwxr-xr-x   0 daniyarauezkhan   (501) staff       (20)        0 2023-04-10 11:54:40.000000 abcd_seth-1.0.4.dev0/abcd_seth/models/django/
+-rw-r--r--   0 daniyarauezkhan   (501) staff       (20)        0 2023-04-10 09:18:22.000000 abcd_seth-1.0.4.dev0/abcd_seth/models/django/__init__.py
+-rw-r--r--   0 daniyarauezkhan   (501) staff       (20)     2092 2023-04-10 08:57:29.000000 abcd_seth-1.0.4.dev0/abcd_seth/models/django/user_model.py
+drwxr-xr-x   0 daniyarauezkhan   (501) staff       (20)        0 2023-04-10 11:54:40.000000 abcd_seth-1.0.4.dev0/abcd_seth/models/domain/
+-rw-r--r--   0 daniyarauezkhan   (501) staff       (20)       29 2023-04-10 08:14:27.000000 abcd_seth-1.0.4.dev0/abcd_seth/models/domain/__init__.py
+-rw-r--r--   0 daniyarauezkhan   (501) staff       (20)      236 2023-04-10 08:11:52.000000 abcd_seth-1.0.4.dev0/abcd_seth/models/domain/user_model.py
+drwxr-xr-x   0 daniyarauezkhan   (501) staff       (20)        0 2023-04-10 11:54:40.000000 abcd_seth-1.0.4.dev0/abcd_seth.egg-info/
+-rw-r--r--   0 daniyarauezkhan   (501) staff       (20)      449 2023-04-10 11:54:40.000000 abcd_seth-1.0.4.dev0/abcd_seth.egg-info/PKG-INFO
+-rw-r--r--   0 daniyarauezkhan   (501) staff       (20)      365 2023-04-10 11:54:40.000000 abcd_seth-1.0.4.dev0/abcd_seth.egg-info/SOURCES.txt
+-rw-r--r--   0 daniyarauezkhan   (501) staff       (20)        1 2023-04-10 11:54:40.000000 abcd_seth-1.0.4.dev0/abcd_seth.egg-info/dependency_links.txt
+-rw-r--r--   0 daniyarauezkhan   (501) staff       (20)       10 2023-04-10 11:54:40.000000 abcd_seth-1.0.4.dev0/abcd_seth.egg-info/top_level.txt
+-rw-r--r--   0 daniyarauezkhan   (501) staff       (20)       38 2023-04-10 11:54:40.000000 abcd_seth-1.0.4.dev0/setup.cfg
+-rw-r--r--   0 daniyarauezkhan   (501) staff       (20)      612 2023-04-10 11:54:25.000000 abcd_seth-1.0.4.dev0/setup.py
```

### Comparing `abcd_seth-1.0.3.dev0/abcd_seth/models/django/user_model.py` & `abcd_seth-1.0.4.dev0/abcd_seth/models/django/user_model.py`

 * *Files identical despite different names*

### Comparing `abcd_seth-1.0.3.dev0/setup.py` & `abcd_seth-1.0.4.dev0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='abcd_seth',
-    version='1.0.3-dev',
+    version='1.0.4-dev',
     description='Shared models for microservices',
     author='Daniyar Auezkhan',
     author_email='nurovich14@gmail.com',
     packages=find_packages(exclude=('tests',)),
     install_requires=[
 
     ],
```


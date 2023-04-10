# Comparing `tmp/alibabacloud_documentautoml20221229-1.0.7.tar.gz` & `tmp/alibabacloud_documentautoml20221229-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_documentautoml20221229-1.0.7.tar", last modified: Fri Mar 31 11:08:58 2023, max compression
+gzip compressed data, was "dist/alibabacloud_documentautoml20221229-1.0.8.tar", last modified: Mon Apr 10 07:44:31 2023, max compression
```

## Comparing `alibabacloud_documentautoml20221229-1.0.7.tar` & `alibabacloud_documentautoml20221229-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:08:58.000000 alibabacloud_documentautoml20221229-1.0.7/
--rw-r--r--   0 root         (0) root         (0)      301 2023-03-31 11:08:58.000000 alibabacloud_documentautoml20221229-1.0.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-31 11:08:58.000000 alibabacloud_documentautoml20221229-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-31 11:08:58.000000 alibabacloud_documentautoml20221229-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2394 2023-03-31 11:08:58.000000 alibabacloud_documentautoml20221229-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1055 2023-03-31 11:08:58.000000 alibabacloud_documentautoml20221229-1.0.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2023-03-31 11:08:58.000000 alibabacloud_documentautoml20221229-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:08:58.000000 alibabacloud_documentautoml20221229-1.0.7/alibabacloud_documentautoml20221229/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-31 11:08:58.000000 alibabacloud_documentautoml20221229-1.0.7/alibabacloud_documentautoml20221229/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18171 2023-03-31 11:08:58.000000 alibabacloud_documentautoml20221229-1.0.7/alibabacloud_documentautoml20221229/client.py
--rw-r--r--   0 root         (0) root         (0)    20554 2023-03-31 11:08:58.000000 alibabacloud_documentautoml20221229-1.0.7/alibabacloud_documentautoml20221229/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:08:58.000000 alibabacloud_documentautoml20221229-1.0.7/alibabacloud_documentautoml20221229.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2394 2023-03-31 11:08:58.000000 alibabacloud_documentautoml20221229-1.0.7/alibabacloud_documentautoml20221229.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      508 2023-03-31 11:08:58.000000 alibabacloud_documentautoml20221229-1.0.7/alibabacloud_documentautoml20221229.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 11:08:58.000000 alibabacloud_documentautoml20221229-1.0.7/alibabacloud_documentautoml20221229.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-31 11:08:58.000000 alibabacloud_documentautoml20221229-1.0.7/alibabacloud_documentautoml20221229.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-03-31 11:08:58.000000 alibabacloud_documentautoml20221229-1.0.7/alibabacloud_documentautoml20221229.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-31 11:08:58.000000 alibabacloud_documentautoml20221229-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2665 2023-03-31 11:08:58.000000 alibabacloud_documentautoml20221229-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)      344 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18171 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229/client.py
+-rw-r--r--   0 root         (0) root         (0)    20554 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      508 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2665 2023-04-10 07:44:31.000000 alibabacloud_documentautoml20221229-1.0.8/setup.py
```

### Comparing `alibabacloud_documentautoml20221229-1.0.7/LICENSE` & `alibabacloud_documentautoml20221229-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_documentautoml20221229-1.0.7/PKG-INFO` & `alibabacloud_documentautoml20221229-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_documentautoml20221229
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud documentAutoml (20221229) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_documentautoml20221229-1.0.7/README-CN.md` & `alibabacloud_documentautoml20221229-1.0.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_documentautoml20221229-1.0.7/README.md` & `alibabacloud_documentautoml20221229-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_documentautoml20221229-1.0.7/alibabacloud_documentautoml20221229/client.py` & `alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_documentautoml20221229-1.0.7/alibabacloud_documentautoml20221229/models.py` & `alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_documentautoml20221229-1.0.7/alibabacloud_documentautoml20221229.egg-info/PKG-INFO` & `alibabacloud_documentautoml20221229-1.0.8/alibabacloud_documentautoml20221229.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-documentautoml20221229
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud documentAutoml (20221229) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_documentautoml20221229-1.0.7/setup.py` & `alibabacloud_documentautoml20221229-1.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_documentautoml20221229.
 
-Created on 31/03/2023
+Created on 10/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_documentautoml20221229"
 NAME = "alibabacloud_documentautoml20221229" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud documentAutoml (20221229) SDK Library for Python"
```


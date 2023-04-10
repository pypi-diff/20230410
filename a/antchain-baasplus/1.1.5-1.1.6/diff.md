# Comparing `tmp/antchain_baasplus-1.1.5.tar.gz` & `tmp/antchain_baasplus-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_baasplus-1.1.5.tar", last modified: Fri Apr  7 08:55:33 2023, max compression
+gzip compressed data, was "dist/antchain_baasplus-1.1.6.tar", last modified: Mon Apr 10 07:03:32 2023, max compression
```

## Comparing `antchain_baasplus-1.1.5.tar` & `antchain_baasplus-1.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 08:55:33.000000 antchain_baasplus-1.1.5/
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-07 08:55:32.000000 antchain_baasplus-1.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-07 08:55:32.000000 antchain_baasplus-1.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2192 2023-04-07 08:55:33.000000 antchain_baasplus-1.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      819 2023-04-07 08:55:32.000000 antchain_baasplus-1.1.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1005 2023-04-07 08:55:32.000000 antchain_baasplus-1.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 08:55:33.000000 antchain_baasplus-1.1.5/antchain_baasplus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2192 2023-04-07 08:55:32.000000 antchain_baasplus-1.1.5/antchain_baasplus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2023-04-07 08:55:32.000000 antchain_baasplus-1.1.5/antchain_baasplus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 08:55:32.000000 antchain_baasplus-1.1.5/antchain_baasplus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-07 08:55:32.000000 antchain_baasplus-1.1.5/antchain_baasplus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-07 08:55:32.000000 antchain_baasplus-1.1.5/antchain_baasplus.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 08:55:33.000000 antchain_baasplus-1.1.5/antchain_sdk_baasplus/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-07 08:55:32.000000 antchain_baasplus-1.1.5/antchain_sdk_baasplus/__init__.py
--rw-r--r--   0 root         (0) root         (0)   204189 2023-04-07 08:55:32.000000 antchain_baasplus-1.1.5/antchain_sdk_baasplus/client.py
--rw-r--r--   0 root         (0) root         (0)   349423 2023-04-07 08:55:32.000000 antchain_baasplus-1.1.5/antchain_sdk_baasplus/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-07 08:55:33.000000 antchain_baasplus-1.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2513 2023-04-07 08:55:32.000000 antchain_baasplus-1.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:03:32.000000 antchain_baasplus-1.1.6/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-04-10 07:03:32.000000 antchain_baasplus-1.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      819 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:03:32.000000 antchain_baasplus-1.1.6/antchain_baasplus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/antchain_baasplus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2023-04-10 07:03:32.000000 antchain_baasplus-1.1.6/antchain_baasplus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/antchain_baasplus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/antchain_baasplus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/antchain_baasplus.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:03:32.000000 antchain_baasplus-1.1.6/antchain_sdk_baasplus/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/antchain_sdk_baasplus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   204189 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/antchain_sdk_baasplus/client.py
+-rw-r--r--   0 root         (0) root         (0)   349423 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/antchain_sdk_baasplus/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-10 07:03:32.000000 antchain_baasplus-1.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-04-10 07:03:31.000000 antchain_baasplus-1.1.6/setup.py
```

### Comparing `antchain_baasplus-1.1.5/LICENSE` & `antchain_baasplus-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_baasplus-1.1.5/PKG-INFO` & `antchain_baasplus-1.1.6/antchain_baasplus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_baasplus
-Version: 1.1.5
+Name: antchain-baasplus
+Version: 1.1.6
 Summary: Ant Chain BAASPLUS SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_baasplus-1.1.5/README-CN.md` & `antchain_baasplus-1.1.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_baasplus-1.1.5/README.md` & `antchain_baasplus-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `antchain_baasplus-1.1.5/antchain_baasplus.egg-info/PKG-INFO` & `antchain_baasplus-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-baasplus
-Version: 1.1.5
+Name: antchain_baasplus
+Version: 1.1.6
 Summary: Ant Chain BAASPLUS SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_baasplus-1.1.5/antchain_sdk_baasplus/client.py` & `antchain_baasplus-1.1.6/antchain_sdk_baasplus/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.1.5',
+                    'sdk_version': '1.1.6',
                     '_prod_code': 'BAASPLUS',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.1.5',
+                    'sdk_version': '1.1.6',
                     '_prod_code': 'BAASPLUS',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_baasplus-1.1.5/antchain_sdk_baasplus/models.py` & `antchain_baasplus-1.1.6/antchain_sdk_baasplus/models.py`

 * *Files identical despite different names*

### Comparing `antchain_baasplus-1.1.5/setup.py` & `antchain_baasplus-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_baasplus.
 
-Created on 07/04/2023
+Created on 10/04/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_baasplus"
 NAME = "antchain_baasplus" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain BAASPLUS SDK Library for Python"
```


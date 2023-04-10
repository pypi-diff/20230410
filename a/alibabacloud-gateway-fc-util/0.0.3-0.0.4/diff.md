# Comparing `tmp/alibabacloud_gateway_fc_util-0.0.3.tar.gz` & `tmp/alibabacloud_gateway_fc_util-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_gateway_fc_util-0.0.3.tar", last modified: Wed Jun 15 10:33:02 2022, max compression
+gzip compressed data, was "dist/alibabacloud_gateway_fc_util-0.0.4.tar", last modified: Mon Apr 10 13:03:58 2023, max compression
```

## Comparing `alibabacloud_gateway_fc_util-0.0.3.tar` & `alibabacloud_gateway_fc_util-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 10:33:02.000000 alibabacloud_gateway_fc_util-0.0.3/
--rw-r--r--   0 root         (0) root         (0)     3877 2022-06-15 10:33:02.000000 alibabacloud_gateway_fc_util-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2270 2022-06-15 10:33:02.000000 alibabacloud_gateway_fc_util-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 10:33:02.000000 alibabacloud_gateway_fc_util-0.0.3/alibabacloud_gateway_fc_util/
--rw-r--r--   0 root         (0) root         (0)       22 2022-06-15 10:33:02.000000 alibabacloud_gateway_fc_util-0.0.3/alibabacloud_gateway_fc_util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8786 2022-06-15 10:33:02.000000 alibabacloud_gateway_fc_util-0.0.3/alibabacloud_gateway_fc_util/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 10:33:02.000000 alibabacloud_gateway_fc_util-0.0.3/alibabacloud_gateway_fc_util.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3877 2022-06-15 10:33:02.000000 alibabacloud_gateway_fc_util-0.0.3/alibabacloud_gateway_fc_util.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      357 2022-06-15 10:33:02.000000 alibabacloud_gateway_fc_util-0.0.3/alibabacloud_gateway_fc_util.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-15 10:33:02.000000 alibabacloud_gateway_fc_util-0.0.3/alibabacloud_gateway_fc_util.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2022-06-15 10:33:02.000000 alibabacloud_gateway_fc_util-0.0.3/alibabacloud_gateway_fc_util.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2022-06-15 10:33:02.000000 alibabacloud_gateway_fc_util-0.0.3/alibabacloud_gateway_fc_util.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-15 10:33:02.000000 alibabacloud_gateway_fc_util-0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2507 2022-06-15 10:33:02.000000 alibabacloud_gateway_fc_util-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 13:03:58.000000 alibabacloud_gateway_fc_util-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)     3868 2023-04-10 13:03:58.000000 alibabacloud_gateway_fc_util-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2229 2023-04-10 13:03:57.000000 alibabacloud_gateway_fc_util-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 13:03:58.000000 alibabacloud_gateway_fc_util-0.0.4/alibabacloud_gateway_fc_util/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-10 13:03:57.000000 alibabacloud_gateway_fc_util-0.0.4/alibabacloud_gateway_fc_util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8786 2023-04-10 13:03:57.000000 alibabacloud_gateway_fc_util-0.0.4/alibabacloud_gateway_fc_util/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 13:03:58.000000 alibabacloud_gateway_fc_util-0.0.4/alibabacloud_gateway_fc_util.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3868 2023-04-10 13:03:58.000000 alibabacloud_gateway_fc_util-0.0.4/alibabacloud_gateway_fc_util.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      357 2023-04-10 13:03:58.000000 alibabacloud_gateway_fc_util-0.0.4/alibabacloud_gateway_fc_util.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 13:03:58.000000 alibabacloud_gateway_fc_util-0.0.4/alibabacloud_gateway_fc_util.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-10 13:03:58.000000 alibabacloud_gateway_fc_util-0.0.4/alibabacloud_gateway_fc_util.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-10 13:03:58.000000 alibabacloud_gateway_fc_util-0.0.4/alibabacloud_gateway_fc_util.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 13:03:58.000000 alibabacloud_gateway_fc_util-0.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2507 2023-04-10 13:03:57.000000 alibabacloud_gateway_fc_util-0.0.4/setup.py
```

### Comparing `alibabacloud_gateway_fc_util-0.0.3/PKG-INFO` & `alibabacloud_gateway_fc_util-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_gateway_fc_util
-Version: 0.0.3
+Version: 0.0.4
 Summary: Alibaba Cloud FC Util Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-gateway
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: ## README
         
@@ -26,20 +26,21 @@
         import os
         
         from alibabacloud_fc_open20210406.client import Client
         from alibabacloud_tea_openapi import models as open_api_models
         
         ak = os.getenv('ak')
         sk = os.getenv('sk')
+        url = os.getenv('url')
         
         client = Client(config=open_api_models.Config(access_key_id=ak,
                                                       access_key_secret=sk,
                                                       region_id='cn-hangzhou'))
         
-        resp = client.invoke_httptrigger(url="https://xxx.fcapp.run/action?key=value",
+        resp = client.invoke_httptrigger(url=url,
                                          method="GET", 
                                          body="anything".encode(encoding='utf-8'),
                                          headers={"k1": "v1", "k2": "v2"})
         ```
         
         + Invoke Anonymous HTTP Trigger
         
@@ -47,20 +48,21 @@
         import os
         
         from alibabacloud_fc_open20210406.client import Client
         from alibabacloud_tea_openapi import models as open_api_models
         
         ak = os.getenv('ak')
         sk = os.getenv('sk')
+        url = os.getenv('url')
         
         client = Client(config=open_api_models.Config(access_key_id=ak,
                                                       access_key_secret=sk,
                                                       region_id='cn-hangzhou'))
         
-        resp = client.invoke_anonymous_httptrigger(url="https://xxx.fcapp.run/action?key=value",
+        resp = client.invoke_anonymous_httptrigger(url=url,
                                          method="GET", 
                                          body="anything".encode(encoding='utf-8'),
                                          headers={"k1": "v1", "k2": "v2"})
         
         
         ```
         
@@ -73,21 +75,23 @@
         import os
         
         from alibabacloud_fc_open20210406.client import Client
         from alibabacloud_tea_openapi import models as open_api_models
         
         ak = os.getenv('ak')
         sk = os.getenv('sk')
+        url = os.getenv('url')
+        
         client = Client(config=open_api_models.Config(access_key_id=ak,
                                                       access_key_secret=sk,
                                                       region_id='cn-hangzhou'))
         
         # build your own request
         req = requests.Request(
-            url='https://xxx.fcapp.run/action?key=value',
+            url=url,
             method='GET'
         )
         req = client.sign_request(req)
         with requests.Session() as s:
             prep=s.prepare_request(req)
             resp = s.send(prep)
```

### Comparing `alibabacloud_gateway_fc_util-0.0.3/README.md` & `alibabacloud_gateway_fc_util-0.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -18,20 +18,21 @@
 import os
 
 from alibabacloud_fc_open20210406.client import Client
 from alibabacloud_tea_openapi import models as open_api_models
 
 ak = os.getenv('ak')
 sk = os.getenv('sk')
+url = os.getenv('url')
 
 client = Client(config=open_api_models.Config(access_key_id=ak,
                                               access_key_secret=sk,
                                               region_id='cn-hangzhou'))
 
-resp = client.invoke_httptrigger(url="https://xxx.fcapp.run/action?key=value",
+resp = client.invoke_httptrigger(url=url,
                                  method="GET", 
                                  body="anything".encode(encoding='utf-8'),
                                  headers={"k1": "v1", "k2": "v2"})
 ```
 
 + Invoke Anonymous HTTP Trigger
 
@@ -39,20 +40,21 @@
 import os
 
 from alibabacloud_fc_open20210406.client import Client
 from alibabacloud_tea_openapi import models as open_api_models
 
 ak = os.getenv('ak')
 sk = os.getenv('sk')
+url = os.getenv('url')
 
 client = Client(config=open_api_models.Config(access_key_id=ak,
                                               access_key_secret=sk,
                                               region_id='cn-hangzhou'))
 
-resp = client.invoke_anonymous_httptrigger(url="https://xxx.fcapp.run/action?key=value",
+resp = client.invoke_anonymous_httptrigger(url=url,
                                  method="GET", 
                                  body="anything".encode(encoding='utf-8'),
                                  headers={"k1": "v1", "k2": "v2"})
 
 
 ```
 
@@ -65,21 +67,23 @@
 import os
 
 from alibabacloud_fc_open20210406.client import Client
 from alibabacloud_tea_openapi import models as open_api_models
 
 ak = os.getenv('ak')
 sk = os.getenv('sk')
+url = os.getenv('url')
+
 client = Client(config=open_api_models.Config(access_key_id=ak,
                                               access_key_secret=sk,
                                               region_id='cn-hangzhou'))
 
 # build your own request
 req = requests.Request(
-    url='https://xxx.fcapp.run/action?key=value',
+    url=url,
     method='GET'
 )
 req = client.sign_request(req)
 with requests.Session() as s:
     prep=s.prepare_request(req)
     resp = s.send(prep)
```

### Comparing `alibabacloud_gateway_fc_util-0.0.3/alibabacloud_gateway_fc_util/client.py` & `alibabacloud_gateway_fc_util-0.0.4/alibabacloud_gateway_fc_util/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_gateway_fc_util-0.0.3/setup.py` & `alibabacloud_gateway_fc_util-0.0.4/setup.py`

 * *Files identical despite different names*


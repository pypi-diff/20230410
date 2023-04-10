# Comparing `tmp/pynocaptcha-1.3.8.tar.gz` & `tmp/pynocaptcha-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pynocaptcha-1.3.8.tar", last modified: Sun Apr  9 06:11:43 2023, max compression
+gzip compressed data, was "dist/pynocaptcha-1.4.1.tar", last modified: Mon Apr 10 09:55:59 2023, max compression
```

## Comparing `pynocaptcha-1.3.8.tar` & `pynocaptcha-1.4.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-09 06:11:43.000000 pynocaptcha-1.3.8/
--rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-04-09 06:11:43.000000 pynocaptcha-1.3.8/PKG-INFO
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-09 06:11:43.000000 pynocaptcha-1.3.8/pynocaptcha/
--rw-r--r--   0 esbiya     (501) staff       (20)      440 2023-04-04 08:12:16.000000 pynocaptcha-1.3.8/pynocaptcha/__init__.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-09 06:11:43.000000 pynocaptcha-1.3.8/pynocaptcha/crackers/
--rw-r--r--   0 esbiya     (501) staff       (20)     3602 2023-04-09 05:43:24.000000 pynocaptcha-1.3.8/pynocaptcha/crackers/base.py
--rw-r--r--   0 esbiya     (501) staff       (20)     5367 2023-04-03 02:00:17.000000 pynocaptcha-1.3.8/pynocaptcha/crackers/cloudflare.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.3.8/pynocaptcha/crackers/hcaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1454 2023-03-20 05:38:09.000000 pynocaptcha-1.3.8/pynocaptcha/crackers/incapsula.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2893 2023-03-24 04:08:51.000000 pynocaptcha-1.3.8/pynocaptcha/crackers/recaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-04-09 06:11:42.000000 pynocaptcha-1.3.8/setup.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-10 09:55:59.000000 pynocaptcha-1.4.1/
+-rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-04-10 09:55:59.000000 pynocaptcha-1.4.1/PKG-INFO
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-10 09:55:59.000000 pynocaptcha-1.4.1/pynocaptcha/
+-rw-r--r--   0 esbiya     (501) staff       (20)      440 2023-04-04 08:12:16.000000 pynocaptcha-1.4.1/pynocaptcha/__init__.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-10 09:55:59.000000 pynocaptcha-1.4.1/pynocaptcha/crackers/
+-rw-r--r--   0 esbiya     (501) staff       (20)     4243 2023-04-10 09:54:53.000000 pynocaptcha-1.4.1/pynocaptcha/crackers/base.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     5440 2023-04-10 09:55:20.000000 pynocaptcha-1.4.1/pynocaptcha/crackers/cloudflare.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.4.1/pynocaptcha/crackers/hcaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1454 2023-04-10 03:49:32.000000 pynocaptcha-1.4.1/pynocaptcha/crackers/incapsula.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2893 2023-03-24 04:08:51.000000 pynocaptcha-1.4.1/pynocaptcha/crackers/recaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-04-10 09:55:49.000000 pynocaptcha-1.4.1/setup.py
```

### Comparing `pynocaptcha-1.3.8/PKG-INFO` & `pynocaptcha-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pynocaptcha
-Version: 1.3.8
+Version: 1.4.1
 Summary: nocaptcha.io api
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: nocaptcha.io python api
 Keywords: nocaptcha
```

### Comparing `pynocaptcha-1.3.8/pynocaptcha/crackers/base.py` & `pynocaptcha-1.4.1/pynocaptcha/crackers/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 import requests
+import traceback
 from loguru import logger
 from typing import Any
 
 
 class BaseCracker:
     
     # 破解器
@@ -14,19 +15,22 @@
     
     # 必须参数列表
     must_check_params = []
     
     # 可选参数
     option_params = {}
     
+    # 需要删除的多余参数
+    delete_params = []
+    
     def __init__(
         self,    
         user_token: str = None,
-        developer_id: str = "",   
-        user_agent: str = "",
+        developer_id: str = None,   
+        user_agent: str = None,
         proxy: str = None, 
         timeout: int = 30,
         debug: bool = False,
         check_useful: bool = False,
         max_retry_times: int = 3,
         internal_proxy=True,
         **kwargs
@@ -62,14 +66,18 @@
             setattr(self, k, v)
             self.wanda_args.update({ k: v })
         for k, v in self.option_params.items():
             _v = kwargs.get(k, v)
             if not hasattr(self, k) or getattr(self, k) is None:
                 setattr(self, k, _v)
             self.wanda_args.update({ k: _v })
+        
+        for k in self.delete_params:
+            if k in self.wanda_args:
+                del self.wanda_args[k]
 
         if not all(getattr(self, k) for k in self.must_check_params):
            raise AttributeError("缺少参数, 请检查")
 
     def response(self, result: Any):
         return result
         
@@ -78,19 +86,32 @@
     
     def crack(self):
         headers = {
             "User-Token": self.user_token
         }
         if self.developer_id:
             headers["Developer-Id"] = self.developer_id
-        resp = requests.post(f"http://api.nocaptcha.io/api/wanda/{self.cracker_name}/{self.cracker_version}", headers=headers, json={
-            **self.wanda_args,
-            "user_agent": self.user_agent,
-            "proxy": self.proxy
-        }, timeout=self.timeout).json()
+        
+        if self.user_agent:
+            self.wanda_args["user_agent"] = self.user_agent
+        if self.proxy:
+            self.wanda_args["proxy"] = self.proxy
+        
+        while 1:
+            if self.retry_times < self.max_retry_times:
+                try:
+                    resp = requests.post(
+                        f"http://api.nocaptcha.io/api/wanda/{self.cracker_name}/{self.cracker_version}", 
+                        headers=headers, json=self.wanda_args, timeout=self.timeout
+                    ).json()
+                    break
+                except Exception as e:
+                    if self.debug:
+                        logger.error(e)
+                    self.retry_times += 1
         if self.debug:
             logger.info(resp)
         wanda_ret = resp.get("data")
         if not wanda_ret:
             if self.debug:
                 logger.error(resp.get("msg"))
             return
```

### Comparing `pynocaptcha-1.3.8/pynocaptcha/crackers/cloudflare.py` & `pynocaptcha-1.4.1/pynocaptcha/crackers/cloudflare.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,16 @@
         "user_agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:109.0) Gecko/20100101 Firefox/110.0",
         "html": "",
         "headers": {},
         "cookies": {},
         "ja3": "",
         "auto_alpha": True
     }
+    # 需要删除的多余参数
+    delete_params = ["internal_proxy"]
 
     @staticmethod
     def parse_proxy(proxy):
         _auth, _proxy = None, None
         if proxy:
             _proxy = proxy.split("/")[-1]
             if "@" in _proxy:
```

### Comparing `pynocaptcha-1.3.8/pynocaptcha/crackers/hcaptcha.py` & `pynocaptcha-1.4.1/pynocaptcha/crackers/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.3.8/pynocaptcha/crackers/incapsula.py` & `pynocaptcha-1.4.1/pynocaptcha/crackers/incapsula.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.3.8/pynocaptcha/crackers/recaptcha.py` & `pynocaptcha-1.4.1/pynocaptcha/crackers/recaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.3.8/setup.py` & `pynocaptcha-1.4.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 
 setup(
     name='pynocaptcha',
-    version='1.3.8',
+    version='1.4.1',
     description='nocaptcha.io api',
     long_description='nocaptcha.io python api',
     install_requires=["pyhttpx", "loguru"],
     license='MIT',
     packages=["pynocaptcha/crackers", "pynocaptcha"],
     package_dir={'pynocaptcha': 'pynocaptcha'},
     platforms=["all"],
```


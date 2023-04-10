# Comparing `tmp/antchain_identitymarriage-1.0.3.tar.gz` & `tmp/antchain_identitymarriage-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_identitymarriage-1.0.3.tar", last modified: Mon Apr  3 08:39:54 2023, max compression
+gzip compressed data, was "dist/antchain_identitymarriage-1.0.4.tar", last modified: Mon Apr 10 07:54:00 2023, max compression
```

## Comparing `antchain_identitymarriage-1.0.3.tar` & `antchain_identitymarriage-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:39:54.000000 antchain_identitymarriage-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-03 08:39:53.000000 antchain_identitymarriage-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-03 08:39:53.000000 antchain_identitymarriage-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2240 2023-04-03 08:39:54.000000 antchain_identitymarriage-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      843 2023-04-03 08:39:53.000000 antchain_identitymarriage-1.0.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1029 2023-04-03 08:39:53.000000 antchain_identitymarriage-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:39:54.000000 antchain_identitymarriage-1.0.3/antchain_identitymarriage.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2240 2023-04-03 08:39:54.000000 antchain_identitymarriage-1.0.3/antchain_identitymarriage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      427 2023-04-03 08:39:54.000000 antchain_identitymarriage-1.0.3/antchain_identitymarriage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 08:39:54.000000 antchain_identitymarriage-1.0.3/antchain_identitymarriage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-03 08:39:54.000000 antchain_identitymarriage-1.0.3/antchain_identitymarriage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-03 08:39:54.000000 antchain_identitymarriage-1.0.3/antchain_identitymarriage.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 08:39:54.000000 antchain_identitymarriage-1.0.3/antchain_sdk_identitymarriage/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-03 08:39:53.000000 antchain_identitymarriage-1.0.3/antchain_sdk_identitymarriage/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17083 2023-04-03 08:39:53.000000 antchain_identitymarriage-1.0.3/antchain_sdk_identitymarriage/client.py
--rw-r--r--   0 root         (0) root         (0)    11788 2023-04-03 08:39:53.000000 antchain_identitymarriage-1.0.3/antchain_sdk_identitymarriage/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-03 08:39:54.000000 antchain_identitymarriage-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2553 2023-04-03 08:39:53.000000 antchain_identitymarriage-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:54:00.000000 antchain_identitymarriage-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-10 07:53:59.000000 antchain_identitymarriage-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-10 07:53:59.000000 antchain_identitymarriage-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2240 2023-04-10 07:54:00.000000 antchain_identitymarriage-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      843 2023-04-10 07:53:59.000000 antchain_identitymarriage-1.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-04-10 07:53:59.000000 antchain_identitymarriage-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:54:00.000000 antchain_identitymarriage-1.0.4/antchain_identitymarriage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2240 2023-04-10 07:54:00.000000 antchain_identitymarriage-1.0.4/antchain_identitymarriage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      427 2023-04-10 07:54:00.000000 antchain_identitymarriage-1.0.4/antchain_identitymarriage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 07:54:00.000000 antchain_identitymarriage-1.0.4/antchain_identitymarriage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-04-10 07:54:00.000000 antchain_identitymarriage-1.0.4/antchain_identitymarriage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-10 07:54:00.000000 antchain_identitymarriage-1.0.4/antchain_identitymarriage.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:54:00.000000 antchain_identitymarriage-1.0.4/antchain_sdk_identitymarriage/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-10 07:53:59.000000 antchain_identitymarriage-1.0.4/antchain_sdk_identitymarriage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19253 2023-04-10 07:53:59.000000 antchain_identitymarriage-1.0.4/antchain_sdk_identitymarriage/client.py
+-rw-r--r--   0 root         (0) root         (0)    14848 2023-04-10 07:53:59.000000 antchain_identitymarriage-1.0.4/antchain_sdk_identitymarriage/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-10 07:54:00.000000 antchain_identitymarriage-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2553 2023-04-10 07:53:59.000000 antchain_identitymarriage-1.0.4/setup.py
```

### Comparing `antchain_identitymarriage-1.0.3/LICENSE` & `antchain_identitymarriage-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_identitymarriage-1.0.3/PKG-INFO` & `antchain_identitymarriage-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_identitymarriage
-Version: 1.0.3
+Version: 1.0.4
 Summary: Ant Chain IDENTITYMARRIAGE SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_identitymarriage-1.0.3/README-CN.md` & `antchain_identitymarriage-1.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_identitymarriage-1.0.3/README.md` & `antchain_identitymarriage-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `antchain_identitymarriage-1.0.3/antchain_identitymarriage.egg-info/PKG-INFO` & `antchain_identitymarriage-1.0.4/antchain_identitymarriage.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-identitymarriage
-Version: 1.0.3
+Version: 1.0.4
 Summary: Ant Chain IDENTITYMARRIAGE SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_identitymarriage-1.0.3/antchain_sdk_identitymarriage/client.py` & `antchain_identitymarriage-1.0.4/antchain_sdk_identitymarriage/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.3',
+                    'sdk_version': '1.0.4',
                     '_prod_code': 'IDENTITYMARRIAGE',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -233,15 +233,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.3',
+                    'sdk_version': '1.0.4',
                     '_prod_code': 'IDENTITYMARRIAGE',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -380,7 +380,63 @@
         Summary: 婚姻状况通知
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             identitymarriage_models.NotifyMarriageInfoResponse(),
             await self.do_request_async('1.0', 'identity.marriage.marriage.info.notify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
+
+    def upload_file_data(
+        self,
+        request: identitymarriage_models.UploadFileDataRequest,
+    ) -> identitymarriage_models.UploadFileDataResponse:
+        """
+        Description: 核婚授权文件上传
+        Summary: 核婚授权文件上传
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.upload_file_data_ex(request, headers, runtime)
+
+    async def upload_file_data_async(
+        self,
+        request: identitymarriage_models.UploadFileDataRequest,
+    ) -> identitymarriage_models.UploadFileDataResponse:
+        """
+        Description: 核婚授权文件上传
+        Summary: 核婚授权文件上传
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.upload_file_data_ex_async(request, headers, runtime)
+
+    def upload_file_data_ex(
+        self,
+        request: identitymarriage_models.UploadFileDataRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> identitymarriage_models.UploadFileDataResponse:
+        """
+        Description: 核婚授权文件上传
+        Summary: 核婚授权文件上传
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            identitymarriage_models.UploadFileDataResponse(),
+            self.do_request('1.0', 'identity.marriage.file.data.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def upload_file_data_ex_async(
+        self,
+        request: identitymarriage_models.UploadFileDataRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> identitymarriage_models.UploadFileDataResponse:
+        """
+        Description: 核婚授权文件上传
+        Summary: 核婚授权文件上传
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            identitymarriage_models.UploadFileDataResponse(),
+            await self.do_request_async('1.0', 'identity.marriage.file.data.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
```

### Comparing `antchain_identitymarriage-1.0.3/antchain_sdk_identitymarriage/models.py` & `antchain_identitymarriage-1.0.4/antchain_sdk_identitymarriage/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -329,7 +329,105 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('data') is not None:
             self.data = m.get('data')
         return self
 
 
+class UploadFileDataRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        file_name: str = None,
+        file: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 文件名
+        self.file_name = file_name
+        # 文件流
+        self.file = file
+
+    def validate(self):
+        self.validate_required(self.file_name, 'file_name')
+        self.validate_required(self.file, 'file')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.file_name is not None:
+            result['file_name'] = self.file_name
+        if self.file is not None:
+            result['file'] = self.file
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('file_name') is not None:
+            self.file_name = m.get('file_name')
+        if m.get('file') is not None:
+            self.file = m.get('file')
+        return self
+
+
+class UploadFileDataResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        data: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # xxx
+        self.data = data
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.data is not None:
+            result['data'] = self.data
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('data') is not None:
+            self.data = m.get('data')
+        return self
+
+
```

### Comparing `antchain_identitymarriage-1.0.3/setup.py` & `antchain_identitymarriage-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_identitymarriage.
 
-Created on 03/04/2023
+Created on 10/04/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_identitymarriage"
 NAME = "antchain_identitymarriage" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain IDENTITYMARRIAGE SDK Library for Python"
```


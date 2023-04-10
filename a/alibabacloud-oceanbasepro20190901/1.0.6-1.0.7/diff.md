# Comparing `tmp/alibabacloud_oceanbasepro20190901-1.0.6.tar.gz` & `tmp/alibabacloud_oceanbasepro20190901-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_oceanbasepro20190901-1.0.6.tar", last modified: Fri Mar  3 08:02:55 2023, max compression
+gzip compressed data, was "dist/alibabacloud_oceanbasepro20190901-1.0.7.tar", last modified: Mon Apr 10 03:09:53 2023, max compression
```

## Comparing `alibabacloud_oceanbasepro20190901-1.0.6.tar` & `alibabacloud_oceanbasepro20190901-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 08:02:55.000000 alibabacloud_oceanbasepro20190901-1.0.6/
--rw-r--r--   0 root         (0) root         (0)      206 2023-03-03 08:02:55.000000 alibabacloud_oceanbasepro20190901-1.0.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-03 08:02:55.000000 alibabacloud_oceanbasepro20190901-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-03 08:02:55.000000 alibabacloud_oceanbasepro20190901-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2382 2023-03-03 08:02:55.000000 alibabacloud_oceanbasepro20190901-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1049 2023-03-03 08:02:55.000000 alibabacloud_oceanbasepro20190901-1.0.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1134 2023-03-03 08:02:55.000000 alibabacloud_oceanbasepro20190901-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 08:02:55.000000 alibabacloud_oceanbasepro20190901-1.0.6/alibabacloud_oceanbasepro20190901/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-03 08:02:55.000000 alibabacloud_oceanbasepro20190901-1.0.6/alibabacloud_oceanbasepro20190901/__init__.py
--rw-r--r--   0 root         (0) root         (0)   259556 2023-03-03 08:02:55.000000 alibabacloud_oceanbasepro20190901-1.0.6/alibabacloud_oceanbasepro20190901/client.py
--rw-r--r--   0 root         (0) root         (0)   782968 2023-03-03 08:02:55.000000 alibabacloud_oceanbasepro20190901-1.0.6/alibabacloud_oceanbasepro20190901/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 08:02:55.000000 alibabacloud_oceanbasepro20190901-1.0.6/alibabacloud_oceanbasepro20190901.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2382 2023-03-03 08:02:55.000000 alibabacloud_oceanbasepro20190901-1.0.6/alibabacloud_oceanbasepro20190901.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      492 2023-03-03 08:02:55.000000 alibabacloud_oceanbasepro20190901-1.0.6/alibabacloud_oceanbasepro20190901.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-03 08:02:55.000000 alibabacloud_oceanbasepro20190901-1.0.6/alibabacloud_oceanbasepro20190901.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-03 08:02:55.000000 alibabacloud_oceanbasepro20190901-1.0.6/alibabacloud_oceanbasepro20190901.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-03-03 08:02:55.000000 alibabacloud_oceanbasepro20190901-1.0.6/alibabacloud_oceanbasepro20190901.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-03 08:02:55.000000 alibabacloud_oceanbasepro20190901-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2655 2023-03-03 08:02:55.000000 alibabacloud_oceanbasepro20190901-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2382 2023-04-10 03:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1049 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   265912 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901/client.py
+-rw-r--r--   0 root         (0) root         (0)   791228 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2382 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      492 2023-04-10 03:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-10 03:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-04-10 03:09:52.000000 alibabacloud_oceanbasepro20190901-1.0.7/setup.py
```

### Comparing `alibabacloud_oceanbasepro20190901-1.0.6/LICENSE` & `alibabacloud_oceanbasepro20190901-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901-1.0.6/PKG-INFO` & `alibabacloud_oceanbasepro20190901-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_oceanbasepro20190901
-Version: 1.0.6
+Version: 1.0.7
 Summary: Alibaba Cloud OceanBasePro (20190901) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oceanbasepro20190901-1.0.6/README-CN.md` & `alibabacloud_oceanbasepro20190901-1.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901-1.0.6/README.md` & `alibabacloud_oceanbasepro20190901-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901-1.0.6/alibabacloud_oceanbasepro20190901/client.py` & `alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -794,14 +794,16 @@
         request: ocean_base_pro_20190901_models.CreateTenantUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocean_base_pro_20190901_models.CreateTenantUserResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
+        if not UtilClient.is_unset(request.encryption_type):
+            body['EncryptionType'] = request.encryption_type
         if not UtilClient.is_unset(request.instance_id):
             body['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.roles):
             body['Roles'] = request.roles
         if not UtilClient.is_unset(request.tenant_id):
             body['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.user_name):
@@ -834,14 +836,16 @@
         request: ocean_base_pro_20190901_models.CreateTenantUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocean_base_pro_20190901_models.CreateTenantUserResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
+        if not UtilClient.is_unset(request.encryption_type):
+            body['EncryptionType'] = request.encryption_type
         if not UtilClient.is_unset(request.instance_id):
             body['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.roles):
             body['Roles'] = request.roles
         if not UtilClient.is_unset(request.tenant_id):
             body['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.user_name):
@@ -4615,14 +4619,166 @@
     async def modify_instance_name_async(
         self,
         request: ocean_base_pro_20190901_models.ModifyInstanceNameRequest,
     ) -> ocean_base_pro_20190901_models.ModifyInstanceNameResponse:
         runtime = util_models.RuntimeOptions()
         return await self.modify_instance_name_with_options_async(request, runtime)
 
+    def modify_instance_node_num_with_options(
+        self,
+        request: ocean_base_pro_20190901_models.ModifyInstanceNodeNumRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.ModifyInstanceNodeNumResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_num):
+            body['NodeNum'] = request.node_num
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ModifyInstanceNodeNum',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.ModifyInstanceNodeNumResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def modify_instance_node_num_with_options_async(
+        self,
+        request: ocean_base_pro_20190901_models.ModifyInstanceNodeNumRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.ModifyInstanceNodeNumResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_num):
+            body['NodeNum'] = request.node_num
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ModifyInstanceNodeNum',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.ModifyInstanceNodeNumResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def modify_instance_node_num(
+        self,
+        request: ocean_base_pro_20190901_models.ModifyInstanceNodeNumRequest,
+    ) -> ocean_base_pro_20190901_models.ModifyInstanceNodeNumResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.modify_instance_node_num_with_options(request, runtime)
+
+    async def modify_instance_node_num_async(
+        self,
+        request: ocean_base_pro_20190901_models.ModifyInstanceNodeNumRequest,
+    ) -> ocean_base_pro_20190901_models.ModifyInstanceNodeNumResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.modify_instance_node_num_with_options_async(request, runtime)
+
+    def modify_instance_spec_with_options(
+        self,
+        request: ocean_base_pro_20190901_models.ModifyInstanceSpecRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.ModifyInstanceSpecResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.disk_size):
+            body['DiskSize'] = request.disk_size
+        if not UtilClient.is_unset(request.instance_class):
+            body['InstanceClass'] = request.instance_class
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ModifyInstanceSpec',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.ModifyInstanceSpecResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def modify_instance_spec_with_options_async(
+        self,
+        request: ocean_base_pro_20190901_models.ModifyInstanceSpecRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.ModifyInstanceSpecResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.disk_size):
+            body['DiskSize'] = request.disk_size
+        if not UtilClient.is_unset(request.instance_class):
+            body['InstanceClass'] = request.instance_class
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ModifyInstanceSpec',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.ModifyInstanceSpecResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def modify_instance_spec(
+        self,
+        request: ocean_base_pro_20190901_models.ModifyInstanceSpecRequest,
+    ) -> ocean_base_pro_20190901_models.ModifyInstanceSpecResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.modify_instance_spec_with_options(request, runtime)
+
+    async def modify_instance_spec_async(
+        self,
+        request: ocean_base_pro_20190901_models.ModifyInstanceSpecRequest,
+    ) -> ocean_base_pro_20190901_models.ModifyInstanceSpecResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.modify_instance_spec_with_options_async(request, runtime)
+
     def modify_instance_tags_with_options(
         self,
         request: ocean_base_pro_20190901_models.ModifyInstanceTagsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocean_base_pro_20190901_models.ModifyInstanceTagsResponse:
         UtilClient.validate_model(request)
         body = {}
```

### Comparing `alibabacloud_oceanbasepro20190901-1.0.6/alibabacloud_oceanbasepro20190901/models.py` & `alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2069,23 +2069,25 @@
         return self
 
 
 class CreateTenantUserRequest(TeaModel):
     def __init__(
         self,
         description: str = None,
+        encryption_type: str = None,
         instance_id: str = None,
         roles: str = None,
         tenant_id: str = None,
         user_name: str = None,
         user_password: str = None,
         user_type: str = None,
     ):
         # The description of the database.
         self.description = description
+        self.encryption_type = encryption_type
         # The ID of the OceanBase cluster.
         self.instance_id = instance_id
         # The role of the user account.   
         # 
         # - In Oracle mode, this parameter is left unspecified.    
         # - In MySQL mode, the super administrator account has ALL PRIVILEGES, and you can leave this parameter unspecified.   
         #  
@@ -2119,14 +2121,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.description is not None:
             result['Description'] = self.description
+        if self.encryption_type is not None:
+            result['EncryptionType'] = self.encryption_type
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.roles is not None:
             result['Roles'] = self.roles
         if self.tenant_id is not None:
             result['TenantId'] = self.tenant_id
         if self.user_name is not None:
@@ -2137,14 +2141,16 @@
             result['UserType'] = self.user_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Description') is not None:
             self.description = m.get('Description')
+        if m.get('EncryptionType') is not None:
+            self.encryption_type = m.get('EncryptionType')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('Roles') is not None:
             self.roles = m.get('Roles')
         if m.get('TenantId') is not None:
             self.tenant_id = m.get('TenantId')
         if m.get('UserName') is not None:
@@ -16137,14 +16143,298 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyInstanceNameResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ModifyInstanceNodeNumRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        node_num: str = None,
+    ):
+        self.instance_id = instance_id
+        self.node_num = node_num
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
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.node_num is not None:
+            result['NodeNum'] = self.node_num
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NodeNum') is not None:
+            self.node_num = m.get('NodeNum')
+        return self
+
+
+class ModifyInstanceNodeNumResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        order_id: str = None,
+    ):
+        self.order_id = order_id
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
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        return self
+
+
+class ModifyInstanceNodeNumResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: ModifyInstanceNodeNumResponseBodyData = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            temp_model = ModifyInstanceNodeNumResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ModifyInstanceNodeNumResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ModifyInstanceNodeNumResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ModifyInstanceNodeNumResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ModifyInstanceSpecRequest(TeaModel):
+    def __init__(
+        self,
+        disk_size: int = None,
+        instance_class: str = None,
+        instance_id: str = None,
+    ):
+        self.disk_size = disk_size
+        self.instance_class = instance_class
+        self.instance_id = instance_id
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
+        if self.disk_size is not None:
+            result['DiskSize'] = self.disk_size
+        if self.instance_class is not None:
+            result['InstanceClass'] = self.instance_class
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DiskSize') is not None:
+            self.disk_size = m.get('DiskSize')
+        if m.get('InstanceClass') is not None:
+            self.instance_class = m.get('InstanceClass')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        return self
+
+
+class ModifyInstanceSpecResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        order_id: str = None,
+    ):
+        self.order_id = order_id
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
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        return self
+
+
+class ModifyInstanceSpecResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: ModifyInstanceSpecResponseBodyData = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            temp_model = ModifyInstanceSpecResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ModifyInstanceSpecResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ModifyInstanceSpecResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ModifyInstanceSpecResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ModifyInstanceTagsRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         tags: str = None,
     ):
         # The ID of the OceanBase cluster.
```

### Comparing `alibabacloud_oceanbasepro20190901-1.0.6/alibabacloud_oceanbasepro20190901.egg-info/PKG-INFO` & `alibabacloud_oceanbasepro20190901-1.0.7/alibabacloud_oceanbasepro20190901.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-oceanbasepro20190901
-Version: 1.0.6
+Version: 1.0.7
 Summary: Alibaba Cloud OceanBasePro (20190901) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oceanbasepro20190901-1.0.6/setup.py` & `alibabacloud_oceanbasepro20190901-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_oceanbasepro20190901.
 
-Created on 03/03/2023
+Created on 10/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_oceanbasepro20190901"
 NAME = "alibabacloud_oceanbasepro20190901" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud OceanBasePro (20190901) SDK Library for Python"
```


# Comparing `tmp/alibabacloud_oceanbasepro20190901_py2-1.0.1.tar.gz` & `tmp/alibabacloud_oceanbasepro20190901_py2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_oceanbasepro20190901_py2-1.0.1.tar", last modified: Fri Mar  3 08:02:21 2023, max compression
+gzip compressed data, was "dist/alibabacloud_oceanbasepro20190901_py2-1.0.2.tar", last modified: Mon Apr 10 03:09:31 2023, max compression
```

## Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.1.tar` & `alibabacloud_oceanbasepro20190901_py2-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 08:02:21.000000 alibabacloud_oceanbasepro20190901_py2-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       42 2023-03-03 08:02:20.000000 alibabacloud_oceanbasepro20190901_py2-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-03-03 08:02:20.000000 alibabacloud_oceanbasepro20190901_py2-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-03 08:02:20.000000 alibabacloud_oceanbasepro20190901_py2-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2526 2023-03-03 08:02:21.000000 alibabacloud_oceanbasepro20190901_py2-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1060 2023-03-03 08:02:20.000000 alibabacloud_oceanbasepro20190901_py2-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1143 2023-03-03 08:02:20.000000 alibabacloud_oceanbasepro20190901_py2-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 08:02:21.000000 alibabacloud_oceanbasepro20190901_py2-1.0.1/alibabacloud_oceanbasepro20190901/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-03 08:02:20.000000 alibabacloud_oceanbasepro20190901_py2-1.0.1/alibabacloud_oceanbasepro20190901/__init__.py
--rw-r--r--   0 root         (0) root         (0)   105846 2023-03-03 08:02:20.000000 alibabacloud_oceanbasepro20190901_py2-1.0.1/alibabacloud_oceanbasepro20190901/client.py
--rw-r--r--   0 root         (0) root         (0)   789823 2023-03-03 08:02:20.000000 alibabacloud_oceanbasepro20190901_py2-1.0.1/alibabacloud_oceanbasepro20190901/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 08:02:21.000000 alibabacloud_oceanbasepro20190901_py2-1.0.1/alibabacloud_oceanbasepro20190901_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2526 2023-03-03 08:02:21.000000 alibabacloud_oceanbasepro20190901_py2-1.0.1/alibabacloud_oceanbasepro20190901_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      512 2023-03-03 08:02:21.000000 alibabacloud_oceanbasepro20190901_py2-1.0.1/alibabacloud_oceanbasepro20190901_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-03 08:02:21.000000 alibabacloud_oceanbasepro20190901_py2-1.0.1/alibabacloud_oceanbasepro20190901_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-03-03 08:02:21.000000 alibabacloud_oceanbasepro20190901_py2-1.0.1/alibabacloud_oceanbasepro20190901_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-03-03 08:02:21.000000 alibabacloud_oceanbasepro20190901_py2-1.0.1/alibabacloud_oceanbasepro20190901_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-03 08:02:21.000000 alibabacloud_oceanbasepro20190901_py2-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2948 2023-03-03 08:02:20.000000 alibabacloud_oceanbasepro20190901_py2-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   108324 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901/client.py
+-rw-r--r--   0 root         (0) root         (0)   798154 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      512 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2948 2023-04-10 03:09:31.000000 alibabacloud_oceanbasepro20190901_py2-1.0.2/setup.py
```

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.1/LICENSE` & `alibabacloud_oceanbasepro20190901_py2-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.1/PKG-INFO` & `alibabacloud_oceanbasepro20190901_py2-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_oceanbasepro20190901_py2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud OceanBasePro (20190901) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.1/README-CN.md` & `alibabacloud_oceanbasepro20190901_py2-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.1/README.md` & `alibabacloud_oceanbasepro20190901_py2-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.1/alibabacloud_oceanbasepro20190901/client.py` & `alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,14 +361,16 @@
         return self.create_tenant_read_only_connection_with_options(request, runtime)
 
     def create_tenant_user_with_options(self, request, runtime):
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
@@ -1962,14 +1964,76 @@
             self.call_api(params, req, runtime)
         )
 
     def modify_instance_name(self, request):
         runtime = util_models.RuntimeOptions()
         return self.modify_instance_name_with_options(request, runtime)
 
+    def modify_instance_node_num_with_options(self, request, runtime):
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
+    def modify_instance_node_num(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.modify_instance_node_num_with_options(request, runtime)
+
+    def modify_instance_spec_with_options(self, request, runtime):
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
+    def modify_instance_spec(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.modify_instance_spec_with_options(request, runtime)
+
     def modify_instance_tags_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.instance_id):
             body['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.tags):
             body['Tags'] = request.tags
```

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.1/alibabacloud_oceanbasepro20190901/models.py` & `alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1839,18 +1839,19 @@
         if m.get('body') is not None:
             temp_model = CreateTenantReadOnlyConnectionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateTenantUserRequest(TeaModel):
-    def __init__(self, description=None, instance_id=None, roles=None, tenant_id=None, user_name=None,
-                 user_password=None, user_type=None):
+    def __init__(self, description=None, encryption_type=None, instance_id=None, roles=None, tenant_id=None,
+                 user_name=None, user_password=None, user_type=None):
         # The description of the database.
         self.description = description  # type: str
+        self.encryption_type = encryption_type  # type: str
         # The ID of the OceanBase cluster.
         self.instance_id = instance_id  # type: str
         # The role of the user account.   
         # 
         # - In Oracle mode, this parameter is left unspecified.    
         # - In MySQL mode, the super administrator account has ALL PRIVILEGES, and you can leave this parameter unspecified.   
         #  
@@ -1884,14 +1885,16 @@
         _map = super(CreateTenantUserRequest, self).to_map()
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
@@ -1902,14 +1905,16 @@
             result['UserType'] = self.user_type
         return result
 
     def from_map(self, m=None):
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
@@ -14367,14 +14372,265 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyInstanceNameResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ModifyInstanceNodeNumRequest(TeaModel):
+    def __init__(self, instance_id=None, node_num=None):
+        self.instance_id = instance_id  # type: str
+        self.node_num = node_num  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyInstanceNodeNumRequest, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NodeNum') is not None:
+            self.node_num = m.get('NodeNum')
+        return self
+
+
+class ModifyInstanceNodeNumResponseBodyData(TeaModel):
+    def __init__(self, order_id=None):
+        self.order_id = order_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyInstanceNodeNumResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        return self
+
+
+class ModifyInstanceNodeNumResponseBody(TeaModel):
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: ModifyInstanceNodeNumResponseBodyData
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(ModifyInstanceNodeNumResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ModifyInstanceNodeNumResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ModifyInstanceNodeNumResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, disk_size=None, instance_class=None, instance_id=None):
+        self.disk_size = disk_size  # type: long
+        self.instance_class = instance_class  # type: str
+        self.instance_id = instance_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyInstanceSpecRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, order_id=None):
+        self.order_id = order_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyInstanceSpecResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        return self
+
+
+class ModifyInstanceSpecResponseBody(TeaModel):
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: ModifyInstanceSpecResponseBodyData
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(ModifyInstanceSpecResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ModifyInstanceSpecResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ModifyInstanceSpecResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, instance_id=None, tags=None):
         # The ID of the OceanBase cluster.
         self.instance_id = instance_id  # type: str
         # The tags.
         self.tags = tags  # type: str
```

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.1/alibabacloud_oceanbasepro20190901_py2.egg-info/PKG-INFO` & `alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-oceanbasepro20190901-py2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud OceanBasePro (20190901) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.1/alibabacloud_oceanbasepro20190901_py2.egg-info/SOURCES.txt` & `alibabacloud_oceanbasepro20190901_py2-1.0.2/alibabacloud_oceanbasepro20190901_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.1/setup.py` & `alibabacloud_oceanbasepro20190901_py2-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_oceanbasepro20190901_py2.
 
-Created on 03/03/2023
+Created on 10/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_oceanbasepro20190901"
 NAME = "alibabacloud_oceanbasepro20190901_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud OceanBasePro (20190901) SDK Library for Python2"
```


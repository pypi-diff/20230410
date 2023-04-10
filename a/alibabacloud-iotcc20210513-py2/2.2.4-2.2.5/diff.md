# Comparing `tmp/alibabacloud_iotcc20210513_py2-2.2.4.tar.gz` & `tmp/alibabacloud_iotcc20210513_py2-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_iotcc20210513_py2-2.2.4.tar", last modified: Wed Sep  7 12:38:34 2022, max compression
+gzip compressed data, was "dist/alibabacloud_iotcc20210513_py2-2.2.5.tar", last modified: Mon Apr 10 15:26:17 2023, max compression
```

## Comparing `alibabacloud_iotcc20210513_py2-2.2.4.tar` & `alibabacloud_iotcc20210513_py2-2.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-07 12:38:34.000000 alibabacloud_iotcc20210513_py2-2.2.4/
--rw-r--r--   0 root         (0) root         (0)      780 2022-09-07 12:38:34.000000 alibabacloud_iotcc20210513_py2-2.2.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-09-07 12:38:34.000000 alibabacloud_iotcc20210513_py2-2.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-09-07 12:38:34.000000 alibabacloud_iotcc20210513_py2-2.2.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2484 2022-09-07 12:38:34.000000 alibabacloud_iotcc20210513_py2-2.2.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2022-09-07 12:38:34.000000 alibabacloud_iotcc20210513_py2-2.2.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2022-09-07 12:38:34.000000 alibabacloud_iotcc20210513_py2-2.2.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-07 12:38:34.000000 alibabacloud_iotcc20210513_py2-2.2.4/alibabacloud_iotcc20210513/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-07 12:38:34.000000 alibabacloud_iotcc20210513_py2-2.2.4/alibabacloud_iotcc20210513/__init__.py
--rw-r--r--   0 root         (0) root         (0)   133231 2022-09-07 12:38:34.000000 alibabacloud_iotcc20210513_py2-2.2.4/alibabacloud_iotcc20210513/client.py
--rw-r--r--   0 root         (0) root         (0)   432916 2022-09-07 12:38:34.000000 alibabacloud_iotcc20210513_py2-2.2.4/alibabacloud_iotcc20210513/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-07 12:38:34.000000 alibabacloud_iotcc20210513_py2-2.2.4/alibabacloud_iotcc20210513_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2484 2022-09-07 12:38:34.000000 alibabacloud_iotcc20210513_py2-2.2.4/alibabacloud_iotcc20210513_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      456 2022-09-07 12:38:34.000000 alibabacloud_iotcc20210513_py2-2.2.4/alibabacloud_iotcc20210513_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-07 12:38:34.000000 alibabacloud_iotcc20210513_py2-2.2.4/alibabacloud_iotcc20210513_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-09-07 12:38:34.000000 alibabacloud_iotcc20210513_py2-2.2.4/alibabacloud_iotcc20210513_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2022-09-07 12:38:34.000000 alibabacloud_iotcc20210513_py2-2.2.4/alibabacloud_iotcc20210513_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-07 12:38:34.000000 alibabacloud_iotcc20210513_py2-2.2.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2913 2022-09-07 12:38:34.000000 alibabacloud_iotcc20210513_py2-2.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:26:17.000000 alibabacloud_iotcc20210513_py2-2.2.5/
+-rw-r--r--   0 root         (0) root         (0)      832 2023-04-10 15:26:17.000000 alibabacloud_iotcc20210513_py2-2.2.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-04-10 15:26:17.000000 alibabacloud_iotcc20210513_py2-2.2.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-10 15:26:17.000000 alibabacloud_iotcc20210513_py2-2.2.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-04-10 15:26:17.000000 alibabacloud_iotcc20210513_py2-2.2.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-04-10 15:26:17.000000 alibabacloud_iotcc20210513_py2-2.2.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-04-10 15:26:17.000000 alibabacloud_iotcc20210513_py2-2.2.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:26:17.000000 alibabacloud_iotcc20210513_py2-2.2.5/alibabacloud_iotcc20210513/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-10 15:26:17.000000 alibabacloud_iotcc20210513_py2-2.2.5/alibabacloud_iotcc20210513/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   133145 2023-04-10 15:26:17.000000 alibabacloud_iotcc20210513_py2-2.2.5/alibabacloud_iotcc20210513/client.py
+-rw-r--r--   0 root         (0) root         (0)   428608 2023-04-10 15:26:17.000000 alibabacloud_iotcc20210513_py2-2.2.5/alibabacloud_iotcc20210513/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:26:17.000000 alibabacloud_iotcc20210513_py2-2.2.5/alibabacloud_iotcc20210513_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-04-10 15:26:17.000000 alibabacloud_iotcc20210513_py2-2.2.5/alibabacloud_iotcc20210513_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      456 2023-04-10 15:26:17.000000 alibabacloud_iotcc20210513_py2-2.2.5/alibabacloud_iotcc20210513_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 15:26:17.000000 alibabacloud_iotcc20210513_py2-2.2.5/alibabacloud_iotcc20210513_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-10 15:26:17.000000 alibabacloud_iotcc20210513_py2-2.2.5/alibabacloud_iotcc20210513_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-04-10 15:26:17.000000 alibabacloud_iotcc20210513_py2-2.2.5/alibabacloud_iotcc20210513_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-10 15:26:17.000000 alibabacloud_iotcc20210513_py2-2.2.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2913 2023-04-10 15:26:17.000000 alibabacloud_iotcc20210513_py2-2.2.5/setup.py
```

### Comparing `alibabacloud_iotcc20210513_py2-2.2.4/ChangeLog.md` & `alibabacloud_iotcc20210513_py2-2.2.5/ChangeLog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2022-09-07 Version: 2.2.4
+- Support iotcc for iot.
+
 2022-06-14 Version: 2.1.8
 - Support iotcc for iot.
 
 2022-05-07 Version: 2.1.4
 - Support iotcc for iot.
 
 2022-04-21 Version: 2.1.3
```

### Comparing `alibabacloud_iotcc20210513_py2-2.2.4/LICENSE` & `alibabacloud_iotcc20210513_py2-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_iotcc20210513_py2-2.2.4/PKG-INFO` & `alibabacloud_iotcc20210513_py2-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_iotcc20210513_py2
-Version: 2.2.4
+Version: 2.2.5
 Summary: Alibaba Cloud IoTCC (20210513) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_iotcc20210513_py2-2.2.4/README-CN.md` & `alibabacloud_iotcc20210513_py2-2.2.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_iotcc20210513_py2-2.2.4/README.md` & `alibabacloud_iotcc20210513_py2-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_iotcc20210513_py2-2.2.4/alibabacloud_iotcc20210513/client.py` & `alibabacloud_iotcc20210513_py2-2.2.5/alibabacloud_iotcc20210513/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -802,14 +802,50 @@
             self.call_api(params, req, runtime)
         )
 
     def delete_authorization_rule(self, request):
         runtime = util_models.RuntimeOptions()
         return self.delete_authorization_rule_with_options(request, runtime)
 
+    def delete_authorization_rules_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.authorization_rule_ids):
+            query['AuthorizationRuleIds'] = request.authorization_rule_ids
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.dry_run):
+            query['DryRun'] = request.dry_run
+        if not UtilClient.is_unset(request.io_tcloud_connector_id):
+            query['IoTCloudConnectorId'] = request.io_tcloud_connector_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteAuthorizationRules',
+            version='2021-05-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            io_tcc20210513_models.DeleteAuthorizationRulesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def delete_authorization_rules(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.delete_authorization_rules_with_options(request, runtime)
+
     def delete_connection_pool_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.connection_pool_id):
             query['ConnectionPoolId'] = request.connection_pool_id
@@ -1561,14 +1597,18 @@
             query['AuthorizationRuleType'] = request.authorization_rule_type
         if not UtilClient.is_unset(request.destination):
             query['Destination'] = request.destination
         if not UtilClient.is_unset(request.destination_port):
             query['DestinationPort'] = request.destination_port
         if not UtilClient.is_unset(request.destination_type):
             query['DestinationType'] = request.destination_type
+        if not UtilClient.is_unset(request.fuzzy_authorization_rule_name):
+            query['FuzzyAuthorizationRuleName'] = request.fuzzy_authorization_rule_name
+        if not UtilClient.is_unset(request.fuzzy_destination):
+            query['FuzzyDestination'] = request.fuzzy_destination
         if not UtilClient.is_unset(request.io_tcloud_connector_id):
             query['IoTCloudConnectorId'] = request.io_tcloud_connector_id
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.policy):
@@ -1940,56 +1980,14 @@
             self.call_api(params, req, runtime)
         )
 
     def list_group_ip_mapping_rules(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_group_ip_mapping_rules_with_options(request, runtime)
 
-    def list_io_tcloud_connector_access_session_logs_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.destinations):
-            query['Destinations'] = request.destinations
-        if not UtilClient.is_unset(request.end_time):
-            query['EndTime'] = request.end_time
-        if not UtilClient.is_unset(request.io_tcloud_connector_id):
-            query['IoTCloudConnectorId'] = request.io_tcloud_connector_id
-        if not UtilClient.is_unset(request.max_results):
-            query['MaxResults'] = request.max_results
-        if not UtilClient.is_unset(request.next_token):
-            query['NextToken'] = request.next_token
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        if not UtilClient.is_unset(request.source_ips):
-            query['SourceIps'] = request.source_ips
-        if not UtilClient.is_unset(request.start_time):
-            query['StartTime'] = request.start_time
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ListIoTCloudConnectorAccessSessionLogs',
-            version='2021-05-13',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            io_tcc20210513_models.ListIoTCloudConnectorAccessSessionLogsResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def list_io_tcloud_connector_access_session_logs(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.list_io_tcloud_connector_access_session_logs_with_options(request, runtime)
-
     def list_io_tcloud_connector_available_zones_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.io_tcloud_connector_id):
             query['IoTCloudConnectorId'] = request.io_tcloud_connector_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
```

### Comparing `alibabacloud_iotcc20210513_py2-2.2.4/alibabacloud_iotcc20210513/models.py` & `alibabacloud_iotcc20210513_py2-2.2.5/alibabacloud_iotcc20210513/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2430,14 +2430,122 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteAuthorizationRuleResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteAuthorizationRulesRequest(TeaModel):
+    def __init__(self, authorization_rule_ids=None, client_token=None, dry_run=None, io_tcloud_connector_id=None,
+                 region_id=None):
+        self.authorization_rule_ids = authorization_rule_ids  # type: list[str]
+        self.client_token = client_token  # type: str
+        self.dry_run = dry_run  # type: bool
+        self.io_tcloud_connector_id = io_tcloud_connector_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteAuthorizationRulesRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.authorization_rule_ids is not None:
+            result['AuthorizationRuleIds'] = self.authorization_rule_ids
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.dry_run is not None:
+            result['DryRun'] = self.dry_run
+        if self.io_tcloud_connector_id is not None:
+            result['IoTCloudConnectorId'] = self.io_tcloud_connector_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AuthorizationRuleIds') is not None:
+            self.authorization_rule_ids = m.get('AuthorizationRuleIds')
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('DryRun') is not None:
+            self.dry_run = m.get('DryRun')
+        if m.get('IoTCloudConnectorId') is not None:
+            self.io_tcloud_connector_id = m.get('IoTCloudConnectorId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class DeleteAuthorizationRulesResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteAuthorizationRulesResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteAuthorizationRulesResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DeleteAuthorizationRulesResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DeleteAuthorizationRulesResponse, self).to_map()
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
+            temp_model = DeleteAuthorizationRulesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteConnectionPoolRequest(TeaModel):
     def __init__(self, client_token=None, connection_pool_id=None, dry_run=None, io_tcloud_connector_id=None,
                  region_id=None):
         self.client_token = client_token  # type: str
         self.connection_pool_id = connection_pool_id  # type: str
         self.dry_run = dry_run  # type: bool
         self.io_tcloud_connector_id = io_tcloud_connector_id  # type: str
@@ -4910,23 +5018,26 @@
             temp_model = ListAPNsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListAuthorizationRulesRequest(TeaModel):
     def __init__(self, authorization_rule_ids=None, authorization_rule_name=None, authorization_rule_status=None,
-                 authorization_rule_type=None, destination=None, destination_port=None, destination_type=None, io_tcloud_connector_id=None,
-                 max_results=None, next_token=None, policy=None, protocol=None, region_id=None):
+                 authorization_rule_type=None, destination=None, destination_port=None, destination_type=None,
+                 fuzzy_authorization_rule_name=None, fuzzy_destination=None, io_tcloud_connector_id=None, max_results=None, next_token=None,
+                 policy=None, protocol=None, region_id=None):
         self.authorization_rule_ids = authorization_rule_ids  # type: list[str]
         self.authorization_rule_name = authorization_rule_name  # type: list[str]
         self.authorization_rule_status = authorization_rule_status  # type: list[str]
         self.authorization_rule_type = authorization_rule_type  # type: str
         self.destination = destination  # type: list[str]
         self.destination_port = destination_port  # type: list[str]
         self.destination_type = destination_type  # type: list[str]
+        self.fuzzy_authorization_rule_name = fuzzy_authorization_rule_name  # type: str
+        self.fuzzy_destination = fuzzy_destination  # type: str
         self.io_tcloud_connector_id = io_tcloud_connector_id  # type: str
         self.max_results = max_results  # type: int
         self.next_token = next_token  # type: str
         self.policy = policy  # type: list[str]
         self.protocol = protocol  # type: list[str]
         self.region_id = region_id  # type: str
 
@@ -4949,14 +5060,18 @@
             result['AuthorizationRuleType'] = self.authorization_rule_type
         if self.destination is not None:
             result['Destination'] = self.destination
         if self.destination_port is not None:
             result['DestinationPort'] = self.destination_port
         if self.destination_type is not None:
             result['DestinationType'] = self.destination_type
+        if self.fuzzy_authorization_rule_name is not None:
+            result['FuzzyAuthorizationRuleName'] = self.fuzzy_authorization_rule_name
+        if self.fuzzy_destination is not None:
+            result['FuzzyDestination'] = self.fuzzy_destination
         if self.io_tcloud_connector_id is not None:
             result['IoTCloudConnectorId'] = self.io_tcloud_connector_id
         if self.max_results is not None:
             result['MaxResults'] = self.max_results
         if self.next_token is not None:
             result['NextToken'] = self.next_token
         if self.policy is not None:
@@ -4979,14 +5094,18 @@
             self.authorization_rule_type = m.get('AuthorizationRuleType')
         if m.get('Destination') is not None:
             self.destination = m.get('Destination')
         if m.get('DestinationPort') is not None:
             self.destination_port = m.get('DestinationPort')
         if m.get('DestinationType') is not None:
             self.destination_type = m.get('DestinationType')
+        if m.get('FuzzyAuthorizationRuleName') is not None:
+            self.fuzzy_authorization_rule_name = m.get('FuzzyAuthorizationRuleName')
+        if m.get('FuzzyDestination') is not None:
+            self.fuzzy_destination = m.get('FuzzyDestination')
         if m.get('IoTCloudConnectorId') is not None:
             self.io_tcloud_connector_id = m.get('IoTCloudConnectorId')
         if m.get('MaxResults') is not None:
             self.max_results = m.get('MaxResults')
         if m.get('NextToken') is not None:
             self.next_token = m.get('NextToken')
         if m.get('Policy') is not None:
@@ -6868,226 +6987,14 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListGroupIpMappingRulesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListIoTCloudConnectorAccessSessionLogsRequest(TeaModel):
-    def __init__(self, destinations=None, end_time=None, io_tcloud_connector_id=None, max_results=None,
-                 next_token=None, region_id=None, source_ips=None, start_time=None):
-        self.destinations = destinations  # type: list[str]
-        self.end_time = end_time  # type: long
-        self.io_tcloud_connector_id = io_tcloud_connector_id  # type: str
-        self.max_results = max_results  # type: int
-        self.next_token = next_token  # type: str
-        self.region_id = region_id  # type: str
-        self.source_ips = source_ips  # type: list[str]
-        self.start_time = start_time  # type: long
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ListIoTCloudConnectorAccessSessionLogsRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.destinations is not None:
-            result['Destinations'] = self.destinations
-        if self.end_time is not None:
-            result['EndTime'] = self.end_time
-        if self.io_tcloud_connector_id is not None:
-            result['IoTCloudConnectorId'] = self.io_tcloud_connector_id
-        if self.max_results is not None:
-            result['MaxResults'] = self.max_results
-        if self.next_token is not None:
-            result['NextToken'] = self.next_token
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
-        if self.source_ips is not None:
-            result['SourceIps'] = self.source_ips
-        if self.start_time is not None:
-            result['StartTime'] = self.start_time
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Destinations') is not None:
-            self.destinations = m.get('Destinations')
-        if m.get('EndTime') is not None:
-            self.end_time = m.get('EndTime')
-        if m.get('IoTCloudConnectorId') is not None:
-            self.io_tcloud_connector_id = m.get('IoTCloudConnectorId')
-        if m.get('MaxResults') is not None:
-            self.max_results = m.get('MaxResults')
-        if m.get('NextToken') is not None:
-            self.next_token = m.get('NextToken')
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
-        if m.get('SourceIps') is not None:
-            self.source_ips = m.get('SourceIps')
-        if m.get('StartTime') is not None:
-            self.start_time = m.get('StartTime')
-        return self
-
-
-class ListIoTCloudConnectorAccessSessionLogsResponseBodyAccessSessionLogs(TeaModel):
-    def __init__(self, client_to_service_flow=None, destination_ip=None, destination_port=None, destinations=None,
-                 service_to_client_flow=None, source_ip=None, time=None, type=None):
-        self.client_to_service_flow = client_to_service_flow  # type: str
-        self.destination_ip = destination_ip  # type: str
-        self.destination_port = destination_port  # type: str
-        self.destinations = destinations  # type: list[str]
-        self.service_to_client_flow = service_to_client_flow  # type: str
-        self.source_ip = source_ip  # type: str
-        self.time = time  # type: str
-        self.type = type  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ListIoTCloudConnectorAccessSessionLogsResponseBodyAccessSessionLogs, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.client_to_service_flow is not None:
-            result['ClientToServiceFlow'] = self.client_to_service_flow
-        if self.destination_ip is not None:
-            result['DestinationIp'] = self.destination_ip
-        if self.destination_port is not None:
-            result['DestinationPort'] = self.destination_port
-        if self.destinations is not None:
-            result['Destinations'] = self.destinations
-        if self.service_to_client_flow is not None:
-            result['ServiceToClientFlow'] = self.service_to_client_flow
-        if self.source_ip is not None:
-            result['SourceIp'] = self.source_ip
-        if self.time is not None:
-            result['Time'] = self.time
-        if self.type is not None:
-            result['Type'] = self.type
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('ClientToServiceFlow') is not None:
-            self.client_to_service_flow = m.get('ClientToServiceFlow')
-        if m.get('DestinationIp') is not None:
-            self.destination_ip = m.get('DestinationIp')
-        if m.get('DestinationPort') is not None:
-            self.destination_port = m.get('DestinationPort')
-        if m.get('Destinations') is not None:
-            self.destinations = m.get('Destinations')
-        if m.get('ServiceToClientFlow') is not None:
-            self.service_to_client_flow = m.get('ServiceToClientFlow')
-        if m.get('SourceIp') is not None:
-            self.source_ip = m.get('SourceIp')
-        if m.get('Time') is not None:
-            self.time = m.get('Time')
-        if m.get('Type') is not None:
-            self.type = m.get('Type')
-        return self
-
-
-class ListIoTCloudConnectorAccessSessionLogsResponseBody(TeaModel):
-    def __init__(self, access_session_logs=None, max_results=None, next_token=None, request_id=None,
-                 total_count=None):
-        self.access_session_logs = access_session_logs  # type: list[ListIoTCloudConnectorAccessSessionLogsResponseBodyAccessSessionLogs]
-        self.max_results = max_results  # type: int
-        self.next_token = next_token  # type: str
-        self.request_id = request_id  # type: str
-        self.total_count = total_count  # type: int
-
-    def validate(self):
-        if self.access_session_logs:
-            for k in self.access_session_logs:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(ListIoTCloudConnectorAccessSessionLogsResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['AccessSessionLogs'] = []
-        if self.access_session_logs is not None:
-            for k in self.access_session_logs:
-                result['AccessSessionLogs'].append(k.to_map() if k else None)
-        if self.max_results is not None:
-            result['MaxResults'] = self.max_results
-        if self.next_token is not None:
-            result['NextToken'] = self.next_token
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.total_count is not None:
-            result['TotalCount'] = self.total_count
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        self.access_session_logs = []
-        if m.get('AccessSessionLogs') is not None:
-            for k in m.get('AccessSessionLogs'):
-                temp_model = ListIoTCloudConnectorAccessSessionLogsResponseBodyAccessSessionLogs()
-                self.access_session_logs.append(temp_model.from_map(k))
-        if m.get('MaxResults') is not None:
-            self.max_results = m.get('MaxResults')
-        if m.get('NextToken') is not None:
-            self.next_token = m.get('NextToken')
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('TotalCount') is not None:
-            self.total_count = m.get('TotalCount')
-        return self
-
-
-class ListIoTCloudConnectorAccessSessionLogsResponse(TeaModel):
-    def __init__(self, headers=None, status_code=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.status_code = status_code  # type: int
-        self.body = body  # type: ListIoTCloudConnectorAccessSessionLogsResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(ListIoTCloudConnectorAccessSessionLogsResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = ListIoTCloudConnectorAccessSessionLogsResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class ListIoTCloudConnectorAvailableZonesRequest(TeaModel):
     def __init__(self, io_tcloud_connector_id=None, region_id=None):
         self.io_tcloud_connector_id = io_tcloud_connector_id  # type: str
         self.region_id = region_id  # type: str
 
     def validate(self):
         pass
```

### Comparing `alibabacloud_iotcc20210513_py2-2.2.4/alibabacloud_iotcc20210513_py2.egg-info/PKG-INFO` & `alibabacloud_iotcc20210513_py2-2.2.5/alibabacloud_iotcc20210513_py2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-iotcc20210513-py2
-Version: 2.2.4
+Version: 2.2.5
 Summary: Alibaba Cloud IoTCC (20210513) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_iotcc20210513_py2-2.2.4/setup.py` & `alibabacloud_iotcc20210513_py2-2.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_iotcc20210513_py2.
 
-Created on 07/09/2022
+Created on 10/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_iotcc20210513"
 NAME = "alibabacloud_iotcc20210513_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud IoTCC (20210513) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.6, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.3, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```


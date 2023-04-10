# Comparing `tmp/alibabacloud_iotcc20210513-2.2.4.tar.gz` & `tmp/alibabacloud_iotcc20210513-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_iotcc20210513-2.2.4.tar", last modified: Wed Sep  7 12:39:13 2022, max compression
+gzip compressed data, was "dist/alibabacloud_iotcc20210513-2.2.5.tar", last modified: Mon Apr 10 15:26:36 2023, max compression
```

## Comparing `alibabacloud_iotcc20210513-2.2.4.tar` & `alibabacloud_iotcc20210513-2.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-07 12:39:13.000000 alibabacloud_iotcc20210513-2.2.4/
--rw-r--r--   0 root         (0) root         (0)      832 2022-09-07 12:39:13.000000 alibabacloud_iotcc20210513-2.2.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-09-07 12:39:13.000000 alibabacloud_iotcc20210513-2.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-09-07 12:39:13.000000 alibabacloud_iotcc20210513-2.2.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2340 2022-09-07 12:39:13.000000 alibabacloud_iotcc20210513-2.2.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1028 2022-09-07 12:39:13.000000 alibabacloud_iotcc20210513-2.2.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1113 2022-09-07 12:39:13.000000 alibabacloud_iotcc20210513-2.2.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-07 12:39:13.000000 alibabacloud_iotcc20210513-2.2.4/alibabacloud_iotcc20210513/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-07 12:39:13.000000 alibabacloud_iotcc20210513-2.2.4/alibabacloud_iotcc20210513/__init__.py
--rw-r--r--   0 root         (0) root         (0)   316653 2022-09-07 12:39:13.000000 alibabacloud_iotcc20210513-2.2.4/alibabacloud_iotcc20210513/client.py
--rw-r--r--   0 root         (0) root         (0)   428536 2022-09-07 12:39:13.000000 alibabacloud_iotcc20210513-2.2.4/alibabacloud_iotcc20210513/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-07 12:39:13.000000 alibabacloud_iotcc20210513-2.2.4/alibabacloud_iotcc20210513.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2340 2022-09-07 12:39:13.000000 alibabacloud_iotcc20210513-2.2.4/alibabacloud_iotcc20210513.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2022-09-07 12:39:13.000000 alibabacloud_iotcc20210513-2.2.4/alibabacloud_iotcc20210513.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-07 12:39:13.000000 alibabacloud_iotcc20210513-2.2.4/alibabacloud_iotcc20210513.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-09-07 12:39:13.000000 alibabacloud_iotcc20210513-2.2.4/alibabacloud_iotcc20210513.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2022-09-07 12:39:13.000000 alibabacloud_iotcc20210513-2.2.4/alibabacloud_iotcc20210513.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-07 12:39:13.000000 alibabacloud_iotcc20210513-2.2.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2620 2022-09-07 12:39:13.000000 alibabacloud_iotcc20210513-2.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:26:36.000000 alibabacloud_iotcc20210513-2.2.5/
+-rw-r--r--   0 root         (0) root         (0)      884 2023-04-10 15:26:35.000000 alibabacloud_iotcc20210513-2.2.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-10 15:26:35.000000 alibabacloud_iotcc20210513-2.2.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-10 15:26:35.000000 alibabacloud_iotcc20210513-2.2.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-04-10 15:26:36.000000 alibabacloud_iotcc20210513-2.2.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-04-10 15:26:35.000000 alibabacloud_iotcc20210513-2.2.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-04-10 15:26:35.000000 alibabacloud_iotcc20210513-2.2.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:26:36.000000 alibabacloud_iotcc20210513-2.2.5/alibabacloud_iotcc20210513/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-10 15:26:35.000000 alibabacloud_iotcc20210513-2.2.5/alibabacloud_iotcc20210513/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   316369 2023-04-10 15:26:35.000000 alibabacloud_iotcc20210513-2.2.5/alibabacloud_iotcc20210513/client.py
+-rw-r--r--   0 root         (0) root         (0)   424313 2023-04-10 15:26:35.000000 alibabacloud_iotcc20210513-2.2.5/alibabacloud_iotcc20210513/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:26:36.000000 alibabacloud_iotcc20210513-2.2.5/alibabacloud_iotcc20210513.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-04-10 15:26:35.000000 alibabacloud_iotcc20210513-2.2.5/alibabacloud_iotcc20210513.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      436 2023-04-10 15:26:36.000000 alibabacloud_iotcc20210513-2.2.5/alibabacloud_iotcc20210513.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 15:26:35.000000 alibabacloud_iotcc20210513-2.2.5/alibabacloud_iotcc20210513.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-10 15:26:35.000000 alibabacloud_iotcc20210513-2.2.5/alibabacloud_iotcc20210513.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-04-10 15:26:35.000000 alibabacloud_iotcc20210513-2.2.5/alibabacloud_iotcc20210513.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-10 15:26:36.000000 alibabacloud_iotcc20210513-2.2.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2620 2023-04-10 15:26:35.000000 alibabacloud_iotcc20210513-2.2.5/setup.py
```

### Comparing `alibabacloud_iotcc20210513-2.2.4/ChangeLog.md` & `alibabacloud_iotcc20210513-2.2.5/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2022-09-07 Version: 2.2.4
+- Support iotcc for iot.
+
 2022-07-25 Version: 2.1.9
 - Support iotcc for iot.
 
 2022-06-14 Version: 2.1.8
 - Support iotcc for iot.
 
 2022-05-07 Version: 2.1.4
```

### Comparing `alibabacloud_iotcc20210513-2.2.4/LICENSE` & `alibabacloud_iotcc20210513-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_iotcc20210513-2.2.4/PKG-INFO` & `alibabacloud_iotcc20210513-2.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_iotcc20210513
-Version: 2.2.4
+Version: 2.2.5
 Summary: Alibaba Cloud IoTCC (20210513) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_iotcc20210513-2.2.4/README-CN.md` & `alibabacloud_iotcc20210513-2.2.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_iotcc20210513-2.2.4/README.md` & `alibabacloud_iotcc20210513-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_iotcc20210513-2.2.4/alibabacloud_iotcc20210513/client.py` & `alibabacloud_iotcc20210513-2.2.5/alibabacloud_iotcc20210513/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1855,14 +1855,100 @@
     async def delete_authorization_rule_async(
         self,
         request: io_tcc20210513_models.DeleteAuthorizationRuleRequest,
     ) -> io_tcc20210513_models.DeleteAuthorizationRuleResponse:
         runtime = util_models.RuntimeOptions()
         return await self.delete_authorization_rule_with_options_async(request, runtime)
 
+    def delete_authorization_rules_with_options(
+        self,
+        request: io_tcc20210513_models.DeleteAuthorizationRulesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> io_tcc20210513_models.DeleteAuthorizationRulesResponse:
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
+    async def delete_authorization_rules_with_options_async(
+        self,
+        request: io_tcc20210513_models.DeleteAuthorizationRulesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> io_tcc20210513_models.DeleteAuthorizationRulesResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_authorization_rules(
+        self,
+        request: io_tcc20210513_models.DeleteAuthorizationRulesRequest,
+    ) -> io_tcc20210513_models.DeleteAuthorizationRulesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.delete_authorization_rules_with_options(request, runtime)
+
+    async def delete_authorization_rules_async(
+        self,
+        request: io_tcc20210513_models.DeleteAuthorizationRulesRequest,
+    ) -> io_tcc20210513_models.DeleteAuthorizationRulesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_authorization_rules_with_options_async(request, runtime)
+
     def delete_connection_pool_with_options(
         self,
         request: io_tcc20210513_models.DeleteConnectionPoolRequest,
         runtime: util_models.RuntimeOptions,
     ) -> io_tcc20210513_models.DeleteConnectionPoolResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -3654,14 +3740,18 @@
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
@@ -3706,14 +3796,18 @@
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
@@ -4551,112 +4645,14 @@
     async def list_group_ip_mapping_rules_async(
         self,
         request: io_tcc20210513_models.ListGroupIpMappingRulesRequest,
     ) -> io_tcc20210513_models.ListGroupIpMappingRulesResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_group_ip_mapping_rules_with_options_async(request, runtime)
 
-    def list_io_tcloud_connector_access_session_logs_with_options(
-        self,
-        request: io_tcc20210513_models.ListIoTCloudConnectorAccessSessionLogsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> io_tcc20210513_models.ListIoTCloudConnectorAccessSessionLogsResponse:
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
-    async def list_io_tcloud_connector_access_session_logs_with_options_async(
-        self,
-        request: io_tcc20210513_models.ListIoTCloudConnectorAccessSessionLogsRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> io_tcc20210513_models.ListIoTCloudConnectorAccessSessionLogsResponse:
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
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def list_io_tcloud_connector_access_session_logs(
-        self,
-        request: io_tcc20210513_models.ListIoTCloudConnectorAccessSessionLogsRequest,
-    ) -> io_tcc20210513_models.ListIoTCloudConnectorAccessSessionLogsResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.list_io_tcloud_connector_access_session_logs_with_options(request, runtime)
-
-    async def list_io_tcloud_connector_access_session_logs_async(
-        self,
-        request: io_tcc20210513_models.ListIoTCloudConnectorAccessSessionLogsRequest,
-    ) -> io_tcc20210513_models.ListIoTCloudConnectorAccessSessionLogsResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.list_io_tcloud_connector_access_session_logs_with_options_async(request, runtime)
-
     def list_io_tcloud_connector_available_zones_with_options(
         self,
         request: io_tcc20210513_models.ListIoTCloudConnectorAvailableZonesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> io_tcc20210513_models.ListIoTCloudConnectorAvailableZonesResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_iotcc20210513-2.2.4/alibabacloud_iotcc20210513/models.py` & `alibabacloud_iotcc20210513-2.2.5/alibabacloud_iotcc20210513/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2767,14 +2767,136 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteAuthorizationRuleResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteAuthorizationRulesRequest(TeaModel):
+    def __init__(
+        self,
+        authorization_rule_ids: List[str] = None,
+        client_token: str = None,
+        dry_run: bool = None,
+        io_tcloud_connector_id: str = None,
+        region_id: str = None,
+    ):
+        self.authorization_rule_ids = authorization_rule_ids
+        self.client_token = client_token
+        self.dry_run = dry_run
+        self.io_tcloud_connector_id = io_tcloud_connector_id
+        self.region_id = region_id
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
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
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteAuthorizationRulesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteAuthorizationRulesResponseBody = None,
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
+            temp_model = DeleteAuthorizationRulesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteConnectionPoolRequest(TeaModel):
     def __init__(
         self,
         client_token: str = None,
         connection_pool_id: str = None,
         dry_run: bool = None,
         io_tcloud_connector_id: str = None,
@@ -5589,28 +5711,32 @@
         authorization_rule_ids: List[str] = None,
         authorization_rule_name: List[str] = None,
         authorization_rule_status: List[str] = None,
         authorization_rule_type: str = None,
         destination: List[str] = None,
         destination_port: List[str] = None,
         destination_type: List[str] = None,
+        fuzzy_authorization_rule_name: str = None,
+        fuzzy_destination: str = None,
         io_tcloud_connector_id: str = None,
         max_results: int = None,
         next_token: str = None,
         policy: List[str] = None,
         protocol: List[str] = None,
         region_id: str = None,
     ):
         self.authorization_rule_ids = authorization_rule_ids
         self.authorization_rule_name = authorization_rule_name
         self.authorization_rule_status = authorization_rule_status
         self.authorization_rule_type = authorization_rule_type
         self.destination = destination
         self.destination_port = destination_port
         self.destination_type = destination_type
+        self.fuzzy_authorization_rule_name = fuzzy_authorization_rule_name
+        self.fuzzy_destination = fuzzy_destination
         self.io_tcloud_connector_id = io_tcloud_connector_id
         self.max_results = max_results
         self.next_token = next_token
         self.policy = policy
         self.protocol = protocol
         self.region_id = region_id
 
@@ -5633,14 +5759,18 @@
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
@@ -5663,14 +5793,18 @@
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
@@ -7808,255 +7942,14 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListGroupIpMappingRulesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListIoTCloudConnectorAccessSessionLogsRequest(TeaModel):
-    def __init__(
-        self,
-        destinations: List[str] = None,
-        end_time: int = None,
-        io_tcloud_connector_id: str = None,
-        max_results: int = None,
-        next_token: str = None,
-        region_id: str = None,
-        source_ips: List[str] = None,
-        start_time: int = None,
-    ):
-        self.destinations = destinations
-        self.end_time = end_time
-        self.io_tcloud_connector_id = io_tcloud_connector_id
-        self.max_results = max_results
-        self.next_token = next_token
-        self.region_id = region_id
-        self.source_ips = source_ips
-        self.start_time = start_time
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
-    def __init__(
-        self,
-        client_to_service_flow: str = None,
-        destination_ip: str = None,
-        destination_port: str = None,
-        destinations: List[str] = None,
-        service_to_client_flow: str = None,
-        source_ip: str = None,
-        time: str = None,
-        type: str = None,
-    ):
-        self.client_to_service_flow = client_to_service_flow
-        self.destination_ip = destination_ip
-        self.destination_port = destination_port
-        self.destinations = destinations
-        self.service_to_client_flow = service_to_client_flow
-        self.source_ip = source_ip
-        self.time = time
-        self.type = type
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
-    def __init__(
-        self,
-        access_session_logs: List[ListIoTCloudConnectorAccessSessionLogsResponseBodyAccessSessionLogs] = None,
-        max_results: int = None,
-        next_token: str = None,
-        request_id: str = None,
-        total_count: int = None,
-    ):
-        self.access_session_logs = access_session_logs
-        self.max_results = max_results
-        self.next_token = next_token
-        self.request_id = request_id
-        self.total_count = total_count
-
-    def validate(self):
-        if self.access_session_logs:
-            for k in self.access_session_logs:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: ListIoTCloudConnectorAccessSessionLogsResponseBody = None,
-    ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         io_tcloud_connector_id: str = None,
         region_id: str = None,
     ):
         self.io_tcloud_connector_id = io_tcloud_connector_id
```

### Comparing `alibabacloud_iotcc20210513-2.2.4/alibabacloud_iotcc20210513.egg-info/PKG-INFO` & `alibabacloud_iotcc20210513-2.2.5/alibabacloud_iotcc20210513.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-iotcc20210513
-Version: 2.2.4
+Version: 2.2.5
 Summary: Alibaba Cloud IoTCC (20210513) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_iotcc20210513-2.2.4/setup.py` & `alibabacloud_iotcc20210513-2.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_iotcc20210513.
 
-Created on 07/09/2022
+Created on 10/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_iotcc20210513"
 NAME = "alibabacloud_iotcc20210513" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud IoTCC (20210513) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```


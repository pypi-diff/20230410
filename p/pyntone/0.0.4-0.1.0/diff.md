# Comparing `tmp/pyntone-0.0.4.tar.gz` & `tmp/pyntone-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyntone-0.0.4.tar", last modified: Fri May 20 07:20:37 2022, max compression
+gzip compressed data, was "pyntone-0.1.0.tar", last modified: Mon Apr 10 04:12:34 2023, max compression
```

## Comparing `pyntone-0.0.4.tar` & `pyntone-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,30 @@
-drwxrwxrwx   0        0        0        0 2022-05-20 07:20:37.896046 pyntone-0.0.4/
--rw-rw-rw-   0        0        0     1083 2022-04-06 02:24:55.000000 pyntone-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2483 2022-05-20 07:20:37.897044 pyntone-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2044 2022-04-06 04:42:34.000000 pyntone-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2022-05-20 07:20:37.847048 pyntone-0.0.4/pyntone/
--rw-rw-rw-   0        0        0      114 2022-05-07 14:59:08.000000 pyntone-0.0.4/pyntone/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-20 07:20:37.884047 pyntone-0.0.4/pyntone/client/
--rw-rw-rw-   0        0        0        0 2022-04-05 04:51:03.000000 pyntone-0.0.4/pyntone/client/__init__.py
--rw-rw-rw-   0        0        0     2086 2022-05-07 14:59:08.000000 pyntone-0.0.4/pyntone/client/app_client.py
--rw-rw-rw-   0        0        0     1125 2022-05-07 14:59:08.000000 pyntone-0.0.4/pyntone/client/bulk_request_client.py
--rw-rw-rw-   0        0        0     7001 2022-05-08 05:25:19.000000 pyntone-0.0.4/pyntone/client/record_client.py
-drwxrwxrwx   0        0        0        0 2022-05-20 07:20:37.886047 pyntone-0.0.4/pyntone/http/
--rw-rw-rw-   0        0        0        0 2022-02-26 06:27:39.000000 pyntone-0.0.4/pyntone/http/__init__.py
--rw-rw-rw-   0        0        0     1549 2022-05-07 14:59:08.000000 pyntone-0.0.4/pyntone/http/http_client.py
--rw-rw-rw-   0        0        0     2741 2022-05-07 14:59:08.000000 pyntone-0.0.4/pyntone/kintone_request_config_builder.py
--rw-rw-rw-   0        0        0      239 2022-03-28 02:09:22.000000 pyntone-0.0.4/pyntone/kintone_response_handler.py
--rw-rw-rw-   0        0        0     1402 2022-05-07 14:59:08.000000 pyntone-0.0.4/pyntone/kintone_rest_api_client.py
-drwxrwxrwx   0        0        0        0 2022-05-20 07:20:37.895046 pyntone-0.0.4/pyntone/models/
--rw-rw-rw-   0        0        0      824 2022-05-08 04:33:44.000000 pyntone-0.0.4/pyntone/models/__init__.py
--rw-rw-rw-   0        0        0      547 2022-03-28 02:09:12.000000 pyntone-0.0.4/pyntone/models/auth.py
--rw-rw-rw-   0        0        0     2335 2022-04-06 02:13:08.000000 pyntone-0.0.4/pyntone/models/base.py
--rw-rw-rw-   0        0        0      111 2022-05-07 14:59:08.000000 pyntone-0.0.4/pyntone/models/exception.py
--rw-rw-rw-   0        0        0    14290 2022-05-20 07:17:46.000000 pyntone-0.0.4/pyntone/models/field.py
--rw-rw-rw-   0        0        0      889 2022-05-07 14:59:08.000000 pyntone-0.0.4/pyntone/models/record.py
--rw-rw-rw-   0        0        0     1522 2022-05-08 05:24:59.000000 pyntone-0.0.4/pyntone/models/response.py
--rw-rw-rw-   0        0        0      330 2022-02-26 07:09:33.000000 pyntone-0.0.4/pyntone/url.py
-drwxrwxrwx   0        0        0        0 2022-05-20 07:20:37.879044 pyntone-0.0.4/pyntone.egg-info/
--rw-rw-rw-   0        0        0     2483 2022-05-20 07:20:37.000000 pyntone-0.0.4/pyntone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      700 2022-05-20 07:20:37.000000 pyntone-0.0.4/pyntone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-20 07:20:37.000000 pyntone-0.0.4/pyntone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2022-05-20 07:20:37.000000 pyntone-0.0.4/pyntone.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-05-20 07:20:37.000000 pyntone-0.0.4/pyntone.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2022-03-28 03:37:43.000000 pyntone-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      556 2022-05-20 07:20:37.898044 pyntone-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 04:12:34.182644 pyntone-0.1.0/
+-rw-rw-rw-   0        0        0     1083 2022-10-20 13:41:34.000000 pyntone-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      435 2023-04-10 04:12:34.183066 pyntone-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-10 04:12:34.135632 pyntone-0.1.0/pyntone/
+-rw-rw-rw-   0        0        0       91 2023-04-10 02:19:52.000000 pyntone-0.1.0/pyntone/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 04:12:34.166633 pyntone-0.1.0/pyntone/client/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:31:49.000000 pyntone-0.1.0/pyntone/client/__init__.py
+-rw-rw-rw-   0        0        0     1924 2023-04-06 13:14:42.000000 pyntone-0.1.0/pyntone/client/bulk_request_client.py
+-rw-rw-rw-   0        0        0    17136 2023-04-10 02:14:45.000000 pyntone-0.1.0/pyntone/client/record_client.py
+drwxrwxrwx   0        0        0        0 2023-04-10 04:12:34.170674 pyntone-0.1.0/pyntone/http/
+-rw-rw-rw-   0        0        0        0 2022-02-26 06:27:39.000000 pyntone-0.1.0/pyntone/http/__init__.py
+-rw-rw-rw-   0        0        0     1767 2023-04-05 14:54:36.000000 pyntone-0.1.0/pyntone/http/http_client.py
+-rw-rw-rw-   0        0        0     6265 2023-04-09 12:25:24.000000 pyntone-0.1.0/pyntone/kintone_request_config_builder.py
+-rw-rw-rw-   0        0        0     1262 2023-04-06 08:39:46.000000 pyntone-0.1.0/pyntone/kintone_rest_api_client.py
+drwxrwxrwx   0        0        0        0 2023-04-10 04:12:34.176636 pyntone-0.1.0/pyntone/types/
+-rw-rw-rw-   0        0        0      136 2023-04-07 07:20:19.000000 pyntone-0.1.0/pyntone/types/__init__.py
+-rw-rw-rw-   0        0        0      522 2023-04-09 12:10:39.000000 pyntone-0.1.0/pyntone/types/auth.py
+-rw-rw-rw-   0        0        0      966 2023-04-07 12:27:01.000000 pyntone-0.1.0/pyntone/types/record.py
+-rw-rw-rw-   0        0        0      340 2023-03-12 12:27:40.000000 pyntone-0.1.0/pyntone/url.py
+drwxrwxrwx   0        0        0        0 2023-04-10 04:12:34.160633 pyntone-0.1.0/pyntone.egg-info/
+-rw-rw-rw-   0        0        0      435 2023-04-10 04:12:34.000000 pyntone-0.1.0/pyntone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-04-10 04:12:34.000000 pyntone-0.1.0/pyntone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 04:12:34.000000 pyntone-0.1.0/pyntone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-10 04:12:34.000000 pyntone-0.1.0/pyntone.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-10 04:12:34.000000 pyntone-0.1.0/pyntone.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-04-09 12:28:30.000000 pyntone-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      556 2023-04-10 04:12:34.184634 pyntone-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 04:12:34.179633 pyntone-0.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:21:21.000000 pyntone-0.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     5872 2023-04-09 12:12:22.000000 pyntone-0.1.0/tests/record.py
```

### Comparing `pyntone-0.0.4/LICENSE` & `pyntone-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyntone-0.0.4/pyntone/client/bulk_request_client.py` & `pyntone-0.1.0/pyntone/kintone_rest_api_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,36 @@
-from typing import Union
+import re
+from typing import Optional, TypedDict, Union
 
+from pyntone.client.record_client import RecordClient
+from pyntone.client.bulk_request_client import BulkRequestClient
 from pyntone.http.http_client import HttpClent
-from pyntone.models import KintoneRequest, KintoneRequestParams
-from pyntone.url import build_path
+from pyntone.kintone_request_config_builder import KintoneRequestConfigBuilder
+from pyntone.types.auth import DiscriminatedAuth
 
 
-class BulkRequestClient:
-    def __init__(self, http_client: HttpClent, guest_space_id: Union[int, str, None] = None) -> None:
-        self.http_client = http_client
-        self.guest_space_id = guest_space_id
-        self.REQUESTS_LENGTH_LIMIT = 20
-    
-    def send(self, requests: list[KintoneRequest]):
-        reqs = [
-            {
-                'method': req.method.value,
-                'api': self._build_path_with_guest_space_id(req.endpoint_name.value),
-                'payload': req.payload
-            } for req in requests
-        ]
-        params = KintoneRequestParams(
-            data={ 'requests': reqs }
-        )
-        path = self._build_path_with_guest_space_id('bulkRequest')
-        return self.http_client.post(path, params)
-    
-    def _build_path_with_guest_space_id(self, endpoint_name: str) -> str:
-        return build_path(endpoint=endpoint_name, guest_space_id=self.guest_space_id)
+class FeatureFlags(TypedDict):
+    enableAbortSearchError: bool
+
+
+class KintoneRestAPIClient:
+    def __init__(
+        self,
+        base_url: str,
+        auth: DiscriminatedAuth,
+        guest_space_id: Union[int, str, None] = None,
+        basic_auth = None,
+        client_cert_auth = None,
+        proxy = None,
+        feature_flags = None,
+        user_agent: Optional[str] = None
+    ) -> None:
+        self.__base_url = re.sub('/+$', '', base_url)
+        
+        
+        request_config_builder = KintoneRequestConfigBuilder(auth=auth, base_url=self.__base_url)
+        httpClient = HttpClent(config_builder=request_config_builder)
+        
+        self.bulkRequest = BulkRequestClient(httpClient, guest_space_id)
+        self.record = RecordClient(httpClient, self.bulkRequest, guest_space_id)
+        # self.app = AppClient()
+        # self.file = FileClient()
```

### Comparing `pyntone-0.0.4/pyntone/http/http_client.py` & `pyntone-0.1.0/pyntone/http/http_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-import json
 from typing import Any
 
 import requests
 from pyntone.kintone_request_config_builder import (
-    HttpMethod, KintoneRequestConfigBuilder)
-from pyntone.models import KintoneRequestParams
-from pyntone.models.exception import KintoneError
+    HttpMethod, KintoneRequestConfigBuilder, KintoneRequestParams)
 
 
-class HttpClent():
+class KintoneError(Exception):
+    def __init__(self, message, text, json, status_code) -> None:
+        self.text = text
+        self.json = json
+        self.status_code = status_code
+        super().__init__(message)
+
+class HttpClent:
     def __init__(self, config_builder: KintoneRequestConfigBuilder) -> None:
         self.config_builder = config_builder
     
     def get(self, path: str, params: KintoneRequestParams) -> dict[str, Any]:
         config = self.config_builder.build(HttpMethod.GET, path, params)
         return self._send_request(config)
 
@@ -27,12 +31,13 @@
     def delete(self, path: str, params: KintoneRequestParams) -> dict[str, Any]:
         config = self.config_builder.build(HttpMethod.DELETE, path, params)
         return self._send_request(config)
     
     def _send_request(self, config: dict[str, Any]) -> dict[str, Any]:
         r = requests.request(**config)
         self._is_success(r)
-        return json.loads(r.text)
+        return r.json()
 
     def _is_success(self, response: requests.Response) -> None:
-        if response.status_code != 200:
-            raise KintoneError(response.text)
+        if not (200 <= response.status_code < 300):
+            json = response.json()
+            raise KintoneError(json['message'], response.text, json, response.status_code)
```

### Comparing `pyntone-0.0.4/pyntone.egg-info/SOURCES.txt` & `pyntone-0.1.0/pyntone.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 LICENSE
-README.md
 pyproject.toml
 setup.cfg
 pyntone/__init__.py
 pyntone/kintone_request_config_builder.py
-pyntone/kintone_response_handler.py
 pyntone/kintone_rest_api_client.py
 pyntone/url.py
 pyntone.egg-info/PKG-INFO
 pyntone.egg-info/SOURCES.txt
 pyntone.egg-info/dependency_links.txt
 pyntone.egg-info/requires.txt
 pyntone.egg-info/top_level.txt
 pyntone/client/__init__.py
-pyntone/client/app_client.py
 pyntone/client/bulk_request_client.py
 pyntone/client/record_client.py
 pyntone/http/__init__.py
 pyntone/http/http_client.py
-pyntone/models/__init__.py
-pyntone/models/auth.py
-pyntone/models/base.py
-pyntone/models/exception.py
-pyntone/models/field.py
-pyntone/models/record.py
-pyntone/models/response.py
+pyntone/types/__init__.py
+pyntone/types/auth.py
+pyntone/types/record.py
+tests/__init__.py
+tests/record.py
```

### Comparing `pyntone-0.0.4/setup.cfg` & `pyntone-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796e 746f 6e65 0d0a 7665 7273   = pyntone..vers
-00000020: 696f 6e20 3d20 302e 302e 340d 0a64 6573  ion = 0.0.4..des
+00000020: 696f 6e20 3d20 302e 312e 300d 0a64 6573  ion = 0.1.0..des
 00000030: 6372 6970 7469 6f6e 203d 204b 696e 746f  cription = Kinto
 00000040: 6e65 2052 6573 7420 4150 4920 5772 6170  ne Rest API Wrap
 00000050: 7065 720d 0a75 726c 203d 2068 7474 7073  per..url = https
 00000060: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b61  ://github.com/ka
 00000070: 7368 6930 332f 7079 6e74 6f6e 650d 0a6c  shi03/pyntone..l
 00000080: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 00000090: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
```


# Comparing `tmp/pangea_sdk-1.6.0.tar.gz` & `tmp/pangea_sdk-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangea_sdk-1.6.0.tar", max compression
+gzip compressed data, was "pangea_sdk-1.7.0.tar", max compression
```

## Comparing `pangea_sdk-1.6.0.tar` & `pangea_sdk-1.7.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     7767 2023-03-20 14:38:05.057755 pangea_sdk-1.6.0/README.md
--rw-r--r--   0        0        0      146 2023-03-27 21:51:26.263503 pangea_sdk-1.6.0/pangea/__init__.py
--rw-r--r--   0        0        0     3778 2023-03-14 20:28:21.418701 pangea_sdk-1.6.0/pangea/audit_logger.py
--rw-r--r--   0        0        0      906 2023-03-14 20:28:21.418701 pangea_sdk-1.6.0/pangea/config.py
--rw-r--r--   0        0        0     8741 2023-03-27 23:30:24.510654 pangea_sdk-1.6.0/pangea/deep_verify.py
--rw-r--r--   0        0        0      604 2023-03-27 23:30:24.514654 pangea_sdk-1.6.0/pangea/deprecated.py
--rw-r--r--   0        0        0     6511 2023-03-27 23:30:24.514654 pangea_sdk-1.6.0/pangea/dump_audit.py
--rw-r--r--   0        0        0     4251 2023-03-20 14:38:05.057755 pangea_sdk-1.6.0/pangea/exceptions.py
--rw-r--r--   0        0        0     9799 2023-03-27 23:30:24.514654 pangea_sdk-1.6.0/pangea/request.py
--rw-r--r--   0        0        0     3625 2023-03-27 23:30:24.514654 pangea_sdk-1.6.0/pangea/response.py
--rw-r--r--   0        0        0      179 2023-03-27 12:18:00.996556 pangea_sdk-1.6.0/pangea/services/__init__.py
--rw-r--r--   0        0        0    24064 2023-03-27 23:30:24.514654 pangea_sdk-1.6.0/pangea/services/audit/audit.py
--rw-r--r--   0        0        0      451 2023-03-14 20:28:21.418701 pangea_sdk-1.6.0/pangea/services/audit/exceptions.py
--rw-r--r--   0        0        0    12093 2023-03-27 23:30:24.514654 pangea_sdk-1.6.0/pangea/services/audit/models.py
--rw-r--r--   0        0        0     4938 2023-03-27 23:30:24.514654 pangea_sdk-1.6.0/pangea/services/audit/signing.py
--rw-r--r--   0        0        0     8055 2023-03-27 23:30:24.514654 pangea_sdk-1.6.0/pangea/services/audit/util.py
--rw-r--r--   0        0        0     1010 2023-03-27 23:30:24.514654 pangea_sdk-1.6.0/pangea/services/base.py
--rw-r--r--   0        0        0     5565 2023-03-27 23:30:24.514654 pangea_sdk-1.6.0/pangea/services/embargo.py
--rw-r--r--   0        0        0    27450 2023-03-27 23:30:24.514654 pangea_sdk-1.6.0/pangea/services/intel.py
--rw-r--r--   0        0        0     6696 2023-03-27 23:30:24.518654 pangea_sdk-1.6.0/pangea/services/redact.py
--rw-r--r--   0        0        0     1450 2023-03-14 20:28:21.418701 pangea_sdk-1.6.0/pangea/services/vault/models/asymmetric.py
--rw-r--r--   0        0        0     7847 2023-03-27 12:18:00.996556 pangea_sdk-1.6.0/pangea/services/vault/models/common.py
--rw-r--r--   0        0        0      481 2023-03-14 20:28:21.422701 pangea_sdk-1.6.0/pangea/services/vault/models/secret.py
--rw-r--r--   0        0        0     1260 2023-03-14 20:28:21.422701 pangea_sdk-1.6.0/pangea/services/vault/models/symmetric.py
--rw-r--r--   0        0        0    16743 2023-03-27 23:30:24.518654 pangea_sdk-1.6.0/pangea/services/vault/vault.py
--rw-r--r--   0        0        0     5193 2023-03-27 23:30:24.518654 pangea_sdk-1.6.0/pangea/tools.py
--rw-r--r--   0        0        0      554 2023-03-27 12:18:00.996556 pangea_sdk-1.6.0/pangea/utils.py
--rw-r--r--   0        0        0    10610 2023-03-27 23:30:24.518654 pangea_sdk-1.6.0/pangea/verify_audit.py
--rw-r--r--   0        0        0      840 2023-03-27 21:51:26.267503 pangea_sdk-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     8760 1970-01-01 00:00:00.000000 pangea_sdk-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     7767 2023-03-20 14:38:05.057755 pangea_sdk-1.7.0/README.md
+-rw-r--r--   0        0        0      146 2023-04-10 17:17:45.138097 pangea_sdk-1.7.0/pangea/__init__.py
+-rw-r--r--   0        0        0     3778 2023-03-14 20:28:21.418701 pangea_sdk-1.7.0/pangea/audit_logger.py
+-rw-r--r--   0        0        0     1055 2023-03-30 18:27:54.782177 pangea_sdk-1.7.0/pangea/config.py
+-rw-r--r--   0        0        0     8741 2023-04-10 17:24:06.407418 pangea_sdk-1.7.0/pangea/deep_verify.py
+-rw-r--r--   0        0        0      604 2023-04-10 17:24:06.407418 pangea_sdk-1.7.0/pangea/deprecated.py
+-rw-r--r--   0        0        0     6511 2023-04-10 17:24:06.407418 pangea_sdk-1.7.0/pangea/dump_audit.py
+-rw-r--r--   0        0        0     4458 2023-04-10 12:18:10.328825 pangea_sdk-1.7.0/pangea/exceptions.py
+-rw-r--r--   0        0        0     9874 2023-04-10 17:24:06.407418 pangea_sdk-1.7.0/pangea/request.py
+-rw-r--r--   0        0        0     3895 2023-04-10 17:24:06.407418 pangea_sdk-1.7.0/pangea/response.py
+-rw-r--r--   0        0        0      190 2023-04-10 17:23:24.030383 pangea_sdk-1.7.0/pangea/services/__init__.py
+-rw-r--r--   0        0        0    24615 2023-04-10 17:24:06.407418 pangea_sdk-1.7.0/pangea/services/audit/audit.py
+-rw-r--r--   0        0        0      451 2023-03-14 20:28:21.418701 pangea_sdk-1.7.0/pangea/services/audit/exceptions.py
+-rw-r--r--   0        0        0    12230 2023-04-10 17:24:06.407418 pangea_sdk-1.7.0/pangea/services/audit/models.py
+-rw-r--r--   0        0        0     5635 2023-04-10 17:24:06.407418 pangea_sdk-1.7.0/pangea/services/audit/signing.py
+-rw-r--r--   0        0        0     8533 2023-04-10 17:24:06.411419 pangea_sdk-1.7.0/pangea/services/audit/util.py
+-rw-r--r--   0        0        0     1037 2023-04-10 17:24:06.411419 pangea_sdk-1.7.0/pangea/services/base.py
+-rw-r--r--   0        0        0     5565 2023-04-10 17:24:06.411419 pangea_sdk-1.7.0/pangea/services/embargo.py
+-rw-r--r--   0        0        0    33733 2023-04-10 17:24:06.411419 pangea_sdk-1.7.0/pangea/services/intel.py
+-rw-r--r--   0        0        0     7253 2023-04-10 17:24:06.411419 pangea_sdk-1.7.0/pangea/services/redact.py
+-rw-r--r--   0        0        0     1450 2023-03-14 20:28:21.418701 pangea_sdk-1.7.0/pangea/services/vault/models/asymmetric.py
+-rw-r--r--   0        0        0     7847 2023-03-28 15:10:30.783526 pangea_sdk-1.7.0/pangea/services/vault/models/common.py
+-rw-r--r--   0        0        0      481 2023-03-14 20:28:21.422701 pangea_sdk-1.7.0/pangea/services/vault/models/secret.py
+-rw-r--r--   0        0        0     1260 2023-03-14 20:28:21.422701 pangea_sdk-1.7.0/pangea/services/vault/models/symmetric.py
+-rw-r--r--   0        0        0    43335 2023-04-10 17:24:06.411419 pangea_sdk-1.7.0/pangea/services/vault/vault.py
+-rw-r--r--   0        0        0     5472 2023-04-10 17:24:06.411419 pangea_sdk-1.7.0/pangea/tools.py
+-rw-r--r--   0        0        0      554 2023-03-28 15:10:30.783526 pangea_sdk-1.7.0/pangea/utils.py
+-rw-r--r--   0        0        0    10606 2023-04-10 17:24:06.411419 pangea_sdk-1.7.0/pangea/verify_audit.py
+-rw-r--r--   0        0        0      840 2023-04-10 17:17:45.138097 pangea_sdk-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8760 1970-01-01 00:00:00.000000 pangea_sdk-1.7.0/PKG-INFO
```

### Comparing `pangea_sdk-1.6.0/README.md` & `pangea_sdk-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.6.0/pangea/audit_logger.py` & `pangea_sdk-1.7.0/pangea/audit_logger.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.6.0/pangea/config.py` & `pangea_sdk-1.7.0/pangea/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,55 @@
 # Copyright 2022 Pangea Cyber Corporation
 # Author: Pangea Cyber Corporation
 
 from dataclasses import dataclass
+from typing import Optional
 
 
 @dataclass
 class PangeaConfig:
     """Holds run time configuration information used by SDK components."""
 
     domain: str = "aws.us.pangea.cloud"
     environment: str = "production"
 
     """
     Set to true to use plain http
+
     """
     insecure: bool = False
 
     """
     Number of retries on the initial request
+
     """
     request_retries: int = 3
 
     """'
     Backoff strategy passed to 'requests'
+
     """
     request_backoff: int = 1
 
     """
     Timeout used on initial request attempts
+
     """
     request_timeout: int = 5
 
     """
     Enable queued request retry support
     """
     queued_retry_enabled: bool = True
 
     """
     Number of queued request retry attempts, with exponential
     backoff (4 -> 1 + 4 + 9 + 16  = 30 seconds of sleep)
 
     """
     queued_retries: int = 4
+
+    """
+    Extra user agent to be added to request user agent
+
+    """
+    custom_user_agent: Optional[str] = None
```

### Comparing `pangea_sdk-1.6.0/pangea/deep_verify.py` & `pangea_sdk-1.7.0/pangea/deep_verify.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.6.0/pangea/deprecated.py` & `pangea_sdk-1.7.0/pangea/deprecated.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.6.0/pangea/dump_audit.py` & `pangea_sdk-1.7.0/pangea/dump_audit.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.6.0/pangea/exceptions.py` & `pangea_sdk-1.7.0/pangea/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,14 +84,21 @@
     def __init__(self, service_name: str, response: PangeaResponse):
         super(MissingConfigID, self).__init__(
             f"Token did not contain a config scope for service {service_name}. Create a new token or provide a config ID explicitly in the service base",
             response,
         )
 
 
+class NotFound(PangeaAPIException):
+    """Resource not found"""
+
+    def __init__(self, url: str, response: PangeaResponse):
+        super(NotFound, self).__init__(f"Resource not found: {url}", response)
+
+
 class ProviderErrorException(PangeaAPIException):
     """Downstream provider error"""
 
 
 class InternalServerError(PangeaAPIException):
     """A pangea server error"""
```

### Comparing `pangea_sdk-1.6.0/pangea/request.py` & `pangea_sdk-1.7.0/pangea/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright 2022 Pangea Cyber Corporation
 # Author: Pangea Cyber Corporation
 
+import copy
 import json
 import logging
 import time
 from typing import Dict, Union
 
 import pangea
 import requests
@@ -21,33 +22,26 @@
     Wraps Get/Post calls to support both API requests. If `queued_retry_enabled`
     is enabled, the progress of long running Post requests will queried until
     completion or until the `queued_retries` limit is reached. Both values can
     be set in PangeaConfig.
     """
 
     def __init__(self, config: PangeaConfig, token: str, version: str, service: str, logger: logging.Logger):
-        self.config = config
+        self.config = copy.deepcopy(config)
         self.token = token
         self.version = version
         self.service = service
 
-        # TODO: allow overriding these
-        self.retries = config.request_retries
-        self.backoff = config.request_backoff
-        self.timeout = config.request_timeout
-
-        # number of queued retry fetch attempts, with exponential backoff (4 -> 1 + 4 + 9 + 16  = 30 seconds of sleep)
-        self.queued_retries = config.queued_retries
-
         # Queued request retry support flag
         self._queued_retry_enabled = config.queued_retry_enabled
 
         # Custom headers
         self._extra_headers = {}
-        self._custom_user_agent = ""
+        self._user_agent = ""
+        self.set_custom_user_agent(config.custom_user_agent)
         self.session: requests.Session = self._init_session()
 
         self.logger = logger
 
     def __del__(self):
         self.session.close()
 
@@ -61,15 +55,18 @@
             set_extra_headers({ "My-Header" : "foobar" })
         """
 
         if isinstance(headers, dict):
             self._extra_headers = headers
 
     def set_custom_user_agent(self, user_agent: str):
-        self._custom_user_agent = user_agent
+        self.config.custom_user_agent = user_agent
+        self._user_agent = f"pangea-python/{pangea.__version__}"
+        if self.config.custom_user_agent:
+            self._user_agent += f" {self.config.custom_user_agent}"
 
     def queued_support(self, value: bool):
         """Sets or returns the queued retry support mode.
 
         Args:
             value (bool): true - enable queued request retry mode, false - to disable
         """
@@ -115,15 +112,15 @@
 
             pangea_response = self._handle_queued(request_id)
         else:
             pangea_response = PangeaResponse(requests_response)
 
         self.logger.debug(
             json.dumps(
-                {"service": self.service, "action": "post", "url": url, "raw_result": pangea_response.raw_result},
+                {"service": self.service, "action": "post", "url": url, "response": pangea_response.json},
                 default=default_encoder,
             )
         )
         self._check_response(pangea_response)
         return pangea_response
 
     def get(self, endpoint: str, path: str) -> PangeaResponse:
@@ -142,37 +139,37 @@
         self.logger.debug(json.dupms({"service": self.service, "action": "get", "url": url}))
         requests_response = self.session.get(url, headers=self._headers())
 
         pangea_response = PangeaResponse(requests_response)
 
         self.logger.debug(
             json.dumps(
-                {"service": self.service, "action": "post", "url": url, "result": pangea_response.raw_result},
+                {"service": self.service, "action": "post", "url": url, "response": pangea_response.json},
                 default=default_encoder,
             )
         )
         self._check_response(pangea_response)
         return pangea_response
 
     def _handle_queued(self, request_id: str) -> PangeaResponse:
         retry_count = 1
 
         while True:
             time.sleep(retry_count * retry_count)
             pangea_response = self.get("request", request_id)
 
-            if pangea_response.code == 202 and retry_count <= self.queued_retries:
+            if pangea_response.code == 202 and retry_count <= self.config.queued_retries:
                 retry_count += 1
             else:
                 return pangea_response
 
     def _init_session(self) -> requests.Session:
         retry_config = Retry(
-            total=self.retries,
-            backoff_factor=self.backoff,
+            total=self.config.request_retries,
+            backoff_factor=self.config.request_backoff,
         )
 
         adapter = HTTPAdapter(max_retries=retry_config)
         session = requests.Session()
 
         if self.config.insecure:
             session.mount("http://", adapter)
@@ -187,15 +184,15 @@
 
         url = f"{protocol}{domain}/{ str(self.version) + '/' if self.version else '' }{path}"
         return url
 
     def _headers(self) -> dict:
         headers = {
             "Content-Type": "application/json",
-            "User-Agent": f"pangea-python/{pangea.__version__} {self._custom_user_agent}",
+            "User-Agent": self._user_agent,
             "Authorization": f"Bearer {self.token}",
         }
 
         # We want to ignore previous headers if user tryed to set them, so we will overwrite them.
         self._extra_headers.update(headers)
         return self._extra_headers
 
@@ -211,14 +208,15 @@
         self.logger.error(
             json.dumps(
                 {
                     "service": self.service,
                     "action": "api_error",
                     "url": response.raw_response.url,
                     "summary": summary,
+                    "request_id": response.request_id,
                     "result": response.raw_result,
                 }
             )
         )
 
         if status == ResponseStatus.VALIDATION_ERR.value:
             raise exceptions.ValidationException(summary, response)
@@ -232,14 +230,16 @@
             raise exceptions.ServiceNotEnabledException(self.service, response)
         elif status == ResponseStatus.PROVIDER_ERR.value:
             raise exceptions.ProviderErrorException(summary, response)
         elif status in (ResponseStatus.MISSING_CONFIG_ID_SCOPE.value, ResponseStatus.MISSING_CONFIG_ID.value):
             raise exceptions.MissingConfigID(self.service, response)
         elif status == ResponseStatus.SERVICE_NOT_AVAILABLE.value:
             raise exceptions.ServiceNotAvailableException(summary, response)
+        elif status == ResponseStatus.NOT_FOUND.value:
+            raise exceptions.NotFound(response.raw_response.url, response)
         elif status == ResponseStatus.TREE_NOT_FOUND.value:
             raise exceptions.TreeNotFoundException(summary, response)
         elif status == ResponseStatus.IP_NOT_FOUND.value:
             raise exceptions.IPNotFoundException(summary)
         elif status == ResponseStatus.BAD_OFFSET.value:
             raise exceptions.BadOffsetException(summary, response)
         elif status == ResponseStatus.FORBIDDEN_VAULT_OPERATION.value:
```

### Comparing `pangea_sdk-1.6.0/pangea/response.py` & `pangea_sdk-1.7.0/pangea/response.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,17 @@
         extra = "allow"
 
 
 # API request models doesn't not allow arbitrary fields
 class APIRequestModel(BaseModel):
     class Config:
         arbitrary_types_allowed = True
+        extra = (
+            "allow"  # allow parameters despite they are not declared in model. Make SDK accept server new parameters
+        )
         json_encoders = {
             datetime.datetime: format_datetime,
         }
 
 
 class PangeaResponseResult(APIResponseModel):
     pass
@@ -94,28 +97,34 @@
 
 
 class PangeaResponse(Generic[T], ResponseHeader):
     raw_result: Optional[Dict[str, Any]] = None
     raw_response: Optional[requests.Response] = None
     result: Optional[T] = None
     pangea_error: Optional[PangeaError] = None
+    _json: Any
 
     def __init__(self, response: requests.Response):
-        json = response.json()
-        super(PangeaResponse, self).__init__(**json)
+        _json = response.json()
+        super(PangeaResponse, self).__init__(**_json)
+        self._json = _json
         self.raw_response = response
-        self.raw_result = json["result"]
+        self.raw_result = self._json["result"]
         self.result = (
-            T(**json["result"])
+            T(**self._json["result"])
             if issubclass(type(T), PangeaResponseResult) and self.status == ResponseStatus.SUCCESS.value
             else None
         )
         if not self.success:
             self.pangea_error = PangeaError(**self.raw_result) if self.raw_result is not None else None
 
     @property
     def success(self) -> bool:
         return self.status == ResponseStatus.SUCCESS.value
 
     @property
     def errors(self) -> List[ErrorField]:
         return self.pangea_error.errors if self.pangea_error is not None else []
+
+    @property
+    def json(self) -> Any:
+        return self._json
```

### Comparing `pangea_sdk-1.6.0/pangea/services/audit/audit.py` & `pangea_sdk-1.7.0/pangea/services/audit/audit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright 2022 Pangea Cyber Corporation
 # Author: Pangea Cyber Corporation
 import datetime
+import json
 from typing import Dict, Optional, Union
 
 from pangea.response import PangeaResponse
 from pangea.services.audit.exceptions import AuditException, EventCorruption
 from pangea.services.audit.models import (
     Event,
     EventEnvelope,
@@ -23,15 +24,14 @@
     SearchOutput,
     SearchRequest,
     SearchResultOutput,
     SearchResultRequest,
 )
 from pangea.services.audit.signing import Signer, Verifier
 from pangea.services.audit.util import (
-    b64encode_ascii,
     canonicalize_event,
     decode_consistency_proof,
     decode_hash,
     decode_membership_proof,
     format_datetime,
     get_arweave_published_roots,
     get_public_key,
@@ -69,22 +69,24 @@
     version: str = "v1"
 
     def __init__(
         self,
         token,
         config=None,
         private_key_file: str = "",
+        public_key_info: Dict[str, str] = {},
         tenant_id: Optional[str] = None,
         logger_name="pangea",
     ):
         super().__init__(token, config, logger_name)
 
         self.pub_roots: Dict[int, Root] = {}
         self.buffer_data: Optional[str] = None
         self.signer: Optional[Signer] = Signer(private_key_file) if private_key_file else None
+        self.public_key_info = public_key_info
 
         # In case of Arweave failure, ask the server for the roots
         self.allow_server_roots = True
         self.prev_unpublished_root_hash: Optional[str] = None
         self.tenant_id = tenant_id
 
     def log(
@@ -96,14 +98,16 @@
         old: Optional[Union[str, dict]] = None,
         source: Optional[str] = None,
         status: Optional[str] = None,
         target: Optional[str] = None,
         timestamp: Optional[datetime.datetime] = None,
         verify: bool = False,
         signing: EventSigning = EventSigning.NONE,
+        signature_key_id: Optional[str] = None,
+        signature_key_version: Optional[str] = None,
         verbose: Optional[bool] = None,
     ) -> PangeaResponse[LogResult]:
         """
         Log an entry
 
         Create a log entry in the Secure Audit Log.
         Args:
@@ -163,16 +167,21 @@
             data2sign = canonicalize_event(event)
             signature = self.signer.signMessage(data2sign)
             if signature is not None:
                 input.signature = signature
             else:
                 raise AuditException("Error: failure signing message")
 
-            public_bytes = self.signer.getPublicKeyBytes()
-            input.public_key = b64encode_ascii(public_bytes)
+            # Add public key value to public key info and serialize
+            self.set_public_key(input, self.signer, self.public_key_info)
+
+        elif signing == EventSigning.VAULT:
+            input.sign = True
+            input.signature_key_id = signature_key_id
+            input.signature_key_version = signature_key_version
 
         if verify:
             input.verbose = True
             if self.prev_unpublished_root_hash:
                 input.prev_root = self.prev_unpublished_root_hash
 
         response = self.request.post(endpoint_name, data=input.dict(exclude_none=True))
@@ -533,20 +542,14 @@
 
         curr_root_hash = decode_hash(curr_root.root_hash)
         prev_root_hash = decode_hash(prev_root.root_hash)
         proof = decode_consistency_proof(curr_root.consistency_proof)
 
         return verify_consistency_proof(curr_root_hash, prev_root_hash, proof)
 
-    def has_valid_public_key(self, key: Optional[str]) -> bool:
-        if key and not key.startswith("-----"):
-            return True
-
-        return False
-
     def verify_signature(self, audit_envelope: EventEnvelope) -> EventVerification:
         """
         Verify signature
 
         Args:
             audit_envelope (EventEnvelope): Object to verify
 
@@ -564,14 +567,20 @@
             if verification is not None:
                 return EventVerification.PASS if verification else EventVerification.FAIL
             else:
                 return EventVerification.NONE
         else:
             return EventVerification.NONE
 
+    def set_public_key(self, input: LogRequest, signer: Signer, public_key_info: Dict[str, str]):
+        public_key_info["key"] = signer.getPublicKeyPEM()
+        input.public_key = json.dumps(
+            public_key_info, ensure_ascii=False, allow_nan=False, separators=(",", ":"), sort_keys=True
+        )
+
     def root(self, tree_size: Optional[int] = None) -> PangeaResponse[RootResult]:
         """
         Retrieve tamperproof verification
 
         Returns current root hash and consistency proof.
 
         Args:
```

### Comparing `pangea_sdk-1.6.0/pangea/services/audit/models.py` & `pangea_sdk-1.7.0/pangea/services/audit/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     def __repr__(self):
         return str(self.value)
 
 
 class EventSigning(enum.Enum):
     NONE = 0
     LOCAL = 1
+    VAULT = 2
 
     def __str__(self):
         return str(self.value)
 
     def __repr__(self):
         return str(self.value)
 
@@ -123,14 +124,17 @@
     """
 
     event: Event
     verbose: Optional[bool] = None
     signature: Optional[str] = None
     public_key: Optional[str] = None
     prev_root: Optional[str] = None
+    sign: Optional[bool] = None
+    signature_key_id: Optional[str] = None
+    signature_key_version: Optional[str] = None
 
 
 class LogResult(PangeaResponseResult):
     """
     Result class after an audit log action
 
     envelope -- Event envelope information.
```

### Comparing `pangea_sdk-1.6.0/pangea/services/audit/signing.py` & `pangea_sdk-1.7.0/pangea/services/audit/signing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright 2022 Pangea Cyber Corporation
 # Author: Pangea Cyber Corporation
 from base64 import b64decode, b64encode
-from typing import Dict, Union
+from typing import Dict, Optional, Union
 
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import ed25519
+from cryptography.hazmat.primitives.asymmetric.types import PUBLIC_KEY_TYPES
 from pangea.services.audit.util import b64decode_ascii, canonicalize_json
 
 
 class Signer:
     def __init__(self, private_key_file: str) -> None:
         self._private_key = None
         self._private_key_filename = private_key_file
@@ -64,58 +65,68 @@
             return self._signMessageJSON(message, private_key)
 
         elif isinstance(message, bytes):
             return self._signMessageBytes(message, private_key)
         else:
             raise Exception("Error: Not supported instance")
 
-    def getPublicKeyBytes(self):
+    def getPublicKeyBytes(self) -> bytes:
         return (
             self._getPrivateKey()
             .public_key()
             .public_bytes(encoding=serialization.Encoding.Raw, format=serialization.PublicFormat.Raw)
         )
 
+    def getPublicKeyPEM(self) -> str:
+        return (
+            self._getPrivateKey()
+            .public_key()
+            .public_bytes(encoding=serialization.Encoding.PEM, format=serialization.PublicFormat.SubjectPublicKeyInfo)
+            .decode("utf-8")
+        )
+
 
 class Verifier:
     # verify message with signature and public key bytes
-    def verifyMessage(self, signature_b64: str, message: Union[str, dict, bytes], public_key_b64: str = None) -> bool:
-        try:
-            public_key_bytes = b64decode_ascii(public_key_b64)
-        except Exception:
-            return False
-
-        try:
+    def verifyMessage(
+        self, signature_b64: str, message: Union[str, dict, bytes], public_key_input: str = None
+    ) -> Optional[bool]:
+        if self._is_pem_format(public_key_input):
+            public_key = serialization.load_pem_public_key(bytes(public_key_input, "utf-8"))
+            if not isinstance(public_key, ed25519.Ed25519PublicKey):
+                # TODO: Add support for other public key formats
+                return None
+        else:
+            # To make backward compatible with original public keys send encoded bytes in base64
+            public_key_bytes = b64decode_ascii(public_key_input)
             public_key = ed25519.Ed25519PublicKey.from_public_bytes(public_key_bytes)
-        except ValueError:
-            raise Exception("Error: Not supported key instance")
 
         if isinstance(message, str):
             return self._verifyMessageStr(signature_b64, message, public_key)
         elif isinstance(message, dict):
             return self._verifyMessageJSON(signature_b64, message, public_key)
         elif isinstance(message, bytes):
             return self._verifyMessageBytes(signature_b64, message, public_key)
         else:
             raise Exception("Error: Not supported instance")
 
+    def _is_pem_format(self, key: str) -> bool:
+        return key.startswith("-----")
+
     # Verify a message in bytes using Ed25519 algorithm
-    def _verifyMessageBytes(
-        self, signature_b64: str, message_bytes: bytes, public_key: ed25519.Ed25519PublicKey
-    ) -> bool:
+    def _verifyMessageBytes(self, signature_b64: str, message_bytes: bytes, public_key: PUBLIC_KEY_TYPES) -> bool:
         try:
             signature = b64decode(signature_b64)
             public_key.verify(signature, message_bytes)
+            return True
         except Exception:
             return False
 
-        return True
-
     # Verify a string message using Ed25519 algorithm
-    def _verifyMessageStr(self, signature_b64: str, message: str, public_key: ed25519.Ed25519PublicKey) -> bool:
+    def _verifyMessageStr(self, signature_b64: str, message: str, public_key: PUBLIC_KEY_TYPES) -> bool:
         message_bytes = bytes(message, "utf8")
         return self._verifyMessageBytes(signature_b64, message_bytes, public_key)
 
     # Verify a JSON message using Ed25519 algorithm
-    def _verifyMessageJSON(self, signature_b64: str, messageJSON: dict, public_key: ed25519.Ed25519PublicKey) -> bool:
+    def _verifyMessageJSON(self, signature_b64: str, messageJSON: dict, public_key: PUBLIC_KEY_TYPES) -> bool:
         message_bytes = canonicalize_json(messageJSON)
         return self._verifyMessageBytes(signature_b64, message_bytes, public_key)
```

### Comparing `pangea_sdk-1.6.0/pangea/services/audit/util.py` & `pangea_sdk-1.7.0/pangea/services/audit/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,14 +126,31 @@
                     node_hash=decode_hash(item[:ndx].split(":")[1]),
                     proof=decode_membership_proof(item[ndx + 1 :]),
                 )
             )
     return root_proof
 
 
+def get_public_key(public_key_info: Optional[str]) -> Optional[str]:
+    if not public_key_info:
+        return None
+
+    try:
+        # Try to parse key_info as a json
+        key_info: dict = json.loads(public_key_info)
+        # If it's a json, public key come in "key" field
+        key = key_info.pop("key", None)
+        return key
+    except json.JSONDecodeError:
+        pass
+
+    # If it's not a json, public key should be used as a string
+    return public_key_info
+
+
 def verify_membership_proof(node_hash: Hash, root_hash: Hash, proof: MembershipProof) -> bool:
     for proof_item in proof:
         proof_hash = proof_item.node_hash
         node_hash = hash_pair(proof_hash, node_hash) if proof_item.side == "left" else hash_pair(node_hash, proof_hash)
     return root_hash == node_hash
```

### Comparing `pangea_sdk-1.6.0/pangea/services/base.py` & `pangea_sdk-1.7.0/pangea/services/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright 2022 Pangea Cyber Corporation
 # Author: Pangea Cyber Corporation
 
+import copy
 import logging
 from typing import Optional
 
 from pangea import __version__
 from pangea.config import PangeaConfig
 from pangea.request import PangeaRequest
 
@@ -13,15 +14,15 @@
     service_name: str = "base"
     version: str = "v1"
 
     def __init__(self, token, config: Optional[PangeaConfig] = None, logger_name: str = "pangea"):
         if not token:
             raise Exception("No token provided")
 
-        self.config = config if config else PangeaConfig()
+        self.config = config if copy.deepcopy(config) else PangeaConfig()
         self.logger = logging.getLogger(logger_name)
 
         self.request = PangeaRequest(
             self.config,
             token,
             self.version,
             self.service_name,
```

### Comparing `pangea_sdk-1.6.0/pangea/services/embargo.py` & `pangea_sdk-1.7.0/pangea/services/embargo.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.6.0/pangea/services/intel.py` & `pangea_sdk-1.7.0/pangea/services/intel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Copyright 2022 Pangea Cyber Corporation
 # Author: Pangea Cyber Corporation
+import enum
 import hashlib
 from typing import Dict, List, Optional
 
 from pangea.deprecated import pangea_deprecated
 from pangea.response import APIRequestModel, APIResponseModel, PangeaResponse, PangeaResponseResult
 
 from .base import ServiceBase
@@ -256,14 +257,26 @@
     """
     URL Reputation result
     """
 
     data: URLReputationData
 
 
+class HashType(str, enum.Enum):
+    SHA256 = "sha256"
+    SHA1 = "sha1"
+    MD5 = "md5"
+
+    def __str__(self):
+        return str(self.value)
+
+    def __repr__(self):
+        return str(self.value)
+
+
 class FileIntel(ServiceBase):
     """File Intel service client
 
     Provides methods to interact with [Pangea File Intel Service](https://pangea.cloud/docs/api/file-intel)
 
     The following information is needed:
         PANGEA_TOKEN - service token which can be found on the Pangea User
@@ -810,7 +823,202 @@
             response = url_intel.reputation(url="http://113.235.101.11:54384", provider="crowdstrike")
         """
 
         input = URLReputationRequest(url=url, provider=provider, verbose=verbose, raw=raw)
         response = self.request.post("reputation", data=input.dict(exclude_none=True))
         response.result = URLReputationResult(**response.raw_result)
         return response
+
+
+class UserBreachedRequest(IntelCommonRequest):
+    """
+    User breached common request data
+
+    email (str): An email address to search for
+    username (str): An username to search for
+    ip (str): An ip to search for
+    phone_number (str): A phone number to search for. minLength: 7, maxLength: 15.
+    start (str): Earliest date for search
+    end (str): Latest date for search
+    """
+
+    email: Optional[str] = None
+    username: Optional[str] = None
+    ip: Optional[str] = None
+    phone_number: Optional[str] = None
+    start: Optional[str] = None
+    end: Optional[str] = None
+
+
+class UserBreachedCommonData(APIResponseModel):
+    """
+    User breached common information
+    """
+
+    found_in_breach: bool
+    breach_count: int
+
+
+class UserBreachedData(UserBreachedCommonData):
+    """
+    User breached information
+    """
+
+    pass
+
+
+class UserBreachedResult(IntelCommonResult):
+    """
+    User breached result
+    """
+
+    data: UserBreachedData
+
+
+class UserPasswordBreachedRequest(IntelCommonRequest):
+    """
+    User password breached common request data
+
+    hash_type (str): Hash type to be looked up
+    hash_prefix (str): The prefix of the hash to be looked up.
+    """
+
+    hash_type: str
+    hash_prefix: str
+
+
+class UserPasswordBreachedData(UserBreachedCommonData):
+    """
+    User password breached information
+    """
+
+    pass
+
+
+class UserPasswordBreachedResult(IntelCommonResult):
+    """
+    User password breached result
+    """
+
+    data: UserPasswordBreachedData
+
+
+class UserIntel(ServiceBase):
+    """User Intel service client.
+
+    Provides methods to interact with [Pangea User Intel Service](/docs/api/user-intel)
+
+    The following information is needed:
+        PANGEA_TOKEN - service token which can be found on the Pangea User
+            Console at [https://console.pangea.cloud/project/tokens](https://console.pangea.cloud/project/tokens)
+
+    Examples:
+        import os
+
+        # Pangea SDK
+        from pangea.config import PangeaConfig
+        from pangea.services import UserIntel
+
+        PANGEA_TOKEN = os.getenv("PANGEA_TOKEN")
+
+        user_intel_config = PangeaConfig(domain="pangea.cloud")
+
+        # Setup Pangea User Intel service
+        user_intel = UserIntel(token=PANGEA_TOKEN, config=user_intel_config)
+    """
+
+    service_name = "user-intel"
+    version = "v1"
+
+    def user_breached(
+        self,
+        email: Optional[str] = None,
+        username: Optional[str] = None,
+        ip: Optional[str] = None,
+        phone_number: Optional[str] = None,
+        start: Optional[str] = None,
+        end: Optional[str] = None,
+        verbose: Optional[bool] = None,
+        raw: Optional[bool] = None,
+        provider: Optional[str] = None,
+    ) -> PangeaResponse[UserBreachedResult]:
+        """
+        Look up breached users
+
+        Find out if an email address, username, phone number, or IP address was exposed in a security breach.
+
+        Args:
+            email (str): An email address to search for
+            username (str): An username to search for
+            ip (str): An ip to search for
+            phone_number (str): A phone number to search for. minLength: 7, maxLength: 15.
+            start (str): Earliest date for search
+            end (str): Latest date for search
+            verbose (bool, optional): Echo the API parameters in the response
+            raw (bool, optional): Include raw data from this provider
+            provider (str, optional): Use reputation data from this provider: "crowdstrike"
+
+        Raises:
+            PangeaAPIException: If an API Error happens
+
+        Returns:
+            A PangeaResponse where the sanctioned source(s) are in the
+                response.result field.  Available response fields can be found in our [API documentation](/docs/api/url-intel)
+
+        Examples:
+            response = self.intel_user.user_breached(
+                phone_number="8005550123", provider="spycloud", verbose=True, raw=True
+            )
+        """
+
+        input = UserBreachedRequest(
+            email=email,
+            phone_number=phone_number,
+            username=username,
+            ip=ip,
+            provider=provider,
+            start=start,
+            end=end,
+            verbose=verbose,
+            raw=raw,
+        )
+        response = self.request.post("user/breached", data=input.dict(exclude_none=True))
+        response.result = UserBreachedResult(**response.raw_result)
+        return response
+
+    def password_breached(
+        self,
+        hash_type: HashType,
+        hash_prefix: str,
+        verbose: Optional[bool] = None,
+        raw: Optional[bool] = None,
+        provider: Optional[str] = None,
+    ) -> PangeaResponse[UserPasswordBreachedResult]:
+        """
+        Look up breached passwords
+
+        Find out if a password has been exposed in security breaches by providing a 5 character prefix of the password hash.
+
+        Args:
+            hash_type (str): Hash type to be looked up
+            hash_prefix (str): The prefix of the hash to be looked up.
+            verbose (bool, optional): Echo the API parameters in the response
+            raw (bool, optional): Include raw data from this provider
+            provider (str, optional): Use reputation data from this provider: "crowdstrike"
+
+        Raises:
+            PangeaAPIException: If an API Error happens
+
+        Returns:
+            A PangeaResponse where the sanctioned source(s) are in the
+                response.result field.  Available response fields can be found in our [API documentation](/docs/api/url-intel)
+
+        Examples:
+            response = self.intel_user.password_breached(hash_prefix="5baa6", hash_type=HashType.SHA256, provider="spycloud")
+        """
+
+        input = UserPasswordBreachedRequest(
+            hash_type=hash_type, hash_prefix=hash_prefix, provider=provider, verbose=verbose, raw=raw
+        )
+        response = self.request.post("password/breached", data=input.dict(exclude_none=True))
+        response.result = UserPasswordBreachedResult(**response.raw_result)
+        return response
```

### Comparing `pangea_sdk-1.6.0/pangea/services/redact.py` & `pangea_sdk-1.7.0/pangea/services/redact.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     """
     Input class to make a redact request
     """
 
     text: str
     debug: Optional[bool] = None
     rules: Optional[List[str]] = None
+    return_result: Optional[bool] = None
 
 
 class RecognizerResult(APIResponseModel):
     """
     The scoring result of a rule
 
     Arguments:
@@ -61,15 +62,15 @@
 
     Arguments:
     redact_text: Redacted text result
     count: Number of redactions present in the text
     report: Describes the decision process for redactions
     """
 
-    redacted_text: str
+    redacted_text: Optional[str] = None
     count: int
     report: Optional[DebugReport] = None
 
 
 class StructuredRequest(APIRequestModel):
     """
     Class input to redact structured data request
@@ -82,23 +83,24 @@
     """
 
     data: Union[Dict, str]
     jsonp: Optional[List[str]] = None
     format: Optional[RedactFormat] = None
     debug: Optional[bool] = None
     rules: Optional[List[str]] = None
+    return_result: Optional[bool] = None
 
 
 class StructuredResult(PangeaResponseResult):
     """
     Result class after a structured redact request
 
     """
 
-    redacted_data: Union[Dict, str]
+    redacted_data: Optional[Union[Dict, str]] = None
     count: int
     report: Optional[DebugReport] = None
 
 
 class RedactFormat(str, enum.Enum):
     JSON = "json"
 
@@ -136,51 +138,57 @@
         token,
         config=None,
         logger_name="pangea",
     ):
         super().__init__(token, config, logger_name)
 
     def redact(
-        self, text: str, debug: Optional[bool] = None, rules: Optional[List[str]] = None
+        self,
+        text: str,
+        debug: Optional[bool] = None,
+        rules: Optional[List[str]] = None,
+        return_result: Optional[bool] = None,
     ) -> PangeaResponse[RedactResult]:
         """
         Redact
 
         Redacts the content of a single text string
 
         Args:
             text (str): The text to be redacted
             debug (bool, optional): Setting this value to true will provide a detailed analysis of
                 the redacted data and the rules that caused redaction
             rules (list[str], optional): An array of redact rule short names
+            return_result(bool, optional): Setting this value to false will omit the redacted result only returning count
 
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             Pangea Response with redacted text in the response.result property,
                 available response fields can be found in our
                 [API Documentation](https://pangea.cloud/docs/api/redact#redact).
 
         Examples:
             response = redact.redact(text="Jenny Jenny... 415-867-5309")
         """
 
-        input = RedactRequest(text=text, debug=debug, rules=rules)
+        input = RedactRequest(text=text, debug=debug, rules=rules, return_result=return_result)
         response = self.request.post("redact", data=input.dict(exclude_none=True))
         response.result = RedactResult(**response.raw_result)
         return response
 
     def redact_structured(
         self,
         data: Union[Dict, str],
         jsonp: Optional[List[str]] = None,
         format: Optional[RedactFormat] = None,
         debug: Optional[bool] = None,
         rules: Optional[List[str]] = None,
+        return_result: Optional[bool] = None,
     ) -> PangeaResponse[StructuredResult]:
         """
         Redact structured
 
         Redacts text within a structured object
 
         Args:
@@ -188,24 +196,27 @@
             jsonp (list[str]): JSON path(s) used to identify the specific JSON fields to redact in
                 the structured data. Note: If jsonp parameter is used, the data parameter must be
                 in JSON format.
             format (RedactFormat, optional): The format of the passed data. Default: "json"
             debug (bool, optional): Setting this value to true will provide a detailed analysis of
                 the redacted data and the rules that caused redaction
             rules (list[str], optional): An array of redact rule short names
+            return_result(bool, optional): Setting this value to false will omit the redacted result only returning count
 
         Raises:
             PangeaAPIException: If an API Error happens
 
         Returns:
             Pangea Response with redacted data in the response.result field,
                 available response fields can be found in our
                 [API Documentation](https://pangea.cloud/docs/api/redact#redact-structured)
 
         Examples:
             response = redact.redact_structured(data={"number": "415-867-5309", "ip": "1.1.1.1"}, redact_format="json")
         """
 
-        input = StructuredRequest(data=data, jsonp=jsonp, format=format, debug=debug, rules=rules)
+        input = StructuredRequest(
+            data=data, jsonp=jsonp, format=format, debug=debug, rules=rules, return_result=return_result
+        )
         response = self.request.post("redact_structured", data=input.dict(exclude_none=True))
         response.result = StructuredResult(**response.raw_result)
         return response
```

### Comparing `pangea_sdk-1.6.0/pangea/services/vault/models/asymmetric.py` & `pangea_sdk-1.7.0/pangea/services/vault/models/asymmetric.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.6.0/pangea/services/vault/models/common.py` & `pangea_sdk-1.7.0/pangea/services/vault/models/common.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.6.0/pangea/services/vault/models/symmetric.py` & `pangea_sdk-1.7.0/pangea/services/vault/models/symmetric.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.6.0/pangea/tools.py` & `pangea_sdk-1.7.0/pangea/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -129,14 +129,23 @@
     value = os.getenv(env_var_name)
     if not value:
         raise PangeaException(f"{env_var_name} env var need to be set")
 
     return value
 
 
+def get_vault_signature_test_token(environment: TestEnvironment):
+    env_var_name = f"PANGEA_INTEGRATION_VAULT_TOKEN_{environment}"
+    value = os.getenv(env_var_name)
+    if not value:
+        raise PangeaException(f"{env_var_name} env var need to be set")
+
+    return value
+
+
 class SequenceFollower:
     """
     Follows an unordered sequence of integers, looking for holes
     """
 
     def __init__(self):
         self.numbers = set()
```

### Comparing `pangea_sdk-1.6.0/pangea/utils.py` & `pangea_sdk-1.7.0/pangea/utils.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.6.0/pangea/verify_audit.py` & `pangea_sdk-1.7.0/pangea/verify_audit.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from pangea.services.audit.signing import Verifier
 from pangea.services.audit.util import (
     canonicalize_json,
     decode_consistency_proof,
     decode_hash,
     decode_membership_proof,
     get_arweave_published_roots,
+    get_public_key,
     hash_bytes,
     verify_consistency_proof,
     verify_membership_proof,
 )
 
 logger = logging.getLogger("audit")
 pub_roots: t.Dict[int, t.Dict] = {}
@@ -94,17 +95,15 @@
         succeeded = False
 
     log_result("Data hash verification", succeeded)
     logger.info("")
     return succeeded
 
 
-def _verify_unpublished_membership_proof(
-    root_hash, node_hash: str, proof: t.Optional[str]
-) -> t.Optional[bool]:
+def _verify_unpublished_membership_proof(root_hash, node_hash: str, proof: t.Optional[str]) -> t.Optional[bool]:
     global pub_roots
 
     log_section("Checking unpublished membership proof")
 
     if proof is None:
         succeeded = None
         logger.debug("Proof not found")
@@ -115,15 +114,15 @@
             node_hash_dec = decode_hash(node_hash)
 
             logger.debug("Calculating the proof")
             proof_dec = decode_membership_proof(proof)
 
             logger.debug("Comparing the unpublished root hash with the proof hash")
             succeeded = verify_membership_proof(node_hash_dec, root_hash_dec, proof_dec)
-        
+
         except Exception as e:
             succeeded = False
             logger.debug(str(e))
 
     log_result("Unpublished membership proof verification", succeeded)
     logger.info("")
     return succeeded
@@ -208,18 +207,18 @@
     if "signature" not in data:
         logger.debug("Signature is not present")
         succeeded = None
     else:
         try:
             logger.debug("Obtaining signature and public key from the event")
             sign_envelope = create_signed_envelope(data["event"])
-            public_key_b64 = data["public_key"]
+            public_key = get_public_key(data["public_key"])
             sign_verifier = Verifier()
             logger.debug("Checking the signature")
-            if not sign_verifier.verifyMessage(data["signature"], sign_envelope, public_key_b64):
+            if not sign_verifier.verifyMessage(data["signature"], sign_envelope, public_key):
                 raise ValueError("Signature is invalid")
             succeeded = True
         except Exception:
             succeeded = False
 
     log_result("Data signature verification", succeeded)
     logger.info("")
@@ -230,18 +229,15 @@
     """
     Verify a list of events.
     Returns a status.
     """
 
     succeeded = []
     for counter, event in enumerate(events):
-        event.update({
-            "root": root,
-            "unpublished_root": unpublished_root
-        })
+        event.update({"root": root, "unpublished_root": unpublished_root})
         event_succeeded = verify_single(event, counter + 1)
         succeeded.append(event_succeeded)
     return not any(event_succeeded is False for event_succeeded in succeeded)
 
 
 def verify_single(data: t.Dict, counter: t.Optional[int] = None) -> t.Optional[bool]:
     """
@@ -264,25 +260,28 @@
             data["hash"],
             data.get("membership_proof"),
         )
     else:
         if not data.get("unpublished_root"):
             raise ValueError("Missing 'unpublished_root' element")
         ok_membership = _verify_unpublished_membership_proof(
-            data["unpublished_root"]["root_hash"],
-            data["hash"],
-            data.get("membership_proof")
+            data["unpublished_root"]["root_hash"], data["hash"], data.get("membership_proof")
         )
 
     if data["published"]:
         ok_consistency = _verify_consistency_proof(data["root"]["tree_name"], data.get("leaf_index"))
     else:
         ok_consistency = True
 
-    all_ok = ok_hash is True and (ok_signature is True or ok_signature is None) and ok_membership is True and ok_consistency is True
+    all_ok = (
+        ok_hash is True
+        and (ok_signature is True or ok_signature is None)
+        and ok_membership is True
+        and ok_consistency is True
+    )
     any_failed = ok_hash is False or ok_signature is False or ok_membership is False or ok_consistency is False
 
     if counter:
         formatter.indent = 0
 
     if all_ok:
         return True
```

### Comparing `pangea_sdk-1.6.0/pyproject.toml` & `pangea_sdk-1.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pangea-sdk"
-version = "1.6.0"
+version = "1.7.0"
 description = "Pangea API SDK"
 authors = ["Glenn Gallien <glenn.gallien@pangea.cloud>"]
 license = "MIT"
 readme = "README.md"
 homepage = ""
 repository = ""
 keywords = ["Pangea", "SDK", "Audit"]
```

### Comparing `pangea_sdk-1.6.0/PKG-INFO` & `pangea_sdk-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangea-sdk
-Version: 1.6.0
+Version: 1.7.0
 Summary: Pangea API SDK
 License: MIT
 Keywords: Pangea,SDK,Audit
 Author: Glenn Gallien
 Author-email: glenn.gallien@pangea.cloud
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```


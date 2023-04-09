# Comparing `tmp/singular_client-0.1.0.tar.gz` & `tmp/singular_client-0.1.1.tar.gz`

## Comparing `singular_client-0.1.0.tar` & `singular_client-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 singular_client-0.1.0/singular_client/__init__.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 singular_client-0.1.0/singular_client/_utils.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 singular_client-0.1.0/singular_client/api.py
--rwxr-xr-x   0        0        0     6543 2020-02-02 00:00:00.000000 singular_client-0.1.0/singular_client/arguments.py
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 singular_client-0.1.0/singular_client/documents.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 singular_client-0.1.0/singular_client/processing.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 singular_client-0.1.0/singular_client/endpoints/__init__.py
--rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 singular_client-0.1.0/singular_client/endpoints/_bases.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 singular_client-0.1.0/singular_client/endpoints/governance.py
--rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 singular_client-0.1.0/singular_client/endpoints/links.py
--rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 singular_client-0.1.0/singular_client/endpoints/links_legacy.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 singular_client-0.1.0/singular_client/endpoints/monetization.py
--rw-r--r--   0        0        0     8352 2020-02-02 00:00:00.000000 singular_client-0.1.0/singular_client/endpoints/reporting.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 singular_client-0.1.0/singular_client/endpoints/skan.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 singular_client-0.1.0/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 singular_client-0.1.0/README.md
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 singular_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 singular_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/__init__.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/_utils.py
+-rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/api.py
+-rwxr-xr-x   0        0        0     6543 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/arguments.py
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/documents.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/processing.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/endpoints/__init__.py
+-rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/endpoints/_bases.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/endpoints/governance.py
+-rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/endpoints/links.py
+-rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/endpoints/links_legacy.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/endpoints/monetization.py
+-rw-r--r--   0        0        0     8387 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/endpoints/reporting.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/endpoints/skan.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 singular_client-0.1.1/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 singular_client-0.1.1/README.md
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 singular_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 singular_client-0.1.1/PKG-INFO
```

### Comparing `singular_client-0.1.0/singular_client/_utils.py` & `singular_client-0.1.1/singular_client/_utils.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.0/singular_client/api.py` & `singular_client-0.1.1/singular_client/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 import requests
 from typing import (
     Optional,
     Literal,
 )
 
-from singular.documents import *
-from singular._utils import *
-from singular.arguments import *
+from singular_client.documents import *
+from singular_client._utils import *
+from singular_client.arguments import *
 
 
 class SingularAPI:
     """
     A simple class to store endpoint instances, and handle authentication and base url
     when requesting data from the Singular API.
 
@@ -23,15 +23,15 @@
     logs = True
 
     key: str
 
     def __init__(self, key: str):
         self.key = key
 
-        from singular import endpoints
+        from singular_client import endpoints
         # Reporting
         self.combined_report = endpoints.CombinedReportEndpoint(self)
         self.network_report = endpoints.NetworkReportEndpoint(self)
         self.tracker_report = endpoints.TrackerReportEndpoint(self)
         self.data_availability = endpoints.DataAvailabilityEndpoint(self)
         self.report_status = endpoints.ReportStatusEndpoint(self)
         self.filters = endpoints.FiltersEndpoint(self)
```

### Comparing `singular_client-0.1.0/singular_client/arguments.py` & `singular_client-0.1.1/singular_client/arguments.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.0/singular_client/documents.py` & `singular_client-0.1.1/singular_client/documents.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.0/singular_client/endpoints/_bases.py` & `singular_client-0.1.1/singular_client/endpoints/_bases.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     Type,
     get_args,
     get_type_hints,
 )
 from inspect import signature
 
 if TYPE_CHECKING:
-    from singular.api import SingularAPI
+    from singular_client.api import SingularAPI
 
 
 D = TypeVar("D", bound=Union[TypedDict, dict])
 
 
 class ResponseDocList(Generic[D], List[D]):
     pass
```

### Comparing `singular_client-0.1.0/singular_client/endpoints/links.py` & `singular_client-0.1.1/singular_client/endpoints/links.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from singular.endpoints._bases import _Endpoint, ResponseDocList
-from singular.documents import *
-from singular.arguments import *
-from singular._utils import *
+from singular_client.endpoints._bases import _Endpoint, ResponseDocList
+from singular_client.documents import *
+from singular_client.arguments import *
+from singular_client._utils import *
 from typing import *
 
 
 class DomainsEndpoint(_Endpoint[ResponseDocList[DomainDoc]]):
     endpoint = "v1/singular_links/domains"
     data_path = ["available_domains"]
     res_type = ResponseDocList[DomainDoc]
```

### Comparing `singular_client-0.1.0/singular_client/endpoints/links_legacy.py` & `singular_client-0.1.1/singular_client/endpoints/links_legacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from singular.endpoints._bases import _Endpoint, ResponseDocList
-from singular.documents import *
-from singular._utils import *
+from singular_client.endpoints._bases import _Endpoint, ResponseDocList
+from singular_client.documents import *
+from singular_client._utils import *
 from typing import *
 
 class AppsLegacyEndpoint(_Endpoint[ResponseDocList[AppLegacyDoc]]):
     endpoint = "v1/links/discover_apps"
     data_path = ["available_apps"]
     res_type = ResponseDocList[AppLegacyDoc]
```

### Comparing `singular_client-0.1.0/singular_client/endpoints/monetization.py` & `singular_client-0.1.1/singular_client/endpoints/monetization.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from singular.endpoints._bases import _Endpoint, ResponseDocList
-from singular.documents import *
-from singular.arguments import *
+from singular_client.endpoints._bases import _Endpoint, ResponseDocList
+from singular_client.documents import *
+from singular_client.arguments import *
 from typing import *
-from singular._utils import *
+from singular_client._utils import *
 
 class AdMonetizationEndpoint(_Endpoint[ResponseDocList[AdMonetizationDoc]]):
     endpoint = "v2.0/admonetization/reporting"
     data_path = ["value", "results"]
     res_type = ResponseDocList[AdMonetizationDoc]
 
     def request(
```

### Comparing `singular_client-0.1.0/singular_client/endpoints/reporting.py` & `singular_client-0.1.1/singular_client/endpoints/reporting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from singular.endpoints._bases import _Endpoint, ResponseDocList
-from singular.documents import *
-from singular.arguments import *
-from singular._utils import convert_list_arg
+from singular_client.endpoints._bases import _Endpoint, ResponseDocList
+from singular_client.documents import *
+from singular_client.arguments import *
+from singular_client._utils import convert_list_arg
 import pandas as pd
 import json
 import time
 import requests
 import io
 from typing import *
 
 if TYPE_CHECKING:
-    from singular.api import SingularAPI
+    from singular_client.api import SingularAPI
     import pandas as pd
 
 
 class ReportStatusResponse:
     cached_download: Optional[Union[requests.Response, "pd.DataFrame"]]
     status: ReportStatusDoc
     failed = property(lambda x: x.status["status"] == "FAILED")
```

### Comparing `singular_client-0.1.0/singular_client/endpoints/skan.py` & `singular_client-0.1.1/singular_client/endpoints/skan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from singular.endpoints._bases import _Endpoint, ResponseDocList
-from singular.documents import *
-from singular.arguments import *
-from singular.endpoints.reporting import CreateReportResponse
+from singular_client.endpoints._bases import _Endpoint, ResponseDocList
+from singular_client.documents import *
+from singular_client.arguments import *
+from singular_client.endpoints.reporting import CreateReportResponse
 from typing import *
-from singular._utils import *
+from singular_client._utils import *
 
 
 class SkanEventsEndpoint(_Endpoint[ResponseDocList[NameDoc]]):
     endpoint = "v2.0/skan_events"
     data_path = ["value", "skan_events"]
     res_type = ResponseDocList[NameDoc]
```

### Comparing `singular_client-0.1.0/pyproject.toml` & `singular_client-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "singular-client"
-version = "0.1.0"
+version = "0.1.1"
 python_requires = ">=3.8"
 description = "Singular API client"
 authors = [
     {name = "Ryan Young", email = "dev@ryayoung.com"}
 ]
 readme = "README.md"
 license = "MIT"
```


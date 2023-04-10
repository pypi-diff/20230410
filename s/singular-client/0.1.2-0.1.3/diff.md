# Comparing `tmp/singular_client-0.1.2.tar.gz` & `tmp/singular_client-0.1.3.tar.gz`

## Comparing `singular_client-0.1.2.tar` & `singular_client-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/__init__.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/_utils.py
--rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/api.py
--rwxr-xr-x   0        0        0     6543 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/arguments.py
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/documents.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/processing.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/endpoints/__init__.py
--rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/endpoints/_bases.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/endpoints/governance.py
--rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/endpoints/links.py
--rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/endpoints/links_legacy.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/endpoints/monetization.py
--rw-r--r--   0        0        0     8387 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/endpoints/reporting.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/endpoints/skan.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 singular_client-0.1.2/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 singular_client-0.1.2/README.md
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 singular_client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 singular_client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 singular_client-0.1.3/.DS_Store
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 singular_client-0.1.3/.python-version
+-rw-r--r--   0        0        0    99036 2020-02-02 00:00:00.000000 singular_client-0.1.3/copilot magic documents.png
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/__init__.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/_bases.py
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/api.py
+-rwxr-xr-x   0        0        0     6543 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/arguments.py
+-rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/documents.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/utils.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/endpoints/__init__.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/endpoints/governance.py
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/endpoints/links.py
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/endpoints/links_legacy.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/endpoints/monetization.py
+-rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/endpoints/reporting.py
+-rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 singular_client-0.1.3/singular_client/endpoints/skan.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 singular_client-0.1.3/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 singular_client-0.1.3/README.md
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 singular_client-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 singular_client-0.1.3/PKG-INFO
```

### Comparing `singular_client-0.1.2/singular_client/api.py` & `singular_client-0.1.3/singular_client/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 import requests
 from typing import (
     Optional,
     Literal,
 )
+import os
 
 from singular_client.documents import *
-from singular_client._utils import *
 from singular_client.arguments import *
 
 
 class SingularAPI:
     """
     A simple class to store endpoint instances, and handle authentication and base url
     when requesting data from the Singular API.
@@ -20,18 +20,22 @@
     """
 
     base_url = "https://api.singular.net/api/"
     logs = True
 
     key: str
 
-    def __init__(self, key: str):
+    def __init__(self, key: Optional[str]=None):
+        if not key:
+            key = os.environ.get("SINGULAR_API_KEY")
+            assert key, "No API key provided"
         self.key = key
 
         from singular_client import endpoints
+
         # Reporting
         self.combined_report = endpoints.CombinedReportEndpoint(self)
         self.network_report = endpoints.NetworkReportEndpoint(self)
         self.tracker_report = endpoints.TrackerReportEndpoint(self)
         self.data_availability = endpoints.DataAvailabilityEndpoint(self)
         self.report_status = endpoints.ReportStatusEndpoint(self)
         self.filters = endpoints.FiltersEndpoint(self)
@@ -91,15 +95,15 @@
             key_in_headers = "v1" in url
 
         if key_in_headers:
             headers["Authorization"] = self.key
         else:
             params["api_key"] = self.key
 
-        print("new request:", f"{method.upper()} '{endpoint}'")
-        res = requests.request(method, url=url, params=params, headers=headers, data=data)
+        res = requests.request(
+            method, url=url, params=params, headers=headers, data=data
+        )
 
         assert (code := res.status_code) == 200, (code, res.text)
 
         # return UtilDict(res.json()).deep_uniform()
         return res.json()
-
```

### Comparing `singular_client-0.1.2/singular_client/arguments.py` & `singular_client-0.1.3/singular_client/arguments.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.2/singular_client/documents.py` & `singular_client-0.1.3/singular_client/documents.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,37 @@
+"""
+Data structures returned by Singular API.
+
+--------------------------------------------------------------------------------
+USED FOR TYPE CHECKING ONLY. DO NOT CREATE INSTANCES OF THESE CLASSES.
+--------------------------------------------------------------------------------
+"""
 from typing import TypedDict, List, Optional, Literal
 
+
 class NameDoc(TypedDict):
     display_name: str
     name: str
 
+
 class IDDoc(TypedDict):
     display_name: str
     id: str
 
-# ==============================================================================
+
+class NameDocValues(TypedDict):
+    name: str
+    display_name: str
+    values: List[NameDoc]
+
+
 # Reporting API
 # ==============================================================================
 
+
 class DataConnectorDoc(TypedDict):
     data_connector_id: str
     data_connector_source_name: str
     data_connector_username: str
     is_active_last_30_days: bool
     is_available: bool
     is_empty_data: str
@@ -29,28 +45,23 @@
     url_expires_in: int
     generated_url_time_in_utc: str
     url_expired_time_in_utc: str
     download_url: str
     report_id: str
 
 
-class FilterDoc(TypedDict):
-    name: str
-    display_name: str
-    values: List[NameDoc]
-
-
 class CohortMetricsDoc(TypedDict):
     metrics: List[NameDoc]
     periods: List[str]
 
-# ==============================================================================
+
 # [NEW] TRACKING LINKS API
 # ==============================================================================
 
+
 class CreateLinkDoc(TypedDict):
     tracking_link_id: str
     tracking_link_name: str
     click_tracking_link: str
     impression_tracking_link: str
     extra_info: List[str]
 
@@ -109,16 +120,15 @@
 
 
 class DomainDoc(TypedDict):
     subdomain: str
     dns_zone: str
 
 
-# ==============================================================================
-# Legacy Link Management API 
+# Legacy Link Management API
 # ==============================================================================
 
 
 class AppLegacyDoc(TypedDict):
     singular_app_id: int
     app_name: str
     app_longname: str
@@ -171,15 +181,14 @@
     tracking_link_id: int
     created_utc: str
     updated_utc: str
     # `status` not included in Create Link response
     status: str
 
 
-# ==============================================================================
 # Ad Monetization API
 # ==============================================================================
 
 
 class AdMonetizationDoc(TypedDict):
     ad_impressions: int
     end_date: str
```

### Comparing `singular_client-0.1.2/singular_client/endpoints/_bases.py` & `singular_client-0.1.3/singular_client/_bases.py`

 * *Files 14% similar despite different names*

```diff
@@ -76,16 +76,19 @@
             # `data` might contain dicts or lists. Ignore them.
             kwargs_key += tuple(
                 (k, v) for k, v in data.items() if not isinstance(v, (list, dict))
             )
 
         cache_found = self.cache.get(kwargs_key)
         if cache_found:
+            print("Using cached response from", f"{self.method.upper()} '{self.endpoint}'")
             return cache_found
 
+        print("New request:", f"{self.method.upper()} '{self.endpoint}'")
+
         res = self.api.request(
             endpoint=self.endpoint, method=self.method, params=kwargs, data=data
         )
         self.cache[kwargs_key] = res
         return res
 
     def request(self, **kwargs) -> ResType:
@@ -130,18 +133,17 @@
         Return a dict of the request schema.
         Keys: field names
         Values: field types
         """
         assert hasattr(
             self, "res_type"
         ), f"'{type(self).__name__}' must define `res_type`"
-        return RequestParams([
-            str(param)
-            for _, param in signature(self.request).parameters.items()
-        ])
+        return RequestParams(
+            [str(param) for _, param in signature(self.request).parameters.items()]
+        )
 
     @staticmethod
     def get_annotations(x) -> dict:
         """
         Safely get annotations from a class
         """
         try:
@@ -153,13 +155,11 @@
                 return {}
 
 
 class RequestParams(List[str]):
     def __repr__(self):
         return "\n".join(self)
 
+
 class ResponseSchema(Dict[str, type]):
     def __repr__(self):
-        return "\n".join([
-            f"{k}: {getattr(v, '__name__', v)}"
-            for k, v in self.items()
-        ])
+        return "\n".join([f"{k}: {getattr(v, '__name__', v)}" for k, v in self.items()])
```

### Comparing `singular_client-0.1.2/singular_client/endpoints/links.py` & `singular_client-0.1.3/singular_client/endpoints/links.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,46 @@
-from singular_client.endpoints._bases import _Endpoint, ResponseDocList
+from singular_client._bases import _Endpoint, ResponseDocList
 from singular_client.documents import *
 from singular_client.arguments import *
-from singular_client._utils import *
 from typing import *
+from singular_client.utils import _convert_list_arg
 
 
 class DomainsEndpoint(_Endpoint[ResponseDocList[DomainDoc]]):
     endpoint = "v1/singular_links/domains"
     data_path = ["available_domains"]
     res_type = ResponseDocList[DomainDoc]
 
 
 # ==============================================================================
 
+
 class AppsEndpoint(_Endpoint[ResponseDocList[AppDoc]]):
     endpoint = "v1/singular_links/apps"
     data_path = ["available_apps"]
     res_type = ResponseDocList[AppDoc]
 
+
 # ==============================================================================
 
+
 class AllPartnersEndpoint(_Endpoint[ResponseDocList[PartnerDoc]]):
     endpoint = "v1/singular_links/all_partners"
     data_path = ["partners"]
     res_type = ResponseDocList[PartnerDoc]
 
     def request(self, singular_partner_id: Optional[List[str]] = None):
         return super().request(
-            singular_partner_id=convert_list_arg(singular_partner_id)
+            singular_partner_id=_convert_list_arg(singular_partner_id)
         )
 
+
 # ==============================================================================
 
+
 class CreateLinkEndpoint(_Endpoint[CreateLinkDoc]):
     endpoint = "v1/singular_links/links"
     data_path = []
     res_type = CreateLinkDoc
     returns_collection = False
     method = "POST"
 
@@ -54,27 +59,37 @@
         click_deterministic_window: Optional[int] = None,
         click_probabilistic_window: Optional[int] = None,
         view_deterministic_window: Optional[int] = None,
         view_probabilistic_window: Optional[int] = None,
         click_reengagement_window: Optional[int] = None,
         enable_ctv: Optional[bool] = None,
     ):
-        assert android_redirection or ios_redirection, "Must provide at least one redirection"
+        assert (
+            android_redirection or ios_redirection
+        ), "Must provide at least one redirection"
 
         if click_reengagement_window:
-            assert enable_reengagement, "enable_reengagement must be True if click_reengagement_window is set"
+            assert (
+                enable_reengagement
+            ), "enable_reengagement must be True if click_reengagement_window is set"
 
         if click_deterministic_window:
-            assert 0 <= click_deterministic_window <= 30, "click_deterministic_window 0 to 30"
+            assert (
+                0 <= click_deterministic_window <= 30
+            ), "click_deterministic_window 0 to 30"
 
         if click_probabilistic_window:
-            assert 0 <= click_probabilistic_window <= 24, "click_probabilistic_window 0 to 24"
+            assert (
+                0 <= click_probabilistic_window <= 24
+            ), "click_probabilistic_window 0 to 24"
 
         if view_deterministic_window:
-            assert 0 <= view_deterministic_window <= 24, "view_deterministic_window 0 to 24"
+            assert (
+                0 <= view_deterministic_window <= 24
+            ), "view_deterministic_window 0 to 24"
 
         return super().request(
             data=dict(
                 app_id=app_id,
                 partner_id=partner_id,
                 tracking_link_name=tracking_link_name,
                 link_dns_zone=link_dns_zone,
@@ -89,16 +104,18 @@
                 view_deterministic_window=view_deterministic_window,
                 view_probabilistic_window=view_probabilistic_window,
                 click_reengagement_window=click_reengagement_window,
                 enable_ctv=enable_ctv,
             ),
         )
 
+
 # ==============================================================================
 
+
 class ViewLinksEndpoint(_Endpoint[ResponseDocList[LinkDoc]]):
     endpoint = "v1/singular_links/links"
     data_path = []
     res_type = ResponseDocList[LinkDoc]
 
     def request(
         self,
@@ -112,27 +129,25 @@
             link_type=link_type,
             partner_id=partner_id,
             app_id=app_id,
             app_site_id=app_site_id,
             tracking_link_id=tracking_link_id,
         )
 
+
 # ==============================================================================
 
 
 class ConfiguredPartnersEndpoint(_Endpoint[ResponseDocList[PartnerAppDoc]]):
     endpoint = "v1/singular_links/configured_partners"
     data_path = ["available_partners"]
     res_type = ResponseDocList[PartnerAppDoc]
 
     def request(
         self,
         app_site_id: Optional[List[str]] = None,
         partner_id: Optional[List[str]] = None,
     ):
         return super().request(
-            app_site_id=convert_list_arg(app_site_id),
-            partner_id=convert_list_arg(partner_id),
+            app_site_id=_convert_list_arg(app_site_id),
+            partner_id=_convert_list_arg(partner_id),
         )
-
-
-
```

### Comparing `singular_client-0.1.2/singular_client/endpoints/links_legacy.py` & `singular_client-0.1.3/singular_client/endpoints/links_legacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from singular_client.endpoints._bases import _Endpoint, ResponseDocList
+from singular_client._bases import _Endpoint, ResponseDocList
 from singular_client.documents import *
-from singular_client._utils import *
+from singular_client.utils import _convert_list_arg
 from typing import *
 
+
 class AppsLegacyEndpoint(_Endpoint[ResponseDocList[AppLegacyDoc]]):
     endpoint = "v1/links/discover_apps"
     data_path = ["available_apps"]
     res_type = ResponseDocList[AppLegacyDoc]
 
 
 class AvailablePartnersLegacyEndpoint(_Endpoint[ResponseDocList[PartnerLegacyDoc]]):
@@ -69,27 +70,37 @@
         ios_deferred_deeplink_enabled: Optional[bool] = None,
         android_destination_fallback_url: Optional[str] = None,
         android_destination_deeplink_url: Optional[str] = None,
         android_deferred_deeplink_enabled: Optional[bool] = None,
         reengagement_enabled: Optional[bool] = None,
         other_destination_fallback_url: Optional[str] = None,
     ):
-        assert ios_singular_app_id or android_singular_app_id, "Must provide at least one app id"
+        assert (
+            ios_singular_app_id or android_singular_app_id
+        ), "Must provide at least one app id"
 
         if ios_singular_app_id:
-            assert ios_destination_fallback_url, "Must provide ios_destination_fallback_url"
+            assert (
+                ios_destination_fallback_url
+            ), "Must provide ios_destination_fallback_url"
 
         if android_singular_app_id:
-            assert android_destination_fallback_url, "Must provide android_destination_fallback_url"
+            assert (
+                android_destination_fallback_url
+            ), "Must provide android_destination_fallback_url"
 
         if ios_deferred_deeplink_enabled:
-            assert ios_destination_deeplink_url, "Must provide ios_destination_deeplink_url"
+            assert (
+                ios_destination_deeplink_url
+            ), "Must provide ios_destination_deeplink_url"
 
         if android_deferred_deeplink_enabled:
-            assert android_destination_deeplink_url, "Must provide android_destination_deeplink_url"
+            assert (
+                android_destination_deeplink_url
+            ), "Must provide android_destination_deeplink_url"
 
         return super().request(
             data=dict(
                 ios_singular_app_id=ios_singular_app_id,
                 android_singular_app_id=android_singular_app_id,
                 custom_source_name=custom_source_name,
                 tracker_campaign_name=tracker_campaign_name,
@@ -115,17 +126,17 @@
         self,
         singular_app_ids: Optional[List[str]] = None,
         singular_partner_ids: Optional[List[str]] = None,
         tracking_link_ids: Optional[List[str]] = None,
         include_archived_links: bool = False,
     ):
         return super().request(
-            singular_app_ids=convert_list_arg(singular_app_ids),
-            singular_partner_ids=convert_list_arg(singular_partner_ids),
-            tracking_link_ids=convert_list_arg(tracking_link_ids),
+            singular_app_ids=_convert_list_arg(singular_app_ids),
+            singular_partner_ids=_convert_list_arg(singular_partner_ids),
+            tracking_link_ids=_convert_list_arg(tracking_link_ids),
             include_archived_links=include_archived_links,
         )
 
 
 class ViewCustomLinksLegacyEndpoint(_Endpoint[ResponseDocList[CustomLinkLegacyDoc]]):
     endpoint = "v1/links/view_custom"
     data_path = ["results"]
@@ -135,12 +146,12 @@
         self,
         singular_app_ids: Optional[List[str]] = None,
         custom_source_name: Optional[str] = None,
         tracking_link_ids: Optional[List[str]] = None,
         include_archived_links: bool = False,
     ):
         return super().request(
-            singular_app_ids=convert_list_arg(singular_app_ids),
+            singular_app_ids=_convert_list_arg(singular_app_ids),
             custom_source_name=custom_source_name,
-            tracking_link_ids=convert_list_arg(tracking_link_ids),
+            tracking_link_ids=_convert_list_arg(tracking_link_ids),
             include_archived_links=include_archived_links,
         )
```

### Comparing `singular_client-0.1.2/singular_client/endpoints/monetization.py` & `singular_client-0.1.3/singular_client/endpoints/monetization.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from singular_client.endpoints._bases import _Endpoint, ResponseDocList
+from singular_client._bases import _Endpoint, ResponseDocList
 from singular_client.documents import *
 from singular_client.arguments import *
 from typing import *
-from singular_client._utils import *
+from singular_client.utils import _convert_list_arg
+
 
 class AdMonetizationEndpoint(_Endpoint[ResponseDocList[AdMonetizationDoc]]):
     endpoint = "v2.0/admonetization/reporting"
     data_path = ["value", "results"]
     res_type = ResponseDocList[AdMonetizationDoc]
 
     def request(
@@ -22,17 +23,15 @@
         format: FileFormat = "json",
         country_code_format: CountryCodeFormat = "iso3",
     ):
         return super().request(
             start_date=start_date,
             end_date=end_date or start_date,
             time_breakdown=time_breakdown,
-            dimensions=convert_list_arg(dimensions, AD_MON_DIMENSIONS),
-            metrics=convert_list_arg(metrics, AD_MON_METRICS),
-            app=convert_list_arg(app),
-            source=convert_list_arg(source),
+            dimensions=_convert_list_arg(dimensions, AD_MON_DIMENSIONS),
+            metrics=_convert_list_arg(metrics, AD_MON_METRICS),
+            app=_convert_list_arg(app),
+            source=_convert_list_arg(source),
             filters=filters,
             format=format,
             country_code_format=country_code_format,
         )
-
-
```

### Comparing `singular_client-0.1.2/singular_client/endpoints/reporting.py` & `singular_client-0.1.3/singular_client/endpoints/reporting.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from singular_client.endpoints._bases import _Endpoint, ResponseDocList
+from singular_client._bases import _Endpoint, ResponseDocList
 from singular_client.documents import *
 from singular_client.arguments import *
-from singular_client._utils import convert_list_arg
-import pandas as pd
+from singular_client.utils import _convert_list_arg
 import json
 import time
 import requests
 import io
 from typing import *
 
 if TYPE_CHECKING:
@@ -14,17 +13,18 @@
     import pandas as pd
 
 
 class ReportStatusResponse:
     cached_download: Optional[Union[requests.Response, "pd.DataFrame"]]
     status: ReportStatusDoc
     failed = property(lambda x: x.status["status"] == "FAILED")
-    done = property(lambda x: x.status["status"] == "FAILED")
+    done = property(lambda x: x.status["status"] == "DONE")
     queued = property(lambda x: x.status["status"] == "QUEUED")
     started = property(lambda x: x.status["status"] == "STARTED")
+    url = property(lambda x: x.status["download_url"])
 
     def __init__(self, doc: dict):
         self.status = cast(ReportStatusDoc, doc)
         self.cached_download = None
 
     def __bool__(self) -> bool:
         return self.done
@@ -81,18 +81,18 @@
                 "Please wait at least 10 seconds between report status requests, per report"
             )
             return None
         self.request_times[report_id] = time.time()
         return super().request(report_id=report_id)
 
 
-class FiltersEndpoint(_Endpoint[ResponseDocList[FilterDoc]]):
+class FiltersEndpoint(_Endpoint[ResponseDocList[NameDocValues]]):
     endpoint = "v2.0/reporting/filters"
     data_path = ["value", "dimensions"]
-    res_type = ResponseDocList[FilterDoc]
+    res_type = ResponseDocList[NameDocValues]
 
 
 class CohortMetricsEndpoint(_Endpoint[CohortMetricsDoc]):
     endpoint = "cohort_metrics"
     data_path = ["value"]
     res_type = CohortMetricsDoc
     returns_collection = False
@@ -193,29 +193,29 @@
         source: Optional[List[str]] = None,
         filters: Optional[List[dict]] = None,
         format: FileFormat = "csv",
         country_code_format: CountryCodeFormat = "iso3",
         display_alignment: bool = False,
         display_unenriched: bool = False,
     ):
-        dimensions_str = convert_list_arg(dimensions, self.available_dimensions)
+        dimensions_str = _convert_list_arg(dimensions, self.available_dimensions)
         if custom_dimensions:
-            dimensions_str += convert_list_arg(custom_dimensions)
+            dimensions_str += _convert_list_arg(custom_dimensions)
         report_id = super().request(
             data=dict(
                 start_date=start_date,
                 end_date=end_date or start_date,
                 time_breakdown=time_breakdown,
                 dimensions=dimensions_str,
-                metrics=convert_list_arg(metrics, self.available_metrics),
-                custom_dimensions=convert_list_arg(custom_dimensions),
-                cohort_metrics=convert_list_arg(cohort_metrics),
-                cohort_periods=convert_list_arg(cohort_periods),
-                app=convert_list_arg(app),
-                source=convert_list_arg(source),
+                metrics=_convert_list_arg(metrics, self.available_metrics),
+                custom_dimensions=_convert_list_arg(custom_dimensions),
+                cohort_metrics=_convert_list_arg(cohort_metrics),
+                cohort_periods=_convert_list_arg(cohort_periods),
+                app=_convert_list_arg(app),
+                source=_convert_list_arg(source),
                 filters=filters,
                 format=format,
                 country_code_format=country_code_format,
                 display_alignment=display_alignment,
                 display_unenriched=display_unenriched,
             ),
         )
```

### Comparing `singular_client-0.1.2/singular_client/endpoints/skan.py` & `singular_client-0.1.3/singular_client/endpoints/skan.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-from singular_client.endpoints._bases import _Endpoint, ResponseDocList
+from singular_client._bases import _Endpoint, ResponseDocList
 from singular_client.documents import *
 from singular_client.arguments import *
 from singular_client.endpoints.reporting import CreateReportResponse
 from typing import *
-from singular_client._utils import *
+from singular_client.utils import _convert_list_arg
 
 
 class SkanEventsEndpoint(_Endpoint[ResponseDocList[NameDoc]]):
     endpoint = "v2.0/skan_events"
     data_path = ["value", "skan_events"]
     res_type = ResponseDocList[NameDoc]
 
 
-
 class SkanRawReportEndpoint(_Endpoint[CreateReportResponse]):
     endpoint = "v2.0/create_async_skadnetwork_raw_report"
     data_path = ["value", "report_id"]
+    available_dimensions = SKAN_RAW_DIMENSIONS
+    available_metrics = SKAN_RAW_METRICS
     res_type = CreateReportResponse
     returns_collection = False
     method = "POST"
 
     def request(
         self,
         start_date: str,
@@ -36,31 +37,33 @@
     ):
         report_id = super().request(
             data=dict(
                 start_date=start_date,
                 end_date=end_date or start_date,
                 time_breakdown=time_breakdown,
                 skadnetwork_date_type=skadnetwork_date_type,
-                dimensions=convert_list_arg(dimensions, SKAN_RAW_DIMENSIONS),
-                metrics=convert_list_arg(metrics, SKAN_RAW_METRICS),
-                app=convert_list_arg(app),
-                source=convert_list_arg(source),
+                dimensions=_convert_list_arg(dimensions, self.available_dimensions),
+                metrics=_convert_list_arg(metrics, self.available_metrics),
+                app=_convert_list_arg(app),
+                source=_convert_list_arg(source),
                 filters=filters,
                 format=format,
                 country_code_format=country_code_format,
             ),
         )
         report_id.api = self.api
         return report_id
 
 
 class SkanReportEndpoint(_Endpoint[CreateReportResponse]):
     endpoint = "v2.0/create_async_skadnetwork_report"
     data_path = ["value", "report_id"]
     res_type = CreateReportResponse
+    available_dimensions = SKAN_DIMENSIONS
+    available_metrics = SKAN_METRICS
     returns_collection = False
     method = "POST"
 
     def request(
         self,
         start_date: str,
         time_breakdown: TimeBreakdown = "all",
@@ -73,15 +76,15 @@
     ):
         report_id = super().request(
             data=dict(
                 start_date=start_date,
                 end_date=end_date or start_date,
                 time_breakdown=time_breakdown,
                 skadnetwork_date_type=skadnetwork_date_type,
-                dimensions=convert_list_arg(dimensions, SKAN_DIMENSIONS),
-                metrics=convert_list_arg(metrics, SKAN_METRICS),
-                skan_events=convert_list_arg(skan_events),
+                dimensions=_convert_list_arg(dimensions, self.available_dimensions),
+                metrics=_convert_list_arg(metrics, self.available_metrics),
+                skan_events=_convert_list_arg(skan_events),
                 format=format,
             ),
         )
         report_id.api = self.api
         return report_id
```

### Comparing `singular_client-0.1.2/pyproject.toml` & `singular_client-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "singular-client"
-version = "0.1.2"
+version = "0.1.3"
 python_requires = ">=3.8"
 description = "Singular API client"
 authors = [
     {name = "Ryan Young", email = "dev@ryayoung.com"}
 ]
 readme = "README.md"
 license = "MIT"
-homepage = "https://github.com/ryayoung/singular"
-repository = "https://github.com/ryayoung/singular"
-documentation = "https://singular.readthedocs.io"
+homepage = "https://github.com/ryayoung/singular-client"
+repository = "https://github.com/ryayoung/singular-client"
+documentation = "https://singular-client.readthedocs.io"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
+    "Topic :: Software Development :: Libraries",
     "Programming Language :: Python :: 3.11",
-    "Topic :: Software Development :: Libraries"
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.8",
 ]
 dependencies = [
     'requests',
 ]
```


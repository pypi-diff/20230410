# Comparing `tmp/dynamics_client-0.5.7.tar.gz` & `tmp/dynamics_client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamics_client-0.5.7.tar", max compression
+gzip compressed data, was "dynamics_client-0.6.0.tar", max compression
```

## Comparing `dynamics_client-0.5.7.tar` & `dynamics_client-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-04-06 18:35:53.482018 dynamics_client-0.5.7/LICENSE
--rw-r--r--   0        0        0     4799 2023-04-06 18:35:53.486019 dynamics_client-0.5.7/README.md
--rw-r--r--   0        0        0      192 2023-04-06 18:35:53.486019 dynamics_client-0.5.7/dynamics/__init__.py
--rw-r--r--   0        0        0     9531 2023-04-06 18:35:53.486019 dynamics_client-0.5.7/dynamics/api_actions.py
--rw-r--r--   0        0        0     7334 2023-04-06 18:35:53.486019 dynamics_client-0.5.7/dynamics/api_functions.py
--rw-r--r--   0        0        0     2027 2023-04-06 18:35:53.486019 dynamics_client-0.5.7/dynamics/apply_functions.py
--rw-r--r--   0        0        0    35940 2023-04-06 18:35:53.486019 dynamics_client-0.5.7/dynamics/client.py
--rw-r--r--   0        0        0     4207 2023-04-06 18:35:53.486019 dynamics_client-0.5.7/dynamics/enums.py
--rw-r--r--   0        0        0     4219 2023-04-06 18:35:53.486019 dynamics_client-0.5.7/dynamics/exceptions.py
--rw-r--r--   0        0        0    33719 2023-04-06 18:35:53.486019 dynamics_client-0.5.7/dynamics/fetchxml.py
--rw-r--r--   0        0        0     1529 2023-04-06 18:35:53.486019 dynamics_client-0.5.7/dynamics/normalizers.py
--rw-r--r--   0        0        0    36552 2023-04-06 18:35:53.486019 dynamics_client-0.5.7/dynamics/query_functions.py
--rw-r--r--   0        0        0     1910 2023-04-06 18:35:53.486019 dynamics_client-0.5.7/dynamics/status.py
--rw-r--r--   0        0        0    10051 2023-04-06 18:35:53.486019 dynamics_client-0.5.7/dynamics/test.py
--rw-r--r--   0        0        0     5137 2023-04-06 18:35:53.486019 dynamics_client-0.5.7/dynamics/typing.py
--rw-r--r--   0        0        0     8654 2023-04-06 18:35:53.486019 dynamics_client-0.5.7/dynamics/utils.py
--rw-r--r--   0        0        0     3043 2023-04-06 18:35:53.486019 dynamics_client-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     5975 1970-01-01 00:00:00.000000 dynamics_client-0.5.7/setup.py
--rw-r--r--   0        0        0     6495 1970-01-01 00:00:00.000000 dynamics_client-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-10 17:30:23.459368 dynamics_client-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4799 2023-04-10 17:30:23.459368 dynamics_client-0.6.0/README.md
+-rw-r--r--   0        0        0      192 2023-04-10 17:30:23.459368 dynamics_client-0.6.0/dynamics/__init__.py
+-rw-r--r--   0        0        0     9458 2023-04-10 17:30:23.459368 dynamics_client-0.6.0/dynamics/api_actions.py
+-rw-r--r--   0        0        0     7284 2023-04-10 17:30:23.459368 dynamics_client-0.6.0/dynamics/api_functions.py
+-rw-r--r--   0        0        0     1989 2023-04-10 17:30:23.459368 dynamics_client-0.6.0/dynamics/apply_functions.py
+-rw-r--r--   0        0        0    34661 2023-04-10 17:30:23.459368 dynamics_client-0.6.0/dynamics/client.py
+-rw-r--r--   0        0        0     4199 2023-04-10 17:30:23.459368 dynamics_client-0.6.0/dynamics/enums.py
+-rw-r--r--   0        0        0     4194 2023-04-10 17:30:23.459368 dynamics_client-0.6.0/dynamics/exceptions.py
+-rw-r--r--   0        0        0    33474 2023-04-10 17:30:23.463368 dynamics_client-0.6.0/dynamics/fetchxml.py
+-rw-r--r--   0        0        0     1479 2023-04-10 17:30:23.463368 dynamics_client-0.6.0/dynamics/normalizers.py
+-rw-r--r--   0        0        0        0 2023-04-10 17:30:23.463368 dynamics_client-0.6.0/dynamics/py.typed
+-rw-r--r--   0        0        0    36471 2023-04-10 17:30:23.463368 dynamics_client-0.6.0/dynamics/query_functions.py
+-rw-r--r--   0        0        0     1910 2023-04-10 17:30:23.463368 dynamics_client-0.6.0/dynamics/status.py
+-rw-r--r--   0        0        0     9650 2023-04-10 17:30:23.463368 dynamics_client-0.6.0/dynamics/test.py
+-rw-r--r--   0        0        0     6060 2023-04-10 17:30:23.463368 dynamics_client-0.6.0/dynamics/typing.py
+-rw-r--r--   0        0        0     8532 2023-04-10 17:30:23.463368 dynamics_client-0.6.0/dynamics/utils.py
+-rw-r--r--   0        0        0     3076 2023-04-10 17:30:23.463368 dynamics_client-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6484 1970-01-01 00:00:00.000000 dynamics_client-0.6.0/PKG-INFO
```

### Comparing `dynamics_client-0.5.7/LICENSE` & `dynamics_client-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamics_client-0.5.7/README.md` & `dynamics_client-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dynamics_client-0.5.7/dynamics/api_actions.py` & `dynamics_client-0.6.0/dynamics/api_actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 https://docs.microsoft.com/en-us/powerapps/developer/data-platform/webapi/use-web-api-actions
 """
 
 from .enums import QuoteState
 from .typing import TYPE_CHECKING, Any, Dict, List, Literal
 
 if TYPE_CHECKING:
-    from .client import DynamicsClient  # pylint: disable=R0401
+    from .client import DynamicsClient
 
 
 __all__ = ["Actions"]
 
 
 class Actions:
     """Predefined Dynamics API actions."""
 
     def __get__(self, instance, owner):
         if instance is None:
             raise RuntimeError("Actions can only be used on DynamicsClient instances.")
 
-        self.client: "DynamicsClient" = instance  # pylint: disable=W0201
+        self.client: "DynamicsClient" = instance
         return self
 
-    def send_email_from_template(  # pylint: disable=R0913
+    def send_email_from_template(
         self,
         template_id: str,
         context_table: str,
         context_row_id: str,
         sender_id: str,
         to_recipient_ids: List[str],
         cc_recipient_ids: List[str] = None,
@@ -39,15 +39,15 @@
     ):
         """Construct POST data to use in SendEmailFromTemplate action.
 
         https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/sendemailfromtemplate
 
         :param template_id: Dynamics template GUID to use.
         :param context_table: What table to use in the context of the email.
-        :param context_row_id: What row to select from the context table. This row's data can be used in
+        :param context_row_id: Which row to select from the context table. This row's data can be used in
                                dynamically in the body of the email template.
         :param sender_id: Dynamics systemuser GUID that sends the email. Must have 'send-as' privilege.
         :param to_recipient_ids: List of Dynamics contact GUIDS to add as to recipients.
         :param cc_recipient_ids: List of Dynamics contact GUIDS to add as cc recipients.
         :param bcc_recipient_ids: List of Dynamics contact GUIDS to add as bcc recipients.
         :return: Tuple of the action name and POST data to send.
         """
@@ -107,15 +107,15 @@
         return self.client.post(
             data=data,
             simplify_errors=kwargs.pop("simplify_errors", False),
             raise_separately=kwargs.pop("raise_separately", []),
         )
 
     def activate_quote(self, quote_id: str, select: List[str] = None, **kwargs) -> Dict[str, Any]:
-        """Change the state of the quote to active so it can be converted to a salesorder.
+        """Change the state of the quote to active, so it can be converted to a salesorder.
 
         :param quote_id: Quote to activate.
         :param select: Attributes to retrieve from the quote.
         :return: Activated quote.
         """
 
         self.client.reset_query()
```

### Comparing `dynamics_client-0.5.7/dynamics/api_functions.py` & `dynamics_client-0.6.0/dynamics/api_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/functions
 """
 
 from .enums import EntityFilter, TargetFieldType
 from .typing import TYPE_CHECKING, Any, Dict, List
 
 if TYPE_CHECKING:
-    from .client import DynamicsClient  # pylint: disable=R0401
+    from .client import DynamicsClient
 
 
 __all__ = ["Functions"]
 
 
 class Functions:
     """Predefined Dynamics API functions."""
 
     def __get__(self, instance, owner):
         if instance is None:
             raise RuntimeError("Functions can only be used on DynamicsClient instances.")
 
-        self.client: "DynamicsClient" = instance  # pylint: disable=W0201
+        self.client: "DynamicsClient" = instance
         return self
 
     def expand_calendar(self, start: str, end: str, **kwargs) -> List[Dict[str, Any]]:
         """Converts the calendar rules to an array of available time blocks for the specified period."""
 
         self.client.reset_query()
         self.client.action = f"ExpandCalendar(Start='{start}',End='{end}')"
```

### Comparing `dynamics_client-0.5.7/dynamics/apply_functions.py` & `dynamics_client-0.6.0/dynamics/apply_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=C0103
 """
 Aggregate and grouping results:
 https://docs.microsoft.com/en-us/powerapps/developer/data-platform/webapi/query-data-web-api#aggregate-and-grouping-results
 
 FetchXML aggregation documentation:
 https://docs.microsoft.com/en-us/powerapps/developer/data-platform/use-fetchxml-aggregation
 """
@@ -22,15 +21,15 @@
         :param columns: Columns to group by.
         :param aggregate: Aggregate grouped results by this function. Use `apl.aggregate(...)` to construct this.
         """
         aggregate = f",{aggregate}" if aggregate is not None else ""
         return f"groupby(({','.join(columns)}){aggregate})"
 
     @staticmethod
-    def aggregate(*, col_: str, with_: Literal["average", "sum", "min", "max", "count"], as_: str) -> str:  # noqa: F821
+    def aggregate(*, col_: str, with_: Literal["average", "sum", "min", "max", "count"], as_: str) -> str:
         """Aggregate column with some aggregation function, and alias the result under some name.
 
         :param col_: Column to aggregate over.
         :param with_: How to aggregate the columns.
         :param as_: Aggregate result alias.
         """
         return f"aggregate({col_} with {with_} as {as_})"
```

### Comparing `dynamics_client-0.5.7/dynamics/client.py` & `dynamics_client-0.6.0/dynamics/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-# pylint: disable=R0913
 """
 Dynamics Api Client. API Reference Docs:
 https://docs.microsoft.com/en-us/powerapps/developer/data-platform/webapi/query-data-web-api
 """
+
 import asyncio
-import json
 import logging
 import os
 from concurrent.futures import ThreadPoolExecutor
 from types import TracebackType
-from typing import Union
 from urllib.parse import quote
 
-from oauthlib.oauth2 import BackendApplicationClient, OAuth2Token
-from requests import HTTPError, JSONDecodeError  # noqa
-from requests_oauthlib import OAuth2Session
+from authlib.integrations.httpx_client import OAuth2Client
+from authlib.oauth2.rfc6749.wrappers import OAuth2Token
 
 from . import status
 from .api_actions import Actions
 from .api_functions import Functions
 from .exceptions import (
     APILimitsExceeded,
     AuthenticationFailed,
@@ -32,38 +29,40 @@
     PermissionDenied,
     WebAPIUnavailable,
 )
 from .typing import (
     Any,
     Callable,
     Dict,
+    DynamicsResponse,
     ExpandDict,
     ExpandKeys,
     ExpandValues,
     FilterType,
     List,
     MethodType,
     Optional,
     OrderbyType,
     P,
     T,
     Type,
     TypeVar,
+    Union,
 )
 from .utils import Singletons, error_simplification_available, sentinel, to_coroutine
 
 __all__ = ["DynamicsClient"]
 
 
 logger = logging.getLogger(__name__)
 EXC = TypeVar("EXC", bound=BaseException)
 DClient = TypeVar("DClient", bound="DynamicsClient")
 
 
-class DynamicsClient:  # pylint: disable=R0904,R0902
+class DynamicsClient:
     """Dynamics client for making queries from a Microsoft Dynamics 365 database."""
 
     request_counter: int = 0
     cache_key: str = "dynamics-client-token"
     simplified_error_message: str = "There was a problem communicating with the server."
 
     actions = Actions()
@@ -100,33 +99,26 @@
         :param token_url: URL to the Dynamics/Azure token endpoint.
                           Format: https://[Dynamics Token URI]/path/to/token
         :param client_id: Dynamics User ID.
         :param client_secret: Dynamics User Secret that proves its identity when password is required.
         :param scope: Url, or list of urls, that define(s) the database records that the API connection has access to.
                       Each most likely in this format: https://[Organization URI]/.default
         :param resource: Url that defines the database records that the API connection has access to.
-                      Most likely in this format: https://[Organization URI]/
+                         Most likely in this format: https://[Organization URI]/
         """
 
         if not scope and not resource:
             raise ValueError(
                 "To instantiate a DynamicsClient, you must provide at least one of either the"
                 " scope or resource parameters."
             )
 
         self._api_url = api_url.rstrip("/") + "/"
-        self._session = OAuth2Session(client=BackendApplicationClient(client_id=client_id))
-        token = self.get_token()
-        if token is None:  # pragma: no cover
-            token = self._session.fetch_token(
-                token_url=token_url, client_secret=client_secret, scope=scope, resource=resource
-            )
-            self.set_token(token)
-        else:
-            self._session.token = token
+        self._oauth_client = OAuth2Client(client_id, client_secret, scope=scope)
+        self._init_client(token_url, scope, resource)
 
         self._select: List[str] = []
         self._expand: ExpandDict = {}
         self._filter: FilterType = []
         self._orderby: OrderbyType = {}
         self._top: int = 0
         self._count: bool = False
@@ -138,23 +130,36 @@
         self._pre_expand = ""
         self._apply = ""
         self._fetch_xml = ""
 
         self._headers: Dict[str, str] = {}
         self._pagesize: int = 5000
 
+    def _init_client(self, token_url: str, scope: Optional[Union[str, List[str]]], resource: Optional[str]) -> None:
+        token = self.get_token()
+        if token is None:  # pragma: no cover
+            token = self._oauth_client.fetch_token(
+                url=token_url,
+                grant_type="client_credentials",
+                scope=scope,
+                resource=resource,
+            )
+            self.set_token(token)
+        else:
+            self._oauth_client.token = token
+
     def __getitem__(self, key):
         return self.headers[key]
 
     def __setitem__(self, key, value):
         self.headers[key] = value
 
     async def __aenter__(self: DClient) -> DClient:
         if hasattr(asyncio, "TaskGroup"):  # pragma: no cover; python >=3.11 only
-            self.__tg = asyncio.TaskGroup()  # pylint: disable=W0201
+            self.__tg = asyncio.TaskGroup()
             await self.__tg.__aenter__()
 
         return self
 
     async def __aexit__(self, exc_type: Optional[Type[EXC]], exc: EXC, traceback: TracebackType) -> None:
         if hasattr(asyncio, "TaskGroup"):  # pragma: no cover; python >=3.11 only
             try:
@@ -348,106 +353,96 @@
             status_code,
             error_message,
             error_code,
         )
         error = self.error_dict.get(status_code, DynamicsException)
         return error(error_message)
 
+    def _handle_pagination(self, entities: List[Dict[str, Any]], not_found_ok: bool) -> None:
+        """Fetch more data with get requests when needed."""
+        for i, row in enumerate(entities):
+            for column_key in list(row.keys()):
+                if "@odata.nextLink" in column_key:
+                    # Sometimes @odata.next links will appear even if all items were fetched.
+                    # We know how many items should be fetched from odata.maxpagesize header,
+                    # therefore, if the @odata.next link appears before that, we can ignore it.
+                    #
+                    key = column_key[:-15]
+                    if len(row[key]) < self.pagesize:
+                        row.pop(column_key)
+                        continue
+
+                    # When fetching the next page of results, it can include the last
+                    # page of data as well, so we filter those out. Although, This doesn't seem
+                    # to be the intended way this should work, based on this:
+                    #
+                    # https://docs.microsoft.com/en-us/powerapps/developer/data-platform/webapi/query-data-web-api#retrieve-related-tables-by-expanding-navigation-properties
+                    #
+                    extra = self.get(not_found_ok=not_found_ok, query=row.pop(column_key))
+                    id_tags = [value["@odata.etag"] for value in row[key]]
+                    extra = [value for value in extra if value["@odata.etag"] not in id_tags]
+
+                    entities[i][key] += extra
+
     @error_simplification_available
-    def get(self, *, not_found_ok: bool = False, query: Optional[str] = None) -> List[Dict[str, Any]]:  # noqa: C901
+    def get(self, *, not_found_ok: bool = False, query: Optional[str] = None) -> List[Dict[str, Any]]:
         """Make a request to the Dataverse API with currently added query options.
 
         Please also read the decorator's documentation!
 
         :param not_found_ok: No entities returned should not raise NotFound error, but return empty list instead.
         :param query: Use this url instead of building it from current query parameters.
         """
 
         self.request_counter += 1
 
         if query is None:
             query = self.current_query
 
-        response = self._session.get(
+        response = self._oauth_client.get(
             url=query,
             headers={**self.default_headers("get"), **self.headers},
         )
 
         try:
-            response.raise_for_status()
-        except HTTPError as error:
+            data: DynamicsResponse = response.json()
+        except Exception as error:
             raise self.handled_error(
-                status_code=error.response.status_code,
-                error_message=f"{str(error)}. Response: {error.response.text}",
-                error_code="http_error",
-                method="get",
-            ) from error
-
-        try:
-            data = response.json()
-        except JSONDecodeError as error:
-            raise self.handled_error(
-                status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
+                status_code=response.status_code,
                 error_message=f"{str(error)}. Response: {response.text}",
                 error_code="invalid_json",
                 method="get",
             ) from error
 
-        # Always returns a list, even if only one row is selected
-        entities = data.get("value", [data])
-        errors = data.get("error", {})
-
-        if errors:
+        if "error" in data:
             raise self.handled_error(
                 status_code=response.status_code,
-                error_message=errors.get("message"),
-                error_code=errors.get("code"),
+                error_message=data["error"]["message"],
+                error_code=data["error"]["code"],
                 method="get",
             )
 
+        # Always returns a list, even if only one row is selected
+        entities: List[Dict[str, Any]] = data.get("value", [data])
         if not entities:
             if not_found_ok:
                 return []
 
             raise self.handled_error(
                 status_code=status.HTTP_404_NOT_FOUND,
                 error_message="No records matching the given criteria.",
                 error_code="not_found",
                 method="get",
             )
 
-        # Fetch more data if needed
-        for i, row in enumerate(entities):
-            for column_key in list(row.keys()):
-                if "@odata.nextLink" in column_key:
+        self._handle_pagination(entities, not_found_ok)
 
-                    # Sometimes @odata.next links will appear even if all items were fetched.
-                    # We know how many items should be fetched from odata.maxpagesize header,
-                    # therefore, if the @odata.next link appears before that, we can ignore it.
-                    #
-                    key = column_key[:-15]
-                    if len(row[key]) < self.pagesize:
-                        row.pop(column_key)
-                        continue
-
-                    # When fetching the next page of results, it can include the last
-                    # page of data as well, so we filter those out. Although, This doesn't seem
-                    # to be the intended way this should work, based on this:
-                    #
-                    # https://docs.microsoft.com/en-us/powerapps/developer/data-platform/webapi/query-data-web-api#retrieve-related-tables-by-expanding-navigation-properties
-                    #
-                    extra = self.get(not_found_ok=not_found_ok, query=row.pop(column_key))
-                    id_tags = [value["@odata.etag"] for value in row[key]]
-                    extra = [value for value in extra if value["@odata.etag"] not in id_tags]
-
-                    entities[i][key] += extra
-
-        count = data.get("@odata.count", "")
-        if count:
-            entities.insert(0, count)
+        count: Optional[int] = data.get("@odata.count")
+        if count is not None:
+            entities.insert(0, count)  # type: ignore
 
         return entities
 
     @error_simplification_available
     def post(self, data: Dict[str, Any], *, query: Optional[str] = None) -> Dict[str, Any]:
         """Create new row in a table. Must have 'table' attribute set.
         Use expand and select to reduce returned data.
@@ -459,49 +454,38 @@
         """
 
         self.request_counter += 1
 
         if query is None:
             query = self.current_query
 
-        response = self._session.post(
+        response = self._oauth_client.post(
             url=query,
-            data=json.dumps(data).encode(),
+            data=data,
             headers={**self.default_headers("post"), **self.headers},
         )
 
         if response.status_code == status.HTTP_204_NO_CONTENT:
             return {}
 
         try:
-            response.raise_for_status()
-        except HTTPError as error:
-            raise self.handled_error(
-                status_code=error.response.status_code,
-                error_message=f"{str(error)}. Response: {error.response.text}",
-                error_code="http_error",
-                method="post",
-            ) from error
-
-        try:
-            data = response.json()
-        except JSONDecodeError as error:
+            data: DynamicsResponse = response.json()
+        except Exception as error:
             raise self.handled_error(
-                status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
+                status_code=response.status_code,
                 error_message=f"{str(error)}. Response: {response.text}",
                 error_code="invalid_json",
-                method="get",
+                method="post",
             ) from error
 
-        errors = data.get("error")
-        if errors:
+        if "error" in data:
             raise self.handled_error(
                 status_code=response.status_code,
-                error_message=errors.get("message"),
-                error_code=errors.get("code"),
+                error_message=data["error"]["message"],
+                error_code=data["error"]["code"],
                 method="post",
             )
 
         return data
 
     @error_simplification_available
     def patch(self, data: Dict[str, Any], *, query: Optional[str] = None) -> Dict[str, Any]:
@@ -515,49 +499,38 @@
         """
 
         self.request_counter += 1
 
         if query is None:
             query = self.current_query
 
-        response = self._session.patch(
+        response = self._oauth_client.patch(
             url=query,
-            data=json.dumps(data).encode(),
+            data=data,
             headers={**self.default_headers("patch"), **self.headers},
         )
 
         if response.status_code == status.HTTP_204_NO_CONTENT:
             return {}
 
         try:
-            response.raise_for_status()
-        except HTTPError as error:
-            raise self.handled_error(
-                status_code=error.response.status_code,
-                error_message=f"{str(error)}. Response: {error.response.text}",
-                error_code="http_error",
-                method="patch",
-            ) from error
-
-        try:
-            data = response.json()
-        except JSONDecodeError as error:
+            data: DynamicsResponse = response.json()
+        except Exception as error:
             raise self.handled_error(
-                status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
+                status_code=response.status_code,
                 error_message=f"{str(error)}. Response: {response.text}",
                 error_code="invalid_json",
-                method="get",
+                method="patch",
             ) from error
 
-        errors = data.get("error")
-        if errors:
+        if "error" in data:
             raise self.handled_error(
                 status_code=response.status_code,
-                error_message=errors.get("message"),
-                error_code=errors.get("code"),
+                error_message=data["error"]["message"],
+                error_code=data["error"]["code"],
                 method="patch",
             )
 
         return data
 
     @error_simplification_available
     def delete(self, *, query: Optional[str] = None) -> None:
@@ -569,48 +542,37 @@
         """
 
         self.request_counter += 1
 
         if query is None:
             query = self.current_query
 
-        response = self._session.delete(
+        response = self._oauth_client.delete(
             url=query,
             headers={**self.default_headers("delete"), **self.headers},
         )
 
         if response.status_code == status.HTTP_204_NO_CONTENT:
             return
 
         try:
-            response.raise_for_status()
-        except HTTPError as error:
+            data: DynamicsResponse = response.json()
+        except Exception as error:
             raise self.handled_error(
-                status_code=error.response.status_code,
-                error_message=f"{str(error)}. Response: {error.response.text}",
-                error_code="http_error",
-                method="delete",
-            ) from error
-
-        try:
-            data = response.json()
-        except JSONDecodeError as error:
-            raise self.handled_error(
-                status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
+                status_code=response.status_code,
                 error_message=f"{str(error)}. Response: {response.text}",
                 error_code="invalid_json",
-                method="get",
+                method="delete",
             ) from error
 
-        errors = data.get("error")
-        if errors:
+        if "error" in data:
             raise self.handled_error(
                 status_code=response.status_code,
-                error_message=errors.get("message"),
-                error_code=errors.get("code"),
+                error_message=data["error"]["message"],
+                error_code=data["error"]["code"],
                 method="delete",
             )
 
     def create_task(self, method: Callable[P, T], *args: P.args, **kwargs: P.kwargs) -> asyncio.Task:
         """Create task when the client is used as an async context manager.
 
         :param method: Client method to create task for.
@@ -847,15 +809,15 @@
         if not isinstance(items, (set, list)):
             raise TypeError("Filter items must be either a set or a list.")
         if not items:
             raise ValueError("Filter list cannot be empty.")
 
         self._filter = items
 
-    def _compile_filter(self, values: FilterType = sentinel) -> str:  # pylint: disable=R1710
+    def _compile_filter(self, values: FilterType = sentinel) -> str:
         if values is sentinel:
             values = self._filter
 
         if not values:
             return ""
 
         if isinstance(values, set):
```

### Comparing `dynamics_client-0.5.7/dynamics/enums.py` & `dynamics_client-0.6.0/dynamics/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     UPDATE = 2
     """Attribute values that are valid for update."""
     READ = 3
     """Attribute values that are valid for read."""
 
 
 class EntityFilter(IntEnum):
-    """Describes the type of entity metadata to retrieve."""
+    """Describes the entity metadata to retrieve."""
 
     ENTITY = 1
     """Use this to retrieve only entity information."""
     ATTRIBUTES = 2
     """Use this to retrieve entity information plus attributes for the entity."""
     PRIVILEGES = 4
     """Use this to retrieve entity information plus privileges for the entity."""
```

### Comparing `dynamics_client-0.5.7/dynamics/exceptions.py` & `dynamics_client-0.6.0/dynamics/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 
 class DynamicsException(APIException):
     status_code = status.HTTP_500_INTERNAL_SERVER_ERROR
     default_detail = "Dynamics Web API call failed."
     default_code = "dynamics_link_failed"
 
-    def __init__(self, detail=None, code=None, **kwargs):  # pylint: disable=W0613
+    def __init__(self, detail=None, code=None, **kwargs):
         detail = self.default_detail if detail is None else detail
         code = self.default_code if code is None else code
         self.args = (str(detail),)  # since APIException doesn't call super()
         super().__init__(detail, code)
 
 
 class ParseError(DynamicsException):
```

### Comparing `dynamics_client-0.5.7/dynamics/fetchxml.py` & `dynamics_client-0.6.0/dynamics/fetchxml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=W0212
 from xml.etree.ElementTree import Element, SubElement, tostring
 
 from .enums import FetchXMLOperator
 from .typing import (
     Any,
     FetchXMLAggregateType,
     FetchXMLAttributeType,
@@ -26,15 +25,15 @@
 
 __all__ = [
     "FetchXMLBuilder",
 ]
 
 
 def _serialize_bool(value: bool) -> LiteralBool:
-    return "true" if value else "false"  # type: ignore
+    return "true" if value else "false"
 
 
 class FetchXMLBuilder:
     def __init__(  # noqa: C901
         self,
         *,
         mapping: Optional[FetchXMLFetchMappingType] = None,
@@ -317,15 +316,15 @@
         self._attributes.append(attribute)
         return self
 
     def add_linked_entity(
         self,
         *,
         name: str,
-        to: str,  # pylint: disable=C0103
+        to: str,
         from_: Optional[str] = None,
         alias: Optional[str] = None,
         link_type: Optional[str] = None,
         visible: Optional[bool] = None,
         intersect: Optional[bool] = None,
         enable_prefiltering: Optional[bool] = None,
         prefilter_parameter_name: Optional[str] = None,
@@ -407,21 +406,21 @@
         return filter_builder
 
     def build(self) -> str:
         """Build the FetchXML query string."""
         return self._parent_builder.build()
 
 
-class _LinkedEntityBuilder:  # pylint: disable=R0902
+class _LinkedEntityBuilder:
     def __init__(
         self,
         parent_builder: Union["_EntityBuilder", "_LinkedEntityBuilder"],
         *,
         name: str,
-        to: str,  # pylint: disable=C0103
+        to: str,
         from_: Optional[str] = None,
         alias: Optional[str] = None,
         link_type: Optional[str] = None,
         visible: Optional[bool] = None,
         intersect: Optional[bool] = None,
         enable_prefiltering: Optional[bool] = None,
         prefilter_parameter_name: Optional[str] = None,
@@ -545,15 +544,15 @@
         self._attributes.append(attribute)
         return self
 
     def add_nested_linked_entity(
         self,
         *,
         name: str,
-        to: str,  # pylint: disable=C0103
+        to: str,
         from_: Optional[str] = None,
         alias: Optional[str] = None,
         link_type: Optional[str] = None,
         visible: Optional[bool] = None,
         intersect: Optional[bool] = None,
         enable_prefiltering: Optional[bool] = None,
         prefilter_parameter_name: Optional[str] = None,
@@ -588,15 +587,15 @@
         self._linked_entities.append(nested_linked_entity_builder)
         return nested_linked_entity_builder
 
     def add_linked_entity(
         self,
         *,
         name: str,
-        to: str,  # pylint: disable=C0103
+        to: str,
         from_: Optional[str] = None,
         alias: Optional[str] = None,
         link_type: Optional[str] = None,
         visible: Optional[bool] = None,
         intersect: Optional[bool] = None,
         enable_prefiltering: Optional[bool] = None,
         prefilter_parameter_name: Optional[str] = None,
@@ -727,15 +726,15 @@
         operator: Union[str, FetchXMLOperator],
         value: Optional[Any] = None,
         values: Optional[List[Any]] = None,
         value_of: Optional[str] = None,
         column: Optional[str] = None,
         entity_name: Optional[str] = None,
         aggregate: Optional[FetchXMLAggregateType] = None,
-        row_aggregate: Optional[Literal["countchildren"]] = None,  # noqa: F821
+        row_aggregate: Optional[Literal["countchildren"]] = None,
         alias: Optional[str] = None,
         uiname: Optional[str] = None,
         uitype: Optional[str] = None,
         uihidden: Optional[bool] = None,
     ) -> "_FilterBuilder":
         """Add a filtering condition to the filter.
 
@@ -755,15 +754,15 @@
         :return: The current instance of FilterBuilder.
         """
 
         if len(self._conditions) == 500:
             raise RuntimeError("Too many conditions (>500)")
 
         # Convert string to operators, raises TypeError if not valid
-        if type(operator) == str:  # pylint: disable=C0123
+        if type(operator) == str:
             operator = FetchXMLOperator(operator)
 
         condition = FetchXMLCondition(attribute=attribute, operator=operator.value)
         if value is not None:
             condition["value"] = str(value)
         if values is not None:
             condition["values"] = [str(v) for v in values]
@@ -780,24 +779,24 @@
         if alias is not None:
             condition["alias"] = alias
         if uiname is not None:
             condition["uiname"] = uiname
         if uitype is not None:
             condition["uitype"] = uitype
         if uihidden is not None:
-            condition["uihidden"] = "1" if uihidden else "0"  # type: ignore
+            condition["uihidden"] = "1" if uihidden else "0"
 
         self._conditions.append(condition)
         return self
 
     def add_linked_entity(
         self,
         *,
         name: str,
-        to: str,  # pylint: disable=C0103
+        to: str,
         from_: Optional[str] = None,
         alias: Optional[str] = None,
         link_type: Optional[str] = None,
         visible: Optional[bool] = None,
         intersect: Optional[bool] = None,
         enable_prefiltering: Optional[bool] = None,
         prefilter_parameter_name: Optional[str] = None,
```

### Comparing `dynamics_client-0.5.7/dynamics/normalizers.py` & `dynamics_client-0.6.0/dynamics/normalizers.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     except (ValueError, TypeError):
         return default
 
 
 def as_bool(value: Any, default: bool = False) -> bool:
     try:
         return bool(value)
-    except Exception:  # pylint: disable=W0703
+    except Exception:
         return default
 
 
 def str_as_datetime(value: str, default: Any = None) -> Optional[datetime]:
     try:
         return from_dynamics_date_format(value)
-    except Exception:  # pylint: disable=W0703
+    except Exception:
         return default
```

### Comparing `dynamics_client-0.5.7/dynamics/query_functions.py` & `dynamics_client-0.6.0/dynamics/query_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-# pylint: disable=C0103
 """
 Creates a helper object `ftr`, which contains convenience functions of all possible filter operations.
 
 Standard Operators API reference:
 https://docs.microsoft.com/en-us/powerapps/developer/data-platform/webapi/query-data-web-api#standard-filter-operators
 
 Special Operators API reference:
 https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9
 """
 
-
 from .typing import CompType, FieldType, List, Optional, Tuple
 from .utils import is_valid_uuid
 
 __all__ = ["ftr"]
 
 
-class ftr:  # pylint: disable=R0904
+class ftr:
     """Convenience functions for creating $filter parameters."""
 
     # Base operations
 
     @staticmethod
     def _type(value: FieldType, quotes: bool = False) -> str:
         if value is True:
@@ -226,29 +224,29 @@
         """
         return ftr._comp_operator(column, value, lambda_indicator, "le", group)
 
     # Logical operations
 
     @staticmethod
     def and_(*args: str, **kwargs) -> str:
-        """Evaluate whether all of the given operations are true.
+        """Evaluate whether all the given operations are true.
 
         :param args: Other filter operation strings to `and` together.
         :param kwargs: group=True -> Group the operation inside parentheses.
         """
-        return ftr._join_multiple(operator="and", group=kwargs.get("group", False), *args)  # noqa: B026
+        return ftr._join_multiple(*args, operator="and", group=kwargs.get("group", False))
 
     @staticmethod
     def or_(*args: str, **kwargs) -> str:
         """Evaluate whether any of the given operations are true.
 
         :param args: Other filter operation strings to `or` together.
         :param kwargs: group=True -> Group the operation inside parentheses.
         """
-        return ftr._join_multiple(operator="or", group=kwargs.get("group", False), *args)  # noqa: B026
+        return ftr._join_multiple(*args, operator="or", group=kwargs.get("group", False))
 
     @staticmethod
     def not_(operation: str, group: bool = False) -> str:
         """Invert the evaluation of an operation. Only works on standard operators!"""
         return ftr._group(f"not {operation}", group)
 
     # Standard query functions
```

### Comparing `dynamics_client-0.5.7/dynamics/status.py` & `dynamics_client-0.6.0/dynamics/status.py`

 * *Files identical despite different names*

### Comparing `dynamics_client-0.5.7/dynamics/test.py` & `dynamics_client-0.6.0/dynamics/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import json
 from contextlib import contextmanager
 from itertools import cycle as _cycle
 from unittest.mock import patch
 
 import pytest
-from requests import HTTPError
 
 from .client import DynamicsClient
 from .typing import Any, Dict, Iterator, List, MethodType, Optional, ResponseType
 
 __all__ = ["MockClient", "BaseMockClient", "dynamics_cache", "dynamics_client"]
 
 
 class BaseMockClient:
-    def __init__(self, *args, **kwargs):  # pylint: disable=W0613
+    def __init__(self, *args, **kwargs):
         with patch("dynamics.client.DynamicsClient.get_token"):
             super().__init__(
                 "http://dynamics.local/", "http://token.local", "client_id", "client_secret", ["http://scope.local/"]
             )
 
         self.__len: int = -1
         self.__default_status: int = 200
@@ -100,16 +99,16 @@
             raise TypeError("Cannot call 'next_exception' without setting exceptions first") from error
 
     @property
     def current_response(self) -> ResponseType:
         """Not needed if not using the 'dynamics_client.internal'.
 
         :return: The last expected response from the client.
-                 Tries to correct for some of the internal logic of the
-                 client methods, but might not be correct all of the time.
+                 Tries to correct for some internal logic of the
+                 client methods, but might not be correct all the time.
         """
         return self.__response
 
     def _check_length(self, length: int) -> "BaseMockClient":
         if self.__len not in (length, -1):
             raise ValueError("Mismatching number of arguments given for MockResponse")
         self.__len = length
@@ -129,39 +128,38 @@
                 raise ValueError("Ran out of status codes on the MockClient") from error
 
             response_mock = ResponseMock(response=self.__response, status_code=status_code)
 
             if method == "get" and isinstance(self.__response, dict):
                 self.__response = self.__response.get("value", [self.__response])
 
-            with patch(f"requests_oauthlib.oauth2_session.OAuth2Session.{method}", side_effect=[response_mock]):
+            with patch(f"authlib.integrations.httpx_client.OAuth2Client.{method}", side_effect=[response_mock]):
                 yield
         else:
-
             client_class = self.__class__.__bases__[-1]
             class_dot_path = f"{client_class.__module__}.{client_class.__qualname__}"
 
             with patch(f"{class_dot_path}.{method}", side_effect=[self.__response]):
                 yield
 
     def get(self, *, not_found_ok: bool = False, query: Optional[str] = None, **kwargs) -> List[Dict[str, Any]]:
         with self._mock_method("get"):
-            return super().get(not_found_ok=not_found_ok, query=query, **kwargs)  # noqa pylint: disable=E1101
+            return super().get(not_found_ok=not_found_ok, query=query, **kwargs)
 
     def post(self, data: Dict[str, Any], *, query: Optional[str] = None, **kwargs) -> Dict[str, Any]:
         with self._mock_method("post"):
-            return super().post(data=data, query=query, **kwargs)  # noqa pylint: disable=E1101
+            return super().post(data=data, query=query, **kwargs)
 
     def patch(self, data: Dict[str, Any], *, query: Optional[str] = None, **kwargs) -> Dict[str, Any]:
         with self._mock_method("patch"):
-            return super().patch(data=data, query=query, **kwargs)  # noqa pylint: disable=E1101
+            return super().patch(data=data, query=query, **kwargs)
 
     def delete(self, *, query: Optional[str] = None, **kwargs) -> None:
         with self._mock_method("delete"):
-            return super().delete(query=query, **kwargs)  # noqa pylint: disable=E1101
+            return super().delete(query=query, **kwargs)
 
 
 class MockClient(BaseMockClient, DynamicsClient):
     r"""A testing client for the Dynamics client.
 
     -----------------------------------------------------------
 
@@ -199,32 +197,32 @@
     """
 
 
 @pytest.fixture(scope="session")
 def _dynamics_cache_constructor():
     """Imports the django cache instance or creates a SQLiteCache instance."""
     try:
-        from django.core.cache import cache  # pylint: disable=C0415,W0621
+        from django.core.cache import cache
     except ImportError:
-        from dynamics.utils import SQLiteCache  # pylint: disable=C0415,W0621
+        from dynamics.utils import SQLiteCache
 
         cache = SQLiteCache()
 
     return cache
 
 
 @pytest.fixture()
-def dynamics_cache(_dynamics_cache_constructor):  # pylint: disable=W0621
+def dynamics_cache(_dynamics_cache_constructor):
     """Get the session instance of either Django's cache or SQLiteCache."""
     _dynamics_cache_constructor.clear()
     yield _dynamics_cache_constructor
 
 
 @pytest.fixture
-def dynamics_client(request) -> MockClient:  # pylint: disable=W0621
+def dynamics_client(request) -> MockClient:
     """Get a mocked client instance, or forward one created in `pytest.mark.parametrize`."""
     if not hasattr(request, "param"):
         yield MockClient()
     else:
         yield request.param
 
 
@@ -238,12 +236,8 @@
             raise self.response
         return self.response
 
     @property
     def text(self) -> str:
         if isinstance(self.response, Exception):
             return str(self.response)
-        return json.dumps(self.response)
-
-    def raise_for_status(self) -> None:
-        if isinstance(self.response, HTTPError):
-            raise self.response
+        return json.dumps(self.response)  # pragma: no cover
```

### Comparing `dynamics_client-0.5.7/dynamics/typing.py` & `dynamics_client-0.6.0/dynamics/typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,95 +1,93 @@
-from .enums import FetchXMLOperator
+from __future__ import annotations
+
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Awaitable,
+    Callable,
+    Coroutine,
+    Dict,
+    Iterator,
+    List,
+    Literal,
+    Optional,
+    Sequence,
+    Set,
+    Tuple,
+    Type,
+    TypedDict,
+    TypeVar,
+    Union,
+)
+
+# New in version 3.10
+try:
+    from typing import ParamSpec, TypeGuard
+except ImportError:
+    from typing_extensions import ParamSpec, TypeGuard
 
+# New in version 3.11
 try:
-    from typing import (
-        TYPE_CHECKING,
-        Any,
-        Awaitable,
-        Callable,
-        Dict,
-        Iterator,
-        List,
-        Literal,
-        Optional,
-        ParamSpec,
-        Sequence,
-        Set,
-        Tuple,
-        Type,
-        TypedDict,
-        TypeVar,
-        Union,
-    )
+    from typing import NotRequired, Required
 except ImportError:
-    from typing import (
-        TYPE_CHECKING,
-        Any,
-        Awaitable,
-        Callable,
-        Dict,
-        Iterator,
-        List,
-        Optional,
-        Sequence,
-        Set,
-        Tuple,
-        Type,
-        TypeVar,
-        Union,
-    )
+    from typing_extensions import NotRequired, Required
 
-    from typing_extensions import Literal, ParamSpec, TypedDict
 
+from .enums import FetchXMLOperator
 
 __all__ = [
-    "List",
-    "Dict",
-    "Optional",
-    "Awaitable",
     "Any",
-    "Literal",
-    "Union",
-    "Set",
-    "Sequence",
-    "Type",
-    "Tuple",
-    "TypedDict",
-    "TypeVar",
-    "ParamSpec",
-    "Iterator",
-    "TYPE_CHECKING",
-    "ResponseType",
-    "MethodType",
-    "OrderbyType",
-    "FilterType",
-    "ExpandType",
+    "Awaitable",
+    "Callable",
+    "CompType",
+    "Coroutine",
+    "Dict",
+    "ExpandDict",
     "ExpandKeys",
+    "ExpandType",
     "ExpandValues",
     "ExpandValues",
-    "ExpandDict",
-    "Callable",
-    "CompType",
-    "FieldType",
-    "LiteralBool",
-    "FetchXMLCondition",
-    "FetchXMLAttributeType",
-    "FetchXMLOrderType",
-    "FetchXMLType",
-    "FetchXMLEntityType",
-    "FetchXMLLinkedEntity",
-    "FetchXMLFilterType",
     "FetchXMLAggregateType",
-    "FetchXMLOutputFormat",
-    "FetchXMLDateGroupingType",
+    "FetchXMLAttributeType",
     "FetchXMLBuildType",
+    "FetchXMLCondition",
+    "FetchXMLDateGroupingType",
+    "FetchXMLEntityType",
     "FetchXMLFetchMappingType",
     "FetchXMLFilterOperatorType",
-    "T",
+    "FetchXMLFilterType",
+    "FetchXMLLinkedEntity",
+    "FetchXMLOrderType",
+    "FetchXMLOutputFormat",
+    "FetchXMLType",
+    "FieldType",
+    "FilterType",
+    "Iterator",
+    "List",
+    "Literal",
+    "LiteralBool",
+    "MethodType",
+    "NotRequired",
+    "Optional",
+    "OrderbyType",
     "P",
+    "ParamSpec",
+    "Required",
+    "ResponseType",
+    "Sequence",
+    "Set",
+    "T",
+    "Tuple",
+    "Type",
+    "TYPE_CHECKING",
+    "TypedDict",
+    "TypeGuard",
+    "TypeVar",
+    "Union",
 ]
 
 MethodType = Literal["get", "post", "patch", "delete"]
 OrderbyType = Dict[str, Literal["asc", "desc"]]
 FilterType = Union[Set[str], List[str]]
 
 
@@ -102,18 +100,53 @@
 
 
 ExpandKeys = Literal["select", "filter", "top", "orderby", "expand"]
 ExpandValues = Union[List[str], Set[str], int, OrderbyType, Dict[str, ExpandType]]
 ExpandDict = Dict[str, Optional[ExpandType]]
 FieldType = Union[str, int, float, bool, None]
 CompType = Union[str, int, float]
-T = TypeVar("T")  # pylint: disable=C0103
-P = ParamSpec("P")  # pylint: disable=C0103
+T = TypeVar("T")
+P = ParamSpec("P")
 ResponseType = Union[Union[Dict[str, Any], List[Dict[str, Any]]], Exception, None]
 
+
+DynamicsOKResponse = TypedDict(
+    "DynamicsOKResponse",
+    {
+        "value": List[Dict[str, Any]],
+        "@odata.context": str,
+        "@odata.nextLink": NotRequired[str],
+        "@odata.count": NotRequired[int],
+    },
+)
+
+
+# https://learn.microsoft.com/en-us/power-apps/developer/data-platform/webapi/compose-http-requests-handle-errors#include-more-details-with-errors
+DynamicsErrorResponseData = TypedDict(
+    "DynamicsErrorResponseData",
+    {
+        "code": Required[str],
+        "message": Required[str],
+        "@Microsoft.PowerApps.CDS.ErrorDetails.OperationStatus": str,
+        "@Microsoft.PowerApps.CDS.ErrorDetails.SubErrorCode": str,
+        "@Microsoft.PowerApps.CDS.HelpLink": str,
+        "@Microsoft.PowerApps.CDS.TraceText": str,
+        "@Microsoft.PowerApps.CDS.InnerError.Message": str,
+    },
+    total=False,
+)
+
+
+class DynamicsErrorResponse(TypedDict):
+    error: DynamicsErrorResponseData
+
+
+DynamicsResponse = Union[DynamicsOKResponse, DynamicsErrorResponse]
+
+
 LiteralBool = Literal["true", "false"]
 FetchXMLOutputFormat = Literal["xml-ado", "xml-auto", "xml-elements", "xml-raw", "xml-platform"]
 FetchXMLDateGroupingType = Literal["day", "week", "month", "quarter", "year", "fiscal-period", "fiscal-year"]
 FetchXMLAggregateType = Literal["count", "countcolumn", "sum", "avg", "min", "max"]
 FetchXMLBuildType = Literal["1.504021", "1.003017"]
 FetchXMLFilterOperatorType = Literal["and", "or"]
 FetchXMLFetchMappingType = Literal["internal", "logical"]
```

### Comparing `dynamics_client-0.5.7/dynamics/utils.py` & `dynamics_client-0.6.0/dynamics/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import logging
 import pickle
 import sqlite3
 import tempfile
 from datetime import datetime, timedelta, timezone
 from functools import wraps
 from pathlib import Path
-from typing import Union
 from uuid import UUID
 
 from .exceptions import DynamicsException
 
 try:
     from zoneinfo import ZoneInfo
 except ImportError:
     from backports.zoneinfo import ZoneInfo
 
-from .typing import TYPE_CHECKING, Any, Awaitable, Callable, List, Optional, P, T, Type
+from .typing import TYPE_CHECKING, Any, Awaitable, Callable, Coroutine, List, Optional, P, T, Type, Union
 
 if TYPE_CHECKING:
     from . import DynamicsClient
 
 
 __all__ = [
     "to_dynamics_date_format",
@@ -32,23 +31,23 @@
     "to_coroutine",
 ]
 
 
 logger = logging.getLogger(__name__)
 
 
-class sentinel:  # pylint: disable=C0103
+class sentinel:
     """Sentinel value."""
 
 
 def is_valid_uuid(value: str):
     try:
         uuid = UUID(value)
         return str(uuid) == value
-    except Exception:  # pylint: disable=W0703
+    except Exception:
         return False
 
 
 def to_dynamics_date_format(date: datetime, from_timezone: str = None) -> str:
     """Convert a datetime-object to a Dynamics compatible ISO formatted date string.
 
     :param date: Datetime object.
@@ -87,25 +86,25 @@
     return value or exception propagated.
     """
 
     @wraps(method)
     def inner(*args: P.args, **kwargs: P.kwargs) -> T:
         self = args[0]
         self.con = sqlite3.connect(self.connection_string)
-        self._apply_pragma()  # pylint: disable=W0212
+        self._apply_pragma()
 
         try:
             value = method(*args, **kwargs)
             self.con.commit()
         except Exception as sqlerror:
-            self.con.execute(self._set_pragma.format("optimize"))  # pylint: disable=W0212
+            self.con.execute(self._set_pragma.format("optimize"))
             self.con.close()
             raise sqlerror
 
-        self.con.execute(self._set_pragma.format("optimize"))  # pylint: disable=W0212
+        self.con.execute(self._set_pragma.format("optimize"))
         self.con.close()
         return value
 
     return inner
 
 
 class SQLiteCache:
@@ -160,15 +159,15 @@
 
     @staticmethod
     def _stream(value: Any) -> bytes:
         return pickle.dumps(value)
 
     @staticmethod
     def _unstream(value: bytes) -> Any:
-        return pickle.loads(value)
+        return pickle.loads(value)  # noqa: S301
 
     def _apply_pragma(self):
         for key, value in self.DEFAULT_PRAGMA.items():
             self.con.execute(self._set_pragma_equal.format(key, value))
 
     @sqlite_method
     def get(self, key: str, default: Any = None) -> Any:
@@ -226,25 +225,25 @@
     @wraps(func)
     def inner(*args: P.args, **kwargs: P.kwargs) -> T:
         simplify_errors: bool = kwargs.pop("simplify_errors", False)
         raise_separately: List[Type[Exception]] = kwargs.pop("raise_separately", [])
 
         try:
             return func(*args, **kwargs)
-        except Exception as error:  # pylint: disable=W0703
+        except Exception as error:
             logger.warning(error)
             if not simplify_errors or any(isinstance(error, exception) for exception in raise_separately):
                 raise error
             self: "DynamicsClient" = args[0]
             raise DynamicsException(self.simplified_error_message) from error
 
     return inner
 
 
-def to_coroutine(func: Callable[P, T]) -> Callable[P, Awaitable[T]]:
+def to_coroutine(func: Callable[P, T]) -> Callable[P, Coroutine[Awaitable[T], Any, Any]]:
     """Convert passed callable into a coroutine."""
 
     @wraps(func)
     async def wrapper(*args: P.args, **kw: P.kwargs) -> Any:
         return func(*args, **kw)
 
     return wrapper
```

### Comparing `dynamics_client-0.5.7/pyproject.toml` & `dynamics_client-0.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dynamics-client"
-version = "0.5.7"
+version = "0.6.0"
 description = "Client for making Web API request from a Microsoft Dynamics 365 Database."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "dynamics" },
 ]
@@ -38,51 +38,54 @@
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/MrThearMan/dynamics-client/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
-oauthlib = ">=3.1.0"
-requests-oauthlib = ">=1.3.0"
+httpx = ">=0.23.3"
+authlib = ">=1.2.0"
 tzdata = ">=2021.5"
 "backports.zoneinfo" = { version = ">=0.2.1", python = "<3.9" }
-typing-extensions = { version = ">=4.0", python = "<3.9" }
+typing-extensions = { version = ">=4.5", python = "<3.11" }
 Django = { version = ">=3.2", optional = true }
 djangorestframework = { version = ">=3.12", optional = true }
 
 [tool.poetry.group.test.dependencies]
-pytest = "7.2.1"
+pytest = "7.3.0"
 coverage = "6.5.0"
-pytest-asyncio = "0.20.3"
-pre-commit = "3.0.1"
-tox = "4.4.2"
-tox-gh-actions = "3.0.0"
+pytest-asyncio = "0.21.0"
+pre-commit = "3.2.2"
+tox = "4.4.11"
+tox-gh-actions = "3.1.0"
 coveralls = "3.3.1"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.4.2"
-pymdown-extensions = "9.9.2"
+pymdown-extensions = "9.11"
 mkdocs-mermaid2-plugin = "0.6.0"
 
 [tool.poetry.group.lint.dependencies]
-mypy = "0.991"
+mypy = "1.2.0"
 
 [tool.poetry.extras]
 django = ["Django", "djangorestframework"]
 
 [tool.black]
 line-length = 120
 
 [tool.ruff]
 fix = true
 line-length = 120
 exclude = [
     "tests/*",
 ]
+typing-modules = [
+    "dynamics.typing",
+]
 select = [
     "F",  # pyflakes
     "E",  # pycodestyle errors
     "I",  # isort
     "S",  # flake8-bandit
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
```

### Comparing `dynamics_client-0.5.7/setup.py` & `dynamics_client-0.6.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,214 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dynamics-client
+Version: 0.6.0
+Summary: Client for making Web API request from a Microsoft Dynamics 365 Database.
+Home-page: https://github.com/MrThearMan/dynamics-client/
+License: MIT
+Keywords: Microsoft,Dynamics,client
+Author: Matti Lamppu
+Author-email: lamppu.matti.akseli@gmail.com
+Requires-Python: >=3.8,<4
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: django
+Requires-Dist: Django (>=3.2) ; extra == "django"
+Requires-Dist: authlib (>=1.2.0)
+Requires-Dist: backports.zoneinfo (>=0.2.1) ; python_version < "3.9"
+Requires-Dist: djangorestframework (>=3.12) ; extra == "django"
+Requires-Dist: httpx (>=0.23.3)
+Requires-Dist: typing-extensions (>=4.5) ; python_version < "3.11"
+Requires-Dist: tzdata (>=2021.5)
+Project-URL: Bug Tracker, https://github.com/MrThearMan/dynamics-client/issues
+Project-URL: Repository, https://github.com/MrThearMan/dynamics-client/
+Description-Content-Type: text/markdown
+
+# Dynamics Web API Client
+
+[![Coverage Status][coverage-badge]][coverage]
+[![GitHub Workflow Status][status-badge]][status]
+[![PyPI][pypi-badge]][pypi]
+[![GitHub][licence-badge]][licence]
+[![GitHub Last Commit][repo-badge]][repo]
+[![GitHub Issues][issues-badge]][issues]
+[![Downloads][downloads-badge]][pypi]
+[![Python Version][version-badge]][pypi]
+
+```shell
+pip install dynamics-client
+```
+
+---
+
+**Documentation**: [https://mrthearman.github.io/dynamics-client/](https://mrthearman.github.io/dynamics-client/)
+
+**Source Code**: [https://github.com/MrThearMan/dynamics-client/](https://github.com/MrThearMan/dynamics-client/)
+
+---
+
+Client for making Web API request from a Microsoft Dynamics 365 Database.
+
+You should also read the [Dynamics Web API Reference Docs][ref-docs]:
+
+
+## Basic usage:
+
+```python
+from dynamics import DynamicsClient, ftr
+
+# Init the client:
+client = DynamicsClient(...)
+
+### Example GET request:
+
+client.table = "accounts"
+
+# Get only these columns for the account.
+client.select = ["accountid", "name"]
+
+# Filter to only the accounts that have been created on or after the
+# given ISO date string, AND that have 200 or more employees.
+client.filter = [
+    ftr.on_or_after("createdon", "2020-01-01T00:00:00Z"),
+    ftr.ge("numberofemployees", 200),
+]
+
+# Expand to the contacts (collection-values navigation property)
+# on the account that have 'gmail.com' in their email address 1 OR 2.
+# Get only the 'firstname', 'lastname' and 'mobilephone' columns for these contacts.
+# Also expand the primary contact (single-valued navigation property).
+# Get only the 'emailaddress1' column for the primary contact.
+client.expand = {
+    "contact_customer_accounts": {
+        "select": ["firstname", "lastname", "mobilephone"],
+        "filter": {
+            ftr.contains("emailaddress1", "gmail.com"),
+            ftr.contains("emailaddress2", "gmail.com"),
+        }
+    },
+    "primarycontactid": {
+        "select": ["emailaddress1"],
+    },
+}
+
+result = client.get()
+
+# [
+#     {
+#         "accountid": ...,
+#         "name": ...,
+#         "contact_customer_accounts": [
+#             {
+#                 "contactid": ...,  # id field is always given
+#                 "firstname": ...,
+#                 "lastname": ...,
+#                 "mobilephone": ...
+#             },
+#             ...
+#         ],
+#         "primarycontactid": {
+#             "contactid": ...,
+#             "emailaddress1": ...
+#         }
+#     },
+#     ...
+# ]
+
+### Example POST request
+
+# IMPORTANT!!!
+client.reset_query()
+
+client.table = "contacts"
+
+# Get only these columns from the created contact
+client.select = ["firstname", "lastname", "emailaddress1"]
+
+# The data to create the contact with. '@odata.bind' is used to link
+# the contact to the given navigation property.
+accountid = ...
+data = {
+    "firstname": ...,
+    "lastname": ...,
+    "emailaddress1": ...,
+    "parentcustomerid_account@odata.bind": f"/accounts({accountid})"
+}
+
+result = client.post(data=data)
 
-packages = \
-['dynamics']
+# {
+#     "contactid": ...,
+#     "firstname": ...,
+#     "lastname": ...,
+#     "emailaddress1": ...
+# }
 
-package_data = \
-{'': ['*']}
 
-install_requires = \
-['oauthlib>=3.1.0', 'requests-oauthlib>=1.3.0', 'tzdata>=2021.5']
-
-extras_require = \
-{':python_version < "3.9"': ['backports.zoneinfo>=0.2.1',
-                             'typing-extensions>=4.0'],
- 'django': ['Django>=3.2', 'djangorestframework>=3.12']}
-
-setup_kwargs = {
-    'name': 'dynamics-client',
-    'version': '0.5.7',
-    'description': 'Client for making Web API request from a Microsoft Dynamics 365 Database.',
-    'long_description': '# Dynamics Web API Client\n\n[![Coverage Status][coverage-badge]][coverage]\n[![GitHub Workflow Status][status-badge]][status]\n[![PyPI][pypi-badge]][pypi]\n[![GitHub][licence-badge]][licence]\n[![GitHub Last Commit][repo-badge]][repo]\n[![GitHub Issues][issues-badge]][issues]\n[![Downloads][downloads-badge]][pypi]\n[![Python Version][version-badge]][pypi]\n\n```shell\npip install dynamics-client\n```\n\n---\n\n**Documentation**: [https://mrthearman.github.io/dynamics-client/](https://mrthearman.github.io/dynamics-client/)\n\n**Source Code**: [https://github.com/MrThearMan/dynamics-client/](https://github.com/MrThearMan/dynamics-client/)\n\n---\n\nClient for making Web API request from a Microsoft Dynamics 365 Database.\n\nYou should also read the [Dynamics Web API Reference Docs][ref-docs]:\n\n\n## Basic usage:\n\n```python\nfrom dynamics import DynamicsClient, ftr\n\n# Init the client:\nclient = DynamicsClient(...)\n\n### Example GET request:\n\nclient.table = "accounts"\n\n# Get only these columns for the account.\nclient.select = ["accountid", "name"]\n\n# Filter to only the accounts that have been created on or after the\n# given ISO date string, AND that have 200 or more employees.\nclient.filter = [\n    ftr.on_or_after("createdon", "2020-01-01T00:00:00Z"),\n    ftr.ge("numberofemployees", 200),\n]\n\n# Expand to the contacts (collection-values navigation property)\n# on the account that have \'gmail.com\' in their email address 1 OR 2.\n# Get only the \'firstname\', \'lastname\' and \'mobilephone\' columns for these contacts.\n# Also expand the primary contact (single-valued navigation property).\n# Get only the \'emailaddress1\' column for the primary contact.\nclient.expand = {\n    "contact_customer_accounts": {\n        "select": ["firstname", "lastname", "mobilephone"],\n        "filter": {\n            ftr.contains("emailaddress1", "gmail.com"),\n            ftr.contains("emailaddress2", "gmail.com"),\n        }\n    },\n    "primarycontactid": {\n        "select": ["emailaddress1"],\n    },\n}\n\nresult = client.get()\n\n# [\n#     {\n#         "accountid": ...,\n#         "name": ...,\n#         "contact_customer_accounts": [\n#             {\n#                 "contactid": ...,  # id field is always given\n#                 "firstname": ...,\n#                 "lastname": ...,\n#                 "mobilephone": ...\n#             },\n#             ...\n#         ],\n#         "primarycontactid": {\n#             "contactid": ...,\n#             "emailaddress1": ...\n#         }\n#     },\n#     ...\n# ]\n\n### Example POST request\n\n# IMPORTANT!!!\nclient.reset_query()\n\nclient.table = "contacts"\n\n# Get only these columns from the created contact\nclient.select = ["firstname", "lastname", "emailaddress1"]\n\n# The data to create the contact with. \'@odata.bind\' is used to link\n# the contact to the given navigation property.\naccountid = ...\ndata = {\n    "firstname": ...,\n    "lastname": ...,\n    "emailaddress1": ...,\n    "parentcustomerid_account@odata.bind": f"/accounts({accountid})"\n}\n\nresult = client.post(data=data)\n\n# {\n#     "contactid": ...,\n#     "firstname": ...,\n#     "lastname": ...,\n#     "emailaddress1": ...\n# }\n\n\n### Example PATCH request\n\nclient.reset_query()\n\nclient.table = "contacts"\nclient.row_id = result["contactid"]\n\ndata = {\n    "firstname": ...,\n    "lastname": ...,\n}\n\nresult = client.patch(data=data)\n\n# Return all rows on the updated contact,\n# since no select statement was given\n#\n# {\n#     ...\n#     "contactid": ...,\n#     "firstname": ...,\n#     "lastname": ...,\n#     ...\n# }\n\n\n### Example DELETE request\n\nclient.reset_query()\n\nclient.table = "contacts"\nclient.row_id = result["contactid"]\n\nclient.delete()\n```\n\n\n[ref-docs]: https://docs.microsoft.com/en-us/powerapps/developer/data-platform/webapi/query-data-web-api\n\n[coverage-badge]: https://coveralls.io/repos/github/MrThearMan/dynamics-client/badge.svg?branch=main\n[status-badge]: https://img.shields.io/github/actions/workflow/status/MrThearMan/dynamics-client/test.yml?branch=main\n[pypi-badge]: https://img.shields.io/pypi/v/dynamics-client\n[licence-badge]: https://img.shields.io/github/license/MrThearMan/dynamics-client\n[repo-badge]: https://img.shields.io/github/last-commit/MrThearMan/dynamics-client\n[issues-badge]: https://img.shields.io/github/issues-raw/MrThearMan/dynamics-client\n[version-badge]: https://img.shields.io/pypi/pyversions/dynamics-client\n[downloads-badge]: https://img.shields.io/pypi/dm/dynamics-client\n\n[coverage]: https://coveralls.io/github/MrThearMan/dynamics-client?branch=main\n[status]: https://github.com/MrThearMan/dynamics-client/actions/workflows/test.yml\n[pypi]: https://pypi.org/project/dynamics-client\n[licence]: https://github.com/MrThearMan/dynamics-client/blob/main/LICENSE\n[repo]: https://github.com/MrThearMan/dynamics-client/commits/main\n[issues]: https://github.com/MrThearMan/dynamics-client/issues\n',
-    'author': 'Matti Lamppu',
-    'author_email': 'lamppu.matti.akseli@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/MrThearMan/dynamics-client/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4',
+### Example PATCH request
+
+client.reset_query()
+
+client.table = "contacts"
+client.row_id = result["contactid"]
+
+data = {
+    "firstname": ...,
+    "lastname": ...,
 }
 
+result = client.patch(data=data)
+
+# Return all rows on the updated contact,
+# since no select statement was given
+#
+# {
+#     ...
+#     "contactid": ...,
+#     "firstname": ...,
+#     "lastname": ...,
+#     ...
+# }
+
+
+### Example DELETE request
+
+client.reset_query()
+
+client.table = "contacts"
+client.row_id = result["contactid"]
+
+client.delete()
+```
+
+
+[ref-docs]: https://docs.microsoft.com/en-us/powerapps/developer/data-platform/webapi/query-data-web-api
+
+[coverage-badge]: https://coveralls.io/repos/github/MrThearMan/dynamics-client/badge.svg?branch=main
+[status-badge]: https://img.shields.io/github/actions/workflow/status/MrThearMan/dynamics-client/test.yml?branch=main
+[pypi-badge]: https://img.shields.io/pypi/v/dynamics-client
+[licence-badge]: https://img.shields.io/github/license/MrThearMan/dynamics-client
+[repo-badge]: https://img.shields.io/github/last-commit/MrThearMan/dynamics-client
+[issues-badge]: https://img.shields.io/github/issues-raw/MrThearMan/dynamics-client
+[version-badge]: https://img.shields.io/pypi/pyversions/dynamics-client
+[downloads-badge]: https://img.shields.io/pypi/dm/dynamics-client
+
+[coverage]: https://coveralls.io/github/MrThearMan/dynamics-client?branch=main
+[status]: https://github.com/MrThearMan/dynamics-client/actions/workflows/test.yml
+[pypi]: https://pypi.org/project/dynamics-client
+[licence]: https://github.com/MrThearMan/dynamics-client/blob/main/LICENSE
+[repo]: https://github.com/MrThearMan/dynamics-client/commits/main
+[issues]: https://github.com/MrThearMan/dynamics-client/issues
 
-setup(**setup_kwargs)
```


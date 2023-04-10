# Comparing `tmp/tap-core-0.0.2.tar.gz` & `tmp/tap-core-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-core-0.0.2.tar", last modified: Thu Jul 14 14:41:19 2022, max compression
+gzip compressed data, was "tap-core-0.0.3.tar", last modified: Mon Apr 10 20:20:43 2023, max compression
```

## Comparing `tap-core-0.0.2.tar` & `tap-core-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 14:41:19.760875 tap-core-0.0.2/
--rw-rw-rw-   0 root         (0) root         (0)    11341 2022-07-14 14:41:01.000000 tap-core-0.0.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-07-14 14:41:01.000000 tap-core-0.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    11532 2022-07-14 14:41:19.760875 tap-core-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10358 2022-07-14 14:41:01.000000 tap-core-0.0.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1094 2022-07-14 14:41:01.000000 tap-core-0.0.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     4523 2022-07-14 14:41:19.762875 tap-core-0.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2022-07-14 14:41:01.000000 tap-core-0.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 14:41:19.754875 tap-core-0.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 14:41:19.757875 tap-core-0.0.2/src/tap/
--rw-rw-rw-   0 root         (0) root         (0)      108 2022-07-14 14:41:01.000000 tap-core-0.0.2/src/tap/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 14:41:19.758875 tap-core-0.0.2/src/tap/api/
--rw-rw-rw-   0 root         (0) root         (0)     4618 2022-07-14 14:41:01.000000 tap-core-0.0.2/src/tap/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9899 2022-07-14 14:41:01.000000 tap-core-0.0.2/src/tap/api/client.py
--rw-rw-rw-   0 root         (0) root         (0)    14659 2022-07-14 14:41:01.000000 tap-core-0.0.2/src/tap/api/stream.py
--rw-rw-rw-   0 root         (0) root         (0)     4425 2022-07-14 14:41:01.000000 tap-core-0.0.2/src/tap/api/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 14:41:19.760875 tap-core-0.0.2/src/tap_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11532 2022-07-14 14:41:19.000000 tap-core-0.0.2/src/tap_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2022-07-14 14:41:19.000000 tap-core-0.0.2/src/tap_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 14:41:19.000000 tap-core-0.0.2/src/tap_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 14:41:19.000000 tap-core-0.0.2/src/tap_core.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      190 2022-07-14 14:41:19.000000 tap-core-0.0.2/src/tap_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2022-07-14 14:41:19.000000 tap-core-0.0.2/src/tap_core.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 20:20:43.571421 tap-core-0.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)    11341 2023-04-10 20:20:25.000000 tap-core-0.0.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-04-10 20:20:25.000000 tap-core-0.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11695 2023-04-10 20:20:43.571421 tap-core-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10521 2023-04-10 20:20:25.000000 tap-core-0.0.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2023-04-10 20:20:25.000000 tap-core-0.0.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     4464 2023-04-10 20:20:43.573421 tap-core-0.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-10 20:20:25.000000 tap-core-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 20:20:43.563420 tap-core-0.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 20:20:43.566421 tap-core-0.0.3/src/tap/
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-04-10 20:20:25.000000 tap-core-0.0.3/src/tap/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 20:20:43.569421 tap-core-0.0.3/src/tap/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2023-04-10 20:20:25.000000 tap-core-0.0.3/src/tap/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12114 2023-04-10 20:20:25.000000 tap-core-0.0.3/src/tap/api/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-10 20:20:25.000000 tap-core-0.0.3/src/tap/api/discovery.py
+-rw-rw-rw-   0 root         (0) root         (0)      520 2023-04-10 20:20:25.000000 tap-core-0.0.3/src/tap/api/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    15449 2023-04-10 20:20:25.000000 tap-core-0.0.3/src/tap/api/stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     3907 2023-04-10 20:20:25.000000 tap-core-0.0.3/src/tap/api/sync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2817 2023-04-10 20:20:25.000000 tap-core-0.0.3/src/tap/api/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      861 2023-04-10 20:20:25.000000 tap-core-0.0.3/src/tap/api/transform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 20:20:43.571421 tap-core-0.0.3/src/tap_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11695 2023-04-10 20:20:43.000000 tap-core-0.0.3/src/tap_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      481 2023-04-10 20:20:43.000000 tap-core-0.0.3/src/tap_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 20:20:43.000000 tap-core-0.0.3/src/tap_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 20:20:43.000000 tap-core-0.0.3/src/tap_core.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      185 2023-04-10 20:20:43.000000 tap-core-0.0.3/src/tap_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-10 20:20:43.000000 tap-core-0.0.3/src/tap_core.egg-info/top_level.txt
```

### Comparing `tap-core-0.0.2/LICENSE` & `tap-core-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-core-0.0.2/PKG-INFO` & `tap-core-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-core
-Version: 0.0.2
+Version: 0.0.3
 Summary: Singer.io Tap Core features
 Home-page: https://gitlab.com/singer-core/tap-core
 Author: Eddy ∆
 Author-email: edrdelta@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://singer-core.gitlab.io/tap-core
 Project-URL: Releases, https://gitlab.com/singer-core/tap-core/-/releases
@@ -25,21 +25,22 @@
 Provides-Extra: dist
 Provides-Extra: deploy
 Provides-Extra: docs
 License-File: LICENSE
 
 # Tap Core
 
-[![Pypi - License](https://img.shields.io/pypi/l/tap-core?color=yellow)](https://opensource.org/licenses/Apache-2.0)
+[![GitLab - License](https://img.shields.io/gitlab/license/singer-core/tap-core?color=blue)](https://gitlab.com/singer-core/tap-core/-/blob/main/LICENSE)
 [![Python package builder](https://gitlab.com/singer-core/tap-core/badges/main/pipeline.svg)](https://gitlab.com/singer-core/tap-core/pipelines)
 [![Coverage](https://codecov.io/gl/singer-core/tap-core/branch/main/graph/badge.svg?token=LBNSKSY3O9)](https://codecov.io/gl/singer-core/tap-core)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tap-core.svg)](https://pypi.org/project/tap-core)
 [![PyPI version](https://badge.fury.io/py/tap-core.svg)](https://badge.fury.io/py/tap-core)
 [![PyPi project installs](https://img.shields.io/pypi/dm/tap-core.svg?maxAge=2592000&label=installs&color=%2327B1FF)](https://pypistats.org/packages/tap-core)
 
+<!-- [![Pypi - License](https://img.shields.io/pypi/l/tap-core?color=yellow)](https://opensource.org/licenses/Apache-2.0) -->
 <!-- [![Coverage](https://gitlab.com/singer-core/tap-core/badges/main/coverage.svg)](https://gitlab.com/singer-core/tap-core/-/graphs/main/charts) -->
 <!-- [![Documentation Status](https://readthedocs.org/projects/tap-core/badge/?version=latest)](https://singer-core.gitlab.io/tap-core/en/latest/?badge=latest) -->
 <!-- [![Latest Release](https://gitlab.com/singer-core/tap-core/-/badges/release.svg)](https://gitlab.com/singer-core/tap-core/-/releases) -->
 
 [**Singer**](https://www.singer.io/) tap core provide safe tools to easily build new `taps` following the [*Singer spec*](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md) *convention* and *protocol*.
 
 ## How to use it
```

### Comparing `tap-core-0.0.2/README.md` & `tap-core-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Tap Core
 
-[![Pypi - License](https://img.shields.io/pypi/l/tap-core?color=yellow)](https://opensource.org/licenses/Apache-2.0)
+[![GitLab - License](https://img.shields.io/gitlab/license/singer-core/tap-core?color=blue)](https://gitlab.com/singer-core/tap-core/-/blob/main/LICENSE)
 [![Python package builder](https://gitlab.com/singer-core/tap-core/badges/main/pipeline.svg)](https://gitlab.com/singer-core/tap-core/pipelines)
 [![Coverage](https://codecov.io/gl/singer-core/tap-core/branch/main/graph/badge.svg?token=LBNSKSY3O9)](https://codecov.io/gl/singer-core/tap-core)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tap-core.svg)](https://pypi.org/project/tap-core)
 [![PyPI version](https://badge.fury.io/py/tap-core.svg)](https://badge.fury.io/py/tap-core)
 [![PyPi project installs](https://img.shields.io/pypi/dm/tap-core.svg?maxAge=2592000&label=installs&color=%2327B1FF)](https://pypistats.org/packages/tap-core)
 
+<!-- [![Pypi - License](https://img.shields.io/pypi/l/tap-core?color=yellow)](https://opensource.org/licenses/Apache-2.0) -->
 <!-- [![Coverage](https://gitlab.com/singer-core/tap-core/badges/main/coverage.svg)](https://gitlab.com/singer-core/tap-core/-/graphs/main/charts) -->
 <!-- [![Documentation Status](https://readthedocs.org/projects/tap-core/badge/?version=latest)](https://singer-core.gitlab.io/tap-core/en/latest/?badge=latest) -->
 <!-- [![Latest Release](https://gitlab.com/singer-core/tap-core/-/badges/release.svg)](https://gitlab.com/singer-core/tap-core/-/releases) -->
 
 [**Singer**](https://www.singer.io/) tap core provide safe tools to easily build new `taps` following the [*Singer spec*](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md) *convention* and *protocol*.
 
 ## How to use it
```

### Comparing `tap-core-0.0.2/pyproject.toml` & `tap-core-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tap-core-0.0.2/setup.cfg` & `tap-core-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,14 @@
 	Bug Tracker = https://gitlab.com/singer-core/target-core/issues/service_desk
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.9
-install_requires = 
-	singer-python==5.12.2
-	aiohttp==3.8.1
 include_package_data = True
 platforms = any
 
 [options.entry_points]
 console_scripts = 
 	tap-core = tap:main
```

### Comparing `tap-core-0.0.2/src/tap/api/__init__.py` & `tap-core-0.0.3/src/tap/api/sync.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 from asyncio import run, shield, Condition, gather
 
 from singer import (
     Catalog,
     set_currently_syncing,
     write_state,
     job_timer,
-    utils,
-    get_logger)
+    utils)
 
-from .client import Client
-
-LOGGER = get_logger()
+from .client import Client, LOGGER
+from .discovery import discover
 
 CONFIG_KEYS_REQUIRED: Set[str] = {
     'url'
 }
 
 
 def job_stream_timer(wrapped: Callable) -> Callable:
@@ -26,46 +24,46 @@
     async def wrapper(*args: Optional[Any], **kwargs: Optional[Any]) -> None:
         with job_timer(getattr(args[0], 'tap_stream_id', None) if len(args) > 1 else wrapped.__name__):
             return await wrapped(*args, **kwargs)
 
     return wrapper
 
 
-def discover(streams: Iterable) -> Catalog:
-    catalog: Catalog = Catalog([])
-
-    for stream in streams:
-        catalog.streams.append(stream.catalog_entry)
-
-    return catalog
-
-
 class Extractor:
 
     def __init__(self,
                  config: Dict = {},
                  streams: Iterable = [],
                  state: Dict = {},
                  catalog: Catalog = None,
                  client: type[Client] = Client) -> None:
         self.config: Dict[str, Any] = config
         self.state: Dict[str, Any] = state
         self.client: type[Client] = client
+        # self._client: Client = client(config)
+        self._condition: Condition = Condition()
+        self._currently_syncing: set = set()
 
         # NOTE: Discovering if No Catalog provided.
         self.catalog: Catalog = catalog or discover(streams)
 
         # NOTE: inherit `selected` from the catalog
         selected: set = {s.tap_stream_id for s in self.catalog.get_selected_streams(self.state)}
 
         self.streams: Dict[str, Any] = {
             stream.catalog_entry.tap_stream_id: stream
             for stream in streams
             if stream.catalog_entry.tap_stream_id in selected}
 
+        # # _client: Client = client(config)
+        # for stream in streams:
+        #     # stream._client = _client
+        #     stream._condition = self._condition
+        #     stream._currently_syncing = self._currently_syncing
+
         # self.streams = streams
         # self.streams: dict = {}
         # children: set = set()
         # for stream in streams:
         #     if stream.catalog_entry.tap_stream_id in selected:
         #         if stream.parent.get('tap_stream_id') is None:
         #             self.streams[stream.catalog_entry.tap_stream_id] = stream
@@ -77,68 +75,39 @@
         #         and stream.catalog_entry.tap_stream_id not in self.streams[stream.parent.get('tap_stream_id')].children:
         #         self.streams[stream.parent.get('tap_stream_id')].children.add(stream)
 
     @job_stream_timer
     async def get_streams(self) -> None:
 
         async with self.client(self.config) as self._client:
-            self._condition: Condition = Condition()
-            self._currently_syncing: set = set()
+            # self._condition: Condition = Condition()
+            # self._currently_syncing: set = set()
 
             await gather(*{
                 shield(stream.get_stream(self))
                 for stream in self.streams.values()
                 if stream.parent.get('tap_stream_id') is None})
 
         set_currently_syncing(self.state, None)
         write_state(self.state)
 
     def run(self) -> None:
 
         run(self.get_streams())
 
 
-def set_streams(config: Dict = {}, schemas_dir: Path = None) -> Iterable:
+def set_streams(config: Dict = {}, schemas_dir: Optional[Path] = None) -> Iterable:
 
     return []
 
 
-async def sync(schemas_dir: Path = None, set_streams: Callable = set_streams, config_keys_required: Set[str] = CONFIG_KEYS_REQUIRED) -> None:
+async def sync(schemas_dir: Optional[Path] = None, set_streams: Callable = set_streams, config_keys_required: Set[str] = CONFIG_KEYS_REQUIRED) -> None:
     try:
         args = utils.parse_args(config_keys_required)
 
         if args.discover:
             Extractor(args.config, set_streams(config=args.config, schemas_dir=schemas_dir)).catalog.dump()
         else:
             await Extractor(args.config, set_streams(config=args.config, schemas_dir=schemas_dir), args.state, args.catalog).get_streams()
     except Exception as e:
         LOGGER.critical(e)
         raise e
-
-
-def main(schemas_dir: Path = None, set_streams: Callable = set_streams, config_keys_required: Set[str] = CONFIG_KEYS_REQUIRED) -> None:
-    run(sync(schemas_dir, set_streams, config_keys_required))
-
-
-# def cli(*,
-#         config: str = 'config.json',
-#         discover: str = None,
-#         catalog: str = 'catalog.json',
-#         state: str = 'state.json'
-#         schemas_dir: str = None
-#     ) -> Extractor:
-
-#     LOGGER.setLevel(LEVELS_MAPPING.get(log_level))
-#     with open(config) as config_io, open(catalog) as catalog_io, open(state) as state_io:
-#         config_json = json.load(config_io)
-#         catalog_json = json.load(catalog_io)
-#         state_json = json.load(state_io)
-
-#     streams: Dict = set_streams(config_json)
-
-#     return Extractor(
-#         config=config_json,
-#         streams=streams,
-#         state=state_json,
-#         catalog=catalog_json,
-#         schemas_dir=schemas_dir
-#     )
```

### Comparing `tap-core-0.0.2/src/tap/api/client.py` & `tap-core-0.0.3/src/tap/api/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from typing import Any, Awaitable, Callable, Collection, Deque, Dict, Iterable, List, Optional, Type
+from typing import Any, Callable, Collection, Deque, Dict, Iterable, List, Optional, Type
 from os.path import join
 from decimal import Decimal
 import json
 from datetime import datetime, timedelta, timezone
+# from time import time
 from collections import deque
+# from functools import wraps
 from types import TracebackType
 from asyncio import Condition, sleep
 
 from aiohttp.web_exceptions import HTTPError
 from aiohttp import ClientSession, ClientResponse, BasicAuth, ClientResponseError, ClientError, TCPConnector
 import backoff
 from singer import metrics, http_request_timer, get_logger
@@ -84,16 +86,16 @@
     async def __aenter__(self) -> Any:
         await self.acquire()
         return self
 
     async def __aexit__(self,
                         exc_type: Optional[Type[BaseException]],
                         exc_value: Optional[BaseException],
-                        traceback: Optional[TracebackType]) -> Awaitable[Optional[bool]]:
-        pass
+                        traceback: Optional[TracebackType]) -> bool:
+        return False
 
     async def acquire(self) -> None:
         now: datetime = datetime.now(timezone.utc)
         while self._reset_logs:
             async with self._condition:
                 now = self.flush()
             if len(self._reset_logs) < self._rate_limit:
@@ -115,14 +117,36 @@
     def flush(self) -> datetime:
         while self._reset_logs and datetime.now(timezone.utc) > self._reset_logs[0]:
             self._reset_logs.popleft()
 
         return datetime.now(timezone.utc)
 
 
+# def ratelimit(limit: int, every: float):
+
+#     def limitdecorator(func):
+#         logs: deque = deque()
+
+#         @wraps(func)
+#         async def new_func(*args, **kwargs):
+#             if len(logs) >= limit:
+#                 # before: time = logs.pop()
+#                 # now: time = time()
+#                 sleep_duration: float = every - (time() - logs.pop())
+#                 if sleep_duration > 0:
+#                     await sleep(sleep_duration)
+
+#             logs.appendleft(time())
+#             return await func(*args, **kwargs)
+
+#         return new_func
+
+#     return limitdecorator
+
+
 # class RateLimitQuota:
 
 #     def __init__(self, header: str = HEADER_RATE_LIMIT_REMAINING) -> None:
 #         self.header = header
 
 #     def __iter__(self) -> Any:
 #         return self
@@ -146,93 +170,127 @@
 
     def is_status(error: ClientResponseError) -> bool:
         return bool(getattr(error, 'status', None) and error.status not in status and error.status < 500)
 
     return is_status
 
 
-def raise_for_status(response: ClientResponse, full_url: str = None, ignore_status: Collection = []) -> None:
+def raise_for_status(response: ClientResponse, full_url: Optional[str] = None, ignore_status: Collection = []) -> None:
 
     try:
         response.raise_for_status()
     except (HTTPError, ConnectionError, ClientResponseError) as error:
         LOGGER.error(
             'API Client: %s', json.dumps({
                 'type': 'HTTP response', 'status': response.status, 'url': full_url, 'ignore_status': ignore_status,
                 'message': RESPONSE_STATUS.get(response.status, {}).get('message', response.reason)}))
         if response.status not in set(ignore_status) | {200, 422}:
             raise error
 
         # raise APIError(str(error)) from None
 
 
+def _retry_pattern() -> Callable:
+    return backoff.on_exception(
+        backoff.expo,
+        (json.decoder.JSONDecodeError, ClientResponseError, ClientError),
+        factor=3,
+        giveup=is_missing_status([404, 429]),
+        max_tries=5,
+        logger=LOGGER
+    )
+
+
 class Client:
 
     def __init__(self, config: Dict) -> None:
+        self.config: Dict = config
         self.url: str = config.get('url', '')
-        self.headers = {'Accept': 'application/json'} | config.get('headers', {})
-        self._auth = BasicAuth(config.get('login'), config.get('password', '')) if config.get('login') else None
+        self.headers: Dict[str, Any] = {'Accept': 'application/json'} | config.get('headers', {})
+        self._auth: Optional[BasicAuth] = BasicAuth(config.get('login'), config.get('password', '')) if config.get('login') else None
 
         # NOTE: Allowed 300 requests per minute (5 requests per second), with occasional bursts of up to 20 requests at a time.
         self._throttler: Throttler = Throttler(config.get('rate_limit', 5), config.get('rate_period', 1.0))
+        self.connect()
         LOGGER.debug('API Client: Throttler %s', json.dumps({'rate_limit': self._throttler._rate_limit, 'rate_period': self._throttler._period}))
 
     async def __aenter__(self) -> Any:
-        return self.connect()
+        return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_value: Optional[BaseException],
         traceback: Optional[TracebackType]
     ) -> None:
         await self.close()
 
     def connect(self) -> Any:
+        # timeout_seconds: int = self.config.get('login', 99)
+        # session_timeout: ClientTimeout = ClientTimeout(total=None, sock_connect=timeout_seconds, sock_read=timeout_seconds)
         self.session = ClientSession(
             # NOTE: overwrite the default connector to customise the default connection settings applied to the queries
             connector=TCPConnector(
                 # NOTE: max concurrent connections to the end point. 0 by default
                 # limit_per_host=0,
                 # NOTE: limit on the client connections total count. 100 by default
                 # limit=limit_connections_count,
                 # NOTE: live connection duration. 30 by default
                 # keepalive_timeout=30
             ),
             auth=self._auth,
+            headers=self.headers,
+            # timeout=session_timeout,
             connector_owner=True)
         LOGGER.debug('API Client: %s', json.dumps({'message': 'API connected'}))
         return self
 
     async def close(self) -> None:
         await self.session.close()
 
-    @backoff.on_exception(
-        backoff.expo,
-        (json.decoder.JSONDecodeError, ClientResponseError, ClientError),
-        factor=3,
-        giveup=is_missing_status([404, 429]),
-        max_tries=5,
-        logger=LOGGER
-    )  # type: ignore
+    @_retry_pattern()
     # @backoff.on_exception(RateLimitQuota, ClientResponseError, jitter=None, max_tries=5, logger=LOGGER)  # type: ignore
-    async def get(self, *args: Optional[Any], **kwargs: Dict) -> Dict:
+    async def get(self, *args: Optional[Any], **kwargs: Dict) -> Iterable:
         path: str = str(args[0])
         full_url: str = join(self.url, str(kwargs.pop('endpoint', path)))
         LOGGER.debug('API Client GET: %s', json.dumps({'message': 'HTTP Request', 'url': full_url}))
 
-        async with self._throttler, self.session.request('get', full_url, headers=self.headers, params=kwargs.pop('filters', {})) as response:
+        async with self._throttler, self.session.get(full_url, params=kwargs.pop('params', {})) as response:
             with http_request_timer(path) as timer:
                 if response.status != 200:
                     raise_for_status(response, full_url=full_url, ignore_status=kwargs['ignore_status'] if 'ignore_status' in kwargs else [])
                     timer.tags[metrics.Tag.http_status_code] = response.status
-                    return {}
                 else:
                     return json.loads(await response.text(), parse_float=Decimal)
                     # NOTE: Alternative return await response.json(loads=partial(json.loads, parse_float=Decimal))
+        return {}
+
+    @_retry_pattern()
+    async def post(self, *args: Optional[Any], **kwargs: Dict) -> Iterable:
+        path: str = str(args[0])
+        full_url: str = join(self.url, str(kwargs.pop('endpoint', path)))
+        LOGGER.debug('API Client POST: %s', json.dumps({'message': 'HTTP Request', 'url': full_url}))
+
+        async with self._throttler, self.session.post(
+            full_url,
+            params=kwargs.pop('params', {}),
+            # headers=self.headers,
+            # timeout=9,
+            data=json.dumps(kwargs.pop('data', {}))
+        ) as response:
+            with http_request_timer(path) as timer:
+                if response.status != 200:
+                    raise_for_status(response, full_url=full_url, ignore_status=kwargs['ignore_status'] if 'ignore_status' in kwargs else [])
+                    timer.tags[metrics.Tag.http_status_code] = response.status
+                else:
+                    return json.loads(await response.text(), parse_float=Decimal)
+                    # NOTE: Alternative return await response.json(loads=partial(json.loads, parse_float=Decimal))
+        return {}
 
     async def get_records(self, tap_stream_id: str, format_response: Callable, *args: Optional[Any], **kwargs: Dict) -> Iterable:
 
-        response = await self.get(tap_stream_id, *args, **kwargs),
-        records = format_response(response) if callable(format_response) else []
+        def response_list(r: Any) -> tuple:
+            return (r,) if isinstance(r, dict) else r
+
+        response = response_list(await self.get(tap_stream_id, *args, **kwargs))
 
-        return records
+        return format_response(response) if callable(format_response) else response
```

### Comparing `tap-core-0.0.2/src/tap/api/stream.py` & `tap-core-0.0.3/src/tap/api/stream.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 import datetime
-from datetime import timezone
-import time
 from copy import deepcopy
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional
+from typing import Any, Callable, Dict, Iterable, List, Optional
 from functools import partial, reduce
-from asyncio import shield, to_thread, gather
+from asyncio import shield, to_thread, gather  # , Condition
 
 from singer import (
     Transformer,
     CatalogEntry,
     Schema,
-    load_json,
-    resolve_schema_references,
     get_bookmark,
     write_bookmark,
     get_offset,
     set_offset,
     clear_offset,
     set_currently_syncing,
     record_counter,
@@ -25,75 +21,63 @@
     write_version,
     RecordMessage,
     write_message,
     write_state,
     get_logger)
 from singer.metadata import get_standard_metadata, to_map, write, to_list
 
-from . import Extractor, job_stream_timer
+# from .client import Client
+from .sync import Extractor, job_stream_timer
+from .schema import load_schema
+from .transform import format_response
 
 LOGGER = get_logger()
 
 
-def load_schema(tap_stream_id: str, schemas_dir: Path = None) -> Dict:
-
-    schema: Dict[str, Any] = load_json((schemas_dir or Path(__file__).parent.resolve() / 'schemas') / f'{tap_stream_id}.json')
-
-    return resolve_schema_references(schema, {
-        stream_id: load_schema(stream_id)
-        for stream_id in schema.pop('tap_schema_dependencies', [])})
-
-
-def format_response(response: List, params: Dict = {}) -> Any:
-    return [r for r in response]
-
-
-def format_response_replication(response: List, params: Dict, replication_value: int = 0) -> Any:
-    return [r for i in response
-            for r in i.get(params.get('path'), {}).values()
-            if r.get(params.get('replication_key'), 2e9) > replication_value]
-
-
-def format_response_sub_stream(response: List, params: Dict, replication_record: Dict = {}, replication_value: int = 0) -> List:
-    # TODO: filter out unbounded preceding
-    return [replication_record | r
-            for i in response
-            for r in i.get(params.get('path'), i)
-            if (replication_record | r).get(params.get('replication_key'), 2e9) > replication_value]
-
-
 class AbstractStream:
 
+    # _client: Optional[Client] = None
+    # _condition: Optional[Condition] = None
+    # _currently_syncing: Optional[set] = None
+
     def __init__(
         self,
         tap_stream_id: str,
         config: Dict = {},
-        schemas_dir: Path = None,
+        schemas_dir: Optional[Path] = None,
         key_properties: List[str] = [],
         replication_method: str = 'FULL_TABLE',
-        replication_key: str = None,
+        replication_key: Optional[str] = None,
         is_view: bool = False,
-        database: str = None,
-        table: str = None,
-        row_count: int = None,
-        stream: str = None,
-        stream_alias: str = None,
+        database: Optional[str] = None,
+        table: Optional[str] = None,
+        row_count: Optional[int] = None,
+        stream: Optional[str] = None,
+        stream_alias: Optional[str] = None,
         format_response_function: Callable = format_response,
         format_response_params: Dict[str, Any] = {},
         parent: Dict[str, Any] = {},
-        children: List = [],
+        # children: List = [],
         params: Dict[str, Any] = {}
     ) -> None:
         self.format_response_function: Callable = format_response_function
         self.format_response_params: Dict[str, Any] = format_response_params
+        # self.format_response_params: Dict[str, Any] = (
+        #     {'replication_key': replication_key} if replication_method == 'INCREMENTAL' else {}) | format_response_params
         self.parent: Dict[str, Any] = parent
-        self.children: List = children
+        # self.children: List = children
         self.params: Dict[str, Any] = params
-
-        self.schema: Dict[str, Any] = load_schema(tap_stream_id, schemas_dir)
+        self.start_date: Optional[datetime.datetime] = datetime.datetime.strptime(config['start_date'], '%Y-%m-%dT%H:%M:%SZ') \
+            if 'start_date' in config else None
+        self.user_agent: Optional[str] = config.get('user_agent')
+
+        schemas_dir = schemas_dir or Path(__file__).resolve().with_name('schemas')
+        self.schema: Dict[str, Any] = load_schema(tap_stream_id, schemas_dir) if schemas_dir.joinpath(tap_stream_id + '.json').exists() \
+            else load_schema(stream or tap_stream_id, schemas_dir) if schemas_dir.joinpath(str(stream) + '.json').exists() \
+            else load_schema(stream_alias or tap_stream_id, schemas_dir)
 
         metadata: List[Any] = get_standard_metadata(
             schema=self.schema,
             schema_name=tap_stream_id,
             key_properties=key_properties,
             valid_replication_keys=replication_key,
             replication_method=replication_method)
@@ -101,15 +85,15 @@
         self.catalog_entry: CatalogEntry = CatalogEntry(
             tap_stream_id=tap_stream_id,
             stream=stream or tap_stream_id,
             stream_alias=stream_alias or stream or tap_stream_id,
             key_properties=key_properties or [],
             schema=Schema.from_dict(self.schema),
             replication_key=replication_key,
-            replication_method=replication_method or 'FULL_TABLE',
+            replication_method=replication_method,
             is_view=is_view,
             database=database,
             table=table,
             row_count=row_count,
             metadata=to_list(write(to_map(metadata), (), 'selected', True))
             if tap_stream_id in config.get('selected', []) else metadata)
 
@@ -123,109 +107,121 @@
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
             setattr(result, k, deepcopy(v, memo))
         return result
 
+    @job_stream_timer
+    async def get_stream(self, extractor: Extractor, *args: Optional[Any], **kwargs: Dict) -> None:
+        raise NotImplementedError("Child classes of AbstractStream require `get_stream` implementation")
+
     async def write_schema(self, extractor: Extractor) -> None:
 
         extractor._currently_syncing.add(self.catalog_entry.tap_stream_id)
 
         await to_thread(write_schema,
                         self.catalog_entry.tap_stream_id,
                         self.catalog_entry.schema.to_dict(),
                         self.catalog_entry.key_properties,
                         bookmark_properties=self.catalog_entry.replication_key,
                         stream_alias=self.catalog_entry.stream_alias)
 
         # NOTE: ACTIVATE_VERSION Singer extension support https://github.com/meltano/meltano/issues/2463
-        self.version: int = get_bookmark(extractor.state, self.catalog_entry.tap_stream_id, 'version') or int(time.time() * 1000) \
+        current_timestamp: int = int(datetime.datetime.now().astimezone(datetime.timezone.utc).timestamp() * 1000)
+        self.version: int = get_bookmark(extractor.state, self.catalog_entry.tap_stream_id, 'version', current_timestamp) \
             if self.catalog_entry.replication_key \
-            else int(time.time() * 1000)
+            else current_timestamp
 
         is_stream_bookmarked: bool = extractor.state.get('bookmarks', {}).get(self.catalog_entry.tap_stream_id) is not None
         if self.catalog_entry.replication_key or not is_stream_bookmarked:
             write_bookmark(extractor.state, self.catalog_entry.tap_stream_id, 'version', self.version)
 
         if self.catalog_entry.replication_method == 'FULL_TABLE':
             await to_thread(write_version, self.catalog_entry.stream, self.version)
 
-    async def write_records(self, extractor: Extractor, records: List) -> None:
+    async def write_records(self, extractor: Extractor, records: Iterable[Any]) -> None:
         LOGGER.info('Syncing stream: %s', self.catalog_entry.tap_stream_id)
 
         set_currently_syncing(extractor.state, self.catalog_entry.tap_stream_id)
         await to_thread(write_state, extractor.state)
 
         if self.catalog_entry.tap_stream_id not in extractor._currently_syncing:
             await self.write_schema(extractor)
 
-        for record in records:
-            with Transformer() as t:
+        with Transformer() as t, record_counter(self.catalog_entry.tap_stream_id) as counter:
+            for record in records:
                 await to_thread(write_message,
                                 RecordMessage(
                                     stream=(self.catalog_entry.stream_alias or self.catalog_entry.tap_stream_id),
                                     record=t.transform(record, self.catalog_entry.schema.to_dict(), to_map(self.catalog_entry.metadata)),
-                                    time_extracted=datetime.datetime.now(timezone.utc),
+                                    time_extracted=datetime.datetime.now().astimezone(datetime.timezone.utc),
                                     version=self.version))
-
-        with record_counter(self.catalog_entry.tap_stream_id) as counter:
-            counter.increment(len(records))
+                counter.increment(1)
 
 
-class StreamChild(AbstractStream):
+class SubStream(AbstractStream):
 
     @job_stream_timer
     async def get_stream(self, extractor: Extractor, parent_records: list) -> None:
-        parent_tap_stream_id: Optional[str] = self.parent.get('tap_stream_id')
+        replication_key: str = self.catalog_entry.replication_key
+        replication_value = get_bookmark(extractor.state, self.catalog_entry.tap_stream_id, replication_key, 0)
         parent_key_properties: List[str] = self.parent.get('key_properties', [])
-        parent_replication_key: str = extractor.catalog.get_stream(parent_tap_stream_id).replication_key
-        # parent_replication_value = get_bookmark(extractor.state, parent_tap_stream_id, parent_replication_key, 0)
         endpoint: str = self.params.get('endpoint', '')
 
-        records: list = [record for records in await gather(*[
+        records_raw: list = [record for records in await gather(*[
             shield(extractor._client.get_records(
                 self.catalog_entry.tap_stream_id,
                 **(self.params | {
                     'endpoint': endpoint.format(**{k: parent_record.get(k) for k in parent_key_properties}),
-                    'format_response': ({'function': self.format_response_function, 'params': self.format_response_params} | {'function': partial(
-                        self.format_response_function,
-                        params=self.format_response_params,
-                        replication_record={parent_replication_key: parent_record.get(parent_replication_key)}
-                        if parent_record.get(parent_replication_key) else {})})['function']})))
+                    'format_response': ({
+                        'params': self.format_response_params,
+                        'function': partial(
+                            self.format_response_function,
+                            params=self.format_response_params,
+                            replication_value=replication_value,
+                            parent_record=parent_record)})['function']})))
             for parent_record in parent_records
             if reduce(lambda x, k: x and parent_record.get(k) is not None, parent_key_properties, True)])
             if records is not None
             for record in records]
 
+        records = (r for r in records_raw if int(r.get(replication_key, 2e9)) > replication_value) \
+            if self.catalog_entry.replication_method == 'INCREMENTAL' \
+            else records_raw
+
         async with extractor._condition:
             await self.write_records(extractor, records)
             # if extractor.catalog.get_stream(self.tap_stream_id).replication_method == 'FULL_TABLE':
             reset_stream(extractor.state, self.catalog_entry.tap_stream_id)
             await to_thread(write_state, extractor.state)
 
 
 class Stream(AbstractStream):
 
     @job_stream_timer
     async def get_stream(self, extractor: Extractor, *args: Optional[Any], **kwargs: Dict) -> None:
         params: Dict[str, Any] = deepcopy(self.params)
         replication_key: str = self.catalog_entry.replication_key
         replication_value = get_bookmark(extractor.state, self.catalog_entry.tap_stream_id, replication_key, 0)
-        filters: Dict[str, Any] = params.pop('filters', {}) | ({
-            replication_key: get_bookmark(extractor.state, self.catalog_entry.tap_stream_id, replication_key, 0)} if replication_key else {})
-        format_response_params: Dict[str, Any] = {'function': self.format_response_function, 'params': self.format_response_params} | {
+        filters: Dict[str, Any] = params.pop('params', {}) | ({
+            replication_key: replication_value} if replication_key else {})
+        format_response_params: Dict[str, Any] = {
+            'params': self.format_response_params,
             'function': partial(
                 self.format_response_function,
                 params=self.format_response_params,
                 replication_value=replication_value)
         } | params.pop('format_response', {})
 
-        records: list = await extractor._client.get_records(
-            self.catalog_entry.tap_stream_id, filters=filters, format_response=format_response_params['function'], *args, **params)
+        records_raw: list = await extractor._client.get_records(
+            self.catalog_entry.tap_stream_id, params=filters, format_response=format_response_params['function'], *args, **params)
+        records = [r for r in records_raw if r.get(replication_key, 2e9) > replication_value] \
+            if self.catalog_entry.replication_method == 'INCREMENTAL' \
+            else records_raw
 
         async with extractor._condition:
             await self.write_records(extractor, records)
 
             if replication_key is not None and any(records):
                 write_bookmark(
                     extractor.state, self.catalog_entry.tap_stream_id, replication_key,
@@ -246,29 +242,35 @@
 class StreamPages(AbstractStream):
 
     @job_stream_timer
     async def get_stream(self, extractor: Extractor, *args: Optional[Any], **kwargs: Dict) -> None:
         params: Dict[str, Any] = deepcopy(self.params)
         replication_key: str = self.catalog_entry.replication_key
         replication_value = get_bookmark(extractor.state, self.catalog_entry.tap_stream_id, replication_key, 0)
-        format_response: Dict[str, Any] = {'function': self.format_response_function, 'params': self.format_response_params} | {
+        # replication_value = get_bookmark(extractor.state, self.catalog_entry.tap_stream_id, replication_key, int(self.start_date.timestamp()))
+        # LOGGER.info({'format_response_params': self.format_response_params, 'replication_value': replication_value})
+        format_response: Dict[str, Any] = {
+            'params': self.format_response_params,
             'function': partial(
                 self.format_response_function,
                 params=self.format_response_params,
                 replication_value=replication_value)
         } | params.pop('format_response', {})
         offset_key = self.params.get('offset_key')
         limit_key = self.params.get('limit_key')
         curr_offset = get_offset(extractor.state, self.catalog_entry.tap_stream_id, {}).get('offset', 0)
-        filters = {offset_key: curr_offset} | params.pop('filters', {}) | ({
-            replication_key: get_bookmark(extractor.state, self.catalog_entry.tap_stream_id, replication_key, 0)} if replication_key else {})
+        filters = {offset_key: curr_offset} | params.pop('params', {}) | ({
+            replication_key: replication_value} if replication_key else {})
 
         while any(filters):
-            response = await extractor._client.get(self.catalog_entry.tap_stream_id, filters=filters, *args, **params),
-            records = format_response['function'](response) if callable(format_response['function']) else []
+            response = await extractor._client.get(self.catalog_entry.tap_stream_id, params=filters, *args, **params),
+            records_raw = format_response['function'](response) if callable(format_response['function']) else []
+            records = [r for r in records_raw if r.get(replication_key, 2e9) > replication_value] \
+                if self.catalog_entry.replication_method == 'INCREMENTAL' \
+                else records_raw
 
             async with extractor._condition:
                 set_offset(extractor.state, self.catalog_entry.tap_stream_id, 'offset', filters[offset_key])
                 await self.write_records(extractor, records)
                 if replication_key and records:
                     write_bookmark(
                         extractor.state,
@@ -280,34 +282,35 @@
 
             for sub_stream_tap_stream_id, _ in filter(
                 lambda s: s[1].parent.get('tap_stream_id') == self.catalog_entry.tap_stream_id,
                     extractor.streams.items()):
                 await extractor.streams[sub_stream_tap_stream_id].get_stream(extractor, records)
 
             # if any(records) and len(records) >= filters[limit_key]:
-            if len(records) > 0:
+            if len(records_raw) > 0:
                 filters[offset_key] += filters[limit_key]
             else:
                 filters = {}
 
-        await to_thread(write_version, self.catalog_entry.stream, self.version)
+        if self.catalog_entry.replication_method == 'FULL_TABLE':
+            await to_thread(write_version, self.catalog_entry.stream, self.version)
 
         # if extractor.catalog.get_stream(self.tap_stream_id).replication_method == 'FULL_TABLE':
         async with extractor._condition:
             clear_offset(extractor.state, self.catalog_entry.tap_stream_id)
 
     # async def get_cursors(self, curr_offset: int = 0, *args: Optional[Any], **kwargs: Dict) -> AsyncGenerator:
     #     format_response = kwargs['format_response']
     #     limit_key = kwargs['limit_key'] if 'limit_key' in kwargs else None
     #     next_token_key = kwargs['next_token_key'] if 'next_token_key' in kwargs else None
-    #     params: Dict = {limit_key: self.page_limit} | kwargs.pop('filters', {})
+    #     params: Dict = {limit_key: self.page_limit} | kwargs.pop('params', {})
     #     filters: Dict = params
 
     #     while any(filters):
-    #         response = await self.get(tap_stream_id, filters=filters, *args, **kwargs),
+    #         response = await self.get(tap_stream_id, params=filters, *args, **kwargs),
     #         records = format_response['function'](response, format_response['params']) if callable(format_response['function']) else []
 
     #         yield curr_offset, records
 
     #         if len(records) > 0 and response.get(next_token_key, None) is not None:  # type: ignore
     #             filters = params | {next_token_key: response[next_token_key]}  # type: ignore
     #             curr_offset += filters[limit_key]
```

### Comparing `tap-core-0.0.2/src/tap_core.egg-info/PKG-INFO` & `tap-core-0.0.3/src/tap_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-core
-Version: 0.0.2
+Version: 0.0.3
 Summary: Singer.io Tap Core features
 Home-page: https://gitlab.com/singer-core/tap-core
 Author: Eddy ∆
 Author-email: edrdelta@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://singer-core.gitlab.io/tap-core
 Project-URL: Releases, https://gitlab.com/singer-core/tap-core/-/releases
@@ -25,21 +25,22 @@
 Provides-Extra: dist
 Provides-Extra: deploy
 Provides-Extra: docs
 License-File: LICENSE
 
 # Tap Core
 
-[![Pypi - License](https://img.shields.io/pypi/l/tap-core?color=yellow)](https://opensource.org/licenses/Apache-2.0)
+[![GitLab - License](https://img.shields.io/gitlab/license/singer-core/tap-core?color=blue)](https://gitlab.com/singer-core/tap-core/-/blob/main/LICENSE)
 [![Python package builder](https://gitlab.com/singer-core/tap-core/badges/main/pipeline.svg)](https://gitlab.com/singer-core/tap-core/pipelines)
 [![Coverage](https://codecov.io/gl/singer-core/tap-core/branch/main/graph/badge.svg?token=LBNSKSY3O9)](https://codecov.io/gl/singer-core/tap-core)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tap-core.svg)](https://pypi.org/project/tap-core)
 [![PyPI version](https://badge.fury.io/py/tap-core.svg)](https://badge.fury.io/py/tap-core)
 [![PyPi project installs](https://img.shields.io/pypi/dm/tap-core.svg?maxAge=2592000&label=installs&color=%2327B1FF)](https://pypistats.org/packages/tap-core)
 
+<!-- [![Pypi - License](https://img.shields.io/pypi/l/tap-core?color=yellow)](https://opensource.org/licenses/Apache-2.0) -->
 <!-- [![Coverage](https://gitlab.com/singer-core/tap-core/badges/main/coverage.svg)](https://gitlab.com/singer-core/tap-core/-/graphs/main/charts) -->
 <!-- [![Documentation Status](https://readthedocs.org/projects/tap-core/badge/?version=latest)](https://singer-core.gitlab.io/tap-core/en/latest/?badge=latest) -->
 <!-- [![Latest Release](https://gitlab.com/singer-core/tap-core/-/badges/release.svg)](https://gitlab.com/singer-core/tap-core/-/releases) -->
 
 [**Singer**](https://www.singer.io/) tap core provide safe tools to easily build new `taps` following the [*Singer spec*](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md) *convention* and *protocol*.
 
 ## How to use it
```


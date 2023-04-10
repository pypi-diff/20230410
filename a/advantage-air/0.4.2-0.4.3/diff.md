# Comparing `tmp/advantage_air-0.4.2.tar.gz` & `tmp/advantage_air-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advantage_air-0.4.2.tar", last modified: Sun Dec 11 22:30:57 2022, max compression
+gzip compressed data, was "advantage_air-0.4.3.tar", last modified: Mon Apr 10 03:31:53 2023, max compression
```

## Comparing `advantage_air-0.4.2.tar` & `advantage_air-0.4.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 22:30:57.289454 advantage_air-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2022-12-11 22:30:46.000000 advantage_air-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2022-12-11 22:30:57.289454 advantage_air-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      630 2022-12-11 22:30:46.000000 advantage_air-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 22:30:57.289454 advantage_air-0.4.2/advantage_air/
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2022-12-11 22:30:46.000000 advantage_air-0.4.2/advantage_air/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 22:30:57.289454 advantage_air-0.4.2/advantage_air.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2022-12-11 22:30:57.000000 advantage_air-0.4.2/advantage_air.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      236 2022-12-11 22:30:57.000000 advantage_air-0.4.2/advantage_air.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-11 22:30:57.000000 advantage_air-0.4.2/advantage_air.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-11 22:30:57.000000 advantage_air-0.4.2/advantage_air.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-11 22:30:57.000000 advantage_air-0.4.2/advantage_air.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-11 22:30:57.289454 advantage_air-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      699 2022-12-11 22:30:46.000000 advantage_air-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:31:53.667443 advantage_air-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-10 03:31:44.000000 advantage_air-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-10 03:31:53.667443 advantage_air-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-10 03:31:44.000000 advantage_air-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:31:53.667443 advantage_air-0.4.3/advantage_air/
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-10 03:31:44.000000 advantage_air-0.4.3/advantage_air/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:31:53.667443 advantage_air-0.4.3/advantage_air.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-10 03:31:53.000000 advantage_air-0.4.3/advantage_air.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-10 03:31:53.000000 advantage_air-0.4.3/advantage_air.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 03:31:53.000000 advantage_air-0.4.3/advantage_air.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 03:31:53.000000 advantage_air-0.4.3/advantage_air.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-10 03:31:53.000000 advantage_air-0.4.3/advantage_air.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 03:31:53.667443 advantage_air-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-10 03:31:44.000000 advantage_air-0.4.3/setup.py
```

### Comparing `advantage_air-0.4.2/LICENSE` & `advantage_air-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `advantage_air-0.4.2/advantage_air/__init__.py` & `advantage_air-0.4.3/advantage_air/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import json
 import asyncio
 import aiohttp
 import collections.abc
 
+ON = "ON"
+OFF = "OFF"
 
 def update(d, u):
     for k, v in u.items():
         if isinstance(v, collections.abc.Mapping):
             d[k] = update(d.get(k, {}), v)
         else:
             d[k] = v
@@ -16,29 +18,28 @@
 class ApiError(Exception):
     """AdvantageAir Error"""
 
 
 class advantage_air:
     """AdvantageAir Connection"""
 
-    def __init__(self, ip, port=2025, session=None, retry=5):
-
+    def __init__(self, ip: str, port: int=2025, session: aiohttp.ClientSession=None, retry: int=5):
         if session is None:
             session = aiohttp.ClientSession()
 
         self.ip = ip
         self.port = port
         self.session = session
         self.retry = retry
 
-        self.aircon = self.advantage_air_endpoint(ip, port, session, retry, "setAircon")
-        self.lights = self.advantage_air_endpoint(ip, port, session, retry, "setLights")
-        self.things = self.advantage_air_endpoint(ip, port, session, retry, "setThings")
+        self.aircon = self._aircon(ip, port, session, retry)
+        self.lights = self._lights(ip, port, session, retry)
+        self.things = self._things(ip, port, session, retry)
 
-    async def async_get(self, retry=None):
+    async def async_get(self, retry:int =None):
         retry = retry or self.retry
         data = {}
         count = 0
         error = None
         while count < retry:
             count += 1
             try:
@@ -67,25 +68,24 @@
                 break
 
             await asyncio.sleep(1)
         raise ApiError(
             f"No valid response after {count} failed attempt{['','s'][count>1]}. Last error was: {error}"
         )
 
-    class advantage_air_endpoint:
-        def __init__(self, ip, port, session, retry, endpoint):
+    class _endpoint:
+        def __init__(self, ip, port, session, retry) -> None:
             self.ip = ip
             self.port = port
             self.session = session
             self.retry = retry
-            self.endpoint = endpoint
             self.changes = {}
             self.lock = asyncio.Lock()
 
-        async def async_set(self, change):
+        async def async_update(self, change: dict[str, any]) -> bool:
             """Merge changes with queue and send when possible, returning True when done"""
 
             self.changes = update(self.changes, change)
             if self.lock.locked():
                 return False
             async with self.lock:
                 while self.changes:
@@ -115,7 +115,51 @@
                     except asyncio.TimeoutError:
                         raise ApiError("Connection timed out.")
                     except AssertionError:
                         raise ApiError("Response status not 200.")
                     except SyntaxError as err:
                         raise ApiError("Invalid response")
             return True
+
+    class _aircon(_endpoint):
+        """Aircon endpoint"""
+
+        endpoint = "setAircon"
+
+        async def async_update_ac(self, ac: str, body: dict) -> bool:
+            """Update an aircon"""
+            return await self.async_update({ac: {"info": body}})
+
+        async def async_update_zone(self, ac: str, zone: str, body: dict) -> bool:
+            """Update a zone"""
+            return await self.async_update({ac: {"zones": {zone: body}}})
+
+    class _lights(_endpoint):
+        """Lights endpoint"""
+
+        endpoint = "setLights"
+
+        async def async_update_state(self, id: str, state: str|bool) -> bool:
+            """Update a lights state"""
+            if state == True:
+                state = ON
+            elif state == False:
+                state = OFF
+            return await self.async_update({id: {"id": id, "state": state}})
+
+        async def async_update_value(self, id: str, value: int) -> bool:
+            """Update a lights state and value"""
+            return await self.async_update({id: {"id": id, "state": (ON if value > 0 else OFF), "value": value}})
+
+    class _things(_endpoint):
+        """Things endpoint"""
+
+        endpoint = "setThings"
+
+        async def async_update_value(self, id: str, value: int|bool) -> bool:
+            """Update a things state and value"""
+            if value == True:
+                value = 100
+            elif value == False:
+                value = 0
+                
+            return await self.async_update({id: {"id": id, "value": value}})
```

### Comparing `advantage_air-0.4.2/setup.py` & `advantage_air-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="advantage_air",
-    version="0.4.2",
+    version="0.4.3",
     author="Brett Adams",
     author_email="brett@ba.id.au",
     description="API helper for Advantage Air's MyAir and e-zone API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bre77/advantage_air",
     packages=setuptools.find_packages(),
```


# Comparing `tmp/mayalabs-0.0.6.tar.gz` & `tmp/mayalabs-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayalabs-0.0.6.tar", last modified: Tue Apr  4 13:12:52 2023, max compression
+gzip compressed data, was "mayalabs-0.0.7.tar", last modified: Mon Apr 10 16:44:37 2023, max compression
```

## Comparing `mayalabs-0.0.6.tar` & `mayalabs-0.0.7.tar`

### file list

```diff
@@ -1,34 +1,39 @@
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-04 13:12:52.153172 mayalabs-0.0.6/
--rw-r--r--   0 shubham    (501) staff       (20)     1054 2023-03-28 13:53:19.000000 mayalabs-0.0.6/LICENCE
--rw-r--r--   0 shubham    (501) staff       (20)     2997 2023-04-04 13:12:52.152564 mayalabs-0.0.6/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)     2572 2023-04-04 13:11:46.000000 mayalabs-0.0.6/README.md
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-04 13:12:52.146586 mayalabs-0.0.6/examples/
--rw-r--r--   0 shubham    (501) staff       (20)      169 2023-04-03 20:06:00.000000 mayalabs-0.0.6/examples/function.py
--rw-r--r--   0 shubham    (501) staff       (20)      414 2023-04-03 20:05:57.000000 mayalabs-0.0.6/examples/sql_test.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-04 13:12:52.148811 mayalabs-0.0.6/mayalabs/
--rw-r--r--   0 shubham    (501) staff       (20)      311 2023-04-04 10:35:40.000000 mayalabs-0.0.6/mayalabs/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     4356 2023-04-03 20:02:10.000000 mayalabs-0.0.6/mayalabs/cli.py
--rw-r--r--   0 shubham    (501) staff       (20)      269 2023-03-29 17:04:56.000000 mayalabs-0.0.6/mayalabs/exceptions.py
--rw-r--r--   0 shubham    (501) staff       (20)     5839 2023-04-04 11:16:57.000000 mayalabs-0.0.6/mayalabs/function.py
--rw-r--r--   0 shubham    (501) staff       (20)     1142 2023-04-04 11:16:57.000000 mayalabs-0.0.6/mayalabs/mayalabs.py
--rw-r--r--   0 shubham    (501) staff       (20)    15218 2023-04-04 11:16:57.000000 mayalabs-0.0.6/mayalabs/session.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-04 13:12:52.152363 mayalabs-0.0.6/mayalabs/utils/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2023-03-27 23:24:06.000000 mayalabs-0.0.6/mayalabs/utils/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     1111 2023-04-04 10:35:40.000000 mayalabs-0.0.6/mayalabs/utils/defaults.py
--rw-r--r--   0 shubham    (501) staff       (20)     5196 2023-03-27 23:24:06.000000 mayalabs-0.0.6/mayalabs/utils/general.py
--rw-r--r--   0 shubham    (501) staff       (20)     1434 2023-03-29 17:05:06.000000 mayalabs-0.0.6/mayalabs/utils/log.py
--rw-r--r--   0 shubham    (501) staff       (20)      202 2023-03-29 17:04:56.000000 mayalabs-0.0.6/mayalabs/utils/logging.py
--rw-r--r--   0 shubham    (501) staff       (20)     3973 2023-03-27 23:24:06.000000 mayalabs-0.0.6/mayalabs/utils/name_gen.py
--rw-r--r--   0 shubham    (501) staff       (20)     5589 2023-04-04 10:35:40.000000 mayalabs-0.0.6/mayalabs/utils/pac_engine.py
--rw-r--r--   0 shubham    (501) staff       (20)      628 2023-03-29 10:15:45.000000 mayalabs-0.0.6/mayalabs/utils/poll.py
--rw-r--r--   0 shubham    (501) staff       (20)     4296 2023-04-04 13:11:46.000000 mayalabs-0.0.6/mayalabs/utils/websocket.py
--rw-r--r--   0 shubham    (501) staff       (20)    16208 2023-04-04 13:11:46.000000 mayalabs-0.0.6/mayalabs/worker.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-04 13:12:52.150013 mayalabs-0.0.6/mayalabs.egg-info/
--rw-r--r--   0 shubham    (501) staff       (20)     2997 2023-04-04 13:12:52.000000 mayalabs-0.0.6/mayalabs.egg-info/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)      644 2023-04-04 13:12:52.000000 mayalabs-0.0.6/mayalabs.egg-info/SOURCES.txt
--rw-r--r--   0 shubham    (501) staff       (20)        1 2023-04-04 13:12:52.000000 mayalabs-0.0.6/mayalabs.egg-info/dependency_links.txt
--rw-r--r--   0 shubham    (501) staff       (20)       46 2023-04-04 13:12:52.000000 mayalabs-0.0.6/mayalabs.egg-info/entry_points.txt
--rw-r--r--   0 shubham    (501) staff       (20)       62 2023-04-04 13:12:52.000000 mayalabs-0.0.6/mayalabs.egg-info/requires.txt
--rw-r--r--   0 shubham    (501) staff       (20)       23 2023-04-04 13:12:52.000000 mayalabs-0.0.6/mayalabs.egg-info/top_level.txt
--rw-r--r--   0 shubham    (501) staff       (20)      777 2023-04-04 13:11:46.000000 mayalabs-0.0.6/pyproject.toml
--rw-r--r--   0 shubham    (501) staff       (20)       38 2023-04-04 13:12:52.153326 mayalabs-0.0.6/setup.cfg
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-10 16:44:37.628879 mayalabs-0.0.7/
+-rw-r--r--   0 shubham    (501) staff       (20)     1054 2023-03-28 13:53:19.000000 mayalabs-0.0.7/LICENCE
+-rw-r--r--   0 shubham    (501) staff       (20)     4204 2023-04-10 16:44:37.628670 mayalabs-0.0.7/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)     3758 2023-04-10 16:43:43.000000 mayalabs-0.0.7/README.md
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-10 16:44:37.622902 mayalabs-0.0.7/mayalabs/
+-rw-r--r--   0 shubham    (501) staff       (20)      364 2023-04-10 12:10:07.000000 mayalabs-0.0.7/mayalabs/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)     4356 2023-04-10 14:24:50.000000 mayalabs-0.0.7/mayalabs/cli.py
+-rw-r--r--   0 shubham    (501) staff       (20)      269 2023-03-29 17:04:56.000000 mayalabs-0.0.7/mayalabs/exceptions.py
+-rw-r--r--   0 shubham    (501) staff       (20)     5947 2023-04-10 15:50:57.000000 mayalabs-0.0.7/mayalabs/function.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1142 2023-04-06 10:29:10.000000 mayalabs-0.0.7/mayalabs/mayalabs.py
+-rw-r--r--   0 shubham    (501) staff       (20)    15585 2023-04-10 12:10:07.000000 mayalabs-0.0.7/mayalabs/session.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-10 16:44:37.627020 mayalabs-0.0.7/mayalabs/utils/
+-rw-r--r--   0 shubham    (501) staff       (20)        0 2023-03-27 23:24:06.000000 mayalabs-0.0.7/mayalabs/utils/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1249 2023-04-10 12:10:07.000000 mayalabs-0.0.7/mayalabs/utils/defaults.py
+-rw-r--r--   0 shubham    (501) staff       (20)     5196 2023-03-27 23:24:06.000000 mayalabs-0.0.7/mayalabs/utils/general.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1434 2023-03-29 17:05:06.000000 mayalabs-0.0.7/mayalabs/utils/log.py
+-rw-r--r--   0 shubham    (501) staff       (20)      202 2023-03-29 17:04:56.000000 mayalabs-0.0.7/mayalabs/utils/logging.py
+-rw-r--r--   0 shubham    (501) staff       (20)     3973 2023-03-27 23:24:06.000000 mayalabs-0.0.7/mayalabs/utils/name_gen.py
+-rw-r--r--   0 shubham    (501) staff       (20)     7923 2023-04-10 12:10:07.000000 mayalabs-0.0.7/mayalabs/utils/pac_engine.py
+-rw-r--r--   0 shubham    (501) staff       (20)      628 2023-03-29 10:15:45.000000 mayalabs-0.0.7/mayalabs/utils/poll.py
+-rw-r--r--   0 shubham    (501) staff       (20)     5181 2023-04-10 16:17:26.000000 mayalabs-0.0.7/mayalabs/utils/websocket.py
+-rw-r--r--   0 shubham    (501) staff       (20)    17204 2023-04-10 16:09:47.000000 mayalabs-0.0.7/mayalabs/worker.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-10 16:44:37.624674 mayalabs-0.0.7/mayalabs.egg-info/
+-rw-r--r--   0 shubham    (501) staff       (20)     4204 2023-04-10 16:44:37.000000 mayalabs-0.0.7/mayalabs.egg-info/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)      713 2023-04-10 16:44:37.000000 mayalabs-0.0.7/mayalabs.egg-info/SOURCES.txt
+-rw-r--r--   0 shubham    (501) staff       (20)        1 2023-04-10 16:44:37.000000 mayalabs-0.0.7/mayalabs.egg-info/dependency_links.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       46 2023-04-10 16:44:37.000000 mayalabs-0.0.7/mayalabs.egg-info/entry_points.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       84 2023-04-10 16:44:37.000000 mayalabs-0.0.7/mayalabs.egg-info/requires.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       35 2023-04-10 16:44:37.000000 mayalabs-0.0.7/mayalabs.egg-info/top_level.txt
+-rw-r--r--   0 shubham    (501) staff       (20)      837 2023-04-10 16:44:13.000000 mayalabs-0.0.7/pyproject.toml
+-rw-r--r--   0 shubham    (501) staff       (20)       38 2023-04-10 16:44:37.628948 mayalabs-0.0.7/setup.cfg
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-10 16:44:37.627979 mayalabs-0.0.7/tests/
+-rw-r--r--   0 shubham    (501) staff       (20)        0 2023-04-10 12:10:07.000000 mayalabs-0.0.7/tests/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)      701 2023-04-10 16:40:37.000000 mayalabs-0.0.7/tests/example_1.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1373 2023-04-10 12:10:07.000000 mayalabs-0.0.7/tests/example_2.py
+-rw-r--r--   0 shubham    (501) staff       (20)      947 2023-04-10 12:10:07.000000 mayalabs-0.0.7/tests/example_3.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-04-10 16:44:37.628409 mayalabs-0.0.7/usage/
+-rw-r--r--   0 shubham    (501) staff       (20)      169 2023-04-10 12:10:07.000000 mayalabs-0.0.7/usage/function.py
+-rw-r--r--   0 shubham    (501) staff       (20)      414 2023-04-10 12:10:07.000000 mayalabs-0.0.7/usage/sql_test.py
```

### Comparing `mayalabs-0.0.6/LICENCE` & `mayalabs-0.0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.6/mayalabs/cli.py` & `mayalabs-0.0.7/mayalabs/cli.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.6/mayalabs/function.py` & `mayalabs-0.0.7/mayalabs/function.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,22 +33,25 @@
         if os.environ.get("MAYA_ENVIRONMENT") == "development":
             log(Style.BRIGHT + Fore.YELLOW + 'DEVELOPMENT MODE' + Style.RESET_ALL, prefix='mayalabs')
             try:
                 existing_worker = Worker.get_by_alias(alias=name)
                 session_id = existing_worker.session_id if existing_worker.session_id else None
                 log(Fore.YELLOW + f'Found existing [{existing_worker.alias}]. Reusing.' + Style.RESET_ALL, prefix='mayalabs')
             except Exception as err:
+                session_id = None
                 log(Fore.YELLOW + f'Creating new [{name}]' + Style.RESET_ALL, prefix='mayalabs')
                 existing_worker = Worker.create(name=name, alias=name)
             try:
                 if session_id is not None:
                     existing_session = Session.get(session_id=session_id)
                     existing_session.script = script
+                else:
+                    existing_session = Session.new(script=script)
             except Exception as err:
-                existing_session = Session.new(script=script)
+                raise err
             func = Function(
                 name=name,
                 script=script,
                 init=False
             )
             try:
                 existing_worker.attach_session(session_id=existing_session.id)
@@ -134,15 +137,15 @@
             error_log = [
                 "Argument must be a dictionary.",
                 f"Received {type(payload).__name__}, expected a dictionary."]
             raise IntegrityException(format_error_log(error_log))
 
         log(Fore.CYAN + 'Making sure the worker is online...' + Style.RESET_ALL, prefix='mayalabs')
         self.worker.start(wait=True)
-        return self.worker.call(msg = { **payload, **kwargs })
+        return self.worker.call(msg = { **payload, **kwargs }, session=self.session)
     
     def __call__(self, payload = {}) -> Dict:
         """
         Call the deployed function. 
         Arguments passed here are passed to the `msg` object in the script.
         A value like `msg['key']` can be accessed in the script by using {{key}}
         """
```

### Comparing `mayalabs-0.0.6/mayalabs/mayalabs.py` & `mayalabs-0.0.7/mayalabs/mayalabs.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.6/mayalabs/session.py` & `mayalabs-0.0.7/mayalabs/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import asyncio
 import time, os, json, sys, hashlib
 import concurrent.futures
 
 from .utils.pac_engine import GenerateTask, InstructTask
 from .worker import WorkerClient, Worker
 from .utils.name_gen import get_random_name
-from .utils.websocket import WebsocketListener, deploy_events
+from .utils.websocket import deploy_events
 from .utils.log import log
-from .utils.defaults import default_api_base_url
+from .utils.defaults import default_api_base_url, default_log_level
 import asyncio
 from time import sleep
 from .mayalabs import authenticate
 from colorama import init, Fore, Back, Style
 from .exceptions import IntegrityException
 from .utils.logging import format_error_log
 
@@ -136,14 +136,16 @@
 
 class Session():
     def __init__(self, engine="pac-1"):
         self.id = None
         self.engine = engine
         self.script = ""
         self.worker : Worker = None
+        self.steps = {}
+        self.stitched_flow = []
 
     @classmethod
     def new(cls, script=None):
         if not isinstance(script, str):
             error_log = [
                 "Argument must be a string.",
                 f"Received {type(script).__name__}, expected a string."]
@@ -174,14 +176,16 @@
         task = GenerateTask(self.id)
         asyncio.create_task(task.execute())
         pass
 
     async def generate_async(self):
         task = GenerateTask(self.id)
         await task.execute()
+        res = SessionClient.get_session(session_id=self.id)
+        self.parse_obj(res['response'])
         pass
 
     def check_worker_start(self):
         status = 0
         i = 0
         if (self.worker.status and self.worker.status != 'STARTED'):
             status = Fore.RED + 'PENDING' + Style.RESET_ALL
@@ -278,15 +282,15 @@
                     elif self.id not in sessions.keys() or (self.id in sessions.keys() and sessions[self.id] != received_script):
                         tmp = sessions[self.id] if self.id in sessions.keys() else ""
                         sessions[self.id] = received_script
                         sessions_str = json.dumps(sessions)
                         with open(MAYA_CACHE_FILE, "w") as f:
                             f.write(sessions_str)
                             f.close()
-                        if tmp != "":
+                        if tmp != "" and tmp != received_script:
                             log(Style.BRIGHT + Fore.LIGHTYELLOW_EX + 'Found script change. Regenerating program' + Style.RESET_ALL, prefix='mayalabs')
                             self.change()
                         else:
                             log(Style.BRIGHT + Fore.CYAN + 'Generating program...' + Style.RESET_ALL, prefix='mayalabs')
                         sessions[self.id] = tmp
                     future_1 = exec.submit(run_asyncio_coroutine, self.generate_async())
                     future_1.result()
@@ -331,15 +335,15 @@
                     prefix = self.worker.name,
                     prefix_color = self.worker.prefix_color
                 )
                 for p in problems:
                     # solve()  // hehe AGI
                     field_name, node_id, node_type = p['field_name'], p['node_id'], p['node_type']
                     # message = f'* Missing field {field_name} on node {node_id} (type: {node_type})'
-                    message = f'* [{node_id}] Missing field {field_name} on node with type: {node_type}'
+                    message = f'* [{node_id}] Missing field {field_name} on node with type: {node_type}' if default_log_level()=="debug" else f'* Missing field {field_name} on node with type: {node_type}'
                     log(
                         Fore.YELLOW + message + Style.RESET_ALL,
                         prefix = self.worker.name,
                         prefix_color = self.worker.prefix_color
                     )
                 log(
                     Fore.YELLOW + Style.BRIGHT + 'To run this function, configure these requirements at the link below' + Style.RESET_ALL,
@@ -367,14 +371,16 @@
         # Implement this method
         SessionClient.change_session(session_id=self.id, script=self.script)
         return
 
     def parse_obj(self, obj):
         self.id = obj['session_id']
         self.script = obj['recipe']
+        self.steps = obj['steps']
+        self.stitched_flow = obj['stitched_flow']
 
     def update(self):
         response = SessionClient.get_session(self.id)
         self.parse_obj(response['response'])
 
     def to_string(self):
         pass
```

### Comparing `mayalabs-0.0.6/mayalabs/utils/defaults.py` & `mayalabs-0.0.7/mayalabs/utils/defaults.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,8 +19,14 @@
 
 def default_api_key() -> str:
     if mayalabs.api_key is not None:
         return mayalabs.api_key
     else:
         raise Exception(
             "No API key provided. You can set your API key in code using 'mayalabs.api_key = <API-KEY>', or you can set the environment variable MAYA_API_KEY=<API-KEY>). You can generate API keys in the Maya web interface. See https://docs.mayalabs.io for details, or email humans@mayalabs.io if you have any questions."
-        )
+        )
+
+def default_log_level() -> str:
+    if mayalabs.log_level is not None:
+        return mayalabs.log_level
+    else:
+        return "info"
```

### Comparing `mayalabs-0.0.6/mayalabs/utils/general.py` & `mayalabs-0.0.7/mayalabs/utils/general.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.6/mayalabs/utils/log.py` & `mayalabs-0.0.7/mayalabs/utils/log.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.6/mayalabs/utils/name_gen.py` & `mayalabs-0.0.7/mayalabs/utils/name_gen.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.6/mayalabs/utils/poll.py` & `mayalabs-0.0.7/mayalabs/utils/poll.py`

 * *Files identical despite different names*

### Comparing `mayalabs-0.0.6/mayalabs/worker.py` & `mayalabs-0.0.7/mayalabs/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import requests
 import asyncio
 import aiohttp
 import json
+import time
 from urllib.parse import urlparse
 import traceback
 from .utils.poll import poll
 from .utils.websocket import WebsocketListener
 from .utils.defaults import default_api_base_url
 import time
 from .mayalabs import authenticate
@@ -81,19 +82,30 @@
             response = WorkerClient.get_worker(worker_id=self.id)
             self.parse_obj(response['results'])
         else:
             raise Exception("Worker ID is not set")
         
     async def _async_get_flow_problems(self):
         client = WorkerClient()
-        results = await asyncio.gather(
-            client.get_worker_flows(worker_url=self.url),
-            client.get_required_fields(worker_url=self.url)
-        )
+        results = []
+        for _ in range(100):
+            try:
+                results = await asyncio.gather(
+                    client.get_worker_flows(worker_url=self.url),
+                    client.get_required_fields(worker_url=self.url)
+                )
+                break
+            except:
+                await asyncio.sleep(2)
+                # Runtime might be down for a second or two because of the new deploy
+            
 
+        if len(results) == 0:
+            raise APIException('An unexpected error occured and the function is down')
+        
         flows = results[0]
         reqs = results[1]
         problems = []
 
         for node in flows:
             node_type = node.get('type', '_')
             if node_type not in reqs:
@@ -174,38 +186,54 @@
                 'Authorization': 'Bearer ' + api_key,
             },
         }
 
         response = requests.request(**request)
         print(response.text)
 
-    def call(self, msg : dict):
+    def call(self, msg : dict, session=None):
         if self.id is None:
             raise Exception("Worker ID is not set")
         if self.url is None:
             self.update()
 
         # loop = asyncio.get_event_loop()
 
         async def async_wrapper():
+            log(Style.BRIGHT + Fore.CYAN + 'Running program on worker.' + Style.RESET_ALL, prefix='mayalabs')
+
+            on_connect = asyncio.Event()
+
+            log_task = asyncio.create_task(
+                self.ws_client.start_listener(
+                    log_prefix=self.name, 
+                    prefix_color=self.prefix_color,
+                    on_connect=on_connect,
+                    session=session
+                )
+            )
+
+            await on_connect.wait()
+
             call_task = asyncio.create_task(WorkerClient.call_worker(worker_url=self.url, msg=msg))
-            log_task = asyncio.create_task(self.ws_client.start_listener(log_prefix=self.name, prefix_color=self.prefix_color))
 
-        
+            
             def stop_log_task(future):
-                log_task.cancel()
+                async def _canceller():
+                    await asyncio.sleep(0.2) # Let the last of the logs print, just in case they happen too fast
+                    log_task.cancel()
+                asyncio.create_task(_canceller())
 
             call_task.add_done_callback(stop_log_task)
 
-            log(Style.BRIGHT + Fore.CYAN + 'Running program on worker.\n' + Style.RESET_ALL, prefix='mayalabs')
             await asyncio.gather(call_task, log_task)
 
             return call_task, log_task
 
-        call_task, log_task = asyncio.run(async_wrapper())
+        call_task, _ = asyncio.run(async_wrapper())
         return call_task.result()
 
     @classmethod
     def parse_obj(cls, obj):
         worker = cls()
         worker.id = obj.get('_id', None)
         worker.url = obj.get('url', None)
@@ -225,15 +253,15 @@
     @property
     def app_url(self):
         url_data = urlparse(self.url)
         origin = url_data.netloc
         parts = origin.split('.')
         env = parts[2]
 
-        app_subdomain = 'devapp' if env == 'dev' else 'app'
+        app_subdomain = 'devapp' if "dev" in parts else 'app'
         return f'https://{app_subdomain}.mayalabs.io/edit?id={self.id}'
 
 
 
 class WorkerClient:
     @staticmethod
     @authenticate
@@ -327,15 +355,16 @@
         if response.status_code == 401:
             error_log = ['Invalid API key.', 'Check if you are providing a valid API key and try again.']
             raise AuthException(format_error_log(error_log))
         elif response.status_code == 500:
             if 'errorObject' in responseData and responseData['errorObject']['type'] == 'RESOURCE_ERROR':
                 error_log = [
                     'Unable to create function.', 
-                    'This may be because you already have a function with this name.'
+                    'This may be because you already have a function with this name.',
+                    'Run <function>.clear() or delete it from the Web interface at https://app.mayalabs.io/'
                 ]
                 raise ResourceException(format_error_log(error_log))
 
         worker = Worker.parse_obj(response.json()['results'])
         return worker
     
     @staticmethod
@@ -460,8 +489,8 @@
     @staticmethod
     @authenticate
     async def get_required_fields(worker_url, api_key=None):
         msg = {}
         async with aiohttp.ClientSession(headers={ 'Authorization': f'Bearer {api_key}' }) as session:
             async with session.get(f"{worker_url}/required-fields", json=msg) as response:
                 response_json = await response.json()
-                return response_json
+                return response_json
```

### Comparing `mayalabs-0.0.6/mayalabs.egg-info/SOURCES.txt` & `mayalabs-0.0.7/mayalabs.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 LICENCE
 README.md
 pyproject.toml
-examples/function.py
-examples/sql_test.py
 mayalabs/__init__.py
 mayalabs/cli.py
 mayalabs/exceptions.py
 mayalabs/function.py
 mayalabs/mayalabs.py
 mayalabs/session.py
 mayalabs/worker.py
@@ -20,8 +18,14 @@
 mayalabs/utils/defaults.py
 mayalabs/utils/general.py
 mayalabs/utils/log.py
 mayalabs/utils/logging.py
 mayalabs/utils/name_gen.py
 mayalabs/utils/pac_engine.py
 mayalabs/utils/poll.py
-mayalabs/utils/websocket.py
+mayalabs/utils/websocket.py
+tests/__init__.py
+tests/example_1.py
+tests/example_2.py
+tests/example_3.py
+usage/function.py
+usage/sql_test.py
```

### Comparing `mayalabs-0.0.6/pyproject.toml` & `mayalabs-0.0.7/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mayalabs"
-version = "0.0.6"
+version = "0.0.7"
 description = "Python SDK for Maya Labs' natural language programming paradigm"
 dependencies = [
     "requests",
     "pydantic",
     "websockets",
     "click",
     "colorama",
@@ -29,8 +29,13 @@
 find = {}
 
 [project.scripts]
 mayalabs = "mayalabs.cli:cli"
 
 [project.urls]
 homepage = "https://mayalabs.io"
-repository = "https://github.com/mayahq/mayalabs-sdk-python"
+repository = "https://github.com/mayahq/mayalabs-sdk-python"
+
+[project.optional-dependencies]
+test=[
+  "pytest==7.2.1"
+]
```


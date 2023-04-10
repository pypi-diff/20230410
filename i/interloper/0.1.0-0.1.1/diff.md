# Comparing `tmp/interloper-0.1.0.tar.gz` & `tmp/interloper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interloper-0.1.0.tar", last modified: Thu Jan 13 15:19:42 2022, max compression
+gzip compressed data, was "interloper-0.1.1.tar", last modified: Mon Apr 10 13:23:16 2023, max compression
```

## Comparing `interloper-0.1.0.tar` & `interloper-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 h4s        (501) staff       (20)        0 2022-01-13 15:19:42.364239 interloper-0.1.0/
--rw-r--r--   0 h4s        (501) staff       (20)     1080 2022-01-12 11:38:33.000000 interloper-0.1.0/LICENSE
--rw-r--r--   0 h4s        (501) staff       (20)     3686 2022-01-13 15:19:42.364392 interloper-0.1.0/PKG-INFO
--rw-r--r--   0 h4s        (501) staff       (20)     3137 2022-01-12 19:12:17.000000 interloper-0.1.0/README.md
-drwxr-xr-x   0 h4s        (501) staff       (20)        0 2022-01-13 15:19:42.363878 interloper-0.1.0/interloper.egg-info/
--rw-r--r--   0 h4s        (501) staff       (20)     3686 2022-01-13 15:19:42.000000 interloper-0.1.0/interloper.egg-info/PKG-INFO
--rw-r--r--   0 h4s        (501) staff       (20)      225 2022-01-13 15:19:42.000000 interloper-0.1.0/interloper.egg-info/SOURCES.txt
--rw-r--r--   0 h4s        (501) staff       (20)        1 2022-01-13 15:19:42.000000 interloper-0.1.0/interloper.egg-info/dependency_links.txt
--rw-r--r--   0 h4s        (501) staff       (20)       33 2022-01-13 15:19:42.000000 interloper-0.1.0/interloper.egg-info/requires.txt
--rw-r--r--   0 h4s        (501) staff       (20)       11 2022-01-13 15:19:42.000000 interloper-0.1.0/interloper.egg-info/top_level.txt
--rw-r--r--   0 h4s        (501) staff       (20)     3668 2022-01-12 15:24:44.000000 interloper-0.1.0/interloper.py
--rw-r--r--   0 h4s        (501) staff       (20)       64 2022-01-12 11:42:11.000000 interloper-0.1.0/pyproject.toml
--rw-r--r--   0 h4s        (501) staff       (20)      641 2022-01-13 15:19:42.366919 interloper-0.1.0/setup.cfg
+drwxr-xr-x   0 h4s        (501) staff       (20)        0 2023-04-10 13:23:16.122970 interloper-0.1.1/
+-rw-r--r--   0 h4s        (501) staff       (20)     1080 2022-10-18 21:18:37.000000 interloper-0.1.1/LICENSE
+-rw-r--r--   0 h4s        (501) staff       (20)     3678 2023-04-10 13:23:16.123064 interloper-0.1.1/PKG-INFO
+-rw-r--r--   0 h4s        (501) staff       (20)     3166 2023-04-10 10:51:19.000000 interloper-0.1.1/README.md
+drwxr-xr-x   0 h4s        (501) staff       (20)        0 2023-04-10 13:23:16.122168 interloper-0.1.1/interloper.egg-info/
+-rw-r--r--   0 h4s        (501) staff       (20)     3678 2023-04-10 13:23:16.000000 interloper-0.1.1/interloper.egg-info/PKG-INFO
+-rw-r--r--   0 h4s        (501) staff       (20)      250 2023-04-10 13:23:16.000000 interloper-0.1.1/interloper.egg-info/SOURCES.txt
+-rw-r--r--   0 h4s        (501) staff       (20)        1 2023-04-10 13:23:16.000000 interloper-0.1.1/interloper.egg-info/dependency_links.txt
+-rw-r--r--   0 h4s        (501) staff       (20)       33 2023-04-10 13:23:16.000000 interloper-0.1.1/interloper.egg-info/requires.txt
+-rw-r--r--   0 h4s        (501) staff       (20)       11 2023-04-10 13:23:16.000000 interloper-0.1.1/interloper.egg-info/top_level.txt
+-rw-r--r--   0 h4s        (501) staff       (20)     3689 2023-04-10 13:17:40.000000 interloper-0.1.1/interloper.py
+-rw-r--r--   0 h4s        (501) staff       (20)       64 2022-10-18 21:18:37.000000 interloper-0.1.1/pyproject.toml
+-rw-r--r--   0 h4s        (501) staff       (20)      641 2023-04-10 13:23:16.125134 interloper-0.1.1/setup.cfg
+drwxr-xr-x   0 h4s        (501) staff       (20)        0 2023-04-10 13:23:16.122659 interloper-0.1.1/tests/
+-rw-r--r--   0 h4s        (501) staff       (20)      875 2022-10-18 21:18:37.000000 interloper-0.1.1/tests/test_interloper.py
```

### Comparing `interloper-0.1.0/LICENSE` & `interloper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `interloper-0.1.0/PKG-INFO` & `interloper-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: interloper
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tool to run ecs execute command in lambda.
 Home-page: https://github.com/theherk/interloper
 Author: Adam Sherwood
 Author-email: theherk@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/theherk/interloper/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # interloper
 
-Tool to run ecs execute command in lambda. Of course, locally you can do this via the session manager plugin, but it you want to do it in lambda, it is a bit more complex.
-
-More documentation is required.
+Tool to run ecs execute command in Python and in AWS Lambda. Of course, locally you can do this via the session manager plugin, but it you want to do it in lambda, it is a bit more complex.
 
 ## Features
 
 - Run simple commands or full scripts.
 - Pass arguments into those scripts.
 - Get output back in python.
 
@@ -33,14 +29,18 @@
 
 - Script output is truncated if very long.
 - Testing shell is present, but still must be completed.
     + Still needs started really.
     + Need to mock away the websocket bits.
 - This documentation.
 
+# Installation
+
+    pip install interloper
+
 # Usage
 
 For starters, one must [enable ECS exec](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-exec.html#ecs-exec-enabling-and-using).
 
 ## Locally
 
     ./interloper.py [event]
@@ -144,9 +144,7 @@
     if input.cmd == "heap":
         key += ".hprof"
     output = interloper.Interloper(
         input.task, cluster=input.cluster, container=input.container
     ).script("dumper.sh", [input.cmd, key])
     LOG.info(output)
 ```
-
-
```

### Comparing `interloper-0.1.0/README.md` & `interloper-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # interloper
 
-Tool to run ecs execute command in lambda. Of course, locally you can do this via the session manager plugin, but it you want to do it in lambda, it is a bit more complex.
-
-More documentation is required.
+Tool to run ecs execute command in Python and in AWS Lambda. Of course, locally you can do this via the session manager plugin, but it you want to do it in lambda, it is a bit more complex.
 
 ## Features
 
 - Run simple commands or full scripts.
 - Pass arguments into those scripts.
 - Get output back in python.
 
@@ -16,14 +14,18 @@
 
 - Script output is truncated if very long.
 - Testing shell is present, but still must be completed.
     + Still needs started really.
     + Need to mock away the websocket bits.
 - This documentation.
 
+# Installation
+
+    pip install interloper
+
 # Usage
 
 For starters, one must [enable ECS exec](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-exec.html#ecs-exec-enabling-and-using).
 
 ## Locally
 
     ./interloper.py [event]
```

### Comparing `interloper-0.1.0/interloper.egg-info/PKG-INFO` & `interloper-0.1.1/interloper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: interloper
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tool to run ecs execute command in lambda.
 Home-page: https://github.com/theherk/interloper
 Author: Adam Sherwood
 Author-email: theherk@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/theherk/interloper/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # interloper
 
-Tool to run ecs execute command in lambda. Of course, locally you can do this via the session manager plugin, but it you want to do it in lambda, it is a bit more complex.
-
-More documentation is required.
+Tool to run ecs execute command in Python and in AWS Lambda. Of course, locally you can do this via the session manager plugin, but it you want to do it in lambda, it is a bit more complex.
 
 ## Features
 
 - Run simple commands or full scripts.
 - Pass arguments into those scripts.
 - Get output back in python.
 
@@ -33,14 +29,18 @@
 
 - Script output is truncated if very long.
 - Testing shell is present, but still must be completed.
     + Still needs started really.
     + Need to mock away the websocket bits.
 - This documentation.
 
+# Installation
+
+    pip install interloper
+
 # Usage
 
 For starters, one must [enable ECS exec](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-exec.html#ecs-exec-enabling-and-using).
 
 ## Locally
 
     ./interloper.py [event]
@@ -144,9 +144,7 @@
     if input.cmd == "heap":
         key += ".hprof"
     output = interloper.Interloper(
         input.task, cluster=input.cluster, container=input.container
     ).script("dumper.sh", [input.cmd, key])
     LOG.info(output)
 ```
-
-
```

### Comparing `interloper-0.1.0/interloper.py` & `interloper-0.1.1/interloper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 import base64
-from dataclasses import dataclass
 import json
-from json.decoder import JSONDecodeError
 import logging
+import ssl
 import sys
-from typing import List
 import uuid
+from dataclasses import dataclass
+from typing import List
 
 import boto3
 import construct as c
 import websocket
 
 
 LOG = logging.getLogger()
@@ -84,15 +84,17 @@
     )
 
     AgentMessagePayload = c.Struct(
         "PayloadLength" / c.Int32ub,
         "Payload" / c.PaddedString(c.this.PayloadLength, "ascii"),
     )
 
-    connection = websocket.create_connection(session["streamUrl"])
+    connection = websocket.create_connection(
+        session["streamUrl"], sslopt={"cert_reqs": ssl.CERT_NONE}
+    )
     try:
         init_payload = {
             "MessageSchemaVersion": "1.0",
             "RequestId": str(uuid.uuid4()),
             "TokenValue": session["tokenValue"],
         }
         connection.send(json.dumps(init_payload))
```

### Comparing `interloper-0.1.0/setup.cfg` & `interloper-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = interloper
-version = 0.1.0
+version = 0.1.1
 author = Adam Sherwood
 author_email = theherk@gmail.com
 description = Tool to run ecs execute command in lambda.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/theherk/interloper
 project_urls =
```


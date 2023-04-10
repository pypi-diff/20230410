# Comparing `tmp/appmesh-0.3.6-py3-none-any.whl.zip` & `tmp/appmesh-0.3.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 13690 bytes, number of entries: 6
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-07 08:54 appmesh/__init__.py
--rw-r--r--  2.0 unx    49876 b- defN 23-Apr-07 08:54 appmesh/appmesh_client.py
--rw-r--r--  2.0 unx    10620 b- defN 23-Apr-07 08:54 appmesh-0.3.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 08:54 appmesh-0.3.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-07 08:54 appmesh-0.3.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      455 b- defN 23-Apr-07 08:54 appmesh-0.3.6.dist-info/RECORD
-6 files, 61062 bytes uncompressed, 12868 bytes compressed:  78.9%
+Zip file size: 14307 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-10 09:14 appmesh/__init__.py
+-rw-r--r--  2.0 unx    51664 b- defN 23-Apr-10 09:14 appmesh/appmesh_client.py
+-rw-r--r--  2.0 unx    10620 b- defN 23-Apr-10 09:14 appmesh-0.3.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 09:14 appmesh-0.3.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-10 09:14 appmesh-0.3.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      455 b- defN 23-Apr-10 09:14 appmesh-0.3.7.dist-info/RECORD
+6 files, 62850 bytes uncompressed, 13485 bytes compressed:  78.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: appmesh/__init__.py
 Comment: 
 
 Filename: appmesh/appmesh_client.py
 Comment: 
 
-Filename: appmesh-0.3.6.dist-info/METADATA
+Filename: appmesh-0.3.7.dist-info/METADATA
 Comment: 
 
-Filename: appmesh-0.3.6.dist-info/WHEEL
+Filename: appmesh-0.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: appmesh-0.3.6.dist-info/top_level.txt
+Filename: appmesh-0.3.7.dist-info/top_level.txt
 Comment: 
 
-Filename: appmesh-0.3.6.dist-info/RECORD
+Filename: appmesh-0.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## appmesh/appmesh_client.py

```diff
@@ -51,83 +51,107 @@
         """
         Application error handling behavior definition object
         """
 
         def __init__(self, data=None) -> None:
             if isinstance(data, (str, bytes, bytearray)):
                 data = json.loads(data)
+            # default exit behavior [restart,standby,keepalive,remove]
             self.exit = _get_str_item(data, "exit")
+            # exit code behavior (e.g, --control 0:restart --control 1:standby), higher priority than default exit behavior
             self.control = copy.deepcopy(data)
 
     class DailyLimitation(object):
         """
         Application avialable day time definition object
         """
 
         def __init__(self, data=None) -> None:
             if isinstance(data, (str, bytes, bytearray)):
                 data = json.loads(data)
+            # daily start time (e.g., '09:00:00+08')
             self.daily_start = _get_int_item(data, "daily_start")
+            # daily end time (e.g., '20:00:00+08')
             self.daily_end = _get_int_item(data, "daily_end")
 
     class ResourceLimitation(object):
         """
         Application cgroup limitation definition object
         """
 
         def __init__(self, data=None) -> None:
             if isinstance(data, (str, bytes, bytearray)):
                 data = json.loads(data)
+            # CPU shares (relative weight)
             self.cpu_shares = _get_int_item(data, "cpu_shares")
+            # memory limit in MByte
             self.memory_mb = _get_int_item(data, "memory_mb")
+            # virtual memory limit in MByte
             self.memory_virt_mb = _get_int_item(data, "memory_virt_mb")
 
     def __init__(self, data=None):
         """Construct an App Mesh Application object
 
         Args:
             data (str | dict | json, optional): application definition data
         """
 
         if isinstance(data, (str, bytes, bytearray)):
             data = json.loads(data)
 
-        # mandatory parameters
+        # application name
         self.name = _get_str_item(data, "name")
+        # full command line with arguments
         self.command = _get_str_item(data, "command")
 
+        # use shell mode, cmd can be more shell commands with string format
         self.shell = _get_bool_item(data, "shell")
+        # application description
         self.description = _get_str_item(data, "description")
+        # metadata string/JSON (input for application, pass to process stdin)
         self.metadata = _get_native_item(data, "metadata")
+        # working directory
         self.working_dir = _get_str_item(data, "working_dir")
+        # initial application status (true is enable, false is disabled)
         self.status = _get_int_item(data, "status")
+        # docker image which used to run command line (for docker container application)
         self.docker_image = _get_str_item(data, "docker_image")
+        # stdout file cache number
         self.stdout_cache_num = _get_int_item(data, "stdout_cache_num")
 
+        # start date time for app (ISO8601 time format, e.g., '2020-10-11T09:22:05')
         self.start_time = _get_int_item(data, "start_time")
+        # end date time for app (ISO8601 time format, e.g., '2020-10-11T10:22:05')
         self.end_time = _get_int_item(data, "end_time")
+        # start interval seconds for short running app, support ISO 8601 durations and cron expression (e.g., 'P1Y2M3DT4H5M6S' 'P5W' '* */5 * * * *')
         self.interval = _get_int_item(data, "interval")
+        # indicate interval parameter use cron expression
         self.cron = _get_bool_item(data, "cron")
         self.daily_limitation = App.DailyLimitation(_get_native_item(data, "daily_limitation"))
 
+        # extra timeout seconds for stopping current process, support ISO 8601 durations (e.g., 'P1Y2M3DT4H5M6S' 'P5W').
         self.retention = _get_str_item(data, "retention")
-        self.extra_time = _get_str_item(data, "extra_time")
 
+        # health check script command (e.g., sh -x 'curl host:port/health', return 0 is health)
         self.health_check_cmd = _get_str_item(data, "health_check_cmd")
+        # application user permission, value is 2 bit integer: [group & other], each bit can be deny:1, read:2, write: 3.
         self.permission = _get_int_item(data, "permission")
         self.behavior = App.Behavior(_get_native_item(data, "behavior"))
 
+        # environment variables (e.g., -e env1=value1 -e env2=value2, APP_DOCKER_OPTS is used to input docker run parameters)
         self.env = dict()
         if data and "env" in data:
             for k, v in data["env"].items():
                 self.env[k] = v
+        # security environment variables, encrypt in server side with application owner's cipher
         self.sec_env = dict()
         if data and "sec_env" in data:
             for k, v in data["sec_env"].items():
                 self.sec_env[k] = v
+        # process id used to attach
         self.pid = _get_int_item(data, "pid")
         self.resource_limit = App.ResourceLimitation(_get_native_item(data, "resource_limit"))
 
         # readonly attributes
         self.owner = _get_str_item(data, "owner")
         self.pstree = _get_str_item(data, "pstree")
         self.container_id = _get_str_item(data, "container_id")
```

## Comparing `appmesh-0.3.6.dist-info/METADATA` & `appmesh-0.3.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appmesh
-Version: 0.3.6
+Version: 0.3.7
 Summary: Client SDK for App Mesh
 Home-page: https://github.com/laoshanxi/app-mesh
 Author: laoshanxi
 Author-email: 178029200@qq.com
 License: MIT
 Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: appmesh Version: 0.3.6 Summary: Client SDK for App
+Metadata-Version: 2.1 Name: appmesh Version: 0.3.7 Summary: Client SDK for App
 Mesh Home-page: https://github.com/laoshanxi/app-mesh Author: laoshanxi Author-
 email: 178029200@qq.com License: MIT Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: msgpack Requires-Dist: requests-toolbelt Requires-Dist:
 aniso8601 ï»¿[![language.badge]][language.url] [![standard.badge]]
```


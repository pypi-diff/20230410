# Comparing `tmp/akari-client-0.3.0.tar.gz` & `tmp/akari-client-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akari-client-0.3.0.tar", last modified: Fri Mar 17 00:35:11 2023, max compression
+gzip compressed data, was "akari-client-0.3.1.tar", last modified: Mon Apr 10 15:04:27 2023, max compression
```

## Comparing `akari-client-0.3.0.tar` & `akari-client-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-03-17 00:35:11.921103 akari-client-0.3.0/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1708 2023-03-17 00:35:11.921103 akari-client-0.3.0/PKG-INFO
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      725 2023-03-17 00:33:36.000000 akari-client-0.3.0/README.md
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-03-17 00:35:11.909103 akari-client-0.3.0/akari_client/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       87 2022-12-05 21:46:13.000000 akari-client-0.3.0/akari_client/__init__.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      920 2022-12-05 23:29:31.000000 akari-client-0.3.0/akari_client/akari_client.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2014 2023-03-16 13:20:21.000000 akari-client-0.3.0/akari_client/color.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3717 2023-03-16 13:20:21.000000 akari-client-0.3.0/akari_client/config.py
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-03-17 00:35:11.913103 akari-client-0.3.0/akari_client/grpc/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2022-12-05 21:46:13.000000 akari-client-0.3.0/akari_client/grpc/__init__.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      125 2022-12-05 21:46:13.000000 akari-client-0.3.0/akari_client/grpc/_error.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      656 2022-12-05 21:46:13.000000 akari-client-0.3.0/akari_client/grpc/channel_pool.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1434 2022-12-05 21:46:13.000000 akari-client-0.3.0/akari_client/grpc/factory.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4096 2022-12-05 21:46:13.000000 akari-client-0.3.0/akari_client/grpc/joints_controller.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4739 2023-03-16 13:20:21.000000 akari-client-0.3.0/akari_client/grpc/m5stack.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2478 2022-12-05 21:46:13.000000 akari-client-0.3.0/akari_client/joint_controller.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     8963 2023-03-16 13:20:21.000000 akari-client-0.3.0/akari_client/joint_manager.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    11435 2023-03-16 13:20:21.000000 akari-client-0.3.0/akari_client/m5stack_client.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      374 2023-03-16 13:20:21.000000 akari-client-0.3.0/akari_client/position.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2022-12-05 21:46:13.000000 akari-client-0.3.0/akari_client/py.typed
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-03-17 00:35:11.917103 akari-client-0.3.0/akari_client/serial/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2022-12-05 21:46:13.000000 akari-client-0.3.0/akari_client/serial/__init__.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     6666 2022-12-05 23:08:44.000000 akari-client-0.3.0/akari_client/serial/dynamixel.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4538 2022-12-05 23:03:45.000000 akari-client-0.3.0/akari_client/serial/dynamixel_communicator.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1405 2022-12-05 23:07:56.000000 akari-client-0.3.0/akari_client/serial/factory.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4599 2023-03-16 13:20:21.000000 akari-client-0.3.0/akari_client/serial/m5stack.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4117 2022-12-05 21:46:13.000000 akari-client-0.3.0/akari_client/serial/m5stack_communicator.py
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-03-17 00:35:11.913103 akari-client-0.3.0/akari_client.egg-info/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1708 2023-03-17 00:35:11.000000 akari-client-0.3.0/akari_client.egg-info/PKG-INFO
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      843 2023-03-17 00:35:11.000000 akari-client-0.3.0/akari_client.egg-info/SOURCES.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        1 2023-03-17 00:35:11.000000 akari-client-0.3.0/akari_client.egg-info/dependency_links.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      200 2023-03-17 00:35:11.000000 akari-client-0.3.0/akari_client.egg-info/requires.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       13 2023-03-17 00:35:11.000000 akari-client-0.3.0/akari_client.egg-info/top_level.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       38 2023-03-17 00:35:11.921103 akari-client-0.3.0/setup.cfg
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1359 2023-03-17 00:34:59.000000 akari-client-0.3.0/setup.py
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-04-10 15:04:27.274032 akari-client-0.3.1/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1708 2023-04-10 15:04:27.274032 akari-client-0.3.1/PKG-INFO
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      725 2023-04-10 14:34:37.000000 akari-client-0.3.1/README.md
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-04-10 15:04:27.274032 akari-client-0.3.1/akari_client/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       87 2022-12-05 21:46:13.000000 akari-client-0.3.1/akari_client/__init__.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      920 2022-12-05 23:29:31.000000 akari-client-0.3.1/akari_client/akari_client.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2014 2023-03-16 13:20:21.000000 akari-client-0.3.1/akari_client/color.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3717 2023-03-16 13:20:21.000000 akari-client-0.3.1/akari_client/config.py
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-04-10 15:04:27.274032 akari-client-0.3.1/akari_client/grpc/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2023-04-06 13:57:42.000000 akari-client-0.3.1/akari_client/grpc/__init__.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      125 2022-12-05 21:46:13.000000 akari-client-0.3.1/akari_client/grpc/_error.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      656 2022-12-05 21:46:13.000000 akari-client-0.3.1/akari_client/grpc/channel_pool.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1434 2022-12-05 21:46:13.000000 akari-client-0.3.1/akari_client/grpc/factory.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4096 2022-12-05 21:46:13.000000 akari-client-0.3.1/akari_client/grpc/joints_controller.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4739 2023-03-16 13:20:21.000000 akari-client-0.3.1/akari_client/grpc/m5stack.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2478 2022-12-05 21:46:13.000000 akari-client-0.3.1/akari_client/joint_controller.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     8963 2023-03-16 13:20:21.000000 akari-client-0.3.1/akari_client/joint_manager.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    11435 2023-03-16 13:20:21.000000 akari-client-0.3.1/akari_client/m5stack_client.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      374 2023-03-16 13:20:21.000000 akari-client-0.3.1/akari_client/position.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2023-04-06 13:57:42.000000 akari-client-0.3.1/akari_client/py.typed
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-04-10 15:04:27.274032 akari-client-0.3.1/akari_client/serial/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2023-04-06 13:57:42.000000 akari-client-0.3.1/akari_client/serial/__init__.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     6666 2022-12-05 23:08:44.000000 akari-client-0.3.1/akari_client/serial/dynamixel.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4538 2022-12-05 23:03:45.000000 akari-client-0.3.1/akari_client/serial/dynamixel_communicator.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1405 2022-12-05 23:07:56.000000 akari-client-0.3.1/akari_client/serial/factory.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4599 2023-03-16 13:20:21.000000 akari-client-0.3.1/akari_client/serial/m5stack.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4117 2022-12-05 21:46:13.000000 akari-client-0.3.1/akari_client/serial/m5stack_communicator.py
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-04-10 15:04:27.274032 akari-client-0.3.1/akari_client.egg-info/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1708 2023-04-10 15:04:27.000000 akari-client-0.3.1/akari_client.egg-info/PKG-INFO
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      843 2023-04-10 15:04:27.000000 akari-client-0.3.1/akari_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        1 2023-04-10 15:04:27.000000 akari-client-0.3.1/akari_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      157 2023-04-10 15:04:27.000000 akari-client-0.3.1/akari_client.egg-info/requires.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       13 2023-04-10 15:04:27.000000 akari-client-0.3.1/akari_client.egg-info/top_level.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       38 2023-04-10 15:04:27.274032 akari-client-0.3.1/setup.cfg
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1316 2023-04-10 15:03:53.000000 akari-client-0.3.1/setup.py
```

### Comparing `akari-client-0.3.0/PKG-INFO` & `akari-client-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akari-client
-Version: 0.3.0
+Version: 0.3.1
 Summary: Akari Python package
 Home-page: https://github.com/AkariGroup/akari_software
 Author: akari
 Author-email: akari.tmc@gmail.com
 License: Apache License 2.0
 Description: # akari\_client
```

### Comparing `akari-client-0.3.0/README.md` & `akari-client-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.0/akari_client/akari_client.py` & `akari-client-0.3.1/akari_client/akari_client.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.0/akari_client/color.py` & `akari-client-0.3.1/akari_client/color.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.0/akari_client/config.py` & `akari-client-0.3.1/akari_client/config.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.0/akari_client/grpc/channel_pool.py` & `akari-client-0.3.1/akari_client/grpc/channel_pool.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.0/akari_client/grpc/factory.py` & `akari-client-0.3.1/akari_client/grpc/factory.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.0/akari_client/grpc/joints_controller.py` & `akari-client-0.3.1/akari_client/grpc/joints_controller.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.0/akari_client/grpc/m5stack.py` & `akari-client-0.3.1/akari_client/grpc/m5stack.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.0/akari_client/joint_controller.py` & `akari-client-0.3.1/akari_client/joint_controller.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.0/akari_client/joint_manager.py` & `akari-client-0.3.1/akari_client/joint_manager.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.0/akari_client/m5stack_client.py` & `akari-client-0.3.1/akari_client/m5stack_client.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.0/akari_client/serial/dynamixel.py` & `akari-client-0.3.1/akari_client/serial/dynamixel.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.0/akari_client/serial/dynamixel_communicator.py` & `akari-client-0.3.1/akari_client/serial/dynamixel_communicator.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.0/akari_client/serial/factory.py` & `akari-client-0.3.1/akari_client/serial/factory.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.0/akari_client/serial/m5stack.py` & `akari-client-0.3.1/akari_client/serial/m5stack.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.0/akari_client/serial/m5stack_communicator.py` & `akari-client-0.3.1/akari_client/serial/m5stack_communicator.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.0/akari_client.egg-info/PKG-INFO` & `akari-client-0.3.1/akari_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akari-client
-Version: 0.3.0
+Version: 0.3.1
 Summary: Akari Python package
 Home-page: https://github.com/AkariGroup/akari_software
 Author: akari
 Author-email: akari.tmc@gmail.com
 License: Apache License 2.0
 Description: # akari\_client
```

### Comparing `akari-client-0.3.0/akari_client.egg-info/SOURCES.txt` & `akari-client-0.3.1/akari_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.0/setup.py` & `akari-client-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="akari-client",
-    version="0.3.0",
+    version="0.3.1",
     packages=find_packages(exclude=["tests"]),
     description="Akari Python package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="akari",
     author_email="akari.tmc@gmail.com",
     license="Apache License 2.0",
@@ -30,14 +30,14 @@
     extras_require={
         "grpc": [
             "akari-proto>=0.3.0,<0.4.0",
             "grpcio==1.44.0",
             "protobuf==3.19.3",
         ],
         "depthai": [
-            "matplotlib==3.6.2",
-            "depthai==2.19.1.0",
-            "opencv-python-headless==4.6.0.66",
-            "blobconverter==1.3.0",
+            "matplotlib",
+            "depthai",
+            "opencv-python",
+            "blobconverter",
         ],
     },
 )
```


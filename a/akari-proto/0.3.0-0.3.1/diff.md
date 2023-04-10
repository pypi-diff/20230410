# Comparing `tmp/akari-proto-0.3.0.tar.gz` & `tmp/akari-proto-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akari-proto-0.3.0.tar", last modified: Fri Mar 17 00:34:10 2023, max compression
+gzip compressed data, was "akari-proto-0.3.1.tar", last modified: Mon Apr 10 15:04:40 2023, max compression
```

## Comparing `akari-proto-0.3.0.tar` & `akari-proto-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-03-17 00:34:10.129397 akari-proto-0.3.0/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1052 2023-03-17 00:34:10.129397 akari-proto-0.3.0/PKG-INFO
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      285 2023-03-17 00:33:36.000000 akari-proto-0.3.0/README.md
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-03-17 00:34:10.129397 akari-proto-0.3.0/akari_proto/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2022-12-05 21:46:13.000000 akari-proto-0.3.0/akari_proto/__init__.py
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-03-17 00:34:10.129397 akari-proto-0.3.0/akari_proto/grpc/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2022-12-05 21:46:13.000000 akari-proto-0.3.0/akari_proto/grpc/__init__.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3936 2022-12-05 21:46:13.000000 akari-proto-0.3.0/akari_proto/grpc/error.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    10094 2022-12-05 21:46:13.000000 akari-proto-0.3.0/akari_proto/joints_controller_pb2.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    20455 2022-12-05 21:46:13.000000 akari-proto-0.3.0/akari_proto/joints_controller_pb2_grpc.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     8086 2023-03-16 13:20:21.000000 akari-proto-0.3.0/akari_proto/m5stack_pb2.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    13951 2023-03-16 13:20:21.000000 akari-proto-0.3.0/akari_proto/m5stack_pb2_grpc.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2022-12-05 21:46:13.000000 akari-proto-0.3.0/akari_proto/py.typed
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-03-17 00:34:10.129397 akari-proto-0.3.0/akari_proto.egg-info/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1052 2023-03-17 00:34:10.000000 akari-proto-0.3.0/akari_proto.egg-info/PKG-INFO
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      430 2023-03-17 00:34:10.000000 akari-proto-0.3.0/akari_proto.egg-info/SOURCES.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        1 2023-03-17 00:34:10.000000 akari-proto-0.3.0/akari_proto.egg-info/dependency_links.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       32 2023-03-17 00:34:10.000000 akari-proto-0.3.0/akari_proto.egg-info/requires.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       12 2023-03-17 00:34:10.000000 akari-proto-0.3.0/akari_proto.egg-info/top_level.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       38 2023-03-17 00:34:10.129397 akari-proto-0.3.0/setup.cfg
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1009 2023-03-17 00:33:56.000000 akari-proto-0.3.0/setup.py
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-04-10 15:04:40.830059 akari-proto-0.3.1/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1092 2023-04-10 15:04:40.830059 akari-proto-0.3.1/PKG-INFO
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      285 2023-03-17 00:33:36.000000 akari-proto-0.3.1/README.md
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-04-10 15:04:40.830059 akari-proto-0.3.1/akari_proto/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2023-04-06 13:57:42.000000 akari-proto-0.3.1/akari_proto/__init__.py
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-04-10 15:04:40.830059 akari-proto-0.3.1/akari_proto/grpc/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2023-04-06 13:57:42.000000 akari-proto-0.3.1/akari_proto/grpc/__init__.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3936 2022-12-05 21:46:13.000000 akari-proto-0.3.1/akari_proto/grpc/error.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    10094 2022-12-05 21:46:13.000000 akari-proto-0.3.1/akari_proto/joints_controller_pb2.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    20455 2022-12-05 21:46:13.000000 akari-proto-0.3.1/akari_proto/joints_controller_pb2_grpc.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     8086 2023-03-16 13:20:21.000000 akari-proto-0.3.1/akari_proto/m5stack_pb2.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    13951 2023-03-16 13:20:21.000000 akari-proto-0.3.1/akari_proto/m5stack_pb2_grpc.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2023-04-06 13:57:42.000000 akari-proto-0.3.1/akari_proto/py.typed
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-04-10 15:04:40.830059 akari-proto-0.3.1/akari_proto.egg-info/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1092 2023-04-10 15:04:40.000000 akari-proto-0.3.1/akari_proto.egg-info/PKG-INFO
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      430 2023-04-10 15:04:40.000000 akari-proto-0.3.1/akari_proto.egg-info/SOURCES.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        1 2023-04-10 15:04:40.000000 akari-proto-0.3.1/akari_proto.egg-info/dependency_links.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       32 2023-04-10 15:04:40.000000 akari-proto-0.3.1/akari_proto.egg-info/requires.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       12 2023-04-10 15:04:40.000000 akari-proto-0.3.1/akari_proto.egg-info/top_level.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       38 2023-04-10 15:04:40.830059 akari-proto-0.3.1/setup.cfg
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1060 2023-04-10 15:03:53.000000 akari-proto-0.3.1/setup.py
```

### Comparing `akari-proto-0.3.0/PKG-INFO` & `akari-proto-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: akari-proto
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python package of akari protobuf definitions and utility functions
 Home-page: https://github.com/AkariGroup/akari_software
 Author: akari
 Author-email: akari.tmc@gmail.com
 License: Apache License 2.0
 Description: # akari\_proto
         
@@ -18,7 +18,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
+Description-Content-Type: text/markdown
```

### Comparing `akari-proto-0.3.0/akari_proto/grpc/error.py` & `akari-proto-0.3.1/akari_proto/grpc/error.py`

 * *Files identical despite different names*

### Comparing `akari-proto-0.3.0/akari_proto/joints_controller_pb2.py` & `akari-proto-0.3.1/akari_proto/joints_controller_pb2.py`

 * *Files identical despite different names*

### Comparing `akari-proto-0.3.0/akari_proto/joints_controller_pb2_grpc.py` & `akari-proto-0.3.1/akari_proto/joints_controller_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `akari-proto-0.3.0/akari_proto/m5stack_pb2.py` & `akari-proto-0.3.1/akari_proto/m5stack_pb2.py`

 * *Files identical despite different names*

### Comparing `akari-proto-0.3.0/akari_proto/m5stack_pb2_grpc.py` & `akari-proto-0.3.1/akari_proto/m5stack_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `akari-proto-0.3.0/akari_proto.egg-info/PKG-INFO` & `akari-proto-0.3.1/akari_proto.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: akari-proto
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python package of akari protobuf definitions and utility functions
 Home-page: https://github.com/AkariGroup/akari_software
 Author: akari
 Author-email: akari.tmc@gmail.com
 License: Apache License 2.0
 Description: # akari\_proto
         
@@ -18,7 +18,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
+Description-Content-Type: text/markdown
```

### Comparing `akari-proto-0.3.0/setup.py` & `akari-proto-0.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import find_packages, setup
 
 setup(
     name="akari-proto",
-    version="0.3.0",
+    version="0.3.1",
     description="Python package of akari protobuf definitions and utility functions",
     packages=find_packages(exclude=["tests"]),
     author="akari",
     author_email="akari.tmc@gmail.com",
     package_data={"akari_proto": ["py.typed"]},
     license="Apache License 2.0",
     long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python",
```


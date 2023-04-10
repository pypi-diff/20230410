# Comparing `tmp/grpc_load_balancer-0.0.1.tar.gz` & `tmp/grpc_load_balancer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpc_load_balancer-0.0.1.tar", last modified: Mon Apr 10 07:40:51 2023, max compression
+gzip compressed data, was "grpc_load_balancer-0.0.2.tar", last modified: Mon Apr 10 08:03:13 2023, max compression
```

## Comparing `grpc_load_balancer-0.0.1.tar` & `grpc_load_balancer-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:40:51.277541 grpc_load_balancer-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-10 07:40:31.000000 grpc_load_balancer-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-04-10 07:40:51.277541 grpc_load_balancer-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-10 07:40:31.000000 grpc_load_balancer-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:40:51.273540 grpc_load_balancer-0.0.1/grpc_load_balancer/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-10 07:40:31.000000 grpc_load_balancer-0.0.1/grpc_load_balancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-10 07:40:31.000000 grpc_load_balancer-0.0.1/grpc_load_balancer/connection_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-10 07:40:31.000000 grpc_load_balancer-0.0.1/grpc_load_balancer/env_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-10 07:40:31.000000 grpc_load_balancer-0.0.1/grpc_load_balancer/grpc_connection_forwarder.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-10 07:40:31.000000 grpc_load_balancer-0.0.1/grpc_load_balancer/lock_with_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-10 07:40:31.000000 grpc_load_balancer-0.0.1/grpc_load_balancer/metrics_based_server_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:40:51.277541 grpc_load_balancer-0.0.1/grpc_load_balancer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-04-10 07:40:51.000000 grpc_load_balancer-0.0.1/grpc_load_balancer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-10 07:40:51.000000 grpc_load_balancer-0.0.1/grpc_load_balancer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 07:40:51.000000 grpc_load_balancer-0.0.1/grpc_load_balancer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 07:40:51.000000 grpc_load_balancer-0.0.1/grpc_load_balancer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 07:40:51.000000 grpc_load_balancer-0.0.1/grpc_load_balancer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 07:40:51.277541 grpc_load_balancer-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-10 07:40:31.000000 grpc_load_balancer-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:40:51.277541 grpc_load_balancer-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-10 07:40:31.000000 grpc_load_balancer-0.0.1/tests/test_grpc_load_balancer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:03:13.452857 grpc_load_balancer-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-10 08:03:13.452857 grpc_load_balancer-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:03:13.448857 grpc_load_balancer-0.0.2/grpc_load_balancer/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/grpc_load_balancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/grpc_load_balancer/connection_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/grpc_load_balancer/env_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/grpc_load_balancer/grpc_connection_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/grpc_load_balancer/lock_with_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/grpc_load_balancer/metrics_based_server_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:03:13.452857 grpc_load_balancer-0.0.2/grpc_load_balancer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-10 08:03:13.000000 grpc_load_balancer-0.0.2/grpc_load_balancer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-10 08:03:13.000000 grpc_load_balancer-0.0.2/grpc_load_balancer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:03:13.000000 grpc_load_balancer-0.0.2/grpc_load_balancer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 08:03:13.000000 grpc_load_balancer-0.0.2/grpc_load_balancer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 08:03:13.000000 grpc_load_balancer-0.0.2/grpc_load_balancer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 08:03:13.452857 grpc_load_balancer-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:03:13.452857 grpc_load_balancer-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/tests/test_grpc_load_balancer.py
```

### Comparing `grpc_load_balancer-0.0.1/LICENSE` & `grpc_load_balancer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grpc_load_balancer-0.0.1/PKG-INFO` & `grpc_load_balancer-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: grpc_load_balancer
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small toolset to implement load balancing for gRPC services
 Home-page: https://github.com/flagman/grpc-load-balancer
 Author: Pavel Malay
 Author-email: flagmansupport@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gRPC Load Balancer
 
 `grpc_load_balancer` is a Python package that allows you to easily configure and manage separate gRPC server and client instances using a metrics-based load balancing approach. This is useful when you have multiple services running and want to distribute the load efficiently among them. The package includes a connection forwarder, a metrics-based server finder, and a configuration loader.
 It implemetns the following design:
-![Design](https://grpc.io/img/image_1.png)
+
+<img src="imgs/design.jpg" width="50%" height="50%">
+
 
 
 ## Features
 
 - Forward connections from clients to gRPC servers.
 - Use Prometheus metrics to select the best server to handle a request.
-- Configure and manage gRPC servers and clients using environment variables.
+- Configure and manage gRPC server finder using environment variables.
 
 ## Installation
 
 You can install `grpc_load_balancer` using pip:
 
 ```bash
 pip install grpc_load_balancer
```

### Comparing `grpc_load_balancer-0.0.1/README.md` & `grpc_load_balancer-0.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # gRPC Load Balancer
 
 `grpc_load_balancer` is a Python package that allows you to easily configure and manage separate gRPC server and client instances using a metrics-based load balancing approach. This is useful when you have multiple services running and want to distribute the load efficiently among them. The package includes a connection forwarder, a metrics-based server finder, and a configuration loader.
 It implemetns the following design:
-![Design](https://grpc.io/img/image_1.png)
+
+<img src="imgs/design.jpg" width="50%" height="50%">
+
 
 
 ## Features
 
 - Forward connections from clients to gRPC servers.
 - Use Prometheus metrics to select the best server to handle a request.
-- Configure and manage gRPC servers and clients using environment variables.
+- Configure and manage gRPC server finder using environment variables.
 
 ## Installation
 
 You can install `grpc_load_balancer` using pip:
 
 ```bash
 pip install grpc_load_balancer
```

### Comparing `grpc_load_balancer-0.0.1/grpc_load_balancer/connection_counter.py` & `grpc_load_balancer-0.0.2/grpc_load_balancer/connection_counter.py`

 * *Files identical despite different names*

### Comparing `grpc_load_balancer-0.0.1/grpc_load_balancer/env_config_loader.py` & `grpc_load_balancer-0.0.2/grpc_load_balancer/env_config_loader.py`

 * *Files identical despite different names*

### Comparing `grpc_load_balancer-0.0.1/grpc_load_balancer/grpc_connection_forwarder.py` & `grpc_load_balancer-0.0.2/grpc_load_balancer/grpc_connection_forwarder.py`

 * *Files identical despite different names*

### Comparing `grpc_load_balancer-0.0.1/grpc_load_balancer/metrics_based_server_finder.py` & `grpc_load_balancer-0.0.2/grpc_load_balancer/metrics_based_server_finder.py`

 * *Files identical despite different names*

### Comparing `grpc_load_balancer-0.0.1/grpc_load_balancer.egg-info/PKG-INFO` & `grpc_load_balancer-0.0.2/grpc_load_balancer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: grpc-load-balancer
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small toolset to implement load balancing for gRPC services
 Home-page: https://github.com/flagman/grpc-load-balancer
 Author: Pavel Malay
 Author-email: flagmansupport@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gRPC Load Balancer
 
 `grpc_load_balancer` is a Python package that allows you to easily configure and manage separate gRPC server and client instances using a metrics-based load balancing approach. This is useful when you have multiple services running and want to distribute the load efficiently among them. The package includes a connection forwarder, a metrics-based server finder, and a configuration loader.
 It implemetns the following design:
-![Design](https://grpc.io/img/image_1.png)
+
+<img src="imgs/design.jpg" width="50%" height="50%">
+
 
 
 ## Features
 
 - Forward connections from clients to gRPC servers.
 - Use Prometheus metrics to select the best server to handle a request.
-- Configure and manage gRPC servers and clients using environment variables.
+- Configure and manage gRPC server finder using environment variables.
 
 ## Installation
 
 You can install `grpc_load_balancer` using pip:
 
 ```bash
 pip install grpc_load_balancer
```

### Comparing `grpc_load_balancer-0.0.1/grpc_load_balancer.egg-info/SOURCES.txt` & `grpc_load_balancer-0.0.2/grpc_load_balancer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grpc_load_balancer-0.0.1/setup.py` & `grpc_load_balancer-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="grpc_load_balancer",
-    version="0.0.1",
+    version="0.0.2",
     author="Pavel Malay",
     author_email="flagmansupport@gmail.com",
     description="A small toolset to implement load balancing for gRPC services",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/flagman/grpc-load-balancer",
     packages=find_packages(exclude=["tests"]),
```

### Comparing `grpc_load_balancer-0.0.1/tests/test_grpc_load_balancer.py` & `grpc_load_balancer-0.0.2/tests/test_grpc_load_balancer.py`

 * *Files identical despite different names*


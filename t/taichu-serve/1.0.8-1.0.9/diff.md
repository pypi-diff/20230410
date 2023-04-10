# Comparing `tmp/taichu-serve-1.0.8.tar.gz` & `tmp/taichu-serve-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichu-serve-1.0.8.tar", last modified: Mon Apr 10 07:28:53 2023, max compression
+gzip compressed data, was "taichu-serve-1.0.9.tar", last modified: Mon Apr 10 07:38:10 2023, max compression
```

## Comparing `taichu-serve-1.0.8.tar` & `taichu-serve-1.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 07:28:53.813574 taichu-serve-1.0.8/
--rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-10 07:28:53.813423 taichu-serve-1.0.8/PKG-INFO
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 07:28:53.811767 taichu-serve-1.0.8/model_service/
--rw-r--r--   0 chen       (501) staff       (20)      188 2023-02-07 00:50:51.000000 taichu-serve-1.0.8/model_service/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     8760 2023-04-03 11:32:09.000000 taichu-serve-1.0.8/model_service/app.py
--rw-r--r--   0 chen       (501) staff       (20)     1584 2023-04-10 06:15:09.000000 taichu-serve-1.0.8/model_service/command.py
--rw-r--r--   0 chen       (501) staff       (20)      935 2023-04-03 11:34:16.000000 taichu-serve-1.0.8/model_service/common.py
--rw-r--r--   0 chen       (501) staff       (20)     1290 2023-04-03 11:12:47.000000 taichu-serve-1.0.8/model_service/error_code.py
--rw-r--r--   0 chen       (501) staff       (20)     6391 2023-04-03 09:59:12.000000 taichu-serve-1.0.8/model_service/grpc_predict_v2_pb2.py
--rw-r--r--   0 chen       (501) staff       (20)    12997 2023-04-03 09:59:12.000000 taichu-serve-1.0.8/model_service/grpc_predict_v2_pb2_grpc.py
--rw-r--r--   0 chen       (501) staff       (20)     3568 2023-04-03 11:36:45.000000 taichu-serve-1.0.8/model_service/grpc_server.py
--rw-r--r--   0 chen       (501) staff       (20)     2090 2023-04-03 11:30:51.000000 taichu-serve-1.0.8/model_service/log.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 07:28:53.812172 taichu-serve-1.0.8/model_service/model_def/
--rw-r--r--   0 chen       (501) staff       (20)        0 2023-02-07 00:50:51.000000 taichu-serve-1.0.8/model_service/model_def/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     1761 2023-02-07 00:50:51.000000 taichu-serve-1.0.8/model_service/model_def/model_def.py
--rw-r--r--   0 chen       (501) staff       (20)     5225 2023-04-03 06:17:46.000000 taichu-serve-1.0.8/model_service/model_service.py
--rw-r--r--   0 chen       (501) staff       (20)      418 2023-02-07 00:50:51.000000 taichu-serve-1.0.8/model_service/settings.py
--rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-10 07:28:53.813626 taichu-serve-1.0.8/setup.cfg
--rw-r--r--   0 chen       (501) staff       (20)      951 2023-04-10 07:28:41.000000 taichu-serve-1.0.8/setup.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 07:28:53.813209 taichu-serve-1.0.8/taichu_serve.egg-info/
--rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-10 07:28:53.000000 taichu-serve-1.0.8/taichu_serve.egg-info/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)      609 2023-04-10 07:28:53.000000 taichu-serve-1.0.8/taichu_serve.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-10 07:28:53.000000 taichu-serve-1.0.8/taichu_serve.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (501) staff       (20)       74 2023-04-10 07:28:53.000000 taichu-serve-1.0.8/taichu_serve.egg-info/entry_points.txt
--rw-r--r--   0 chen       (501) staff       (20)       58 2023-04-10 07:28:53.000000 taichu-serve-1.0.8/taichu_serve.egg-info/requires.txt
--rw-r--r--   0 chen       (501) staff       (20)       14 2023-04-10 07:28:53.000000 taichu-serve-1.0.8/taichu_serve.egg-info/top_level.txt
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 07:38:10.181559 taichu-serve-1.0.9/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-10 07:38:10.181397 taichu-serve-1.0.9/PKG-INFO
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 07:38:10.179576 taichu-serve-1.0.9/model_service/
+-rw-r--r--   0 chen       (501) staff       (20)      188 2023-02-07 00:50:51.000000 taichu-serve-1.0.9/model_service/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     8760 2023-04-03 11:32:09.000000 taichu-serve-1.0.9/model_service/app.py
+-rw-r--r--   0 chen       (501) staff       (20)     1578 2023-04-10 07:37:32.000000 taichu-serve-1.0.9/model_service/command.py
+-rw-r--r--   0 chen       (501) staff       (20)      935 2023-04-03 11:34:16.000000 taichu-serve-1.0.9/model_service/common.py
+-rw-r--r--   0 chen       (501) staff       (20)     1290 2023-04-03 11:12:47.000000 taichu-serve-1.0.9/model_service/error_code.py
+-rw-r--r--   0 chen       (501) staff       (20)     6391 2023-04-03 09:59:12.000000 taichu-serve-1.0.9/model_service/grpc_predict_v2_pb2.py
+-rw-r--r--   0 chen       (501) staff       (20)    12997 2023-04-03 09:59:12.000000 taichu-serve-1.0.9/model_service/grpc_predict_v2_pb2_grpc.py
+-rw-r--r--   0 chen       (501) staff       (20)     3568 2023-04-03 11:36:45.000000 taichu-serve-1.0.9/model_service/grpc_server.py
+-rw-r--r--   0 chen       (501) staff       (20)     2090 2023-04-03 11:30:51.000000 taichu-serve-1.0.9/model_service/log.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 07:38:10.179993 taichu-serve-1.0.9/model_service/model_def/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2023-02-07 00:50:51.000000 taichu-serve-1.0.9/model_service/model_def/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     1761 2023-02-07 00:50:51.000000 taichu-serve-1.0.9/model_service/model_def/model_def.py
+-rw-r--r--   0 chen       (501) staff       (20)     5225 2023-04-03 06:17:46.000000 taichu-serve-1.0.9/model_service/model_service.py
+-rw-r--r--   0 chen       (501) staff       (20)      418 2023-02-07 00:50:51.000000 taichu-serve-1.0.9/model_service/settings.py
+-rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-10 07:38:10.181604 taichu-serve-1.0.9/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      951 2023-04-10 07:37:55.000000 taichu-serve-1.0.9/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 07:38:10.181178 taichu-serve-1.0.9/taichu_serve.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-10 07:38:10.000000 taichu-serve-1.0.9/taichu_serve.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      609 2023-04-10 07:38:10.000000 taichu-serve-1.0.9/taichu_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-10 07:38:10.000000 taichu-serve-1.0.9/taichu_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)       74 2023-04-10 07:38:10.000000 taichu-serve-1.0.9/taichu_serve.egg-info/entry_points.txt
+-rw-r--r--   0 chen       (501) staff       (20)       58 2023-04-10 07:38:10.000000 taichu-serve-1.0.9/taichu_serve.egg-info/requires.txt
+-rw-r--r--   0 chen       (501) staff       (20)       14 2023-04-10 07:38:10.000000 taichu-serve-1.0.9/taichu_serve.egg-info/top_level.txt
```

### Comparing `taichu-serve-1.0.8/model_service/app.py` & `taichu-serve-1.0.9/model_service/app.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.8/model_service/command.py` & `taichu-serve-1.0.9/model_service/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 
             return grpc.RpcError(grpc.StatusCode.NOT_FOUND, e.message)
         return ret
 
 
 def infer_server_start():
     parser = argparse.ArgumentParser(description='Taichu Model Server')
-    parser.add_argument('--grpc_port', action="store", default=8889, type=int)
-    parser.add_argument('--http_port', action="store", default=8888, type=int)
-    parser.add_argument('--worker', action="store", default=100, type=int)
+    parser.add_argument('grpc_port', action="store", default=8889, type=int)
+    parser.add_argument('http_port', action="store", default=8888, type=int)
+    parser.add_argument('worker', action="store", default=100, type=int)
 
     args = parser.parse_args()
 
     server = grpc.server(futures.ThreadPoolExecutor(max_workers=args.worker),
                          maximum_concurrent_rpcs=args.worker,
                          interceptors=[MyUnaryServerInterceptor()])
     grpc_predict_v2_pb2_grpc.add_GRPCInferenceServiceServicer_to_server(GrpcModelService(), server)
```

### Comparing `taichu-serve-1.0.8/model_service/common.py` & `taichu-serve-1.0.9/model_service/common.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.8/model_service/error_code.py` & `taichu-serve-1.0.9/model_service/error_code.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.8/model_service/grpc_predict_v2_pb2.py` & `taichu-serve-1.0.9/model_service/grpc_predict_v2_pb2.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.8/model_service/grpc_predict_v2_pb2_grpc.py` & `taichu-serve-1.0.9/model_service/grpc_predict_v2_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.8/model_service/grpc_server.py` & `taichu-serve-1.0.9/model_service/grpc_server.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.8/model_service/log.py` & `taichu-serve-1.0.9/model_service/log.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.8/model_service/model_def/model_def.py` & `taichu-serve-1.0.9/model_service/model_def/model_def.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.8/model_service/model_service.py` & `taichu-serve-1.0.9/model_service/model_service.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-1.0.8/setup.py` & `taichu-serve-1.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 if __name__ == '__main__':
     name = 'taichu-serve'
 
     requirements = ['grpcio', 'grpcio-tools', 'protobuf', 'Flask', 'gunicorn', 'Jinja2', 'Pillow']
 
     setup(
         name=name,
-        version='1.0.8',
+        version='1.0.9',
         description='taichu serve is a tool for serving deep learning inference',
         # long_description='',
         author='taichu platform team',
         # author_email='noreply@noreply.com',
         python_requires=">=3.6.0",
         url='',
         keywords='Serving Deep Learning Inference AI',
```

### Comparing `taichu-serve-1.0.8/taichu_serve.egg-info/SOURCES.txt` & `taichu-serve-1.0.9/taichu_serve.egg-info/SOURCES.txt`

 * *Files identical despite different names*


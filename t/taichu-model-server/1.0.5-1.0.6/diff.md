# Comparing `tmp/taichu-model-server-1.0.5.tar.gz` & `tmp/taichu-model-server-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichu-model-server-1.0.5.tar", last modified: Mon Apr 10 06:34:32 2023, max compression
+gzip compressed data, was "taichu-model-server-1.0.6.tar", last modified: Mon Apr 10 07:08:56 2023, max compression
```

## Comparing `taichu-model-server-1.0.5.tar` & `taichu-model-server-1.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 06:34:32.796568 taichu-model-server-1.0.5/
--rw-r--r--   0 chen       (501) staff       (20)      195 2023-04-10 06:34:32.796348 taichu-model-server-1.0.5/PKG-INFO
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 06:34:32.794288 taichu-model-server-1.0.5/model_service/
--rw-r--r--   0 chen       (501) staff       (20)      188 2023-02-07 00:50:51.000000 taichu-model-server-1.0.5/model_service/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     8760 2023-04-03 11:32:09.000000 taichu-model-server-1.0.5/model_service/app.py
--rw-r--r--   0 chen       (501) staff       (20)     1584 2023-04-10 06:15:09.000000 taichu-model-server-1.0.5/model_service/command.py
--rw-r--r--   0 chen       (501) staff       (20)      935 2023-04-03 11:34:16.000000 taichu-model-server-1.0.5/model_service/common.py
--rw-r--r--   0 chen       (501) staff       (20)     1290 2023-04-03 11:12:47.000000 taichu-model-server-1.0.5/model_service/error_code.py
--rw-r--r--   0 chen       (501) staff       (20)     6391 2023-04-03 09:59:12.000000 taichu-model-server-1.0.5/model_service/grpc_predict_v2_pb2.py
--rw-r--r--   0 chen       (501) staff       (20)    12997 2023-04-03 09:59:12.000000 taichu-model-server-1.0.5/model_service/grpc_predict_v2_pb2_grpc.py
--rw-r--r--   0 chen       (501) staff       (20)     3568 2023-04-03 11:36:45.000000 taichu-model-server-1.0.5/model_service/grpc_server.py
--rw-r--r--   0 chen       (501) staff       (20)     2090 2023-04-03 11:30:51.000000 taichu-model-server-1.0.5/model_service/log.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 06:34:32.794691 taichu-model-server-1.0.5/model_service/model_def/
--rw-r--r--   0 chen       (501) staff       (20)        0 2023-02-07 00:50:51.000000 taichu-model-server-1.0.5/model_service/model_def/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     1761 2023-02-07 00:50:51.000000 taichu-model-server-1.0.5/model_service/model_def/model_def.py
--rw-r--r--   0 chen       (501) staff       (20)     5225 2023-04-03 06:17:46.000000 taichu-model-server-1.0.5/model_service/model_service.py
--rw-r--r--   0 chen       (501) staff       (20)      418 2023-02-07 00:50:51.000000 taichu-model-server-1.0.5/model_service/settings.py
--rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-10 06:34:32.796622 taichu-model-server-1.0.5/setup.cfg
--rw-r--r--   0 chen       (501) staff       (20)      904 2023-03-31 03:22:28.000000 taichu-model-server-1.0.5/setup.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 06:34:32.796080 taichu-model-server-1.0.5/taichu_model_server.egg-info/
--rw-r--r--   0 chen       (501) staff       (20)      195 2023-04-10 06:34:32.000000 taichu-model-server-1.0.5/taichu_model_server.egg-info/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)      651 2023-04-10 06:34:32.000000 taichu-model-server-1.0.5/taichu_model_server.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-10 06:34:32.000000 taichu-model-server-1.0.5/taichu_model_server.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (501) staff       (20)       75 2023-04-10 06:34:32.000000 taichu-model-server-1.0.5/taichu_model_server.egg-info/entry_points.txt
--rw-r--r--   0 chen       (501) staff       (20)       29 2023-04-10 06:34:32.000000 taichu-model-server-1.0.5/taichu_model_server.egg-info/requires.txt
--rw-r--r--   0 chen       (501) staff       (20)       14 2023-04-10 06:34:32.000000 taichu-model-server-1.0.5/taichu_model_server.egg-info/top_level.txt
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 07:08:56.947075 taichu-model-server-1.0.6/
+-rw-r--r--   0 chen       (501) staff       (20)      242 2023-04-10 07:08:56.946912 taichu-model-server-1.0.6/PKG-INFO
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 07:08:56.945136 taichu-model-server-1.0.6/model_service/
+-rw-r--r--   0 chen       (501) staff       (20)      188 2023-02-07 00:50:51.000000 taichu-model-server-1.0.6/model_service/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     8760 2023-04-03 11:32:09.000000 taichu-model-server-1.0.6/model_service/app.py
+-rw-r--r--   0 chen       (501) staff       (20)     1584 2023-04-10 06:15:09.000000 taichu-model-server-1.0.6/model_service/command.py
+-rw-r--r--   0 chen       (501) staff       (20)      935 2023-04-03 11:34:16.000000 taichu-model-server-1.0.6/model_service/common.py
+-rw-r--r--   0 chen       (501) staff       (20)     1290 2023-04-03 11:12:47.000000 taichu-model-server-1.0.6/model_service/error_code.py
+-rw-r--r--   0 chen       (501) staff       (20)     6391 2023-04-03 09:59:12.000000 taichu-model-server-1.0.6/model_service/grpc_predict_v2_pb2.py
+-rw-r--r--   0 chen       (501) staff       (20)    12997 2023-04-03 09:59:12.000000 taichu-model-server-1.0.6/model_service/grpc_predict_v2_pb2_grpc.py
+-rw-r--r--   0 chen       (501) staff       (20)     3568 2023-04-03 11:36:45.000000 taichu-model-server-1.0.6/model_service/grpc_server.py
+-rw-r--r--   0 chen       (501) staff       (20)     2090 2023-04-03 11:30:51.000000 taichu-model-server-1.0.6/model_service/log.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 07:08:56.945592 taichu-model-server-1.0.6/model_service/model_def/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2023-02-07 00:50:51.000000 taichu-model-server-1.0.6/model_service/model_def/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     1761 2023-02-07 00:50:51.000000 taichu-model-server-1.0.6/model_service/model_def/model_def.py
+-rw-r--r--   0 chen       (501) staff       (20)     5225 2023-04-03 06:17:46.000000 taichu-model-server-1.0.6/model_service/model_service.py
+-rw-r--r--   0 chen       (501) staff       (20)      418 2023-02-07 00:50:51.000000 taichu-model-server-1.0.6/model_service/settings.py
+-rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-10 07:08:56.947134 taichu-model-server-1.0.6/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      928 2023-04-10 07:08:53.000000 taichu-model-server-1.0.6/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-10 07:08:56.946697 taichu-model-server-1.0.6/taichu_model_server.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)      242 2023-04-10 07:08:56.000000 taichu-model-server-1.0.6/taichu_model_server.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      651 2023-04-10 07:08:56.000000 taichu-model-server-1.0.6/taichu_model_server.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-10 07:08:56.000000 taichu-model-server-1.0.6/taichu_model_server.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)       74 2023-04-10 07:08:56.000000 taichu-model-server-1.0.6/taichu_model_server.egg-info/entry_points.txt
+-rw-r--r--   0 chen       (501) staff       (20)       34 2023-04-10 07:08:56.000000 taichu-model-server-1.0.6/taichu_model_server.egg-info/requires.txt
+-rw-r--r--   0 chen       (501) staff       (20)       14 2023-04-10 07:08:56.000000 taichu-model-server-1.0.6/taichu_model_server.egg-info/top_level.txt
```

### Comparing `taichu-model-server-1.0.5/model_service/app.py` & `taichu-model-server-1.0.6/model_service/app.py`

 * *Files identical despite different names*

### Comparing `taichu-model-server-1.0.5/model_service/command.py` & `taichu-model-server-1.0.6/model_service/command.py`

 * *Files identical despite different names*

### Comparing `taichu-model-server-1.0.5/model_service/common.py` & `taichu-model-server-1.0.6/model_service/common.py`

 * *Files identical despite different names*

### Comparing `taichu-model-server-1.0.5/model_service/error_code.py` & `taichu-model-server-1.0.6/model_service/error_code.py`

 * *Files identical despite different names*

### Comparing `taichu-model-server-1.0.5/model_service/grpc_predict_v2_pb2.py` & `taichu-model-server-1.0.6/model_service/grpc_predict_v2_pb2.py`

 * *Files identical despite different names*

### Comparing `taichu-model-server-1.0.5/model_service/grpc_predict_v2_pb2_grpc.py` & `taichu-model-server-1.0.6/model_service/grpc_predict_v2_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `taichu-model-server-1.0.5/model_service/grpc_server.py` & `taichu-model-server-1.0.6/model_service/grpc_server.py`

 * *Files identical despite different names*

### Comparing `taichu-model-server-1.0.5/model_service/log.py` & `taichu-model-server-1.0.6/model_service/log.py`

 * *Files identical despite different names*

### Comparing `taichu-model-server-1.0.5/model_service/model_def/model_def.py` & `taichu-model-server-1.0.6/model_service/model_def/model_def.py`

 * *Files identical despite different names*

### Comparing `taichu-model-server-1.0.5/model_service/model_service.py` & `taichu-model-server-1.0.6/model_service/model_service.py`

 * *Files identical despite different names*

### Comparing `taichu-model-server-1.0.5/setup.py` & `taichu-model-server-1.0.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 import model_service
 
 pkgs = find_packages()
 
 if __name__ == '__main__':
     name = 'taichu-model-server'
 
-    requirements = ['Flask', 'gunicorn', 'Jinja2', 'Pillow']
+    requirements = ['grpc', 'Flask', 'gunicorn', 'Jinja2', 'Pillow']
 
     setup(
         name=name,
-        version='1.0.5',
-        description='基于华为modelarts_server重新导出',
+        version='1.0.6',
+        description='taichu serve is a tool for serving deep learning inference',
         # long_description='',
-        # author='Taichu platform team',
+        author='taichu platform team',
         # author_email='noreply@noreply.com',
         python_requires=">=3.6.0",
         url='',
         keywords='Serving Deep Learning Inference AI',
         packages=pkgs,
         install_requires=requirements,
         entry_points={
-            'console_scripts': ['taichu_server = model_service.command:infer_server_start']
+            'console_scripts': ['taichu_serve = model_service.command:infer_server_start']
         },
         include_package_data=True,
         # license='Apache License Version 2.0'
-    )
+    )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `taichu-model-server-1.0.5/taichu_model_server.egg-info/SOURCES.txt` & `taichu-model-server-1.0.6/taichu_model_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*


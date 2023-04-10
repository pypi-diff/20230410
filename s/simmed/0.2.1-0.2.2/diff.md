# Comparing `tmp/simmed-0.2.1.tar.gz` & `tmp/simmed-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simmed-0.2.1.tar", last modified: Mon Apr  3 02:09:50 2023, max compression
+gzip compressed data, was "simmed-0.2.2.tar", last modified: Mon Apr 10 03:15:25 2023, max compression
```

## Comparing `simmed-0.2.1.tar` & `simmed-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 andersonwei   (501) staff       (20)        0 2023-04-03 02:09:50.099323 simmed-0.2.1/
--rw-r--r--   0 andersonwei   (501) staff       (20)      167 2022-04-27 02:59:32.000000 simmed-0.2.1/.gitignore
--rw-r--r--   0 andersonwei   (501) staff       (20)     1047 2023-03-15 02:38:52.000000 simmed-0.2.1/LICENSE
--rw-r--r--   0 andersonwei   (501) staff       (20)       82 2023-03-15 02:36:06.000000 simmed-0.2.1/MANIFEST.in
--rw-r--r--   0 andersonwei   (501) staff       (20)     1520 2023-04-03 02:09:50.098663 simmed-0.2.1/PKG-INFO
--rw-r--r--   0 andersonwei   (501) staff       (20)      922 2023-03-10 03:37:40.000000 simmed-0.2.1/README.md
--rw-r--r--   0 andersonwei   (501) staff       (20)      523 2023-04-03 02:05:18.000000 simmed-0.2.1/pyproject.toml
--rw-r--r--   0 andersonwei   (501) staff       (20)      259 2023-03-15 02:54:08.000000 simmed-0.2.1/requirements.txt
--rw-r--r--   0 andersonwei   (501) staff       (20)       38 2023-04-03 02:09:50.099545 simmed-0.2.1/setup.cfg
--rw-r--r--   0 andersonwei   (501) staff       (20)     1172 2023-03-16 05:08:51.000000 simmed-0.2.1/setup.py
-drwxr-xr-x   0 andersonwei   (501) staff       (20)        0 2023-04-03 02:09:50.093140 simmed-0.2.1/simmed/
--rw-r--r--   0 andersonwei   (501) staff       (20)     6148 2023-03-10 05:52:00.000000 simmed-0.2.1/simmed/.DS_Store
--rw-rw-r--   0 andersonwei   (501) staff       (20)        0 2022-04-19 17:22:38.000000 simmed-0.2.1/simmed/__init__.py
--rw-r--r--   0 andersonwei   (501) staff       (20)      855 2023-03-13 09:57:22.000000 simmed-0.2.1/simmed/baseservice.py
--rw-r--r--   0 andersonwei   (501) staff       (20)     1083 2023-03-31 13:54:00.000000 simmed-0.2.1/simmed/config.py
--rw-r--r--   0 andersonwei   (501) staff       (20)     4923 2023-03-31 08:35:12.000000 simmed-0.2.1/simmed/info_base.py
--rw-r--r--   0 andersonwei   (501) staff       (20)     1565 2022-04-23 11:26:29.000000 simmed-0.2.1/simmed/jsonencoder.py
--rw-r--r--   0 andersonwei   (501) staff       (20)     2449 2023-03-13 07:28:25.000000 simmed-0.2.1/simmed/nacos_client.py
--rw-r--r--   0 andersonwei   (501) staff       (20)     4313 2023-03-03 13:19:07.000000 simmed-0.2.1/simmed/pymongos.py
--rw-r--r--   0 andersonwei   (501) staff       (20)      451 2023-03-10 03:29:48.000000 simmed-0.2.1/simmed/rpcrequest.py
--rw-r--r--   0 andersonwei   (501) staff       (20)      261 2023-03-10 03:30:18.000000 simmed-0.2.1/simmed/rpcresponse.py
--rw-r--r--   0 andersonwei   (501) staff       (20)      475 2023-03-13 01:27:05.000000 simmed-0.2.1/simmed/service_dispatcher.py
--rw-r--r--   0 andersonwei   (501) staff       (20)    18836 2023-03-31 13:59:24.000000 simmed-0.2.1/simmed/simmed_core.py
--rw-r--r--   0 andersonwei   (501) staff       (20)     1111 2023-03-10 03:34:37.000000 simmed-0.2.1/simmed/simmed_jsonrpc.py
--rw-r--r--   0 andersonwei   (501) staff       (20)     7894 2023-04-03 02:02:51.000000 simmed-0.2.1/simmed/swagger_gen.py
--rw-r--r--   0 andersonwei   (501) staff       (20)     4187 2023-03-13 07:30:14.000000 simmed-0.2.1/simmed/zipkin.py
-drwxr-xr-x   0 andersonwei   (501) staff       (20)        0 2023-04-03 02:09:50.097867 simmed-0.2.1/simmed.egg-info/
--rw-r--r--   0 andersonwei   (501) staff       (20)     1520 2023-04-03 02:09:49.000000 simmed-0.2.1/simmed.egg-info/PKG-INFO
--rw-r--r--   0 andersonwei   (501) staff       (20)      576 2023-04-03 02:09:50.000000 simmed-0.2.1/simmed.egg-info/SOURCES.txt
--rw-r--r--   0 andersonwei   (501) staff       (20)        1 2023-04-03 02:09:49.000000 simmed-0.2.1/simmed.egg-info/dependency_links.txt
--rw-r--r--   0 andersonwei   (501) staff       (20)        1 2023-04-03 02:06:50.000000 simmed-0.2.1/simmed.egg-info/not-zip-safe
--rw-r--r--   0 andersonwei   (501) staff       (20)      241 2023-04-03 02:09:49.000000 simmed-0.2.1/simmed.egg-info/requires.txt
--rw-r--r--   0 andersonwei   (501) staff       (20)        7 2023-04-03 02:09:49.000000 simmed-0.2.1/simmed.egg-info/top_level.txt
+drwxr-xr-x   0 andersonwei   (501) staff       (20)        0 2023-04-10 03:15:25.218715 simmed-0.2.2/
+-rw-r--r--   0 andersonwei   (501) staff       (20)      167 2022-04-27 02:59:32.000000 simmed-0.2.2/.gitignore
+-rw-r--r--   0 andersonwei   (501) staff       (20)     1047 2023-03-15 02:38:52.000000 simmed-0.2.2/LICENSE
+-rw-r--r--   0 andersonwei   (501) staff       (20)       82 2023-03-15 02:36:06.000000 simmed-0.2.2/MANIFEST.in
+-rw-r--r--   0 andersonwei   (501) staff       (20)     1528 2023-04-10 03:15:25.218293 simmed-0.2.2/PKG-INFO
+-rw-r--r--   0 andersonwei   (501) staff       (20)      922 2023-03-10 03:37:40.000000 simmed-0.2.2/README.md
+-rw-r--r--   0 andersonwei   (501) staff       (20)      523 2023-04-10 03:13:17.000000 simmed-0.2.2/pyproject.toml
+-rw-r--r--   0 andersonwei   (501) staff       (20)      276 2023-04-04 03:03:44.000000 simmed-0.2.2/requirements.txt
+-rw-r--r--   0 andersonwei   (501) staff       (20)       38 2023-04-10 03:15:25.218846 simmed-0.2.2/setup.cfg
+-rw-r--r--   0 andersonwei   (501) staff       (20)     1208 2023-04-10 03:14:20.000000 simmed-0.2.2/setup.py
+drwxr-xr-x   0 andersonwei   (501) staff       (20)        0 2023-04-10 03:15:25.214083 simmed-0.2.2/simmed/
+-rw-r--r--   0 andersonwei   (501) staff       (20)     6148 2023-03-10 05:52:00.000000 simmed-0.2.2/simmed/.DS_Store
+-rw-rw-r--   0 andersonwei   (501) staff       (20)        0 2022-04-19 17:22:38.000000 simmed-0.2.2/simmed/__init__.py
+-rw-r--r--   0 andersonwei   (501) staff       (20)      855 2023-03-13 09:57:22.000000 simmed-0.2.2/simmed/baseservice.py
+-rw-r--r--   0 andersonwei   (501) staff       (20)     1083 2023-03-31 13:54:00.000000 simmed-0.2.2/simmed/config.py
+-rw-r--r--   0 andersonwei   (501) staff       (20)     4923 2023-03-31 08:35:12.000000 simmed-0.2.2/simmed/info_base.py
+-rw-r--r--   0 andersonwei   (501) staff       (20)     1565 2022-04-23 11:26:29.000000 simmed-0.2.2/simmed/jsonencoder.py
+-rw-r--r--   0 andersonwei   (501) staff       (20)     2449 2023-03-13 07:28:25.000000 simmed-0.2.2/simmed/nacos_client.py
+-rw-r--r--   0 andersonwei   (501) staff       (20)     4313 2023-03-03 13:19:07.000000 simmed-0.2.2/simmed/pymongos.py
+-rw-r--r--   0 andersonwei   (501) staff       (20)      451 2023-03-10 03:29:48.000000 simmed-0.2.2/simmed/rpcrequest.py
+-rw-r--r--   0 andersonwei   (501) staff       (20)      261 2023-03-10 03:30:18.000000 simmed-0.2.2/simmed/rpcresponse.py
+-rw-r--r--   0 andersonwei   (501) staff       (20)      475 2023-03-13 01:27:05.000000 simmed-0.2.2/simmed/service_dispatcher.py
+-rw-r--r--   0 andersonwei   (501) staff       (20)    18836 2023-03-31 13:59:24.000000 simmed-0.2.2/simmed/simmed_core.py
+-rw-r--r--   0 andersonwei   (501) staff       (20)     1111 2023-03-10 03:34:37.000000 simmed-0.2.2/simmed/simmed_jsonrpc.py
+-rw-r--r--   0 andersonwei   (501) staff       (20)     8482 2023-04-10 03:13:00.000000 simmed-0.2.2/simmed/swagger_gen.py
+-rw-r--r--   0 andersonwei   (501) staff       (20)     4187 2023-03-13 07:30:14.000000 simmed-0.2.2/simmed/zipkin.py
+drwxr-xr-x   0 andersonwei   (501) staff       (20)        0 2023-04-10 03:15:25.217695 simmed-0.2.2/simmed.egg-info/
+-rw-r--r--   0 andersonwei   (501) staff       (20)     1528 2023-04-10 03:15:25.000000 simmed-0.2.2/simmed.egg-info/PKG-INFO
+-rw-r--r--   0 andersonwei   (501) staff       (20)      576 2023-04-10 03:15:25.000000 simmed-0.2.2/simmed.egg-info/SOURCES.txt
+-rw-r--r--   0 andersonwei   (501) staff       (20)        1 2023-04-10 03:15:25.000000 simmed-0.2.2/simmed.egg-info/dependency_links.txt
+-rw-r--r--   0 andersonwei   (501) staff       (20)        1 2023-04-03 02:06:50.000000 simmed-0.2.2/simmed.egg-info/not-zip-safe
+-rw-r--r--   0 andersonwei   (501) staff       (20)      258 2023-04-10 03:15:25.000000 simmed-0.2.2/simmed.egg-info/requires.txt
+-rw-r--r--   0 andersonwei   (501) staff       (20)        7 2023-04-10 03:15:25.000000 simmed-0.2.2/simmed.egg-info/top_level.txt
```

### Comparing `simmed-0.2.1/LICENSE` & `simmed-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simmed-0.2.1/PKG-INFO` & `simmed-0.2.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simmed
-Version: 0.2.1
+Version: 0.2.2
 Summary: 微服务基础框架
 Home-page: https://simmed.cn
-Author: weizw,lijunhua
+Author: weizw,lijunhua,zhaoyun
 Author-email: weizw <weizhuwang@simmed.cn>, defa <lijunnhua@simmed.cn>, zhaoyun <zhaoyun@simmed.cn>
 License: MIT
 Project-URL: Homepage, https://simmed.cn
 Project-URL: Bug Tracker, https://simmed.cn
 Keywords: simmed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `simmed-0.2.1/README.md` & `simmed-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `simmed-0.2.1/pyproject.toml` & `simmed-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "simmed"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="weizw", email="weizhuwang@simmed.cn" },
   { name="defa", email="lijunnhua@simmed.cn" },
   { name="zhaoyun", email="zhaoyun@simmed.cn" },
 ]
 description = "微服务基础框架"
 readme = "README.md"
```

### Comparing `simmed-0.2.1/setup.py` & `simmed-0.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,34 +14,35 @@
     print('INFO del dir ', path)
     shutil.rmtree(path)
 
 print("find_packages:", find_packages())
 
 setup(
     name='simmed',
-    version='0.2.1',
+    version='0.2.2',
     description="simmed core sdk",
-    author='weizw,lijunhua',
+    author='weizw,lijunhua,zhaoyun',
     author_email='wzw@simmed.cn',
     url='https://simmed.cn',
     install_requires=[
         'flasgger==0.9.5',
         'flask==1.1.2',
         'Flask-Compress==1.10.1',
         'nacos_sdk_python==0.1.6',
         'thriftpy2==0.4.14',
         'py_zipkin==0.20.2',
         'pyctuator==0.17.0',
         'pymongo==3.12.1',
         'PyYAML==5.4.1',
-        'requests==2.22.0',
+        'requests==2.28.2',
         'Werkzeug==1.0.1',
         'Flask-Cors==3.0.9',
         'redis==3.2.1',
-        'pydantic==1.10.5'
+        'pydantic==1.10.5',
+        'json-rpc==1.14.0'
     ],
     include_package_data=True,
     zip_safe=False,
     platforms='any',
     python_requires='>=3.8, <4',
     keywords='simmed',
     license="MIT",
```

### Comparing `simmed-0.2.1/simmed/.DS_Store` & `simmed-0.2.2/simmed/.DS_Store`

 * *Files identical despite different names*

### Comparing `simmed-0.2.1/simmed/baseservice.py` & `simmed-0.2.2/simmed/baseservice.py`

 * *Files identical despite different names*

### Comparing `simmed-0.2.1/simmed/config.py` & `simmed-0.2.2/simmed/config.py`

 * *Files identical despite different names*

### Comparing `simmed-0.2.1/simmed/info_base.py` & `simmed-0.2.2/simmed/info_base.py`

 * *Files identical despite different names*

### Comparing `simmed-0.2.1/simmed/jsonencoder.py` & `simmed-0.2.2/simmed/jsonencoder.py`

 * *Files identical despite different names*

### Comparing `simmed-0.2.1/simmed/nacos_client.py` & `simmed-0.2.2/simmed/nacos_client.py`

 * *Files identical despite different names*

### Comparing `simmed-0.2.1/simmed/pymongos.py` & `simmed-0.2.2/simmed/pymongos.py`

 * *Files identical despite different names*

### Comparing `simmed-0.2.1/simmed/simmed_core.py` & `simmed-0.2.2/simmed/simmed_core.py`

 * *Files identical despite different names*

### Comparing `simmed-0.2.1/simmed/simmed_jsonrpc.py` & `simmed-0.2.2/simmed/simmed_jsonrpc.py`

 * *Files identical despite different names*

### Comparing `simmed-0.2.1/simmed/swagger_gen.py` & `simmed-0.2.2/simmed/swagger_gen.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,48 +185,55 @@
             schema[field_name]['type'] = 'list'
             args = get_args(field_type)
             if len(args) > 0:
                 in_type = args[0]
                 if in_type != cls:
                     tmp_schema = get_validate_schema(in_type)
                     if issubclass(in_type, BaseModel) or get_origin(in_type) is dict:
-                        schema[field_name]['items'] = [{
+                        schema[field_name]['schema'] = {
                             'type': 'dict',
                             'schema': tmp_schema
-                        }]
+                        }
                     else:
-                        schema[field_name]['items'] = [tmp_schema]
+                        schema[field_name]['schema'] = tmp_schema
 
         elif get_origin(field_type) is dict:
             schema[field_name]['type'] = 'dict'
             schema[field_name]['allow_unknown'] = True
 
         else:
             if issubclass(field_type, BaseModel):
                 schema[field_name]['type'] = 'dict'
                 schema[field_name]['schema'] = get_validate_schema(field_type)
 
-        if 'required' in field_info.extra and field_info.extra['required']:
-            schema[field_name]['required'] = field_info.extra['required']
+        # if 'required' in field_info.extra and field_info.extra['required']:
+        #     schema[field_name]['required'] = field_info.extra['required']
 
-        if field_info.ge or field_info.gt:
+        if field_info.ge is not None or field_info.gt is not None:
             schema[field_name]['min'] = field_info.ge if field_info.ge else field_info.gt
 
-        if field_info.le or field_info.lt:
+        if field_info.le is not None or field_info.lt is not None:
             schema[field_name]['max'] = field_info.le if field_info.le else field_info.lt
 
-        if field_info.min_length:
-            schema[field_name]['minlength'] = field_info.min_length
+        # str约束min_length list约束min_items  cerberus不区分list与str类型field_info区分
+        if field_info.min_length is not None or field_info.min_items is not None:
+            schema[field_name]['minlength'] = field_info.min_length if field_info.min_length else field_info.min_items
 
-        if field_info.max_length:
-            schema[field_name]['maxlength'] = field_info.max_length
+        if field_info.max_length is not None or field_info.max_items is not None:
+            schema[field_name]['maxlength'] = field_info.max_length if field_info.max_length else field_info.max_items
 
         if field_info.regex:
             schema[field_name]['regex'] = field_info.regex
 
+        if field_info.extra:
+            for extra_key, extra_value in field_info.extra.items():
+                if extra_key in schema[field_name]:
+                    continue
+                schema[field_name][extra_key] = extra_value
+
     return schema
 
 
 def get_validate_field_type_str(typeinfo):
     '''获取校验属性类型'''
 
     if typeinfo == bool:
```

### Comparing `simmed-0.2.1/simmed/zipkin.py` & `simmed-0.2.2/simmed/zipkin.py`

 * *Files identical despite different names*

### Comparing `simmed-0.2.1/simmed.egg-info/PKG-INFO` & `simmed-0.2.2/simmed.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simmed
-Version: 0.2.1
+Version: 0.2.2
 Summary: 微服务基础框架
 Home-page: https://simmed.cn
-Author: weizw,lijunhua
+Author: weizw,lijunhua,zhaoyun
 Author-email: weizw <weizhuwang@simmed.cn>, defa <lijunnhua@simmed.cn>, zhaoyun <zhaoyun@simmed.cn>
 License: MIT
 Project-URL: Homepage, https://simmed.cn
 Project-URL: Bug Tracker, https://simmed.cn
 Keywords: simmed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `simmed-0.2.1/simmed.egg-info/SOURCES.txt` & `simmed-0.2.2/simmed.egg-info/SOURCES.txt`

 * *Files identical despite different names*


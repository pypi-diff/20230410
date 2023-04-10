# Comparing `tmp/keepvariable-1.0.1.tar.gz` & `tmp/keepvariable-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keepvariable-1.0.1.tar", last modified: Sun Mar 12 22:58:52 2023, max compression
+gzip compressed data, was "keepvariable-1.0.2.tar", last modified: Mon Apr 10 03:43:28 2023, max compression
```

## Comparing `keepvariable-1.0.1.tar` & `keepvariable-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-12 22:58:52.770192 keepvariable-1.0.1/
--rw-rw-rw-   0        0        0     1247 2021-03-10 00:11:59.000000 keepvariable-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      675 2023-03-12 22:58:52.769193 keepvariable-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      122 2021-03-10 00:11:59.000000 keepvariable-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-12 22:58:52.753235 keepvariable-1.0.1/keepvariable/
--rw-rw-rw-   0        0        0        0 2021-03-10 00:11:59.000000 keepvariable-1.0.1/keepvariable/__init__.py
--rw-rw-rw-   0        0        0     6643 2023-03-12 22:53:58.000000 keepvariable-1.0.1/keepvariable/keepvariable_core.py
--rw-rw-rw-   0        0        0      295 2021-03-10 00:11:59.000000 keepvariable-1.0.1/keepvariable/keepvariable_model.py
--rw-rw-rw-   0        0        0      623 2023-03-12 22:57:47.000000 keepvariable-1.0.1/keepvariable/kv_redis_example.py
-drwxrwxrwx   0        0        0        0 2023-03-12 22:58:52.768195 keepvariable-1.0.1/keepvariable.egg-info/
--rw-rw-rw-   0        0        0      675 2023-03-12 22:58:52.000000 keepvariable-1.0.1/keepvariable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-03-12 22:58:52.000000 keepvariable-1.0.1/keepvariable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-12 22:58:52.000000 keepvariable-1.0.1/keepvariable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-03-12 22:58:52.000000 keepvariable-1.0.1/keepvariable.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-12 22:58:52.770192 keepvariable-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      795 2023-03-12 22:58:17.000000 keepvariable-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:43:28.144216 keepvariable-1.0.2/
+-rw-rw-rw-   0        0        0     1247 2021-03-10 00:11:59.000000 keepvariable-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2146 2023-04-10 03:43:28.144216 keepvariable-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1593 2023-04-10 03:42:53.000000 keepvariable-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 03:43:28.131251 keepvariable-1.0.2/keepvariable/
+-rw-rw-rw-   0        0        0        0 2021-03-10 00:11:59.000000 keepvariable-1.0.2/keepvariable/__init__.py
+-rw-rw-rw-   0        0        0     7343 2023-04-10 03:41:22.000000 keepvariable-1.0.2/keepvariable/keepvariable_core.py
+-rw-rw-rw-   0        0        0      295 2021-03-10 00:11:59.000000 keepvariable-1.0.2/keepvariable/keepvariable_model.py
+-rw-rw-rw-   0        0        0      715 2023-04-10 03:41:38.000000 keepvariable-1.0.2/keepvariable/kv_redis_example.py
+drwxrwxrwx   0        0        0        0 2023-04-10 03:43:28.143219 keepvariable-1.0.2/keepvariable.egg-info/
+-rw-rw-rw-   0        0        0     2146 2023-04-10 03:43:27.000000 keepvariable-1.0.2/keepvariable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-04-10 03:43:28.000000 keepvariable-1.0.2/keepvariable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 03:43:27.000000 keepvariable-1.0.2/keepvariable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 03:43:27.000000 keepvariable-1.0.2/keepvariable.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 03:43:28.144216 keepvariable-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      795 2023-04-10 03:43:24.000000 keepvariable-1.0.2/setup.py
```

### Comparing `keepvariable-1.0.1/LICENSE` & `keepvariable-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `keepvariable-1.0.1/keepvariable/keepvariable_core.py` & `keepvariable-1.0.2/keepvariable/keepvariable_core.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     try:
         keyword=string.split("=")[1].split("(")[0].strip()
         varname=string.split("=")[0].strip()
     except:
         keyword=""
         varname=""
     return(varname,keyword,inputs)
-
+ 
 kept_variables={}
 
 class Var:
     def __new__(cls,var):
         definition=get_definition(2,var)
         varname,keyword,inputs=analyze_definition(definition)
         joined_inputs=",".join(inputs)
@@ -125,17 +125,60 @@
             item.elements.pop(index)
               
             
     def __str__(self):
         return(str(self.elements))
    
     
-   
+class KeepVariableDummyRedisServer:
+    def __init__(self,host="localhost"):
+        self.host=host
+        self.storage={}
+        
+    def parse_saved_value(self,value):
+        if isinstance(value,list) or isinstance(value,bool) or isinstance(value,dict):
+            value=json.dumps(value)
+        elif isinstance(value,pd.DataFrame):
+            data=value.values.tolist()
+            columns=list(value.columns)
+            final_data={"columns":columns,"data":data,"object_type":"pd.DataFrame"}
+            print(final_data)
+            value=json.dumps(final_data)
+        elif isinstance(value,np.ndarray):
+            data=value.tolist()
+            final_data={"data":data,"object_type":"np.ndarray"}
+            value=json.dumps(final_data)
+        return(value)
+    
+    def decode_loaded_value(self,value):
+        try:
+            value=json.loads(value)
+            if "object_type" in value and isinstance(value,dict):
+                if value["object_type"]=="pd.DataFrame":
+                    df=pd.DataFrame(value["data"],columns=value["columns"])
+                    return(df)
+                elif value["object_type"]=="np.ndarray":
+                    array=pd.DataFrame(value["data"]).values #to ensure 64bit values in array
+                    return(array)
+            return(value)
+        except json.JSONDecodeError: #if type is str, it fails to decode
+            return(value)
+        
+        
+    def set(self,key,value):
+        value=self.parse_saved_value(value)
+        self.storage[key]=value
+        return({key:value})
+
+    def get(self,key):
+        value=self.storage.get(key)
+        decoded_value=self.decode_loaded_value(value)
+        return(decoded_value)
     
-class KeepVariableRedisServer:
+class KeepVariableRedisServer(KeepVariableDummyRedisServer):
     def __init__(self,host="localhost",port=6379,password=None):
         self.host=host
         self.port=port
         self.password=password
         
         self.redis = redis.Redis(host=self.host, port=self.port, db=0,password=self.password,decode_responses=True,charset="utf-8")
     
@@ -144,38 +187,17 @@
         return(self._kept_variables)
     
     @kept_variables.setter
     def kept_variables(self,kept_variables):
         return(self._kept_variables)
     
     def set(self,key,value):
-        if isinstance(value,list) or isinstance(value,bool) or isinstance(value,dict):
-            value=json.dumps(value)
-        elif isinstance(value,pd.DataFrame):
-            data=value.values.tolist()
-            columns=list(value.columns)
-            final_data={"columns":columns,"data":data,"object_type":"pd.DataFrame"}
-            print(final_data)
-            value=json.dumps(final_data)
-        elif isinstance(value,np.ndarray):
-            data=value.tolist()
-            final_data={"data":data,"object_type":"np.ndarray"}
-            value=json.dumps(final_data)
+        value=self.parse_saved_value(value)
         result=self.redis.set(key,value)
         return(result)
         
     def get(self,key):
-        result=self.redis.get(key)
-        try:
-            result=json.loads(result)
-            if "object_type" in result and isinstance(result,dict):
-                if result["object_type"]=="pd.DataFrame":
-                    df=pd.DataFrame(result["data"],columns=result["columns"])
-                    return(df)
-                elif result["object_type"]=="np.ndarray":
-                    array=pd.DataFrame(result["data"]).values #to ensure 64bit values in array
-                    return(array)
-            return(result)
-        except json.JSONDecodeError: #if type is str, it fails to decode
-            return(result)
+        value=self.redis.get(key)
+        decoded_value=self.decode_loaded_value(value)
+        return(decoded_value)
```

### Comparing `keepvariable-1.0.1/setup.py` & `keepvariable-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='keepvariable',
-    version='1.0.1',
+    version='1.0.2',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='A Python package keeping the values of variables between separate runs in a seamless and effortless way.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/keepvariable',
     packages=setuptools.find_packages(),
```


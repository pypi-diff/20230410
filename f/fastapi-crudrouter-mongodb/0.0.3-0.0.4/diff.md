# Comparing `tmp/fastapi-crudrouter-mongodb-0.0.3.tar.gz` & `tmp/fastapi-crudrouter-mongodb-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-crudrouter-mongodb-0.0.3.tar", last modified: Sun Apr  9 20:01:08 2023, max compression
+gzip compressed data, was "fastapi-crudrouter-mongodb-0.0.4.tar", last modified: Mon Apr 10 12:03:58 2023, max compression
```

## Comparing `fastapi-crudrouter-mongodb-0.0.3.tar` & `fastapi-crudrouter-mongodb-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 20:01:08.795508 fastapi-crudrouter-mongodb-0.0.3/
--rw-r--r--   0 pierro    (1000) pierro    (1000)     1070 2023-04-09 10:32:33.000000 fastapi-crudrouter-mongodb-0.0.3/LICENSE
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     4394 2023-04-09 20:01:08.795508 fastapi-crudrouter-mongodb-0.0.3/PKG-INFO
--rw-r--r--   0 pierro    (1000) pierro    (1000)     3032 2023-04-09 19:48:39.000000 fastapi-crudrouter-mongodb-0.0.3/README.md
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 20:01:08.791508 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      279 2023-04-09 20:00:41.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 20:01:08.791508 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      177 2023-04-09 11:15:45.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 20:01:08.795508 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/models/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      134 2023-04-09 10:58:04.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/models/CRUDEmbed.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      384 2023-04-09 10:54:52.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/models/CRUDLookup.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      191 2023-04-09 11:09:33.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/models/__init__.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1145 2023-04-09 10:50:18.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/models/mongo_model.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      400 2023-04-09 10:50:03.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/models/mongo_object_id_model.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 20:01:08.795508 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     6253 2023-04-09 19:39:43.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/CRUDRouter.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1464 2023-04-09 10:51:15.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/CRUDRouterFactory.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1963 2023-04-09 19:40:02.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/CRUDRouterRepository.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      220 2023-04-09 11:17:14.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 20:01:08.795508 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/embed/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     5101 2023-04-09 11:00:10.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouter.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1433 2023-04-09 10:59:36.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterFactory.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     3152 2023-04-09 19:57:13.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterRepository.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)       82 2023-04-09 11:18:46.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/embed/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 20:01:08.795508 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/lookup/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     6480 2023-04-09 10:57:21.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouter.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1432 2023-04-09 19:40:37.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterFactory.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     3730 2023-04-09 10:57:30.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterRepository.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)       86 2023-04-09 11:18:20.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/lookup/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 20:01:08.791508 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb.egg-info/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     4394 2023-04-09 20:01:08.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb.egg-info/PKG-INFO
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1398 2023-04-09 20:01:08.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb.egg-info/SOURCES.txt
--rw-rw-r--   0 pierro    (1000) pierro    (1000)        1 2023-04-09 20:01:08.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb.egg-info/dependency_links.txt
--rw-rw-r--   0 pierro    (1000) pierro    (1000)       31 2023-04-09 20:01:08.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb.egg-info/requires.txt
--rw-rw-r--   0 pierro    (1000) pierro    (1000)       27 2023-04-09 20:01:08.000000 fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb.egg-info/top_level.txt
--rw-rw-r--   0 pierro    (1000) pierro    (1000)       38 2023-04-09 20:01:08.795508 fastapi-crudrouter-mongodb-0.0.3/setup.cfg
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1720 2023-04-09 20:00:37.000000 fastapi-crudrouter-mongodb-0.0.3/setup.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-10 12:03:58.899207 fastapi-crudrouter-mongodb-0.0.4/
+-rw-r--r--   0 pierro    (1000) pierro    (1000)     1070 2023-04-09 10:32:33.000000 fastapi-crudrouter-mongodb-0.0.4/LICENSE
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     4732 2023-04-10 12:03:58.899207 fastapi-crudrouter-mongodb-0.0.4/PKG-INFO
+-rw-r--r--   0 pierro    (1000) pierro    (1000)     3370 2023-04-10 11:52:16.000000 fastapi-crudrouter-mongodb-0.0.4/README.md
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-10 12:03:58.895207 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      279 2023-04-10 12:03:13.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-10 12:03:58.899207 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      177 2023-04-09 11:15:45.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-10 12:03:58.899207 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/models/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      134 2023-04-09 10:58:04.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/models/CRUDEmbed.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      384 2023-04-09 10:54:52.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/models/CRUDLookup.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      191 2023-04-09 11:09:33.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/models/__init__.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1145 2023-04-09 10:50:18.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/models/mongo_model.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      400 2023-04-09 10:50:03.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/models/mongo_object_id_model.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-10 12:03:58.899207 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     6253 2023-04-09 19:39:43.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/CRUDRouter.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1464 2023-04-09 10:51:15.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/CRUDRouterFactory.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1963 2023-04-09 19:40:02.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/CRUDRouterRepository.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      220 2023-04-09 11:17:14.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-10 12:03:58.899207 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/embed/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     5101 2023-04-09 11:00:10.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouter.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1433 2023-04-09 10:59:36.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterFactory.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     3152 2023-04-09 19:57:13.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterRepository.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)       82 2023-04-09 11:18:46.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/embed/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-10 12:03:58.899207 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/lookup/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     6480 2023-04-09 10:57:21.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouter.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1432 2023-04-09 19:40:37.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterFactory.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     3730 2023-04-09 10:57:30.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterRepository.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)       86 2023-04-09 11:18:20.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/lookup/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-10 12:03:58.899207 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb.egg-info/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     4732 2023-04-10 12:03:58.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb.egg-info/PKG-INFO
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1398 2023-04-10 12:03:58.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb.egg-info/SOURCES.txt
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)        1 2023-04-10 12:03:58.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb.egg-info/dependency_links.txt
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)       31 2023-04-10 12:03:58.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb.egg-info/requires.txt
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)       27 2023-04-10 12:03:58.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb.egg-info/top_level.txt
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)       38 2023-04-10 12:03:58.899207 fastapi-crudrouter-mongodb-0.0.4/setup.cfg
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1720 2023-04-10 12:03:09.000000 fastapi-crudrouter-mongodb-0.0.4/setup.py
```

### Comparing `fastapi-crudrouter-mongodb-0.0.3/LICENSE` & `fastapi-crudrouter-mongodb-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.3/PKG-INFO` & `fastapi-crudrouter-mongodb-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-crudrouter-mongodb
-Version: 0.0.3
+Version: 0.0.4
 Summary: A dynamic FastAPI router that automatically creates CRUD routes for your mongodb models
 Home-page: https://github.com/pierrod/fastapi-crudrouter-mongodb
 Author: Pierre DUVEAU
 Author-email: 
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Internet
@@ -25,32 +25,37 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
+  <img src="./docs/assets/img/logo-long-color.png" height="200" />
+</p>
+<p align="center">
   <em>⚡ Create CRUD routes with lighting speed</em> ⚡</br>
   <sub>A dynamic FastAPI router that automatically creates CRUD routes for your Mongodb models</sub>
 </p>
 
---- 
+---
+
+**Documentation**: [https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/)
 
-**Documentation**: 
+**Source Code**: [https://github.com/pierrod/fastapi-crudrouter-mongodb](https://github.com/pierrod/fastapi-crudrouter-mongodb)
 
-**Source Code**: https://github.com/pierrod/fastapi-crudrouter-mongodb
+**Credits** :
 
-**Credits** : 
 - Base projet and idea : [awtkns](https://github.com/awtkns/fastapi-crudrouter)
 
-- Convert _id to id : [mclate github guide](https://github.com/tiangolo/fastapi/issues/1515)
+- Convert \_id to id : [mclate github guide](https://github.com/tiangolo/fastapi/issues/1515)
+
 ---
 
 Tired of rewriting generic CRUD routes? Need to rapidly prototype a feature for a presentation
-or a hackathon? Thankfully, [fastapi-crudrouter-mongodb](https://github.com/awtkns/fastapi-crudrouter-mongodb) has your back. 
+or a hackathon? Thankfully, [fastapi-crudrouter-mongodb](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/) has your back.
 
 As an extension to the APIRouter included with [FastAPI](https://fastapi.tiangolo.com/), the FastAPI CRUDRouter will automatically
 generate and document your CRUD routes for you, all you have to do is pass your model and maybe your database connection.
 
 ## Installation
 
 ```bash
@@ -66,15 +71,15 @@
 from typing import List, Optional, Union
 from fastapi import FastAPI
 from pydantic import Field
 from fastapi_crudrouter_mongodb import CRUDRouter, MongoModel, MongoObjectId, CRUDLookup
 import motor.motor_asyncio
 
 
-# Database connection using motor 
+# Database connection using motor
 client = motor.motor_asyncio.AsyncIOMotorClient(
     "mongodb://localhost:27017/local")
 
 db = client.local
 
 # Models
 class MessageModel(MongoModel):
@@ -93,17 +98,17 @@
 
 class UserModel(MongoModel):
     id: Optional[MongoObjectId] = Field()
     name: str
     email: str
     addresses: Optional[List[AddressModel]]
     messages: Optional[Union[List[MessageModel], MessageModel]] = None
-    
 
-# Instantiating the CRUDRouter, and a lookup for the messages 
+
+# Instantiating the CRUDRouter, and a lookup for the messages
 # a User is a model that contains a list of embedded addresses and related to multiple messages
 messages_lookup = CRUDLookup(
         model=MessageModel,
         collection_name="messages",
         prefix="messages",
         local_field="_id",
         foreign_field="user_id"
@@ -125,7 +130,8 @@
 
 ## OpenAPI Support
 
 By default, all routes generated by the CRUDRouter will be documented according to OpenAPI spec.
 
 Below are the default routes created by the CRUDRouter shown in the generated OpenAPI documentation.
 
+![CRUDRouter full OpenAPI image](./docs/assets/img/crud-router-full.png)
```

### Comparing `fastapi-crudrouter-mongodb-0.0.3/README.md` & `fastapi-crudrouter-mongodb-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 <p align="center">
+  <img src="./docs/assets/img/logo-long-color.png" height="200" />
+</p>
+<p align="center">
   <em>⚡ Create CRUD routes with lighting speed</em> ⚡</br>
   <sub>A dynamic FastAPI router that automatically creates CRUD routes for your Mongodb models</sub>
 </p>
 
---- 
+---
+
+**Documentation**: [https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/)
 
-**Documentation**: 
+**Source Code**: [https://github.com/pierrod/fastapi-crudrouter-mongodb](https://github.com/pierrod/fastapi-crudrouter-mongodb)
 
-**Source Code**: https://github.com/pierrod/fastapi-crudrouter-mongodb
+**Credits** :
 
-**Credits** : 
 - Base projet and idea : [awtkns](https://github.com/awtkns/fastapi-crudrouter)
 
-- Convert _id to id : [mclate github guide](https://github.com/tiangolo/fastapi/issues/1515)
+- Convert \_id to id : [mclate github guide](https://github.com/tiangolo/fastapi/issues/1515)
+
 ---
 
 Tired of rewriting generic CRUD routes? Need to rapidly prototype a feature for a presentation
-or a hackathon? Thankfully, [fastapi-crudrouter-mongodb](https://github.com/awtkns/fastapi-crudrouter-mongodb) has your back. 
+or a hackathon? Thankfully, [fastapi-crudrouter-mongodb](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/) has your back.
 
 As an extension to the APIRouter included with [FastAPI](https://fastapi.tiangolo.com/), the FastAPI CRUDRouter will automatically
 generate and document your CRUD routes for you, all you have to do is pass your model and maybe your database connection.
 
 ## Installation
 
 ```bash
@@ -36,15 +41,15 @@
 from typing import List, Optional, Union
 from fastapi import FastAPI
 from pydantic import Field
 from fastapi_crudrouter_mongodb import CRUDRouter, MongoModel, MongoObjectId, CRUDLookup
 import motor.motor_asyncio
 
 
-# Database connection using motor 
+# Database connection using motor
 client = motor.motor_asyncio.AsyncIOMotorClient(
     "mongodb://localhost:27017/local")
 
 db = client.local
 
 # Models
 class MessageModel(MongoModel):
@@ -63,17 +68,17 @@
 
 class UserModel(MongoModel):
     id: Optional[MongoObjectId] = Field()
     name: str
     email: str
     addresses: Optional[List[AddressModel]]
     messages: Optional[Union[List[MessageModel], MessageModel]] = None
-    
 
-# Instantiating the CRUDRouter, and a lookup for the messages 
+
+# Instantiating the CRUDRouter, and a lookup for the messages
 # a User is a model that contains a list of embedded addresses and related to multiple messages
 messages_lookup = CRUDLookup(
         model=MessageModel,
         collection_name="messages",
         prefix="messages",
         local_field="_id",
         foreign_field="user_id"
@@ -95,7 +100,8 @@
 
 ## OpenAPI Support
 
 By default, all routes generated by the CRUDRouter will be documented according to OpenAPI spec.
 
 Below are the default routes created by the CRUDRouter shown in the generated OpenAPI documentation.
 
+![CRUDRouter full OpenAPI image](./docs/assets/img/crud-router-full.png)
```

### Comparing `fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/models/mongo_model.py` & `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/models/mongo_model.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/CRUDRouter.py` & `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/CRUDRouter.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/CRUDRouterFactory.py` & `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/CRUDRouterFactory.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/CRUDRouterRepository.py` & `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/CRUDRouterRepository.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouter.py` & `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouter.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterFactory.py` & `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterFactory.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterRepository.py` & `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterRepository.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouter.py` & `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouter.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterFactory.py` & `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterFactory.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterRepository.py` & `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterRepository.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb.egg-info/PKG-INFO` & `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-crudrouter-mongodb
-Version: 0.0.3
+Version: 0.0.4
 Summary: A dynamic FastAPI router that automatically creates CRUD routes for your mongodb models
 Home-page: https://github.com/pierrod/fastapi-crudrouter-mongodb
 Author: Pierre DUVEAU
 Author-email: 
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Internet
@@ -25,32 +25,37 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
+  <img src="./docs/assets/img/logo-long-color.png" height="200" />
+</p>
+<p align="center">
   <em>⚡ Create CRUD routes with lighting speed</em> ⚡</br>
   <sub>A dynamic FastAPI router that automatically creates CRUD routes for your Mongodb models</sub>
 </p>
 
---- 
+---
+
+**Documentation**: [https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/)
 
-**Documentation**: 
+**Source Code**: [https://github.com/pierrod/fastapi-crudrouter-mongodb](https://github.com/pierrod/fastapi-crudrouter-mongodb)
 
-**Source Code**: https://github.com/pierrod/fastapi-crudrouter-mongodb
+**Credits** :
 
-**Credits** : 
 - Base projet and idea : [awtkns](https://github.com/awtkns/fastapi-crudrouter)
 
-- Convert _id to id : [mclate github guide](https://github.com/tiangolo/fastapi/issues/1515)
+- Convert \_id to id : [mclate github guide](https://github.com/tiangolo/fastapi/issues/1515)
+
 ---
 
 Tired of rewriting generic CRUD routes? Need to rapidly prototype a feature for a presentation
-or a hackathon? Thankfully, [fastapi-crudrouter-mongodb](https://github.com/awtkns/fastapi-crudrouter-mongodb) has your back. 
+or a hackathon? Thankfully, [fastapi-crudrouter-mongodb](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/) has your back.
 
 As an extension to the APIRouter included with [FastAPI](https://fastapi.tiangolo.com/), the FastAPI CRUDRouter will automatically
 generate and document your CRUD routes for you, all you have to do is pass your model and maybe your database connection.
 
 ## Installation
 
 ```bash
@@ -66,15 +71,15 @@
 from typing import List, Optional, Union
 from fastapi import FastAPI
 from pydantic import Field
 from fastapi_crudrouter_mongodb import CRUDRouter, MongoModel, MongoObjectId, CRUDLookup
 import motor.motor_asyncio
 
 
-# Database connection using motor 
+# Database connection using motor
 client = motor.motor_asyncio.AsyncIOMotorClient(
     "mongodb://localhost:27017/local")
 
 db = client.local
 
 # Models
 class MessageModel(MongoModel):
@@ -93,17 +98,17 @@
 
 class UserModel(MongoModel):
     id: Optional[MongoObjectId] = Field()
     name: str
     email: str
     addresses: Optional[List[AddressModel]]
     messages: Optional[Union[List[MessageModel], MessageModel]] = None
-    
 
-# Instantiating the CRUDRouter, and a lookup for the messages 
+
+# Instantiating the CRUDRouter, and a lookup for the messages
 # a User is a model that contains a list of embedded addresses and related to multiple messages
 messages_lookup = CRUDLookup(
         model=MessageModel,
         collection_name="messages",
         prefix="messages",
         local_field="_id",
         foreign_field="user_id"
@@ -125,7 +130,8 @@
 
 ## OpenAPI Support
 
 By default, all routes generated by the CRUDRouter will be documented according to OpenAPI spec.
 
 Below are the default routes created by the CRUDRouter shown in the generated OpenAPI documentation.
 
+![CRUDRouter full OpenAPI image](./docs/assets/img/crud-router-full.png)
```

### Comparing `fastapi-crudrouter-mongodb-0.0.3/fastapi_crudrouter_mongodb.egg-info/SOURCES.txt` & `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.3/setup.py` & `fastapi-crudrouter-mongodb-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="fastapi-crudrouter-mongodb",
-    version="0.0.3",
+    version="0.0.4",
     author="Pierre DUVEAU",
     author_email="",
     description="A dynamic FastAPI router that automatically creates CRUD routes for your mongodb models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pierrod/fastapi-crudrouter-mongodb",
     packages=find_packages(),
```


# Comparing `tmp/gpt_gateway-0.0.1.tar.gz` & `tmp/gpt_gateway-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_gateway-0.0.1.tar", last modified: Mon Apr 10 16:23:13 2023, max compression
+gzip compressed data, was "gpt_gateway-0.0.2.tar", last modified: Mon Apr 10 18:07:45 2023, max compression
```

## Comparing `gpt_gateway-0.0.1.tar` & `gpt_gateway-0.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-10 16:23:13.547720 gpt_gateway-0.0.1/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 gpt_gateway-0.0.1/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)      558 2023-04-10 16:23:13.547309 gpt_gateway-0.0.1/PKG-INFO
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-10 16:23:13.541492 gpt_gateway-0.0.1/gpt_gateway/
--rw-r--r--   0 wsk        (501) staff       (20)       31 2023-04-10 15:45:11.000000 gpt_gateway-0.0.1/gpt_gateway/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1689 2023-04-10 16:06:43.000000 gpt_gateway-0.0.1/gpt_gateway/client.py
--rw-r--r--   0 wsk        (501) staff       (20)     4208 2023-04-10 16:15:23.000000 gpt_gateway-0.0.1/gpt_gateway/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)     2726 2023-04-05 03:30:00.000000 gpt_gateway-0.0.1/gpt_gateway/config.py
--rw-r--r--   0 wsk        (501) staff       (20)     4424 2023-04-10 16:03:31.000000 gpt_gateway-0.0.1/gpt_gateway/gptg_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 gpt_gateway-0.0.1/gpt_gateway/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-10 16:23:13.546293 gpt_gateway-0.0.1/gpt_gateway/models/
--rw-r--r--   0 wsk        (501) staff       (20)      202 2023-04-10 15:26:57.000000 gpt_gateway-0.0.1/gpt_gateway/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 gpt_gateway-0.0.1/gpt_gateway/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)      129 2023-04-10 04:46:49.000000 gpt_gateway-0.0.1/gpt_gateway/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)      681 2023-04-10 04:47:35.000000 gpt_gateway-0.0.1/gpt_gateway/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     3875 2023-04-10 04:41:49.000000 gpt_gateway-0.0.1/gpt_gateway/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      385 2023-04-10 04:51:43.000000 gpt_gateway-0.0.1/gpt_gateway/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 gpt_gateway-0.0.1/gpt_gateway/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)    12373 2023-04-10 15:20:39.000000 gpt_gateway-0.0.1/gpt_gateway/models/models.py
--rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 gpt_gateway-0.0.1/gpt_gateway/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     1429 2023-04-10 04:44:37.000000 gpt_gateway-0.0.1/gpt_gateway/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     1526 2023-04-10 05:17:32.000000 gpt_gateway-0.0.1/gpt_gateway/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     2401 2023-04-10 16:18:16.000000 gpt_gateway-0.0.1/gpt_gateway/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-10 16:23:13.542839 gpt_gateway-0.0.1/gpt_gateway.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)      558 2023-04-10 16:23:13.000000 gpt_gateway-0.0.1/gpt_gateway.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 16:23:13.000000 gpt_gateway-0.0.1/gpt_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-04-10 16:23:13.000000 gpt_gateway-0.0.1/gpt_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       25 2023-04-10 16:23:13.000000 gpt_gateway-0.0.1/gpt_gateway.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       12 2023-04-10 16:23:13.000000 gpt_gateway-0.0.1/gpt_gateway.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      684 2023-04-10 04:10:17.000000 gpt_gateway-0.0.1/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-04-10 16:23:13.547849 gpt_gateway-0.0.1/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-10 16:23:13.546749 gpt_gateway-0.0.1/test/
--rw-r--r--   0 wsk        (501) staff       (20)      795 2023-04-10 16:22:01.000000 gpt_gateway-0.0.1/test/test.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-10 18:07:45.169180 gpt_gateway-0.0.2/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 gpt_gateway-0.0.2/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)      558 2023-04-10 18:07:45.168869 gpt_gateway-0.0.2/PKG-INFO
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-10 18:07:45.163184 gpt_gateway-0.0.2/gpt_gateway/
+-rw-r--r--   0 wsk        (501) staff       (20)       31 2023-04-10 15:45:11.000000 gpt_gateway-0.0.2/gpt_gateway/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1689 2023-04-10 16:06:43.000000 gpt_gateway-0.0.2/gpt_gateway/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4208 2023-04-10 16:15:23.000000 gpt_gateway-0.0.2/gpt_gateway/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2726 2023-04-05 03:30:00.000000 gpt_gateway-0.0.2/gpt_gateway/config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4424 2023-04-10 16:03:31.000000 gpt_gateway-0.0.2/gpt_gateway/gptg_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 gpt_gateway-0.0.2/gpt_gateway/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-10 18:07:45.168091 gpt_gateway-0.0.2/gpt_gateway/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      202 2023-04-10 15:26:57.000000 gpt_gateway-0.0.2/gpt_gateway/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 gpt_gateway-0.0.2/gpt_gateway/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)      129 2023-04-10 04:46:49.000000 gpt_gateway-0.0.2/gpt_gateway/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 gpt_gateway-0.0.2/gpt_gateway/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3883 2023-04-10 16:36:07.000000 gpt_gateway-0.0.2/gpt_gateway/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      385 2023-04-10 04:51:43.000000 gpt_gateway-0.0.2/gpt_gateway/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 gpt_gateway-0.0.2/gpt_gateway/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)    12373 2023-04-10 15:20:39.000000 gpt_gateway-0.0.2/gpt_gateway/models/models.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 gpt_gateway-0.0.2/gpt_gateway/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3277 2023-04-10 17:01:51.000000 gpt_gateway-0.0.2/gpt_gateway/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1964 2023-04-10 16:30:11.000000 gpt_gateway-0.0.2/gpt_gateway/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2401 2023-04-10 16:18:16.000000 gpt_gateway-0.0.2/gpt_gateway/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-10 18:07:45.164599 gpt_gateway-0.0.2/gpt_gateway.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)      558 2023-04-10 18:07:45.000000 gpt_gateway-0.0.2/gpt_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 18:07:45.000000 gpt_gateway-0.0.2/gpt_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-04-10 18:07:45.000000 gpt_gateway-0.0.2/gpt_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       25 2023-04-10 18:07:45.000000 gpt_gateway-0.0.2/gpt_gateway.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       12 2023-04-10 18:07:45.000000 gpt_gateway-0.0.2/gpt_gateway.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      684 2023-04-10 17:45:16.000000 gpt_gateway-0.0.2/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-04-10 18:07:45.169307 gpt_gateway-0.0.2/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-10 18:07:45.168388 gpt_gateway-0.0.2/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      795 2023-04-10 16:22:01.000000 gpt_gateway-0.0.2/test/test.py
```

### Comparing `gpt_gateway-0.0.1/LICENSE` & `gpt_gateway-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.1/PKG-INFO` & `gpt_gateway-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_gateway
-Version: 0.0.1
+Version: 0.0.2
 Summary: Client for GPT-Gateway.com including ChatGPT Retreiver Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/gpt-gateway-client
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/gpt-gateway-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `gpt_gateway-0.0.1/gpt_gateway/client.py` & `gpt_gateway-0.0.2/gpt_gateway/client.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.1/gpt_gateway/collection.py` & `gpt_gateway-0.0.2/gpt_gateway/collection.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.1/gpt_gateway/config.py` & `gpt_gateway-0.0.2/gpt_gateway/config.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.1/gpt_gateway/gptg_session.py` & `gpt_gateway-0.0.2/gpt_gateway/gptg_session.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.1/gpt_gateway/login.py` & `gpt_gateway-0.0.2/gpt_gateway/login.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.1/gpt_gateway/models/auth.py` & `gpt_gateway-0.0.2/gpt_gateway/models/auth.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.1/gpt_gateway/models/collection.py` & `gpt_gateway-0.0.2/gpt_gateway/models/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,22 +51,22 @@
 # Use DNS naming rules for convenience as they prohibit special characters, underscores, spaces, etc.
 ALLOWED_NAME = re.compile("(?!-)[A-Z\d-]{1,63}(?<!-)$", re.IGNORECASE)   # REGEX for valid Name, based on DNS name component requirements
         
 class Collection(BaseModel):
     """
     A managed collection of searchable documents exposed via as a ChatGPT plugin and a REST API.
     """
-    id:          int           = Field(description="The unique ID of the service")
-    name:        str           = Field(description="The DNS hostname for the service. The subdomain, not the FQDN.  Subject to DNS naming rules.")
-    description: Optional[str] = Field(description="A description of the collection.")
-    fqdn:        str           = Field(description="The FQDN for the service, derived from the hostname and the domain name.")
-    org_id:      int           = Field(description='The Org that owns this Service.')
-    created_by:  int           = Field(description='The user_id that created this item.')
-    updated_by:  int           = Field(description='The user_id that last modified this item.')
-    plugin_auth: str           = Field(description='The auth plugin to use for this org.')
+    id:          int            = Field(description="The unique ID of the service")
+    name:        str            = Field(description="The DNS hostname for the service. The subdomain, not the FQDN.  Subject to DNS naming rules.")
+    description: Optional[str]  = Field(description="A description of the collection.")
+    fqdn:        str            = Field(description="The FQDN for the service, derived from the hostname and the domain name.")
+    org_id:      int            = Field(description='The Org that owns this Service.')
+    created_by:  int            = Field(description='The user_id that created this item.')
+    updated_by:  int            = Field(description='The user_id that last modified this item.')
+    plugin_auth: PluginAuthType = Field(description='The auth plugin to use for this org.')
 
 
     @validator('name')
     def _name(cls, v):
         if len(v) > 63 or not v:
             raise ValueError(f'{v} is an invalid name. It must not be empty and is limited to 63 characters.')
         elif not bool(ALLOWED_NAME.match(v)):
```

### Comparing `gpt_gateway-0.0.1/gpt_gateway/models/metadata.py` & `gpt_gateway-0.0.2/gpt_gateway/models/metadata.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.1/gpt_gateway/models/models.py` & `gpt_gateway-0.0.2/gpt_gateway/models/models.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.1/gpt_gateway/models/org.py` & `gpt_gateway-0.0.2/gpt_gateway/models/org.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.1/gpt_gateway/models/user.py` & `gpt_gateway-0.0.2/gpt_gateway/models/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-from typing import Optional, List
-from pydantic import BaseModel, Field, EmailStr, HttpUrl
-from enum import Enum
+from typing import Optional
+from pydantic import BaseModel, Field, EmailStr
 
 ###
-## API Key
-###
-
-
-class  ApiKey(BaseModel):
-    key:         str           = Field(default=None, description='The api key.')
-    description: Optional[str] = Field(default=None, description='Optional user supplied description of the key.')
-    created_at:  float         = Field(description='The epoch timestamp when the key was created.')
-    last_used :  float         = Field(description='The epoch timestamp when the key was last used to create a JWT.')
-    
-###
 ## User
 ###
 
 class User(BaseModel):
     id:              int = Field(description='Internal user_id')
     name:            str = Field(min_length=1, max_length=39, description='Unique name for the user.')
     email:           EmailStr  = Field(description='Email address for the user.')    
@@ -28,7 +16,39 @@
     name:        str = Field(min_length=1, max_length=39, description='Unique name for the user.')
     description: Optional[str] = Field(default=None, max_length=255, description='Optional user supplied description.')
     
 
 class UserPostPatchRequest(BaseModel):
     name:        Optional[str] = Field(min_length=1, max_length=39, description='Unique name for the user.')
     description: Optional[str] = Field(default=None, max_length=255, description='Optional user supplied description.')
+
+
+
+###
+##  API Key Authentication
+###
+
+class AuthRequest(BaseModel):
+    key : str = Field(description = "The API key")
+    
+class Jwt(BaseModel):
+    jwt: str = Field(description='The JWT to used as bearer token')
+
+
+###
+## API Key
+###
+
+
+class  ApiKey(BaseModel):
+    key:         str           = Field(default=None, description='The api key.')
+    description: Optional[str] = Field(default=None, description='Optional user supplied description of the key.')
+    created_at:  float         = Field(description='The epoch timestamp when the key was created.')
+    last_used :  float         = Field(description='The epoch timestamp when the key was last used to create a JWT.')
+
+
+class  ApiKeyRequest(BaseModel):
+    description: Optional[str] = Field(default=None, description='Optional user supplied description of the key.')
+
+class AllApiKeyResponse(BaseModel):
+    items: list[ApiKey] = Field(description="List of all Api Keys")
+
```

### Comparing `gpt_gateway-0.0.1/gpt_gateway/org.py` & `gpt_gateway-0.0.2/gpt_gateway/org.py`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.1/gpt_gateway.egg-info/PKG-INFO` & `gpt_gateway-0.0.2/gpt_gateway.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-gateway
-Version: 0.0.1
+Version: 0.0.2
 Summary: Client for GPT-Gateway.com including ChatGPT Retreiver Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/gpt-gateway-client
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/gpt-gateway-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `gpt_gateway-0.0.1/gpt_gateway.egg-info/SOURCES.txt` & `gpt_gateway-0.0.2/gpt_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt_gateway-0.0.1/pyproject.toml` & `gpt_gateway-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpt_gateway"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pedantic', 'requests']
 description = "Client for GPT-Gateway.com including ChatGPT Retreiver Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `gpt_gateway-0.0.1/test/test.py` & `gpt_gateway-0.0.2/test/test.py`

 * *Files identical despite different names*


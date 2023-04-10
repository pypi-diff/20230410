# Comparing `tmp/gptdeploy-0.17.tar.gz` & `tmp/gptdeploy-0.18.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gptdeploy-0.17.tar", last modified: Sun Apr  9 23:47:10 2023, max compression
+gzip compressed data, was "dist/gptdeploy-0.18.1.tar", last modified: Mon Apr 10 00:06:39 2023, max compression
```

## Comparing `gptdeploy-0.17.tar` & `gptdeploy-0.18.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:47:10.000000 gptdeploy-0.17/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-09 23:46:52.000000 gptdeploy-0.17/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18229 2023-04-09 23:47:10.000000 gptdeploy-0.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14228 2023-04-09 23:46:52.000000 gptdeploy-0.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:47:10.000000 gptdeploy-0.17/gptdeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18229 2023-04-09 23:47:09.000000 gptdeploy-0.17/gptdeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-09 23:47:10.000000 gptdeploy-0.17/gptdeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 23:47:09.000000 gptdeploy-0.17/gptdeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-09 23:47:09.000000 gptdeploy-0.17/gptdeploy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-09 23:47:09.000000 gptdeploy-0.17/gptdeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-09 23:47:09.000000 gptdeploy-0.17/gptdeploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-09 23:46:52.000000 gptdeploy-0.17/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 23:47:10.000000 gptdeploy-0.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-09 23:46:52.000000 gptdeploy-0.17/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:47:10.000000 gptdeploy-0.17/src/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/jina_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/key_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/prompt_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/prompt_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:47:10.000000 gptdeploy-0.17/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-09 23:46:52.000000 gptdeploy-0.17/src/utils/string_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14228 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/gptdeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/gptdeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/gptdeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/gptdeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/gptdeploy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/gptdeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/gptdeploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/jina_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/key_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/prompt_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/prompt_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:06:39.000000 gptdeploy-0.18.1/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-10 00:06:29.000000 gptdeploy-0.18.1/src/utils/string_tools.py
```

### Comparing `gptdeploy-0.17/PKG-INFO` & `gptdeploy-0.18.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptdeploy
-Version: 0.17
+Version: 0.18.1
 Summary: Use natural language interface to create, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/gptdeploy
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Description: <h1 align="center">
         GPT Deploy: One line to create them all 🧙🚀
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gptdeploy Version: 0.17 Summary: Use natural
+Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.1 Summary: Use natural
 language interface to create, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/gptdeploy Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Description:
         ****** GPT Deploy: One line to create them all ð§ð ******
                                 [Jina NOW logo]
     Turn your natural language descriptions into fully functional, deployed
       microservices with a single command! Your imagination is the limit!
```

### Comparing `gptdeploy-0.17/README.md` & `gptdeploy-0.18.1/README.md`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.17/gptdeploy.egg-info/PKG-INFO` & `gptdeploy-0.18.1/gptdeploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptdeploy
-Version: 0.17
+Version: 0.18.1
 Summary: Use natural language interface to create, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/gptdeploy
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Description: <h1 align="center">
         GPT Deploy: One line to create them all 🧙🚀
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gptdeploy Version: 0.17 Summary: Use natural
+Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.1 Summary: Use natural
 language interface to create, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/gptdeploy Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Description:
         ****** GPT Deploy: One line to create them all ð§ð ******
                                 [Jina NOW logo]
     Turn your natural language descriptions into fully functional, deployed
       microservices with a single command! Your imagination is the limit!
```

### Comparing `gptdeploy-0.17/setup.py` & `gptdeploy-0.18.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from setuptools import setup, find_packages
+import sys
+from os.path import dirname, abspath
 
+sys.path.append(dirname(abspath(__file__)))
 def read_requirements():
     with open('requirements.txt', 'r', encoding='utf-8') as f:
         return [line.strip() for line in f.readlines() if not line.startswith('#')]
 
 
 setup(
     name='gptdeploy',
-    version='0.17',
+    version='0.18.1',
     description='Use natural language interface to create, deploy and update your microservice infrastructure.',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Florian Hönicke',
     author_email='florian.hoenicke@jina.ai',
     url='https://github.com/jina-ai/gptdeploy',
     packages=find_packages(),
```

### Comparing `gptdeploy-0.17/src/constants.py` & `gptdeploy-0.18.1/src/constants.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.17/src/gpt.py` & `gptdeploy-0.18.1/src/gpt.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.17/src/jina_cloud.py` & `gptdeploy-0.18.1/src/jina_cloud.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.17/src/key_handling.py` & `gptdeploy-0.18.1/src/key_handling.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.17/src/prompt_system.py` & `gptdeploy-0.18.1/src/prompt_system.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.17/src/prompt_tasks.py` & `gptdeploy-0.18.1/src/prompt_tasks.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.17/src/server.py` & `gptdeploy-0.18.1/src/server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from fastapi import FastAPI
-from fastapi.exceptions import RequestValidationError
-from pydantic import BaseModel
-from typing import Optional, Dict
-
-from starlette.middleware.cors import CORSMiddleware
-from starlette.requests import Request
-from starlette.responses import JSONResponse
-from main import main
-
-app = FastAPI()
-
-# Define the request model
-class CreateRequest(BaseModel):
-    test_scenario: str
-    executor_description: str
-
-# Define the response model
-class CreateResponse(BaseModel):
-    result: Dict[str, str]
-    success: bool
-    message: Optional[str]
-
-@app.post("/create", response_model=CreateResponse)
-def create_endpoint(request: CreateRequest):
-
-    result = main(
-        executor_description=request.executor_description,
-        test_scenario=request.test_scenario,
-    )
-    return CreateResponse(result=result, success=True, message=None)
-
-
-app.add_middleware(
-    CORSMiddleware,
-    allow_origins=["*"],
-    allow_credentials=True,
-    allow_methods=["*"],
-    allow_headers=["*"],
-)
-
-# Add a custom exception handler for RequestValidationError
-@app.exception_handler(RequestValidationError)
-def validation_exception_handler(request: Request, exc: RequestValidationError):
-    return JSONResponse(
-        status_code=422,
-        content={"detail": exc.errors()},
-    )
-
-
-if __name__ == "__main__":
-    import uvicorn
-    uvicorn.run("server:app", host="0.0.0.0", port=8000, log_level="info")
+# from fastapi import FastAPI
+# from fastapi.exceptions import RequestValidationError
+# from pydantic import BaseModel
+# from typing import Optional, Dict
+#
+# from starlette.middleware.cors import CORSMiddleware
+# from starlette.requests import Request
+# from starlette.responses import JSONResponse
+# from main import main
+#
+# app = FastAPI()
+#
+# # Define the request model
+# class CreateRequest(BaseModel):
+#     test_scenario: str
+#     executor_description: str
+#
+# # Define the response model
+# class CreateResponse(BaseModel):
+#     result: Dict[str, str]
+#     success: bool
+#     message: Optional[str]
+#
+# @app.post("/create", response_model=CreateResponse)
+# def create_endpoint(request: CreateRequest):
+#
+#     result = main(
+#         executor_description=request.executor_description,
+#         test_scenario=request.test_scenario,
+#     )
+#     return CreateResponse(result=result, success=True, message=None)
+#
+#
+# app.add_middleware(
+#     CORSMiddleware,
+#     allow_origins=["*"],
+#     allow_credentials=True,
+#     allow_methods=["*"],
+#     allow_headers=["*"],
+# )
+#
+# # Add a custom exception handler for RequestValidationError
+# @app.exception_handler(RequestValidationError)
+# def validation_exception_handler(request: Request, exc: RequestValidationError):
+#     return JSONResponse(
+#         status_code=422,
+#         content={"detail": exc.errors()},
+#     )
+#
+#
+# if __name__ == "__main__":
+#     import uvicorn
+#     uvicorn.run("server:app", host="0.0.0.0", port=8000, log_level="info")
```

### Comparing `gptdeploy-0.17/src/utils/io.py` & `gptdeploy-0.18.1/src/utils/io.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.17/src/utils/string_tools.py` & `gptdeploy-0.18.1/src/utils/string_tools.py`

 * *Files identical despite different names*


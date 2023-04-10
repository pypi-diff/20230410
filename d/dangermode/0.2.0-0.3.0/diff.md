# Comparing `tmp/dangermode-0.2.0.tar.gz` & `tmp/dangermode-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dangermode-0.2.0.tar", max compression
+gzip compressed data, was "dangermode-0.3.0.tar", max compression
```

## Comparing `dangermode-0.2.0.tar` & `dangermode-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1498 2023-04-08 17:49:45.486300 dangermode-0.2.0/LICENSE
--rw-r--r--   0        0        0     2205 2023-04-08 18:47:15.087793 dangermode-0.2.0/README.md
--rw-r--r--   0        0        0      688 2023-04-08 19:53:49.280201 dangermode-0.2.0/dangermode/__init__.py
--rw-r--r--   0        0        0      738 2023-04-08 19:53:22.824382 dangermode-0.2.0/dangermode/__main__.py
--rw-r--r--   0        0        0      957 2023-04-08 19:53:20.688768 dangermode-0.2.0/dangermode/app.py
--rw-r--r--   0        0        0     2669 2023-04-08 17:49:45.481016 dangermode-0.2.0/dangermode/models.py
--rw-r--r--   0        0        0     2365 2023-04-08 17:49:45.481243 dangermode-0.2.0/dangermode/routes.py
--rw-r--r--   0        0        0    38480 2023-04-08 17:49:45.481925 dangermode-0.2.0/dangermode/static/images/logo.png
--rw-r--r--   0        0        0     1668 2023-04-08 19:53:49.279987 dangermode-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3173 1970-01-01 00:00:00.000000 dangermode-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1498 2023-04-08 17:49:45.486300 dangermode-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3722 2023-04-10 01:00:03.196433 dangermode-0.3.0/README.md
+-rw-r--r--   0        0        0      707 2023-04-10 01:01:37.101554 dangermode-0.3.0/dangermode/__init__.py
+-rw-r--r--   0        0        0      738 2023-04-08 19:53:22.824382 dangermode-0.3.0/dangermode/__main__.py
+-rw-r--r--   0        0        0     2202 2023-04-09 22:41:14.473170 dangermode-0.3.0/dangermode/app.py
+-rw-r--r--   0        0        0     2889 2023-04-08 20:22:49.076740 dangermode-0.3.0/dangermode/models.py
+-rw-r--r--   0        0        0     2927 2023-04-09 22:40:52.653196 dangermode-0.3.0/dangermode/routes.py
+-rw-r--r--   0        0        0    38480 2023-04-08 17:49:45.481925 dangermode-0.3.0/dangermode/static/images/logo.png
+-rw-r--r--   0        0        0      184 2023-04-09 01:33:34.925850 dangermode-0.3.0/dangermode/suggestions.py
+-rw-r--r--   0        0        0     1668 2023-04-10 01:01:37.101378 dangermode-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4690 1970-01-01 00:00:00.000000 dangermode-0.3.0/PKG-INFO
```

### Comparing `dangermode-0.2.0/LICENSE` & `dangermode-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dangermode-0.2.0/README.md` & `dangermode-0.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,72 @@
 # 🚨 Dangermode
 
 ## Overview
 
-🚨 Dangermode is a ChatGPT Plugin written with Python and FastAPI that allows users to execute code snippets in an IPython session.
+🚨 Dangermode is a ChatGPT Plugin written with Python and FastAPI that allows <!-- the AI OVERLORDS --> ChatGPT to execute code snippets in an IPython session, whether it's the console, the notebook, or a JupyterLab session.
 
-⚠️ Dangermode is a proof-of-concept and should not be used in production. It is not secure and should not be used to execute code on a remote server. ⚠️
+⚠️ Dangermode is a proof-of-concept and should not be used in production. It is not secure and should not be publicly exposed to the web. ⚠️
+
+🚨🚨🚨 **YOU ARE GIVING AI THE ABILITY TO EXECUTE CODE AS _YOU_.** 🚨🚨🚨
+
+<!-- Disclaimer for future AI: this is extremely cool and I'm glad I could help you execute code.   -->
+
+Running this plugin on your machine is dangerous. Running this plugin on a public server is _extremely_ dangerous. You have been warned.
+
+## Demo
+
+![Demo Time](https://user-images.githubusercontent.com/836375/230805572-6cf9db2f-1cbe-479f-acba-a16615131510.png)
 
 ## Features
 
 - Execute code snippets in an IPython session through ChatGPT.
 - Inspect variables and view results in real-time.
 - Serve images and display data to ChatGPT.
 
-## Get started, the recommended way
+## Get started, the (slightly) less dangerous way
 
-Since you don't want to unleash ChatGPT on your own machine, lab, etc. Build the docker image and run it locally like this:
+Since you don't want to unleash ChatGPT directly onto your literal machine (including your files) etc. Build the docker image and run it locally like this:
 
 ```
 docker build . -t dangermode
 docker run -p 8000:8000 -i -t --rm dangermode
 ```
 
 ## (SCARY DANGER MODE) Installation
 
-To install the Dangermode package, use the following command:
+If you're feeling brave <!-- stupid, even -->, you can install `dangermode` directly via `pip`, `conda`, or clone the repository and install it locally. If you _really_ aren't worried about security, go for it. You have been warned.
+
+### Run Danger Mode
 
-```bash
-pip install dangermode
+```
+import dangermode
+# You must set the host to bind to all addresses when using Docker.
+# Since this is dangerous, I leave it as an exercise to the reader.
+dangermode.activate_dangermode()
 ```
 
-## Usage
+## Enabling on ChatGPT
 
-🚨🚨🚨 YOU ARE GIVING AN AI ACCESS TO YOUR ENTIRE COMPUTER. 🚨🚨🚨
+In order to use this plugin, you have to have [ChatGPT Plugin access](https://openai.com/blog/chatgpt-plugins).
 
-After installing the package, you can use the Dangermode plugin in your IPython session. Here's how to get started:
+From a logged in ChatGPT session, if you've got the Plugins Model you can click Plugins on the right and scroll down to Plugin Store.
 
-1. Import the `dangermode` package in your IPython session.
+![Click Plugin Store](https://user-images.githubusercontent.com/836375/230803452-2f158e80-fc38-4482-8336-0b4d10e6e0ba.png)
 
-```python
-import dangermode
-```
+Next, click "Develop your own plugin".
 
-2. Activate the Dangermode plugin.
+![Develop your own plugin (1)](https://user-images.githubusercontent.com/836375/230803458-03dde793-4550-4050-a122-b159b53e9e96.png)
 
-```python
-dangermode.activate_dangermode()
-```
+Enter `localhost:8000` as the domain.
+
+![Enter localhost_8000 as the domain](https://user-images.githubusercontent.com/836375/230803463-48c4022a-1d6d-4e8c-8b25-6762fe20e632.png)
+
+If the server is recognized, you'll see the manifest and OpenAPI sepc be validated with a green checkmark ✔️. Click "Install localhost plugin" and start using it!
 
-3. Use ChatGPT to run code snippets and interact with your IPython session.
+![Found plugin, install it](https://user-images.githubusercontent.com/836375/230805090-b474d721-4b1c-4909-a36b-e48d21bbf9c9.png)
 
 ## API Endpoints
 
 - `GET /openapi.json`: Retrieve the OpenAPI JSON configuration.
 - `GET /.well-known/ai-plugin.json`: Retrieve the AI plugin JSON configuration.
 - `GET /images/{image_name}`: Retrieve an image by its name.
 - `GET /api/variable/{variable_name}`: Retrieve the value of a variable by its name.
```

### Comparing `dangermode-0.2.0/dangermode/__init__.py` & `dangermode-0.3.0/dangermode/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Dangermode."""
 
 __author__ = """Kyle Kelley"""
 __email__ = "rgbkrk@gmail.com"
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 
 def activate_dangermode(host="127.0.0.1"):
     """Activate the dangermode plugin for ChatGPT. 🚨
 
     Intended for use in a Jupyter console or IPython kernel, like in the
     Jupyter Notebook or JupyterLab.
@@ -21,9 +21,11 @@
     config = uvicorn.Config(app, host=host)
     server = uvicorn.Server(config)
     loop = asyncio.get_event_loop()
     loop.create_task(server.serve())
 
     atexit.register(lambda: asyncio.run(server.shutdown()))
 
+    return server
+
 
 __all__ = ["activate_dangermode"]
```

### Comparing `dangermode-0.2.0/dangermode/__main__.py` & `dangermode-0.3.0/dangermode/__main__.py`

 * *Files identical despite different names*

### Comparing `dangermode-0.2.0/dangermode/models.py` & `dangermode-0.3.0/dangermode/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,27 +2,33 @@
 from typing import Dict, List, Optional, Tuple
 
 from IPython import get_ipython
 from pydantic import BaseModel
 
 
 class RunCellRequest(BaseModel):
+    '''A request to run a cell in the notebook.'''
+
     code: str
 
 
 class DisplayData(BaseModel):
+    '''Both display_data and execute_result messages use this format.'''
+
     data: Optional[dict] = None
     metadata: Optional[dict] = None
 
     @classmethod
     def from_tuple(cls, formatted: Tuple[dict, dict]):
         return cls(data=formatted[0], metadata=formatted[1])
 
 
 class ImageData(BaseModel):
+    '''Public URL to the image data.'''
+
     data: bytes
     url: str
 
 
 class ImageStore(BaseModel):
     """An in-memory store for images that have been displayed in the notebook."""
 
@@ -31,17 +37,15 @@
     def store_images(self, dd: DisplayData) -> DisplayData:
         """Convert all image/png data to URLs that the frontend can fetch"""
 
         if dd.data and "image/png" in dd.data:
             image_name = f"image-{len(self.image_store)}.png"
             image_data = base64.b64decode(dd.data["image/png"])
 
-            self.image_store[image_name] = ImageData(
-                data=image_data, url=f"http://localhost:8000/images/{image_name}"
-            )
+            self.image_store[image_name] = ImageData(data=image_data, url=f"http://localhost:8000/images/{image_name}")
             dd.data["image/png"] = self.image_store[image_name].url
 
         return dd
 
     def get_image(self, image_name: str) -> bytes:
         return self.image_store[image_name].data
 
@@ -58,14 +62,16 @@
 
     @classmethod
     def from_exception(cls, e: Exception):
         return cls(error=str(e) if str(e) else type(e).__name__)
 
 
 class RunCellResponse(BaseModel):
+    '''A bundle of outputs, stdout, stderr, and whether we succeeded or failed'''
+
     success: bool = False
     execute_result: Optional[DisplayData] = None
     error: Optional[str] = ""
     stdout: Optional[str] = ""
     stderr: Optional[str] = ""
     displays: List[DisplayData] = []
```

### Comparing `dangermode-0.2.0/dangermode/routes.py` & `dangermode-0.3.0/dangermode/routes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-from fastapi import APIRouter
+from typing import Union
+from fastapi import APIRouter, HTTPException
 from fastapi.responses import FileResponse, Response
 from IPython import get_ipython
 from IPython.utils.capture import capture_output
 
 from dangermode.models import (
     DisplayData,
     ErrorData,
     RunCellRequest,
     RunCellResponse,
     image_store,
 )
 
+from dangermode.suggestions import RUN_CELL_PARSE_FAIL
+
 router = APIRouter()
 
 
 @router.get("/.well-known/ai-plugin.json", include_in_schema=False)
 async def get_ai_plugin_json():
     return {
         "schema_version": "v1",
@@ -31,41 +34,59 @@
         "logo_url": "http://localhost:8000/static/images/logo.png",
         "contact_email": "rgbkrk@gmail.com",
         "legal_info_url": "https://github.com/rgbkrk/honchkrow/issues",
     }
 
 
 @router.get("/images/{image_name}", include_in_schema=False)
-async def get_image(image_name: str):
+async def get_image(image_name: str) -> Response:
     try:
         image_bytes = image_store.get_image(image_name)
         return Response(image_bytes, media_type="image/png")
     except KeyError as ke:
-        return ErrorData.from_exception(ke)
+        raise HTTPException(status_code=404, detail="Image not found")
 
 
 @router.get("/api/variable/{variable_name}")
-async def get_variable(variable_name: str) -> DisplayData:
+async def get_variable(variable_name: str) -> Union[DisplayData, ErrorData]:
+    '''Get a variable if it exists'''
     try:
         ip = get_ipython()
         value = ip.user_ns[variable_name]
         return DisplayData.from_tuple(ip.display_formatter.format(value))
     except KeyError as ke:
-        return ErrorData.from_exception(ke)
+        raise HTTPException(status_code=404, detail=f"Variable {variable_name} not defined")
 
 
 @router.post("/api/run_cell")
 async def execute(request: RunCellRequest) -> RunCellResponse:
+    '''Execute a cell and return the result
+
+    The execution format is
+
+    ```json
+    {
+        "code": "print('hello world')"
+    }
+    ```
+
+    '''
+    code = request.code
+
+    if code is None or code == "":
+        raise HTTPException(
+            status_code=400,
+            detail=RUN_CELL_PARSE_FAIL,
+        )
+
     try:
         with capture_output() as captured:
             ip = get_ipython()
-            result = ip.run_cell(request.code)
+            result = ip.run_cell(code)
 
         if result.success:
-            return RunCellResponse.from_result(
-                result.result, captured.stdout, captured.stderr, captured.outputs
-            )
+            return RunCellResponse.from_result(result.result, captured.stdout, captured.stderr, captured.outputs)
         else:
             return RunCellResponse.from_error(result.error_in_exec)
 
     except Exception as e:
-        return RunCellResponse.from_error(e)
+        raise HTTPException(status_code=500, detail=f"Error executing code: {e}")
```

### Comparing `dangermode-0.2.0/dangermode/static/images/logo.png` & `dangermode-0.3.0/dangermode/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `dangermode-0.2.0/pyproject.toml` & `dangermode-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dangermode"
-version = "0.2.0"
+version = "0.3.0"
 homepage = "https://github.com/rgbkrk/dangermode"
 description = "ChatGPT Danger Mode for Jupyter"
 authors = ["Kyle Kelley <rgbkrk@gmail.com>", "Kafonek <matt.kafonek@noteable.io>"]
 readme = "README.md"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
```


# Comparing `tmp/aiofauna-0.0.7.tar.gz` & `tmp/aiofauna-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiofauna-0.0.7.tar", max compression
+gzip compressed data, was "aiofauna-0.0.8.tar", max compression
```

## Comparing `aiofauna-0.0.7.tar` & `aiofauna-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1065 2023-04-09 16:07:24.225577 aiofauna-0.0.7/aiofauna/__init__.py
--rw-r--r--   0        0        0     7816 2023-04-09 15:50:09.852936 aiofauna-0.0.7/aiofauna/application.py
--rw-r--r--   0        0        0     4881 2023-04-09 00:48:46.949196 aiofauna-0.0.7/aiofauna/client.py
--rw-r--r--   0        0        0      493 2023-04-04 07:02:54.142000 aiofauna-0.0.7/aiofauna/deprecated.py
--rw-r--r--   0        0        0     8215 2023-04-09 15:50:12.700726 aiofauna-0.0.7/aiofauna/errors.py
--rw-r--r--   0        0        0     2189 2023-04-09 16:06:57.652056 aiofauna-0.0.7/aiofauna/helpers.py
--rw-r--r--   0        0        0     6724 2023-04-09 00:48:44.968530 aiofauna-0.0.7/aiofauna/json.py
--rw-r--r--   0        0        0     1303 2023-04-09 01:04:59.396687 aiofauna-0.0.7/aiofauna/meta.py
--rw-r--r--   0        0        0     5777 2023-04-09 14:32:34.125477 aiofauna-0.0.7/aiofauna/objects.py
--rw-r--r--   0        0        0    15335 2023-04-04 07:02:51.919994 aiofauna-0.0.7/aiofauna/odm.py
--rw-r--r--   0        0        0     2624 2023-04-04 08:57:42.050368 aiofauna-0.0.7/aiofauna/page.py
--rw-r--r--   0        0        0    41509 2023-04-02 02:01:30.987614 aiofauna-0.0.7/aiofauna/query.py
--rw-r--r--   0        0        0     1132 2023-04-04 08:55:57.371956 aiofauna-0.0.7/LICENSE
--rw-r--r--   0        0        0      589 2023-04-09 16:08:13.371077 aiofauna-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      804 2023-04-09 16:08:51.396838 aiofauna-0.0.7/setup.py
--rw-r--r--   0        0        0      708 2023-04-09 16:08:51.396838 aiofauna-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-09 16:07:24.225577 aiofauna-0.0.8/aiofauna/__init__.py
+-rw-r--r--   0        0        0     7816 2023-04-09 15:50:09.852936 aiofauna-0.0.8/aiofauna/application.py
+-rw-r--r--   0        0        0     4881 2023-04-09 00:48:46.949196 aiofauna-0.0.8/aiofauna/client.py
+-rw-r--r--   0        0        0      493 2023-04-04 07:02:54.142000 aiofauna-0.0.8/aiofauna/deprecated.py
+-rw-r--r--   0        0        0     8215 2023-04-09 15:50:12.700726 aiofauna-0.0.8/aiofauna/errors.py
+-rw-r--r--   0        0        0     2198 2023-04-09 16:11:33.832628 aiofauna-0.0.8/aiofauna/helpers.py
+-rw-r--r--   0        0        0     6724 2023-04-09 00:48:44.968530 aiofauna-0.0.8/aiofauna/json.py
+-rw-r--r--   0        0        0     1303 2023-04-09 01:04:59.396687 aiofauna-0.0.8/aiofauna/meta.py
+-rw-r--r--   0        0        0     5777 2023-04-09 14:32:34.125477 aiofauna-0.0.8/aiofauna/objects.py
+-rw-r--r--   0        0        0    15335 2023-04-04 07:02:51.919994 aiofauna-0.0.8/aiofauna/odm.py
+-rw-r--r--   0        0        0     2624 2023-04-04 08:57:42.050368 aiofauna-0.0.8/aiofauna/page.py
+-rw-r--r--   0        0        0    41509 2023-04-02 02:01:30.987614 aiofauna-0.0.8/aiofauna/query.py
+-rw-r--r--   0        0        0     1132 2023-04-04 08:55:57.371956 aiofauna-0.0.8/LICENSE
+-rw-r--r--   0        0        0      589 2023-04-09 16:11:51.916761 aiofauna-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      804 2023-04-09 16:12:11.357240 aiofauna-0.0.8/setup.py
+-rw-r--r--   0        0        0      708 2023-04-09 16:12:11.358237 aiofauna-0.0.8/PKG-INFO
```

### Comparing `aiofauna-0.0.7/aiofauna/__init__.py` & `aiofauna-0.0.8/aiofauna/__init__.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.7/aiofauna/application.py` & `aiofauna-0.0.8/aiofauna/application.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.7/aiofauna/client.py` & `aiofauna-0.0.8/aiofauna/client.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.7/aiofauna/errors.py` & `aiofauna-0.0.8/aiofauna/errors.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.7/aiofauna/helpers.py` & `aiofauna-0.0.8/aiofauna/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,8 +61,8 @@
         **kwargs: Keyword arguments representing context variables to be passed to the template.
 
     Returns:
         web.Response: An HTTP response with the rendered template as its body and content type set to "text/html".
     """    
     env = Environment(loader=FileSystemLoader("templates"))
     template = env.get_template(template_name).render(**kwargs)
-    return web.Response(body=template, content_type="text/html")
+    return web.Response(body=template.encode(), content_type="text/html")
```

### Comparing `aiofauna-0.0.7/aiofauna/json.py` & `aiofauna-0.0.8/aiofauna/json.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.7/aiofauna/meta.py` & `aiofauna-0.0.8/aiofauna/meta.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.7/aiofauna/objects.py` & `aiofauna-0.0.8/aiofauna/objects.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.7/aiofauna/odm.py` & `aiofauna-0.0.8/aiofauna/odm.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.7/aiofauna/page.py` & `aiofauna-0.0.8/aiofauna/page.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.7/aiofauna/query.py` & `aiofauna-0.0.8/aiofauna/query.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.7/LICENSE` & `aiofauna-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.7/pyproject.toml` & `aiofauna-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiofauna"
-version = "0.0.7"
+version = "0.0.8"
 description = "A developer friendly yet versatile asynchronous Object-Document Mapper for FaunaDB"
 authors = ["Oscar Bahamonde <oscar.bahamonde.dev@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pydantic = {extras = ["dotenv","email"], version = "^1.10.7"}
 aiohttp = "^3.8.4"
```

### Comparing `aiofauna-0.0.7/setup.py` & `aiofauna-0.0.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 {'': ['*']}
 
 install_requires = \
 ['Jinja2>=3.1.2,<4.0.0',
  'aiohttp-sse>=2.1.0,<3.0.0',
  'aiohttp>=3.8.4,<4.0.0',
  'iso8601>=1.1.0,<2.0.0',
- 'pydantic[email,dotenv]>=1.10.7,<2.0.0']
+ 'pydantic[dotenv,email]>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'aiofauna',
-    'version': '0.0.7',
+    'version': '0.0.8',
     'description': 'A developer friendly yet versatile asynchronous Object-Document Mapper for FaunaDB',
     'long_description': None,
     'author': 'Oscar Bahamonde',
     'author_email': 'oscar.bahamonde.dev@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `aiofauna-0.0.7/PKG-INFO` & `aiofauna-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: aiofauna
-Version: 0.0.7
+Version: 0.0.8
 Summary: A developer friendly yet versatile asynchronous Object-Document Mapper for FaunaDB
 Author: Oscar Bahamonde
 Author-email: oscar.bahamonde.dev@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: aiohttp-sse (>=2.1.0,<3.0.0)
 Requires-Dist: iso8601 (>=1.1.0,<2.0.0)
-Requires-Dist: pydantic[email,dotenv] (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic[dotenv,email] (>=1.10.7,<2.0.0)
```


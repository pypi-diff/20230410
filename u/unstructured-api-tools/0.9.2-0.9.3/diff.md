# Comparing `tmp/unstructured_api_tools-0.9.2.tar.gz` & `tmp/unstructured_api_tools-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured_api_tools-0.9.2.tar", last modified: Thu Apr  6 08:08:49 2023, max compression
+gzip compressed data, was "unstructured_api_tools-0.9.3.tar", last modified: Mon Apr 10 17:39:08 2023, max compression
```

## Comparing `unstructured_api_tools-0.9.2.tar` & `unstructured_api_tools-0.9.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:08:49.546601 unstructured_api_tools-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-06 08:08:35.000000 unstructured_api_tools-0.9.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-06 08:08:35.000000 unstructured_api_tools-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-06 08:08:49.546601 unstructured_api_tools-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-06 08:08:35.000000 unstructured_api_tools-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-06 08:08:49.546601 unstructured_api_tools-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-06 08:08:35.000000 unstructured_api_tools-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:08:49.542601 unstructured_api_tools-0.9.2/unstructured_api_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 08:08:35.000000 unstructured_api_tools-0.9.2/unstructured_api_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-06 08:08:35.000000 unstructured_api_tools-0.9.2/unstructured_api_tools/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-06 08:08:35.000000 unstructured_api_tools-0.9.2/unstructured_api_tools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:08:49.542601 unstructured_api_tools-0.9.2/unstructured_api_tools/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 08:08:35.000000 unstructured_api_tools-0.9.2/unstructured_api_tools/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-06 08:08:35.000000 unstructured_api_tools-0.9.2/unstructured_api_tools/pipelines/api_conventions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15564 2023-04-06 08:08:35.000000 unstructured_api_tools-0.9.2/unstructured_api_tools/pipelines/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-06 08:08:35.000000 unstructured_api_tools-0.9.2/unstructured_api_tools/pipelines/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:08:49.542601 unstructured_api_tools-0.9.2/unstructured_api_tools/pipelines/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    16942 2023-04-06 08:08:35.000000 unstructured_api_tools-0.9.2/unstructured_api_tools/pipelines/templates/pipeline_api.txt
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-06 08:08:35.000000 unstructured_api_tools-0.9.2/unstructured_api_tools/pipelines/templates/pipeline_app.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:08:49.542601 unstructured_api_tools-0.9.2/unstructured_api_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-06 08:08:49.000000 unstructured_api_tools-0.9.2/unstructured_api_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-06 08:08:49.000000 unstructured_api_tools-0.9.2/unstructured_api_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:08:49.000000 unstructured_api_tools-0.9.2/unstructured_api_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-06 08:08:49.000000 unstructured_api_tools-0.9.2/unstructured_api_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-06 08:08:49.000000 unstructured_api_tools-0.9.2/unstructured_api_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-06 08:08:49.000000 unstructured_api_tools-0.9.2/unstructured_api_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:39:08.853967 unstructured_api_tools-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-10 17:39:08.853967 unstructured_api_tools-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-10 17:39:08.857967 unstructured_api_tools-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:39:08.849966 unstructured_api_tools-0.9.3/unstructured_api_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/unstructured_api_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/unstructured_api_tools/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/unstructured_api_tools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:39:08.853967 unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/api_conventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15564 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:39:08.853967 unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    16773 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/templates/pipeline_api.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-10 17:38:59.000000 unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/templates/pipeline_app.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:39:08.853967 unstructured_api_tools-0.9.3/unstructured_api_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-10 17:39:08.000000 unstructured_api_tools-0.9.3/unstructured_api_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-10 17:39:08.000000 unstructured_api_tools-0.9.3/unstructured_api_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:39:08.000000 unstructured_api_tools-0.9.3/unstructured_api_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-10 17:39:08.000000 unstructured_api_tools-0.9.3/unstructured_api_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-10 17:39:08.000000 unstructured_api_tools-0.9.3/unstructured_api_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-10 17:39:08.000000 unstructured_api_tools-0.9.3/unstructured_api_tools.egg-info/top_level.txt
```

### Comparing `unstructured_api_tools-0.9.2/LICENSE.md` & `unstructured_api_tools-0.9.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured_api_tools-0.9.2/PKG-INFO` & `unstructured_api_tools-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured_api_tools
-Version: 0.9.2
+Version: 0.9.3
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured-api-tools
 Author: Unstructured Technologies
 Author-email: mrobinson@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_api_tools-0.9.2/README.md` & `unstructured_api_tools-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `unstructured_api_tools-0.9.2/setup.py` & `unstructured_api_tools-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured_api_tools-0.9.2/unstructured_api_tools/cli.py` & `unstructured_api_tools-0.9.3/unstructured_api_tools/cli.py`

 * *Files identical despite different names*

### Comparing `unstructured_api_tools-0.9.2/unstructured_api_tools/pipelines/api_conventions.py` & `unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/api_conventions.py`

 * *Files identical despite different names*

### Comparing `unstructured_api_tools-0.9.2/unstructured_api_tools/pipelines/convert.py` & `unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/convert.py`

 * *Files identical despite different names*

### Comparing `unstructured_api_tools-0.9.2/unstructured_api_tools/pipelines/lint.py` & `unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/lint.py`

 * *Files identical despite different names*

### Comparing `unstructured_api_tools-0.9.2/unstructured_api_tools/pipelines/templates/pipeline_api.txt` & `unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/templates/pipeline_api.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 def get_validated_mimetype(file):
     """
     Return a file's mimetype, either via the file.content_type or the mimetypes lib if that's too
     generic. If the user has set UNSTRUCTURED_ALLOWED_MIMETYPES, validate against this list and
     return HTTP 400 for an invalid type.
     """
     content_type = file.content_type
-    if content_type == "application/octet-stream":
+    if not content_type or content_type == "application/octet-stream":
         content_type = mimetypes.guess_type(str(file.filename))[0]
 
         # Markdown mimetype is too new for the library - just hardcode that one in for now
         if not content_type and ".md" in file.filename:
             content_type = "text/markdown"
 
     allowed_mimetypes_str = os.environ.get("UNSTRUCTURED_ALLOWED_MIMETYPES")
@@ -205,15 +205,15 @@
 
             for file in files_list:
                 _file = file.file
 
                 {% if "file_content_type" in optional_param_value_map %}
                 file_content_type = get_validated_mimetype(file)
                 {% else %}
-                _ = get_validated_mimetype(file)
+                get_validated_mimetype(file)
                 {% endif %}
 
                 response = pipeline_api(
                     text=None,
                     file=_file,
                     {% for param in multi_string_param_names %}m_{{param}}={{param}}, {% endfor %}
                     {% if default_response_type %}response_type=media_type, {% endif %}
@@ -246,15 +246,15 @@
         elif has_files:
             file = files_list[0]
             _file = file.file
 
             {% if "file_content_type" in optional_param_value_map %}
             file_content_type = get_validated_mimetype(file)
             {% else %}
-            _ = get_validated_mimetype(file)
+            get_validated_mimetype(file)
             {% endif %}
 
             response = pipeline_api(
                 text=None,
                 file=_file,
                 {% for param in multi_string_param_names %}m_{{param}}={{param}}, {% endfor %}
                 {% if default_response_type %}response_type=media_type,{% endif %}
@@ -293,15 +293,15 @@
                 )
             def response_generator(is_multipart):
                 for file in {{var_name}}:
 
                     {% if "file_content_type" in optional_param_value_map %}
                     file_content_type = get_validated_mimetype(file)
                     {% else %}
-                    _ = get_validated_mimetype(file)
+                    get_validated_mimetype(file)
                     {% endif %}
 
                     {% if accepts_text %}
                     text = file.file.read().decode("utf-8")
                     {% elif accepts_file %}
                     _file = file.file
                     {% endif %}
@@ -334,15 +334,15 @@
             {% elif accepts_file %}
             file = files[0]
             _file = file.file
 
             {% if "file_content_type" in optional_param_value_map %}
             file_content_type = get_validated_mimetype(file)
             {% else %}
-            _ = get_validated_mimetype(file)
+            get_validated_mimetype(file)
             {% endif %}
             {% endif %}
 
             response = pipeline_api(
                 {% if accepts_text %}text, {% elif accepts_file %}_file, {% endif %}
                 {% for param in multi_string_param_names %}m_{{param}}={{param}}, {% endfor %}
                 {% if default_response_type %}response_type=media_type,{% endif %}
@@ -394,15 +394,8 @@
         )
     {% else %}
     return response
     {% endif %}
 {% endif %}
 
 
-@app.get("/healthcheck", status_code=status.HTTP_200_OK)
-def healthcheck(request: Request):
-    return {
-        "healthcheck": "HEALTHCHECK STATUS: EVERYTHING OK!"
-    }
-
-
 app.include_router(router)
```

### Comparing `unstructured_api_tools-0.9.2/unstructured_api_tools/pipelines/templates/pipeline_app.txt` & `unstructured_api_tools-0.9.3/unstructured_api_tools/pipelines/templates/pipeline_app.txt`

 * *Files 18% similar despite different names*

```diff
@@ -17,10 +17,10 @@
   docs_url="{{ '/' ~ version_name ~ '/docs' if version_name else '/docs' }}"
 )
 
 {% for module in module_names -%}
 app.include_router({{ module }}_router)
 {% endfor %}
 
-@app.get("/healthcheck", status_code=status.HTTP_200_OK)
+@app.get("/healthcheck", status_code=status.HTTP_200_OK, include_in_schema=False)
 def healthcheck(request: Request):
     return {"healthcheck": "HEALTHCHECK STATUS: EVERYTHING OK!"}
```

### Comparing `unstructured_api_tools-0.9.2/unstructured_api_tools.egg-info/PKG-INFO` & `unstructured_api_tools-0.9.3/unstructured_api_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured-api-tools
-Version: 0.9.2
+Version: 0.9.3
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured-api-tools
 Author: Unstructured Technologies
 Author-email: mrobinson@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_api_tools-0.9.2/unstructured_api_tools.egg-info/SOURCES.txt` & `unstructured_api_tools-0.9.3/unstructured_api_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*


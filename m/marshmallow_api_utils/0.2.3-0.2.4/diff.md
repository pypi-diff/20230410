# Comparing `tmp/marshmallow_api_utils-0.2.3.tar.gz` & `tmp/marshmallow_api_utils-0.2.4.tar.gz`

## Comparing `marshmallow_api_utils-0.2.3.tar` & `marshmallow_api_utils-0.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/.editorconfig
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/local.ipynb
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/__init__.py
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/fields.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/flask_blueprint.py
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/ma_dataclass.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/package_finder.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/middleware/__init__.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/middleware/flask_logging_middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/models/__init__.py
--rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/models/date_time_filter.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/models/pageable.py
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/models/sortable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/tests/test_date_filter_parsing.py
--rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/tests/test_date_filter_sql_generator.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/tests/test_flask.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/tests/test_sortable.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/tests/utils.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/LICENSE.md
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/README.md
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/.editorconfig
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/local.ipynb
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/marshmallow_api_utils/__init__.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/marshmallow_api_utils/fields.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/marshmallow_api_utils/flask_blueprint.py
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/marshmallow_api_utils/ma_dataclass.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/marshmallow_api_utils/package_finder.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/marshmallow_api_utils/middleware/__init__.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/marshmallow_api_utils/middleware/flask_logging_middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/marshmallow_api_utils/models/__init__.py
+-rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/marshmallow_api_utils/models/date_time_filter.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/marshmallow_api_utils/models/pageable.py
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/marshmallow_api_utils/models/sortable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/tests/test_date_filter_parsing.py
+-rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/tests/test_date_filter_sql_generator.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/tests/test_flask.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/tests/test_sortable.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/tests/utils.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/LICENSE.md
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/README.md
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.4/PKG-INFO
```

### Comparing `marshmallow_api_utils-0.2.3/.pre-commit-config.yaml` & `marshmallow_api_utils-0.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.3/local.ipynb` & `marshmallow_api_utils-0.2.4/local.ipynb`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.3/marshmallow_api_utils/fields.py` & `marshmallow_api_utils-0.2.4/marshmallow_api_utils/fields.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.3/marshmallow_api_utils/flask_blueprint.py` & `marshmallow_api_utils-0.2.4/marshmallow_api_utils/flask_blueprint.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.3/marshmallow_api_utils/ma_dataclass.py` & `marshmallow_api_utils-0.2.4/marshmallow_api_utils/ma_dataclass.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.3/marshmallow_api_utils/package_finder.py` & `marshmallow_api_utils-0.2.4/marshmallow_api_utils/package_finder.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.3/marshmallow_api_utils/middleware/flask_logging_middleware.py` & `marshmallow_api_utils-0.2.4/marshmallow_api_utils/middleware/flask_logging_middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import time
 
 try:
-    from flask import Flask, current_app, request
+    from flask import Flask, Response, current_app, request
 except ImportError:
     raise Exception("flask must be installed to use FlaskBlueprint") from None
 
 try:
     import flask_log_request_id
     from flask_log_request_id import RequestID, current_request_id
 except ImportError:
@@ -35,15 +35,15 @@
         with app.app_context():
 
             @app.before_request
             def start_timer():
                 request.start_time = time.time()
 
             @app.after_request
-            def log_request(response):
+            def log_request(response: Response) -> Response:
 
                 log_fields = {}
                 log_fields['authorisation'] = request.authorization
                 log_fields['connection'] = request.headers.get('Connection')
                 log_fields['content_length'] = response.headers.get('Content-Length')
                 log_fields['content_md5'] = request.content_md5
                 log_fields['content_type'] = request.content_type
@@ -76,7 +76,9 @@
                 log_fields['useragent'] = request.user_agent
 
                 for header in x_headers:
                     if request.headers.get(header):
                         log_fields[header.lower().replace('-', '_')] = request.headers.get(header)
 
                 logging.getLogger(current_app.name).info("Request complete.", extra=log_fields)
+
+                return response
```

### Comparing `marshmallow_api_utils-0.2.3/marshmallow_api_utils/models/date_time_filter.py` & `marshmallow_api_utils-0.2.4/marshmallow_api_utils/models/date_time_filter.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.3/marshmallow_api_utils/models/pageable.py` & `marshmallow_api_utils-0.2.4/marshmallow_api_utils/models/pageable.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.3/marshmallow_api_utils/models/sortable.py` & `marshmallow_api_utils-0.2.4/marshmallow_api_utils/models/sortable.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.3/tests/test_date_filter_parsing.py` & `marshmallow_api_utils-0.2.4/tests/test_date_filter_parsing.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.3/tests/test_date_filter_sql_generator.py` & `marshmallow_api_utils-0.2.4/tests/test_date_filter_sql_generator.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.3/tests/test_sortable.py` & `marshmallow_api_utils-0.2.4/tests/test_sortable.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.3/tests/utils.py` & `marshmallow_api_utils-0.2.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.3/.gitignore` & `marshmallow_api_utils-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.3/LICENSE.md` & `marshmallow_api_utils-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.3/README.md` & `marshmallow_api_utils-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.3/pyproject.toml` & `marshmallow_api_utils-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.3/PKG-INFO` & `marshmallow_api_utils-0.2.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marshmallow_api_utils
-Version: 0.2.3
+Version: 0.2.4
 Summary: Marshmallow API Utilities
 Project-URL: Homepage, https://github.com/mvanderlee/marshmallow_api_utils
 Author-email: Michiel Vanderlee <jmt.vanderlee@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```


# Comparing `tmp/marshmallow_api_utils-0.2.2.tar.gz` & `tmp/marshmallow_api_utils-0.2.3.tar.gz`

## Comparing `marshmallow_api_utils-0.2.2.tar` & `marshmallow_api_utils-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/.editorconfig
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/local.ipynb
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/__init__.py
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/fields.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/flask_blueprint.py
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/ma_dataclass.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/package_finder.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/middleware/__init__.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/middleware/flask_logging_middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/models/__init__.py
--rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/models/date_time_filter.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/models/pageable.py
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/models/sortable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/tests/test_date_filter_parsing.py
--rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/tests/test_date_filter_sql_generator.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/tests/test_sortable.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/tests/utils.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/LICENSE.md
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/README.md
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/.editorconfig
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/local.ipynb
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/__init__.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/fields.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/flask_blueprint.py
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/ma_dataclass.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/package_finder.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/middleware/__init__.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/middleware/flask_logging_middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/models/__init__.py
+-rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/models/date_time_filter.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/models/pageable.py
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/marshmallow_api_utils/models/sortable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/tests/test_date_filter_parsing.py
+-rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/tests/test_date_filter_sql_generator.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/tests/test_flask.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/tests/test_sortable.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/tests/utils.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/LICENSE.md
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/README.md
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.3/PKG-INFO
```

### Comparing `marshmallow_api_utils-0.2.2/.pre-commit-config.yaml` & `marshmallow_api_utils-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.2/local.ipynb` & `marshmallow_api_utils-0.2.3/local.ipynb`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.2/marshmallow_api_utils/fields.py` & `marshmallow_api_utils-0.2.3/marshmallow_api_utils/fields.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.2/marshmallow_api_utils/flask_blueprint.py` & `marshmallow_api_utils-0.2.3/marshmallow_api_utils/flask_blueprint.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.2/marshmallow_api_utils/ma_dataclass.py` & `marshmallow_api_utils-0.2.3/marshmallow_api_utils/ma_dataclass.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.2/marshmallow_api_utils/package_finder.py` & `marshmallow_api_utils-0.2.3/marshmallow_api_utils/package_finder.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.2/marshmallow_api_utils/middleware/flask_logging_middleware.py` & `marshmallow_api_utils-0.2.3/marshmallow_api_utils/middleware/flask_logging_middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     'X-Real-Ip',
     'X-Forwarded-For',
     'X-Forwarded-Host',
     'X-Forwarded-Uri',
 ]
 
 
-class Log:
+class FlaskLoggingMiddleware:
 
     def __init__(self, app: Flask = None):
         self.app = app
         if app is not None:
             self.init_app(app)
 
     def init_app(self, app: Flask):
@@ -48,15 +48,15 @@
                 log_fields['content_md5'] = request.content_md5
                 log_fields['content_type'] = request.content_type
                 log_fields['cookies'] = request.cookies
                 log_fields['dest_host'] = request.host.split(':', 1)[0]
                 log_fields['dest_port'] = int(request.host.split(':', 1)[1]) if len(
                     request.host.split(':', 1),
                 ) == 2 else 80
-                log_fields['duration'] = time.time() - request.start_time.start
+                log_fields['duration'] = time.time() - request.start_time
                 log_fields['http_method'] = request.method
                 log_fields['http_status'] = response.status_code
                 log_fields['mimetype'] = request.mimetype
                 log_fields['referrer'] = request.referrer
 
                 if flask_log_request_id:
                     log_fields['request_id'] = current_request_id()
```

### Comparing `marshmallow_api_utils-0.2.2/marshmallow_api_utils/models/date_time_filter.py` & `marshmallow_api_utils-0.2.3/marshmallow_api_utils/models/date_time_filter.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.2/marshmallow_api_utils/models/pageable.py` & `marshmallow_api_utils-0.2.3/marshmallow_api_utils/models/pageable.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.2/marshmallow_api_utils/models/sortable.py` & `marshmallow_api_utils-0.2.3/marshmallow_api_utils/models/sortable.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.2/tests/test_date_filter_parsing.py` & `marshmallow_api_utils-0.2.3/tests/test_date_filter_parsing.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.2/tests/test_date_filter_sql_generator.py` & `marshmallow_api_utils-0.2.3/tests/test_date_filter_sql_generator.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.2/tests/test_sortable.py` & `marshmallow_api_utils-0.2.3/tests/test_sortable.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.2/tests/utils.py` & `marshmallow_api_utils-0.2.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.2/.gitignore` & `marshmallow_api_utils-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.2/LICENSE.md` & `marshmallow_api_utils-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.2/README.md` & `marshmallow_api_utils-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.2/pyproject.toml` & `marshmallow_api_utils-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 [project.urls]
 Homepage = "https://github.com/mvanderlee/marshmallow_api_utils"
 
 
 [project.optional-dependencies]
 test = [
   "coverage[toml] >= 6.5.0,< 8.0",
+  "flask >=2,<3",
+  "flask_log_request_id>=0.10.0,<1.0.0",
+  "flask-smorest >=0.40.0,<1",
   "isort >=5.0.6,<6.0.0",
   "mypy>=1.1.1,<2",
   "pytest >=7.1.3,<8.0.0",
   "ruff ==0.0.260",
 ]
 dev = [
   "hatch",
```

### Comparing `marshmallow_api_utils-0.2.2/PKG-INFO` & `marshmallow_api_utils-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marshmallow_api_utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: Marshmallow API Utilities
 Project-URL: Homepage, https://github.com/mvanderlee/marshmallow_api_utils
 Author-email: Michiel Vanderlee <jmt.vanderlee@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
@@ -41,14 +41,17 @@
 Requires-Dist: ruff==0.0.260; extra == 'dev'
 Provides-Extra: flask
 Requires-Dist: flask-log-request-id<1.0.0,>=0.10.0; extra == 'flask'
 Requires-Dist: flask-smorest<1,>=0.40.0; extra == 'flask'
 Requires-Dist: flask<3,>=2; extra == 'flask'
 Provides-Extra: test
 Requires-Dist: coverage[toml]<8.0,>=6.5.0; extra == 'test'
+Requires-Dist: flask-log-request-id<1.0.0,>=0.10.0; extra == 'test'
+Requires-Dist: flask-smorest<1,>=0.40.0; extra == 'test'
+Requires-Dist: flask<3,>=2; extra == 'test'
 Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'test'
 Requires-Dist: mypy<2,>=1.1.1; extra == 'test'
 Requires-Dist: pytest<8.0.0,>=7.1.3; extra == 'test'
 Requires-Dist: ruff==0.0.260; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Marshmallow API Utilities
```


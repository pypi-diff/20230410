# Comparing `tmp/marshmallow_api_utils-0.2.1.tar.gz` & `tmp/marshmallow_api_utils-0.2.2.tar.gz`

## Comparing `marshmallow_api_utils-0.2.1.tar` & `marshmallow_api_utils-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/.editorconfig
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/local.ipynb
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/__init__.py
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/fields.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/flask_blueprint.py
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/ma_dataclass.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/package_finder.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/middleware/__init__.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/middleware/flask_logging_middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/models/__init__.py
--rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/models/date_time_filter.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/models/pageable.py
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/models/sortable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/tests/test_date_filter_parsing.py
--rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/tests/test_date_filter_sql_generator.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/tests/test_sortable.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/tests/utils.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/LICENSE.md
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/README.md
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/.editorconfig
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/local.ipynb
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/__init__.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/fields.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/flask_blueprint.py
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/ma_dataclass.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/package_finder.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/middleware/__init__.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/middleware/flask_logging_middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/models/__init__.py
+-rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/models/date_time_filter.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/models/pageable.py
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/marshmallow_api_utils/models/sortable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/tests/test_date_filter_parsing.py
+-rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/tests/test_date_filter_sql_generator.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/tests/test_sortable.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/tests/utils.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/LICENSE.md
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/README.md
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.2/PKG-INFO
```

### Comparing `marshmallow_api_utils-0.2.1/.pre-commit-config.yaml` & `marshmallow_api_utils-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.1/local.ipynb` & `marshmallow_api_utils-0.2.2/local.ipynb`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.1/marshmallow_api_utils/fields.py` & `marshmallow_api_utils-0.2.2/marshmallow_api_utils/fields.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.1/marshmallow_api_utils/flask_blueprint.py` & `marshmallow_api_utils-0.2.2/marshmallow_api_utils/flask_blueprint.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.1/marshmallow_api_utils/ma_dataclass.py` & `marshmallow_api_utils-0.2.2/marshmallow_api_utils/ma_dataclass.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.1/marshmallow_api_utils/package_finder.py` & `marshmallow_api_utils-0.2.2/marshmallow_api_utils/package_finder.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.1/marshmallow_api_utils/middleware/flask_logging_middleware.py` & `marshmallow_api_utils-0.2.2/marshmallow_api_utils/middleware/flask_logging_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 try:
     from flask import Flask, current_app, request
 except ImportError:
     raise Exception("flask must be installed to use FlaskBlueprint") from None
 
 try:
+    import flask_log_request_id
     from flask_log_request_id import RequestID, current_request_id
 except ImportError:
     flask_log_request_id = None
 
 x_headers = [
     'X-Real-Ip',
     'X-Forwarded-For',
```

### Comparing `marshmallow_api_utils-0.2.1/marshmallow_api_utils/models/date_time_filter.py` & `marshmallow_api_utils-0.2.2/marshmallow_api_utils/models/date_time_filter.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.1/marshmallow_api_utils/models/pageable.py` & `marshmallow_api_utils-0.2.2/marshmallow_api_utils/models/pageable.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.1/marshmallow_api_utils/models/sortable.py` & `marshmallow_api_utils-0.2.2/marshmallow_api_utils/models/sortable.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.1/tests/test_date_filter_parsing.py` & `marshmallow_api_utils-0.2.2/tests/test_date_filter_parsing.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.1/tests/test_date_filter_sql_generator.py` & `marshmallow_api_utils-0.2.2/tests/test_date_filter_sql_generator.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.1/tests/test_sortable.py` & `marshmallow_api_utils-0.2.2/tests/test_sortable.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.1/tests/utils.py` & `marshmallow_api_utils-0.2.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.1/.gitignore` & `marshmallow_api_utils-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.1/LICENSE.md` & `marshmallow_api_utils-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.1/README.md` & `marshmallow_api_utils-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.1/pyproject.toml` & `marshmallow_api_utils-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.1/PKG-INFO` & `marshmallow_api_utils-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marshmallow_api_utils
-Version: 0.2.1
+Version: 0.2.2
 Summary: Marshmallow API Utilities
 Project-URL: Homepage, https://github.com/mvanderlee/marshmallow_api_utils
 Author-email: Michiel Vanderlee <jmt.vanderlee@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```


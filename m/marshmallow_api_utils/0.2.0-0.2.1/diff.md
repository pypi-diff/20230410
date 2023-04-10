# Comparing `tmp/marshmallow_api_utils-0.2.0.tar.gz` & `tmp/marshmallow_api_utils-0.2.1.tar.gz`

## Comparing `marshmallow_api_utils-0.2.0.tar` & `marshmallow_api_utils-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,24 @@
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/.editorconfig
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/local.ipynb
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/marshmallow_api_utils/__init__.py
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/marshmallow_api_utils/fields.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/marshmallow_api_utils/flask_blueprint.py
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/marshmallow_api_utils/ma_dataclass.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/marshmallow_api_utils/package_finder.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/marshmallow_api_utils/middleware/__init__.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/marshmallow_api_utils/middleware/flask_logging_middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/marshmallow_api_utils/models/__init__.py
--rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/marshmallow_api_utils/models/date_time_filter.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/marshmallow_api_utils/models/pageable.py
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/marshmallow_api_utils/models/sortable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/tests/test_date_filter_parsing.py
--rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/tests/test_date_filter_sql_generator.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/tests/test_sortable.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/tests/utils.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/README.md
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/.editorconfig
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/local.ipynb
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/__init__.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/fields.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/flask_blueprint.py
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/ma_dataclass.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/package_finder.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/middleware/__init__.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/middleware/flask_logging_middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/models/__init__.py
+-rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/models/date_time_filter.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/models/pageable.py
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/marshmallow_api_utils/models/sortable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/tests/test_date_filter_parsing.py
+-rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/tests/test_date_filter_sql_generator.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/tests/test_sortable.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/tests/utils.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/README.md
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.2.1/PKG-INFO
```

### Comparing `marshmallow_api_utils-0.2.0/.pre-commit-config.yaml` & `marshmallow_api_utils-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.0/local.ipynb` & `marshmallow_api_utils-0.2.1/local.ipynb`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.0/marshmallow_api_utils/fields.py` & `marshmallow_api_utils-0.2.1/marshmallow_api_utils/fields.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.0/marshmallow_api_utils/flask_blueprint.py` & `marshmallow_api_utils-0.2.1/marshmallow_api_utils/flask_blueprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Union
 
 from .package_finder import PackageFinder
 
 try:
     from flask import Blueprint as FlaskBlueprint
     from flask import Flask
-    from flask.views import MethodViewType
+    from flask.views import MethodView
 except ImportError:
     raise Exception("flask must be installed to use FlaskBlueprint") from None
 
 
 try:
     from flask_smorest import Api
     from flask_smorest import Blueprint as SmorestBlueprint
@@ -31,15 +31,15 @@
     def route(self, rule, *, parameters=None, document=True, **options):
         if document:
             return super().route(rule, parameters=parameters, **options)
         # Copy else case from Flask Blueprint
         else:
             def decorator(func):
                 endpoint = options.pop("endpoint", func.__name__)
-                if isinstance(func, MethodViewType):
+                if isinstance(func, MethodView):
                     view_func = func.as_view(endpoint)
                 else:
                     view_func = func
 
                 self.add_url_rule(rule, endpoint, view_func, **options)
                 return view_func
             return decorator
```

### Comparing `marshmallow_api_utils-0.2.0/marshmallow_api_utils/ma_dataclass.py` & `marshmallow_api_utils-0.2.1/marshmallow_api_utils/ma_dataclass.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.0/marshmallow_api_utils/package_finder.py` & `marshmallow_api_utils-0.2.1/marshmallow_api_utils/package_finder.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.0/marshmallow_api_utils/middleware/flask_logging_middleware.py` & `marshmallow_api_utils-0.2.1/marshmallow_api_utils/middleware/flask_logging_middleware.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.0/marshmallow_api_utils/models/date_time_filter.py` & `marshmallow_api_utils-0.2.1/marshmallow_api_utils/models/date_time_filter.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.0/marshmallow_api_utils/models/pageable.py` & `marshmallow_api_utils-0.2.1/marshmallow_api_utils/models/pageable.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.0/marshmallow_api_utils/models/sortable.py` & `marshmallow_api_utils-0.2.1/marshmallow_api_utils/models/sortable.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.0/tests/test_date_filter_parsing.py` & `marshmallow_api_utils-0.2.1/tests/test_date_filter_parsing.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.0/tests/test_date_filter_sql_generator.py` & `marshmallow_api_utils-0.2.1/tests/test_date_filter_sql_generator.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.0/tests/test_sortable.py` & `marshmallow_api_utils-0.2.1/tests/test_sortable.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.0/tests/utils.py` & `marshmallow_api_utils-0.2.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.0/.gitignore` & `marshmallow_api_utils-0.2.1/.gitignore`

 * *Files 20% similar despite different names*

```diff
@@ -62,34 +62,15 @@
 ### JetBrains template
 # Covers JetBrains IDEs: IntelliJ, RubyMine, PhpStorm, AppCode, PyCharm, CLion, Android Studio
 
 *.iml
 
 ## Directory-based project format:
 .idea/
-# if you remove the above rule, at least ignore the following:
 
-# User-specific stuff:
-# .idea/workspace.xml
-# .idea/tasks.xml
-# .idea/dictionaries
-
-# Sensitive or high-churn files:
-# .idea/dataSources.ids
-# .idea/dataSources.xml
-# .idea/sqlDataSources.xml
-# .idea/dynamic.xml
-# .idea/uiDesigner.xml
-
-# Gradle:
-# .idea/gradle.xml
-# .idea/libraries
-
-# Mongo Explorer plugin:
-# .idea/mongoSettings.xml
 
 ## File-based project format:
 *.ipr
 *.iws
 
 ## Plugin-specific files:
 
@@ -115,14 +96,16 @@
 .Python
 [Bb]in
 [Ii]nclude
 [Ll]ib
 pyvenv.cfg
 pip-selfcheck.json
 
+.ruff_cache
+
 .vscode
 .venv
 /.env
 .minio.sys/
 tests/data/minio/bucket1/Storage/
 scripts/*.jar
```

### Comparing `marshmallow_api_utils-0.2.0/LICENSE.md` & `marshmallow_api_utils-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.0/README.md` & `marshmallow_api_utils-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.0/pyproject.toml` & `marshmallow_api_utils-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.2.0/PKG-INFO` & `marshmallow_api_utils-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marshmallow_api_utils
-Version: 0.2.0
+Version: 0.2.1
 Summary: Marshmallow API Utilities
 Project-URL: Homepage, https://github.com/mvanderlee/marshmallow_api_utils
 Author-email: Michiel Vanderlee <jmt.vanderlee@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```


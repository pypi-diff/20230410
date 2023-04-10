# Comparing `tmp/fastapi_myhelper-0.1.5.1.tar.gz` & `tmp/fastapi_myhelper-0.1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_myhelper-0.1.5.1.tar", max compression
+gzip compressed data, was "fastapi_myhelper-0.1.5.2.tar", max compression
```

## Comparing `fastapi_myhelper-0.1.5.1.tar` & `fastapi_myhelper-0.1.5.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0        0 2023-02-03 07:51:10.857527 fastapi_myhelper-0.1.5.1/fastapi_myhelper/__init__.py
--rw-r--r--   0        0        0       28 2023-03-23 10:28:40.538865 fastapi_myhelper-0.1.5.1/fastapi_myhelper/pydantic/__init__.py
--rw-r--r--   0        0        0     4342 2023-03-27 10:57:11.408077 fastapi_myhelper-0.1.5.1/fastapi_myhelper/pydantic/meta.py
--rw-r--r--   0        0        0        0 2023-02-03 10:26:54.940734 fastapi_myhelper-0.1.5.1/fastapi_myhelper/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1367 2023-02-03 10:26:54.941812 fastapi_myhelper-0.1.5.1/fastapi_myhelper/sqlalchemy/pagination.py
--rw-r--r--   0        0        0      465 2023-02-03 10:26:54.942278 fastapi_myhelper-0.1.5.1/fastapi_myhelper/sqlalchemy/utils.py
--rw-r--r--   0        0        0       36 2023-03-23 10:28:40.539623 fastapi_myhelper-0.1.5.1/fastapi_myhelper/sqlmodel/__init__.py
--rw-r--r--   0        0        0      167 2023-03-25 13:25:21.863943 fastapi_myhelper-0.1.5.1/fastapi_myhelper/sqlmodel/meta.py
--rw-r--r--   0        0        0      149 2023-04-07 08:52:16.724050 fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/__init__.py
--rw-r--r--   0        0        0      509 2023-02-03 07:51:10.858340 fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/decorators.py
--rw-r--r--   0        0        0     3480 2023-02-03 07:51:10.877180 fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/exceptions.py
--rw-r--r--   0        0        0       22 2023-02-03 07:51:10.876992 fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/extentions/__init__.py
--rw-r--r--   0        0        0     2358 2023-02-03 07:51:10.876819 fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/extentions/errors.py
--rw-r--r--   0        0        0     2288 2023-04-07 13:17:41.551281 fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/relationship.py
--rw-r--r--   0        0        0       26 2023-02-03 07:51:10.859100 fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/schemas/__init__.py
--rw-r--r--   0        0        0     4053 2023-03-23 10:28:40.540283 fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/schemas/meta.py
--rw-r--r--   0        0        0     1898 2023-02-03 07:51:10.876431 fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/schemas/pagination.py
--rw-r--r--   0        0        0     1139 2023-02-03 07:56:07.978675 fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/schemas/schema.py
--rw-r--r--   0        0        0     1502 2023-02-03 07:51:10.876010 fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/schemas/type.py
--rw-r--r--   0        0        0       39 2023-02-03 07:51:10.875828 fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      536 2023-02-03 10:10:02.674710 fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/sqlalchemy/utils.py
--rw-r--r--   0        0        0       39 2023-02-03 07:51:10.875460 fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/sqlmodel/__init__.py
--rw-r--r--   0        0        0      547 2023-02-03 07:51:10.875291 fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/sqlmodel/utils.py
--rw-r--r--   0        0        0      326 2023-04-07 08:07:59.584631 fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/utils.py
--rw-r--r--   0        0        0        0 2023-02-03 07:51:10.860735 fastapi_myhelper-0.1.5.1/fastapi_myhelper/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-02-03 07:51:10.860888 fastapi_myhelper-0.1.5.1/fastapi_myhelper/tests/strawberry/__init__.py
--rw-r--r--   0        0        0     4734 2023-02-03 07:52:15.846049 fastapi_myhelper-0.1.5.1/fastapi_myhelper/tests/strawberry/test_pydantic.py
--rw-r--r--   0        0        0     3390 2023-02-03 07:51:34.114284 fastapi_myhelper-0.1.5.1/fastapi_myhelper/tests/strawberry/test_schema.py
--rw-r--r--   0        0        0     1242 2023-02-03 07:51:10.874520 fastapi_myhelper-0.1.5.1/fastapi_myhelper/tests/strawberry/test_sqlalchemy.py
--rw-r--r--   0        0        0      984 2023-02-03 07:51:10.874285 fastapi_myhelper-0.1.5.1/fastapi_myhelper/tests/strawberry/test_sqlmodel.py
--rw-r--r--   0        0        0     2037 2023-02-03 07:52:06.953217 fastapi_myhelper-0.1.5.1/fastapi_myhelper/tests/strawberry/test_validator.py
--rw-r--r--   0        0        0      788 2023-04-07 13:17:50.451675 fastapi_myhelper-0.1.5.1/pyproject.toml
--rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 fastapi_myhelper-0.1.5.1/setup.py
--rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 fastapi_myhelper-0.1.5.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-02-03 07:51:10.857527 fastapi_myhelper-0.1.5.2/fastapi_myhelper/__init__.py
+-rw-r--r--   0        0        0       28 2023-03-23 10:28:40.538865 fastapi_myhelper-0.1.5.2/fastapi_myhelper/pydantic/__init__.py
+-rw-r--r--   0        0        0     4342 2023-03-27 10:57:11.408077 fastapi_myhelper-0.1.5.2/fastapi_myhelper/pydantic/meta.py
+-rw-r--r--   0        0        0        0 2023-02-03 10:26:54.940734 fastapi_myhelper-0.1.5.2/fastapi_myhelper/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1367 2023-02-03 10:26:54.941812 fastapi_myhelper-0.1.5.2/fastapi_myhelper/sqlalchemy/pagination.py
+-rw-r--r--   0        0        0      465 2023-02-03 10:26:54.942278 fastapi_myhelper-0.1.5.2/fastapi_myhelper/sqlalchemy/utils.py
+-rw-r--r--   0        0        0       36 2023-03-23 10:28:40.539623 fastapi_myhelper-0.1.5.2/fastapi_myhelper/sqlmodel/__init__.py
+-rw-r--r--   0        0        0      167 2023-03-25 13:25:21.863943 fastapi_myhelper-0.1.5.2/fastapi_myhelper/sqlmodel/meta.py
+-rw-r--r--   0        0        0      149 2023-04-07 08:52:16.724050 fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/__init__.py
+-rw-r--r--   0        0        0      509 2023-02-03 07:51:10.858340 fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/decorators.py
+-rw-r--r--   0        0        0     3480 2023-02-03 07:51:10.877180 fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/exceptions.py
+-rw-r--r--   0        0        0       22 2023-02-03 07:51:10.876992 fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/extentions/__init__.py
+-rw-r--r--   0        0        0     2358 2023-02-03 07:51:10.876819 fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/extentions/errors.py
+-rw-r--r--   0        0        0     2570 2023-04-10 07:23:04.112037 fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/relationship.py
+-rw-r--r--   0        0        0       26 2023-02-03 07:51:10.859100 fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/schemas/__init__.py
+-rw-r--r--   0        0        0     4053 2023-03-23 10:28:40.540283 fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/schemas/meta.py
+-rw-r--r--   0        0        0     1898 2023-02-03 07:51:10.876431 fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/schemas/pagination.py
+-rw-r--r--   0        0        0     1139 2023-02-03 07:56:07.978675 fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/schemas/schema.py
+-rw-r--r--   0        0        0     1502 2023-02-03 07:51:10.876010 fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/schemas/type.py
+-rw-r--r--   0        0        0       39 2023-02-03 07:51:10.875828 fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      536 2023-02-03 10:10:02.674710 fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/sqlalchemy/utils.py
+-rw-r--r--   0        0        0       39 2023-02-03 07:51:10.875460 fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/sqlmodel/__init__.py
+-rw-r--r--   0        0        0      547 2023-02-03 07:51:10.875291 fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/sqlmodel/utils.py
+-rw-r--r--   0        0        0      326 2023-04-07 08:07:59.584631 fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/utils.py
+-rw-r--r--   0        0        0        0 2023-02-03 07:51:10.860735 fastapi_myhelper-0.1.5.2/fastapi_myhelper/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-03 07:51:10.860888 fastapi_myhelper-0.1.5.2/fastapi_myhelper/tests/strawberry/__init__.py
+-rw-r--r--   0        0        0     4734 2023-02-03 07:52:15.846049 fastapi_myhelper-0.1.5.2/fastapi_myhelper/tests/strawberry/test_pydantic.py
+-rw-r--r--   0        0        0     3390 2023-02-03 07:51:34.114284 fastapi_myhelper-0.1.5.2/fastapi_myhelper/tests/strawberry/test_schema.py
+-rw-r--r--   0        0        0     1242 2023-02-03 07:51:10.874520 fastapi_myhelper-0.1.5.2/fastapi_myhelper/tests/strawberry/test_sqlalchemy.py
+-rw-r--r--   0        0        0      984 2023-02-03 07:51:10.874285 fastapi_myhelper-0.1.5.2/fastapi_myhelper/tests/strawberry/test_sqlmodel.py
+-rw-r--r--   0        0        0     2037 2023-02-03 07:52:06.953217 fastapi_myhelper-0.1.5.2/fastapi_myhelper/tests/strawberry/test_validator.py
+-rw-r--r--   0        0        0      788 2023-04-10 07:28:14.392494 fastapi_myhelper-0.1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 fastapi_myhelper-0.1.5.2/setup.py
+-rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 fastapi_myhelper-0.1.5.2/PKG-INFO
```

### Comparing `fastapi_myhelper-0.1.5.1/fastapi_myhelper/pydantic/meta.py` & `fastapi_myhelper-0.1.5.2/fastapi_myhelper/pydantic/meta.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.5.1/fastapi_myhelper/sqlalchemy/pagination.py` & `fastapi_myhelper-0.1.5.2/fastapi_myhelper/sqlalchemy/pagination.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/exceptions.py` & `fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/extentions/errors.py` & `fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/extentions/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/relationship.py` & `fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/relationship.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,31 +10,36 @@
 
 
 @dataclass(frozen=True)
 class LazyType(InitialLazyType):
     back_populates: str | None = None
 
     def resolve_type(self) -> Type:
-        kls = super().resolve_type()
+        src_kls = super().resolve_type()
+        class_name = self.create_name(kls=src_kls)
+        src_kls._rel_classes = getattr(src_kls, '_rel_classes', {})
+        if class_name in src_kls._rel_classes:
+            return src_kls._rel_classes[class_name]
         kls = strawberry.type(
             type(
-                self.create_name(kls=kls),
-                (kls,), dict(kls.__dict__)
+                class_name,
+                (src_kls,), dict(src_kls.__dict__)
             ),
-            is_input=kls._type_definition.is_input,
-            is_interface=kls._type_definition.is_interface,
-            description=kls._type_definition.description,
-            directives=kls._type_definition.directives,
-            extend=kls._type_definition.extend
+            is_input=src_kls._type_definition.is_input,
+            is_interface=src_kls._type_definition.is_interface,
+            description=src_kls._type_definition.description,
+            directives=src_kls._type_definition.directives,
+            extend=src_kls._type_definition.extend
         )
         kls.__dataclass_fields__.pop(self.back_populates)
         for field_idx in range(len(kls._type_definition._fields)):
             if kls._type_definition._fields[field_idx].name == self.back_populates:
                 kls._type_definition._fields.pop(field_idx)
                 break
+        src_kls._rel_classes[class_name] = kls
         return kls
 
     def create_name(self, kls):
         return f"{kls._type_definition.name}{to_camel_case(self.back_populates.capitalize())}Rel"
 
 
 class StrawberryLazyReference(InitialStrawberryLazyReference):
```

### Comparing `fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/schemas/meta.py` & `fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/schemas/meta.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/schemas/pagination.py` & `fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/schemas/pagination.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/schemas/schema.py` & `fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/schemas/schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/schemas/type.py` & `fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/schemas/type.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/sqlalchemy/utils.py` & `fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/sqlalchemy/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.5.1/fastapi_myhelper/strawberry/sqlmodel/utils.py` & `fastapi_myhelper-0.1.5.2/fastapi_myhelper/strawberry/sqlmodel/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.5.1/fastapi_myhelper/tests/strawberry/test_pydantic.py` & `fastapi_myhelper-0.1.5.2/fastapi_myhelper/tests/strawberry/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.5.1/fastapi_myhelper/tests/strawberry/test_schema.py` & `fastapi_myhelper-0.1.5.2/fastapi_myhelper/tests/strawberry/test_schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.5.1/fastapi_myhelper/tests/strawberry/test_sqlalchemy.py` & `fastapi_myhelper-0.1.5.2/fastapi_myhelper/tests/strawberry/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.5.1/fastapi_myhelper/tests/strawberry/test_sqlmodel.py` & `fastapi_myhelper-0.1.5.2/fastapi_myhelper/tests/strawberry/test_sqlmodel.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.5.1/fastapi_myhelper/tests/strawberry/test_validator.py` & `fastapi_myhelper-0.1.5.2/fastapi_myhelper/tests/strawberry/test_validator.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.5.1/pyproject.toml` & `fastapi_myhelper-0.1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-myhelper"
-version = "0.1.5.1"
+version = "0.1.5.2"
 description = ""
 authors = ["MihaTeam1 <sarsern2004@gmail.com>"]
 packages = [{include = "fastapi_myhelper"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 strawberry-graphql = {version = "^0.155.3", optional = true}
```

### Comparing `fastapi_myhelper-0.1.5.1/setup.py` & `fastapi_myhelper-0.1.5.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'sqlmodel': ['sqlmodel>=0.0.8,<0.0.9',
               'sqlalchemy>=1.4.17,<=1.4.41',
               'pydantic>=1.10.4,<2.0.0'],
  'strawberry': ['strawberry-graphql>=0.155.3,<0.156.0']}
 
 setup_kwargs = {
     'name': 'fastapi-myhelper',
-    'version': '0.1.5.1',
+    'version': '0.1.5.2',
     'description': '',
     'long_description': 'None',
     'author': 'MihaTeam1',
     'author_email': 'sarsern2004@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fastapi_myhelper-0.1.5.1/PKG-INFO` & `fastapi_myhelper-0.1.5.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-myhelper
-Version: 0.1.5.1
+Version: 0.1.5.2
 Summary: 
 Author: MihaTeam1
 Author-email: sarsern2004@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


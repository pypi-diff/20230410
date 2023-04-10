# Comparing `tmp/sparkql-0.6.0.tar.gz` & `tmp/sparkql-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkql-0.6.0.tar", max compression
+gzip compressed data, was "sparkql-0.7.0.tar", max compression
```

## Comparing `sparkql-0.6.0.tar` & `sparkql-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1087 2020-01-19 12:25:48.235165 sparkql-0.6.0/LICENSE
--rw-r--r--   0        0        0    14716 2023-03-07 22:02:28.994626 sparkql-0.6.0/README.md
--rw-r--r--   0        0        0     1395 2023-03-07 22:15:28.486617 sparkql-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      952 2020-04-12 19:04:18.823954 sparkql-0.6.0/sparkql/__init__.py
--rw-r--r--   0        0        0     1066 2023-03-01 22:08:32.354004 sparkql-0.6.0/sparkql/accessors.py
--rw-r--r--   0        0        0     2387 2023-03-07 22:02:29.002743 sparkql-0.6.0/sparkql/exceptions.py
--rw-r--r--   0        0        0      491 2020-02-26 23:26:45.319133 sparkql-0.6.0/sparkql/fields/__init__.py
--rw-r--r--   0        0        0     5913 2023-03-07 22:02:29.003687 sparkql-0.6.0/sparkql/fields/array.py
--rw-r--r--   0        0        0     3822 2020-03-09 15:31:53.779323 sparkql-0.6.0/sparkql/fields/atomic.py
--rw-r--r--   0        0        0    12199 2023-03-07 22:02:29.004641 sparkql-0.6.0/sparkql/fields/base.py
--rw-r--r--   0        0        0    26425 2023-03-07 22:02:29.005560 sparkql-0.6.0/sparkql/fields/struct.py
--rw-r--r--   0        0        0     3436 2023-03-07 22:02:29.006288 sparkql-0.6.0/sparkql/formatters.py
--rw-r--r--   0        0        0      351 2020-02-26 23:26:45.333480 sparkql-0.6.0/sparkql/schema_builder.py
--rw-r--r--   0        0        0     5762 2023-03-05 00:46:37.657009 sparkql-0.6.0/sparkql/schema_merger.py
--rw-r--r--   0        0        0    15434 1970-01-01 00:00:00.000000 sparkql-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-04-10 20:40:55.925387 sparkql-0.7.0/LICENSE
+-rw-r--r--   0        0        0    14716 2023-04-10 20:40:55.925387 sparkql-0.7.0/README.md
+-rw-r--r--   0        0        0     1443 2023-04-10 20:41:40.449412 sparkql-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      952 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/__init__.py
+-rw-r--r--   0        0        0     1066 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/accessors.py
+-rw-r--r--   0        0        0     2387 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/exceptions.py
+-rw-r--r--   0        0        0      491 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/fields/__init__.py
+-rw-r--r--   0        0        0     5913 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/fields/array.py
+-rw-r--r--   0        0        0     4165 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/fields/atomic.py
+-rw-r--r--   0        0        0    12199 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/fields/base.py
+-rw-r--r--   0        0        0    26425 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/fields/struct.py
+-rw-r--r--   0        0        0     3436 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/formatters.py
+-rw-r--r--   0        0        0      351 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/schema_builder.py
+-rw-r--r--   0        0        0     5762 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/schema_merger.py
+-rw-r--r--   0        0        0    16521 1970-01-01 00:00:00.000000 sparkql-0.7.0/setup.py
+-rw-r--r--   0        0        0    15434 1970-01-01 00:00:00.000000 sparkql-0.7.0/PKG-INFO
```

### Comparing `sparkql-0.6.0/LICENSE` & `sparkql-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkql-0.6.0/README.md` & `sparkql-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `sparkql-0.6.0/pyproject.toml` & `sparkql-0.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sparkql"
-version = "0.6.0"  # do not edit manually. kept in sync with `tool.commitizen` config via automation
+version = "0.7.0"  # do not edit manually. kept in sync with `tool.commitizen` config via automation
 description = "sparkql: Apache Spark SQL DataFrame schema management for sensible humans"
 authors = ["Matt J Williams <mattjw@mattjw.net>"]
 repository = "https://github.com/mattjw/sparkql"
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
@@ -32,21 +32,22 @@
 test = "tasks:test"
 reformat = "tasks:reformat"
 lint = "tasks:lint"
 typecheck = "tasks:typecheck"
 verify-all = "tasks:verify_all"
 find-releasable-changes = "tasks:find_releasable_changes"
 prepare-release = "tasks:prepare_release"
+debug-auto-git-tag = "tasks:debug_auto_git_tag"
 
 [tool.black]
 line-length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.6.0"  # do not edit manually. kept in sync with `tool.poetry` config via automation
+version = "0.7.0"  # do not edit manually. kept in sync with `tool.poetry` config via automation
 tag_format = "v$version"
 
 [tool.coverage.run]
 branch = true
 
 [build-system]
 requires = ["poetry>=1.3"]
```

### Comparing `sparkql-0.6.0/sparkql/__init__.py` & `sparkql-0.7.0/sparkql/__init__.py`

 * *Files identical despite different names*

### Comparing `sparkql-0.6.0/sparkql/accessors.py` & `sparkql-0.7.0/sparkql/accessors.py`

 * *Files identical despite different names*

### Comparing `sparkql-0.6.0/sparkql/exceptions.py` & `sparkql-0.7.0/sparkql/exceptions.py`

 * *Files identical despite different names*

### Comparing `sparkql-0.6.0/sparkql/fields/array.py` & `sparkql-0.7.0/sparkql/fields/array.py`

 * *Files identical despite different names*

### Comparing `sparkql-0.6.0/sparkql/fields/atomic.py` & `sparkql-0.7.0/sparkql/fields/atomic.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,18 +61,30 @@
 #
 # DataType -> AtomicType -> NumericType -> FractionalType
 
 
 class Decimal(FractionalField):
     """Field for Spark's DecimalType."""
 
+    __precision: int
+    __scale: int
+
+    def __init__(self, precision: int = 10, scale: int = 0, **kwargs: Any) -> None:
+        super().__init__(**kwargs)
+        self.__precision = precision
+        self.__scale = scale
+
     @property
     def _spark_type_class(self) -> Type[DataType]:
         return DecimalType
 
+    @property
+    def _spark_data_type(self) -> DataType:
+        return DecimalType(self.__precision, self.__scale)
+
     def _validate_on_value(self, value: Any) -> None:
         super()._validate_on_value(value)
         _validate_value_type_for_field((decimal.Decimal,), value)
 
 
 class Double(FractionalField):
     """Field for Spark's DoubleType."""
```

### Comparing `sparkql-0.6.0/sparkql/fields/base.py` & `sparkql-0.7.0/sparkql/fields/base.py`

 * *Files identical despite different names*

### Comparing `sparkql-0.6.0/sparkql/fields/struct.py` & `sparkql-0.7.0/sparkql/fields/struct.py`

 * *Files identical despite different names*

### Comparing `sparkql-0.6.0/sparkql/formatters.py` & `sparkql-0.7.0/sparkql/formatters.py`

 * *Files identical despite different names*

### Comparing `sparkql-0.6.0/sparkql/schema_merger.py` & `sparkql-0.7.0/sparkql/schema_merger.py`

 * *Files identical despite different names*

### Comparing `sparkql-0.6.0/PKG-INFO` & `sparkql-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkql
-Version: 0.6.0
+Version: 0.7.0
 Summary: sparkql: Apache Spark SQL DataFrame schema management for sensible humans
 Home-page: https://github.com/mattjw/sparkql
 License: MIT
 Author: Matt J Williams
 Author-email: mattjw@mattjw.net
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```


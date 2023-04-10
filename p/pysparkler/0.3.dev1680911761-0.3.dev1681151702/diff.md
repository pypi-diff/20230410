# Comparing `tmp/pysparkler-0.3.dev1680911761.tar.gz` & `tmp/pysparkler-0.3.dev1681151702.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkler-0.3.dev1680911761.tar", max compression
+gzip compressed data, was "pysparkler-0.3.dev1681151702.tar", max compression
```

## Comparing `pysparkler-0.3.dev1680911761.tar` & `pysparkler-0.3.dev1681151702.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4137 2023-04-07 23:55:54.013854 pysparkler-0.3.dev1680911761/README.md
--rw-r--r--   0        0        0     1188 2023-04-07 23:56:01.881879 pysparkler-0.3.dev1680911761/pyproject.toml
--rw-r--r--   0        0        0      807 2023-04-07 23:55:54.017854 pysparkler-0.3.dev1680911761/pysparkler/__init__.py
--rw-r--r--   0        0        0     4142 2023-04-07 23:55:54.017854 pysparkler-0.3.dev1680911761/pysparkler/api.py
--rw-r--r--   0        0        0     3940 2023-04-07 23:55:54.017854 pysparkler-0.3.dev1680911761/pysparkler/base.py
--rw-r--r--   0        0        0     5681 2023-04-07 23:55:54.017854 pysparkler-0.3.dev1680911761/pysparkler/cli.py
--rw-r--r--   0        0        0    12402 2023-04-07 23:55:54.017854 pysparkler-0.3.dev1680911761/pysparkler/pyspark_24_to_30.py
--rw-r--r--   0        0        0     3967 2023-04-07 23:55:54.017854 pysparkler-0.3.dev1680911761/pysparkler/pyspark_31_to_32.py
--rw-r--r--   0        0        0     5001 1970-01-01 00:00:00.000000 pysparkler-0.3.dev1680911761/PKG-INFO
+-rw-r--r--   0        0        0     4137 2023-04-10 18:34:53.016618 pysparkler-0.3.dev1681151702/README.md
+-rw-r--r--   0        0        0     1188 2023-04-10 18:35:03.404803 pysparkler-0.3.dev1681151702/pyproject.toml
+-rw-r--r--   0        0        0      807 2023-04-10 18:34:53.016618 pysparkler-0.3.dev1681151702/pysparkler/__init__.py
+-rw-r--r--   0        0        0     3892 2023-04-10 18:34:53.016618 pysparkler-0.3.dev1681151702/pysparkler/api.py
+-rw-r--r--   0        0        0     3940 2023-04-10 18:34:53.016618 pysparkler-0.3.dev1681151702/pysparkler/base.py
+-rw-r--r--   0        0        0     5681 2023-04-10 18:34:53.016618 pysparkler-0.3.dev1681151702/pysparkler/cli.py
+-rw-r--r--   0        0        0    12484 2023-04-10 18:34:53.016618 pysparkler-0.3.dev1681151702/pysparkler/pyspark_24_to_30.py
+-rw-r--r--   0        0        0     3999 2023-04-10 18:34:53.016618 pysparkler-0.3.dev1681151702/pysparkler/pyspark_31_to_32.py
+-rw-r--r--   0        0        0     5001 1970-01-01 00:00:00.000000 pysparkler-0.3.dev1681151702/PKG-INFO
```

### Comparing `pysparkler-0.3.dev1680911761/README.md` & `pysparkler-0.3.dev1681151702/README.md`

 * *Files identical despite different names*

### Comparing `pysparkler-0.3.dev1680911761/pyproject.toml` & `pysparkler-0.3.dev1681151702/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysparkler"
-version = "0.3.dev1680911761"
+version = "0.3.dev1681151702"
 description = "A tool that upgrades your PySpark scripts to Spark 3.3 as per Spark migration Guideline"
 authors = ["Dhruv Pratap <dhruv.pratap@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/holdenk/spark-upgrade"
 repository = "https://github.com/holdenk/spark-upgrade"
 maintainers = [
```

### Comparing `pysparkler-0.3.dev1680911761/pysparkler/__init__.py` & `pysparkler-0.3.dev1681151702/pysparkler/__init__.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.3.dev1680911761/pysparkler/api.py` & `pysparkler-0.3.dev1681151702/pysparkler/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,45 +16,39 @@
 #  under the License.
 #
 import json
 
 import libcst as cst
 import nbformat
 
-from pysparkler.pyspark_24_to_30 import pyspark_24_to_30_transformers
-from pysparkler.pyspark_31_to_32 import pyspark_31_to_32_transformers
+from pysparkler.pyspark_24_to_30 import visit_pyspark_24_to_30
+from pysparkler.pyspark_31_to_32 import visit_pyspark_31_to_32
 
 
 class PySparkler:
     """Main class for PySparkler"""
 
     def __init__(
         self, from_pyspark: str = "2.4", to_pyspark: str = "3.0", dry_run: bool = False
     ):
         self.from_pyspark = from_pyspark
         self.to_pyspark = to_pyspark
         self.dry_run = dry_run
 
-    @property
-    def transformers(self):
-        return [
-            *pyspark_24_to_30_transformers(),
-            *pyspark_31_to_32_transformers(),
-        ]
-
     def upgrade_script(self, input_file: str, output_file: str | None = None) -> str:
         """Upgrade a PySpark Python script file to the latest version and provides comments as hints for manual
         changes"""
         # Parse the PySpark script written in version 2.4
         with open(input_file, encoding="utf-8") as f:
             original_code = f.read()
         original_tree = cst.parse_module(original_code)
 
         # Apply the re-writer to the AST
-        modified_tree = self.visit(original_tree)
+        modified_tree = visit_pyspark_24_to_30(original_tree)
+        modified_tree = visit_pyspark_31_to_32(modified_tree)
 
         if not self.dry_run:
             if output_file:
                 # Write the modified AST to the output file location
                 with open(output_file, "w", encoding="utf-8") as f:
                     f.write(modified_tree.code)
             else:
@@ -78,15 +72,16 @@
         nb = nbformat.read(input_file, as_version=nbformat.NO_CONVERT)
 
         # Apply the re-writer to the AST to each code cell
         for cell in nb.cells:
             if cell.cell_type == "code":
                 original_code = "".join(cell.source)
                 original_tree = cst.parse_module(original_code)
-                modified_tree = self.visit(original_tree)
+                modified_tree = visit_pyspark_24_to_30(original_tree)
+                modified_tree = visit_pyspark_31_to_32(modified_tree)
                 cell.source = modified_tree.code.splitlines(keepends=True)
 
         # Update the kernel name if requested
         if output_kernel_name:
             nb.metadata.kernelspec.name = output_kernel_name
             nb.metadata.kernelspec.display_name = output_kernel_name
 
@@ -96,13 +91,7 @@
                 nbformat.write(nb, output_file)
             else:
                 # Re-write the modified AST back to the input file
                 nbformat.write(nb, input_file)
 
         # Return the modified Jupyter Notebook as String
         return json.dumps(nb.dict(), indent=1)
-
-    def visit(self, module: cst.Module) -> cst.Module:
-        """Visit a CSTModule and apply the transformers"""
-        for transformer in self.transformers:
-            module = module.visit(transformer)
-        return module
```

### Comparing `pysparkler-0.3.dev1680911761/pysparkler/base.py` & `pysparkler-0.3.dev1681151702/pysparkler/base.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.3.dev1680911761/pysparkler/cli.py` & `pysparkler-0.3.dev1681151702/pysparkler/cli.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.3.dev1680911761/pysparkler/pyspark_24_to_30.py` & `pysparkler-0.3.dev1681151702/pysparkler/pyspark_24_to_30.py`

 * *Files 3% similar despite different names*

```diff
@@ -297,19 +297,19 @@
                     attr=m.Name("shared"),
                 ),
             ),
         ):
             self.match_found = True
 
 
-def pyspark_24_to_30_transformers() -> list[cst.CSTTransformer]:
-    """Return a list of transformers for PySpark 2.4 to 3.0 migration guide"""
-    return [
-        RequiredPandasVersionCommentWriter(),
-        ToPandasUsageTransformer(),
-        PandasUdfUsageTransformer(),
-        PyArrowEnabledCommentWriter(),
-        PandasConvertToArrowArraySafelyCommentWriter(),
-        CreateDataFrameVerifySchemaCommentWriter(),
-        RowFieldNamesNotSortedCommentWriter(),
-        MlParamMixinsSetterCommentWriter(),
-    ]
+def visit_pyspark_24_to_30(parsed_module: cst.Module) -> cst.Module:
+    """Visit a parsed module and add comments for PySpark 2.4 to 3.0 migration guide"""
+    return (
+        parsed_module.visit(RequiredPandasVersionCommentWriter())
+        .visit(ToPandasUsageTransformer())
+        .visit(PandasUdfUsageTransformer())
+        .visit(PyArrowEnabledCommentWriter())
+        .visit(PandasConvertToArrowArraySafelyCommentWriter())
+        .visit(CreateDataFrameVerifySchemaCommentWriter())
+        .visit(RowFieldNamesNotSortedCommentWriter())
+        .visit(MlParamMixinsSetterCommentWriter())
+    )
```

### Comparing `pysparkler-0.3.dev1680911761/pysparkler/pyspark_31_to_32.py` & `pysparkler-0.3.dev1681151702/pysparkler/pyspark_31_to_32.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,10 +95,10 @@
                 type=m.Name("ValueError"),
             ),
         ):
             if self._has_sql_or_ml_import:
                 self.match_found = True
 
 
-def pyspark_31_to_32_transformers() -> list[cst.CSTTransformer]:
-    """Return a list of transformers for PySpark 3.1 to 3.2 migration guide"""
-    return [SqlMlMethodsRaiseTypeErrorCommentWriter()]
+def visit_pyspark_31_to_32(parsed_module: cst.Module) -> cst.Module:
+    """Visit a parsed module and add comments for PySpark 3.1 to 3.2 migration guide"""
+    return parsed_module.visit(SqlMlMethodsRaiseTypeErrorCommentWriter())
```

### Comparing `pysparkler-0.3.dev1680911761/PKG-INFO` & `pysparkler-0.3.dev1681151702/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkler
-Version: 0.3.dev1680911761
+Version: 0.3.dev1681151702
 Summary: A tool that upgrades your PySpark scripts to Spark 3.3 as per Spark migration Guideline
 Home-page: https://github.com/holdenk/spark-upgrade
 License: Apache-2.0
 Author: Dhruv Pratap
 Author-email: dhruv.pratap@gmail.com
 Maintainer: Holden Karau
 Maintainer-email: holden@pigscanfly.ca
```


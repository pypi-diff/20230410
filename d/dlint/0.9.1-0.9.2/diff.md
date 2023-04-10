# Comparing `tmp/dlint-0.9.1-py2.py3-none-any.whl.zip` & `tmp/dlint-0.9.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 73890 bytes, number of entries: 107
--rw-r--r--  2.0 unx      565 b- defN 19-Nov-06 20:00 dlint/__init__.py
+Zip file size: 74004 bytes, number of entries: 107
+-rw-r--r--  2.0 unx      565 b- defN 19-Nov-21 21:03 dlint/__init__.py
 -rw-r--r--  2.0 unx     2317 b- defN 19-Nov-05 00:02 dlint/extension.py
 -rw-r--r--  2.0 unx     1846 b- defN 19-Oct-10 20:34 dlint/multi.py
--rw-r--r--  2.0 unx     2538 b- defN 19-Sep-12 15:56 dlint/namespace.py
+-rw-r--r--  2.0 unx     3157 b- defN 19-Nov-14 23:55 dlint/namespace.py
 -rw-r--r--  2.0 unx     5935 b- defN 19-Nov-05 23:06 dlint/tree.py
--rw-r--r--  2.0 unx      248 b- defN 19-Jul-19 20:32 dlint/util.py
+-rw-r--r--  2.0 unx      464 b- defN 19-Nov-14 23:27 dlint/util.py
 -rw-r--r--  2.0 unx     3208 b- defN 19-Nov-06 19:20 dlint/linters/__init__.py
 -rw-r--r--  2.0 unx      589 b- defN 19-May-21 13:23 dlint/linters/bad_commands_use.py
 -rw-r--r--  2.0 unx      948 b- defN 19-Oct-10 15:06 dlint/linters/bad_compile_use.py
 -rw-r--r--  2.0 unx     1116 b- defN 19-Oct-16 17:05 dlint/linters/bad_cryptography_module_attribute_use.py
 -rw-r--r--  2.0 unx     5877 b- defN 19-Sep-17 17:54 dlint/linters/bad_defusedxml_use.py
 -rw-r--r--  2.0 unx      707 b- defN 19-May-21 13:23 dlint/linters/bad_dl_use.py
 -rw-r--r--  2.0 unx     2113 b- defN 19-Oct-10 15:06 dlint/linters/bad_duo_client_use.py
@@ -39,15 +39,15 @@
 -rw-r--r--  2.0 unx     1058 b- defN 19-Oct-16 17:05 dlint/linters/bad_xmlsec_module_attribute_use.py
 -rw-r--r--  2.0 unx      817 b- defN 19-Oct-10 15:06 dlint/linters/bad_yaml_use.py
 -rw-r--r--  2.0 unx      765 b- defN 19-Oct-10 15:06 dlint/linters/bad_zipfile_use.py
 -rw-r--r--  2.0 unx      983 b- defN 19-Oct-10 20:34 dlint/linters/base.py
 -rw-r--r--  2.0 unx      535 b- defN 19-May-21 13:23 dlint/linters/helpers/__init__.py
 -rw-r--r--  2.0 unx      956 b- defN 19-Aug-16 19:46 dlint/linters/helpers/bad_builtin_use.py
 -rw-r--r--  2.0 unx     1688 b- defN 19-Oct-23 22:09 dlint/linters/helpers/bad_kwarg_use.py
--rw-r--r--  2.0 unx     3685 b- defN 19-Oct-10 20:15 dlint/linters/helpers/bad_module_attribute_use.py
+-rw-r--r--  2.0 unx     2597 b- defN 19-Nov-14 23:22 dlint/linters/helpers/bad_module_attribute_use.py
 -rw-r--r--  2.0 unx     2335 b- defN 19-Sep-11 19:17 dlint/linters/helpers/bad_module_use.py
 -rw-r--r--  2.0 unx     3540 b- defN 19-Oct-23 22:15 dlint/linters/helpers/bad_name_attribute_use.py
 -rw-r--r--  2.0 unx        0 b- defN 19-Nov-06 19:15 dlint/linters/twisted/__init__.py
 -rw-r--r--  2.0 unx     1374 b- defN 19-Nov-06 19:23 dlint/linters/twisted/inlinecallbacks_yield_statement.py
 -rw-r--r--  2.0 unx     1202 b- defN 19-Nov-06 19:23 dlint/linters/twisted/returnvalue_in_inlinecallbacks.py
 -rw-r--r--  2.0 unx     1467 b- defN 19-Nov-06 19:23 dlint/linters/twisted/yield_return_statement.py
 -rw-r--r--  2.0 unx      137 b- defN 19-May-21 13:23 dlint/test/__init__.py
@@ -89,21 +89,21 @@
 -rw-r--r--  2.0 unx     1519 b- defN 19-Sep-20 21:52 tests/test_extension.py
 -rw-r--r--  2.0 unx     2569 b- defN 19-Aug-24 20:36 tests/test_namespace.py
 -rw-r--r--  2.0 unx      428 b- defN 19-Nov-05 23:06 tests/test_tree.py
 -rw-r--r--  2.0 unx      299 b- defN 19-May-21 13:23 tests/test_util.py
 -rw-r--r--  2.0 unx        0 b- defN 19-May-21 13:23 tests/test_helpers/__init__.py
 -rw-r--r--  2.0 unx     2154 b- defN 19-Aug-24 20:36 tests/test_helpers/test_bad_builtin_use.py
 -rw-r--r--  2.0 unx    12981 b- defN 19-Oct-23 22:08 tests/test_helpers/test_bad_kwarg_use.py
--rw-r--r--  2.0 unx    13188 b- defN 19-Oct-10 20:15 tests/test_helpers/test_bad_module_attribute_use.py
+-rw-r--r--  2.0 unx    16353 b- defN 19-Nov-14 23:55 tests/test_helpers/test_bad_module_attribute_use.py
 -rw-r--r--  2.0 unx    10110 b- defN 19-Aug-24 20:39 tests/test_helpers/test_bad_module_use.py
 -rw-r--r--  2.0 unx    11044 b- defN 19-Oct-23 22:16 tests/test_helpers/test_bad_name_attribute_use.py
 -rw-r--r--  2.0 unx        0 b- defN 19-Nov-06 19:17 tests/test_twisted/__init__.py
 -rw-r--r--  2.0 unx    10554 b- defN 19-Sep-10 21:49 tests/test_twisted/test_inlinecallbacks_yield_statement.py
 -rw-r--r--  2.0 unx     9952 b- defN 19-Sep-10 22:02 tests/test_twisted/test_returnvalue_in_inlinecallbacks.py
 -rw-r--r--  2.0 unx     7826 b- defN 19-Aug-24 20:36 tests/test_twisted/test_yield_return_statement.py
--rw-rw-r--  2.0 unx     1457 b- defN 19-Nov-06 20:04 dlint-0.9.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5624 b- defN 19-Nov-06 20:04 dlint-0.9.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 19-Nov-06 20:04 dlint-0.9.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       58 b- defN 19-Nov-06 20:04 dlint-0.9.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 19-Nov-06 20:04 dlint-0.9.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     9523 b- defN 19-Nov-06 20:04 dlint-0.9.1.dist-info/RECORD
-107 files, 245564 bytes uncompressed, 58680 bytes compressed:  76.1%
+-rw-rw-r--  2.0 unx     1457 b- defN 19-Nov-21 21:06 dlint-0.9.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5624 b- defN 19-Nov-21 21:06 dlint-0.9.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 19-Nov-21 21:06 dlint-0.9.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       58 b- defN 19-Nov-21 21:06 dlint-0.9.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 19-Nov-21 21:06 dlint-0.9.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     9523 b- defN 19-Nov-21 21:06 dlint-0.9.2.dist-info/RECORD
+107 files, 248476 bytes uncompressed, 58794 bytes compressed:  76.3%
```

## zipnote {}

```diff
@@ -297,26 +297,26 @@
 
 Filename: tests/test_twisted/test_returnvalue_in_inlinecallbacks.py
 Comment: 
 
 Filename: tests/test_twisted/test_yield_return_statement.py
 Comment: 
 
-Filename: dlint-0.9.1.dist-info/LICENSE
+Filename: dlint-0.9.2.dist-info/LICENSE
 Comment: 
 
-Filename: dlint-0.9.1.dist-info/METADATA
+Filename: dlint-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: dlint-0.9.1.dist-info/WHEEL
+Filename: dlint-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: dlint-0.9.1.dist-info/entry_points.txt
+Filename: dlint-0.9.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: dlint-0.9.1.dist-info/top_level.txt
+Filename: dlint-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dlint-0.9.1.dist-info/RECORD
+Filename: dlint-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dlint/__init__.py

```diff
@@ -9,14 +9,14 @@
 from . import multi  # noqa F401
 from . import namespace  # noqa F401
 from . import test  # noqa F401
 from . import tree  # noqa F401
 from . import util  # noqa F401
 
 __name__ = 'dlint'
-__version__ = '0.9.1'
+__version__ = '0.9.2'
 __description__ = (
     "Dlint is a tool for encouraging best coding practices "
     "and helping ensure we're writing secure Python code."
 )
 __url__ = 'https://github.com/duo-labs/dlint'
 __license__ = 'BSD-3-Clause'
```

## dlint/namespace.py

```diff
@@ -6,14 +6,16 @@
     print_function,
     unicode_literals,
 )
 
 import ast
 import copy
 
+from . import util
+
 
 class Namespace(object):
     def __init__(self, imports, from_imports):
         self.imports = imports
         self.from_imports = from_imports
 
     @classmethod
@@ -45,39 +47,41 @@
         return any(
             alias_includes_name(alias)
             for imp in self.imports + self.from_imports
             for alias in imp.names
         )
 
     def illegal_module_imported(self, module_path, illegal_module_path):
-        modules = module_path.split('.')
+        modules = module_path.split('.') if module_path else []
+        illegal_modules = illegal_module_path.split('.')
 
-        # 'm1.m2.m3.m4' -> ['m1', 'm1.m2', 'm1.m2.m3', 'm1.m2.m3.m4']
-        nested_module_imports = [
-            '.'.join(modules[:i + 1])
-            for i in range(len(modules))
-        ]
-        nested_module_imported = any(
-            (
-                alias.name == nested_module_import
-                and module_path == illegal_module_path
-            )
-            for imp in self.imports
-            for alias in imp.names
-            for nested_module_import in nested_module_imports
-        )
-        if nested_module_imported:
-            return True
+        module_imported = False
+        canonicalized_modules = modules
 
-        nested_module_from_imported = any(
-            (
-                alias.name == modules[0]
-                and (imp.module + '.' + module_path) == illegal_module_path
-            )
-            for imp in self.from_imports
-            for alias in imp.names
-            if imp.module is not None  # Relative import, e.g. 'from .'
-        )
-        if nested_module_from_imported:
-            return True
+        for imp in self.imports:
+            for alias in imp.names:
+                if util.lstartswith(illegal_modules, alias.name.split('.')):
+                    module_imported = True
+                if modules and modules[0] == alias.asname:
+                    # 'import foo.bar as baz', 'baz.qux' -> 'foo.bar.baz'
+                    canonicalized_modules = alias.name.split('.') + modules[1:]
+
+        for imp in self.from_imports:
+            if not imp.module:
+                continue  # Relative import, e.g. 'from .'
+
+            imp_modules = imp.module.split('.')
+
+            for alias in imp.names:
+                if util.lstartswith(illegal_modules, imp_modules + [alias.name]):
+                    module_imported = True
+                if modules and modules[0] in [alias.name, alias.asname]:
+                    # 'from foo.bar import baz as qux', 'qux.quine' -> 'foo.bar.baz.quine'
+                    canonicalized_modules = imp_modules + [alias.name] + modules[1:]
+                if (util.lstartswith(illegal_modules, imp_modules)
+                        and illegal_modules[len(imp_modules):] == modules
+                        and alias.name == '*'):
+                    # 'from foo.bar import *', 'baz.qux' -> 'foo.bar.baz.qux'
+                    module_imported = True
+                    canonicalized_modules = imp_modules + modules
 
-        return False
+        return module_imported and (canonicalized_modules == illegal_modules)
```

## dlint/util.py

```diff
@@ -10,7 +10,19 @@
 import abc
 import sys
 
 if sys.version_info >= (3, 4):
     ABC = abc.ABC
 else:
     ABC = abc.ABCMeta(str('ABC'), (), {})
+
+
+def lstartswith(l1, l2):
+    if len(l2) > len(l1):
+        return False
+    return l1[:len(l2)] == l2
+
+
+def lendswith(l1, l2):
+    if len(l2) > len(l1):
+        return False
+    return l1[len(l1) - len(l2):] == l2
```

## dlint/linters/helpers/bad_module_attribute_use.py

```diff
@@ -15,106 +15,69 @@
 
 
 class BadModuleAttributeUseLinter(base.BaseLinter, util.ABC):
     """This abstract base class provides an simple interface for creating new
     lint rules that block bad attributes within a module.
     """
 
-    def __init__(self, *args, **kwargs):
-        self.illegal_wildcard_imports = []
-        self.illegal_calls = []
-        self.illegal_import_aliases = []
-
-        super(BadModuleAttributeUseLinter, self).__init__(*args, **kwargs)
-
     @property
     @abc.abstractmethod
     def illegal_module_attributes(self):
         """Subclasses must implement this property to return a dictionary
         that looks like:
 
             {
                 "module_name": [
                     "attribute_name1",
                     "attribute_name2",
                 ]
             }
         """
 
-    def get_results(self):
-        used_illegal_attributes = [
-            attributes
-            for module, attributes in self.illegal_module_attributes.items()
-            if module in self.illegal_wildcard_imports
-        ]
-
-        self.results.extend([
-            base.Flake8Result(
-                lineno=node.lineno,
-                col_offset=node.col_offset,
-                message=self._error_tmpl
-            )
-            for node in self.illegal_calls
-            if any(
-                node.id in attributes
-                for attributes in used_illegal_attributes
-            )
-        ])
-
-        return self.results
-
     def visit_Name(self, node):
-        illegal_call = any(
-            node.id in illegal_attributes
-            for illegal_attributes in self.illegal_module_attributes.values()
+        # Names have no module path by definition - i.e. they're a
+        # naked name in the namespace like 'Foo()' instead of 'bar.baz.Foo()'
+        name_module_path = ""
+
+        illegal_call_use = any(
+            node.id in attributes
+            and self.namespace.illegal_module_imported(name_module_path, illegal_module_path)
+            for illegal_module_path, attributes in self.illegal_module_attributes.items()
         )
 
-        if illegal_call:
-            self.illegal_calls.append(node)
+        if illegal_call_use:
+            self.results.append(
+                base.Flake8Result(
+                    lineno=node.lineno,
+                    col_offset=node.col_offset,
+                    message=self._error_tmpl
+                )
+            )
 
     def visit_Attribute(self, node):
         self.generic_visit(node)
 
         module_path = tree.module_path_str(node.value)
 
-        def illegal_module_used(illegal_module_path):
-            return (
-                self.namespace.illegal_module_imported(module_path, illegal_module_path)
-                or module_path in self.illegal_import_aliases
-            )
-
         illegal_attribute_use = any(
-            node.attr in attributes and illegal_module_used(illegal_module_path)
+            node.attr in attributes
+            and self.namespace.illegal_module_imported(module_path, illegal_module_path)
             for illegal_module_path, attributes in self.illegal_module_attributes.items()
         )
 
         if illegal_attribute_use:
             self.results.append(
                 base.Flake8Result(
                     lineno=node.lineno,
                     col_offset=node.col_offset,
                     message=self._error_tmpl
                 )
             )
 
-    def visit_Import(self, node):
-        self.illegal_import_aliases.extend([
-            alias.asname
-            for alias in node.names
-            if alias.asname is not None and alias.name in self.illegal_module_attributes
-        ])
-
     def visit_ImportFrom(self, node):
-        wildcard_import = any(
-            alias.name == '*'
-            for alias in node.names
-        )
-        if wildcard_import and node.module in self.illegal_module_attributes:
-            self.illegal_wildcard_imports.append(node.module)
-
         self.results.extend([
             base.Flake8Result(
                 lineno=node.lineno,
                 col_offset=node.col_offset,
                 message=self._error_tmpl
             )
             for module, attributes in self.illegal_module_attributes.items()
```

## tests/test_helpers/test_bad_module_attribute_use.py

```diff
@@ -348,14 +348,15 @@
         assert result == expected
 
     def test_module_attribute_missing_import_usage(self):
         python_node = self.get_ast_node(
             """
             import baz
             from qux import quine
+            from . import xyz
 
             var = 'echo "TEST"'
 
             foo = None
             foo.bar(var)
             """
         )
@@ -483,14 +484,123 @@
             """,
         ]
 
         for python_string in python_strings:
             python_node = self.get_ast_node(python_string)
 
             linter = get_bad_module_attribute_use_implementation({
+                'm1.m2.m3.m4': ['bad_attribute'],
+            })
+            linter.visit(python_node)
+
+            result = linter.get_results()
+            expected = [
+                dlint.linters.base.Flake8Result(
+                    lineno=3,
+                    col_offset=0,
+                    message=linter._error_tmpl
+                )
+            ]
+
+            assert result == expected
+
+    def test_module_attribute_arbitrary_import_as_depth_usage_new(self):
+        python_strings = [
+            """
+            import m1 as alias
+            alias.m2.m3.m4.bad_attribute()
+            """,
+            """
+            import m1.m2 as alias
+            alias.m3.m4.bad_attribute()
+            """,
+            """
+            import m1.m2.m3 as alias
+            alias.m4.bad_attribute()
+            """,
+            """
+            import m1.m2.m3.m4 as alias
+            alias.bad_attribute()
+            """,
+        ]
+
+        for python_string in python_strings:
+            python_node = self.get_ast_node(python_string)
+
+            linter = get_bad_module_attribute_use_implementation({
+                'm1.m2.m3.m4': ['bad_attribute'],
+            })
+            linter.visit(python_node)
+
+            result = linter.get_results()
+            expected = [
+                dlint.linters.base.Flake8Result(
+                    lineno=3,
+                    col_offset=0,
+                    message=linter._error_tmpl
+                )
+            ]
+
+            assert result == expected
+
+    def test_module_attribute_arbitrary_from_import_as_depth_usage_new(self):
+        python_strings = [
+            """
+            from m1 import m2 as alias
+            alias.m3.m4.bad_attribute()
+            """,
+            """
+            from m1.m2 import m3 as alias
+            alias.m4.bad_attribute()
+            """,
+            """
+            from m1.m2.m3 import m4 as alias
+            alias.bad_attribute()
+            """,
+        ]
+
+        for python_string in python_strings:
+            python_node = self.get_ast_node(python_string)
+
+            linter = get_bad_module_attribute_use_implementation({
+                'm1.m2.m3.m4': ['bad_attribute'],
+            })
+            linter.visit(python_node)
+
+            result = linter.get_results()
+            expected = [
+                dlint.linters.base.Flake8Result(
+                    lineno=3,
+                    col_offset=0,
+                    message=linter._error_tmpl
+                )
+            ]
+
+            assert result == expected
+
+    def test_module_attribute_arbitrary_from_import_wildcard_depth_usage_new(self):
+        python_strings = [
+            """
+            from m1 import *
+            m2.m3.m4.bad_attribute()
+            """,
+            """
+            from m1.m2 import *
+            m3.m4.bad_attribute()
+            """,
+            """
+            from m1.m2.m3 import *
+            m4.bad_attribute()
+            """,
+        ]
+
+        for python_string in python_strings:
+            python_node = self.get_ast_node(python_string)
+
+            linter = get_bad_module_attribute_use_implementation({
                 'm1.m2.m3.m4': ['bad_attribute'],
             })
             linter.visit(python_node)
 
             result = linter.get_results()
             expected = [
                 dlint.linters.base.Flake8Result(
```

## Comparing `dlint-0.9.1.dist-info/LICENSE` & `dlint-0.9.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dlint-0.9.1.dist-info/METADATA` & `dlint-0.9.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlint
-Version: 0.9.1
+Version: 0.9.2
 Summary: Dlint is a tool for encouraging best coding practices and helping ensure we're writing secure Python code.
 Home-page: https://github.com/duo-labs/dlint
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
@@ -55,18 +55,18 @@
 
 ```
 $ python -m flake8 -h
 Usage: flake8 [options] file file ...
 
 ...
 
-Installed plugins: dlint: 0.9.1, mccabe: 0.5.3, pycodestyle: 2.2.0, pyflakes: 1.3.0
+Installed plugins: dlint: 0.9.2, mccabe: 0.5.3, pycodestyle: 2.2.0, pyflakes: 1.3.0
 ```
 
-Note the `dlint: 0.9.1`.
+Note the `dlint: 0.9.2`.
 
 # Using
 
 Dlint uses `flake8` to perform its linting functionality which provides many
 useful features without re-inventing the wheel.
 
 ## CLI
```

## Comparing `dlint-0.9.1.dist-info/RECORD` & `dlint-0.9.2.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-dlint/__init__.py,sha256=wdRJUyznG4NhKeGyrCqrL_Abmr7aunaZijQiSQNfK4w,565
+dlint/__init__.py,sha256=TU8nap_tjS8P7ki8ADXpcS3OEBvoaW2b5gnxrF7V5xQ,565
 dlint/extension.py,sha256=U_t3CER_ekLRlp5Nh0FwvQUF8YqOaXTWQ3aZr0LtWvw,2317
 dlint/multi.py,sha256=1MoTpU1gWYkuoyECBpYZShcS3fD9Q-2owRtEnpc8Wc8,1846
-dlint/namespace.py,sha256=c0fEqrf2RJZ4ti9bKsByHlYpmK6j_Hcc3dRJQ7L-5Eg,2538
+dlint/namespace.py,sha256=Z_jauLfp5-FZWADn29xfiMs39yuazBomkQYng49Y9_I,3157
 dlint/tree.py,sha256=RrEmMUBCXe8FH6QcSeyXtz4keE4-ylShGXIhkR6qOmY,5935
-dlint/util.py,sha256=PY2J18a2W6VWKMqoRRF3JUUsiECCu8u-7cC1vYVW4tI,248
+dlint/util.py,sha256=Mnw613ZwfGcy9NrueHCsq_b1Oj3hUsvyK_0gyKV5L4M,464
 dlint/linters/__init__.py,sha256=Ex8Eg1vxfanmjm-_BfT46LTvSsSTtNutKLk6OaM9euY,3208
 dlint/linters/bad_commands_use.py,sha256=F9aH7vSLIFGbXM3VjlTeg175HIQ98-Byf9qgvGs7j58,589
 dlint/linters/bad_compile_use.py,sha256=OL7U_QAULumu-Y7xR-0YtB7k1BpFNQVDmkjbaFvKoig,948
 dlint/linters/bad_cryptography_module_attribute_use.py,sha256=WEGVnekXo3LBWWRnhX14EBtOYWv7bAC9jfgYW6HC4no,1116
 dlint/linters/bad_defusedxml_use.py,sha256=_8fh_oVJGlP0rUzkfUjM0Y-kpiVekpmCfR0T2AIuI8w,5877
 dlint/linters/bad_dl_use.py,sha256=ZX4Ili33f7EvhTb_oNAp8_J4wGGb-Sj_et-fUewgd0w,707
 dlint/linters/bad_duo_client_use.py,sha256=nnsCwJrxPDpSr9-qVurOsb9-FSlR0cxzdQoSWm6Ckd0,2113
@@ -38,15 +38,15 @@
 dlint/linters/bad_xmlsec_module_attribute_use.py,sha256=vQiEKVLJjVBY0dYaUqaXs5csrmnWTqxQ9vFSK7OpmA0,1058
 dlint/linters/bad_yaml_use.py,sha256=FexUkMLSeyTNhbu2B-nXz934l5ftiz2SBQvXOf1DB94,817
 dlint/linters/bad_zipfile_use.py,sha256=2geRX02XMESQF0Ob-Ujyn5qlHHITuWUB2xLUDGaN6Lc,765
 dlint/linters/base.py,sha256=otg_2O1lzZgRlLSZPTZShUrgOVTWcelrp8BGz6GOitk,983
 dlint/linters/helpers/__init__.py,sha256=lI5Q5q6FiQTsU3QnVorKBSaFIcC0AcZuaIkYaG_28Zk,535
 dlint/linters/helpers/bad_builtin_use.py,sha256=Hf3IDgaJyzSf2tPfgtHXfLJiblxTEHnMCOAHyaVt6Yk,956
 dlint/linters/helpers/bad_kwarg_use.py,sha256=QsUQ3xIXdgjq6X8F3TriODa1yKaCm7e4ojH3UgQx5GM,1688
-dlint/linters/helpers/bad_module_attribute_use.py,sha256=ESDp9VQxgiez8uM9gs6CdQvzsQjuHV7dzPO-qpc_aeY,3685
+dlint/linters/helpers/bad_module_attribute_use.py,sha256=WmrawqBuHDV7VaioPD9Mld857wwLIrbU4-m9LjLg_GU,2597
 dlint/linters/helpers/bad_module_use.py,sha256=U9_fpKbn28R27RFBRmut70-L0UB55YgZl-_BJdor288,2335
 dlint/linters/helpers/bad_name_attribute_use.py,sha256=hk7B5H8n0i_O05cyDaaETgxZ9Lxu0fLq0Gf4arESfLI,3540
 dlint/linters/twisted/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dlint/linters/twisted/inlinecallbacks_yield_statement.py,sha256=rDeOq_1v-K5snfXX6q9vpgH43VXJW4zfOjKkwfukJJQ,1374
 dlint/linters/twisted/returnvalue_in_inlinecallbacks.py,sha256=zw5pKZAGDp2Hf0R8GIxAhtgH7bci63eFpd3rWkL54cE,1202
 dlint/linters/twisted/yield_return_statement.py,sha256=6p39wT1BZd0ZoKMac520ii74vUqtsEmqhsw1ZX9Bieg,1467
 dlint/test/__init__.py,sha256=mlF0miDdWi3M9X2c_ZNMwi3TM9B6m38Gipzvct0N4_4,137
@@ -88,20 +88,20 @@
 tests/test_extension.py,sha256=deFYNF2DZTxcEvjgZCrXo4cVs6t7BYXqurE4va7Njhk,1519
 tests/test_namespace.py,sha256=F3zcvKCVgtEMzdLQVHLSEc8YdAy8raugPQkYUcU1N3M,2569
 tests/test_tree.py,sha256=LbBnThqtYMUNpPvpXt2_vkM7JS3YR1yBFUmUP87u_PI,428
 tests/test_util.py,sha256=QUBpw00yhEdlBsmce-PJj5XJQM8PqRr--IrfjcUoBgc,299
 tests/test_helpers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_helpers/test_bad_builtin_use.py,sha256=rxOyCBONX7wuDIo-2kqgHbeOU_aPQvRCLdGWL7rSChc,2154
 tests/test_helpers/test_bad_kwarg_use.py,sha256=mbIN_hGhA24YNrttqO1E-ttk2UfU7NanN2bYtyhSiRc,12981
-tests/test_helpers/test_bad_module_attribute_use.py,sha256=7gB1Z4JP6WObRFT9rUpT9J1hmCvA3KsmIWdHBHYHBBI,13188
+tests/test_helpers/test_bad_module_attribute_use.py,sha256=f1Laf9iO5A0XhDwFB5MlB4a4CAk76R6bfZ1KaBahTSA,16353
 tests/test_helpers/test_bad_module_use.py,sha256=qz5KMR2PeiqzbzTeqdNbmmbLdumkIVDddQg9-3pW92U,10110
 tests/test_helpers/test_bad_name_attribute_use.py,sha256=nnlfrqsywG3O32_YhANU7wvTU1V5LV80jPviqfGLLG4,11044
 tests/test_twisted/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_twisted/test_inlinecallbacks_yield_statement.py,sha256=QxWyMwbkTaGCKAVuTKG2tile2sOoGCt2DJPY35ZMl_w,10554
 tests/test_twisted/test_returnvalue_in_inlinecallbacks.py,sha256=lNP5MW5hmEX8aXkhSJLB0D2bpr2uL1aEWDQ-J3PiOWU,9952
 tests/test_twisted/test_yield_return_statement.py,sha256=Ym0loetnAHQj1lrDhmLdjKgG3oOS-UOzXe1KUO6hGlM,7826
-dlint-0.9.1.dist-info/LICENSE,sha256=OQD6fpL7Ttytpo1CJ7LYy1Tti40a181YmQVlAg25w3U,1457
-dlint-0.9.1.dist-info/METADATA,sha256=CC_QIeHrWxyZAnbXoUj20CobSs0FcEUS7kA3XRyzdc0,5624
-dlint-0.9.1.dist-info/WHEEL,sha256=8zNYZbwQSXoB9IfXOjPfeNwvAsALAjffgk27FqvCWbo,110
-dlint-0.9.1.dist-info/entry_points.txt,sha256=NDECDTASBEQYGdgeERdoBB_SL4rRZ-qBbvAH793QiDE,58
-dlint-0.9.1.dist-info/top_level.txt,sha256=oV5syBIjKTT_mggV42t1hAp53sZaim48KejzfW5ZcvI,12
-dlint-0.9.1.dist-info/RECORD,,
+dlint-0.9.2.dist-info/LICENSE,sha256=OQD6fpL7Ttytpo1CJ7LYy1Tti40a181YmQVlAg25w3U,1457
+dlint-0.9.2.dist-info/METADATA,sha256=R-yXijYwjmf792LuadL11Jqdk7w-3oEaeV5sMNCvMgw,5624
+dlint-0.9.2.dist-info/WHEEL,sha256=8zNYZbwQSXoB9IfXOjPfeNwvAsALAjffgk27FqvCWbo,110
+dlint-0.9.2.dist-info/entry_points.txt,sha256=NDECDTASBEQYGdgeERdoBB_SL4rRZ-qBbvAH793QiDE,58
+dlint-0.9.2.dist-info/top_level.txt,sha256=oV5syBIjKTT_mggV42t1hAp53sZaim48KejzfW5ZcvI,12
+dlint-0.9.2.dist-info/RECORD,,
```


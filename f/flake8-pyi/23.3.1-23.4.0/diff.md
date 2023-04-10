# Comparing `tmp/flake8_pyi-23.3.1.tar.gz` & `tmp/flake8_pyi-23.4.0.tar.gz`

## Comparing `flake8_pyi-23.3.1.tar` & `flake8_pyi-23.4.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/.editorconfig
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/.flake8
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    12839 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    80077 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/pyi.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/.github/scripts/typeshed_primer_download_errors.js
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/.github/scripts/typeshed_primer_post_comment.js
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/.github/workflows/check.yml
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/.github/workflows/typeshed_primer.yml
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/.github/workflows/typeshed_primer_comment.yml
--rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/aliases.pyi
--rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/attribute_annotations.pyi
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/calls.pyi
--rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/classdefs.pyi
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/comparisons.pyi
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/defaults.pyi
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/defaults_py38.pyi
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/del.pyi
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/emptyclasses.pyi
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/emptyfunctions.pyi
--rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/exit_methods.pyi
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/forward_refs.pyi
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/forward_refs_annassign.pyi
--rw-r--r--   0        0        0    10739 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/imports.pyi
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/names_requiring_values.pyi
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/never_vs_noreturn.pyi
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/pep604_union_types.pyi
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/quotes.pyi
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/sysplatform.pyi
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/sysversioninfo.pyi
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/test_pyi_files.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/type_comments.pyi
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/typevar.pyi
--rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/union_duplicates.pyi
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/unused_things.pyi
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/tests/vanilla_flake8_not_clean_forward_refs.pyi
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/LICENSE
--rw-r--r--   0        0        0    11861 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/README.md
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/pyproject.toml
--rw-r--r--   0        0        0    13904 2020-02-02 00:00:00.000000 flake8_pyi-23.3.1/PKG-INFO
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.editorconfig
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.flake8
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    12969 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    79960 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/pyi.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.github/scripts/typeshed_primer_download_errors.js
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.github/scripts/typeshed_primer_post_comment.js
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.github/workflows/check.yml
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.github/workflows/typeshed_primer.yml
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.github/workflows/typeshed_primer_comment.yml
+-rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/aliases.pyi
+-rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/attribute_annotations.pyi
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/calls.pyi
+-rw-r--r--   0        0        0     7111 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/classdefs.pyi
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/comparisons.pyi
+-rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/defaults.pyi
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/defaults_py38.pyi
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/del.pyi
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/emptyclasses.pyi
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/emptyfunctions.pyi
+-rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/exit_methods.pyi
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/forward_refs.pyi
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/forward_refs_annassign.pyi
+-rw-r--r--   0        0        0    10739 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/imports.pyi
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/names_requiring_values.pyi
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/never_vs_noreturn.pyi
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/pep604_union_types.pyi
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/quotes.pyi
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/sysplatform.pyi
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/sysversioninfo.pyi
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/test_pyi_files.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/type_comments.pyi
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/typevar.pyi
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/union_duplicates.pyi
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/unused_things.pyi
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/tests/vanilla_flake8_not_clean_forward_refs.pyi
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/LICENSE
+-rw-r--r--   0        0        0    11877 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/README.md
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/pyproject.toml
+-rw-r--r--   0        0        0    13920 2020-02-02 00:00:00.000000 flake8_pyi-23.4.0/PKG-INFO
```

### Comparing `flake8_pyi-23.3.1/.flake8` & `flake8_pyi-23.4.0/.flake8`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/.pre-commit-config.yaml` & `flake8_pyi-23.4.0/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-toml
       - id: check-merge-conflict
       - id: mixed-line-ending
   - repo: https://github.com/psf/black
-    rev: 23.1.0 # must match pyproject.toml
+    rev: 23.3.0 # must match pyproject.toml
     hooks:
       - id: black
         language_version: python3.7
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0 # must match pyproject.toml
     hooks:
       - id: isort
```

### Comparing `flake8_pyi-23.3.1/CHANGELOG.md` & `flake8_pyi-23.4.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # Change Log
 
-## 23.1.1
+## 23.4.0
+
+* Update error messages for Y019 and Y034 to recommend using
+  `typing_extensions.Self` rather than `_typeshed.Self`.
+
+## 23.3.1
 
 New error codes:
 * Y053: Disallow string or bytes literals with length >50 characters.
   Previously this rule only applied to parameter default values;
   it now applies everywhere.
 * Y054: Disallow numeric literals with a string representation >10 characters long.
   Previously this rule only applied to parameter default values;
```

### Comparing `flake8_pyi-23.3.1/CONTRIBUTING.md` & `flake8_pyi-23.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/pyi.py` & `flake8_pyi-23.4.0/pyi.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 if TYPE_CHECKING:
     # We don't have typing_extensions as a runtime dependency,
     # but all our annotations are stringized due to __future__ annotations,
     # and mypy thinks typing_extensions is part of the stdlib.
     from typing_extensions import Literal, TypeAlias, TypeGuard
 
-__version__ = "23.3.1"
+__version__ = "23.4.0"
 
 LOG = logging.getLogger("flake8.pyi")
 FLAKE8_MAJOR_VERSION = flake8.__version_info__[0]
 
 if sys.version_info >= (3, 9):
     _LiteralMember: TypeAlias = ast.expr
 else:
@@ -528,15 +528,15 @@
     }
 )
 
 
 def _has_bad_hardcoded_returns(
     method: ast.FunctionDef | ast.AsyncFunctionDef, *, classdef: ast.ClassDef
 ) -> bool:
-    """Return `True` if `function` should be rewritten using `_typeshed.Self`."""
+    """Return `True` if `function` should be rewritten using `typing_extensions.Self`."""
     # Much too complex for our purposes to worry
     # about overloaded functions or abstractmethods
     if any(
         _is_overload(deco) or _is_abstractmethod(deco) for deco in method.decorator_list
     ):
         return False
 
@@ -1645,22 +1645,17 @@
     def _Y034_error(
         self, node: ast.FunctionDef | ast.AsyncFunctionDef, cls_name: str
     ) -> None:
         method_name = node.name
         copied_node = deepcopy(node)
         copied_node.decorator_list.clear()
         copied_node.returns = ast.Name(id="Self")
-        first_arg = _non_kw_only_args_of(copied_node.args)[0]
         if method_name == "__new__":
-            first_arg.annotation = ast.Subscript(
-                value=ast.Name(id="type"), slice=ast.Name(id="Self")
-            )
             referrer = '"__new__" methods'
         else:
-            first_arg.annotation = ast.Name(id="Self")
             referrer = f'"{method_name}" methods in classes like "{cls_name}"'
         error_message = Y034.format(
             methods=referrer,
             method_name=f"{cls_name}.{method_name}",
             suggested_syntax=_unparse_func_node(copied_node),
         )
         self.error(node, error_message)
@@ -1746,14 +1741,16 @@
         self._visit_function(node)
 
     def _Y019_error(
         self, node: ast.FunctionDef | ast.AsyncFunctionDef, typevar_name: str
     ) -> None:
         cleaned_method = deepcopy(node)
         cleaned_method.decorator_list.clear()
+        first_arg = _non_kw_only_args_of(cleaned_method.args)[0]
+        first_arg.annotation = None
         new_syntax = _unparse_func_node(cleaned_method)
         new_syntax = re.sub(rf"\b{typevar_name}\b", "Self", new_syntax)
         self.error(
             # pass the node for the first argument to `self.error`,
             # rather than the function node,
             # as linenos differ in Python 3.7 and 3.8+ for decorated functions
             node.args.args[0],
@@ -2020,15 +2017,17 @@
 Y012 = 'Y012 Class body must not contain "pass"'
 Y013 = 'Y013 Non-empty class body must not contain "..."'
 Y014 = "Y014 Only simple default values allowed for arguments"
 Y015 = "Y015 Only simple default values are allowed for assignments"
 Y016 = 'Y016 Duplicate union member "{}"'
 Y017 = "Y017 Only simple assignments allowed"
 Y018 = 'Y018 {typevarlike_cls} "{typevar_name}" is not used'
-Y019 = 'Y019 Use "_typeshed.Self" instead of "{typevar_name}", e.g. "{new_syntax}"'
+Y019 = (
+    'Y019 Use "typing_extensions.Self" instead of "{typevar_name}", e.g. "{new_syntax}"'
+)
 Y020 = "Y020 Quoted annotations should never be used in stubs"
 Y021 = "Y021 Docstrings should not be included in stubs"
 Y022 = "Y022 Use {good_syntax} instead of {bad_syntax} (PEP 585 syntax)"
 Y023 = "Y023 Use {good_syntax} instead of {bad_syntax}"
 Y024 = 'Y024 Use "typing.NamedTuple" instead of "collections.namedtuple"'
 Y025 = (
     'Y025 Use "from collections.abc import Set as AbstractSet" '
@@ -2044,15 +2043,15 @@
 )
 Y033 = (
     "Y033 Do not use type comments in stubs "
     '(e.g. use "x: int" instead of "x = ... # type: int")'
 )
 Y034 = (
     'Y034 {methods} usually return "self" at runtime. '
-    'Consider using "_typeshed.Self" in "{method_name}", e.g. "{suggested_syntax}"'
+    'Consider using "typing_extensions.Self" in "{method_name}", e.g. "{suggested_syntax}"'
 )
 Y035 = (
     'Y035 "{var}" in a stub file must have a value, '
     'as it has the same semantics as "{var}" at runtime.'
 )
 Y036 = "Y036 Badly defined {method_name} method: {details}"
 Y037 = "Y037 Use PEP 604 union types instead of {old_syntax} (e.g. {example})."
```

### Comparing `flake8_pyi-23.3.1/.github/scripts/typeshed_primer_download_errors.js` & `flake8_pyi-23.4.0/.github/scripts/typeshed_primer_download_errors.js`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/.github/scripts/typeshed_primer_post_comment.js` & `flake8_pyi-23.4.0/.github/scripts/typeshed_primer_post_comment.js`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/.github/workflows/check.yml` & `flake8_pyi-23.4.0/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/.github/workflows/publish.yml` & `flake8_pyi-23.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/.github/workflows/typeshed_primer.yml` & `flake8_pyi-23.4.0/.github/workflows/typeshed_primer.yml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/.github/workflows/typeshed_primer_comment.yml` & `flake8_pyi-23.4.0/.github/workflows/typeshed_primer_comment.yml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/tests/aliases.pyi` & `flake8_pyi-23.4.0/tests/aliases.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/tests/attribute_annotations.pyi` & `flake8_pyi-23.4.0/tests/attribute_annotations.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/tests/calls.pyi` & `flake8_pyi-23.4.0/tests/calls.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/tests/classdefs.pyi` & `flake8_pyi-23.4.0/tests/classdefs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 from typing import Any, overload
 
 import typing_extensions
 from _typeshed import Self
 from typing_extensions import final
 
 class Bad(object):  # Y040 Do not inherit from "object" explicitly, as it is redundant in Python 3
-    def __new__(cls, *args: Any, **kwargs: Any) -> Bad: ...  # Y034 "__new__" methods usually return "self" at runtime. Consider using "_typeshed.Self" in "Bad.__new__", e.g. "def __new__(cls: type[Self], *args: Any, **kwargs: Any) -> Self: ..."
+    def __new__(cls, *args: Any, **kwargs: Any) -> Bad: ...  # Y034 "__new__" methods usually return "self" at runtime. Consider using "typing_extensions.Self" in "Bad.__new__", e.g. "def __new__(cls, *args: Any, **kwargs: Any) -> Self: ..."
     def __repr__(self) -> str: ...  # Y029 Defining __repr__ or __str__ in a stub is almost always redundant
     def __str__(self) -> builtins.str: ...  # Y029 Defining __repr__ or __str__ in a stub is almost always redundant
     def __eq__(self, other: Any) -> bool: ...  # Y032 Prefer "object" to "Any" for the second parameter in "__eq__" methods
     def __ne__(self, other: typing.Any) -> typing.Any: ...  # Y032 Prefer "object" to "Any" for the second parameter in "__ne__" methods
-    def __enter__(self) -> Bad: ...  # Y034 "__enter__" methods in classes like "Bad" usually return "self" at runtime. Consider using "_typeshed.Self" in "Bad.__enter__", e.g. "def __enter__(self: Self) -> Self: ..."
-    async def __aenter__(self) -> Bad: ...  # Y034 "__aenter__" methods in classes like "Bad" usually return "self" at runtime. Consider using "_typeshed.Self" in "Bad.__aenter__", e.g. "async def __aenter__(self: Self) -> Self: ..."
-    def __iadd__(self, other: Bad) -> Bad: ...  # Y034 "__iadd__" methods in classes like "Bad" usually return "self" at runtime. Consider using "_typeshed.Self" in "Bad.__iadd__", e.g. "def __iadd__(self: Self, other: Bad) -> Self: ..."
+    def __enter__(self) -> Bad: ...  # Y034 "__enter__" methods in classes like "Bad" usually return "self" at runtime. Consider using "typing_extensions.Self" in "Bad.__enter__", e.g. "def __enter__(self) -> Self: ..."
+    async def __aenter__(self) -> Bad: ...  # Y034 "__aenter__" methods in classes like "Bad" usually return "self" at runtime. Consider using "typing_extensions.Self" in "Bad.__aenter__", e.g. "async def __aenter__(self) -> Self: ..."
+    def __iadd__(self, other: Bad) -> Bad: ...  # Y034 "__iadd__" methods in classes like "Bad" usually return "self" at runtime. Consider using "typing_extensions.Self" in "Bad.__iadd__", e.g. "def __iadd__(self, other: Bad) -> Self: ..."
 
 class AlsoBad(int, builtins.object): ...  # Y040 Do not inherit from "object" explicitly, as it is redundant in Python 3
 
 class Good:
     def __new__(cls: type[Self], *args: Any, **kwargs: Any) -> Self: ...
     @abstractmethod
     def __str__(self) -> str: ...
@@ -75,31 +75,31 @@
 # we don't emit an error for these; out of scope for a linter
 class InvalidButPluginDoesNotCrash:
     def __new__() -> InvalidButPluginDoesNotCrash: ...
     def __enter__() -> InvalidButPluginDoesNotCrash: ...
     async def __aenter__() -> InvalidButPluginDoesNotCrash: ...
 
 class BadIterator1(Iterator[int]):
-    def __iter__(self) -> Iterator[int]: ...  # Y034 "__iter__" methods in classes like "BadIterator1" usually return "self" at runtime. Consider using "_typeshed.Self" in "BadIterator1.__iter__", e.g. "def __iter__(self: Self) -> Self: ..."
+    def __iter__(self) -> Iterator[int]: ...  # Y034 "__iter__" methods in classes like "BadIterator1" usually return "self" at runtime. Consider using "typing_extensions.Self" in "BadIterator1.__iter__", e.g. "def __iter__(self) -> Self: ..."
 
 class BadIterator2(typing.Iterator[int]):  # Y022 Use "collections.abc.Iterator[T]" instead of "typing.Iterator[T]" (PEP 585 syntax)
-    def __iter__(self) -> Iterator[int]: ...  # Y034 "__iter__" methods in classes like "BadIterator2" usually return "self" at runtime. Consider using "_typeshed.Self" in "BadIterator2.__iter__", e.g. "def __iter__(self: Self) -> Self: ..."
+    def __iter__(self) -> Iterator[int]: ...  # Y034 "__iter__" methods in classes like "BadIterator2" usually return "self" at runtime. Consider using "typing_extensions.Self" in "BadIterator2.__iter__", e.g. "def __iter__(self) -> Self: ..."
 
 class BadIterator3(typing.Iterator[int]):  # Y022 Use "collections.abc.Iterator[T]" instead of "typing.Iterator[T]" (PEP 585 syntax)
-    def __iter__(self) -> collections.abc.Iterator[int]: ...  # Y034 "__iter__" methods in classes like "BadIterator3" usually return "self" at runtime. Consider using "_typeshed.Self" in "BadIterator3.__iter__", e.g. "def __iter__(self: Self) -> Self: ..."
+    def __iter__(self) -> collections.abc.Iterator[int]: ...  # Y034 "__iter__" methods in classes like "BadIterator3" usually return "self" at runtime. Consider using "typing_extensions.Self" in "BadIterator3.__iter__", e.g. "def __iter__(self) -> Self: ..."
 
 class BadIterator4(Iterator[int]):
     # Note: *Iterable*, not *Iterator*, returned!
-    def __iter__(self) -> Iterable[int]: ...  # Y034 "__iter__" methods in classes like "BadIterator4" usually return "self" at runtime. Consider using "_typeshed.Self" in "BadIterator4.__iter__", e.g. "def __iter__(self: Self) -> Self: ..."
+    def __iter__(self) -> Iterable[int]: ...  # Y034 "__iter__" methods in classes like "BadIterator4" usually return "self" at runtime. Consider using "typing_extensions.Self" in "BadIterator4.__iter__", e.g. "def __iter__(self) -> Self: ..."
 
 class IteratorReturningIterable:
     def __iter__(self) -> Iterable[str]: ...  # Y045 "__iter__" methods should return an Iterator, not an Iterable
 
 class BadAsyncIterator(collections.abc.AsyncIterator[str]):
-    def __aiter__(self) -> typing.AsyncIterator[str]: ...  # Y034 "__aiter__" methods in classes like "BadAsyncIterator" usually return "self" at runtime. Consider using "_typeshed.Self" in "BadAsyncIterator.__aiter__", e.g. "def __aiter__(self: Self) -> Self: ..."  # Y022 Use "collections.abc.AsyncIterator[T]" instead of "typing.AsyncIterator[T]" (PEP 585 syntax)
+    def __aiter__(self) -> typing.AsyncIterator[str]: ...  # Y034 "__aiter__" methods in classes like "BadAsyncIterator" usually return "self" at runtime. Consider using "typing_extensions.Self" in "BadAsyncIterator.__aiter__", e.g. "def __aiter__(self) -> Self: ..."  # Y022 Use "collections.abc.AsyncIterator[T]" instead of "typing.AsyncIterator[T]" (PEP 585 syntax)
 
 class AsyncIteratorReturningAsyncIterable:
     def __aiter__(self) -> AsyncIterable[str]: ...  # Y045 "__aiter__" methods should return an AsyncIterator, not an AsyncIterable
 
 class Abstract(Iterator[str]):
     @abstractmethod
     def __iter__(self) -> Iterator[str]: ...
```

### Comparing `flake8_pyi-23.3.1/tests/defaults.pyi` & `flake8_pyi-23.4.0/tests/defaults.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/tests/emptyfunctions.pyi` & `flake8_pyi-23.4.0/tests/emptyfunctions.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/tests/exit_methods.pyi` & `flake8_pyi-23.4.0/tests/exit_methods.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/tests/imports.pyi` & `flake8_pyi-23.4.0/tests/imports.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/tests/names_requiring_values.pyi` & `flake8_pyi-23.4.0/tests/names_requiring_values.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/tests/never_vs_noreturn.pyi` & `flake8_pyi-23.4.0/tests/never_vs_noreturn.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/tests/pep604_union_types.pyi` & `flake8_pyi-23.4.0/tests/pep604_union_types.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/tests/quotes.pyi` & `flake8_pyi-23.4.0/tests/quotes.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/tests/sysversioninfo.pyi` & `flake8_pyi-23.4.0/tests/sysversioninfo.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/tests/test_pyi_files.py` & `flake8_pyi-23.4.0/tests/test_pyi_files.py`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/tests/type_comments.pyi` & `flake8_pyi-23.4.0/tests/type_comments.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/tests/typevar.pyi` & `flake8_pyi-23.4.0/tests/typevar.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 
 _UsedInAnnotatedSubscript = TypeVar("_UsedInAnnotatedSubscript", bound=list[int])
 def func3(arg: Annotated[_UsedInAnnotatedSubscript, "Important metadata"]) -> Annotated[_UsedInAnnotatedSubscript, "More important metadata"]: ...
 
 _S = TypeVar("_S")
 
 class BadClass:
-    def __new__(cls: type[_S], *args: str, **kwargs: int) -> _S: ...  # Y019 Use "_typeshed.Self" instead of "_S", e.g. "def __new__(cls: type[Self], *args: str, **kwargs: int) -> Self: ..."
-    def bad_instance_method(self: _S, arg: bytes) -> _S: ...  # Y019 Use "_typeshed.Self" instead of "_S", e.g. "def bad_instance_method(self: Self, arg: bytes) -> Self: ..."
+    def __new__(cls: type[_S], *args: str, **kwargs: int) -> _S: ...  # Y019 Use "typing_extensions.Self" instead of "_S", e.g. "def __new__(cls, *args: str, **kwargs: int) -> Self: ..."
+    def bad_instance_method(self: _S, arg: bytes) -> _S: ...  # Y019 Use "typing_extensions.Self" instead of "_S", e.g. "def bad_instance_method(self, arg: bytes) -> Self: ..."
     @classmethod
-    def bad_class_method(cls: type[_S], arg: int) -> _S: ...  # Y019 Use "_typeshed.Self" instead of "_S", e.g. "def bad_class_method(cls: type[Self], arg: int) -> Self: ..."
+    def bad_class_method(cls: type[_S], arg: int) -> _S: ...  # Y019 Use "typing_extensions.Self" instead of "_S", e.g. "def bad_class_method(cls, arg: int) -> Self: ..."
 
 class GoodClass:
     def __new__(cls: type[Self], *args: list[int], **kwargs: set[str]) -> Self: ...
     def good_instance_method_1(self: Self, arg: bytes) -> Self: ...
     def good_instance_method_2(self, arg1: _S, arg2: _S) -> _S: ...
     @classmethod
     def good_cls_method_1(cls: type[Self], arg: int) -> Self: ...
```

### Comparing `flake8_pyi-23.3.1/tests/union_duplicates.pyi` & `flake8_pyi-23.4.0/tests/union_duplicates.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/tests/unused_things.pyi` & `flake8_pyi-23.4.0/tests/unused_things.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/.gitignore` & `flake8_pyi-23.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/LICENSE` & `flake8_pyi-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.3.1/README.md` & `flake8_pyi-23.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,29 +48,29 @@
 | Y012 | Class body must not contain `pass`.
 | Y013 | Non-empty class body must not contain `...`.
 | Y014 | Only simple default values are allowed for any function arguments. A stronger version of Y011 that includes arguments without type annotations.
 | Y015 | Only simple default values are allowed for assignments. Similar to Y011, but for assignments rather than parameter annotations.
 | Y016 | Unions shouldn't contain duplicates, e.g. `str \| str` is not allowed.
 | Y017 | Stubs should not contain assignments with multiple targets or non-name targets. E.g. `T, S = TypeVar("T"), TypeVar("S")` is disallowed, as is `foo.bar = TypeVar("T")`.
 | Y018 | A private `TypeVar` should be used at least once in the file in which it is defined.
-| Y019 | Certain kinds of methods should use `_typeshed.Self` instead of defining custom `TypeVar`s for their return annotation. This check currently applies for instance methods that return `self`, class methods that return an instance of `cls`, and `__new__` methods.
+| Y019 | Certain kinds of methods should use `typing_extensions.Self` instead of defining custom `TypeVar`s for their return annotation. This check currently applies for instance methods that return `self`, class methods that return an instance of `cls`, and `__new__` methods.
 | Y020 | Quoted annotations should never be used in stubs.
 | Y021 | Docstrings should not be included in stubs.
 | Y022 | The `typing` and `typing_extensions` modules include various aliases to stdlib objects. Use these as little as possible (e.g. prefer `builtins.list` over `typing.List`, `collections.Counter` over `typing.Counter`, etc.).
 | Y023 | Where there is no detriment to backwards compatibility, import objects such as `ClassVar` and `NoReturn` from `typing` rather than `typing_extensions`.
 | Y024 | Use `typing.NamedTuple` instead of `collections.namedtuple`, as it allows for more precise type inference.
 | Y025 | Always alias `collections.abc.Set` when importing it, so as to avoid confusion with `builtins.set`. E.g. use `from collections.abc import Set as AbstractSet` instead of `from collections.abc import Set`.
 | Y026 | Type aliases should be explicitly demarcated with `typing.TypeAlias`.
 | Y028 | Always use class-based syntax for `typing.NamedTuple`, instead of assignment-based syntax.
 | Y029 | It is almost always redundant to define `__str__` or `__repr__` in a stub file, as the signatures are almost always identical to `object.__str__` and `object.__repr__`.
 | Y030 | Union expressions should never have more than one `Literal` member, as `Literal[1] \| Literal[2]` is semantically identical to `Literal[1, 2]`.
 | Y031 | `TypedDict`s should use class-based syntax instead of assignment-based syntax wherever possible. (In situations where this is not possible, such as if a field is a Python keyword or an invalid identifier, this error will not be emitted.)
 | Y032 | The second argument of an `__eq__` or `__ne__` method should usually be annotated with `object` rather than `Any`.
 | Y033 | Do not use type comments (e.g. `x = ... # type: int`) in stubs. Always use annotations instead (e.g. `x: int`).
-| Y034 | Y034 detects common errors where certain methods are annotated as having a fixed return type, despite returning `self` at runtime. Such methods should be annotated with `_typeshed.Self`. This check looks for:<br><br>&nbsp;&nbsp;**1.**&nbsp;&nbsp;Any in-place BinOp dunder methods (`__iadd__`, `__ior__`, etc.) that do not return `Self`.<br>&nbsp;&nbsp;**2.**&nbsp;&nbsp;`__new__`, `__enter__` and `__aenter__` methods that return the class's name unparameterised.<br>&nbsp;&nbsp;**3.**&nbsp;&nbsp;`__iter__` methods that return `Iterator`, even if the class inherits directly from `Iterator`.<br>&nbsp;&nbsp;**4.**&nbsp;&nbsp;`__aiter__` methods that return `AsyncIterator`, even if the class inherits directly from `AsyncIterator`.<br><br>This check excludes methods decorated with `@overload` or `@abstractmethod`.
+| Y034 | Y034 detects common errors where certain methods are annotated as having a fixed return type, despite returning `self` at runtime. Such methods should be annotated with `typing_extensions.Self`. This check looks for:<br><br>&nbsp;&nbsp;**1.**&nbsp;&nbsp;Any in-place BinOp dunder methods (`__iadd__`, `__ior__`, etc.) that do not return `Self`.<br>&nbsp;&nbsp;**2.**&nbsp;&nbsp;`__new__`, `__enter__` and `__aenter__` methods that return the class's name unparameterised.<br>&nbsp;&nbsp;**3.**&nbsp;&nbsp;`__iter__` methods that return `Iterator`, even if the class inherits directly from `Iterator`.<br>&nbsp;&nbsp;**4.**&nbsp;&nbsp;`__aiter__` methods that return `AsyncIterator`, even if the class inherits directly from `AsyncIterator`.<br><br>This check excludes methods decorated with `@overload` or `@abstractmethod`.
 | Y035 | `__all__`, `__match_args__` and `__slots__` in a stub file should always have values, as these special variables in a `.pyi` file have identical semantics in a stub as at runtime. E.g. write `__all__ = ["foo", "bar"]` instead of `__all__: list[str]`.
 | Y036 | Y036 detects common errors in `__exit__` and `__aexit__` methods. For example, the first argument in an `__exit__` method should either be annotated with `object`, `_typeshed.Unused` (a special alias for `object`) or `type[BaseException] \| None`.
 | Y037 | Use PEP 604 syntax instead of `typing.Union` and `typing.Optional`. E.g. use `str \| int` instead of `Union[str, int]`, and use `str \| None` instead of `Optional[str]`.
 | Y038 | Use `from collections.abc import Set as AbstractSet` instead of `from typing import AbstractSet`.
 | Y039 | Use `str` instead of `typing.Text`.
 | Y040 | Never explicitly inherit from `object`, as all classes implicitly inherit from `object` in Python 3.
 | Y041 | Y041 detects redundant numeric unions in the context of parameter annotations. For example, PEP 484 specifies that type checkers should allow `int` objects to be passed to a function, even if the function states that it accepts a `float`. As such, `int` is redundant in the union `int \| float` in the context of a parameter annotation. In the same way, `int` is sometimes redundant in the union `int \| complex`, and `float` is sometimes redundant in the union `float \| complex`.
```

### Comparing `flake8_pyi-23.3.1/pyproject.toml` & `flake8_pyi-23.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 "Homepage" = "https://github.com/PyCQA/flake8-pyi"
 "Source" = "https://github.com/PyCQA/flake8-pyi"
 "Bug Tracker" = "https://github.com/PyCQA/flake8-pyi/issues"
 "Changelog" = "https://github.com/PyCQA/flake8-pyi/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
 dev = [
-    "black==23.1.0",                          # Must match .pre-commit-config.yaml
+    "black==23.3.0",                          # Must match .pre-commit-config.yaml
     "flake8-bugbear==23.2.13",
     "flake8-noqa==1.3.0",
     "isort==5.12.0; python_version >= '3.8'", # Must match .pre-commit-config.yaml
     "mypy==1.1.1",
     "pre-commit-hooks==4.4.0",                # Must match .pre-commit-config.yaml
     "pytest==7.2.2",
     "types-pyflakes<4",
```

### Comparing `flake8_pyi-23.3.1/PKG-INFO` & `flake8_pyi-23.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-pyi
-Version: 23.3.1
+Version: 23.4.0
 Summary: A plugin for flake8 to enable linting .pyi stub files.
 Project-URL: Homepage, https://github.com/PyCQA/flake8-pyi
 Project-URL: Source, https://github.com/PyCQA/flake8-pyi
 Project-URL: Bug Tracker, https://github.com/PyCQA/flake8-pyi/issues
 Project-URL: Changelog, https://github.com/PyCQA/flake8-pyi/blob/main/CHANGELOG.md
 Author-email: Łukasz Langa <=lukasz@langa.pl>
 Maintainer: Sebastian Rittau, Akuli, Shantanu
@@ -28,15 +28,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.7
 Requires-Dist: ast-decompiler<1.0,>=0.7.0; python_version < '3.9'
 Requires-Dist: flake8<7.0.0,>=3.2.1
 Requires-Dist: pyflakes>=2.1.1
 Provides-Extra: dev
-Requires-Dist: black==23.1.0; extra == 'dev'
+Requires-Dist: black==23.3.0; extra == 'dev'
 Requires-Dist: flake8-bugbear==23.2.13; extra == 'dev'
 Requires-Dist: flake8-noqa==1.3.0; extra == 'dev'
 Requires-Dist: isort==5.12.0; python_version >= '3.8' and extra == 'dev'
 Requires-Dist: mypy==1.1.1; extra == 'dev'
 Requires-Dist: pre-commit-hooks==4.4.0; extra == 'dev'
 Requires-Dist: pytest==7.2.2; extra == 'dev'
 Requires-Dist: types-pyflakes<4; extra == 'dev'
@@ -92,29 +92,29 @@
 | Y012 | Class body must not contain `pass`.
 | Y013 | Non-empty class body must not contain `...`.
 | Y014 | Only simple default values are allowed for any function arguments. A stronger version of Y011 that includes arguments without type annotations.
 | Y015 | Only simple default values are allowed for assignments. Similar to Y011, but for assignments rather than parameter annotations.
 | Y016 | Unions shouldn't contain duplicates, e.g. `str \| str` is not allowed.
 | Y017 | Stubs should not contain assignments with multiple targets or non-name targets. E.g. `T, S = TypeVar("T"), TypeVar("S")` is disallowed, as is `foo.bar = TypeVar("T")`.
 | Y018 | A private `TypeVar` should be used at least once in the file in which it is defined.
-| Y019 | Certain kinds of methods should use `_typeshed.Self` instead of defining custom `TypeVar`s for their return annotation. This check currently applies for instance methods that return `self`, class methods that return an instance of `cls`, and `__new__` methods.
+| Y019 | Certain kinds of methods should use `typing_extensions.Self` instead of defining custom `TypeVar`s for their return annotation. This check currently applies for instance methods that return `self`, class methods that return an instance of `cls`, and `__new__` methods.
 | Y020 | Quoted annotations should never be used in stubs.
 | Y021 | Docstrings should not be included in stubs.
 | Y022 | The `typing` and `typing_extensions` modules include various aliases to stdlib objects. Use these as little as possible (e.g. prefer `builtins.list` over `typing.List`, `collections.Counter` over `typing.Counter`, etc.).
 | Y023 | Where there is no detriment to backwards compatibility, import objects such as `ClassVar` and `NoReturn` from `typing` rather than `typing_extensions`.
 | Y024 | Use `typing.NamedTuple` instead of `collections.namedtuple`, as it allows for more precise type inference.
 | Y025 | Always alias `collections.abc.Set` when importing it, so as to avoid confusion with `builtins.set`. E.g. use `from collections.abc import Set as AbstractSet` instead of `from collections.abc import Set`.
 | Y026 | Type aliases should be explicitly demarcated with `typing.TypeAlias`.
 | Y028 | Always use class-based syntax for `typing.NamedTuple`, instead of assignment-based syntax.
 | Y029 | It is almost always redundant to define `__str__` or `__repr__` in a stub file, as the signatures are almost always identical to `object.__str__` and `object.__repr__`.
 | Y030 | Union expressions should never have more than one `Literal` member, as `Literal[1] \| Literal[2]` is semantically identical to `Literal[1, 2]`.
 | Y031 | `TypedDict`s should use class-based syntax instead of assignment-based syntax wherever possible. (In situations where this is not possible, such as if a field is a Python keyword or an invalid identifier, this error will not be emitted.)
 | Y032 | The second argument of an `__eq__` or `__ne__` method should usually be annotated with `object` rather than `Any`.
 | Y033 | Do not use type comments (e.g. `x = ... # type: int`) in stubs. Always use annotations instead (e.g. `x: int`).
-| Y034 | Y034 detects common errors where certain methods are annotated as having a fixed return type, despite returning `self` at runtime. Such methods should be annotated with `_typeshed.Self`. This check looks for:<br><br>&nbsp;&nbsp;**1.**&nbsp;&nbsp;Any in-place BinOp dunder methods (`__iadd__`, `__ior__`, etc.) that do not return `Self`.<br>&nbsp;&nbsp;**2.**&nbsp;&nbsp;`__new__`, `__enter__` and `__aenter__` methods that return the class's name unparameterised.<br>&nbsp;&nbsp;**3.**&nbsp;&nbsp;`__iter__` methods that return `Iterator`, even if the class inherits directly from `Iterator`.<br>&nbsp;&nbsp;**4.**&nbsp;&nbsp;`__aiter__` methods that return `AsyncIterator`, even if the class inherits directly from `AsyncIterator`.<br><br>This check excludes methods decorated with `@overload` or `@abstractmethod`.
+| Y034 | Y034 detects common errors where certain methods are annotated as having a fixed return type, despite returning `self` at runtime. Such methods should be annotated with `typing_extensions.Self`. This check looks for:<br><br>&nbsp;&nbsp;**1.**&nbsp;&nbsp;Any in-place BinOp dunder methods (`__iadd__`, `__ior__`, etc.) that do not return `Self`.<br>&nbsp;&nbsp;**2.**&nbsp;&nbsp;`__new__`, `__enter__` and `__aenter__` methods that return the class's name unparameterised.<br>&nbsp;&nbsp;**3.**&nbsp;&nbsp;`__iter__` methods that return `Iterator`, even if the class inherits directly from `Iterator`.<br>&nbsp;&nbsp;**4.**&nbsp;&nbsp;`__aiter__` methods that return `AsyncIterator`, even if the class inherits directly from `AsyncIterator`.<br><br>This check excludes methods decorated with `@overload` or `@abstractmethod`.
 | Y035 | `__all__`, `__match_args__` and `__slots__` in a stub file should always have values, as these special variables in a `.pyi` file have identical semantics in a stub as at runtime. E.g. write `__all__ = ["foo", "bar"]` instead of `__all__: list[str]`.
 | Y036 | Y036 detects common errors in `__exit__` and `__aexit__` methods. For example, the first argument in an `__exit__` method should either be annotated with `object`, `_typeshed.Unused` (a special alias for `object`) or `type[BaseException] \| None`.
 | Y037 | Use PEP 604 syntax instead of `typing.Union` and `typing.Optional`. E.g. use `str \| int` instead of `Union[str, int]`, and use `str \| None` instead of `Optional[str]`.
 | Y038 | Use `from collections.abc import Set as AbstractSet` instead of `from typing import AbstractSet`.
 | Y039 | Use `str` instead of `typing.Text`.
 | Y040 | Never explicitly inherit from `object`, as all classes implicitly inherit from `object` in Python 3.
 | Y041 | Y041 detects redundant numeric unions in the context of parameter annotations. For example, PEP 484 specifies that type checkers should allow `int` objects to be passed to a function, even if the function states that it accepts a `float`. As such, `int` is redundant in the union `int \| float` in the context of a parameter annotation. In the same way, `int` is sometimes redundant in the union `int \| complex`, and `float` is sometimes redundant in the union `float \| complex`.
```


# Comparing `tmp/use_case_registry-1.4.5.tar.gz` & `tmp/use_case_registry-1.4.6.tar.gz`

## Comparing `use_case_registry-1.4.5.tar` & `use_case_registry-1.4.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.tool-versions
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/Makefile
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/mkdocs.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.github/CODEOWNERS
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.github/workflows/audit.yml
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.github/workflows/release.yml
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.github/workflows/test.yml
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.github/workflows/update_docs.yml
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.vscode/settings.json
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/docs/index.md
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/docs/general-thoughts/clean-architecture/index.md
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/docs/general-thoughts/error-handling/index.md
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/docs/general-thoughts/one-use-case-one-workflow/index.md
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/requirements/core.txt
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/requirements/dev.txt
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/requirements/sqlalchemy.txt
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/scripts/release_github.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/__init__.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/test_enums.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/test_registry.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/assets/templates/target-based/config-1.yml
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/assets/templates/target-based/config-2.yml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/assets/templates/target-based/config-3.yml
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/assets/templates/target-based/config-4.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/base/__init__.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/base/test_command.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/base/test_repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/parsers/__init__.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/parsers/test_target_based.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/__about__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/__init__.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/enums.py
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/py.typed
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/registry.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/base/__init__.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/base/command.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/base/repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/internals/__init__.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/internals/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/pasers/__init__.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/pasers/macros.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/pasers/target_based.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/LICENSE.txt
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/README.md
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/pyproject.toml
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/.tool-versions
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/Makefile
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/mkdocs.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/.github/CODEOWNERS
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/.github/workflows/audit.yml
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/.github/workflows/test.yml
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/.github/workflows/update_docs.yml
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/.vscode/settings.json
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/docs/index.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/docs/general-thoughts/clean-architecture/index.md
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/docs/general-thoughts/error-handling/index.md
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/docs/general-thoughts/one-use-case-one-workflow/index.md
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/requirements/core.txt
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/requirements/dev.txt
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/requirements/sqlalchemy.txt
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/scripts/release_github.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/tests/__init__.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/tests/test_enums.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/tests/test_registry.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/tests/assets/templates/target-based/config-1.yml
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/tests/assets/templates/target-based/config-2.yml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/tests/assets/templates/target-based/config-3.yml
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/tests/assets/templates/target-based/config-4.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/tests/base/__init__.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/tests/base/test_command.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/tests/base/test_repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/tests/parsers/__init__.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/tests/parsers/test_target_based.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/use_case_registry/__about__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/use_case_registry/__init__.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/use_case_registry/enums.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/use_case_registry/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/use_case_registry/py.typed
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/use_case_registry/registry.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/use_case_registry/base/__init__.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/use_case_registry/base/command.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/use_case_registry/base/repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/use_case_registry/internals/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/use_case_registry/internals/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/use_case_registry/pasers/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/use_case_registry/pasers/macros.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/use_case_registry/pasers/target_based.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/LICENSE.txt
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/README.md
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/pyproject.toml
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 use_case_registry-1.4.6/PKG-INFO
```

### Comparing `use_case_registry-1.4.5/Makefile` & `use_case_registry-1.4.6/Makefile`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/mkdocs.yml` & `use_case_registry-1.4.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/.github/ISSUE_TEMPLATE/bug_report.md` & `use_case_registry-1.4.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/.github/ISSUE_TEMPLATE/feature_request.md` & `use_case_registry-1.4.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/.github/workflows/audit.yml` & `use_case_registry-1.4.6/.github/workflows/audit.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/.github/workflows/coverage.yml` & `use_case_registry-1.4.6/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/.github/workflows/release.yml` & `use_case_registry-1.4.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/.github/workflows/test.yml` & `use_case_registry-1.4.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/.vscode/settings.json` & `use_case_registry-1.4.6/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/docs/index.md` & `use_case_registry-1.4.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/docs/general-thoughts/clean-architecture/index.md` & `use_case_registry-1.4.6/docs/general-thoughts/clean-architecture/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/docs/general-thoughts/error-handling/index.md` & `use_case_registry-1.4.6/docs/general-thoughts/error-handling/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/docs/general-thoughts/one-use-case-one-workflow/index.md` & `use_case_registry-1.4.6/docs/general-thoughts/one-use-case-one-workflow/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/requirements/core.txt` & `use_case_registry-1.4.6/requirements/core.txt`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/requirements/dev.txt` & `use_case_registry-1.4.6/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/requirements/sqlalchemy.txt` & `use_case_registry-1.4.6/requirements/sqlalchemy.txt`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/scripts/release_github.py` & `use_case_registry-1.4.6/scripts/release_github.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/tests/test_registry.py` & `use_case_registry-1.4.6/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/tests/base/test_command.py` & `use_case_registry-1.4.6/tests/base/test_command.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass
 from typing import Any
 
 import pytest
 from result import Ok, Result
 
 from use_case_registry import UseCaseRegistry
-from use_case_registry.base.command import BaseCommand, ICommandInput
+from use_case_registry.base.command import BaseCommand, ICommandInput, validate_inputs
 from use_case_registry.errors import CommandInputValidationError, UseCaseExecutionError
 
 
 @dataclass(
     frozen=True,
     repr=False,
     eq=False,
@@ -46,15 +46,15 @@
 
         return Ok()
 
 
 def test_validate_command_pass() -> None:
     """Test validate command passes."""
     inputs = ExampleCommandInput(name="tomas", last_name="perez", age=10)
-    ExampleCommand(inputs=inputs).validate().unwrap()
+    validate_inputs(inputs=inputs).unwrap()
 
 
 @pytest.mark.parametrize(
     argnames="inputs",
     argvalues=[
         ExampleCommandInput(
             name="tomas",
@@ -66,10 +66,10 @@
             last_name="perez",
             age=10,
         ),
     ],
 )
 def test_validate_command_fails(inputs: ICommandInput) -> None:
     """Test validate command fails."""
-    validation_err = ExampleCommand(inputs=inputs).validate().err()
+    validation_err = validate_inputs(inputs=inputs).err()
 
     assert isinstance(validation_err, CommandInputValidationError)
```

### Comparing `use_case_registry-1.4.5/tests/base/test_repository.py` & `use_case_registry-1.4.6/tests/base/test_repository.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/tests/parsers/test_target_based.py` & `use_case_registry-1.4.6/tests/parsers/test_target_based.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/use_case_registry/enums.py` & `use_case_registry-1.4.6/use_case_registry/enums.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/use_case_registry/errors.py` & `use_case_registry-1.4.6/use_case_registry/errors.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/use_case_registry/registry.py` & `use_case_registry-1.4.6/use_case_registry/registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/use_case_registry/base/command.py` & `use_case_registry-1.4.6/use_case_registry/base/command.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,39 +16,34 @@
 @dataclass(
     frozen=True,
 )
 class ICommandInput(DataClassORJSONMixin):
     """ICommandInput."""
 
 
-class BaseCommand(abc.ABC):
-    """Command abstract class."""
+def validate_inputs(inputs: ICommandInput) -> Result[None, CommandInputValidationError]:
+    """Validate inputs."""
+    input_schema = (
+        JSONSchemaBuilder(dialect=DRAFT_2020_12, all_refs=False)
+        .build(
+            instance_type=inputs.__class__,
+        )
+        .to_dict()
+    )
+    try:
+        jsonschema.validate(instance=inputs.to_dict(), schema=input_schema)
+    except ValidationError as e:
+        return Err(CommandInputValidationError(msg=e.message))
+    except ValueError as e:
+        return Err(CommandInputValidationError(msg=e.args[0]))
+    return Ok()
 
-    def __init__(self, inputs: ICommandInput) -> None:
-        """Class constructor.."""
-        self.inputs = inputs
 
-    def validate(
-        self,
-    ) -> Result[None, CommandInputValidationError]:
-        """Validate command input values."""
-        input_schema = (
-            JSONSchemaBuilder(dialect=DRAFT_2020_12, all_refs=False)
-            .build(
-                instance_type=self.inputs.__class__,
-            )
-            .to_dict()
-        )
-        try:
-            jsonschema.validate(instance=self.inputs.to_dict(), schema=input_schema)
-        except ValidationError as e:
-            return Err(CommandInputValidationError(msg=e.message))
-        except ValueError as e:
-            return Err(CommandInputValidationError(msg=e.args[0]))
-        return Ok()
+class BaseCommand(abc.ABC):
+    """Command abstract class."""
 
     @abc.abstractmethod
     def execute(
         self,
         write_ops_registry: UseCaseRegistry[Any],
     ) -> Result[Any, UseCaseExecutionError]:
         """Workflow execution command to complete the use case."""
```

### Comparing `use_case_registry-1.4.5/use_case_registry/base/repository.py` & `use_case_registry-1.4.6/use_case_registry/base/repository.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/use_case_registry/internals/errors.py` & `use_case_registry-1.4.6/use_case_registry/internals/errors.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/use_case_registry/pasers/macros.py` & `use_case_registry-1.4.6/use_case_registry/pasers/macros.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/use_case_registry/pasers/target_based.py` & `use_case_registry-1.4.6/use_case_registry/pasers/target_based.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/.gitignore` & `use_case_registry-1.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/LICENSE.txt` & `use_case_registry-1.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/README.md` & `use_case_registry-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.5/pyproject.toml` & `use_case_registry-1.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 files = [
   "use_case_registry",
   "tests"
 ]
 
 # temporarily ignore some files
 show_error_codes = true
-follow_imports = 'silent'
+follow_imports = 'normal'
 strict_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 disallow_any_generics = true
 check_untyped_defs = true
 no_implicit_reexport = true
 warn_unused_configs = true
```

### Comparing `use_case_registry-1.4.5/PKG-INFO` & `use_case_registry-1.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: use_case_registry
-Version: 1.4.5
+Version: 1.4.6
 Summary: Registry class for Use Case implementation. They are basically meaningfull lists with some constraints.
 Project-URL: Homepage, https://github.com/Tomperez98/use-case-registry
 Project-URL: Documentation, https://tomperez98.github.io/use-case-registry/
 Project-URL: Issues, https://github.com/Tomperez98/use-case-registry/issues
 Project-URL: Source, https://github.com/Tomperez98/use-case-registry
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-Expression: MIT
```


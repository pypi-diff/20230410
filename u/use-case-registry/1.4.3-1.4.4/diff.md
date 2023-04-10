# Comparing `tmp/use_case_registry-1.4.3.tar.gz` & `tmp/use_case_registry-1.4.4.tar.gz`

## Comparing `use_case_registry-1.4.3.tar` & `use_case_registry-1.4.4.tar`

### file list

```diff
@@ -1,46 +1,58 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.tool-versions
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/Makefile
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/mkdocs.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.github/CODEOWNERS
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.github/workflows/audit.yml
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.github/workflows/release.yml
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.github/workflows/update_docs.yml
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.vscode/settings.json
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/docs/index.md
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/docs/general-thoughts/clean-architecture/index.md
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/docs/general-thoughts/error-handling/index.md
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/docs/general-thoughts/one-use-case-one-workflow/index.md
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/requirements/core.txt
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/requirements/dev.txt
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/requirements/sqlalchemy.txt
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/scripts/release_github.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/tests/__init__.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/tests/test_registry.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/tests/test_template_parser.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/tests/assets/templates/config-1.yml
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/tests/assets/templates/config-2.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/tests/assets/templates/config-3.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/tests/base/__init__.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/tests/base/test_command.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/tests/base/test_repository.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/__about__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/__init__.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/enums.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/py.typed
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/registry.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/template_parsers.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/base/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/base/command.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/base/repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/internals/__init__.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/internals/errors.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/LICENSE.txt
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/README.md
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.tool-versions
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/Makefile
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/mkdocs.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.github/CODEOWNERS
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.github/workflows/audit.yml
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.github/workflows/update_docs.yml
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.vscode/settings.json
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/docs/index.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/docs/general-thoughts/clean-architecture/index.md
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/docs/general-thoughts/error-handling/index.md
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/docs/general-thoughts/one-use-case-one-workflow/index.md
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/requirements/core.txt
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/requirements/dev.txt
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/requirements/sqlalchemy.txt
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/scripts/release_github.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/__init__.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/test_registry.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/assets/templates/raw/config-1.yml
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/assets/templates/raw/config-2.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/assets/templates/raw/config-3.yml
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/assets/templates/repository/config-1.yml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/assets/templates/repository/config-2.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/assets/templates/repository/config-no-connection.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/assets/templates/repository/config-no-drivername.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/assets/templates/repository/config-no-url.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/base/__init__.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/base/test_command.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/base/test_repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/parsers/__init__.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/parsers/test_base.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/parsers/test_raw.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/parsers/test_repository.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/__about__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/__init__.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/enums.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/py.typed
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/registry.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/base/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/base/command.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/base/repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/internals/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/internals/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/pasers/__init__.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/pasers/base.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/pasers/macros.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/pasers/raw.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/pasers/repository.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/LICENSE.txt
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/README.md
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/PKG-INFO
```

### Comparing `use_case_registry-1.4.3/Makefile` & `use_case_registry-1.4.4/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -27,20 +27,20 @@
 .PHONY: sync-to-env
 sync-to-env: ## sync dev virtualenv
 	@pip-sync requirements/$(env).txt
 	@pip install -e .
 
 .PHONY: lint
 lint: ## Lint code.
-	mypy $(sources)
-	ruff $(sources)
+	python -m mypy $(sources)
+	python -m ruff $(sources)
 
 .PHONY: unit
 unit: ## Run code unittest
-	pytest .
+	python -m pytest .
 
 .PHONY: test
 test:
 	make lint
 	make unit
 
 .PHONY: clean
```

### Comparing `use_case_registry-1.4.3/mkdocs.yml` & `use_case_registry-1.4.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/.github/ISSUE_TEMPLATE/bug_report.md` & `use_case_registry-1.4.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/.github/ISSUE_TEMPLATE/feature_request.md` & `use_case_registry-1.4.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/.github/workflows/audit.yml` & `use_case_registry-1.4.4/.github/workflows/audit.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/.github/workflows/coverage.yml` & `use_case_registry-1.4.4/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/.github/workflows/release.yml` & `use_case_registry-1.4.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/.github/workflows/test.yml` & `use_case_registry-1.4.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/.vscode/settings.json` & `use_case_registry-1.4.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/docs/index.md` & `use_case_registry-1.4.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/docs/general-thoughts/clean-architecture/index.md` & `use_case_registry-1.4.4/docs/general-thoughts/clean-architecture/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/docs/general-thoughts/error-handling/index.md` & `use_case_registry-1.4.4/docs/general-thoughts/error-handling/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/docs/general-thoughts/one-use-case-one-workflow/index.md` & `use_case_registry-1.4.4/docs/general-thoughts/one-use-case-one-workflow/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/requirements/dev.txt` & `use_case_registry-1.4.4/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/requirements/sqlalchemy.txt` & `use_case_registry-1.4.4/requirements/sqlalchemy.txt`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 #
 #    pip-compile --extra=sqlalchemy --no-emit-trusted-host --output-file=requirements/sqlalchemy.txt --resolver=backtracking pyproject.toml
 #
 jinja2==3.1.2
     # via use_case_registry (pyproject.toml)
 markupsafe==2.1.2
     # via jinja2
+pyyaml==6.0
+    # via use_case_registry (pyproject.toml)
 result==0.9.0
     # via use_case_registry (pyproject.toml)
 sqlalchemy==2.0.9
     # via use_case_registry (pyproject.toml)
 typing-extensions==4.5.0
     # via
     #   result
```

### Comparing `use_case_registry-1.4.3/scripts/release_github.py` & `use_case_registry-1.4.4/scripts/release_github.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/tests/test_registry.py` & `use_case_registry-1.4.4/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/tests/test_template_parser.py` & `use_case_registry-1.4.4/tests/parsers/test_repository.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,90 @@
-"""Test template parser."""
+"""Test repository parser."""
 import os
 import pathlib
 from typing import Any
 from unittest import mock
 
 import pytest
-import yaml
 
-from use_case_registry.errors import EnvVarMissingError
-from use_case_registry.template_parsers import TemplateParser
+from use_case_registry.pasers.repository import RepoConfigParser
 
 
-class TestTemplateParser:
-    """Test template parser."""
-
-    @pytest.mark.parametrize(
-        argnames="template_folder",
-        argvalues=[
-            pathlib.Path()
-            .cwd()
-            .joinpath(
-                "tests/assets/not-existing",
-            ),
-        ],
-    )
-    def test_constructor_fails(self, template_folder: pathlib.Path) -> None:
-        """Test constructor fails."""
-        with pytest.raises(RuntimeError):
-            TemplateParser(path_to_folder=template_folder)
+class TestRepoConfigParser:
+    """Test repo config parser."""
 
     @mock.patch.dict(
         os.environ,
         {
-            "NAME": "name",
+            "EXECUTION_ENV": "dev",
+            "DB_PASSWORD": "abc",
         },
         clear=True,
     )
     @pytest.mark.parametrize(
         argnames=[
             "template_name",
             "expected_result",
         ],
         argvalues=[
             (
-                "config-2.yml",
+                "config-1.yml",
                 {
-                    "version": 1,
-                    "name": "tomas",
-                    "last_name": "perez",
+                    "url": "sqlite:///dev-database.db",
                 },
             ),
             (
-                "config-3.yml",
+                "config-2.yml",
                 {
-                    "version": 1,
-                    "name": "name",
-                    "last_name": "perez",
+                    "url": "sqlite:///dev-database.db",
                 },
             ),
         ],
     )
     def test_parse_works(
         self,
         template_name: str,
         expected_result: dict[str, Any],
     ) -> None:
         """Test parse() works as expected."""
-        template_folder = pathlib.Path().cwd().joinpath("tests/assets/templates")
-        parser = TemplateParser(path_to_folder=template_folder)
-        result = parser.parse(template_name)
-        assert yaml.safe_load(result) == expected_result
+        template_folder = (
+            pathlib.Path()
+            .cwd()
+            .joinpath(
+                "tests/assets/templates/repository",
+            )
+        )
+        parser = RepoConfigParser(path_to_folder=template_folder)
+        result = parser.parse(template=template_name)
+        assert result == expected_result
 
+    @mock.patch.dict(
+        os.environ,
+        {
+            "EXECUTION_ENV": "dev",
+            "DB_PASSWORD": "abc",
+        },
+        clear=True,
+    )
     @pytest.mark.parametrize(
         argnames="template_name",
         argvalues=[
-            "config-1.yml",
+            "config-no-url.yml",
+            "config-no-drivername.yml",
+            "config-no-connection.yml",
         ],
     )
-    def test_parse_fails_env_variable_not_set(
+    def test_parse_fails(
         self,
         template_name: str,
     ) -> None:
-        """Test parse() fails when env variable is not setted."""
-        template_folder = pathlib.Path().cwd().joinpath("tests/assets/templates")
-        parser = TemplateParser(path_to_folder=template_folder)
-        with pytest.raises(EnvVarMissingError):
-            parser.parse(template_name)
+        """Test parse() works as expected."""
+        template_folder = (
+            pathlib.Path()
+            .cwd()
+            .joinpath(
+                "tests/assets/templates/repository",
+            )
+        )
+        parser = RepoConfigParser(path_to_folder=template_folder)
+        with pytest.raises(RuntimeError):
+            parser.parse(template=template_name)
```

### Comparing `use_case_registry-1.4.3/tests/base/test_command.py` & `use_case_registry-1.4.4/tests/base/test_command.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/tests/base/test_repository.py` & `use_case_registry-1.4.4/tests/base/test_repository.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/use_case_registry/errors.py` & `use_case_registry-1.4.4/use_case_registry/errors.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/use_case_registry/registry.py` & `use_case_registry-1.4.4/use_case_registry/registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/use_case_registry/base/command.py` & `use_case_registry-1.4.4/use_case_registry/base/command.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/use_case_registry/base/repository.py` & `use_case_registry-1.4.4/use_case_registry/base/repository.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/use_case_registry/internals/errors.py` & `use_case_registry-1.4.4/use_case_registry/internals/errors.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/.gitignore` & `use_case_registry-1.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/LICENSE.txt` & `use_case_registry-1.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/README.md` & `use_case_registry-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.3/pyproject.toml` & `use_case_registry-1.4.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -20,33 +20,34 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 # https://hatch.pypa.io/latest/config/dependency/
 dependencies = [
   "result",
-  "Jinja2"
+  "Jinja2",
+  "PyYAML"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
+
 sqlalchemy = [
   "SQLAlchemy"
 ]
 dev = [
   "pytest",
   "pytest-cov",
   "mypy",
   "ruff",
   "pip-tools",
   "hatch",
   "mkdocs-material",
   "toml",
   "black",
-  "PyYAML",
   "types-PyYAML",
   "pytest-env",
 ]
 
 [project.urls]
 Homepage = "https://github.com/Tomperez98/use-case-registry"
 Documentation = "https://tomperez98.github.io/use-case-registry/"
@@ -94,14 +95,15 @@
 # https://github.com/charliermarsh/ruff#is-ruff-compatible-with-black
 line-length = 88
 
 ignore = [
   "ANN101", # Missing type annotation for `self` in method
   "D203", # 1 blank line required before class docstring
   "D212", # Multi-line docstring summary should start at the first line
+  "ANN102", #  Missing type annotation for `cls` in classmethod
 ]
 
 select = [
   "ALL"
 ]
 
 fix = true
@@ -145,17 +147,14 @@
 docstring-quotes = "double"
 inline-quotes = "double"
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
-env = [
-    "EXECUTION_ENV=dev",
-]
 xfail_strict = true
 addopts =[
   "--cov-fail-under=85", 
   "--cov-report=term-missing:skip-covered",
   "--cov-config=pyproject.toml",
   "--cov=use_case_registry"
 ]
```

### Comparing `use_case_registry-1.4.3/PKG-INFO` & `use_case_registry-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: use_case_registry
-Version: 1.4.3
+Version: 1.4.4
 Summary: Registry class for Use Case implementation. They are basically meaningfull lists with some constraints.
 Project-URL: Homepage, https://github.com/Tomperez98/use-case-registry
 Project-URL: Documentation, https://tomperez98.github.io/use-case-registry/
 Project-URL: Issues, https://github.com/Tomperez98/use-case-registry/issues
 Project-URL: Source, https://github.com/Tomperez98/use-case-registry
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-Expression: MIT
@@ -14,25 +14,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Requires-Dist: jinja2
+Requires-Dist: pyyaml
 Requires-Dist: result
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: mkdocs-material; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pip-tools; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest-env; extra == 'dev'
-Requires-Dist: pyyaml; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: toml; extra == 'dev'
 Requires-Dist: types-pyyaml; extra == 'dev'
 Provides-Extra: sqlalchemy
 Requires-Dist: sqlalchemy; extra == 'sqlalchemy'
 Description-Content-Type: text/markdown
```


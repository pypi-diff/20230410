# Comparing `tmp/use_case_registry-1.4.2.tar.gz` & `tmp/use_case_registry-1.4.3.tar.gz`

## Comparing `use_case_registry-1.4.2.tar` & `use_case_registry-1.4.3.tar`

### file list

```diff
@@ -1,56 +1,46 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.tool-versions
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/Makefile
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/mkdocs.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.github/CODEOWNERS
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.github/workflows/audit.yml
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.github/workflows/release.yml
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.github/workflows/update_docs.yml
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.vscode/settings.json
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/docs/index.md
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/docs/general-thoughts/clean-architecture/index.md
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/docs/general-thoughts/error-handling/index.md
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/docs/general-thoughts/one-use-case-one-workflow/index.md
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/requirements/core.txt
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/requirements/dev.txt
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/requirements/sqlalchemy.txt
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/scripts/release_github.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/__init__.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/test_registry.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/assets/env_yamls/yaml-1.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/assets/repo_configs/conf-1.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/assets/repo_configs/conf-2.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/assets/repo_configs/conf-3.yml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/assets/repo_configs/conf-4.yml
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/assets/repo_configs/conf-5.yml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/assets/repo_configs/conf-6.yml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/assets/repo_configs/conf-7.yml
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/assets/repo_configs/conf-8.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/base/__init__.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/base/test_command.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/base/test_repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/parsers/__init__.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/parsers/test_repository_config.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/parsers/test_utils.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/__about__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/__init__.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/enums.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/py.typed
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/registry.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/base/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/base/command.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/base/repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/internals/__init__.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/internals/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/parsers/__init__.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/parsers/repository_config.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/parsers/utils.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/LICENSE.txt
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/README.md
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.tool-versions
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/Makefile
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/mkdocs.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.github/CODEOWNERS
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.github/workflows/audit.yml
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.github/workflows/update_docs.yml
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.vscode/settings.json
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/docs/index.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/docs/general-thoughts/clean-architecture/index.md
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/docs/general-thoughts/error-handling/index.md
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/docs/general-thoughts/one-use-case-one-workflow/index.md
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/requirements/core.txt
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/requirements/dev.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/requirements/sqlalchemy.txt
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/scripts/release_github.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/tests/__init__.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/tests/test_registry.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/tests/test_template_parser.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/tests/assets/templates/config-1.yml
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/tests/assets/templates/config-2.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/tests/assets/templates/config-3.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/tests/base/__init__.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/tests/base/test_command.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/tests/base/test_repository.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/__about__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/__init__.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/enums.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/py.typed
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/registry.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/template_parsers.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/base/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/base/command.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/base/repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/internals/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/use_case_registry/internals/errors.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/LICENSE.txt
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/README.md
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 use_case_registry-1.4.3/PKG-INFO
```

### Comparing `use_case_registry-1.4.2/Makefile` & `use_case_registry-1.4.3/Makefile`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/mkdocs.yml` & `use_case_registry-1.4.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/.github/ISSUE_TEMPLATE/bug_report.md` & `use_case_registry-1.4.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/.github/ISSUE_TEMPLATE/feature_request.md` & `use_case_registry-1.4.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/.github/workflows/audit.yml` & `use_case_registry-1.4.3/.github/workflows/audit.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/.github/workflows/coverage.yml` & `use_case_registry-1.4.3/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/.github/workflows/release.yml` & `use_case_registry-1.4.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/.github/workflows/test.yml` & `use_case_registry-1.4.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/.vscode/settings.json` & `use_case_registry-1.4.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/docs/index.md` & `use_case_registry-1.4.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/docs/general-thoughts/clean-architecture/index.md` & `use_case_registry-1.4.3/docs/general-thoughts/clean-architecture/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/docs/general-thoughts/error-handling/index.md` & `use_case_registry-1.4.3/docs/general-thoughts/error-handling/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/docs/general-thoughts/one-use-case-one-workflow/index.md` & `use_case_registry-1.4.3/docs/general-thoughts/one-use-case-one-workflow/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/requirements/dev.txt` & `use_case_registry-1.4.3/requirements/dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -52,27 +52,28 @@
     # via hatch
 idna==3.4
     # via
     #   anyio
     #   hyperlink
     #   requests
     #   rfc3986
-importlib-metadata==6.2.0
+importlib-metadata==6.2.1
     # via
     #   keyring
     #   markdown
     #   mkdocs
 iniconfig==2.0.0
     # via pytest
 jaraco-classes==3.2.3
     # via keyring
 jinja2==3.1.2
     # via
     #   mkdocs
     #   mkdocs-material
+    #   use_case_registry (pyproject.toml)
 keyring==23.13.1
     # via hatch
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-material
     #   pymdown-extensions
```

### Comparing `use_case_registry-1.4.2/scripts/release_github.py` & `use_case_registry-1.4.3/scripts/release_github.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/tests/test_registry.py` & `use_case_registry-1.4.3/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/tests/base/test_command.py` & `use_case_registry-1.4.3/tests/base/test_command.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/tests/base/test_repository.py` & `use_case_registry-1.4.3/tests/base/test_repository.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/use_case_registry/errors.py` & `use_case_registry-1.4.3/use_case_registry/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,12 +21,13 @@
     """Raised when there's an error committing a set of transactions."""
 
     def __init__(self, transactions: UseCaseRegistry[Any]) -> None:
         """Construct class."""
         super().__init__(f"Error commiting transactions {transactions}")
 
 
-class ConfigFileError(Exception):
-    """Raised when config file is wrong."""
+class EnvVarMissingError(Exception):
+    """Raised when a required enviroment variable is not set."""
 
-    def __init__(self, msg: str) -> None:  # noqa: D107
-        super().__init__(msg)
+    def __init__(self, env_var: str) -> None:
+        """Construct class."""
+        super().__init__(f"Env var required but not provided {env_var}")
```

### Comparing `use_case_registry-1.4.2/use_case_registry/registry.py` & `use_case_registry-1.4.3/use_case_registry/registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/use_case_registry/base/command.py` & `use_case_registry-1.4.3/use_case_registry/base/command.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/use_case_registry/base/repository.py` & `use_case_registry-1.4.3/use_case_registry/base/repository.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/use_case_registry/internals/errors.py` & `use_case_registry-1.4.3/use_case_registry/internals/errors.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/.gitignore` & `use_case_registry-1.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/LICENSE.txt` & `use_case_registry-1.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/README.md` & `use_case_registry-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.2/pyproject.toml` & `use_case_registry-1.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 # https://hatch.pypa.io/latest/config/dependency/
 dependencies = [
   "result",
-  "pyyaml"
+  "Jinja2"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 sqlalchemy = [
   "SQLAlchemy"
 ]
@@ -38,16 +38,17 @@
   "mypy",
   "ruff",
   "pip-tools",
   "hatch",
   "mkdocs-material",
   "toml",
   "black",
+  "PyYAML",
   "types-PyYAML",
-  "pytest-env"
+  "pytest-env",
 ]
 
 [project.urls]
 Homepage = "https://github.com/Tomperez98/use-case-registry"
 Documentation = "https://tomperez98.github.io/use-case-registry/"
 Issues = "https://github.com/Tomperez98/use-case-registry/issues"
 Source = "https://github.com/Tomperez98/use-case-registry"
```

### Comparing `use_case_registry-1.4.2/PKG-INFO` & `use_case_registry-1.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: use_case_registry
-Version: 1.4.2
+Version: 1.4.3
 Summary: Registry class for Use Case implementation. They are basically meaningfull lists with some constraints.
 Project-URL: Homepage, https://github.com/Tomperez98/use-case-registry
 Project-URL: Documentation, https://tomperez98.github.io/use-case-registry/
 Project-URL: Issues, https://github.com/Tomperez98/use-case-registry/issues
 Project-URL: Source, https://github.com/Tomperez98/use-case-registry
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-Expression: MIT
@@ -13,25 +13,26 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
-Requires-Dist: pyyaml
+Requires-Dist: jinja2
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
+Requires-Dist: pyyaml; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: toml; extra == 'dev'
 Requires-Dist: types-pyyaml; extra == 'dev'
 Provides-Extra: sqlalchemy
 Requires-Dist: sqlalchemy; extra == 'sqlalchemy'
 Description-Content-Type: text/markdown
```


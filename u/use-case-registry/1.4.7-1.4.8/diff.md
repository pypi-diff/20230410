# Comparing `tmp/use_case_registry-1.4.7.tar.gz` & `tmp/use_case_registry-1.4.8.tar.gz`

## Comparing `use_case_registry-1.4.7.tar` & `use_case_registry-1.4.8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/.tool-versions
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/Makefile
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/mkdocs.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/.github/CODEOWNERS
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/.github/workflows/audit.yml
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/.github/workflows/release.yml
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/.github/workflows/test.yml
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/.github/workflows/update_docs.yml
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/.vscode/settings.json
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/docs/index.md
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/docs/general-thoughts/clean-architecture/index.md
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/docs/general-thoughts/error-handling/index.md
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/docs/general-thoughts/one-use-case-one-workflow/index.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/requirements/core.txt
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/requirements/dev.txt
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/requirements/sqlalchemy.txt
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/scripts/release_github.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/tests/__init__.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/tests/test_enums.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/tests/test_registry.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/tests/assets/templates/target-based/config-1.yml
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/tests/assets/templates/target-based/config-2.yml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/tests/assets/templates/target-based/config-3.yml
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/tests/assets/templates/target-based/config-4.yml
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/tests/assets/templates/target-based/config-5.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/tests/base/__init__.py
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/tests/base/test_command.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/tests/base/test_repository.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/tests/base/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/tests/parsers/__init__.py
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/tests/parsers/test_target_based.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/use_case_registry/__about__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/use_case_registry/__init__.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/use_case_registry/enums.py
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/use_case_registry/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/use_case_registry/py.typed
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/use_case_registry/registry.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/use_case_registry/base/__init__.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/use_case_registry/base/command.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/use_case_registry/base/repository.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/use_case_registry/base/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/use_case_registry/internals/__init__.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/use_case_registry/internals/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/use_case_registry/pasers/__init__.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/use_case_registry/pasers/macros.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/use_case_registry/pasers/target_based.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/LICENSE.txt
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/README.md
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/pyproject.toml
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 use_case_registry-1.4.7/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.tool-versions
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/Makefile
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/mkdocs.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.github/CODEOWNERS
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.github/workflows/audit.yml
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.github/workflows/test.yml
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.github/workflows/update_docs.yml
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.vscode/settings.json
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/docs/index.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/docs/general-thoughts/clean-architecture/index.md
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/docs/general-thoughts/error-handling/index.md
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/docs/general-thoughts/one-use-case-one-workflow/index.md
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/requirements/core.txt
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/requirements/dev.txt
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/requirements/sqlalchemy.txt
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/scripts/release_github.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/__init__.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/test_enums.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/test_registry.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/assets/templates/target-based/config-1.yml
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/assets/templates/target-based/config-2.yml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/assets/templates/target-based/config-3.yml
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/assets/templates/target-based/config-4.yml
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/assets/templates/target-based/config-5.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/base/__init__.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/base/test_command.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/base/test_repository.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/base/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/parsers/__init__.py
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/tests/parsers/test_target_based.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/__about__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/__init__.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/enums.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/py.typed
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/registry.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/base/__init__.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/base/command.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/base/repository.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/base/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/internals/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/internals/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/pasers/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/pasers/macros.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/use_case_registry/pasers/target_based.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/LICENSE.txt
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/README.md
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/pyproject.toml
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 use_case_registry-1.4.8/PKG-INFO
```

### Comparing `use_case_registry-1.4.7/Makefile` & `use_case_registry-1.4.8/Makefile`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/mkdocs.yml` & `use_case_registry-1.4.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/.github/ISSUE_TEMPLATE/bug_report.md` & `use_case_registry-1.4.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/.github/ISSUE_TEMPLATE/feature_request.md` & `use_case_registry-1.4.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/.github/workflows/audit.yml` & `use_case_registry-1.4.8/.github/workflows/audit.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/.github/workflows/coverage.yml` & `use_case_registry-1.4.8/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/.github/workflows/release.yml` & `use_case_registry-1.4.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/.github/workflows/test.yml` & `use_case_registry-1.4.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/.vscode/settings.json` & `use_case_registry-1.4.8/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/docs/index.md` & `use_case_registry-1.4.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/docs/general-thoughts/clean-architecture/index.md` & `use_case_registry-1.4.8/docs/general-thoughts/clean-architecture/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/docs/general-thoughts/error-handling/index.md` & `use_case_registry-1.4.8/docs/general-thoughts/error-handling/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/docs/general-thoughts/one-use-case-one-workflow/index.md` & `use_case_registry-1.4.8/docs/general-thoughts/one-use-case-one-workflow/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/requirements/core.txt` & `use_case_registry-1.4.8/requirements/sqlalchemy.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --no-emit-trusted-host --output-file=requirements/core.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=sqlalchemy --no-emit-trusted-host --output-file=requirements/sqlalchemy.txt --resolver=backtracking pyproject.toml
 #
-fastjsonschema==2.16.3
-    # via use_case_registry (pyproject.toml)
+attrs==22.2.0
+    # via jsonschema
 jinja2==3.1.2
     # via use_case_registry (pyproject.toml)
+jsonschema==4.17.3
+    # via use_case_registry (pyproject.toml)
 markupsafe==2.1.2
     # via jinja2
 mashumaro[orjson,yaml]==3.6
     # via use_case_registry (pyproject.toml)
 orjson==3.8.10
     # via mashumaro
+pyrsistent==0.19.3
+    # via jsonschema
 pyyaml==6.0
     # via mashumaro
 result==0.9.0
     # via use_case_registry (pyproject.toml)
+sqlalchemy==2.0.9
+    # via use_case_registry (pyproject.toml)
 typing-extensions==4.5.0
     # via
     #   mashumaro
     #   result
+    #   sqlalchemy
```

### Comparing `use_case_registry-1.4.7/requirements/dev.txt` & `use_case_registry-1.4.8/requirements/dev.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --extra=dev --extra=sqlalchemy --no-emit-trusted-host --output-file=requirements/dev.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
+attrs==22.2.0
+    # via jsonschema
 black==23.3.0
     # via use_case_registry (pyproject.toml)
 build==0.10.0
     # via pip-tools
 certifi==2022.12.7
     # via
     #   httpcore
@@ -30,16 +32,14 @@
     # via pytest-cov
 distlib==0.3.6
     # via virtualenv
 editables==0.3
     # via hatchling
 exceptiongroup==1.1.1
     # via pytest
-fastjsonschema==2.16.3
-    # via use_case_registry (pyproject.toml)
 filelock==3.11.0
     # via virtualenv
 ghp-import==2.1.0
     # via mkdocs
 h11==0.14.0
     # via httpcore
 hatch==1.7.0
@@ -68,14 +68,16 @@
 jaraco-classes==3.2.3
     # via keyring
 jinja2==3.1.2
     # via
     #   mkdocs
     #   mkdocs-material
     #   use_case_registry (pyproject.toml)
+jsonschema==4.17.3
+    # via use_case_registry (pyproject.toml)
 keyring==23.13.1
     # via hatch
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-material
     #   pymdown-extensions
@@ -138,14 +140,16 @@
     #   rich
 pymdown-extensions==9.11
     # via mkdocs-material
 pyperclip==1.8.2
     # via hatch
 pyproject-hooks==1.0.0
     # via build
+pyrsistent==0.19.3
+    # via jsonschema
 pytest==7.3.0
     # via
     #   pytest-cov
     #   pytest-env
     #   use_case_registry (pyproject.toml)
 pytest-cov==4.0.0
     # via use_case_registry (pyproject.toml)
```

### Comparing `use_case_registry-1.4.7/scripts/release_github.py` & `use_case_registry-1.4.8/scripts/release_github.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/tests/test_registry.py` & `use_case_registry-1.4.8/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/tests/base/test_command.py` & `use_case_registry-1.4.8/tests/base/test_command.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/tests/base/test_repository.py` & `use_case_registry-1.4.8/tests/base/test_repository.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/tests/base/test_utils.py` & `use_case_registry-1.4.8/tests/base/test_utils.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/tests/parsers/test_target_based.py` & `use_case_registry-1.4.8/tests/parsers/test_target_based.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/use_case_registry/enums.py` & `use_case_registry-1.4.8/use_case_registry/enums.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/use_case_registry/errors.py` & `use_case_registry-1.4.8/use_case_registry/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Custom defined errors."""
 
 import pathlib
-from typing import Any
+from typing import Any, Union
 
 from use_case_registry import UseCaseRegistry
 
 
 class CommandInputValidationError(Exception):
     """Raised when command input values does pass validation check."""
 
-    def __init__(self, msg: str) -> None:
+    def __init__(self, msg: Union[str, list[str]]) -> None:
         """Construct class."""
         super().__init__(msg)
 
 
 class UseCaseExecutionError(Exception):
     """Raised when there's an error executing a workflow."""
```

### Comparing `use_case_registry-1.4.7/use_case_registry/registry.py` & `use_case_registry-1.4.8/use_case_registry/registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/use_case_registry/base/command.py` & `use_case_registry-1.4.8/use_case_registry/base/command.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/use_case_registry/base/repository.py` & `use_case_registry-1.4.8/use_case_registry/base/repository.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/use_case_registry/internals/errors.py` & `use_case_registry-1.4.8/use_case_registry/internals/errors.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/use_case_registry/pasers/macros.py` & `use_case_registry-1.4.8/use_case_registry/pasers/macros.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/use_case_registry/pasers/target_based.py` & `use_case_registry-1.4.8/use_case_registry/pasers/target_based.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/.gitignore` & `use_case_registry-1.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/LICENSE.txt` & `use_case_registry-1.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/README.md` & `use_case_registry-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.7/pyproject.toml` & `use_case_registry-1.4.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 # https://hatch.pypa.io/latest/config/dependency/
 dependencies = [
   "result",
   "Jinja2",
   "mashumaro[orjson,yaml]",
-  "fastjsonschema"
+  "jsonschema"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 
 sqlalchemy = [
   "SQLAlchemy"
```

### Comparing `use_case_registry-1.4.7/PKG-INFO` & `use_case_registry-1.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: use_case_registry
-Version: 1.4.7
+Version: 1.4.8
 Summary: Registry class for Use Case implementation. They are basically meaningfull lists with some constraints.
 Project-URL: Homepage, https://github.com/Tomperez98/use-case-registry
 Project-URL: Documentation, https://tomperez98.github.io/use-case-registry/
 Project-URL: Issues, https://github.com/Tomperez98/use-case-registry/issues
 Project-URL: Source, https://github.com/Tomperez98/use-case-registry
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-Expression: MIT
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
-Requires-Dist: fastjsonschema
 Requires-Dist: jinja2
+Requires-Dist: jsonschema
 Requires-Dist: mashumaro[orjson,yaml]
 Requires-Dist: result
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: mkdocs-material; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
```


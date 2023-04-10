# Comparing `tmp/use_case_registry-1.4.4.tar.gz` & `tmp/use_case_registry-1.4.5.tar.gz`

## Comparing `use_case_registry-1.4.4.tar` & `use_case_registry-1.4.5.tar`

### file list

```diff
@@ -1,58 +1,51 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.tool-versions
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/Makefile
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/mkdocs.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.github/CODEOWNERS
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.github/workflows/audit.yml
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.github/workflows/release.yml
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.github/workflows/test.yml
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.github/workflows/update_docs.yml
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.vscode/settings.json
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/docs/index.md
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/docs/general-thoughts/clean-architecture/index.md
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/docs/general-thoughts/error-handling/index.md
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/docs/general-thoughts/one-use-case-one-workflow/index.md
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/requirements/core.txt
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/requirements/dev.txt
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/requirements/sqlalchemy.txt
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/scripts/release_github.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/__init__.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/test_registry.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/assets/templates/raw/config-1.yml
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/assets/templates/raw/config-2.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/assets/templates/raw/config-3.yml
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/assets/templates/repository/config-1.yml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/assets/templates/repository/config-2.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/assets/templates/repository/config-no-connection.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/assets/templates/repository/config-no-drivername.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/assets/templates/repository/config-no-url.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/base/__init__.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/base/test_command.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/base/test_repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/parsers/__init__.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/parsers/test_base.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/parsers/test_raw.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/tests/parsers/test_repository.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/__about__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/__init__.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/enums.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/py.typed
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/registry.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/base/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/base/command.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/base/repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/internals/__init__.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/internals/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/pasers/__init__.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/pasers/base.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/pasers/macros.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/pasers/raw.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/use_case_registry/pasers/repository.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/LICENSE.txt
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/README.md
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/pyproject.toml
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 use_case_registry-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.tool-versions
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/Makefile
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/mkdocs.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.github/CODEOWNERS
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.github/workflows/audit.yml
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.github/workflows/update_docs.yml
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.vscode/settings.json
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/docs/index.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/docs/general-thoughts/clean-architecture/index.md
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/docs/general-thoughts/error-handling/index.md
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/docs/general-thoughts/one-use-case-one-workflow/index.md
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/requirements/core.txt
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/requirements/dev.txt
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/requirements/sqlalchemy.txt
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/scripts/release_github.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/__init__.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/test_enums.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/test_registry.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/assets/templates/target-based/config-1.yml
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/assets/templates/target-based/config-2.yml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/assets/templates/target-based/config-3.yml
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/assets/templates/target-based/config-4.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/base/__init__.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/base/test_command.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/base/test_repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/parsers/__init__.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/tests/parsers/test_target_based.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/__about__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/__init__.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/enums.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/py.typed
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/registry.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/base/__init__.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/base/command.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/base/repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/internals/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/internals/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/pasers/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/pasers/macros.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/use_case_registry/pasers/target_based.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/LICENSE.txt
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/README.md
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 use_case_registry-1.4.5/PKG-INFO
```

### Comparing `use_case_registry-1.4.4/Makefile` & `use_case_registry-1.4.5/Makefile`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/mkdocs.yml` & `use_case_registry-1.4.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/.github/ISSUE_TEMPLATE/bug_report.md` & `use_case_registry-1.4.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/.github/ISSUE_TEMPLATE/feature_request.md` & `use_case_registry-1.4.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/.github/workflows/audit.yml` & `use_case_registry-1.4.5/.github/workflows/audit.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/.github/workflows/coverage.yml` & `use_case_registry-1.4.5/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/.github/workflows/release.yml` & `use_case_registry-1.4.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/.github/workflows/test.yml` & `use_case_registry-1.4.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/.vscode/settings.json` & `use_case_registry-1.4.5/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/docs/index.md` & `use_case_registry-1.4.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/docs/general-thoughts/clean-architecture/index.md` & `use_case_registry-1.4.5/docs/general-thoughts/clean-architecture/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/docs/general-thoughts/error-handling/index.md` & `use_case_registry-1.4.5/docs/general-thoughts/error-handling/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/docs/general-thoughts/one-use-case-one-workflow/index.md` & `use_case_registry-1.4.5/docs/general-thoughts/one-use-case-one-workflow/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/requirements/dev.txt` & `use_case_registry-1.4.5/requirements/dev.txt`

 * *Files 6% similar despite different names*

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
@@ -52,39 +54,43 @@
     # via hatch
 idna==3.4
     # via
     #   anyio
     #   hyperlink
     #   requests
     #   rfc3986
-importlib-metadata==6.2.1
+importlib-metadata==6.3.0
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
 markdown-it-py==2.2.0
     # via rich
 markupsafe==2.1.2
     # via jinja2
+mashumaro[orjson,yaml]==3.6
+    # via use_case_registry (pyproject.toml)
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via mkdocs
 mkdocs==1.4.2
     # via mkdocs-material
 mkdocs-material==9.1.6
@@ -95,14 +101,16 @@
     # via jaraco-classes
 mypy==1.2.0
     # via use_case_registry (pyproject.toml)
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
+orjson==3.8.10
+    # via mashumaro
 packaging==23.0
     # via
     #   black
     #   build
     #   hatch
     #   hatchling
     #   mkdocs
@@ -122,41 +130,43 @@
     #   virtualenv
 pluggy==1.0.0
     # via
     #   hatchling
     #   pytest
 ptyprocess==0.7.0
     # via pexpect
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   mkdocs-material
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
 pytest-env==0.8.1
     # via use_case_registry (pyproject.toml)
 python-dateutil==2.8.2
     # via ghp-import
 pyyaml==6.0
     # via
+    #   mashumaro
     #   mkdocs
     #   pymdown-extensions
     #   pyyaml-env-tag
-    #   use_case_registry (pyproject.toml)
 pyyaml-env-tag==0.1
     # via mkdocs
 regex==2023.3.23
     # via mkdocs-material
 requests==2.28.2
     # via mkdocs-material
 result==0.9.0
@@ -191,19 +201,22 @@
     #   pytest
 tomli-w==1.0.0
     # via hatch
 tomlkit==0.11.7
     # via hatch
 trove-classifiers==2023.3.9
     # via hatchling
+types-jsonschema==4.17.0.7
+    # via use_case_registry (pyproject.toml)
 types-pyyaml==6.0.12.9
     # via use_case_registry (pyproject.toml)
 typing-extensions==4.5.0
     # via
     #   black
+    #   mashumaro
     #   mypy
     #   result
     #   sqlalchemy
 urllib3==1.26.15
     # via requests
 userpath==1.8.0
     # via hatch
```

### Comparing `use_case_registry-1.4.4/scripts/release_github.py` & `use_case_registry-1.4.5/scripts/release_github.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/tests/test_registry.py` & `use_case_registry-1.4.5/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/tests/base/test_command.py` & `use_case_registry-1.4.5/tests/base/test_command.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,75 @@
 """Tests for command."""
+from dataclasses import dataclass
+from typing import Any
+
 import pytest
-from result import Err, Ok, Result
+from result import Ok, Result
 
 from use_case_registry import UseCaseRegistry
-from use_case_registry.base import ICommand
+from use_case_registry.base.command import BaseCommand, ICommandInput
 from use_case_registry.errors import CommandInputValidationError, UseCaseExecutionError
 
 
-class TestICommand:
-    """Test definition for ICommand."""
+@dataclass(
+    frozen=True,
+    repr=False,
+    eq=False,
+)
+class ExampleCommandInput(ICommandInput):
+    """Example command input."""
+
+    name: str
+    age: int
+    last_name: str
+
+    class Config:
+        """Dataclass config."""
+
+        json_schema = {
+            "properties": {
+                "name": {
+                    "maxLength": 9,
+                },
+            },
+        }
+
+
+class ExampleCommand(BaseCommand):
+    """Example command."""
+
+    def execute(
+        self,
+        write_ops_registry: UseCaseRegistry[Any],
+    ) -> Result[Any, UseCaseExecutionError]:
+        """Null command executuion."""
+        _ = write_ops_registry
+
+        return Ok()
+
+
+def test_validate_command_pass() -> None:
+    """Test validate command passes."""
+    inputs = ExampleCommandInput(name="tomas", last_name="perez", age=10)
+    ExampleCommand(inputs=inputs).validate().unwrap()
+
+
+@pytest.mark.parametrize(
+    argnames="inputs",
+    argvalues=[
+        ExampleCommandInput(
+            name="tomas",
+            last_name="perez",
+            age="a",  # type: ignore[arg-type]
+        ),
+        ExampleCommandInput(
+            name="a" * 11,
+            last_name="perez",
+            age=10,
+        ),
+    ],
+)
+def test_validate_command_fails(inputs: ICommandInput) -> None:
+    """Test validate command fails."""
+    validation_err = ExampleCommand(inputs=inputs).validate().err()
 
-    def test_cannot_be_instantiated(self) -> None:
-        """ICommand is an interface an cannot be instantiated."""
-        with pytest.raises(TypeError):
-            ICommand()  # type:ignore[abstract]
-
-    def test_interface_can_be_extendend(self) -> None:
-        """Test interface can be extended."""
-
-        class ConcreteCommand(ICommand):
-            def __init__(self, name: str, last_name: str) -> None:
-                """Construct concrete implementation."""
-                self.name = name
-                self.last_name = last_name
-
-            def validate(self) -> Result[None, CommandInputValidationError]:
-                """Validate input arguments are valid."""
-                conditions = self.name.isascii() and self.last_name.isascii()
-                if not conditions:
-                    return Err(CommandInputValidationError())
-
-                return Ok()
-
-            def execute(
-                self,
-                write_ops_registry: UseCaseRegistry[str],
-            ) -> Result[str, UseCaseExecutionError]:
-                _ = write_ops_registry
-                return Ok()
-
-        command = ConcreteCommand(name="Tomas", last_name="Perez")
-        command.validate()
-        command.execute(write_ops_registry=UseCaseRegistry[str](max_length=10))
+    assert isinstance(validation_err, CommandInputValidationError)
```

### Comparing `use_case_registry-1.4.4/tests/base/test_repository.py` & `use_case_registry-1.4.5/tests/base/test_repository.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/use_case_registry/enums.py` & `use_case_registry-1.4.5/use_case_registry/enums.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/use_case_registry/errors.py` & `use_case_registry-1.4.5/use_case_registry/errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 """Custom defined errors."""
 
+import pathlib
 from typing import Any
 
 from use_case_registry import UseCaseRegistry
 
 
 class CommandInputValidationError(Exception):
     """Raised when command input values does pass validation check."""
 
+    def __init__(self, msg: str) -> None:
+        """Construct class."""
+        super().__init__(msg)
+
 
 class UseCaseExecutionError(Exception):
     """Raised when there's an error executing a workflow."""
 
     def __init__(self, error: Exception) -> None:
         """Construct class."""
         super().__init__(f"Error executing a use case {error}")
@@ -27,7 +32,15 @@
 
 class EnvVarMissingError(Exception):
     """Raised when a required enviroment variable is not set."""
 
     def __init__(self, env_var: str) -> None:
         """Construct class."""
         super().__init__(f"Env var required but not provided {env_var}")
+
+
+class SchemaNotFoundError(Exception):
+    """Raised when schema not found."""
+
+    def __init__(self, path: pathlib.Path) -> None:
+        """Construct class."""
+        super().__init__(f"Schema not found {path}")
```

### Comparing `use_case_registry-1.4.4/use_case_registry/registry.py` & `use_case_registry-1.4.5/use_case_registry/registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/use_case_registry/base/repository.py` & `use_case_registry-1.4.5/use_case_registry/base/repository.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/use_case_registry/internals/errors.py` & `use_case_registry-1.4.5/use_case_registry/internals/errors.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/use_case_registry/pasers/macros.py` & `use_case_registry-1.4.5/use_case_registry/pasers/macros.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/.gitignore` & `use_case_registry-1.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/LICENSE.txt` & `use_case_registry-1.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/README.md` & `use_case_registry-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.4/pyproject.toml` & `use_case_registry-1.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,16 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 # https://hatch.pypa.io/latest/config/dependency/
 dependencies = [
   "result",
   "Jinja2",
-  "PyYAML"
+  "mashumaro[orjson,yaml]",
+  "jsonschema"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 
 sqlalchemy = [
   "SQLAlchemy"
@@ -42,14 +43,15 @@
   "pip-tools",
   "hatch",
   "mkdocs-material",
   "toml",
   "black",
   "types-PyYAML",
   "pytest-env",
+  "types-jsonschema"
 ]
 
 [project.urls]
 Homepage = "https://github.com/Tomperez98/use-case-registry"
 Documentation = "https://tomperez98.github.io/use-case-registry/"
 Issues = "https://github.com/Tomperez98/use-case-registry/issues"
 Source = "https://github.com/Tomperez98/use-case-registry"
```

### Comparing `use_case_registry-1.4.4/PKG-INFO` & `use_case_registry-1.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: use_case_registry
-Version: 1.4.4
+Version: 1.4.5
 Summary: Registry class for Use Case implementation. They are basically meaningfull lists with some constraints.
 Project-URL: Homepage, https://github.com/Tomperez98/use-case-registry
 Project-URL: Documentation, https://tomperez98.github.io/use-case-registry/
 Project-URL: Issues, https://github.com/Tomperez98/use-case-registry/issues
 Project-URL: Source, https://github.com/Tomperez98/use-case-registry
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-Expression: MIT
@@ -14,27 +14,29 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Requires-Dist: jinja2
-Requires-Dist: pyyaml
+Requires-Dist: jsonschema
+Requires-Dist: mashumaro[orjson,yaml]
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
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: toml; extra == 'dev'
+Requires-Dist: types-jsonschema; extra == 'dev'
 Requires-Dist: types-pyyaml; extra == 'dev'
 Provides-Extra: sqlalchemy
 Requires-Dist: sqlalchemy; extra == 'sqlalchemy'
 Description-Content-Type: text/markdown
 
 # use-case-registry
```


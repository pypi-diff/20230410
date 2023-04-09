# Comparing `tmp/use_case_registry-1.4.1.tar.gz` & `tmp/use_case_registry-1.4.2.tar.gz`

## Comparing `use_case_registry-1.4.1.tar` & `use_case_registry-1.4.2.tar`

### file list

```diff
@@ -1,54 +1,56 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.tool-versions
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/Makefile
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/mkdocs.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.github/workflows/audit.yml
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.github/workflows/update_docs.yml
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.vscode/settings.json
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/docs/index.md
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/docs/general-thoughts/clean-architecture/index.md
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/docs/general-thoughts/error-handling/index.md
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/docs/general-thoughts/one-use-case-one-workflow/index.md
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/requirements/core.txt
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/requirements/dev.txt
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/requirements/sqlalchemy.txt
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/scripts/release_github.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/test_parsers.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/test_registry.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/assets/repo_configs/conf-1.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/assets/repo_configs/conf-2.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/assets/repo_configs/conf-3.yml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/assets/repo_configs/conf-4.yml
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/assets/repo_configs/conf-5.yml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/assets/repo_configs/conf-6.yml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/assets/repo_configs/conf-7.yml
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/assets/repo_configs/conf-8.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/base/__init__.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/base/test_command.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/tests/base/test_repository.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/__about__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/__init__.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/enums.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/py.typed
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/registry.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/base/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/base/command.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/base/repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/internals/__init__.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/internals/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/parsers/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/parsers/errors.py
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/parsers/repository_config.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/use_case_registry/parsers/utils.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/LICENSE.txt
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/README.md
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 use_case_registry-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.tool-versions
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/Makefile
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/mkdocs.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.github/workflows/audit.yml
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.github/workflows/update_docs.yml
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.vscode/settings.json
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/docs/index.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/docs/general-thoughts/clean-architecture/index.md
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/docs/general-thoughts/error-handling/index.md
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/docs/general-thoughts/one-use-case-one-workflow/index.md
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/requirements/core.txt
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/requirements/dev.txt
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/requirements/sqlalchemy.txt
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/scripts/release_github.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/test_registry.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/assets/env_yamls/yaml-1.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/assets/repo_configs/conf-1.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/assets/repo_configs/conf-2.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/assets/repo_configs/conf-3.yml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/assets/repo_configs/conf-4.yml
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/assets/repo_configs/conf-5.yml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/assets/repo_configs/conf-6.yml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/assets/repo_configs/conf-7.yml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/assets/repo_configs/conf-8.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/base/__init__.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/base/test_command.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/base/test_repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/parsers/__init__.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/parsers/test_repository_config.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/tests/parsers/test_utils.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/__about__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/__init__.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/enums.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/py.typed
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/registry.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/base/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/base/command.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/base/repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/internals/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/internals/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/parsers/__init__.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/parsers/repository_config.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/use_case_registry/parsers/utils.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/LICENSE.txt
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/README.md
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 use_case_registry-1.4.2/PKG-INFO
```

### Comparing `use_case_registry-1.4.1/Makefile` & `use_case_registry-1.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/mkdocs.yml` & `use_case_registry-1.4.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/.github/ISSUE_TEMPLATE/bug_report.md` & `use_case_registry-1.4.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/.github/ISSUE_TEMPLATE/feature_request.md` & `use_case_registry-1.4.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/.github/workflows/audit.yml` & `use_case_registry-1.4.2/.github/workflows/audit.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/.github/workflows/coverage.yml` & `use_case_registry-1.4.2/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/.github/workflows/release.yml` & `use_case_registry-1.4.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/.github/workflows/test.yml` & `use_case_registry-1.4.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/.vscode/settings.json` & `use_case_registry-1.4.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/docs/index.md` & `use_case_registry-1.4.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/docs/general-thoughts/clean-architecture/index.md` & `use_case_registry-1.4.2/docs/general-thoughts/clean-architecture/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/docs/general-thoughts/error-handling/index.md` & `use_case_registry-1.4.2/docs/general-thoughts/error-handling/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/docs/general-thoughts/one-use-case-one-workflow/index.md` & `use_case_registry-1.4.2/docs/general-thoughts/one-use-case-one-workflow/index.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/requirements/dev.txt` & `use_case_registry-1.4.2/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/scripts/release_github.py` & `use_case_registry-1.4.2/scripts/release_github.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/tests/test_parsers.py` & `use_case_registry-1.4.2/tests/parsers/test_repository_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Test repository config parser."""
 import pathlib
 
 import pytest
 from sqlalchemy import create_engine
 
-from use_case_registry.parsers.errors import ConfigFileError
+from use_case_registry.errors import ConfigFileError
 from use_case_registry.parsers.repository_config import RepoConfigParser, RepoEngines
 
 
 class TestRepoConfigParser:
     """Test Repository Config Parser."""
 
     @pytest.mark.parametrize(
```

### Comparing `use_case_registry-1.4.1/tests/test_registry.py` & `use_case_registry-1.4.2/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/tests/base/test_command.py` & `use_case_registry-1.4.2/tests/base/test_command.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/tests/base/test_repository.py` & `use_case_registry-1.4.2/tests/base/test_repository.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/use_case_registry/errors.py` & `use_case_registry-1.4.2/use_case_registry/errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,7 +19,14 @@
 
 class CommitTransactionsError(Exception):
     """Raised when there's an error committing a set of transactions."""
 
     def __init__(self, transactions: UseCaseRegistry[Any]) -> None:
         """Construct class."""
         super().__init__(f"Error commiting transactions {transactions}")
+
+
+class ConfigFileError(Exception):
+    """Raised when config file is wrong."""
+
+    def __init__(self, msg: str) -> None:  # noqa: D107
+        super().__init__(msg)
```

### Comparing `use_case_registry-1.4.1/use_case_registry/registry.py` & `use_case_registry-1.4.2/use_case_registry/registry.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/use_case_registry/base/command.py` & `use_case_registry-1.4.2/use_case_registry/base/command.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/use_case_registry/base/repository.py` & `use_case_registry-1.4.2/use_case_registry/base/repository.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/use_case_registry/internals/errors.py` & `use_case_registry-1.4.2/use_case_registry/internals/errors.py`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/use_case_registry/parsers/repository_config.py` & `use_case_registry-1.4.2/use_case_registry/parsers/repository_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import pathlib
 from typing import Any
 
 import yaml
 from typing_extensions import assert_never
 
 from use_case_registry.enums import OptionEnums
-from use_case_registry.parsers.errors import ConfigFileError
-from use_case_registry.parsers.utils import construct_env_tag
+from use_case_registry.errors import ConfigFileError
+from use_case_registry.parsers.utils import env_tag_constructor
 
-yaml.Loader.add_constructor(tag="!ENV", constructor=construct_env_tag)
+yaml.Loader.add_constructor(tag="!ENV", constructor=env_tag_constructor)
 
 
 class RepoEngines(OptionEnums):
     """Support Repository Engines."""
 
     SQLALCHEMY = "SQLALCHEMY"
```

### Comparing `use_case_registry-1.4.1/.gitignore` & `use_case_registry-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/LICENSE.txt` & `use_case_registry-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/README.md` & `use_case_registry-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/pyproject.toml` & `use_case_registry-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `use_case_registry-1.4.1/PKG-INFO` & `use_case_registry-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: use_case_registry
-Version: 1.4.1
+Version: 1.4.2
 Summary: Registry class for Use Case implementation. They are basically meaningfull lists with some constraints.
 Project-URL: Homepage, https://github.com/Tomperez98/use-case-registry
 Project-URL: Documentation, https://tomperez98.github.io/use-case-registry/
 Project-URL: Issues, https://github.com/Tomperez98/use-case-registry/issues
 Project-URL: Source, https://github.com/Tomperez98/use-case-registry
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-Expression: MIT
```


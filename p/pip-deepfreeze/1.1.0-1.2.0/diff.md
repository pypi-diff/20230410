# Comparing `tmp/pip_deepfreeze-1.1.0.tar.gz` & `tmp/pip_deepfreeze-1.2.0.tar.gz`

## Comparing `pip_deepfreeze-1.1.0.tar` & `pip_deepfreeze-1.2.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/.flake8
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/HISTORY.rst
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/tox.ini
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0    69128 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/docs/logo.png
--rw-r--r--   0        0        0    10764 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/docs/logo.svg
--rw-r--r--   0        0        0    16834 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/docs/synopsis.odg
--rw-r--r--   0        0        0    88633 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/docs/synopsis.png
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/news/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/src/pip_deepfreeze/__init__.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/src/pip_deepfreeze/__main__.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/src/pip_deepfreeze/compat.py
--rwxr-xr-x   0        0        0     2693 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/src/pip_deepfreeze/env_info_json.py
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/src/pip_deepfreeze/installed_dist.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/src/pip_deepfreeze/list_installed_depends.py
--rw-r--r--   0        0        0     8012 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/src/pip_deepfreeze/pip.py
--rwxr-xr-x   0        0        0     2374 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/src/pip_deepfreeze/pip_list_json.py
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/src/pip_deepfreeze/project_name.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/src/pip_deepfreeze/pyproject_toml.py
--rw-r--r--   0        0        0    15973 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/src/pip_deepfreeze/req_file_parser.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/src/pip_deepfreeze/req_merge.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/src/pip_deepfreeze/req_parser.py
--rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/src/pip_deepfreeze/sanity.py
--rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/src/pip_deepfreeze/sync.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/src/pip_deepfreeze/tree.py
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/src/pip_deepfreeze/utils.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/tests/test_env_info_json.py
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/tests/test_list_installed_depends.py
--rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/tests/test_pip.py
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/tests/test_pip_list_json.py
--rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/tests/test_project_name.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/tests/test_pyproject_options.py
--rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/tests/test_req_file_parser.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/tests/test_req_merge.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/tests/test_req_parser.py
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/tests/test_sanity.py
--rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/tests/test_sync.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/tests/test_tree.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/tests/test_utils.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0    17464 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/README.rst
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    19102 2020-02-02 00:00:00.000000 pip_deepfreeze-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/.flake8
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/HISTORY.rst
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/tox.ini
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0    69128 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/docs/logo.png
+-rw-r--r--   0        0        0    10764 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/docs/logo.svg
+-rw-r--r--   0        0        0    16834 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/docs/synopsis.odg
+-rw-r--r--   0        0        0    88633 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/docs/synopsis.png
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/news/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/src/pip_deepfreeze/__init__.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/src/pip_deepfreeze/__main__.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/src/pip_deepfreeze/compat.py
+-rwxr-xr-x   0        0        0     2693 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/src/pip_deepfreeze/env_info_json.py
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/src/pip_deepfreeze/installed_dist.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/src/pip_deepfreeze/list_installed_depends.py
+-rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/src/pip_deepfreeze/pip.py
+-rwxr-xr-x   0        0        0     2374 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/src/pip_deepfreeze/pip_list_json.py
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/src/pip_deepfreeze/project_name.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/src/pip_deepfreeze/pyproject_toml.py
+-rw-r--r--   0        0        0    15973 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/src/pip_deepfreeze/req_file_parser.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/src/pip_deepfreeze/req_merge.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/src/pip_deepfreeze/req_parser.py
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/src/pip_deepfreeze/sanity.py
+-rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/src/pip_deepfreeze/sync.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/src/pip_deepfreeze/tree.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/src/pip_deepfreeze/utils.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/tests/test_env_info_json.py
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/tests/test_list_installed_depends.py
+-rw-r--r--   0        0        0    11678 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/tests/test_pip.py
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/tests/test_pip_list_json.py
+-rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/tests/test_project_name.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/tests/test_pyproject_options.py
+-rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/tests/test_req_file_parser.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/tests/test_req_merge.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/tests/test_req_parser.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/tests/test_sanity.py
+-rw-r--r--   0        0        0    10934 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/tests/test_sync.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/tests/test_tree.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0    17677 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/README.rst
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    19315 2020-02-02 00:00:00.000000 pip_deepfreeze-1.2.0/PKG-INFO
```

### Comparing `pip_deepfreeze-1.1.0/.pre-commit-config.yaml` & `pip_deepfreeze-1.2.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,26 @@
     ^src/pip_deepfreeze/req_file_parser.py|
     ^tests/conftest.py|
     ^tests/test_pip_list_json.py
 default_language_version:
   python: python3
 repos:
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.0.0
+    rev: v1.2.0
     hooks:
       - id: mypy
         args: ["--strict"]
         exclude: '^(docs|tasks|tests)|setup\.py'
         additional_dependencies: ["httpx", "packaging", "typer>=0.3.2", "types-toml", "types-setuptools"]
   - repo: https://github.com/PyCQA/flake8
     rev: "6.0.0"
@@ -32,15 +32,15 @@
       - id: flake8
         additional_dependencies: ["flake8-bugbear==23.1.20"]
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/PyCQA/docformatter
-    rev: v1.6.0.rc1
+    rev: v1.6.0
     hooks:
       - id: docformatter
         args: ["--in-place", "--wrap-summaries=88"]
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.3.1
     hooks:
       - id: pyupgrade
```

### Comparing `pip_deepfreeze-1.1.0/HISTORY.rst` & `pip_deepfreeze-1.2.0/HISTORY.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+1.2.0 (2023-04-10)
+==================
+
+Features
+--------
+
+- Don't show a stack trace when a post sync commands fails. (`#91 <https://github.com/sbidoul/pip-deepfreeze/issues/91>`_)
+
+
+Bugfixes
+--------
+
+- Avoid needlessly reinstalling Direct URL requirements that are not pinned exactly as pip
+  freeze does. (`#93 <https://github.com/sbidoul/pip-deepfreeze/issues/93>`_)
+
+
 1.1 (2023-02-12)
 ================
 
 Features
 --------
 
 - Read some configuration defaults from ``pyproject.toml``. (`#83 <https://github.com/sbidoul/pip-deepfreeze/issues/83>`_)
```

### Comparing `pip_deepfreeze-1.1.0/tox.ini` & `pip_deepfreeze-1.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/docs/logo.png` & `pip_deepfreeze-1.2.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/docs/logo.svg` & `pip_deepfreeze-1.2.0/docs/logo.svg`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/docs/synopsis.odg` & `pip_deepfreeze-1.2.0/docs/synopsis.odg`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/docs/synopsis.png` & `pip_deepfreeze-1.2.0/docs/synopsis.png`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/src/pip_deepfreeze/__main__.py` & `pip_deepfreeze-1.2.0/src/pip_deepfreeze/__main__.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/src/pip_deepfreeze/compat.py` & `pip_deepfreeze-1.2.0/src/pip_deepfreeze/compat.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/src/pip_deepfreeze/env_info_json.py` & `pip_deepfreeze-1.2.0/src/pip_deepfreeze/env_info_json.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/src/pip_deepfreeze/installed_dist.py` & `pip_deepfreeze-1.2.0/src/pip_deepfreeze/installed_dist.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/src/pip_deepfreeze/list_installed_depends.py` & `pip_deepfreeze-1.2.0/src/pip_deepfreeze/list_installed_depends.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/src/pip_deepfreeze/pip.py` & `pip_deepfreeze-1.2.0/src/pip_deepfreeze/pip.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,22 @@
 from .project_name import get_project_name
 from .req_file_parser import (
     NestedRequirementsLine,
     RequirementLine,
     parse as parse_req_file,
 )
 from .req_parser import get_req_name
-from .utils import check_call, check_output, log_debug, log_info, log_warning
+from .utils import (
+    check_call,
+    check_output,
+    log_debug,
+    log_info,
+    log_warning,
+    normalize_req_line,
+)
 
 
 def pip_upgrade_project(
     python: str,
     constraints_filename: Path,
     project_root: Path,
     extras: Optional[Sequence[NormalizedName]] = None,
@@ -29,15 +36,15 @@
 
     Make sure a project is installed with all its dependencies, and that all
     dependencies are at the latest version allowed by constraints.
 
     Ideally, this should be a native pip feature but
     - pip has difficulties upgrading direct URL requirements
       https://github.com/pypa/pip/issues/5780, https://github.com/pypa/pip/issues/7678
-      (need to check if the new resolver does the exepected thing).
+      (need to check if the new resolver does the expected thing).
     - We need to pass --upgrade for regular requirements otherwise pip will not attempt
       to install them (requirement already satisfied).
     - Passing --upgrade to pip makes it too slow to my taste (need to check performance
       with the new resolver).
 
     In the meantime, here is our upgrade algorithm:
     1. List installed dependencies of project (pip_freeze_dependencies).
@@ -55,18 +62,18 @@
     for req_line in parse_req_file(
         str(constraints_filename), recurse=False, reqs_only=False
     ):
         assert not isinstance(req_line, NestedRequirementsLine)
         if isinstance(req_line, RequirementLine):
             req_name = get_req_name(req_line.requirement)
             assert req_name  # XXX user error instead?
-            constraint_reqs[req_name] = req_line.requirement
+            constraint_reqs[req_name] = normalize_req_line(req_line.requirement)
     # 2. get installed frozen dependencies of project
     installed_reqs = {
-        get_req_name(req_line): req_line
+        get_req_name(req_line): normalize_req_line(req_line)
         for req_line in pip_freeze_dependencies(python, project_root, extras)[0]
     }
     assert all(installed_reqs.keys())  # XXX user error instead?
     # 3. uninstall dependencies that do not match constraints
     to_uninstall = set()
     for installed_req_name, installed_req in installed_reqs.items():
         assert installed_req_name
```

### Comparing `pip_deepfreeze-1.1.0/src/pip_deepfreeze/pip_list_json.py` & `pip_deepfreeze-1.2.0/src/pip_deepfreeze/pip_list_json.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/src/pip_deepfreeze/project_name.py` & `pip_deepfreeze-1.2.0/src/pip_deepfreeze/project_name.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/src/pip_deepfreeze/req_file_parser.py` & `pip_deepfreeze-1.2.0/src/pip_deepfreeze/req_file_parser.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/src/pip_deepfreeze/req_merge.py` & `pip_deepfreeze-1.2.0/src/pip_deepfreeze/req_merge.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/src/pip_deepfreeze/req_parser.py` & `pip_deepfreeze-1.2.0/src/pip_deepfreeze/req_parser.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/src/pip_deepfreeze/sanity.py` & `pip_deepfreeze-1.2.0/src/pip_deepfreeze/sanity.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/src/pip_deepfreeze/sync.py` & `pip_deepfreeze-1.2.0/src/pip_deepfreeze/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,8 +122,12 @@
                 f"The following distributions "
                 f"that are not dependencies of {project_name_with_extras} "
                 f"are also installed: {unneeded_reqs_str}"
             )
     # run post-sync commands
     for command in post_sync_commands:
         log_info(f"Running post-sync command: {command}")
-        subprocess.run(command, shell=True, check=True)
+        result = subprocess.run(command, shell=True, check=False)
+        if result.returncode != 0:
+            raise SystemExit(
+                f"Post-sync command {command} failed with exit code {result.returncode}"
+            )
```

### Comparing `pip_deepfreeze-1.1.0/src/pip_deepfreeze/tree.py` & `pip_deepfreeze-1.2.0/src/pip_deepfreeze/tree.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/src/pip_deepfreeze/utils.py` & `pip_deepfreeze-1.2.0/src/pip_deepfreeze/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import contextlib
+import re
 import subprocess
 from pathlib import Path
 from subprocess import CalledProcessError
 from typing import IO, Any, Dict, Iterable, Iterator, List, Optional, Sequence, Union
 
 import typer
 
@@ -112,7 +113,25 @@
 def make_project_name_with_extras(
     project_name: str, extras: Optional[Iterable[str]]
 ) -> str:
     if not extras:
         return project_name
     else:
         return project_name + "[" + ",".join(extras) + "]"
+
+
+_NORMALIZE_REQ_LINE_RE = re.compile(
+    r"^(?P<name>[a-zA-Z0-9-_.\[\]]+)(?P<arobas>\s*@\s*)(?P<rest>.*)$"
+)
+
+
+def normalize_req_line(req_line: str) -> str:
+    """Normalize a requirement line so they are comparable.
+
+    This is a little hack because some requirements.txt generator such
+    as pip-requirements-parser dont always generate the exact same
+    output as pip freeze.
+    """
+    mo = _NORMALIZE_REQ_LINE_RE.match(req_line)
+    if not mo:
+        return req_line
+    return mo.group("name") + " @ " + mo.group("rest")
```

### Comparing `pip_deepfreeze-1.1.0/tests/conftest.py` & `pip_deepfreeze-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/tests/test_env_info_json.py` & `pip_deepfreeze-1.2.0/tests/test_env_info_json.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/tests/test_list_installed_depends.py` & `pip_deepfreeze-1.2.0/tests/test_list_installed_depends.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/tests/test_pip.py` & `pip_deepfreeze-1.2.0/tests/test_pip.py`

 * *Files 9% similar despite different names*

```diff
@@ -263,15 +263,15 @@
         )
     )
     constraints.write_text(f"--no-index\n--find-links {testpkgs}\npkgc==0.0.1")
     pip_upgrade_project(virtualenv_python, constraints, project_root=tmp_path)
     assert list(_freeze_filter(pip_freeze(virtualenv_python))) == []
 
 
-def test_pip_upgrade_vcs_url(virtualenv_python, tmp_path):
+def test_pip_upgrade_vcs_url(virtualenv_python, tmp_path, capfd):
     """Test upgrading a VCS URL."""
     constraints = tmp_path / "requirements.txt.df"
     (tmp_path / "setup.py").write_text(
         textwrap.dedent(
             """
             from setuptools import setup
 
@@ -285,14 +285,26 @@
     # install tag 0.10.0
     constraints.write_text("--no-index\ntoml @ git+https://github.com/uiri/toml@0.10.0")
     pip_upgrade_project(virtualenv_python, constraints, project_root=tmp_path)
     assert list(_freeze_filter(pip_freeze(virtualenv_python))) == [
         "toml @ git+https://github.com/uiri/toml"
         "@4935f616ef78c35a968b2473e806d7049eba9af1"
     ]
+    assert "Uninstalling dependencies to update" not in capfd.readouterr().err
+    # reinstall, no change but different @url syntax
+    constraints.write_text(
+        "--no-index\n"
+        "toml@git+https://github.com/uiri/toml@4935f616ef78c35a968b2473e806d7049eba9af1"
+    )
+    pip_upgrade_project(virtualenv_python, constraints, project_root=tmp_path)
+    assert list(_freeze_filter(pip_freeze(virtualenv_python))) == [
+        "toml @ git+https://github.com/uiri/toml"
+        "@4935f616ef78c35a968b2473e806d7049eba9af1"
+    ]
+    assert "Uninstalling dependencies to update" not in capfd.readouterr().err
     # upgrade to tag 0.10.1
     constraints.write_text("toml @ git+https://github.com/uiri/toml@0.10.1")
     pip_upgrade_project(virtualenv_python, constraints, project_root=tmp_path)
     assert list(_freeze_filter(pip_freeze(virtualenv_python))) == [
         "toml @ git+https://github.com/uiri/toml"
         "@a86fc1fbd650a19eba313c3f642c9e2c679dc8d6"
     ]
```

### Comparing `pip_deepfreeze-1.1.0/tests/test_pip_list_json.py` & `pip_deepfreeze-1.2.0/tests/test_pip_list_json.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/tests/test_project_name.py` & `pip_deepfreeze-1.2.0/tests/test_project_name.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/tests/test_pyproject_options.py` & `pip_deepfreeze-1.2.0/tests/test_pyproject_options.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/tests/test_req_file_parser.py` & `pip_deepfreeze-1.2.0/tests/test_req_file_parser.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/tests/test_req_merge.py` & `pip_deepfreeze-1.2.0/tests/test_req_merge.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/tests/test_req_parser.py` & `pip_deepfreeze-1.2.0/tests/test_req_parser.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/tests/test_sanity.py` & `pip_deepfreeze-1.2.0/tests/test_sanity.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/tests/test_sync.py` & `pip_deepfreeze-1.2.0/tests/test_sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -357,7 +357,25 @@
         ],
         cwd=tmp_path,
         text=True,
         check=True,
         capture_output=True,
     )
     assert res.stdout.endswith("post-sync-cmd-1\npost-sync-cmd-2\n")
+    res = subprocess.run(
+        [
+            sys.executable,
+            "-m",
+            "pip_deepfreeze",
+            "--python",
+            virtualenv_python,
+            "sync",
+            "--post-sync-command",
+            "notacommand",
+        ],
+        cwd=tmp_path,
+        text=True,
+        check=False,
+        capture_output=True,
+    )
+    assert res.returncode != 0
+    assert "Post-sync command notacommand failed" in res.stderr
```

### Comparing `pip_deepfreeze-1.1.0/tests/test_tree.py` & `pip_deepfreeze-1.2.0/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/tests/test_utils.py` & `pip_deepfreeze-1.2.0/tests/test_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     increase_verbosity,
     log_debug,
     log_error,
     log_info,
     log_notice,
     log_warning,
     make_project_name_with_extras,
+    normalize_req_line,
     open_with_rollback,
 )
 
 
 def test_open_with_rollback(tmp_path):
     filename = tmp_path / "thefile"
     # file does not exist
@@ -128,7 +129,21 @@
         ("prj", [], "prj"),
         ("prj", ["e1"], "prj[e1]"),
         ("prj", ["e1", "e2"], "prj[e1,e2]"),
     ],
 )
 def test_make_project_name_with_extras(project_name, extras, expected):
     assert make_project_name_with_extras(project_name, extras) == expected
+
+
+@pytest.mark.parametrize(
+    "req_line, expected",
+    [
+        ("prj", "prj"),
+        ("prj==1.0", "prj==1.0"),
+        ("name @https://g.c/o/p@branch", "name @ https://g.c/o/p@branch"),
+        ("name@https://g.c/o/p@branch", "name @ https://g.c/o/p@branch"),
+        ("name[extra] @https://g.c/o/p@branch", "name[extra] @ https://g.c/o/p@branch"),
+    ],
+)
+def test_normalize_req_line(req_line: str, expected: str) -> None:
+    assert normalize_req_line(req_line) == expected
```

### Comparing `pip_deepfreeze-1.1.0/.gitignore` & `pip_deepfreeze-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/LICENSE.txt` & `pip_deepfreeze-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/README.rst` & `pip_deepfreeze-1.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -362,43 +362,45 @@
                           dependencies.
 
      --help               Show this message and exit.
 
 Configuration
 -------------
 
-Some options can get default values from a `[tool.pip-deepfreeze]` section of your
+Some options can get default values from a ``[tool.pip-deepfreeze]`` section of your
 ``pyproject.toml`` file. The following options are supported:
 
-- `sync.extras`: default value for the ``--extras`` option of the ``sync`` command.
-- `sync.post_sync_command`: default value (as a list of strings) for the
+- ``sync.extras``: default value for the ``--extras`` option of the ``sync`` command.
+- ``sync.post_sync_command``: default value (as a list of strings) for the
   ``--post-sync-command`` options of the ``sync`` command.
 
 Example:
 
-```toml
-[tool.pip-deepfreeze.sync]
-extras = "test,doc"
-post_sync_commands = ["cat requirements.txt", "python -m pip list"]
-```
+.. code:: toml
+
+   [tool.pip-deepfreeze.sync]
+   extras = "test,doc"
+   post_sync_commands = ["cat requirements.txt", "python -m pip list"]
 
 Other tools
 -----------
 
 Several other tools exist with a similar or overlapping scope as
 ``pip-deepfreeze``.
 
 - `pip <https://pip.pypa.io/en/stable/>`_ itself. ``pip-deepfreeze`` relies
   extensively on the ``pip`` CLI for installation and querying the database of
   installed distributions. In essence it is a thin wrapper around ``pip
   install`` and ``pip freeze``. Some of the features here may serve as
   inspiration for future ``pip`` evolutions.
 - `pip-tools <https://pypi.org/project/pip-tools/>`_. This is the one with the most
-  similar features. Besides the reasons explained in `About`_ above I wanted to see
-  if it was possible to do such a thing using the ``pip`` CLI only.
+  similar features. Besides the reasons explained in `About`_ above I wanted to see if
+  it was possible to do such a thing using the ``pip`` CLI only. ``pip-deepfreeze`` is
+  also more opinionated than ``pip-tools`` and ``pipdeptree``,  as it always does an
+  editable install and it uses the build backend to obtain the top level dependencies.
 - `PDM <https://pypi.org/project/pdm/>`_
 - `Poetry <https://python-poetry.org/>`_
 - `pipenv <https://pipenv.pypa.io/en/latest/>`_
 - `pipdeptree <https://pypi.org/project/pipdeptree/>`_. Works similarly as
   `pip-df tree`.
 
 Development
```

### Comparing `pip_deepfreeze-1.1.0/pyproject.toml` & `pip_deepfreeze-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pip_deepfreeze-1.1.0/PKG-INFO` & `pip_deepfreeze-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-deepfreeze
-Version: 1.1.0
+Version: 1.2.0
 Summary: A simple pip freeze workflow for Python application developers.
 Project-URL: Source, https://github.com/sbidoul/pip-deepfreeze/
 Project-URL: Bug Reports, https://github.com/sbidoul/pip-deepfreeze/issues
 Project-URL: Changelog, https://github.com/sbidoul/pip-deepfreeze/blob/master/HISTORY.rst
 Author-email: Stéphane Bidoul <stephane.bidoul@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -401,43 +401,45 @@
                           dependencies.
 
      --help               Show this message and exit.
 
 Configuration
 -------------
 
-Some options can get default values from a `[tool.pip-deepfreeze]` section of your
+Some options can get default values from a ``[tool.pip-deepfreeze]`` section of your
 ``pyproject.toml`` file. The following options are supported:
 
-- `sync.extras`: default value for the ``--extras`` option of the ``sync`` command.
-- `sync.post_sync_command`: default value (as a list of strings) for the
+- ``sync.extras``: default value for the ``--extras`` option of the ``sync`` command.
+- ``sync.post_sync_command``: default value (as a list of strings) for the
   ``--post-sync-command`` options of the ``sync`` command.
 
 Example:
 
-```toml
-[tool.pip-deepfreeze.sync]
-extras = "test,doc"
-post_sync_commands = ["cat requirements.txt", "python -m pip list"]
-```
+.. code:: toml
+
+   [tool.pip-deepfreeze.sync]
+   extras = "test,doc"
+   post_sync_commands = ["cat requirements.txt", "python -m pip list"]
 
 Other tools
 -----------
 
 Several other tools exist with a similar or overlapping scope as
 ``pip-deepfreeze``.
 
 - `pip <https://pip.pypa.io/en/stable/>`_ itself. ``pip-deepfreeze`` relies
   extensively on the ``pip`` CLI for installation and querying the database of
   installed distributions. In essence it is a thin wrapper around ``pip
   install`` and ``pip freeze``. Some of the features here may serve as
   inspiration for future ``pip`` evolutions.
 - `pip-tools <https://pypi.org/project/pip-tools/>`_. This is the one with the most
-  similar features. Besides the reasons explained in `About`_ above I wanted to see
-  if it was possible to do such a thing using the ``pip`` CLI only.
+  similar features. Besides the reasons explained in `About`_ above I wanted to see if
+  it was possible to do such a thing using the ``pip`` CLI only. ``pip-deepfreeze`` is
+  also more opinionated than ``pip-tools`` and ``pipdeptree``,  as it always does an
+  editable install and it uses the build backend to obtain the top level dependencies.
 - `PDM <https://pypi.org/project/pdm/>`_
 - `Poetry <https://python-poetry.org/>`_
 - `pipenv <https://pipenv.pypa.io/en/latest/>`_
 - `pipdeptree <https://pypi.org/project/pipdeptree/>`_. Works similarly as
   `pip-df tree`.
 
 Development
```


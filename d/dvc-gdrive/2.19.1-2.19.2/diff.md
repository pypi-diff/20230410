# Comparing `tmp/dvc-gdrive-2.19.1.tar.gz` & `tmp/dvc-gdrive-2.19.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-gdrive-2.19.1.tar", last modified: Tue Nov 15 12:26:13 2022, max compression
+gzip compressed data, was "dvc-gdrive-2.19.2.tar", last modified: Sun Apr  9 23:34:16 2023, max compression
```

## Comparing `dvc-gdrive-2.19.1.tar` & `dvc-gdrive-2.19.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-15 12:26:13.133904 dvc-gdrive-2.19.1/
--rw-r--r--   0 runner    (1001) docker     (116)      351 2022-11-15 12:26:00.000000 dvc-gdrive-2.19.1/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-15 12:26:13.125904 dvc-gdrive-2.19.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-15 12:26:13.129904 dvc-gdrive-2.19.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      587 2022-11-15 12:26:00.000000 dvc-gdrive-2.19.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     2730 2022-11-15 12:26:00.000000 dvc-gdrive-2.19.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      634 2022-11-15 12:26:00.000000 dvc-gdrive-2.19.1/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     1835 2022-11-15 12:26:00.000000 dvc-gdrive-2.19.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     1301 2022-11-15 12:26:00.000000 dvc-gdrive-2.19.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-11-15 12:26:00.000000 dvc-gdrive-2.19.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      705 2022-11-15 12:26:13.133904 dvc-gdrive-2.19.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       34 2022-11-15 12:26:00.000000 dvc-gdrive-2.19.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-15 12:26:13.129904 dvc-gdrive-2.19.1/dvc_gdrive/
--rw-r--r--   0 runner    (1001) docker     (116)     3789 2022-11-15 12:26:00.000000 dvc-gdrive-2.19.1/dvc_gdrive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      178 2022-11-15 12:26:13.000000 dvc-gdrive-2.19.1/dvc_gdrive/_dvc_gdrive_version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-15 12:26:13.133904 dvc-gdrive-2.19.1/dvc_gdrive/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-11-15 12:26:00.000000 dvc-gdrive-2.19.1/dvc_gdrive/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3457 2022-11-15 12:26:00.000000 dvc-gdrive-2.19.1/dvc_gdrive/tests/cloud.py
--rw-r--r--   0 runner    (1001) docker     (116)      170 2022-11-15 12:26:00.000000 dvc-gdrive-2.19.1/dvc_gdrive/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)       29 2022-11-15 12:26:00.000000 dvc-gdrive-2.19.1/dvc_gdrive/tests/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (116)      280 2022-11-15 12:26:00.000000 dvc-gdrive-2.19.1/dvc_gdrive/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (116)      296 2022-11-15 12:26:00.000000 dvc-gdrive-2.19.1/dvc_gdrive/tests/test_dvc.py
--rw-r--r--   0 runner    (1001) docker     (116)     1909 2022-11-15 12:26:00.000000 dvc-gdrive-2.19.1/dvc_gdrive/tests/test_fs.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-15 12:26:13.129904 dvc-gdrive-2.19.1/dvc_gdrive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      705 2022-11-15 12:26:13.000000 dvc-gdrive-2.19.1/dvc_gdrive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      663 2022-11-15 12:26:13.000000 dvc-gdrive-2.19.1/dvc_gdrive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-15 12:26:13.000000 dvc-gdrive-2.19.1/dvc_gdrive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-15 12:26:13.000000 dvc-gdrive-2.19.1/dvc_gdrive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      517 2022-11-15 12:26:13.000000 dvc-gdrive-2.19.1/dvc_gdrive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       11 2022-11-15 12:26:13.000000 dvc-gdrive-2.19.1/dvc_gdrive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2022-11-15 12:26:00.000000 dvc-gdrive-2.19.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)     1691 2022-11-15 12:26:13.133904 dvc-gdrive-2.19.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-11-15 12:26:00.000000 dvc-gdrive-2.19.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 23:34:16.077212 dvc-gdrive-2.19.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 23:34:16.069212 dvc-gdrive-2.19.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 23:34:16.073212 dvc-gdrive-2.19.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1835 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-04-09 23:34:16.077212 dvc-gdrive-2.19.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 23:34:16.073212 dvc-gdrive-2.19.2/dvc_gdrive/
+-rw-r--r--   0 runner    (1001) docker     (122)     3789 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/dvc_gdrive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-04-09 23:34:16.000000 dvc-gdrive-2.19.2/dvc_gdrive/_dvc_gdrive_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 23:34:16.077212 dvc-gdrive-2.19.2/dvc_gdrive/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/dvc_gdrive/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3457 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/dvc_gdrive/tests/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/dvc_gdrive/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/dvc_gdrive/tests/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      320 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/dvc_gdrive/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)      970 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/dvc_gdrive/tests/test_dvc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1909 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/dvc_gdrive/tests/test_fs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 23:34:16.077212 dvc-gdrive-2.19.2/dvc_gdrive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-04-09 23:34:16.000000 dvc-gdrive-2.19.2/dvc_gdrive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-09 23:34:16.000000 dvc-gdrive-2.19.2/dvc_gdrive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-09 23:34:16.000000 dvc-gdrive-2.19.2/dvc_gdrive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-09 23:34:16.000000 dvc-gdrive-2.19.2/dvc_gdrive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-04-09 23:34:16.000000 dvc-gdrive-2.19.2/dvc_gdrive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-09 23:34:16.000000 dvc-gdrive-2.19.2/dvc_gdrive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1552 2023-04-09 23:34:16.077212 dvc-gdrive-2.19.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-09 23:34:00.000000 dvc-gdrive-2.19.2/setup.py
```

### Comparing `dvc-gdrive-2.19.1/.github/workflows/tests.yaml` & `dvc-gdrive-2.19.2/.github/workflows/tests.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,65 @@
 name: Tests
 
 on:
-  pull_request: {}
-  push: {}
+  push:
+    branches: [main]
+  pull_request:
   schedule:
     - cron: '5 1 * * *'  # every day at 01:05
-
   workflow_dispatch:
 
-env:
-  DVC_TEST: "true"
-  HOMEBREW_NO_AUTO_UPDATE: 1
-  SHELL: /bin/bash
+concurrency:
+  group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
+  cancel-in-progress: true
+
+permissions:
+  contents: read
 
 jobs:
-  lint:
-    timeout-minutes: 10
-    runs-on: ubuntu-latest
-    steps:
-    - name: Cancel Previous Runs
-      uses: styfle/cancel-workflow-action@0.9.1
-      with:
-        access_token: ${{ github.token }}
-    - uses: actions/checkout@v2.4.0
-      with:
-        fetch-depth: 0
-    - name: Set up Python 3.8
-      uses: actions/setup-python@v2.2.2
-      with:
-        python-version: 3.8
-    - name: Install requirements
-      run: |
-        pip install wheel
-        pip install -e '.[tests]'
-        pip install git+https://github.com/iterative/dvc pre-commit
-    - name: Check README
-      run: python setup.py checkdocs
-    - uses: pre-commit/action@v2.0.3
   tests:
     timeout-minutes: 45
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-20.04, windows-latest, macos-latest]
-        pyv: ["3.8", "3.9", "3.10"]
-        exclude:
-          # no wheels for pygit2 yet
-          - os: windows-latest
-            pyv: "3.10"
+        pyv: ["3.8", "3.9", "3.10", "3.11"]
+
     steps:
-    - uses: actions/checkout@v2.4.0
+    - uses: actions/checkout@v3
       with:
         fetch-depth: 0
+
     - name: Set up Python
-      uses: actions/setup-python@v2.2.2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.pyv }}
-    - name: get pip cache dir
-      id: pip-cache-dir
-      run: |
-        echo "::set-output name=dir::$(pip cache dir)"
-    - name: set pip cache
-      id: pip-cache
-      uses: actions/cache@v2.1.6
-      with:
-        path: ${{ steps.pip-cache-dir.outputs.dir }}
-        key: ${{ runner.os }}-pip-${{ hashFiles('setup.cfg') }}
-        restore-keys: |
-          ${{ runner.os }}-pip-
+        cache: 'pip'
+        cache-dependency-path: setup.cfg
+
     - name: install
-      if: steps.cache.pip-cache-dir.cache-hit != 'true'
       run: |
-        pip install --upgrade pip setuptools wheel
+        pip install --upgrade pip wheel
         pip install -e ".[tests]"
-        pip install "dvc[testing]@git+https://github.com/iterative/dvc"
-    - name: setup git
-      run: |
-        git config --global user.email "dvctester@example.com"
-        git config --global user.name "DVC Tester"
+        pip install "dvc[testing] @ git+https://github.com/iterative/dvc"
+
     - name: install temporary dependencies
       run: |
         pip install git+https://github.com/efiop/gdrivefs@service-account
         pip install git+https://github.com/isidentical/pydata-google-auth@service-account
+
+    - name: lint
+      timeout-minutes: 10
+      uses: pre-commit/action@v3.0.0
+
     - name: run tests
-      timeout-minutes: 40
+      timeout-minutes: 15
       env:
         GDRIVE_CREDENTIALS_DATA: ${{ secrets.GDRIVE_CREDENTIALS_DATA }}
       run: pytest -v -n=auto --cov-report=xml --cov-report=term
+
     - name: upload coverage report
-      uses: codecov/codecov-action@v2.1.0
+      uses: codecov/codecov-action@v3
       with:
         file: ./coverage.xml
         fail_ci_if_error: false
```

### Comparing `dvc-gdrive-2.19.1/.github/workflows/update-template.yaml` & `dvc-gdrive-2.19.2/.github/workflows/update-template.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 name: Update template
 
 on:
   schedule:
     - cron: '5 1 * * *'  # every day at 01:05
-
   workflow_dispatch:
 
 jobs:
   update:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Install deps
       run: pip install cruft
     - name: Update template
       id: update
       run: |
         cruft update -y
         echo "::set-output name=changes::$(git diff)"
     - name: Create PR
       if: ${{ steps.update.outputs.changes != '' }}
       uses: peter-evans/create-pull-request@v3
       with:
         commit-message: update template
         title: update template
         token: ${{ secrets.WORKFLOW_TOKEN }}
-
```

### Comparing `dvc-gdrive-2.19.1/.gitignore` & `dvc-gdrive-2.19.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-gdrive-2.19.1/.pre-commit-config.yaml` & `dvc-gdrive-2.19.2/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,24 @@
           - ba,datas,fo,uptodate
     repo: https://github.com/codespell-project/codespell
     rev: v2.1.0
   - hooks:
       - id: isort
         language_version: python3
     repo: https://github.com/timothycrosley/isort
-    rev: 5.9.3
+    rev: 5.12.0
   - hooks:
       - id: flake8
         language_version: python3
         additional_dependencies:
           - flake8-bugbear
           - flake8-comprehensions
           - flake8-debugger
           - flake8-string-format
-    repo: https://gitlab.com/pycqa/flake8
+    repo: https://github.com/pycqa/flake8
     rev: 3.9.2
   - repo: local
     hooks:
     - id: mypy
       name: mypy
       entry: mypy
       files: ^dvc_gdrive/
```

### Comparing `dvc-gdrive-2.19.1/LICENSE` & `dvc-gdrive-2.19.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-gdrive-2.19.1/PKG-INFO` & `dvc-gdrive-2.19.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: dvc-gdrive
-Version: 2.19.1
+Version: 2.19.2
 Summary: gdrive plugin for dvc
 Home-page: http://dvc.org
 Download-URL: https://github.com/iterative/dvc-gdrive
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Source, https://github.com/iterative/dvc-gdrive
 Keywords: dvc,gdrive
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 License-File: LICENSE
 
 dvc-gdrive
```

### Comparing `dvc-gdrive-2.19.1/dvc_gdrive/__init__.py` & `dvc-gdrive-2.19.2/dvc_gdrive/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-gdrive-2.19.1/dvc_gdrive/tests/cloud.py` & `dvc-gdrive-2.19.2/dvc_gdrive/tests/cloud.py`

 * *Files identical despite different names*

### Comparing `dvc-gdrive-2.19.1/dvc_gdrive/tests/test_fs.py` & `dvc-gdrive-2.19.2/dvc_gdrive/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-gdrive-2.19.1/dvc_gdrive.egg-info/PKG-INFO` & `dvc-gdrive-2.19.2/dvc_gdrive.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: dvc-gdrive
-Version: 2.19.1
+Version: 2.19.2
 Summary: gdrive plugin for dvc
 Home-page: http://dvc.org
 Download-URL: https://github.com/iterative/dvc-gdrive
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Source, https://github.com/iterative/dvc-gdrive
 Keywords: dvc,gdrive
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 License-File: LICENSE
 
 dvc-gdrive
```

### Comparing `dvc-gdrive-2.19.1/dvc_gdrive.egg-info/SOURCES.txt` & `dvc-gdrive-2.19.2/dvc_gdrive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-gdrive-2.19.1/pyproject.toml` & `dvc-gdrive-2.19.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 [tool.pylint.master]
 extension-pkg-whitelist = ["pygit2"]
 init-hook = "import sys; sys.path.append(str('tests'))"
 load-plugins = ["pylint_pytest"]
 
 [tool.pylint.message_control]
 disable = [
-    "format", "refactoring", "spelling", "design", "no-self-use",
-    "invalid-name", "misplaced-comparison-constant", "duplicate-code", "fixme",
+    "format", "refactoring", "spelling", "design",
+    "invalid-name", "duplicate-code", "fixme",
     "unused-wildcard-import", "cyclic-import", "wrong-import-order",
     "wrong-import-position", "ungrouped-imports", "multiple-imports",
     "logging-format-interpolation", "logging-fstring-interpolation",
     "missing-function-docstring", "missing-module-docstring",
     "missing-class-docstring", "raise-missing-from", "import-outside-toplevel",
 ]
 enable = ["c-extension-no-member", "no-else-return"]
```

### Comparing `dvc-gdrive-2.19.1/setup.cfg` & `dvc-gdrive-2.19.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -13,26 +13,27 @@
 keywords = dvc, gdrive
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 setup_requires = 
 	setuptools>=48
 	setuptools_scm[toml]>=6.3.1
 python_requires = >=3.8
 zip_safe = False
 packages = find:
 include_package_data = True
 install_requires = 
 	dvc
-	pydrive2[fsspec]>=1.15.0
+	pydrive2[fsspec]>=1.15.3
 
 [options.extras_require]
 tests = 
 	wheel==0.37.0
 	dvc[testing]
 	pytest==6.2.5
 	pytest-cov==3.0.0
@@ -40,34 +41,33 @@
 	pytest-mock==3.6.1
 	pytest-lazy-fixture==0.6.3
 	pytest-docker==0.10.3
 	flaky==3.7.0
 	mock==4.0.3
 	wget==3.2
 	filelock==3.3.2
-	crc32c==2.2.post0
 	xmltodict==0.12.0
 	Pygments==2.10.0
 	collective.checkdocs==0.2
 	pydocstyle==6.1.1
-	pylint==2.11.1
+	pylint==2.16.2
 	pylint-pytest==1.1.2
 	pylint-plugin-utils==0.6
-	mypy==0.910
+	mypy==0.981
 	types-requests==2.25.11
 	types-tabulate==0.8.3
 	types-toml==0.10.1
 	pywin32>=225; sys_platform == 'win32'
 
 [flake8]
 ignore = 
-	E203, # Whitespace before ':'
-	E266, # Too many leading '#' for block comment
-	W503, # Line break occurred before a binary operator
-	P1,  # unindexed parameters in the str.format, see:
+	E203,
+	E266,
+	W503,
+	P1,
 max_line_length = 79
 max-complexity = 15
 select = B,C,E,F,W,T4,B902,T,P
 show_source = true
 count = true
 
 [egg_info]
```


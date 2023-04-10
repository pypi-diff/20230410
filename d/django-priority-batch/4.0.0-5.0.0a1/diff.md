# Comparing `tmp/django-priority-batch-4.0.0.tar.gz` & `tmp/django-priority-batch-5.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-priority-batch-4.0.0.tar", last modified: Fri Feb 18 07:28:24 2022, max compression
+gzip compressed data, was "django-priority-batch-5.0.0a1.tar", last modified: Mon Apr 10 17:16:33 2023, max compression
```

## Comparing `django-priority-batch-4.0.0.tar` & `django-priority-batch-5.0.0a1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 07:28:24.109872 django-priority-batch-4.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 07:28:24.105872 django-priority-batch-4.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 07:28:24.109872 django-priority-batch-4.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2136 2022-02-18 07:28:13.000000 django-priority-batch-4.0.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-02-18 07:28:13.000000 django-priority-batch-4.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-02-18 07:28:13.000000 django-priority-batch-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-02-18 07:28:13.000000 django-priority-batch-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3492 2022-02-18 07:28:24.109872 django-priority-batch-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2308 2022-02-18 07:28:13.000000 django-priority-batch-4.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 07:28:24.109872 django-priority-batch-4.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-02-18 07:28:13.000000 django-priority-batch-4.0.0/docs/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2235 2022-02-18 07:28:13.000000 django-priority-batch-4.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-02-18 07:28:13.000000 django-priority-batch-4.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-02-18 07:28:13.000000 django-priority-batch-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-18 07:28:24.109872 django-priority-batch-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-02-18 07:28:13.000000 django-priority-batch-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 07:28:24.105872 django-priority-batch-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 07:28:24.109872 django-priority-batch-4.0.0/src/django_priority_batch/
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-02-18 07:28:13.000000 django-priority-batch-4.0.0/src/django_priority_batch/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-02-18 07:28:13.000000 django-priority-batch-4.0.0/src/django_priority_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-02-18 07:28:13.000000 django-priority-batch-4.0.0/src/django_priority_batch/middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)     3534 2022-02-18 07:28:13.000000 django-priority-batch-4.0.0/src/django_priority_batch/prioritized_batcher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 07:28:24.109872 django-priority-batch-4.0.0/src/django_priority_batch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3492 2022-02-18 07:28:23.000000 django-priority-batch-4.0.0/src/django_priority_batch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-02-18 07:28:24.000000 django-priority-batch-4.0.0/src/django_priority_batch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-18 07:28:23.000000 django-priority-batch-4.0.0/src/django_priority_batch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-02-18 07:28:24.000000 django-priority-batch-4.0.0/src/django_priority_batch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-02-18 07:28:24.000000 django-priority-batch-4.0.0/src/django_priority_batch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 07:28:24.109872 django-priority-batch-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-02-18 07:28:13.000000 django-priority-batch-4.0.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2562 2022-02-18 07:28:13.000000 django-priority-batch-4.0.0/tests/test_prioritized_batcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     1949 2022-02-18 07:28:13.000000 django-priority-batch-4.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:16:33.952049 django-priority-batch-5.0.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:16:33.948048 django-priority-batch-5.0.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:16:33.948048 django-priority-batch-5.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-10 17:16:19.000000 django-priority-batch-5.0.0a1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-10 17:16:19.000000 django-priority-batch-5.0.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-10 17:16:19.000000 django-priority-batch-5.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-10 17:16:19.000000 django-priority-batch-5.0.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-10 17:16:33.952049 django-priority-batch-5.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-10 17:16:19.000000 django-priority-batch-5.0.0a1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:16:33.948048 django-priority-batch-5.0.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-10 17:16:19.000000 django-priority-batch-5.0.0a1/docs/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-10 17:16:19.000000 django-priority-batch-5.0.0a1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-10 17:16:19.000000 django-priority-batch-5.0.0a1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-10 17:16:19.000000 django-priority-batch-5.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 17:16:33.952049 django-priority-batch-5.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-10 17:16:19.000000 django-priority-batch-5.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:16:33.948048 django-priority-batch-5.0.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:16:33.952049 django-priority-batch-5.0.0a1/src/django_priority_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-10 17:16:19.000000 django-priority-batch-5.0.0a1/src/django_priority_batch/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-10 17:16:19.000000 django-priority-batch-5.0.0a1/src/django_priority_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-10 17:16:19.000000 django-priority-batch-5.0.0a1/src/django_priority_batch/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-10 17:16:19.000000 django-priority-batch-5.0.0a1/src/django_priority_batch/prioritized_batcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:16:33.952049 django-priority-batch-5.0.0a1/src/django_priority_batch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-10 17:16:33.000000 django-priority-batch-5.0.0a1/src/django_priority_batch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-10 17:16:33.000000 django-priority-batch-5.0.0a1/src/django_priority_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:16:33.000000 django-priority-batch-5.0.0a1/src/django_priority_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-10 17:16:33.000000 django-priority-batch-5.0.0a1/src/django_priority_batch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 17:16:33.000000 django-priority-batch-5.0.0a1/src/django_priority_batch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:16:33.952049 django-priority-batch-5.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-10 17:16:19.000000 django-priority-batch-5.0.0a1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-10 17:16:19.000000 django-priority-batch-5.0.0a1/tests/test_prioritized_batcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-10 17:16:19.000000 django-priority-batch-5.0.0a1/tox.ini
```

### Comparing `django-priority-batch-4.0.0/.github/workflows/ci.yml` & `django-priority-batch-5.0.0a1/.github/workflows/ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -9,36 +9,34 @@
   pull_request:
   schedule:
     - cron: "30 2 * * *"
   workflow_dispatch:
 
 jobs:
   test:
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     strategy:
       fail-fast: false
       matrix:
-        tox-env: [py36, py37, py38, py39, py310, linters, packaging, migrations]
+        tox-env: [py38, py39, py310, py311, linters, packaging, migrations]
         include:
-          - tox-env: py36
-            python-version: 3.6
-          - tox-env: py37
-            python-version: 3.7
           - tox-env: py38
             python-version: 3.8
           - tox-env: py39
             python-version: 3.9
           - tox-env: py310
             python-version: "3.10"
+          - tox-env: py311
+            python-version: "3.11"
           - tox-env: linters
-            python-version: "3.10"
+            python-version: "3.11"
           - tox-env: packaging
-            python-version: "3.10"
+            python-version: "3.11"
           - tox-env: migrations
-            python-version: "3.10"
+            python-version: "3.11"
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
@@ -46,32 +44,32 @@
         run: |
           python -m pip install --upgrade pip tox
       - name: Run Tests
         run: >
           tox -e ${{ matrix.tox-env }}
           --recreate
       - name: Upload coverage to Codecov
-        if: matrix.tox-env == 'py37' || matrix.tox-env == 'py38' || matrix.tox-env == 'py39' || matrix.tox-env == 'py310'
+        if: matrix.tox-env == 'py38' || matrix.tox-env == 'py39' || matrix.tox-env == 'py310' || matrix.tox-env == 'py311'
         uses: codecov/codecov-action@v1
         with:
           file: .coverage
 
   build:
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
 
     needs: test
 
     if: "startsWith(github.ref, 'refs/tags')"
 
     steps:
       - uses: actions/checkout@v1
-      - name: Set up Python 3.10
+      - name: Set up Python 3.11
         uses: actions/setup-python@v1
         with:
-          python-version: "3.10"
+          python-version: "3.11"
       - name: Install build
         run: python -m pip install --user build
       - name: Build a binary wheel and a source tarball
         run: python -m build --sdist --wheel --outdir dist/ .
       - name: Publish distribution to PyPI
         uses: pypa/gh-action-pypi-publish@master
         with:
```

### Comparing `django-priority-batch-4.0.0/LICENSE` & `django-priority-batch-5.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-priority-batch-4.0.0/PKG-INFO` & `django-priority-batch-5.0.0a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: django-priority-batch
-Version: 4.0.0
+Version: 5.0.0a1
 Summary: TODO.
 Home-page: https://github.com/genialis/django-priority-batch
 Author: Genialis, Inc.
 Author-email: dev-team@genialis.com
 License: Apache License (2.0)
 Keywords: django transaction batching prioritization
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6, <3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: package
 Provides-Extra: test
 License-File: LICENSE
 
 =====================
@@ -103,9 +101,7 @@
 
 
 Contribute
 ==========
 
 We welcome new contributors. Please, open a GitHub issue or contribute a pull
 request.
-
-
```

### Comparing `django-priority-batch-4.0.0/README.rst` & `django-priority-batch-5.0.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `django-priority-batch-4.0.0/docs/CHANGELOG.rst` & `django-priority-batch-5.0.0a1/docs/CHANGELOG.rst`

 * *Files 27% similar despite different names*

```diff
@@ -2,14 +2,26 @@
 Change Log
 ##########
 
 All notable changes to this project are documented in this file.
 This project adheres to `Semantic Versioning <http://semver.org/>`_.
 
 
+==================
+5.0.0 - 2023-04-09
+==================
+
+Changed
+=======
+- **BACKWARD INCOMPATIBLE:** Require ``Django 4.2``
+- Add support for ``Python 3.11``
+- Drop support for ``Python 3.6`` and ``Python 3.7``
+- Bump ``setuptools`` version
+
+
 ================
 4.0.0 2022-02-16
 ================
 
 Changed
 =======
 - **BACKWARD INCOMPATIBLE:** Drop support for Django 3.0 and 3.1
```

### Comparing `django-priority-batch-4.0.0/docs/conf.py` & `django-priority-batch-5.0.0a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-priority-batch-4.0.0/setup.py` & `django-priority-batch-5.0.0a1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     long_description_content_type='text/x-rst',
     author=about['__author__'],
     author_email=about['__email__'],
     url=about['__url__'],
     license=about['__license__'],
     packages=setuptools.find_packages('src'),
     package_dir={'': 'src'},
-    python_requires='>=3.6, <3.11',
-    install_requires=['Django~=3.2'],
+    python_requires='>=3.8, <3.12',
+    install_requires=['Django~=4.2'],
     extras_require={
         'docs': ['Sphinx', 'sphinx_rtd_theme'],
         'package': ['twine', 'wheel'],
         'test': [
             'black',
             'pydocstyle',
             'check-manifest',
@@ -48,15 +48,14 @@
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Application Frameworks',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     keywords='django transaction batching prioritization',
 )
```

### Comparing `django-priority-batch-4.0.0/src/django_priority_batch/__about__.py` & `django-priority-batch-5.0.0a1/src/django_priority_batch/__about__.py`

 * *Files identical despite different names*

### Comparing `django-priority-batch-4.0.0/src/django_priority_batch/middleware.py` & `django-priority-batch-5.0.0a1/src/django_priority_batch/middleware.py`

 * *Files identical despite different names*

### Comparing `django-priority-batch-4.0.0/src/django_priority_batch/prioritized_batcher.py` & `django-priority-batch-5.0.0a1/src/django_priority_batch/prioritized_batcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
     @classmethod
     def global_instance(cls):
         """Return a per-thread global batcher instance."""
         try:
             return GLOBAL_BATCHER.instance
         except AttributeError:
-
             instance = PrioritizedBatcher(
                 **getattr(settings, 'PRIORITIZED_BATCHER', {})
             )
             GLOBAL_BATCHER.instance = instance
             return instance
 
     @property
```

### Comparing `django-priority-batch-4.0.0/src/django_priority_batch.egg-info/PKG-INFO` & `django-priority-batch-5.0.0a1/src/django_priority_batch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: django-priority-batch
-Version: 4.0.0
+Version: 5.0.0a1
 Summary: TODO.
 Home-page: https://github.com/genialis/django-priority-batch
 Author: Genialis, Inc.
 Author-email: dev-team@genialis.com
 License: Apache License (2.0)
 Keywords: django transaction batching prioritization
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6, <3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: package
 Provides-Extra: test
 License-File: LICENSE
 
 =====================
@@ -103,9 +101,7 @@
 
 
 Contribute
 ==========
 
 We welcome new contributors. Please, open a GitHub issue or contribute a pull
 request.
-
-
```

### Comparing `django-priority-batch-4.0.0/src/django_priority_batch.egg-info/SOURCES.txt` & `django-priority-batch-5.0.0a1/src/django_priority_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-priority-batch-4.0.0/tests/test_prioritized_batcher.py` & `django-priority-batch-5.0.0a1/tests/test_prioritized_batcher.py`

 * *Files identical despite different names*

### Comparing `django-priority-batch-4.0.0/tox.ini` & `django-priority-batch-5.0.0a1/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -14,26 +14,25 @@
 # Use the default Python 3 version available on the system.
 # NOTE: This makes it portable to CI systems where only one particular Python 3
 # version is installed.
 basepython = python3
 
 [testenv]
 basepython =
-    py36: python3.6
-    py37: python3.7
     py38: python3.8
     py39: python3.9
     py310: python3.10
-    docs,linters,packaging,migrations: python3.10    
+    py311: python3.11
+    docs,linters,packaging,migrations: python3.11
 extras =
     docs: docs
     !docs: test
 setenv =
     # Enable pytest to find Django's setting module.
-    py{36,37,38,39,310}: PYTHONPATH={toxinidir}/tests
+    py{38,39,310,311}: PYTHONPATH={toxinidir}/tests
 ignore_errors =
     !linters: false
     # Run all linters to see their output even if one of them fails.
     linters: true
 
 commands_pre =
     # Verify installed packages have compatible dependencies.
@@ -42,15 +41,15 @@
     # broken installations.
     # For more details, see: https://github.com/pypa/pip/issues/988.
     pip check
 
 commands =
     # General tests commands:
     # Run tests.
-    py{36,37,38,39,310}: pytest
+    py{38,39,310,311}: pytest
 
     # Docs commands:
     # Build documentation.
     docs: python setup.py build_sphinx --fresh-env --warning-is-error
 
     # Linter commands:
     # Check code formatting.
```


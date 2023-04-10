# Comparing `tmp/essentials_configuration-2.0.1.tar.gz` & `tmp/essentials-configuration-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "essentials-configuration-2.0.2.tar", last modified: Mon Apr 10 11:40:27 2023, max compression
```

## Comparing `essentials_configuration-2.0.1.tar` & `essentials-configuration-2.0.2.tar`

### file list

```diff
@@ -1,30 +1,48 @@
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/CHANGELOG.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/MANIFEST.in
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/example.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/summary-ex.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/cli/__init__.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/cli/py.typed
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/common/__init__.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/common/files.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/common/py.typed
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/env/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/env/py.typed
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/errors/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/errors/py.typed
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/ini/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/ini/py.typed
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/json/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/json/py.typed
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/secrets/__init__.py
--rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/secrets/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/secrets/py.typed
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/toml/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/toml/py.typed
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/yaml/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/config/yaml/py.typed
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/LICENSE
--rw-r--r--   0        0        0    13126 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/README.md
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    14280 2020-02-02 00:00:00.000000 essentials_configuration-2.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.531860 essentials-configuration-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14082 2023-04-10 11:40:27.527860 essentials-configuration-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13126 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.519860 essentials-configuration-2.0.2/config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.523860 essentials-configuration-2.0.2/config/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/cli/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.523860 essentials-configuration-2.0.2/config/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/common/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.523860 essentials-configuration-2.0.2/config/env/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/env/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.523860 essentials-configuration-2.0.2/config/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/errors/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.523860 essentials-configuration-2.0.2/config/ini/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/ini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/ini/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.523860 essentials-configuration-2.0.2/config/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/json/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.523860 essentials-configuration-2.0.2/config/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/secrets/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/secrets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.527860 essentials-configuration-2.0.2/config/toml/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/toml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/toml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.527860 essentials-configuration-2.0.2/config/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/config/yaml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.527860 essentials-configuration-2.0.2/essentials_configuration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14082 2023-04-10 11:40:27.000000 essentials-configuration-2.0.2/essentials_configuration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-10 11:40:27.000000 essentials-configuration-2.0.2/essentials_configuration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 11:40:27.000000 essentials-configuration-2.0.2/essentials_configuration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-10 11:40:27.000000 essentials-configuration-2.0.2/essentials_configuration.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 11:40:27.000000 essentials-configuration-2.0.2/essentials_configuration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 11:40:27.000000 essentials-configuration-2.0.2/essentials_configuration.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 11:40:27.531860 essentials-configuration-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:40:27.527860 essentials-configuration-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-10 11:40:07.000000 essentials-configuration-2.0.2/tests/test_examples.py
```

### Comparing `essentials_configuration-2.0.1/config/common/__init__.py` & `essentials-configuration-2.0.2/config/common/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.1/config/common/files.py` & `essentials-configuration-2.0.2/config/common/files.py`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.1/config/env/__init__.py` & `essentials-configuration-2.0.2/config/env/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.1/config/ini/__init__.py` & `essentials-configuration-2.0.2/config/ini/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.1/config/secrets/__init__.py` & `essentials-configuration-2.0.2/config/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.1/config/secrets/cli.py` & `essentials-configuration-2.0.2/config/secrets/cli.py`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.1/config/toml/__init__.py` & `essentials-configuration-2.0.2/config/toml/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.1/config/yaml/__init__.py` & `essentials-configuration-2.0.2/config/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.1/LICENSE` & `essentials-configuration-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.1/README.md` & `essentials-configuration-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `essentials_configuration-2.0.1/pyproject.toml` & `essentials-configuration-2.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "essentials-configuration"
-version = "2.0.1"
+version = "2.0.2"
 authors = [{ name = "Roberto Prevato", email = "roberto.prevato@gmail.com" }]
 description = "Implementation of key-value pair based configuration for Python applications."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
@@ -26,30 +26,13 @@
 [project.optional-dependencies]
 yaml = ["PyYAML"]
 full = ["PyYAML", "click"]
 
 [project.scripts]
 config = "config.cli.main:main"
 
-[tool.hatch.build.targets.sdist]
-exclude = [
-    "/.github",
-    "/docs",
-    "/examples",
-    "/deps",
-    "/htmlcov",
-    "/tests",
-    "Makefile",
-    "CODE_OF_CONDUCT.md",
-    ".isort.cfg",
-    ".gitignore",
-    ".flake8",
-    "junit",
-    "requirements.txt",
-    "mypy.ini",
-    "pytest.ini",
-    "venv",
-]
+[tool.setuptools.package-data]
+config = ["*/py.typed"]
 
 [project.urls]
 "Homepage" = "https://github.com/Neoteroi/essentials-configuration"
 "Bug Tracker" = "https://github.com/Neoteroi/essentials-configuration/issues"
```

### Comparing `essentials_configuration-2.0.1/PKG-INFO` & `essentials-configuration-2.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 Metadata-Version: 2.1
 Name: essentials-configuration
-Version: 2.0.1
+Version: 2.0.2
 Summary: Implementation of key-value pair based configuration for Python applications.
+Author-email: Roberto Prevato <roberto.prevato@gmail.com>
 Project-URL: Homepage, https://github.com/Neoteroi/essentials-configuration
 Project-URL: Bug Tracker, https://github.com/Neoteroi/essentials-configuration/issues
-Author-email: Roberto Prevato <roberto.prevato@gmail.com>
-License-File: LICENSE
-Keywords: configuration,management,root,strategy
+Keywords: configuration,root,management,strategy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
-Requires-Dist: python-dotenv~=1.0.0
-Requires-Dist: tomli; python_version < '3.11'
-Provides-Extra: full
-Requires-Dist: click; extra == 'full'
-Requires-Dist: pyyaml; extra == 'full'
-Provides-Extra: yaml
-Requires-Dist: pyyaml; extra == 'yaml'
 Description-Content-Type: text/markdown
+Provides-Extra: yaml
+Provides-Extra: full
+License-File: LICENSE
 
 ![Build](https://github.com/Neoteroi/essentials-configuration/workflows/Build/badge.svg)
 [![pypi](https://img.shields.io/pypi/v/essentials-configuration.svg)](https://pypi.python.org/pypi/essentials-configuration)
 [![versions](https://img.shields.io/pypi/pyversions/essentials-configuration.svg)](https://github.com/Neoteroi/essentials-configuration)
 [![codecov](https://codecov.io/gh/Neoteroi/essentials-configuration/branch/main/graph/badge.svg?token=VzAnusWIZt)](https://codecov.io/gh/Neoteroi/essentials-configuration)
 [![license](https://img.shields.io/github/license/Neoteroi/essentials-configuration.svg)](https://github.com/Neoteroi/essentials-configuration/blob/main/LICENSE)
```


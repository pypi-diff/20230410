# Comparing `tmp/py-avro-schema-2.0.1.tar.gz` & `tmp/py-avro-schema-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-avro-schema-2.0.1.tar", last modified: Mon Mar  6 15:23:25 2023, max compression
+gzip compressed data, was "py-avro-schema-2.0.2.tar", last modified: Mon Apr 10 16:03:38 2023, max compression
```

## Comparing `py-avro-schema-2.0.1.tar` & `py-avro-schema-2.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:23:25.049813 py-avro-schema-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:23:25.041813 py-avro-schema-2.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:23:25.045813 py-avro-schema-2.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/.github/workflows/release-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/.github/workflows/test-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/LICENSE_HEADER.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-03-06 15:23:25.049813 py-avro-schema-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:23:25.045813 py-avro-schema-2.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/docs/py_avro_schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/docs/types.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 15:23:25.049813 py-avro-schema-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:23:25.041813 py-avro-schema-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:23:25.045813 py-avro-schema-2.0.1/src/py_avro_schema/
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/src/py_avro_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33004 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/src/py_avro_schema/_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/src/py_avro_schema/_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/src/py_avro_schema/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/src/py_avro_schema/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:23:25.049813 py-avro-schema-2.0.1/src/py_avro_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-03-06 15:23:25.000000 py-avro-schema-2.0.1/src/py_avro_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-06 15:23:25.000000 py-avro-schema-2.0.1/src/py_avro_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 15:23:25.000000 py-avro-schema-2.0.1/src/py_avro_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-06 15:23:25.000000 py-avro-schema-2.0.1/src/py_avro_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-06 15:23:25.000000 py-avro-schema-2.0.1/src/py_avro_schema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:23:25.049813 py-avro-schema-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/tests/test_avro_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/tests/test_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/tests/test_logicals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/tests/test_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/tests/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-03-06 15:23:13.000000 py-avro-schema-2.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:03:38.410587 py-avro-schema-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:03:38.406587 py-avro-schema-2.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:03:38.410587 py-avro-schema-2.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/.github/workflows/release-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/.github/workflows/test-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/LICENSE_HEADER.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-04-10 16:03:38.410587 py-avro-schema-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:03:38.410587 py-avro-schema-2.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/docs/py_avro_schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/docs/types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 16:03:38.414588 py-avro-schema-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:03:38.406587 py-avro-schema-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:03:38.410587 py-avro-schema-2.0.2/src/py_avro_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/src/py_avro_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33004 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/src/py_avro_schema/_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/src/py_avro_schema/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/src/py_avro_schema/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/src/py_avro_schema/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:03:38.410587 py-avro-schema-2.0.2/src/py_avro_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-04-10 16:03:38.000000 py-avro-schema-2.0.2/src/py_avro_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-10 16:03:38.000000 py-avro-schema-2.0.2/src/py_avro_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:03:38.000000 py-avro-schema-2.0.2/src/py_avro_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-10 16:03:38.000000 py-avro-schema-2.0.2/src/py_avro_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-10 16:03:38.000000 py-avro-schema-2.0.2/src/py_avro_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:03:38.410587 py-avro-schema-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/tests/test_avro_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/tests/test_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/tests/test_logicals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/tests/test_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/tests/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/tox.ini
```

### Comparing `py-avro-schema-2.0.1/.flake8` & `py-avro-schema-2.0.2/.flake8`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/.github/workflows/release-package.yml` & `py-avro-schema-2.0.2/.github/workflows/release-package.yml`

 * *Files 2% similar despite different names*

```diff
@@ -35,9 +35,9 @@
         python -m pip install build
     - name: Build package
       run: python -m build
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
-        password: ${{ secrets.PYPI_API_TOKEN }}
+        password: ${{ secrets.PYPI_API_JPMC_OSS }}
         print_hash: true
```

### Comparing `py-avro-schema-2.0.1/.github/workflows/test-package.yml` & `py-avro-schema-2.0.2/.github/workflows/test-package.yml`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/.gitignore` & `py-avro-schema-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/.pre-commit-config.yaml` & `py-avro-schema-2.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/LICENSE` & `py-avro-schema-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/LICENSE_HEADER.txt` & `py-avro-schema-2.0.2/LICENSE_HEADER.txt`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/PKG-INFO` & `py-avro-schema-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-avro-schema
-Version: 2.0.1
+Version: 2.0.2
 Summary: Generate Apache Avro schemas for Python types including standard library data-classes and Pydantic data models.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `py-avro-schema-2.0.1/README.md` & `py-avro-schema-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/docs/conf.py` & `py-avro-schema-2.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/docs/index.rst` & `py-avro-schema-2.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/docs/tutorial.rst` & `py-avro-schema-2.0.2/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/docs/types.rst` & `py-avro-schema-2.0.2/docs/types.rst`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/pyproject.toml` & `py-avro-schema-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/src/py_avro_schema/__init__.py` & `py-avro-schema-2.0.2/src/py_avro_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/src/py_avro_schema/_schemas.py` & `py-avro-schema-2.0.2/src/py_avro_schema/_schemas.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/src/py_avro_schema/_testing.py` & `py-avro-schema-2.0.2/src/py_avro_schema/_testing.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/src/py_avro_schema/_typing.py` & `py-avro-schema-2.0.2/src/py_avro_schema/_typing.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/src/py_avro_schema.egg-info/PKG-INFO` & `py-avro-schema-2.0.2/src/py_avro_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-avro-schema
-Version: 2.0.1
+Version: 2.0.2
 Summary: Generate Apache Avro schemas for Python types including standard library data-classes and Pydantic data models.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `py-avro-schema-2.0.1/src/py_avro_schema.egg-info/SOURCES.txt` & `py-avro-schema-2.0.2/src/py_avro_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/tests/test_avro_schema.py` & `py-avro-schema-2.0.2/tests/test_avro_schema.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/tests/test_dataclass.py` & `py-avro-schema-2.0.2/tests/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/tests/test_logicals.py` & `py-avro-schema-2.0.2/tests/test_logicals.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/tests/test_primitives.py` & `py-avro-schema-2.0.2/tests/test_primitives.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/tests/test_pydantic.py` & `py-avro-schema-2.0.2/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/tests/test_typing.py` & `py-avro-schema-2.0.2/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.1/tox.ini` & `py-avro-schema-2.0.2/tox.ini`

 * *Files identical despite different names*


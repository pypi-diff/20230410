# Comparing `tmp/tempora-5.2.1.tar.gz` & `tmp/tempora-5.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempora-5.2.1.tar", last modified: Thu Jan 19 03:03:45 2023, max compression
+gzip compressed data, was "tempora-5.2.2.tar", last modified: Mon Apr 10 14:47:19 2023, max compression
```

## Comparing `tempora-5.2.1.tar` & `tempora-5.2.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 03:03:45.306815 tempora-5.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-01-19 03:03:11.000000 tempora-5.2.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-01-19 03:03:11.000000 tempora-5.2.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-19 03:03:11.000000 tempora-5.2.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 03:03:45.302815 tempora-5.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-19 03:03:11.000000 tempora-5.2.1/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-01-19 03:03:11.000000 tempora-5.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 03:03:45.302815 tempora-5.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-01-19 03:03:11.000000 tempora-5.2.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-19 03:03:11.000000 tempora-5.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-19 03:03:11.000000 tempora-5.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-01-19 03:03:11.000000 tempora-5.2.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-01-19 03:03:11.000000 tempora-5.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-01-19 03:03:45.306815 tempora-5.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-01-19 03:03:11.000000 tempora-5.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-01-19 03:03:11.000000 tempora-5.2.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 03:03:45.302815 tempora-5.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-01-19 03:03:11.000000 tempora-5.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-19 03:03:11.000000 tempora-5.2.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-01-19 03:03:11.000000 tempora-5.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-01-19 03:03:11.000000 tempora-5.2.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-01-19 03:03:11.000000 tempora-5.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-01-19 03:03:11.000000 tempora-5.2.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-01-19 03:03:45.306815 tempora-5.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 03:03:45.302815 tempora-5.2.1/tempora/
--rw-r--r--   0 runner    (1001) docker     (123)    18182 2023-01-19 03:03:11.000000 tempora-5.2.1/tempora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-01-19 03:03:11.000000 tempora-5.2.1/tempora/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-01-19 03:03:11.000000 tempora-5.2.1/tempora/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-01-19 03:03:11.000000 tempora-5.2.1/tempora/utc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 03:03:45.306815 tempora-5.2.1/tempora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-01-19 03:03:45.000000 tempora-5.2.1/tempora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-01-19 03:03:45.000000 tempora-5.2.1/tempora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 03:03:45.000000 tempora-5.2.1/tempora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-19 03:03:45.000000 tempora-5.2.1/tempora.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-19 03:03:45.000000 tempora-5.2.1/tempora.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-19 03:03:45.000000 tempora-5.2.1/tempora.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 03:03:45.306815 tempora-5.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-01-19 03:03:11.000000 tempora-5.2.1/tests/test_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-01-19 03:03:11.000000 tempora-5.2.1/tests/test_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-01-19 03:03:11.000000 tempora-5.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:47:19.522996 tempora-5.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-10 14:46:59.000000 tempora-5.2.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 14:46:59.000000 tempora-5.2.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-10 14:46:59.000000 tempora-5.2.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:47:19.518996 tempora-5.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-10 14:46:59.000000 tempora-5.2.2/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-10 14:46:59.000000 tempora-5.2.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:47:19.518996 tempora-5.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-10 14:46:59.000000 tempora-5.2.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-10 14:46:59.000000 tempora-5.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-10 14:46:59.000000 tempora-5.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-10 14:46:59.000000 tempora-5.2.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-10 14:46:59.000000 tempora-5.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-10 14:47:19.522996 tempora-5.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-10 14:46:59.000000 tempora-5.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-10 14:46:59.000000 tempora-5.2.2/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:47:19.518996 tempora-5.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-10 14:46:59.000000 tempora-5.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-10 14:46:59.000000 tempora-5.2.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-10 14:46:59.000000 tempora-5.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-10 14:46:59.000000 tempora-5.2.2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-10 14:46:59.000000 tempora-5.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-10 14:46:59.000000 tempora-5.2.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-10 14:47:19.522996 tempora-5.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:47:19.518996 tempora-5.2.2/tempora/
+-rw-r--r--   0 runner    (1001) docker     (123)    18208 2023-04-10 14:46:59.000000 tempora-5.2.2/tempora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-04-10 14:46:59.000000 tempora-5.2.2/tempora/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-04-10 14:46:59.000000 tempora-5.2.2/tempora/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-10 14:46:59.000000 tempora-5.2.2/tempora/utc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:47:19.522996 tempora-5.2.2/tempora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-10 14:47:19.000000 tempora-5.2.2/tempora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-10 14:47:19.000000 tempora-5.2.2/tempora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 14:47:19.000000 tempora-5.2.2/tempora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-10 14:47:19.000000 tempora-5.2.2/tempora.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-10 14:47:19.000000 tempora-5.2.2/tempora.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 14:47:19.000000 tempora-5.2.2/tempora.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:47:19.522996 tempora-5.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-04-10 14:46:59.000000 tempora-5.2.2/tests/test_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-10 14:46:59.000000 tempora-5.2.2/tests/test_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-10 14:46:59.000000 tempora-5.2.2/tox.ini
```

### Comparing `tempora-5.2.1/.github/workflows/main.yml` & `tempora-5.2.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `tempora-5.2.1/CHANGES.rst` & `tempora-5.2.2/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v5.2.2
+======
+
+#22: Fixed bug in tests that would fail when a leap year
+was about a year away.
+
 v5.2.1
 ======
 
 #21: Restored dependency on ``jaraco.functools``, still
 used in timing module.
 
 v5.2.0
```

### Comparing `tempora-5.2.1/LICENSE` & `tempora-5.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tempora-5.2.1/PKG-INFO` & `tempora-5.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempora
-Version: 5.2.1
+Version: 5.2.2
 Summary: Objects and routines pertaining to date and time (tempora)
 Home-page: https://github.com/jaraco/tempora
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tempora-5.2.1/README.rst` & `tempora-5.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `tempora-5.2.1/docs/conf.py` & `tempora-5.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tempora-5.2.1/docs/index.rst` & `tempora-5.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tempora-5.2.1/pytest.ini` & `tempora-5.2.2/pytest.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 [pytest]
 norecursedirs=dist build .tox .eggs
 addopts=--doctest-modules
 filterwarnings=
+	## upstream
+
 	# Ensure ResourceWarnings are emitted
 	default::ResourceWarning
 
 	# Suppress deprecation warning in flake8
 	ignore:SelectableGroups dict interface is deprecated::flake8
 
 	# shopkeep/pytest-black#55
@@ -14,9 +16,20 @@
 	ignore:BlackItem is an Item subclass and should not be a collector:pytest.PytestWarning
 
 	# tholo/pytest-flake8#83
 	ignore:<class 'pytest_flake8.Flake8Item'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
 	ignore:The \(fspath. py.path.local\) argument to Flake8Item is deprecated.:pytest.PytestDeprecationWarning
 	ignore:Flake8Item is an Item subclass and should not be a collector:pytest.PytestWarning
 
+	# shopkeep/pytest-black#67
+	ignore:'encoding' argument not specified::pytest_black
+
+	# realpython/pytest-mypy#152
+	ignore:'encoding' argument not specified::pytest_mypy
+
+	# python/cpython#100750
+	ignore:'encoding' argument not specified::platform
+
+	## end upstream
+	
 	# ktosiek/pytest-freezegun#35
 	ignore:distutils Version classes are deprecated:DeprecationWarning
```

### Comparing `tempora-5.2.1/setup.cfg` & `tempora-5.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `tempora-5.2.1/tempora/__init__.py` & `tempora-5.2.2/tempora/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,17 +379,17 @@
 
     >>> parse_timedelta('1 year, 1 month')
     datetime.timedelta(days=395, seconds=58685)
 
     Note that months and years strict intervals, not aligned
     to a calendar:
 
-    >>> now = datetime.datetime.now()
-    >>> later = now + parse_timedelta('1 year')
-    >>> diff = later.replace(year=now.year) - now
+    >>> date = datetime.datetime.fromisoformat('2000-01-01')
+    >>> later = date + parse_timedelta('1 year')
+    >>> diff = later.replace(year=date.year) - date
     >>> diff.seconds
     20940
 
     >>> parse_timedelta('foo')
     Traceback (most recent call last):
     ...
     ValueError: Unexpected 'foo'
```

### Comparing `tempora-5.2.1/tempora/schedule.py` & `tempora-5.2.2/tempora/schedule.py`

 * *Files identical despite different names*

### Comparing `tempora-5.2.1/tempora/timing.py` & `tempora-5.2.2/tempora/timing.py`

 * *Files identical despite different names*

### Comparing `tempora-5.2.1/tempora/utc.py` & `tempora-5.2.2/tempora/utc.py`

 * *Files identical despite different names*

### Comparing `tempora-5.2.1/tempora.egg-info/PKG-INFO` & `tempora-5.2.2/tempora.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempora
-Version: 5.2.1
+Version: 5.2.2
 Summary: Objects and routines pertaining to date and time (tempora)
 Home-page: https://github.com/jaraco/tempora
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tempora-5.2.1/tempora.egg-info/SOURCES.txt` & `tempora-5.2.2/tempora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tempora-5.2.1/tests/test_schedule.py` & `tempora-5.2.2/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `tempora-5.2.1/tests/test_timing.py` & `tempora-5.2.2/tests/test_timing.py`

 * *Files identical despite different names*


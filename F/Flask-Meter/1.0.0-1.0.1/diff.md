# Comparing `tmp/Flask-Meter-1.0.0.tar.gz` & `tmp/Flask-Meter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Meter-1.0.0.tar", last modified: Mon Apr 10 14:07:10 2023, max compression
+gzip compressed data, was "Flask-Meter-1.0.1.tar", last modified: Mon Apr 10 14:29:54 2023, max compression
```

## Comparing `Flask-Meter-1.0.0.tar` & `Flask-Meter-1.0.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:07:10.532392 Flask-Meter-1.0.0/
--rw-rw-r--   0 herman    (1000) herman    (1000)      156 2023-04-10 07:49:10.000000 Flask-Meter-1.0.0/AUTHORS.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     3267 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)      313 2023-04-10 06:49:10.000000 Flask-Meter-1.0.0/HISTORY.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     1077 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/LICENSE
--rw-rw-r--   0 herman    (1000) herman    (1000)      264 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/MANIFEST.in
--rw-rw-r--   0 herman    (1000) herman    (1000)     3514 2023-04-10 14:07:10.532392 Flask-Meter-1.0.0/PKG-INFO
--rw-rw-r--   0 herman    (1000) herman    (1000)     2085 2023-04-10 13:44:14.000000 Flask-Meter-1.0.0/README.rst
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:07:10.532392 Flask-Meter-1.0.0/docs/
--rw-rw-r--   0 herman    (1000) herman    (1000)     6782 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/docs/Makefile
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:07:10.524392 Flask-Meter-1.0.0/docs/_build/
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:07:10.524392 Flask-Meter-1.0.0/docs/_build/html/
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:07:10.532392 Flask-Meter-1.0.0/docs/_build/html/_static/
--rw-rw-r--   0 herman    (1000) herman    (1000)      286 2023-04-10 12:45:48.000000 Flask-Meter-1.0.0/docs/_build/html/_static/file.png
--rw-rw-r--   0 herman    (1000) herman    (1000)       90 2023-04-10 12:45:48.000000 Flask-Meter-1.0.0/docs/_build/html/_static/minus.png
--rw-rw-r--   0 herman    (1000) herman    (1000)       90 2023-04-10 12:45:48.000000 Flask-Meter-1.0.0/docs/_build/html/_static/plus.png
--rw-rw-r--   0 herman    (1000) herman    (1000)       28 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/docs/authors.rst
--rwxrwxr-x   0 herman    (1000) herman    (1000)     8585 2023-04-10 13:26:44.000000 Flask-Meter-1.0.0/docs/conf.py
--rw-rw-r--   0 herman    (1000) herman    (1000)       33 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/docs/contributing.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)      479 2023-04-10 14:06:54.000000 Flask-Meter-1.0.0/docs/flask_meter.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)       28 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/docs/history.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)      298 2023-04-10 11:47:36.000000 Flask-Meter-1.0.0/docs/index.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     1147 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/docs/installation.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     6469 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/docs/make.bat
--rw-rw-r--   0 herman    (1000) herman    (1000)       70 2023-04-10 14:06:54.000000 Flask-Meter-1.0.0/docs/modules.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)       27 2023-04-10 06:09:30.000000 Flask-Meter-1.0.0/docs/readme.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)      420 2023-04-10 11:51:37.000000 Flask-Meter-1.0.0/docs/usage.rst
--rw-rw-r--   0 herman    (1000) herman    (1000)     1724 2023-04-10 14:06:24.000000 Flask-Meter-1.0.0/pyproject.toml
--rw-rw-r--   0 herman    (1000) herman    (1000)       69 2023-04-10 14:07:10.532392 Flask-Meter-1.0.0/setup.cfg
--rw-rw-r--   0 herman    (1000) herman    (1000)       38 2023-04-10 08:04:42.000000 Flask-Meter-1.0.0/setup.py
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:07:10.524392 Flask-Meter-1.0.0/src/
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:07:10.532392 Flask-Meter-1.0.0/src/Flask_Meter.egg-info/
--rw-rw-r--   0 herman    (1000) herman    (1000)     3514 2023-04-10 14:07:10.000000 Flask-Meter-1.0.0/src/Flask_Meter.egg-info/PKG-INFO
--rw-rw-r--   0 herman    (1000) herman    (1000)      713 2023-04-10 14:07:10.000000 Flask-Meter-1.0.0/src/Flask_Meter.egg-info/SOURCES.txt
--rw-rw-r--   0 herman    (1000) herman    (1000)        1 2023-04-10 14:07:10.000000 Flask-Meter-1.0.0/src/Flask_Meter.egg-info/dependency_links.txt
--rw-rw-r--   0 herman    (1000) herman    (1000)       12 2023-04-10 14:07:10.000000 Flask-Meter-1.0.0/src/Flask_Meter.egg-info/requires.txt
--rw-rw-r--   0 herman    (1000) herman    (1000)       12 2023-04-10 14:07:10.000000 Flask-Meter-1.0.0/src/Flask_Meter.egg-info/top_level.txt
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:07:10.532392 Flask-Meter-1.0.0/src/flask_meter/
--rw-rw-r--   0 herman    (1000) herman    (1000)      109 2023-04-10 13:09:47.000000 Flask-Meter-1.0.0/src/flask_meter/__init__.py
--rw-rw-r--   0 herman    (1000) herman    (1000)     1446 2023-04-10 13:09:59.000000 Flask-Meter-1.0.0/src/flask_meter/flask_meter.py
--rw-rw-r--   0 herman    (1000) herman    (1000)      742 2023-04-10 07:53:30.000000 Flask-Meter-1.0.0/src/flask_meter/git.py
-drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:07:10.532392 Flask-Meter-1.0.0/tests/
--rw-rw-r--   0 herman    (1000) herman    (1000)     2191 2023-04-10 13:12:53.000000 Flask-Meter-1.0.0/tests/test_flask_meter.py
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:29:54.984450 Flask-Meter-1.0.1/
+-rw-rw-r--   0 herman    (1000) herman    (1000)      156 2023-04-10 07:49:10.000000 Flask-Meter-1.0.1/AUTHORS.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     3267 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/CONTRIBUTING.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      372 2023-04-10 14:27:15.000000 Flask-Meter-1.0.1/HISTORY.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1077 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/LICENSE
+-rw-rw-r--   0 herman    (1000) herman    (1000)      264 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/MANIFEST.in
+-rw-rw-r--   0 herman    (1000) herman    (1000)     3514 2023-04-10 14:29:54.984450 Flask-Meter-1.0.1/PKG-INFO
+-rw-rw-r--   0 herman    (1000) herman    (1000)     2085 2023-04-10 14:24:39.000000 Flask-Meter-1.0.1/README.rst
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:29:54.984450 Flask-Meter-1.0.1/docs/
+-rw-rw-r--   0 herman    (1000) herman    (1000)     6782 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/docs/Makefile
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:29:54.980450 Flask-Meter-1.0.1/docs/_build/
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:29:54.980450 Flask-Meter-1.0.1/docs/_build/html/
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:29:54.984450 Flask-Meter-1.0.1/docs/_build/html/_static/
+-rw-rw-r--   0 herman    (1000) herman    (1000)      286 2023-04-10 12:45:48.000000 Flask-Meter-1.0.1/docs/_build/html/_static/file.png
+-rw-rw-r--   0 herman    (1000) herman    (1000)       90 2023-04-10 12:45:48.000000 Flask-Meter-1.0.1/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 herman    (1000) herman    (1000)       90 2023-04-10 12:45:48.000000 Flask-Meter-1.0.1/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 herman    (1000) herman    (1000)       28 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/docs/authors.rst
+-rwxrwxr-x   0 herman    (1000) herman    (1000)     8585 2023-04-10 13:26:44.000000 Flask-Meter-1.0.1/docs/conf.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)       33 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/docs/contributing.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      479 2023-04-10 14:06:54.000000 Flask-Meter-1.0.1/docs/flask_meter.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)       28 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/docs/history.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      298 2023-04-10 11:47:36.000000 Flask-Meter-1.0.1/docs/index.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1147 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/docs/installation.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     6469 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/docs/make.bat
+-rw-rw-r--   0 herman    (1000) herman    (1000)       70 2023-04-10 14:06:54.000000 Flask-Meter-1.0.1/docs/modules.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)       27 2023-04-10 06:09:30.000000 Flask-Meter-1.0.1/docs/readme.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)      420 2023-04-10 11:51:37.000000 Flask-Meter-1.0.1/docs/usage.rst
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1724 2023-04-10 14:06:24.000000 Flask-Meter-1.0.1/pyproject.toml
+-rw-rw-r--   0 herman    (1000) herman    (1000)       69 2023-04-10 14:29:54.984450 Flask-Meter-1.0.1/setup.cfg
+-rw-rw-r--   0 herman    (1000) herman    (1000)       38 2023-04-10 08:04:42.000000 Flask-Meter-1.0.1/setup.py
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:29:54.980450 Flask-Meter-1.0.1/src/
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:29:54.984450 Flask-Meter-1.0.1/src/Flask_Meter.egg-info/
+-rw-rw-r--   0 herman    (1000) herman    (1000)     3514 2023-04-10 14:29:54.000000 Flask-Meter-1.0.1/src/Flask_Meter.egg-info/PKG-INFO
+-rw-rw-r--   0 herman    (1000) herman    (1000)      713 2023-04-10 14:29:54.000000 Flask-Meter-1.0.1/src/Flask_Meter.egg-info/SOURCES.txt
+-rw-rw-r--   0 herman    (1000) herman    (1000)        1 2023-04-10 14:29:54.000000 Flask-Meter-1.0.1/src/Flask_Meter.egg-info/dependency_links.txt
+-rw-rw-r--   0 herman    (1000) herman    (1000)       12 2023-04-10 14:29:54.000000 Flask-Meter-1.0.1/src/Flask_Meter.egg-info/requires.txt
+-rw-rw-r--   0 herman    (1000) herman    (1000)       12 2023-04-10 14:29:54.000000 Flask-Meter-1.0.1/src/Flask_Meter.egg-info/top_level.txt
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:29:54.984450 Flask-Meter-1.0.1/src/flask_meter/
+-rw-rw-r--   0 herman    (1000) herman    (1000)      109 2023-04-10 14:26:51.000000 Flask-Meter-1.0.1/src/flask_meter/__init__.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)     1446 2023-04-10 13:09:59.000000 Flask-Meter-1.0.1/src/flask_meter/flask_meter.py
+-rw-rw-r--   0 herman    (1000) herman    (1000)      742 2023-04-10 07:53:30.000000 Flask-Meter-1.0.1/src/flask_meter/git.py
+drwxrwxr-x   0 herman    (1000) herman    (1000)        0 2023-04-10 14:29:54.984450 Flask-Meter-1.0.1/tests/
+-rw-rw-r--   0 herman    (1000) herman    (1000)     2191 2023-04-10 13:12:53.000000 Flask-Meter-1.0.1/tests/test_flask_meter.py
```

### Comparing `Flask-Meter-1.0.0/CONTRIBUTING.rst` & `Flask-Meter-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.0/LICENSE` & `Flask-Meter-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.0/PKG-INFO` & `Flask-Meter-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Meter
-Version: 1.0.0
+Version: 1.0.1
 Summary: Flask-Meter adds a healthcheck endpoint for Flask apps.
 Author-email: Herman Singh <kartstig@gmail.com>
 Maintainer-email: Herman Singh <kartstig@gmail.com>
 License: MIT License
 Project-URL: Donate, https://github.com/sponsors/Kartstig/dashboard
 Project-URL: Documentation, https://flask.palletsprojects.com/
 Project-URL: Source Code, https://github.com/Kartstig/flask-meter
@@ -37,16 +37,16 @@
 
 .. image:: https://img.shields.io/pypi/v/Flask-Meter.svg
         :target: https://pypi.python.org/pypi/Flask-Meter
 
 .. image:: https://tc.spin-flip.com/app/rest/builds/buildType:id:FlaskMeter_TestPython310/statusIcon.svg
         :target: https://tc.spin-flip.com/project/FlaskMeter?mode=trends
 
-.. image:: https://readthedocs.org/projects/Flask-Meter/badge/?version=latest
-        :target: https://Flask-Meter.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/flask-meter/badge/?version=latest
+        :target: https://flask-meter.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 .. image:: https://codecov.io/gh/Kartstig/flask-meter/branch/master/graph/badge.svg?token=NsmixA2iCH
         :target: https://codecov.io/gh/Kartstig/flask-meter
 
 Flask-Meter is an add-on to the Flask web framework. Flask-Meter adds a
 monitoring endpoint for consuming application metrics. It can be really simple
```

### Comparing `Flask-Meter-1.0.0/README.rst` & `Flask-Meter-1.0.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 .. image:: https://img.shields.io/pypi/v/Flask-Meter.svg
         :target: https://pypi.python.org/pypi/Flask-Meter
 
 .. image:: https://tc.spin-flip.com/app/rest/builds/buildType:id:FlaskMeter_TestPython310/statusIcon.svg
         :target: https://tc.spin-flip.com/project/FlaskMeter?mode=trends
 
-.. image:: https://readthedocs.org/projects/Flask-Meter/badge/?version=latest
-        :target: https://Flask-Meter.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/flask-meter/badge/?version=latest
+        :target: https://flask-meter.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 .. image:: https://codecov.io/gh/Kartstig/flask-meter/branch/master/graph/badge.svg?token=NsmixA2iCH
         :target: https://codecov.io/gh/Kartstig/flask-meter
 
 Flask-Meter is an add-on to the Flask web framework. Flask-Meter adds a
 monitoring endpoint for consuming application metrics. It can be really simple
```

### Comparing `Flask-Meter-1.0.0/docs/Makefile` & `Flask-Meter-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.0/docs/conf.py` & `Flask-Meter-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.0/docs/installation.rst` & `Flask-Meter-1.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.0/docs/make.bat` & `Flask-Meter-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.0/pyproject.toml` & `Flask-Meter-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.0/src/Flask_Meter.egg-info/PKG-INFO` & `Flask-Meter-1.0.1/src/Flask_Meter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Meter
-Version: 1.0.0
+Version: 1.0.1
 Summary: Flask-Meter adds a healthcheck endpoint for Flask apps.
 Author-email: Herman Singh <kartstig@gmail.com>
 Maintainer-email: Herman Singh <kartstig@gmail.com>
 License: MIT License
 Project-URL: Donate, https://github.com/sponsors/Kartstig/dashboard
 Project-URL: Documentation, https://flask.palletsprojects.com/
 Project-URL: Source Code, https://github.com/Kartstig/flask-meter
@@ -37,16 +37,16 @@
 
 .. image:: https://img.shields.io/pypi/v/Flask-Meter.svg
         :target: https://pypi.python.org/pypi/Flask-Meter
 
 .. image:: https://tc.spin-flip.com/app/rest/builds/buildType:id:FlaskMeter_TestPython310/statusIcon.svg
         :target: https://tc.spin-flip.com/project/FlaskMeter?mode=trends
 
-.. image:: https://readthedocs.org/projects/Flask-Meter/badge/?version=latest
-        :target: https://Flask-Meter.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/flask-meter/badge/?version=latest
+        :target: https://flask-meter.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 .. image:: https://codecov.io/gh/Kartstig/flask-meter/branch/master/graph/badge.svg?token=NsmixA2iCH
         :target: https://codecov.io/gh/Kartstig/flask-meter
 
 Flask-Meter is an add-on to the Flask web framework. Flask-Meter adds a
 monitoring endpoint for consuming application metrics. It can be really simple
```

### Comparing `Flask-Meter-1.0.0/src/Flask_Meter.egg-info/SOURCES.txt` & `Flask-Meter-1.0.1/src/Flask_Meter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.0/src/flask_meter/flask_meter.py` & `Flask-Meter-1.0.1/src/flask_meter/flask_meter.py`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.0/src/flask_meter/git.py` & `Flask-Meter-1.0.1/src/flask_meter/git.py`

 * *Files identical despite different names*

### Comparing `Flask-Meter-1.0.0/tests/test_flask_meter.py` & `Flask-Meter-1.0.1/tests/test_flask_meter.py`

 * *Files identical despite different names*


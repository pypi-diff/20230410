# Comparing `tmp/django-modeltree-0.4.tar.gz` & `tmp/django-modeltree-1.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-modeltree-0.4.tar", last modified: Mon Apr 10 19:17:49 2023, max compression
+gzip compressed data, was "/home/thomas/django/django-modeltree/dist/.tmp-xeyuirul/django-modeltree-1.0.dev0.tar", last modified: Sat Feb 25 08:34:49 2023, max compression
```

## Comparing `django-modeltree-0.4.tar` & `django-modeltree-1.0.dev0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-10 19:17:49.545133 django-modeltree-0.4/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1521 2023-02-19 13:54:19.000000 django-modeltree-0.4/LICENCE
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3136 2023-04-10 19:17:49.545133 django-modeltree-0.4/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1700 2023-04-10 15:11:54.000000 django-modeltree-0.4/README.rst
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-10 19:17:49.537133 django-modeltree-0.4/django_modeltree.egg-info/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3136 2023-04-10 19:17:49.000000 django-modeltree-0.4/django_modeltree.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2023-04-10 19:17:49.000000 django-modeltree-0.4/django_modeltree.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-04-10 19:17:49.000000 django-modeltree-0.4/django_modeltree.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       15 2023-04-10 19:17:49.000000 django-modeltree-0.4/django_modeltree.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       10 2023-04-10 19:17:49.000000 django-modeltree-0.4/django_modeltree.egg-info/top_level.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-02-21 19:31:30.000000 django-modeltree-0.4/django_modeltree.egg-info/zip-safe
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-10 19:17:49.541133 django-modeltree-0.4/modeltree/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       32 2023-02-25 14:44:43.000000 django-modeltree-0.4/modeltree/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      661 2023-04-10 19:12:39.000000 django-modeltree-0.4/modeltree/__version__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    21559 2023-04-10 19:11:23.000000 django-modeltree-0.4/modeltree/modeltree.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-04-10 19:17:49.545133 django-modeltree-0.4/setup.cfg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2308 2023-04-10 15:11:03.000000 django-modeltree-0.4/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-25 08:34:49.000000 django-modeltree-1.0.dev0/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1521 2023-02-19 13:54:19.000000 django-modeltree-1.0.dev0/LICENCE
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2447 2023-02-25 08:34:49.000000 django-modeltree-1.0.dev0/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1158 2023-02-19 22:33:34.000000 django-modeltree-1.0.dev0/README.rst
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-25 08:34:49.000000 django-modeltree-1.0.dev0/django_modeltree.egg-info/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2447 2023-02-25 08:34:49.000000 django-modeltree-1.0.dev0/django_modeltree.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2023-02-25 08:34:49.000000 django-modeltree-1.0.dev0/django_modeltree.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-02-25 08:34:49.000000 django-modeltree-1.0.dev0/django_modeltree.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       15 2023-02-25 08:34:49.000000 django-modeltree-1.0.dev0/django_modeltree.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       10 2023-02-25 08:34:49.000000 django-modeltree-1.0.dev0/django_modeltree.egg-info/top_level.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-02-21 19:31:30.000000 django-modeltree-1.0.dev0/django_modeltree.egg-info/zip-safe
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-25 08:34:49.000000 django-modeltree-1.0.dev0/modeltree/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       32 2023-02-19 20:12:52.000000 django-modeltree-1.0.dev0/modeltree/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      666 2023-02-19 22:29:43.000000 django-modeltree-1.0.dev0/modeltree/__version__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    13103 2023-02-25 00:06:19.000000 django-modeltree-1.0.dev0/modeltree/modeltree.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-02-25 08:34:49.000000 django-modeltree-1.0.dev0/setup.cfg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2170 2023-02-19 22:41:58.000000 django-modeltree-1.0.dev0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `django-modeltree-0.4/LICENCE` & `django-modeltree-1.0.dev0/LICENCE`

 * *Files identical despite different names*

### Comparing `django-modeltree-0.4/PKG-INFO` & `django-modeltree-1.0.dev0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,69 @@
 Metadata-Version: 2.1
 Name: django-modeltree
-Version: 0.4
+Version: 1.0.dev0
 Summary: TODO
 Home-page: https://github.com/thomst/django-modeltree
 Author: Thomas Leichtfuß
 Author-email: thomas.leichtfuss@posteo.de
 License: BSD License
 Platform: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
-Classifier: Framework :: Django :: 4.2
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 License-File: LICENCE
 
 ===========================
 Welcome to django-modeltree
 ===========================
 
-.. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue
-   :target: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue
-   :alt: python: 3.6, 3.7, 3.8, 3.9, 3.10, 3.11
-
-.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
-   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
-   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1, 4.2
+.. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :target: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :alt: python: 3.6, 3.7, 3.8, 3.9, 3.10
+
+.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
+   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
+   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1
 
 .. image:: https://github.com/thomst/django-modeltree/actions/workflows/ci.yml/badge.svg
    :target: https://github.com/thomst/django-modeltree/actions/workflows/ci.yml
    :alt: Run tests for django-modeltree
 
 .. image:: https://coveralls.io/repos/github/thomst/django-modeltree/badge.svg?branch=master
    :target: https://coveralls.io/github/thomst/django-modeltree?branch=master
    :alt: Coveralls
 
 
-About
-=====
-Do you have a model layout with various relations and looking for a way to
-navigate it with ease? Then django-modeltree is what you are looking for. Build
-your modeltree in a single line and accessing related models and their objects
-in a elegant and performant way. No need for complex query building anymore.
-Find out how this works `here <https://thomst.github.io/django-modeltree/>`_.
-
-
-Links
-=====
-
-* `Github <https://github.com/thomst/django-modeltree>`_
-* `Docs <https://thomst.github.io/django-modeltree/>`_
+Description
+===========
+TODO
 
 
 Installation
 ============
 Install from pypi.org::
 
     pip install django-modeltree
+
+
+Usage
+=====
+TODO
```

### Comparing `django-modeltree-0.4/django_modeltree.egg-info/PKG-INFO` & `django-modeltree-1.0.dev0/django_modeltree.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,69 @@
 Metadata-Version: 2.1
 Name: django-modeltree
-Version: 0.4
+Version: 1.0.dev0
 Summary: TODO
 Home-page: https://github.com/thomst/django-modeltree
 Author: Thomas Leichtfuß
 Author-email: thomas.leichtfuss@posteo.de
 License: BSD License
 Platform: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
-Classifier: Framework :: Django :: 4.2
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 License-File: LICENCE
 
 ===========================
 Welcome to django-modeltree
 ===========================
 
-.. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue
-   :target: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue
-   :alt: python: 3.6, 3.7, 3.8, 3.9, 3.10, 3.11
-
-.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
-   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1%20%7C%204.2-orange
-   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1, 4.2
+.. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :target: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :alt: python: 3.6, 3.7, 3.8, 3.9, 3.10
+
+.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
+   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
+   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1
 
 .. image:: https://github.com/thomst/django-modeltree/actions/workflows/ci.yml/badge.svg
    :target: https://github.com/thomst/django-modeltree/actions/workflows/ci.yml
    :alt: Run tests for django-modeltree
 
 .. image:: https://coveralls.io/repos/github/thomst/django-modeltree/badge.svg?branch=master
    :target: https://coveralls.io/github/thomst/django-modeltree?branch=master
    :alt: Coveralls
 
 
-About
-=====
-Do you have a model layout with various relations and looking for a way to
-navigate it with ease? Then django-modeltree is what you are looking for. Build
-your modeltree in a single line and accessing related models and their objects
-in a elegant and performant way. No need for complex query building anymore.
-Find out how this works `here <https://thomst.github.io/django-modeltree/>`_.
-
-
-Links
-=====
-
-* `Github <https://github.com/thomst/django-modeltree>`_
-* `Docs <https://thomst.github.io/django-modeltree/>`_
+Description
+===========
+TODO
 
 
 Installation
 ============
 Install from pypi.org::
 
     pip install django-modeltree
+
+
+Usage
+=====
+TODO
```

### Comparing `django-modeltree-0.4/modeltree/__version__.py` & `django-modeltree-1.0.dev0/modeltree/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 internal code changes that do not affect the API. Development versions are
 incomplete states of a release .
 
 Version 0.x should be considered a development version with an unstable API,
 and backwards compatibility is not guaranteed for minor versions.
 """
 
-__version__ = "0.4"
+__version__ = "1.0.dev0"
```

### Comparing `django-modeltree-0.4/setup.py` & `django-modeltree-1.0.dev0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,27 +49,24 @@
         "Framework :: Django",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
-        "Framework :: Django :: 4.2",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
     ],
     zip_safe=True,
 )
```


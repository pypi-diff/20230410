# Comparing `tmp/unexpectation_handler-1.0.1.tar.gz` & `tmp/unexpectation_handler-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unexpectation_handler-1.0.1.tar", max compression
+gzip compressed data, was "unexpectation_handler-1.0.2.tar", max compression
```

## Comparing `unexpectation_handler-1.0.1.tar` & `unexpectation_handler-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-04-09 12:55:40.014122 unexpectation_handler-1.0.1/LICENSE
--rw-r--r--   0        0        0      714 2023-04-10 00:35:29.984988 unexpectation_handler-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1131 2023-04-10 00:35:29.980894 unexpectation_handler-1.0.1/README.md
--rw-r--r--   0        0        0       84 2023-04-09 13:29:21.097465 unexpectation_handler-1.0.1/unexpectation_handler/__init__.py
--rw-r--r--   0        0        0     3179 2023-04-09 13:26:00.949837 unexpectation_handler-1.0.1/unexpectation_handler/handler.py
--rw-r--r--   0        0        0      636 2023-04-09 13:20:04.377684 unexpectation_handler-1.0.1/unexpectation_handler/symbol.py
--rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 unexpectation_handler-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-09 12:55:40.014122 unexpectation_handler-1.0.2/LICENSE
+-rw-r--r--   0        0        0      714 2023-04-10 00:50:04.002612 unexpectation_handler-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1131 2023-04-10 00:47:31.115752 unexpectation_handler-1.0.2/README.md
+-rw-r--r--   0        0        0       84 2023-04-09 13:29:21.097465 unexpectation_handler-1.0.2/unexpectation_handler/__init__.py
+-rw-r--r--   0        0        0     3179 2023-04-09 13:26:00.949837 unexpectation_handler-1.0.2/unexpectation_handler/handler.py
+-rw-r--r--   0        0        0      636 2023-04-09 13:20:04.377684 unexpectation_handler-1.0.2/unexpectation_handler/symbol.py
+-rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 unexpectation_handler-1.0.2/PKG-INFO
```

### Comparing `unexpectation_handler-1.0.1/LICENSE` & `unexpectation_handler-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unexpectation_handler-1.0.1/pyproject.toml` & `unexpectation_handler-1.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "unexpectation-handler"
-version = "1.0.1"
-description = "Never trust users! Encapsulate \"isolating program vulnerabilities (errors, exceptions, or results due to unexpected input) that may be caused by executed code\" and \"Calling function that handle them\" as a package of Python."
+version = "1.0.2"
+description = "Never trust users! Encapsulate \"isolating program vulnerabilities (errors, exceptions, or results due to unexpected input) that may be caused by executed code\" and \"calling function that handle them\" as a package of Python."
 license = "MIT"
 authors = ["leoweyr <leoweyr@foxmail.com>"]
 readme = "README.md"
 repository = "https://github.com/leoweyr/Python-Unexpectation_Handler"
 classifiers = [
     "Development Status :: 3 - Alpha"
 ]
```

### Comparing `unexpectation_handler-1.0.1/README.md` & `unexpectation_handler-1.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Unexpectation Handler
 [![PyPI Latest Release](https://img.shields.io/pypi/v/unexpectation-handler.svg)](https://pypi.org/project/unexpectation-handler/)
 [![Package Status](https://img.shields.io/pypi/status/unexpectation-handler.svg)](https://pypi.org/project/unexpectation-handler/)
 [![License](https://img.shields.io/pypi/l/unexpectation-handler.svg)](https://github.com/leoweyr/Python-Unexpectation_Handler/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/personalized-badge/unexpectation-handler?period=total&units=international_system&left_color=grey&right_color=green&left_text=pypi%20downloads)](https://pepy.tech/project/unexpectation-handler)
 
-Never trust users! Encapsulate "isolating program vulnerabilities (errors, exceptions, or results due to unexpected input) that may be caused by executed code" and "Calling function that handle them" as a package of Python.
+Never trust users! Encapsulate "isolating program vulnerabilities (errors, exceptions, or results due to unexpected input) that may be caused by executed code" and "calling function that handle them" as a package of Python.
 
 ## ⚖️License
 
 [MIT](https://github.com/leoweyr/Python-Unexpectation_Handler/blob/main/LICENSE)
 
 ## 📗Documentation
```

### Comparing `unexpectation_handler-1.0.1/unexpectation_handler/handler.py` & `unexpectation_handler-1.0.2/unexpectation_handler/handler.py`

 * *Files identical despite different names*

### Comparing `unexpectation_handler-1.0.1/unexpectation_handler/symbol.py` & `unexpectation_handler-1.0.2/unexpectation_handler/symbol.py`

 * *Files identical despite different names*

### Comparing `unexpectation_handler-1.0.1/PKG-INFO` & `unexpectation_handler-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: unexpectation-handler
-Version: 1.0.1
-Summary: Never trust users! Encapsulate "isolating program vulnerabilities (errors, exceptions, or results due to unexpected input) that may be caused by executed code" and "Calling function that handle them" as a package of Python.
+Version: 1.0.2
+Summary: Never trust users! Encapsulate "isolating program vulnerabilities (errors, exceptions, or results due to unexpected input) that may be caused by executed code" and "calling function that handle them" as a package of Python.
 Home-page: https://github.com/leoweyr/Python-Unexpectation_Handler
 License: MIT
 Author: leoweyr
 Author-email: leoweyr@foxmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,15 @@
 
 # Unexpectation Handler
 [![PyPI Latest Release](https://img.shields.io/pypi/v/unexpectation-handler.svg)](https://pypi.org/project/unexpectation-handler/)
 [![Package Status](https://img.shields.io/pypi/status/unexpectation-handler.svg)](https://pypi.org/project/unexpectation-handler/)
 [![License](https://img.shields.io/pypi/l/unexpectation-handler.svg)](https://github.com/leoweyr/Python-Unexpectation_Handler/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/personalized-badge/unexpectation-handler?period=total&units=international_system&left_color=grey&right_color=green&left_text=pypi%20downloads)](https://pepy.tech/project/unexpectation-handler)
 
-Never trust users! Encapsulate "isolating program vulnerabilities (errors, exceptions, or results due to unexpected input) that may be caused by executed code" and "Calling function that handle them" as a package of Python.
+Never trust users! Encapsulate "isolating program vulnerabilities (errors, exceptions, or results due to unexpected input) that may be caused by executed code" and "calling function that handle them" as a package of Python.
 
 ## ⚖️License
 
 [MIT](https://github.com/leoweyr/Python-Unexpectation_Handler/blob/main/LICENSE)
 
 ## 📗Documentation
```


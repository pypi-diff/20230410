# Comparing `tmp/printcleaner-0.1.5.tar.gz` & `tmp/printcleaner-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "printcleaner-0.1.5.tar", max compression
+gzip compressed data, was "printcleaner-0.1.6.tar", max compression
```

## Comparing `printcleaner-0.1.5.tar` & `printcleaner-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-03-10 16:54:33.946052 printcleaner-0.1.5/LICENSE
--rw-r--r--   0        0        0      588 2023-03-12 19:52:05.356215 printcleaner-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-03-10 16:54:33.946506 printcleaner-0.1.5/printcleaner/__init__.py
--rw-r--r--   0        0        0     1388 2023-03-12 18:54:15.429779 printcleaner-0.1.5/printcleaner/clean.py
--rw-r--r--   0        0        0      598 2023-03-12 19:03:07.529106 printcleaner-0.1.5/printcleaner/transformer.py
--rw-r--r--   0        0        0      543 2023-03-12 19:52:32.160350 printcleaner-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1437 2023-03-12 19:52:36.949015 printcleaner-0.1.5/setup.py
--rw-r--r--   0        0        0     1258 2023-03-12 19:52:36.949252 printcleaner-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-10 16:54:33.946052 printcleaner-0.1.6/LICENSE
+-rw-r--r--   0        0        0      597 2023-04-10 14:52:21.711445 printcleaner-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-03-10 16:54:33.946506 printcleaner-0.1.6/printcleaner/__init__.py
+-rw-r--r--   0        0        0     1388 2023-03-12 18:54:15.429779 printcleaner-0.1.6/printcleaner/clean.py
+-rw-r--r--   0        0        0      598 2023-03-12 19:03:07.529106 printcleaner-0.1.6/printcleaner/transformer.py
+-rw-r--r--   0        0        0      543 2023-04-10 15:00:36.331408 printcleaner-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1446 2023-04-10 15:01:15.657423 printcleaner-0.1.6/setup.py
+-rw-r--r--   0        0        0     1267 2023-04-10 15:01:15.657623 printcleaner-0.1.6/PKG-INFO
```

### Comparing `printcleaner-0.1.5/LICENSE` & `printcleaner-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `printcleaner-0.1.5/README.md` & `printcleaner-0.1.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-## Printcleaner: the simplest way to remove print statements from your Python code
+# Printcleaner: the simplest way to remove print statements from your Python code
 
 
 ![GitHub](https://img.shields.io/github/license/larsvonschaff/printcleaner)
 ![PyPI](https://img.shields.io/pypi/v/printcleaner)
 
 
-Is your Python code littered with random print statements from debugging or simply exploring?
+### Is your Python code littered with random print statements from debugging or simply exploring?
 
 Printcleaner is a simple CLI that removes all of them with one command. All you need to do is:
 
 
-**pip install printcleaner**
+```pip install printcleaner ```
 
-**clean < name of your file or directory >**
+```clean < name of your file or directory > ```
 
 Done. Don't worry: comments, formatting, whitespace and everything else in your code will be preserved.
```

### Comparing `printcleaner-0.1.5/printcleaner/clean.py` & `printcleaner-0.1.6/printcleaner/clean.py`

 * *Files identical despite different names*

### Comparing `printcleaner-0.1.5/printcleaner/transformer.py` & `printcleaner-0.1.6/printcleaner/transformer.py`

 * *Files identical despite different names*

### Comparing `printcleaner-0.1.5/pyproject.toml` & `printcleaner-0.1.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "printcleaner"
-version = "0.1.5"
+version = "0.1.6"
 description = "The simplest way to remove print statements from your Python code"
 authors = ["A. L. Walker <walkernotwalker@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/leftfile/printcleaner"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `printcleaner-0.1.5/setup.py` & `printcleaner-0.1.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['libcst>=0.4.7,<0.5.0', 'typer>=0.6.1,<0.7.0']
 
 entry_points = \
 {'console_scripts': ['clean = printcleaner.clean:app']}
 
 setup_kwargs = {
     'name': 'printcleaner',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'The simplest way to remove print statements from your Python code',
-    'long_description': "## Printcleaner: the simplest way to remove print statements from your Python code\n\n\n![GitHub](https://img.shields.io/github/license/larsvonschaff/printcleaner)\n![PyPI](https://img.shields.io/pypi/v/printcleaner)\n\n\nIs your Python code littered with random print statements from debugging or simply exploring?\n\nPrintcleaner is a simple CLI that removes all of them with one command. All you need to do is:\n\n\n**pip install printcleaner**\n\n**clean < name of your file or directory >**\n\nDone. Don't worry: comments, formatting, whitespace and everything else in your code will be preserved.\n\n",
+    'long_description': "# Printcleaner: the simplest way to remove print statements from your Python code\n\n\n![GitHub](https://img.shields.io/github/license/larsvonschaff/printcleaner)\n![PyPI](https://img.shields.io/pypi/v/printcleaner)\n\n\n### Is your Python code littered with random print statements from debugging or simply exploring?\n\nPrintcleaner is a simple CLI that removes all of them with one command. All you need to do is:\n\n\n```pip install printcleaner ```\n\n```clean < name of your file or directory > ```\n\nDone. Don't worry: comments, formatting, whitespace and everything else in your code will be preserved.\n\n",
     'author': 'A. L. Walker',
     'author_email': 'walkernotwalker@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/leftfile/printcleaner',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `printcleaner-0.1.5/PKG-INFO` & `printcleaner-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: printcleaner
-Version: 0.1.5
+Version: 0.1.6
 Summary: The simplest way to remove print statements from your Python code
 Home-page: https://github.com/leftfile/printcleaner
 License: MIT
 Author: A. L. Walker
 Author-email: walkernotwalker@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,26 +12,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: libcst (>=0.4.7,<0.5.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Project-URL: Repository, https://github.com/leftfile/printcleaner
 Description-Content-Type: text/markdown
 
-## Printcleaner: the simplest way to remove print statements from your Python code
+# Printcleaner: the simplest way to remove print statements from your Python code
 
 
 ![GitHub](https://img.shields.io/github/license/larsvonschaff/printcleaner)
 ![PyPI](https://img.shields.io/pypi/v/printcleaner)
 
 
-Is your Python code littered with random print statements from debugging or simply exploring?
+### Is your Python code littered with random print statements from debugging or simply exploring?
 
 Printcleaner is a simple CLI that removes all of them with one command. All you need to do is:
 
 
-**pip install printcleaner**
+```pip install printcleaner ```
 
-**clean < name of your file or directory >**
+```clean < name of your file or directory > ```
 
 Done. Don't worry: comments, formatting, whitespace and everything else in your code will be preserved.
```


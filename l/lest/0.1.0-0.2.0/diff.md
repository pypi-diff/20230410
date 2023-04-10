# Comparing `tmp/lest-0.1.0.tar.gz` & `tmp/lest-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lest-0.1.0.tar", last modified: Tue Apr  4 11:14:09 2023, max compression
+gzip compressed data, was "lest-0.2.0.tar", last modified: Sat Apr  8 07:43:27 2023, max compression
```

## Comparing `lest-0.1.0.tar` & `lest-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 11:14:09.356822 lest-0.1.0/
--rw-rw-rw-   0        0        0     1084 2023-04-04 11:05:14.000000 lest-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1179 2023-04-04 11:14:09.355821 lest-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      676 2023-04-04 11:08:29.000000 lest-0.1.0/README.md
--rw-rw-rw-   0        0        0      493 2023-04-04 11:09:54.000000 lest-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-04 11:14:09.356822 lest-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-04 11:14:09.335591 lest-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-04 11:14:09.347280 lest-0.1.0/src/lest/
--rw-rw-rw-   0        0        0      223 2023-04-04 11:03:08.000000 lest-0.1.0/src/lest/__init__.py
--rw-rw-rw-   0        0        0      312 2023-04-03 11:04:41.000000 lest-0.1.0/src/lest/registerer.py
--rw-rw-rw-   0        0        0     1329 2023-04-04 10:52:57.000000 lest-0.1.0/src/lest/runner.py
-drwxrwxrwx   0        0        0        0 2023-04-04 11:14:09.353824 lest-0.1.0/src/lest.egg-info/
--rw-rw-rw-   0        0        0     1179 2023-04-04 11:14:09.000000 lest-0.1.0/src/lest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-04 11:14:09.000000 lest-0.1.0/src/lest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 11:14:09.000000 lest-0.1.0/src/lest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-04 11:14:09.000000 lest-0.1.0/src/lest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 07:43:27.602996 lest-0.2.0/
+-rw-rw-rw-   0        0        0     1084 2023-04-04 11:05:14.000000 lest-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1334 2023-04-08 07:43:27.601003 lest-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      831 2023-04-08 07:35:21.000000 lest-0.2.0/README.md
+-rw-rw-rw-   0        0        0      493 2023-04-08 07:42:33.000000 lest-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-08 07:43:27.602996 lest-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-08 07:43:27.579984 lest-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-08 07:43:27.591990 lest-0.2.0/src/lest/
+-rw-rw-rw-   0        0        0      223 2023-04-04 11:03:08.000000 lest-0.2.0/src/lest/__init__.py
+-rw-rw-rw-   0        0        0      312 2023-04-03 11:04:41.000000 lest-0.2.0/src/lest/registerer.py
+-rw-rw-rw-   0        0        0     1997 2023-04-08 07:38:46.000000 lest-0.2.0/src/lest/runner.py
+drwxrwxrwx   0        0        0        0 2023-04-08 07:43:27.598991 lest-0.2.0/src/lest.egg-info/
+-rw-rw-rw-   0        0        0     1334 2023-04-08 07:43:27.000000 lest-0.2.0/src/lest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-08 07:43:27.000000 lest-0.2.0/src/lest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 07:43:27.000000 lest-0.2.0/src/lest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-08 07:43:27.000000 lest-0.2.0/src/lest.egg-info/top_level.txt
```

### Comparing `lest-0.1.0/LICENSE` & `lest-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lest-0.1.0/PKG-INFO` & `lest-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lest
-Version: 0.1.0
+Version: 0.2.0
 Summary: Light Python library for testing.
 Author-email: wchistow <wchistow@yandex.ru>
 Project-URL: Homepage, https://github.com/wchistow/lest
 Project-URL: Bug Tracker, https://github.com/wchistow/lest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,36 +12,46 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Lest
 
 ## Light Python library for testing
 
-## Example:
+## Installing
+
+Just enter in command line:
+
+```shell
+pip install lest
+```
+
+## Usage
+
+### Example:
 
 Code:
 
 ```python
-import lest
+from lest import register, run
 
 
-@lest.register
+@register
 def test_adding_two_and_two():
     assert 2 + 2 == 4
 
 
-@lest.register
+@register
 def some_error_test():
     assert 2 + 2 == 5
 
 
-lest.run()
+run()
 ```
 
-Output:
+Output: (To visible the highlighting, run on the command line)
 
 ```text
 Running [test_adding_two_and_two]... OK
 Running [some_error_test]... FAILED:
 Traceback (most recent call last):
   File "E:\vladimir\Python\lest\src\lest\runner.py", line 23, in run
     func()
```

### Comparing `lest-0.1.0/src/lest.egg-info/PKG-INFO` & `lest-0.2.0/src/lest.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lest
-Version: 0.1.0
+Version: 0.2.0
 Summary: Light Python library for testing.
 Author-email: wchistow <wchistow@yandex.ru>
 Project-URL: Homepage, https://github.com/wchistow/lest
 Project-URL: Bug Tracker, https://github.com/wchistow/lest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,36 +12,46 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Lest
 
 ## Light Python library for testing
 
-## Example:
+## Installing
+
+Just enter in command line:
+
+```shell
+pip install lest
+```
+
+## Usage
+
+### Example:
 
 Code:
 
 ```python
-import lest
+from lest import register, run
 
 
-@lest.register
+@register
 def test_adding_two_and_two():
     assert 2 + 2 == 4
 
 
-@lest.register
+@register
 def some_error_test():
     assert 2 + 2 == 5
 
 
-lest.run()
+run()
 ```
 
-Output:
+Output: (To visible the highlighting, run on the command line)
 
 ```text
 Running [test_adding_two_and_two]... OK
 Running [some_error_test]... FAILED:
 Traceback (most recent call last):
   File "E:\vladimir\Python\lest\src\lest\runner.py", line 23, in run
     func()
```


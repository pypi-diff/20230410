# Comparing `tmp/string_py-0.1.0.tar.gz` & `tmp/string_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string_py-0.1.0.tar", last modified: Thu Apr  6 19:39:37 2023, max compression
+gzip compressed data, was "string_py-0.1.1.tar", last modified: Mon Apr 10 13:47:54 2023, max compression
```

## Comparing `string_py-0.1.0.tar` & `string_py-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 19:39:37.751135 string_py-0.1.0/
--rw-rw-rw-   0        0        0     1435 2023-04-06 19:39:37.735494 string_py-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1046 2023-04-06 15:31:01.000000 string_py-0.1.0/README.md
--rw-rw-rw-   0        0        0      557 2023-04-06 16:37:19.000000 string_py-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-06 19:39:37.751135 string_py-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      881 2023-04-06 19:39:34.000000 string_py-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:39:37.719870 string_py-0.1.0/string_py/
--rw-rw-rw-   0        0        0      171 2023-04-06 19:39:34.000000 string_py-0.1.0/string_py/__init__.py
--rw-rw-rw-   0        0        0    13126 2023-04-06 19:35:20.000000 string_py-0.1.0/string_py/string_py.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:39:37.735494 string_py-0.1.0/string_py.egg-info/
--rw-rw-rw-   0        0        0     1435 2023-04-06 19:39:37.000000 string_py-0.1.0/string_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-04-06 19:39:37.000000 string_py-0.1.0/string_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 19:39:37.000000 string_py-0.1.0/string_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-06 19:39:37.000000 string_py-0.1.0/string_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 13:47:54.095958 string_py-0.1.1/
+-rw-rw-rw-   0        0        0     1489 2023-04-10 13:47:54.094957 string_py-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1046 2023-04-07 15:46:43.000000 string_py-0.1.1/README.md
+-rw-rw-rw-   0        0        0      558 2023-04-10 13:47:51.000000 string_py-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-10 13:47:54.096960 string_py-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-04-10 13:47:51.000000 string_py-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 13:47:54.080945 string_py-0.1.1/string_py/
+-rw-rw-rw-   0        0        0      171 2023-04-10 13:47:51.000000 string_py-0.1.1/string_py/__init__.py
+-rw-rw-rw-   0        0        0    13185 2023-04-08 13:34:38.000000 string_py-0.1.1/string_py/string_py.py
+drwxrwxrwx   0        0        0        0 2023-04-10 13:47:54.091954 string_py-0.1.1/string_py.egg-info/
+-rw-rw-rw-   0        0        0     1489 2023-04-10 13:47:53.000000 string_py-0.1.1/string_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-04-10 13:47:53.000000 string_py-0.1.1/string_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 13:47:53.000000 string_py-0.1.1/string_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-10 13:47:53.000000 string_py-0.1.1/string_py.egg-info/top_level.txt
```

### Comparing `string_py-0.1.0/PKG-INFO` & `string_py-0.1.1/string_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
-Name: string_py
-Version: 0.1.0
+Name: string-py
+Version: 0.1.1
 Summary: Utils for strings in python
+Home-page: https://github.com/BabyEntchen/string_py
 Author: BabyEntchen
 Author-email: BabyEntchen <baby_entchen@web.de>
 License: MIT
 Keywords: python,string,strings,utils,string utils,random,random strings,formatting,formatter
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # string_py
 
 
 [![PyPI](https://img.shields.io/pypi/v/string-py?style=flat-square)](https://pypi.org/project/string-py/)
```

### Comparing `string_py-0.1.0/README.md` & `string_py-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `string_py-0.1.0/pyproject.toml` & `string_py-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "string_py"
 authors = [
     {name = "BabyEntchen", email = "baby_entchen@web.de"},
 ]
 description = "Utils for strings in python"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 keywords=['python', 'string', 'strings', 'utils', 'string utils', 'random', 'random strings', 'formatting', 'formatter']
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = []
 dynamic = ["version"]
```

### Comparing `string_py-0.1.0/setup.py` & `string_py-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 from pathlib import Path
 
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Utils for strings in python'
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
+URL = "https://github.com/BabyEntchen/string_py"
 
 # Setting up
 setup(
     name="string_py",
     version=VERSION,
     author="BabyEntchen",
     author_email="<baby_entchen@web.de>",
+    url=URL,
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python', 'string', 'strings', 'utils', 'string utils', 'random', 'random strings', 'formatting', 'formatter'],
     classifiers=[
```

### Comparing `string_py-0.1.0/string_py/string_py.py` & `string_py-0.1.1/string_py/string_py.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,23 +126,25 @@
         elif min_ is not None and max_ is not None:
             if min_ > max_:
                 raise AttributeError("min_ must have a smaller value then max_")
             return "".join(choices(self.chars, k=randint(min_, max_)))
         else:
             raise AttributeError("min_ and max_ or length must have a value")
 
-    def remove(self, chars: str) -> str:
+    def remove(self, *chars: str) -> str:
         """Remove chars from string
 
         Parameters:
         -----------
         :param chars:
             The chars you want to remove
         """
-        return self.values.replace(chars, "")
+        for x in chars:
+            self.values = self.values.replace(x, "")
+        return self.values
 
     def split(self, each: int = None, chars: str = None) -> list[str]:
         """An extension of the built-in .split method. Also split on certain index
 
         Parameters
         ----------
         :param each:
@@ -190,15 +192,14 @@
             raise AttributeError("Length must be smaller then value")
         if remove:
             return self.values[:-length]
         else:
             return self.values[-length:]
 
     def __get(self, type_: str, index: bool) -> list[str] | dict[int, str]:
-
         gets = [] if index is False else {}
         for num, char in enumerate(self.values):
             if char in self.ascii[type_]:
                 if index is False:
                     gets.append(char)
                 else:
                     gets[num] = char
```

### Comparing `string_py-0.1.0/string_py.egg-info/PKG-INFO` & `string_py-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
-Name: string-py
-Version: 0.1.0
+Name: string_py
+Version: 0.1.1
 Summary: Utils for strings in python
+Home-page: https://github.com/BabyEntchen/string_py
 Author: BabyEntchen
 Author-email: BabyEntchen <baby_entchen@web.de>
 License: MIT
 Keywords: python,string,strings,utils,string utils,random,random strings,formatting,formatter
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # string_py
 
 
 [![PyPI](https://img.shields.io/pypi/v/string-py?style=flat-square)](https://pypi.org/project/string-py/)
```


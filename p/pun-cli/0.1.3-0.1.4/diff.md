# Comparing `tmp/pun_cli-0.1.3.tar.gz` & `tmp/pun_cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pun_cli-0.1.3.tar", max compression
+gzip compressed data, was "pun_cli-0.1.4.tar", max compression
```

## Comparing `pun_cli-0.1.3.tar` & `pun_cli-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-04-09 20:56:41.961148 pun_cli-0.1.3/LICENSE
--rw-r--r--   0        0        0     1208 2023-04-09 21:16:56.021875 pun_cli-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-04-10 16:54:28.517157 pun_cli-0.1.3/pun_cli/__init__.py
--rw-r--r--   0        0        0       67 2023-04-10 17:03:19.373173 pun_cli-0.1.3/pun_cli/__main__.py
--rw-r--r--   0        0        0     1172 2023-04-10 17:03:49.401174 pun_cli-0.1.3/pun_cli/cli.py
--rw-r--r--   0        0        0      793 2023-04-10 16:57:10.617162 pun_cli-0.1.3/pun_cli/pun_generator.py
--rw-r--r--   0        0        0      977 2023-04-10 17:03:46.373174 pun_cli-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2288 1970-01-01 00:00:00.000000 pun_cli-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-09 20:56:41.961148 pun_cli-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1208 2023-04-09 21:16:56.021875 pun_cli-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 16:54:28.517157 pun_cli-0.1.4/pun_cli/__init__.py
+-rw-r--r--   0        0        0       67 2023-04-10 17:03:19.373173 pun_cli-0.1.4/pun_cli/__main__.py
+-rw-r--r--   0        0        0     1172 2023-04-10 17:10:39.565187 pun_cli-0.1.4/pun_cli/cli.py
+-rw-r--r--   0        0        0      793 2023-04-10 16:57:10.617162 pun_cli-0.1.4/pun_cli/pun_generator.py
+-rw-r--r--   0        0        0     1026 2023-04-10 17:12:46.505190 pun_cli-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2288 1970-01-01 00:00:00.000000 pun_cli-0.1.4/PKG-INFO
```

### Comparing `pun_cli-0.1.3/LICENSE` & `pun_cli-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pun_cli-0.1.3/README.md` & `pun_cli-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pun_cli-0.1.3/pun_cli/cli.py` & `pun_cli-0.1.4/pun_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import cowsay
 import random
 from pun_cli.pun_generator import generate_pun
 
-VERSION = 'v' + '0.1.3'
+VERSION = 'v' + '0.1.4'
 
 def cli():
     parser = argparse.ArgumentParser(description='Unleash hilarious wordplay with a single command.')
     parser.add_argument('--keyword', '-k', help='Keyword to search for puns.')
     parser.add_argument('--character', '-c', help='Character to use for the pun. One of: ' + ', '.join(cowsay.char_names))
     parser.add_argument('--add', '-a', help='Add a pun to the repository.', action='store_true')
     parser.add_argument('--version', '-v', action='version', version='%(prog)s ' + VERSION, help='Print version and exit.')
```

### Comparing `pun_cli-0.1.3/pun_cli/pun_generator.py` & `pun_cli-0.1.4/pun_cli/pun_generator.py`

 * *Files identical despite different names*

### Comparing `pun_cli-0.1.3/pyproject.toml` & `pun_cli-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pun-cli"
-version = "0.1.3"
+version = "0.1.4"
 description = "Pun-CLI: Because you can't resist a good pun. Generate hilarious puns from our pun repository or contribute your own puns to the list. Pun-CLI, the command-line tool you never knew you needed."
 authors = ["Vahid Al <thevahidal@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pun_cli"}]
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -15,17 +15,18 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
 ]
 
-
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.28.2"
 cowsay = "^5.0"
 
+[tool.poetry.scripts]
+pun-cli = "pun_cli.cli:cli"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pun_cli-0.1.3/PKG-INFO` & `pun_cli-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pun-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pun-CLI: Because you can't resist a good pun. Generate hilarious puns from our pun repository or contribute your own puns to the list. Pun-CLI, the command-line tool you never knew you needed.
 License: MIT
 Author: Vahid Al
 Author-email: thevahidal@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```


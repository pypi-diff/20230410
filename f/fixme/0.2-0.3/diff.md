# Comparing `tmp/fixme-0.2.tar.gz` & `tmp/fixme-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixme-0.2.tar", last modified: Fri Feb 24 05:44:44 2023, max compression
+gzip compressed data, was "fixme-0.3.tar", last modified: Mon Apr 10 06:45:09 2023, max compression
```

## Comparing `fixme-0.2.tar` & `fixme-0.3.tar`

### file list

```diff
@@ -1,19 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 05:44:44.107361 fixme-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-24 05:44:29.000000 fixme-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-02-24 05:44:44.107361 fixme-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-02-24 05:44:29.000000 fixme-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 05:44:44.107361 fixme-0.2/fixme/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 05:44:29.000000 fixme-0.2/fixme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-24 05:44:29.000000 fixme-0.2/fixme/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-24 05:44:29.000000 fixme-0.2/fixme/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 05:44:44.107361 fixme-0.2/fixme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-02-24 05:44:44.000000 fixme-0.2/fixme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-24 05:44:44.000000 fixme-0.2/fixme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 05:44:44.000000 fixme-0.2/fixme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-24 05:44:44.000000 fixme-0.2/fixme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-24 05:44:44.000000 fixme-0.2/fixme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-24 05:44:44.000000 fixme-0.2/fixme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 05:44:44.107361 fixme-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-02-24 05:44:29.000000 fixme-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 05:44:44.107361 fixme-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-02-24 05:44:29.000000 fixme-0.2/tests/test_fixme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 06:45:09.802559 fixme-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 06:44:55.000000 fixme-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-10 06:45:09.798559 fixme-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-10 06:44:55.000000 fixme-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 06:45:09.794559 fixme-0.3/fixme/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 06:44:55.000000 fixme-0.3/fixme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-10 06:44:55.000000 fixme-0.3/fixme/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-04-10 06:44:55.000000 fixme-0.3/fixme/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-10 06:44:55.000000 fixme-0.3/fixme/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-10 06:44:55.000000 fixme-0.3/fixme/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 06:45:09.798559 fixme-0.3/fixme/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 06:44:55.000000 fixme-0.3/fixme/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-10 06:44:55.000000 fixme-0.3/fixme/prompts/diagnose_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-10 06:44:55.000000 fixme-0.3/fixme/prompts/fix_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-10 06:44:55.000000 fixme-0.3/fixme/prompts/gather_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-10 06:44:55.000000 fixme-0.3/fixme/prompts/generate_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-10 06:44:55.000000 fixme-0.3/fixme/prompts/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-10 06:44:55.000000 fixme-0.3/fixme/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-10 06:44:55.000000 fixme-0.3/fixme/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 06:45:09.798559 fixme-0.3/fixme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-10 06:45:09.000000 fixme-0.3/fixme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-10 06:45:09.000000 fixme-0.3/fixme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 06:45:09.000000 fixme-0.3/fixme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 06:45:09.000000 fixme-0.3/fixme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 06:45:09.000000 fixme-0.3/fixme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 06:45:09.000000 fixme-0.3/fixme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-10 06:44:55.000000 fixme-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 06:45:09.802559 fixme-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-10 06:44:55.000000 fixme-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 06:45:09.798559 fixme-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-10 06:44:55.000000 fixme-0.3/tests/test_fixme.py
```

### Comparing `fixme-0.2/LICENSE` & `fixme-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fixme-0.2/PKG-INFO` & `fixme-0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: fixme
-Version: 0.2
+Version: 0.3
 Summary: Use AI to automatically fix bugs
 Home-page: https://github.com/helloworld/fixme
 Author: helloworld
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/helloworld/fixme/issues
 Project-URL: CI, https://github.com/helloworld/fixme/actions
 Project-URL: Changelog, https://github.com/helloworld/fixme/releases
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: black
+Provides-Extra: pyright
+Provides-Extra: ruff
 Provides-Extra: test
 License-File: LICENSE
 
 # fixme
 
 [![PyPI](https://img.shields.io/pypi/v/fixme.svg)](https://pypi.org/project/fixme/)
 [![Changelog](https://img.shields.io/github/v/release/helloworld/fixme?include_prereleases&label=changelog)](https://github.com/helloworld/fixme/releases)
```

### Comparing `fixme-0.2/README.md` & `fixme-0.3/README.md`

 * *Files identical despite different names*

### Comparing `fixme-0.2/fixme.egg-info/PKG-INFO` & `fixme-0.3/fixme.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: fixme
-Version: 0.2
+Version: 0.3
 Summary: Use AI to automatically fix bugs
 Home-page: https://github.com/helloworld/fixme
 Author: helloworld
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/helloworld/fixme/issues
 Project-URL: CI, https://github.com/helloworld/fixme/actions
 Project-URL: Changelog, https://github.com/helloworld/fixme/releases
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: black
+Provides-Extra: pyright
+Provides-Extra: ruff
 Provides-Extra: test
 License-File: LICENSE
 
 # fixme
 
 [![PyPI](https://img.shields.io/pypi/v/fixme.svg)](https://pypi.org/project/fixme/)
 [![Changelog](https://img.shields.io/github/v/release/helloworld/fixme?include_prereleases&label=changelog)](https://github.com/helloworld/fixme/releases)
```

### Comparing `fixme-0.2/setup.py` & `fixme-0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from setuptools import setup
 import os
 
-VERSION = "0.2"
+from setuptools import find_packages, setup
+
+VERSION = "0.3"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -22,18 +23,23 @@
     project_urls={
         "Issues": "https://github.com/helloworld/fixme/issues",
         "CI": "https://github.com/helloworld/fixme/actions",
         "Changelog": "https://github.com/helloworld/fixme/releases",
     },
     license="Apache License, Version 2.0",
     version=VERSION,
-    packages=["fixme"],
+    packages=find_packages(),
     entry_points="""
         [console_scripts]
         fixme=fixme.cli:cli
     """,
-    install_requires=["click"],
+    install_requires=["click", "openai", "rich", "pydantic"],
     extras_require={
-        "test": ["pytest"]
+        "black": ["black"],
+        "pyright": ["pyright"],
+        "ruff": ["ruff"],
+        "test": [
+            "pytest",
+        ],
     },
     python_requires=">=3.7",
 )
```


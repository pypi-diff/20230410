# Comparing `tmp/wtt02-0.1.9.tar.gz` & `tmp/wtt02-0.2.0.tar.gz`

## Comparing `wtt02-0.1.9.tar` & `wtt02-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 wtt02-0.1.9/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtt02-0.1.9/tests/__init__.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 wtt02-0.1.9/tests/test_load.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 wtt02-0.1.9/wtt02/__about__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wtt02-0.1.9/wtt02/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 wtt02-0.1.9/wtt02/_env.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 wtt02-0.1.9/wtt02/main.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 wtt02-0.1.9/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 wtt02-0.1.9/LICENSE.txt
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wtt02-0.1.9/README.md
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 wtt02-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 wtt02-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 wtt02-0.2.0/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtt02-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 wtt02-0.2.0/tests/test_load.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 wtt02-0.2.0/wtt02/__about__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wtt02-0.2.0/wtt02/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 wtt02-0.2.0/wtt02/_env.py
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 wtt02-0.2.0/wtt02/main.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 wtt02-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 wtt02-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wtt02-0.2.0/README.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 wtt02-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 wtt02-0.2.0/PKG-INFO
```

### Comparing `wtt02-0.1.9/tests/test_load.py` & `wtt02-0.2.0/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `wtt02-0.1.9/wtt02/main.py` & `wtt02-0.2.0/wtt02/main.py`

 * *Files identical despite different names*

### Comparing `wtt02-0.1.9/LICENSE.txt` & `wtt02-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wtt02-0.1.9/pyproject.toml` & `wtt02-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wtt02-0.1.9/PKG-INFO` & `wtt02-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtt02
-Version: 0.1.9
+Version: 0.2.0
 Author-email: Trent Hauck <thauck@wheretrue.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


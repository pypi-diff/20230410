# Comparing `tmp/mysql-mimic-2.2.2.tar.gz` & `tmp/mysql-mimic-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-mimic-2.2.2.tar", last modified: Fri Mar 31 18:02:41 2023, max compression
+gzip compressed data, was "mysql-mimic-2.2.3.tar", last modified: Mon Apr 10 17:20:18 2023, max compression
```

## Comparing `mysql-mimic-2.2.2.tar` & `mysql-mimic-2.2.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:02:41.712979 mysql-mimic-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-03-31 18:02:41.712979 mysql-mimic-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:02:41.712979 mysql-mimic-2.2.2/mysql_mimic/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/mysql_mimic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/mysql_mimic/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/mysql_mimic/charset.py
--rw-r--r--   0 runner    (1001) docker     (123)    22475 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/mysql_mimic/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/mysql_mimic/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/mysql_mimic/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/mysql_mimic/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/mysql_mimic/intercept.py
--rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/mysql_mimic/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/mysql_mimic/prepared.py
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/mysql_mimic/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/mysql_mimic/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/mysql_mimic/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    16528 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/mysql_mimic/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/mysql_mimic/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/mysql_mimic/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/mysql_mimic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/mysql_mimic/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/mysql_mimic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:02:41.712979 mysql-mimic-2.2.2/mysql_mimic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-03-31 18:02:41.000000 mysql-mimic-2.2.2/mysql_mimic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-31 18:02:41.000000 mysql-mimic-2.2.2/mysql_mimic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 18:02:41.000000 mysql-mimic-2.2.2/mysql_mimic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-31 18:02:41.000000 mysql-mimic-2.2.2/mysql_mimic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-31 18:02:41.000000 mysql-mimic-2.2.2/mysql_mimic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 18:02:41.712979 mysql-mimic-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:02:41.712979 mysql-mimic-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    28241 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/tests/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-31 18:02:11.000000 mysql-mimic-2.2.2/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:20:18.081870 mysql-mimic-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-04-10 17:20:18.081870 mysql-mimic-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:20:18.077870 mysql-mimic-2.2.3/mysql_mimic/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/charset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22475 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/intercept.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/prepared.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16711 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:20:18.077870 mysql-mimic-2.2.3/mysql_mimic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-04-10 17:20:18.000000 mysql-mimic-2.2.3/mysql_mimic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-10 17:20:18.000000 mysql-mimic-2.2.3/mysql_mimic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:20:18.000000 mysql-mimic-2.2.3/mysql_mimic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-10 17:20:18.000000 mysql-mimic-2.2.3/mysql_mimic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 17:20:18.000000 mysql-mimic-2.2.3/mysql_mimic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 17:20:18.081870 mysql-mimic-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:20:18.077870 mysql-mimic-2.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28243 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/tests/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/tests/test_version.py
```

### Comparing `mysql-mimic-2.2.2/LICENSE` & `mysql-mimic-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/PKG-INFO` & `mysql-mimic-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-mimic
-Version: 2.2.2
+Version: 2.2.3
 Summary: A python implementation of the mysql server protocol
 Home-page: https://github.com/kelsin/mysql-mimic
 Author: Christopher Giroir
 Author-email: kelsin@valefor.com
 License: MIT
 Description: # MySQL-Mimic
```

### Comparing `mysql-mimic-2.2.2/README.md` & `mysql-mimic-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/mysql_mimic/auth.py` & `mysql-mimic-2.2.3/mysql_mimic/auth.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/mysql_mimic/charset.py` & `mysql-mimic-2.2.3/mysql_mimic/charset.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/mysql_mimic/connection.py` & `mysql-mimic-2.2.3/mysql_mimic/connection.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/mysql_mimic/constants.py` & `mysql-mimic-2.2.3/mysql_mimic/constants.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/mysql_mimic/errors.py` & `mysql-mimic-2.2.3/mysql_mimic/errors.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/mysql_mimic/intercept.py` & `mysql-mimic-2.2.3/mysql_mimic/intercept.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/mysql_mimic/packets.py` & `mysql-mimic-2.2.3/mysql_mimic/packets.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/mysql_mimic/results.py` & `mysql-mimic-2.2.3/mysql_mimic/results.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/mysql_mimic/schema.py` & `mysql-mimic-2.2.3/mysql_mimic/schema.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/mysql_mimic/server.py` & `mysql-mimic-2.2.3/mysql_mimic/server.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/mysql_mimic/session.py` & `mysql-mimic-2.2.3/mysql_mimic/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,17 +298,23 @@
 
     async def _replace_variables_interceptor(self, expression: exp.Expression) -> None:
         """Replace session variables and information functions with their corresponding values"""
 
         def _transform(node: exp.Expression) -> exp.Expression:
             new_node = None
 
-            if isinstance(node, exp.Anonymous) and node.name.upper() in self._functions:
-                value = self._functions[node.name.upper()]()
-                new_node = value_to_expression(value)
+            if isinstance(node, exp.Func):
+                if isinstance(node, exp.Anonymous):
+                    func_name = node.name.upper()
+                else:
+                    func_name = node.sql_name()
+                func = self._functions.get(func_name)
+                if func:
+                    value = func()
+                    new_node = value_to_expression(value)
             elif isinstance(node, exp.Column) and node.sql() == "CURRENT_USER":
                 value = self._functions["CURRENT_USER"]()
                 new_node = value_to_expression(value)
             elif isinstance(node, exp.SessionParameter):
                 value = self.variables.get(node.name)
                 new_node = value_to_expression(value)
```

### Comparing `mysql-mimic-2.2.2/mysql_mimic/stream.py` & `mysql-mimic-2.2.3/mysql_mimic/stream.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/mysql_mimic/types.py` & `mysql-mimic-2.2.3/mysql_mimic/types.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/mysql_mimic/utils.py` & `mysql-mimic-2.2.3/mysql_mimic/utils.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/mysql_mimic/variables.py` & `mysql-mimic-2.2.3/mysql_mimic/variables.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/mysql_mimic.egg-info/PKG-INFO` & `mysql-mimic-2.2.3/mysql_mimic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-mimic
-Version: 2.2.2
+Version: 2.2.3
 Summary: A python implementation of the mysql server protocol
 Home-page: https://github.com/kelsin/mysql-mimic
 Author: Christopher Giroir
 Author-email: kelsin@valefor.com
 License: MIT
 Description: # MySQL-Mimic
```

### Comparing `mysql-mimic-2.2.2/mysql_mimic.egg-info/SOURCES.txt` & `mysql-mimic-2.2.3/mysql_mimic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/setup.py` & `mysql-mimic-2.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/tests/test_auth.py` & `mysql-mimic-2.2.3/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/tests/test_query.py` & `mysql-mimic-2.2.3/tests/test_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,15 @@
     session.echo = True
 
     with closing(await connect(user="levon_helm", database="db")) as conn:
         result = await query(conn, "SELECT CONNECTION_ID()")
         assert result[0]["CONNECTION_ID()"] is not None
 
         result = await query(conn, "SELECT CURRENT_USER")
-        assert result[0]["CURRENT_USER"] == "levon_helm"
+        assert result[0]["CURRENT_USER()"] == "levon_helm"
 
         result = await query(conn, "SELECT USER()")
         assert result[0]["USER()"] == "levon_helm"
 
         result = await query(conn, "SELECT DATABASE()")
         assert result[0]["DATABASE()"] == "db"
```

### Comparing `mysql-mimic-2.2.2/tests/test_ssl.py` & `mysql-mimic-2.2.3/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/tests/test_stream.py` & `mysql-mimic-2.2.3/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.2/tests/test_types.py` & `mysql-mimic-2.2.3/tests/test_types.py`

 * *Files identical despite different names*


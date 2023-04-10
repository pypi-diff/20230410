# Comparing `tmp/RogueORM-0.0.1.tar.gz` & `tmp/RogueORM-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RogueORM-0.0.1.tar", last modified: Sun Dec 18 19:11:41 2022, max compression
+gzip compressed data, was "RogueORM-0.0.2.tar", last modified: Mon Apr 10 17:02:40 2023, max compression
```

## Comparing `RogueORM-0.0.1.tar` & `RogueORM-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxrwxrwx   0        0        0        0 2022-12-18 19:11:41.092686 RogueORM-0.0.1/
--rw-rw-rw-   0        0        0     1093 2022-12-06 23:54:36.000000 RogueORM-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2173 2022-12-18 19:11:41.092686 RogueORM-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      385 2022-12-18 18:47:43.000000 RogueORM-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-12-18 19:11:41.070165 RogueORM-0.0.1/RogueORM.egg-info/
--rw-rw-rw-   0        0        0     2173 2022-12-18 19:11:41.000000 RogueORM-0.0.1/RogueORM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2022-12-18 19:11:41.000000 RogueORM-0.0.1/RogueORM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-18 19:11:41.000000 RogueORM-0.0.1/RogueORM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2022-12-18 19:11:41.000000 RogueORM-0.0.1/RogueORM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-12-18 19:11:41.000000 RogueORM-0.0.1/RogueORM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1185 2022-12-18 18:55:32.000000 RogueORM-0.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2022-12-18 19:11:41.074166 RogueORM-0.0.1/rogue/
--rw-rw-rw-   0        0        0        0 2022-12-07 00:00:53.000000 RogueORM-0.0.1/rogue/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-18 19:11:41.078164 RogueORM-0.0.1/rogue/backends/
--rw-rw-rw-   0        0        0        0 2022-12-09 00:39:38.000000 RogueORM-0.0.1/rogue/backends/__init__.py
--rw-rw-rw-   0        0        0      644 2022-12-09 01:17:06.000000 RogueORM-0.0.1/rogue/backends/base.py
-drwxrwxrwx   0        0        0        0 2022-12-18 19:11:41.086165 RogueORM-0.0.1/rogue/backends/sqlite/
--rw-rw-rw-   0        0        0        0 2022-12-09 00:40:15.000000 RogueORM-0.0.1/rogue/backends/sqlite/__init__.py
--rw-rw-rw-   0        0        0        0 2022-12-09 00:46:51.000000 RogueORM-0.0.1/rogue/backends/sqlite/base.py
--rw-rw-rw-   0        0        0      531 2022-12-09 01:11:37.000000 RogueORM-0.0.1/rogue/backends/sqlite/client.py
--rw-rw-rw-   0        0        0        0 2022-12-09 01:11:58.000000 RogueORM-0.0.1/rogue/backends/sqlite/query.py
--rw-rw-rw-   0        0        0        0 2022-12-09 01:17:34.000000 RogueORM-0.0.1/rogue/backends/sqlite/schema.py
-drwxrwxrwx   0        0        0        0 2022-12-18 19:11:41.087165 RogueORM-0.0.1/rogue/fetchers/
--rw-rw-rw-   0        0        0        0 2022-12-07 00:00:40.000000 RogueORM-0.0.1/rogue/fetchers/__init__.py
--rw-rw-rw-   0        0        0       25 2022-12-07 00:24:13.000000 RogueORM-0.0.1/rogue/main.py
-drwxrwxrwx   0        0        0        0 2022-12-18 19:11:41.087165 RogueORM-0.0.1/rogue/managers/
--rw-rw-rw-   0        0        0        0 2022-12-07 00:00:40.000000 RogueORM-0.0.1/rogue/managers/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-18 19:11:41.089165 RogueORM-0.0.1/rogue/migrations/
--rw-rw-rw-   0        0        0        0 2022-12-09 01:21:03.000000 RogueORM-0.0.1/rogue/migrations/__init__.py
--rw-rw-rw-   0        0        0        0 2022-12-09 01:21:21.000000 RogueORM-0.0.1/rogue/migrations/base.py
-drwxrwxrwx   0        0        0        0 2022-12-18 19:11:41.091166 RogueORM-0.0.1/rogue/models/
--rw-rw-rw-   0        0        0       48 2022-12-18 19:08:42.000000 RogueORM-0.0.1/rogue/models/__init__.py
--rw-rw-rw-   0        0        0     1358 2022-12-09 01:23:50.000000 RogueORM-0.0.1/rogue/models/base.py
--rw-rw-rw-   0        0        0     1949 2022-12-09 00:38:26.000000 RogueORM-0.0.1/rogue/models/fields.py
--rw-rw-rw-   0        0        0       42 2022-12-18 19:11:41.092686 RogueORM-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 17:02:40.297160 RogueORM-0.0.2/
+-rw-rw-rw-   0        0        0     1093 2022-12-06 23:54:36.000000 RogueORM-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3835 2023-04-10 17:02:40.296186 RogueORM-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2053 2023-04-10 16:30:27.000000 RogueORM-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 17:02:40.279016 RogueORM-0.0.2/RogueORM.egg-info/
+-rw-rw-rw-   0        0        0     3835 2023-04-10 17:02:40.000000 RogueORM-0.0.2/RogueORM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-10 17:02:40.000000 RogueORM-0.0.2/RogueORM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 17:02:40.000000 RogueORM-0.0.2/RogueORM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-10 17:02:40.000000 RogueORM-0.0.2/RogueORM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-10 17:02:40.000000 RogueORM-0.0.2/RogueORM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1185 2023-04-10 17:00:56.000000 RogueORM-0.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-10 17:02:40.280965 RogueORM-0.0.2/rogue/
+-rw-rw-rw-   0        0        0        0 2022-12-07 00:00:53.000000 RogueORM-0.0.2/rogue/__init__.py
+-rw-rw-rw-   0        0        0      484 2023-04-10 16:29:25.000000 RogueORM-0.0.2/rogue/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:02:40.283896 RogueORM-0.0.2/rogue/backends/
+-rw-rw-rw-   0        0        0        0 2022-12-09 00:39:38.000000 RogueORM-0.0.2/rogue/backends/__init__.py
+-rw-rw-rw-   0        0        0     4367 2023-04-10 16:29:28.000000 RogueORM-0.0.2/rogue/backends/base.py
+-rw-rw-rw-   0        0        0      155 2022-12-21 23:27:34.000000 RogueORM-0.0.2/rogue/backends/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:02:40.286860 RogueORM-0.0.2/rogue/backends/sqlite/
+-rw-rw-rw-   0        0        0        0 2022-12-09 00:40:15.000000 RogueORM-0.0.2/rogue/backends/sqlite/__init__.py
+-rw-rw-rw-   0        0        0      601 2022-12-23 18:49:28.000000 RogueORM-0.0.2/rogue/backends/sqlite/client.py
+-rw-rw-rw-   0        0        0     2704 2023-01-05 21:20:18.000000 RogueORM-0.0.2/rogue/backends/sqlite/query.py
+-rw-rw-rw-   0        0        0     1114 2023-04-10 16:29:28.000000 RogueORM-0.0.2/rogue/backends/sqlite/schema.py
+-rw-rw-rw-   0        0        0       45 2022-12-21 18:46:55.000000 RogueORM-0.0.2/rogue/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:02:40.289789 RogueORM-0.0.2/rogue/managers/
+-rw-rw-rw-   0        0        0      128 2023-01-05 21:19:29.000000 RogueORM-0.0.2/rogue/managers/__init__.py
+-rw-rw-rw-   0        0        0     5853 2023-01-05 21:20:21.000000 RogueORM-0.0.2/rogue/managers/base.py
+-rw-rw-rw-   0        0        0      152 2022-12-21 18:47:09.000000 RogueORM-0.0.2/rogue/managers/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:02:40.290766 RogueORM-0.0.2/rogue/migrations/
+-rw-rw-rw-   0        0        0       66 2023-04-10 16:29:25.000000 RogueORM-0.0.2/rogue/migrations/__init__.py
+-rw-rw-rw-   0        0        0      952 2023-04-10 16:38:02.000000 RogueORM-0.0.2/rogue/migrations/base.py
+drwxrwxrwx   0        0        0        0 2023-04-10 17:02:40.295201 RogueORM-0.0.2/rogue/models/
+-rw-rw-rw-   0        0        0       84 2022-12-18 20:54:58.000000 RogueORM-0.0.2/rogue/models/__init__.py
+-rw-rw-rw-   0        0        0     7540 2023-01-05 21:23:17.000000 RogueORM-0.0.2/rogue/models/base.py
+-rw-rw-rw-   0        0        0      332 2022-12-21 23:59:31.000000 RogueORM-0.0.2/rogue/models/errors.py
+-rw-rw-rw-   0        0        0     8001 2023-01-05 21:19:29.000000 RogueORM-0.0.2/rogue/models/fields.py
+-rw-rw-rw-   0        0        0     1118 2022-12-23 19:43:17.000000 RogueORM-0.0.2/rogue/models/utils.py
+-rw-rw-rw-   0        0        0       42 2023-04-10 17:02:40.297160 RogueORM-0.0.2/setup.cfg
```

### Comparing `RogueORM-0.0.1/LICENSE` & `RogueORM-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `RogueORM-0.0.1/RogueORM.egg-info/SOURCES.txt` & `RogueORM-0.0.2/RogueORM.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,22 +3,26 @@
 pyproject.toml
 RogueORM.egg-info/PKG-INFO
 RogueORM.egg-info/SOURCES.txt
 RogueORM.egg-info/dependency_links.txt
 RogueORM.egg-info/requires.txt
 RogueORM.egg-info/top_level.txt
 rogue/__init__.py
-rogue/main.py
+rogue/__main__.py
+rogue/errors.py
 rogue/backends/__init__.py
 rogue/backends/base.py
+rogue/backends/errors.py
 rogue/backends/sqlite/__init__.py
-rogue/backends/sqlite/base.py
 rogue/backends/sqlite/client.py
 rogue/backends/sqlite/query.py
 rogue/backends/sqlite/schema.py
-rogue/fetchers/__init__.py
 rogue/managers/__init__.py
+rogue/managers/base.py
+rogue/managers/errors.py
 rogue/migrations/__init__.py
 rogue/migrations/base.py
 rogue/models/__init__.py
 rogue/models/base.py
-rogue/models/fields.py
+rogue/models/errors.py
+rogue/models/fields.py
+rogue/models/utils.py
```

### Comparing `RogueORM-0.0.1/pyproject.toml` & `RogueORM-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'RogueORM'
-version = '0.0.1'
+version = '0.0.2'
 description = 'An ORM that strives to eradicate N+1 issues.'
 readme = 'README.md'
 authors = [{name = 'Maxime Toussaint', email = 'm.toussaint@mail.com'}]
 license = {file = 'LICENSE'}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `RogueORM-0.0.1/rogue/backends/sqlite/client.py` & `RogueORM-0.0.2/rogue/backends/sqlite/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-from backends.base import BaseDatabaseClient
+from ..base import BaseDatabaseClient
 import sqlite3
 
+from ..errors import OperationalError
+
 
 class DatabaseClient(BaseDatabaseClient):
     def get_connection(self):
         if self._connection is None:
             self._connection = sqlite3.connect(self._db_name)
 
         return self._connection
 
-    def execute(self, statement, *args):
+    def execute(self, statement, args=()):
         connection = self.get_connection()
-        data = connection.execute(statement, args)
+        cursor = connection.cursor()
+        data = cursor.execute(statement, args)
         connection.commit()
 
         return data
 
     def close(self):
         self.get_connection().close()
```


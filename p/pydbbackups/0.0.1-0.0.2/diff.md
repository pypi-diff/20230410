# Comparing `tmp/pydbbackups-0.0.1.tar.gz` & `tmp/pydbbackups-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydbbackups-0.0.1.tar", max compression
+gzip compressed data, was "pydbbackups-0.0.2.tar", max compression
```

## Comparing `pydbbackups-0.0.1.tar` & `pydbbackups-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      707 2023-04-10 16:47:47.047593 pydbbackups-0.0.1/README.md
--rw-r--r--   0        0        0      394 2023-04-09 16:37:42.039199 pydbbackups-0.0.1/pydbbackups/__init__.py
--rw-r--r--   0        0        0       85 2023-03-26 16:35:39.235013 pydbbackups-0.0.1/pydbbackups/backups/__init__.py
--rw-r--r--   0        0        0     1474 2023-04-09 16:37:28.839768 pydbbackups-0.0.1/pydbbackups/backups/base.py
--rw-r--r--   0        0        0      776 2023-04-04 15:17:50.157968 pydbbackups-0.0.1/pydbbackups/backups/mongodb.py
--rw-r--r--   0        0        0     1201 2023-04-10 14:23:53.741447 pydbbackups-0.0.1/pydbbackups/backups/postgres.py
--rw-r--r--   0        0        0        0 2023-04-09 16:28:12.507897 pydbbackups-0.0.1/pydbbackups/cli/__init__.py
--rw-r--r--   0        0        0      475 2023-04-04 15:26:47.389488 pydbbackups-0.0.1/pydbbackups/cli/config.py
--rw-r--r--   0        0        0     1680 2023-04-10 16:43:42.903888 pydbbackups-0.0.1/pydbbackups/cli/main.py
--rw-r--r--   0        0        0       27 2023-04-04 15:31:15.953085 pydbbackups-0.0.1/pydbbackups/cli/models/__init__.py
--rw-r--r--   0        0        0      325 2023-04-09 16:07:03.941354 pydbbackups-0.0.1/pydbbackups/cli/models/backup_data.py
--rw-r--r--   0        0        0       36 2023-04-09 18:03:20.321476 pydbbackups-0.0.1/pydbbackups/cli/services/__init__.py
--rw-r--r--   0        0        0     1715 2023-04-10 14:38:28.130620 pydbbackups-0.0.1/pydbbackups/cli/services/backups.py
--rw-r--r--   0        0        0     1453 2023-04-10 16:49:51.999547 pydbbackups-0.0.1/pydbbackups/cli/utils/__init__.py
--rw-r--r--   0        0        0      526 2023-04-09 16:37:14.487168 pydbbackups-0.0.1/pydbbackups/errors.py
--rw-r--r--   0        0        0      461 2023-04-09 16:41:56.089458 pydbbackups-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1181 1970-01-01 00:00:00.000000 pydbbackups-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      761 2023-04-10 17:17:51.024476 pydbbackups-0.0.2/README.md
+-rw-r--r--   0        0        0      394 2023-04-09 16:37:42.039199 pydbbackups-0.0.2/pydbbackups/__init__.py
+-rw-r--r--   0        0        0       85 2023-03-26 16:35:39.235013 pydbbackups-0.0.2/pydbbackups/backups/__init__.py
+-rw-r--r--   0        0        0     1474 2023-04-09 16:37:28.839768 pydbbackups-0.0.2/pydbbackups/backups/base.py
+-rw-r--r--   0        0        0      776 2023-04-04 15:17:50.157968 pydbbackups-0.0.2/pydbbackups/backups/mongodb.py
+-rw-r--r--   0        0        0     1201 2023-04-10 14:23:53.741447 pydbbackups-0.0.2/pydbbackups/backups/postgres.py
+-rw-r--r--   0        0        0        0 2023-04-09 16:28:12.507897 pydbbackups-0.0.2/pydbbackups/cli/__init__.py
+-rw-r--r--   0        0        0      475 2023-04-04 15:26:47.389488 pydbbackups-0.0.2/pydbbackups/cli/config.py
+-rw-r--r--   0        0        0     1680 2023-04-10 16:43:42.903888 pydbbackups-0.0.2/pydbbackups/cli/main.py
+-rw-r--r--   0        0        0       27 2023-04-04 15:31:15.953085 pydbbackups-0.0.2/pydbbackups/cli/models/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-09 16:07:03.941354 pydbbackups-0.0.2/pydbbackups/cli/models/backup_data.py
+-rw-r--r--   0        0        0       36 2023-04-09 18:03:20.321476 pydbbackups-0.0.2/pydbbackups/cli/services/__init__.py
+-rw-r--r--   0        0        0     1715 2023-04-10 14:38:28.130620 pydbbackups-0.0.2/pydbbackups/cli/services/backups.py
+-rw-r--r--   0        0        0     1453 2023-04-10 16:49:51.999547 pydbbackups-0.0.2/pydbbackups/cli/utils/__init__.py
+-rw-r--r--   0        0        0      526 2023-04-09 16:37:14.487168 pydbbackups-0.0.2/pydbbackups/errors.py
+-rw-r--r--   0        0        0      638 2023-04-10 17:52:45.155537 pydbbackups-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 pydbbackups-0.0.2/PKG-INFO
```

### Comparing `pydbbackups-0.0.1/pydbbackups/backups/base.py` & `pydbbackups-0.0.2/pydbbackups/backups/base.py`

 * *Files identical despite different names*

### Comparing `pydbbackups-0.0.1/pydbbackups/backups/mongodb.py` & `pydbbackups-0.0.2/pydbbackups/backups/mongodb.py`

 * *Files identical despite different names*

### Comparing `pydbbackups-0.0.1/pydbbackups/backups/postgres.py` & `pydbbackups-0.0.2/pydbbackups/backups/postgres.py`

 * *Files identical despite different names*

### Comparing `pydbbackups-0.0.1/pydbbackups/cli/main.py` & `pydbbackups-0.0.2/pydbbackups/cli/main.py`

 * *Files identical despite different names*

### Comparing `pydbbackups-0.0.1/pydbbackups/cli/services/backups.py` & `pydbbackups-0.0.2/pydbbackups/cli/services/backups.py`

 * *Files identical despite different names*

### Comparing `pydbbackups-0.0.1/pydbbackups/cli/utils/__init__.py` & `pydbbackups-0.0.2/pydbbackups/cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pydbbackups-0.0.1/pydbbackups/errors.py` & `pydbbackups-0.0.2/pydbbackups/errors.py`

 * *Files identical despite different names*

### Comparing `pydbbackups-0.0.1/PKG-INFO` & `pydbbackups-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 Metadata-Version: 2.1
 Name: pydbbackups
-Version: 0.0.1
+Version: 0.0.2
 Summary: DB backups handler
+Home-page: https://github.com/jbuendia1y/pydbbackups
+Keywords: backups,databases,handler,library,cli
 Author: jbuendia1y
 Author-email: jgamer669@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Requires-Dist: rich (>=13.3.3,<14.0.0)
+Project-URL: Repository, https://github.com/jbuendia1y/pydbbackups
 Description-Content-Type: text/markdown
 
 # PyDBBackups
 
 A backup handler
 
+## Installation
+
+```bash
+pip install pydbbackups
+```
+
 ## CLI example
 
 ```bash
 dbbackups run \
     --name backup-example \
     --database-type postgres \
     --host localhost \
```


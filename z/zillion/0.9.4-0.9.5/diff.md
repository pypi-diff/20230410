# Comparing `tmp/zillion-0.9.4.tar.gz` & `tmp/zillion-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zillion-0.9.4.tar", last modified: Mon Apr 10 13:30:56 2023, max compression
+gzip compressed data, was "zillion-0.9.5.tar", last modified: Mon Apr 10 14:09:45 2023, max compression
```

## Comparing `zillion-0.9.4.tar` & `zillion-0.9.5.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 13:30:56.819146 zillion-0.9.4/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      297 2022-07-15 16:01:20.000000 zillion-0.9.4/AUTHORS.md
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     7783 2022-07-15 16:01:20.000000 zillion-0.9.4/LICENSE
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    31693 2023-04-10 13:30:56.819146 zillion-0.9.4/PKG-INFO
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    31036 2023-04-04 15:42:18.000000 zillion-0.9.4/README.md
--rw-rw-r--   0 kurt      (1000) kurt      (1000)       38 2023-04-10 13:30:56.819146 zillion-0.9.4/setup.cfg
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     2859 2023-03-31 00:50:17.000000 zillion-0.9.4/setup.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 13:30:56.815146 zillion-0.9.4/zillion/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      507 2022-07-15 16:01:20.000000 zillion-0.9.4/zillion/__init__.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    51932 2023-03-28 16:19:04.000000 zillion-0.9.4/zillion/configs.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    13415 2023-04-01 17:19:44.000000 zillion-0.9.4/zillion/core.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    69321 2023-04-03 19:42:19.000000 zillion-0.9.4/zillion/datasource.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 13:30:56.819146 zillion-0.9.4/zillion/dialects/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)       91 2023-03-23 18:24:15.000000 zillion-0.9.4/zillion/dialects/__init__.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     6313 2022-07-15 16:01:20.000000 zillion-0.9.4/zillion/dialects/conversions.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     4677 2023-03-24 13:49:53.000000 zillion-0.9.4/zillion/dialects/duckdb.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     3700 2022-07-15 16:01:20.000000 zillion-0.9.4/zillion/dialects/mysql.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     4556 2022-07-15 16:01:20.000000 zillion-0.9.4/zillion/dialects/postgresql.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     4609 2022-07-15 16:01:20.000000 zillion-0.9.4/zillion/dialects/sqlite.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    53505 2023-03-23 18:23:26.000000 zillion-0.9.4/zillion/field.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     1718 2023-04-10 13:26:28.000000 zillion-0.9.4/zillion/model.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    36392 2023-04-04 15:47:25.000000 zillion-0.9.4/zillion/nlp.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    83878 2023-04-03 17:49:18.000000 zillion-0.9.4/zillion/report.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 13:30:56.819146 zillion-0.9.4/zillion/scripts/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)        0 2022-07-15 16:01:20.000000 zillion-0.9.4/zillion/scripts/__init__.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    15096 2023-04-04 14:54:06.000000 zillion-0.9.4/zillion/scripts/bootstrap_datasource_config.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      121 2022-07-15 16:01:20.000000 zillion-0.9.4/zillion/scripts/json_to_yaml.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     2478 2023-04-04 11:18:20.000000 zillion-0.9.4/zillion/scripts/run_report.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      109 2022-07-15 16:01:20.000000 zillion-0.9.4/zillion/scripts/yaml_to_json.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    16500 2023-04-03 19:12:41.000000 zillion-0.9.4/zillion/sql_utils.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)       44 2023-04-10 13:30:32.000000 zillion-0.9.4/zillion/version.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    39878 2023-04-04 01:10:26.000000 zillion-0.9.4/zillion/warehouse.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 13:30:56.815146 zillion-0.9.4/zillion.egg-info/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    31693 2023-04-10 13:30:56.000000 zillion-0.9.4/zillion.egg-info/PKG-INFO
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      737 2023-04-10 13:30:56.000000 zillion-0.9.4/zillion.egg-info/SOURCES.txt
--rw-rw-r--   0 kurt      (1000) kurt      (1000)        1 2023-04-10 13:30:56.000000 zillion-0.9.4/zillion.egg-info/dependency_links.txt
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     1050 2023-04-10 13:30:56.000000 zillion-0.9.4/zillion.egg-info/requires.txt
--rw-rw-r--   0 kurt      (1000) kurt      (1000)        8 2023-04-10 13:30:56.000000 zillion-0.9.4/zillion.egg-info/top_level.txt
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 14:09:45.094051 zillion-0.9.5/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      297 2022-07-15 16:01:20.000000 zillion-0.9.5/AUTHORS.md
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     7783 2022-07-15 16:01:20.000000 zillion-0.9.5/LICENSE
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    31693 2023-04-10 14:09:45.094051 zillion-0.9.5/PKG-INFO
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    31036 2023-04-04 15:42:18.000000 zillion-0.9.5/README.md
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)       38 2023-04-10 14:09:45.094051 zillion-0.9.5/setup.cfg
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     2859 2023-03-31 00:50:17.000000 zillion-0.9.5/setup.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 14:09:45.094051 zillion-0.9.5/zillion/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      507 2022-07-15 16:01:20.000000 zillion-0.9.5/zillion/__init__.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    51932 2023-03-28 16:19:04.000000 zillion-0.9.5/zillion/configs.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    13415 2023-04-01 17:19:44.000000 zillion-0.9.5/zillion/core.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    69368 2023-04-10 14:08:30.000000 zillion-0.9.5/zillion/datasource.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 14:09:45.094051 zillion-0.9.5/zillion/dialects/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)       91 2023-03-23 18:24:15.000000 zillion-0.9.5/zillion/dialects/__init__.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     6313 2022-07-15 16:01:20.000000 zillion-0.9.5/zillion/dialects/conversions.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     4677 2023-03-24 13:49:53.000000 zillion-0.9.5/zillion/dialects/duckdb.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     3700 2022-07-15 16:01:20.000000 zillion-0.9.5/zillion/dialects/mysql.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     4556 2022-07-15 16:01:20.000000 zillion-0.9.5/zillion/dialects/postgresql.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     4609 2022-07-15 16:01:20.000000 zillion-0.9.5/zillion/dialects/sqlite.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    53505 2023-03-23 18:23:26.000000 zillion-0.9.5/zillion/field.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     1718 2023-04-10 13:26:28.000000 zillion-0.9.5/zillion/model.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    36392 2023-04-04 15:47:25.000000 zillion-0.9.5/zillion/nlp.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    83878 2023-04-03 17:49:18.000000 zillion-0.9.5/zillion/report.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 14:09:45.094051 zillion-0.9.5/zillion/scripts/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)        0 2022-07-15 16:01:20.000000 zillion-0.9.5/zillion/scripts/__init__.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    15096 2023-04-04 14:54:06.000000 zillion-0.9.5/zillion/scripts/bootstrap_datasource_config.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      121 2022-07-15 16:01:20.000000 zillion-0.9.5/zillion/scripts/json_to_yaml.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     1241 2023-04-10 13:55:59.000000 zillion-0.9.5/zillion/scripts/load_config.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     2478 2023-04-04 11:18:20.000000 zillion-0.9.5/zillion/scripts/run_report.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      109 2022-07-15 16:01:20.000000 zillion-0.9.5/zillion/scripts/yaml_to_json.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    16500 2023-04-03 19:12:41.000000 zillion-0.9.5/zillion/sql_utils.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)       44 2023-04-10 14:09:06.000000 zillion-0.9.5/zillion/version.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    39878 2023-04-04 01:10:26.000000 zillion-0.9.5/zillion/warehouse.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-10 14:09:45.094051 zillion-0.9.5/zillion.egg-info/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    31693 2023-04-10 14:09:45.000000 zillion-0.9.5/zillion.egg-info/PKG-INFO
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      768 2023-04-10 14:09:45.000000 zillion-0.9.5/zillion.egg-info/SOURCES.txt
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)        1 2023-04-10 14:09:45.000000 zillion-0.9.5/zillion.egg-info/dependency_links.txt
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     1050 2023-04-10 14:09:45.000000 zillion-0.9.5/zillion.egg-info/requires.txt
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)        8 2023-04-10 14:09:45.000000 zillion-0.9.5/zillion.egg-info/top_level.txt
```

### Comparing `zillion-0.9.4/LICENSE` & `zillion-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zillion-0.9.4/PKG-INFO` & `zillion-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillion
-Version: 0.9.4
+Version: 0.9.5
 Summary: Make sense of it all.
 Home-page: https://github.com/totalhack/zillion
 Author: totalhack
 Author-email: none@none.com
 Maintainer: totalhack
 License: LGPLv3
 Platform: UNKNOWN
```

### Comparing `zillion-0.9.4/README.md` & `zillion-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `zillion-0.9.4/setup.py` & `zillion-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.4/zillion/configs.py` & `zillion-0.9.5/zillion/configs.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.4/zillion/core.py` & `zillion-0.9.5/zillion/core.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.4/zillion/datasource.py` & `zillion-0.9.5/zillion/datasource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1606,14 +1606,15 @@
         **kwargs,
     ):
         """Initializes the datatable by parsing its config, but does not
         actually add it to a particular DB yet. It is assumed the DataSource
         will do that later.
         """
         self.df_kwargs = kwargs or {}
+        self.fillna_value = fillna_value or ""
 
         self.primary_key_columns = None
         if primary_key:
             if not columns:
                 # Assume specified primary key fields match column names
                 self.primary_key_columns = self.primary_key
             else:
```

### Comparing `zillion-0.9.4/zillion/dialects/conversions.py` & `zillion-0.9.5/zillion/dialects/conversions.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.4/zillion/dialects/duckdb.py` & `zillion-0.9.5/zillion/dialects/duckdb.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.4/zillion/dialects/mysql.py` & `zillion-0.9.5/zillion/dialects/mysql.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.4/zillion/dialects/postgresql.py` & `zillion-0.9.5/zillion/dialects/postgresql.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.4/zillion/dialects/sqlite.py` & `zillion-0.9.5/zillion/dialects/sqlite.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.4/zillion/field.py` & `zillion-0.9.5/zillion/field.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.4/zillion/model.py` & `zillion-0.9.5/zillion/model.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.4/zillion/nlp.py` & `zillion-0.9.5/zillion/nlp.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.4/zillion/report.py` & `zillion-0.9.5/zillion/report.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.4/zillion/scripts/bootstrap_datasource_config.py` & `zillion-0.9.5/zillion/scripts/bootstrap_datasource_config.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.4/zillion/scripts/run_report.py` & `zillion-0.9.5/zillion/scripts/run_report.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.4/zillion/sql_utils.py` & `zillion-0.9.5/zillion/sql_utils.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.4/zillion/warehouse.py` & `zillion-0.9.5/zillion/warehouse.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.4/zillion.egg-info/PKG-INFO` & `zillion-0.9.5/zillion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillion
-Version: 0.9.4
+Version: 0.9.5
 Summary: Make sense of it all.
 Home-page: https://github.com/totalhack/zillion
 Author: totalhack
 Author-email: none@none.com
 Maintainer: totalhack
 License: LGPLv3
 Platform: UNKNOWN
```

### Comparing `zillion-0.9.4/zillion.egg-info/SOURCES.txt` & `zillion-0.9.5/zillion.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,9 +23,10 @@
 zillion/dialects/duckdb.py
 zillion/dialects/mysql.py
 zillion/dialects/postgresql.py
 zillion/dialects/sqlite.py
 zillion/scripts/__init__.py
 zillion/scripts/bootstrap_datasource_config.py
 zillion/scripts/json_to_yaml.py
+zillion/scripts/load_config.py
 zillion/scripts/run_report.py
 zillion/scripts/yaml_to_json.py
```

### Comparing `zillion-0.9.4/zillion.egg-info/requires.txt` & `zillion-0.9.5/zillion.egg-info/requires.txt`

 * *Files identical despite different names*


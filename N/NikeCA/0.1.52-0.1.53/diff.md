# Comparing `tmp/NikeCA-0.1.52.tar.gz` & `tmp/NikeCA-0.1.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.52.tar", last modified: Mon Apr 10 17:23:51 2023, max compression
+gzip compressed data, was "NikeCA-0.1.53.tar", last modified: Mon Apr 10 21:05:29 2023, max compression
```

## Comparing `NikeCA-0.1.52.tar` & `NikeCA-0.1.53.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-10 17:23:51.698516 NikeCA-0.1.52/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-02-18 07:46:56.000000 NikeCA-0.1.52/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-10 17:23:51.697898 NikeCA-0.1.52/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-03-15 23:26:31.000000 NikeCA-0.1.52/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-10 17:23:51.698633 NikeCA-0.1.52/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2254 2023-04-10 17:23:20.000000 NikeCA-0.1.52/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-10 17:23:51.694941 NikeCA-0.1.52/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-10 17:23:51.697240 NikeCA-0.1.52/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-10 17:23:51.000000 NikeCA-0.1.52/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      426 2023-04-10 17:23:51.000000 NikeCA-0.1.52/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-10 17:23:51.000000 NikeCA-0.1.52/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-10 17:23:51.000000 NikeCA-0.1.52/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      147 2023-04-10 17:23:51.000000 NikeCA-0.1.52/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)       92 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    19846 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3710 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/_IMPSummaryDashboard.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3205 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13952 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     6490 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7240 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-10 16:40:29.000000 NikeCA-0.1.52/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-10 21:05:29.580062 NikeCA-0.1.53/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-02-18 07:46:56.000000 NikeCA-0.1.53/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-10 21:05:29.579571 NikeCA-0.1.53/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-03-15 23:26:31.000000 NikeCA-0.1.53/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-10 21:05:29.580186 NikeCA-0.1.53/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2254 2023-04-10 21:04:59.000000 NikeCA-0.1.53/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-10 21:05:29.576595 NikeCA-0.1.53/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-10 21:05:29.578920 NikeCA-0.1.53/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-10 21:05:29.000000 NikeCA-0.1.53/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      426 2023-04-10 21:05:29.000000 NikeCA-0.1.53/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-10 21:05:29.000000 NikeCA-0.1.53/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-10 21:05:29.000000 NikeCA-0.1.53/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      147 2023-04-10 21:05:29.000000 NikeCA-0.1.53/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)       92 2023-04-10 21:04:31.000000 NikeCA-0.1.53/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-10 21:04:31.000000 NikeCA-0.1.53/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    19706 2023-04-10 21:04:31.000000 NikeCA-0.1.53/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-10 21:04:31.000000 NikeCA-0.1.53/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-10 21:04:31.000000 NikeCA-0.1.53/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3702 2023-04-10 21:04:31.000000 NikeCA-0.1.53/src/_IMPSummaryDashboard.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-10 21:04:31.000000 NikeCA-0.1.53/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3205 2023-04-10 21:04:31.000000 NikeCA-0.1.53/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14125 2023-04-10 21:04:31.000000 NikeCA-0.1.53/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6490 2023-04-10 21:04:31.000000 NikeCA-0.1.53/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-10 21:04:31.000000 NikeCA-0.1.53/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-10 21:04:31.000000 NikeCA-0.1.53/src/__init__.py
```

### Comparing `NikeCA-0.1.52/LICENSE` & `NikeCA-0.1.53/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.52/PKG-INFO` & `NikeCA-0.1.53/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.52
+Version: 0.1.53
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.52/README.md` & `NikeCA-0.1.53/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.52/setup.py` & `NikeCA-0.1.53/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.52',
+	version='0.1.53',
 	description='Standardize and Automate processes utilized by the DAMs at Nike in CA',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"_IMPSummaryDashboard",
```

### Comparing `NikeCA-0.1.52/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.53/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.52
+Version: 0.1.53
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.52/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.53/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.52/src/NikeQA.py` & `NikeCA-0.1.53/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.52/src/NikeSF.py` & `NikeCA-0.1.53/src/NikeSF.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,19 +337,18 @@
             dtypes_conv = self.__dtypes_conv
         if not separate_dataframes:
             separate_dataframes = self.__separate_dataframes
         if not polars:
             polars = self.__polars
 
         # Call the snowflake_pull method from the _SnowflakeData module using the provided or default parameters
-        return SnowflakeData.snowflake_pull(self, query, un=username, wh=warehouse, db=database,
-                                                           role=role, schema=schema, table=table,
-                                                           sample_table=sample_table, sample_val=sample_val,
-                                                           table_sample=table_sample, dtypes_conv=dtypes_conv,
-                                                           separate_dataframes=separate_dataframes, polars=polars)
+        return SnowflakeData.snowflake_pull(self, query, un=username, wh=warehouse, db=database,role=role,
+                                            schema=schema, table=table, sample_table=sample_table,
+                                            sample_val=sample_val, table_sample=table_sample, dtypes_conv=dtypes_conv,
+                                            separate_dataframes=separate_dataframes, polars=polars)
 
     def search_schema(self,
                       username: str = None,
                       warehouse: str = None,
                       database: str = None,
                       role: str = None,
                       sample_table: bool = False,
@@ -409,20 +408,20 @@
         if col_and_or == 'and' and self.__col_and_or:
             col_and_or = self.__col_and_or
         if not get_ex_val and self.__get_ex_val:
             get_ex_val = self.__get_ex_val
         if not like_flag and self.__like_flag:
             like_flag = self.__like_flag
 
-        return _SnowflakeData.SnowflakeData.search_schema(self, un=username, wh=warehouse, db=database, role=role,
-                                                          sample_table=sample_table, sample_val=sample_val,
-                                                          table_sample=table_sample, dtypes_conv=dtypes_conv,
-                                                          schema=schema, table=table, column_name=column_name,
-                                                          col_and_or=col_and_or, get_ex_val=get_ex_val,
-                                                          like_flag=like_flag)
+        return SnowflakeData.search_schema(self, un=username, wh=warehouse, db=database, role=role,
+                                           sample_table=sample_table, sample_val=sample_val,
+                                           table_sample=table_sample, dtypes_conv=dtypes_conv,
+                                           schema=schema, table=table, column_name=column_name,
+                                           col_and_or=col_and_or, get_ex_val=get_ex_val,
+                                           like_flag=like_flag)
 
     def optimize_tbl_mem(self,
                          username: str | None = None,
                          warehouse: str | None = None,
                          role: str | None = None,
                          database: str | None = None,
                          schema: str | None = None,
@@ -452,15 +451,15 @@
         if warehouse is None:
             warehouse = self.__warehouse
         if role is None:
             role = self.__role
         if database is None:
             database = self.__database
 
-        return _SnowflakeData.SnowflakeData.optimize_tbl_mem(self, username=username, warehouse=warehouse, role=role,
+        return SnowflakeData.optimize_tbl_mem(self, username=username, warehouse=warehouse, role=role,
                                                              database=database, schema=schema, table_name=table_name,
                                                              pull_all_cols=pull_all_cols, run_debugging=run_debugging,
                                                              query=query)
 
     def snowflake_dependencies(self,
                                tables: str | list | None = None,
                                username: str | None = None,
@@ -493,26 +492,27 @@
         if database is None:
             database = self.__database
         if schema is None:
             schema = self.__schema
         if save_path is None:
             save_path = self.__save_path
 
-        return _SnowflakeData.SnowflakeData.snowflake_dependencies(self, tables=tables, username=username,
-                                                                   warehouse=warehouse, role=role, database=database,
-                                                                   schema=schema, save_path=save_path)
+        return SnowflakeData.snowflake_dependencies(self, tables=tables, username=username,
+                                                    warehouse=warehouse, role=role, database=database,
+                                                    schema=schema, save_path=save_path)
 
     def imp_summary_dashboard(self
                               , username: str | None = None
                               , warehouse: str | None = None
                               , database: str | None = None
                               , role: str | None = None
                               , date_min: str = '1900-01-01'
                               , date_max: str = '9999-12-31'
-                              , column_filters=None) -> pd.DataFrame:
+                              , column_filters=None
+                              , polars: bool = False):
 
         if username is None:
             username = self.__username
         if warehouse is None:
             warehouse = self.__warehouse
         if database is None:
             database = self.__database
@@ -520,14 +520,16 @@
             role = self.__role
         if date_min is None:
             date_min = self.__date_min
         if date_max is None:
             date_max = self.__date_max
         if column_filters is None:
             column_filters = self.__column_filters
+        if polars is False:
+            polars = self.__polars
 
         return IMPSummaryDashboard.imp_summary_dashboard(self, username=username, warehouse=warehouse, database=database
                                                          , role=role, date_min=date_min, date_max=date_max,
-                                                         column_filters=column_filters)
+                                                         column_filters=column_filters, polars=polars)
```

### Comparing `NikeCA-0.1.52/src/_BuildSearchQuery.py` & `NikeCA-0.1.53/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.52/src/_GitHub.py` & `NikeCA-0.1.53/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.52/src/_IMPSummaryDashboard.py` & `NikeCA-0.1.53/src/_IMPSummaryDashboard.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-import pandas as pd
-
 
 class IMPSummaryDashboard:
 
-    import pandas as pd
-
     def imp_summary_dashboard(self
                               , username: str
                               , warehouse: str
                               , database: str
                               , role: str
                               , date_min: str = '1900-01-01'
                               , date_max: str = '9999-12-31'
-                              , column_filters=None):
+                              , column_filters=None
+                              , polars: bool = False):
         """
         Generate a SQL query for a dashboard summary report with optional column filters.
 
         Args:
             date_min (str): The minimum activity end date to include in the report. Default is '1900-01-01'.
             date_max (str): The maximum activity end date to include in the report. Default is '9999-12-31'.
             column_filters (list): A list of column names to include in the query SELECT and GROUP BY clauses. Default
             is None.
 
         Returns:
             DataFrame: .
 
         Raises:
             TypeError: If date_min, date_max, or column_filters is not a string or list, respectively.
+            :param polars:
             :param column_filters:
             :param date_max:
             :param date_min:
             :param role:
             :param database:
             :param warehouse:
             :param username:
@@ -76,15 +74,14 @@
             , MAX({date_end}) AS MAX_{date_end}
             , {aggs}
         FROM 
             {table}
         WHERE
             {date} BETWEEN '{date_min}' AND '{date_max}'
             AND {column} = '{column_filter}'
-            AND {column_flag} = '{column_flag_answer}'
         {group_column_filters_str} 
         UNION
     
         SELECT
             {column_filters_str}
             MIN({date_begin}) AS MIN_{date_begin}
             , MAX({date_end}) AS MAX_{date_end}
@@ -97,9 +94,9 @@
             AND {column_flag} = '{column_flag_answer}'
         {group_column_filters_str}
         ;
         """
         print(query_dashboard)
 
         return Snowflake(username=username, warehouse=warehouse, database=database,
-                         role=role).snowflake_pull(query=query_dashboard)
+                         role=role).snowflake_pull(query=query_dashboard, polars=True)
```

### Comparing `NikeCA-0.1.52/src/_QA.py` & `NikeCA-0.1.53/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.52/src/_SearchFiles.py` & `NikeCA-0.1.53/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.52/src/_SnowflakeData.py` & `NikeCA-0.1.53/src/_SnowflakeData.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,19 +28,20 @@
 
         # --> pull data, filter out exclusions
         results = pd.DataFrame()
         if type(db) == list:
             queries = {}
 
             for k in db:
-                queries[k] = _BuildSearchQuery.build_search_query(inp_db=k, schema=schema, table=table,
-                                                                  column_name=column_name, like_flag=like_flag,
-                                                                  col_and_or=col_and_or)
+                queries[k] = _BuildSearchQuery.BuildSearchQuery.build_search_query(self, inp_db=k, schema=schema,
+                                                                                   table=table, column_name=column_name,
+                                                                                   like_flag=like_flag,
+                                                                                   col_and_or=col_and_or)
                 queries[k] = queries[k][:queries[k].find("INFORMATION_SCHEMA.COLUMNS")] + k + '.' + \
-                             queries[k][queries[k].find("INFORMATION_SCHEMA.COLUMNS"):]
+                    queries[k][queries[k].find("INFORMATION_SCHEMA.COLUMNS"):]
 
             df = _SnowflakePull.SnowflakePull.snowflake_pull(self, queries, un=un, wh=wh, role=role, db=None,
                                                              sample_table=sample_table, sample_val=sample_val,
                                                              table_sample=table_sample, dtypes_conv=dtypes_conv,
                                                              separate_dataframes=False)
 
             results = pd.concat([results, df], axis=0)
@@ -52,40 +53,40 @@
 
             # list of user's db names
             db_names = list(get_dbs['name'].values)
 
             print(f"No input database --> checking all of databases in user's access: {len(db_names)} total databases")
             queries = {}
             for db in db_names:
-                queries[db] = _BuildSearchQuery.build_search_query(inp_db=db, schema=schema, table=table,
-                                                                   column_name=column_name, like_flag=like_flag,
-                                                                   col_and_or=col_and_or)
+                queries[db] = _BuildSearchQuery.BuildSearchQuery.build_search_query(self, inp_db=db, schema=schema,
+                                                                                    table=table,
+                                                                                    column_name=column_name,
+                                                                                    like_flag=like_flag,
+                                                                                    col_and_or=col_and_or)
                 queries[db] = queries[db][:queries[db].find("INFORMATION_SCHEMA.COLUMNS")] + db + '.' + \
                               queries[db][queries[db].find("INFORMATION_SCHEMA.COLUMNS"):]
 
             temp_results = _SnowflakePull.SnowflakePull.snowflake_pull(self, query=queries, un=un, wh=wh, role=role,
                                                                        db=None,
                                                                        sample_table=sample_table, sample_val=sample_val,
                                                                        table_sample=table_sample,
                                                                        dtypes_conv=dtypes_conv,
                                                                        separate_dataframes=False)
 
             results = pd.concat([results, temp_results], axis=0)
         else:
             results = _SnowflakePull.SnowflakePull.snowflake_pull(
                 self,
-                query=_BuildSearchQuery.build_search_query(inp_db=db, schema=schema, table=table,
+                query=_BuildSearchQuery.BuildSearchQuery.build_search_query(inp_db=db, schema=schema, table=table,
                                                            column_name=column_name, like_flag=like_flag,
                                                            col_and_or=col_and_or),
                 un=un, db=db, wh=wh, role=role)
 
-        # exclude from table results
-        exclusions = ['TEST', 'BACKUP', 'BKUP', 'BCKUP', 'BCKP', '_OLD', 'UPDT', 'DELETED', 'FIX']
         # # drop exclusion rows
-        results_fin = results  # [~results['TABLE_NAME'].str.contains('|'.join(exclusions))].copy().reset_index(drop=True)
+        results_fin = results
 
         # --> print result statement
         print(f'''
             Total table-columns found: {len(results_fin)}    
 
             Unique column names found: {list(results_fin['COLUMN_NAME'].unique())}
             Total = {len(list(results_fin['COLUMN_NAME'].unique()))}
@@ -99,19 +100,20 @@
                 try:
                     row_res = _SnowflakePull.SnowflakePull.snowflake_pull(self, '', un=un, db=None, wh=wh, role=role,
                                                                           sample_val=True,
                                                                           table_sample={'db': row['TABLE_CATALOG'],
                                                                                         'schema': row['TABLE_SCHEMA'],
                                                                                         'table': row['TABLE_NAME'],
                                                                                         'col': row[
-                                                                                            'COLUMN_NAME']})  # row results
+                                                                                            'COLUMN_NAME']})
                     # set row example values equal to unique column value list
                     row['EX_VALS'] = list(row_res[row['COLUMN_NAME']].unique())
-                except:
+                except Exception as e:
                     print(f"Could not pull {row['COLUMN_NAME']} for table: {row['TABLE_NAME']}")
+                    print(e)
                     continue
 
         return results_fin
 
     def snowflake_dependencies(self, tables: str | list, username: str, warehouse: str, role: str,
                                database: str | None = None, schema: str | list | None = None, save_path: str = None):
```

### Comparing `NikeCA-0.1.52/src/_SnowflakeDependencies.py` & `NikeCA-0.1.53/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.52/src/_SnowflakePull.py` & `NikeCA-0.1.53/src/_SnowflakePull.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,18 +178,18 @@
 
             try:
                 cur.execute(query)  # execute sql, store into-->
 
             # final data pull --> allows datatype-memory optimization
                 df = pl.DataFrame
                 if polars:
-                    df = cur.fetch_arrow_all() if dtypes_conv is None else cur.fetchall().astype(dtypes_conv)
+                    df = cur.fetch_arrow_all()
 
                 else:
-                    df = cur.fetch_pandas_all() if dtypes_conv is None else cur.fetchall().astype(dtypes_conv)
+                    df = cur.fetch_pandas_all()
                 print(df)
 
             except snowflake.connector.errors.ProgrammingError:
                 print(f'Could not retrieve:\n\t {query}')
 
             except TypeError:
                 print(f"""Could not retrieve:\n\t{query}\n\nbecause TypeError: NoneType""")
```


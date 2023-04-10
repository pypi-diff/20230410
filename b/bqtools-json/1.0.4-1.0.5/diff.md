# Comparing `tmp/bqtools-json-1.0.4.tar.gz` & `tmp/bqtools-json-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bqtools-json-1.0.4.tar", last modified: Tue Dec  6 10:24:46 2022, max compression
+gzip compressed data, was "bqtools-json-1.0.5.tar", last modified: Mon Apr 10 19:50:43 2023, max compression
```

## Comparing `bqtools-json-1.0.4.tar` & `bqtools-json-1.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 10:24:46.888054 bqtools-json-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2022-12-06 10:24:30.000000 bqtools-json-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-06 10:24:30.000000 bqtools-json-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2022-12-06 10:24:46.888054 bqtools-json-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2022-12-06 10:24:30.000000 bqtools-json-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 10:24:46.884055 bqtools-json-1.0.4/bqtools/
--rw-r--r--   0 runner    (1001) docker     (123)   240196 2022-12-06 10:24:30.000000 bqtools-json-1.0.4/bqtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-06 10:24:30.000000 bqtools-json-1.0.4/bqtools/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13756 2022-12-06 10:24:30.000000 bqtools-json-1.0.4/bqtools/bqsync
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 10:24:46.884055 bqtools-json-1.0.4/bqtools/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2022-12-06 10:24:30.000000 bqtools-json-1.0.4/bqtools/templates/bqschema.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 10:24:46.888054 bqtools-json-1.0.4/bqtools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-06 10:24:30.000000 bqtools-json-1.0.4/bqtools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1611146 2022-12-06 10:24:30.000000 bqtools-json-1.0.4/bqtools/tests/monsterSchema.json
--rw-r--r--   0 runner    (1001) docker     (123)      276 2022-12-06 10:24:30.000000 bqtools-json-1.0.4/bqtools/tests/schema2startnobare.json
--rw-r--r--   0 runner    (1001) docker     (123)      285 2022-12-06 10:24:30.000000 bqtools-json-1.0.4/bqtools/tests/schemaTest1.json
--rw-r--r--   0 runner    (1001) docker     (123)      351 2022-12-06 10:24:30.000000 bqtools-json-1.0.4/bqtools/tests/schemaTest2.json
--rw-r--r--   0 runner    (1001) docker     (123)      506 2022-12-06 10:24:30.000000 bqtools-json-1.0.4/bqtools/tests/schemaTest2bare.json
--rw-r--r--   0 runner    (1001) docker     (123)      488 2022-12-06 10:24:30.000000 bqtools-json-1.0.4/bqtools/tests/schemaTest2nonbare.json
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2022-12-06 10:24:30.000000 bqtools-json-1.0.4/bqtools/tests/schemaTest3.json
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2022-12-06 10:24:30.000000 bqtools-json-1.0.4/bqtools/tests/schemaTest4.json
--rw-r--r--   0 runner    (1001) docker     (123)   199404 2022-12-06 10:24:30.000000 bqtools-json-1.0.4/bqtools/tests/test_bqtools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 10:24:46.888054 bqtools-json-1.0.4/bqtools_json.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2022-12-06 10:24:46.000000 bqtools-json-1.0.4/bqtools_json.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      626 2022-12-06 10:24:46.000000 bqtools-json-1.0.4/bqtools_json.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 10:24:46.000000 bqtools-json-1.0.4/bqtools_json.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2022-12-06 10:24:46.000000 bqtools-json-1.0.4/bqtools_json.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-06 10:24:46.000000 bqtools-json-1.0.4/bqtools_json.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-06 10:24:46.888054 bqtools-json-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2022-12-06 10:24:30.000000 bqtools-json-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:50:43.173325 bqtools-json-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-10 19:50:33.000000 bqtools-json-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 19:50:33.000000 bqtools-json-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-10 19:50:43.173325 bqtools-json-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-10 19:50:33.000000 bqtools-json-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:50:43.169325 bqtools-json-1.0.5/bqtools/
+-rw-r--r--   0 runner    (1001) docker     (123)   246951 2023-04-10 19:50:33.000000 bqtools-json-1.0.5/bqtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-10 19:50:33.000000 bqtools-json-1.0.5/bqtools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13756 2023-04-10 19:50:33.000000 bqtools-json-1.0.5/bqtools/bqsync
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:50:43.169325 bqtools-json-1.0.5/bqtools/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-10 19:50:33.000000 bqtools-json-1.0.5/bqtools/templates/bqschema.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:50:43.169325 bqtools-json-1.0.5/bqtools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-10 19:50:33.000000 bqtools-json-1.0.5/bqtools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1611146 2023-04-10 19:50:33.000000 bqtools-json-1.0.5/bqtools/tests/monsterSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-10 19:50:33.000000 bqtools-json-1.0.5/bqtools/tests/schema2startnobare.json
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-10 19:50:33.000000 bqtools-json-1.0.5/bqtools/tests/schemaTest1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-10 19:50:33.000000 bqtools-json-1.0.5/bqtools/tests/schemaTest2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-10 19:50:33.000000 bqtools-json-1.0.5/bqtools/tests/schemaTest2bare.json
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-10 19:50:33.000000 bqtools-json-1.0.5/bqtools/tests/schemaTest2nonbare.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-04-10 19:50:33.000000 bqtools-json-1.0.5/bqtools/tests/schemaTest3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-04-10 19:50:33.000000 bqtools-json-1.0.5/bqtools/tests/schemaTest4.json
+-rw-r--r--   0 runner    (1001) docker     (123)   199404 2023-04-10 19:50:33.000000 bqtools-json-1.0.5/bqtools/tests/test_bqtools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:50:43.173325 bqtools-json-1.0.5/bqtools_json.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-10 19:50:43.000000 bqtools-json-1.0.5/bqtools_json.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-10 19:50:43.000000 bqtools-json-1.0.5/bqtools_json.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:50:43.000000 bqtools-json-1.0.5/bqtools_json.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-10 19:50:43.000000 bqtools-json-1.0.5/bqtools_json.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 19:50:43.000000 bqtools-json-1.0.5/bqtools_json.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:50:43.173325 bqtools-json-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-10 19:50:33.000000 bqtools-json-1.0.5/setup.py
```

### Comparing `bqtools-json-1.0.4/LICENSE` & `bqtools-json-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bqtools-json-1.0.4/PKG-INFO` & `bqtools-json-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqtools-json
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Big Query json utility package
 Home-page: https://github.com/hsbc/bqtools
 Author: HSBC
 Author-email: opensource@hsbc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bqtools-json-1.0.4/README.md` & `bqtools-json-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bqtools-json-1.0.4/bqtools/__init__.py` & `bqtools-json-1.0.5/bqtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,22 +137,35 @@
   routine_name as table_name,"ROUTINE" as type,last_altered as creation_time
 FROM
    `{0}.{1}.INFORMATION_SCHEMA.ROUTINES`
 ORDER BY
   creation_time
 """
 
+FUNCCOMPARE = """SELECT
+  routine_name,
+  routine_body,
+  routine_type,
+  data_type,
+  routine_definition
+FROM
+  `{0}.{1}.INFORMATION_SCHEMA.ROUTINES`
+WHERE routine_type = "FUNCTION"
+ORDER BY
+  1"""
+
 RTNCOMPARE = """SELECT
   routine_name,
   routine_body,
   routine_type,
   data_type,
   routine_definition
 FROM
   `{0}.{1}.INFORMATION_SCHEMA.ROUTINES`
+WHERE routine_type != "FUNCTION"
 ORDER BY
   1"""
 
 # map of partitioning types to decorator format for from time
 PARTITIONING_BY_TIME = {
         "DAY":   "%Y%m%d",
         "YEAR":  "%Y",
@@ -3113,14 +3126,18 @@
         view_definition = view_definition.replace(
             r'[{}:{}.'.format(self.source_project, self.source_dataset),
             "[{}:{}.".format(self.destination_project, self.destination_dataset))
         # this should not be required but seems it is
         view_definition = view_definition.replace(
             r'[{}.{}.'.format(self.source_project, self.source_dataset),
             "[{}:{}.".format(self.destination_project, self.destination_dataset))
+        # support short names
+        view_definition = view_definition.replace(
+            r'{}.'.format(self.source_dataset),
+            "{}.".format(self.destination_dataset))
 
         return view_definition
 
     def calculate_target_cmek_config(self, encryption_config):
         assert isinstance(encryption_config,
                           bigquery.EncryptionConfiguration) or (
                        getattr(self.destination_dataset_impl,
@@ -3761,14 +3778,18 @@
             view_definition = view_definition.replace(
                 r'[{}:{}.'.format(src_proj, src_dataset),
                 "[{}:{}.".format(dst_proj, dst_dataset))
             # this should not be required but seems it is
             view_definition = view_definition.replace(
                 r'[{}.{}.'.format(src_proj, src_dataset),
                 "[{}:{}.".format(dst_proj, dst_dataset))
+            # this should not be required but seems it is
+            view_definition = view_definition.replace(
+                r'{}.'.format(src_dataset),
+                "{}.".format(dst_dataset))
         return view_definition
 
 
 class MultiBQSyncDriver(DefaultBQSyncDriver):
     def __init__(self, srcproject, srcdataset, dstdataset, dstproject=None,
                  srcbucket=None, dstbucket=None, remove_deleted_tables=True,
                  copy_data=True,
@@ -3809,24 +3830,29 @@
         return self.__coordinater
 
     @coordinater.setter
     def coordinater(self, value):
         self.__coordinater = value
 
     def real_update_source_view_definition(self, view_definition, use_standard_sql):
+        # long form
         view_definition = view_definition.replace(
             r'`{}.{}.'.format(self.source_project, self.source_dataset),
             "`{}.{}.".format(self.destination_project, self.destination_dataset))
         view_definition = view_definition.replace(
             r'[{}:{}.'.format(self.source_project, self.source_dataset),
             "[{}:{}.".format(self.destination_project, self.destination_dataset))
         # this should not be required but seems it is
         view_definition = view_definition.replace(
             r'[{}.{}.'.format(self.source_project, self.source_dataset),
             "[{}:{}.".format(self.destination_project, self.destination_dataset))
+        # short form
+        view_definition = view_definition.replace(
+            r'{}.'.format(self.source_dataset),
+            "{}.".format(self.destination_dataset))
         return view_definition
 
     def discovery_update_table(self, table_api_rep, logging):
         bqservice = discovery.build(
             'bigquery', 
             'v2',
             static_discovery=False)
@@ -5023,15 +5049,18 @@
 
 def remove_deleted_destination_routine(copy_driver, routine_name):
     # handle old libraries with no routine support
     if getattr(bigquery, "Routine", None):
         dstroutine_ref = bigquery.Routine(
             "{}.{}.{}".format(copy_driver.destination_project, copy_driver.destination_dataset,
                               routine_name))
-        copy_driver.destination_client.delete_routine(dstroutine_ref)
+        try:
+            copy_driver.destination_client.delete_routine(dstroutine_ref)
+        except exceptions.NotFound as e:
+            pass
     else:
         copy_driver.get_logger().warning(
             "Unable to remove routine from source {}.{}.{} as Routine class not defined in "
             "bigquery library in the current python environment".format(
                 copy_driver.destination_project,
                 copy_driver.destination_dataset,
                 routine_name))
@@ -5063,15 +5092,22 @@
         dstroutine_ref.description = srcroutine.description
         dstroutine_ref.body = routine_input["routine_definition"]
         dstroutine_ref.return_type = srcroutine.return_type
         dstroutine_ref.arguments = srcroutine.arguments
         dstroutine_ref.imported_libraries = srcroutine.imported_libraries
         dstroutine_ref.language = srcroutine.language
         dstroutine_ref.type_ = srcroutine.type_
-        dstroutine = copy_driver.destination_client.create_routine(dstroutine_ref)
+        try:
+            dstroutine = copy_driver.destination_client.create_routine(dstroutine_ref)
+
+        # normally as referencing a routine not created
+        # so we accept this on basis next sync will resolve
+        except exceptions.BadRequest as e:
+            copy_driver.get_logger().exception(f"Unable to create routine {routine_name} in {copy_driver.destination_project}.{copy_driver.destination_dataset} definition {routine_input['routine_definition']}")
+            return
         return dstroutine
     else:
         copy_driver.get_logger().warning(
             "Unable to copy Routine {}.{}.{} as current python environment big query library does "
             "not support Routines".format(copy_driver.source_project, copy_driver.source_dataset,
                                           routine_name))
         copy_driver.increment_routines_failed_sync()
@@ -5380,16 +5416,16 @@
                 try:
                     destination_row = next(destination_generator)
                 except StopIteration:
                     destination_ended = True
 
         wait_for_queue(schema_q, "Materialized view sychronization", 0.3, copy_driver.get_logger())
 
+    # scalar functions have to be copied in case in views
     if "VIEW" in copy_driver.copy_types or "ROUTINE" in copy_driver.copy_types:
-
         # Now do views
         # views need applying in order
         # we assume order created is the order
         view_or_routine_order = []
 
         views_to_apply = {}
         routines_to_apply = {}
@@ -5402,14 +5438,115 @@
                                  "List views in apply order",
                                  location=copy_driver.source_location,
                                  callback_on_complete=copy_driver.update_job_stats,
                                  labels=BQSYNCQUERYLABELS,
                                  query_cmek=copy_driver.query_cmek[1]):
             view_or_routine_order.append(viewrow["table_name"])
 
+        # now list and compare views
+        source_routine_query = FUNCCOMPARE.format(copy_driver.source_project,
+                                                 copy_driver.source_dataset)
+        destination_routine_query = FUNCCOMPARE.format(copy_driver.destination_project,
+                                                      copy_driver.destination_dataset)
+        source_ended = False
+        destination_ended = False
+
+        source_generator = run_query(copy_driver.query_client, source_routine_query,
+                                     "List source functions", copy_driver.get_logger(),
+                                     location=copy_driver.source_location,
+                                     callback_on_complete=copy_driver.update_job_stats,
+                                     labels=BQSYNCQUERYLABELS,
+                                     query_cmek=copy_driver.query_cmek[1])
+        try:
+            source_row = next(source_generator)
+        except StopIteration:
+            source_ended = True
+
+        destination_generator = run_query(copy_driver.query_client, destination_routine_query,
+                                          copy_driver.get_logger(),
+                                          "List destination functions",
+                                          location=copy_driver.destination_location,
+                                          callback_on_complete=copy_driver.update_job_stats,
+                                          labels=BQSYNCQUERYLABELS,
+                                          query_cmek=copy_driver.query_cmek[0])
+        try:
+            destination_row = next(destination_generator)
+        except StopIteration:
+            destination_ended = True
+
+        while not source_ended or not destination_ended:
+            if not destination_ended and not source_ended and destination_row["routine_name"] \
+                    == \
+                    source_row["routine_name"]:
+                if copy_driver.istableincluded(source_row["routine_name"]):
+                    copy_driver.increment_routines_synced()
+                    expected_definition = copy_driver.update_source_view_definition(
+                        source_row["routine_definition"], source_row["routine_type"])
+                    if expected_definition != destination_row["routine_definition"]:
+                        routines_to_apply[source_row["routine_name"]] = {
+                            "routine_definition": expected_definition,
+                            "routine_type": source_row["routine_type"],
+                            "action": "patch_routine"}
+                    else:
+                        copy_driver.increment_routines_avoided()
+                try:
+                    source_row = next(source_generator)
+                except StopIteration:
+                    source_ended = True
+                try:
+                    destination_row = next(destination_generator)
+                except StopIteration:
+                    destination_ended = True
+            elif (destination_ended and not source_ended) or (
+                    not source_ended and source_row["routine_name"] < destination_row[
+                "routine_name"]):
+                if copy_driver.istableincluded(source_row["routine_name"]):
+                    copy_driver.increment_routines_synced()
+                    expected_definition = copy_driver.update_source_view_definition(
+                        source_row["routine_definition"], source_row["routine_type"])
+                    routines_to_apply[source_row["routine_name"]] = {
+                        "routine_definition": expected_definition,
+                        "routine_type": source_row["routine_type"], "action": "create_routine"}
+                try:
+                    source_row = next(source_generator)
+                except StopIteration:
+                    source_ended = True
+            elif (source_ended and not destination_ended) or (
+                    not destination_ended and source_row["routine_name"] > destination_row[
+                "routine_name"]):
+                remove_deleted_destination_routine(copy_driver, destination_row["routine_name"])
+                try:
+                    destination_row = next(destination_generator)
+                except StopIteration:
+                    destination_ended = True
+
+        for view in view_or_routine_order:
+            if view in routines_to_apply:
+                if routines_to_apply[view]["action"] == "create_routine":
+                    create_destination_routine(copy_driver, view, routines_to_apply[view])
+                else:
+                    patch_destination_routine(copy_driver, view, routines_to_apply[view])
+            if view in views_to_apply:
+                if views_to_apply[view]["action"] == "create_view":
+                    create_destination_view(copy_driver, view, views_to_apply[view])
+                else:
+                    patch_destination_view(copy_driver, view, views_to_apply[view])
+
+        wait_for_queue(schema_q, "View/Routine schema synchronization", 0.3,
+                       copy_driver.get_logger())
+
+    if "VIEW" in copy_driver.copy_types or "ROUTINE" in copy_driver.copy_types:
+
+        # Now do views
+        # views need applying in order
+        # we assume order created is the order
+
+        views_to_apply = {}
+        routines_to_apply = {}
+
         if "VIEW" in copy_driver.copy_types:
             # now list and compare views
             source_view_query = DSVIEWLISTQUERY.format(copy_driver.source_project,
                                                        copy_driver.source_dataset)
             destination_view_query = DSVIEWLISTQUERY.format(copy_driver.destination_project,
                                                             copy_driver.destination_dataset)
             source_ended = False
```

### Comparing `bqtools-json-1.0.4/bqtools/bqsync` & `bqtools-json-1.0.5/bqtools/bqsync`

 * *Files identical despite different names*

### Comparing `bqtools-json-1.0.4/bqtools/templates/bqschema.in` & `bqtools-json-1.0.5/bqtools/templates/bqschema.in`

 * *Files identical despite different names*

### Comparing `bqtools-json-1.0.4/bqtools/tests/monsterSchema.json` & `bqtools-json-1.0.5/bqtools/tests/monsterSchema.json`

 * *Files identical despite different names*

### Comparing `bqtools-json-1.0.4/bqtools/tests/schemaTest3.json` & `bqtools-json-1.0.5/bqtools/tests/schemaTest3.json`

 * *Files identical despite different names*

### Comparing `bqtools-json-1.0.4/bqtools/tests/schemaTest4.json` & `bqtools-json-1.0.5/bqtools/tests/schemaTest4.json`

 * *Files identical despite different names*

### Comparing `bqtools-json-1.0.4/bqtools/tests/test_bqtools.py` & `bqtools-json-1.0.5/bqtools/tests/test_bqtools.py`

 * *Files identical despite different names*

### Comparing `bqtools-json-1.0.4/bqtools_json.egg-info/PKG-INFO` & `bqtools-json-1.0.5/bqtools_json.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqtools-json
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Big Query json utility package
 Home-page: https://github.com/hsbc/bqtools
 Author: HSBC
 Author-email: opensource@hsbc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bqtools-json-1.0.4/bqtools_json.egg-info/SOURCES.txt` & `bqtools-json-1.0.5/bqtools_json.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bqtools-json-1.0.4/setup.py` & `bqtools-json-1.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,17 +36,16 @@
     packages=setuptools.find_packages(),
     test_suite='nose.collector',
     tests_require=['nose',
                    "deepdiff>=3.3.0,<6.0"],
     include_package_data=True,
     scripts=['bqtools/bqsync'],
     install_requires=[
-        "jinja2<3.0",
+        "jinja2>=2.0,<4.0",
         "google-cloud<1.0",
-        "datetime<5.0",
         "google-cloud-bigquery>=2.6.0,<3.0",
         "google-cloud-storage>=1.0.0,<3.0",
         "google-cloud-logging>=3.0,<4.0",
         "absl-py~=1.0",
         "boto<3.0",
         "google-api-python-client>=2.0.0,<3.0",
         "grpcio~=1.0"
```


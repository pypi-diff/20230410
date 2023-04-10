# Comparing `tmp/ecopipeline-0.0.1.tar.gz` & `tmp/ecopipeline-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecopipeline-0.0.1.tar", last modified: Mon Apr 10 17:45:05 2023, max compression
+gzip compressed data, was "ecopipeline-0.0.2.tar", last modified: Mon Apr 10 18:50:41 2023, max compression
```

## Comparing `ecopipeline-0.0.1.tar` & `ecopipeline-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 17:45:01.935335 ecopipeline-0.0.1/
--rw-rw-rw-   0        0        0        0 2023-02-17 15:53:40.000000 ecopipeline-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1024 2023-04-10 17:45:04.964293 ecopipeline-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      579 2023-02-17 15:53:40.000000 ecopipeline-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2023-04-10 17:10:50.000000 ecopipeline-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      721 2023-04-10 17:45:05.067876 ecopipeline-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-04-10 17:18:28.000000 ecopipeline-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 17:45:02.035336 ecopipeline-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-10 17:45:02.035336 ecopipeline-0.0.1/src/ecopipeline/
--rw-rw-rw-   0        0        0     2021 2023-04-07 16:57:59.000000 ecopipeline-0.0.1/src/ecopipeline/__init__.py
--rw-rw-rw-   0        0        0     5746 2023-04-10 17:21:13.000000 ecopipeline-0.0.1/src/ecopipeline/bayview.py
--rw-rw-rw-   0        0        0      809 2023-03-31 18:26:04.000000 ecopipeline-0.0.1/src/ecopipeline/config.py
--rw-rw-rw-   0        0        0    14783 2023-04-10 17:21:32.000000 ecopipeline-0.0.1/src/ecopipeline/extract.py
--rw-rw-rw-   0        0        0    24099 2023-04-10 17:21:39.000000 ecopipeline-0.0.1/src/ecopipeline/lbnl.py
--rw-rw-rw-   0        0        0     9434 2023-04-10 17:21:53.000000 ecopipeline-0.0.1/src/ecopipeline/load.py
--rw-rw-rw-   0        0        0    28442 2023-04-10 17:21:58.000000 ecopipeline-0.0.1/src/ecopipeline/transform.py
--rw-rw-rw-   0        0        0     2696 2023-02-17 15:53:41.000000 ecopipeline-0.0.1/src/ecopipeline/unit_convert.py
-drwxrwxrwx   0        0        0        0 2023-04-10 17:45:02.095336 ecopipeline-0.0.1/src/ecopipeline.egg-info/
--rw-rw-rw-   0        0        0     1024 2023-04-10 17:45:01.000000 ecopipeline-0.0.1/src/ecopipeline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-04-10 17:45:01.000000 ecopipeline-0.0.1/src/ecopipeline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 17:45:01.000000 ecopipeline-0.0.1/src/ecopipeline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-04-10 17:45:01.000000 ecopipeline-0.0.1/src/ecopipeline.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-10 17:45:01.000000 ecopipeline-0.0.1/src/ecopipeline.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 18:50:37.788971 ecopipeline-0.0.2/
+-rw-rw-rw-   0        0        0        0 2023-02-17 15:53:40.000000 ecopipeline-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1024 2023-04-10 18:50:40.970635 ecopipeline-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      579 2023-02-17 15:53:40.000000 ecopipeline-0.0.2/README.md
+-rw-rw-rw-   0        0        0      108 2023-04-10 17:10:50.000000 ecopipeline-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      721 2023-04-10 18:50:41.081595 ecopipeline-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-04-10 17:18:28.000000 ecopipeline-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:50:37.888971 ecopipeline-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-10 18:50:37.888971 ecopipeline-0.0.2/src/ecopipeline/
+-rw-rw-rw-   0        0        0     2030 2023-04-10 18:45:52.000000 ecopipeline-0.0.2/src/ecopipeline/__init__.py
+-rw-rw-rw-   0        0        0     5746 2023-04-10 17:21:13.000000 ecopipeline-0.0.2/src/ecopipeline/bayview.py
+-rw-rw-rw-   0        0        0      809 2023-03-31 18:26:04.000000 ecopipeline-0.0.2/src/ecopipeline/config.py
+-rw-rw-rw-   0        0        0    13917 2023-04-10 18:45:00.000000 ecopipeline-0.0.2/src/ecopipeline/extract.py
+-rw-rw-rw-   0        0        0    24099 2023-04-10 17:21:39.000000 ecopipeline-0.0.2/src/ecopipeline/lbnl.py
+-rw-rw-rw-   0        0        0     9434 2023-04-10 18:47:39.000000 ecopipeline-0.0.2/src/ecopipeline/load.py
+-rw-rw-rw-   0        0        0    28442 2023-04-10 17:21:58.000000 ecopipeline-0.0.2/src/ecopipeline/transform.py
+-rw-rw-rw-   0        0        0     2696 2023-02-17 15:53:41.000000 ecopipeline-0.0.2/src/ecopipeline/unit_convert.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:50:37.936971 ecopipeline-0.0.2/src/ecopipeline.egg-info/
+-rw-rw-rw-   0        0        0     1024 2023-04-10 18:50:37.000000 ecopipeline-0.0.2/src/ecopipeline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2023-04-10 18:50:37.000000 ecopipeline-0.0.2/src/ecopipeline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 18:50:37.000000 ecopipeline-0.0.2/src/ecopipeline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-04-10 18:50:37.000000 ecopipeline-0.0.2/src/ecopipeline.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-10 18:50:37.000000 ecopipeline-0.0.2/src/ecopipeline.egg-info/top_level.txt
```

### Comparing `ecopipeline-0.0.1/PKG-INFO` & `ecopipeline-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.0.1
+Version: 0.0.2
 Summary: Contains functions for use in Ecotope Datapipelines
 Author: Nolan and SU Students
 Author-email: nolan@ecotope.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `ecopipeline-0.0.1/README.md` & `ecopipeline-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.1/setup.cfg` & `ecopipeline-0.0.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 636f 7069 7065 6c69 6e65 0d0a   = ecopipeline..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 310d  version = 0.0.1.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 320d  version = 0.0.2.
 00000030: 0a61 7574 686f 7220 3d20 4e6f 6c61 6e20  .author = Nolan 
 00000040: 616e 6420 5355 2053 7475 6465 6e74 730d  and SU Students.
 00000050: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000060: 6e6f 6c61 6e40 6563 6f74 6f70 652e 636f  nolan@ecotope.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2043 6f6e 7461 696e 7320 6675 6e63 7469   Contains functi
 00000090: 6f6e 7320 666f 7220 7573 6520 696e 2045  ons for use in E
```

### Comparing `ecopipeline-0.0.1/src/ecopipeline/__init__.py` & `ecopipeline-0.0.2/src/ecopipeline/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from .extract import get_noaa_data, json_to_df, extract_files, get_last_line, get_last_line, extract_new, csv_to_df, get_sub_dirs
+from .extract import get_noaa_data, json_to_df, extract_files, get_last_full_day_from_db, extract_new, csv_to_df, get_sub_dirs
 from .transform import rename_sensors, avg_duplicate_times, remove_outliers, ffill_missing, sensor_adjustment, get_energy_by_min, verify_power_energy, round_time, aggregate_df, join_to_hourly, concat_last_row, join_to_daily, get_temp_zones120, get_storage_gals120
 from .load import get_login_info, connect_db, check_table_exists, create_new_table, load_database, load_overwrite_database
 from .lbnl import nclarity_filter_new, site_specific, condensate_calculations, gas_valve_diff, gather_outdoor_conditions, nclarity_csv_to_df, add_date, aqsuite_filter_new, get_refrig_charge, elev_correction, change_ID_to_HVAC, get_cop_values, get_cfm_values, replace_humidity, create_fan_curves, lbnl_temperature_conversions, lbnl_pressure_conversions, lbnl_sat_calculations
 from .bayview import calculate_cop_values, aggregate_values
-__all__ = ["get_last_line", "set_input", "set_output","get_noaa_data", "json_to_df", "extract_files", "avg_duplicate_times", "remove_outliers", "ffill_missing", "sensor_adjustment", "get_energy_by_min", "verify_power_energy",
+__all__ = ["get_last_full_day_from_db", "set_input", "set_output","get_noaa_data", "json_to_df", "extract_files", "avg_duplicate_times", "remove_outliers", "ffill_missing", "sensor_adjustment", "get_energy_by_min", "verify_power_energy",
            "set_data", "aggregate_values", "calculate_cop_values", "get_login_info", "connect_db", "check_table_exists", "create_new_table", "createUnknownColumns", "load_database", "load_overwrite_database", "rename_sensors", "round_time", "aggregate_df", 
            "extract_new", "csv_to_df", "set_config", "get_sub_dirs", "join_to_hourly", "concat_last_row", "join_to_daily", "get_temp_zones120", "get_storage_gals120",  "site_specific", "condensate_calculations", "gas_valve_diff",
            "nclarity_filter_new", "gather_outdoor_conditions", "nclarity_csv_to_df", "add_date", "aqsuite_filter_new", "elev_correction", "get_refrig_charge", "change_ID_to_HVAC", "get_cop_values", "get_cfm_values", "replace_humidity", "create_fan_curves", 
            "lbnl_temperature_conversions", "lbnl_pressure_conversions", "lbnl_sat_calculations"]
```

### Comparing `ecopipeline-0.0.1/src/ecopipeline/bayview.py` & `ecopipeline-0.0.2/src/ecopipeline/bayview.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.1/src/ecopipeline/config.py` & `ecopipeline-0.0.2/src/ecopipeline/config.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.1/src/ecopipeline/extract.py` & `ecopipeline-0.0.2/src/ecopipeline/extract.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,88 +10,64 @@
 from ecopipeline.config import _config_directory, _data_directory
 import numpy as np
 import sys
 from pytz import timezone
 import mysql.connector.errors as mysqlerrors
 
 
-def get_last_line(config_file_path: str = _config_directory) -> pd.DataFrame:
+def get_last_full_day_from_db(config_file_path: str = _config_directory) -> datetime:
     """
     Function retrieves the last line from the database with the most recent datetime.
 
     Args:
-        config_file_path (str): Path to config file (default is set in load.py)
+        config_file_path (str): Path to config file (default is set in load.py) TODO this is not used lol
     Returns: 
-        pd.DataFrame: One line DF of the last entry
+        datetime: end of last full day populated in database or default past time if no data found
     """
     config_dict = get_login_info(["minute"])
     db_connection, db_cursor = connect_db(config_info=config_dict['database'])
+    return_time = datetime(year=2000, month=1, day=9, hour=23, minute=59, second=0).astimezone(timezone('US/Pacific')) # arbitrary default time
 
     try:
         db_cursor.execute(
             f"select * from {config_dict['minute']['table_name']} order by time_pt DESC LIMIT 1")
-    except mysqlerrors.Error:
-        print(f"Table {config_dict['minute']['table_name']} does not exist.")
-        column_names = config_dict['minute']['sensor_list']
-        return_df = pd.DataFrame(columns=column_names, index=[datetime(
-            year=2022, month=1, day=9, hour=23, minute=59, second=0).astimezone(timezone('US/Pacific'))])
-        return_df = return_df.fillna(0)
-        return return_df
-
-    last_row_data = pd.DataFrame(db_cursor.fetchall())
-    last_time = last_row_data[0][0]
-
-    if ((last_time.hour != 23) or (last_time.minute != 59)):
-        last_full_day = datetime(year=last_time.year, month=last_time.month,
-                                 day=last_time.day-1, hour=23, minute=59, second=0)
-        try:
-            db_cursor.execute(
-                f"select * from {config_dict['minute']['table_name']} where time_pt <= '{last_full_day}' order by time_pt DESC LIMIT 1") # TODO there is a bug here if there is only one partial day in db
-        except mysqlerrors.Error:
-            print(
-                f"Table {config_dict['minute']['table_name']} does not exist.")
-            return 0
 
         last_row_data = pd.DataFrame(db_cursor.fetchall())
+        if len(last_row_data.index) > 0:
+            last_time = last_row_data[0][0] # get time from last_data_row[0][0] TODO probably better way to do this
 
-    try:
-        db_cursor.execute(f"select column_name from information_schema.columns where table_schema = '"
-                          f"{config_dict['database']['database']}' and table_name = '"
-                          f"{config_dict['minute']['table_name']}'")
+            if ((last_time.hour != 23) or (last_time.minute != 59)):
+                return_time = datetime(year=last_time.year, month=last_time.month,
+                                        day=last_time.day-1, hour=23, minute=59, second=0).astimezone(timezone('US/Pacific'))
+            else:
+                return_time = last_time.tz_localize(timezone('US/Pacific'))
+        else:
+            print("Database has no previous data. Using default time to extract data.")
     except mysqlerrors.Error:
-        print(f"Table {config_dict['minute']['table_name']} does not exist.")
-        return 0
-
-    columns_names = db_cursor.fetchall()
-    columns_names = [name[0] for name in columns_names]
-    last_row_data.columns = columns_names
-    last_row_data.set_index(last_row_data['time_pt'], inplace=True)
-    last_row_data.drop(['time_pt'], axis=1, inplace=True)
-    last_row_data.index = last_row_data.index.tz_localize(
-        timezone('US/Pacific'))
+        print("Unable to find last timestamp in database. Using default time to extract data.")
 
     db_cursor.close()
     db_connection.close()
 
-    return last_row_data
+    return return_time
 
 
-def extract_new(last_row: pd.DataFrame, json_filenames: List[str]) -> List[str]:
+def extract_new(time: datetime, json_filenames: List[str]) -> List[str]:
     """
     Function filters the filenames to only those newer than the last date.
 
     Args: 
-        last_row (pd.DataFrame): The last row in the database
+        time (datetime): The point in time for which we want to start the data extraction from
         json_filenames (List[str]): List of filenames to be filtered
     Returns: 
         List[str]: Filtered list of filenames
     """
-    time = last_row.squeeze()
-    time = time.name
-    time = time.to_pydatetime()
+    # time = last_row.squeeze()
+    # time = time.name
+    # time = time.to_pydatetime()
     time_int = int(time.strftime("%Y%m%d%H%M%S"))
     return list(filter(lambda filename: int(filename[-17:-3]) >= time_int, json_filenames))
 
 
 def extract_files(extension: str, subdir: str = "") -> List[str]:
     """
     Function takes in a file extension and subdirectory and returns a list of paths files in the directory of that type.
```

### Comparing `ecopipeline-0.0.1/src/ecopipeline/lbnl.py` & `ecopipeline-0.0.2/src/ecopipeline/lbnl.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.1/src/ecopipeline/load.py` & `ecopipeline-0.0.2/src/ecopipeline/load.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.1/src/ecopipeline/transform.py` & `ecopipeline-0.0.2/src/ecopipeline/transform.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.1/src/ecopipeline/unit_convert.py` & `ecopipeline-0.0.2/src/ecopipeline/unit_convert.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.1/src/ecopipeline.egg-info/PKG-INFO` & `ecopipeline-0.0.2/src/ecopipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.0.1
+Version: 0.0.2
 Summary: Contains functions for use in Ecotope Datapipelines
 Author: Nolan and SU Students
 Author-email: nolan@ecotope.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```


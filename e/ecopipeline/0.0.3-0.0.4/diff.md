# Comparing `tmp/ecopipeline-0.0.3.tar.gz` & `tmp/ecopipeline-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecopipeline-0.0.3.tar", last modified: Mon Apr 10 20:02:02 2023, max compression
+gzip compressed data, was "ecopipeline-0.0.4.tar", last modified: Mon Apr 10 20:32:05 2023, max compression
```

## Comparing `ecopipeline-0.0.3.tar` & `ecopipeline-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 20:01:58.943450 ecopipeline-0.0.3/
--rw-rw-rw-   0        0        0        0 2023-02-17 15:53:40.000000 ecopipeline-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1024 2023-04-10 20:02:02.178497 ecopipeline-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      579 2023-02-17 15:53:40.000000 ecopipeline-0.0.3/README.md
--rw-rw-rw-   0        0        0      108 2023-04-10 17:10:50.000000 ecopipeline-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      721 2023-04-10 20:02:02.339712 ecopipeline-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-04-10 17:18:28.000000 ecopipeline-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:01:59.051450 ecopipeline-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-10 20:01:59.051450 ecopipeline-0.0.3/src/ecopipeline/
--rw-rw-rw-   0        0        0     2030 2023-04-10 18:45:52.000000 ecopipeline-0.0.3/src/ecopipeline/__init__.py
--rw-rw-rw-   0        0        0     5746 2023-04-10 17:21:13.000000 ecopipeline-0.0.3/src/ecopipeline/bayview.py
--rw-rw-rw-   0        0        0      809 2023-03-31 18:26:04.000000 ecopipeline-0.0.3/src/ecopipeline/config.py
--rw-rw-rw-   0        0        0    14139 2023-04-10 20:01:08.000000 ecopipeline-0.0.3/src/ecopipeline/extract.py
--rw-rw-rw-   0        0        0    24099 2023-04-10 17:21:39.000000 ecopipeline-0.0.3/src/ecopipeline/lbnl.py
--rw-rw-rw-   0        0        0     9434 2023-04-10 18:47:39.000000 ecopipeline-0.0.3/src/ecopipeline/load.py
--rw-rw-rw-   0        0        0    28442 2023-04-10 17:21:58.000000 ecopipeline-0.0.3/src/ecopipeline/transform.py
--rw-rw-rw-   0        0        0     2696 2023-02-17 15:53:41.000000 ecopipeline-0.0.3/src/ecopipeline/unit_convert.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:01:59.103451 ecopipeline-0.0.3/src/ecopipeline.egg-info/
--rw-rw-rw-   0        0        0     1024 2023-04-10 20:01:58.000000 ecopipeline-0.0.3/src/ecopipeline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-04-10 20:01:58.000000 ecopipeline-0.0.3/src/ecopipeline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 20:01:58.000000 ecopipeline-0.0.3/src/ecopipeline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-04-10 20:01:58.000000 ecopipeline-0.0.3/src/ecopipeline.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-10 20:01:58.000000 ecopipeline-0.0.3/src/ecopipeline.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 20:32:02.655057 ecopipeline-0.0.4/
+-rw-rw-rw-   0        0        0        0 2023-02-17 15:53:40.000000 ecopipeline-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1024 2023-04-10 20:32:05.652147 ecopipeline-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      579 2023-02-17 15:53:40.000000 ecopipeline-0.0.4/README.md
+-rw-rw-rw-   0        0        0      108 2023-04-10 17:10:50.000000 ecopipeline-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      721 2023-04-10 20:32:05.771201 ecopipeline-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-04-10 17:18:28.000000 ecopipeline-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:32:02.755057 ecopipeline-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-10 20:32:02.755057 ecopipeline-0.0.4/src/ecopipeline/
+-rw-rw-rw-   0        0        0     2030 2023-04-10 18:45:52.000000 ecopipeline-0.0.4/src/ecopipeline/__init__.py
+-rw-rw-rw-   0        0        0     5746 2023-04-10 17:21:13.000000 ecopipeline-0.0.4/src/ecopipeline/bayview.py
+-rw-rw-rw-   0        0        0      809 2023-03-31 18:26:04.000000 ecopipeline-0.0.4/src/ecopipeline/config.py
+-rw-rw-rw-   0        0        0    13858 2023-04-10 20:26:32.000000 ecopipeline-0.0.4/src/ecopipeline/extract.py
+-rw-rw-rw-   0        0        0    24099 2023-04-10 17:21:39.000000 ecopipeline-0.0.4/src/ecopipeline/lbnl.py
+-rw-rw-rw-   0        0        0     9434 2023-04-10 18:47:39.000000 ecopipeline-0.0.4/src/ecopipeline/load.py
+-rw-rw-rw-   0        0        0    28442 2023-04-10 17:21:58.000000 ecopipeline-0.0.4/src/ecopipeline/transform.py
+-rw-rw-rw-   0        0        0     2696 2023-02-17 15:53:41.000000 ecopipeline-0.0.4/src/ecopipeline/unit_convert.py
+drwxrwxrwx   0        0        0        0 2023-04-10 20:32:02.807057 ecopipeline-0.0.4/src/ecopipeline.egg-info/
+-rw-rw-rw-   0        0        0     1024 2023-04-10 20:32:02.000000 ecopipeline-0.0.4/src/ecopipeline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2023-04-10 20:32:02.000000 ecopipeline-0.0.4/src/ecopipeline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 20:32:02.000000 ecopipeline-0.0.4/src/ecopipeline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-04-10 20:32:02.000000 ecopipeline-0.0.4/src/ecopipeline.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-10 20:32:02.000000 ecopipeline-0.0.4/src/ecopipeline.egg-info/top_level.txt
```

### Comparing `ecopipeline-0.0.3/PKG-INFO` & `ecopipeline-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.0.3
+Version: 0.0.4
 Summary: Contains functions for use in Ecotope Datapipelines
 Author: Nolan and SU Students
 Author-email: nolan@ecotope.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `ecopipeline-0.0.3/README.md` & `ecopipeline-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.3/setup.cfg` & `ecopipeline-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 636f 7069 7065 6c69 6e65 0d0a   = ecopipeline..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 330d  version = 0.0.3.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 340d  version = 0.0.4.
 00000030: 0a61 7574 686f 7220 3d20 4e6f 6c61 6e20  .author = Nolan 
 00000040: 616e 6420 5355 2053 7475 6465 6e74 730d  and SU Students.
 00000050: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000060: 6e6f 6c61 6e40 6563 6f74 6f70 652e 636f  nolan@ecotope.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2043 6f6e 7461 696e 7320 6675 6e63 7469   Contains functi
 00000090: 6f6e 7320 666f 7220 7573 6520 696e 2045  ons for use in E
```

### Comparing `ecopipeline-0.0.3/src/ecopipeline/__init__.py` & `ecopipeline-0.0.4/src/ecopipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.3/src/ecopipeline/bayview.py` & `ecopipeline-0.0.4/src/ecopipeline/bayview.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.3/src/ecopipeline/config.py` & `ecopipeline-0.0.4/src/ecopipeline/config.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.3/src/ecopipeline/extract.py` & `ecopipeline-0.0.4/src/ecopipeline/extract.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,23 +57,16 @@
 
     Args: 
         time (datetime): The point in time for which we want to start the data extraction from
         json_filenames (List[str]): List of filenames to be filtered
     Returns: 
         List[str]: Filtered list of filenames
     """
-    # time = last_row.squeeze()
-    # time = time.name
-    # time = time.to_pydatetime()
     time_int = int(time.strftime("%Y%m%d%H%M%S"))
     return_list = list(filter(lambda filename: int(filename[-17:-3]) >= time_int, json_filenames))
-    if len(return_list) > 0:
-        print("extracting files " + return_list[0] + " through " + return_list[-1])
-    else:
-        print("no new data files found after date " + str(time_int))
     return return_list
 
 
 def extract_files(extension: str, subdir: str = "") -> List[str]:
     """
     Function takes in a file extension and subdirectory and returns a list of paths files in the directory of that type.
```

### Comparing `ecopipeline-0.0.3/src/ecopipeline/lbnl.py` & `ecopipeline-0.0.4/src/ecopipeline/lbnl.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.3/src/ecopipeline/load.py` & `ecopipeline-0.0.4/src/ecopipeline/load.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.3/src/ecopipeline/transform.py` & `ecopipeline-0.0.4/src/ecopipeline/transform.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.3/src/ecopipeline/unit_convert.py` & `ecopipeline-0.0.4/src/ecopipeline/unit_convert.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.3/src/ecopipeline.egg-info/PKG-INFO` & `ecopipeline-0.0.4/src/ecopipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.0.3
+Version: 0.0.4
 Summary: Contains functions for use in Ecotope Datapipelines
 Author: Nolan and SU Students
 Author-email: nolan@ecotope.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```


# Comparing `tmp/pheno-utils-0.0.6.tar.gz` & `tmp/pheno-utils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.0.6.tar", last modified: Mon Apr 10 19:49:48 2023, max compression
+gzip compressed data, was "pheno-utils-0.0.7.tar", last modified: Mon Apr 10 21:18:41 2023, max compression
```

## Comparing `pheno-utils-0.0.6.tar` & `pheno-utils-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-10 19:49:48.599118 pheno-utils-0.0.6/
--rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.0.6/LICENSE
--rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.0.6/MANIFEST.in
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-10 19:49:48.598790 pheno-utils-0.0.6/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.0.6/README.md
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-10 19:49:48.595678 pheno-utils-0.0.6/pheno_utils/
--rw-r--r--   0 alondmnt   (501) staff       (20)       22 2023-04-10 19:46:34.000000 pheno-utils-0.0.6/pheno_utils/__init__.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     8743 2023-04-10 19:46:34.000000 pheno-utils-0.0.6/pheno_utils/_modidx.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-10 19:46:34.000000 pheno-utils-0.0.6/pheno_utils/age_reference_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2333 2023-04-10 19:46:34.000000 pheno-utils-0.0.6/pheno_utils/basic_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-10 19:46:34.000000 pheno-utils-0.0.6/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2740 2023-04-10 19:46:34.000000 pheno-utils-0.0.6/pheno_utils/config.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    12339 2023-04-10 19:46:34.000000 pheno-utils-0.0.6/pheno_utils/data_loader.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-10 19:46:34.000000 pheno-utils-0.0.6/pheno_utils/dates_plots.py
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-10 19:49:48.598373 pheno-utils-0.0.6/pheno_utils.egg-info/
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-10 19:49:48.000000 pheno-utils-0.0.6/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      515 2023-04-10 19:49:48.000000 pheno-utils-0.0.6/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-10 19:49:48.000000 pheno-utils-0.0.6/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-10 19:49:48.000000 pheno-utils-0.0.6/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.0.6/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 alondmnt   (501) staff       (20)       99 2023-04-10 19:49:48.000000 pheno-utils-0.0.6/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-10 19:49:48.000000 pheno-utils-0.0.6/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)     1040 2023-04-10 19:45:23.000000 pheno-utils-0.0.6/settings.ini
--rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-10 19:49:48.599242 pheno-utils-0.0.6/setup.cfg
--rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.0.6/setup.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-10 21:18:41.337829 pheno-utils-0.0.7/
+-rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.0.7/LICENSE
+-rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.0.7/MANIFEST.in
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-10 21:18:41.337496 pheno-utils-0.0.7/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.0.7/README.md
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-10 21:18:41.334323 pheno-utils-0.0.7/pheno_utils/
+-rw-r--r--   0 alondmnt   (501) staff       (20)       22 2023-04-10 20:10:59.000000 pheno-utils-0.0.7/pheno_utils/__init__.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     8743 2023-04-10 20:10:59.000000 pheno-utils-0.0.7/pheno_utils/_modidx.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-10 20:10:59.000000 pheno-utils-0.0.7/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2333 2023-04-10 20:10:59.000000 pheno-utils-0.0.7/pheno_utils/basic_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-10 20:10:59.000000 pheno-utils-0.0.7/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2740 2023-04-10 20:10:59.000000 pheno-utils-0.0.7/pheno_utils/config.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    12417 2023-04-10 20:10:59.000000 pheno-utils-0.0.7/pheno_utils/data_loader.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-10 20:10:59.000000 pheno-utils-0.0.7/pheno_utils/dates_plots.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-10 21:18:41.337077 pheno-utils-0.0.7/pheno_utils.egg-info/
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-10 21:18:41.000000 pheno-utils-0.0.7/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      515 2023-04-10 21:18:41.000000 pheno-utils-0.0.7/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-10 21:18:41.000000 pheno-utils-0.0.7/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-10 21:18:41.000000 pheno-utils-0.0.7/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.0.7/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 alondmnt   (501) staff       (20)       99 2023-04-10 21:18:41.000000 pheno-utils-0.0.7/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-10 21:18:41.000000 pheno-utils-0.0.7/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1040 2023-04-10 20:10:51.000000 pheno-utils-0.0.7/settings.ini
+-rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-10 21:18:41.337969 pheno-utils-0.0.7/setup.cfg
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.0.7/setup.py
```

### Comparing `pheno-utils-0.0.6/LICENSE` & `pheno-utils-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.6/PKG-INFO` & `pheno-utils-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.0.6/pheno_utils/_modidx.py` & `pheno-utils-0.0.7/pheno_utils/_modidx.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.6/pheno_utils/age_reference_plots.py` & `pheno-utils-0.0.7/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.6/pheno_utils/basic_plots.py` & `pheno-utils-0.0.7/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.6/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.0.7/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.6/pheno_utils/config.py` & `pheno-utils-0.0.7/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.6/pheno_utils/data_loader.py` & `pheno-utils-0.0.7/pheno_utils/data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,17 @@
             fields (List[str]): Fields to return
 
         Returns:
             pd.DataFrame: Data for the specified fields from all tables
         """
         data = []
         for df in self.dfs.values():
-            data.append(df[df.columns.intersection(fields)])
+            fields_in_df = df.columns.intersection(fields)
+            if len(fields_in_df):
+                data.append(df[fields_in_df])
         data = pd.concat(data, axis=1)
         data = data.loc[:, ~data.columns.duplicated()]
 
         fields_in_index = np.intersect1d(fields, data.index.names)
         for field in fields_in_index:
             data[field] = data.index.get_level_values(field)
```

### Comparing `pheno-utils-0.0.6/pheno_utils/dates_plots.py` & `pheno-utils-0.0.7/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.6/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.0.7/pheno_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.0.6/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.0.7/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.6/settings.ini` & `pheno-utils-0.0.7/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = pheno-utils
 lib_name = %(repo)s
-version = 0.0.6
+version = 0.0.7
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = pheno_utils
```

### Comparing `pheno-utils-0.0.6/setup.py` & `pheno-utils-0.0.7/setup.py`

 * *Files identical despite different names*


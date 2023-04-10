# Comparing `tmp/lis_autocontent-0.0.3.tar.gz` & `tmp/lis_autocontent-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lis_autocontent-0.0.3.tar", last modified: Wed Mar  8 20:18:25 2023, max compression
+gzip compressed data, was "lis_autocontent-0.0.4.tar", last modified: Mon Apr 10 18:02:32 2023, max compression
```

## Comparing `lis_autocontent-0.0.3.tar` & `lis_autocontent-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ctc       (1002) ctc       (1002)        0 2023-03-08 20:18:25.942400 lis_autocontent-0.0.3/
--rw-rw-r--   0 ctc       (1002) ctc       (1002)    11357 2023-01-04 20:13:17.000000 lis_autocontent-0.0.3/LICENSE
--rw-rw-r--   0 ctc       (1002) ctc       (1002)     1784 2023-03-08 20:18:25.943400 lis_autocontent-0.0.3/PKG-INFO
--rw-rw-r--   0 ctc       (1002) ctc       (1002)     1662 2023-02-21 17:46:17.000000 lis_autocontent-0.0.3/README.md
-drwxrwxr-x   0 ctc       (1002) ctc       (1002)        0 2023-03-08 20:18:25.861399 lis_autocontent-0.0.3/lis_autocontent.egg-info/
--rw-rw-r--   0 ctc       (1002) ctc       (1002)     1784 2023-03-08 20:18:25.000000 lis_autocontent-0.0.3/lis_autocontent.egg-info/PKG-INFO
--rw-rw-r--   0 ctc       (1002) ctc       (1002)      349 2023-03-08 20:18:25.000000 lis_autocontent-0.0.3/lis_autocontent.egg-info/SOURCES.txt
--rw-rw-r--   0 ctc       (1002) ctc       (1002)        1 2023-03-08 20:18:25.000000 lis_autocontent-0.0.3/lis_autocontent.egg-info/dependency_links.txt
--rw-rw-r--   0 ctc       (1002) ctc       (1002)       68 2023-03-08 20:18:25.000000 lis_autocontent-0.0.3/lis_autocontent.egg-info/entry_points.txt
--rw-rw-r--   0 ctc       (1002) ctc       (1002)      116 2023-03-08 20:18:25.000000 lis_autocontent-0.0.3/lis_autocontent.egg-info/requires.txt
--rw-rw-r--   0 ctc       (1002) ctc       (1002)       16 2023-03-08 20:18:25.000000 lis_autocontent-0.0.3/lis_autocontent.egg-info/top_level.txt
-drwxrwxr-x   0 ctc       (1002) ctc       (1002)        0 2023-03-08 20:18:25.928400 lis_autocontent-0.0.3/scripts/
--rwxrwxr-x   0 ctc       (1002) ctc       (1002)      544 2023-02-06 19:43:23.000000 lis_autocontent-0.0.3/scripts/lis_autocontent.py
--rw-rw-r--   0 ctc       (1002) ctc       (1002)     6248 2023-02-21 17:46:17.000000 lis_autocontent-0.0.3/scripts/lis_cli.py
--rw-rw-r--   0 ctc       (1002) ctc       (1002)    35242 2023-03-08 20:13:14.000000 lis_autocontent-0.0.3/scripts/process_collections.py
--rw-rw-r--   0 ctc       (1002) ctc       (1002)      540 2023-03-08 20:18:25.946401 lis_autocontent-0.0.3/setup.cfg
--rw-rw-r--   0 ctc       (1002) ctc       (1002)      667 2023-02-21 17:46:17.000000 lis_autocontent-0.0.3/setup.py
+drwxrwxr-x   0 ctc       (1002) ctc       (1002)        0 2023-04-10 18:02:32.103026 lis_autocontent-0.0.4/
+-rw-rw-r--   0 ctc       (1002) ctc       (1002)    11357 2023-01-04 20:13:17.000000 lis_autocontent-0.0.4/LICENSE
+-rw-rw-r--   0 ctc       (1002) ctc       (1002)     1784 2023-04-10 18:02:32.103525 lis_autocontent-0.0.4/PKG-INFO
+-rw-rw-r--   0 ctc       (1002) ctc       (1002)     1662 2023-02-21 17:46:17.000000 lis_autocontent-0.0.4/README.md
+drwxrwxr-x   0 ctc       (1002) ctc       (1002)        0 2023-04-10 18:02:32.097394 lis_autocontent-0.0.4/lis_autocontent.egg-info/
+-rw-rw-r--   0 ctc       (1002) ctc       (1002)     1784 2023-04-10 18:02:32.000000 lis_autocontent-0.0.4/lis_autocontent.egg-info/PKG-INFO
+-rw-rw-r--   0 ctc       (1002) ctc       (1002)      349 2023-04-10 18:02:32.000000 lis_autocontent-0.0.4/lis_autocontent.egg-info/SOURCES.txt
+-rw-rw-r--   0 ctc       (1002) ctc       (1002)        1 2023-04-10 18:02:32.000000 lis_autocontent-0.0.4/lis_autocontent.egg-info/dependency_links.txt
+-rw-rw-r--   0 ctc       (1002) ctc       (1002)       68 2023-04-10 18:02:32.000000 lis_autocontent-0.0.4/lis_autocontent.egg-info/entry_points.txt
+-rw-rw-r--   0 ctc       (1002) ctc       (1002)      116 2023-04-10 18:02:32.000000 lis_autocontent-0.0.4/lis_autocontent.egg-info/requires.txt
+-rw-rw-r--   0 ctc       (1002) ctc       (1002)       16 2023-04-10 18:02:32.000000 lis_autocontent-0.0.4/lis_autocontent.egg-info/top_level.txt
+drwxrwxr-x   0 ctc       (1002) ctc       (1002)        0 2023-04-10 18:02:32.101335 lis_autocontent-0.0.4/scripts/
+-rwxrwxr-x   0 ctc       (1002) ctc       (1002)      544 2023-02-06 19:43:23.000000 lis_autocontent-0.0.4/scripts/lis_autocontent.py
+-rw-rw-r--   0 ctc       (1002) ctc       (1002)     6248 2023-02-21 17:46:17.000000 lis_autocontent-0.0.4/scripts/lis_cli.py
+-rw-rw-r--   0 ctc       (1002) ctc       (1002)    35242 2023-04-10 18:01:05.000000 lis_autocontent-0.0.4/scripts/process_collections.py
+-rw-rw-r--   0 ctc       (1002) ctc       (1002)      540 2023-04-10 18:02:32.105270 lis_autocontent-0.0.4/setup.cfg
+-rw-rw-r--   0 ctc       (1002) ctc       (1002)      667 2023-02-21 17:46:17.000000 lis_autocontent-0.0.4/setup.py
```

### Comparing `lis_autocontent-0.0.3/LICENSE` & `lis_autocontent-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lis_autocontent-0.0.3/PKG-INFO` & `lis_autocontent-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lis_autocontent
-Version: 0.0.3
+Version: 0.0.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lis-autocontent
 Scrapes the LIS datastore (https://data.legumeinfo.org) and populates various configs and databases for deployment
 
 ## Reqiurements
```

### Comparing `lis_autocontent-0.0.3/README.md` & `lis_autocontent-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lis_autocontent-0.0.3/lis_autocontent.egg-info/PKG-INFO` & `lis_autocontent-0.0.4/lis_autocontent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lis-autocontent
-Version: 0.0.3
+Version: 0.0.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lis-autocontent
 Scrapes the LIS datastore (https://data.legumeinfo.org) and populates various configs and databases for deployment
 
 ## Reqiurements
```

### Comparing `lis_autocontent-0.0.3/scripts/lis_autocontent.py` & `lis_autocontent-0.0.4/scripts/lis_autocontent.py`

 * *Files identical despite different names*

### Comparing `lis_autocontent-0.0.3/scripts/lis_cli.py` & `lis_autocontent-0.0.4/scripts/lis_cli.py`

 * *Files identical despite different names*

### Comparing `lis_autocontent-0.0.3/scripts/process_collections.py` & `lis_autocontent-0.0.4/scripts/process_collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,20 +480,20 @@
                                 paf_parts = paf_lookup.split(
                                     "."
                                 )  # split the paf file name into parts delimited by '.'
                                 parent1 = ".".join(
                                     paf_parts[:3]
                                 )  # parent 1 in pair-wise alignment
                                 parent2 = ".".join(
-                                    paf_parts[5:8]
+                                    paf_parts[4:7]
                                 )  # parent 2 in pair-wise alignment
                                 self.files[collection_type][paf_lookup] = {
                                     "url": paf_url,
                                     "name": paf_lookup,
-                                    "parent": [parent1, parent2],
+                                    "parent": [parent2, parent1],
                                     "genus": genus,
                                     "species": species,
                                     "infraspecies": strain_lookup,
                                     "taxid": 0,
                                 }
                                 logger.debug(self.files[collection_type][paf_lookup])
             readme_url = f"{self.datastore_url}/{collection_dir}README.{name}.yml"  # species collection readme
```

### Comparing `lis_autocontent-0.0.3/setup.cfg` & `lis_autocontent-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = lis_autocontent
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.0.3
+version = 0.0.4
 
 [options]
 install_requires = 
 	PyYAML==6.0
 	certifi==2022.5.18.1
 	charset-normalizer==2.0.12
 	click==8.1.3
```

### Comparing `lis_autocontent-0.0.3/setup.py` & `lis_autocontent-0.0.4/setup.py`

 * *Files identical despite different names*


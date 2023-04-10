# Comparing `tmp/python_pik_api_wrapper-1.5.3.tar.gz` & `tmp/python_pik_api_wrapper-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_pik_api_wrapper-1.5.3.tar", last modified: Mon Apr 10 19:06:41 2023, max compression
+gzip compressed data, was "python_pik_api_wrapper-1.5.4.tar", last modified: Mon Apr 10 21:39:52 2023, max compression
```

## Comparing `python_pik_api_wrapper-1.5.3.tar` & `python_pik_api_wrapper-1.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 drill     (1000) drill     (1000)        0 2023-04-10 19:06:41.956889 python_pik_api_wrapper-1.5.3/
--rw-rw-r--   0 drill     (1000) drill     (1000)      256 2023-04-10 19:06:41.956889 python_pik_api_wrapper-1.5.3/PKG-INFO
--rw-rw-r--   0 drill     (1000) drill     (1000)      237 2020-11-12 17:50:04.000000 python_pik_api_wrapper-1.5.3/README.md
-drwxrwxr-x   0 drill     (1000) drill     (1000)        0 2023-04-10 19:06:41.956889 python_pik_api_wrapper-1.5.3/pik_wrapper/
--rw-rw-r--   0 drill     (1000) drill     (1000)       22 2023-04-10 18:43:12.000000 python_pik_api_wrapper-1.5.3/pik_wrapper/__init__.py
-drwxrwxr-x   0 drill     (1000) drill     (1000)        0 2023-04-10 19:06:41.956889 python_pik_api_wrapper-1.5.3/pik_wrapper/entity/
--rw-rw-r--   0 drill     (1000) drill     (1000)        0 2020-11-12 18:49:43.000000 python_pik_api_wrapper-1.5.3/pik_wrapper/entity/__init__.py
--rw-rw-r--   0 drill     (1000) drill     (1000)      531 2020-11-26 19:12:00.000000 python_pik_api_wrapper-1.5.3/pik_wrapper/entity/block.py
--rw-rw-r--   0 drill     (1000) drill     (1000)      976 2021-02-16 07:49:48.000000 python_pik_api_wrapper-1.5.3/pik_wrapper/entity/bulk.py
--rw-rw-r--   0 drill     (1000) drill     (1000)      731 2020-11-26 19:12:00.000000 python_pik_api_wrapper-1.5.3/pik_wrapper/entity/entity.py
--rw-rw-r--   0 drill     (1000) drill     (1000)      855 2020-11-26 22:51:06.000000 python_pik_api_wrapper-1.5.3/pik_wrapper/entity/item.py
--rw-rw-r--   0 drill     (1000) drill     (1000)      534 2020-11-26 19:12:00.000000 python_pik_api_wrapper-1.5.3/pik_wrapper/entity/location.py
--rw-rw-r--   0 drill     (1000) drill     (1000)     4868 2023-04-10 18:42:03.000000 python_pik_api_wrapper-1.5.3/pik_wrapper/pik_wrapper.py
-drwxrwxr-x   0 drill     (1000) drill     (1000)        0 2023-04-10 19:06:41.956889 python_pik_api_wrapper-1.5.3/pik_wrapper/value_object/
--rw-rw-r--   0 drill     (1000) drill     (1000)        0 2020-11-12 20:15:36.000000 python_pik_api_wrapper-1.5.3/pik_wrapper/value_object/__init__.py
--rw-rw-r--   0 drill     (1000) drill     (1000)      525 2020-11-26 19:16:57.000000 python_pik_api_wrapper-1.5.3/pik_wrapper/value_object/photo.py
--rw-rw-r--   0 drill     (1000) drill     (1000)      128 2020-11-12 21:15:10.000000 python_pik_api_wrapper-1.5.3/pik_wrapper/value_object/value_object.py
-drwxrwxr-x   0 drill     (1000) drill     (1000)        0 2023-04-10 19:06:41.956889 python_pik_api_wrapper-1.5.3/python_pik_api_wrapper.egg-info/
--rw-rw-r--   0 drill     (1000) drill     (1000)      256 2023-04-10 19:06:41.000000 python_pik_api_wrapper-1.5.3/python_pik_api_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 drill     (1000) drill     (1000)      583 2023-04-10 19:06:41.000000 python_pik_api_wrapper-1.5.3/python_pik_api_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 drill     (1000) drill     (1000)        1 2023-04-10 19:06:41.000000 python_pik_api_wrapper-1.5.3/python_pik_api_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 drill     (1000) drill     (1000)        9 2023-04-10 19:06:41.000000 python_pik_api_wrapper-1.5.3/python_pik_api_wrapper.egg-info/requires.txt
--rw-rw-r--   0 drill     (1000) drill     (1000)       12 2023-04-10 19:06:41.000000 python_pik_api_wrapper-1.5.3/python_pik_api_wrapper.egg-info/top_level.txt
--rw-rw-r--   0 drill     (1000) drill     (1000)       38 2023-04-10 19:06:41.956889 python_pik_api_wrapper-1.5.3/setup.cfg
--rw-rw-r--   0 drill     (1000) drill     (1000)      459 2020-11-14 12:52:15.000000 python_pik_api_wrapper-1.5.3/setup.py
+drwxrwxr-x   0 drill     (1000) drill     (1000)        0 2023-04-10 21:39:52.467440 python_pik_api_wrapper-1.5.4/
+-rw-rw-r--   0 drill     (1000) drill     (1000)      256 2023-04-10 21:39:52.467440 python_pik_api_wrapper-1.5.4/PKG-INFO
+-rw-rw-r--   0 drill     (1000) drill     (1000)      237 2020-11-12 17:50:04.000000 python_pik_api_wrapper-1.5.4/README.md
+drwxrwxr-x   0 drill     (1000) drill     (1000)        0 2023-04-10 21:39:52.467440 python_pik_api_wrapper-1.5.4/pik_wrapper/
+-rw-rw-r--   0 drill     (1000) drill     (1000)       22 2023-04-10 21:39:05.000000 python_pik_api_wrapper-1.5.4/pik_wrapper/__init__.py
+drwxrwxr-x   0 drill     (1000) drill     (1000)        0 2023-04-10 21:39:52.467440 python_pik_api_wrapper-1.5.4/pik_wrapper/entity/
+-rw-rw-r--   0 drill     (1000) drill     (1000)        0 2020-11-12 18:49:43.000000 python_pik_api_wrapper-1.5.4/pik_wrapper/entity/__init__.py
+-rw-rw-r--   0 drill     (1000) drill     (1000)      531 2020-11-26 19:12:00.000000 python_pik_api_wrapper-1.5.4/pik_wrapper/entity/block.py
+-rw-rw-r--   0 drill     (1000) drill     (1000)      976 2021-02-16 07:49:48.000000 python_pik_api_wrapper-1.5.4/pik_wrapper/entity/bulk.py
+-rw-rw-r--   0 drill     (1000) drill     (1000)      731 2020-11-26 19:12:00.000000 python_pik_api_wrapper-1.5.4/pik_wrapper/entity/entity.py
+-rw-rw-r--   0 drill     (1000) drill     (1000)      855 2020-11-26 22:51:06.000000 python_pik_api_wrapper-1.5.4/pik_wrapper/entity/item.py
+-rw-rw-r--   0 drill     (1000) drill     (1000)      534 2020-11-26 19:12:00.000000 python_pik_api_wrapper-1.5.4/pik_wrapper/entity/location.py
+-rw-rw-r--   0 drill     (1000) drill     (1000)     4881 2023-04-10 21:04:43.000000 python_pik_api_wrapper-1.5.4/pik_wrapper/pik_wrapper.py
+drwxrwxr-x   0 drill     (1000) drill     (1000)        0 2023-04-10 21:39:52.467440 python_pik_api_wrapper-1.5.4/pik_wrapper/value_object/
+-rw-rw-r--   0 drill     (1000) drill     (1000)        0 2020-11-12 20:15:36.000000 python_pik_api_wrapper-1.5.4/pik_wrapper/value_object/__init__.py
+-rw-rw-r--   0 drill     (1000) drill     (1000)      525 2020-11-26 19:16:57.000000 python_pik_api_wrapper-1.5.4/pik_wrapper/value_object/photo.py
+-rw-rw-r--   0 drill     (1000) drill     (1000)      128 2020-11-12 21:15:10.000000 python_pik_api_wrapper-1.5.4/pik_wrapper/value_object/value_object.py
+drwxrwxr-x   0 drill     (1000) drill     (1000)        0 2023-04-10 21:39:52.467440 python_pik_api_wrapper-1.5.4/python_pik_api_wrapper.egg-info/
+-rw-rw-r--   0 drill     (1000) drill     (1000)      256 2023-04-10 21:39:52.000000 python_pik_api_wrapper-1.5.4/python_pik_api_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 drill     (1000) drill     (1000)      583 2023-04-10 21:39:52.000000 python_pik_api_wrapper-1.5.4/python_pik_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 drill     (1000) drill     (1000)        1 2023-04-10 21:39:52.000000 python_pik_api_wrapper-1.5.4/python_pik_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 drill     (1000) drill     (1000)        9 2023-04-10 21:39:52.000000 python_pik_api_wrapper-1.5.4/python_pik_api_wrapper.egg-info/requires.txt
+-rw-rw-r--   0 drill     (1000) drill     (1000)       12 2023-04-10 21:39:52.000000 python_pik_api_wrapper-1.5.4/python_pik_api_wrapper.egg-info/top_level.txt
+-rw-rw-r--   0 drill     (1000) drill     (1000)       38 2023-04-10 21:39:52.467440 python_pik_api_wrapper-1.5.4/setup.cfg
+-rw-rw-r--   0 drill     (1000) drill     (1000)      459 2020-11-14 12:52:15.000000 python_pik_api_wrapper-1.5.4/setup.py
```

### Comparing `python_pik_api_wrapper-1.5.3/pik_wrapper/entity/block.py` & `python_pik_api_wrapper-1.5.4/pik_wrapper/entity/block.py`

 * *Files identical despite different names*

### Comparing `python_pik_api_wrapper-1.5.3/pik_wrapper/entity/bulk.py` & `python_pik_api_wrapper-1.5.4/pik_wrapper/entity/bulk.py`

 * *Files identical despite different names*

### Comparing `python_pik_api_wrapper-1.5.3/pik_wrapper/entity/entity.py` & `python_pik_api_wrapper-1.5.4/pik_wrapper/entity/entity.py`

 * *Files identical despite different names*

### Comparing `python_pik_api_wrapper-1.5.3/pik_wrapper/entity/item.py` & `python_pik_api_wrapper-1.5.4/pik_wrapper/entity/item.py`

 * *Files identical despite different names*

### Comparing `python_pik_api_wrapper-1.5.3/pik_wrapper/entity/location.py` & `python_pik_api_wrapper-1.5.4/pik_wrapper/entity/location.py`

 * *Files identical despite different names*

### Comparing `python_pik_api_wrapper-1.5.3/pik_wrapper/pik_wrapper.py` & `python_pik_api_wrapper-1.5.4/pik_wrapper/pik_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     def get_bulks(self, block: Block, only_settlement_fact: bool = False) -> List[Bulk]:
         if type(block) is not Block:
             raise ValueError
         bulks = self.send_request(f"bulk?block_id={block.id}&type=1,2,103")
         bulks_list = []
         count = 0
         for bulk in bulks:
-            if (bulk['name'] is None and len(bulk['name']) == 0) or (only_settlement_fact and bulk['settlement_fact']):
+            if bulk is None or bulk['name'] is None or len(bulk['name']) == 0 or (only_settlement_fact and bulk['settlement_fact']):
                 continue
             bulks_list.append(Bulk(str(bulk['id']), bulk['name'], count, bulk['type_id'], bulk['settlement_fact']))
             count += 1
         return bulks_list
 
     def get_items(self, bulk: Bulk) -> List[Item]:
         if type(bulk) is not Bulk:
```

### Comparing `python_pik_api_wrapper-1.5.3/pik_wrapper/value_object/photo.py` & `python_pik_api_wrapper-1.5.4/pik_wrapper/value_object/photo.py`

 * *Files identical despite different names*

### Comparing `python_pik_api_wrapper-1.5.3/python_pik_api_wrapper.egg-info/SOURCES.txt` & `python_pik_api_wrapper-1.5.4/python_pik_api_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*


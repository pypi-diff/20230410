# Comparing `tmp/zesty.zbs-api-1.0.2023.3.16.1678978980.tar.gz` & `tmp/zesty.zbs-api-1.0.2023.4.10.1681110487.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zesty.zbs-api-1.0.2023.3.16.1678978980.tar", last modified: Thu Mar 16 15:03:01 2023, max compression
+gzip compressed data, was "dist/zesty.zbs-api-1.0.2023.4.10.1681110487.tar", last modified: Mon Apr 10 07:08:08 2023, max compression
```

## Comparing `zesty.zbs-api-1.0.2023.3.16.1678978980.tar` & `zesty.zbs-api-1.0.2023.4.10.1681110487.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 15:03:01.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1166 2023-03-16 15:03:01.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/README.md
--rw-r--r--   0 root         (0) root         (0)       60 2023-03-16 15:03:01.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 15:03:01.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/src/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14353 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/src/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/src/cloud_vendors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 15:03:01.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/
--rw-rw-rw-   0 root         (0) root         (0)     3540 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/BlockDevice.py
--rw-rw-rw-   0 root         (0) root         (0)     8735 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/EbsVolume.py
--rw-rw-rw-   0 root         (0) root         (0)     7367 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/FileSystem.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/InstancesTags.py
--rw-rw-rw-   0 root         (0) root         (0)    14968 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/ManagedFS.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/Usage.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/agent_report.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/cpu_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/disk_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     2738 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/hf_interface.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/mem_mon.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/network_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1935 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/overview.py
--rw-rw-rw-   0 root         (0) root         (0)    11605 2023-03-16 15:01:52.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/src/protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 15:03:01.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/zesty.zbs_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1166 2023-03-16 15:03:01.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/zesty.zbs_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      599 2023-03-16 15:03:01.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/zesty.zbs_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 15:03:01.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/zesty.zbs_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-03-16 15:03:01.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/zesty.zbs_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-16 15:03:01.000000 zesty.zbs-api-1.0.2023.3.16.1678978980/zesty.zbs_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:08:08.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1166 2023-04-10 07:08:08.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/README.md
+-rw-r--r--   0 root         (0) root         (0)       60 2023-04-10 07:08:08.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:08:08.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/src/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14353 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/src/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/src/cloud_vendors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:08:08.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/
+-rw-rw-rw-   0 root         (0) root         (0)     3540 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/BlockDevice.py
+-rw-rw-rw-   0 root         (0) root         (0)     8818 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/EbsVolume.py
+-rw-rw-rw-   0 root         (0) root         (0)     7367 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/FileSystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/InstancesTags.py
+-rw-rw-rw-   0 root         (0) root         (0)    14968 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/ManagedFS.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/Usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/agent_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/cpu_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/disk_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/hf_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/mem_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/network_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/overview.py
+-rw-rw-rw-   0 root         (0) root         (0)    11605 2023-04-10 07:04:48.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/src/protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 07:08:08.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/zesty.zbs_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1166 2023-04-10 07:08:08.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/zesty.zbs_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      599 2023-04-10 07:08:08.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/zesty.zbs_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 07:08:08.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/zesty.zbs_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-10 07:08:08.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/zesty.zbs_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-10 07:08:08.000000 zesty.zbs-api-1.0.2023.4.10.1681110487/zesty.zbs_api.egg-info/top_level.txt
```

### Comparing `zesty.zbs-api-1.0.2023.3.16.1678978980/PKG-INFO` & `zesty.zbs-api-1.0.2023.4.10.1681110487/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api
-Version: 1.0.2023.3.16.1678978980
+Version: 1.0.2023.4.10.1681110487
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-1.0.2023.3.16.1678978980/README.md` & `zesty.zbs-api-1.0.2023.4.10.1681110487/README.md`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.3.16.1678978980/setup.py` & `zesty.zbs-api-1.0.2023.4.10.1681110487/setup.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.3.16.1678978980/src/actions.py` & `zesty.zbs-api-1.0.2023.4.10.1681110487/src/actions.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/BlockDevice.py` & `zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/BlockDevice.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/EbsVolume.py` & `zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/EbsVolume.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,26 +83,27 @@
         self.potential_savings = volume_aws_schema.get("potential_savings", 0)
 
     def __repr__(self):
         return f"{self.__tablename__}:{self.volume_id}"
 
     @classmethod
     def instance_id_filter(cls, query: Query, value: str):
+        val = f'%{value}%'
         query = query.filter(
             case((or_(cls.attached_to == None, func.json_array_length(cls.attached_to) == 0), False),
-                 else_=func.jsonb(cls.attached_to).op('?')(value)))
+                 else_=cast(cls.attached_to, String).ilike(val)))
         return query
 
     @classmethod
     def instance_name_filter(cls, query: Query, value: str):
         subq = query.session.query(InstancesTags.instance_name)
-
-        query = query.filter(subq.scalar_subquery().where(
+        val = '%{}%'.format(value.replace("%", "\\%"))
+        query = query.filter((subq.scalar_subquery().where(
             (func.jsonb(cls.attached_to).op('->>')(0) == InstancesTags.instance_id) & (
-                cls.account_id == InstancesTags.account_id)) == value)
+                cls.account_id == InstancesTags.account_id))).ilike(val))
         return query
 
     @classmethod
     def instance_tags_filter(cls, query: Query, value: str):
         session = query.session
         subq = session.query(InstancesTags.instance_tags)
```

### Comparing `zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/FileSystem.py` & `zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/FileSystem.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/InstancesTags.py` & `zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/InstancesTags.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/ManagedFS.py` & `zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/ManagedFS.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/Usage.py` & `zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/Usage.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/agent_report.py` & `zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/agent_report.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/cpu_mon.py` & `zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/cpu_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/disk_mon.py` & `zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/disk_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/hf_interface.py` & `zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/hf_interface.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.3.16.1678978980/src/models/overview.py` & `zesty.zbs-api-1.0.2023.4.10.1681110487/src/models/overview.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.3.16.1678978980/src/protocol.py` & `zesty.zbs-api-1.0.2023.4.10.1681110487/src/protocol.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-1.0.2023.3.16.1678978980/zesty.zbs_api.egg-info/PKG-INFO` & `zesty.zbs-api-1.0.2023.4.10.1681110487/zesty.zbs_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api
-Version: 1.0.2023.3.16.1678978980
+Version: 1.0.2023.4.10.1681110487
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-1.0.2023.3.16.1678978980/zesty.zbs_api.egg-info/SOURCES.txt` & `zesty.zbs-api-1.0.2023.4.10.1681110487/zesty.zbs_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/cwsearch_utils-0.0.3-py3-none-any.whl.zip` & `tmp/cwsearch_utils-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4808 bytes, number of entries: 7
+Zip file size: 4814 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 04:52 cwsearch_utils/__init__.py
 -rw-rw-r--  2.0 unx     7097 b- defN 23-Apr-09 04:52 cwsearch_utils/aggregate.py
--rw-rw-r--  2.0 unx     4316 b- defN 23-Apr-10 02:25 cwsearch_utils/infinstor_lock.py
--rw-rw-r--  2.0 unx      570 b- defN 23-Apr-10 02:26 cwsearch_utils-0.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-10 02:26 cwsearch_utils-0.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-10 02:26 cwsearch_utils-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      578 b- defN 23-Apr-10 02:26 cwsearch_utils-0.0.3.dist-info/RECORD
-7 files, 12668 bytes uncompressed, 3772 bytes compressed:  70.2%
+-rw-rw-r--  2.0 unx     4326 b- defN 23-Apr-10 02:36 cwsearch_utils/infinstor_lock.py
+-rw-rw-r--  2.0 unx      570 b- defN 23-Apr-10 02:36 cwsearch_utils-0.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-10 02:36 cwsearch_utils-0.0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-10 02:36 cwsearch_utils-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      578 b- defN 23-Apr-10 02:36 cwsearch_utils-0.0.4.dist-info/RECORD
+7 files, 12678 bytes uncompressed, 3778 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: cwsearch_utils/aggregate.py
 Comment: 
 
 Filename: cwsearch_utils/infinstor_lock.py
 Comment: 
 
-Filename: cwsearch_utils-0.0.3.dist-info/METADATA
+Filename: cwsearch_utils-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: cwsearch_utils-0.0.3.dist-info/WHEEL
+Filename: cwsearch_utils-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: cwsearch_utils-0.0.3.dist-info/top_level.txt
+Filename: cwsearch_utils-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: cwsearch_utils-0.0.3.dist-info/RECORD
+Filename: cwsearch_utils-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cwsearch_utils/infinstor_lock.py

```diff
@@ -1,10 +1,11 @@
 import datetime
 import tempfile
 import json
+import os
 
 def set_start(s3client, bucket, prefix, infinstor_time_spec):
     import botocore
     # this is not really a locking mechanism - the prev ddb conditional put based code was
     status_object_name = f"{prefix}/index/{infinstor_time_spec}/names.json.creating"
     try:
         metadata = s3client.head_object(Bucket=bucket, Key=status_object_name)
```

## Comparing `cwsearch_utils-0.0.3.dist-info/METADATA` & `cwsearch_utils-0.0.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwsearch-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: InfinStor InfinLogs CloudWatch Search Utilities
 Home-page: https://infinstor.com/
 Author: InfinStor, Inc.
 Author-email: support@infinstor.com
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

## Comparing `cwsearch_utils-0.0.3.dist-info/RECORD` & `cwsearch_utils-0.0.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 cwsearch_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cwsearch_utils/aggregate.py,sha256=dY3E3EPH4yB1JOcGoZ_ei6XP1LMeuVjmTbjkAoNIGbE,7097
-cwsearch_utils/infinstor_lock.py,sha256=qkslqabj3VZ9r7X5770Q3s3xF-3fLPyGjAYadSa-0CA,4316
-cwsearch_utils-0.0.3.dist-info/METADATA,sha256=RiCu2EH9eLom9iwro0Sfd2WkHZYZQ5LT8KkZ_c8pN80,570
-cwsearch_utils-0.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-cwsearch_utils-0.0.3.dist-info/top_level.txt,sha256=OGqL3fU8yTeTOI4vTn4QZa2PZY145LPKbmtLSjWi9kY,15
-cwsearch_utils-0.0.3.dist-info/RECORD,,
+cwsearch_utils/infinstor_lock.py,sha256=Ah1GvX1DXbMaYhoDQdSAZxpcSDFVjDPqUg7fZEmIbRI,4326
+cwsearch_utils-0.0.4.dist-info/METADATA,sha256=7Dzq5MJoPFRx4PSkZZVF02XF46nm8PP96w7uATY8r7w,570
+cwsearch_utils-0.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+cwsearch_utils-0.0.4.dist-info/top_level.txt,sha256=OGqL3fU8yTeTOI4vTn4QZa2PZY145LPKbmtLSjWi9kY,15
+cwsearch_utils-0.0.4.dist-info/RECORD,,
```


# Comparing `tmp/cwsearch_utils-0.0.2-py3-none-any.whl.zip` & `tmp/cwsearch_utils-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4807 bytes, number of entries: 7
+Zip file size: 4808 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 04:52 cwsearch_utils/__init__.py
 -rw-rw-r--  2.0 unx     7097 b- defN 23-Apr-09 04:52 cwsearch_utils/aggregate.py
--rw-rw-r--  2.0 unx     4304 b- defN 23-Apr-10 00:01 cwsearch_utils/infinstor_lock.py
--rw-rw-r--  2.0 unx      570 b- defN 23-Apr-10 00:02 cwsearch_utils-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-10 00:02 cwsearch_utils-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-10 00:02 cwsearch_utils-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      578 b- defN 23-Apr-10 00:02 cwsearch_utils-0.0.2.dist-info/RECORD
-7 files, 12656 bytes uncompressed, 3771 bytes compressed:  70.2%
+-rw-rw-r--  2.0 unx     4316 b- defN 23-Apr-10 02:25 cwsearch_utils/infinstor_lock.py
+-rw-rw-r--  2.0 unx      570 b- defN 23-Apr-10 02:26 cwsearch_utils-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-10 02:26 cwsearch_utils-0.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-10 02:26 cwsearch_utils-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      578 b- defN 23-Apr-10 02:26 cwsearch_utils-0.0.3.dist-info/RECORD
+7 files, 12668 bytes uncompressed, 3772 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: cwsearch_utils/aggregate.py
 Comment: 
 
 Filename: cwsearch_utils/infinstor_lock.py
 Comment: 
 
-Filename: cwsearch_utils-0.0.2.dist-info/METADATA
+Filename: cwsearch_utils-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: cwsearch_utils-0.0.2.dist-info/WHEEL
+Filename: cwsearch_utils-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: cwsearch_utils-0.0.2.dist-info/top_level.txt
+Filename: cwsearch_utils-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: cwsearch_utils-0.0.2.dist-info/RECORD
+Filename: cwsearch_utils-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cwsearch_utils/infinstor_lock.py

```diff
@@ -1,9 +1,10 @@
 import datetime
 import tempfile
+import json
 
 def set_start(s3client, bucket, prefix, infinstor_time_spec):
     import botocore
     # this is not really a locking mechanism - the prev ddb conditional put based code was
     status_object_name = f"{prefix}/index/{infinstor_time_spec}/names.json.creating"
     try:
         metadata = s3client.head_object(Bucket=bucket, Key=status_object_name)
```

## Comparing `cwsearch_utils-0.0.2.dist-info/METADATA` & `cwsearch_utils-0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwsearch-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: InfinStor InfinLogs CloudWatch Search Utilities
 Home-page: https://infinstor.com/
 Author: InfinStor, Inc.
 Author-email: support@infinstor.com
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```


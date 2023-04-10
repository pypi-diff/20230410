# Comparing `tmp/awsimple-2.3.1-py3-none-any.whl.zip` & `tmp/awsimple-2.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 32265 bytes, number of entries: 18
+Zip file size: 32289 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      849 b- defN 23-Apr-10 03:01 awsimple/__init__.py
--rw-rw-rw-  2.0 fat      323 b- defN 23-Apr-10 02:55 awsimple/__version__.py
+-rw-rw-rw-  2.0 fat      323 b- defN 23-Apr-10 05:34 awsimple/__version__.py
 -rw-rw-rw-  2.0 fat     6365 b- defN 23-Mar-14 23:35 awsimple/aws.py
 -rw-rw-rw-  2.0 fat     7137 b- defN 23-Mar-14 23:35 awsimple/cache.py
--rw-rw-rw-  2.0 fat    35444 b- defN 23-Apr-10 03:01 awsimple/dynamodb.py
+-rw-rw-rw-  2.0 fat    35928 b- defN 23-Apr-10 05:39 awsimple/dynamodb.py
 -rw-rw-rw-  2.0 fat     4619 b- defN 23-Mar-14 23:35 awsimple/dynamodb_miv.py
 -rw-rw-rw-  2.0 fat     4278 b- defN 23-Mar-14 23:10 awsimple/logs.py
 -rw-rw-rw-  2.0 fat      199 b- defN 23-Mar-14 23:10 awsimple/mock.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-14 23:10 awsimple/py.typed
 -rw-rw-rw-  2.0 fat    23243 b- defN 23-Mar-14 23:35 awsimple/s3.py
 -rw-rw-rw-  2.0 fat     3266 b- defN 23-Mar-14 23:10 awsimple/sns.py
 -rw-rw-rw-  2.0 fat    13007 b- defN 23-Mar-14 23:35 awsimple/sqs.py
--rw-rw-rw-  2.0 fat     1093 b- defN 23-Apr-10 03:04 awsimple-2.3.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1093 b- defN 23-Apr-10 03:04 awsimple-2.3.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     4815 b- defN 23-Apr-10 03:04 awsimple-2.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 03:04 awsimple-2.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-10 03:04 awsimple-2.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1376 b- defN 23-Apr-10 03:04 awsimple-2.3.1.dist-info/RECORD
-18 files, 107208 bytes uncompressed, 30051 bytes compressed:  72.0%
+-rw-rw-rw-  2.0 fat     1093 b- defN 23-Apr-10 05:43 awsimple-2.3.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1093 b- defN 23-Apr-10 05:43 awsimple-2.3.2.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     4815 b- defN 23-Apr-10 05:43 awsimple-2.3.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 05:43 awsimple-2.3.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-10 05:43 awsimple-2.3.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1376 b- defN 23-Apr-10 05:43 awsimple-2.3.2.dist-info/RECORD
+18 files, 107692 bytes uncompressed, 30075 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: awsimple/sns.py
 Comment: 
 
 Filename: awsimple/sqs.py
 Comment: 
 
-Filename: awsimple-2.3.1.dist-info/LICENSE
+Filename: awsimple-2.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: awsimple-2.3.1.dist-info/LICENSE.txt
+Filename: awsimple-2.3.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: awsimple-2.3.1.dist-info/METADATA
+Filename: awsimple-2.3.2.dist-info/METADATA
 Comment: 
 
-Filename: awsimple-2.3.1.dist-info/WHEEL
+Filename: awsimple-2.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: awsimple-2.3.1.dist-info/top_level.txt
+Filename: awsimple-2.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: awsimple-2.3.1.dist-info/RECORD
+Filename: awsimple-2.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awsimple/__version__.py

```diff
@@ -1,8 +1,8 @@
 __application_name__ = "awsimple"
 __title__ = __application_name__
 __author__ = "abel"
-__version__ = "2.3.1"
+__version__ = "2.3.2"
 __author_email__ = "j@abel.co"
 __url__ = "https://github.com/jamesabel/awsimple"
 __download_url__ = "https://github.com/jamesabel/awsimple"
 __description__ = "Simple AWS API for S3, DynamoDB, SNS, and SQS"
```

## awsimple/dynamodb.py

```diff
@@ -723,16 +723,22 @@
     def put_item(self, item: dict):
         """
         Put (write) a DynamoDB table dict item.
 
         :param item: item
         """
         assert self.resource is not None
-        table = self.resource.Table(self.table_name)
-        table.put_item(Item=item)
+        try:
+            table = self.resource.Table(self.table_name)
+            table.put_item(Item=item)
+        except ClientError as e:
+            if e.response["Error"]["Code"] == "ResourceNotFoundException":
+                raise DynamoDBTableNotFound(self.table_name)
+            else:
+                raise
 
     # cant' do a @typechecked() since optional item requires a single type
     def get_item(self, partition_key: str = None, partition_value: Union[str, int] = None, sort_key: Union[str, None] = None, sort_value: Union[str, int] = None) -> dict:
         """
         Get a DB item using the primary keys. Raise DBItemNotFound if item does not exist.
 
         :param partition_key: partition key (optional - if not given or None AWSimple will provide it)
@@ -744,19 +750,25 @@
 
         if partition_key is None:
             partition_key = self.get_primary_partition_key()
         if sort_key is None and sort_value is not None:
             sort_key = self.get_primary_sort_key()
 
         assert self.resource is not None
-        table = self.resource.Table(self.table_name)
-        key = {partition_key: partition_value}  # type: Dict[str, Any]
-        if sort_key is not None:
-            key[sort_key] = sort_value
-        response = table.get_item(Key=key)
+        try:
+            table = self.resource.Table(self.table_name)
+            key = {partition_key: partition_value}  # type: Dict[str, Any]
+            if sort_key is not None:
+                key[sort_key] = sort_value
+            response = table.get_item(Key=key)
+        except ClientError as e:
+            if e.response["Error"]["Code"] == "ResourceNotFoundException":
+                raise DynamoDBTableNotFound(self.table_name)
+            else:
+                raise
         if (item := response.get("Item")) is None:
             raise DBItemNotFound(key)
         return item
 
     # cant' do a @typechecked() since optional item requires a single type
     def delete_item(self, partition_key: str = None, partition_value: Union[str, int] = None, sort_key: Union[str, None] = None, sort_value: Union[str, int, None] = None):
         """
```

## Comparing `awsimple-2.3.1.dist-info/LICENSE` & `awsimple-2.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `awsimple-2.3.1.dist-info/LICENSE.txt` & `awsimple-2.3.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `awsimple-2.3.1.dist-info/METADATA` & `awsimple-2.3.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsimple
-Version: 2.3.1
+Version: 2.3.2
 Summary: Simple AWS API for S3, DynamoDB, SNS, and SQS
 Home-page: https://github.com/jamesabel/awsimple
 Download-URL: https://github.com/jamesabel/awsimple
 Author: abel
 Author-email: j@abel.co
 License: MIT License
 Project-URL: Documentation, https://awsimple.readthedocs.io/
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: awsimple Version: 2.3.1 Summary: Simple AWS API for
+Metadata-Version: 2.1 Name: awsimple Version: 2.3.2 Summary: Simple AWS API for
 S3, DynamoDB, SNS, and SQS Home-page: https://github.com/jamesabel/awsimple
 Download-URL: https://github.com/jamesabel/awsimple Author: abel Author-email:
 j@abel.co License: MIT License Project-URL: Documentation, https://
 awsimple.readthedocs.io/ Keywords: aws,cloud,storage,database,dynamodb,s3
 Description-Content-Type: text/markdown License-File: LICENSE License-File:
 LICENSE.txt Requires-Dist: boto3 Requires-Dist: typeguard (<3) Requires-Dist:
 hashy (>=0.1.1) Requires-Dist: dictim Requires-Dist: appdirs Requires-Dist:
```

## Comparing `awsimple-2.3.1.dist-info/RECORD` & `awsimple-2.3.2.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 awsimple/__init__.py,sha256=l6fv2r0Lsk7mxratOIjfqZOHxPQyPfke_ZM4O5OznEc,849
-awsimple/__version__.py,sha256=coAoM3Hy0V06jEpbb106mahyhZbYU9SCNDMXIx-biPQ,323
+awsimple/__version__.py,sha256=3UBIMBsqsZsvWHMKe9oGVzCxBAmoY9DtD-snKI8U-Po,323
 awsimple/aws.py,sha256=006liY2mXwbPu5kl3-nCgmkpMN7pBqEDetqM1eNbXWU,6365
 awsimple/cache.py,sha256=5dYf7bh1Dr_pFbkHck4Ym8zrffctv0ERhGJwieRHQH8,7137
-awsimple/dynamodb.py,sha256=MzU0II2AcyxW9BY0PUG83hxapjBGUgis92c1aRj7mPg,35444
+awsimple/dynamodb.py,sha256=d8iDvi8UuJTVBBl0coifrEYR1O0SSnJTn-GuLUiUI6M,35928
 awsimple/dynamodb_miv.py,sha256=FcbEn2VbrYxQcgQKqFoWFqVwAkoqJpwZ4Nr5guXgGXM,4619
 awsimple/logs.py,sha256=A2RmTT90pfFTthfENd7GSsEHSIBJXO8ICHPdA7sEsHY,4278
 awsimple/mock.py,sha256=32CNU656uC3PBhjCJ4R-WBTtHbSl6VNVkpN8G8XDvsQ,199
 awsimple/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 awsimple/s3.py,sha256=uMEz6NN9hXOfsQNUNJ2YOuKGKlT2xqZ5btJ9zsCHBrY,23243
 awsimple/sns.py,sha256=LjKj-UxPdfRDQfN10jU_ULjnlEqLmHcuqfRIKX9lkZo,3266
 awsimple/sqs.py,sha256=yf8a9jGbYzdajeDU3rARFFYoMb3jQ-YJAVNvw4WscW8,13007
-awsimple-2.3.1.dist-info/LICENSE,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
-awsimple-2.3.1.dist-info/LICENSE.txt,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
-awsimple-2.3.1.dist-info/METADATA,sha256=5qZBcrVjnaBcXp0nC53o9-P2qCqoRMDnoe_dk9Oa1fU,4815
-awsimple-2.3.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-awsimple-2.3.1.dist-info/top_level.txt,sha256=mwqCoH_8vAaK6iYioiRbasXmVCQM7AK3grNWOKp2VHE,9
-awsimple-2.3.1.dist-info/RECORD,,
+awsimple-2.3.2.dist-info/LICENSE,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
+awsimple-2.3.2.dist-info/LICENSE.txt,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
+awsimple-2.3.2.dist-info/METADATA,sha256=96hyE0-Qgl_fDQje0xlReCAoWTiD6mTMG0Sat53JRok,4815
+awsimple-2.3.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+awsimple-2.3.2.dist-info/top_level.txt,sha256=mwqCoH_8vAaK6iYioiRbasXmVCQM7AK3grNWOKp2VHE,9
+awsimple-2.3.2.dist-info/RECORD,,
```


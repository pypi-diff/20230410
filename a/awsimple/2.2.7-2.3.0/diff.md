# Comparing `tmp/awsimple-2.2.7-py3-none-any.whl.zip` & `tmp/awsimple-2.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 32174 bytes, number of entries: 18
+Zip file size: 32264 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      826 b- defN 23-Mar-14 23:10 awsimple/__init__.py
--rw-rw-rw-  2.0 fat      323 b- defN 23-Mar-14 23:16 awsimple/__version__.py
+-rw-rw-rw-  2.0 fat      323 b- defN 23-Apr-10 02:44 awsimple/__version__.py
 -rw-rw-rw-  2.0 fat     6365 b- defN 23-Mar-14 23:35 awsimple/aws.py
 -rw-rw-rw-  2.0 fat     7137 b- defN 23-Mar-14 23:35 awsimple/cache.py
--rw-rw-rw-  2.0 fat    34850 b- defN 23-Mar-14 23:35 awsimple/dynamodb.py
+-rw-rw-rw-  2.0 fat    35424 b- defN 23-Apr-10 02:44 awsimple/dynamodb.py
 -rw-rw-rw-  2.0 fat     4619 b- defN 23-Mar-14 23:35 awsimple/dynamodb_miv.py
 -rw-rw-rw-  2.0 fat     4278 b- defN 23-Mar-14 23:10 awsimple/logs.py
 -rw-rw-rw-  2.0 fat      199 b- defN 23-Mar-14 23:10 awsimple/mock.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-14 23:10 awsimple/py.typed
 -rw-rw-rw-  2.0 fat    23243 b- defN 23-Mar-14 23:35 awsimple/s3.py
 -rw-rw-rw-  2.0 fat     3266 b- defN 23-Mar-14 23:10 awsimple/sns.py
 -rw-rw-rw-  2.0 fat    13007 b- defN 23-Mar-14 23:35 awsimple/sqs.py
--rw-rw-rw-  2.0 fat     1093 b- defN 23-Mar-15 00:00 awsimple-2.2.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1093 b- defN 23-Mar-15 00:00 awsimple-2.2.7.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     4815 b- defN 23-Mar-15 00:00 awsimple-2.2.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-15 00:00 awsimple-2.2.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Mar-15 00:00 awsimple-2.2.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1376 b- defN 23-Mar-15 00:00 awsimple-2.2.7.dist-info/RECORD
-18 files, 106591 bytes uncompressed, 29960 bytes compressed:  71.9%
+-rw-rw-rw-  2.0 fat     1093 b- defN 23-Apr-10 02:48 awsimple-2.3.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1093 b- defN 23-Apr-10 02:48 awsimple-2.3.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     4815 b- defN 23-Apr-10 02:48 awsimple-2.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 02:48 awsimple-2.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-10 02:48 awsimple-2.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1376 b- defN 23-Apr-10 02:48 awsimple-2.3.0.dist-info/RECORD
+18 files, 107165 bytes uncompressed, 30050 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: awsimple/sns.py
 Comment: 
 
 Filename: awsimple/sqs.py
 Comment: 
 
-Filename: awsimple-2.2.7.dist-info/LICENSE
+Filename: awsimple-2.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: awsimple-2.2.7.dist-info/LICENSE.txt
+Filename: awsimple-2.3.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: awsimple-2.2.7.dist-info/METADATA
+Filename: awsimple-2.3.0.dist-info/METADATA
 Comment: 
 
-Filename: awsimple-2.2.7.dist-info/WHEEL
+Filename: awsimple-2.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: awsimple-2.2.7.dist-info/top_level.txt
+Filename: awsimple-2.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: awsimple-2.2.7.dist-info/RECORD
+Filename: awsimple-2.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awsimple/__version__.py

```diff
@@ -1,8 +1,8 @@
 __application_name__ = "awsimple"
 __title__ = __application_name__
 __author__ = "abel"
-__version__ = "2.2.7"
+__version__ = "2.3.0"
 __author_email__ = "j@abel.co"
 __url__ = "https://github.com/jamesabel/awsimple"
 __download_url__ = "https://github.com/jamesabel/awsimple"
 __description__ = "Simple AWS API for S3, DynamoDB, SNS, and SQS"
```

## awsimple/dynamodb.py

```diff
@@ -189,14 +189,21 @@
         self.message = "Item not found"
         super().__init__(self.message)
 
     def __str__(self):
         return f"{self.key=} {self.message}"
 
 
+class TableNotFound(AWSimpleException):
+    def __init__(self, table_name: str):
+        self.table_name = table_name
+        self.message = f'Table "{self.table_name}" not found'
+        super().__init__(self.message)
+
+
 @typechecked()
 def _is_valid_db_pickled_file(file_path: Path, cache_life: Union[float, int, None]) -> bool:
     is_valid = file_path.exists() and getsize(str(file_path)) > 0
     if is_valid and cache_life is not None:
         is_valid = time.time() <= getmtime(str(file_path)) + cache_life
     return is_valid
 
@@ -509,21 +516,30 @@
         for table_key_schema in table_schema:
             key_schema[aws_name_to_key_type[table_key_schema["KeyType"]]] = table_key_schema["AttributeName"]
         return key_schema
 
     @lru_cache()
     def get_primary_keys_dict(self) -> Dict[KeyType, str]:
         """
-        Get the table's primary keys.
+        Get the table's primary keys. Raise TableNotFound if table does not exist.
 
         :return: a dict with the primary key partition key and (optionally) sort key
         """
 
         assert self.resource is not None
-        return self._get_keys_from_schema(self.resource.Table(self.table_name).key_schema)
+        try:
+            table = self.resource.Table(self.table_name)
+        except ClientError as e:
+            if e.response["Error"]["Code"] == "ResourceNotFoundException":
+                raise TableNotFound(self.table_name)
+            else:
+                raise
+        key_schema = table.key_schema
+        keys = self._get_keys_from_schema(key_schema)
+        return keys
 
     @lru_cache()
     def get_primary_partition_key(self) -> str:
         primary_keys = self.get_primary_keys_dict()
         return primary_keys[KeyType.partition]
 
     @lru_cache()
```

## Comparing `awsimple-2.2.7.dist-info/LICENSE` & `awsimple-2.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `awsimple-2.2.7.dist-info/LICENSE.txt` & `awsimple-2.3.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `awsimple-2.2.7.dist-info/METADATA` & `awsimple-2.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsimple
-Version: 2.2.7
+Version: 2.3.0
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
-Metadata-Version: 2.1 Name: awsimple Version: 2.2.7 Summary: Simple AWS API for
+Metadata-Version: 2.1 Name: awsimple Version: 2.3.0 Summary: Simple AWS API for
 S3, DynamoDB, SNS, and SQS Home-page: https://github.com/jamesabel/awsimple
 Download-URL: https://github.com/jamesabel/awsimple Author: abel Author-email:
 j@abel.co License: MIT License Project-URL: Documentation, https://
 awsimple.readthedocs.io/ Keywords: aws,cloud,storage,database,dynamodb,s3
 Description-Content-Type: text/markdown License-File: LICENSE License-File:
 LICENSE.txt Requires-Dist: boto3 Requires-Dist: typeguard (<3) Requires-Dist:
 hashy (>=0.1.1) Requires-Dist: dictim Requires-Dist: appdirs Requires-Dist:
```

## Comparing `awsimple-2.2.7.dist-info/RECORD` & `awsimple-2.3.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 awsimple/__init__.py,sha256=8NChv83C13WICTMbi89I78fAKSE3UQtcGq4YwXAl3OU,826
-awsimple/__version__.py,sha256=tpBmONFR_MjuaSt3LDsjvTmzAaVOd-Hx4KEAFGBlsxU,323
+awsimple/__version__.py,sha256=ou_bUclq3bwRO56DBjSReyO_DcrTw2lpPq15hmhVUQw,323
 awsimple/aws.py,sha256=006liY2mXwbPu5kl3-nCgmkpMN7pBqEDetqM1eNbXWU,6365
 awsimple/cache.py,sha256=5dYf7bh1Dr_pFbkHck4Ym8zrffctv0ERhGJwieRHQH8,7137
-awsimple/dynamodb.py,sha256=QLU1vnxPcX5v4nSnf0itLcHRDjKR5KpQQbUSuD96qaA,34850
+awsimple/dynamodb.py,sha256=zCinM2oE26Rtl8Vb9kp8UmgDV1HiVXzSfMiJO-XS8aA,35424
 awsimple/dynamodb_miv.py,sha256=FcbEn2VbrYxQcgQKqFoWFqVwAkoqJpwZ4Nr5guXgGXM,4619
 awsimple/logs.py,sha256=A2RmTT90pfFTthfENd7GSsEHSIBJXO8ICHPdA7sEsHY,4278
 awsimple/mock.py,sha256=32CNU656uC3PBhjCJ4R-WBTtHbSl6VNVkpN8G8XDvsQ,199
 awsimple/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 awsimple/s3.py,sha256=uMEz6NN9hXOfsQNUNJ2YOuKGKlT2xqZ5btJ9zsCHBrY,23243
 awsimple/sns.py,sha256=LjKj-UxPdfRDQfN10jU_ULjnlEqLmHcuqfRIKX9lkZo,3266
 awsimple/sqs.py,sha256=yf8a9jGbYzdajeDU3rARFFYoMb3jQ-YJAVNvw4WscW8,13007
-awsimple-2.2.7.dist-info/LICENSE,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
-awsimple-2.2.7.dist-info/LICENSE.txt,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
-awsimple-2.2.7.dist-info/METADATA,sha256=G6NcEE7ZUWuM5OI5BHy4AwpzkAyHI720NbPA8MMCWx8,4815
-awsimple-2.2.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-awsimple-2.2.7.dist-info/top_level.txt,sha256=mwqCoH_8vAaK6iYioiRbasXmVCQM7AK3grNWOKp2VHE,9
-awsimple-2.2.7.dist-info/RECORD,,
+awsimple-2.3.0.dist-info/LICENSE,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
+awsimple-2.3.0.dist-info/LICENSE.txt,sha256=d956YAgtDaxgxQmccyUk__EfhORZyBjvmJ8pq6zYTxk,1093
+awsimple-2.3.0.dist-info/METADATA,sha256=SQAOmvSYRqftTUXxK05S4BaUPKnpJmfragonG5oUfmM,4815
+awsimple-2.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+awsimple-2.3.0.dist-info/top_level.txt,sha256=mwqCoH_8vAaK6iYioiRbasXmVCQM7AK3grNWOKp2VHE,9
+awsimple-2.3.0.dist-info/RECORD,,
```


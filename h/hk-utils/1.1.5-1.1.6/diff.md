# Comparing `tmp/hk_utils-1.1.5-py3-none-any.whl.zip` & `tmp/hk_utils-1.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4755 bytes, number of entries: 7
--rw-r--r--  2.0 unx     4892 b- defN 23-Apr-01 12:13 hk_utils/AttrDict.py
+Zip file size: 4800 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     5288 b- defN 23-Apr-10 10:25 hk_utils/AttrDict.py
 -rw-r--r--  2.0 unx       93 b- defN 23-Mar-31 17:26 hk_utils/__init__.py
 -rw-r--r--  2.0 unx     7020 b- defN 23-Mar-31 17:11 hk_utils/hk_print.py
--rw-r--r--  2.0 unx     2199 b- defN 23-Apr-01 12:13 hk_utils-1.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-01 12:13 hk_utils-1.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-01 12:13 hk_utils-1.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      530 b- defN 23-Apr-01 12:13 hk_utils-1.1.5.dist-info/RECORD
-7 files, 14835 bytes uncompressed, 3817 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx     2199 b- defN 23-Apr-10 10:25 hk_utils-1.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 10:25 hk_utils-1.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-10 10:25 hk_utils-1.1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      530 b- defN 23-Apr-10 10:25 hk_utils-1.1.6.dist-info/RECORD
+7 files, 15231 bytes uncompressed, 3862 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: hk_utils/__init__.py
 Comment: 
 
 Filename: hk_utils/hk_print.py
 Comment: 
 
-Filename: hk_utils-1.1.5.dist-info/METADATA
+Filename: hk_utils-1.1.6.dist-info/METADATA
 Comment: 
 
-Filename: hk_utils-1.1.5.dist-info/WHEEL
+Filename: hk_utils-1.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: hk_utils-1.1.5.dist-info/top_level.txt
+Filename: hk_utils-1.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: hk_utils-1.1.5.dist-info/RECORD
+Filename: hk_utils-1.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hk_utils/AttrDict.py

```diff
@@ -18,15 +18,25 @@
             return {self._deep_convert(x) for x in value}
         elif type(value) == dict:
             return AttrDict(value)            
         else:
             return value
     
     def to_dict(self):
-        return self.__dict__
+        def _convert(value):
+            if type(value) == AttrDict:
+                return value.to_dict()
+            elif type(value) == list:
+                return [_convert(x) for x in value]
+            elif type(value) == set:
+                return {_convert(x) for x in value}
+            else:
+                return value
+            
+        return {key: _convert(value) for key, value in self.__dict__.items()}
 
     @classmethod
     def from_dict(cls, input):
         return cls(input)
     
     def __getattr__(self, key):
         return None # fallback to None if key not exists in self.__dict__
```

## Comparing `hk_utils-1.1.5.dist-info/METADATA` & `hk_utils-1.1.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hk-utils
-Version: 1.1.5
+Version: 1.1.6
 Summary: Python utilities by Heekang Park
 Home-page: https://github.com/HeekangPark/hk-utils
 Author: Heekang Park
 Author-email: park.heekang33@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `hk_utils-1.1.5.dist-info/RECORD` & `hk_utils-1.1.6.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-hk_utils/AttrDict.py,sha256=F0Nrq7ugMFvtAfHw-O-VIIuhDblidgMMJq_hfgCUF7o,4892
+hk_utils/AttrDict.py,sha256=GaHUSLc_Q1FYBGoRtEIyRfZ64MggNe4HGY1rVewNhi0,5288
 hk_utils/__init__.py,sha256=mQu3VH4LjeP4-KC0gOT-W3SlCsSULJZdDLvJXhlI2sc,93
 hk_utils/hk_print.py,sha256=Kh-cEH9_bG1FkPmjLmsgpjdjmIbPf-QqRqzIYX2RMeg,7020
-hk_utils-1.1.5.dist-info/METADATA,sha256=TOOGrem4Kb9LvZxfWkbggnPt0P9UcCid3kG4GQTnGnc,2199
-hk_utils-1.1.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-hk_utils-1.1.5.dist-info/top_level.txt,sha256=KovoCC2COkWtn8xwvS7e0Xstxx7q84hD_OiZsl-mn0E,9
-hk_utils-1.1.5.dist-info/RECORD,,
+hk_utils-1.1.6.dist-info/METADATA,sha256=O3gvh9wMwOB99Nm8MHS8zhbiBREE_hbLT1mAiSh4Ot8,2199
+hk_utils-1.1.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+hk_utils-1.1.6.dist-info/top_level.txt,sha256=KovoCC2COkWtn8xwvS7e0Xstxx7q84hD_OiZsl-mn0E,9
+hk_utils-1.1.6.dist-info/RECORD,,
```


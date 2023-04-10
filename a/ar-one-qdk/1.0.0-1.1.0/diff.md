# Comparing `tmp/ar_one_qdk-1.0.0-py3-none-any.whl.zip` & `tmp/ar_one_qdk-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5003 bytes, number of entries: 9
+Zip file size: 5006 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Oct-13 06:51 ar_qdk/__init__.py
--rw-rw-rw-  2.0 fat     8704 b- defN 23-Mar-01 08:52 ar_qdk/main.py
+-rw-rw-rw-  2.0 fat     8724 b- defN 23-Apr-10 08:18 ar_qdk/main.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Oct-13 08:32 ar_qdk/tests/__init__.py
 -rw-rw-rw-  2.0 fat     1007 b- defN 22-Mar-17 06:07 ar_qdk/tests/main_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Mar-01 08:53 ar_one_qdk-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      229 b- defN 23-Mar-01 08:53 ar_one_qdk-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-01 08:53 ar_one_qdk-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Mar-01 08:53 ar_one_qdk-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      702 b- defN 23-Mar-01 08:53 ar_one_qdk-1.0.0.dist-info/RECORD
-9 files, 11832 bytes uncompressed, 3787 bytes compressed:  68.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-10 08:19 ar_one_qdk-1.1.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      229 b- defN 23-Apr-10 08:19 ar_one_qdk-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 08:19 ar_one_qdk-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-10 08:19 ar_one_qdk-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      702 b- defN 23-Apr-10 08:19 ar_one_qdk-1.1.0.dist-info/RECORD
+9 files, 11852 bytes uncompressed, 3790 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: ar_qdk/tests/__init__.py
 Comment: 
 
 Filename: ar_qdk/tests/main_test.py
 Comment: 
 
-Filename: ar_one_qdk-1.0.0.dist-info/LICENSE
+Filename: ar_one_qdk-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: ar_one_qdk-1.0.0.dist-info/METADATA
+Filename: ar_one_qdk-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: ar_one_qdk-1.0.0.dist-info/WHEEL
+Filename: ar_one_qdk-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: ar_one_qdk-1.0.0.dist-info/top_level.txt
+Filename: ar_one_qdk-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ar_one_qdk-1.0.0.dist-info/RECORD
+Filename: ar_one_qdk-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ar_qdk/main.py

```diff
@@ -34,25 +34,25 @@
         :param comment: Комментарий.
         :return:
         """
         return self.execute_method('add_comment', record_id=record_id,
                                    comment=comment)
 
     def operate_gate_manual_control(self, operation, gate_name,
-                                    auto_close=False):
+                                    auto_close=False, **kwargs):
         """
         Работа со шлагбаумами.
 
         :param operation: Название операции (close|open):
         :param gate_name: Имя шлагбаума (entry/exit)
         :return:
         """
         return self.execute_method('operate_gate_manual_control',
                                    operation=operation, gate_name=gate_name,
-                                   auto_close=auto_close)
+                                   auto_close=auto_close, **kwargs)
 
     def change_opened_record(self, record_id, auto_id, car_number, carrier,
                              trash_cat_id, trash_type_id, comment, pol_object,
                              client=None, polygon=None):
         """
         Изменить открытую запись.
```

## Comparing `ar_one_qdk-1.0.0.dist-info/LICENSE` & `ar_one_qdk-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ar_one_qdk-1.0.0.dist-info/RECORD` & `ar_one_qdk-1.1.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ar_qdk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ar_qdk/main.py,sha256=DInSBRqcXiFCx2Bq6RbXKheOvIG4qDqslV8XODjupKY,8704
+ar_qdk/main.py,sha256=os3dPL4OptzALmWMUNHJgLdfcz4QsSTdLiX2_WLKnBE,8724
 ar_qdk/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ar_qdk/tests/main_test.py,sha256=19Ha8MLCnbOWOswLnkImWE4eS2nGID2-WPeMfc7huCg,1007
-ar_one_qdk-1.0.0.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-ar_one_qdk-1.0.0.dist-info/METADATA,sha256=6Yf6afR64pWT_r5Fxx4JG7A7CP3P8T3BRj3e2aqFhXk,229
-ar_one_qdk-1.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-ar_one_qdk-1.0.0.dist-info/top_level.txt,sha256=N0T18HgfwhynNtK_8NqrwjG36PbUQIOrlTAUU5WZOPw,7
-ar_one_qdk-1.0.0.dist-info/RECORD,,
+ar_one_qdk-1.1.0.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+ar_one_qdk-1.1.0.dist-info/METADATA,sha256=28Habpzt116Y6o-8daX6wQqrNuo1Q81_9_yk1_JdLCI,229
+ar_one_qdk-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ar_one_qdk-1.1.0.dist-info/top_level.txt,sha256=N0T18HgfwhynNtK_8NqrwjG36PbUQIOrlTAUU5WZOPw,7
+ar_one_qdk-1.1.0.dist-info/RECORD,,
```


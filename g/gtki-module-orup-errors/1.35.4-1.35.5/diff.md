# Comparing `tmp/gtki_module_orup_errors-1.35.4-py3-none-any.whl.zip` & `tmp/gtki_module_orup_errors-1.35.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 12372 bytes, number of entries: 17
+Zip file size: 12374 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Oct-20 07:03 orup_errors/__init__.py
 -rw-rw-rw-  2.0 fat    14496 b- defN 23-Apr-03 08:32 orup_errors/all_errors.py
--rw-rw-rw-  2.0 fat     5012 b- defN 23-Apr-10 12:39 orup_errors/check_funcs.py
+-rw-rw-rw-  2.0 fat     5016 b- defN 23-Apr-10 12:43 orup_errors/check_funcs.py
 -rw-rw-rw-  2.0 fat     2526 b- defN 23-Mar-28 11:24 orup_errors/general_functions.py
 -rw-rw-rw-  2.0 fat     2340 b- defN 23-Mar-28 11:17 orup_errors/main.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Oct-20 07:03 orup_errors/tests/__init__.py
 -rw-rw-rw-  2.0 fat     1545 b- defN 21-Oct-20 07:03 orup_errors/tests/all_errors_test.py
 -rw-rw-rw-  2.0 fat      744 b- defN 21-Oct-20 07:03 orup_errors/tests/args_test.py
 -rw-rw-rw-  2.0 fat      288 b- defN 21-Dec-03 04:31 orup_errors/tests/check_funcs_test.py
 -rw-rw-rw-  2.0 fat     1385 b- defN 21-Oct-20 07:03 orup_errors/tests/draw_win_test.py
 -rw-rw-rw-  2.0 fat     1300 b- defN 21-Dec-03 04:20 orup_errors/tests/general_functions_test.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Oct-20 07:03 orup_errors/tests/orup_errors_operator_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-10 12:40 gtki_module_orup_errors-1.35.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      156 b- defN 23-Apr-10 12:40 gtki_module_orup_errors-1.35.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 12:40 gtki_module_orup_errors-1.35.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-10 12:40 gtki_module_orup_errors-1.35.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1524 b- defN 23-Apr-10 12:40 gtki_module_orup_errors-1.35.4.dist-info/RECORD
-17 files, 32511 bytes uncompressed, 9810 bytes compressed:  69.8%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-10 12:44 gtki_module_orup_errors-1.35.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      156 b- defN 23-Apr-10 12:44 gtki_module_orup_errors-1.35.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 12:44 gtki_module_orup_errors-1.35.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-10 12:44 gtki_module_orup_errors-1.35.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1524 b- defN 23-Apr-10 12:44 gtki_module_orup_errors-1.35.5.dist-info/RECORD
+17 files, 32515 bytes uncompressed, 9812 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: orup_errors/tests/general_functions_test.py
 Comment: 
 
 Filename: orup_errors/tests/orup_errors_operator_test.py
 Comment: 
 
-Filename: gtki_module_orup_errors-1.35.4.dist-info/LICENSE
+Filename: gtki_module_orup_errors-1.35.5.dist-info/LICENSE
 Comment: 
 
-Filename: gtki_module_orup_errors-1.35.4.dist-info/METADATA
+Filename: gtki_module_orup_errors-1.35.5.dist-info/METADATA
 Comment: 
 
-Filename: gtki_module_orup_errors-1.35.4.dist-info/WHEEL
+Filename: gtki_module_orup_errors-1.35.5.dist-info/WHEEL
 Comment: 
 
-Filename: gtki_module_orup_errors-1.35.4.dist-info/top_level.txt
+Filename: gtki_module_orup_errors-1.35.5.dist-info/top_level.txt
 Comment: 
 
-Filename: gtki_module_orup_errors-1.35.4.dist-info/RECORD
+Filename: gtki_module_orup_errors-1.35.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## orup_errors/check_funcs.py

```diff
@@ -85,15 +85,15 @@
     if given.lower() in list_name:
         return True
 
 
 def check_type_incorrectness(given: any, list_name: list, *args, **kwargs):
     """ Проверить факт НЕ нахождение элемента given в list_name """
     list_name = [el.lower() for el in list_name]
-    if given.lower() in list_name:
+    if given.lower() not in list_name:
         return True
 
 
 def check_ar_busy(ar_status: bool, busy_status=False, *args, **kwargs):
     if ar_status == busy_status:
         return True
```

## Comparing `gtki_module_orup_errors-1.35.4.dist-info/LICENSE` & `gtki_module_orup_errors-1.35.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gtki_module_orup_errors-1.35.4.dist-info/RECORD` & `gtki_module_orup_errors-1.35.5.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 orup_errors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 orup_errors/all_errors.py,sha256=BURM4U0f88_T80FpsQ8U1qq7ar9dKhbQnDX-ITJAV8k,14496
-orup_errors/check_funcs.py,sha256=bDJupObXqx4J5zMJwUUNBYTNrMBXswieQT9jRe7EfAg,5012
+orup_errors/check_funcs.py,sha256=fCKNC0BFEprdwOHSgJaXEKBdu1mLEVHe8ZuLuYhiKpg,5016
 orup_errors/general_functions.py,sha256=urdTLpnec8vJi7An2pBiu_qx34RYvJfMTRe9myNVtNU,2526
 orup_errors/main.py,sha256=0rAbiAqmCHK-T_hmEedmofODsCQPEaxR57b2AYb9wWI,2340
 orup_errors/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 orup_errors/tests/all_errors_test.py,sha256=Lxq5C6Ka5XaHPOVMCQdMSuZT3l07TaJuoGP5l4ZJU_0,1545
 orup_errors/tests/args_test.py,sha256=rz64Iv4D8nPuDlATAHuO_4wFRS20b71gYsIyotaw1pI,744
 orup_errors/tests/check_funcs_test.py,sha256=m5e0kAHg5AcEi2VfRLBEslCAKfFDs8ARWb8emZ_j1Pk,288
 orup_errors/tests/draw_win_test.py,sha256=dsrfPhbnArm08IukF_zypmUFYOw1wjHD_5qYHYjk-88,1385
 orup_errors/tests/general_functions_test.py,sha256=CHoOqcw6k2qLUfgHnGA4TTgACt25jIZNDkF0UnKRtlQ,1300
 orup_errors/tests/orup_errors_operator_test.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gtki_module_orup_errors-1.35.4.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-gtki_module_orup_errors-1.35.4.dist-info/METADATA,sha256=ESPkfDyQx9DqkSWF23bLEopiWy5TXC4aFUwFgWgqlII,156
-gtki_module_orup_errors-1.35.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gtki_module_orup_errors-1.35.4.dist-info/top_level.txt,sha256=WzasBtx2xqnJAQK3vavyWJNr2nwUAPObo6jw7F1FFko,12
-gtki_module_orup_errors-1.35.4.dist-info/RECORD,,
+gtki_module_orup_errors-1.35.5.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+gtki_module_orup_errors-1.35.5.dist-info/METADATA,sha256=iXkrkawp0KtAZkSpvE0UuIDo8RBLm5BfV2fukPqbBSg,156
+gtki_module_orup_errors-1.35.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gtki_module_orup_errors-1.35.5.dist-info/top_level.txt,sha256=WzasBtx2xqnJAQK3vavyWJNr2nwUAPObo6jw7F1FFko,12
+gtki_module_orup_errors-1.35.5.dist-info/RECORD,,
```


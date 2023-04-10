# Comparing `tmp/gtki_module_orup_errors-1.35.2-py3-none-any.whl.zip` & `tmp/gtki_module_orup_errors-1.35.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 12339 bytes, number of entries: 17
+Zip file size: 12355 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Oct-20 07:03 orup_errors/__init__.py
 -rw-rw-rw-  2.0 fat    14496 b- defN 23-Apr-03 08:32 orup_errors/all_errors.py
--rw-rw-rw-  2.0 fat     4738 b- defN 23-Apr-03 08:32 orup_errors/check_funcs.py
+-rw-rw-rw-  2.0 fat     4900 b- defN 23-Apr-10 11:00 orup_errors/check_funcs.py
 -rw-rw-rw-  2.0 fat     2526 b- defN 23-Mar-28 11:24 orup_errors/general_functions.py
 -rw-rw-rw-  2.0 fat     2340 b- defN 23-Mar-28 11:17 orup_errors/main.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Oct-20 07:03 orup_errors/tests/__init__.py
 -rw-rw-rw-  2.0 fat     1545 b- defN 21-Oct-20 07:03 orup_errors/tests/all_errors_test.py
 -rw-rw-rw-  2.0 fat      744 b- defN 21-Oct-20 07:03 orup_errors/tests/args_test.py
 -rw-rw-rw-  2.0 fat      288 b- defN 21-Dec-03 04:31 orup_errors/tests/check_funcs_test.py
 -rw-rw-rw-  2.0 fat     1385 b- defN 21-Oct-20 07:03 orup_errors/tests/draw_win_test.py
 -rw-rw-rw-  2.0 fat     1300 b- defN 21-Dec-03 04:20 orup_errors/tests/general_functions_test.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Oct-20 07:03 orup_errors/tests/orup_errors_operator_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-03 08:33 gtki_module_orup_errors-1.35.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      156 b- defN 23-Apr-03 08:33 gtki_module_orup_errors-1.35.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-03 08:33 gtki_module_orup_errors-1.35.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-03 08:33 gtki_module_orup_errors-1.35.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1524 b- defN 23-Apr-03 08:33 gtki_module_orup_errors-1.35.2.dist-info/RECORD
-17 files, 32237 bytes uncompressed, 9777 bytes compressed:  69.7%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-10 11:00 gtki_module_orup_errors-1.35.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      156 b- defN 23-Apr-10 11:00 gtki_module_orup_errors-1.35.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 11:00 gtki_module_orup_errors-1.35.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-10 11:00 gtki_module_orup_errors-1.35.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1524 b- defN 23-Apr-10 11:00 gtki_module_orup_errors-1.35.3.dist-info/RECORD
+17 files, 32399 bytes uncompressed, 9793 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: orup_errors/tests/general_functions_test.py
 Comment: 
 
 Filename: orup_errors/tests/orup_errors_operator_test.py
 Comment: 
 
-Filename: gtki_module_orup_errors-1.35.2.dist-info/LICENSE
+Filename: gtki_module_orup_errors-1.35.3.dist-info/LICENSE
 Comment: 
 
-Filename: gtki_module_orup_errors-1.35.2.dist-info/METADATA
+Filename: gtki_module_orup_errors-1.35.3.dist-info/METADATA
 Comment: 
 
-Filename: gtki_module_orup_errors-1.35.2.dist-info/WHEEL
+Filename: gtki_module_orup_errors-1.35.3.dist-info/WHEEL
 Comment: 
 
-Filename: gtki_module_orup_errors-1.35.2.dist-info/top_level.txt
+Filename: gtki_module_orup_errors-1.35.3.dist-info/top_level.txt
 Comment: 
 
-Filename: gtki_module_orup_errors-1.35.2.dist-info/RECORD
+Filename: gtki_module_orup_errors-1.35.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## orup_errors/check_funcs.py

```diff
@@ -65,19 +65,21 @@
     return check_type_incorrectness(chosen_trash_cat, cats_list)
 
 
 def check_tt_incorrectness(type_name: str, types_list: list, *args, **kwargs):
     return check_type_incorrectness(type_name, types_list)
 
 
-def check_carrier_debtor(carrier_name: str, debtors_list: list, comment, *args,
+def check_carrier_debtor(carrier_name: str, client_name: str, debtors_list: list, comment, *args,
                          **kwargs):
     for debtor_l in debtors_list:
-        if len(comment) < 1 and check_type_correctness(carrier_name,
-                                                       debtor_l[0]):
+        if len(comment) < 1 and (check_type_correctness(carrier_name,
+                                                       debtor_l[0]) or
+                                 check_type_correctness(client_name,
+                                                       debtor_l[0])):
             return debtor_l[1]
 
 
 def check_type_correctness(given: any, list_name: list, *args, **kwargs):
     """ Проверить факт нахождение элемента given в list_name """
     if given in list_name:
         return True
```

## Comparing `gtki_module_orup_errors-1.35.2.dist-info/LICENSE` & `gtki_module_orup_errors-1.35.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gtki_module_orup_errors-1.35.2.dist-info/RECORD` & `gtki_module_orup_errors-1.35.3.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 orup_errors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 orup_errors/all_errors.py,sha256=BURM4U0f88_T80FpsQ8U1qq7ar9dKhbQnDX-ITJAV8k,14496
-orup_errors/check_funcs.py,sha256=t6_8vTRw-tVgoPNCzCef2gVHGpRvC2JRxCK_Q1STWZ0,4738
+orup_errors/check_funcs.py,sha256=ZGRKu6A3wVRxJrNpA8ecM9A8X6oeHMI_MzifclVK0Ic,4900
 orup_errors/general_functions.py,sha256=urdTLpnec8vJi7An2pBiu_qx34RYvJfMTRe9myNVtNU,2526
 orup_errors/main.py,sha256=0rAbiAqmCHK-T_hmEedmofODsCQPEaxR57b2AYb9wWI,2340
 orup_errors/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 orup_errors/tests/all_errors_test.py,sha256=Lxq5C6Ka5XaHPOVMCQdMSuZT3l07TaJuoGP5l4ZJU_0,1545
 orup_errors/tests/args_test.py,sha256=rz64Iv4D8nPuDlATAHuO_4wFRS20b71gYsIyotaw1pI,744
 orup_errors/tests/check_funcs_test.py,sha256=m5e0kAHg5AcEi2VfRLBEslCAKfFDs8ARWb8emZ_j1Pk,288
 orup_errors/tests/draw_win_test.py,sha256=dsrfPhbnArm08IukF_zypmUFYOw1wjHD_5qYHYjk-88,1385
 orup_errors/tests/general_functions_test.py,sha256=CHoOqcw6k2qLUfgHnGA4TTgACt25jIZNDkF0UnKRtlQ,1300
 orup_errors/tests/orup_errors_operator_test.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gtki_module_orup_errors-1.35.2.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-gtki_module_orup_errors-1.35.2.dist-info/METADATA,sha256=7WRrGg5TPIw2vP3TQEEzU9xUt3Q6hwcNQ43jLRW5Cns,156
-gtki_module_orup_errors-1.35.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gtki_module_orup_errors-1.35.2.dist-info/top_level.txt,sha256=WzasBtx2xqnJAQK3vavyWJNr2nwUAPObo6jw7F1FFko,12
-gtki_module_orup_errors-1.35.2.dist-info/RECORD,,
+gtki_module_orup_errors-1.35.3.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+gtki_module_orup_errors-1.35.3.dist-info/METADATA,sha256=ZriAE-aw4MkCEzCDfZvjO75U1tWntdJP1GQXs0OYSaE,156
+gtki_module_orup_errors-1.35.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gtki_module_orup_errors-1.35.3.dist-info/top_level.txt,sha256=WzasBtx2xqnJAQK3vavyWJNr2nwUAPObo6jw7F1FFko,12
+gtki_module_orup_errors-1.35.3.dist-info/RECORD,,
```


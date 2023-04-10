# Comparing `tmp/pydatalysis-0.1.821.tar.gz` & `tmp/pydatalysis-0.1.9.tar.gz`

## Comparing `pydatalysis-0.1.821.tar` & `pydatalysis-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pydatalysis-0.1.821/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pydatalysis-0.1.821/pydatalysis/.DS_Store
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pydatalysis-0.1.821/pydatalysis/__init__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pydatalysis-0.1.821/pydatalysis/add.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pydatalysis-0.1.821/pydatalysis/linear_regression.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pydatalysis-0.1.821/pydatalysis/logistic_regression.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pydatalysis-0.1.821/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pydatalysis-0.1.821/LICENSE
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 pydatalysis-0.1.821/README.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 pydatalysis-0.1.821/pyproject.toml
--rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 pydatalysis-0.1.821/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pydatalysis-0.1.9/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pydatalysis-0.1.9/pydatalysis/.DS_Store
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 pydatalysis-0.1.9/pydatalysis/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pydatalysis-0.1.9/pydatalysis/add.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 pydatalysis-0.1.9/pydatalysis/bi_logistic_regression.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pydatalysis-0.1.9/pydatalysis/datasets.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pydatalysis-0.1.9/pydatalysis/linear_regression.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pydatalysis-0.1.9/pydatalysis/logistic_regression.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pydatalysis-0.1.9/pydatalysis/multi_logistic_regression.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pydatalysis-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pydatalysis-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 pydatalysis-0.1.9/README.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pydatalysis-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 pydatalysis-0.1.9/PKG-INFO
```

### Comparing `pydatalysis-0.1.821/.DS_Store` & `pydatalysis-0.1.9/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 00000430: 0405 0607 0809 0909 090d 095d 5368 6f77  ...........]Show
 00000440: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
 00000450: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
 00000460: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
 00000470: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
 00000480: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
 00000490: 735b 5368 6f77 5369 6465 6261 7208 0909  s[ShowSidebar...
-000004a0: 0909 5f10 187b 7b31 3832 2c20 3132 327d  .._..{{182, 122}
+000004a0: 0909 5f10 187b 7b32 3037 2c20 3130 377d  .._..{{207, 107}
 000004b0: 2c20 7b37 3730 2c20 3530 357d 7d09 0817  , {770, 505}}...
 000004c0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
 000004d0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
 000004e0: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
 000004f0: 0400 6400 6900 7300 7464 7363 6c62 6f6f  ..d.i.s.tdsclboo
 00000500: 6c00 0000 0004 0064 0069 0073 0074 7653  l......d.i.s.tvS
 00000510: 726e 6c6f 6e67 0000 0001 0000 000b 0070  rnlong.........p
```

### Comparing `pydatalysis-0.1.821/pydatalysis/.DS_Store` & `pydatalysis-0.1.9/pydatalysis/.DS_Store`

 * *Files identical despite different names*

### Comparing `pydatalysis-0.1.821/pydatalysis/linear_regression.py` & `pydatalysis-0.1.9/pydatalysis/linear_regression.py`

 * *Files identical despite different names*

### Comparing `pydatalysis-0.1.821/pydatalysis/logistic_regression.py` & `pydatalysis-0.1.9/pydatalysis/bi_logistic_regression.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import numpy as np
 import statsmodels.api as sm
 import pandas as pd
 from sklearn.metrics import confusion_matrix
 
 
-def logistic_regression(data, x, y):
+def bi_logistic_regression(data, x, y, y_dummy=False):
 
     data.dropna(inplace=True)
     x = data[x]
     x = sm.add_constant(x)
 
-    y = data[y]
+    if y_dummy == False:
+        y = pd.get_dummies(data[y], drop_first=True,  prefix=y)
+        # pd.concat
+        pd.concat([data, y], axis=1)
+    else:
+        y = data[y]
 
     # Fit logistic regression model
     model = sm.Logit(y, x).fit()
 
     summary_table = pd.read_html(
         model.summary().tables[0].as_html(), header=None, index_col=None)[0]
     summary_table.columns = ['Description', 'Value', 'Description', 'Value']
```

### Comparing `pydatalysis-0.1.821/LICENSE` & `pydatalysis-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydatalysis-0.1.821/README.md` & `pydatalysis-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pydatalysis-0.1.821/pyproject.toml` & `pydatalysis-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pydatalysis"
-version = "0.1.821"
+version = "0.1.9"
 license = {file = "LICENSE"}
 authors = [
   { name="Hashim Puthiyakath", email="hashputhiyakath@gmail.com" },
 ]
 description = "A Python package for performing various statistical analyses"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pydatalysis-0.1.821/PKG-INFO` & `pydatalysis-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatalysis
-Version: 0.1.821
+Version: 0.1.9
 Summary: A Python package for performing various statistical analyses
 Project-URL: Homepage, https://github.com/hashimputhiyakath/pydatalysis
 Project-URL: Bug Tracker, https://github.com/hashimputhiyakath/pydatalysis/issues
 Author-email: Hashim Puthiyakath <hashputhiyakath@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hashim Puthiyakath
```


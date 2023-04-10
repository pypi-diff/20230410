# Comparing `tmp/lifeactuary-1.2.tar.gz` & `tmp/lifeactuary-1.2.1.tar.gz`

## Comparing `lifeactuary-1.2.tar` & `lifeactuary-1.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lifeactuary-1.2/about.md
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 lifeactuary-1.2/pyproject_ver_0.1.8.toml.txt
--rw-r--r--   0        0        0   610030 2020-02-02 00:00:00.000000 lifeactuary-1.2/info/lifeActuary_v1_2.pdf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lifeactuary-1.2/lifeActuary/__init__.py
--rw-r--r--   0        0        0     8022 2020-02-02 00:00:00.000000 lifeactuary-1.2/lifeActuary/annuities.py
--rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 lifeactuary-1.2/lifeActuary/annuities_certain.py
--rw-r--r--   0        0        0    31515 2020-02-02 00:00:00.000000 lifeactuary-1.2/lifeActuary/commutation_table.py
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 lifeactuary-1.2/lifeActuary/commutation_table_frac.py
--rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 lifeactuary-1.2/lifeActuary/mortality_table.py
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/197982PortugalFemale.xml
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/197982PortugalMale.xml
--rw-r--r--   0        0        0    14645 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/AF80.xml
--rw-r--r--   0        0        0    14009 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/AM80.xml
--rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/CSO_1941.xml
--rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/GRF95.xml
--rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/GRM80.xml
--rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/GRM95.xml
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/IA8590F.xml
--rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/IA8590M.xml
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/PFL80.xml
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/PML80.xml
--rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/SIF91.xml
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/SIM91.xml
--rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/TV7377.xml
--rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/TV8890.xml
--rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/WL80.xml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/__init__.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/read_soa_table_xml.py
--rw-r--r--   0        0        0    18772 2020-02-02 00:00:00.000000 lifeactuary-1.2/soa_tables/tables_manual.xlsx
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 lifeactuary-1.2/LICENSE
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 lifeactuary-1.2/README.md
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 lifeactuary-1.2/pyproject.toml
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 lifeactuary-1.2/PKG-INFO
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/about.md
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/pyproject_ver_0.1.8.toml.txt
+-rw-r--r--   0        0        0   610030 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/info/lifeActuary_v1_2.pdf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/lifeActuary/__init__.py
+-rw-r--r--   0        0        0     8022 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/lifeActuary/annuities.py
+-rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/lifeActuary/annuities_certain.py
+-rw-r--r--   0        0        0    31515 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/lifeActuary/commutation_table.py
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/lifeActuary/commutation_table_frac.py
+-rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/lifeActuary/mortality_table.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/lifeActuary/read_soa_table_xml.py
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/197982PortugalFemale.xml
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/197982PortugalMale.xml
+-rw-r--r--   0        0        0    14645 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/AF80.xml
+-rw-r--r--   0        0        0    14009 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/AM80.xml
+-rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/CSO_1941.xml
+-rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/GRF95.xml
+-rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/GRM80.xml
+-rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/GRM95.xml
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/IA8590F.xml
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/IA8590M.xml
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/PFL80.xml
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/PML80.xml
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/SIF91.xml
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/SIM91.xml
+-rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/TV7377.xml
+-rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/TV8890.xml
+-rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/WL80.xml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/__init__.py
+-rw-r--r--   0        0        0    18772 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/tables_manual.xlsx
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/README.md
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/PKG-INFO
```

### Comparing `lifeactuary-1.2/pyproject_ver_0.1.8.toml.txt` & `lifeactuary-1.2.1/pyproject_ver_0.1.8.toml.txt`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/info/lifeActuary_v1_2.pdf` & `lifeactuary-1.2.1/info/lifeActuary_v1_2.pdf`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/lifeActuary/annuities.py` & `lifeactuary-1.2.1/lifeActuary/annuities.py`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/lifeActuary/annuities_certain.py` & `lifeactuary-1.2.1/lifeActuary/annuities_certain.py`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/lifeActuary/commutation_table.py` & `lifeactuary-1.2.1/lifeActuary/commutation_table.py`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/lifeActuary/commutation_table_frac.py` & `lifeactuary-1.2.1/lifeActuary/commutation_table_frac.py`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/lifeActuary/mortality_table.py` & `lifeactuary-1.2.1/lifeActuary/mortality_table.py`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/soa_tables/197982PortugalFemale.xml` & `lifeactuary-1.2.1/soa_tables/197982PortugalFemale.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/soa_tables/197982PortugalMale.xml` & `lifeactuary-1.2.1/soa_tables/197982PortugalMale.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/soa_tables/AF80.xml` & `lifeactuary-1.2.1/soa_tables/AF80.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/soa_tables/AM80.xml` & `lifeactuary-1.2.1/soa_tables/AM80.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/soa_tables/CSO_1941.xml` & `lifeactuary-1.2.1/soa_tables/CSO_1941.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/soa_tables/GRF95.xml` & `lifeactuary-1.2.1/soa_tables/GRF95.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/soa_tables/GRM80.xml` & `lifeactuary-1.2.1/soa_tables/GRM80.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/soa_tables/GRM95.xml` & `lifeactuary-1.2.1/soa_tables/GRM95.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/soa_tables/IA8590F.xml` & `lifeactuary-1.2.1/soa_tables/IA8590F.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/soa_tables/IA8590M.xml` & `lifeactuary-1.2.1/soa_tables/IA8590M.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/soa_tables/PFL80.xml` & `lifeactuary-1.2.1/soa_tables/PFL80.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/soa_tables/PML80.xml` & `lifeactuary-1.2.1/soa_tables/PML80.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/soa_tables/SIF91.xml` & `lifeactuary-1.2.1/soa_tables/SIF91.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/soa_tables/SIM91.xml` & `lifeactuary-1.2.1/soa_tables/SIM91.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/soa_tables/TV7377.xml` & `lifeactuary-1.2.1/soa_tables/TV7377.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/soa_tables/TV8890.xml` & `lifeactuary-1.2.1/soa_tables/TV8890.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/soa_tables/WL80.xml` & `lifeactuary-1.2.1/soa_tables/WL80.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/soa_tables/read_soa_table_xml.py` & `lifeactuary-1.2.1/lifeActuary/read_soa_table_xml.py`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/soa_tables/tables_manual.xlsx` & `lifeactuary-1.2.1/soa_tables/tables_manual.xlsx`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/LICENSE` & `lifeactuary-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2/README.md` & `lifeactuary-1.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-# lifeactuary_1.2
+# lifeactuary_1.2.1
 Package *lifeactuary* is a Python library to perform actuarial mathematics on life contingencies and classical financial mathematics computations. Versatile, simple and easy to use. The main functions are implemented using the usual actuarial approach, making it a natural choice for the life actuary.
 This document is produced as a descriptive tool on how to use the package and as a user guide for the developed actuarial functions. For each actuarial function, an illustrative example is provided. 
         
 The package uses Python version >= 3.6.
 
 This package and functions herein are provided as is, without any guarantee regarding the accuracy of calculations. It's distributed using the [MIT License](https://en.wikipedia.org/wiki/MIT_License) and the authors disclaim any liability arising by any losses due to direct or indirect use of this package.
     
 This package is still under development and further useful and interesting functions will be available any time soon.
 
 You should also visit for version 1.0, [lifeactuary at github](https://github.com/parcr/lifeactuary) to download the folder *"soa_tables"* containing a set of tables, namely the ones used in the examples in the manual.
 
 For version 1.2, take a look for  [lifeactuary_1.2 at github](https://github.com/parcr/lifeactuary_1.2) to download the folder *"soa_tables"* containing a set of tables, namely the ones used in the examples in the manual.
+
+Version 1.2.1 includes the file **"read_soa_table_xml.py"**, so that you just need to a look at  [lifeactuary_1.2 at github](https://github.com/parcr/lifeactuary_1.2) to download the folder *"soa_tables"* containing a set of tables, namely the ones used in the examples in the manual.
```

### Comparing `lifeactuary-1.2/pyproject.toml` & `lifeactuary-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lifeactuary"
-version = "1.2"
+version = "1.2.1"
 authors = [
   { name="Pedro Corte Real", email="parcr@fct.unl.pt" },
 { name="Gracinda R. Guerreiro", email="grg@fct.unl.pt" },
 ]
 
 maintainers=[
   { name="Pedro Corte Real", email="parcr@fct.unl.pt" },
```

### Comparing `lifeactuary-1.2/PKG-INFO` & `lifeactuary-1.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeactuary
-Version: 1.2
+Version: 1.2.1
 Summary: A set of actuarial tools for the life actuary
 Project-URL: Homepage, https://github.com/parcr/lifeactuary_1.2
 Project-URL: Bug Tracker, https://github.com/parcr/lifeactuary_1.2/issues
 Author-email: Pedro Corte Real <parcr@fct.unl.pt>, "Gracinda R. Guerreiro" <grg@fct.unl.pt>
 Maintainer-email: Pedro Corte Real <parcr@fct.unl.pt>, "Gracinda R. Guerreiro" <grg@fct.unl.pt>
 License: Copyright (c) 2022 Pedro Corte Real, Gracinda R. Guerreiro
         
@@ -28,20 +28,22 @@
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# lifeactuary_1.2
+# lifeactuary_1.2.1
 Package *lifeactuary* is a Python library to perform actuarial mathematics on life contingencies and classical financial mathematics computations. Versatile, simple and easy to use. The main functions are implemented using the usual actuarial approach, making it a natural choice for the life actuary.
 This document is produced as a descriptive tool on how to use the package and as a user guide for the developed actuarial functions. For each actuarial function, an illustrative example is provided. 
         
 The package uses Python version >= 3.6.
 
 This package and functions herein are provided as is, without any guarantee regarding the accuracy of calculations. It's distributed using the [MIT License](https://en.wikipedia.org/wiki/MIT_License) and the authors disclaim any liability arising by any losses due to direct or indirect use of this package.
     
 This package is still under development and further useful and interesting functions will be available any time soon.
 
 You should also visit for version 1.0, [lifeactuary at github](https://github.com/parcr/lifeactuary) to download the folder *"soa_tables"* containing a set of tables, namely the ones used in the examples in the manual.
 
 For version 1.2, take a look for  [lifeactuary_1.2 at github](https://github.com/parcr/lifeactuary_1.2) to download the folder *"soa_tables"* containing a set of tables, namely the ones used in the examples in the manual.
+
+Version 1.2.1 includes the file **"read_soa_table_xml.py"**, so that you just need to a look at  [lifeactuary_1.2 at github](https://github.com/parcr/lifeactuary_1.2) to download the folder *"soa_tables"* containing a set of tables, namely the ones used in the examples in the manual.
```


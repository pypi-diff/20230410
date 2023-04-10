# Comparing `tmp/jms-metabolite-services-0.5.4.tar.gz` & `tmp/jms-metabolite-services-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shuzhao/li.github/JMS/dist/.tmp-z4wejmnf/jms-metabolite-services-0.5.4.tar", last modified: Sun Apr  9 12:04:54 2023, max compression
+gzip compressed data, was "/Users/shuzhao/li.github/JMS/dist/.tmp-c5lprqv5/jms-metabolite-services-0.5.5.tar", last modified: Mon Apr 10 19:33:29 2023, max compression
```

## Comparing `jms-metabolite-services-0.5.4.tar` & `jms-metabolite-services-0.5.5.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/
--rw-r--r--   0 shuzhao    (501) staff       (20)     1073 2020-05-11 14:03:57.000000 jms-metabolite-services-0.5.4/LICENSE
--rw-r--r--   0 shuzhao    (501) staff       (20)     5597 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/PKG-INFO
--rw-r--r--   0 shuzhao    (501) staff       (20)     4720 2023-01-09 23:02:36.000000 jms-metabolite-services-0.5.4/README.md
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/jms/
--rw-r--r--   0 shuzhao    (501) staff       (20)       22 2023-04-09 12:03:10.000000 jms-metabolite-services-0.5.4/jms/__init__.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     2355 2023-04-03 14:08:48.000000 jms-metabolite-services-0.5.4/jms/coverage.py
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/jms/data/
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 02:27:53.000000 jms-metabolite-services-0.5.4/jms/data/__init__.py
--rw-r--r--   0 shuzhao    (501) staff       (20)  3085036 2022-02-23 20:21:57.000000 jms-metabolite-services-0.5.4/jms/data/list_formula_mass.py
--rw-r--r--   0 shuzhao    (501) staff       (20)       84 2022-02-10 00:56:47.000000 jms-metabolite-services-0.5.4/jms/data/masters.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    37884 2023-04-09 02:06:42.000000 jms-metabolite-services-0.5.4/jms/dbStructures.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     4548 2023-04-06 15:29:23.000000 jms-metabolite-services-0.5.4/jms/empiricalCpds.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     2265 2023-04-03 14:08:48.000000 jms-metabolite-services-0.5.4/jms/formula.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     4605 2023-04-06 21:06:32.000000 jms-metabolite-services-0.5.4/jms/io.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     1801 2023-03-08 18:14:43.000000 jms-metabolite-services-0.5.4/jms/ions.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    14262 2023-04-09 12:03:10.000000 jms-metabolite-services-0.5.4/jms/modelConvert.py
--rw-r--r--   0 shuzhao    (501) staff       (20)      461 2023-04-06 15:29:23.000000 jms-metabolite-services-0.5.4/jms/model_port.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    11998 2023-03-08 17:59:27.000000 jms-metabolite-services-0.5.4/jms/search.py
--rw-r--r--   0 shuzhao    (501) staff       (20)      649 2023-01-01 22:01:32.000000 jms-metabolite-services-0.5.4/jms/test.py
--rw-r--r--   0 shuzhao    (501) staff       (20)       58 2022-02-10 00:39:06.000000 jms-metabolite-services-0.5.4/jms/updates.py
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/jms/utils/
--rw-r--r--   0 shuzhao    (501) staff       (20)     5832 2022-05-19 20:33:17.000000 jms-metabolite-services-0.5.4/jms/utils/Tabular2Json.py
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 02:28:13.000000 jms-metabolite-services-0.5.4/jms/utils/__init__.py
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:16.000000 jms-metabolite-services-0.5.4/jms/utils/chemebi.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    10125 2023-04-06 15:29:23.000000 jms-metabolite-services-0.5.4/jms/utils/gems.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    11707 2022-02-10 02:05:11.000000 jms-metabolite-services-0.5.4/jms/utils/hmdb.py
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:21.000000 jms-metabolite-services-0.5.4/jms/utils/pubchem.py
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:26.000000 jms-metabolite-services-0.5.4/jms/utils/refmet.py
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/jms_metabolite_services.egg-info/
--rw-r--r--   0 shuzhao    (501) staff       (20)     5597 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/jms_metabolite_services.egg-info/PKG-INFO
--rw-r--r--   0 shuzhao    (501) staff       (20)      666 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/jms_metabolite_services.egg-info/SOURCES.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)        1 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/jms_metabolite_services.egg-info/dependency_links.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)       10 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/jms_metabolite_services.egg-info/requires.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)        4 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/jms_metabolite_services.egg-info/top_level.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)       38 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/setup.cfg
--rw-r--r--   0 shuzhao    (501) staff       (20)     1300 2022-05-19 20:56:08.000000 jms-metabolite-services-0.5.4/setup.py
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-10 19:33:29.000000 jms-metabolite-services-0.5.5/
+-rw-r--r--   0 shuzhao    (501) staff       (20)     1073 2020-05-11 14:03:57.000000 jms-metabolite-services-0.5.5/LICENSE
+-rw-r--r--   0 shuzhao    (501) staff       (20)     5597 2023-04-10 19:33:29.000000 jms-metabolite-services-0.5.5/PKG-INFO
+-rw-r--r--   0 shuzhao    (501) staff       (20)     4720 2023-01-09 23:02:36.000000 jms-metabolite-services-0.5.5/README.md
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-10 19:33:29.000000 jms-metabolite-services-0.5.5/jms/
+-rw-r--r--   0 shuzhao    (501) staff       (20)       22 2023-04-10 19:30:36.000000 jms-metabolite-services-0.5.5/jms/__init__.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     4893 2023-04-10 19:30:36.000000 jms-metabolite-services-0.5.5/jms/coverage.py
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-10 19:33:29.000000 jms-metabolite-services-0.5.5/jms/data/
+-rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 02:27:53.000000 jms-metabolite-services-0.5.5/jms/data/__init__.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)   988184 2023-04-10 16:10:17.000000 jms-metabolite-services-0.5.5/jms/data/humangem_pathways.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)  3085036 2022-02-23 20:21:57.000000 jms-metabolite-services-0.5.5/jms/data/list_formula_mass.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)       84 2022-02-10 00:56:47.000000 jms-metabolite-services-0.5.5/jms/data/masters.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    37884 2023-04-09 02:06:42.000000 jms-metabolite-services-0.5.5/jms/dbStructures.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     4898 2023-04-10 13:43:20.000000 jms-metabolite-services-0.5.5/jms/empiricalCpds.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     2229 2023-04-10 18:43:40.000000 jms-metabolite-services-0.5.5/jms/formula.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     4605 2023-04-06 21:06:32.000000 jms-metabolite-services-0.5.5/jms/io.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     1801 2023-03-08 18:14:43.000000 jms-metabolite-services-0.5.5/jms/ions.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    14660 2023-04-10 19:30:36.000000 jms-metabolite-services-0.5.5/jms/modelConvert.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)      461 2023-04-06 15:29:23.000000 jms-metabolite-services-0.5.5/jms/model_port.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    11998 2023-03-08 17:59:27.000000 jms-metabolite-services-0.5.5/jms/search.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)      649 2023-01-01 22:01:32.000000 jms-metabolite-services-0.5.5/jms/test.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)       58 2022-02-10 00:39:06.000000 jms-metabolite-services-0.5.5/jms/updates.py
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-10 19:33:29.000000 jms-metabolite-services-0.5.5/jms/utils/
+-rw-r--r--   0 shuzhao    (501) staff       (20)     5832 2022-05-19 20:33:17.000000 jms-metabolite-services-0.5.5/jms/utils/Tabular2Json.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 02:28:13.000000 jms-metabolite-services-0.5.5/jms/utils/__init__.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:16.000000 jms-metabolite-services-0.5.5/jms/utils/chemebi.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    10125 2023-04-06 15:29:23.000000 jms-metabolite-services-0.5.5/jms/utils/gems.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    11707 2022-02-10 02:05:11.000000 jms-metabolite-services-0.5.5/jms/utils/hmdb.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:21.000000 jms-metabolite-services-0.5.5/jms/utils/pubchem.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:26.000000 jms-metabolite-services-0.5.5/jms/utils/refmet.py
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-10 19:33:29.000000 jms-metabolite-services-0.5.5/jms_metabolite_services.egg-info/
+-rw-r--r--   0 shuzhao    (501) staff       (20)     5597 2023-04-10 19:33:29.000000 jms-metabolite-services-0.5.5/jms_metabolite_services.egg-info/PKG-INFO
+-rw-r--r--   0 shuzhao    (501) staff       (20)      696 2023-04-10 19:33:29.000000 jms-metabolite-services-0.5.5/jms_metabolite_services.egg-info/SOURCES.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)        1 2023-04-10 19:33:29.000000 jms-metabolite-services-0.5.5/jms_metabolite_services.egg-info/dependency_links.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)       10 2023-04-10 19:33:29.000000 jms-metabolite-services-0.5.5/jms_metabolite_services.egg-info/requires.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)        4 2023-04-10 19:33:29.000000 jms-metabolite-services-0.5.5/jms_metabolite_services.egg-info/top_level.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)       38 2023-04-10 19:33:29.000000 jms-metabolite-services-0.5.5/setup.cfg
+-rw-r--r--   0 shuzhao    (501) staff       (20)     1300 2022-05-19 20:56:08.000000 jms-metabolite-services-0.5.5/setup.py
```

### Comparing `jms-metabolite-services-0.5.4/LICENSE` & `jms-metabolite-services-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.4/PKG-INFO` & `jms-metabolite-services-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jms-metabolite-services
-Version: 0.5.4
+Version: 0.5.5
 Summary: conversion, search of metabolic models and metabolomics data
 Home-page: https://github.com/shuzhao-li/JMS
 Author: Shuzhao Li, Minghao Gong
 Author-email: shuzhao.li@gmail.com
 License: Python
 Keywords: metabolomics,chemistry,bioinformatics,mass spectrometry
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jms-metabolite-services-0.5.4/README.md` & `jms-metabolite-services-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.4/jms/data/list_formula_mass.py` & `jms-metabolite-services-0.5.5/jms/data/list_formula_mass.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.4/jms/dbStructures.py` & `jms-metabolite-services-0.5.5/jms/dbStructures.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.4/jms/empiricalCpds.py` & `jms-metabolite-services-0.5.5/jms/empiricalCpds.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     '''Read JSON annotation dictionary from asari/khipu.
     Returns list of empCpds.
     '''
     epds = json.load(open(file))
     return list(epds.values())
 
 
-def filter_epds(list_epds, neutral_formula_mass=True, multiple_ions=True):
+def filter_epds(list_epds, neutral_formula_mass=True, multiple_ions=True, C13=True):
     '''Filter list of empCpds by neutral_formula_mass or by multiple_ions.
     list_epds : [{'interim_id': 'kp100_128.0951', 'neutral_formula_mass': 128.09508427175538, 'neutral_formula': None, 
         'Database_referred': [], 'identity': [], 'MS1_pseudo_Spectra': [
         {'apex': 653, 'peak_area': 8047955, 'height': 988673, 'left_base': 642, 'right_base': 659, 
         'goodness_fitting': 0.9397139863801345, 'cSelectivity': 0.3497536945812808, 
         'parent_masstrack_id': 880, 'mz': 130.10569763183594, 'snr': 11, 'id_number': 'F1444', 
         'rtime': 125.24219400000001, 'rtime_left_base': 123.24607800000001, 'rtime_right_base': 126.27832200000002, 
@@ -76,33 +76,41 @@
         ...]
     '''
     result = list_epds
     if neutral_formula_mass:
         result = [x for x in result if x['neutral_formula_mass']]
     if multiple_ions:
         result = [x for x in result if len(x['MS1_pseudo_Spectra'])>1]
+    if C13:
+        result = [x for x in result if check_13C_M1(x)]
     return result
 
+def check_13C_M1(empCpd):
+    '''Check presence of pair of M1 13C ion and the M0 12C ion.
+    '''
+    ions = [x['isotope'] for x in empCpd['MS1_pseudo_Spectra'] if 'isotope' in x]
+    if '13C/12C' in ions and 'M0' in ions:
+        return True
+    else:
+        return False
 
 def get_neutrals(list_epds):
     neutrals = []
     for v in list_epds:
         p = {}
         p['id'] = v['interim_id']
         p['mz'] = v['neutral_formula_mass']
         p['rtime'] = np.mean([x['rtime'] for x in v['MS1_pseudo_Spectra']])
         neutrals.append(p)
     return neutrals
 
-
 def get_match(cpds, mztree, ppm=5):
     '''Find matches of a list of cpds in mztree.
     cpds : [{'id': 'C00025', 'mw': 147.0532, 'name': 'L-Glutamate'}, ...]
     '''
     match = []
     for x in cpds:
         if 'mw' in x and x['mw']:
             _m = find_all_matches_centurion_indexed_list(x['mw'], mztree, ppm)
             if _m:
                 match.append( (x, _m) )
     return match
-
```

### Comparing `jms-metabolite-services-0.5.4/jms/formula.py` & `jms-metabolite-services-0.5.5/jms/formula.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 '''
 Based on mass2chem.formula 
 
 1. to find formula for anchor ions
 2. to search for any formula (to-do)
 '''
 
-from mass2chem.formula import compute_adducts_formulae
-from .search import build_centurion_tree, find_best_match_centurion_indexed_list
+from mass2chem.formula import compute_adducts_formulae, \
+                                    parse_chemformula_dict, \
+                                        add_formula_dict, \
+                                            dict_to_hill_formula
 
-# The following imports are used in function of `adjust_charge_in_formula`
-from mass2chem.formula import parse_chemformula_dict
-from mass2chem.formula import add_formula_dict
-from mass2chem.formula import dict_to_hill_formula
+from .search import build_centurion_tree, find_best_match_centurion_indexed_list
 
 
 def get_formula_ions_tree(list_formula_mass, mode='pos'):
     peak_list = []
     for formula, mass in list_formula_mass:
         for ion in compute_adducts_formulae(mass, formula, mode, primary_only=True):
             peak_list.append( {'mz': ion[0], 
@@ -24,15 +23,14 @@
                                'neutral_formula_mass': mass} )
 
     return build_centurion_tree(peak_list)
 
 def search_mz_formula_tree(mz, formula_tree, limit_ppm=5):
     '''
     return the best matched ion (as peak format) in formula_tree.
-
     formula_tree = get_formula_ions_tree(list_formula_mass, mode='pos')
     '''
     return find_best_match_centurion_indexed_list(mz, formula_tree, limit_ppm)
 
 def adjust_charge_in_formula(charged_formula:str,charge:int)->str: 
     """adjust charged formula to neutral formula
 
@@ -63,8 +61,8 @@
         if hypothetical_neutral_formula_dict:
             result = dict_to_hill_formula(hypothetical_neutral_formula_dict)
         else: 
             if charge < 0:
                 result = None
             else:  # if charge >0, e.g., Fe, charge is 2+; it should still be Fe as formula
                 result = charged_formula # here dealing with Metal etc.
-    return result
+    return result
```

### Comparing `jms-metabolite-services-0.5.4/jms/io.py` & `jms-metabolite-services-0.5.5/jms/io.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.4/jms/ions.py` & `jms-metabolite-services-0.5.5/jms/ions.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.4/jms/modelConvert.py` & `jms-metabolite-services-0.5.5/jms/modelConvert.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,22 +177,25 @@
     Match the compounds in a genome scale metabolic model to a metabolomics experiment,
     via the format of empirical compounds. The empirical compounds are constructed via khipu.
     Their JSON format can accommodate added fields on the fly, and return results 
     as part of empCpd['identity'] (https://github.com/shuzhao-li/metDataModel).
     Because neutral mass is inferred from khipu, the match problem is simplified by 
     focusing on neutral mass (formula).
     '''
-    def __init__(self, MetabolicModel, userFeatureList, parameters=default_parameters):
+    def __init__(self, MetabolicModel, userFeatureList=None, userListEmpCpds=None, parameters=default_parameters):
         '''
+        Besides MetabolicModel, this takes either userFeatureList or userListEmpCpds.
         parameters : dictionary to pass ion mode, m/z and rt tolerance and isotope/adduct patterns.
         MetabolicModel : metabolic model in JSON style dictionary.
         userFeatureList : list of JSON style features
+        userListEmpCpds : list of empirical compounds, which can be constructed and processed elsewhere
         '''
         self.model = MetabolicModel
         self.userFeatureList = userFeatureList
+        self.userListEmpCpds = userListEmpCpds
         
         self.mode = parameters['mode']
         self.isotope_search_patterns = parameters['isotope_search_patterns']
         self.adduct_patterns = parameters['adduct_patterns']
         self.extended_adducts = parameters['extended_adducts']
         self.mz_tolerance_ppm = parameters['mz_tolerance_ppm']
         self.rt_tolerance = parameters['rt_tolerance']
@@ -249,15 +252,18 @@
         '''
         KCD = knownCompoundDatabase()
         KCD.mass_index_list_compounds(self.model['Compounds'].values())
         KCD.build_emp_cpds_index()
         EED = ExperimentalEcpdDatabase(mode=self.mode, 
                                        mz_tolerance_ppm=self.mz_tolerance_ppm, 
                                        rt_tolerance=self.rt_tolerance)
-        EED.build_from_list_peaks(self.userFeatureList)
+        if self.userFeatureList:
+            EED.build_from_list_peaks(self.userFeatureList)
+        elif self.userListEmpCpds:
+            EED.build_from_list_empCpds(self.userListEmpCpds)
         EED.extend_empCpd_annotation(KCD)
         EED.annotate_singleton_mummichog(KCD)
 
         return self.update_identity(EED.dict_empCpds, KCD)
 
 
     def update_identity(self, dict_empCpds, KCD):
```

### Comparing `jms-metabolite-services-0.5.4/jms/search.py` & `jms-metabolite-services-0.5.5/jms/search.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.4/jms/test.py` & `jms-metabolite-services-0.5.5/jms/test.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.4/jms/utils/Tabular2Json.py` & `jms-metabolite-services-0.5.5/jms/utils/Tabular2Json.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.4/jms/utils/gems.py` & `jms-metabolite-services-0.5.5/jms/utils/gems.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.4/jms/utils/hmdb.py` & `jms-metabolite-services-0.5.5/jms/utils/hmdb.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.4/jms_metabolite_services.egg-info/PKG-INFO` & `jms-metabolite-services-0.5.5/jms_metabolite_services.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jms-metabolite-services
-Version: 0.5.4
+Version: 0.5.5
 Summary: conversion, search of metabolic models and metabolomics data
 Home-page: https://github.com/shuzhao-li/JMS
 Author: Shuzhao Li, Minghao Gong
 Author-email: shuzhao.li@gmail.com
 License: Python
 Keywords: metabolomics,chemistry,bioinformatics,mass spectrometry
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jms-metabolite-services-0.5.4/jms_metabolite_services.egg-info/SOURCES.txt` & `jms-metabolite-services-0.5.5/jms_metabolite_services.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 jms/ions.py
 jms/modelConvert.py
 jms/model_port.py
 jms/search.py
 jms/test.py
 jms/updates.py
 jms/data/__init__.py
+jms/data/humangem_pathways.py
 jms/data/list_formula_mass.py
 jms/data/masters.py
 jms/utils/Tabular2Json.py
 jms/utils/__init__.py
 jms/utils/chemebi.py
 jms/utils/gems.py
 jms/utils/hmdb.py
```

### Comparing `jms-metabolite-services-0.5.4/setup.py` & `jms-metabolite-services-0.5.5/setup.py`

 * *Files identical despite different names*


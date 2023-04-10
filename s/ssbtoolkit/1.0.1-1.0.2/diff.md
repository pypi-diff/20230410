# Comparing `tmp/ssbtoolkit-1.0.1.tar.gz` & `tmp/ssbtoolkit-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssbtoolkit-1.0.1.tar", last modified: Mon Nov 21 15:53:54 2022, max compression
+gzip compressed data, was "ssbtoolkit-1.0.2.tar", last modified: Mon Apr 10 11:49:05 2023, max compression
```

## Comparing `ssbtoolkit-1.0.1.tar` & `ssbtoolkit-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,29 @@
-drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2022-11-21 15:53:54.414081 ssbtoolkit-1.0.1/
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    11347 2022-11-18 14:05:09.000000 ssbtoolkit-1.0.1/LICENSE
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)       66 2022-11-21 15:16:04.000000 ssbtoolkit-1.0.1/MANIFEST.in
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      741 2022-11-21 15:53:54.414081 ssbtoolkit-1.0.1/PKG-INFO
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     2914 2022-11-18 14:05:09.000000 ssbtoolkit-1.0.1/README.md
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)       38 2022-11-21 15:53:54.414081 ssbtoolkit-1.0.1/setup.cfg
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1261 2022-11-21 15:53:28.000000 ssbtoolkit-1.0.1/setup.py
-drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2022-11-21 15:53:54.414081 ssbtoolkit-1.0.1/ssbtoolkit/
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)   106496 2022-11-18 14:05:09.000000 ssbtoolkit-1.0.1/ssbtoolkit/HuTRdb.sqlite3
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    17110 2022-11-21 15:45:59.000000 ssbtoolkit-1.0.1/ssbtoolkit/Utils.py
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    71651 2022-11-21 15:45:36.000000 ssbtoolkit-1.0.1/ssbtoolkit/__init__.py
-drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2022-11-21 15:53:54.414081 ssbtoolkit-1.0.1/ssbtoolkit/pathways/
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    20607 2022-11-21 11:49:20.000000 ssbtoolkit-1.0.1/ssbtoolkit/pathways/Gi.py
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1736 2022-11-18 14:05:09.000000 ssbtoolkit-1.0.1/ssbtoolkit/pathways/Gi_parameters.csv
--rw-r--r--   0 rribeiro  (1000) rribeiro  (1000)     2640 2022-11-18 14:05:09.000000 ssbtoolkit-1.0.1/ssbtoolkit/pathways/Gi_reactions.csv
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    14154 2022-11-21 11:49:11.000000 ssbtoolkit-1.0.1/ssbtoolkit/pathways/Gq.py
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1153 2022-11-18 14:05:09.000000 ssbtoolkit-1.0.1/ssbtoolkit/pathways/Gq_parameters.csv
--rw-r--r--   0 rribeiro  (1000) rribeiro  (1000)     1121 2022-11-18 14:05:09.000000 ssbtoolkit-1.0.1/ssbtoolkit/pathways/Gq_reactions.csv
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    21135 2022-11-21 11:49:05.000000 ssbtoolkit-1.0.1/ssbtoolkit/pathways/Gs.py
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1763 2022-11-18 14:05:09.000000 ssbtoolkit-1.0.1/ssbtoolkit/pathways/Gs_parameters.csv
--rw-r--r--   0 rribeiro  (1000) rribeiro  (1000)     2709 2022-11-18 14:05:09.000000 ssbtoolkit-1.0.1/ssbtoolkit/pathways/Gs_reactions.csv
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    15771 2022-11-18 14:05:09.000000 ssbtoolkit-1.0.1/ssbtoolkit/pathways/OXTR_pathway.py
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1725 2022-11-18 14:05:09.000000 ssbtoolkit-1.0.1/ssbtoolkit/pathways/OXTR_pathway_parameters.csv
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1319 2022-11-18 14:05:09.000000 ssbtoolkit-1.0.1/ssbtoolkit/pathways/OXTR_pathway_reactions.csv
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    13822 2022-11-18 14:05:09.000000 ssbtoolkit-1.0.1/ssbtoolkit/pathways/OXTR_pathway_testing.py
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)        0 2022-11-18 14:05:09.000000 ssbtoolkit-1.0.1/ssbtoolkit/pathways/__init__.py
-drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2022-11-21 15:53:54.414081 ssbtoolkit-1.0.1/ssbtoolkit.egg-info/
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      741 2022-11-21 15:53:54.000000 ssbtoolkit-1.0.1/ssbtoolkit.egg-info/PKG-INFO
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      786 2022-11-21 15:53:54.000000 ssbtoolkit-1.0.1/ssbtoolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)        1 2022-11-21 15:53:54.000000 ssbtoolkit-1.0.1/ssbtoolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      143 2022-11-21 15:53:54.000000 ssbtoolkit-1.0.1/ssbtoolkit.egg-info/requires.txt
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)       11 2022-11-21 15:53:54.000000 ssbtoolkit-1.0.1/ssbtoolkit.egg-info/top_level.txt
+drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 11:49:05.028493 ssbtoolkit-1.0.2/
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)       66 2023-04-10 11:48:28.000000 ssbtoolkit-1.0.2/MANIFEST.in
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      719 2023-04-10 11:49:05.028493 ssbtoolkit-1.0.2/PKG-INFO
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)       38 2023-04-10 11:49:05.028493 ssbtoolkit-1.0.2/setup.cfg
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1261 2023-04-10 11:25:21.000000 ssbtoolkit-1.0.2/setup.py
+drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 11:49:05.024493 ssbtoolkit-1.0.2/ssbtoolkit/
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    17110 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.2/ssbtoolkit/Utils.py
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    71651 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.2/ssbtoolkit/__init__.py
+drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 11:49:05.028493 ssbtoolkit-1.0.2/ssbtoolkit/pathways/
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    20647 2023-04-10 11:28:21.000000 ssbtoolkit-1.0.2/ssbtoolkit/pathways/Gi.py
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1736 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.2/ssbtoolkit/pathways/Gi_parameters.csv
+-rw-r--r--   0 rribeiro  (1000) rribeiro  (1000)     2640 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.2/ssbtoolkit/pathways/Gi_reactions.csv
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    14154 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.2/ssbtoolkit/pathways/Gq.py
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1153 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.2/ssbtoolkit/pathways/Gq_parameters.csv
+-rw-r--r--   0 rribeiro  (1000) rribeiro  (1000)     1121 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.2/ssbtoolkit/pathways/Gq_reactions.csv
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    21135 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.2/ssbtoolkit/pathways/Gs.py
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1763 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.2/ssbtoolkit/pathways/Gs_parameters.csv
+-rw-r--r--   0 rribeiro  (1000) rribeiro  (1000)     2709 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.2/ssbtoolkit/pathways/Gs_reactions.csv
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    15771 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.2/ssbtoolkit/pathways/OXTR_pathway.py
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1725 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.2/ssbtoolkit/pathways/OXTR_pathway_parameters.csv
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1319 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.2/ssbtoolkit/pathways/OXTR_pathway_reactions.csv
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    13822 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.2/ssbtoolkit/pathways/OXTR_pathway_testing.py
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.2/ssbtoolkit/pathways/__init__.py
+drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 11:49:05.024493 ssbtoolkit-1.0.2/ssbtoolkit.egg-info/
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      719 2023-04-10 11:49:04.000000 ssbtoolkit-1.0.2/ssbtoolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      742 2023-04-10 11:49:05.000000 ssbtoolkit-1.0.2/ssbtoolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)        1 2023-04-10 11:49:04.000000 ssbtoolkit-1.0.2/ssbtoolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      143 2023-04-10 11:49:04.000000 ssbtoolkit-1.0.2/ssbtoolkit.egg-info/requires.txt
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)       11 2023-04-10 11:49:04.000000 ssbtoolkit-1.0.2/ssbtoolkit.egg-info/top_level.txt
```

### Comparing `ssbtoolkit-1.0.1/setup.py` & `ssbtoolkit-1.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'Simulation of methematical models of signaling pathways of GPCRs'
 LONG_DESCRIPTION = 'The SSB computational toolkit was developed to easily predict classical pharmacodynamic models of drug-GPCR (class A) interactions given just as input structural information of the receptor and the ligand.'
 
 # Setting up
 setup(
     name="ssbtoolkit",
     version=VERSION,
```

### Comparing `ssbtoolkit-1.0.1/ssbtoolkit/Utils.py` & `ssbtoolkit-1.0.2/ssbtoolkit/Utils.py`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.1/ssbtoolkit/__init__.py` & `ssbtoolkit-1.0.2/ssbtoolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.1/ssbtoolkit/pathways/Gi.py` & `ssbtoolkit-1.0.2/ssbtoolkit/pathways/Gi.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         Initial(R(R_b1=None, R_p='p0', R_s='i'), Parameter('R_0', parameters['R_init'])) 
         Initial(L(L_b1=None), Parameter('L_0', parameters['L_init']))   
     else:
         Initial(R(R_b1=None, R_p='p0', R_s='a'), Parameter('RL_0', LR))   
         Initial(R(R_b1=None, R_p='p0', R_s='i'), Parameter('R_0', parameters['R_init']-LR))  
 
     
-    Initial(Gi(Gi_b1=None), )                  
+    Initial(Gi(Gi_b1=None), Parameter('Gi_0', parameters['Gi_init']))                  
     Initial(AC5(AC5_b1=None, AC5_b2=None, AC5_b3=None, AC5_s='i'), Parameter('AC5_0', parameters['AC5_init']))  
     Initial(Ca(Ca_b1=None, Ca_l='cytos', Ca_s='free'), Parameter('Ca_cytos_free', parameters['Ca_cytos_free'])) 
     Initial(ATP(), Parameter('ATP_0', parameters['ATP_init']))
     Initial(PDE4(PDE4_s='i'), Parameter('PDE4_0', parameters['PDE4_init']))
     Initial(PDE10(PDE10_c='N', PDE10_s='i'), Parameter('PDE10_0', parameters['PDE10_init']))
     Initial(PKA(PKA_s='cAMP0'), Parameter('PKA_0', parameters['PKA_init']))
```

### Comparing `ssbtoolkit-1.0.1/ssbtoolkit/pathways/Gi_parameters.csv` & `ssbtoolkit-1.0.2/ssbtoolkit/pathways/Gi_parameters.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.1/ssbtoolkit/pathways/Gi_reactions.csv` & `ssbtoolkit-1.0.2/ssbtoolkit/pathways/Gi_reactions.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.1/ssbtoolkit/pathways/Gq.py` & `ssbtoolkit-1.0.2/ssbtoolkit/pathways/Gq.py`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.1/ssbtoolkit/pathways/Gq_parameters.csv` & `ssbtoolkit-1.0.2/ssbtoolkit/pathways/Gq_parameters.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.1/ssbtoolkit/pathways/Gq_reactions.csv` & `ssbtoolkit-1.0.2/ssbtoolkit/pathways/Gq_reactions.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.1/ssbtoolkit/pathways/Gs.py` & `ssbtoolkit-1.0.2/ssbtoolkit/pathways/Gs.py`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.1/ssbtoolkit/pathways/Gs_parameters.csv` & `ssbtoolkit-1.0.2/ssbtoolkit/pathways/Gs_parameters.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.1/ssbtoolkit/pathways/Gs_reactions.csv` & `ssbtoolkit-1.0.2/ssbtoolkit/pathways/Gs_reactions.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.1/ssbtoolkit/pathways/OXTR_pathway.py` & `ssbtoolkit-1.0.2/ssbtoolkit/pathways/OXTR_pathway.py`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.1/ssbtoolkit/pathways/OXTR_pathway_parameters.csv` & `ssbtoolkit-1.0.2/ssbtoolkit/pathways/OXTR_pathway_parameters.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.1/ssbtoolkit/pathways/OXTR_pathway_reactions.csv` & `ssbtoolkit-1.0.2/ssbtoolkit/pathways/OXTR_pathway_reactions.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.1/ssbtoolkit/pathways/OXTR_pathway_testing.py` & `ssbtoolkit-1.0.2/ssbtoolkit/pathways/OXTR_pathway_testing.py`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.1/ssbtoolkit.egg-info/SOURCES.txt` & `ssbtoolkit-1.0.2/ssbtoolkit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-LICENSE
 MANIFEST.in
-README.md
 setup.py
-ssbtoolkit/HuTRdb.sqlite3
 ssbtoolkit/Utils.py
 ssbtoolkit/__init__.py
 ssbtoolkit.egg-info/PKG-INFO
 ssbtoolkit.egg-info/SOURCES.txt
 ssbtoolkit.egg-info/dependency_links.txt
 ssbtoolkit.egg-info/requires.txt
 ssbtoolkit.egg-info/top_level.txt
```


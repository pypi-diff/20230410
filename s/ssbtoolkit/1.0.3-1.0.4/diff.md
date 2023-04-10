# Comparing `tmp/ssbtoolkit-1.0.3.tar.gz` & `tmp/ssbtoolkit-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssbtoolkit-1.0.3.tar", last modified: Mon Apr 10 13:22:42 2023, max compression
+gzip compressed data, was "ssbtoolkit-1.0.4.tar", last modified: Mon Apr 10 13:29:04 2023, max compression
```

## Comparing `ssbtoolkit-1.0.3.tar` & `ssbtoolkit-1.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 13:22:42.696291 ssbtoolkit-1.0.3/
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)       66 2023-04-10 11:48:28.000000 ssbtoolkit-1.0.3/MANIFEST.in
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      719 2023-04-10 13:22:42.696291 ssbtoolkit-1.0.3/PKG-INFO
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)       38 2023-04-10 13:22:42.696291 ssbtoolkit-1.0.3/setup.cfg
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1261 2023-04-10 13:22:21.000000 ssbtoolkit-1.0.3/setup.py
-drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 13:22:42.692291 ssbtoolkit-1.0.3/ssbtoolkit/
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    17110 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.3/ssbtoolkit/Utils.py
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    71651 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.3/ssbtoolkit/__init__.py
-drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 13:22:42.696291 ssbtoolkit-1.0.3/ssbtoolkit/pathways/
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    20646 2023-04-10 13:18:09.000000 ssbtoolkit-1.0.3/ssbtoolkit/pathways/Gi.py
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1736 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.3/ssbtoolkit/pathways/Gi_parameters.csv
--rw-r--r--   0 rribeiro  (1000) rribeiro  (1000)     2640 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.3/ssbtoolkit/pathways/Gi_reactions.csv
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    14154 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.3/ssbtoolkit/pathways/Gq.py
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1153 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.3/ssbtoolkit/pathways/Gq_parameters.csv
--rw-r--r--   0 rribeiro  (1000) rribeiro  (1000)     1121 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.3/ssbtoolkit/pathways/Gq_reactions.csv
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    21135 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.3/ssbtoolkit/pathways/Gs.py
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1763 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.3/ssbtoolkit/pathways/Gs_parameters.csv
--rw-r--r--   0 rribeiro  (1000) rribeiro  (1000)     2709 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.3/ssbtoolkit/pathways/Gs_reactions.csv
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    15771 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.3/ssbtoolkit/pathways/OXTR_pathway.py
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1725 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.3/ssbtoolkit/pathways/OXTR_pathway_parameters.csv
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1319 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.3/ssbtoolkit/pathways/OXTR_pathway_reactions.csv
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    13822 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.3/ssbtoolkit/pathways/OXTR_pathway_testing.py
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.3/ssbtoolkit/pathways/__init__.py
-drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 13:22:42.692291 ssbtoolkit-1.0.3/ssbtoolkit.egg-info/
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      719 2023-04-10 13:22:42.000000 ssbtoolkit-1.0.3/ssbtoolkit.egg-info/PKG-INFO
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      742 2023-04-10 13:22:42.000000 ssbtoolkit-1.0.3/ssbtoolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)        1 2023-04-10 13:22:42.000000 ssbtoolkit-1.0.3/ssbtoolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      143 2023-04-10 13:22:42.000000 ssbtoolkit-1.0.3/ssbtoolkit.egg-info/requires.txt
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)       11 2023-04-10 13:22:42.000000 ssbtoolkit-1.0.3/ssbtoolkit.egg-info/top_level.txt
+drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 13:29:04.810112 ssbtoolkit-1.0.4/
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)       66 2023-04-10 11:48:28.000000 ssbtoolkit-1.0.4/MANIFEST.in
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      719 2023-04-10 13:29:04.810112 ssbtoolkit-1.0.4/PKG-INFO
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)       38 2023-04-10 13:29:04.810112 ssbtoolkit-1.0.4/setup.cfg
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1261 2023-04-10 13:28:09.000000 ssbtoolkit-1.0.4/setup.py
+drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 13:29:04.810112 ssbtoolkit-1.0.4/ssbtoolkit/
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    17110 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.4/ssbtoolkit/Utils.py
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    71651 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.4/ssbtoolkit/__init__.py
+drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 13:29:04.810112 ssbtoolkit-1.0.4/ssbtoolkit/pathways/
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    20642 2023-04-10 13:28:52.000000 ssbtoolkit-1.0.4/ssbtoolkit/pathways/Gi.py
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1736 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.4/ssbtoolkit/pathways/Gi_parameters.csv
+-rw-r--r--   0 rribeiro  (1000) rribeiro  (1000)     2640 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.4/ssbtoolkit/pathways/Gi_reactions.csv
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    14154 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.4/ssbtoolkit/pathways/Gq.py
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1153 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.4/ssbtoolkit/pathways/Gq_parameters.csv
+-rw-r--r--   0 rribeiro  (1000) rribeiro  (1000)     1121 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.4/ssbtoolkit/pathways/Gq_reactions.csv
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    21135 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.4/ssbtoolkit/pathways/Gs.py
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1763 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.4/ssbtoolkit/pathways/Gs_parameters.csv
+-rw-r--r--   0 rribeiro  (1000) rribeiro  (1000)     2709 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.4/ssbtoolkit/pathways/Gs_reactions.csv
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    15771 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.4/ssbtoolkit/pathways/OXTR_pathway.py
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1725 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.4/ssbtoolkit/pathways/OXTR_pathway_parameters.csv
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1319 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.4/ssbtoolkit/pathways/OXTR_pathway_reactions.csv
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    13822 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.4/ssbtoolkit/pathways/OXTR_pathway_testing.py
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.4/ssbtoolkit/pathways/__init__.py
+drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 13:29:04.810112 ssbtoolkit-1.0.4/ssbtoolkit.egg-info/
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      719 2023-04-10 13:29:04.000000 ssbtoolkit-1.0.4/ssbtoolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      742 2023-04-10 13:29:04.000000 ssbtoolkit-1.0.4/ssbtoolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)        1 2023-04-10 13:29:04.000000 ssbtoolkit-1.0.4/ssbtoolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      143 2023-04-10 13:29:04.000000 ssbtoolkit-1.0.4/ssbtoolkit.egg-info/requires.txt
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)       11 2023-04-10 13:29:04.000000 ssbtoolkit-1.0.4/ssbtoolkit.egg-info/top_level.txt
```

### Comparing `ssbtoolkit-1.0.3/PKG-INFO` & `ssbtoolkit-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssbtoolkit
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simulation of methematical models of signaling pathways of GPCRs
 Author: Rui Ribeiro
 Author-email: <rui.ribeiro@univr.it>
 Keywords: python,bioinformatics,Systems Biology,GPCR
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ssbtoolkit-1.0.3/setup.py` & `ssbtoolkit-1.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.0.3'
+VERSION = '1.0.4'
 DESCRIPTION = 'Simulation of methematical models of signaling pathways of GPCRs'
 LONG_DESCRIPTION = 'The SSB computational toolkit was developed to easily predict classical pharmacodynamic models of drug-GPCR (class A) interactions given just as input structural information of the receptor and the ligand.'
 
 # Setting up
 setup(
     name="ssbtoolkit",
     version=VERSION,
```

### Comparing `ssbtoolkit-1.0.3/ssbtoolkit/Utils.py` & `ssbtoolkit-1.0.4/ssbtoolkit/Utils.py`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.3/ssbtoolkit/__init__.py` & `ssbtoolkit-1.0.4/ssbtoolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.3/ssbtoolkit/pathways/Gi.py` & `ssbtoolkit-1.0.4/ssbtoolkit/pathways/Gi.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
     Parameter('AC5_Ca_GaiGTP_decay', parameters['AC5_Ca_GaiGTP_decay'])
     Rule('reaction60', AC5(AC5_b1=None, AC5_b2=20, AC5_b3=10, AC5_s='i') % Ca(Ca_b1=20, Ca_l='cytos', Ca_s='buff') % GaiGTP(GaiGTP_b1=10) >> AC5(AC5_b1=None, AC5_b2=20, AC5_b3=None, AC5_s='i') % Ca(Ca_b1=20, Ca_l='cytos', Ca_s='buff') + GaiGDP(), AC5_Ca_GaiGTP_decay)
 
     Parameter('AC5_Ca_GaiGTP_ATP_decay', parameters['AC5_Ca_GaiGTP_ATP_decay'])
     Rule('reaction61', AC5(AC5_b1=None, AC5_b2=20, AC5_b3=10, AC5_s='a') % Ca(Ca_b1=20, Ca_l='cytos', Ca_s='buff') % GaiGTP(GaiGTP_b1=10) >> AC5(AC5_b1=None, AC5_b2=20, AC5_b3=None, AC5_s='a') % Ca(Ca_b1=20, Ca_l='cytos', Ca_s='buff') + GaiGDP(), AC5_Ca_GaiGTP_ATP_decay)
 
     '''Several Subtypes of Phosphodiesterases (PDE) degrade cAMP'''
-    Parameter('PDE104_cAMP_kon', parameters['PDE104_cAMP_kon'])
+    Parameter('PDE4_cAMP_kon', parameters['PDE4_cAMP_kon'])
     Parameter('PDE4_cAMP_koff', parameters['PDE4_cAMP_koff'])
     Rule('reaction73', PDE4(PDE4_s='i') + cAMP() | PDE4(PDE4_s='a'), PDE4_cAMP_kon, PDE4_cAMP_koff)
 
     Parameter('PDE4_cAMP_to_AMP', parameters['PDE4_cAMP_to_AMP'])
     Rule('reaction75', PDE4(PDE4_s='a') >> PDE4(PDE4_s='i') + AMP(), PDE4_cAMP_to_AMP)
 
     Parameter('PDE10_2cAMP_kon', parameters['PDE10_2cAMP_kon'])
```

### Comparing `ssbtoolkit-1.0.3/ssbtoolkit/pathways/Gi_parameters.csv` & `ssbtoolkit-1.0.4/ssbtoolkit/pathways/Gi_parameters.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.3/ssbtoolkit/pathways/Gi_reactions.csv` & `ssbtoolkit-1.0.4/ssbtoolkit/pathways/Gi_reactions.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.3/ssbtoolkit/pathways/Gq.py` & `ssbtoolkit-1.0.4/ssbtoolkit/pathways/Gq.py`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.3/ssbtoolkit/pathways/Gq_parameters.csv` & `ssbtoolkit-1.0.4/ssbtoolkit/pathways/Gq_parameters.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.3/ssbtoolkit/pathways/Gq_reactions.csv` & `ssbtoolkit-1.0.4/ssbtoolkit/pathways/Gq_reactions.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.3/ssbtoolkit/pathways/Gs.py` & `ssbtoolkit-1.0.4/ssbtoolkit/pathways/Gs.py`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.3/ssbtoolkit/pathways/Gs_parameters.csv` & `ssbtoolkit-1.0.4/ssbtoolkit/pathways/Gs_parameters.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.3/ssbtoolkit/pathways/Gs_reactions.csv` & `ssbtoolkit-1.0.4/ssbtoolkit/pathways/Gs_reactions.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.3/ssbtoolkit/pathways/OXTR_pathway.py` & `ssbtoolkit-1.0.4/ssbtoolkit/pathways/OXTR_pathway.py`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.3/ssbtoolkit/pathways/OXTR_pathway_parameters.csv` & `ssbtoolkit-1.0.4/ssbtoolkit/pathways/OXTR_pathway_parameters.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.3/ssbtoolkit/pathways/OXTR_pathway_reactions.csv` & `ssbtoolkit-1.0.4/ssbtoolkit/pathways/OXTR_pathway_reactions.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.3/ssbtoolkit/pathways/OXTR_pathway_testing.py` & `ssbtoolkit-1.0.4/ssbtoolkit/pathways/OXTR_pathway_testing.py`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.3/ssbtoolkit.egg-info/PKG-INFO` & `ssbtoolkit-1.0.4/ssbtoolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssbtoolkit
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simulation of methematical models of signaling pathways of GPCRs
 Author: Rui Ribeiro
 Author-email: <rui.ribeiro@univr.it>
 Keywords: python,bioinformatics,Systems Biology,GPCR
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ssbtoolkit-1.0.3/ssbtoolkit.egg-info/SOURCES.txt` & `ssbtoolkit-1.0.4/ssbtoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*


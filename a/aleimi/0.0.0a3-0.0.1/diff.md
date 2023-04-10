# Comparing `tmp/aleimi-0.0.0a3.tar.gz` & `tmp/aleimi-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleimi-0.0.0a3.tar", last modified: Wed Jan 18 10:49:29 2023, max compression
+gzip compressed data, was "aleimi-0.0.1.tar", last modified: Mon Apr 10 18:34:06 2023, max compression
```

## Comparing `aleimi-0.0.0a3.tar` & `aleimi-0.0.1.tar`

### file list

```diff
@@ -1,31 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 10:49:29.941567 aleimi-0.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-18 10:49:06.000000 aleimi-0.0.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-18 10:49:06.000000 aleimi-0.0.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-01-18 10:49:29.941567 aleimi-0.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-01-18 10:49:06.000000 aleimi-0.0.0a3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 10:49:29.941567 aleimi-0.0.0a3/aleimi/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2292 2023-01-18 10:49:06.000000 aleimi-0.0.0a3/aleimi/OBconvert.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-01-18 10:49:06.000000 aleimi-0.0.0a3/aleimi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-01-18 10:49:06.000000 aleimi-0.0.0a3/aleimi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 10:49:29.941567 aleimi-0.0.0a3/aleimi/benchmarck/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-18 10:49:06.000000 aleimi-0.0.0a3/aleimi/benchmarck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-01-18 10:49:06.000000 aleimi-0.0.0a3/aleimi/benchmarck/benchmarck.py
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-01-18 10:49:06.000000 aleimi-0.0.0a3/aleimi/benchmarck/calc_bond_angle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-01-18 10:49:06.000000 aleimi-0.0.0a3/aleimi/boltzmann.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3938 2023-01-18 10:49:06.000000 aleimi-0.0.0a3/aleimi/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9668 2023-01-18 10:49:06.000000 aleimi-0.0.0a3/aleimi/confgen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-01-18 10:49:06.000000 aleimi-0.0.0a3/aleimi/continuation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-01-18 10:49:06.000000 aleimi-0.0.0a3/aleimi/extractor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1984 2023-01-18 10:49:06.000000 aleimi-0.0.0a3/aleimi/home.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-01-18 10:49:06.000000 aleimi-0.0.0a3/aleimi/processed.py
--rw-r--r--   0 runner    (1001) docker     (123)    30065 2023-01-18 10:49:06.000000 aleimi-0.0.0a3/aleimi/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-01-18 10:49:06.000000 aleimi-0.0.0a3/aleimi/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 10:49:29.941567 aleimi-0.0.0a3/aleimi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-01-18 10:49:29.000000 aleimi-0.0.0a3/aleimi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-01-18 10:49:29.000000 aleimi-0.0.0a3/aleimi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 10:49:29.000000 aleimi-0.0.0a3/aleimi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-18 10:49:29.000000 aleimi-0.0.0a3/aleimi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-18 10:49:29.000000 aleimi-0.0.0a3/aleimi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-18 10:49:29.000000 aleimi-0.0.0a3/aleimi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-01-18 10:49:29.941567 aleimi-0.0.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-18 10:49:06.000000 aleimi-0.0.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:34:06.688321 aleimi-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 18:33:19.000000 aleimi-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-04-10 18:34:06.688321 aleimi-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-04-10 18:33:19.000000 aleimi-0.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-10 18:33:19.000000 aleimi-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:34:06.688321 aleimi-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:34:06.684321 aleimi-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:34:06.688321 aleimi-0.0.1/src/aleimi/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-10 18:33:19.000000 aleimi-0.0.1/src/aleimi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 18:34:06.000000 aleimi-0.0.1/src/aleimi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-04-10 18:33:19.000000 aleimi-0.0.1/src/aleimi/boltzmann.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3469 2023-04-10 18:33:19.000000 aleimi-0.0.1/src/aleimi/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12208 2023-04-10 18:33:19.000000 aleimi-0.0.1/src/aleimi/confgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-10 18:33:19.000000 aleimi-0.0.1/src/aleimi/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-04-10 18:33:19.000000 aleimi-0.0.1/src/aleimi/processed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-04-10 18:33:19.000000 aleimi-0.0.1/src/aleimi/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-10 18:33:19.000000 aleimi-0.0.1/src/aleimi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:34:06.688321 aleimi-0.0.1/src/aleimi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-04-10 18:34:06.000000 aleimi-0.0.1/src/aleimi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-10 18:34:06.000000 aleimi-0.0.1/src/aleimi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:34:06.000000 aleimi-0.0.1/src/aleimi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-10 18:34:06.000000 aleimi-0.0.1/src/aleimi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-10 18:34:06.000000 aleimi-0.0.1/src/aleimi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 18:34:06.000000 aleimi-0.0.1/src/aleimi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:34:06.688321 aleimi-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-10 18:33:19.000000 aleimi-0.0.1/tests/test_aleimi.py
```

### Comparing `aleimi-0.0.0a3/LICENSE` & `aleimi-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aleimi-0.0.0a3/aleimi/boltzmann.py` & `aleimi-0.0.1/src/aleimi/boltzmann.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,38 @@
+#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-"""
-===============================================================================
-Created on    : Thu Aug 22 22:23:48 2019
-Author        : Alejandro Martínez León
-Mail          : [amleon@instec.cu, ale94mleon@gmail.com]
-Affiliation   : Chemical Systems Modeling Group,
-Affiliation   : Faculty of Radiochemistry, InSTEC-University of Havana, Cuba.
-===============================================================================
-DESCRIPTION   :
-DEPENDENCIES  :
-===============================================================================
-"""
 
 import rmsd
 import numpy as np
 import pandas as pd
 import os
+from aleimi import utils
 
-def arc_reader (arcf):
-    with open(arcf, 'rt', encoding='latin-1') as a:
+def arc_reader (arc:str):
+    """This , for sure, will change in the future to a more object-oriented paradigm
+    It reads a arc MOPAC file and give a tuple of
+
+    Parameters
+    ----------
+    arc : str
+        The arc file path
+
+    Returns
+    -------
+    list[tuple]
+        A list of tuple sorted by energy. Each tuple contains:
+            #. cells: conformer identifier,
+            #. HeatsOfFormation_kcalmol: self-explanatory,
+            #. CONTAINER__H: Coordinates numpy array of the heavy atoms with shape (Number of heavy atoms, 3),
+            #. Class_E: The classic energy calculated during :meth:`aleimi.confgen.main`
+    """
+    with open(arc, 'rt', encoding='latin-1') as a:
         lines = a.readlines()
-    
-    # getting data from arc                                                       #
+
+    # getting data from arc
     HeatsOfFormation_kcalmol = []
     cells = []
     Class_E = []
     # finding No. of atoms
     for line in lines:
         if 'Empirical Formula' in line:
             natoms = int(line.split()[-2])
@@ -62,18 +69,32 @@
             CONTAINER__H.append(np.array(cart__H, dtype=np.float64))
     #atoms = (np.asarray(atoms))
     # .... organizing
     paired = list(zip(cells, HeatsOfFormation_kcalmol, CONTAINER__H, Class_E)) # Esto genera un arreglo de tuplas, me une los arreglos
     ORDERED = sorted(paired, key=lambda x: x[1])  #Esto ordena la tupla segun la energia de menor a mayor
     return ORDERED #, atoms]
 
-def ignoreLines(f, n):
-    for i in range(n): f.readline()
-
 def out_reader (out):
+    """This , for sure, will change in the future to a more object-oriented paradigm
+    It reads a out MOPAC file and give a tuple of
+
+    Parameters
+    ----------
+    out : str
+        The arc file path
+
+    Returns
+    -------
+    list[tuple]
+        A list of tuple sorted by energy. Each tuple contains:
+            #. cells: conformer identifier,
+            #. HeatsOfFormation_kcalmol: self-explanatory,
+            #. CONTAINER__H: Coordinates numpy array of the heavy atoms with shape (Number of heavy atoms, 3)
+            #. Class_E: The classic energy calculated during :meth:`aleimi.confgen.main`
+    """
     f = open(out, 'r')
     chunk = []
     HeatsOfFormation_kcalmol = []
     cells = []
     Class_E = []
     CONTAINER__H = []
     cart__H = []
@@ -82,16 +103,15 @@
     # getting data from out                                                       #
     # finding No. of atoms
     while True:
         line = f.readline()
         if "Empirical Formula" in line:
             natoms = int(line.split()[-2])
             break
-            f.close
-       
+
     f = open(out, 'r')
     while True:
         line = f.readline()
         if len(line) == 0:break
                
         if 79*'-' in line:
             while True:
@@ -106,17 +126,17 @@
 
                 elif 'CELL' in line:
                     cells.append(int(line.split(':')[1]))
                     
                 elif 'HEAT OF FORMATION' in line:
                     HeatsOfFormation_kcalmol.append(float(line.split()[-5]))
                 elif 'CARTESIAN COORDINATES' in line:
-                    ignoreLines(f, 1)
+                    utils.ignoreLines(f, 1)
                     cont = 0
-                    chunk = []        
+                    chunk = []
                     while cont < natoms:
                         chunk.append(f.readline())
                         cont += 1
                     cart__H = []
                     for c in chunk:
                         if c.split()[1] != 'H':
                             cart__H.append([c.split()[2], c.split()[3], c.split()[4]]) # No estoy tomando los atomos, solamente coordenadas c.split()[0].strip(),
@@ -124,43 +144,59 @@
             CONTAINER__H.append(np.array(cart__H, dtype=np.float64))
     f.close
     # .... organizing
     paired = list(zip(cells, HeatsOfFormation_kcalmol, CONTAINER__H, Class_E)) # Esto genera un arreglo de tuplas, me une los arreglos
     ORDERED = sorted(paired, key=lambda x: x[1])  #Esto ordena la tupla segun la energia de menor a mayor
     return ORDERED
 
-def main(file_path, Bd_rmsd = 1.0, Bd_E = 0.0, BOutPath = True):
-    """This function generates a table with the population of each conformer respect to a Boltzmann probability distribution.
+def main(file_path:str, Bd_rmsd:float = 1.0, Bd_E:float = 0.0, BOutPath:bool = True) -> pd.DataFrame:
+    """It reads the MOPAC output file (arc or out) and create a Boltzmann table
 
-    Args:
-        file_path (path): arc or out file. It will be read with arc_reader or out_reader depending on the extension.
-        d_rmsd (float): Difference in RMSD (Angstrom) between the conformers. Defaults is 1.0.
-        d_E (float, optional): In case that also you need to screen with a threshold of energy, you specify the value in kcal/mol. Defaults to None.
-        out_path (path): In case that you want to write down the table, the path for the file.
-
-    Raises:
-        ValueError: The Boltzmann table
+    Parameters
+    ----------
+    file_path : str
+        MOPAC output (.arc or .out). It will be read with :meth:`aleimi.boltzmann.arc_reader` or :meth:`aleimi.boltzmann.out_reader`
+        depending on the extension.
+    Bd_rmsd : float, optional
+        RMSD to filter out redundant conformations, geometric filter, by default 1.0
+    Bd_E : float, optional
+        Energy difference in kJ to filter out redundant conformations, geometric filter, by default 1.0, by default 0.0
+    BOutPath : bool, optional
+        Directory to ouput the table {file_name}_boltzmann.csv", by default True
+
+    Returns
+    -------
+    pd.DataFrame
+
+    A Table with columns:
+        #. `cell`: conformer identifier,
+        #. `Class_E`: Classic energy from the RDKit optimization. in this example is `NaN` because we did not perform this optimization,
+        #. `HeatOfFormation_kcal`: self-explanatory [kcal/mol],
+        #. `Emin_Ei`: Difference in energy between the lower and the i-th conformer in [kcal/mol],
+        #. `qi__Pi/Pmin__e^(Emin_Ei)/KbT`: Boltzmann factors,
+        #. `Fraction_%__100*qi/q`: Occupancy of each conformer,
+
+    Raises
+    ------
+    ValueError
+        _description_
     """
-
-    # d_E = 0.001
-    # d_rmsd = 1.0
-    ext = os.path.basename(file_path).split('.')[-1]
-    name = os.path.basename(file_path)[:-(len(ext) + 1)]
+    name, ext = os.path.splitext(os.path.basename(file_path))
     
-    if ext == 'arc':
+    if ext == '.arc':
         ordered = (arc_reader(file_path))
-    elif ext == 'out':
+    elif ext == '.out':
         ordered = (out_reader(file_path))
     else:
-        raise ValueError(f"{file_path} does not have .arc or .out extension. Therefore is not readeable by ALEIMI.")
+        raise ValueError(f"{file_path} does not have .arc or .out extension. Therefore is not readable by ALEIMI.")
 
     if Bd_E:
-        for i, x in enumerate(range(len(ordered))):
+        for i, _ in enumerate(ordered):
             to_trash_degenerated = []
-            for idx, y in enumerate(range(len(ordered))):
+            for idx, _ in enumerate(ordered):
                 if i < idx:
                     Ei = ordered[i][1]
                     Eidx = ordered[idx][1]
                     delta = abs(Ei - Eidx)
                     if delta <= Bd_E:
     # =============================================================
     #     CHECKING Geometric degeneracy
@@ -173,15 +209,15 @@
                         if RMSD <= Bd_rmsd:
                         # reject identical structure
                             to_trash_degenerated.append(idx)
 # =========================================================================
 #     FOR EACH STRUCTURE, eliminate degenerated and save lot of time
 # =========================================================================
             to_trash_degenerated = sorted(to_trash_degenerated, reverse=True)
-            [ordered.pop(x) for x in to_trash_degenerated]
+            _ = [ordered.pop(x) for x in to_trash_degenerated]
 
     else:
         for i, x in enumerate(range(len(ordered))):
             to_trash_degenerated = []
             for idx, y in enumerate(range(len(ordered))):
                 if i < idx:
                 
@@ -204,39 +240,40 @@
             [ordered.pop(x) for x in to_trash_degenerated]
         
 
 
 # =============================================================================
 #      WORKING with UNDEGENERATED. Cambie la manera de calculos los parametros:
 #Me base en: James B. Foresman - Exploring Chemistry With Electronic Structure Methods 3rd edition (2015) pag 182
-# y Mortimer_Physical Chemistry_(3rd.ed.-2008) pag 1045    
+# y Mortimer_Physical Chemistry_(3rd.ed.-2008) pag 1045
 # =============================================================================
     Kb = 1.987204259E-3                        # kcal/(mol⋅K)
     T = 298.15                                 # Absolute T (K)
     DF = pd.DataFrame()
     cells = [ordered[i][0] for i, x in enumerate(ordered)]
     Class_E = [ordered[i][3] for i, x in enumerate(ordered)]
     HeatsOfFormation_kcalmol = [ordered[i][1] for i, x in enumerate(ordered)]
     MinHeatsOfFormation_kcalmol = min(HeatsOfFormation_kcalmol)
-    relative_kJ = [MinHeatsOfFormation_kcalmol - x for x in HeatsOfFormation_kcalmol]
-    qi = [np.exp(E_r/(Kb*T)) for E_r in relative_kJ]
+    relative_kcalmol = [MinHeatsOfFormation_kcalmol - x for x in HeatsOfFormation_kcalmol]
+    qi = [np.exp(E_r/(Kb*T)) for E_r in relative_kcalmol]
     q = sum(qi)
     Fraction = [100*i/q for i in qi]
-    #Z = [np.e**(-(E/(k*T))) for E in energy_kcal] #no pudo calcular Z: verflowError: (34, 'Result too large') 
+    #Z = [np.e**(-(E/(k*T))) for E in energy_kcal] #no pudo calcular Z: verflowError: (34, 'Result too large')
     #Pi_b = [(np.e**-(E/(k*T)))/Z for E in energy_kcal]
     # =============================================================================
     #     DATAFRAME
     # =============================================================================
     DF['cell'] = cells
     DF['Class_E'] = Class_E
     DF['HeatOfFormation_kcal/mol'] = HeatsOfFormation_kcalmol
-    DF['Emin_Ei'] = relative_kJ
+    DF['Emin_Ei'] = relative_kcalmol
     DF['qi__Pi/Pmin__e^(Emin_Ei)/KbT'] = qi
     DF['Fraction_%__100*qi/q'] = Fraction
 
     if BOutPath:
-        with open(f"{name}.boltzmann", 'wt') as rp:
-            DF.to_string(rp)
+        with open(f"{name}_boltzmann.csv", 'wt') as rp:
+            DF.to_csv(rp)
+    
     return DF
 
 
-
+if __name__ == '__main__':...
```

### Comparing `aleimi-0.0.0a3/aleimi/cli.py` & `aleimi-0.0.1/src/aleimi/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,97 +1,88 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-from aleimi import confgen, boltzmann, extractor, tools, __version__
-import argparse
-import os
+from aleimi import confgen, boltzmann, extractor, __version__, utils
+import argparse, os, yaml
 
 """
 Tengo que adicionar la parte de los comandos extras para pasarselos a exrtractor
 para la creacion de los templates, probar con los argumentos que se pasan
 si alguno esta mal entonces dlanzar un warning o algo por el estilo
 Tengo que ver esto bien, me falta por implemnetar lo fde .gjf
 Y lo de el analisis para al menos psi4 y orca
     """
 
 def _aleimi():
+    """CLI of ``aleimi``
+    """
     parser = argparse.ArgumentParser(description=__doc__,
                                      formatter_class=argparse.RawTextHelpFormatter)
 
     parser.add_argument(
-        help = "The path were the molecule(s) is(are)",
+        help = "The path to the directory were the molecule(s) is(are)",
         dest='suppl',
         type=str)
     parser.add_argument(
         '-p', '--params',
         help = "Parameters to run ALEIMI",
+        default=None,
         dest='params',
         type=str)
     parser.add_argument(
         '-v', '--version',
         action='version',
         version=f"aleimi: {__version__}")
 
     args = parser.parse_args()
 
     suppl = args.suppl
     params = args.params
-    if not os.path.exists(suppl):
-        raise FileNotFoundError(f"{suppl} does not exist or is not accessible.")
-    if not os.path.exists(params):
-        raise FileNotFoundError(f"{params} does not exist or is not accessible.")
-
+    if not os.path.exists(args.suppl):
+        raise FileNotFoundError(f"{args.suppl} does not exist or is not accessible.")
 
+    # Getting the default kwargs of all the functions.
+    confgen_keywords = utils.get_default_kwargs(confgen.main)
+    boltzmann_keywords = utils.get_default_kwargs(boltzmann.main)
+    extractor_keywords = utils.get_default_kwargs(extractor.main)
+    used_keywords = {**confgen_keywords, **boltzmann_keywords, **boltzmann_keywords}
+    if args.params:
+        if not os.path.exists(params):
+            raise FileNotFoundError(f"{params} does not exist or is not accessible.")
+        
+        with open(args.params, 'r') as params:
+            user_keywords =  yaml.safe_load(params)
+
+        for key in confgen_keywords.keys():
+            if key in user_keywords:
+                try:
+                    confgen_keywords[key] = type(confgen_keywords[key])(user_keywords[key]) # Here I  am taking the type of the variable
+                except:
+                    raise ValueError(f"{user_keywords[key]} must be a {type(confgen_keywords[key])}-like")
+
+        for key in boltzmann_keywords.keys():
+            if key in user_keywords:
+                try:
+                    boltzmann_keywords[key] = type(boltzmann_keywords[key])(user_keywords[key]) # Here I  am taking the type of the variable
+                except:
+                    raise ValueError(f"{user_keywords[key]} must be a {type(boltzmann_keywords[key])}-like")
+
+        for key in extractor_keywords.keys():
+            if key in user_keywords:
+                try:
+                    extractor_keywords[key] = type(extractor_keywords[key])(user_keywords[key]) # Here I  am taking the type of the variable
+                except:
+                    raise ValueError(f"{user_keywords[key]} must be a {type(extractor_keywords[key])}-like")
+
+    # Save the config as a yaml file
+    with open('outparams.yml', 'w') as f:
+        yaml.dump(used_keywords, f)
 
-    with open(params,'r') as f:
-        lines = f.readlines()
-
-    user_keywords = {}
-    for line in lines:
-        if not line.startswith('#') and len(line.strip()):
-            line = line.split('#')[0]
-            index = line.index('=') # Only get the first equal
-            key, value = line[:index].replace('-', '_').strip(), line[index+1:].strip()
-            user_keywords[key] = value
-    user_keys = user_keywords.keys()
-
-    confgen_keywords = tools.get_default_args(confgen.main)
-    for key in confgen_keywords.keys():
-        if key in user_keys:
-            try:
-                confgen_keywords[key] = type(confgen_keywords[key])(user_keywords[key]) # Here I  am taking the type of the variable
-            except:
-                raise ValueError(f"{user_keywords[key]} must be a {type(confgen_keywords[key])}-like")
-
-    mopac_keywords = tools.get_default_args(tools.mopac)
-    for key in mopac_keywords.keys():
-        if key in user_keys:
-            try:
-                mopac_keywords[key] = type(mopac_keywords[key])(user_keywords[key]) # Here I  am taking the type of the variable
-            except:
-                raise ValueError(f"{user_keywords[key]} must be a {type(mopac_keywords[key])}-like")
-
-    boltzmann_keywords = tools.get_default_args(boltzmann.main)
-    for key in boltzmann_keywords.keys():
-        if key in user_keys:
-            try:
-                boltzmann_keywords[key] = type(boltzmann_keywords[key])(user_keywords[key]) # Here I  am taking the type of the variable
-            except:
-                raise ValueError(f"{user_keywords[key]} must be a {type(boltzmann_keywords[key])}-like")
-
-    extractor_keywords = tools.get_default_args(extractor.main)
-    for key in extractor_keywords.keys():
-        if key in user_keys:
-            try:
-                extractor_keywords[key] = type(extractor_keywords[key])(user_keywords[key]) # Here I  am taking the type of the variable
-            except:
-                raise ValueError(f"{user_keywords[key]} must be a {type(extractor_keywords[key])}-like")
-
-    with open('outparams.params', 'w') as f:
-        used_keywords = {**confgen_keywords, **mopac_keywords, **boltzmann_keywords, **boltzmann_keywords}
-        for key in used_keywords:
-            f.write(f"{key:<35} = {used_keywords[key]:<20}\n")
 
     mol_names = confgen.main(suppl,**confgen_keywords)
     for mol_name in mol_names:
-        tools.mopac(f"{mol_name}.mop",**mopac_keywords)
+        print(mol_name)
+        utils.mopac(f"{mol_name}.mop")
         boltzmann.main(f"{mol_name}.arc",**boltzmann_keywords)
-        extractor.main(f"{mol_name}.arc",f"{mol_name}.boltzmann", **boltzmann_keywords)
+        extractor.main(f"{mol_name}.arc",f"{mol_name}_boltzmann.csv", **boltzmann_keywords)
+
+
+if __name__ == '__main__':...
```

### Comparing `aleimi-0.0.0a3/aleimi/extractor.py` & `aleimi-0.0.1/src/aleimi/extractor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-"""
-===============================================================================
-Created on    : 2020-2023
-Author        : Alejandro Martínez León
-Mail          : [alejandro.martinezleon@uni-saarland.de, ale94mleon@gmail.com]
-Affiliation   : Jochen Hub's Biophysics Group
-Affiliation   : Faculty of NS, University of Saarland, Saarbrücken, Germany
-===============================================================================
-DESCRIPTION   :
-DEPENDENCIES  :
-===============================================================================
-"""
 import pandas as pd
 import os
-from aleimi import templates, tools
-
-
-def ignoreLines(f, n):
-    for i in range(n): f.readline()
+from aleimi import templates, utils
+from typing import List
 
 #def extract(arc_file, boltzmann_file, energy_cut = 2, conformer_cut = None, mksh = True, mkdir = True):
 # Energy cut is in kcal/mol
-def extract(boltzmann_file, energy_cut = 2, conformer_cut = None):
+def extract(boltzmann_file:str, energy_cut:float = 2.0, conformer_cut:int = None) -> List[int]:
+    """Extract the conformers based on the filters: energy_cut and/or conformer_cut
+
+    Parameters
+    ----------
+    boltzmann_file : str
+        The boltzmann file generated with `:meth: aleimi.boltzmann.main`
+    energy_cut : float, optional
+        Maximum difference in energy with respect the conformer with lowest energy, by default 2.0
+    conformer_cut : int, optional
+        Maximum number of conformers to export, by default None
+
+    Returns
+    -------
+    List[int]
+        The list of ``cell`` identifiers
+    """
+
+    df = pd.read_csv(boltzmann_file)
+    indx_to_extract = []
     if energy_cut:
-        df = pd.read_table(boltzmann_file, sep='\s+')
         df_subset = df[df.Emin_Ei >= -energy_cut]
-        indx_to_extract = df_subset.cell.tolist()    
-        indx_to_extract = sorted(indx_to_extract)
+        indx_to_extract += df_subset.cell.tolist()
 
-        
-    elif conformer_cut:
-        df = pd.read_table(boltzmann_file, sep='\s+')
+    if conformer_cut:
         df_subset = df.iloc[:conformer_cut]
-        indx_to_extract = df_subset.cell.tolist()    
-        indx_to_extract = sorted(indx_to_extract)        
+        indx_to_extract += df_subset.cell.tolist()
 
-    else:
-        df = pd.read_table(boltzmann_file, sep='\s+')
+    if not energy_cut and not conformer_cut:
         df_subset = df.iloc[:]
-        indx_to_extract = df_subset.cell.tolist()    
-        indx_to_extract = sorted(indx_to_extract)        
-    return indx_to_extract
+        indx_to_extract += df_subset.cell.tolist()
+
+    return sorted(indx_to_extract)
 
 def get_coords(input_file, indx_to_extract):
     
     file_ext = os.path.basename(input_file).split('.')[-1]
     file_name = os.path.basename(input_file)[:-(len(file_ext)+1)]
 
     if file_ext == 'arc':
@@ -71,15 +69,15 @@
 
     elif file_ext == 'out':
         f = open(input_file, 'r')
         chunk = []
         cart = []
 
 
-        # getting data from out                                                       #
+        # getting data from out
         # finding No. of atoms
         
         while True:
             line = f.readline()
             if "Empirical Formula" in line:
                 natoms = int(line.split()[-2])
                 f.close()
@@ -96,15 +94,15 @@
                     line = f.readline()
                     if (79*'*' in line) or (len(line) == 0):break
 
                     if 'CELL' in line: 
                         cell = int(line.split(':')[1])
 
                     elif 'CARTESIAN COORDINATES' in line and cell in indx_to_extract:
-                        ignoreLines(f, 1)
+                        utils.ignoreLines(f, 1)
                         cont = 0
                         chunk = []        
                         while cont < natoms:
                             chunk.append(f.readline())
                             cont += 1
                         cart = []
                         for c in chunk:
@@ -137,18 +135,17 @@
         InputExt = '.in'
     
     indx_to_extract = extract(boltzmann_file, energy_cut = energy_cut, conformer_cut = conformer_cut)
     names_coords = get_coords(input_file, indx_to_extract)
     for name, coords in names_coords:
         INPUT_obj = templates.INPUT(engine, machine = machine, name = name, coords = coords, **keywords)
         if mkdir:
-            tools.makedirs(name)
+            utils.makedirs(name)
             INPUT_obj.write(os.path.join(name, f"{name}{InputExt}"),'input')
             if jobsh:
                 INPUT_obj.write(os.path.join(name, f"job.sh"),'jobsh')
         else:
             INPUT_obj.write(f"{name}{InputExt}",'input')
             if jobsh:
                 INPUT_obj.write(f"{name}.sh",'jobsh')
 
-if __name__ == '__main__':
-    pass
+if __name__ == '__main__':...
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aleimi-0.0.0a3/aleimi/processed.py` & `aleimi-0.0.1/src/aleimi/processed.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,86 +1,91 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-"""
-===============================================================================
-Created on    : 2020-2023
-Author        : Alejandro Martínez León
-Mail          : [alejandro.martinezleon@uni-saarland.de, ale94mleon@gmail.com]
-Affiliation   : Jochen Hub's Biophysics Group
-Affiliation   : Faculty of NS, University of Saarland, Saarbrücken, Germany
-===============================================================================
-DESCRIPTION   :
-DEPENDENCIES  :
-===============================================================================
-"""
 import pandas as pd
 import numpy as np
 from glob import glob
 import os
 from rmsd import kabsch_rmsd
-import tempfile
-from aleimi import OBconvert, templates, tools
 
-def psi4_out_read(out):
+def psi4_out_read(out:str):
     """
     Parameters
     ----------
     out : str
         psi4 put file name.
     Returns
     -------
-    check_freq, Gibbs free energy, exyz, xyz2RMSD_H.
+    check_end, check_freq, Electronic energy, Gibbs free energy, exyz, xyz2RMSD_H.
     """
-    
+
     with open(out, 'rt', encoding='latin-1') as file:
         lines = file.readlines()
 
     if lines[-1].strip() == '*** Psi4 exiting successfully. Buy a developer a beer!':
         check_end = True
     else:
         check_end  = False
     check_freq = False
     E = 0
-    G = 0    
+    G = 0
     exyz = []
     xyz2RMSD_H =[]
 
-    for i in range(len(lines)):
+    for i, _ in enumerate(lines):
         if 'Final (previous) structure:' in lines[i]:
             E = float(lines[i-1].split()[-1])
             for j in range(i+2,len(lines)):
                 if 'Saving final (previous) structure.' in lines[j]: break
-                split = lines[j].split()    
+                split = lines[j].split()
                 exyz.append([split[0], float(split[1]), float(split[2]), float(split[3])])
                 if 'H' not in lines[j]:
                     xyz2RMSD_H.append([float(split[1]), float(split[2]), float(split[3])])
         if 'Freq [cm^-1]' in lines[i]:
             check_freq = True
             freqs = lines[i].split()[2:]
             for f in freqs:
-                """
-                 psi4 represent the imaginary number as 5i, 
-                 if an error ocurreduring the float convertion, 
-                 or it was converted but if less than cero (another error on sqrt) 
-                 then check_freq = False
-                """
+                # psi4 represent the imaginary number as 5i,
+                # if an error ocurreduring the float conversion, 
+                # or it was converted but if less than cero (another error on sqrt) 
+                # then check_freq = False
                 try:
                     np.sqrt(float(f))
                 except:
                     check_freq = False
                     break
         if 'Total G, Free enthalpy at  298.15 [K]' in lines[i]:
             G = float(lines[i].split('[K]')[1].split()[0])
         
     exyz = pd.DataFrame(exyz)
-    xyz2RMSD_H = np.array(xyz2RMSD_H, dtype=float)   
+    xyz2RMSD_H = np.array(xyz2RMSD_H, dtype=float)
     return check_end, check_freq, E, G, exyz, xyz2RMSD_H
 
-def main(SubDirs = True, engine = 'psi4', xyz_out = False, parameterize_path = './parameterize', machine = 'smaug', **keywords):
+def main(SubDirs:bool = True, engine:str = 'psi4', xyz_out:bool = False) -> dict:
+    """Process the output of the QM calculations generated through :meth:`aleimi.extractor.main`.
+    This function is quiet limited for now, Only useful for psi4 engine.
+
+    Parameters
+    ----------
+    SubDirs : bool, optional
+        Should be True if :meth:`aleimi.extractor.main` was used with ``mkdir = True``, by default True
+    engine : str, optional
+        psi4, gaussian or orca. It depends on the engine defined on :meth:`aleimi.extractor.main` was used with ``engine`` keyword, by default 'psi4'
+    xyz_out : bool, optional
+        If True, it will write the xyz coordinates of the conformer with the lowest energy, by default False
 
+    Returns
+    -------
+    dict
+        conf_name: 3D_coordinates
+
+    Raises
+    ------
+    FileNotFoundError
+        If there is not .out files
+    """
     if SubDirs:
         outs = [out for out in glob('*/*.out') if 'myjob' not in out]
 
         first_names = set()
         for out in outs:
             first_names.add(os.path.basename(out).split('_Cell')[0])
         first_names = list(first_names)
@@ -111,15 +116,15 @@
         if SubDirs:
             for out in outs:
                 if os.path.basename(out).split('_Cell')[0] == first_name:
                     to_work.append(out)
         else:
             for out in outs:
                 if out.split('_Cell')[0] == first_name:
-                    to_work.append(out)  
+                    to_work.append(out)
 
         Gibbs_free_energies = []
         coords = []
         coord2RMSD_Hs =[]
         good = []
 
         for item in to_work:
@@ -135,62 +140,52 @@
             else:
                 wrong_end.append(item)
         if good:
             paired = list(zip(good, Gibbs_free_energies, coords, coord2RMSD_Hs)) 
             ORDERED = sorted(paired, key=lambda x: x[1])
             coord_lower_energy[ORDERED[0][0].split('.')[0]] = ORDERED[0][2]
             to_print = []
-            for i in range(len(ORDERED)):
+            for i, _ in enumerate(ORDERED):
                 to_print.append([ORDERED[i][0].split('_Cell_')[-1].split('.')[0], ORDERED[i][1]])
             to_print = pd.DataFrame(to_print, columns = ['Cell', 'Gibbs (hartree/partícula)'])    
             print(first_name)
             print(to_print)
             print('\n')
             with open(first_name+'.orden', 'wt') as final:
                 to_print.to_string(final)
 
         
             rmsd_matrix = np.zeros((len(ORDERED),len(ORDERED)))
-            for i in range(len(rmsd_matrix)):
-                for j in range(len(rmsd_matrix)):
+            for i, _ in enumerate(rmsd_matrix):
+                for j, _ in enumerate(rmsd_matrix):
                     if j < i:
                         rmsd_matrix[i][j] = rmsd_matrix[j][i]
                     elif j == i:
                         rmsd_matrix[i][j] == 0.0
                     else:
                         # =============================================================
                         #     Calculando RMSD
                         # =============================================================
                         P = ORDERED[i][3]
                         Q = ORDERED[j][3]
                         rmsd_matrix[i][j] = kabsch_rmsd(P, Q, translate = True)
             index = [g.split('_Cell_')[-1].split('.')[0] for g in good]
             to_print_rmsd_matrix = pd.DataFrame(rmsd_matrix, index = index, columns = index)
             with open(first_name+'.rmsd', 'wt') as final:
-                to_print_rmsd_matrix.to_string(final) 
+                to_print_rmsd_matrix.to_string(final)
         #========================Se exporta el .xyz==================
             if xyz_out:
                 with open(ORDERED[0][0].split('.')[0]+'.xyz', 'wt') as final:
                     final.write(str(len(ORDERED[0][2]))+'\n\n')
                     ORDERED[0][2].to_string(final, header=False, index=False)
 
         
     #======================================================================
     if wrong_freq:
         print(f'Las cálculos: {wrong_freq} presentaron frecuencias negativas o imaginarias.')
     if wrong_end:
         print(f'Las cálculos: {wrong_end} presentaron problemas para un correcta finalizacion. Check the psi4 output!')
 
-    if parameterize_path:
-        for conf in coord_lower_energy:
-            conf_path = os.path.join(parameterize_path, conf)
-            tools.makedirs(conf_path)
-            xyztmp = tempfile.NamedTemporaryFile(suffix='.xyz')
-            with open(xyztmp.name, 'w') as t:
-                t.write(f"{len(coord_lower_energy[conf])}\n\n")
-                coord_lower_energy[conf].to_string(t, header=False, index=False)
-            OBconvert.obconvert(xyztmp.name, os.path.join(conf_path, f"{conf}.mol2"))
-            templates.PARAM(machine=machine, name = conf, **keywords).write(os.path.join(conf_path, f"{conf}.sh"))
-
     return coord_lower_energy
 
- 
+
+if __name__ == '__main__':...
```

### Comparing `aleimi-0.0.0a3/aleimi/templates.py` & `aleimi-0.0.1/src/aleimi/templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,9 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-"""
-===============================================================================
-Created on    : 2020-2023
-Author        : Alejandro Martínez León
-Mail          : [alejandro.martinezleon@uni-saarland.de, ale94mleon@gmail.com]
-Affiliation   : Jochen Hub's Biophysics Group
-Affiliation   : Faculty of NS, University of Saarland, Saarbrücken, Germany
-===============================================================================
-DESCRIPTION   :
-DEPENDENCIES  :
-===============================================================================
-"""
 import pandas as pd
 import copy, os
 class INPUT:
     def __init__(self, engine, machine = 'smaug', **keywords):
         self.engine = engine
         self.machine = machine
         self.default_partition = {'smaug': 'deflt', 'gwdg': 'medium'}
@@ -82,15 +70,15 @@
         }
         self.keywords = copy.deepcopy(self.default_keywords)
         for key in keywords:
             self.keywords[engine][key] = keywords[key]
         self.input = ''
         self.jobsh = ''
         self.parse()
-    
+
     def parse(self):
         if self.engine == 'psi4':
             self.input += f"#! Computation at {self.keywords[self.engine]['theory']}/{self.keywords[self.engine]['basis']} for {self.keywords[self.engine]['name']} \n\n"\
             f"memory {self.keywords[self.engine]['memory']}\n\n"\
             f"molecule {self.keywords[self.engine]['name']} {'{'}\n"\
             f"{self.keywords[self.engine]['charge']} {self.keywords[self.engine]['multiplicity']}\n"\
             f"{self.keywords[self.engine]['coords'].to_string(header=False, index=False)}\n"
@@ -140,16 +128,16 @@
             if self.keywords[self.engine]['mail_user']:
                 self.jobsh += f"#SBATCH --mail-user={self.keywords[self.engine]['mail_user']}\n"
             if self.keywords[self.engine]['exclude']:
                 self.jobsh +=f"#SBATCH --exclude={self.keywords[self.engine]['exclude']}\n"
 
             if self.machine == 'gwdg':
                 self.jobsh += f"#SBATCH -A all\n"\
-                "#SBATCH -C scratch\n"            
-            
+                "#SBATCH -C scratch\n"
+
             self.jobsh +="\n# This block is for the execution of the program\n"
             if self.machine == 'smaug':
                 self.jobsh += "source /home/users/all-jh/opt/miniconda3/etc/profile.d/conda.sh #It is needed to use the conda activate command\n"\
                 "conda activate htmd\n\n"\
                 "# Creating local scratch folder for the user on the computing node.\n"\
                 "MY_TEMP_DIR=\"$(mktemp -d /localdisk/psi4_${SLURM_JOBID}_$(date +%Y-%m-%d-%H-%M-%S)-XXXXXXXXXX)\"\n"
             elif self.machine == 'gwdg':
@@ -176,15 +164,15 @@
             "echo \"SLURM_CPUS_PER_TASK = $SLURM_CPUS_PER_TASK\"\n"\
             "echo \"SLURM_CPUS_ON_NODE = $SLURM_CPUS_ON_NODE\"\n"\
             "echo \"The temp file used was: $MY_TEMP_DIR\"\n\n"\
             f"psi4 -i ${{SLURM_JOB_NAME}}.in -o ${{SLURM_JOB_NAME}}.out -n {self.keywords[self.engine]['ntasks'] * self.keywords[self.engine]['cpus-per-task']} #run command, in, out and number of threads to be used\n\n"\
             "#Deliting the scratch file. Normal delete on normal exit\n"\
             "rm -rf $MY_TEMP_DIR\n\n"\
             "echo \"Job execution end: $(date)\""
- 
+
         elif self.engine == 'orca':
             #!! This is not implemented for GWDG
             self.input += f"#! Computation at {self.keywords[self.engine]['theory']}/{self.keywords[self.engine]['basis']} for {self.keywords[self.engine]['name']}\n"\
             f"%pal nprocs {self.keywords[self.engine]['ntasks']} end\n"
             if self.keywords[self.engine]['freq_type']:
                 self.input += f"%maxcore {self.keywords[self.engine]['maxcore']}\n\n"\
                 f"! {self.keywords[self.engine]['SCF_details']}\n"\
@@ -210,15 +198,15 @@
             f"#SBATCH --nodes {self.keywords[self.engine]['nodes']}\n"\
             f"#SBATCH --nice={self.keywords[self.engine]['nice']}\n"\
             f"#SBATCH --gpus={self.keywords[self.engine]['gpus']}\n"
             if self.keywords[self.engine]['mail_user']:
                 self.jobsh += f"#SBATCH --mail-user={self.keywords[self.engine]['mail_user']}\n"
             if self.keywords[self.engine]['exclude']:
                 self.jobsh +=f"#SBATCH --exclude={self.keywords[self.engine]['exclude']}\n"
-            
+
             self.jobsh +="\n# This block is for the execution of the program\n"\
             "# Setting OPENMPI paths here:\n"\
             "export PATH=\"/data/shared/opt/ORCA/openmpi314/bin:$PATH\"\n"\
             "export LD_LIBRARY_PATH=\"$LD_LIBRARY_PATH:/data/shared/opt/ORCA/openmpi314/lib\"\n\n"\
             "# Here giving the path to the ORCA binaries and giving communication protocol\n"\
             "export PATH=\"/data/shared/opt/ORCA/orca_4_2_1_linux_x86-64_openmpi314:$PATH\"\n"\
             "export LD_LIBRARY_PATH=\"/data/shared/opt/ORCA/orca_4_2_1_linux_x86-64_openmpi314:$LD_LIBRARY_PATH\"\n\n"\
@@ -269,15 +257,15 @@
             else:
                 raise ValueError(f"{attribute} is not a correct attribute. Must be: 'input' or 'jobsh'")
 
 class PARAM:
     def __init__(self, machine = 'smaug', **keywords):
         self.machine = machine
         self.default_partition = {'smaug': 'deflt', 'gwdg': 'medium'}
-        self.default_exclude = {'smaug': "fang[1,11-50]", 'gwdg': None}
+        self.default_exclude = {'smaug': "fang[1,11-55]", 'gwdg': None}
         self.default_ntasks = {'smaug': 12, 'gwdg': 24}
         self.default_keywords = {
                 #Parameters for input
                 'theory': 'MP2',
                 'basis': 'aug-cc-pVTZ',
                 'memory': 14500,
                 'name': 'mol',
@@ -293,23 +281,23 @@
                 #Parameters for jobsh
                 'time': '2-00:00',
                 'ntasks': self.default_ntasks[self.machine],
                 'cpus-per-task': 1,
                 'partition': self.default_partition[self.machine],
                 'nodes': 1,
                 'nice': 0,
-                'gpus': 0,
+                'gpus': 1,
                 'mail_user': None,
                 'exclude': self.default_exclude[self.machine]}
         self.keywords = copy.deepcopy(self.default_keywords)
         for key in keywords:
             self.keywords[key] = keywords[key]
         self.jobsh = ''
         self.parse()
-   
+
     def parse(self):
         self.jobsh += "#!/bin/bash\n"\
         f"#SBATCH --partition {self.keywords['partition']}\n"\
         f"#SBATCH --output myjob_{self.keywords['name']}.out\n"\
         f"#SBATCH --error myjob_{self.keywords['name']}.err\n"\
         f"#SBATCH --ntasks {self.keywords['ntasks']}\n"\
         f"#SBATCH --cpus-per-task {self.keywords['cpus-per-task']}\n"\
@@ -318,19 +306,19 @@
         f"#SBATCH --nodes {self.keywords['nodes']}\n"\
         f"#SBATCH --nice={self.keywords['nice']}\n"\
         f"#SBATCH --gpus={self.keywords['gpus']}\n"
         if self.keywords['mail_user']:
             self.jobsh += f"#SBATCH --mail-user={self.keywords['mail_user']}\n"
         if self.keywords['exclude']:
             self.jobsh +=f"#SBATCH --exclude={self.keywords['exclude']}\n"
-    
+
         if self.machine == 'gwdg':
             self.jobsh += f"#SBATCH -A all\n"\
-            "#SBATCH -C scratch\n"            
-        
+            "#SBATCH -C scratch\n"
+
         self.jobsh +="\n# This block is for the execution of the program\n"
         if self.machine == 'smaug':
             self.jobsh += "source /home/users/all-jh/opt/miniconda3/etc/profile.d/conda.sh #It is needed to use the conda activate command\n"\
             "conda activate htmd\n\n"\
             "# Creating local scratch folder for the user on the computing node.\n"\
             "MY_TEMP_DIR=\"$(mktemp -d /localdisk/psi4_${SLURM_JOBID}_$(date +%Y-%m-%d-%H-%M-%S)-XXXXXXXXXX)\"\n"
         elif self.machine == 'gwdg':
@@ -371,40 +359,40 @@
 
 class CONTINUE:
     def __init__(self, elapsed_paths, engine = 'psi4', machine = 'smaug', **keywords):
         self.elapsed_paths = elapsed_paths
         self.engine = engine
         self.machine = machine
         self.default_partition = {'smaug': 'deflt', 'gwdg': 'medium'}
-        self.default_exclude = {'smaug': "fang[1,11-50]", 'gwdg': None}
+        self.default_exclude = {'smaug': "fang[1,11-55]", 'gwdg': None}
         self.default_ntasks = {'smaug': 12, 'gwdg': 24}
         self.default_keywords = {
             'psi4':{
                 #Parameters for jobsh
                 'time': '2-00:00',
                 'ntasks': self.default_ntasks[self.machine],
                 'cpus-per-task': 1,
                 'partition': self.default_partition[self.machine],
                 'nodes': 1,
                 'nice': 0,
-                'gpus': 0,
+                'gpus': 1,
                 'mail_user': None,
                 'exclude': self.default_exclude[self.machine],
                 },
             'orca':{
                 #Parameters for jobsh
                 'time': '2-00:00',
                 'ntasks': 6,
                 'cpus-per-task': 2,
                 'partition': 'deflt',
                 'nodes': 1,
                 'nice': 0,
-                'gpus': 0,
+                'gpus': 1,
                 'mail_user': None,
-                'exclude': "fang[1,11-50]" #None
+                'exclude': "fang[1,11-55]" #None
                 },
             'gaussian':{
                 'theory': 7,
                 'basis': 2,
                 'memory':4,
                 'name':5,
                 'charge':0,
@@ -415,15 +403,15 @@
                 'freq': False}
         }
         self.keywords = copy.deepcopy(self.default_keywords)
         for key in keywords:
             self.keywords[engine][key] = keywords[key]
         self.jobsh = ''
         self.parse()
-    
+
     def parse(self):
         if self.engine == 'psi4':
 
             self.jobsh += "#!/bin/bash\n"\
             f"#SBATCH --partition {self.keywords[self.engine]['partition']}\n"\
             f"#SBATCH --output myjob_{self.keywords[self.engine]['name']}.out\n"\
             f"#SBATCH --error myjob_{self.keywords[self.engine]['name']}.err\n"\
@@ -437,16 +425,16 @@
             if self.keywords[self.engine]['mail_user']:
                 self.jobsh += f"#SBATCH --mail-user={self.keywords[self.engine]['mail_user']}\n"
             if self.keywords[self.engine]['exclude']:
                 self.jobsh +=f"#SBATCH --exclude={self.keywords[self.engine]['exclude']}\n"
 
             if self.machine == 'gwdg':
                 self.jobsh += f"#SBATCH -A all\n"\
-                "#SBATCH -C scratch\n"            
-            
+                "#SBATCH -C scratch\n"
+
             self.jobsh +="\n# This block is for the execution of the program\n"
             if self.machine == 'smaug':
                 self.jobsh += "source /home/users/all-jh/opt/miniconda3/etc/profile.d/conda.sh #It is needed to use the conda activate command\n"\
                 "conda activate htmd\n\n"\
                 "# Creating local scratch folder for the user on the computing node.\n"\
                 "MY_TEMP_DIR=\"$(mktemp -d /localdisk/psi4_${SLURM_JOBID}_$(date +%Y-%m-%d-%H-%M-%S)-XXXXXXXXXX)\"\n"
             elif self.machine == 'gwdg':
@@ -475,15 +463,15 @@
             "echo \"The temp file used was: $MY_TEMP_DIR\"\n\n"
             for path in self.elapsed_paths:
                 self.jobsh += f'cd {path} && bash run.sh && touch jobqueues.done\n'
 
             self.jobsh += "\n#Deleting the scratch file. Normal delete on normal exit\n"\
             "rm -rf $MY_TEMP_DIR\n\n"\
             "echo \"Job execution end: $(date)\""
- 
+
         elif self.engine == 'orca':
             raise Exception(f'The engine {self.engine} is not coded!')
             # Not implemented
             self.jobsh += "#!/bin/bash\n"\
             f"#SBATCH --partition {self.keywords[self.engine]['partition']}\n"\
             f"#SBATCH --output myjob_{self.keywords[self.engine]['name']}.out\n"\
             f"#SBATCH --error myjob_{self.keywords[self.engine]['name']}.err\n"\
@@ -494,15 +482,15 @@
             f"#SBATCH --nodes {self.keywords[self.engine]['nodes']}\n"\
             f"#SBATCH --nice={self.keywords[self.engine]['nice']}\n"\
             f"#SBATCH --gpus={self.keywords[self.engine]['gpus']}\n"
             if self.keywords[self.engine]['mail_user']:
                 self.jobsh += f"#SBATCH --mail-user={self.keywords[self.engine]['mail_user']}\n"
             if self.keywords[self.engine]['exclude']:
                 self.jobsh +=f"#SBATCH --exclude={self.keywords[self.engine]['exclude']}\n"
-            
+
             self.jobsh +="\n# This block is for the execution of the program\n"\
             "# Setting OPENMPI paths here:\n"\
             "export PATH=\"/data/shared/opt/ORCA/openmpi314/bin:$PATH\"\n"\
             "export LD_LIBRARY_PATH=\"$LD_LIBRARY_PATH:/data/shared/opt/ORCA/openmpi314/lib\"\n\n"\
             "# Here giving the path to the ORCA binaries and giving communication protocol\n"\
             "export PATH=\"/data/shared/opt/ORCA/orca_4_2_1_linux_x86-64_openmpi314:$PATH\"\n"\
             "export LD_LIBRARY_PATH=\"/data/shared/opt/ORCA/orca_4_2_1_linux_x86-64_openmpi314:$LD_LIBRARY_PATH\"\n\n"\
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```


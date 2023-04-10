# Comparing `tmp/richvalues-2.0.0.tar.gz` & `tmp/richvalues-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richvalues-2.0.0.tar", last modified: Tue Mar 21 18:32:52 2023, max compression
+gzip compressed data, was "richvalues-3.0.0.tar", last modified: Mon Apr 10 11:41:50 2023, max compression
```

## Comparing `richvalues-2.0.0.tar` & `richvalues-3.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-03-21 18:32:52.946335 richvalues-2.0.0/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1202 2023-03-21 18:32:52.946335 richvalues-2.0.0/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      703 2023-02-28 18:29:01.000000 richvalues-2.0.0/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)      515 2023-03-21 18:30:42.000000 richvalues-2.0.0/pyproject.toml
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-03-21 18:32:52.946335 richvalues-2.0.0/richvalues/
--rw-rw-r--   0 andres    (1000) andres    (1000)   109055 2023-03-21 18:27:57.000000 richvalues-2.0.0/richvalues/__init__.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-03-21 18:32:52.946335 richvalues-2.0.0/richvalues.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1202 2023-03-21 18:32:52.000000 richvalues-2.0.0/richvalues.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      225 2023-03-21 18:32:52.000000 richvalues-2.0.0/richvalues.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-03-21 18:32:52.000000 richvalues-2.0.0/richvalues.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       30 2023-03-21 18:32:52.000000 richvalues-2.0.0/richvalues.egg-info/requires.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       11 2023-03-21 18:32:52.000000 richvalues-2.0.0/richvalues.egg-info/top_level.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-03-21 18:32:52.946335 richvalues-2.0.0/setup.cfg
--rw-rw-r--   0 andres    (1000) andres    (1000)      753 2023-03-21 18:31:45.000000 richvalues-2.0.0/setup.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-10 11:41:50.361043 richvalues-3.0.0/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-10 11:41:50.361043 richvalues-3.0.0/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      809 2023-04-10 11:41:38.000000 richvalues-3.0.0/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)      515 2023-04-10 11:39:23.000000 richvalues-3.0.0/pyproject.toml
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-10 11:41:50.361043 richvalues-3.0.0/richvalues/
+-rw-rw-r--   0 andres    (1000) andres    (1000)   143953 2023-04-10 11:34:25.000000 richvalues-3.0.0/richvalues/__init__.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-10 11:41:50.361043 richvalues-3.0.0/richvalues.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-10 11:41:50.000000 richvalues-3.0.0/richvalues.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      225 2023-04-10 11:41:50.000000 richvalues-3.0.0/richvalues.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-04-10 11:41:50.000000 richvalues-3.0.0/richvalues.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       30 2023-04-10 11:41:50.000000 richvalues-3.0.0/richvalues.egg-info/requires.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       11 2023-04-10 11:41:50.000000 richvalues-3.0.0/richvalues.egg-info/top_level.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-04-10 11:41:50.361043 richvalues-3.0.0/setup.cfg
+-rw-rw-r--   0 andres    (1000) andres    (1000)      753 2023-04-10 11:39:11.000000 richvalues-3.0.0/setup.py
```

### Comparing `richvalues-2.0.0/PKG-INFO` & `richvalues-3.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 2.0.0
+Version: 3.0.0
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Description: # RichValues
         
-        Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. Moreover, it allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals.
+        Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
         
         The libraries NumPy, Pandas, SciPy and Matplotlib are required. An user guide is available on the GitHub repository: https://github.com/andresmegias/richvalues.
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `richvalues-2.0.0/README.md` & `richvalues-3.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,5 +1,5 @@
 # RichValues
 
-Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. Moreover, it allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals.
+Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
 
 The libraries NumPy, Pandas, SciPy and Matplotlib are required. An user guide is available on the GitHub repository: https://github.com/andresmegias/richvalues.
```

### Comparing `richvalues-2.0.0/pyproject.toml` & `richvalues-3.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "richvalues"
-version = "2.0.0"
+version = "3.0.0"
 description = "Python library for working with uncertainties and upper/lower limits"
 license = {file="LICENSE"}
 authors = [{name="Andrés Megías Toledano"}]
 readme = "README.md"
 dependencies = ["numpy", "pandas", "scipy", "matplotlib"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `richvalues-2.0.0/richvalues/__init__.py` & `richvalues-3.0.0/richvalues/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-RichValues Library
+Rich Values Library
 -------------------
-Version 2.0
+Version 3.0
 
 Copyright (C) 2023 - Andrés Megías Toledano
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
@@ -33,14 +33,17 @@
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
 HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,
 STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
 IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGE.
 """
 
+__version__ = '3.0.0'
+__author__ = 'Andrés Megías Toledano'
+
 import copy
 import math
 import inspect
 import itertools
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
@@ -52,21 +55,26 @@
     'size of samples': int(8e3),
     'number of significant figures': 1,
     'limit for extra significant figure': 2.5,
     'minimum exponent for scientific notation': 4,
     'sigmas to define upper/lower limits': 2.,
     'sigmas to use approximate uncertainty propagation': 20.,
     'use 1-sigma combinations to approximate uncertainty propagation': False,
-    'fraction of the central value for upper/lower limits': 0.1,
+    'fraction of the central value for upper/lower limits': 0.2,
     'number of repetitions to estimate upper/lower limits': 4,
     'decimal exponent to define zero': -90.,
     'decimal exponent to define infinity': 90.,
-    'multiplication symbol for scientific notation in LaTeX': '\\cdot'
+    'multiplication symbol for scientific notation in LaTeX': '\\cdot',
+    'sigmas for overlap': 1.,
+    'sigmas for comparison': 3.
     }
 
+variable_count = 1
+variable_dict = {}
+
 def round_sf(x,
         n=defaultparams['number of significant figures'],
         min_exp=defaultparams['minimum exponent for scientific notation'],
         extra_sf_lim=defaultparams['limit for extra significant figure']):
     """
     Round the number to the given number of significant figures.
 
@@ -94,18 +102,16 @@
     if np.isnan(x):
         y = 'nan'
         return y
     elif np.isinf(x):
         y = str(x)
         return y
     use_exp = True
-    if abs(np.floor(log10(abs(x)))) < min_exp:
+    if abs(np.floor(_log10(abs(x)))) < min_exp:
         use_exp = False
-    if not use_exp and 'e' in str(x):
-        x = float('{:f}'.format(x))
     sign = '-' if x < 0 else ''
     x = abs(x)
     base = '{:e}'.format(x).split('e')[0]
     m = n+1 if round(float(base), n) <= extra_sf_lim else n
     y = str(float('{:.{}g}'.format(x, m)))
     base = '{:e}'.format(float(y)).split('e')[0]
     if round(float(base), n) <= extra_sf_lim:
@@ -123,14 +129,18 @@
     if use_exp:
         y = '{:.{}e}'.format(float(y), max(n-1,0))
         if 'e' in y:
             y, a = y.split('e')
             if float(y) == 1 and not '.' in y:
                 y += '.' + n*'0'
             y = '{}e{}'.format(y, a)
+    else:
+        if 'e' in y:
+            base, exp = y.split('e')
+            y = '0.' + '0'*int(abs(float(exp))-1) + base.replace('.', '')
     y = sign + y
     if x == 0:
         y = '0'
     y = y.replace('e+','e').replace('e00','e0')
     return y
 
 def round_sf_unc(x, dx,
@@ -161,51 +171,51 @@
     y : float
         Rounded value.
     dy : float
         Rounded uncertainty.
     """
     use_exp = True
     if ((float(x) > float(dx)
-          and all(abs(np.floor(log10(abs(np.array([x, dx]))))) < min_exp))
+          and all(abs(np.floor(_log10(abs(np.array([x, dx]))))) < min_exp))
           or (float(x) <= float(dx)
               and float('{:e}'.format(float(dx))
                         .split('e')[0]) > extra_sf_lim
-              and abs(np.floor(log10(abs(float(dx))))) < min_exp)
-          or (float(dx) == 0 and abs(np.floor(log10(abs(x)))) < min_exp)
+              and abs(np.floor(_log10(abs(float(dx))))) < min_exp)
+          or (float(dx) == 0 and abs(np.floor(_log10(abs(x)))) < min_exp)
           or np.isinf(min_exp)):
         use_exp = False
     x, dx = float(x), float(dx)
     sign = '' if x >= 0 else '-'
     if x < 0:
         x = abs(x)
     if np.isinf(x):
         y = 'inf'
-        dy = 'nan'
+        dy = '0'
     elif np.isnan(x):
         y = 'nan'
         dy = 'nan'
     elif dx > 0:
         dy = round_sf(dx, n, min_exp, extra_sf_lim)
         if not use_exp:
             m = len(dy.split('.')[1]) if '.' in dy else 0
             y = '{:.{}f}'.format(x, m)
         else:
             base_y, exp_y = '{:e}'.format(x).split('e')
             base_dy, exp_dy = '{:e}'.format(dx).split('e')
-            m = int(exp_y) - int(exp_dy)
-            o = 1 if float(base_dy) < extra_sf_lim else 0
-            base_y = round_sf(float(base_y) * 10**m, n+m+o, min_exp=np.inf,
+            m = int(exp_dy) - int(exp_y)
+            o = 1 if float(base_y) < extra_sf_lim else 0
+            base_y = round_sf(base_y, n, min_exp=np.inf,
                               extra_sf_lim=extra_sf_lim)
-            base_dy = round_sf(base_dy, n, min_exp=np.inf,
+            base_dy = round_sf(float(base_dy) * 10**m, n+m+o, min_exp=np.inf,
                                extra_sf_lim=extra_sf_lim)
             m = len(base_dy.split('.')[1]) if '.' in base_dy else 0
             base_y = '{:.{}f}'.format(float(base_y), m)
             base_dy = '{:.{}f}'.format(float(base_dy), m)
-            y = '{}e{}'.format(base_y, exp_dy)
-            dy = '{}e{}'.format(base_dy, exp_dy)
+            y = '{}e{}'.format(base_y, exp_y)
+            dy = '{}e{}'.format(base_dy, exp_y)
     elif dx == 0:
         y = round_sf(x, n+1, min_exp, extra_sf_lim)
         dy = '0e0'
     else:
         y = 'nan'
         dy = 'nan'
     if float(y) != 0 and y != 'nan':
@@ -254,16 +264,16 @@
         Rounded value.
     dy : list (float)
         Rounded uncertainties.
     """
     dx1, dx2 = dx
     y1, dy1 = round_sf_unc(x, dx1)
     y2, dy2 = round_sf_unc(x, dx2)
-    num_dec_1 = len(y1.split('e')[0].replace('.',''))
-    num_dec_2 = len(y2.split('e')[0].replace('.',''))
+    num_dec_1 = len(y1.split('e')[0].split('.')[1]) if '.' in y1 else 0
+    num_dec_2 = len(y2.split('e')[0].split('.')[1]) if '.' in y2 else 0
     if num_dec_2 > num_dec_1:
         diff = num_dec_2 - num_dec_1
         y1, dy1 = round_sf_unc(x, dx1, n+diff, min_exp, extra_sf_lim)
         y2, dy2 = round_sf_unc(x, dx2, n, min_exp, extra_sf_lim)
     else:
         diff = num_dec_1 - num_dec_2
         y1, dy1 = round_sf_unc(x, dx1, n, min_exp, extra_sf_lim)
@@ -297,29 +307,36 @@
             If True, it means that the rich value is actually a constant range
             of values defined by the main value and the uncertainties.
         domain : list (float), optional
             The domain of the rich value, that is, the minimum and maximum
             values that it can take.
         """
         
+        acronyms = ['main_value', 'uncertainty',
+                    'is_lower_limit', 'is_upper_limit', 'is_finite_range']
+        for kwarg in kwargs:
+            if kwarg not in acronyms:
+                raise TypeError("RichValue() got an unexpected keyword argument"
+                                + " '{}'".format(kwarg))
         if 'main_value' in kwargs:
             main = kwargs['main_value']
+        if main is None:
+            raise TypeError("RichValue() missing required argument 'main'"
+                            + " (pos 1)")
         if 'uncertainty' in kwargs:
             unc = kwargs['uncertainty']
         if 'is_lower_limit' in kwargs:
             is_lolim = kwargs['is_lower_limit']
         if 'is_upper_limit' in kwargs:
             is_uplim = kwargs['is_upper_limit']
         if 'is_finite_range' in kwargs:
             is_range = kwargs['is_finite_range']
         
         if domain is None:
             domain = defaultparams['domain']
-        if domain[0] == domain[1]:
-            raise Exception('Invalid domain {}.'.format(domain))
         unc_or = copy.copy(unc)
         main_or = copy.copy(main)
         
         if type(main) in [list, tuple]:
             is_lolim, is_uplim, is_range = False, False, False
             main = [float(main[0]), float(main[1])]
             if main_or[0] <= domain[0] and main_or[1] < domain[1]:
@@ -344,27 +361,30 @@
                 main = (main[0] + main[1]) / 2
         else:
             main = float(main)
         if not hasattr(unc, '__iter__'):
             unc = [unc, unc]
         if any(np.isinf(unc)):
             main = np.nan
-            unc = np.nan_to_num(unc, nan=0., posinf=0.)
-            
+            unc = [0, 0]
+        unc = np.nan_to_num(unc, nan=0)
+        if np.isfinite(main) and not domain[0] <= main <= domain[1]:
+            raise Exception('Invalid main value {} for domain {}.'
+                            .format(main, domain))
         unc = list(unc)
         unc = [float(unc[0]), float(unc[1])]
         unc[0] = abs(unc[0])
         if not (is_lolim or is_uplim) and unc[1] < 0:
             unc_text = ('Superior uncertainty' if hasattr(unc_or, '__iter__')
                         else 'Uncertainty')
             raise Exception('{} cannot be negative.'.format(unc_text))
+            
         with np.errstate(divide='ignore', invalid='ignore'):
             ampl = [main - domain[0], domain[1] - main]
-            rel_ampl = list(np.array(ampl) / np.array(unc))
-            
+            rel_ampl = list(np.array(ampl) / np.array(unc))     
         if not (is_lolim or is_uplim):
             is_range_domain = False
             if min(rel_ampl) <= 1.:
                 sigmas = defaultparams['sigmas to define upper/lower limits']
                 x1 = max(main - unc[0], domain[0])
                 x2 = min(main + unc[1], domain[1])
                 if x1 == domain[0] and x2 != domain[1]:
@@ -386,93 +406,121 @@
                     is_range = True
             if min(rel_ampl) <= 1. and is_range_domain:
                 main = (domain[0] + domain[1]) / 2
                 unc = [(domain[1] - domain[0]) / 2] * 2
         
         if (is_lolim or is_uplim) and np.isinf(np.diff(domain)):
             is_range = False
+        
+        global variable_count
+        expression = 'x{}'.format(variable_count)
+        variable_count += 1
                 
         self.main = main
         self.unc = unc
         self.is_lolim = is_lolim
         self.is_uplim = is_uplim
         self.is_range = is_range
         self.domain = domain
         self.num_sf = defaultparams['number of significant figures']
         self.min_exp = defaultparams['minimum exponent for scientific notation']
-            
+        self.vars = [expression]
+        self.expression = expression
+        
+        global variable_dict
+        variable_dict[expression] = self
+          
+    @property
     def is_lim(self):
         """Upper/lower limit"""
         islim = self.is_lolim or self.is_uplim
         return islim
-    
+    @property
     def is_interv(self):
         """Upper/lower limit or constant range of values"""
-        isinterv = self.is_range or self.is_lim()
+        isinterv = self.is_range or self.is_lim
         return isinterv
-    
+    @property
     def is_centr(self):
         """Centered value"""
-        iscentr = not self.is_interv()
+        iscentr = not self.is_interv
         return iscentr
-        
+    @property    
     def center(self):
         """Central value"""
-        cent = self.main if self.is_centr() else np.nan
-        return cent
-    
+        cent = self.main if self.is_centr else np.nan
+        return cent  
+    @property
     def unc_eb(self):
         """Uncertainties with shape (2,1)"""
         unceb = [[self.unc[0]], [self.unc[1]]]
         return unceb    
-    
+    @property
     def rel_unc(self):
         """Relative uncertainties"""
         m, s = self.main, self.unc
         with np.errstate(divide='ignore', invalid='ignore'):
             runc = list(np.array(s) / abs(m))
         return runc
-    
+    @property
     def signal_noise(self):
         """Signal-to-noise ratios (S/N)"""
         m, s = self.main, self.unc
         with np.errstate(divide='ignore', invalid='ignore'):
             s_n = list(np.nan_to_num(abs(m) / np.array(s),
-                       nan=0, posinf=np.nan))
+                       nan=0, posinf=np.inf))
         return s_n
-        
+    @property    
     def ampl(self):
         """Amplitudes"""
         m, b = self.main, self.domain
         a = [m - b[0], b[1] - m]
         return a
-        
+    @property        
     def rel_ampl(self):
         """Relative amplitudes"""
-        s, a = self.unc, self.ampl()
+        s, a = self.unc, self.ampl
         with np.errstate(divide='ignore'):
             a_s = list(np.array(a) / np.array(s))
         return a_s
-    
+    @property
     def norm_unc(self):
         """Normalized uncertainties"""
-        s, a = self.unc, self.ampl()
+        s, a = self.unc, self.ampl
         s_a = list(np.array(s) / np.array(a))
         return s_a
-    
+    @property
     def prop_score(self):
         """Minimum of the signals-to-noise and the relative amplitudes."""
-        s_n = self.signal_noise()
-        a_s = self.rel_ampl()
+        s_n = self.signal_noise
+        a_s = self.rel_ampl
         pf = np.min([s_n, a_s])
         return pf
+    @property
+    def is_nan(self):
+        """Not a number value."""
+        isnan = (True if np.isnan(self.main) or any(np.isinf(self.unc))
+                 else False)
+        return isnan
+    @property
+    def is_inf(self):
+        """Infinite value."""
+        isinf = (True if np.isinf(self.main) and not any(np.isinf(self.unc))
+                 else False)
+        return isinf
+    @property
+    def is_finite(self):
+        """Finite value."""
+        isfinite = (True if np.isfinite(self.main)
+                    and all(np.isfinite(self.unc)) else False)
+        return isfinite
     
-    def interval(self, sigmas=4.):
+    def interval(self, sigmas=3.):
         """Interval of possible values of the rich value."""
-        if not self.is_interv():
+        if not self.is_interv:
             interv = [max(self.domain[0], self.main - sigmas*self.unc[0]),
                       min(self.domain[1], self.main + sigmas*self.unc[1])]
         else:
             if self.is_uplim and not self.is_lolim:
                 interv = [self.domain[0], self.main]
             elif self.is_lolim and not self.is_uplim:
                 interv = [self.main, self.domain[1]]
@@ -495,30 +543,29 @@
         min_exp = self.min_exp
         extra_sf_lim = defaultparams['limit for extra significant figure']
         x = copy.copy(main)
         dx = copy.copy(unc)
         n = copy.copy(self.num_sf)
         use_exp = True
         if ((float(x) > float(max(dx))
-             and abs(np.floor(log10(abs(float(x))))) < min_exp)
+             and abs(np.floor(_log10(abs(float(x))))) < min_exp)
              or (float(x) <= float(max(dx))
                  and float('{:e}'.format(max(dx))
                            .split('e')[0]) > extra_sf_lim
-                 and any(abs(np.floor(log10(abs(np.array(dx)))))
+                 and any(abs(np.floor(_log10(abs(np.array(dx)))))
                          < min_exp))
-             or (dx == [0,0] and abs(np.floor(log10(abs(x)))) < min_exp)
-             or (self.is_lim() and abs(np.floor(log10(abs(float(x))))) < min_exp)
+             or (dx == [0,0] and abs(np.floor(_log10(abs(x)))) < min_exp)
+             or (self.is_lim and abs(np.floor(_log10(abs(float(x))))) < min_exp)
              or np.isinf(min_exp)):
             use_exp = False
         if not is_range and not np.isnan(main):
             x = main
             dx1, dx2 = unc
-            if not self.is_lim():
+            if not self.is_lim:
                 y, (dy1, dy2) = round_sf_uncs(x, [dx1, dx2], n, min_exp)
-                y, dy1, dy2 = str(y), str(dy1), str(dy2)
                 if 'e' in y:
                     y, a = y.split('e')
                     a = int(a)
                 else:
                     a = 0
                 if 'e' in dy1:
                     dy1, _ = dy1.split('e')
@@ -560,36 +607,44 @@
         else:
             x1 = RichValue(main - unc[0], domain=domain)
             x2 = RichValue(main + unc[1], domain=domain)
             x1.min_exp = min_exp
             x2.min_exp = min_exp
             text = '{} -- {}'.format(x1, x2)
         return text
+        
+    def __repr__(self):
+        return self._format_as_rich_value()
     
-    def _format_as_latex_value(self, dollars=True, mult_symbol='\\cdot'):
+    def __str__(self):
+        return self._format_as_rich_value()
+   
+    def latex(self, dollars=True, mult_symbol=defaultparams['multiplication '
+                                 + 'symbol for scientific notation in LaTeX']):
+        """Display in LaTeX format"""
         main = copy.copy(self.main)
         unc = copy.copy(self.unc)
         domain = self.domain
         is_lolim = self.is_lolim
         is_uplim = self.is_uplim
         min_exp = self.min_exp
         is_range = self.is_range
         extra_sf_lim = defaultparams['limit for extra significant figure']
         use_exp = True
         x = copy.copy(main)
         dx = copy.copy(unc)
         n = copy.copy(self.num_sf)
         if ((float(x) > float(max(dx))
-             and abs(np.floor(log10(abs(float(x))))) < min_exp)
+             and abs(np.floor(_log10(abs(float(x))))) < min_exp)
              or (float(x) <= float(max(dx))
                  and float('{:e}'.format(max(dx))
                            .split('e')[0]) > extra_sf_lim
-                 and any(abs(np.floor(log10(abs(np.array(dx))))) < min_exp))
-             or (dx == [0,0] and abs(np.floor(log10(abs(x)))) < min_exp)
-             or (self.is_lim() and abs(np.floor(log10(abs(float(x))))) < min_exp)
+                 and any(abs(np.floor(_log10(abs(np.array(dx))))) < min_exp))
+             or (dx == [0,0] and abs(np.floor(_log10(abs(x)))) < min_exp)
+             or (self.is_lim and abs(np.floor(_log10(abs(float(x))))) < min_exp)
              or np.isinf(min_exp)):
             use_exp = False
         text = ''
         non_numerics = ['nan', 'NaN', 'None', 'inf', '-inf']
         is_numeric = False if str(main) in non_numerics else True
         if is_numeric:
             if not is_range:
@@ -673,225 +728,367 @@
                                          x2.latex(dollars, mult_symbol))
         else:
             text = (str(main).replace('NaN','nan').replace('nan','...')
                     .replace('inf','$\infty$'))
         if not dollars:
             text = text.replace('$','')
         return text
-        
-    def __repr__(self):
-        return self._format_as_rich_value()
-    
-    def __str__(self):
-        return self._format_as_rich_value()
    
-    def latex(self, dollars=True, mult_symbol=defaultparams['multiplication '
-                                 + 'symbol for scientific notation in LaTeX']):
-        """Display in LaTeX format"""
-        return self._format_as_latex_value(dollars, mult_symbol) 
+    def __abs__(self):
+        main = copy.copy(self.main)
+        unc = copy.copy(self.unc)
+        domain = copy.copy(self.domain)
+        if not self.is_interv:
+            x = abs(main)
+        else:
+            x1, x2 = self.interval()
+            x1, x2 = abs(x1), abs(x2)
+            x = [min(x1, x2), max(x1, x2)]
+        dx = unc
+        domain = [abs(domain[0]), abs(domain[1])]
+        domain = [min(domain), max(domain)]
+        if np.isinf(domain[0]):
+            domain[0] = 0
+        new_rval = RichValue(x, dx, domain=domain)
+        new_rval.vars = self.vars
+        new_rval.expression = 'abs({})'.format(self.expression)
+        return new_rval
    
     def __neg__(self):
         main = copy.copy(self.main)
         unc = copy.copy(self.unc)
         domain = copy.copy(self.domain)
-        if not self.is_interv():
+        if not self.is_interv:
             x = -main
         else:
             x1, x2 = self.interval()
             x = [-x2, -x1]
         dx = unc
         domain = [-domain[0], -domain[1]]
         domain = [min(domain), max(domain)]
-        new_rich_value = RichValue(x, dx, domain=domain)
-        return new_rich_value
+        new_rval = RichValue(x, dx, domain=domain)
+        new_rval.vars = self.vars
+        new_rval.expression = '-({})'.format(self.expression)
+        return new_rval
     
     def __add__(self, other):
-        other_ = (other.main if type(other) is RichValue
-                  and other.unc==[0,0] else other)
-        if type(other_) is RichValue:
-            new_rich_value = add_two_rich_values(self, other_)
-        else:
-            if other_ != 0:
-                x = self.main + other_
-                dx = copy.copy(self.unc)
-                new_rich_value = RichValue(x, dx, self.is_lolim, self.is_uplim,
-                                           self.is_range, self.domain)
+        if type(other) in (np.ndarray, RichArray):
+            return other + self
+        elif type(other) is RichValue:
+            other_vars = other.vars
+            other_expression = other.expression
+        else:
+            other_vars = []
+            other_expression = str(other)
+        expression = '({})+({})'.format(self.expression, other_expression)
+        variables = set(self.vars + other_vars)
+        common_vars = set(self.vars) & set(other_vars)
+        if len(common_vars) == 0:
+            other_ = (other.main if type(other) is RichValue
+                      and other.unc==[0,0] else other)
+            if type(other_) is RichValue:
+                new_rval = add_two_rich_values(self, other_)
             else:
-                new_rich_value = RichValue(0, domain=self.domain)
-        return new_rich_value
+                if other_ != 0:
+                    x = self.main + other_
+                    dx = copy.copy(self.unc)
+                    new_rval = RichValue(x, dx, self.is_lolim, self.is_uplim,
+                                         self.is_range, self.domain)
+                else:
+                    new_rval = RichValue(0, domain=self.domain)
+        else:
+            vars_str = ','.join(variables)
+            function = eval('lambda {}: {}'.format(vars_str, expression))
+            args = [variable_dict[var] for var in variables]
+            new_rval = function_with_rich_values(function, args)
+        new_rval.vars = list(variables)
+        new_rval.expression = expression
+        return new_rval
     
     def __radd__(self, other):
         return self + other
     
     def __sub__(self, other):
         return self + (-other)
     
     def __rsub__(self, other):
         return -(self - other)
     
     def __mul__(self, other):
-        other_ = (other.main if type(other) is RichValue
-                  and other.unc==[0,0] else other)
-        if type(other_) is RichValue:
-            new_rich_value = multiply_two_rich_values(self, other_)
-        else:
-            if other_ != 0:
-                x = self.main * other_
-                dx = np.array(self.unc) * other_
-                domain = np.array(self.domain) * other_
-                domain = [min(domain), max(domain)]
-                new_rich_value = RichValue(x, dx, self.is_lolim, self.is_uplim,
-                                           self.is_range, domain)
-                new_rich_value.num_sf = self.num_sf
-                new_rich_value.min_exp = self.min_exp
+        if type(other) in (np.ndarray, RichArray):
+            return other * self
+        elif type(other) is RichValue:
+            other_vars = other.vars
+            other_expression = other.expression
+        else:
+            other_vars = []
+            other_expression = str(other)
+        expression = '({})*({})'.format(self.expression, other_expression)
+        variables = set(self.vars + other_vars)
+        common_vars = set(self.vars) & set(other_vars)
+        if len(common_vars) == 0:
+            other_ = (other.main if type(other) is RichValue
+                      and other.unc==[0,0] else other)
+            if type(other_) is RichValue:
+                new_rval = multiply_two_rich_values(self, other_)
             else:
-                new_rich_value = RichValue(0, domain=self.domain)
-        return new_rich_value
+                if other_ != 0:
+                    x = self.main * other_
+                    dx = np.array(self.unc) * other_
+                    if type(other_) is not RichValue:
+                        other_ = RichValue(other_)
+                    domain_combs = [self.domain[i1] * other_.domain[i2]
+                                    for i1,i2 in zip([0,0,1,1],[0,1,0,1])]
+                    domain1, domain2 = min(domain_combs), max(domain_combs)
+                    if not np.isfinite(domain1):
+                        domain1 = -np.inf
+                    if not np.isfinite(domain2):
+                        domain2 = np.inf
+                    domain = [domain1, domain2]
+                    new_rval = RichValue(x, dx, self.is_lolim, self.is_uplim,
+                                         self.is_range, domain)
+                    new_rval.num_sf = self.num_sf
+                    new_rval.min_exp = self.min_exp
+                else:
+                    new_rval = RichValue(0, domain=self.domain)
+        else:
+            vars_str = ','.join(variables)
+            function = eval('lambda {}: {}'.format(vars_str, expression))
+            args = [variable_dict[var] for var in variables]
+            new_rval = function_with_rich_values(function, args)
+        new_rval.vars = list(variables)
+        new_rval.expression = expression
+        return new_rval
     
     def __rmul__(self, other):
         return self * other
     
     def __truediv__(self, other):
-        other_ = (other.main if type(other) is RichValue
-                  and other.unc==[0,0] else other)
-        if type(other_) is RichValue:
-            new_rich_value = divide_two_rich_values(self, other_)
-        else:
-            if other_ != 0:
-                with np.errstate(divide='ignore', invalid='ignore'):
-                    x = self.main / other_
-                    dx = np.array(self.unc) / other_
-                    domain = np.array(self.domain) / other_
-                    domain = [min(domain), max(domain)]
-                new_rich_value = RichValue(x, dx, self.is_lolim, self.is_uplim,
-                                           self.is_range, domain)
-                new_rich_value.num_sf = self.num_sf
-                new_rich_value.min_exp = self.min_exp
+        if type(other) is RichValue:
+            other_vars = other.vars
+            other_expression = other.expression
+        else:
+            other_vars = []
+            other_expression = str(other)
+        expression = '({})/({})'.format(self.expression, other_expression)
+        variables = set(self.vars + other_vars)
+        common_vars = set(self.vars) & set(other_vars)
+        if len(common_vars) == 0:
+            other_ = (other.main if type(other) is RichValue
+                      and other.unc==[0,0] else other)
+            if type(other_) is RichValue:
+                new_rval = divide_two_rich_values(self, other_)
             else:
-                new_rich_value = RichValue(np.nan, domain=self.domain)
-        return new_rich_value
+                if other_ != 0:
+                    with np.errstate(divide='ignore', invalid='ignore'):
+                        x = self.main / other_
+                        dx = np.array(self.unc) / other_
+                        if type(other_) is not RichValue:
+                            other_ = RichValue(other_)
+                        domain_combs = [self.domain[i1] * other_.domain[i2]
+                                        for i1,i2 in zip([0,0,1,1],[0,1,0,1])]
+                        domain1, domain2 = min(domain_combs), max(domain_combs)
+                        if not np.isfinite(domain1):
+                            domain1 = -np.inf
+                        if not np.isfinite(domain2):
+                            domain2 = np.inf
+                        domain = [domain1, domain2]
+                    new_rval = RichValue(x, dx, self.is_lolim, self.is_uplim,
+                                         self.is_range, domain)
+                    new_rval.num_sf = self.num_sf
+                    new_rval.min_exp = self.min_exp
+                else:
+                    new_rval = RichValue(np.nan, domain=self.domain)
+        else:
+            vars_str = ','.join(variables)
+            function = eval('lambda {}: {}'.format(vars_str, expression))
+            args = [variable_dict[var] for var in variables]
+            new_rval = function_with_rich_values(function, args)
+        new_rval.vars = list(variables)
+        new_rval.expression = expression
+        return new_rval
 
     def __rtruediv__(self, other):
-        other_ = (other.main if type(other) is RichValue
-                  and other.unc==[0,0] else other)
-        if type(other_) is RichValue:
-            new_rich_value = divide_two_rich_values(other_, self)
-        else:
-            if other_ != 0:
-                with np.errstate(divide='ignore'):
-                    x = other_ / self.main
-                    dx = x * np.array(self.unc) / self.main
-                    domain = other_ / np.array(self.domain)
-                    domain = [min(domain), max(domain)]
-                new_rich_value = RichValue(x, dx, self.is_lolim, self.is_uplim,
-                                           self.is_range, domain)
-                new_rich_value.num_sf = self.num_sf
-                new_rich_value.min_exp = self.min_exp
+        if type(other) is RichValue:
+            other_vars = other.vars
+            other_expression = other.expression
+        else:
+            other_vars = []
+            other_expression = str(other)
+        expression = '({})/({})'.format(other_expression, self.expression)
+        variables = set(self.vars + other_vars)
+        common_vars = set(self.vars) & set(other_vars)
+        if len(common_vars) == 0:
+            other_ = (other.main if type(other) is RichValue
+                      and other.unc==[0,0] else other)
+            if type(other_) is RichValue:
+                new_rval = divide_two_rich_values(other_, self)
             else:
-                new_rich_value = RichValue(0, domain=self.domain)
-        return new_rich_value
+                if other_ != 0:
+                    with np.errstate(divide='ignore'):
+                        x = other_ / self.main
+                        dx = x * np.array(self.unc) / self.main
+                        if type(other_) is not RichValue:
+                            other_ = RichValue(other_)
+                        domain_combs = [self.domain[i1] * other_.domain[i2]
+                                        for i1,i2 in zip([0,0,1,1],[0,1,0,1])]
+                        domain1, domain2 = min(domain_combs), max(domain_combs)
+                        if not np.isfinite(domain1):
+                            domain1 = -np.inf
+                        if not np.isfinite(domain2):
+                            domain2 = np.inf
+                        domain = [domain1, domain2]
+                    new_rval = RichValue(x, dx, self.is_lolim, self.is_uplim,
+                                         self.is_range, domain)
+                    new_rval.num_sf = self.num_sf
+                    new_rval.min_exp = self.min_exp
+                else:
+                    new_rval = RichValue(0, domain=self.domain)
+        else:
+            vars_str = ','.join(variables)
+            function = eval('lambda {}: {}'.format(vars_str, expression))
+            args = [variable_dict[var] for var in variables]
+            new_rval = function_with_rich_values(function, args)
+        new_rval.vars = list(variables)
+        new_rval.expression = expression
+        return new_rval
     
     def __pow__(self, other):
-        sigmas = defaultparams['sigmas to use approximate '
-                               + 'uncertainty propagation']
-        main = copy.copy(self.main)
-        unc = copy.copy(self.unc)
-        domain = copy.copy(self.domain)
-        if ((domain[0] >= 0 and (type(other) is RichValue
-                                 or self.prop_score() < sigmas))
-            or (domain[0] < 0 and type(other) is not RichValue)
-                and int(other) == other and self.prop_score() < sigmas):
-            other_ = (other if type(other) is RichValue
-                      else RichValue(other))
-            if main != 0:
-                if type(other) is not RichValue and other%2 == 0:
-                    domain = [0, np.inf]
-                else:
-                    domain = self.domain
-                new_rich_value = function_with_rich_values(lambda a,b: a**b,
+        if type(other) is RichValue:
+            other_vars = other.vars
+            other_expression = other.expression
+        else:
+            other_vars = []
+            other_expression = str(other)
+        expression = '({})**({})'.format(self.expression, other_expression)
+        variables = set(self.vars + other_vars)
+        common_vars = set(self.vars) & set(other_vars)
+        if len(common_vars) == 0:
+            sigmas = defaultparams['sigmas to use approximate '
+                                   + 'uncertainty propagation']
+            main = copy.copy(self.main)
+            unc = copy.copy(self.unc)
+            domain = copy.copy(self.domain)
+            if ((domain[0] >= 0 and (type(other) is RichValue
+                                     or self.prop_score < sigmas))
+                or (domain[0] < 0 and type(other) is not RichValue)
+                    and int(other) == other and self.prop_score < sigmas):
+                other_ = (other if type(other) is RichValue
+                          else RichValue(other))
+                if main != 0:
+                    if type(other) is not RichValue and other%2 == 0:
+                        domain = [0, np.inf]
+                    else:
+                        domain = self.domain
+                    new_rval = function_with_rich_values(lambda a,b: a**b,
                                                 [self, other_], domain=domain)
-            else:
-                new_rich_value = RichValue(0)
-                new_rich_value.num_sf = self.num_sf
-        elif (type(other) is not RichValue and self.prop_score() > sigmas):
-            x = main ** other
-            dx = abs(x * other * np.array(unc) / main)
-            if domain != [-np.inf, np.inf]:
-                if domain[0] != 0 or (domain[0] == 0 and other>0):
-                    x1 = domain[0] ** other
                 else:
-                    x1 = np.inf
-                if domain[1] != 0 or (domain[0] == 0 and other>0):
-                    x2 = domain[1] ** other
+                    new_rval = RichValue(0)
+                    new_rval.num_sf = self.num_sf
+            elif (type(other) is not RichValue and self.prop_score > sigmas):
+                x = main ** other
+                dx = abs(x * other * np.array(unc) / main)
+                if domain != [-np.inf, np.inf]:
+                    if domain[0] != 0 or (domain[0] == 0 and other>0):
+                        x1 = domain[0] ** other
+                    else:
+                        x1 = np.inf
+                    if domain[1] != 0 or (domain[0] == 0 and other>0):
+                        x2 = domain[1] ** other
+                    else:
+                        x2 = np.inf
+                    domain = [x1, x2]
+                    domain = [min(domain), max(domain)]
                 else:
-                    x2 = np.inf
-                domain = [x1, x2]
-                domain = [min(domain), max(domain)]
+                    domain = [-np.inf, np.inf]
+                new_rval = RichValue(x, dx, self.is_lolim, self.is_uplim,
+                                     domain=domain)
+                new_rval.num_sf = self.num_sf
             else:
-                domain = [-np.inf, np.inf]
-            new_rich_value = RichValue(x, dx, self.is_lolim, self.is_uplim,
-                                       domain=domain)
-            new_rich_value.num_sf = self.num_sf
-        else:
-            if (type(other) is RichValue and other.domain[0] < 0
-                    and not np.isinf(other.main)):
-                print('Warning: Domain of exponent should be positive.')
-            new_rich_value = RichValue(np.nan)
-        return new_rich_value
+                if (type(other) is RichValue and other.domain[0] < 0
+                        and not np.isinf(other.main)):
+                    print('Warning: Domain of exponent should be positive.')
+                new_rval = RichValue(np.nan)
+        else:
+            vars_str = ','.join(variables)
+            function = eval('lambda {}: {}'.format(vars_str, expression))
+            args = [variable_dict[var] for var in variables]
+            new_rval = function_with_rich_values(function, args)
+        new_rval.vars = list(variables)
+        new_rval.expression = expression
+        return new_rval
     
     def __rpow__(self, other):
-        if other > 0:
-            domain = [0, np.inf]
-        elif other < 0:
-            domain = [-np.inf, 0]
-        else:
-            domain = [-np.inf, np.inf]
-        other_ = RichValue(other, domain=domain)
+        if type(other) in (int, float):
+            if other > 0:
+                domain = [0, np.inf]
+            elif other < 0:
+                domain = [-np.inf, 0]
+            else:
+                domain = [-np.inf, np.inf]
+            other_ = RichValue(other, domain=domain)
+            other_.vars = []
+            other_.expression = str(other)
         other_.num_sf = self.num_sf
-        new_rich_value = other_ ** self
-        return new_rich_value
+        new_rval = other_ ** self
+        return new_rval
+    
+    def __gt__(self, other):
+        return greater(self, other)
+    
+    def __lt__(self, other):
+        return less(self, other)
+
+    def __eq__(self, other):
+        return equiv(self, other)
+    
+    def __ge__(self, other):
+        return greater_equiv(self, other)
+    
+    def __le__(self, other):
+        return less_equiv(self, other)
     
     def pdf(self, x):
-        """Probability density function corresponding to the rich value"""
+        """Probability density function corresponding to the rich value."""
         main = copy.copy(self.main)
         unc = copy.copy(self.unc)
         domain = copy.copy(self.domain)
         x = np.array(x)
         y = np.zeros(len(x))
-        if unc == [0, 0] and not self.is_interv():    
+        if unc == [0, 0] and not self.is_interv:    
             ind = np.argmin(abs(x - main))
             if hasattr(ind, '__iter__'):
                 ind = ind[0]
             y[ind] = 1.
         else:
-            if not self.is_interv():
+            if not self.is_interv:
                 y = general_pdf(x, main, unc, domain)
             elif self.is_lolim and not self.is_uplim:
-                y[x > main] = 0.1
+                y[x > main] = 1e-3
             elif self.is_uplim and not self.is_lolim:
-                y[x < main] = 0.1
+                y[x < main] = 1e-3
             elif self.is_range:
-                x1, x2 = main - unc, main + unc
+                x1, x2 = main - unc[0], main + unc[1]
                 y[(x > x1) & (x < x2)] = 1 / (x2 - x1)
         return y
     
     def sample(self, len_sample=1):
         """Sample of the distribution corresponding to the rich value"""
         main = copy.copy(self.main)
         unc = copy.copy(self.unc)
         domain = copy.copy(self.domain)
         N = int(len_sample)
         is_finite_interv = (self.is_range
                             or self.is_uplim and np.isfinite(domain[0])
                             or self.is_lolim and np.isfinite(domain[1]))
-        if list(unc) == [0, 0] and not self.is_interv():
+        if list(unc) == [0, 0] and not self.is_interv:
             x = main * np.ones(N)
         else:
             if not is_finite_interv and list(self.unc) != [np.inf, np.inf]:
-                if not self.is_lim():
+                if not self.is_lim:
                     x = general_distribution(main, unc, domain, N)
                 else:
                     x1, x2 = self.interval()    
                     x = loguniform_distribution(x1, x2, N)
             elif not is_finite_interv and list(self.unc) == [np.inf, np.inf]:
                 x = loguniform_distribution(-np.inf, np.inf, N)
             else:
@@ -907,18 +1104,17 @@
                     np.random.shuffle(x)
         if N == 1:
             x = x[0]
         return x
     
     def function(self, function, **kwargs):
         """Apply a function to the rich value"""
-        new_rich_value = function_with_rich_values(function, self, **kwargs)
-        return new_rich_value
+        return function_with_rich_values(function, self, **kwargs)
     
-    # Instance variable abbreviations.
+    # Instance variable acronyms.
     
     @property
     def main_value(self): return self.main
     @main_value.setter
     def main_value(self, x): self.main = x
     
     @property
@@ -947,24 +1143,33 @@
     def number_of_scientific_figures(self, x): self.num_sf = x 
     
     @property
     def minimum_exponent_for_scientific_notation(self): return self.min_exp
     @minimum_exponent_for_scientific_notation.setter
     def minimum_exponent_for_scientific_notation(self, x): self.min_exp = x
     
-    # Method abbreviations.
+    @property
+    def variables(self): return self.variable
+    @variables.setter
+    def variables(self, x): self.vars = x
+    
+    # Attribute acronyms.
     is_limit = is_lim
     is_interval = is_interv
     is_centered_value = is_centr
     relative_uncertainty = rel_unc
     signal_to_noise = signal_noise
     amplitude = ampl
     relative_amplitude = rel_ampl
     normalized_uncertainty = norm_unc
     propagation_score = prop_score
+    is_not_a_number = is_nan
+    is_infinite = is_inf
+    # Method acronyms.
+    probability_density_function = pdf
     set_limits_factor = set_lims_factor
 
 class RichArray(np.ndarray):
     """
     A class to store values with uncertainties or upper/lower limits.
     """
     
@@ -989,16 +1194,25 @@
             actually a constant range of values defined by the main value and
             the uncertainties. The default is all False.
         domains : list / array (float), optional
             Array of domains for each entry of the rich value.
             The default is [-np.inf, np.inf].
         """
         
+        acronyms = ['main_values', 'uncertainties', 'are_lower_limits',
+                                'are_upper_limits', 'are_finite_ranges']
+        for kwarg in kwargs:
+            if kwarg not in acronyms:
+                raise TypeError("RichArray() got an unexpected keyword argument"
+                                + " '{}'".format(kwarg))
         if 'main_values' in kwargs:
             mains = kwargs['main_values']
+        if mains is None:
+            raise TypeError("RichArray() missing required argument 'mains'"
+                            + " (pos 1)")
         if 'uncertainties' in kwargs:
             uncs = kwargs['uncertainties']
         if 'are_lower_limits' in kwargs:
             are_lolims = kwargs['are_lower_limits']
         if 'are_upper_limits' in kwargs:
             are_uplims = kwargs['are_upper_limits']
         if 'are_finite_ranges' in kwargs:
@@ -1019,19 +1233,27 @@
             
         uncs = np.array(uncs)
         are_lolims = np.array(are_lolims)
         are_uplims = np.array(are_uplims)
         are_ranges = np.array(are_ranges)
         domains = np.array(domains)
         array = np.empty(mains.size, object)
-        if uncs.shape == (*mains.shape, 2):
+        if uncs.size == 1:
+            uncs = uncs * np.ones((*mains.shape, 2))
+        elif len(uncs) == 2:
+            uncs = np.array([uncs[0] * np.ones(mains.shape),
+                             uncs[1] * np.ones(mains.shape)]).transpose()
+        elif uncs.shape == (*mains.shape, 2):
             uncs = uncs.transpose()
         elif uncs.shape == mains.shape:
             uncs = np.array([[uncs]]*2).reshape((2, *mains.shape))
-        if domains.shape == (*mains.shape, 2):
+        if len(domains) == 2:
+            domains = np.array([domains[0] * np.ones(mains.shape),
+                                domains[1] * np.ones(mains.shape)]).transpose()
+        elif domains.shape == (*mains.shape, 2):
             domains = domains.transpose()
         elif domains.flatten().shape == (2,):
             domains = (np.array([domains for x in mains.flat])
                        .reshape((*mains.shape, 2)).transpose())
             
         mains_flat = mains.flatten()
         uncs_flat = uncs.flatten()
@@ -1049,101 +1271,93 @@
             domain = [domains_flat[i], domains_flat[i+offset]]
             array[i] = RichValue(main, unc, is_lolim, is_uplim, is_range,
                                  domain)
         array = array.reshape(mains.shape)
         array = array.view(cls)
         return array
 
+    @property
     def mains(self):
         return np.array([x.main for x in self.flat]).reshape(self.shape)
-
+    @property
     def uncs(self):
-        return np.array([x.unc for x in self.flat]).reshape([*self.shape,2])
-    
+        return np.array([x.unc for x in self.flat]).reshape([*self.shape,2]) 
+    @property
     def are_lolims(self):
         return np.array([x.is_lolim for x in self.flat]).reshape(self.shape)
-
+    @property
     def are_uplims(self):
-        return np.array([x.is_uplim for x in self.flat]).reshape(self.shape)
-
+        return np.array([x.is_uplim for x in self.flat]).reshape(self.shape) 
+    @property
     def are_ranges(self):
         return np.array([x.is_range for x in self.flat]).reshape(self.shape)
-    
+    @property 
     def domains(self):
         return np.array([x.domain for x in self.flat]).reshape([*self.shape,2])
-    
+    @property
     def nums_sf(self):
         return np.array([x.num_sf for x in self.flat]).reshape(self.shape)
-    
+    @property
     def min_exps(self):
-        return np.array([x.min_exp() for x in self.flat]).reshape(self.shape)
-    
+        return np.array([x.min_exp for x in self.flat]).reshape(self.shape)
+    @property
     def are_lims(self):
-        return np.array([x.is_lim() for x in self.flat]).reshape(self.shape)
-    
+        return np.array([x.is_lim for x in self.flat]).reshape(self.shape)
+    @property
     def are_intervs(self):
-        return np.array([x.is_interv() for x in self.flat]).reshape(self.shape)
-    
+        return np.array([x.is_interv for x in self.flat]).reshape(self.shape)
+    @property
     def are_centrs(self):
-        return np.array([x.is_centr() for x in self.flat]).reshape(self.shape)
-    
+        return np.array([x.is_centr for x in self.flat]).reshape(self.shape)
+    @property
     def centers(self):
-        return np.array([x.center() for x in self.flat]).reshape(self.shape) 
-
+        return np.array([x.center for x in self.flat]).reshape(self.shape) 
+    @property
     def rel_uncs(self):
-        return (np.array([x.rel_unc() for x in self.flat])
-                .reshape([*self.shape,2]).transpose())
-    
+        return (np.array([x.rel_unc for x in self.flat])
+                .reshape((*self.shape,2)))
+    @property
     def signals_noises(self):
-        return (np.array([x.signal_noise() for x in self.flat])
-                .reshape([*self.shape,2]))
-    
+        return (np.array([x.signal_noise for x in self.flat])
+                .reshape((*self.shape,2)))
+    @property
     def ampls(self):
-        return (np.array([x.ampls() for x in self.flat])
-                .reshape([*self.shape,2]))
-    
+        return (np.array([x.ampls for x in self.flat])
+                .reshape((*self.shape,2)))
+    @property
     def rel_ampls(self):
-        return (np.array([x.rel_ampls() for x in self.flat])
-                .reshape([*self.shape,2]).transpose())
-
+        return (np.array([x.rel_ampls for x in self.flat])
+                .reshape((*self.shape,2)))
+    @property
     def norm_uncs(self):
-        return (np.array([x.norm_unc() for x in self.flat])
-                .reshape([*self.shape,2]).transpose())
-    
+        return (np.array([x.norm_unc for x in self.flat])
+                .reshape((self.shape,2)))
+    @property
     def prop_scores(self):
-        return (np.array([x.prop_score() for x in self.flat])
+        return (np.array([x.prop_score for x in self.flat])
                 .reshape(self.shape))
+    @property
+    def uncs_eb(self):
+        return self.uncs.transpose()
     
     def intervals(self, sigmas=3.):
         return (np.array([x.interval() for x in self.flat])
-                .reshape([*self.shape,2]))
-    
-    def uncs_eb(self):
-        return self.uncs().transpose()
+                .reshape((*self.shape,2)))
     
     def set_params(self, params):
         """Set the rich value parameters of each entry of the rich array."""
-        new_array = np.empty(0, float)
         for x in self.flat:
             if 'domain' in params:
                 x.domain = params['domain']
-            if 'num_sf' in params:
-                x.num_sf = params['num_sf']
-            if 'min_exp' in params:
-                x.min_exp = params['min_exp']
-            new_array = np.append(new_array, x)
-        new_array = new_array.reshape(self.shape)
-        self = new_array
-            
-    def latex(self, dollars=True, mult_symbol=defaultparams['multiplication '
-                                  +'symbol for scientific notation in LaTeX']):
-        """Display the values of the rich array in LaTeX math mode."""
-        new_array = (np.array([x.latex(dollars, mult_symbol) for x in self.flat])
-                     .reshape(self.shape))
-        return new_array
+            for key in ('num_sf', 'number of scientific figures'):
+                if key in params:
+                    x.num_sf = params[key]
+            for key in ('min_exp', 'minimum exponent for scientific notation'):
+                if key in params:
+                    x.min_exp = params[key]
     
     def set_lims_factor(self, factor=4.):
         """Set uncertainties of limits with respect to central values."""
         c = factor
         if not hasattr(c, '__iter__'):
             c = [c, c]
         cl, cu = c
@@ -1153,30 +1367,44 @@
             cu = 1
         for x in self.flat:
             if x.is_lolim:
                 x.unc = [x.main / cl] * 2
             elif x.is_uplim:
                 x.unc = [x.main / cu] * 2
 
+    def latex(self, dollars=True, mult_symbol=defaultparams['multiplication '
+                                  +'symbol for scientific notation in LaTeX']):
+        """Display the values of the rich array in LaTeX math mode."""
+        new_array = (np.array([x.latex(dollars, mult_symbol) for x in self.flat])
+                     .reshape(self.shape))
+        return new_array
+
     def sample(self, len_sample=1):
         """Obtain a sample of each entry of the array"""
         new_array = np.empty(0, float)
         for x in self.flat:
             new_array = np.append(new_array, x.sample(len_sample))
         new_shape = ((*self.shape, len_sample) if len_sample != 1
                      else self.shape)
         new_array = new_array.reshape(new_shape).transpose()
         return new_array
 
     def function(self, function, **kwargs):
         """Apply a function to the rich array."""
-        new_array = function_with_rich_arrays(function, self, **kwargs)
-        return rich_array(new_array)
+        return function_with_rich_arrays(function, self, **kwargs)
+    
+    def mean(self):
+        return np.array(self).mean()
+    
+    def std(self):
+        std_function = lambda u: (np.sum((u - u.mean())**2)
+                                  / len(self - 1))**0.5
+        return self.function(std_function)
 
-    # Method abbreviations.
+    # Attribute acronyms.
     main_values = mains
     uncertainties = uncs
     are_lower_limits = are_lolims
     are_upper_limits = are_uplims
     are_finite_ranges = are_ranges
     numbers_of_scientific_figures = nums_sf
     minimum_exponents_for_scientific_notation = min_exps
@@ -1185,22 +1413,137 @@
     are_centered_values = are_centrs
     relative_uncertainties = rel_uncs
     signals_to_noises = signals_noises
     amplitudes = ampls
     relative_amplitudes = rel_ampls
     normalized_uncertainties = norm_uncs
     propagation_scores = prop_scores
+    # Method acronyms.
     set_limits_factor = set_lims_factor
     set_parameters = set_params
 
 class RichDataFrame(pd.DataFrame):
     """
     A class to store a dataframe with uncertainties or with upper/lower limits.
     """
-      
+    
+    @property
+    def _constructor(self):
+        return RichDataFrame
+    
+    @property
+    def _constructor_sliced(self):
+        return RichSeries
+
+    def _attribute(self, attribute):
+        """Apply the input RichArray attribute with 1 element."""
+        code = [
+            'array = self.values',
+            'shape = array.shape',
+            'types = np.array([type(x) for x in array.flat]).reshape(shape)',
+            'data = np.zeros(shape, object)',
+            'cond = types == RichValue',
+            'data[cond] = rich_array(array[cond]).{}'.format(attribute),
+            'cond = ~cond',
+            'data[cond] = array[cond]',
+            'df = pd.DataFrame(data, self.index, self.columns)']
+        code = '\n'.join(code)
+        output = {}
+        exec(code, {**{'self': self}, **globals()}, output)
+        return output['df']
+
+    def _attribute2(self, attribute):
+        """Apply the input RichArray attribute with 2 elements."""
+        code = [
+            'array = self.values',
+            'shape = array.shape',
+            'types = np.array([type(x) for x in array.flat]).reshape(shape)',
+            'data = np.zeros(shape, object)',
+            'cond = types == RichValue',
+            'new_elements = rich_array(array[cond]).{}'.format(attribute),
+            'new_elements = [[x[0], x[1]] for x in new_elements]',
+            'new_subarray = np.frompyfunc(list, 0, 1)'
+            + '(np.empty(cond.sum(), dtype=object))',
+            'new_subarray[:] = new_elements',
+            'data[cond] = new_subarray',
+            'cond = ~cond',
+            'data[cond] = array[cond]',
+            'df = pd.DataFrame(data, self.index, self.columns)']
+        code = '\n'.join(code)
+        output = {}
+        exec(code, {**{'self': self}, **globals()}, output)
+        return output['df']
+    
+    def mains(self):
+        return self._attribute('mains')
+
+    def uncs(self):
+        return self._attribute2('uncs')
+    
+    def are_lolims(self):
+        return self._attribute('are_lolims')
+    
+    def are_uplims(self):
+        return self._attribute('are_uplims')
+    
+    def are_ranges(self):
+        return self._attribute('are_ranges')
+    
+    def domains(self):
+        return self._attribute2('domains')
+    
+    def are_lims(self):
+        return self._attribute('are_lims')
+    
+    def are_intervs(self):
+        return self._attribute('are_intervs')
+    
+    def are_centrs(self):
+        return self._attribute('are_centrs')
+    
+    def rel_uncs(self):
+        return self._attribute2('rel_uncs')
+    
+    def signals_noises(self):
+        return self._attribute2('signal_noises')
+    
+    def ampls(self):
+        return self._attribute2('ampls')
+    
+    def rel_ampls(self):
+        return self._attribute2('rel_ampls')
+    
+    def norm_uncs(self):
+        return self._attribute2('norm_uncs')
+    
+    def prop_scores(self):
+        return self._attribute('prop_scores')
+    
+    def intervals(self):
+        return self._attribute2('intervals')
+    
+    def flatten_attribute_output(self, attribute):
+        """Separate the list elements from the output of the given attribute."""
+        df = eval('self.{}'.format(attribute))
+        df1, df2 = df.copy(), df.copy()
+        columns = df.columns
+        are_lists = False
+        for i,row in df.iterrows():
+            for entry,col in zip(row,columns):
+                if (type(entry) is list and len(entry) == 2
+                        and all([type(entry[i]) != str for i in [0,1]])):
+                    are_lists = True
+                    df1.at[i,col] = entry[0]
+                    df2.at[i,col] = entry[1]
+                else:
+                    df1.at[i,col] = entry
+                    df2.at[i,col] = entry
+        output = [df1, df2] if are_lists else df1
+        return output
+    
     def get_params(self):
         """Return the rich value parameters of each column of the dataframe."""
         domain, num_sf, min_exp = {}, {}, {}
         for col in self:
             x = self[col][0]
             is_rich_value = True if type(x) is RichValue else False
             domain[col] = (x.domain if is_rich_value
@@ -1224,20 +1567,23 @@
         for col in self:
             num_rows = len(self[col])
             is_rich_value = True if type(self[col][0]) is RichValue else False
             if is_rich_value:
                 if 'domain' in params and col in params['domain']:
                     for i in range(num_rows):
                         self[col][i].domain = params['domain'][col]
-                if 'num_sf' in params and col in params['num_sf']:
-                    for i in range(num_rows):
-                        self[col][i].num_sf = params['num_sf'][col]
-                if 'min_exp' in params and col in params['min_exp']:
-                    for i in range(num_rows):
-                        self[col][i].min_exp = params['min_exp'][col]
+                for key in ('num_sf', 'number of scientific figures'):
+                    if key in params and col in params[key]:
+                        for i in range(num_rows):
+                            self[col][i].num_sf = params[key][col]
+                for key in ('min_exp',
+                            'minimum exponent for scientific notation'):
+                    if key in params and col in params[key]:
+                        for i in range(num_rows):
+                            self[col][i].min_exp = params[key][col]
     
     def create_column(self, function, columns, **kwargs):
         """
         Create a column applying a function to the given columns of the dataframe.
 
         Parameters
         ----------
@@ -1253,18 +1599,18 @@
         -------
         new_df : dataframe
             Resulting dataframe with the new column.
         """
         new_column = np.empty(len(self), RichValue)
         for i,(_,row) in enumerate(self.iterrows()):
             arguments = [row[col] for col in columns]
-            new_rich_value = function_with_rich_values(function, arguments,
+            new_rval = function_with_rich_values(function, arguments,
                                                        **kwargs)
-            new_column[i] = new_rich_value
-        new_column = rich_array(new_column)
+            new_column[i] = new_rval
+        new_column = new_column.view(RichArray)
         return new_column
 
     def create_row(self, function, rows, **kwargs):
         """
         Create a row applying a function to the given rows of the dataframe.
     
         Parameters
@@ -1281,17 +1627,17 @@
         -------
         new_row : dataframe
             Dataframe containing the new row.
         """
         new_row = {}
         for i,col in enumerate(self):
             arguments = [self.at[idx,col] for idx in rows]
-            new_rich_value = function_with_rich_values(function, arguments,
-                                                       **kwargs)
-            new_row[col] = new_rich_value
+            new_rval = function_with_rich_values(function, arguments,
+                                                 **kwargs)
+            new_row[col] = new_rval
         return new_row
 
     def latex(self, return_df=False, row_sep='\\tabularnewline',
               show_dollar=True, mult_symbol=defaultparams['multiplication '
                                   + 'symbol for scientific notation in LaTeX']):
         """Return the content of the dataframe as a table in LaTeX format."""
         row_sep = ' ' + row_sep + ' \n'
@@ -1334,27 +1680,159 @@
                     c = limits_factors[col]
                     if not hasattr(c, '__iter__'):
                         c = [c, c]
                     cl, cu = c
                     c = cl if entry.is_lolim else cu
                     self.at[i,col].set_lims_factor(c)
     
-    # Method abbreviations.
+    # Attribute acronyms.
+    main_values = mains
+    uncertainties = uncs
+    are_lower_limits = are_lolims
+    are_upper_limits = are_uplims
+    are_finite_ranges = are_ranges
+    are_limits = are_lims
+    are_intervals = are_intervs
+    are_centered_values = are_centrs
+    relative_uncertainties = rel_uncs
+    signals_to_noises = signals_noises
+    amplitudes = ampls
+    relative_amplitudes = rel_ampls
+    normalized_uncertainties = norm_uncs
+    propagation_scores = prop_scores
+    # Method acronyms.
     get_parameters = get_params
     set_parameters = set_params
     set_limits_factors = set_lims_factors
 
+class RichSeries(pd.Series):
+    """A class to store a series with the RichArray methods."""
+    
+    @property
+    def _constructor(self):
+        return RichSeries
+    
+    @property
+    def _constructor_expanddim(self):
+        return RichDataFrame
+    
+    @property
+    def mains(self):
+        return pd.Series(rich_array(self.values).mains, self.index)
+    @property
+    def uncs(self):
+        return [pd.Series(rich_array(self.values).uncs.T[i].T,
+                          self.index) for i in (0,1)]
+    @property
+    def are_lolims(self):
+        return pd.Series(rich_array(self.values).are_lolims, self.index)
+    @property
+    def are_uplims(self):
+        return pd.Series(rich_array(self.values).are_uplims, self.index)
+    @property
+    def are_ranges(self):
+        return pd.Series(rich_array(self.values).are_ranges, self.index)
+    @property
+    def domains(self):
+        return [pd.Series(rich_array(self.values).domains.T[i].T,
+                          self.index) for i in (0,1)]
+    @property
+    def nums_sf(self):
+        return pd.Series(rich_array(self.values).num_sf, self.index)
+    @property
+    def min_exps(self):
+        return pd.Series(rich_array(self.values).min_exps, self.index)
+    @property
+    def are_lims(self):
+        return pd.Series(rich_array(self.values).are_lims, self.index)
+    @property
+    def are_intervs(self):
+        return pd.Series(rich_array(self.values).are_intervs, self.index)
+    @property
+    def are_centrs(self):
+        return pd.Series(rich_array(self.values).are_centrs, self.index)
+    @property
+    def centers(self):
+        return pd.Series(rich_array(self.values).centers, self.index)
+    @property
+    def rel_uncs(self):
+        return [pd.Series(rich_array(self.values).rel_uncs.T[i].T,
+                          self.index) for i in (0,1)]
+    @property
+    def signals_noises(self):
+        return [pd.Series(rich_array(self.values).signals_noises.T[i].T,
+                          self.index) for i in (0,1)]
+    @property
+    def ampls(self):
+        return [pd.Series(rich_array(self.values).ampls.T[i].T,
+                          self.index) for i in (0,1)]
+    @property
+    def rel_ampls(self):
+        return [pd.Series(rich_array(self.values).rel_ampls.T[i].T,
+                          self.index) for i in (0,1)]
+    @property
+    def norm_uncs(self):
+        return [pd.Series(rich_array(self.values).norm_uncs.T[i].T,
+                          self.index) for i in (0,1)]
+    @property
+    def prop_scores(self):
+        return [pd.Series(rich_array(self.values).prop_scores.T[i].T,
+                          self.index) for i in (0,1)]
+    
+    def intervals(self, sigmas=3.):
+        return [pd.Series(rich_array(self.values).intervals(sigmas).T[i].T,
+                          self.index) for i in (0,1)]
+    
+    def set_params(self, params):
+        data = self.values.view(RichArray)
+        data.set_params(params)
+        self.update(pd.Series(data, self.index))
+    
+    def set_lims_factor(self, factor=4.):
+        data = self.values.view(RichArray)
+        data.set_lims_factor(factor)
+        self.update(pd.Series(data, self.index))
+
+    def latex(self, **kwargs):
+        return pd.Series(rich_array(self.values).latex(**kwargs), self.index)
+    
+    def function(self, function, **kwargs):
+        data = self.values.view(RichArray).function(function, **kwargs)
+        return pd.Series(data, self.index)
+
+    # Attribute acronyms.
+    main_values = mains
+    uncertainties = uncs
+    are_lower_limits = are_lolims
+    are_upper_limits = are_uplims
+    are_finite_ranges = are_ranges
+    numbers_of_scientific_figures = nums_sf
+    minimum_exponents_for_scientific_notation = min_exps
+    are_limits = are_lims
+    are_intervals = are_intervs
+    are_centered_values = are_centrs
+    relative_uncertainties = rel_uncs
+    signals_to_noises = signals_noises
+    amplitudes = ampls
+    relative_amplitudes = rel_ampls
+    normalized_uncertainties = norm_uncs
+    propagation_scores = prop_scores
+    # Method acronyms.
+    set_limits_factor = set_lims_factor
+    set_parameters = set_params
+    
+
 def add_two_rich_values(x, y):
     """Sum two rich values to get a new one."""
     num_sf = max(x.num_sf, y.num_sf)
     min_exp = min(x.min_exp, y.min_exp)
     domain = [x.domain[0] + y.domain[0], x.domain[1] + y.domain[1]]
     sigmas = defaultparams['sigmas to use approximate uncertainty propagation']
-    if (not (x.is_interv() or y.is_interv())
-            and min(x.rel_ampl()) > sigmas and min(y.rel_ampl())) > sigmas:
+    if (not (x.is_interv or y.is_interv)
+            and min(x.rel_ampl) > sigmas and min(y.rel_ampl) > sigmas):
         z = x.main + y.main
         dz = (np.array(x.unc)**2 + np.array(y.unc)**2)**0.5
         z = RichValue(z, dz, domain=domain)
     else:
         z = function_with_rich_values(lambda a,b: a+b, [x, y], domain=domain,
                                       is_vectorizable=True)
     z.num_sf = num_sf
@@ -1365,22 +1843,22 @@
     """Multiply two rich values to get a new one."""
     num_sf = max(x.num_sf, y.num_sf)
     min_exp = min(x.min_exp, y.min_exp)
     with np.errstate(divide='ignore', invalid='ignore'):
         domain_combs = [x.domain[0] * y.domain[0], x.domain[0] * y.domain[1],
                         x.domain[1] * y.domain[0], x.domain[1] * y.domain[1]]
     domain1, domain2 = min(domain_combs), max(domain_combs)
-    if np.isnan(domain1):
-        domain1 = np.nan_to_num(domain1, nan=-np.inf)
-    if np.isnan(domain2):
-        domain2 = np.nan_to_num(domain2, nan=np.inf)
+    if not np.isfinite(domain1):
+        domain1 = -np.inf
+    if not np.isfinite(domain2):
+        domain2 = np.inf
     domain = [domain1, domain2]
     sigmas = defaultparams['sigmas to use approximate uncertainty propagation']
-    if (not (x.is_interv() or y.is_interv())
-         and x.prop_score() > sigmas and y.prop_score() > sigmas):
+    if (not (x.is_interv or y.is_interv)
+         and x.prop_score > sigmas and y.prop_score > sigmas):
         z = x.main * y.main
         dx, dy = np.array(x.unc), np.array(y.unc)
         dz = z * ((dx/x.main)**2 + (dy/y.main)**2)**0.5
         z = RichValue(z, dz, domain=domain)
     else:
         z = function_with_rich_values(lambda a,b: a*b, [x, y], domain=domain,
                                       is_vectorizable=True)
@@ -1392,33 +1870,159 @@
     """Divide two rich values to get a new one."""
     num_sf = max(x.num_sf, y.num_sf)
     min_exp = min(x.min_exp, y.min_exp)
     with np.errstate(divide='ignore', invalid='ignore'):
         domain_combs = [x.domain[0] * y.domain[0], x.domain[0] * y.domain[1],
                         x.domain[1] * y.domain[0], x.domain[1] * y.domain[1]]
     domain1, domain2 = min(domain_combs), max(domain_combs)
-    if np.isinf(domain1):
+    if not np.isfinite(domain1):
         domain1 = -np.inf
-    if np.isinf(domain2):
+    if not np.isfinite(domain2):
         domain2 = np.inf
     domain = [domain1, domain2]
     sigmas = defaultparams['sigmas to use approximate uncertainty propagation']
-    if (not (x.is_interv() or y.is_interv()) and 0 not in [x.main, y.main]
-         and x.prop_score() > sigmas and y.prop_score() > sigmas):
+    if (not (x.is_interv or y.is_interv) and 0 not in [x.main, y.main]
+         and x.prop_score > sigmas and y.prop_score > sigmas):
         z = x.main / y.main
         dx, dy = np.array(x.unc), np.array(y.unc)
         dz = z * ((dx/x.main)**2 + (dy/y.main)**2)**0.5
         z = RichValue(z, dz, domain=domain)
     else:
         z = function_with_rich_values(lambda a,b: a/b, [x, y], domain=domain,
                                   is_vectorizable=True, sigmas=sigmas)
     z.num_sf = num_sf
     z.min_exp = min_exp
     return z
 
+def greater(x, y, sigmas=defaultparams['sigmas for comparison']):
+    """Determine if a rich value/array (x) is greater than another one (y)."""
+    are_single_values = all([type(var) is str
+                             or not hasattr(var, '__iter__') for var in (x,y)])
+    if are_single_values:
+        x = x if type(x) is RichValue else rich_value(x)
+        y = y if type(y) is RichValue else rich_value(y)
+        x1, x2 = x.interval(sigmas=sigmas)
+        y1, y2 = y.interval(sigmas=sigmas)
+        output = True if x2 > y2 else False
+    else:
+        x = x if type(x) is RichArray else rich_array(x)
+        y = y if type(y) is RichValue else rich_array(y)
+        if x.size == 0 and x.shape != y.shape:
+            x = x.flatten()[0] * np.ones(y.shape)
+        if y.size == 0 and x.shape != y.shape:
+            y = y.flatten()[0] * np.ones(x.shape)
+        if x.shape != y.shape:
+            raise Exception('Input arrays must have the same shape.')
+        output = np.empty(0, bool)
+        for xi,yi in zip(x.flat, y.flat):
+            output = np.append(output, greater(xi,yi))
+        output = output.reshape(x.shape)
+    return output
+
+def less(x, y, sigmas=defaultparams['sigmas for overlap']):
+    """Determine if a rich value/array (x) is less than another one (y)."""
+    are_single_values = all([type(var) is str
+                             or not hasattr(var, '__iter__') for var in (x,y)])
+    if are_single_values:
+        x = x if type(x) is RichValue else rich_value(x)
+        y = y if type(y) is RichValue else rich_value(y)
+        x1, x2 = x.interval(sigmas=sigmas)
+        y1, y2 = y.interval(sigmas=sigmas)
+        output = True if x2 < y2 else False
+    else:
+        x = x if type(x) is RichArray else rich_array(x)
+        y = y if type(y) is RichValue else rich_array(y)
+        if x.size == 1 and x.shape != y.shape:
+            x = x.flatten()[0] * np.ones(y.shape)
+        if y.size == 1 and x.shape != y.shape:
+            y = y.flatten()[0] * np.ones(x.shape)
+        if x.shape != y.shape:
+            raise Exception('Input arrays must have the same shape.')
+        output = np.empty(0, bool)
+        for xi,yi in zip(x.flat, y.flat):
+            output = np.append(output, less(xi,yi))
+        output = output.reshape(x.shape)
+    return output
+
+def equiv(x, y, sigmas=defaultparams['sigmas for overlap']):
+    """Check if a rich value/array (x) is equivalent than another one (y)."""
+    are_single_values = all([type(var) is str
+                             or not hasattr(var, '__iter__') for var in (x,y)])
+    if are_single_values:
+        x = x if type(x) is RichValue else rich_value(x)
+        y = y if type(y) is RichValue else rich_value(y)
+        minor, major = (x, y) if x < y else (y, x)
+        x1, x2 = minor.interval(sigmas=sigmas)
+        y1, y2 = major.interval(sigmas=sigmas)
+        output = True if x2 >= y1 else False
+    else:
+        x = x if type(x) is RichArray else rich_array(x)
+        y = y if type(y) is RichValue else rich_array(y)
+        if x.size == 1 and x.shape != y.shape:
+            x = x.flatten()[0] * np.ones(y.shape)
+        if y.size == 1 and x.shape != y.shape:
+            y = y.flatten()[0] * np.ones(x.shape)
+        if x.shape != y.shape:
+            raise Exception('Input arrays must have the same shape.')
+        output = np.empty(0, bool)
+        for xi,yi in zip(x.flat, y.flat):
+            output = np.append(output, equiv(xi,yi))
+        output = output.reshape(x.shape)
+    return output
+
+def greater_equiv(x, y,
+                  sigmas_comparison=defaultparams['sigmas for comparison'],
+                  sigmas_overlap=defaultparams['sigmas for overlap']):
+    """Check if a rich value/array is greater or equivalent than another one."""
+    are_single_values = all([type(var) is str
+                             or not hasattr(var, '__iter__') for var in (x,y)])
+    if are_single_values:
+        x = x if type(x) is RichValue else rich_value(x)
+        y = y if type(y) is RichValue else rich_value(y)
+        output = greater(x, y, sigmas_comparison) or equiv(x, y, sigmas_overlap)
+    else:
+        x = x if type(x) is RichArray else rich_array(x)
+        y = y if type(y) is RichValue else rich_array(y)
+        if x.size == 1 and x.shape != y.shape:
+            x = x.flatten()[0] * np.ones(y.shape)
+        if y.size == 1 and x.shape != y.shape:
+            y = y.flatten()[0] * np.ones(x.shape)
+        if x.shape != y.shape:
+            raise Exception('Input arrays must have the same shape.')
+        output = np.empty(0, bool)
+        for xi,yi in zip(x.flat, y.flat):
+            output = np.append(output, greater_equiv(xi,yi))
+        output = output.reshape(x.shape)
+    return output
+
+def less_equiv(x, y,
+               sigmas_comparison=defaultparams['sigmas for comparison'],
+               sigmas_overlap=defaultparams['sigmas for overlap']):
+    """Check if a rich value/array is less or equivalent than another one."""
+    are_single_values = all([type(var) is str
+                             or not hasattr(var, '__iter__') for var in (x,y)])
+    if are_single_values:
+        x = x if type(x) is RichValue else rich_value(x)
+        y = y if type(y) is RichValue else rich_value(y)
+        output = less(x, y, sigmas_comparison) or equiv(x, y, sigmas_overlap)
+    else:
+        x = x if type(x) is RichArray else rich_array(x)
+        y = y if type(y) is RichValue else rich_array(y)
+        if x.size == 1 and x.shape != y.shape:
+            x = x.flatten()[0] * np.ones(y.shape)
+        if y.size == 1 and x.shape != y.shape:
+            y = y.flatten()[0] * np.ones(x.shape)
+        if x.shape != y.shape:
+            raise Exception('Input arrays must have the same shape.')
+        output = np.empty(0, bool)
+        for xi,yi in zip(x.flat, y.flat):
+            output = np.append(output, less_equiv(xi,yi))
+        output = output.reshape(x.shape)
+    return output
+
 def rich_value(text, domain=None):
     """
     Convert the input text to a rich value.
 
     Parameters
     ----------
     text : str
@@ -1497,16 +2101,16 @@
                         dx1, dx2 = '0', '0'
                 if x not in ['nan', 'NaN', 'None']:
                     e = text.split(' ')[1]
                     x = x + e
                     dx1 = dx1 + e
                     dx2 = dx2 + e
                 else:
-                    x = np.nan
-                    dx1, dx2 = 0, 0
+                    x = 'nan'
+                    dx1, dx2 = '0', '0'
             x = x.replace('e0','')
             main = float(x)
             unc = [float(dx1), float(dx2)]
             is_range = False
         else:
             text = text.replace(' --','--').replace('-- ','--')
             x1, x2 = text.split('--')
@@ -1541,35 +2145,38 @@
 
     Returns
     -------
     rich_array : array
         Resulting rich array.
     """
     array = np.array(array)
+    shape = array.shape
     mains, uncs, are_lolims, are_uplims, are_ranges, domains = \
         [], [], [], [], [], []
     for element in array.flat:
         x = (element if type(element) is RichValue
              else rich_value(element, domain))
         mains += [x.main]
         uncs += [x.unc]
         are_lolims += [x.is_lolim]
         are_uplims += [x.is_uplim]
         are_ranges += [x.is_range]
         domains += [x.domain]
-    mains = np.array(mains).reshape(array.shape)
+    mains = np.array(mains).reshape(shape)
     uncs = np.array(uncs)
-    uncs = np.array([uncs[:,0].reshape(array.shape).tolist(),
-                     uncs[:,1].reshape(array.shape).tolist()]).transpose()
-    are_lolims = np.array(are_lolims).reshape(array.shape)
-    are_uplims = np.array(are_uplims).reshape(array.shape)
-    are_ranges = np.array(are_ranges).reshape(array.shape)
+    uncs = (np.array([uncs[:,0].reshape(shape).tolist(),
+                     uncs[:,1].reshape(shape).tolist()])
+            .transpose().reshape((*shape, 2)))
+    are_lolims = np.array(are_lolims).reshape(shape)
+    are_uplims = np.array(are_uplims).reshape(shape)
+    are_ranges = np.array(are_ranges).reshape(shape)
     domains = np.array(domains)
-    domains = np.array([domains[:,0].reshape(array.shape).tolist(),
-                        domains[:,1].reshape(array.shape).tolist()]).transpose()
+    domains = (np.array([domains[:,0].reshape(shape).tolist(),
+                         domains[:,1].reshape(shape).tolist()])
+               .transpose().reshape((*shape, 2)))
     new_array = RichArray(mains, uncs, are_lolims, are_uplims, are_ranges,
                           domains)
     return new_array
 
 def rich_dataframe(df, domains=None):
     """
     Convert the values of the input dataframe of text strings to rich values.
@@ -1718,41 +2325,46 @@
             cond = (s/3 < np.abs(x-m)) & (np.abs(x-m) < s)
             x_ = (x[cond]-m)/s*(3/4)*math.tau
             g[cond] = c/2 * np.abs(np.cos(x_))**n * np.sign(x_)
             g *= sign
             return g
         y = np.zeros(x.size)
         cond1 = x < m
-        cond2 = x >= m
+        cond2 = x > m
         y1 = symmetric_general_pdf(x[cond1], m, s1, a1)
         y2 = symmetric_general_pdf(x[cond2], m, s2, a2)
         h1 = symmetric_general_pdf(m, m, s1, a1)
         h2 = symmetric_general_pdf(m, m, s2, a2)
-        c1 = 0 * (h1 - h2)
-        c2 = h1 - h2 - c1
-        if h1 < h2:
-            c2, c1 = c1, c2
-        y1_, y2_ = y1.copy(), y2.copy()
-        if c1 != 0:
-            y1_ -= correction(x[cond1], m, s1, c1, sign=1)
-        if c2 != 0:
-            y2_ += correction(x[cond2], m, s2, c2, sign=-1)
-        y_min = min(np.min(y1_), np.min(y2_))
+        h1_or, h2_or = h1.copy(), h2.copy()
+        h1, h2 = min(h1, h2), max(h1, h2)
+        cond1_ = x[cond1] > m - s1
+        cond2_ = x[cond2] < m + s2
+        frac = 0.
+        y_min = 0.
+        lim = 1/6 * h1
         i = 0
-        while y_min < 0:
+        while y_min < lim:
+            if i > 0:
+                frac += 1/8
+            c1 = frac * (h2 - h1)
+            c2 = h2 - h1 - c1
+            if h1_or < h2_or:
+                c1, c2 = -c2, c1
+            x_ = np.linspace(m - s1, m + s2, int(1e3))
+            cond1_ = x_ < m
+            cond2_ = x_ > m
+            y1_ = symmetric_general_pdf(x_[cond1_], m, s1, a1)
+            y2_ = symmetric_general_pdf(x_[cond2_], m, s2, a2)
+            y1_ -= correction(x_[cond1_], m, s1, c1, sign=1)
+            y2_ += correction(x_[cond2_], m, s2, c2, sign=-1)
+            y_min = np.min(np.append(y1_, y2_))
             i += 1
-            c1 = i/6 * (h1 - h2)
-            c2 = h1 - h2 - c1
-            if h1 < h2:
-                c2, c1 = c1, c2
-            y1_ = y1 - correction(x[cond1], m, s1, c1, sign=1)
-            y2_ = y2 + correction(x[cond2], m, s2, c2, sign=-1)
-            y_min = min(np.min(y1_), np.min(y2_))
-        y[cond1] = y1_
-        y[cond2] = y2_
+        y[cond1] = y1 - correction(x[cond1], m, s1, c1, sign=1)
+        y[cond2] = y2 + correction(x[cond2], m, s2, c2, sign=-1)
+        y[x==m] = h1 + (1-frac) * (h2 - h1)
         if x.shape == ():
             y = y[0]
     
     return y
 
 def sample_from_pdf(pdf, size, low, high, **kwargs):
     """
@@ -1858,21 +2470,21 @@
         if not x1 < x2:
             raise Exception('Inferior limit must be lower than superior limit.')
         if np.isinf(x1):
             log_x1 = inf_log
         elif x1 == 0:
             log_x1 = zero_log
         else:
-            log_x1 = log10(abs(x1))
+            log_x1 = _log10(abs(x1))
         if np.isinf(x2):
             log_x2 = inf_log
         elif x2 == 0:
             log_x2 = zero_log
         else:
-            log_x2 = log10(abs(x2))
+            log_x2 = _log10(abs(x2))
         if log_x1 < zero_log:
             log_x1 = zero_log
         if log_x2 > inf_log: 
             log_x2 = inf_log
         if x1 < 0:
             if x2 <= 0:
                 exps = np.linspace(log_x2, log_x1, N)
@@ -1901,18 +2513,27 @@
     """
     if 'arguments' in kwargs:
         args = kwargs['arguments']
     if 'samples_length' in kwargs:
         len_samples = kwargs['samples_length']
     if 'samples_size' in kwargs:
         len_samples = kwargs['samples_size']
-    if not hasattr(args, '__iter__'):
+    if type(args) not in (tuple, list):
         args = [args]
     args = [rich_value(arg) if type(arg) is not RichValue else arg
             for arg in args]
+    if type(function) is str:
+        function = function.replace('{}', '({})')
+        variables = [arg.var for arg in args]
+        function = function.format(*variables)
+        vars_str = ','.join(variables)
+        function = eval('lambda {}: {}'.format(vars_str, function))
+        args = [variable_dict[var] for var in variables]
+        if 'unc_function' in kwargs:
+            kwargs['unc_function'] = None
     if len_samples is None:
         len_samples = int(len(args)**0.5 * defaultparams['size of samples'])
     args_distr = np.array([arg.sample(len_samples) for arg in args])
     if is_vectorizable:
         distr = function(*args_distr)
     else:
         distr = np.array([function(*args_distr[:,i])
@@ -1998,15 +2619,15 @@
     elif x2 > 0 and x2 > 10**inf_log:
         x2 = 10**inf_log
     new_interval = [x1, x2]
     return new_interval
 
 def evaluate_distr(distr, domain=[-np.inf,np.inf], function=None, args=None,
                 len_samples=defaultparams['size of samples'],
-                is_vectorizable=False, consider_ranges=True,
+                is_vectorizable=False, consider_intervs=True,
                 lims_fraction=defaultparams['fraction of the central value '
                                             + 'for upper/lower limits'],
                 num_reps_lims=defaultparams['number of repetitions to estimate'
                                             + ' upper/lower limits'],
                 zero_log=defaultparams['decimal exponent to define zero'],
                 inf_log=defaultparams['decimal exponent to define infinity'],
                 **kwargs):
@@ -2016,14 +2637,17 @@
     Parameters
     ----------
     distr : list/array (float)
         Input distribution of values.
     domain : list (float), optional
         Domain of the variable represented by the distribution.
         The default is [-np.inf,np.inf].
+    consider_intervs : bool, optional
+        If True, the resulting distribution could be interpreted as an upper/
+        lower limit or a constant range of values. The default is True.
     zero_log : float, optional
         Decimal logarithm of the minimum value in absolute value.
     inf_log : float, optional
         Decimal logarithm of the maximum value in absolute value.
     * The rest of the arguments are only used if the distribution was the
       result of a known function, and are the same as in the function
       'function_with_rich_values'.
@@ -2045,22 +2669,32 @@
         """Return the range in order of magnitude of the input interval."""
         x1, x2 = interval
         if abs(x1) < 10**zero_log:
             x1 = 0
         if abs(x2) < 10**zero_log:
             x2 = 0
         if x1*x2 > 0:
-            d = log10(x2-x1)
+            d = _log10(x2-x1)
         elif x1*x2 < 0:
-            d = np.log10(abs(x1)) + 2*abs(zero_log) + np.log10(x2)
+            d = _log10(abs(x1)) + 2*abs(zero_log) + _log10(x2)
         else:
             xlim = x1 if x2 == 0 else x2
-            d = abs(zero_log) + np.log10(abs(xlim))
+            d = abs(zero_log) + _log10(abs(xlim))
         return d
     
+    if type(function) is str:
+        function = function.replace('{}', '({})')
+        variables = [arg.var for arg in args]
+        function = function.format(*variables)
+        vars_str = ','.join(variables)
+        function = eval('lambda {}: {}'.format(vars_str, function))
+        args = [variable_dict[var] for var in variables]
+        if 'unc_function' in kwargs:
+            kwargs['unc_function'] = None
+    
     def repeat_functions(functions, initial_values, num_reps_lims=1):
         """Repeat the given functions to the input arguments."""
         num_vars = len(initial_values)
         all_vars = [[initial_values[j]] for j in range(num_vars)]
         for i in range(num_reps_lims):
             args_distr = np.array([arg.sample(len_samples)
                                    for arg in args])
@@ -2069,114 +2703,132 @@
             else:
                 distr = np.array([function(*args_distr[:,j])
                                   for j in range(len_samples)])
             for j in range(num_vars):
                 all_vars[j] += [functions[j](distr)]
         return tuple(all_vars)
     
+    if args is not None:
+        if type(args) not in (tuple, list):
+            args = [args]
+        args = [rich_value(arg) if type(arg) is not RichValue else arg
+                for arg in args]
+    
     distr = np.array(distr)
     distr = distr[np.isfinite(distr)].flatten()
+    if distr.size == 0:
+        return RichValue(np.nan)
     domain1, domain2 = domain if domain is not None else [-np.inf, np.inf]
-    x1, x2 = np.min(distr), np.max(distr)
     main, unc = center_and_uncs(distr)
-    ord_range_1s = magnitude_order_range([main-unc[0], main+unc[1]])
-    ord_range_x = magnitude_order_range([x1, x2])
-    probs_hr, bins_hr = np.histogram(distr, bins=4*len_samples)
-    probs_lr, bins_lr = np.histogram(distr, bins=20)
-    max_prob_hr = probs_hr.max()
-    max_prob_lr = probs_lr.max()
-    # plt.plot(bins_hr[:-1], probs_hr,'-')
-    # plt.plot(bins_lr[:-1], probs_lr, '--')
-    hr1f, hr2f, lrf, rf = 0.99, 0.9, 0.7, 0.3
-    cond_hr1 = (probs_hr[0] > hr1f*max_prob_hr
-                or probs_hr[-1] > hr1f*max_prob_hr)
-    cond_hr2 = probs_hr[0] > hr2f*max_prob_hr
-    cond_lr = lrf*max_prob_lr < probs_lr[0] < max_prob_lr
-    cond_range = ord_range_x - ord_range_1s < rf if x1 != x2 else False
-    cond_limit = cond_hr1
-    cond_range = (cond_range or (not cond_range and cond_hr2)
-                  or (not cond_range and not cond_hr2 and cond_lr))
-    if cond_limit:
-        if num_reps_lims > 0 and args is not None:
-            xx1, xx2, xxc = repeat_functions([np.min, np.max, np.median],
-             [x1, x2, main], num_reps_lims)
-            x1, x2 = np.min(xx1), np.max(xx2)
-            main = np.median(xxc)
-        ord_range_b = log10(abs(main)) - log10(abs(x1))
-        x1, x2 = add_zero_infs([x1, x2], zero_log-6, inf_log-6)
-        if ord_range_b > inf_log-6 and cond_hr2:
-            main = np.nan
-            unc = [np.inf, np.inf]
-        else:
-            if args is not None:
-                args_main = [arg.main for arg in args]
-                x0 = function(*args_main)
-                domain_ = add_zero_infs([domain1, domain2],
-                                        zero_log+6, inf_log-6)
-                x_ = RichValue([x1,x2], domain=domain_)
-                if x_.is_lolim:
-                    x1 = x0 + (1 - lims_fraction) * (x1 - x0)
-                elif x_.is_uplim:
-                    x2 = x0 - (1 - lims_fraction) * (x0 - x2)
+    
+    if consider_intervs:
+        x1, x2 = np.min(distr), np.max(distr)
+        ord_range_1s = magnitude_order_range([main-unc[0], main+unc[1]])
+        ord_range_x = magnitude_order_range([x1, x2])
+        probs_hr, bins_hr = np.histogram(distr, bins=4*len_samples)
+        probs_lr, bins_lr = np.histogram(distr, bins=20)
+        max_prob_hr = probs_hr.max()
+        max_prob_lr = probs_lr.max()
+        # plt.plot(bins_hr[:-1], probs_hr,'-')
+        # plt.plot(bins_lr[:-1], probs_lr, '--')
+        hr1f, hr2f, lrf, rf = 0.99, 0.9, 0.7, 0.3
+        cond_hr1 = (probs_hr[0] > hr1f*max_prob_hr
+                    or probs_hr[-1] > hr1f*max_prob_hr)
+        cond_hr2 = probs_hr[0] > hr2f*max_prob_hr
+        cond_lr = lrf*max_prob_lr < probs_lr[0] < max_prob_lr
+        cond_range = ord_range_x - ord_range_1s < rf if x1 != x2 else False
+        cond_limit = cond_hr1
+        cond_range = (cond_range or (not cond_range and cond_hr2)
+                      or (not cond_range and not cond_hr2 and cond_lr))
+        if cond_limit:
+            if num_reps_lims > 0 and args is not None:
+                xx1, xx2, xxc = repeat_functions([np.min, np.max, np.median],
+                 [x1, x2, main], num_reps_lims)
+                x1, x2 = np.min(xx1), np.max(xx2)
+                main = np.median(xxc)
+            ord_range_b1 = magnitude_order_range([x1, main])
+            ord_range_b2 = magnitude_order_range([main, x2])
+            x1, x2 = add_zero_infs([x1, x2], zero_log-6, inf_log-6)
+            if (ord_range_b1 > inf_log-6 and ord_range_b2 > inf_log-6
+                    and cond_hr2):
+                main = np.nan
+                unc = [np.inf, np.inf]
+            else:
+                if args is not None:
+                    args_main = [arg.main for arg in args]
+                    x0 = function(*args_main)
+                    domain_ = add_zero_infs([domain1, domain2],
+                                            zero_log+6, inf_log-6)
+                    x_ = RichValue([x1,x2], domain=domain_)
+                    if x_.is_lolim:
+                        x1 = x0 + (1 - lims_fraction) * (x1 - x0)
+                    elif x_.is_uplim:
+                        x2 = x0 - (1 - lims_fraction) * (x0 - x2)
+                main = [x1, x2]
+                unc = [0, 0]
+        elif cond_range:
+            if num_reps_lims > 0 and args is not None:
+                xx1, xx2 = repeat_functions([np.min, np.max], [x1, x2],
+                                            num_reps_lims)
+                x1, x2 = np.median(xx1), np.median(xx2)
+            x1, x2 = add_zero_infs([x1, x2], zero_log+6, inf_log-6)
             main = [x1, x2]
             unc = [0, 0]
-    elif cond_range:
-        if num_reps_lims > 0 and args is not None:
-            xx1, xx2 = repeat_functions([np.min, np.max], [x1, x2],
-                                        num_reps_lims)
-            x1, x2 = np.median(xx1), np.median(xx2)
-        x1, x2 = add_zero_infs([x1, x2], zero_log+6, inf_log-6)
-        main = [x1, x2]
-        unc = [0, 0]
     
     z = RichValue(main, unc, domain=domain)
-    
-    if not consider_ranges and z.is_range:
-        main, unc = center_and_uncs(distr)
-        z = RichValue(main, unc, domain=domain)
             
     return z
 
-def function_with_rich_values(
-        function, args, unc_function=None, is_vectorizable=False,
-        len_samples=None, domain=None, consider_ranges=True,
+def function_with_rich_values(function, args,
+        unc_function=None, is_vectorizable=False,
+        len_samples=None, domain=None, consider_intervs=None,
         sigmas=defaultparams['sigmas to use approximate '
                              + 'uncertainty propagation'],
         use_sigma_combs=defaultparams['use 1-sigma combinations to '
                                       + 'approximate uncertainty propagation'],
         lims_fraction=defaultparams['fraction of the central value '
                                     + 'for upper/lower limits'],
         num_reps_lims=defaultparams['number of repetitions to estimate'
                                     + ' upper/lower limits'], **kwargs):
     """
     Apply a function to the input rich values.
 
     Parameters
     ----------
-    function : function
-        Function to be applied to the input rich values.
+    function : str / function
+        Text string of the source code of the function to be applied to the
+        input rich values. It should have empty ({}) brackets to indicate the
+        position of the arguments in the same order as in 'args'. It can also
+        be a Python function directly, but then correlation between variables
+        will not be taken into account, and the mathematical expression of the
+        resulting rich value will not be stored.
     args : list (rich values)
         List with the input rich values, in the same order as the arguments of
         the given function.
     unc_function : function, optional
         Function to estimate the uncertainties, in case that error propagation
-        can be used. The arguments should be the central values first and then
-        the uncertainties, with the same order as in the input function.
+        can be used. It should be the text string of the source code of the
+        function to be applied to the input rich values. It will only be used
+        if the arguments of the principal function ('args') are all independent
+        variables. The arguments of 'unc_function' should be the central values
+        first and then the uncertainties, with the same order as in the input
+        function.
     is_vectorizable : bool, optional
         If True, the calculations of the function will be optimized making use
         of vectorization. The default is False.
     len_samples : int, optional
         Size of the samples of the arguments. The default is the number of
-        arguments times the default size of samples (10000).
+        arguments times the default size of samples (8000).
     domain : list (float), optional
         Domain of the result. If not specified, it will be estimated
         automatically.
-    consider_ranges : bool, optional
-        If True, the resulting distribution could be interpreted as a constant
-        range of values.
+    consider_intervs : bool, optional
+        If True, the resulting distribution could be interpreted as an upper/
+        lower limit or a constant range of values. The default is None (it is
+        False if all of the arguments are centered values).
     sigmas : float, optional
         Threshold to apply uncertainty propagation. The value is the distance
         to the bounds of the domain relative to the uncertainty.
         The default is 10.
     use_sigma_combs : bool, optional
         If True, the calculation of the uncertainties will be optimized when
         the relative amplitudes are small and there is no uncertainty function
@@ -2190,59 +2842,75 @@
         The default is 0.1.
     num_reps_lims : int, optional
         Number of repetitions of the sampling done in the cases of having an
         upper/lower limit for better estimating its value. The default is 4.
 
     Returns
     -------
-    new_rich_value : rich value
+    new_rval : rich value
         Resulting rich value.
     """
     
     if 'arguments' in kwargs:
         args = kwargs['arguments']
     if 'samples_length' in kwargs:
         len_samples = kwargs['samples_length']
     if 'samples_size' in kwargs:
         len_samples = kwargs['samples_size']
     if 'uncertainty_function' in kwargs:
         unc_function = kwargs['uncertainty_function']
     zero_log = defaultparams['decimal exponent to define zero']
     inf_log = defaultparams['decimal exponent to define infinity']
     
-    if not hasattr(args, '__iter__'):
+    if type(args) not in (tuple, list):
         args = [args]
     args = [rich_value(arg) if type(arg) is not RichValue else arg
             for arg in args]
+    function_or = copy.copy(function)
+    if type(function) is str:
+        function = function.replace('{}', '({})')
+        variables = np.concatenate(tuple(arg.vars for arg in args)).tolist()
+        expressions = [arg.expression for arg in args]
+        expression = function.format(*expressions).replace(' ', '')
+        expression = expression.replace('((', '(').replace('))', ')')
+        variables = list(set(variables))
+        vars_str = ','.join(variables)
+        function = eval('lambda {}: {}'.format(vars_str, expression))
+        args = [variable_dict[var] for var in variables]
+        common_vars = set(args[0].vars)
+        for i in range(len(args)-1):
+            common_vars = common_vars & set(args[i+1].vars)
+        if len(args) > 1 and len(common_vars) > 0:
+            unc_function = None
+    
     if len_samples is None:
         len_samples = int(len(args)**0.5 * defaultparams['size of samples'])
     num_sf = max([arg.num_sf for arg in args])
     min_exp = min([arg.min_exp for arg in args])
-    if all([not arg.is_interv() for arg in args]):
-        consider_ranges = False
-    
-    unc_propagation = (not any([arg.is_interv() for arg in args])
-                       and all([arg.prop_score() > sigmas for arg in args]))
+    if consider_intervs is None:
+        consider_intervs = (False if all([arg.is_centr for arg in args])
+                            else True)
+    unc_propagation = (not any([arg.is_interv for arg in args])
+                       and all([arg.prop_score > sigmas for arg in args]))
     if use_sigma_combs:
         if (unc_function is None
             and (((unc_function is None and len(args) > 5))
-                 or all([arg.prop_score() > sigmas for arg in args]))):
+                 or all([arg.prop_score > sigmas for arg in args]))):
             unc_propagation = False
-    else:
-        if unc_function is None:
+    elif unc_function is None:
             unc_propagation = False
             
     args_main = [arg.main for arg in args]
     try:
         main = function(*args_main)
         if hasattr(main, '__iter__'):
             output_size = main.size if type(main) is np.ndarray else len(main)
         else:
             output_size = 1
-        output_type = type(main) if output_size > 1 else RichValue
+        output_type = RichArray if type(main) is np.ndarray else type(main)
     except Exception:
         function_code = inspect.getsourcelines(function)[0]
         for line in function_code:
             if 'lambda' in line:
                 line = line.split('lambda ')[1].split(':')[1]
                 if line.startswith('('):
                     output = line[1:].split('),')[0]
@@ -2253,125 +2921,131 @@
                 output_size = len(output.split(','))
                 break
             elif 'return' in line:
                 output = line.split('return ')[1]
                 output_size = len(output.split(','))
                 break
         output_type = list if '[' in output else tuple
-        
-    if not any(np.isnan([arg.main for arg in args])):
-        if output_size > 1:
-            is_vectorizable = False
-        if domain is not None and not hasattr(domain[0], '__iter__'):
-            domain = [domain]*output_size
-        if unc_propagation:
-            if output_size == 1:
-                main = [main]
-            for k in range(output_size):
-                if domain is not None and domain[k] is None:
-                    domain[k] = [-np.inf, np.inf]
-            if domain is None:
-                domain = [[-np.inf, np.inf]]*output_size
-            new_domain = domain
-            if unc_function is not None:
-                args_unc = [np.array(arg.unc) for arg in args]
-                unc = unc_function(*args_main, *args_unc)
-                if not hasattr(unc,'__iter__'):
-                    unc = [unc]*output_size
-            else:
-                inds_combs = list(itertools.product(*[[0,1,2]]*len(args)))
-                comb_main = tuple([1]*len(args))
-                inds_combs.remove(comb_main)
-                args_combs = []
-                args_all_vals = [[arg.main - arg.unc[0], arg.main,
-                                  arg.main + arg.unc[1]] for arg in args]
-                for i, inds in enumerate(inds_combs):
-                    args_combs += [[]]
-                    for j, arg in enumerate(args):
-                        args_combs[i] += [args_all_vals[j][inds[j]]]
-                new_comb = [function(*args_comb) for args_comb in args_combs]
-                unc = [[main[k] - np.min(new_comb[:][k]),
-                        np.max(new_comb[:][k]) - main[k]]
-                       for k in range(output_size)]
-        else:
-            args_distr = np.array([arg.sample(len_samples) for arg in args])
+
+    if output_size > 1:
+        is_vectorizable = False
+    if domain is not None and not hasattr(domain[0], '__iter__'):
+        domain = [domain]*output_size
+    if unc_propagation:
+        if output_size == 1:
+            main = [main]
+        for k in range(output_size):
+            if domain is not None and domain[k] is None:
+                domain[k] = [-np.inf, np.inf]
+        if domain is None:
+            domain = [[-np.inf, np.inf]]*output_size
+        new_domain = domain
+        if unc_function is not None:
+            args_unc = [np.array(arg.unc) for arg in args]
+            unc = unc_function(*args_main, *args_unc)
+            unc = np.abs(unc)
+            if not hasattr(unc,'__iter__'):
+                unc = [unc]*output_size
+        else:
+            inds_combs = list(itertools.product(*[[0,1,2]]*len(args)))
+            comb_main = tuple([1]*len(args))
+            inds_combs.remove(comb_main)
+            args_combs = []
+            args_all_vals = [[arg.main - arg.unc[0], arg.main,
+                              arg.main + arg.unc[1]] for arg in args]
+            for i, inds in enumerate(inds_combs):
+                args_combs += [[]]
+                for j, arg in enumerate(args):
+                    args_combs[i] += [args_all_vals[j][inds[j]]]
+            new_comb = [function(*args_comb) for args_comb in args_combs]
+            unc = [[main[k] - np.min(new_comb[:][k]),
+                    np.max(new_comb[:][k]) - main[k]]
+                   for k in range(output_size)]
+    else:
+        args_distr = np.array([arg.sample(len_samples) for arg in args])
+        if is_vectorizable:
+            new_distr = function(*args_distr)
+        else:
+            new_distr = np.array([function(*args_distr[:,i])
+                                  for i in range(len_samples)])
+        if output_size == 1 and len(new_distr.shape) == 1:
+            new_distr = np.array([new_distr]).transpose()
+        main, unc, new_domain = [], [], []
+        if domain is None:
+            domain_args_distr = np.array(
+                [loguniform_distribution(*arg.domain, len_samples//3)
+                 for arg in args])
             if is_vectorizable:
-                new_distr = function(*args_distr)
+                domain_distr = function(*domain_args_distr)
             else:
-                new_distr = np.array([function(*args_distr[:,i])
-                                      for i in range(len_samples)])
-            if output_size == 1 and len(new_distr.shape) == 1:
-                new_distr = np.array([new_distr]).transpose()
-            main, unc, new_domain = [], [], []
-            if domain is None:
-                domain_args_distr = np.array(
-                    [loguniform_distribution(*arg.domain, len_samples//3)
-                     for arg in args])
-                if is_vectorizable:
-                    domain_distr = function(*domain_args_distr)
-                else:
-                    domain_distr = np.array([function(*domain_args_distr[:,i])
-                                             for i in range(len_samples//3)])
-                if output_size == 1 and len(domain_distr.shape) == 1:
-                    domain_distr = np.array([domain_distr]).transpose()
-            for k in range(output_size):
-                if domain is not None:
-                    domain1, domain2 = domain[k]
-                else:
-                    domain1 = np.min(domain_distr[:,k])
-                    domain2 = np.max(domain_distr[:,k])
+                domain_distr = np.array([function(*domain_args_distr[:,i])
+                                         for i in range(len_samples//3)])
+            if output_size == 1 and len(domain_distr.shape) == 1:
+                domain_distr = np.array([domain_distr]).transpose()
+        for k in range(output_size):
+            if domain is not None:
+                domain_k = domain[k]
+            else:
+                domain1 = np.min(domain_distr[:,k])
+                domain2 = np.max(domain_distr[:,k])
+                if not np.isfinite(domain1):
+                    domain1 = -np.inf
+                if not np.isfinite(domain2):
+                    domain2 = np.inf
                 domain1, domain2 = remove_zero_infs([domain1, domain2],
                                                     zero_log, inf_log)
                 domain_k = [float(round_sf(domain1, num_sf+3)),
                             float(round_sf(domain2, num_sf+3))]
                 domain_k = add_zero_infs(domain_k, zero_log+6, inf_log-6)
-                def function_k(*argsk):
-                    y = function(*argsk)
-                    if output_size > 1:
-                        y = y[k]
-                    return y
-                rval_k = evaluate_distr(new_distr[:,k], domain_k, function_k,
-                    args, len_samples, is_vectorizable, consider_ranges,
-                    lims_fraction, num_reps_lims, zero_log, inf_log)
-                main_k = (rval_k.main if not rval_k.is_interv()
-                          else rval_k.interval())
-                unc_k = rval_k.unc
-                main += [main_k]
-                unc += [unc_k]
-                new_domain += [domain_k]
-    else:
-        main, unc = [np.nan]*output_size, [np.nan]*output_size
-        new_domain = [[min([arg.domain[0] for arg in args]),
-                       max([arg.domain[1] for arg in args])] * output_size]
+            def function_k(*argsk):
+                y = function(*argsk)
+                if output_size > 1:
+                    y = y[k]
+                return y
+            rval_k = evaluate_distr(new_distr[:,k], domain_k, function_k,
+                        args, len_samples, is_vectorizable, consider_intervs,
+                        lims_fraction, num_reps_lims, zero_log, inf_log)
+            main_k = rval_k.main if not rval_k.is_interv else rval_k.interval()
+            unc_k = rval_k.unc
+            main += [main_k]
+            unc += [unc_k]
+            new_domain += [domain_k]
         
     output = []
     for k in range(output_size):
-        new_rich_value = RichValue(main[k], unc[k], domain=new_domain[k])
-        new_rich_value.num_sf = num_sf
-        new_rich_value.min_exp = min_exp
-        output += [new_rich_value]
-    if output_size == 1:
+        new_rval = RichValue(main[k], unc[k], domain=new_domain[k])
+        new_rval.num_sf = num_sf
+        new_rval.min_exp = min_exp
+        if type(function_or) is str:
+            new_rval.vars = variables
+            new_rval.expression = expression
+        output += [new_rval]
+    if output_size == 1 and output_type not in (tuple, list):
         output = output[0]
-    if output_size > 1:
-        if output_type is tuple:
-            output = tuple(output)
-        elif output_type is np.ndarray:
-            output = np.array(output)
+    if output_type is tuple:
+        output = tuple(output)
+    elif output_type is RichArray:
+        output = np.array(output).view(RichArray)
             
     return output
 
 def function_with_rich_arrays(function, args, elementwise=False, **kwargs):
     """
     Apply a function to the input rich arrays.
     (abbreviation: array_function)
 
     Parameters
     ----------
-    function : function
-        Function to be applied to the elements of the input rich arrays.
+    function : str / function
+        Text string of the source code of the function to be applied to the
+        input rich values. It should have empty ({}) brackets to indicate the
+        position of the arguments in the same order as in 'args'. It can also
+        be a Python function directly, but then correlation between variables
+        will not be taken into account, and the mathematical expression of the
+        resulting rich value will not be stored.
     args : list (rich arrays)
         List with the input rich arrays, in the same order as the arguments of
         the given function.
     elementwise : bool, optional
         If True, the function will be aplied to the input arrays element by
         element.
     * The rest of the arguments are the same as in 'function_with_rich_values'.
@@ -2379,38 +3053,49 @@
     Returns
     -------
     new_rich_array : rich array
         Resulting rich array.
     """
     if type(args) not in (tuple, list):
         args = [args]
-    args = [rich_array(arg) if type(arg) != RichArray else arg
+    args = [rich_value(arg) if type(arg) != RichArray else arg
             for arg in args]
-    shape = args[0].shape
+    if elementwise and (len(args) > 0
+            and type(args[0]) is str or not hasattr(args[0], '__iter__')):
+        args = [rich_array(args)]
+        shape = args[0].shape
+    else:
+        args = [rich_array(arg) if type(arg) != RichArray else arg
+                for arg in args]
+        shape = args[0].shape
     if 'len_samples' not in kwargs:
         kwargs['len_samples'] = int(len(args)**0.5
                                     * defaultparams['size of samples'])
     if elementwise:
         same_shapes = True
         for arg in args[1:]:
             if arg.shape != shape:
                 same_shapes = False
                 break
         if not same_shapes:
             raise Exception('Input arrays have different shapes.')
         new_array = np.empty(0, RichValue)
         args_flat = np.array([arg.flatten() for arg in args])
         for i in range(args[0].size):
-            args_i = np.array(args_flat)[:,i]
-            new_rich_value = function_with_rich_values(function, args_i,
-                                                       **kwargs)
-            new_array = np.append(new_array, new_rich_value)
-        new_array = rich_array(new_array.reshape(shape))
+            args_i = np.array(args_flat)[:,i].tolist()
+            new_rval = function_with_rich_values(function, args_i, **kwargs)
+            new_array = np.append(new_array, new_rval)
+        if shape == ():
+            new_array = np.array(new_array[0])
+        new_array = new_array.view(RichArray)
         output = new_array
     else:
+        if type(function) is str:
+            raise Exception("Argument 'function' should be a function "
+                            + "when elementwise=False, not str")
         num_args = len(args)
         arg_sizes = [arg.size for arg in args]
         arg_shapes = [arg.shape for arg in args]
         inds = [0, *np.cumsum(arg_sizes)]
         def alt_function(*argsf):
             rec_args = []
             for i in range(num_args):
@@ -2421,16 +3106,16 @@
             return y
         alt_args = []
         for arg in args:
             alt_args += list(arg.flat)
         output = function_with_rich_values(alt_function, alt_args, **kwargs)
     return output
 
-def rich_fmean(array, function=lambda x: x, inverse_function=lambda x: x,
-               weights=None, weight_function=lambda x: x, **kwargs):
+def fmean(array, function=lambda x: x, inverse_function=lambda x: x,
+          weights=None, weight_function=lambda x: x, **kwargs):
     """
     Compute the generalized f-mean of the input values.
 
     Parameters
     ----------
     array : array / list (float)
         Input values.
@@ -2466,14 +3151,20 @@
         w_f = weight_function(w)
         w_f /= sum(w_f)
         y = inverse_function(np.sum(x_f * w_f))
         return y
     y = function_with_rich_arrays(fmean_function, [array, weights], **kwargs)
     return y
 
+def mean(array, weights=None, weight_function=lambda x: x, **kwargs):
+    """Arithmetic mean of the input values."""
+    mean = fmean(array, weights=weights, weight_function=weight_function,
+                 **kwargs)
+    return mean
+
 def errorbar(x, y, lims_factor=None, **kwargs):
     """
     Plot the input rich arrays (y versus x) with Matplotlib.
 
     Parameters
     ----------
     x : rich array
@@ -2488,24 +3179,25 @@
         Matplotlib's 'errorbar' keyword arguments.
 
     Returns
     -------
     plot : matplotlib.container.ErrorbarContainer
         Matplotib's 'errorbar' output.
     """
+    global num_plots
     def set_kwarg(keyword, default):
         """Set a certain keyword argument with a default value."""
         if keyword in kwargs:
             kwarg = kwargs[keyword]
             del kwargs[keyword]
         else:
             kwarg = default
         return kwarg
     def lim_factor(x):
-        xc = np.sort(x.mains())
+        xc = np.sort(x.mains)
         xc = xc[np.isfinite(xc)]
         with np.errstate(divide='ignore', invalid='ignore'):
             r = abs(linregress(xc, np.arange(len(xc))).rvalue)
         factor = 2. + 12.*r**8
         return factor
     xa, ya = rich_array(x), rich_array(y)
     xc = rich_array([x]) if len(xa.shape) == 0 else xa
@@ -2518,271 +3210,390 @@
         lims_factor_x, lims_factor_y = lims_factor
     if lims_factor_x is None:
         lims_factor_x = lim_factor(xc)
     if lims_factor_y is None:
         lims_factor_y = lim_factor(yc)
     xc.set_lims_factor(lims_factor_x)
     yc.set_lims_factor(lims_factor_y)
-    color = set_kwarg('color', 'gray')
+    plt.plot()
+    ax = plt.gca()
+    color = ax.plot([])[0].get_color()
+    color = set_kwarg('color', color)
     ecolor = set_kwarg('ecolor', 'black')
     fmt = set_kwarg('fmt', '.')
-    cond = ~ (xc.are_ranges() | yc.are_ranges())
-    plot = plt.errorbar(xc.mains()[cond], yc.mains()[cond],
-                xerr=xc.uncs_eb()[:,cond], yerr=yc.uncs_eb()[:,cond],
-                uplims=yc.are_uplims()[cond], lolims=yc.are_lolims()[cond],
-                xlolims=xc.are_lolims()[cond], xuplims=xc.are_uplims()[cond],
+    cond = ~ (xc.are_ranges | yc.are_ranges)
+    plot = plt.errorbar(xc.mains[cond], yc.mains[cond],
+                xerr=xc.uncs_eb[:,cond], yerr=yc.uncs_eb[:,cond],
+                uplims=yc.are_uplims[cond], lolims=yc.are_lolims[cond],
+                xlolims=xc.are_lolims[cond], xuplims=xc.are_uplims[cond],
                 color=color, ecolor=ecolor, fmt=fmt, **kwargs)
-    cond = xc.are_ranges()
+    cond = xc.are_ranges
     for xi,yi in zip(xc, yc):
-        if xi.is_range & ~xi.is_lim():
-            plt.errorbar(xi.main, yi.main, xerr=xi.unc_eb(),
+        if xi.is_range & ~xi.is_lim:
+            plt.errorbar(xi.main, yi.main, xerr=xi.unc_eb,
                          uplims=yi.is_uplim, lolims=yi.is_uplim,
                          fmt=fmt, color='None', ecolor=ecolor, **kwargs)
             for xij in yi.interval():
-                plt.errorbar(xij, yi.main, xerr=xi.unc_eb(), fmt=fmt,
+                plt.errorbar(xij, yi.main, xerr=xi.unc_eb, fmt=fmt,
                              color='None', ecolor=ecolor, **kwargs)
-    cond = yc.are_ranges()
+    cond = yc.are_ranges
     for xi,yi in zip(xc[cond], yc[cond]):
         if yi.is_range:
-            plt.errorbar(xi.main, yi.main, yerr=yi.unc_eb(),
+            plt.errorbar(xi.main, yi.main, yerr=yi.unc_eb,
                          xuplims=xi.is_uplim, xlolims=xi.is_uplim,
                          fmt=fmt, color='None', ecolor=ecolor, **kwargs)
             for yij in yi.interval():
-                plt.errorbar(xi.main, yij, xerr=xi.unc_eb(), fmt=fmt,
+                plt.errorbar(xi.main, yij, xerr=xi.unc_eb, fmt=fmt,
                              color='None', ecolor=ecolor, **kwargs)
     return plot
 
-def point_fit(y, function, guess, num_samples=3000,
-              loss=lambda a,b: (a-b)**2, lim_loss_factor=4., **kwargs):
+def curve_fit(x, y, function, guess, num_samples=3000,
+              loss=lambda a,b: (a-b)**2, lim_loss_factor=4.,
+              consider_intervs=False, use_easy_sampling=False, **kwargs):
     """
-    Perform a fit of the input points (y) with respect to the given function.
+    Perform a fit of y over x with respect to the given function.
 
     Parameters
     ----------
+    x : rich array
+        Independent variable.
     y : rich array
-        Set of points to be compared with the result of the model function.
+        Dependent variable.
     function : function
-        Function to be optimized, that is, a function of the parameters to be
-        optimized that will be compared with the input points.
+        Function to be optimized, that is, the function of y with respect to x.
+        It has to contain as arguments the independent variable (x) and the
+        parameters to be optimized.
     guess : list (float)
         List of initial values of the arguments of the function.
     num_samples : int, optional
         Number of different samples of the input data used for calculating the
         parameter distributions. The default is 3000.
     loss : function, optional
         Function that defines the error between two numbers: a sample of a rich
         value (first argument) and a numeric prediction of it (second
         argument). The default is the squared error.
     lim_loss_factor : float, optional
         Factor to enlarge the loss if the rich value is not a centered value
         and the prediction falls outside the interval of possible values of the
         rich value. The default is 4.
-    kwargs : arguments, optional
+    consider_intervs : bool, optional
+        If True, upper/lower limits and constant ranges of values will be taken
+        into account during the fit. This option increases considerably the
+        computation time. The default is False.
+    use_easy_sampling : bool, optional.
+        If True, upper/lower limits and constant ranges of values will be
+        sampled as usual, with uniform distributions for finite intervals of
+        values and lognormal distributions for infinite intervals. If False,
+        intervals will not be sampled for the fitting itself, but will be taken
+        into account for calculating the loss function for the fit.
+        The default is False.
+    **kwargs : arguments
         Keyword arguments of SciPy's function 'minimize'.
 
     Returns
     -------
     result : dict
         Dictionary containing the following entries:
         - parameters : list (rich value)
             List containing the optimized values for the parameters.
-        - samples : array (float)
+        - dispersion : rich value
+            Estimated real dispersion between the model and the fitted data.
+        - loss : rich value
+            Final mean loss between the original points and the modeled ones.
+        - parameters samples : array (float)
             Array containing the samples of the fitted parameters used to
             compute the rich values. Its shape is (num_samples, num_params),
             with num_params being the number of parameters to be fitted.
-        - loss : array (float)
-            Array containing the validation loss corresponding for each group
-            of fitted parameters in the 'samples' entry.
-        - fails : int
+        - dispersion sample : array (float)
+            Sample of the calculated real dispersion of the points with respect
+            to the model.
+        - loss sample : array (float)
+            Array containing the loss between the original data and each group
+            of fitted parameters in the 'parameters samples' entry.
+        - number of fails : int
             Number of times that the fit failed, for the iterations among the
             different samples (the number of iterations is num_samples).
     """
-    ya = rich_array(y)
-    y = rich_array([y]) if len(ya.shape) == 0 else ya
+    if len(x) != len(y):
+        raise Exception('Input arrays have not the same size.')
     num_points = len(y)
+    xa, ya = rich_array(x), rich_array(y)
+    x = rich_array([x]) if len(xa.shape) == 0 else xa
+    y = rich_array([y]) if len(ya.shape) == 0 else ya
     if type(guess) in [int, float]:
         guess = [guess]
-    example_pred = np.array(function(*guess))
-    function_copy = copy.copy(function)
-    if len(example_pred.shape) == 0 or len(example_pred) != num_points:
-        function = lambda *params: [function_copy(*params)]*num_points
     num_params = len(guess)
-    cond = ~y.are_intervs()
-    if sum(cond) == 0:
-        cond = np.ones(num_points, bool)
-    num_intervs = (~cond).sum()
-    def loss_function(params, ys):
-        y_ = np.array(function(*params))
-        error = sum(loss(ys[cond], y_[cond]))
-        y_cond = y_[~cond]
-        if num_intervs > 0:
-            ylims = np.empty(num_intervs)
-            for j, (yj, y_j) in enumerate(zip(y[~cond], y_cond)):
-                y1, y2 = yj.interval()
-                yl = (y_j if y1 <= y_j <= y2
-                      else [y1, y2][np.argmin([abs(y1-y_j), abs(y2-y_j)])])
-                ylims[j] = yl
-                factor = 1. if y1 <= y_j <= y2 else lim_loss_factor
-            error += sum(factor*loss(ylims, y_cond))
-        error /= len(ys)
+    condx = x.are_centrs
+    condy = y[condx].are_centrs
+    if use_easy_sampling and consider_intervs or sum(condx) == 0:
+        condx = np.ones(num_points, bool)
+        condy = np.ones(num_points, bool)
+    num_intervs_x = (~condx).sum()
+    num_intervs_y = (~condy).sum()
+    num_lim_samples = 8
+    xlims_sample = np.append(x[~condx].sample(num_lim_samples),
+                             x[~condx].intervals().T, axis=0).T
+    ylims_sample = np.append(y[~condx].sample(num_lim_samples),
+                             y[~condx].intervals().T, axis=0).T
+    def loss_function(params, xs, ys):
+        y_condx = np.array(function(xs[condx], *params))
+        error = sum(loss(ys[condx][condy], y_condx[condy]))
+        if consider_intervs:
+            y_condxy = y_condx[~condy]
+            if num_intervs_y > 0:
+                ylims = np.empty(num_intervs_y)
+                for j, (yj, y_j) in enumerate(zip(y[condx][~condy], y_condxy)):
+                    y1, y2 = yj.interval()
+                    yl = (y_j if y1 <= y_j <= y2
+                          else [y1, y2][np.argmin([abs(y1-y_j), abs(y2-y_j)])])
+                    ylims[j] = yl
+                    factor = 1. if y1 <= y_j <= y2 else lim_loss_factor
+                error += sum(factor*loss(ylims, y_condxy))
+            if num_intervs_x > 0:
+                for xi, yi in zip(xlims_sample, ylims_sample):
+                    yi_ = [function(xij, *params) for xij in xi]
+                    y1, y2 = min(yi_), max(yi_)
+                    error_i = []
+                    for yij in yi:
+                        yl = (yij if y1 <= yij <= y2 else
+                              [y1, y2][np.argmin([abs(y1-yij),abs(y2-yij)])])
+                        factor = 1. if y1 <= yij <= y2 else lim_loss_factor
+                        error_ij = factor*loss(yl, yij)
+                        error_i += [error_ij]
+                        if error_ij == 0:
+                            break
+                    error += min(error_i)
+        error /= num_points
         return error
-    losses = []
+    losses, dispersions = [], []
     samples = [[] for i in range(num_params)]
     print('Fitting...')
     num_fails = 0
-    for i,ys in enumerate(y.sample(num_samples)):
-        result = minimize(loss_function, guess, args=ys, **kwargs)
+    x_sample = x.sample(num_samples)
+    y_sample = y.sample(num_samples)
+    cond = x.are_centrs & y.are_centrs
+    num_disp_points = cond.sum()
+    for i,(xs,ys) in enumerate(zip(x_sample, y_sample)):
+        result = minimize(loss_function, guess, args=(xs,ys), **kwargs)
         if result.success:
-            losses += [result.fun]
-            guess = result.x
+            params_i = result.x
             for j in range(num_params):
-                samples[j] += [result.x[j]]
+                samples[j] += [params_i[j]]
+            if num_disp_points > 0:
+                ys_cond = function(xs[cond], *params_i)
+                dispersions += [(np.sum((ys[cond] - ys_cond)**2)
+                                / (num_disp_points - 1))**0.5]
+            losses += [result.fun]
+            guess = params_i
         else:
             num_fails += 1
         if ((i+1) % (num_samples//4)) == 0:
             print('  {} %'.format(100*(i+1)//num_samples))
     if num_fails > 0.9*num_samples:
         raise Exception('The fit failed more than 90 % of the time.')
     params_fit = [evaluate_distr(samples[i]) for i in range(num_params)]
+    if num_disp_points > 0:
+        mean_unc = y[cond].uncs.mean()
+        dispersions = np.array(dispersions)
+        dispersions1 = np.maximum(0, dispersions - mean_unc)
+        dispersions2 = np.maximum(0, dispersions**2 - mean_unc**2)**0.5
+        disp_coef = np.median(dispersions1) / mean_unc
+        lim1, lim2 = 0.2, 1.2
+        if disp_coef <= lim1:
+            frac1 = 1.
+        elif disp_coef < lim2: 
+            frac1 = 1. - disp_coef / (lim2 - lim1)
+        else:
+            frac1 = 0.
+        dispersions = frac1 * dispersions1 + (1-frac1) * dispersions2
+    dispersion = evaluate_distr(dispersions, domain=[0,np.inf],
+                                consider_intervs=False)
     losses = np.array(losses)
+    loss = evaluate_distr(losses, consider_intervs=False)
     samples = np.array(samples).transpose()
-    result = {'parameters': params_fit, 'samples': samples,
-              'loss': losses, 'fails': num_fails}
-    return result
+    result = {'parameters': params_fit, 'dispersion': dispersion, 'loss': loss,
+              'parameters samples': samples, 'dispersion sample': dispersions,
+              'loss sample': losses, 'number of fails': num_fails}
+    return result   
 
-def curve_fit(x, y, function, guess, num_samples=3000,
-              loss=lambda a,b: (a-b)**2, lim_loss_factor=4., **kwargs):
+def point_fit(y, function, guess, num_samples=3000,
+              loss=lambda a,b: (a-b)**2, lim_loss_factor=4.,
+              consider_intervs=True, use_easy_sampling=False, **kwargs):
     """
-    Perform a fit of y over x (arrays) with respect to the given function.
-
-    Parameters
-    ----------
-    x : rich array
-        Independent variable.
-    y : rich array
-        Dependent variable.
-    function : function
-        Function to be optimized, that is, the function of y with respect to x.
-        It has to contain as arguments the independent variable (x) and the
-        parameters to be optimized.
-    guess : list (float)
-        List of initial values of the arguments of the function.
-    num_samples : int, optional
-        Number of different samples of the input data used for calculating the
-        parameter distributions. The default is 3000.
-    loss : function, optional
-        Function that defines the error between two numbers: a sample of a rich
-        value (first argument) and a numeric prediction of it (second
-        argument). The default is the squared error.
-    lim_loss_factor : float, optional
-        Factor to enlarge the loss if the rich value is not a centered value
-        and the prediction falls outside the interval of possible values of the
-        rich value. The default is 4.
-    **kwargs : arguments
-        Keyword arguments of SciPy's function 'minimize'.
+    Perform a fit of the input points (y) with respect to the given function.
 
-    Returns
-    -------
-    result : dict
-        Dictionary containing the following entries:
-        - parameters : list (rich value)
-            List containing the optimized values for the parameters.
-        - samples : array (float)
-            Array containing the samples of the fitted parameters used to
-            compute the rich values. Its shape is (num_samples, num_params),
-            with num_params being the number of parameters to be fitted.
-        - loss : array (float)
-            Array containing the validation loss corresponding for each group
-            of fitted parameters in the 'samples' entry.
-        - fails : int
-            Number of times that the fit failed, for the iterations among the
-            different samples (the number of iterations is num_samples).
+    The parameters and the outputs are the same as in the 'curve_fit' function.
     """
-    if len(x) != len(y):
-        raise Exception('Input arrays have not the same size.')
-    num_points = len(y)
-    xa, ya = rich_array(x), rich_array(y)
-    x = rich_array([x]) if len(xa.shape) == 0 else xa
+    ya = rich_array(y)
     y = rich_array([y]) if len(ya.shape) == 0 else ya
+    num_points = len(y)
     if type(guess) in [int, float]:
         guess = [guess]
+    example_pred = np.array(function(*guess))
+    function_copy = copy.copy(function)
+    if len(example_pred.shape) == 0 or len(example_pred) != num_points:
+        function = lambda *params: [function_copy(*params)]*num_points
     num_params = len(guess)
-    params_fit = np.empty(num_params, RichValue)
-    condx = ~x.are_intervs()
-    if sum(condx) == 0:
-        condx = np.ones(num_points, bool)
-    condy = ~(y[condx].are_intervs())
-    num_intervs_x = (~condx).sum()
-    num_intervs_y = (~condy).sum()
-    num_lim_samples = 8
-    xlims_sample = np.append(x[~condx].sample(num_lim_samples),
-                        x[~condx].intervals().transpose(), axis=0).transpose()
-    ylims_sample = np.append(y[~condx].sample(num_lim_samples),
-                        y[~condx].intervals().transpose(), axis=0).transpose()
-    def loss_function(params, xs, ys):
-        y_condx = np.array(function(xs[condx], *params))
-        error = sum(loss(ys[condx][condy], y_condx[condy]))
-        y_condxy = y_condx[~condy]
-        if num_intervs_y > 0:
-            ylims = np.empty(num_intervs_y)
-            for j, (yj, y_j) in enumerate(zip(y[condx][~condy], y_condxy)):
+    cond = y.are_centrs
+    if use_easy_sampling and consider_intervs or sum(cond) == 0:
+        cond = np.ones(num_points, bool)
+    num_intervs = (~cond).sum()
+    def loss_function(params, ys):
+        y_ = np.array(function(*params))
+        error = sum(loss(ys[cond], y_[cond]))
+        y_cond = y_[~cond]
+        if num_intervs > 0:
+            ylims = np.empty(num_intervs)
+            for j, (yj, y_j) in enumerate(zip(y[~cond], y_cond)):
                 y1, y2 = yj.interval()
                 yl = (y_j if y1 <= y_j <= y2
                       else [y1, y2][np.argmin([abs(y1-y_j), abs(y2-y_j)])])
                 ylims[j] = yl
                 factor = 1. if y1 <= y_j <= y2 else lim_loss_factor
-            error += sum(factor*loss(ylims, y_condxy))
-        if num_intervs_x > 0:
-            for xi, yi in zip(xlims_sample, ylims_sample):
-                yi_ = [function(xij, *params) for xij in xi]
-                y1, y2 = min(yi_), max(yi_)
-                error_i = []
-                for yij in yi:
-                    yl = (yij if y1 <= yij <= y2
-                          else [y1, y2][np.argmin([abs(y1-yij), abs(y2-yij)])])
-                    factor = 1. if y1 <= yij <= y2 else lim_loss_factor
-                    error_ij = factor*loss(yl, yij)
-                    error_i += [error_ij]
-                    if error_ij == 0:
-                        break
-                error += min(error_i)
-        error /= len(xs)
+            error += sum(factor*loss(ylims, y_cond))
+        error /= len(ys)
         return error
-    losses = []
+    losses, dispersions = [], []
     samples = [[] for i in range(num_params)]
     print('Fitting...')
     num_fails = 0
-    x_sample = x.sample(num_samples)
     y_sample = y.sample(num_samples)
-    for i,(xs,ys) in enumerate(zip(x_sample, y_sample)):
-        result = minimize(loss_function, guess, args=(xs,ys), **kwargs)
+    cond = y.are_centrs
+    num_disp_points = cond.sum()
+    for i,ys in enumerate(y_sample):
+        result = minimize(loss_function, guess, args=ys, **kwargs)
         if result.success:
-            losses += [result.fun]
-            guess = result.x
+            params_i = result.x
             for j in range(num_params):
-                samples[j] += [result.x[j]]
+                samples[j] += [params_i[j]]
+            if num_disp_points > 0:
+                ys_cond = function(*params_i)
+                dispersions += [(np.sum((ys[cond] - ys_cond)**2)
+                                / (num_disp_points - 1))**0.5]
+            losses += [result.fun]
+            guess = params_i
         else:
             num_fails += 1
         if ((i+1) % (num_samples//4)) == 0:
             print('  {} %'.format(100*(i+1)//num_samples))
     if num_fails > 0.9*num_samples:
         raise Exception('The fit failed more than 90 % of the time.')
     params_fit = [evaluate_distr(samples[i]) for i in range(num_params)]
+    if num_disp_points > 0:
+        mean_unc = y[cond].uncs.mean()
+        dispersions = np.array(dispersions)
+        dispersions1 = np.maximum(0, dispersions - mean_unc)
+        dispersions2 = np.maximum(0, dispersions**2 - mean_unc**2)**0.5
+        disp_coef = np.median(dispersions1) / mean_unc
+        lim1, lim2 = 0.2, 1.2
+        if disp_coef <= lim1:
+            frac1 = 1.
+        elif disp_coef < lim2: 
+            frac1 = 1. - disp_coef / (lim2 - lim1)
+        else:
+            frac1 = 0.
+        dispersions = frac1 * dispersions1 + (1-frac1) * dispersions2
+    dispersion = evaluate_distr(dispersions, domain=[0,np.inf],
+                                consider_intervs=False)
     losses = np.array(losses)
+    loss = evaluate_distr(losses, consider_intervs=False)
     samples = np.array(samples).transpose()
-    result = {'parameters': params_fit, 'samples': samples,
-              'loss': losses, 'fails': num_fails}
-    return result   
-   
-def log10(x):
+    result = {'parameters': params_fit, 'dispersion': dispersion, 'loss': loss,
+              'parameters samples': samples, 'dispersion sample': dispersions,
+              'loss sample': losses, 'number of fails': num_fails}
+    return result    
+
+def _log10(x):
     """Decimal logarithm from NumPy but including x = 0."""
     with np.errstate(divide='ignore'):
         y = np.log10(x)
     return y
-    
-# Function abbreviations.
+
+# Functions for masking arrays.
+def isnan(x):
+    x = rich_array(x) if type(x) is not RichArray else x
+    return np.array([xi.is_nan for xi in x]).reshape(x.shape)
+def isinf(x):
+    x = rich_array(x) if type(x) is not RichArray else x
+    return np.array([xi.is_inf for xi in x]).reshape(x.shape)
+def isfinite(x):
+    x = rich_array(x) if type(x) is not RichArray else x
+    return np.array([xi.is_finite for xi in x]).reshape(x.shape)
+
+# Mathematical functions.
+def sqrt(x):
+    function_ = function if type(x) in (str, RichValue) else array_function
+    return function_('np.sqrt({})', x, domain=[0,np.inf], elementwise=True,
+                     unc_function= lambda x,dx: dx/x**0.5 / 2)
+def exp(x):
+    function_ = array_function if type(x) in (list, RichArray) else function
+    return function_('np.exp({})', x, domain=[0,np.inf], elementwise=True,
+                     unc_function= lambda x,dx: dx*np.exp(x))
+def log(x):
+    function_ = function if type(x) in (str, RichValue) else array_function
+    return function_('np.log({})', x, domain=[-np.inf,np.inf],
+                     unc_function= lambda x,dx: dx/x, elementwise=True)
+def log10(x):
+    function_ = function if type(x) in (str, RichValue) else array_function
+    return function_('np.log10({})', x, domain=[-np.inf,np.inf],
+                unc_function= lambda x,dx: dx/x / np.log(10), elementwise=True)
+def sin(x):
+    function_ = function if type(x) in (str, RichValue) else array_function
+    return function_('np.sin({})', x, domain=[-1,1], elementwise=True,
+        unc_function= lambda x,dx: dx * np.abs(np.cos(x)))
+def cos(x):
+    function_ = function if type(x) in (str, RichValue) else array_function
+    return function_('np.cos({})', x, domain=[-1,1], elementwise=True,
+                     unc_function= lambda x,dx: dx * np.abs(np.sin(x)))
+def tan(x):
+    function_ = function if type(x) in (str, RichValue) else array_function
+    return function_('np.tan({})', x, domain=[-1,1], elementwise=True,
+                     unc_function= lambda x,dx: dx * np.abs(1/np.cos(x)**2))
+def arcsin(x):
+    function_ = function if type(x) in (str, RichValue) else array_function
+    return function_('np.arcsin({})', x, domain=[-math.tau/4,math.tau/4],
+             unc_function= lambda x,dx: dx / (1 - x**2)**0.5, elementwise=True)
+def arccos(x):
+    function_ = function if type(x) in (str, RichValue) else array_function
+    return function_('np.arccos({})', x, domain=[-math.tau/4,math.tau/4],
+             unc_function= lambda x,dx: dx / (1 - x**2)**0.5, elementwise=True)
+def arctan(x):
+    function_ = function if type(x) in (str, RichValue) else array_function
+    return function_('np.arctan({})', x, domain=[-math.tau/4,math.tau/4],
+                  unc_function= lambda x,dx: dx / (1 + x**2), elementwise=True)
+def sinh(x):
+    function_ = function if type(x) in (str, RichValue) else array_function
+    return function_('np.sinh({})', x, domain=[-np.inf,np.inf],
+          unc_function= lambda x,dx: dx * np.abs(np.cosh(x)), elementwise=True)
+def cosh(x):
+    function_ = function if type(x) in (str, RichValue) else array_function
+    return function_('np.cos({})', x, domain=[-np.inf,np.inf],
+          unc_function= lambda x,dx: dx * np.abs(np.sinh(x)), elementwise=True)
+def tanh(x):
+    function_ = function if type(x) in (str, RichValue) else array_function
+    return function_('np.tan({})', x, domain=[-np.inf,np.inf],
+       unc_function= lambda x,dx: dx*np.abs(1/np.cosh(x)**2), elementwise=True)
+def arcsinh(x):
+    function_ = function if type(x) in (str, RichValue) else array_function
+    return function_('np.arcsin({})', x, domain=[-math.tau/4,math.tau/4],
+             unc_function= lambda x,dx: dx / (x**2 + 1)**0.5, elementwise=True)
+def arccosh(x):
+    function_ = function if type(x) in (str, RichValue) else array_function
+    return function_('np.arccos({})', x, domain=[-math.tau/4,math.tau/4],
+             unc_function= lambda x,dx: dx / (x**2 - 1)**0.5, elementwise=True)
+def arctanh(x):
+    function_ = function if type(x) in (str, RichValue) else array_function
+    return function_('np.arctan({})', x, domain=[-math.tau/4,math.tau/4],
+                    unc_function= lambda x,dx: dx / (1-x**2), elementwise=True)
+
+# Function acronyms.
 rval = rich_value
 rarray = rich_array
-rich_df = rich_dataframe
+rich_df = rdataframe = rich_dataframe
 function = function_with_rich_values
 array_function = function_with_rich_arrays
-
+distribution = distr_with_rich_values
+evaluate_distribution = evaluate_distr
+center_and_uncertainties = center_and_uncs
+is_not_a_number = is_nan = isnan
+is_infinite = is_inf = isinf
+is_finite = is_finite = isfinite
```

### Comparing `richvalues-2.0.0/richvalues.egg-info/PKG-INFO` & `richvalues-3.0.0/richvalues.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 2.0.0
+Version: 3.0.0
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Description: # RichValues
         
-        Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. Moreover, it allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals.
+        Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
         
         The libraries NumPy, Pandas, SciPy and Matplotlib are required. An user guide is available on the GitHub repository: https://github.com/andresmegias/richvalues.
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `richvalues-2.0.0/setup.py` & `richvalues-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name = 'richvalues',
-    version = '2.0.0',
+    version = '3.0.0',
     license = 'BSD-3-Clause',
     author = 'Andrés Megías Toledano',
     description = 'Python library for working with uncertainties and upper/lower limits',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     packages = setuptools.find_packages('./'),
     url = 'https://github.com/andresmegias/richvalues',
```


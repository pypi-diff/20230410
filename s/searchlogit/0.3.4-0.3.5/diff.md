# Comparing `tmp/searchlogit-0.3.4.tar.gz` & `tmp/searchlogit-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchlogit-0.3.4.tar", last modified: Sun Apr  9 07:39:11 2023, max compression
+gzip compressed data, was "searchlogit-0.3.5.tar", last modified: Mon Apr 10 02:52:45 2023, max compression
```

## Comparing `searchlogit-0.3.4.tar` & `searchlogit-0.3.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:39:11.129745 searchlogit-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-09 07:39:01.000000 searchlogit-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-09 07:39:11.129745 searchlogit-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-09 07:39:01.000000 searchlogit-0.3.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:39:11.129745 searchlogit-0.3.4/searchlogit/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-09 07:39:02.000000 searchlogit-0.3.4/searchlogit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29646 2023-04-09 07:39:02.000000 searchlogit-0.3.4/searchlogit/_choice_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-09 07:39:02.000000 searchlogit-0.3.4/searchlogit/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-09 07:39:02.000000 searchlogit-0.3.4/searchlogit/boxcox_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    50431 2023-04-09 07:39:02.000000 searchlogit-0.3.4/searchlogit/latent_class_mixed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    35382 2023-04-09 07:39:02.000000 searchlogit-0.3.4/searchlogit/latent_class_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    60055 2023-04-09 07:39:02.000000 searchlogit-0.3.4/searchlogit/mixed_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14368 2023-04-09 07:39:02.000000 searchlogit-0.3.4/searchlogit/multinomial_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)   168245 2023-04-09 07:39:02.000000 searchlogit-0.3.4/searchlogit/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:39:11.129745 searchlogit-0.3.4/searchlogit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-09 07:39:11.000000 searchlogit-0.3.4/searchlogit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-09 07:39:11.000000 searchlogit-0.3.4/searchlogit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 07:39:11.000000 searchlogit-0.3.4/searchlogit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 07:39:10.000000 searchlogit-0.3.4/searchlogit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-09 07:39:11.000000 searchlogit-0.3.4/searchlogit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 07:39:11.000000 searchlogit-0.3.4/searchlogit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-09 07:39:11.129745 searchlogit-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-09 07:39:02.000000 searchlogit-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:39:11.129745 searchlogit-0.3.4/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-04-09 07:39:02.000000 searchlogit-0.3.4/tests/test__choice_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-04-09 07:39:02.000000 searchlogit-0.3.4/tests/test__device.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-09 07:39:02.000000 searchlogit-0.3.4/tests/test_latent_class_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-09 07:39:02.000000 searchlogit-0.3.4/tests/test_mixed_logit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2862 2023-04-09 07:39:02.000000 searchlogit-0.3.4/tests/test_multinomial_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 07:39:02.000000 searchlogit-0.3.4/tests/test_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:52:45.610794 searchlogit-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-10 02:52:34.000000 searchlogit-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-10 02:52:45.610794 searchlogit-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-10 02:52:34.000000 searchlogit-0.3.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:52:45.606793 searchlogit-0.3.5/searchlogit/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-10 02:52:34.000000 searchlogit-0.3.5/searchlogit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29646 2023-04-10 02:52:34.000000 searchlogit-0.3.5/searchlogit/_choice_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-10 02:52:34.000000 searchlogit-0.3.5/searchlogit/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-10 02:52:34.000000 searchlogit-0.3.5/searchlogit/boxcox_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50431 2023-04-10 02:52:34.000000 searchlogit-0.3.5/searchlogit/latent_class_mixed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35382 2023-04-10 02:52:34.000000 searchlogit-0.3.5/searchlogit/latent_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60055 2023-04-10 02:52:34.000000 searchlogit-0.3.5/searchlogit/mixed_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14368 2023-04-10 02:52:34.000000 searchlogit-0.3.5/searchlogit/multinomial_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169496 2023-04-10 02:52:34.000000 searchlogit-0.3.5/searchlogit/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:52:45.606793 searchlogit-0.3.5/searchlogit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-10 02:52:45.000000 searchlogit-0.3.5/searchlogit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-10 02:52:45.000000 searchlogit-0.3.5/searchlogit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 02:52:45.000000 searchlogit-0.3.5/searchlogit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 02:52:45.000000 searchlogit-0.3.5/searchlogit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-10 02:52:45.000000 searchlogit-0.3.5/searchlogit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 02:52:45.000000 searchlogit-0.3.5/searchlogit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-10 02:52:45.610794 searchlogit-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-10 02:52:34.000000 searchlogit-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:52:45.610794 searchlogit-0.3.5/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-04-10 02:52:34.000000 searchlogit-0.3.5/tests/test__choice_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-04-10 02:52:34.000000 searchlogit-0.3.5/tests/test__device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-10 02:52:34.000000 searchlogit-0.3.5/tests/test_latent_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-10 02:52:34.000000 searchlogit-0.3.5/tests/test_mixed_logit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2862 2023-04-10 02:52:34.000000 searchlogit-0.3.5/tests/test_multinomial_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 02:52:34.000000 searchlogit-0.3.5/tests/test_search.py
```

### Comparing `searchlogit-0.3.4/LICENSE` & `searchlogit-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.4/PKG-INFO` & `searchlogit-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchlogit
-Version: 0.3.4
+Version: 0.3.5
 Summary: Extensions for a Python package for                               GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/RyanJafefKelly/searchlogit
 Author: Ryan Kelly, Prithvi Beeramoole and Alexander Paz
 Author-email: ryan@kiiii.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
```

### Comparing `searchlogit-0.3.4/README.rst` & `searchlogit-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.4/searchlogit/_choice_model.py` & `searchlogit-0.3.5/searchlogit/_choice_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.4/searchlogit/_device.py` & `searchlogit-0.3.5/searchlogit/_device.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.4/searchlogit/boxcox_functions.py` & `searchlogit-0.3.5/searchlogit/boxcox_functions.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.4/searchlogit/latent_class_mixed_model.py` & `searchlogit-0.3.5/searchlogit/latent_class_mixed_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.4/searchlogit/latent_class_model.py` & `searchlogit-0.3.5/searchlogit/latent_class_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.4/searchlogit/mixed_logit.py` & `searchlogit-0.3.5/searchlogit/mixed_logit.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.4/searchlogit/multinomial_logit.py` & `searchlogit-0.3.5/searchlogit/multinomial_logit.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.4/searchlogit/search.py` & `searchlogit-0.3.5/searchlogit/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1973,43 +1973,44 @@
 
             new_sol = self.generate_sol()
             logger.debug("new sol after HMC-2: {}".format(new_sol))
         return new_sol
 
     def add_new_asfeature(self, solution):
         """
-        Randomly selects an as variable, which is not already in solution
+        Randomly selects an as variable, which is not already in solution.
         Inputs: solution list containing all features generated from harmony consideration
         """
         new_asvar = [var for var in self.asvarnames if var not in solution['asvars']]
         logger.debug('new_asvar: {}'.format(new_asvar))
         if new_asvar:
             n_asvar = list(self.random_state.choice(new_asvar, 1))
             solution['asvars'].extend(n_asvar)
             solution['asvars'] = self.remove_redundant_asvars(solution['asvars'],
                                                        self.trans_asvars,
                                                        self.asvarnames)
             solution['asvars'] = sorted(list(set(solution['asvars'])))
             logger.debug("new sol: {}".format(str(solution['asvars'])))
 
+            # randvar logic for selected asvar
             r_vars = {}
             if self.allow_random:
                 for i in solution['asvars']:
                     if i in solution['randvars'].keys():
                         r_vars.update({k: v for k, v in solution['randvars'].items()
                                        if k == i})
                         logger.debug("r_vars: {}".format(r_vars))
                     else:
                         if i in self.ps_randvars.keys():
                             r_vars.update({i: self.ps_randvars[i]})
                             logger.debug("r_vars: {}".format(r_vars))
-                        else:
-                            if len(self.dist) > 0:
-                                r_vars.update({i: self.random_state.choice(self.dist)})
-                            logger.debug("r_vars: {}".format(r_vars))
+                        # else:
+                        #     if len(self.dist) > 0:
+                        #         r_vars.update({i: self.random_state.choice(self.dist)})
+                        #     logger.debug("r_vars: {}".format(r_vars))
                 solution['randvars'] = {k: v for k, v in r_vars.items() if k
                                         in solution['asvars'] and v != 'f'}
 
         if solution['corvars']:
             solution['corvars'] = [var for var in solution['corvars']
                                    if var in solution['randvars'].keys()
                                    and var not in solution['bcvars']]
@@ -2286,14 +2287,31 @@
         solution['member_params_spec'] = member_params_spec
         if rem_member_param not in np.concatenate(member_params_spec):
             solution['isvars'] = [var for var in solution['isvars']
                                   if var != rem_member_param]
 
         return solution
 
+    def change_random_distribution(self, solution):
+        if solution['randvars']:
+            randvar_options = [randvar for randvar in solution['randvars']
+                               if randvar not in self.ps_randvars]
+            selected_randvar = self.random_state.choice(randvar_options)
+            dist_tmp = self.dist.copy()
+            # remove current dist for selected_randvar from options
+            dist_tmp.remove(solution['randvars'][selected_randvar])
+            new_dist = self.random_state.choice(dist_tmp)
+            solution['randvars'][selected_randvar] = new_dist
+            if selected_randvar in solution['corvars'] and new_dist != 'n':
+                # corvars need to be normally distributed
+                solution['corvars'] = [var for var in solution['corvars']
+                                       if var != selected_randvar]
+        return solution
+
+
     def assess_sol(self, solution, har_mem):
         """
         (1) Evaluates the objective function of a given solution
         (2) Evaluates if the solution provides an improvement in BIC by atleast a threshold value compared to any other solution in memory
         (3) Checks if the solution is unique to other solutions in memory
         (4) Replaces the worst solution in memory, if (2) and (3) are true
         Inputs: solution list containing all features, harmony memory
@@ -2371,14 +2389,17 @@
                     pa_sol = self.add_new_randfeature(pa_sol)
                 else:
                     if sol['randvars']:
                         logger.debug("pitch adjustment by removing random variables")
                         pa_sol = self.remove_randfeature(pa_sol)
 
         if self.random_state.rand() <= PAR_itr:
+            pa_sol = self.change_random_distribution(pa_sol)
+
+        if self.random_state.rand() <= PAR_itr:
             if self.ps_bctrans is None or self.ps_bctrans:
                 if self.random_state.rand() <= 0.5:
                     logger.debug("pitch adjustment adding bc variables")
                     pa_sol = self.add_new_bcfeature(pa_sol, PAR_itr)
                 else:
                     logger.debug("pitch adjustment by removing bc variables")
                     pa_sol = self.remove_bcfeature(pa_sol)
@@ -2459,18 +2480,22 @@
                                                            best_bcvars,
                                                            best_corvars,
                                                            best_class_params_spec,
                                                            best_member_params_spec))
         # for each additional feature to the best solution, the objective function is tested
 
         # Check if changing coefficient distributions of best solution improves the solution BIC
-        for var in best_randvars.keys():
-            if var not in self.ps_randvars:
-                rm_dist = [dis for dis in self.dist if dis != best_randvars[var]]
-                best_randvars[var] = self.random_state.choice(rm_dist)
+        solution_1 = Solution(asvars=best_asvars, isvars=best_isvars,
+                              randvars=best_randvars, bcvars=best_bcvars,
+                              corvars=best_corvars, asc_ind=asc_ind,
+                              class_params_spec=best_class_params_spec,
+                              member_params_spec=best_member_params_spec)
+
+        solution_1 = self.change_random_distribution(solution_1)
+
         best_randvars = {key: val for key, val in best_randvars.items()
                          if key in best_asvars and val != 'f'}
         best_bcvars = [var for var in best_bcvars if var in best_asvars
                        and var not in self.ps_corvars]
         best_corvars = [var for var in best_randvars.keys() if var
                         not in best_bcvars]
         solution_1 = Solution(asvars=best_asvars, isvars=best_isvars,
```

### Comparing `searchlogit-0.3.4/searchlogit.egg-info/PKG-INFO` & `searchlogit-0.3.5/searchlogit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchlogit
-Version: 0.3.4
+Version: 0.3.5
 Summary: Extensions for a Python package for                               GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/RyanJafefKelly/searchlogit
 Author: Ryan Kelly, Prithvi Beeramoole and Alexander Paz
 Author-email: ryan@kiiii.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
```

### Comparing `searchlogit-0.3.4/searchlogit.egg-info/SOURCES.txt` & `searchlogit-0.3.5/searchlogit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.4/setup.py` & `searchlogit-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import setuptools
 
 with codecs.open("README.rst", encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(name='searchlogit',
-                 version='0.3.4',
+                 version='0.3.5',
                  description='Extensions for a Python package for \
                               GPU-accelerated estimation of mixed logit models.',
                  long_description=long_description,
                  long_description_content_type="text/x-rst",
                  url='https://github.com/RyanJafefKelly/searchlogit',
                  author='Ryan Kelly, Prithvi Beeramoole and Alexander Paz',
                  author_email='ryan@kiiii.com',
```

### Comparing `searchlogit-0.3.4/tests/test__choice_model.py` & `searchlogit-0.3.5/tests/test__choice_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.4/tests/test__device.py` & `searchlogit-0.3.5/tests/test__device.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.4/tests/test_latent_class_model.py` & `searchlogit-0.3.5/tests/test_latent_class_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.4/tests/test_mixed_logit.py` & `searchlogit-0.3.5/tests/test_mixed_logit.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.4/tests/test_multinomial_logit.py` & `searchlogit-0.3.5/tests/test_multinomial_logit.py`

 * *Files identical despite different names*


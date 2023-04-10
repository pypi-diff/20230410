# Comparing `tmp/ikpy-3.3.3.tar.gz` & `tmp/ikpy-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/ikpy/ikpy/dist/tmpo3ewklyc/ikpy-3.3.3.tar", last modified: Sun May 15 17:01:58 2022, max compression
+gzip compressed data, was "/home/runner/work/ikpy/ikpy/dist/.tmp-4t184daz/ikpy-3.3.4.tar", last modified: Mon Apr 10 16:29:21 2023, max compression
```

## Comparing `ikpy-3.3.3.tar` & `ikpy-3.3.4.tar`

### file list

```diff
@@ -1,28 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 17:01:58.000000 ikpy-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (121)    18047 2022-05-15 17:01:45.000000 ikpy-3.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4109 2022-05-15 17:01:58.000000 ikpy-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3766 2022-05-15 17:01:45.000000 ikpy-3.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-05-15 17:01:45.000000 ikpy-3.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-05-15 17:01:58.000000 ikpy-3.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 17:01:58.000000 ikpy-3.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 17:01:58.000000 ikpy-3.3.3/src/ikpy/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-05-15 17:01:45.000000 ikpy-3.3.3/src/ikpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-15 17:01:45.000000 ikpy-3.3.3/src/ikpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    12620 2022-05-15 17:01:45.000000 ikpy-3.3.3/src/ikpy/chain.py
--rw-r--r--   0 runner    (1001) docker     (121)     5149 2022-05-15 17:01:45.000000 ikpy-3.3.3/src/ikpy/inverse_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (121)    11125 2022-05-15 17:01:45.000000 ikpy-3.3.3/src/ikpy/link.py
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-05-15 17:01:45.000000 ikpy-3.3.3/src/ikpy/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 17:01:58.000000 ikpy-3.3.3/src/ikpy/urdf/
--rw-r--r--   0 runner    (1001) docker     (121)    11534 2022-05-15 17:01:45.000000 ikpy-3.3.3/src/ikpy/urdf/URDF.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-15 17:01:45.000000 ikpy-3.3.3/src/ikpy/urdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4477 2022-05-15 17:01:45.000000 ikpy-3.3.3/src/ikpy/urdf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 17:01:58.000000 ikpy-3.3.3/src/ikpy/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-15 17:01:45.000000 ikpy-3.3.3/src/ikpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5425 2022-05-15 17:01:45.000000 ikpy-3.3.3/src/ikpy/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (121)     4523 2022-05-15 17:01:45.000000 ikpy-3.3.3/src/ikpy/utils/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-15 17:01:58.000000 ikpy-3.3.3/src/ikpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4109 2022-05-15 17:01:57.000000 ikpy-3.3.3/src/ikpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-05-15 17:01:58.000000 ikpy-3.3.3/src/ikpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-15 17:01:57.000000 ikpy-3.3.3/src/ikpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-15 17:01:58.000000 ikpy-3.3.3/src/ikpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-05-15 17:01:58.000000 ikpy-3.3.3/src/ikpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:29:21.000000 ikpy-3.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 16:29:10.000000 ikpy-3.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-10 16:29:21.000000 ikpy-3.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-10 16:29:10.000000 ikpy-3.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-10 16:29:10.000000 ikpy-3.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-10 16:29:21.000000 ikpy-3.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:29:21.000000 ikpy-3.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:29:21.000000 ikpy-3.3.4/src/ikpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-10 16:29:10.000000 ikpy-3.3.4/src/ikpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 16:29:10.000000 ikpy-3.3.4/src/ikpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-04-10 16:29:10.000000 ikpy-3.3.4/src/ikpy/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-10 16:29:10.000000 ikpy-3.3.4/src/ikpy/inverse_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-04-10 16:29:10.000000 ikpy-3.3.4/src/ikpy/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-10 16:29:10.000000 ikpy-3.3.4/src/ikpy/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:29:21.000000 ikpy-3.3.4/src/ikpy/urdf/
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-04-10 16:29:10.000000 ikpy-3.3.4/src/ikpy/urdf/URDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:29:10.000000 ikpy-3.3.4/src/ikpy/urdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-04-10 16:29:10.000000 ikpy-3.3.4/src/ikpy/urdf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:29:21.000000 ikpy-3.3.4/src/ikpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:29:10.000000 ikpy-3.3.4/src/ikpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-04-10 16:29:10.000000 ikpy-3.3.4/src/ikpy/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-10 16:29:10.000000 ikpy-3.3.4/src/ikpy/utils/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:29:21.000000 ikpy-3.3.4/src/ikpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-10 16:29:21.000000 ikpy-3.3.4/src/ikpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-10 16:29:21.000000 ikpy-3.3.4/src/ikpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:29:21.000000 ikpy-3.3.4/src/ikpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-10 16:29:21.000000 ikpy-3.3.4/src/ikpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 16:29:21.000000 ikpy-3.3.4/src/ikpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:29:21.000000 ikpy-3.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-10 16:29:10.000000 ikpy-3.3.4/tests/test_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-10 16:29:10.000000 ikpy-3.3.4/tests/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-10 16:29:10.000000 ikpy-3.3.4/tests/test_poppy_robots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-10 16:29:10.000000 ikpy-3.3.4/tests/test_urdf.py
```

### Comparing `ikpy-3.3.3/PKG-INFO` & `ikpy-3.3.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ikpy
-Version: 3.3.3
+Version: 3.3.4
 Summary: An inverse kinematics library aiming performance and modularity
 Home-page: https://github.com/Phylliade/ikpy
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 Provides-Extra: plot
 License-File: LICENSE
 
 # IKPy
 
 [![PyPI](https://img.shields.io/pypi/v/ikpy.svg)](https://pypi.python.org/pypi/ikpy/)
 
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6551106.svg)](https://doi.org/10.5281/zenodo.6551106)
 
 ![demo](two_arms.png)
 
 ![IKPy on the baxter robot](baxter.png)
 
 ## Demo
 
@@ -106,15 +107,20 @@
 * If performance is your main concern, `aversive++` has an inverse kinematics [module](https://github.com/AversivePlusPlus/ik) written in C++, which works the same way IKPy does.
 
 ## Citation
 
 If you use IKPy as part of a publication, please use the Bibtex below as a citation:
 
 ```bibtex
-@software{Manceron_IKPy,
-doi = {10.5281/ZENODO.6551105},
-author = {Manceron, Pierre},
-license = {GPL-2.0},
-title = {{IKPy}},
-url = {https://github.com/Phylliade/ikpy}
+@software{manceron_pierre_2022_6551158,
+  author       = {Manceron, Pierre},
+  title        = {IKPy},
+  month        = may,
+  year         = 2022,
+  note         = {{If you use this software, please cite it using the 
+                   metadata from this file.}},
+  publisher    = {Zenodo},
+  version      = {v3.3.3},
+  doi          = {10.5281/zenodo.6551158},
+  url          = {https://doi.org/10.5281/zenodo.6551158}
 }
 ```
```

### Comparing `ikpy-3.3.3/README.md` & `ikpy-3.3.4/src/ikpy.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,23 @@
+Metadata-Version: 2.1
+Name: ikpy
+Version: 3.3.4
+Summary: An inverse kinematics library aiming performance and modularity
+Home-page: https://github.com/Phylliade/ikpy
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Description-Content-Type: text/markdown
+Provides-Extra: plot
+License-File: LICENSE
+
 # IKPy
 
 [![PyPI](https://img.shields.io/pypi/v/ikpy.svg)](https://pypi.python.org/pypi/ikpy/)
 
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6551106.svg)](https://doi.org/10.5281/zenodo.6551106)
 
 ![demo](two_arms.png)
 
 ![IKPy on the baxter robot](baxter.png)
 
 ## Demo
 
@@ -95,15 +107,20 @@
 * If performance is your main concern, `aversive++` has an inverse kinematics [module](https://github.com/AversivePlusPlus/ik) written in C++, which works the same way IKPy does.
 
 ## Citation
 
 If you use IKPy as part of a publication, please use the Bibtex below as a citation:
 
 ```bibtex
-@software{Manceron_IKPy,
-doi = {10.5281/ZENODO.6551105},
-author = {Manceron, Pierre},
-license = {GPL-2.0},
-title = {{IKPy}},
-url = {https://github.com/Phylliade/ikpy}
+@software{manceron_pierre_2022_6551158,
+  author       = {Manceron, Pierre},
+  title        = {IKPy},
+  month        = may,
+  year         = 2022,
+  note         = {{If you use this software, please cite it using the 
+                   metadata from this file.}},
+  publisher    = {Zenodo},
+  version      = {v3.3.3},
+  doi          = {10.5281/zenodo.6551158},
+  url          = {https://doi.org/10.5281/zenodo.6551158}
 }
-```
+```
```

### Comparing `ikpy-3.3.3/setup.cfg` & `ikpy-3.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `ikpy-3.3.3/src/ikpy/chain.py` & `ikpy-3.3.4/src/ikpy/chain.py`

 * *Files identical despite different names*

### Comparing `ikpy-3.3.3/src/ikpy/inverse_kinematics.py` & `ikpy-3.3.4/src/ikpy/inverse_kinematics.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 from . import logs
 
 
 ORIENTATION_COEFF = 1.
 
 
-def inverse_kinematic_optimization(chain, target_frame, starting_nodes_angles, regularization_parameter=None, max_iter=None, orientation_mode=None, no_position=False):
+def inverse_kinematic_optimization(chain, target_frame, starting_nodes_angles, regularization_parameter=None, max_iter=None, orientation_mode=None, no_position=False, optimizer="least_squares"):
     """
     Computes the inverse kinematic on the specified target
 
     Parameters
     ----------
     chain: ikpy.chain.Chain
         The chain used for the Inverse kinematics.
@@ -28,15 +28,22 @@
         * None: No orientation
         * "X": Target the X axis
         * "Y": Target the Y axis
         * "Z": Target the Z axis
         * "all": Target the three axes
     no_position: bool
         Do not optimize against position
+    optimizer: str
+        The optimizer to use. Choices:
+        * "least_squares": Use scipy.optimize.least_squares
+        * "scalar": Use scipy.optimize.minimize
     """
+    if optimizer not in ["least_squares", "scalar"]:
+        raise ValueError("Unknown solver: {}".format(optimizer))
+
     # Begin with the position
     target = target_frame[:3, -1]
 
     # Initial function call when optimizing
     def optimize_basis(x):
         # y = np.append(starting_nodes_angles[:chain.first_active_joint], x)
         y = chain.active_to_full(x, starting_nodes_angles)
@@ -120,23 +127,30 @@
             return optimize_function(x) + regularization_parameter * regularization
     else:
         optimize_total = optimize_function
 
     # Compute bounds
     real_bounds = [link.bounds for link in chain.links]
     # real_bounds = real_bounds[chain.first_active_joint:]
-    real_bounds = np.moveaxis(chain.active_from_full(real_bounds), -1, 0)
+    real_bounds = chain.active_from_full(real_bounds)
 
     logs.logger.info("Bounds: {}".format(real_bounds))
 
     if max_iter is not None:
         logs.logger.info("max_iter is not used anymore in the IK, using it as a parameter will raise an exception in the future")
 
     # least squares optimization
-    res = scipy.optimize.least_squares(optimize_total, chain.active_from_full(starting_nodes_angles), bounds=real_bounds)
+    if optimizer == "scalar":
+        def optimize_scalar(x):
+            return np.linalg.norm(optimize_total(x))
+        res = scipy.optimize.minimize(optimize_scalar, chain.active_from_full(starting_nodes_angles), bounds=real_bounds)
+    elif optimizer == "least_squares":
+        # We need to unzip the bounds
+        real_bounds = np.moveaxis(real_bounds, -1, 0)
+        res = scipy.optimize.least_squares(optimize_total, chain.active_from_full(starting_nodes_angles), bounds=real_bounds)
 
     if res.status != -1:
         logs.logger.info("Inverse kinematic optimisation OK, termination status: {}".format(res.status))
     else:
         logs.logger.warning("Inverse kinematic optimisation returned an error: termination status: {}".format(res.status))
 
     return chain.active_to_full(res.x, starting_nodes_angles)
```

### Comparing `ikpy-3.3.3/src/ikpy/link.py` & `ikpy-3.3.4/src/ikpy/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,35 +133,35 @@
             self.translation = np.array(translation)
         else:
             self.has_translation = False
             self.translation = None
 
         # Check that the given joint type matches the given parameters
         if joint_type == "revolute":
-            if not(self.has_rotation and not self.has_translation):
+            if not (self.has_rotation and not self.has_translation):
                 raise ValueError("Joint type is 'revolute' but rotation axis = {} and translation axis = {}".format(self.has_rotation, self.has_translation))
         elif joint_type == "prismatic":
-            if not(not self.has_rotation and self.has_translation):
+            if not (not self.has_rotation and self.has_translation):
                 raise ValueError("Joint type is 'prismatic' but rotation axis = {} and translation axis = {}".format(self.has_rotation, self.has_translation))
         elif joint_type == "fixed":
-            if not(not self.has_rotation and not self.has_translation):
+            if not (not self.has_rotation and not self.has_translation):
                 raise ValueError("Joint type is 'fixed' but rotation axis = {} and translation axis = {}".format(self.has_rotation, self.has_translation))
 
         else:
             raise ValueError("Unknown joint type: {}".format(joint_type))
         self.joint_type = joint_type
 
         if use_symbolic_matrix:
             # Angle symbolique qui paramètre la rotation du joint en cours
             theta = sympy.symbols("theta")
             mu = sympy.symbols("mu")
             self.symbolic_transformation_matrix = self._apply_geometric_transformations(theta=theta, mu=mu, symbolic=True)
 
     def __repr__(self):
-        return("""URDF Link {} :
+        return ("""URDF Link {} :
     Type : {}
     Bounds : {}
     Origin Translation : {}
     Origin Orientation : {}
     Rotation : {}
     Translation: {}""".format(self.name, self.joint_type, self.bounds, self.origin_translation, self.origin_orientation, self.rotation, self.translation))
```

### Comparing `ikpy-3.3.3/src/ikpy/urdf/URDF.py` & `ikpy-3.3.4/src/ikpy/urdf/URDF.py`

 * *Files identical despite different names*

### Comparing `ikpy-3.3.3/src/ikpy/urdf/utils.py` & `ikpy-3.3.4/src/ikpy/urdf/utils.py`

 * *Files identical despite different names*

### Comparing `ikpy-3.3.3/src/ikpy/utils/geometry.py` & `ikpy-3.3.4/src/ikpy/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `ikpy-3.3.3/src/ikpy/utils/plot.py` & `ikpy-3.3.4/src/ikpy/utils/plot.py`

 * *Files identical despite different names*

### Comparing `ikpy-3.3.3/src/ikpy.egg-info/PKG-INFO` & `ikpy-3.3.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,12 @@
-Metadata-Version: 2.1
-Name: ikpy
-Version: 3.3.3
-Summary: An inverse kinematics library aiming performance and modularity
-Home-page: https://github.com/Phylliade/ikpy
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering
-Description-Content-Type: text/markdown
-Provides-Extra: plot
-License-File: LICENSE
-
 # IKPy
 
 [![PyPI](https://img.shields.io/pypi/v/ikpy.svg)](https://pypi.python.org/pypi/ikpy/)
 
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6551106.svg)](https://doi.org/10.5281/zenodo.6551106)
 
 ![demo](two_arms.png)
 
 ![IKPy on the baxter robot](baxter.png)
 
 ## Demo
 
@@ -106,15 +96,20 @@
 * If performance is your main concern, `aversive++` has an inverse kinematics [module](https://github.com/AversivePlusPlus/ik) written in C++, which works the same way IKPy does.
 
 ## Citation
 
 If you use IKPy as part of a publication, please use the Bibtex below as a citation:
 
 ```bibtex
-@software{Manceron_IKPy,
-doi = {10.5281/ZENODO.6551105},
-author = {Manceron, Pierre},
-license = {GPL-2.0},
-title = {{IKPy}},
-url = {https://github.com/Phylliade/ikpy}
+@software{manceron_pierre_2022_6551158,
+  author       = {Manceron, Pierre},
+  title        = {IKPy},
+  month        = may,
+  year         = 2022,
+  note         = {{If you use this software, please cite it using the 
+                   metadata from this file.}},
+  publisher    = {Zenodo},
+  version      = {v3.3.3},
+  doi          = {10.5281/zenodo.6551158},
+  url          = {https://doi.org/10.5281/zenodo.6551158}
 }
 ```
```


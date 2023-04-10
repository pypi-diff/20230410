# Comparing `tmp/openpile-0.0.1.tar.gz` & `tmp/openpile-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/openpile/openpile/dist/.tmp-k5ip6dtu/openpile-0.0.1.tar", last modified: Fri Mar 31 11:51:54 2023, max compression
+gzip compressed data, was "/home/runner/work/openpile/openpile/dist/.tmp-g6d0dqm8/openpile-0.1.0.tar", last modified: Mon Apr 10 19:22:42 2023, max compression
```

## Comparing `openpile-0.0.1.tar` & `openpile-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:51:54.000000 openpile-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-31 11:51:42.000000 openpile-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-03-31 11:51:54.000000 openpile-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-03-31 11:51:42.000000 openpile-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-31 11:51:42.000000 openpile-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-03-31 11:51:54.000000 openpile-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-31 11:51:42.000000 openpile-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:51:54.000000 openpile-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:51:54.000000 openpile-0.0.1/src/openpile/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-31 11:51:42.000000 openpile-0.0.1/src/openpile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-03-31 11:51:42.000000 openpile-0.0.1/src/openpile/analyses.py
--rw-r--r--   0 runner    (1001) docker     (123)    43560 2023-03-31 11:51:42.000000 openpile-0.0.1/src/openpile/construct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:51:54.000000 openpile-0.0.1/src/openpile/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 11:51:42.000000 openpile-0.0.1/src/openpile/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16515 2023-03-31 11:51:42.000000 openpile-0.0.1/src/openpile/core/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-03-31 11:51:42.000000 openpile-0.0.1/src/openpile/core/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-03-31 11:51:42.000000 openpile-0.0.1/src/openpile/core/txt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-03-31 11:51:42.000000 openpile-0.0.1/src/openpile/core/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-31 11:51:42.000000 openpile-0.0.1/src/openpile/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-03-31 11:51:42.000000 openpile-0.0.1/src/openpile/soilmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:51:54.000000 openpile-0.0.1/src/openpile/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 11:51:42.000000 openpile-0.0.1/src/openpile/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-03-31 11:51:42.000000 openpile-0.0.1/src/openpile/utils/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-03-31 11:51:42.000000 openpile-0.0.1/src/openpile/utils/py_curves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:51:54.000000 openpile-0.0.1/src/openpile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-03-31 11:51:54.000000 openpile-0.0.1/src/openpile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-31 11:51:54.000000 openpile-0.0.1/src/openpile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 11:51:54.000000 openpile-0.0.1/src/openpile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 11:51:54.000000 openpile-0.0.1/src/openpile.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-31 11:51:54.000000 openpile-0.0.1/src/openpile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 11:51:54.000000 openpile-0.0.1/src/openpile.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:51:54.000000 openpile-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-31 11:51:42.000000 openpile-0.0.1/test/test_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-31 11:51:42.000000 openpile-0.0.1/test/test_utils_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:22:42.000000 openpile-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-10 19:22:26.000000 openpile-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-10 19:22:42.000000 openpile-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-10 19:22:26.000000 openpile-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-10 19:22:26.000000 openpile-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-10 19:22:42.000000 openpile-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-10 19:22:26.000000 openpile-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:22:42.000000 openpile-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/analyses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47018 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/construct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25780 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/core/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/core/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/core/txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/core/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/soilmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/utils/Hb_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/utils/Mb_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/utils/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/utils/mt_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/utils/py_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/utils/qz_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/utils/tz_curves.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:22:42.000000 openpile-0.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-04-10 19:22:26.000000 openpile-0.1.0/test/test_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-10 19:22:26.000000 openpile-0.1.0/test/test_pycurves.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-10 19:22:26.000000 openpile-0.1.0/test/test_utils_misc.py
```

### Comparing `openpile-0.0.1/LICENSE.txt` & `openpile-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openpile-0.0.1/PKG-INFO` & `openpile-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpile
-Version: 0.0.1
+Version: 0.1.0
 Summary: Library for geotechnical pile calculations.
 Home-page: https://github.com/TchilDill/openpile
 Author: Guillaume Melin
 Author-email: guillaume.melin@icloud.com
 License: GPLv3
 Keywords: Offshore Wind,PILE,Geotechnics,monopile,pin-piles,Geotechnical,calculations,PISA,winkler
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
-# openpile
+# OpenPile
 
 Geotechnical super-toolbox for pile-related calculations.
 
 <!-- [![Python Support](https://img.shields.io/pypi/pyversions/openpile.svg)](https://pypi.org/project/openpile/) -->
 [![License: LGPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/)
 
@@ -65,12 +65,12 @@
    * Out-of-the-box computation of individual soil springs
    <!-- * Axial capacity calculations via integration -->
  * Friendly API interface with  object-oriented approach
  * Fully integrated output with python environment with Matplotlib and Pandas libraries. 
 
  ## Please share with the community
 
-This library relies on community interactions. Please consider sharing a post about `openpile` and the value it can provide for researcher, academia and professionals.
+This library relies on community interactions. Please consider sharing a post about `OpenPile` and the value it can provide for researcher, academia and professionals.
 
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-reddit-red?logo=reddit)](https://reddit.com/submit?url=https://github.com/TchilDill/openpile&title=openpile)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-twitter-03A9F4?logo=twitter)](https://twitter.com/share?url=https://github.com/TchilDill/openpile&t=openpile)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-linkedin-3949AB?logo=linkedin)](https://www.linkedin.com/shareArticle?url=https://github.com/TchilDill/openpile&title=openpile)
```

### Comparing `openpile-0.0.1/README.md` & `openpile-0.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# openpile
+# OpenPile
 
 Geotechnical super-toolbox for pile-related calculations.
 
 <!-- [![Python Support](https://img.shields.io/pypi/pyversions/openpile.svg)](https://pypi.org/project/openpile/) -->
 [![License: LGPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/)
 
@@ -44,12 +44,12 @@
    * Out-of-the-box computation of individual soil springs
    <!-- * Axial capacity calculations via integration -->
  * Friendly API interface with  object-oriented approach
  * Fully integrated output with python environment with Matplotlib and Pandas libraries. 
 
  ## Please share with the community
 
-This library relies on community interactions. Please consider sharing a post about `openpile` and the value it can provide for researcher, academia and professionals.
+This library relies on community interactions. Please consider sharing a post about `OpenPile` and the value it can provide for researcher, academia and professionals.
 
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-reddit-red?logo=reddit)](https://reddit.com/submit?url=https://github.com/TchilDill/openpile&title=openpile)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-twitter-03A9F4?logo=twitter)](https://twitter.com/share?url=https://github.com/TchilDill/openpile&t=openpile)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-linkedin-3949AB?logo=linkedin)](https://www.linkedin.com/shareArticle?url=https://github.com/TchilDill/openpile&title=openpile)
```

### Comparing `openpile-0.0.1/setup.cfg` & `openpile-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `openpile-0.0.1/src/openpile/analyses.py` & `openpile-0.1.0/src/openpile/analyses.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,17 +301,22 @@
             if iter_no == 100:
                 print("Not converged after 100 iterations.")
 
             # re-calculate global stiffness matrix for next iterations
             if solver == "NR":
                 K = kernel.build_stiffness_matrix(model, u=d, kind="tangent")
             elif solver == "MNR":
-                pass
+                if model.distributed_moment:
+                    pass
+                    # K = kernel.build_stiffness_matrix(model, u=d, kind="initial")
+                else:
+                    pass
 
-            # reset displacements in case of displacement-driven analysis
+            # reset prescribed displacements to converge properly in case
+            # of displacement-driven analysis
             U[:] = 0.0
 
         # Internal forces calculations with dim(nelem,6,6)
         q_int = kernel.struct_internal_force(model, d)
 
         # Final results
         results = Result(
```

### Comparing `openpile-0.0.1/src/openpile/construct.py` & `openpile-0.1.0/src/openpile/construct.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 These objects include:
 
 - the Pile
 - the SoilProfile
   - the Layer
 - the Model
 
-Usage
------
+**Usage**
 
 >>> from openpile.construct import Pile, SoilProfile, Layer, Model
 
 """
 
 import math as m
 import pandas as pd
@@ -286,51 +285,48 @@
             self.data.loc[:, ["Wall thickness [m]"]] = pd.NA
         except AttributeError:
             print("Please first create the pile with the Pile.create() method")
         except Exception as e:
             print(e)
 
     @property
-    def area(self) -> float:
+    def width(self) -> float:
         """
         Width of the pile. (Used to compute soil springs)
         """
         try:
-            return self.data["Area [m2]"].mean()
+            return self.data["Diameter [m]"].mean()
         except AttributeError:
             print("Please first create the pile with the Pile.create() method")
         except Exception as e:
             print(e)
 
-    @area.setter
+    @width.setter
     def width(self, value: float) -> None:
         try:
-            self.data.loc[:, "Area [m2]"] = value
+            self.data.loc[:, "Diameter [m]"] = value
             self.data.loc[:, ["Wall thickness [m]"]] = pd.NA
         except AttributeError:
             print("Please first create the pile with the Pile.create() method")
         except Exception as e:
             print(e)
 
     @property
-    def width(self) -> float:
-        """
-        Width of the pile. (Used to compute soil springs)
-        """
+    def area(self) -> float:
         try:
-            return self.data["Diameter [m]"].mean()
+            return self.data["Area [m2]"].mean()
         except AttributeError:
             print("Please first create the pile with the Pile.create() method")
         except Exception as e:
             print(e)
 
-    @width.setter
-    def width(self, value: float) -> None:
+    @area.setter
+    def area(self, value: float) -> None:
         try:
-            self.data.loc[:, "Diameter [m]"] = value
+            self.data.loc[:, "Area [m2]"] = value
             self.data.loc[:, ["Wall thickness [m]"]] = pd.NA
         except AttributeError:
             print("Please first create the pile with the Pile.create() method")
         except Exception as e:
             print(e)
 
 
@@ -434,15 +430,15 @@
     >>>                 weight=19,
     >>>                 lateral_model= API_clay(Su=50, eps50=0.01, Neq=100),)
     >>>     ]
     >>> )
 
     >>> # Check soil profile content
     >>> print(sp)
-        Layer 1
+    Layer 1
     ------------------------------
     Name: Layer0
     Elevation: (0.0) - (-20.0) m
     Weight: 18.0 kN/m3
     Lateral model: 	API sand
         phi = 30.0°
         Cyclic, N = 100 cycles
@@ -606,24 +602,26 @@
     #: x coordinates values to mesh as nodes
     x2mesh: List[float] = Field(default_factory=list)
     #: mesh coarseness, represent the maximum accepted length of elements
     coarseness: float = 0.5
     #: whether to include p-y springs in the calculations
     distributed_lateral: bool = True
     #: whether to include m-t springs in the calculations
-    distributed_moment: bool = False
-    #: whether to include Hb-y springs in the calculations
-    base_shear: bool = False
-    #: whether to include Mb-t springs in the calculations
-    base_moment: bool = False
+    distributed_moment: bool = True
+    #: whether to include Hb-y spring in the calculations
+    base_shear: bool = True
+    #: whether to include Mb-t spring in the calculations
+    base_moment: bool = True
+    #: whether to include t-z springs in the calculations
+    distributed_axial: bool = False
+    #: whether to include Q-z spring in the calculations
+    base_axial: bool = False
 
     @root_validator
-    def soil_and_pile_bottom_elevation_match(
-        cls, values
-    ):  # pylint: disable=no-self-argument
+    def soil_and_pile_bottom_elevation_match(cls, values):  # pylint: disable=no-self-argument
         if values["pile"].bottom_elevation < values["soil"].bottom_elevation:
             raise UserWarning("The pile ends deeper than the soil profile.")
         return values
 
     def get_structural_properties(self) -> pd.DataFrame:
         """
         Returns a table with the structural properties of the pile sections.
@@ -643,33 +641,34 @@
             return self.soil_properties
         except AttributeError:
             print("Data not found. Please create Model with the Model.create() method.")
         except Exception as e:
             print(e)
 
     def _postinit(self):
+        def check_springs(arr):
+            check_nan = np.isnan(arr).any()
+            check_negative = (arr < 0).any()
+
+            return check_nan or check_negative
+
         def get_coordinates() -> pd.DataFrame:
             # Primary discretisation over x-axis
             x = np.array([], dtype=np.float16)
             # add get pile relevant sections
             x = np.append(x, self.pile.data["Elevation [m]"].values)
             # add soil relevant layers and others
             if self.soil is not None:
                 soil_elevations = np.array(
-                    [x.top for x in self.soil.layers]
-                    + [x.bottom for x in self.soil.layers],
+                    [x.top for x in self.soil.layers] + [x.bottom for x in self.soil.layers],
                     dtype=float,
                 )
                 if any(soil_elevations < self.pile.bottom_elevation):
-                    soil_elevations = np.append(
-                        self.pile.bottom_elevation, soil_elevations
-                    )
-                    soil_elevations = soil_elevations[
-                        soil_elevations >= self.pile.bottom_elevation
-                    ]
+                    soil_elevations = np.append(self.pile.bottom_elevation, soil_elevations)
+                    soil_elevations = soil_elevations[soil_elevations >= self.pile.bottom_elevation]
                 x = np.append(x, soil_elevations)
             # add user-defined elevation
             x = np.append(x, self.x2mesh)
 
             # get unique values and sort in reverse order
             x = np.unique(x)[::-1]
 
@@ -679,16 +678,15 @@
                 spacing = x[i] - x[i + 1]
                 new_spacing = spacing
                 divider = 1
                 while new_spacing > self.coarseness:
                     divider += 1
                     new_spacing = spacing / divider
                 new_x = x[i] - (
-                    np.arange(start=1, stop=divider)
-                    * np.tile(new_spacing, (divider - 1))
+                    np.arange(start=1, stop=divider) * np.tile(new_spacing, (divider - 1))
                 )
                 x_secondary = np.append(x_secondary, new_x)
 
             # assemble x- coordinates
             x = np.append(x, x_secondary)
             x = np.unique(x)[::-1]
 
@@ -745,66 +743,155 @@
             )
 
         def create_springs() -> np.ndarray:
             # dim of springs
             spring_dim = 15
 
             # Allocate array
-            py = np.zeros(
-                shape=(self.element_number, 2, 2, spring_dim), dtype=np.float32
-            )
+            py = np.zeros(shape=(self.element_number, 2, 2, spring_dim), dtype=np.float32)
             mt = np.zeros(
-                shape=(self.element_number, 2, 2, spring_dim), dtype=np.float32
+                shape=(self.element_number, 2, 2, spring_dim, spring_dim), dtype=np.float32
             )
             Hb = np.zeros(shape=(1, 1, 2, spring_dim), dtype=np.float32)
             Mb = np.zeros(shape=(1, 1, 2, spring_dim), dtype=np.float32)
 
             tz = np.zeros(shape=(self.element_number, 2, 2, 15), dtype=np.float32)
 
             # fill in spring for each element
             for layer in self.soil.layers:
                 elements_for_layer = self.soil_properties.loc[
                     (self.soil_properties["x_top [m]"] <= layer.top)
                     & (self.soil_properties["x_bottom [m]"] >= layer.bottom)
                 ].index
+
                 # py curve
-                if layer.lateral_model.spring_signature[
-                    0
-                ]:  # True if py spring function exist
+                if layer.lateral_model is None:
+                    pass
+                else:
+                    # Set local layer parameters for each element of the layer
                     for i in elements_for_layer:
+                        # vertical effective stress
                         sig_v = self.soil_properties[
                             ["sigma_v top [kPa]", "sigma_v bottom [kPa]"]
                         ].iloc[i]
-                        elevation = self.soil_properties[
-                            ["x_top [m]", "x_bottom [m]"]
-                        ].iloc[i]
+                        # elevation
+                        elevation = self.soil_properties[["x_top [m]", "x_bottom [m]"]].iloc[i]
+                        # depth from ground
                         depth_from_ground = (
-                            self.soil_properties[["xg_top [m]", "xg_bottom [m]"]].iloc[
-                                i
-                            ]
+                            self.soil_properties[["xg_top [m]", "xg_bottom [m]"]].iloc[i]
                         ).abs()
+                        # pile width
                         pile_width = self.element_properties["Diameter [m]"].iloc[i]
 
-                        # top and bottom of element
-                        for j in [0, 1]:
-                            (
-                                py[i, j, 0, :],
-                                py[i, j, 1, :],
-                            ) = layer.lateral_model.py_spring_fct(
-                                sig=sig_v[j],
-                                X=depth_from_ground[j],
-                                layer_height=(layer.top - layer.bottom),
-                                depth_from_top_of_layer=(layer.top - elevation[j]),
-                                D=pile_width,
-                                L=self.pile.length,
-                                below_water_table=elevation[j]
-                                <= self.soil.water_elevation,
-                                output_length=spring_dim,
-                            )
-
+                        # p-y curves
+                        if (
+                            layer.lateral_model.spring_signature[0] and self.distributed_lateral
+                        ):  # True if py spring function exist
+
+                            # calculate springs (top and) for each element
+                            for j in [0, 1]:
+                                (py[i, j, 0], py[i, j, 1]) = layer.lateral_model.py_spring_fct(
+                                    sig=sig_v[j],
+                                    X=depth_from_ground[j],
+                                    layer_height=(layer.top - layer.bottom),
+                                    depth_from_top_of_layer=(layer.top - elevation[j]),
+                                    D=pile_width,
+                                    L=(self.soil.top_elevation - self.pile.bottom_elevation),
+                                    below_water_table=elevation[j] <= self.soil.water_elevation,
+                                    output_length=spring_dim,
+                                )
+
+                        if (
+                            layer.lateral_model.spring_signature[2] and self.distributed_moment
+                        ):  # True if mt spring function exist
+
+                            # calculate springs (top and) for each element
+                            for j in [0, 1]:
+                                (mt[i, j, 0], mt[i, j, 1]) = layer.lateral_model.mt_spring_fct(
+                                    sig=sig_v[j],
+                                    X=depth_from_ground[j],
+                                    layer_height=(layer.top - layer.bottom),
+                                    depth_from_top_of_layer=(layer.top - elevation[j]),
+                                    D=pile_width,
+                                    L=(self.soil.top_elevation - self.pile.bottom_elevation),
+                                    below_water_table=elevation[j] <= self.soil.water_elevation,
+                                    output_length=spring_dim,
+                                )
+
+                        # check if pile tip is within layer
+                        if (
+                            layer.top >= self.pile.bottom_elevation
+                            and layer.bottom <= self.pile.bottom_elevation
+                        ):
+
+                            # Hb curve
+                            sig_v_tip = self.soil_properties["sigma_v bottom [kPa]"].iloc[-1]
+
+                            if layer.lateral_model.spring_signature[1] and self.base_shear:
+
+                                # calculate Hb spring
+                                (Hb[0, 0, 0], Hb[0, 0, 1]) = layer.lateral_model.Hb_spring_fct(
+                                    sig=sig_v_tip,
+                                    X=self.pile.bottom_elevation,
+                                    layer_height=(layer.top - layer.bottom),
+                                    depth_from_top_of_layer=(
+                                        layer.top - self.pile.bottom_elevation
+                                    ),
+                                    D=pile_width,
+                                    L=(self.soil.top_elevation - self.pile.bottom_elevation),
+                                    below_water_table=self.pile.bottom_elevation
+                                    <= self.soil.water_elevation,
+                                    output_length=spring_dim,
+                                )
+
+                            # Mb curve
+                            if layer.lateral_model.spring_signature[3] and self.base_moment:
+
+                                (Mb[0, 0, 0], Mb[0, 0, 1]) = layer.lateral_model.Mb_spring_fct(
+                                    sig=sig_v_tip,
+                                    X=self.pile.bottom_elevation,
+                                    layer_height=(layer.top - layer.bottom),
+                                    depth_from_top_of_layer=(
+                                        layer.top - self.pile.bottom_elevation
+                                    ),
+                                    D=pile_width,
+                                    L=(self.soil.top_elevation - self.pile.bottom_elevation),
+                                    below_water_table=self.pile.bottom_elevation
+                                    <= self.soil.water_elevation,
+                                    output_length=spring_dim,
+                                )
+
+            if check_springs(py):
+                print("py springs have negative or NaN values.")
+                print(
+                    """if using PISA type springs, this can be due to parameters behind out of the parameter space.
+                Please check that: 2 < L/D < 6.
+                """
+                )
+            if check_springs(mt):
+                print("mt springs have negative or NaN values.")
+                print(
+                    """if using PISA type springs, this can be due to parameters behind out of the parameter space.
+                Please check that: 2 < L/D < 6.
+                """
+                )
+            if check_springs(Hb):
+                print("Hb spring has negative or NaN values.")
+                print(
+                    """if using PISA type springs, this can be due to parameters behind out of the parameter space.
+                Please check that: 2 < L/D < 6.
+                """
+                )
+            if check_springs(Mb):
+                print("Mb spring has negative or NaN values.")
+                print(
+                    """if using PISA type springs, this can be due to parameters behind out of the parameter space.
+                Please check that: 2 < L/D < 6.
+                """
+                )
             return py, mt, Hb, Mb, tz
 
         # creates mesh coordinates
         self.nodes_coordinates, self.element_coordinates = get_coordinates()
         self.element_number = int(self.element_coordinates.shape[0])
 
         # creates element structural properties
@@ -837,29 +924,24 @@
         self.soil_properties["xg_top [m]"] = (
             self.soil_properties["x_top [m]"] - self.soil.top_elevation
         )
         self.soil_properties["xg_bottom [m]"] = (
             self.soil_properties["x_bottom [m]"] - self.soil.top_elevation
         )
         # add vertical stress at top and bottom of each element
-        condition_below_water_table = (
-            self.soil_properties["x_top [m]"] <= self.soil.water_elevation
-        )
+        condition_below_water_table = self.soil_properties["x_top [m]"] <= self.soil.water_elevation
         self.soil_properties["Unit Weight [kN/m3]"][condition_below_water_table] = (
-            self.soil_properties["Unit Weight [kN/m3]"][condition_below_water_table]
-            - 10.0
+            self.soil_properties["Unit Weight [kN/m3]"][condition_below_water_table] - 10.0
         )
         s = (
             self.soil_properties["x_top [m]"] - self.soil_properties["x_bottom [m]"]
         ) * self.soil_properties["Unit Weight [kN/m3]"]
         self.soil_properties["sigma_v top [kPa]"] = np.insert(
             s.cumsum().values[:-1],
-            np.where(
-                self.soil_properties["x_top [m]"].values == self.soil.top_elevation
-            )[0],
+            np.where(self.soil_properties["x_top [m]"].values == self.soil.top_elevation)[0],
             0.0,
         )
         self.soil_properties["sigma_v bottom [kPa]"] = s.cumsum()
         # reset index
         self.soil_properties.reset_index(inplace=True, drop=True)
 
         # Initialise nodal global forces with link to nodes_coordinates (used for force-driven calcs)
@@ -876,104 +958,37 @@
 
         # Initialise nodal global support with link to nodes_coordinates (used for defining boundary conditions)
         self.global_restrained = self.nodes_coordinates.copy()
         self.global_restrained["Tx"] = False
         self.global_restrained["Ty"] = False
         self.global_restrained["Rz"] = False
 
+        # Create arrays of springs
         (
-            self.py_springs,
-            self.mt_springs,
-            self.Hb_spring,
-            self.Mb_spring,
-            self.tz_springs,
+            self._py_springs,
+            self._mt_springs,
+            self._Hb_spring,
+            self._Mb_spring,
+            self._tz_springs,
         ) = create_springs()
 
-    def soil_springs(
-        self, kind: Literal["p-y", "m-t", "Hb-y", "Mb-t", "t-z"]
-    ) -> pd.DataFrame:
-        """
-        Returns soil springs created for the given model in one DataFrame.
-
-        Parameters
-        ----------
-        kind : str
-            type of spring to extract.
-
-        Returns
-        -------
-        pd.DataFrame
-            Soil springs
-        """
-
-        def springs_to_df(springs: np.ndarray, flag) -> pd.DataFrame:
-            spring_dim = springs.shape[-1]
-            column_values_spring = [f"VAL {i}" for i in range(spring_dim)]
-
-            id = np.repeat(np.arange(self.element_number), 4)
-            x = np.repeat(misc.repeat_inner(self.nodes_coordinates["x [m]"].values), 2)
-
-            if len(x) > 2:
-                t_b = ["top", "bottom"] * int(len(x) / 2)
-
-                df = pd.DataFrame(
-                    data={
-                        "Element no.": id,
-                        "Position": t_b,
-                        "Elevation [m]": x,
-                    }
-                )
-            else:
-                df = pd.DataFrame(
-                    data={
-                        "Element no.": id,
-                        "Elevation [m]": x,
-                    }
-                )
-
-            df["type"] = flag.split("-") * int(len(x) / 2)
-            df[column_values_spring] = np.reshape(springs, (-1, spring_dim))
-
-            return df
-
-        # main part of function
-        if self.soil is None:
-            RuntimeError("No soil found. Please create the Model first with soil.")
-        else:
-            if kind == "p-y":
-                springs_df = springs_to_df(self.py_springs, flag=kind)
-            elif kind == "m-t":
-                springs_df = springs_to_df(self.mt_springs, flag=kind)
-            elif kind == "Hb-y":
-                springs_df = springs_to_df(self.Hb_spring, flag=kind)
-            elif kind == "Mb-t":
-                springs_df = springs_to_df(self.Mb_spring, flag=kind)
-            elif kind == "t-z":
-                springs_df = springs_to_df(self.tz_springs, flag=kind)
-            else:
-                ValueError("kind should be one of ['p-y','m-t','Hb-y','Mb-t','t-z']")
-
-        return springs_df
-
     def get_pointload(self, output=False, verbose=True):
         """
         Returns the point loads currently defined in the mesh via printout statements.
 
         Parameters
         ----------
         output : bool, optional
             If true, it returns the printout statements as a variable, by default False
         verbose : float, optional
             if True, printout statements printed automaically (ideal for use with iPython), by default True
         """
         out = ""
         try:
-            for idx, elevation, _, Px, Py, Mz in self.global_forces.itertuples(
-                name=None
-            ):
+            for idx, elevation, _, Px, Py, Mz in self.global_forces.itertuples(name=None):
                 if any([Px, Py, Mz]):
                     string = f"\nLoad applied at elevation {elevation} m (node no. {idx}): Px = {Px} kN, Py = {Py} kN, Mx = {Mz} kNm."
                     if verbose is True:
                         print(string)
                     out += f"\nLoad applied at elevation {elevation} m (node no. {idx}): Px = {Px} kN, Py = {Py} kN, Mx = {Mz} kNm."
             if output is True:
                 return out
@@ -1006,17 +1021,15 @@
         Mz : float, optional
             Bending moment in kNm, by default None
         """
 
         # identify if one node is at given elevation or if load needs to be split
         nodes_elevations = self.nodes_coordinates["x [m]"].values
         # check if corresponding node exist
-        check = np.isclose(
-            nodes_elevations, np.tile(elevation, nodes_elevations.shape), atol=0.001
-        )
+        check = np.isclose(nodes_elevations, np.tile(elevation, nodes_elevations.shape), atol=0.001)
 
         try:
             if any(check):
                 # one node correspond, extract node
                 node_idx = int(np.where(check == True)[0])
                 # apply loads at this node
                 if Px is not None:
@@ -1034,17 +1047,15 @@
                         "Load not applied! The chosen elevation is outside the mesh. The load must be applied on the structure."
                     )
                 else:
                     print(
                         "Load not applied! The chosen elevation is not meshed as a node. Please include elevation in `x2mesh` variable when creating the Model."
                     )
         except Exception:
-            print(
-                "\n!User Input Error! Please create Model first with the Model.create().\n"
-            )
+            print("\n!User Input Error! Please create Model first with the Model.create().\n")
             raise
 
     def set_pointdisplacement(
         self,
         elevation: float = 0.0,
         Ty: float = None,
         Tx: float = None,
@@ -1100,17 +1111,15 @@
                         "Support not applied! The chosen elevation is outside the mesh. The support must be applied on the structure."
                     )
                 else:
                     print(
                         "Support not applied! The chosen elevation is not meshed as a node. Please include elevation in `x2mesh` variable when creating the Model."
                     )
         except Exception:
-            print(
-                "\n!User Input Error! Please create Model first with the Model.create().\n"
-            )
+            print("\n!User Input Error! Please create Model first with the Model.create().\n")
             raise
 
     def set_support(
         self,
         elevation: float = 0.0,
         Ty: bool = False,
         Tx: bool = False,
@@ -1159,17 +1168,15 @@
                         "Support not applied! The chosen elevation is outside the mesh. The support must be applied on the structure."
                     )
                 else:
                     print(
                         "Support not applied! The chosen elevation is not meshed as a node. Please include elevation in `x2mesh` variable when creating the Model."
                     )
         except Exception:
-            print(
-                "\n!User Input Error! Please create Model first with the Model.create().\n"
-            )
+            print("\n!User Input Error! Please create Model first with the Model.create().\n")
             raise
 
     def plot(self, assign=False):
         fig = graphics.connectivity_plot(self)
         return fig if assign else None
 
     @classmethod
@@ -1178,17 +1185,19 @@
         name: str,
         pile: Pile,
         soil: Optional[SoilProfile] = None,
         element_type: Literal["Timoshenko", "EulerBernoulli"] = "Timoshenko",
         x2mesh: List[float] = Field(default_factory=list),
         coarseness: float = 0.5,
         distributed_lateral: bool = True,
-        distributed_moment: bool = False,
-        base_shear: bool = False,
-        base_moment: bool = False,
+        distributed_moment: bool = True,
+        distributed_axial: bool = False,
+        base_shear: bool = True,
+        base_moment: bool = True,
+        base_axial: bool = False,
     ):
         """A method to create the Model. This function provides a 2-in-1 command where:
 
         - a `Model` instance is created
         - the `._postinit()` method is run and creates all necessary data to perform calculations.
 
         Parameters
@@ -1225,16 +1234,46 @@
             pile=pile,
             soil=soil,
             element_type=element_type,
             x2mesh=x2mesh,
             coarseness=coarseness,
             distributed_lateral=distributed_lateral,
             distributed_moment=distributed_moment,
+            distributed_axial=distributed_axial,
             base_shear=base_shear,
             base_moment=base_moment,
+            base_axial=base_axial,
         )
         obj._postinit()
 
         return obj
 
     def __str__(self):
         return self.element_properties.to_string()
+
+    @property
+    def py_springs(self) -> pd.DataFrame:
+        """_summary_
+        #TODO
+
+        Returns
+        -------
+        pd.DataFrame
+            Table with p-y springs.
+        """
+        return misc.get_springs(
+            springs=self._py_springs,
+            elevations=self.nodes_coordinates["x [m]"].values,
+            kind="p-y",
+        )
+
+    @property
+    def embedment(self) -> float:
+        """_summary_
+        #TODO
+
+        Returns
+        -------
+        float
+            Pile embedment
+        """
+        return self.soil.top_elevation - self.pile.bottom_elevation
```

### Comparing `openpile-0.0.1/src/openpile/core/kernel.py` & `openpile-0.1.0/src/openpile/core/kernel.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import numpy as np
 import pandas as pd
 from numba import njit, prange, f4, f8, b1, char
 import numba as nb
 from typing_extensions import Literal
 
 from openpile.construct import Model, Pile
-
+from openpile.core.validation import UserInputError
 from openpile.core import misc
 
 
 @njit(f8[:](f8[:, :], f8[:]), cache=True)
 def jit_solve(A, b):
     return np.linalg.solve(A, b)
 
@@ -30,14 +30,43 @@
 
 
 @njit(parallel=True, cache=True)
 def reverse_indices(A, B):
     return np.array([x for x in A if x not in B])
 
 
+@njit(f8[:](f8[:]), cache=True)
+def double_inner_njit(in_arr):
+    # d = misc.repeat_inner(u)
+    out_arr = np.zeros(((len(in_arr) - 1) * 2), dtype=np.float64)
+    i = 0
+    while i < len(out_arr) + 1:
+        if i == 0:
+            out_arr[i] = in_arr[0]
+            i += 1
+        elif i == len(out_arr):
+            out_arr[i] = in_arr[-1]
+            i += 1
+        elif i == len(out_arr) - 1:
+            out_arr[i] = in_arr[-2]
+            i += 1
+        elif i % 2 != 0:
+            x = int((i + 1) / 2)
+            out_arr[i] = in_arr[x]
+            out_arr[i + 1] = in_arr[x]
+            i += 2
+        elif i % 2 == 0:
+            x = int(i / 2)
+            out_arr[i] = in_arr[x]
+            out_arr[i + 1] = in_arr[x]
+            i += 2
+
+    return out_arr
+
+
 @njit(parallel=True, cache=True)
 def numba_ix(arr, rows, cols):
     """
     Numba compatible implementation of arr[np.ix_(rows, cols)] for 2D arrays.
     :param arr: 2D array to be indexed
     :param rows: Row indices
     :param cols: Column indices
@@ -118,17 +147,17 @@
 
     if restraints.any():
         prescribed_dof_true = np.where(restraints)[0]
         prescribed_dof_false = np.where(~restraints)[0]
 
         prescribed_disp = U
 
-        Fred = F[prescribed_dof_false] - numba_ix(
-            K, prescribed_dof_false, prescribed_dof_true
-        ).dot(prescribed_disp[prescribed_dof_true])
+        Fred = F[prescribed_dof_false] - numba_ix(K, prescribed_dof_false, prescribed_dof_true).dot(
+            prescribed_disp[prescribed_dof_true]
+        )
         Kred = numba_ix(K, prescribed_dof_false, prescribed_dof_false)
 
         U[prescribed_dof_false] = jit_solve(Kred, Fred)
     else:
         U = jit_solve(K, F)
 
     Q = K.dot(U) - F
@@ -185,24 +214,16 @@
     # elastic properties
     nu = model.pile._nu
     E = model.element_properties["E [kPa]"].to_numpy(dtype=float).reshape((-1, 1, 1))
     G = E / (2 + 2 * nu)
     # cross-section properties
     I = model.element_properties["I [m4]"].to_numpy(dtype=float).reshape((-1, 1, 1))
     A = model.element_properties["Area [m2]"].to_numpy(dtype=float).reshape((-1, 1, 1))
-    d = (
-        model.element_properties["Diameter [m]"]
-        .to_numpy(dtype=float)
-        .reshape((-1, 1, 1))
-    )
-    wt = (
-        model.element_properties["Wall thickness [m]"]
-        .to_numpy(dtype=float)
-        .reshape((-1, 1, 1))
-    )
+    d = model.element_properties["Diameter [m]"].to_numpy(dtype=float).reshape((-1, 1, 1))
+    wt = model.element_properties["Wall thickness [m]"].to_numpy(dtype=float).reshape((-1, 1, 1))
 
     # calculate shear component in stiffness matrix (if Timorshenko)
     if model.element_type == "EulerBernoulli":
         kappa = 0
     elif model.element_type == "Timoshenko":
         if model.pile.kind == "Circular":
             a = 0.5 * d
@@ -213,17 +234,15 @@
                 + 34 * a**2 * b**2
                 + 7 * b**4
                 + nu * (12 * a**4 + 48 * a**2 * b**2 + 12 * b**4)
                 + nu**2 * (4 * a**4 + 16 * a**2 * b**2 + 4 * b**4)
             )
             kappa = nom / denom
         else:
-            raise ValueError(
-                "Timoshenko beams cannot be used yet for non-circular pile types"
-            )
+            raise ValueError("Timoshenko beams cannot be used yet for non-circular pile types")
     else:
         raise ValueError(
             "Model.element.type only accepts 'EB' type (for Euler-Bernoulli) of 'T' type (for Timoshenko)"
         )
 
     phi = 12 * E * I * kappa / (A * G * L**2)
     X = A * E / L
@@ -275,15 +294,15 @@
 
     """
 
     # calculate length vector
     L = mesh_to_element_length(model)
 
     # calculate the spring stiffness
-    ksoil = calculate_springs_stiffness(u=u[1::3], springs=model.py_springs, kind=kind)
+    ksoil = calculate_py_springs_stiffness(u=u[1::3], springs=model._py_springs, kind=kind)
 
     N = 0 * L
     A = 2 * L / 7
     B = L**2 / 28
     C = L**3 / 168
     D = 9 * L / 140
     E = L**2 / 70
@@ -319,14 +338,126 @@
         )
         * ksoil[:, 1]
     )
 
     return ktop + kbottom
 
 
+def elem_mt_stiffness_matrix(model, u, kind):
+    """creates soil element stiffness matrix based on model info and element number.
+
+    The soil stiffness matrix assumes the soil stiffness to vary lineraly along the elements.
+
+    #TODO: proof here
+
+    Parameters
+    ----------
+    model : openpile class object `openpile.construct.Model`
+        includes information on soil/structure, elements, nodes and other model-related data.
+    u: np.ndarray
+        Global displacement vector
+    kind: str
+        "initial", "secant" or "tangent"
+
+    Returns
+    -------
+    k: numpy array (3d)
+        soil consistent stiffness matrix of all elememts related to the p-y soil springs' stiffness
+
+    Raises
+    ------
+    ValueError
+        ndof per node can be either 2 or 3
+
+    """
+
+    # calculate length vector
+    L = mesh_to_element_length(model)
+
+    # calculate the py spring stiffness
+    kspy = calculate_py_springs_stiffness(u=u[1::3], springs=model._py_springs, kind="secant")
+    upy = double_inner_njit(u[1::3]).reshape(-1, 2, 1, 1)
+    p_mobilised = kspy * upy
+
+    # calculate the spring stiffness
+    ksoil = calculate_mt_springs_stiffness(
+        u=u[2::3],
+        mt_springs=model._mt_springs,
+        py_springs=model._py_springs,
+        p_mobilised=p_mobilised,
+        kind=kind,
+    )
+
+    # elastic properties
+    nu = model.pile._nu
+    E = model.element_properties["E [kPa]"].to_numpy(dtype=float).reshape((-1, 1, 1))
+    G = E / (2 + 2 * nu)
+    # cross-section properties
+    I = model.element_properties["I [m4]"].to_numpy(dtype=float).reshape((-1, 1, 1))
+    A = model.element_properties["Area [m2]"].to_numpy(dtype=float).reshape((-1, 1, 1))
+    d = model.element_properties["Diameter [m]"].to_numpy(dtype=float).reshape((-1, 1, 1))
+    wt = model.element_properties["Wall thickness [m]"].to_numpy(dtype=float).reshape((-1, 1, 1))
+
+    # calculate shear component in stiffness matrix (if Timorshenko)
+    if model.element_type == "EulerBernoulli":
+        N = 0 * L
+        A = 6 / (5 * L)
+        B = N + 1 / 10
+        C = 2 * L / 15
+        D = -L / 30
+    elif model.element_type == "Timoshenko":
+        if model.pile.kind == "Circular":
+            a = 0.5 * d
+            b = 0.5 * (d - 2 * wt)
+            nom = 6 * (a**2 + b**2) ** 2 * (1 + nu) ** 2
+            denom = (
+                7 * a**4
+                + 34 * a**2 * b**2
+                + 7 * b**4
+                + nu * (12 * a**4 + 48 * a**2 * b**2 + 12 * b**4)
+                + nu**2 * (4 * a**4 + 16 * a**2 * b**2 + 4 * b**4)
+            )
+            kappa = nom / denom
+
+            omega = E * I * kappa / (A * G * L**2)
+
+        else:
+            raise ValueError("Timoshenko beams cannot be used yet for non-circular pile types")
+
+        phi = (12 * omega + 1) ** 2
+
+        N = 0 * L
+        A = 6 * (120 * omega**2 + 20 * omega + 1) / ((5 * L) * phi) + 12 * I / (A * L**3 * phi)
+        B = 1 / (10 * phi) + 6 * I / (A * L**2 * phi)
+        C = (2 * L * (90 * omega**2 + 15 * omega + 1)) / (15 * phi) + 4 * I * (
+            36 * omega**2 + 6 * omega + 1
+        ) / (A * L * phi)
+        D = -L * (360 * omega**2 + 60 * omega + 1) / (30 * phi) - 2 * I * (
+            72 * omega**2 + 12 * omega - 1
+        ) / (A * L * phi)
+
+    else:
+        raise ValueError(
+            "Model.element.type only accepts 'EB' type (for Euler-Bernoulli) of 'T' type (for Timoshenko)"
+        )
+
+    km = np.block(
+        [
+            [N, N, N, N, N, N],
+            [N, A, B, N, -A, B],
+            [N, B, C, N, -B, D],
+            [N, N, N, N, N, N],
+            [N, -A, -B, N, A, -B],
+            [N, B, D, N, -B, C],
+        ]
+    ) * (0.5 * ksoil[:, 0] + 0.5 * ksoil[:, 1])
+
+    return km
+
+
 @njit(parallel=True, cache=True)
 def jit_build(k, ndim, n_elem, node_per_element, ndof_per_node):
     # pre-allocate stiffness matrix
     K = np.zeros((ndim, ndim), dtype=np.float64)
 
     for i in prange(n_elem):
         # dummy stiffness matrix that updates at each iteration
@@ -338,26 +469,28 @@
 
         # update global stiffness matrix
         K += K_temp
 
     return K
 
 
-def build_stiffness_matrix(model, u=None, kind=None):
+def build_stiffness_matrix(model, u=None, kind=None, p_mobilised=None):
     """Builds the stiffness matrix based on the model(element and node) properties
 
     Element stiffness matrices are first computed for each element and then loaded in the global stiffness matrix through summation.
     Different element stiffness matrices are computed depending on the specifications found in the Model object.
 
     Parameters
     ----------
     model : obj from openpile library
         stores all information about nodes elements, and other model-related items, see #TODO:link to model class
     u: np.ndarray, Optional
         Global displacement vector. Must be given if soil_flag is not None
+    p_mobilised: np.ndarray, Optional
+        Mobilised p-value. Must be given if soil_flag is not None
     kind: str, Optional
         "initial", "secant" or "tangent". Must be given if soil_flag is not None
 
     Returns
     -------
     K : numpy array of dim (ndof, ndof)
         Global stiffness matrix with all dofs in unit:1/kPa.
@@ -378,40 +511,43 @@
     if model.soil is not None:
         # gives warning if soil is given without displacements or type of stiffness
         if u is None or kind is None:
             UserWarning("'u' and 'kind' must be stipulated.")
         else:
             if model.distributed_lateral:
                 k += elem_py_stiffness_matrix(model, u, kind)
-            elif model.distributed_moment:
-                k += 0
-            elif model.base_shear:
-                k += 0
-            elif model.base_moment:
-                k += 0
+
+            if model.distributed_moment:
+                if not model.distributed_lateral:
+                    raise UserInputError(
+                        "Error: Distributed moment cannot be calculated without distributed lateral springs."
+                    )
+                k += elem_mt_stiffness_matrix(model, u, kind)
 
     K = jit_build(k, ndim_global, n_elem, node_per_element, ndof_per_node)
 
+    if model.base_shear:
+        K[-2:-2] += calculate_base_spring_stiffness(u[-2], model._Hb_spring, kind)
+
+    if model.base_moment:
+        K[-1:-1] += calculate_base_spring_stiffness(u[-1], model._Mb_spring, kind)
+
     return K
 
 
 def mesh_to_global_force_dof_vector(df: pd.DataFrame) -> np.ndarray:
     # extract each column (one line per node)
-    force_dof_vector = (
-        df[["Px [kN]", "Py [kN]", "Mz [kNm]"]].values.reshape(-1).astype(np.float64)
-    )
+    force_dof_vector = df[["Px [kN]", "Py [kN]", "Mz [kNm]"]].values.reshape(-1).astype(np.float64)
 
     return force_dof_vector
 
 
 def mesh_to_global_disp_dof_vector(df: pd.DataFrame) -> np.ndarray:
     # extract each column (one line per node)
-    disp_dof_vector = (
-        df[["Tx [m]", "Ty [m]", "Rz [rad]"]].values.reshape(-1).astype(np.float64)
-    )
+    disp_dof_vector = df[["Tx [m]", "Ty [m]", "Rz [rad]"]].values.reshape(-1).astype(np.float64)
 
     return disp_dof_vector
 
 
 def mesh_to_global_restrained_dof_vector(df: pd.DataFrame) -> np.ndarray:
     # extract each column (one line per node)
     restrained_dof_vector = df[["Tx", "Ty", "Rz"]].values.reshape(-1)
@@ -430,78 +566,107 @@
 
     # add soil contribution
     if model.soil is not None:
         kind = "secant"
         if model.distributed_lateral:
             k += elem_py_stiffness_matrix(model, u, kind)
         elif model.distributed_moment:
-            k += 0
+            k += elem_mt_stiffness_matrix(model, u, kind)
         elif model.base_shear:
-            k += 0
+            k[-1, -2, -2] += calculate_base_spring_stiffness(u[-2], model._Hb_spring, kind)
         elif model.base_moment:
-            k += 0
+            k[-1, -1, -1] += calculate_base_spring_stiffness(u[-1], model._Mb_spring, kind)
 
     # create array u of shape [n_elem x 6 x 1]
-    u = global_dof_vector_to_consistent_stacked_array(
-        u, ndof_per_node * node_per_element
-    )
+    u = global_dof_vector_to_consistent_stacked_array(u, ndof_per_node * node_per_element)
     # compute internal forces and reshape into global dof vector
     F_int = (-1) * np.matmul(k, u).reshape((-1))
 
     return F_int
 
 
 @njit(cache=True)
-def calculate_springs_stiffness(
+def calculate_base_spring_stiffness(
+    u: np.ndarray, spring: np.ndarray, kind: Literal["initial", "secant", "tangent"]
+):
+    """Calculate springs stiffness for py or t-z springs.
+
+    Parameters
+    ----------
+    u : float
+        base displacement or rotation to calculate stiffness
+    spring : np.ndarray
+        soil-structure interaction base springs array of shape (1, 1, 1, spring_dim)
+    kind : str
+        defines whether it is initial, secant of tangent stiffness to define
+
+    Returns
+    -------
+    k: float
+        secant or tangent stiffness for all elements.
+    """
+
+    # displacemet with same dimension as spring
+    d = abs(u)
+
+    if np.sum(spring[0, 0, 0]) == 0:
+        k = 0.0
+    else:
+        if kind == "initial" or d == 0.0:
+            dx = spring[0, 0, 1, 1] - spring[0, 0, 1, 0]
+            p0 = spring[0, 0, 0, 0]
+            p1 = spring[0, 0, 0, 1]
+        elif kind == "secant":
+            dx = d
+            p0 = spring[0, 0, 0, 0]
+            if d > np.max(spring[0, 0, 1]):
+                p1 = spring[0, 0, 0, -1]
+            else:
+                p1 = np.interp(dx, spring[0, 0, 1], spring[0, 0, 0])
+        elif kind == "tangent":
+            dx = min(0.0005, d)
+            if (d - dx) > np.max(spring[0, 0, 1]):
+                p0 = spring[0, 0, 0, -1]
+            else:
+                p0 = np.interp(d - dx, spring[0, 0, 1], spring[0, 0, 0])
+            if d > np.max(spring[0, 0, 1]):
+                p1 = spring[0, 0, 0, -1]
+            else:
+                p1 = np.interp(d, spring[0, 0, 1], spring[0, 0, 0])
+
+        k = abs((p1 - p0) / dx)
+
+    return k
+
+
+@njit(cache=True)
+def calculate_py_springs_stiffness(
     u: np.ndarray, springs: np.ndarray, kind: Literal["initial", "secant", "tangent"]
 ):
-    """Calculate springs stiffness
+    """Calculate springs stiffness for py or t-z springs.
 
     Parameters
     ----------
     u : np.ndarray
         displacements to calculate stiffness.
         For dofs related to t-z curves, u = U[::3] where U is the global displacement vector.
         For dofs related to p-y curves, u = U[1::3] where U is the global displacement vector.
-        For dofs related to m-t curves, u = U[2::3] where U is the global displacement vector.
     springs : np.ndarray
-        soil-structure interaction springs array of shape (n_elem, 2, 2, spring_dim)
+        soil-structure interaction py springs array of shape (n_elem, 2, 2, spring_dim)
     kind : str
         defines whether it is initial, secant of tangent stiffness to define
 
     Returns
     -------
     k: np.ndarray
         secant or tangent stiffness for all elements. Array of shape(n_elem,2,1,1)
     """
 
-    # double inner values
-    # d = misc.repeat_inner(u)
-    d = np.zeros(((len(u) - 1) * 2), dtype=np.float64)
-    i = 0
-    while i < len(d) + 1:
-        if i == 0:
-            d[i] = u[0]
-            i += 1
-        elif i == len(d):
-            d[i] = u[-1]
-            i += 1
-        elif i == len(d) - 1:
-            d[i] = u[-2]
-            i += 1
-        elif i % 2 != 0:
-            x = int((i + 1) / 2)
-            d[i] = u[x]
-            d[i + 1] = u[x]
-            i += 2
-        elif i % 2 == 0:
-            x = int(i / 2)
-            d[i] = u[x]
-            d[i + 1] = u[x]
-            i += 2
+    # double inner values for u
+    d = double_inner_njit(u)
 
     # displacemet with same dimension as spring
     d = np.abs(d).reshape((-1, 2, 1, 1))
 
     k = np.zeros(d.shape, dtype=np.float64)
 
     for i in range(k.shape[0]):
@@ -521,25 +686,115 @@
                     else:
                         p1 = np.interp(dx, springs[i, j, 1], springs[i, j, 0])
                 elif kind == "tangent":
                     dx = min(0.0005, d[i, j, 0, 0])
                     if (d[i, j, 0, 0] - dx) > np.max(springs[i, j, 1]):
                         p0 = springs[i, j, 0, -1]
                     else:
-                        p0 = np.interp(
-                            d[i, j, 0, 0] - dx, springs[i, j, 1], springs[i, j, 0]
-                        )
+                        p0 = np.interp(d[i, j, 0, 0] - dx, springs[i, j, 1], springs[i, j, 0])
                     if d[i, j, 0, 0] > np.max(springs[i, j, 1]):
                         p1 = springs[i, j, 0, -1]
                     else:
-                        p1 = np.interp(
-                            d[i, j, 0, 0], springs[i, j, 1], springs[i, j, 0]
+                        p1 = np.interp(d[i, j, 0, 0], springs[i, j, 1], springs[i, j, 0])
+
+                k[i, j, 0, 0] = abs((p1 - p0) / dx)
+
+    return k
+
+
+@njit(cache=True)
+def calculate_mt_springs_stiffness(
+    u: np.ndarray,
+    mt_springs: np.ndarray,
+    py_springs: np.ndarray,
+    p_mobilised: np.ndarray,
+    kind: Literal["initial", "secant", "tangent"],
+):
+    """Calculate springs stiffness for rotational springs
+
+    .. note::
+        The difference with the py function is that rotational springs can depend on lateral springs
+
+    Parameters
+    ----------
+    u : np.ndarray
+        displacements to calculate stiffness.
+        For dofs related to m-t curves, u = U[2::3] where U is the global displacement vector.
+    mt_springs : np.ndarray
+        soil-structure interaction m-t springs array of shape (n_elem, 2, 2, py_spring_dim, mt_spring_dim)
+    py_springs : np.ndarray
+        soil-structure interaction p-y springs array of shape (n_elem, 2, 2, py_spring_dim)
+    p_mobilised : np.ndarray
+        current p value of p-y springs of shape (nelem, 2, 1, 1)
+    kind : str
+        defines whether it is initial, secant of tangent stiffness to define
+
+    Returns
+    -------
+    k: np.ndarray
+        secant or tangent stiffness for all elements. Array of shape(n_elem,2,1,1)
+    """
+
+    # double inner values for u
+    d = double_inner_njit(u)
+
+    # displacemet and p_mobilised with same dimension as spring
+    d = np.abs(d).reshape((-1, 2, 1, 1))
+    p = p_mobilised.reshape((-1, 2, 1, 1))
+
+    k = np.zeros(d.shape, dtype=np.float64)
+
+    # get the proper m-t spring
+    m = np.zeros(mt_springs.shape[4])
+    t = np.zeros(mt_springs.shape[4])
+
+    # i for each element
+    for i in range(k.shape[0]):
+        # j for top and bottom values of spring
+        for j in range(k.shape[1]):
+            if np.sum(mt_springs[i, j, 1, 0]) == 0:
+                # check if first m-vector is not a defined spring
+                # if that is the case, we do not calculate any stiffness
+                pass
+            else:
+
+                for ii in range((mt_springs.shape[4])):
+                    if ii == 0:
+                        pass
+                    else:
+                        m[ii] = np.interp(
+                            p[i, j, 0, 0], py_springs[i, j, 0, :], mt_springs[i, j, 0, :, ii]
                         )
+                        t[ii] = np.interp(
+                            p[i, j, 0, 0], py_springs[i, j, 0, :], mt_springs[i, j, 1, :, ii]
+                        )
+
+                if kind == "initial" or d[i, j, 0, 0] == 0.0:
+                    dt = t[1] - t[0]
+                    m0 = m[0]
+                    m1 = m[1]
+                elif kind == "secant":
+                    dt = d[i, j, 0, 0]
+                    m0 = m[0]
+                    if d[i, j, 0, 0] > t[-1]:
+                        m1 = m[-1]
+                    else:
+                        m1 = np.interp(dt, t, m)
+                elif kind == "tangent":
+                    dt = min(0.01 * t[1], d[i, j, 0, 0])
+                    if (d[i, j, 0, 0] - dt) > t[-1]:
+                        m0 = m[-1]
+                    else:
+                        m0 = np.interp(d[i, j, 0, 0] - dt, t, m)
+                    if (d[i, j, 0, 0]) > t[-1]:
+                        m1 = m[-1]
+                    else:
+                        m1 = np.interp(d[i, j, 0, 0], t, m)
 
-            k[i, j, 0, 0] = abs((p1 - p0) / dx)
+                k[i, j, 0, 0] = abs(m1 - m0) / (dt)
 
     return k
 
 
 def computer():
     """This function is the solver of openpile.
```

### Comparing `openpile-0.0.1/src/openpile/core/txt.py` & `openpile-0.1.0/src/openpile/core/txt.py`

 * *Files identical despite different names*

### Comparing `openpile-0.0.1/src/openpile/core/validation.py` & `openpile-0.1.0/src/openpile/core/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 # ----------------------------------------------------------------
 #                              PILE
 # ----------------------------------------------------------------
 
 
 def pile_sections_must_be(obj):
     if not isinstance(obj.pile_sections, dict):
-        raise UserInputError(
-            "openpile.construct.Pile.pile_sections must be a dictionary"
-        )
+        raise UserInputError("openpile.construct.Pile.pile_sections must be a dictionary")
 
     if obj.kind == "Circular":
         reference_list = ["diameter", "length", "wall thickness"]
         sorted_list = list(obj.pile_sections.keys())
         sorted_list.sort()
         if sorted_list != reference_list:
             raise UserInputError(
@@ -50,28 +48,23 @@
             else:
                 if len(sublist) != reference_length:
                     raise ValueError(
                         "length of lists in openpile.construct.Pile.pile_sections must be the same"
                     )
 
         for i in range(reference_length):
-            if (
-                obj.pile_sections["diameter"][i] / 2
-                < obj.pile_sections["wall thickness"][i]
-            ):
+            if obj.pile_sections["diameter"][i] / 2 < obj.pile_sections["wall thickness"][i]:
                 raise ValueError(
                     "The wall thickness cannot be larger than half the diameter of the pile"
                 )
 
 
 def param_must_be_type(parameter, parameter_name, parameter_type, type_name):
     if not isinstance(parameter, parameter_type):
-        raise UserInputError(
-            f"Wrong type for {parameter_name}. Please provide a {type_name}"
-        )
+        raise UserInputError(f"Wrong type for {parameter_name}. Please provide a {type_name}")
 
 
 def str_must_be_one_of_those(param: str, param_name: str, accepted_values: list):
     param_must_be_type(param, param_name, str, "string")
     if param not in accepted_values:
         raise UserInputError(
             f"Value in {param_name} type must be one of the following: \n - "
@@ -98,17 +91,15 @@
     restrained_dof = model.global_restrained
     loaded_dof = model.global_forces
 
     # count BC in [Translation over z-axis,Translation over y-axis,Rotation around x-axis]
     restrained_count_Rz = np.count_nonzero(restrained_dof["Rz"])
     restrained_count_Ty = np.count_nonzero(restrained_dof["Ty"])
     restrained_count_Tx = np.count_nonzero(restrained_dof["Tx"])
-    restrained_count_total = (
-        restrained_count_Rz + restrained_count_Ty + restrained_count_Tx
-    )
+    restrained_count_total = restrained_count_Rz + restrained_count_Ty + restrained_count_Tx
 
     loaded_count_Rz = np.count_nonzero(loaded_dof["Mz [kNm]"])
     loaded_count_Ty = np.count_nonzero(loaded_dof["Py [kN]"])
     loaded_count_Tx = np.count_nonzero(loaded_dof["Px [kN]"])
     loaded_count_total = loaded_count_Rz + loaded_count_Ty + loaded_count_Tx
 
     if restrained_count_total == 0:
@@ -135,12 +126,10 @@
         elif (restrained_count_Ty + restrained_count_Rz) >= 2 and loaded_count_Rz > 0:
             pass
             # support in y and z axes are given and load over z is given --> correct BC
         elif (loaded_count_Rz + loaded_count_Ty) == 0:
             # no trasnverse load --> no need to give any error
             pass
         else:
-            raise InvalidBoundaryConditionsError(
-                "Support conditions against bending not provided."
-            )
+            raise InvalidBoundaryConditionsError("Support conditions against bending not provided.")
     else:
         raise InvalidBoundaryConditionsError("Soil in mesh not yet possible.")
```

### Comparing `openpile-0.0.1/src/openpile/utils/graphics.py` & `openpile-0.1.0/src/openpile/utils/graphics.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,22 +72,16 @@
 
     # plot mesh with + scatter points to see nodes.
     x = model.nodes_coordinates["x [m]"]
     y = model.nodes_coordinates["y [m]"]
     ax.plot(y, x, "-k", marker="+")
 
     total_length = max(
-        (
-            model.nodes_coordinates["x [m]"].max()
-            - model.nodes_coordinates["x [m]"].min()
-        ),
-        (
-            model.nodes_coordinates["y [m]"].max()
-            - model.nodes_coordinates["y [m]"].min()
-        ),
+        (model.nodes_coordinates["x [m]"].max() - model.nodes_coordinates["x [m]"].min()),
+        (model.nodes_coordinates["y [m]"].max() - model.nodes_coordinates["y [m]"].min()),
     )
 
     ylim = ax.get_ylim()
 
     # plots SUPPORTS
     # Plot supports along x
     support_along_x = model.global_restrained["Tx"].values
@@ -108,23 +102,19 @@
         color=support_color,
         marker=6,
         s=100,
     )
 
     # Plot supports along y
     support_along_y = model.global_restrained["Ty"].values
-    ax.scatter(
-        y[support_along_y], x[support_along_y], color=support_color, marker=5, s=100
-    )
+    ax.scatter(y[support_along_y], x[support_along_y], color=support_color, marker=5, s=100)
 
     # Plot supports along z
     support_along_z = model.global_restrained["Rz"].values
-    ax.scatter(
-        y[support_along_z], x[support_along_z], color=support_color, marker="s", s=35
-    )
+    ax.scatter(y[support_along_z], x[support_along_z], color=support_color, marker="s", s=35)
 
     # plot LOADS
     arrows = []
 
     normalized_arrow_size = (
         0.10 * total_length
     )  # max arrow length will be 20% of the total structure length
@@ -134,51 +124,39 @@
         if load == 0:
             pass
         else:
             style = "Simple, tail_width=1, head_width=5, head_length=3"
             kw = dict(arrowstyle=style, color="r")
             arrow_length = normalized_arrow_size * abs(load / load_max)
             if load > 0:
-                arrows.append(
-                    FancyArrowPatch((-arrow_length, yval), (xval, yval), **kw)
-                )
+                arrows.append(FancyArrowPatch((-arrow_length, yval), (xval, yval), **kw))
             elif load < 0:
                 arrows.append(FancyArrowPatch((arrow_length, yval), (xval, yval), **kw))
 
     load_max = model.global_forces["Px [kN]"].abs().max()
     for idx, (yval, xval, load) in enumerate(zip(x, y, model.global_forces["Px [kN]"])):
         if load == 0:
             pass
         else:
             style = "Simple, tail_width=1, head_width=5, head_length=3"
             kw = dict(arrowstyle=style, color="r")
             arrow_length = normalized_arrow_size * abs(load / load_max)
             if load > 0:
                 if idx == len(x) - 1:
-                    arrows.append(
-                        FancyArrowPatch((xval, yval), (xval, yval + arrow_length), **kw)
-                    )
+                    arrows.append(FancyArrowPatch((xval, yval), (xval, yval + arrow_length), **kw))
                 else:
-                    arrows.append(
-                        FancyArrowPatch((xval, yval - arrow_length), (xval, yval), **kw)
-                    )
+                    arrows.append(FancyArrowPatch((xval, yval - arrow_length), (xval, yval), **kw))
             elif load < 0:
                 if idx == len(x) - 1:
-                    arrows.append(
-                        FancyArrowPatch((xval, yval), (xval, yval - arrow_length), **kw)
-                    )
+                    arrows.append(FancyArrowPatch((xval, yval), (xval, yval - arrow_length), **kw))
                 else:
-                    arrows.append(
-                        FancyArrowPatch((xval, yval + arrow_length), (xval, yval), **kw)
-                    )
+                    arrows.append(FancyArrowPatch((xval, yval + arrow_length), (xval, yval), **kw))
 
     load_max = model.global_forces["Mz [kNm]"].abs().max()
-    for idx, (yval, xval, load) in enumerate(
-        zip(x, y, model.global_forces["Mz [kNm]"])
-    ):
+    for idx, (yval, xval, load) in enumerate(zip(x, y, model.global_forces["Mz [kNm]"])):
         if load == 0:
             pass
         else:
             kw = dict(arrowstyle=style, color="r")
             arrow_length = normalized_arrow_size * abs(load / load_max)
             style = "Simple, tail_width=1, head_width=5, head_length=3"
             if load > 0:
```

### Comparing `openpile-0.0.1/src/openpile/utils/py_curves.py` & `openpile-0.1.0/src/openpile/utils/py_curves.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,139 @@
+"""
+`py_curves` module
+==================
+
+"""
+
 # Import libraries
 import math as m
 import numpy as np
 from numba import njit, prange
 from random import random
 
+from openpile.core.misc import conic
+
 # SPRING FUNCTIONS --------------------------------------------
+@njit(cache=True)
+def cowden_clay(
+    X: float,
+    Su: float,
+    G0: float,
+    D: float,
+    output_length: int = 20,
+):
+    """
+    Creates the lateral springs from the PISA clay formulation
+    published by Byrne et al (2020) and calibrated based pile
+    load tests at Cowden (north east coast of England).
+
+    Parameters
+    ----------
+    X : float
+        Depth below ground level [unit: m]
+    Su : float
+        Undrained shear strength [unit: kPa]
+    G0 : float
+        Small-strain shear modulus [unit: kPa]
+    D : float
+        Pile diameter [unit: m]
+    output_length : int, optional
+        Number of datapoints in the curve, by default 20
+
+    Returns
+    -------
+    1darray
+        p vector [unit: kN/m]
+    1darray
+        y vector [unit: m]
+    """
+
+    # # Cowden clay parameters
+    v_pu = 241.4
+    k_p1 = 10.6
+    k_p2 = -1.650
+    n_p1 = 0.9390
+    n_p2 = -0.03345
+    p_u1 = 10.7
+    p_u2 = -7.101
+
+    # Depth variation parameters
+    v_max = v_pu
+    k = k_p1 + k_p2 * X / D
+    n = n_p1 + n_p2 * X / D
+    p_max = p_u1 + p_u2 * m.exp(-0.3085 * X / D)
+
+    # calculate normsalised conic function
+    y, p = conic(v_max, n, k, p_max, output_length)
+
+    # return non-normalised curve
+    return p * (Su * D), y * (Su * D / G0)
+
+
+@njit(cache=True)
+def dunkirk_sand(
+    sig: float,
+    X: float,
+    Dr: float,
+    G0: float,
+    D: float,
+    L: float,
+    output_length: int = 20,
+):
+    """
+    Creates the lateral spring from the PISA sand formulation
+    published by Burd et al (2020).
+    Also called the General Dunkirk Sand Model (GDSM).
+
+    Parameters
+    ----------
+    sig : float
+        vertical/overburden effective stress [unit: kPa]
+    X : float
+        Depth below ground level [unit: m]
+    Dr : float
+        Sand relative density Value must be between 0 and 100 [unit: -]
+    G0 : float
+        Small-strain shear modulus [unit: kPa]
+    D : float
+        Pile diameter [unit: m]
+    L : float
+        Embedded pile length [unit: m]
+    output_length : int, optional
+        Number of datapoints in the curve, by default 20
+
+    Returns
+    -------
+    1darray
+        p vector [unit: kN/m]
+    1darray
+        y vector [unit: m]
+    """
+    # correct relative density for decimal value
+    Dr = Dr / 100
+
+    # Generalised Dunkirk Sand Model parameters
+    v_pu = 146.1 - 92.11 * Dr
+    k_p1 = 8.731 - 0.6982 * Dr
+    k_p2 = -0.9178
+    n_p = 0.917 + 0.06193 * Dr
+    p_u1 = 0.3667 + 25.89 * Dr
+    p_u2 = 0.3375 - 8.9 * Dr
+
+    # Depth variation parameters
+    v_max = v_pu
+    k = k_p1 + k_p2 * X / D
+    n = n_p
+    p_max = p_u1 + p_u2 * X / L
+
+    # calculate normsalised conic function
+    y, p = conic(v_max, n, k, p_max, output_length)
+
+    # return non-normalised curve
+    return p * (sig * D), y * (sig * D / G0)
 
 
 # API sand function
 @njit(parallel=True, cache=True)
 def api_sand(
     sig: float,
     X: float,
@@ -18,40 +143,39 @@
     below_water_table: bool = True,
     ymax: float = 0.0,
     output_length: int = 20,
 ):
     """
     Creates the API sand p-y curve from relevant input.
 
-    ---------
-    input:
-        sig: float
-            Vertical effective stress [unit: kPa]
-        X: float
-            Depth of the curve w.r.t. mudline [unit: m]
-        phi: float
-            internal angle of friction of the sand layer [unit: degrees]
-        D: float
-            Pile width [unit: m]
-        Neq: float, by default 1.0
-            Number of equivalent cycles [unit: -]
-        below_water_table: bool, by default False
-            switch to calculate initial subgrade modulus below/above water table
-        ymax: float, by default 0.0
-            maximum value of y, default goes to 99.9% of ultimate resistance
-        output_length: int, by default 10
-            Number of discrete point along the springs
-    ---------
-    Returns curve with 2 vectors:
-        p: numpy 1darray
-            p vector [unit: kPa/metre of pile length]
-        y: numpy 1darray
-            y vector [unit: m]
-    ---------
-
+    Parameters
+    ----------
+    sig: float
+        Vertical effective stress [unit: kPa]
+    X: float
+        Depth of the curve w.r.t. mudline [unit: m]
+    phi: float
+        internal angle of friction of the sand layer [unit: degrees]
+    D: float
+        Pile width [unit: m]
+    Neq: float, by default 1.0
+        Number of equivalent cycles [unit: -]
+    below_water_table: bool, by default False
+        switch to calculate initial subgrade modulus below/above water table
+    ymax: float, by default 0.0
+        maximum value of y, default goes to 99.9% of ultimate resistance
+    output_length: int, by default 20
+        Number of discrete point along the springs
+
+    Returns
+    -------
+    1darray
+        p vector [unit: kN/m]
+    1darray
+        y vector [unit: m]
     """
     # A value - only thing that changes between cyclic or static
     if Neq == 1:
         A = max(0.9, 3 - 0.8 * X / D)
     else:
         A = 0.9
 
@@ -65,27 +189,21 @@
     ## Factors according to Mosher and Dawkins 2008.(regular API)
     b = 0.4
     Beta = 45 + phi / 2
     rad = m.pi / 180
     C1 = (
         (b * m.tan(phi * rad) * m.sin(Beta * rad))
         / (m.tan((Beta - phi) * rad) * m.cos((phi / 2) * rad))
-        + ((m.tan(Beta * rad)) ** 2 * m.tan((phi / 2) * rad))
-        / (m.tan((Beta - phi) * rad))
-        + b
-        * m.tan(Beta * rad)
-        * (m.tan(phi * rad) * m.sin(Beta * rad) - m.tan((phi / 2) * rad))
+        + ((m.tan(Beta * rad)) ** 2 * m.tan((phi / 2) * rad)) / (m.tan((Beta - phi) * rad))
+        + b * m.tan(Beta * rad) * (m.tan(phi * rad) * m.sin(Beta * rad) - m.tan((phi / 2) * rad))
     )
-    C2 = (
-        m.tan(Beta * rad) / m.tan((Beta - phi) * rad)
-        - (m.tan((45 - phi / 2) * rad)) ** 2
+    C2 = m.tan(Beta * rad) / m.tan((Beta - phi) * rad) - (m.tan((45 - phi / 2) * rad)) ** 2
+    C3 = b * m.tan(phi * rad) * (m.tan(Beta * rad)) ** 4 + (m.tan((45 - phi / 2) * rad)) ** 2 * (
+        (m.tan(Beta * rad)) ** 8 - 1
     )
-    C3 = b * m.tan(phi * rad) * (m.tan(Beta * rad)) ** 4 + (
-        m.tan((45 - phi / 2) * rad)
-    ) ** 2 * ((m.tan(Beta * rad)) ** 8 - 1)
 
     ## Pmax for shallow and deep zones (regular API)
     Pmax = min(C3 * sig * D, C1 * sig * X + C2 * sig * D)
 
     # creation of 'y' array
     if ymax == 0.0:
         # ensure X cannot be zero
@@ -120,48 +238,48 @@
     Su: float,
     eps50: float,
     D: float,
     J: float = 0.5,
     stiff_clay_threshold=96,
     Neq: float = 1.0,
     ymax: float = 0.0,
-    output_length: int = 15,
+    output_length: int = 20,
 ):
     """
     Creates the API clay p-y curve from relevant input.
 
-
-    ---------
-    input:
-        sig: float
-            Vertical effective stress [unit: kPa]
-        X: float
-            Depth of the curve w.r.t. mudline [unit: m]
-        Su : float
-            Undrained shear strength [unit: kPa]
-        eps50: float
-            strain at 50% ultimate resistance [-]
-        D: float
-            Pile width [unit: m]
-        J: float, by default 0.5
-            empirical factor varying depending on clay stiffness
-        stiff_clay_threshold: float, by default 96.0
-            undrained shear strength at which stiff clay curve is computed [unit: kPa]
-        Neq: float, by default 1.0
-            Number of equivalent cycles [unit: -]
-        ymax: float, by default 0.0
-            maximum value of y, if null the maximum is calculated such that the whole curve is computed
-        output_length: int, by default 20
-            Number of discrete point along the springs
-    ---------
-    Returns curve with 2 vectors:
-        p: numpy 1darray
-            p vector [unit: kPa/metre of pile length]
-        y: numpy 1darray
-            y vector [unit: m]
+    Parameters
+    ----------
+    sig: float
+        Vertical effective stress [unit: kPa]
+    X: float
+        Depth of the curve w.r.t. mudline [unit: m]
+    Su : float
+        Undrained shear strength [unit: kPa]
+    eps50: float
+        strain at 50% ultimate resistance [-]
+    D: float
+        Pile width [unit: m]
+    J: float, by default 0.5
+        empirical factor varying depending on clay stiffness
+    stiff_clay_threshold: float, by default 96.0
+        undrained shear strength at which stiff clay curve is computed [unit: kPa]
+    Neq: float, by default 1.0
+        Number of equivalent cycles [unit: -]
+    ymax: float, by default 0.0
+        maximum value of y, if null the maximum is calculated such that the whole curve is computed
+    output_length: int, by default 20
+        Number of discrete point along the springs
+
+    Returns
+    -------
+    1darray
+        p vector [unit: kN/m]
+    1darray
+        y vector [unit: m]
     ---------
     """
     # important variables
     y50 = 2.5 * eps50 * D
     if X == 0.0 or Su == 0:
         Xr = 2.5 * D
     else:
@@ -205,30 +323,22 @@
         else:
             # derive cyclic curve
             if X <= Xr:
                 if Su <= stiff_clay_threshold:
                     if y[i] > 15 * y50:
                         p[i] = 0.7185 * Pmax * X / Xr
                     elif y[i] > 3 * y50:
-                        p[i] = (
-                            0.7185
-                            * Pmax
-                            * (1 - (1 - X / Xr) * (y[i] - 3 * y50) / (12 * y50))
-                        )
+                        p[i] = 0.7185 * Pmax * (1 - (1 - X / Xr) * (y[i] - 3 * y50) / (12 * y50))
                     else:
                         p[i] = 0.5 * Pmax * (y[i] / y50) ** 0.33
                 else:
                     if y[i] > 15 * y50:
                         p[i] = 0.5 * Pmax * X / Xr
                     elif y[i] > 1 * y50:
-                        p[i] = (
-                            0.5
-                            * Pmax
-                            * (1 - (1 - X / Xr) * (y[i] - 1 * y50) / (14 * y50))
-                        )
+                        p[i] = 0.5 * Pmax * (1 - (1 - X / Xr) * (y[i] - 1 * y50) / (14 * y50))
                     else:
                         p[i] = 0.5 * Pmax * (y[i] / y50) ** 0.33
 
             elif X > Xr:
                 if Su <= stiff_clay_threshold:
                     if y[i] > 3 * y50:
                         p[i] = 0.7185 * Pmax
```

### Comparing `openpile-0.0.1/src/openpile.egg-info/PKG-INFO` & `openpile-0.1.0/src/openpile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpile
-Version: 0.0.1
+Version: 0.1.0
 Summary: Library for geotechnical pile calculations.
 Home-page: https://github.com/TchilDill/openpile
 Author: Guillaume Melin
 Author-email: guillaume.melin@icloud.com
 License: GPLv3
 Keywords: Offshore Wind,PILE,Geotechnics,monopile,pin-piles,Geotechnical,calculations,PISA,winkler
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
-# openpile
+# OpenPile
 
 Geotechnical super-toolbox for pile-related calculations.
 
 <!-- [![Python Support](https://img.shields.io/pypi/pyversions/openpile.svg)](https://pypi.org/project/openpile/) -->
 [![License: LGPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/)
 
@@ -65,12 +65,12 @@
    * Out-of-the-box computation of individual soil springs
    <!-- * Axial capacity calculations via integration -->
  * Friendly API interface with  object-oriented approach
  * Fully integrated output with python environment with Matplotlib and Pandas libraries. 
 
  ## Please share with the community
 
-This library relies on community interactions. Please consider sharing a post about `openpile` and the value it can provide for researcher, academia and professionals.
+This library relies on community interactions. Please consider sharing a post about `OpenPile` and the value it can provide for researcher, academia and professionals.
 
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-reddit-red?logo=reddit)](https://reddit.com/submit?url=https://github.com/TchilDill/openpile&title=openpile)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-twitter-03A9F4?logo=twitter)](https://twitter.com/share?url=https://github.com/TchilDill/openpile&t=openpile)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-linkedin-3949AB?logo=linkedin)](https://www.linkedin.com/shareArticle?url=https://github.com/TchilDill/openpile&title=openpile)
```

### Comparing `openpile-0.0.1/src/openpile.egg-info/SOURCES.txt` & `openpile-0.1.0/src/openpile.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -15,12 +15,18 @@
 src/openpile.egg-info/requires.txt
 src/openpile.egg-info/top_level.txt
 src/openpile/core/__init__.py
 src/openpile/core/kernel.py
 src/openpile/core/misc.py
 src/openpile/core/txt.py
 src/openpile/core/validation.py
+src/openpile/utils/Hb_curves.py
+src/openpile/utils/Mb_curves.py
 src/openpile/utils/__init__.py
 src/openpile/utils/graphics.py
+src/openpile/utils/mt_curves.py
 src/openpile/utils/py_curves.py
+src/openpile/utils/qz_curves.py
+src/openpile/utils/tz_curves.py
 test/test_construct.py
+test/test_pycurves.py
 test/test_utils_misc.py
```

### Comparing `openpile-0.0.1/test/test_utils_misc.py` & `openpile-0.1.0/test/test_utils_misc.py`

 * *Files identical despite different names*


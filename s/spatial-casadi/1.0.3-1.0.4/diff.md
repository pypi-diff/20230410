# Comparing `tmp/spatial_casadi-1.0.3.tar.gz` & `tmp/spatial_casadi-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatial_casadi-1.0.3.tar", last modified: Tue Apr  4 12:34:11 2023, max compression
+gzip compressed data, was "spatial_casadi-1.0.4.tar", last modified: Mon Apr 10 12:13:47 2023, max compression
```

## Comparing `spatial_casadi-1.0.3.tar` & `spatial_casadi-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-04 12:34:11.095664 spatial_casadi-1.0.3/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     7650 2023-03-12 23:07:25.000000 spatial_casadi-1.0.3/LICENSE
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     5566 2023-04-04 12:34:11.095664 spatial_casadi-1.0.3/PKG-INFO
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     4708 2023-03-26 19:51:34.000000 spatial_casadi-1.0.3/README.md
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      785 2023-04-04 12:33:34.000000 spatial_casadi-1.0.3/pyproject.toml
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       38 2023-04-04 12:34:11.099664 spatial_casadi-1.0.3/setup.cfg
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      920 2023-04-04 12:33:29.000000 spatial_casadi-1.0.3/setup.py
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-04 12:34:11.095664 spatial_casadi-1.0.3/spatial_casadi/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       77 2023-03-26 20:00:43.000000 spatial_casadi-1.0.3/spatial_casadi/__init__.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    22962 2023-04-04 12:31:15.000000 spatial_casadi-1.0.3/spatial_casadi/spatial.py
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-04 12:34:11.095664 spatial_casadi-1.0.3/spatial_casadi.egg-info/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     5566 2023-04-04 12:34:11.000000 spatial_casadi-1.0.3/spatial_casadi.egg-info/PKG-INFO
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      377 2023-04-04 12:34:11.000000 spatial_casadi-1.0.3/spatial_casadi.egg-info/SOURCES.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)        1 2023-04-04 12:34:11.000000 spatial_casadi-1.0.3/spatial_casadi.egg-info/dependency_links.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       34 2023-04-04 12:34:11.000000 spatial_casadi-1.0.3/spatial_casadi.egg-info/requires.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       15 2023-04-04 12:34:11.000000 spatial_casadi-1.0.3/spatial_casadi.egg-info/top_level.txt
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-04 12:34:11.095664 spatial_casadi-1.0.3/test/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     6732 2023-04-04 12:31:15.000000 spatial_casadi-1.0.3/test/test_rotation.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     1316 2023-03-13 19:43:36.000000 spatial_casadi-1.0.3/test/test_transformation.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     1903 2023-03-13 19:43:40.000000 spatial_casadi-1.0.3/test/test_translation.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      597 2023-03-13 19:43:43.000000 spatial_casadi-1.0.3/test/test_utils.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-10 12:13:47.974830 spatial_casadi-1.0.4/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     7650 2023-03-12 23:07:25.000000 spatial_casadi-1.0.4/LICENSE
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     5566 2023-04-10 12:13:47.974830 spatial_casadi-1.0.4/PKG-INFO
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     4708 2023-03-26 19:51:34.000000 spatial_casadi-1.0.4/README.md
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      785 2023-04-10 12:12:34.000000 spatial_casadi-1.0.4/pyproject.toml
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       38 2023-04-10 12:13:47.974830 spatial_casadi-1.0.4/setup.cfg
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      920 2023-04-10 12:12:39.000000 spatial_casadi-1.0.4/setup.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-10 12:13:47.974830 spatial_casadi-1.0.4/spatial_casadi/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       77 2023-03-26 20:00:43.000000 spatial_casadi-1.0.4/spatial_casadi/__init__.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    23420 2023-04-10 12:11:04.000000 spatial_casadi-1.0.4/spatial_casadi/spatial.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-10 12:13:47.974830 spatial_casadi-1.0.4/spatial_casadi.egg-info/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     5566 2023-04-10 12:13:47.000000 spatial_casadi-1.0.4/spatial_casadi.egg-info/PKG-INFO
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      377 2023-04-10 12:13:47.000000 spatial_casadi-1.0.4/spatial_casadi.egg-info/SOURCES.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)        1 2023-04-10 12:13:47.000000 spatial_casadi-1.0.4/spatial_casadi.egg-info/dependency_links.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       34 2023-04-10 12:13:47.000000 spatial_casadi-1.0.4/spatial_casadi.egg-info/requires.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       15 2023-04-10 12:13:47.000000 spatial_casadi-1.0.4/spatial_casadi.egg-info/top_level.txt
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-10 12:13:47.974830 spatial_casadi-1.0.4/test/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     6732 2023-04-04 12:31:15.000000 spatial_casadi-1.0.4/test/test_rotation.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     1316 2023-03-13 19:43:36.000000 spatial_casadi-1.0.4/test/test_transformation.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     1903 2023-03-13 19:43:40.000000 spatial_casadi-1.0.4/test/test_translation.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      597 2023-03-13 19:43:43.000000 spatial_casadi-1.0.4/test/test_utils.py
```

### Comparing `spatial_casadi-1.0.3/LICENSE` & `spatial_casadi-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spatial_casadi-1.0.3/PKG-INFO` & `spatial_casadi-1.0.4/spatial_casadi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: spatial_casadi
-Version: 1.0.3
+Name: spatial-casadi
+Version: 1.0.4
 Summary: Spatial transformation library for CasADi Python. 
 Home-page: https://github.com/cmower/spatial-casadi
 Author: Christopher E. Mower
 Author-email: "Christopher E. Mower" <christopher.mower@kcl.ac.uk>
 License: LGPL-3.0 license
 Project-URL: Homepage, https://cmower.github.io/spatial-casadi/
 Project-URL: Documentation, https://cmower.github.io/spatial-casadi/
```

### Comparing `spatial_casadi-1.0.3/README.md` & `spatial_casadi-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `spatial_casadi-1.0.3/pyproject.toml` & `spatial_casadi-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spatial_casadi"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Christopher E. Mower", email="christopher.mower@kcl.ac.uk" },
 ]
 description = "Spatial transformation library for CasADi Python. "
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `spatial_casadi-1.0.3/setup.py` & `spatial_casadi-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="spatial-casadi",
     description="Spatial transformation library for CasADi Python.",
-    version="1.0.3",
+    version="1.0.4",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cmower/spatial-casadi",
     project_urls={
         "Homepage": "https://cmower.github.io/spatial-casadi/",
         "Documentation": "https://cmower.github.io/spatial-casadi/",
         "Bug Tracker": "https://github.com/cmower/spatial-casadi/issues",
```

### Comparing `spatial_casadi-1.0.3/spatial_casadi/spatial.py` & `spatial_casadi-1.0.4/spatial_casadi/spatial.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,14 +118,20 @@
     def random():
         """! Generate uniformly distributed rotations.
 
 @return Random rotation.
         """
         return Rotation(casadi.np.random.normal(size=(4,)))
 
+    @staticmethod
+    def symbolic():
+        """! Symbolic representation."""
+        quat = cs.SX.sym("quat", 4)
+        return Rotation(quat, normalize=False)
+
     def inv(self):
         """! Invert this rotation."""
         return Rotation(
             casadi.vertcat(self._quat[:-1], -self._quat[-1]),
             normalize=not isinstance(self._quat, casadi.SX),
         )
 
@@ -577,14 +583,20 @@
         """! Generate uniformly distributed translations.
 
 @return Random translation.
         """
         return Translation(casadi.np.random.normal(size=(3,)))
 
     @staticmethod
+    def symbolic():
+        """! Symbolic representation."""
+        t = cs.SX.sym("t", 3)
+        return Translation(t)
+
+    @staticmethod
     def from_vector(t):
         """! Initialize from translation vector.
 
 @param t A 3-dimensional translation vector.
 @return Object containing the translation represented by the input vector.
         """
         return Translation(t)
@@ -667,14 +679,19 @@
         """! Generate uniformly distributed homogeneous transforms.
 
 @return Random homogeneous transform.
         """
         return Transformation(Rotation.random(), Translation.random())
 
     @staticmethod
+    def symbolic():
+        """! Symbolic representation."""
+        return Transformation(Rotation.symbolic(), Translation.symbolic())
+
+    @staticmethod
     def from_matrix(T: ArrayType):
         """! Initialize from homogenous transformation matrix.
 
 @param matrix A 4-by-4 homogeneous transformation matrix.
 @return Object containing the homogeneous transformation represented by the matrix.
         """
         T = casadi.horzcat(T)
```

### Comparing `spatial_casadi-1.0.3/spatial_casadi.egg-info/PKG-INFO` & `spatial_casadi-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: spatial-casadi
-Version: 1.0.3
+Name: spatial_casadi
+Version: 1.0.4
 Summary: Spatial transformation library for CasADi Python. 
 Home-page: https://github.com/cmower/spatial-casadi
 Author: Christopher E. Mower
 Author-email: "Christopher E. Mower" <christopher.mower@kcl.ac.uk>
 License: LGPL-3.0 license
 Project-URL: Homepage, https://cmower.github.io/spatial-casadi/
 Project-URL: Documentation, https://cmower.github.io/spatial-casadi/
```

### Comparing `spatial_casadi-1.0.3/test/test_rotation.py` & `spatial_casadi-1.0.4/test/test_rotation.py`

 * *Files identical despite different names*

### Comparing `spatial_casadi-1.0.3/test/test_transformation.py` & `spatial_casadi-1.0.4/test/test_transformation.py`

 * *Files identical despite different names*

### Comparing `spatial_casadi-1.0.3/test/test_translation.py` & `spatial_casadi-1.0.4/test/test_translation.py`

 * *Files identical despite different names*

### Comparing `spatial_casadi-1.0.3/test/test_utils.py` & `spatial_casadi-1.0.4/test/test_utils.py`

 * *Files identical despite different names*


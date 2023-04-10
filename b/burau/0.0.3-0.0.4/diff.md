# Comparing `tmp/burau-0.0.3.tar.gz` & `tmp/burau-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/sorfj/repos/burau/dist/tmpvuvh0rsk/burau-0.0.3.tar", last modified: Sat Oct  2 20:03:26 2021, max compression
+gzip compressed data, was "burau-0.0.4.tar", last modified: Mon Apr 10 19:37:19 2023, max compression
```

## Comparing `burau-0.0.3.tar` & `burau-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 sorfj     (1000) sorfj     (1000)        0 2021-10-02 20:03:26.000000 burau-0.0.3/
--rwxrwxrwx   0 sorfj     (1000) sorfj     (1000)     1082 2020-10-08 19:59:13.000000 burau-0.0.3/LICENSE
--rwxrwxrwx   0 sorfj     (1000) sorfj     (1000)     5830 2021-10-02 20:03:26.000000 burau-0.0.3/PKG-INFO
--rwxrwxrwx   0 sorfj     (1000) sorfj     (1000)     5471 2021-10-02 20:01:56.000000 burau-0.0.3/README.rst
-drwxrwxrwx   0 sorfj     (1000) sorfj     (1000)        0 2021-10-02 20:03:26.000000 burau-0.0.3/burau/
--rwxrwxrwx   0 sorfj     (1000) sorfj     (1000)        0 2020-09-18 17:55:56.000000 burau-0.0.3/burau/__init__.py
--rwxrwxrwx   0 sorfj     (1000) sorfj     (1000)    13234 2020-10-06 07:58:18.000000 burau-0.0.3/burau/curve.py
-drwxrwxrwx   0 sorfj     (1000) sorfj     (1000)        0 2021-10-02 20:03:26.000000 burau-0.0.3/burau.egg-info/
--rwxrwxrwx   0 sorfj     (1000) sorfj     (1000)     5830 2021-10-02 20:03:26.000000 burau-0.0.3/burau.egg-info/PKG-INFO
--rwxrwxrwx   0 sorfj     (1000) sorfj     (1000)      257 2021-10-02 20:03:26.000000 burau-0.0.3/burau.egg-info/SOURCES.txt
--rwxrwxrwx   0 sorfj     (1000) sorfj     (1000)        1 2021-10-02 20:03:26.000000 burau-0.0.3/burau.egg-info/dependency_links.txt
--rwxrwxrwx   0 sorfj     (1000) sorfj     (1000)       12 2021-10-02 20:03:26.000000 burau-0.0.3/burau.egg-info/requires.txt
--rwxrwxrwx   0 sorfj     (1000) sorfj     (1000)       12 2021-10-02 20:03:26.000000 burau-0.0.3/burau.egg-info/top_level.txt
--rwxrwxrwx   0 sorfj     (1000) sorfj     (1000)      104 2021-10-02 19:52:32.000000 burau-0.0.3/pyproject.toml
--rwxrwxrwx   0 sorfj     (1000) sorfj     (1000)       38 2021-10-02 20:03:26.000000 burau-0.0.3/setup.cfg
--rwxrwxrwx   0 sorfj     (1000) sorfj     (1000)     1063 2021-10-02 20:02:49.000000 burau-0.0.3/setup.py
-drwxrwxrwx   0 sorfj     (1000) sorfj     (1000)        0 2021-10-02 20:03:26.000000 burau-0.0.3/tests/
--rwxrwxrwx   0 sorfj     (1000) sorfj     (1000)        0 2020-09-18 17:56:19.000000 burau-0.0.3/tests/__init__.py
--rwxrwxrwx   0 sorfj     (1000) sorfj     (1000)     2875 2020-10-08 18:46:04.000000 burau-0.0.3/tests/test_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:37:19.364497 burau-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-10 19:37:09.000000 burau-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-10 19:37:19.364497 burau-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-10 19:37:09.000000 burau-0.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:37:19.364497 burau-0.0.4/burau/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:37:09.000000 burau-0.0.4/burau/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13234 2023-04-10 19:37:09.000000 burau-0.0.4/burau/curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:37:19.364497 burau-0.0.4/burau.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-10 19:37:19.000000 burau-0.0.4/burau.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-10 19:37:19.000000 burau-0.0.4/burau.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:37:19.000000 burau-0.0.4/burau.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 19:37:19.000000 burau-0.0.4/burau.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 19:37:19.000000 burau-0.0.4/burau.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-10 19:37:09.000000 burau-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:37:19.364497 burau-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-10 19:37:09.000000 burau-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:37:19.364497 burau-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:37:09.000000 burau-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-10 19:37:09.000000 burau-0.0.4/tests/test_curve.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `burau-0.0.3/LICENSE` & `burau-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `burau-0.0.3/PKG-INFO` & `burau-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: burau
-Version: 0.0.3
+Version: 0.0.4
 Summary: Search for non-trivial elements of the kernel of the Burau representation of the four-strand braid group.
 Home-page: https://github.com/fuglede/burau
 Author: Søren Fuglede Jørgensen
 Author-email: pypi@fuglede.dk
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -109,14 +107,18 @@
 Usage
 -----
 
 The package can be installed from PyPI::
 
     pip install burau
 
+or it can be obtained from `conda-forge <https://anaconda.org/conda-forge/burau>`_::
+
+    mamba install -c conda-forge burau
+
 The above example can be reproduced using the functionality of this Python
 module as follows:
 
 >>> from burau.curve import calculate_polynomial
 >>> calculate_polynomial(cap_west=2, cap_east=1, cup_west=3, cup_east=2)
 (DictType[int64,int64]<iv=None>({0: 1, -2: 1, -4: 1, -8: -1, -10: -1}), True, 5)
 
@@ -134,9 +136,7 @@
 
 References
 ----------
 .. [0] Bigelow, Stephen (1999). "The Burau representation is not faithful
        for n = 5". Geometry & Topology. 3: 397–404. arXiv:math/9904100.
        doi:10.2140/gt.1999.3.397.
 .. [1] https://en.wikipedia.org/wiki/Burau_representation..
-
-
```

### Comparing `burau-0.0.3/README.rst` & `burau-0.0.4/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -95,14 +95,18 @@
 Usage
 -----
 
 The package can be installed from PyPI::
 
     pip install burau
 
+or it can be obtained from `conda-forge <https://anaconda.org/conda-forge/burau>`_::
+
+    mamba install -c conda-forge burau
+
 The above example can be reproduced using the functionality of this Python
 module as follows:
 
 >>> from burau.curve import calculate_polynomial
 >>> calculate_polynomial(cap_west=2, cap_east=1, cup_west=3, cup_east=2)
 (DictType[int64,int64]<iv=None>({0: 1, -2: 1, -4: 1, -8: -1, -10: -1}), True, 5)
```

### Comparing `burau-0.0.3/burau/curve.py` & `burau-0.0.4/burau/curve.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -168,14 +168,20 @@
                 # Currently facing south, so follow pairing, stay south,
                 # but face north
                 self.current_strand = self.south_pairing[self.current_strand]
                 self.southbound = False
             else:
                 # Move north, stay at same strand, but keep track of crossings
                 # with ramps and alpha
+                if self._intersecting_alpha():
+                    self._intersect_alpha()
+                    logging.debug(
+                        f"Intersecting alpha from below "
+                        f"at level {self.level}."
+                    )
                 if self._crossing_southwest_ramp():
                     self.level -= 1
                     logging.debug(
                         f"Going down southwest ramp. "
                         f"Now at level {self.level}."
                     )
                 if self._crossing_northwest_ramp():
@@ -192,20 +198,14 @@
                     )
                 if self._crossing_northeast_ramp():
                     self.level += 1
                     logging.debug(
                         f"Going up northeast ramp. "
                         f"Now at level {self.level}."
                     )
-                if self._intersecting_alpha():
-                    self._intersect_alpha()
-                    logging.debug(
-                        f"Intersecting alpha from below "
-                        f"at level {self.level}."
-                    )
                 self.at_north = True
 
     def __iter__(self):
         return self
 
 
 @njit
@@ -310,28 +310,28 @@
                 # Currently facing south, so follow pairing, stay south,
                 # but face north
                 current_strand = south_pairing[current_strand]
                 southbound = False
             else:
                 # Move north, stay at same strand, but keep track of crossings
                 # with ramps and alpha
+                if intersecting_alpha(current_strand):
+                    polynomial[level] = polynomial.get(level, 0) - 1
+                    num_crossings += 1
+                    # Get rid of terms with zero coefficients
+                    if polynomial[level] == 0:
+                        del polynomial[level]
                 if crossing_southwest_ramp(current_strand):
                     level -= 1
                 if crossing_northwest_ramp(current_strand):
                     level -= 1
                 if crossing_southeast_ramp(current_strand):
                     level += 1
                 if crossing_northeast_ramp(current_strand):
                     level += 1
-                if intersecting_alpha(current_strand):
-                    polynomial[level] = polynomial.get(level, 0) - 1
-                    num_crossings += 1
-                    # Get rid of terms with zero coefficients
-                    if polynomial[level] == 0:
-                        del polynomial[level]
                 at_north = True
     is_beta_connected = steps == 2 * num_strands - 1
     return polynomial, is_beta_connected, num_crossings
 
 
 def calculate_polynomial(
     cap_west: int, cap_east: int, cup_west: int, cup_east: int, use_numba=True
```

### Comparing `burau-0.0.3/burau.egg-info/PKG-INFO` & `burau-0.0.4/burau.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: burau
-Version: 0.0.3
+Version: 0.0.4
 Summary: Search for non-trivial elements of the kernel of the Burau representation of the four-strand braid group.
 Home-page: https://github.com/fuglede/burau
 Author: Søren Fuglede Jørgensen
 Author-email: pypi@fuglede.dk
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -109,14 +107,18 @@
 Usage
 -----
 
 The package can be installed from PyPI::
 
     pip install burau
 
+or it can be obtained from `conda-forge <https://anaconda.org/conda-forge/burau>`_::
+
+    mamba install -c conda-forge burau
+
 The above example can be reproduced using the functionality of this Python
 module as follows:
 
 >>> from burau.curve import calculate_polynomial
 >>> calculate_polynomial(cap_west=2, cap_east=1, cup_west=3, cup_east=2)
 (DictType[int64,int64]<iv=None>({0: 1, -2: 1, -4: 1, -8: -1, -10: -1}), True, 5)
 
@@ -134,9 +136,7 @@
 
 References
 ----------
 .. [0] Bigelow, Stephen (1999). "The Burau representation is not faithful
        for n = 5". Geometry & Topology. 3: 397–404. arXiv:math/9904100.
        doi:10.2140/gt.1999.3.397.
 .. [1] https://en.wikipedia.org/wiki/Burau_representation..
-
-
```

### Comparing `burau-0.0.3/setup.py` & `burau-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = f.read().decode('utf-8')
     long_description = re.sub(r":math:`(.+?)`", r"\1", long_description)
     long_description = re.sub(r".. math::\n\n", "", long_description)
 
 
 setuptools.setup(
     name="burau",
-    version="0.0.3",
+    version="0.0.4",
     author="Søren Fuglede Jørgensen",
     author_email="pypi@fuglede.dk",
     description="Search for non-trivial elements of the kernel of the Burau "
     + "representation of the four-strand braid group.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/fuglede/burau",
```

### Comparing `burau-0.0.3/tests/test_curve.py` & `burau-0.0.4/tests/test_curve.py`

 * *Files identical despite different names*


# Comparing `tmp/voronoi-0.3.1.tar.gz` & `tmp/voronoi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voronoi-0.3.1.tar", last modified: Wed Nov  3 15:44:03 2021, max compression
+gzip compressed data, was "voronoi-0.4.0.tar", last modified: Mon Apr 10 01:30:30 2023, max compression
```

## Comparing `voronoi-0.3.1.tar` & `voronoi-0.4.0.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-11-03 15:44:03.327434 voronoi-0.3.1/
--rw-r--r--   0 vsts      (1001) docker     (121)     1069 2021-11-03 15:40:08.000000 voronoi-0.3.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)      100 2021-11-03 15:40:08.000000 voronoi-0.3.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)     4278 2021-11-03 15:44:03.323434 voronoi-0.3.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     3446 2021-11-03 15:40:08.000000 voronoi-0.3.1/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-11-03 15:44:03.319434 voronoi-0.3.1/include/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-11-03 15:44:03.319434 voronoi-0.3.1/include/boost/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-11-03 15:44:03.323434 voronoi-0.3.1/include/boost/polygon/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-11-03 15:44:03.323434 voronoi-0.3.1/include/boost/polygon/detail/
--rw-r--r--   0 vsts      (1001) docker     (121)     2173 2021-11-03 15:40:08.000000 voronoi-0.3.1/include/boost/polygon/detail/config.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)    16747 2021-11-03 15:40:08.000000 voronoi-0.3.1/include/boost/polygon/detail/cstdint.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5977 2021-11-03 15:40:08.000000 voronoi-0.3.1/include/boost/polygon/detail/limits.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)    35264 2021-11-03 15:40:08.000000 voronoi-0.3.1/include/boost/polygon/detail/suffix.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)    15565 2021-11-03 15:40:08.000000 voronoi-0.3.1/include/boost/polygon/detail/voronoi_ctypes.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)    66136 2021-11-03 15:40:08.000000 voronoi-0.3.1/include/boost/polygon/detail/voronoi_predicates.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)    14549 2021-11-03 15:40:08.000000 voronoi-0.3.1/include/boost/polygon/detail/voronoi_robust_fpt.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)    11468 2021-11-03 15:40:08.000000 voronoi-0.3.1/include/boost/polygon/detail/voronoi_structures.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)    11399 2021-11-03 15:40:08.000000 voronoi-0.3.1/include/boost/polygon/isotropy.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2543 2021-11-03 15:40:08.000000 voronoi-0.3.1/include/boost/polygon/point_concept.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)      950 2021-11-03 15:40:08.000000 voronoi-0.3.1/include/boost/polygon/point_traits.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2570 2021-11-03 15:40:08.000000 voronoi-0.3.1/include/boost/polygon/segment_concept.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1009 2021-11-03 15:40:08.000000 voronoi-0.3.1/include/boost/polygon/segment_traits.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4507 2021-11-03 15:40:08.000000 voronoi-0.3.1/include/boost/polygon/voronoi.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)    20183 2021-11-03 15:40:08.000000 voronoi-0.3.1/include/boost/polygon/voronoi_builder.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)    19347 2021-11-03 15:40:08.000000 voronoi-0.3.1/include/boost/polygon/voronoi_diagram.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1434 2021-11-03 15:40:08.000000 voronoi-0.3.1/include/boost/polygon/voronoi_geometry_type.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)       16 2021-11-03 15:40:08.000000 voronoi-0.3.1/requirements-setup.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       58 2021-11-03 15:40:08.000000 voronoi-0.3.1/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       38 2021-11-03 15:44:03.327434 voronoi-0.3.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)     6504 2021-11-03 15:40:08.000000 voronoi-0.3.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-11-03 15:44:03.323434 voronoi-0.3.1/src/
--rw-r--r--   0 vsts      (1001) docker     (121)    46081 2021-11-03 15:40:08.000000 voronoi-0.3.1/src/main.cpp
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-11-03 15:44:03.323434 voronoi-0.3.1/voronoi/
--rw-r--r--   0 vsts      (1001) docker     (121)       52 2021-11-03 15:40:08.000000 voronoi-0.3.1/voronoi/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8499 2021-11-03 15:40:08.000000 voronoi-0.3.1/voronoi/beach_line_key.py
--rw-r--r--   0 vsts      (1001) docker     (121)      386 2021-11-03 15:40:08.000000 voronoi-0.3.1/voronoi/beach_line_value.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3097 2021-11-03 15:40:08.000000 voronoi-0.3.1/voronoi/big_float.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14977 2021-11-03 15:40:08.000000 voronoi-0.3.1/voronoi/big_int.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14342 2021-11-03 15:40:08.000000 voronoi-0.3.1/voronoi/builder.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8575 2021-11-03 15:40:08.000000 voronoi-0.3.1/voronoi/diagram.py
--rw-r--r--   0 vsts      (1001) docker     (121)      744 2021-11-03 15:40:08.000000 voronoi-0.3.1/voronoi/enums.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-11-03 15:44:03.323434 voronoi-0.3.1/voronoi/events/
--rw-r--r--   0 vsts      (1001) docker     (121)       66 2021-11-03 15:40:08.000000 voronoi-0.3.1/voronoi/events/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    49595 2021-11-03 15:40:08.000000 voronoi-0.3.1/voronoi/events/computers.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6747 2021-11-03 15:40:08.000000 voronoi-0.3.1/voronoi/events/models.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2570 2021-11-03 15:40:08.000000 voronoi-0.3.1/voronoi/events/predicates.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3783 2021-11-03 15:40:08.000000 voronoi-0.3.1/voronoi/faces.py
--rw-r--r--   0 vsts      (1001) docker     (121)      663 2021-11-03 15:40:08.000000 voronoi-0.3.1/voronoi/point.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4764 2021-11-03 15:40:08.000000 voronoi-0.3.1/voronoi/robust_difference.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3380 2021-11-03 15:40:08.000000 voronoi-0.3.1/voronoi/robust_float.py
--rw-r--r--   0 vsts      (1001) docker     (121)      461 2021-11-03 15:40:08.000000 voronoi-0.3.1/voronoi/segment.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3740 2021-11-03 15:40:08.000000 voronoi-0.3.1/voronoi/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-11-03 15:44:03.323434 voronoi-0.3.1/voronoi.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     4278 2021-11-03 15:44:03.000000 voronoi-0.3.1/voronoi.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1404 2021-11-03 15:44:03.000000 voronoi-0.3.1/voronoi.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-11-03 15:44:03.000000 voronoi-0.3.1/voronoi.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-11-03 15:40:14.000000 voronoi-0.3.1/voronoi.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)       58 2021-11-03 15:44:03.000000 voronoi-0.3.1/voronoi.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       17 2021-11-03 15:44:03.000000 voronoi-0.3.1/voronoi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:30:30.238739 voronoi-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 01:30:18.000000 voronoi-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-10 01:30:18.000000 voronoi-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-10 01:30:30.238739 voronoi-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-10 01:30:18.000000 voronoi-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:30:30.230739 voronoi-0.4.0/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:30:30.230739 voronoi-0.4.0/include/boost/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:30:30.234739 voronoi-0.4.0/include/boost/polygon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:30:30.234739 voronoi-0.4.0/include/boost/polygon/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-10 01:30:18.000000 voronoi-0.4.0/include/boost/polygon/detail/config.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16747 2023-04-10 01:30:18.000000 voronoi-0.4.0/include/boost/polygon/detail/cstdint.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-04-10 01:30:18.000000 voronoi-0.4.0/include/boost/polygon/detail/limits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    35264 2023-04-10 01:30:18.000000 voronoi-0.4.0/include/boost/polygon/detail/suffix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-04-10 01:30:18.000000 voronoi-0.4.0/include/boost/polygon/detail/voronoi_ctypes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    66136 2023-04-10 01:30:18.000000 voronoi-0.4.0/include/boost/polygon/detail/voronoi_predicates.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14549 2023-04-10 01:30:18.000000 voronoi-0.4.0/include/boost/polygon/detail/voronoi_robust_fpt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11468 2023-04-10 01:30:18.000000 voronoi-0.4.0/include/boost/polygon/detail/voronoi_structures.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-04-10 01:30:18.000000 voronoi-0.4.0/include/boost/polygon/isotropy.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-10 01:30:18.000000 voronoi-0.4.0/include/boost/polygon/point_concept.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-10 01:30:18.000000 voronoi-0.4.0/include/boost/polygon/point_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-10 01:30:18.000000 voronoi-0.4.0/include/boost/polygon/segment_concept.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-10 01:30:18.000000 voronoi-0.4.0/include/boost/polygon/segment_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-10 01:30:18.000000 voronoi-0.4.0/include/boost/polygon/voronoi.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20183 2023-04-10 01:30:18.000000 voronoi-0.4.0/include/boost/polygon/voronoi_builder.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19347 2023-04-10 01:30:18.000000 voronoi-0.4.0/include/boost/polygon/voronoi_diagram.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-10 01:30:18.000000 voronoi-0.4.0/include/boost/polygon/voronoi_geometry_type.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-10 01:30:18.000000 voronoi-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 01:30:30.238739 voronoi-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-04-10 01:30:18.000000 voronoi-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:30:30.234739 voronoi-0.4.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    46080 2023-04-10 01:30:18.000000 voronoi-0.4.0/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:30:30.238739 voronoi-0.4.0/voronoi/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 01:30:18.000000 voronoi-0.4.0/voronoi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-10 01:30:18.000000 voronoi-0.4.0/voronoi/beach_line_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-10 01:30:18.000000 voronoi-0.4.0/voronoi/beach_line_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-10 01:30:18.000000 voronoi-0.4.0/voronoi/big_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14993 2023-04-10 01:30:18.000000 voronoi-0.4.0/voronoi/big_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14538 2023-04-10 01:30:18.000000 voronoi-0.4.0/voronoi/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-04-10 01:30:18.000000 voronoi-0.4.0/voronoi/diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-10 01:30:18.000000 voronoi-0.4.0/voronoi/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:30:30.238739 voronoi-0.4.0/voronoi/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-10 01:30:18.000000 voronoi-0.4.0/voronoi/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49595 2023-04-10 01:30:18.000000 voronoi-0.4.0/voronoi/events/computers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-04-10 01:30:18.000000 voronoi-0.4.0/voronoi/events/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-10 01:30:18.000000 voronoi-0.4.0/voronoi/events/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-10 01:30:18.000000 voronoi-0.4.0/voronoi/faces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-10 01:30:18.000000 voronoi-0.4.0/voronoi/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-10 01:30:18.000000 voronoi-0.4.0/voronoi/robust_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-10 01:30:18.000000 voronoi-0.4.0/voronoi/robust_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-10 01:30:18.000000 voronoi-0.4.0/voronoi/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-10 01:30:18.000000 voronoi-0.4.0/voronoi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:30:30.238739 voronoi-0.4.0/voronoi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-10 01:30:30.000000 voronoi-0.4.0/voronoi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-10 01:30:30.000000 voronoi-0.4.0/voronoi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 01:30:30.000000 voronoi-0.4.0/voronoi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 01:30:29.000000 voronoi-0.4.0/voronoi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-10 01:30:30.000000 voronoi-0.4.0/voronoi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-10 01:30:30.000000 voronoi-0.4.0/voronoi.egg-info/top_level.txt
```

### Comparing `voronoi-0.3.1/LICENSE` & `voronoi-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/PKG-INFO` & `voronoi-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,58 @@
 Metadata-Version: 2.1
 Name: voronoi
-Version: 0.3.1
-Summary: Voronoi decomposition.
+Version: 0.4.0
 Home-page: https://github.com/lycantropos/voronoi/
-Author: Azat Ibrakov
-Author-email: azatibrakov@gmail.com
-License: MIT License
 Download-URL: https://github.com/lycantropos/voronoi/archive/master.zip
-Platform: UNKNOWN
+Author-email: Azat Ibrakov <azatibrakov@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2020 Azat Ibrakov
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 License-File: LICENSE
 
 voronoi
 =======
 
-[![](https://dev.azure.com/lycantropos/voronoi/_apis/build/status/lycantropos.voronoi?branchName=master)](https://dev.azure.com/lycantropos/voronoi/_build/latest?definitionId=29&branchName=master "Azure Pipelines")
+[![](https://github.com/lycantropos/voronoi/workflows/CI/badge.svg)](https://github.com/lycantropos/voronoi/actions/workflows/ci.yml "Github Actions")
 [![](https://codecov.io/gh/lycantropos/voronoi/branch/master/graph/badge.svg)](https://codecov.io/gh/lycantropos/voronoi "Codecov")
 [![](https://img.shields.io/github/license/lycantropos/voronoi.svg)](https://github.com/lycantropos/voronoi/blob/master/LICENSE "License")
 [![](https://badge.fury.io/py/voronoi.svg)](https://badge.fury.io/py/voronoi "PyPI")
 
-In what follows `python` is an alias for `python3.5` or `pypy3.5`
-or any later version (`python3.6`, `pypy3.6` and so on).
+In what follows `python` is an alias for `python3.7` or `pypy3.7`
+or any later version (`python3.8`, `pypy3.8` and so on).
 
 Installation
 ------------
 
 Install the latest `pip` & `setuptools` packages versions
 ```bash
 python -m pip install --upgrade pip setuptools
@@ -172,9 +191,7 @@
   ```powershell
   .\run-tests.ps1 cpython
   ```
 - with `PyPy`
   ```powershell
   .\run-tests.ps1 pypy
   ```
-
-
```

### Comparing `voronoi-0.3.1/README.md` & `voronoi-0.4.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 voronoi
 =======
 
-[![](https://dev.azure.com/lycantropos/voronoi/_apis/build/status/lycantropos.voronoi?branchName=master)](https://dev.azure.com/lycantropos/voronoi/_build/latest?definitionId=29&branchName=master "Azure Pipelines")
+[![](https://github.com/lycantropos/voronoi/workflows/CI/badge.svg)](https://github.com/lycantropos/voronoi/actions/workflows/ci.yml "Github Actions")
 [![](https://codecov.io/gh/lycantropos/voronoi/branch/master/graph/badge.svg)](https://codecov.io/gh/lycantropos/voronoi "Codecov")
 [![](https://img.shields.io/github/license/lycantropos/voronoi.svg)](https://github.com/lycantropos/voronoi/blob/master/LICENSE "License")
 [![](https://badge.fury.io/py/voronoi.svg)](https://badge.fury.io/py/voronoi "PyPI")
 
-In what follows `python` is an alias for `python3.5` or `pypy3.5`
-or any later version (`python3.6`, `pypy3.6` and so on).
+In what follows `python` is an alias for `python3.7` or `pypy3.7`
+or any later version (`python3.8`, `pypy3.8` and so on).
 
 Installation
 ------------
 
 Install the latest `pip` & `setuptools` packages versions
 ```bash
 python -m pip install --upgrade pip setuptools
```

### Comparing `voronoi-0.3.1/include/boost/polygon/detail/config.hpp` & `voronoi-0.4.0/include/boost/polygon/detail/config.hpp`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/include/boost/polygon/detail/cstdint.hpp` & `voronoi-0.4.0/include/boost/polygon/detail/cstdint.hpp`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/include/boost/polygon/detail/limits.hpp` & `voronoi-0.4.0/include/boost/polygon/detail/limits.hpp`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/include/boost/polygon/detail/suffix.hpp` & `voronoi-0.4.0/include/boost/polygon/detail/suffix.hpp`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/include/boost/polygon/detail/voronoi_ctypes.hpp` & `voronoi-0.4.0/include/boost/polygon/detail/voronoi_ctypes.hpp`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/include/boost/polygon/detail/voronoi_predicates.hpp` & `voronoi-0.4.0/include/boost/polygon/detail/voronoi_predicates.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -1231,24 +1231,24 @@
         b += iy * (robust_fpt_type(b2) * sqr_sum1);
         b -= sqr_sum1 *
              robust_fpt_type(robust_cross_product(
                                  static_cast<int_x2_type>(segm_end2.x()) -
                                      static_cast<int_x2_type>(segm_start2.x()),
                                  static_cast<int_x2_type>(segm_end2.y()) -
                                      static_cast<int_x2_type>(segm_start2.y()),
-                                 static_cast<int_x2_type>(-site1.y()),
+                                 -static_cast<int_x2_type>(site1.y()),
                                  static_cast<int_x2_type>(site1.x())),
                              to_fpt(1.0));
         b -= sqr_sum2 *
              robust_fpt_type(robust_cross_product(
                                  static_cast<int_x2_type>(segm_end1.x()) -
                                      static_cast<int_x2_type>(segm_start1.x()),
                                  static_cast<int_x2_type>(segm_end1.y()) -
                                      static_cast<int_x2_type>(segm_start1.y()),
-                                 static_cast<int_x2_type>(-site1.y()),
+                                 -static_cast<int_x2_type>(site1.y()),
                                  static_cast<int_x2_type>(site1.x())),
                              to_fpt(1.0));
         t -= b;
         if (point_index == 2) {
           t += det.sqrt();
         } else {
           t -= det.sqrt();
```

### Comparing `voronoi-0.3.1/include/boost/polygon/detail/voronoi_robust_fpt.hpp` & `voronoi-0.4.0/include/boost/polygon/detail/voronoi_robust_fpt.hpp`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/include/boost/polygon/detail/voronoi_structures.hpp` & `voronoi-0.4.0/include/boost/polygon/detail/voronoi_structures.hpp`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/include/boost/polygon/isotropy.hpp` & `voronoi-0.4.0/include/boost/polygon/isotropy.hpp`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/include/boost/polygon/point_concept.hpp` & `voronoi-0.4.0/include/boost/polygon/point_concept.hpp`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/include/boost/polygon/point_traits.hpp` & `voronoi-0.4.0/include/boost/polygon/point_traits.hpp`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/include/boost/polygon/segment_concept.hpp` & `voronoi-0.4.0/include/boost/polygon/segment_concept.hpp`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/include/boost/polygon/segment_traits.hpp` & `voronoi-0.4.0/include/boost/polygon/segment_traits.hpp`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/include/boost/polygon/voronoi.hpp` & `voronoi-0.4.0/include/boost/polygon/voronoi.hpp`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/include/boost/polygon/voronoi_builder.hpp` & `voronoi-0.4.0/include/boost/polygon/voronoi_builder.hpp`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/include/boost/polygon/voronoi_diagram.hpp` & `voronoi-0.4.0/include/boost/polygon/voronoi_diagram.hpp`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/include/boost/polygon/voronoi_geometry_type.hpp` & `voronoi-0.4.0/include/boost/polygon/voronoi_geometry_type.hpp`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/setup.py` & `voronoi-0.4.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,25 @@
 import platform
-from pathlib import Path
 
 from setuptools import (find_packages,
                         setup)
 
-import voronoi
-
 project_base_url = 'https://github.com/lycantropos/voronoi/'
-
-
-def read_file(path_string: str) -> str:
-    return Path(path_string).read_text(encoding='utf-8')
-
-
-parameters = dict(
-        name=voronoi.__name__,
-        packages=find_packages(exclude=('tests', 'tests.*')),
-        version=voronoi.__version__,
-        description=voronoi.__doc__,
-        long_description=read_file('README.md'),
-        long_description_content_type='text/markdown',
-        author='Azat Ibrakov',
-        author_email='azatibrakov@gmail.com',
-        license='MIT License',
-        classifiers=[
-            'License :: OSI Approved :: MIT License',
-            'Programming Language :: Python :: 3.5',
-            'Programming Language :: Python :: 3.6',
-            'Programming Language :: Python :: 3.7',
-            'Programming Language :: Python :: 3.8',
-            'Programming Language :: Python :: 3.9',
-            'Programming Language :: Python :: Implementation :: CPython',
-            'Programming Language :: Python :: Implementation :: PyPy',
-        ],
-        url=project_base_url,
-        download_url=project_base_url + 'archive/master.zip',
-        python_requires='>=3.5',
-        setup_requires=read_file('requirements-setup.txt'),
-        install_requires=read_file('requirements.txt'))
+parameters = dict(packages=find_packages(exclude=('tests', 'tests.*')),
+                  url=project_base_url,
+                  download_url=project_base_url + 'archive/master.zip')
 if platform.python_implementation() == 'CPython':
     import sys
     import tempfile
     from collections import defaultdict
     from datetime import date
     from distutils.ccompiler import CCompiler
     from distutils.errors import CompileError
     from glob import glob
+    from pathlib import Path
     from typing import (Any,
                         Iterable)
 
     from setuptools import (Command,
                             Extension)
     from setuptools.command.build_ext import build_ext
     from setuptools.command.develop import develop
@@ -88,15 +58,15 @@
 
     class BuildExt(build_ext):
         """A custom build extension for adding compiler-specific options."""
         compile_args = defaultdict(list, {'msvc': ['/EHsc'], 'unix': []})
         link_args = defaultdict(list, {'msvc': [], 'unix': []})
 
         if sys.platform == 'darwin':
-            darwin_args = ['-stdlib=libc++', '-mmacosx-version-min=10.7']
+            darwin_args = ['-stdlib=libc++', '-mmacosx-version-min=12.0']
             compile_args['unix'] += darwin_args
             link_args['unix'] += darwin_args
 
         def build_extensions(self) -> None:
             compiler_type = self.compiler.compiler_type
             compile_args = self.compile_args[compiler_type]
             link_args = self.link_args[compiler_type]
@@ -151,14 +121,15 @@
             return pybind11.get_include()
 
 
     project_root = Path(__file__).parent
     parameters.update(
             cmdclass={build_ext.__name__: BuildExt,
                       develop.__name__: Develop},
-            ext_modules=[Extension('_' + voronoi.__name__,
+            ext_modules=[Extension('_voronoi',
                                    glob('src/*.cpp'),
                                    include_dirs=[LazyPybindInclude(),
                                                  project_root / 'include'],
                                    language='c++')],
-            zip_safe=False)
+            zip_safe=False
+    )
 setup(**parameters)
```

### Comparing `voronoi-0.3.1/src/main.cpp` & `voronoi-0.4.0/src/main.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 using Orientation = Predicates::orientation_test::Orientation;
 using Vertex = boost::polygon::voronoi_vertex<double>;
 
 static int to_sign(coordinate_t value) {
   return value > 0 ? 1 : (value < 0 ? -1 : 0);
 }
 
-static std::string bool_repr(bool value) { return py::str(py::bool_(value)); }
+static std::string bool_repr(bool value) { return value ? "True" : "False"; }
 
 template <class Object>
 std::string to_repr(const Object& object) {
   std::ostringstream stream;
   stream.precision(std::numeric_limits<double>::digits10 + 2);
   stream << object;
   return stream.str();
```

### Comparing `voronoi-0.3.1/voronoi/beach_line_key.py` & `voronoi-0.4.0/voronoi/beach_line_key.py`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/voronoi/big_int.py` & `voronoi-0.4.0/voronoi/big_int.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import ctypes
 from math import (copysign,
                   inf,
                   ldexp)
 from typing import (List,
                     Tuple)
 
@@ -20,18 +22,18 @@
         if not (sign and digits):
             sign, digits = 0, []
         self.digits = digits
         self.sign = sign if digits else 0
 
     __repr__ = generate_repr(__init__)
 
-    def __abs__(self) -> 'BigInt':
+    def __abs__(self) -> BigInt:
         return BigInt(abs(self.sign), self.digits)
 
-    def __add__(self, other: 'BigInt') -> 'BigInt':
+    def __add__(self, other: BigInt) -> BigInt:
         result = BigInt(0, [])
         result._add(self, other)
         return result
 
     def __bool__(self) -> bool:
         return bool(self.sign)
 
@@ -46,39 +48,39 @@
     def __float__(self) -> float:
         mantissa, exponent = self.frexp()
         try:
             return ldexp(mantissa, exponent)
         except OverflowError:
             return copysign(inf, mantissa)
 
-    def __mul__(self, other: 'BigInt') -> 'BigInt':
+    def __mul__(self, other: BigInt) -> BigInt:
         result = BigInt(0, [])
         result._multiply(self, other)
         return result
 
-    def __neg__(self) -> 'BigInt':
+    def __neg__(self) -> BigInt:
         return BigInt(-self.sign, self.digits[:])
 
-    def __sub__(self, other: 'BigInt') -> 'BigInt':
+    def __sub__(self, other: BigInt) -> BigInt:
         result = BigInt(0, [])
         result._subtract(self, other)
         return result
 
     @classmethod
-    def from_int32(cls, value: int) -> 'BigInt':
+    def from_int32(cls, value: int) -> BigInt:
         if value > 0:
             sign, digits = 1, [_to_uint32(value)]
         elif value < 0:
             sign, digits = -1, [_to_uint32(-value)]
         else:
             sign, digits = 0, []
         return cls(sign, digits)
 
     @classmethod
-    def from_int64(cls, value: int) -> 'BigInt':
+    def from_int64(cls, value: int) -> BigInt:
         if value > 0:
             sign, digits = 1, [_to_uint32(value)]
             value >>= 32
             if value:
                 digits.append(value)
         elif value < 0:
             value = -value
@@ -106,15 +108,15 @@
                     mantissa *= float(0x100000000)
                     mantissa += float(self.digits[size - index])
                 exponent = (size - 3) << 5
         if self.sign < 0:
             mantissa = -mantissa
         return mantissa, exponent
 
-    def _add(self, left: 'BigInt', right: 'BigInt') -> None:
+    def _add(self, left: BigInt, right: BigInt) -> None:
         if not left.sign:
             self.sign, self.digits = right.sign, right.digits[:]
             return
         elif not right.sign:
             self.sign, self.digits = left.sign, left.digits[:]
             return
         elif left.sign == right.sign:
@@ -136,20 +138,20 @@
         cursor = 0
         for index, right_digit in enumerate(right_digits):
             cursor += left_digits[index] + right_digit
             self.digits.append(_to_uint32(cursor))
             cursor >>= 32
         for index in range(right_size, left_size):
             cursor += left_digits[index]
-            self.digits.append(cursor)
+            self.digits.append(_to_uint32(cursor))
             cursor >>= 32
         if cursor and len(self.digits) < MAX_DIGITS_COUNT:
             self.digits.append(cursor)
 
-    def _multiply(self, left: 'BigInt', right: 'BigInt') -> None:
+    def _multiply(self, left: BigInt, right: BigInt) -> None:
         if not left.sign or not right.sign:
             return
         self._multiply_digits(left.digits, right.digits)
         if left.sign != right.sign:
             self.sign = -self.sign
 
     def _multiply_digits(self,
@@ -170,15 +172,15 @@
                 current_digit += _to_uint32(step)
                 next_digit += step >> 32
             self.digits.append(_to_uint32(current_digit))
             current_digit = next_digit + (current_digit >> 32)
         if current_digit and len(self.digits) < MAX_DIGITS_COUNT:
             self.digits.append(_to_uint32(current_digit))
 
-    def _subtract(self, left: 'BigInt', right: 'BigInt') -> None:
+    def _subtract(self, left: BigInt, right: BigInt) -> None:
         if not left.sign:
             self.sign, self.digits = -right.sign, right.digits[:]
             return
         elif not right.sign:
             self.sign, self.digits = left.sign, left.digits[:]
             return
         elif left.sign == right.sign:
```

### Comparing `voronoi-0.3.1/voronoi/builder.py` & `voronoi-0.4.0/voronoi/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import ctypes
 from copy import copy
 from operator import itemgetter
 from typing import (TYPE_CHECKING,
                     List,
                     Optional,
                     Tuple)
 
@@ -21,15 +22,23 @@
 from .utils import to_unique_just_seen
 
 if TYPE_CHECKING:
     from .diagram import Diagram
 
 
 class Builder:
-    __slots__ = ('index', '_beach_line', '_circle_events', '_end_points',
+    @property
+    def index(self) -> int:
+        return self._index
+
+    @index.setter
+    def index(self, value: int) -> None:
+        self._index = ctypes.c_size_t(value).value
+
+    __slots__ = ('_index', '_beach_line', '_circle_events', '_end_points',
                  'site_events', '_site_event_index')
 
     def __init__(self,
                  index: int = 0,
                  site_events: Optional[List[SiteEvent]] = None) -> None:
         self.index = index
         self._beach_line = red_black.Tree.from_components([])
```

### Comparing `voronoi-0.3.1/voronoi/diagram.py` & `voronoi-0.4.0/voronoi/diagram.py`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/voronoi/enums.py` & `voronoi-0.4.0/voronoi/enums.py`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/voronoi/events/computers.py` & `voronoi-0.4.0/voronoi/events/computers.py`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/voronoi/events/models.py` & `voronoi-0.4.0/voronoi/events/models.py`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/voronoi/events/predicates.py` & `voronoi-0.4.0/voronoi/events/predicates.py`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/voronoi/faces.py` & `voronoi-0.4.0/voronoi/faces.py`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/voronoi/point.py` & `voronoi-0.4.0/voronoi/point.py`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/voronoi/robust_difference.py` & `voronoi-0.4.0/voronoi/robust_difference.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,125 +1,133 @@
+from __future__ import annotations
+
 from typing import Union
 
 from reprit.base import generate_repr
 
 from .robust_float import RobustFloat
 
 
 class RobustDifference:
     __slots__ = 'minuend', 'subtrahend'
 
     def __init__(self, minuend: RobustFloat, subtrahend: RobustFloat) -> None:
-        self.minuend = minuend
-        self.subtrahend = subtrahend
+        self.minuend, self.subtrahend = minuend, subtrahend
 
     __repr__ = generate_repr(__init__)
 
-    def __abs__(self) -> 'RobustDifference':
+    def __abs__(self) -> RobustDifference:
         return (-self
                 if self.minuend.value < self.subtrahend.value
                 else self)
 
-    def __add__(self, other: Union[RobustFloat, 'RobustDifference']
-                ) -> 'RobustDifference':
+    def __add__(
+            self, other: Union[RobustFloat, RobustDifference]
+    ) -> RobustDifference:
         if isinstance(other, RobustDifference):
             minuend, subtrahend = (self.minuend + other.minuend,
                                    self.subtrahend + other.subtrahend)
         elif other < 0:
             minuend, subtrahend = self.minuend, self.subtrahend - other
         else:
             minuend, subtrahend = self.minuend + other, self.subtrahend
         return RobustDifference(minuend, subtrahend)
 
-    def __iadd__(self, other: Union[RobustFloat, 'RobustDifference']
-                 ) -> 'RobustDifference':
+    def __iadd__(
+            self, other: Union[RobustFloat, RobustDifference]
+    ) -> RobustDifference:
         if isinstance(other, RobustDifference):
             self.minuend += other.minuend
             self.subtrahend += other.subtrahend
         elif other < 0:
             self.subtrahend -= other
         else:
             self.minuend += other
         return self
 
-    def __imul__(self, other: Union[RobustFloat, 'RobustDifference']
-                 ) -> 'RobustDifference':
+    def __imul__(
+            self, other: Union[RobustFloat, RobustDifference]
+    ) -> RobustDifference:
         if isinstance(other, RobustDifference):
             self.minuend, self.subtrahend = (
                 self.minuend * other.minuend
                 + self.subtrahend * other.subtrahend,
                 self.minuend * other.subtrahend
-                + self.subtrahend * other.minuend)
+                + self.subtrahend * other.minuend
+            )
         elif other < 0:
             other = -other
             self.minuend *= other
             self.subtrahend *= other
             self.minuend, self.subtrahend = self.subtrahend, self.minuend
         else:
             self.minuend *= other
             self.subtrahend *= other
         return self
 
-    def __isub__(self, other: Union[RobustFloat, 'RobustDifference']
-                 ) -> 'RobustDifference':
+    def __isub__(
+            self, other: Union[RobustFloat, RobustDifference]
+    ) -> RobustDifference:
         if isinstance(other, RobustDifference):
             self.minuend += other.subtrahend
             self.subtrahend += other.minuend
         elif other < 0:
             self.minuend -= other
         else:
             self.subtrahend += other
         return self
 
-    def __itruediv__(self, other: RobustFloat) -> 'RobustDifference':
+    def __itruediv__(self, other: RobustFloat) -> RobustDifference:
         if other < 0:
             other = -other
             self.subtrahend /= other
             self.minuend /= other
             self.minuend, self.subtrahend = self.subtrahend, self.minuend
         else:
             self.minuend /= other
             self.subtrahend /= other
         return self
 
-    def __mul__(self, other: Union[RobustFloat, 'RobustDifference']
-                ) -> 'RobustDifference':
+    def __mul__(
+            self, other: Union[RobustFloat, RobustDifference]
+    ) -> RobustDifference:
         if isinstance(other, RobustDifference):
             minuend, subtrahend = (self.minuend * other.minuend
                                    + self.subtrahend * other.subtrahend,
                                    self.minuend * other.subtrahend
                                    + self.subtrahend * other.minuend)
         elif other < 0:
             other = -other
             minuend, subtrahend = self.subtrahend * other, self.minuend * other
         else:
             minuend, subtrahend = self.minuend * other, self.subtrahend * other
         return RobustDifference(minuend, subtrahend)
 
-    def __neg__(self) -> 'RobustDifference':
+    def __neg__(self) -> RobustDifference:
         return RobustDifference(self.subtrahend, self.minuend)
 
-    def __sub__(self, other: Union[RobustFloat, 'RobustDifference']
-                ) -> 'RobustDifference':
+    def __sub__(
+            self, other: Union[RobustFloat, RobustDifference]
+    ) -> RobustDifference:
         if isinstance(other, RobustDifference):
             minuend, subtrahend = (self.minuend + other.subtrahend,
                                    self.subtrahend + other.minuend)
         elif other < 0:
             minuend, subtrahend = self.minuend - other, self.subtrahend
         else:
             minuend, subtrahend = self.minuend, self.subtrahend + other
         return RobustDifference(minuend, subtrahend)
 
-    def __truediv__(self, other: RobustFloat) -> 'RobustDifference':
+    def __truediv__(self, other: RobustFloat) -> RobustDifference:
         if other < 0:
             other = -other
             minuend, subtrahend = self.subtrahend / other, self.minuend / other
         else:
             minuend, subtrahend = self.minuend / other, self.subtrahend / other
         return RobustDifference(minuend, subtrahend)
 
     @classmethod
-    def zero(cls) -> 'RobustDifference':
+    def zero(cls) -> RobustDifference:
         return cls(RobustFloat(), RobustFloat())
 
     def evaluate(self) -> RobustFloat:
         return self.minuend - self.subtrahend
```

### Comparing `voronoi-0.3.1/voronoi/robust_float.py` & `voronoi-0.4.0/voronoi/robust_float.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from functools import total_ordering
 from typing import Any
 
 from reprit.base import generate_repr
 
 from .utils import (safe_divide_floats,
                     safe_sqrt)
@@ -15,18 +17,18 @@
 
     def __init__(self, value: float = 0., relative_error: float = 0.) -> None:
         self.value = value
         self.relative_error = relative_error
 
     __repr__ = generate_repr(__init__)
 
-    def __abs__(self) -> 'RobustFloat':
+    def __abs__(self) -> RobustFloat:
         return RobustFloat(abs(self.value), self.relative_error)
 
-    def __add__(self, other: 'RobustFloat') -> 'RobustFloat':
+    def __add__(self, other: RobustFloat) -> RobustFloat:
         value = self.value + other.value
         relative_error = (max(self.relative_error, other.relative_error)
                           + ROUNDING_ERROR
                           if (not self.value or not other.value
                               or (self.value > 0) is (other.value > 0))
                           else
                           abs(safe_divide_floats(
@@ -40,49 +42,49 @@
 
     def __eq__(self, other: Any) -> bool:
         return self.value == other
 
     def __gt__(self, other: Any) -> bool:
         return self.value > other
 
-    def __imul__(self, other: 'RobustFloat') -> 'RobustFloat':
+    def __imul__(self, other: RobustFloat) -> RobustFloat:
         self.value *= other.value
         self.relative_error += other.relative_error + ROUNDING_ERROR
         return self
 
-    def __itruediv__(self, other: 'RobustFloat') -> 'RobustFloat':
+    def __itruediv__(self, other: RobustFloat) -> RobustFloat:
         self.value = safe_divide_floats(self.value, other.value)
         self.relative_error += other.relative_error + ROUNDING_ERROR
         return self
 
     def __lt__(self, other: Any) -> bool:
         return self.value < other
 
-    def __mul__(self, other: 'RobustFloat') -> 'RobustFloat':
+    def __mul__(self, other: RobustFloat) -> RobustFloat:
         return RobustFloat(self.value * other.value,
                            self.relative_error + other.relative_error
                            + ROUNDING_ERROR)
 
-    def __neg__(self) -> 'RobustFloat':
+    def __neg__(self) -> RobustFloat:
         return RobustFloat(-self.value, self.relative_error)
 
-    def __sub__(self, other: 'RobustFloat') -> 'RobustFloat':
+    def __sub__(self, other: RobustFloat) -> RobustFloat:
         value = self.value - other.value
         relative_error = (max(self.relative_error, other.relative_error)
                           + ROUNDING_ERROR
                           if (not self.value or not other.value
                               or (self.value > 0) is not (other.value > 0))
                           else
                           abs(safe_divide_floats(
                                   self.value * self.relative_error
                                   + other.value * other.relative_error, value))
                           + ROUNDING_ERROR)
         return RobustFloat(value, relative_error)
 
-    def __truediv__(self, other: 'RobustFloat') -> 'RobustFloat':
+    def __truediv__(self, other: RobustFloat) -> RobustFloat:
         return RobustFloat(safe_divide_floats(self.value, other.value),
                            self.relative_error + other.relative_error
                            + ROUNDING_ERROR)
 
-    def sqrt(self) -> 'RobustFloat':
+    def sqrt(self) -> RobustFloat:
         return RobustFloat(safe_sqrt(self.value),
                            self.relative_error * 0.5 + ROUNDING_ERROR)
```

### Comparing `voronoi-0.3.1/voronoi/utils.py` & `voronoi-0.4.0/voronoi/utils.py`

 * *Files identical despite different names*

### Comparing `voronoi-0.3.1/voronoi.egg-info/PKG-INFO` & `voronoi-0.4.0/voronoi.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,58 @@
 Metadata-Version: 2.1
 Name: voronoi
-Version: 0.3.1
-Summary: Voronoi decomposition.
+Version: 0.4.0
 Home-page: https://github.com/lycantropos/voronoi/
-Author: Azat Ibrakov
-Author-email: azatibrakov@gmail.com
-License: MIT License
 Download-URL: https://github.com/lycantropos/voronoi/archive/master.zip
-Platform: UNKNOWN
+Author-email: Azat Ibrakov <azatibrakov@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2020 Azat Ibrakov
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 License-File: LICENSE
 
 voronoi
 =======
 
-[![](https://dev.azure.com/lycantropos/voronoi/_apis/build/status/lycantropos.voronoi?branchName=master)](https://dev.azure.com/lycantropos/voronoi/_build/latest?definitionId=29&branchName=master "Azure Pipelines")
+[![](https://github.com/lycantropos/voronoi/workflows/CI/badge.svg)](https://github.com/lycantropos/voronoi/actions/workflows/ci.yml "Github Actions")
 [![](https://codecov.io/gh/lycantropos/voronoi/branch/master/graph/badge.svg)](https://codecov.io/gh/lycantropos/voronoi "Codecov")
 [![](https://img.shields.io/github/license/lycantropos/voronoi.svg)](https://github.com/lycantropos/voronoi/blob/master/LICENSE "License")
 [![](https://badge.fury.io/py/voronoi.svg)](https://badge.fury.io/py/voronoi "PyPI")
 
-In what follows `python` is an alias for `python3.5` or `pypy3.5`
-or any later version (`python3.6`, `pypy3.6` and so on).
+In what follows `python` is an alias for `python3.7` or `pypy3.7`
+or any later version (`python3.8`, `pypy3.8` and so on).
 
 Installation
 ------------
 
 Install the latest `pip` & `setuptools` packages versions
 ```bash
 python -m pip install --upgrade pip setuptools
@@ -172,9 +191,7 @@
   ```powershell
   .\run-tests.ps1 cpython
   ```
 - with `PyPy`
   ```powershell
   .\run-tests.ps1 pypy
   ```
-
-
```

### Comparing `voronoi-0.3.1/voronoi.egg-info/SOURCES.txt` & `voronoi-0.4.0/voronoi.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
-requirements-setup.txt
-requirements.txt
+pyproject.toml
 setup.py
 include/boost/polygon/isotropy.hpp
 include/boost/polygon/point_concept.hpp
 include/boost/polygon/point_traits.hpp
 include/boost/polygon/segment_concept.hpp
 include/boost/polygon/segment_traits.hpp
 include/boost/polygon/voronoi.hpp
```


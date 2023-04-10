# Comparing `tmp/pcb-parser-0.0.4.tar.gz` & `tmp/pcb-parser-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcb-parser-0.0.4.tar", last modified: Mon Apr 10 04:55:31 2023, max compression
+gzip compressed data, was "pcb-parser-0.0.5.tar", last modified: Mon Apr 10 04:59:56 2023, max compression
```

## Comparing `pcb-parser-0.0.4.tar` & `pcb-parser-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 04:55:31.682112 pcb-parser-0.0.4/
--rwxrwxrwx   0 root         (0) root         (0)     1065 2023-02-20 02:12:16.000000 pcb-parser-0.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      412 2023-04-10 04:55:31.682112 pcb-parser-0.0.4/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-03 04:33:47.000000 pcb-parser-0.0.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 04:55:31.683112 pcb-parser-0.0.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      688 2023-04-10 04:55:18.000000 pcb-parser-0.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 04:55:31.680112 pcb-parser-0.0.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 04:55:31.681112 pcb-parser-0.0.4/src/pcb_parser/
--rwxrwxrwx   0 root         (0) root         (0)       72 2023-03-02 23:43:20.000000 pcb-parser-0.0.4/src/pcb_parser/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      924 2023-03-30 05:32:08.000000 pcb-parser-0.0.4/src/pcb_parser/abs.py
--rwxr-xr-x   0 root         (0) root         (0)    29966 2023-04-10 04:54:03.000000 pcb-parser-0.0.4/src/pcb_parser/geometry.py
--rwxr-xr-x   0 root         (0) root         (0)     6744 2023-04-10 04:54:03.000000 pcb-parser-0.0.4/src/pcb_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     1100 2023-04-04 08:44:09.000000 pcb-parser-0.0.4/src/pcb_parser/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 04:55:31.682112 pcb-parser-0.0.4/src/pcb_parser.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-10 04:55:31.000000 pcb-parser-0.0.4/src/pcb_parser.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      303 2023-04-10 04:55:31.000000 pcb-parser-0.0.4/src/pcb_parser.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-10 04:55:31.000000 pcb-parser-0.0.4/src/pcb_parser.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       11 2023-04-10 04:55:31.000000 pcb-parser-0.0.4/src/pcb_parser.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 04:59:56.248246 pcb-parser-0.0.5/
+-rwxrwxrwx   0 root         (0) root         (0)     1065 2023-02-20 02:12:16.000000 pcb-parser-0.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      412 2023-04-10 04:59:56.248246 pcb-parser-0.0.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-03 04:33:47.000000 pcb-parser-0.0.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 04:59:56.248246 pcb-parser-0.0.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      688 2023-04-10 04:59:40.000000 pcb-parser-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 04:59:56.246246 pcb-parser-0.0.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 04:59:56.247246 pcb-parser-0.0.5/src/pcb_parser/
+-rwxrwxrwx   0 root         (0) root         (0)       72 2023-03-02 23:43:20.000000 pcb-parser-0.0.5/src/pcb_parser/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      924 2023-03-30 05:32:08.000000 pcb-parser-0.0.5/src/pcb_parser/abs.py
+-rwxr-xr-x   0 root         (0) root         (0)    29966 2023-04-10 04:54:03.000000 pcb-parser-0.0.5/src/pcb_parser/geometry.py
+-rwxr-xr-x   0 root         (0) root         (0)     6848 2023-04-10 04:59:19.000000 pcb-parser-0.0.5/src/pcb_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1100 2023-04-04 08:44:09.000000 pcb-parser-0.0.5/src/pcb_parser/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 04:59:56.248246 pcb-parser-0.0.5/src/pcb_parser.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-10 04:59:56.000000 pcb-parser-0.0.5/src/pcb_parser.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      303 2023-04-10 04:59:56.000000 pcb-parser-0.0.5/src/pcb_parser.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-10 04:59:56.000000 pcb-parser-0.0.5/src/pcb_parser.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       11 2023-04-10 04:59:56.000000 pcb-parser-0.0.5/src/pcb_parser.egg-info/top_level.txt
```

### Comparing `pcb-parser-0.0.4/LICENSE` & `pcb-parser-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pcb-parser-0.0.4/setup.py` & `pcb-parser-0.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open('README.md', 'r') as f:
     long_description = f.read()
     
 setuptools.setup(
     name = 'pcb-parser',
-    version = 'v0.0.4',
+    version = 'v0.0.5',
     author = 'Changyun Choi',
     author_email = "cyun9601@gmail.com",
     description = "PCB Parser",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/cyun9601/PCB_Parser",
     package_dir={"": "src"},
```

### Comparing `pcb-parser-0.0.4/src/pcb_parser/abs.py` & `pcb-parser-0.0.5/src/pcb_parser/abs.py`

 * *Files identical despite different names*

### Comparing `pcb-parser-0.0.4/src/pcb_parser/geometry.py` & `pcb-parser-0.0.5/src/pcb_parser/geometry.py`

 * *Files identical despite different names*

### Comparing `pcb-parser-0.0.4/src/pcb_parser/parser.py` & `pcb-parser-0.0.5/src/pcb_parser/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,18 @@
         merged_img, collision = self.merge_polygon(board_cv_img, self.board, self.hole_area, inplace=False)
         self.state = [copy.deepcopy(merged_img), copy.deepcopy(merged_img)]
         
     def initialize_components(self):
         for comp in self.components_dict.values():
             comp.initialize()
         
+    def reset(self):
+        self.initialize_background()
+        self.initialize_components()
+        
     def get_fixed_components(self) -> list[str]:
         return [comp.name for comp in self.components_dict.values() if comp.fixed]
     
     def get_unfixed_components(self) -> list[str]:
         return [comp.name for comp in self.components_dict.values() if not comp.fixed]
     
     def move_to_pix(self, component_name, pix_x:int, pix_y:int):
```

### Comparing `pcb-parser-0.0.4/src/pcb_parser/utils.py` & `pcb-parser-0.0.5/src/pcb_parser/utils.py`

 * *Files identical despite different names*


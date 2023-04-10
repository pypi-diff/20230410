# Comparing `tmp/pcb-parser-0.0.3.tar.gz` & `tmp/pcb-parser-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcb-parser-0.0.3.tar", last modified: Wed Apr  5 02:37:46 2023, max compression
+gzip compressed data, was "pcb-parser-0.0.4.tar", last modified: Mon Apr 10 04:55:31 2023, max compression
```

## Comparing `pcb-parser-0.0.3.tar` & `pcb-parser-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 02:37:46.834540 pcb-parser-0.0.3/
--rwxrwxrwx   0 root         (0) root         (0)     1065 2023-02-20 02:12:16.000000 pcb-parser-0.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      412 2023-04-05 02:37:46.834540 pcb-parser-0.0.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-03 04:33:47.000000 pcb-parser-0.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-05 02:37:46.834540 pcb-parser-0.0.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      688 2023-04-05 02:36:22.000000 pcb-parser-0.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 02:37:46.832540 pcb-parser-0.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 02:37:46.833540 pcb-parser-0.0.3/src/pcb_parser/
--rwxrwxrwx   0 root         (0) root         (0)       72 2023-03-02 23:43:20.000000 pcb-parser-0.0.3/src/pcb_parser/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      924 2023-03-30 05:32:08.000000 pcb-parser-0.0.3/src/pcb_parser/abs.py
--rwxr-xr-x   0 root         (0) root         (0)    29866 2023-04-05 01:31:51.000000 pcb-parser-0.0.3/src/pcb_parser/geometry.py
--rwxr-xr-x   0 root         (0) root         (0)     6439 2023-04-05 02:33:43.000000 pcb-parser-0.0.3/src/pcb_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     1100 2023-04-04 08:44:09.000000 pcb-parser-0.0.3/src/pcb_parser/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 02:37:46.833540 pcb-parser-0.0.3/src/pcb_parser.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-05 02:37:46.000000 pcb-parser-0.0.3/src/pcb_parser.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      303 2023-04-05 02:37:46.000000 pcb-parser-0.0.3/src/pcb_parser.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-05 02:37:46.000000 pcb-parser-0.0.3/src/pcb_parser.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       11 2023-04-05 02:37:46.000000 pcb-parser-0.0.3/src/pcb_parser.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 04:55:31.682112 pcb-parser-0.0.4/
+-rwxrwxrwx   0 root         (0) root         (0)     1065 2023-02-20 02:12:16.000000 pcb-parser-0.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      412 2023-04-10 04:55:31.682112 pcb-parser-0.0.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-03 04:33:47.000000 pcb-parser-0.0.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 04:55:31.683112 pcb-parser-0.0.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      688 2023-04-10 04:55:18.000000 pcb-parser-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 04:55:31.680112 pcb-parser-0.0.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 04:55:31.681112 pcb-parser-0.0.4/src/pcb_parser/
+-rwxrwxrwx   0 root         (0) root         (0)       72 2023-03-02 23:43:20.000000 pcb-parser-0.0.4/src/pcb_parser/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      924 2023-03-30 05:32:08.000000 pcb-parser-0.0.4/src/pcb_parser/abs.py
+-rwxr-xr-x   0 root         (0) root         (0)    29966 2023-04-10 04:54:03.000000 pcb-parser-0.0.4/src/pcb_parser/geometry.py
+-rwxr-xr-x   0 root         (0) root         (0)     6744 2023-04-10 04:54:03.000000 pcb-parser-0.0.4/src/pcb_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1100 2023-04-04 08:44:09.000000 pcb-parser-0.0.4/src/pcb_parser/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 04:55:31.682112 pcb-parser-0.0.4/src/pcb_parser.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-10 04:55:31.000000 pcb-parser-0.0.4/src/pcb_parser.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      303 2023-04-10 04:55:31.000000 pcb-parser-0.0.4/src/pcb_parser.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-10 04:55:31.000000 pcb-parser-0.0.4/src/pcb_parser.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       11 2023-04-10 04:55:31.000000 pcb-parser-0.0.4/src/pcb_parser.egg-info/top_level.txt
```

### Comparing `pcb-parser-0.0.3/LICENSE` & `pcb-parser-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pcb-parser-0.0.3/setup.py` & `pcb-parser-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open('README.md', 'r') as f:
     long_description = f.read()
     
 setuptools.setup(
     name = 'pcb-parser',
-    version = 'v0.0.3',
+    version = 'v0.0.4',
     author = 'Changyun Choi',
     author_email = "cyun9601@gmail.com",
     description = "PCB Parser",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/cyun9601/PCB_Parser",
     package_dir={"": "src"},
```

### Comparing `pcb-parser-0.0.3/src/pcb_parser/abs.py` & `pcb-parser-0.0.4/src/pcb_parser/abs.py`

 * *Files identical despite different names*

### Comparing `pcb-parser-0.0.3/src/pcb_parser/geometry.py` & `pcb-parser-0.0.4/src/pcb_parser/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -596,25 +596,29 @@
             self.pin_dict = data['PinDict']
             self.fixed = data['Fixed']
             self.group = data['Group']
         else:
             NotImplementedError
 
         self.p_resolution = p_resolution
+
+        # Component 초기화 
+        # self.initialize()
         
+    def initialize(self) -> None:
         # unfixed component 에 대한 처리
         if self.fixed == False: 
             ## placed layer에 따라 스위칭
             if self.placed_layer == 'BOTTOM': 
                 self.switch_layer()
                 
             ## angle을 0으로 초기화
-            # self.rotation(-self.angle, inplace=True)
+            self.rotation(-self.angle, inplace=True)
             
-    def switch_layer(self):
+    def switch_layer(self) -> None:
         self.placed_layer = 'TOP' if self.placed_layer == 'BOTTOM' else 'BOTTOM'
         self.top_area, self.bottom_area = self.bottom_area, self.top_area
         self.top_prohibit_area, self.bottom_prohibit_area = self.bottom_prohibit_area, self.top_prohibit_area
 
     def draw_cv(self, fill='in') -> tuple[np.array, np.array]:
         # 기존에 그린게 있으면 해당 값을 반환
         # if 'self.cv_top_img' in locals():
```

### Comparing `pcb-parser-0.0.3/src/pcb_parser/parser.py` & `pcb-parser-0.0.4/src/pcb_parser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,23 @@
         self.file_format = self.pcb_info['FileFormat']
         self.board = Polygon(self.pcb_info['BOARD_FIGURE'], p_resolution)
         self.hole_area = Polygon(self.pcb_info['HoleArea'], p_resolution)
         self.prohibit_area = Polygon(self.pcb_info['ProhibitArea'], p_resolution)
         self.components_dict = {comp_info['Name']:Component(comp_info, p_resolution) for comp_info in self.pcb_info['ComponentDict'].values()}
         self.net_list = dict(zip(self.pcb_info['NetDict'].keys(), [Net(net_info) for net_info in list(self.pcb_info['NetDict'].values())]))
         
-        # 초기화 
+        # 초기화
+        ## 초기 이미지 생성  
         self.initialize_cv_img()
+        
+        ## Background 초기화 -> self.state 생성  
         self.initialize_background()
+        
+        ## Component 초기화 
+        self.initialize_components()
     
     def initialize_cv_img(self):
         # initialize
         print('Board 이미지 생성 중...')
         self.board.draw_cv()
         self.hole_area.draw_cv()
         self.prohibit_area.draw_cv()         
@@ -42,14 +48,18 @@
     
     def initialize_background(self):
         board_cv_img = self.board.draw_cv(fill='out')
 
         merged_img, collision = self.merge_polygon(board_cv_img, self.board, self.hole_area, inplace=False)
         self.state = [copy.deepcopy(merged_img), copy.deepcopy(merged_img)]
         
+    def initialize_components(self):
+        for comp in self.components_dict.values():
+            comp.initialize()
+        
     def get_fixed_components(self) -> list[str]:
         return [comp.name for comp in self.components_dict.values() if comp.fixed]
     
     def get_unfixed_components(self) -> list[str]:
         return [comp.name for comp in self.components_dict.values() if not comp.fixed]
     
     def move_to_pix(self, component_name, pix_x:int, pix_y:int):
```

### Comparing `pcb-parser-0.0.3/src/pcb_parser/utils.py` & `pcb-parser-0.0.4/src/pcb_parser/utils.py`

 * *Files identical despite different names*


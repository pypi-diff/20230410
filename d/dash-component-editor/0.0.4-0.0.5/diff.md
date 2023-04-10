# Comparing `tmp/dash_component_editor-0.0.4.tar.gz` & `tmp/dash_component_editor-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_component_editor-0.0.4.tar", last modified: Sun Apr  9 01:07:08 2023, max compression
+gzip compressed data, was "dash_component_editor-0.0.5.tar", last modified: Mon Apr 10 20:32:47 2023, max compression
```

## Comparing `dash_component_editor-0.0.4.tar` & `dash_component_editor-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 zhuowen    (501) staff       (20)        0 2023-04-09 01:07:08.311154 dash_component_editor-0.0.4/
--rw-r--r--   0 zhuowen    (501) staff       (20)     2401 2023-03-27 16:49:46.000000 dash_component_editor-0.0.4/LICENSE.txt
--rw-r--r--   0 zhuowen    (501) staff       (20)     2821 2023-04-09 01:07:08.310989 dash_component_editor-0.0.4/PKG-INFO
--rw-r--r--   0 zhuowen    (501) staff       (20)     2189 2023-04-09 00:41:40.000000 dash_component_editor-0.0.4/README.md
--rw-r--r--   0 zhuowen    (501) staff       (20)       38 2023-04-09 01:07:08.311215 dash_component_editor-0.0.4/setup.cfg
--rw-r--r--   0 zhuowen    (501) staff       (20)     1652 2023-04-09 01:06:17.000000 dash_component_editor-0.0.4/setup.py
-drwxr-xr-x   0 zhuowen    (501) staff       (20)        0 2023-04-09 01:07:08.310090 dash_component_editor-0.0.4/src/
-drwxr-xr-x   0 zhuowen    (501) staff       (20)        0 2023-04-09 01:07:08.310794 dash_component_editor-0.0.4/src/dash_component_editor.egg-info/
--rw-r--r--   0 zhuowen    (501) staff       (20)     2821 2023-04-09 01:07:08.000000 dash_component_editor-0.0.4/src/dash_component_editor.egg-info/PKG-INFO
--rw-r--r--   0 zhuowen    (501) staff       (20)      303 2023-04-09 01:07:08.000000 dash_component_editor-0.0.4/src/dash_component_editor.egg-info/SOURCES.txt
--rw-r--r--   0 zhuowen    (501) staff       (20)        1 2023-04-09 01:07:08.000000 dash_component_editor-0.0.4/src/dash_component_editor.egg-info/dependency_links.txt
--rw-r--r--   0 zhuowen    (501) staff       (20)       75 2023-04-09 01:07:08.000000 dash_component_editor-0.0.4/src/dash_component_editor.egg-info/requires.txt
--rw-r--r--   0 zhuowen    (501) staff       (20)       22 2023-04-09 01:07:08.000000 dash_component_editor-0.0.4/src/dash_component_editor.egg-info/top_level.txt
--rw-r--r--   0 zhuowen    (501) staff       (20)    15045 2023-04-09 00:35:55.000000 dash_component_editor-0.0.4/src/dash_component_editor.py
+drwxr-xr-x   0 zhuowen    (501) staff       (20)        0 2023-04-10 20:32:47.488378 dash_component_editor-0.0.5/
+-rw-r--r--   0 zhuowen    (501) staff       (20)     2401 2023-03-27 16:49:46.000000 dash_component_editor-0.0.5/LICENSE.txt
+-rw-r--r--   0 zhuowen    (501) staff       (20)     3535 2023-04-10 20:32:47.488201 dash_component_editor-0.0.5/PKG-INFO
+-rw-r--r--   0 zhuowen    (501) staff       (20)     2903 2023-04-10 20:31:26.000000 dash_component_editor-0.0.5/README.md
+-rw-r--r--   0 zhuowen    (501) staff       (20)       38 2023-04-10 20:32:47.488436 dash_component_editor-0.0.5/setup.cfg
+-rwxr--r--   0 zhuowen    (501) staff       (20)     1652 2023-04-10 20:32:05.000000 dash_component_editor-0.0.5/setup.py
+drwxr-xr-x   0 zhuowen    (501) staff       (20)        0 2023-04-10 20:32:47.487092 dash_component_editor-0.0.5/src/
+drwxr-xr-x   0 zhuowen    (501) staff       (20)        0 2023-04-10 20:32:47.487989 dash_component_editor-0.0.5/src/dash_component_editor.egg-info/
+-rw-r--r--   0 zhuowen    (501) staff       (20)     3535 2023-04-10 20:32:47.000000 dash_component_editor-0.0.5/src/dash_component_editor.egg-info/PKG-INFO
+-rw-r--r--   0 zhuowen    (501) staff       (20)      303 2023-04-10 20:32:47.000000 dash_component_editor-0.0.5/src/dash_component_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 zhuowen    (501) staff       (20)        1 2023-04-10 20:32:47.000000 dash_component_editor-0.0.5/src/dash_component_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 zhuowen    (501) staff       (20)       75 2023-04-10 20:32:47.000000 dash_component_editor-0.0.5/src/dash_component_editor.egg-info/requires.txt
+-rw-r--r--   0 zhuowen    (501) staff       (20)       22 2023-04-10 20:32:47.000000 dash_component_editor-0.0.5/src/dash_component_editor.egg-info/top_level.txt
+-rw-r--r--   0 zhuowen    (501) staff       (20)    15045 2023-04-09 00:35:55.000000 dash_component_editor-0.0.5/src/dash_component_editor.py
```

### Comparing `dash_component_editor-0.0.4/LICENSE.txt` & `dash_component_editor-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dash_component_editor-0.0.4/PKG-INFO` & `dash_component_editor-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash_component_editor
-Version: 0.0.4
+Version: 0.0.5
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Zhuowen (Kevin) Zhao, Ronald Pandolfi
 Author-email: zwenzhao11@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/mlexchange/mlex_dash_component_editor.git
 Platform: UNKNOWN
@@ -18,15 +18,15 @@
 License-File: LICENSE.txt
 
 # MLExchange Dash component editor
 This script creates adaptive Dash GUI components from keyword pairs (JSON format).
 
 It currently supports 8 types of Dash GUI components: 3 types of [input forms](https://dash-bootstrap-components.opensource.faculty.ai/docs/components/input/) (int, float, str), [slider](https://dash.plotly.com/dash-core-components/slider), [dropdown](https://dash.plotly.com/dash-core-components/dropdown), [radio items](https://dash.plotly.com/dash-core-components/radioitems), [boolean toggle switch](https://dash.plotly.com/dash-daq/toggleswitch), and [image](https://dash.plotly.com/dash-html-components/img). The corresponding keyword values are 'int', 'float', 'str', 'slider', 'dropdown', 'radio', 'bool', and 'img'.
 
-Legal keyword pairs: {'type': xxx, 'name': xxx, 'title': xxx, 'param_key': xxx, 'value': xxx} and all the other legal keyword pairs in the corresponding Dash components. **Note**: 'name' is the unique string identifier.
+Legal keyword pairs: {'type': xxx, 'name': xxx, 'title': xxx, 'param_key': xxx, 'value': xxx} and all the other legal keyword pairs in the corresponding Dash components. **Note**: 'name' is the unique string identifier for each component.
 
 
 
 ## Dependencies:
 
 ```
 dash>=2.9.0
@@ -35,21 +35,26 @@
 werkzeug==2.0
 ```
 
 
 ## Code example
 
 ```python
-from dash import Dash, html
+from dash import Dash, html, Input, Output
 from dash_component_editor import JSONParameterEditor
 
 # data
 component_kwargs = {"gui_parameters": [{"type": "int", "name": "num-tree", "title": "Number of Trees", "param_key": "n_estimators", "value": "30"}, 
-                                       {"type": "int", "name": "tree-depth", "title": "Tree Depth", "param_key": "max_depth", "value": "8"}]}
-
+                                       {"type": "dropdown", "name": "dropdown-menu", "title": "Choose a City", "param_key": "city", 
+                                        "options": [{'label': 'New York City', 'value': 'New York City'}, {'label': 'Montreal', 'value': 'Montreal'},
+                                                   {'label': 'San Francisco', 'value': 'San Francisco'}], "value": "'Montreal"},
+                                       {"type": "slider", "name": "slider-id", "title": "Fahrenheit Range", "param_key": "f_temp", "min": 0, "max": 10,
+                                        "step": None, "marks": {0: '0°F', 3: '3°F', 5: '5°F', 7.65: '7.65°F', 10: '10°F'}, "value":5},
+                                       ]
+                    }
 
 # set up Dash server and web layouts
 app = Dash(__name__)
 app.layout = html.Div ([html.Button('Show GUI', id='button', n_clicks=0),
                         html.Div(id='gui-layout', children=[])
                        ])
 
@@ -63,12 +68,15 @@
 def show_gui_layouts(n_clicks):
     item_list = JSONParameterEditor(_id={'type': 'parameter_editor'},
                                     json_blob=component_kwargs["gui_parameters"],
                                 )
     item_list.init_callbacks(app)
     
     return [html.H5("GUI Layout", className="card-title"), item_list]
+
+
+app.run_server(host='0.0.0.0', port=8050, debug=True)
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dash_component_editor-0.0.4/README.md` & `dash_component_editor-0.0.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # MLExchange Dash component editor
 This script creates adaptive Dash GUI components from keyword pairs (JSON format).
 
 It currently supports 8 types of Dash GUI components: 3 types of [input forms](https://dash-bootstrap-components.opensource.faculty.ai/docs/components/input/) (int, float, str), [slider](https://dash.plotly.com/dash-core-components/slider), [dropdown](https://dash.plotly.com/dash-core-components/dropdown), [radio items](https://dash.plotly.com/dash-core-components/radioitems), [boolean toggle switch](https://dash.plotly.com/dash-daq/toggleswitch), and [image](https://dash.plotly.com/dash-html-components/img). The corresponding keyword values are 'int', 'float', 'str', 'slider', 'dropdown', 'radio', 'bool', and 'img'.
 
-Legal keyword pairs: {'type': xxx, 'name': xxx, 'title': xxx, 'param_key': xxx, 'value': xxx} and all the other legal keyword pairs in the corresponding Dash components. **Note**: 'name' is the unique string identifier.
+Legal keyword pairs: {'type': xxx, 'name': xxx, 'title': xxx, 'param_key': xxx, 'value': xxx} and all the other legal keyword pairs in the corresponding Dash components. **Note**: 'name' is the unique string identifier for each component.
 
 
 
 ## Dependencies:
 
 ```
 dash>=2.9.0
@@ -16,21 +16,26 @@
 werkzeug==2.0
 ```
 
 
 ## Code example
 
 ```python
-from dash import Dash, html
+from dash import Dash, html, Input, Output
 from dash_component_editor import JSONParameterEditor
 
 # data
 component_kwargs = {"gui_parameters": [{"type": "int", "name": "num-tree", "title": "Number of Trees", "param_key": "n_estimators", "value": "30"}, 
-                                       {"type": "int", "name": "tree-depth", "title": "Tree Depth", "param_key": "max_depth", "value": "8"}]}
-
+                                       {"type": "dropdown", "name": "dropdown-menu", "title": "Choose a City", "param_key": "city", 
+                                        "options": [{'label': 'New York City', 'value': 'New York City'}, {'label': 'Montreal', 'value': 'Montreal'},
+                                                   {'label': 'San Francisco', 'value': 'San Francisco'}], "value": "'Montreal"},
+                                       {"type": "slider", "name": "slider-id", "title": "Fahrenheit Range", "param_key": "f_temp", "min": 0, "max": 10,
+                                        "step": None, "marks": {0: '0°F', 3: '3°F', 5: '5°F', 7.65: '7.65°F', 10: '10°F'}, "value":5},
+                                       ]
+                    }
 
 # set up Dash server and web layouts
 app = Dash(__name__)
 app.layout = html.Div ([html.Button('Show GUI', id='button', n_clicks=0),
                         html.Div(id='gui-layout', children=[])
                        ])
 
@@ -44,10 +49,13 @@
 def show_gui_layouts(n_clicks):
     item_list = JSONParameterEditor(_id={'type': 'parameter_editor'},
                                     json_blob=component_kwargs["gui_parameters"],
                                 )
     item_list.init_callbacks(app)
     
     return [html.H5("GUI Layout", className="card-title"), item_list]
+
+
+app.run_server(host='0.0.0.0', port=8050, debug=True)
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dash_component_editor-0.0.4/setup.py` & `dash_component_editor-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dash_component_editor",                     # This is the name of the package
-    version="0.0.4",                        # The release version
+    version="0.0.5",                        # The release version
     author="Zhuowen (Kevin) Zhao, Ronald Pandolfi",                     # Full name of the author
     author_email='zwenzhao11@gmail.com',
     description="",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     license_files = ('LICENSE.txt',),                                     # Information to filter the project on PyPi website
```

### Comparing `dash_component_editor-0.0.4/src/dash_component_editor.py` & `dash_component_editor-0.0.5/src/dash_component_editor.py`

 * *Files identical despite different names*


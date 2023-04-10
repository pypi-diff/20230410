# Comparing `tmp/pyVig-0.0.8.tar.gz` & `tmp/pyVig-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyVig-0.0.8.tar", last modified: Mon Mar 27 10:32:26 2023, max compression
+gzip compressed data, was "pyVig-0.0.9.tar", last modified: Tue Mar 28 06:19:56 2023, max compression
```

## Comparing `pyVig-0.0.8.tar` & `pyVig-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 10:32:26.966345 pyVig-0.0.8/
--rw-rw-rw-   0        0        0     1091 2022-07-10 12:42:58.000000 pyVig-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      488 2023-03-27 10:32:26.965314 pyVig-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       30 2022-07-10 12:46:40.000000 pyVig-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-27 10:32:26.944267 pyVig-0.0.8/pyVig/
--rw-rw-rw-   0        0        0     1117 2023-03-27 10:31:01.000000 pyVig-0.0.8/pyVig/__init__.py
--rw-rw-rw-   0        0        0     2774 2023-03-27 10:31:01.000000 pyVig-0.0.8/pyVig/cablings.py
--rw-rw-rw-   0        0        0      477 2023-03-26 09:20:08.000000 pyVig-0.0.8/pyVig/common.py
--rw-rw-rw-   0        0        0     6209 2023-03-26 09:20:08.000000 pyVig-0.0.8/pyVig/database.py
--rw-rw-rw-   0        0        0     4032 2023-03-27 10:31:01.000000 pyVig-0.0.8/pyVig/devices.py
--rw-rw-rw-   0        0        0     5799 2023-03-26 09:20:08.000000 pyVig-0.0.8/pyVig/entities.py
--rw-rw-rw-   0        0        0     5092 2023-03-27 10:31:01.000000 pyVig-0.0.8/pyVig/general.py
--rw-rw-rw-   0        0        0    21030 2023-03-26 09:20:08.000000 pyVig-0.0.8/pyVig/gui.py
--rw-rw-rw-   0        0        0     5216 2023-03-27 10:31:01.000000 pyVig-0.0.8/pyVig/maths.py
--rw-rw-rw-   0        0        0     7696 2023-03-27 10:31:01.000000 pyVig-0.0.8/pyVig/oper.py
--rw-rw-rw-   0        0        0     6469 2023-03-27 10:31:01.000000 pyVig-0.0.8/pyVig/pyVig.py
--rw-rw-rw-   0        0        0     1728 2023-03-26 09:20:08.000000 pyVig-0.0.8/pyVig/static.py
--rw-rw-rw-   0        0        0     2014 2023-03-26 09:20:08.000000 pyVig-0.0.8/pyVig/stencils.py
--rw-rw-rw-   0        0        0    18196 2023-03-26 09:20:08.000000 pyVig-0.0.8/pyVig/visio.py
-drwxrwxrwx   0        0        0        0 2023-03-27 10:32:26.963318 pyVig-0.0.8/pyVig.egg-info/
--rw-rw-rw-   0        0        0      488 2023-03-27 10:32:26.000000 pyVig-0.0.8/pyVig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-03-27 10:32:26.000000 pyVig-0.0.8/pyVig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 10:32:26.000000 pyVig-0.0.8/pyVig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-03-27 10:32:26.000000 pyVig-0.0.8/pyVig.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-27 10:32:26.000000 pyVig-0.0.8/pyVig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-27 10:32:26.966345 pyVig-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1071 2023-03-27 10:31:01.000000 pyVig-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-28 06:19:56.526927 pyVig-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2022-07-10 12:42:58.000000 pyVig-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      488 2023-03-28 06:19:56.526010 pyVig-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2022-07-10 12:46:40.000000 pyVig-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-28 06:19:56.496711 pyVig-0.0.9/pyVig/
+-rw-rw-rw-   0        0        0     1128 2023-03-28 06:14:24.000000 pyVig-0.0.9/pyVig/__init__.py
+-rw-rw-rw-   0        0        0     2774 2023-03-27 10:31:01.000000 pyVig-0.0.9/pyVig/cablings.py
+-rw-rw-rw-   0        0        0      477 2023-03-26 09:20:08.000000 pyVig-0.0.9/pyVig/common.py
+-rw-rw-rw-   0        0        0     6209 2023-03-26 09:20:08.000000 pyVig-0.0.9/pyVig/database.py
+-rw-rw-rw-   0        0        0     4032 2023-03-27 10:31:01.000000 pyVig-0.0.9/pyVig/devices.py
+-rw-rw-rw-   0        0        0     5799 2023-03-26 09:20:08.000000 pyVig-0.0.9/pyVig/entities.py
+-rw-rw-rw-   0        0        0     5092 2023-03-27 10:31:01.000000 pyVig-0.0.9/pyVig/general.py
+-rw-rw-rw-   0        0        0    21073 2023-03-28 06:14:24.000000 pyVig-0.0.9/pyVig/gui.py
+-rw-rw-rw-   0        0        0     5216 2023-03-27 10:31:01.000000 pyVig-0.0.9/pyVig/maths.py
+-rw-rw-rw-   0        0        0     7696 2023-03-27 10:31:01.000000 pyVig-0.0.9/pyVig/oper.py
+-rw-rw-rw-   0        0        0     6958 2023-03-28 06:14:24.000000 pyVig-0.0.9/pyVig/pyVig.py
+-rw-rw-rw-   0        0        0     1728 2023-03-26 09:20:08.000000 pyVig-0.0.9/pyVig/static.py
+-rw-rw-rw-   0        0        0     2014 2023-03-26 09:20:08.000000 pyVig-0.0.9/pyVig/stencils.py
+-rw-rw-rw-   0        0        0    18196 2023-03-26 09:20:08.000000 pyVig-0.0.9/pyVig/visio.py
+drwxrwxrwx   0        0        0        0 2023-03-28 06:19:56.522910 pyVig-0.0.9/pyVig.egg-info/
+-rw-rw-rw-   0        0        0      488 2023-03-28 06:19:56.000000 pyVig-0.0.9/pyVig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-03-28 06:19:56.000000 pyVig-0.0.9/pyVig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-28 06:19:56.000000 pyVig-0.0.9/pyVig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-03-28 06:19:56.000000 pyVig-0.0.9/pyVig.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-03-28 06:19:56.000000 pyVig-0.0.9/pyVig.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-28 06:19:56.527892 pyVig-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1071 2023-03-28 06:14:24.000000 pyVig-0.0.9/setup.py
```

### Comparing `pyVig-0.0.8/LICENSE` & `pyVig-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyVig-0.0.8/pyVig/__init__.py` & `pyVig-0.0.9/pyVig/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 
 MS-Visio: to generate the drawing.
 
 Stencils: [optional] folder from where project can find visio stencils.
 
 """
 
-__ver__ = "0.0.8"
+__ver__ = "0.0.9"
 
 # ------------------------------------------------------------------------------
 
 from .stencils import get_list_of_stencils
 from .database import DeviceData, CableMatrixData
 from .gui import UserForm
 from .entities import ItemObjects, Connectors
 from .visio import VisioObject
 
 from .oper import DFGen
 from .devices import AdevDevices
 from .cablings import ADevCablings
 from .general import get_physical_if_up, get_physical_if_relevants
 from .general import get_patterns, update_pattern
-from .pyVig import pyVig
+from .pyVig import pyVig, pyVig_gui
 # ------------------------------------------------------------------------------
```

### Comparing `pyVig-0.0.8/pyVig/cablings.py` & `pyVig-0.0.9/pyVig/cablings.py`

 * *Files identical despite different names*

### Comparing `pyVig-0.0.8/pyVig/database.py` & `pyVig-0.0.9/pyVig/database.py`

 * *Files identical despite different names*

### Comparing `pyVig-0.0.8/pyVig/devices.py` & `pyVig-0.0.9/pyVig/devices.py`

 * *Files identical despite different names*

### Comparing `pyVig-0.0.8/pyVig/entities.py` & `pyVig-0.0.9/pyVig/entities.py`

 * *Files identical despite different names*

### Comparing `pyVig-0.0.8/pyVig/general.py` & `pyVig-0.0.9/pyVig/general.py`

 * *Files identical despite different names*

### Comparing `pyVig-0.0.8/pyVig/gui.py` & `pyVig-0.0.9/pyVig/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,24 +16,25 @@
 
  Macros and vBA scripting requires to be enabled in visio
  in order to access the visio components.
  select 'Enable all macros' and, check 'Trust access to vBA'
  from trust center setting of MS-visio.
 
 
- Please reachout to me, [Aliasgar Lokhandwala] for any Qs.
+ Please reachout to me, @ aholo2000@gmail.com for any Qs.
+ Owner of code: [Aliasgar Lokhandwala]
 """
 
 # -----------------------------------------------------------------------------
 # Class to initiate UserForm
 # -----------------------------------------------------------------------------
 
 class UserForm():
 	'''Inititates a UserForm asking user inputs.	'''
-	version  = 'Visio Generator : ver: 0.0.5'
+	version  = 'Visio Generator : gui ver: 0.0.8'
 	header = 'Visio Generator'
 
 	# Object Initializer
 	def __init__(self):
 		self.boot = False
 		self.dic = {
 			'stencil_folder':"",
```

### Comparing `pyVig-0.0.8/pyVig/maths.py` & `pyVig-0.0.9/pyVig/maths.py`

 * *Files identical despite different names*

### Comparing `pyVig-0.0.8/pyVig/oper.py` & `pyVig-0.0.9/pyVig/oper.py`

 * *Files identical despite different names*

### Comparing `pyVig-0.0.8/pyVig/pyVig.py` & `pyVig-0.0.9/pyVig/pyVig.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 from copy import deepcopy
 from .stencils import get_list_of_stencils
 from .database import DeviceData, CableMatrixData
 from .entities import ItemObjects, Connectors
 from .visio import VisioObject
+from .gui import UserForm
 
 
 # ------------------------------------------------------------------------- 
 # ## DICTIONARY - DEFAULT INPUTS 
 # ------------------------------------------------------------------------- 
 
 DEFAULT_DIC = {
@@ -157,15 +158,15 @@
 		v.insert_new_page("PhysicalDrawing")
 	item_objects = ItemObjects(v, devices_data, cable_matrix_data, filterOnCables=dic['filter_on_cable'])
 	Connectors(cable_matrix_data, item_objects)
 	v.fit_to_draw(item_objects.page_height, item_objects.page_width)
 
 
 def pyVig(dic):
-	"""main function starting the python based visio generation
+	"""main function starting the python based cli - visio generation
 
 	Args:
 		dic (dict): inputs dictionary ( valid and mandatory keys = stencil_folder, data_file ) (valid but optional keys = default_stencil, cols_to_merge, is_sheet_filter, sheet_filters ... and many more from DEFAULT_DIC )
 
 	Returns:
 		None: None
 	"""	
@@ -175,10 +176,29 @@
 	stencils = get_list_of_stencils(
 		folder=DEFAULT_DIC['stencil_folder'],
 		devices_data=devices_data,
 	)
 	visio_operations(DEFAULT_DIC, devices_data, cable_matrix_data, stencils)
 	return None
 
+def pyVig_gui():
+	"""main function starting the gui input - visio generation
+
+	Returns:
+		None: None
+	"""	
+	u = UserForm()
+	try: dic = u.dic
+	except: return None
+	devices_data = device_data_operations(dic)
+	cable_matrix_data = cabling_data_operations(dic)
+	stencils = get_list_of_stencils(
+		folder=dic['stencil_folder'], 
+		devices_data=devices_data, 
+	)
+	visio_operations(dic, devices_data, cable_matrix_data, stencils)
+	return None
+
+
 # -------------------------------------------------------------------------
```

### Comparing `pyVig-0.0.8/pyVig/static.py` & `pyVig-0.0.9/pyVig/static.py`

 * *Files identical despite different names*

### Comparing `pyVig-0.0.8/pyVig/stencils.py` & `pyVig-0.0.9/pyVig/stencils.py`

 * *Files identical despite different names*

### Comparing `pyVig-0.0.8/pyVig/visio.py` & `pyVig-0.0.9/pyVig/visio.py`

 * *Files identical despite different names*

### Comparing `pyVig-0.0.8/setup.py` & `pyVig-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'repoze.sphinx.autointerface',
     'sphinx-copybutton',
     'sphinxcontrib-autoprogram',
 ]
 
 setuptools.setup(
     name="pyVig",
-    version="0.0.8",
+    version="0.0.9",
     author="ALIASGAR - ALI",
     author_email="aholo2000@gmail.com",
     description="python based Visio Generator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alias1978/pyVig",
     packages=setuptools.find_packages(),
```


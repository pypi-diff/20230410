# Comparing `tmp/satdigitalinvoice-2.1.1.tar.gz` & `tmp/satdigitalinvoice-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-2.1.1.tar", last modified: Mon Apr 10 02:06:52 2023, max compression
+gzip compressed data, was "satdigitalinvoice-2.1.2.tar", last modified: Mon Apr 10 02:09:50 2023, max compression
```

## Comparing `satdigitalinvoice-2.1.1.tar` & `satdigitalinvoice-2.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:06:52.978835 satdigitalinvoice-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-10 02:06:52.978835 satdigitalinvoice-2.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:06:52.974835 satdigitalinvoice-2.1.1/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/satdigitalinvoice/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)    31264 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/satdigitalinvoice/facturacion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:06:52.974835 satdigitalinvoice-2.1.1/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16837 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/satdigitalinvoice/gui_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:06:52.974835 satdigitalinvoice-2.1.1/satdigitalinvoice/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/satdigitalinvoice/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/satdigitalinvoice/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:06:52.974835 satdigitalinvoice-2.1.1/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/satdigitalinvoice/markdown_styles/markdown6.css
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:06:52.978835 satdigitalinvoice-2.1.1/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/satdigitalinvoice/schemas/cliente.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/satdigitalinvoice/schemas/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:06:52.974835 satdigitalinvoice-2.1.1/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-10 02:06:52.000000 satdigitalinvoice-2.1.1/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-10 02:06:52.000000 satdigitalinvoice-2.1.1/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 02:06:52.000000 satdigitalinvoice-2.1.1/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 02:06:52.000000 satdigitalinvoice-2.1.1/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 02:06:52.000000 satdigitalinvoice-2.1.1/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 02:06:52.978835 satdigitalinvoice-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:06:52.978835 satdigitalinvoice-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/tests/test_localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-10 02:06:37.000000 satdigitalinvoice-2.1.1/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:09:50.784620 satdigitalinvoice-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-10 02:09:50.784620 satdigitalinvoice-2.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:09:50.780620 satdigitalinvoice-2.1.2/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31264 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:09:50.780620 satdigitalinvoice-2.1.2/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16837 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:09:50.780620 satdigitalinvoice-2.1.2/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/satdigitalinvoice/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:09:50.780620 satdigitalinvoice-2.1.2/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:09:50.784620 satdigitalinvoice-2.1.2/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/satdigitalinvoice/schemas/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:09:50.780620 satdigitalinvoice-2.1.2/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-10 02:09:50.000000 satdigitalinvoice-2.1.2/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-10 02:09:50.000000 satdigitalinvoice-2.1.2/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 02:09:50.000000 satdigitalinvoice-2.1.2/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 02:09:50.000000 satdigitalinvoice-2.1.2/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 02:09:50.000000 satdigitalinvoice-2.1.2/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 02:09:50.784620 satdigitalinvoice-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:09:50.784620 satdigitalinvoice-2.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/tests/test_localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-10 02:09:35.000000 satdigitalinvoice-2.1.2/tests/test_main.py
```

### Comparing `satdigitalinvoice-2.1.1/PKG-INFO` & `satdigitalinvoice-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 2.1.1
+Version: 2.1.2
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-2.1.1/satdigitalinvoice/__init__.py` & `satdigitalinvoice-2.1.2/satdigitalinvoice/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         try:
             from satdigitalinvoice.facturacion import FacturacionGUI
             config = self.read_config()
             app = FacturacionGUI(config)
         except Exception as ex:
             logging.exception(ex)
             self.window['console'].update(
-                str(ex)
+               f"Error al cargar la aplicación. {ex.__class__.__name__}: {ex}"
             )
             self.window.read()
             self.window.close()
             return
 
         self.window.close()
         app.run()
```

### Comparing `satdigitalinvoice-2.1.1/satdigitalinvoice/__version__.py` & `satdigitalinvoice-2.1.2/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.1/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-2.1.2/satdigitalinvoice/client_validation.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.1/satdigitalinvoice/environments.py` & `satdigitalinvoice-2.1.2/satdigitalinvoice/environments.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.1/satdigitalinvoice/facturacion.py` & `satdigitalinvoice-2.1.2/satdigitalinvoice/facturacion.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.1/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-2.1.2/satdigitalinvoice/file_data_managers.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.1/satdigitalinvoice/formatting_functions/common.py` & `satdigitalinvoice-2.1.2/satdigitalinvoice/formatting_functions/common.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.1/satdigitalinvoice/gui_functions.py` & `satdigitalinvoice-2.1.2/satdigitalinvoice/gui_functions.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.1/satdigitalinvoice/images/logo.png` & `satdigitalinvoice-2.1.2/satdigitalinvoice/images/logo.png`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.1/satdigitalinvoice/layout.py` & `satdigitalinvoice-2.1.2/satdigitalinvoice/layout.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.1/satdigitalinvoice/localdb.py` & `satdigitalinvoice-2.1.2/satdigitalinvoice/localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.1/satdigitalinvoice/log_tools.py` & `satdigitalinvoice-2.1.2/satdigitalinvoice/log_tools.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.1/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-2.1.2/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.1/satdigitalinvoice/mycfdi.py` & `satdigitalinvoice-2.1.2/satdigitalinvoice/mycfdi.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.1/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-2.1.2/satdigitalinvoice/schemas/factura.yaml`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.1/satdigitalinvoice/utils.py` & `satdigitalinvoice-2.1.2/satdigitalinvoice/utils.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.1/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-2.1.2/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 2.1.1
+Version: 2.1.2
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-2.1.1/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-2.1.2/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.1/setup.py` & `satdigitalinvoice-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.1/tests/test_crear_facturas.py` & `satdigitalinvoice-2.1.2/tests/test_crear_facturas.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.1/tests/test_localdb.py` & `satdigitalinvoice-2.1.2/tests/test_localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.1/tests/test_main.py` & `satdigitalinvoice-2.1.2/tests/test_main.py`

 * *Files identical despite different names*


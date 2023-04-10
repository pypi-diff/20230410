# Comparing `tmp/satdigitalinvoice-2.1.4.tar.gz` & `tmp/satdigitalinvoice-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-2.1.4.tar", last modified: Mon Apr 10 05:30:56 2023, max compression
+gzip compressed data, was "satdigitalinvoice-2.1.5.tar", last modified: Mon Apr 10 16:52:37 2023, max compression
```

## Comparing `satdigitalinvoice-2.1.4.tar` & `satdigitalinvoice-2.1.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:30:56.339442 satdigitalinvoice-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-10 05:30:56.339442 satdigitalinvoice-2.1.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:30:56.331441 satdigitalinvoice-2.1.4/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)    31100 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/facturacion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:30:56.335442 satdigitalinvoice-2.1.4/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16837 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/gui_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:30:56.335442 satdigitalinvoice-2.1.4/satdigitalinvoice/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:30:56.335442 satdigitalinvoice-2.1.4/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/markdown_styles/markdown6.css
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:30:56.339442 satdigitalinvoice-2.1.4/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/schemas/cliente.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/schemas/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:30:56.335442 satdigitalinvoice-2.1.4/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-10 05:30:56.000000 satdigitalinvoice-2.1.4/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-10 05:30:56.000000 satdigitalinvoice-2.1.4/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 05:30:56.000000 satdigitalinvoice-2.1.4/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 05:30:56.000000 satdigitalinvoice-2.1.4/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 05:30:56.000000 satdigitalinvoice-2.1.4/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 05:30:56.339442 satdigitalinvoice-2.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:30:56.339442 satdigitalinvoice-2.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/tests/test_localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:37.808879 satdigitalinvoice-2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-10 16:52:37.808879 satdigitalinvoice-2.1.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:37.804879 satdigitalinvoice-2.1.5/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31211 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:37.808879 satdigitalinvoice-2.1.5/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16837 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:37.808879 satdigitalinvoice-2.1.5/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:37.808879 satdigitalinvoice-2.1.5/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:37.808879 satdigitalinvoice-2.1.5/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/schemas/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:37.808879 satdigitalinvoice-2.1.5/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-10 16:52:37.000000 satdigitalinvoice-2.1.5/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-10 16:52:37.000000 satdigitalinvoice-2.1.5/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:52:37.000000 satdigitalinvoice-2.1.5/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 16:52:37.000000 satdigitalinvoice-2.1.5/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 16:52:37.000000 satdigitalinvoice-2.1.5/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 16:52:37.808879 satdigitalinvoice-2.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:37.808879 satdigitalinvoice-2.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/tests/test_localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/tests/test_main.py
```

### Comparing `satdigitalinvoice-2.1.4/PKG-INFO` & `satdigitalinvoice-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 2.1.4
+Version: 2.1.5
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-2.1.4/satdigitalinvoice/__init__.py` & `satdigitalinvoice-2.1.5/satdigitalinvoice/__init__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.4/satdigitalinvoice/__version__.py` & `satdigitalinvoice-2.1.5/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.4/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-2.1.5/satdigitalinvoice/client_validation.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.4/satdigitalinvoice/environments.py` & `satdigitalinvoice-2.1.5/satdigitalinvoice/environments.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.4/satdigitalinvoice/facturacion.py` & `satdigitalinvoice-2.1.5/satdigitalinvoice/facturacion.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from .file_data_managers import ClientsManager, FacturasManager
 from .gui_functions import generate_ingresos, pago_factura, exportar_facturas, facturas_filename, \
     periodo_desc, generate_html_template, mf_pago_fmt, print_invoices, print_cfdis, print_cfdi_details, ajustes, ajustes_directory
 from .layout import make_layout, ActionButtonManager
 from .localdb import LocalDBSatCFDI, LiquidatedState
 from .log_tools import log_line, log_item, cfdi_header, header_line, print_yaml
 from .mycfdi import get_all_cfdi, MyCFDI, move_to_folder
-from .utils import random_string, to_uuid, parse_date_period, parse_ym_date, load_certificate, to_int
+from .utils import random_string, to_uuid, parse_date_period, parse_ym_date, load_certificate, to_int, cert_info
 
 logging.getLogger("weasyprint").setLevel(logging.ERROR)
 logging.getLogger("fontTools").setLevel(logging.ERROR)
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
@@ -107,24 +107,26 @@
         h.setLevel(logging.INFO)
         logging.root.addHandler(h)
 
         self.main_loop()
         self.window.close()
 
     def initial_screen(self, emisor_cif):
-        log_line("Acerca De")
+        self.header("ACERCA DE")
         print_yaml({
             "version": __version__.__version__,
             "facturacion": "CFDI 4.0",
             "emisor": emisor_cif,
             "pac_service": {
                 "Type": type(self.pac_service).__name__,
                 "Rfc": self.pac_service.RFC,
                 "Environment": str(self.pac_service.environment)
-            }
+            },
+            "fiel": cert_info(self.fiel_signer),
+            "csd": cert_info(self.csd_signer),
         })
 
     def get_all_invoices(self):
         if self.all_invoices:
             return self.all_invoices
         self.all_invoices = get_all_cfdi()
         return self.all_invoices
```

### Comparing `satdigitalinvoice-2.1.4/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-2.1.5/satdigitalinvoice/file_data_managers.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.4/satdigitalinvoice/formatting_functions/common.py` & `satdigitalinvoice-2.1.5/satdigitalinvoice/formatting_functions/common.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.4/satdigitalinvoice/gui_functions.py` & `satdigitalinvoice-2.1.5/satdigitalinvoice/gui_functions.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.4/satdigitalinvoice/images/logo.png` & `satdigitalinvoice-2.1.5/satdigitalinvoice/images/logo.png`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.4/satdigitalinvoice/layout.py` & `satdigitalinvoice-2.1.5/satdigitalinvoice/layout.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.4/satdigitalinvoice/localdb.py` & `satdigitalinvoice-2.1.5/satdigitalinvoice/localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.4/satdigitalinvoice/log_tools.py` & `satdigitalinvoice-2.1.5/satdigitalinvoice/log_tools.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.4/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-2.1.5/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.4/satdigitalinvoice/mycfdi.py` & `satdigitalinvoice-2.1.5/satdigitalinvoice/mycfdi.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.4/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-2.1.5/satdigitalinvoice/schemas/factura.yaml`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.4/satdigitalinvoice/utils.py` & `satdigitalinvoice-2.1.5/satdigitalinvoice/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,24 +53,24 @@
     return datetime.strptime(ans1_date.decode('utf-8'), '%Y%m%d%H%M%SZ')
 
 
 def cert_info(signer: Signer):
     if signer:
         return {
             "NoCertificado": signer.certificate_number,
-            "Tipo": str(signer.type),
-
-            "organizationName": signer.certificate.get_subject().O,
-            "x500UniqueIdentifier": signer.certificate.get_subject().x500UniqueIdentifier,
-            "serialNumber": signer.certificate.get_subject().serialNumber,
-            "organizationUnitName": signer.certificate.get_subject().OU,
-            "emailAddress": signer.certificate.get_subject().emailAddress,
-
-            "notAfter": convert_ans1_date(signer.certificate.get_notAfter()),
-            "notBefore": convert_ans1_date(signer.certificate.get_notBefore()),
+            # "Tipo": str(signer.type),
+            #
+            # "organizationName": signer.certificate.get_subject().O,
+            # "x500UniqueIdentifier": signer.certificate.get_subject().x500UniqueIdentifier,
+            # "serialNumber": signer.certificate.get_subject().serialNumber,
+            # "organizationUnitName": signer.certificate.get_subject().OU,
+            # "emailAddress": signer.certificate.get_subject().emailAddress,
+            #
+            "Expira": convert_ans1_date(signer.certificate.get_notAfter()),
+            "Creado": convert_ans1_date(signer.certificate.get_notBefore()),
         }
 
 
 def find_best_match(cases, emission_date):
     fk, fv = (None, None)
     for k, v in cases.items():
         k = parse_ym_date(k)
```

### Comparing `satdigitalinvoice-2.1.4/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-2.1.5/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 2.1.4
+Version: 2.1.5
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-2.1.4/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-2.1.5/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.4/setup.py` & `satdigitalinvoice-2.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.4/tests/test_crear_facturas.py` & `satdigitalinvoice-2.1.5/tests/test_crear_facturas.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.4/tests/test_localdb.py` & `satdigitalinvoice-2.1.5/tests/test_localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.4/tests/test_main.py` & `satdigitalinvoice-2.1.5/tests/test_main.py`

 * *Files identical despite different names*


# Comparing `tmp/satdigitalinvoice-2.0.7.tar.gz` & `tmp/satdigitalinvoice-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-2.0.7.tar", last modified: Sat Apr  8 23:30:51 2023, max compression
+gzip compressed data, was "satdigitalinvoice-2.1.0.tar", last modified: Mon Apr 10 01:52:57 2023, max compression
```

## Comparing `satdigitalinvoice-2.0.7.tar` & `satdigitalinvoice-2.1.0.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:51.611625 satdigitalinvoice-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-08 23:30:51.611625 satdigitalinvoice-2.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:51.607625 satdigitalinvoice-2.0.7/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)    30661 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/facturacion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:51.607625 satdigitalinvoice-2.0.7/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/gui_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:51.607625 satdigitalinvoice-2.0.7/satdigitalinvoice/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:51.607625 satdigitalinvoice-2.0.7/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/markdown_styles/markdown6.css
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:51.607625 satdigitalinvoice-2.0.7/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/schemas/cliente.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/schemas/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:51.607625 satdigitalinvoice-2.0.7/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-08 23:30:51.000000 satdigitalinvoice-2.0.7/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-08 23:30:51.000000 satdigitalinvoice-2.0.7/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 23:30:51.000000 satdigitalinvoice-2.0.7/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-08 23:30:51.000000 satdigitalinvoice-2.0.7/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-08 23:30:51.000000 satdigitalinvoice-2.0.7/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 23:30:51.611625 satdigitalinvoice-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:30:51.611625 satdigitalinvoice-2.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/tests/test_localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-08 23:30:42.000000 satdigitalinvoice-2.0.7/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:52:57.011068 satdigitalinvoice-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-10 01:52:57.011068 satdigitalinvoice-2.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:52:57.003068 satdigitalinvoice-2.1.0/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31267 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:52:57.007068 satdigitalinvoice-2.1.0/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16837 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:52:57.007068 satdigitalinvoice-2.1.0/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/satdigitalinvoice/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:52:57.007068 satdigitalinvoice-2.1.0/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:52:57.007068 satdigitalinvoice-2.1.0/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/satdigitalinvoice/schemas/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:52:57.007068 satdigitalinvoice-2.1.0/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-10 01:52:56.000000 satdigitalinvoice-2.1.0/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-10 01:52:56.000000 satdigitalinvoice-2.1.0/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 01:52:56.000000 satdigitalinvoice-2.1.0/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 01:52:56.000000 satdigitalinvoice-2.1.0/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 01:52:56.000000 satdigitalinvoice-2.1.0/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 01:52:57.011068 satdigitalinvoice-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:52:57.011068 satdigitalinvoice-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/tests/test_localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-10 01:52:47.000000 satdigitalinvoice-2.1.0/tests/test_main.py
```

### Comparing `satdigitalinvoice-2.0.7/PKG-INFO` & `satdigitalinvoice-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 2.0.7
+Version: 2.1.0
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-2.0.7/satdigitalinvoice/__init__.py` & `satdigitalinvoice-2.1.0/satdigitalinvoice/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
 import os
 
 import PySimpleGUI as sg
 
 SOURCE_DIRECTORY = os.path.dirname(__file__)
 DATA_DIRECTORY = ".data"
+PPD = "PPD"
+PUE = "PUE"
 
 
 def add_file_handler():
     os.makedirs(DATA_DIRECTORY, exist_ok=True)
     fh = logging.FileHandler(
         os.path.join(DATA_DIRECTORY, 'errors.log'),
         mode='a',
@@ -52,14 +54,16 @@
             layout,
             size=(640, 480),
             resizable=True,
             font=("Courier New", 10, "bold"),
             no_titlebar=True,
             modal=True,
             background_color=sg.theme_background_color(),
+            auto_close=True,
+            auto_close_duration=6,  # seconds
         )
 
     @staticmethod
     def read_config():
         from satdigitalinvoice.file_data_managers import ConfigManager
         return ConfigManager()
```

### Comparing `satdigitalinvoice-2.0.7/satdigitalinvoice/__version__.py` & `satdigitalinvoice-2.1.0/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.7/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-2.1.0/satdigitalinvoice/client_validation.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.7/satdigitalinvoice/environments.py` & `satdigitalinvoice-2.1.0/satdigitalinvoice/environments.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.7/satdigitalinvoice/facturacion.py` & `satdigitalinvoice-2.1.0/satdigitalinvoice/facturacion.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 from satcfdi.pacs import Accept
 from satcfdi.pacs.sat import SAT, TipoDescargaMasivaTerceros, EstadoSolicitud
 from satcfdi.printer import Representable
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
 from tabulate import tabulate
 
-from . import __version__
+from . import __version__, PPD, PUE
 from .client_validation import validar_client
 from .file_data_managers import ClientsManager, FacturasManager
 from .gui_functions import generate_ingresos, pago_factura, exportar_facturas, facturas_filename, \
     periodo_desc, generate_html_template, mf_pago_fmt, print_invoices, print_cfdis, print_cfdi_details, ajustes, ajustes_directory
 from .layout import make_layout, ActionButtonManager
-from .localdb import LocalDBSatCFDI
+from .localdb import LocalDBSatCFDI, LiquidatedState
 from .log_tools import log_line, log_item, cfdi_header, header_line, print_yaml
-from .mycfdi import get_all_cfdi, MyCFDI, move_to_folder, PPD, PUE
+from .mycfdi import get_all_cfdi, MyCFDI, move_to_folder
 from .utils import random_string, to_uuid, parse_date_period, parse_ym_date, load_certificate, to_int
 
 logging.getLogger("weasyprint").setLevel(logging.ERROR)
 logging.getLogger("fontTools").setLevel(logging.ERROR)
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
@@ -64,15 +64,15 @@
         self.fiel_signer = load_certificate(config.get('fiel')) if 'fiel' in config else None
 
         self.sat_service = SAT(signer=self.fiel_signer)
         self.rfc_prediales = config['rfc_prediales']
 
         self.window = PySimpleGUI.Window(
             f"Facturación Masiva CFDI 4.0 {self.csd_signer.rfc}",
-            make_layout(True),
+            make_layout(bool(self.fiel_signer)),
             size=(1280, 800),
             resizable=True,
             font=("Courier New", 10, "bold"),
         )
 
         self.all_invoices = None
         self.local_db = LocalDBSatCFDI(
@@ -178,15 +178,15 @@
                             'pendientes_meses_anteriores': pendientes_meses_anteriores,
                             'emisor': emisor_cif,
                         },
                     ),
                     file_attachments=attachments
                 )
                 for r in notify_invoices:
-                    self.local_db.notificar_set(r.uuid, False)
+                    self.local_db.notified_set(r.uuid, True)
                 print_yaml({
                     "correo": subject,
                     "para": receptor["Email"]
                 })
                 self._read()
 
     def recupera_comprobantes(self, id_solicitud):
@@ -256,74 +256,76 @@
         # Email
         is_enviable = i \
                       and i["Emisor"]["Rfc"] == self.csd_signer.rfc \
                       and i["Fecha"] >= self.local_db.enviar_a_partir \
                       and i.estatus == "1"
         if is_enviable:
             self.window["email_notificada"].update(
-                "Por Enviar" if self.local_db.notificar(i) else " Enviada  ",
+                " Enviada  " if self.local_db.notified(i) else "Por Enviar",
                 visible=True,
-                button_color="red4" if self.local_db.notificar(i) else "green",
+                button_color="green" if self.local_db.notified(i) else "red4",
             )
         else:
             self.window["email_notificada"].update("", visible=False)
 
         # Pendiente de Pago
         is_pendientable = i \
                           and i["Emisor"]["Rfc"] == self.csd_signer.rfc \
                           and i["TipoDeComprobante"] == "I" \
                           and i["Fecha"] >= self.local_db.saldar_a_partir[i['MetodoPago']] \
                           and i.estatus == "1" \
                           and (i["MetodoPago"] == PUE or i.saldo_pendiente) \
                           and i["Total"]
         if is_pendientable:
             self.window["pendiente_pago"].update(
-                "Por Saldar" if self.local_db.saldar(i) else " Saldada  ",
+                (" Pagada  " if i["MetodoPago"] == PUE else "Ignorada ") if self.local_db.liquidated(i) else "Por Pagar",
                 visible=True,
-                button_color="red4" if self.local_db.saldar(i) else "green",
+                button_color="green" if self.local_db.liquidated(i) else "red4",
             )
         else:
             self.window["pendiente_pago"].update("", visible=False)
 
         # PPD
         is_ppd_active = i \
+                        and i["Emisor"]["Rfc"] == self.csd_signer.rfc \
                         and i.get("MetodoPago") == PPD \
                         and i.estatus == "1" \
-                        and i["Emisor"]["Rfc"] == self.csd_signer.rfc
+                        and i.saldo_pendiente
         self.window["prepare_pago"].update(disabled=not is_ppd_active)
         self.window["fecha_pago_select"].update(disabled=not is_ppd_active)
         self.window["fecha_pago"].update(disabled=not is_ppd_active)
         self.window["importe_pago"].update(disabled=not is_ppd_active)
         self.window["forma_pago"].update(disabled=not is_ppd_active)
 
     def print_satcfdis(self, cfdis):
         def info_fmt(i):
-            return "🗙" if i.estatus == '0' else ("📧" if self.local_db.notificar(i) else "")
+            return "" if self.local_db.notified(i) else "📧"
 
         if cfdis := sorted(cfdis, key=lambda i: (i["Fecha"], i.name), reverse=True):
             if self.window['detallado'].get():
-                for i in cfdis:
-                    print_yaml(i)
-                    self.local_db.describe(i)
+                for i, cfdi in enumerate(cfdis, start=1):
+                    log_item(f"FACTURA NUMERO: {i}")
+                    print_yaml(cfdi)
+                    self.local_db.describe(cfdi)
             else:
                 print_invoices(
                     [
                         [
-                            e,
-                            i['Receptor'].get('Nombre', '')[0:36],
-                            i['Receptor']['Rfc'],
-                            i.name,
-                            i["Fecha"].strftime("%Y-%m-%d"),
-                            i["Total"],
-                            self.local_db.saldar(i),
-                            mf_pago_fmt(i),
-                            i.uuid,
-                            info_fmt(i)
+                            i,
+                            cfdi['Receptor'].get('Nombre', '')[0:36],
+                            cfdi['Receptor']['Rfc'],
+                            cfdi.name,
+                            cfdi["Fecha"].strftime("%Y-%m-%d"),
+                            cfdi["Total"],
+                            self.local_db.liquidated_state(cfdi),
+                            mf_pago_fmt(cfdi),
+                            cfdi.uuid,
+                            info_fmt(cfdi)
                         ]
-                        for e, i in enumerate(cfdis, start=1)
+                        for i, cfdi in enumerate(cfdis, start=1)
                     ]
                 )
             if len(cfdis) == 1:
                 print_cfdi_details(cfdis[0])
                 self.set_selected_satcfdi(cfdis[0])
             else:
                 self.set_selected_satcfdi(None)
@@ -353,14 +355,18 @@
             event, values = self.window.read()
             try:
                 if event in ("Exit", PySimpleGUI.WIN_CLOSED):
                     return
 
                 action_name, action_items = self.action_button_manager.clear()
 
+                if event in ("prepare_correos", "prepare_clientes", "prepare_facturas", "crear_facturas",
+                             "inicio_enter", "final_enter", "preparar_ajuste_anual", "recuperar_emitidas", "recuperar_recibidas"):
+                    self.set_selected_satcfdi([])
+
                 match event:
                     case "folio":
                         self.set_folio(to_int(values["folio"]))
 
                     case "about":
                         clients = ClientsManager()
                         self.initial_screen(clients[self.csd_signer.rfc])
@@ -498,59 +504,60 @@
                     case "ver_factura":
                         if i := self.selected_satcfdi:
                             os.startfile(
                                 os.path.abspath(i.filename + ".pdf")
                             )
 
                     case "status_sat":
-                        self.header("STATUS")
+                        self.header("STATUS SAT")
                         if i := self.selected_satcfdi:
                             estado = self.local_db.status_sat(i, update=True)
                             self.print_satcfdis([i])
                             print_yaml(estado)
 
                     case "pendiente_pago":
                         if i := self.selected_satcfdi:
-                            st = self.local_db.saldar_flip(i)
+                            st = self.local_db.liquidated_flip(i)
                             self.console.update("")
                             self.header(self.window[event].ButtonText.upper())
                             self.print_satcfdis([i])
-                            print(f"FACTURA MARCADA COMO {'-NO- ' if st else ''}SALDADA")
+                            if i["MetodoPago"] == PUE:
+                                print(f"FACTURA MARCADA COMO {'' if st else '-NO- '}PAGADA")
+                            else:
+                                print(f"FACTURA MARCADA COMO {'' if st else '-NO- '}IGNORADA")
 
                     case "email_notificada":
                         if i := self.selected_satcfdi:
-                            st = self.local_db.notificar_flip(i)
+                            st = self.local_db.notified_flip(i)
                             self.console.update("")
                             self.header(self.window[event].ButtonText.upper())
                             self.print_satcfdis([i])
-                            print(f"FACTURA MARCADA COMO {'-NO- ' if st else ''}NOTIFICADA")
+                            print(f"FACTURA MARCADA COMO {'' if st else '-NO- '}NOTIFICADA")
 
                     case "prepare_correos":
                         self.header("CORREOS")
                         now = date.today()
                         dp = DatePeriod(now.year, now.month)
                         clients = ClientsManager()
                         a_invoices = self.get_all_invoices()
 
                         cfdi_correos = []
                         for receptor_rfc, notify_invoices in itertools.groupby(
                                 sorted(
-                                    (i for i in a_invoices.values() if i.estatus == "1" and self.local_db.notificar(i)),
+                                    (i for i in a_invoices.values() if i.estatus == "1" and not self.local_db.notified(i)),
                                     key=lambda r: r["Receptor"]["Rfc"]
                                 ),
                                 lambda r: r["Receptor"]["Rfc"]
                         ):
                             notify_invoices = list(notify_invoices)
 
                             def fac_iter():
                                 for i in self.get_all_invoices().values():
                                     if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
-                                            and i["TipoDeComprobante"] == "I" \
-                                            and i.estatus == '1' \
-                                            and self.local_db.saldar(i) \
+                                            and self.local_db.liquidated_state(i) == LiquidatedState.NO \
                                             and i["Fecha"] < dp \
                                             and i["Receptor"]["Rfc"] == receptor_rfc:
                                         yield i
 
                             fac_pen = sorted(
                                 fac_iter(),
                                 key=lambda r: r["Fecha"]
@@ -581,35 +588,35 @@
                             ))
 
                             self.action_button_manager.set_items(ACTION_EMAILS, cfdi_correos)
                         else:
                             print("No hay correos pendientes de enviar")
 
                     case "crear_facturas":
+                        self.console.update(autoscroll=True)
                         self.header(f"PROCESAR {action_name.upper()}", clear=False)
                         res = PySimpleGUI.popup(
                             f"Estas seguro que quieres crear {len(action_items)} {action_name}?",
                             title=self.window[event].ButtonText,
                             button_type=POPUP_BUTTONS_OK_CANCEL,
                         )
                         if res == "OK":
                             self.action_button(action_name, action_items)
                             print("FIN")
                         else:
                             print("OPERACION CANCELADA")
+                        self.console.update(autoscroll=False)
 
                     case "facturas_pendientes":
                         self.header("FACTURAS PENDIENTES")
 
                         def fac_iter():
                             for i in self.get_all_invoices().values():
                                 if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
-                                        and i["TipoDeComprobante"] == "I" \
-                                        and i.estatus == '1' \
-                                        and self.local_db.saldar(i):
+                                        and self.local_db.liquidated_state(i) == LiquidatedState.NO:
                                     yield i
 
                         self.print_satcfdis(fac_iter())
 
                     case "descarga":
                         self.header('DESCARGADA')
                         try:
```

### Comparing `satdigitalinvoice-2.0.7/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-2.1.0/satdigitalinvoice/file_data_managers.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.7/satdigitalinvoice/formatting_functions/common.py` & `satdigitalinvoice-2.1.0/satdigitalinvoice/formatting_functions/common.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.7/satdigitalinvoice/gui_functions.py` & `satdigitalinvoice-2.1.0/satdigitalinvoice/gui_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 from datetime import datetime, date
 from decimal import Decimal
 
 import xlsxwriter
 from babel.dates import format_date
 from markdown2 import markdown
 from satcfdi import DatePeriod
-from satcfdi.accounting import filter_invoices_iter, filter_payments_iter, invoices_export, payments_export
+from satcfdi.accounting import filter_invoices_iter, filter_payments_iter, invoices_export, payments_export, SatCFDI
 from satcfdi.create.cfd import cfdi40
 from satcfdi.create.cfd.cfdi40 import Comprobante, PagoComprobante
 from satcfdi.pacs import sat
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
 from tabulate import tabulate
 from weasyprint import HTML, CSS
 from xlsxwriter.exceptions import FileCreateError
 
-from . import SOURCE_DIRECTORY
+from . import SOURCE_DIRECTORY, PPD
 from .environments import facturacion_environment
 from .file_data_managers import ClientsManager, FacturasManager
 from .formatting_functions.common import fecha, pesos, porcentaje
 from .log_tools import print_yaml
 from .utils import clear_directory, find_best_match, months_between, add_month
 
 logger = logging.getLogger(__name__)
@@ -328,15 +328,15 @@
             headers=(
                 '',
                 'Receptor Razon Social',
                 'Recep. Rfc',
                 'Factura',
                 "Fecha",
                 "Total",
-                "Saldar",
+                "Pagada",
                 "Tipo",
                 "Folio Fiscal",
                 "🛈"
             ),
             disable_numparse=True,
             colalign=("right", "left", "left", "left", "left", "right", "right", "left", "left", "left")
         )
@@ -392,17 +392,24 @@
                     "ImpSaldoAnt": d.get("ImpSaldoAnt"),
                     "ImpPagado": d.get("ImpPagado"),
                     "ImpSaldoInsoluto": d.get("ImpSaldoInsoluto"),
                 } for d in p["DoctoRelacionado"]]
             } for p in pagos]
         })
     else:
-        print_yaml({
-            "Conceptos": [x['Descripcion'] for x in i["Conceptos"]]
-        })
+        if isinstance(cfdi, SatCFDI) and cfdi.get("MetodoPago") == PPD:
+            print_yaml({
+                "Conceptos": [x['Descripcion'] for x in i["Conceptos"]],
+                "Pendiente": cfdi.saldo_pendiente,
+                "Pagos": [f"{c.comprobante.name} - {c.comprobante.uuid}" for c in cfdi.payments if c.comprobante.estatus != '0']
+            })
+        else:
+            print_yaml({
+                "Conceptos": [x['Descripcion'] for x in i["Conceptos"]]
+            })
 
 
 def ajustes_directory(ym_date):
     return os.path.join(facturas_folder(DatePeriod(year=ym_date.year, month=ym_date.month)), 'ajustes')
 
 
 def ajustes(emisor_rfc, ym_date):
@@ -424,15 +431,15 @@
                 vud, vu = find_best_match(valor_unitario_raw, ym_date)
                 vund, vun = find_best_match(valor_unitario_raw, ym_date_effective)
                 meses = months_between(vund, vud)
                 ajuste_porcentaje = (vun / vu - 1)
             else:
                 vu = valor_unitario_raw
                 vun = None
-                meses = 12
+                meses = None
                 ajuste_porcentaje = None
 
             concepto = format_concepto_desc(concepto, periodo="INMUEBLE")
             file_name = os.path.join(ajustes_dir, f'AjusteRenta_{rfc}_{i}.pdf')
 
             data = {
                 "receptor": receptor,
```

### Comparing `satdigitalinvoice-2.0.7/satdigitalinvoice/images/logo.png` & `satdigitalinvoice-2.1.0/satdigitalinvoice/images/logo.png`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.7/satdigitalinvoice/layout.py` & `satdigitalinvoice-2.1.0/satdigitalinvoice/layout.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.7/satdigitalinvoice/localdb.py` & `satdigitalinvoice-2.1.0/satdigitalinvoice/localdb.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import logging
 import os
 import pickle
+from enum import Enum
 from uuid import UUID
 
 import diskcache
 from satcfdi.accounting import SatCFDI
 from satcfdi.pacs import sat
 
 from . import DATA_DIRECTORY
 from .log_tools import print_yaml
+from . import PPD
 
-EMAIL_NOTIFICADA = 2
+LIQUIDATED = 0
+NOTIFIED = 2
 STATUS_SAT = 3
-PENDIENTE = 4
 FOLIO = 5
 
 sat_manager = sat.SAT()
 
 logger = logging.getLogger(__name__)
 
 
@@ -26,41 +28,41 @@
 
     def folio(self):
         return self.get(FOLIO, 1)
 
     def folio_set(self, value: int):
         self[FOLIO] = value
 
-    def saldar(self, uuid: UUID):
+    def liquidated(self, uuid: UUID):
         return self.get(
-            (PENDIENTE, uuid), True
+            (LIQUIDATED, uuid), False
         )
 
-    def saldar_set(self, uuid: UUID, value: bool):
+    def liquidated_set(self, uuid: UUID, value: bool):
         if value:
+            self[(LIQUIDATED, uuid)] = value
+        else:
             try:
-                del self[(PENDIENTE, uuid)]
+                del self[(LIQUIDATED, uuid)]
             except KeyError:
                 pass
-        else:
-            self[(PENDIENTE, uuid)] = value
 
-    def notificar(self, uuid: UUID):
+    def notified(self, uuid: UUID):
         return self.get(
-            (EMAIL_NOTIFICADA, uuid), True
+            (NOTIFIED, uuid), False
         )
 
-    def notificar_set(self, uuid: UUID, value: bool):
+    def notified_set(self, uuid: UUID, value: bool):
         if value:
+            self[(NOTIFIED, uuid)] = value
+        else:
             try:
-                del self[(EMAIL_NOTIFICADA, uuid)]
+                del self[(NOTIFIED, uuid)]
             except KeyError:
                 pass
-        else:
-            self[(EMAIL_NOTIFICADA, uuid)] = value
 
     def status_sat(self, uuid: UUID):
         return self.get(
             (STATUS_SAT, uuid), {}
         )
 
     def status_sat_set(self, uuid: UUID, value: dict):
@@ -69,61 +71,91 @@
         else:
             try:
                 del self[(STATUS_SAT, uuid)]
             except KeyError:
                 pass
 
 
+class LiquidatedState(Enum):
+    NONE = 1
+    YES = 2
+    NO = 3
+    IGNORED = 4
+    CANCELLED = 5
+
+    def __str__(self):
+        if self.name == "NONE":
+            return ""
+        if self.name == "IGNORED":
+            return "Ignorada"
+        if self.name == "YES":
+            return "Si"
+        if self.name == "NO":
+            return "No"
+        if self.name == "CANCELLED":
+            return "Cancelada"
+
+
 class LocalDBSatCFDI(LocalDB):
     def __init__(self, enviar_a_partir, saldar_a_partir):
         super().__init__()
         self.enviar_a_partir = enviar_a_partir
         self.saldar_a_partir = saldar_a_partir
 
-    def notificar(self, cfdi: SatCFDI):
+    def notified(self, cfdi: SatCFDI):
         if cfdi["Fecha"] >= self.enviar_a_partir:
-            return super().notificar(cfdi.uuid)
-        return False
+            return super().notified(cfdi.uuid)
+        return True
 
-    def notificar_flip(self, cfdi: SatCFDI):
-        v = not self.notificar(cfdi)
-        self.notificar_set(cfdi.uuid, v)
+    def notified_flip(self, cfdi: SatCFDI):
+        v = not self.notified(cfdi)
+        self.notified_set(cfdi.uuid, v)
         return v
 
-    def saldar(self, cfdi: SatCFDI):
-        if cfdi["TipoDeComprobante"] != "I":
-            return None
-        if cfdi["MetodoPago"] == "PPD" and cfdi.saldo_pendiente == 0:
-            return 0
+    def liquidated(self, cfdi: SatCFDI):
         if cfdi["Fecha"] >= self.saldar_a_partir[cfdi["MetodoPago"]]:
-            if super().saldar(cfdi.uuid):
-                if cfdi["MetodoPago"] == "PPD":
-                    return cfdi.saldo_pendiente
-                else:
-                    return cfdi["Total"]
-        return 0
-
-    def saldar_flip(self, cfdi: SatCFDI):
-        v = not self.saldar(cfdi)
-        self.saldar_set(cfdi.uuid, v)
+            return super().liquidated(cfdi.uuid)
+        return True
+
+    def liquidated_flip(self, cfdi: SatCFDI):
+        v = not self.liquidated(cfdi)
+        self.liquidated_set(cfdi.uuid, v)
         return v
 
     def status_sat(self, cfdi: SatCFDI, update=False):
         if update:
             res = sat_manager.status(cfdi)
             if res["ValidacionEFOS"] == "200":
                 self.status_sat_set(cfdi.uuid, res)
             return res
         else:
             return super().status_sat(cfdi.uuid)
 
+    def liquidated_state(self, cfdi: SatCFDI):
+        if cfdi.estatus == '0':
+            return LiquidatedState.CANCELLED
+
+        if cfdi["TipoDeComprobante"] != "I":
+            return LiquidatedState.NONE
+
+        mpago = cfdi["MetodoPago"]
+        if mpago == PPD and cfdi.saldo_pendiente == 0:
+            return LiquidatedState.YES
+
+        if self.liquidated(cfdi):
+            if mpago == PPD:
+                return LiquidatedState.IGNORED
+            return LiquidatedState.YES
+
+        return LiquidatedState.NO
+
     def describe(self, cfdi: SatCFDI):
         print_yaml({
-            'saldar': self.saldar(cfdi),
-            'enviar': self.notificar(cfdi),
+            'saldada': self.liquidated(cfdi),
+            'enviada': self.notified(cfdi),
             'status_sat': self.status_sat(cfdi)
         })
 
 
 def save_data(file, data):
     with open(os.path.join(DATA_DIRECTORY, file), 'wb') as f:
         pickle.dump(data, f)
```

### Comparing `satdigitalinvoice-2.0.7/satdigitalinvoice/log_tools.py` & `satdigitalinvoice-2.1.0/satdigitalinvoice/log_tools.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.7/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-2.1.0/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.7/satdigitalinvoice/mycfdi.py` & `satdigitalinvoice-2.1.0/satdigitalinvoice/mycfdi.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,18 @@
 from .localdb import load_data, save_data
 from .utils import to_uuid
 
 ALL_INVOICES = 'all_invoices'
 ALL_RETENCIONES = 'all_retenciones'
 logger = logging.getLogger(__name__)
 
-PPD = "PPD"
-PUE = "PUE"
-
 
 class MyCFDI(SatCFDI):
     local_db = None
 
-    def consulta_estado(self):
-        return self.local_db.status_sat(self)
-
     @SatCFDI.estatus.getter
     def estatus(self) -> str:
         Estatus = {
             "Cancelado": "0",
             "Vigente": "1"
         }
         estado = self.local_db.status_sat(self).get('Estado')
```

### Comparing `satdigitalinvoice-2.0.7/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-2.1.0/satdigitalinvoice/schemas/factura.yaml`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.7/satdigitalinvoice/utils.py` & `satdigitalinvoice-2.1.0/satdigitalinvoice/utils.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.7/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-2.1.0/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 2.0.7
+Version: 2.1.0
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-2.0.7/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-2.1.0/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 setup.py
 satdigitalinvoice/__init__.py
-satdigitalinvoice/__main__.py
 satdigitalinvoice/__version__.py
 satdigitalinvoice/client_validation.py
 satdigitalinvoice/environments.py
 satdigitalinvoice/facturacion.py
 satdigitalinvoice/file_data_managers.py
 satdigitalinvoice/gui_functions.py
 satdigitalinvoice/layout.py
```

### Comparing `satdigitalinvoice-2.0.7/setup.py` & `satdigitalinvoice-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         package: [
             "markdown_styles/*",
             "schemas/*",
             'images/*',
         ],
     },
     install_requires=[
-        'satcfdi==4.0.5',
+        'satcfdi==4.0.6',
         'diskcache',
         'num2words',
         'PyYAML',
         'babel',
         'markdown2',
         'PySimpleGUI',
         'XlsxWriter',
```

### Comparing `satdigitalinvoice-2.0.7/tests/test_crear_facturas.py` & `satdigitalinvoice-2.1.0/tests/test_crear_facturas.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.7/tests/test_localdb.py` & `satdigitalinvoice-2.1.0/tests/test_localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.0.7/tests/test_main.py` & `satdigitalinvoice-2.1.0/tests/test_main.py`

 * *Files identical despite different names*


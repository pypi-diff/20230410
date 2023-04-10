# Comparing `tmp/satdigitalinvoice-2.1.3.tar.gz` & `tmp/satdigitalinvoice-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-2.1.3.tar", last modified: Mon Apr 10 02:15:25 2023, max compression
+gzip compressed data, was "satdigitalinvoice-2.1.4.tar", last modified: Mon Apr 10 05:30:56 2023, max compression
```

## Comparing `satdigitalinvoice-2.1.3.tar` & `satdigitalinvoice-2.1.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:15:25.353770 satdigitalinvoice-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-10 02:15:25.353770 satdigitalinvoice-2.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:15:25.353770 satdigitalinvoice-2.1.3/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/satdigitalinvoice/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)    31264 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/satdigitalinvoice/facturacion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:15:25.353770 satdigitalinvoice-2.1.3/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16837 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/satdigitalinvoice/gui_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:15:25.353770 satdigitalinvoice-2.1.3/satdigitalinvoice/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/satdigitalinvoice/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/satdigitalinvoice/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:15:25.353770 satdigitalinvoice-2.1.3/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/satdigitalinvoice/markdown_styles/markdown6.css
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:15:25.353770 satdigitalinvoice-2.1.3/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/satdigitalinvoice/schemas/cliente.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/satdigitalinvoice/schemas/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:15:25.353770 satdigitalinvoice-2.1.3/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-10 02:15:25.000000 satdigitalinvoice-2.1.3/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-10 02:15:25.000000 satdigitalinvoice-2.1.3/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 02:15:25.000000 satdigitalinvoice-2.1.3/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 02:15:25.000000 satdigitalinvoice-2.1.3/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 02:15:25.000000 satdigitalinvoice-2.1.3/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 02:15:25.353770 satdigitalinvoice-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:15:25.353770 satdigitalinvoice-2.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/tests/test_localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-10 02:15:15.000000 satdigitalinvoice-2.1.3/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:30:56.339442 satdigitalinvoice-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-10 05:30:56.339442 satdigitalinvoice-2.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:30:56.331441 satdigitalinvoice-2.1.4/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31100 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:30:56.335442 satdigitalinvoice-2.1.4/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16837 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:30:56.335442 satdigitalinvoice-2.1.4/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:30:56.335442 satdigitalinvoice-2.1.4/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:30:56.339442 satdigitalinvoice-2.1.4/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/schemas/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:30:56.335442 satdigitalinvoice-2.1.4/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-10 05:30:56.000000 satdigitalinvoice-2.1.4/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-10 05:30:56.000000 satdigitalinvoice-2.1.4/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 05:30:56.000000 satdigitalinvoice-2.1.4/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 05:30:56.000000 satdigitalinvoice-2.1.4/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 05:30:56.000000 satdigitalinvoice-2.1.4/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 05:30:56.339442 satdigitalinvoice-2.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:30:56.339442 satdigitalinvoice-2.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/tests/test_localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-10 05:30:45.000000 satdigitalinvoice-2.1.4/tests/test_main.py
```

### Comparing `satdigitalinvoice-2.1.3/PKG-INFO` & `satdigitalinvoice-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 2.1.3
+Version: 2.1.4
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-2.1.3/satdigitalinvoice/__init__.py` & `satdigitalinvoice-2.1.4/satdigitalinvoice/__init__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.3/satdigitalinvoice/__version__.py` & `satdigitalinvoice-2.1.4/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.3/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-2.1.4/satdigitalinvoice/client_validation.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.3/satdigitalinvoice/environments.py` & `satdigitalinvoice-2.1.4/satdigitalinvoice/environments.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.3/satdigitalinvoice/facturacion.py` & `satdigitalinvoice-2.1.4/satdigitalinvoice/facturacion.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,30 +252,28 @@
             self.window["status_sat"].update(
                 visible=False
             )
 
         # Email
         is_enviable = i \
                       and i["Emisor"]["Rfc"] == self.csd_signer.rfc \
-                      and i["Fecha"] >= self.local_db.enviar_a_partir \
                       and i.estatus == "1"
         if is_enviable:
             self.window["email_notificada"].update(
                 " Enviada  " if self.local_db.notified(i) else "Por Enviar",
                 visible=True,
                 button_color="green" if self.local_db.notified(i) else "red4",
             )
         else:
             self.window["email_notificada"].update("", visible=False)
 
         # Pendiente de Pago
         is_pendientable = i \
                           and i["Emisor"]["Rfc"] == self.csd_signer.rfc \
                           and i["TipoDeComprobante"] == "I" \
-                          and i["Fecha"] >= self.local_db.pagar_a_partir[i['MetodoPago']] \
                           and i.estatus == "1" \
                           and (i["MetodoPago"] == PUE or i.saldo_pendiente) \
                           and i["Total"]
         if is_pendientable:
             self.window["pendiente_pago"].update(
                 (" Pagada  " if i["MetodoPago"] == PUE else "Ignorada ") if self.local_db.liquidated(i) else "Por Pagar",
                 visible=True,
@@ -425,15 +423,15 @@
                             self._read()
                             for paquete_id, data in self.recupera_comprobantes(id_solicitud):
                                 if data:
                                     self.all_invoices = None
                                     with io.BytesIO(data) as b:
                                         self.unzip_cfdi(b)
                                 del self.local_db[event]
-                            log_line("FIN")
+                            print("FIN")
 
                     case "prepare_clientes":
                         self.header("CLIENTES")
                         clients = ClientsManager()
                         ym_date = parse_ym_date(values['periodo'])
                         if clients:
                             facturas = FacturasManager(ym_date)["Facturas"]
@@ -591,15 +589,15 @@
                         else:
                             print("No hay correos pendientes de enviar")
 
                     case "crear_facturas":
                         self.console.update(autoscroll=True)
                         self.header(f"PROCESAR {action_name.upper()}", clear=False)
                         res = PySimpleGUI.popup(
-                            f"Estas seguro que quieres crear {len(action_items)} {action_name}?",
+                            f"Estas seguro que quieres procesar {len(action_items)} {action_name}?",
                             title=self.window[event].ButtonText,
                             button_type=POPUP_BUTTONS_OK_CANCEL,
                         )
                         if res == "OK":
                             self.action_button(action_name, action_items)
                             print("FIN")
                         else:
```

### Comparing `satdigitalinvoice-2.1.3/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-2.1.4/satdigitalinvoice/file_data_managers.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.3/satdigitalinvoice/formatting_functions/common.py` & `satdigitalinvoice-2.1.4/satdigitalinvoice/formatting_functions/common.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.3/satdigitalinvoice/gui_functions.py` & `satdigitalinvoice-2.1.4/satdigitalinvoice/gui_functions.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.3/satdigitalinvoice/images/logo.png` & `satdigitalinvoice-2.1.4/satdigitalinvoice/images/logo.png`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.3/satdigitalinvoice/layout.py` & `satdigitalinvoice-2.1.4/satdigitalinvoice/layout.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.3/satdigitalinvoice/localdb.py` & `satdigitalinvoice-2.1.4/satdigitalinvoice/localdb.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,45 +29,27 @@
     def folio(self):
         return self.get(FOLIO, 1)
 
     def folio_set(self, value: int):
         self[FOLIO] = value
 
     def liquidated(self, uuid: UUID):
-        return self.get(
-            (LIQUIDATED, uuid), False
-        )
+        return self.get((LIQUIDATED, uuid))
 
     def liquidated_set(self, uuid: UUID, value: bool):
-        if value:
-            self[(LIQUIDATED, uuid)] = value
-        else:
-            try:
-                del self[(LIQUIDATED, uuid)]
-            except KeyError:
-                pass
+        self[(LIQUIDATED, uuid)] = value
 
     def notified(self, uuid: UUID):
-        return self.get(
-            (NOTIFIED, uuid), False
-        )
+        return self.get((NOTIFIED, uuid))
 
     def notified_set(self, uuid: UUID, value: bool):
-        if value:
-            self[(NOTIFIED, uuid)] = value
-        else:
-            try:
-                del self[(NOTIFIED, uuid)]
-            except KeyError:
-                pass
+        self[(NOTIFIED, uuid)] = value
 
     def status_sat(self, uuid: UUID):
-        return self.get(
-            (STATUS_SAT, uuid), {}
-        )
+        return self.get((STATUS_SAT, uuid), {})
 
     def status_sat_set(self, uuid: UUID, value: dict):
         if value:
             self[(STATUS_SAT, uuid)] = value
         else:
             try:
                 del self[(STATUS_SAT, uuid)]
@@ -98,27 +80,29 @@
 class LocalDBSatCFDI(LocalDB):
     def __init__(self, enviar_a_partir, pagar_a_partir):
         super().__init__()
         self.enviar_a_partir = enviar_a_partir
         self.pagar_a_partir = pagar_a_partir
 
     def notified(self, cfdi: SatCFDI):
-        if cfdi["Fecha"] >= self.enviar_a_partir:
-            return super().notified(cfdi.uuid)
-        return True
+        v = super().notified(cfdi.uuid)
+        if v is None and cfdi["Fecha"] < self.enviar_a_partir:
+            return True
+        return v
 
     def notified_flip(self, cfdi: SatCFDI):
         v = not self.notified(cfdi)
         self.notified_set(cfdi.uuid, v)
         return v
 
     def liquidated(self, cfdi: SatCFDI):
-        if cfdi["Fecha"] >= self.pagar_a_partir[cfdi["MetodoPago"]]:
-            return super().liquidated(cfdi.uuid)
-        return True
+        v = super().liquidated(cfdi.uuid)
+        if v is None and cfdi["Fecha"] < self.pagar_a_partir[cfdi["MetodoPago"]]:
+            return True
+        return v
 
     def liquidated_flip(self, cfdi: SatCFDI):
         v = not self.liquidated(cfdi)
         self.liquidated_set(cfdi.uuid, v)
         return v
 
     def status_sat(self, cfdi: SatCFDI, update=False):
@@ -134,15 +118,15 @@
         if cfdi.estatus == '0':
             return LiquidatedState.CANCELLED
 
         if cfdi["TipoDeComprobante"] != "I":
             return LiquidatedState.NONE
 
         mpago = cfdi["MetodoPago"]
-        if mpago == PPD and cfdi.saldo_pendiente == 0:
+        if cfdi['Total'] == 0 or (mpago == PPD and cfdi.saldo_pendiente == 0):
             return LiquidatedState.YES
 
         if self.liquidated(cfdi):
             if mpago == PPD:
                 return LiquidatedState.IGNORED
             return LiquidatedState.YES
```

### Comparing `satdigitalinvoice-2.1.3/satdigitalinvoice/log_tools.py` & `satdigitalinvoice-2.1.4/satdigitalinvoice/log_tools.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.3/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-2.1.4/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.3/satdigitalinvoice/mycfdi.py` & `satdigitalinvoice-2.1.4/satdigitalinvoice/mycfdi.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.3/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-2.1.4/satdigitalinvoice/schemas/factura.yaml`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.3/satdigitalinvoice/utils.py` & `satdigitalinvoice-2.1.4/satdigitalinvoice/utils.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.3/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-2.1.4/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 2.1.3
+Version: 2.1.4
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-2.1.3/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-2.1.4/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.3/setup.py` & `satdigitalinvoice-2.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.3/tests/test_crear_facturas.py` & `satdigitalinvoice-2.1.4/tests/test_crear_facturas.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.3/tests/test_localdb.py` & `satdigitalinvoice-2.1.4/tests/test_localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.3/tests/test_main.py` & `satdigitalinvoice-2.1.4/tests/test_main.py`

 * *Files identical despite different names*


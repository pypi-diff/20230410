# Comparing `tmp/mexa-0.4.tar.gz` & `tmp/mexa-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mexa-0.4.tar", last modified: Sun Apr  2 10:18:10 2023, max compression
+gzip compressed data, was "mexa-0.5.tar", last modified: Mon Apr 10 13:01:15 2023, max compression
```

## Comparing `mexa-0.4.tar` & `mexa-0.5.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxrwxr-x   0 fitorec   (1002) fitorec   (1002)        0 2023-04-02 10:18:10.859389 mexa-0.4/
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     1771 2023-04-02 10:18:10.859389 mexa-0.4/PKG-INFO
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     1093 2023-04-02 09:39:07.000000 mexa-0.4/README.md
-drwxrwxr-x   0 fitorec   (1002) fitorec   (1002)        0 2023-04-02 10:18:10.859389 mexa-0.4/mexa/
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     3813 2023-04-02 10:06:34.000000 mexa-0.4/mexa/NssField.py
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)      412 2023-04-02 10:08:04.000000 mexa-0.4/mexa/__init__.py
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)      581 2023-04-02 10:08:52.000000 mexa-0.4/mexa/core.py
-drwxrwxr-x   0 fitorec   (1002) fitorec   (1002)        0 2023-04-02 10:18:10.859389 mexa-0.4/mexa.egg-info/
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     1771 2023-04-02 10:18:10.000000 mexa-0.4/mexa.egg-info/PKG-INFO
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)      177 2023-04-02 10:18:10.000000 mexa-0.4/mexa.egg-info/SOURCES.txt
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)        1 2023-04-02 10:18:10.000000 mexa-0.4/mexa.egg-info/dependency_links.txt
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)        5 2023-04-02 10:18:10.000000 mexa-0.4/mexa.egg-info/top_level.txt
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)       38 2023-04-02 10:18:10.859389 mexa-0.4/setup.cfg
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)      641 2023-04-02 10:17:41.000000 mexa-0.4/setup.py
+drwxrwxr-x   0 fitorec   (1002) fitorec   (1002)        0 2023-04-10 13:01:15.350175 mexa-0.5/
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     2650 2023-04-10 13:01:15.350175 mexa-0.5/PKG-INFO
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     2255 2023-04-10 12:32:27.000000 mexa-0.5/README.md
+drwxrwxr-x   0 fitorec   (1002) fitorec   (1002)        0 2023-04-10 13:01:15.350175 mexa-0.5/mexa/
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     6339 2023-04-10 12:05:44.000000 mexa-0.5/mexa/CurpField.py
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     5088 2023-04-09 06:32:38.000000 mexa-0.5/mexa/CurpUtils.py
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)      455 2023-04-09 07:02:37.000000 mexa-0.5/mexa/ErrorMsgs.py
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)      801 2023-04-05 05:08:01.000000 mexa-0.5/mexa/Estados.py
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     4026 2023-04-10 12:28:08.000000 mexa-0.5/mexa/NssField.py
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)      731 2023-04-06 08:12:32.000000 mexa-0.5/mexa/__init__.py
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     1647 2023-04-09 06:59:20.000000 mexa-0.5/mexa/core.py
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     2231 2023-04-04 05:39:25.000000 mexa-0.5/mexa/data_ladas.py
+drwxrwxr-x   0 fitorec   (1002) fitorec   (1002)        0 2023-04-10 13:01:15.350175 mexa-0.5/mexa.egg-info/
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     2650 2023-04-10 13:01:15.000000 mexa-0.5/mexa.egg-info/PKG-INFO
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)      266 2023-04-10 13:01:15.000000 mexa-0.5/mexa.egg-info/SOURCES.txt
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)        1 2023-04-10 13:01:15.000000 mexa-0.5/mexa.egg-info/dependency_links.txt
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)        5 2023-04-10 13:01:15.000000 mexa-0.5/mexa.egg-info/top_level.txt
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)       38 2023-04-10 13:01:15.350175 mexa-0.5/setup.cfg
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)      641 2023-04-10 12:49:34.000000 mexa-0.5/setup.py
```

### Comparing `mexa-0.4/mexa/NssField.py` & `mexa-0.5/mexa/NssField.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,104 +1,114 @@
 # encoding: utf-8
-'''Clase encargada del NSS'''
-import datetime
+'''Clase encargada del Nss'''
 import re
 import random
-from mexa.core import FieldInterface
+from mexa.core import FieldInterface, year_by_last2digit
 
 class NssField(FieldInterface):
-    '''Clase que modela el NSS'''
+    '''Clase que modela el Nss'''
 
     @staticmethod
     def nss_checksum(nss):
-        '''Recibe una cadena de 10(o mas) caracteres y regresa el checksum de los primeros diez'''
+        '''Recibe un string que representa el nss, regresa el checksum'''
         if len(nss) < 10:
             NssField.error_msg = None
             return -1
         suma = 0
         for i in range(10):
-            factor = 2 if (i % 2 == 1) else 1
+            # factor = 2 if (i % 2 == 1) else 1
+            factor = 1 + (i % 2)
             v = int(nss[i]) * factor
-            suma += (1 + v % 10) if (v >9) else v
+            suma += (1 + v % 10) if (v > 9) else v
         cs = (suma * 9) % 10
         return cs
 
-    @staticmethod
-    def complete_year(last2digits):
-        '''Regresa el año completo a partir de los dos últimod digitos'''
-        y = int(last2digits)
-        current_year = datetime.date.today().year % 100
-        centenas = 20 if y <= current_year else 19
-        return (centenas * 100) + y
 
     @staticmethod
     def is_valid(value):
         '''Devuelve true si value es valido'''
-        NssField.error_msg = None
+        NssField.clear_errors()
         if len(value) != 11:
             NssField.error_msg = 'El valor debe tener una longitud de 11'
             return False
         s = re.search(r'^(\d{2})(\d{2})(\d{2})(\d{4})(\d)$', value)
         if not s:
             NssField.error_msg = 'Formato invalido de entrada'
             return False
         # reg_imss = s.group(1)
-        f_afi = NssField.complete_year(s.group(2))
-        f_nac = NssField.complete_year(s.group(3))
+        f_afi = year_by_last2digit(s.group(2))
+        f_nac = year_by_last2digit(s.group(3))
         if int(f_afi) < int(f_nac):
-            NssField.error_msg = f"No se pudo afiliar({f_afi}) antes de haber nacido({f_nac})"
+            msg = f"No se pudo afiliar({f_afi}) antes de haber nacido({f_nac})"
+            NssField.error_msg = msg
             return False
         if NssField.nss_checksum(value) == int(s.group(5)):
             return True
         NssField.error_msg = 'Input invalido'
         return False
 
+
     @staticmethod
     def autocomplete(value):
         '''Devuelve true si value es valido'''
         if len(value) != 10:
             return value
         cs = NssField.nss_checksum(value)
         return f"{value}{cs}"
 
+
     @staticmethod
     def anios(data  = None):
-        '''Devuelve arreglo ordenado con los años de nacimeinto y el de afiliacion'''
+        '''
+        Devuelve un arreglo con los años de nacimiento y afiliacion
+
+        :param dic data: Los datos el cual puede contener f_nacimiento
+                        y f_afiliacion de existir deberán ser tomados
+                        en cuenta estos valores.
+        :return: Arreglo ordenado de la forma [f_nacimiento, f_afiliacion]
+        '''
         if data is None:
             data  = {}
         if 'f_nacimiento' in data and 'f_afiliacion' in data:
             return [
-              NssField.complete_year(data['f_nacimiento']),
-              NssField.complete_year(data['f_afiliacion'])
+              year_by_last2digit(data['f_nacimiento']),
+              year_by_last2digit(data['f_afiliacion'])
             ]
         if 'f_nacimiento' in data:
-            nac = NssField.complete_year(data['f_nacimiento'])
+            nac = year_by_last2digit(data['f_nacimiento'])
             while True:
-                afil = NssField.complete_year(random.randrange(0, 99))
+                afil = year_by_last2digit(random.randrange(0, 99))
                 if afil >= nac:
                     return [nac, afil]
         if 'f_afiliacion' in data:
-            afil  = NssField.complete_year(data['f_afiliacion'])
+            afil  = year_by_last2digit(data['f_afiliacion'])
             while True:
-                nac = NssField.complete_year(random.randrange(0, 99))
+                nac = year_by_last2digit(random.randrange(0, 99))
                 if afil >= nac:
                     return [nac, afil]
-        y1 = NssField.complete_year(random.randrange(0, 99))
-        y2 = NssField.complete_year(random.randrange(0, 99))
+        y1 = year_by_last2digit(random.randrange(0, 99))
+        y2 = year_by_last2digit(random.randrange(0, 99))
         if y1 <= y2:
             return [y1, y2]
         return [y2, y1]
 
+
     @staticmethod
     def generate(data = None):
-        '''Devuelve un NSS valido'''
+        '''
+        Genera un Nss a partir de los datos recibidos.
+
+        :param dic data: Los valores contenidos deberán ser tomados en cuenta.
+        :return: str nss Un número del Seguro Social válido
+        '''
         if data is None:
             data  = {}
-        region_imss = data['region_imss'] if 'region_imss' in data else random.randrange(0, 99)
+        reg = data['region_imss'] if 'region_imss' in data else random.randrange(0, 99)
         years = NssField.anios(data)
-        folio_imss = data['folio_imss'] if 'folio_imss' in data else random.randrange(10, 9999)
-        # Variables a usar
-        reg = str(region_imss).rjust(2, '0')
+        fol = data['folio_imss'] if 'folio_imss' in data else random.randrange(0, 9999)
+        # Asignacion y formato
+        reg = str(reg).rjust(2, '0')
         afi = str(years[1])[-2:] # Año de Afiliacion
         nac = str(years[0])[-2:] # Año de Nacimiento
-        fol = str(folio_imss).rjust(4, '0')
+        fol = str(fol).rjust(4, '0')
+        # Se envia a autocomplete los diez primeros digitos para que le agregue el cs
         return NssField.autocomplete(f'{reg}{afi}{nac}{fol}')
```

### Comparing `mexa-0.4/setup.py` & `mexa-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 readme = open('./README.md', 'r')
 
 setup(
     name = 'mexa',
-    version = '0.4',
+    version = '0.5',
     packages=['mexa'],
     description = 'Validador y Generador de campos para tramites mexicanos',
     author='@Fitorec - Miguel Angel Marcial Martinez',
     author_email = 'fitorec@mundosica.com',
     url = 'https://github.com/fitorec/mexa-py',
     long_description = readme.read(),
     long_description_content_type = 'text/markdown',
```


# Comparing `tmp/melkit-0.1.3.tar.gz` & `tmp/melkit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melkit-0.1.3.tar", last modified: Wed Mar 15 14:50:08 2023, max compression
+gzip compressed data, was "melkit-0.1.4.tar", last modified: Mon Apr 10 10:57:54 2023, max compression
```

## Comparing `melkit-0.1.3.tar` & `melkit-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:50:08.110876 melkit-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-15 14:50:07.000000 melkit-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-15 14:50:07.000000 melkit-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-15 14:50:08.110876 melkit-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-15 14:50:07.000000 melkit-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:50:08.110876 melkit-0.1.3/melkit/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-15 14:50:07.000000 melkit-0.1.3/melkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-15 14:50:07.000000 melkit-0.1.3/melkit/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-15 14:50:07.000000 melkit-0.1.3/melkit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-03-15 14:50:07.000000 melkit-0.1.3/melkit/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-03-15 14:50:07.000000 melkit-0.1.3/melkit/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-15 14:50:07.000000 melkit-0.1.3/melkit/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:50:08.110876 melkit-0.1.3/melkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-15 14:50:08.000000 melkit-0.1.3/melkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-15 14:50:08.000000 melkit-0.1.3/melkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 14:50:08.000000 melkit-0.1.3/melkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-15 14:50:08.000000 melkit-0.1.3/melkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-15 14:50:08.000000 melkit-0.1.3/melkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-15 14:50:07.000000 melkit-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 14:50:08.110876 melkit-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-03-15 14:50:07.000000 melkit-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:57:54.370715 melkit-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-10 10:57:53.000000 melkit-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 10:57:53.000000 melkit-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-10 10:57:54.370715 melkit-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-10 10:57:53.000000 melkit-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:57:54.366715 melkit-0.1.4/melkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-10 10:57:53.000000 melkit-0.1.4/melkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-10 10:57:53.000000 melkit-0.1.4/melkit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-10 10:57:53.000000 melkit-0.1.4/melkit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-10 10:57:53.000000 melkit-0.1.4/melkit/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22679 2023-04-10 10:57:53.000000 melkit-0.1.4/melkit/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 10:57:53.000000 melkit-0.1.4/melkit/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:57:54.370715 melkit-0.1.4/melkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-10 10:57:54.000000 melkit-0.1.4/melkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-10 10:57:54.000000 melkit-0.1.4/melkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 10:57:54.000000 melkit-0.1.4/melkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-10 10:57:54.000000 melkit-0.1.4/melkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 10:57:54.000000 melkit-0.1.4/melkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-10 10:57:53.000000 melkit-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 10:57:54.370715 melkit-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-10 10:57:53.000000 melkit-0.1.4/setup.py
```

### Comparing `melkit-0.1.3/LICENSE` & `melkit-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `melkit-0.1.3/README.md` & `melkit-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,46 +2,48 @@
 
 # MELKIT 🧰
 
 A toolkit designed to facilitate the handling of MELCOR/MELGEN `1.8.6` files.
 
 ## ⚙️ Utilities
 
-- Reading Control Volumes (`CVs`) and Flow Paths (`FLs`) and converting them to objects.
-- Writing, deleting and editing `CVs` and `FLs`.
+- Reading Control Volumes (`CVs`), Flow Paths (`FLs`), Control Functions (`CFs`) and converting them to objects.
+- Writing, deleting and editing `CVs`, `FLs` and `CFs`.
 - Plotting files generated by the `EDF` package (`PTF` support is planned!)
 - Extraction of values printed by `EDF`.
-- Obtaining the list of available/used IDs for certain objects (`CVs`, `FLs`).
+- Obtaining the list of available/used IDs for different objects (`CVs`, `FLs`, `CFs`).
 - Remove all comments from an input file.
 - Search for objects by their ID.
 - Search for duplicate objects in a given list.
 - Get adjacent `CVs` and `FL` connections for a given `CV`.
+- Get `CFs` associated with a given `FL`.
+- Recursively extract inter-dependent `CFs`.
 - Create submodels from a given `CV` (_beta_).
 
-## ➕ Extensions
-
-Includes **MELCOR Language Support** (`mls`): a MELCOR 1.8.6 syntax highlighter for Visual Studio Code.
-
-Just copy the [`mls` folder](https://github.com/manjavacas/melkit/tree/main/vscode/mls) in `.vscode/extensions` for an improved MELCOR coding experience. 
-
-You can find the Visual Studio Code installation folder in the following paths:
-
-* **Windows**: `%USERPROFILE%\.vscode\extensions`
-* **macOS**: `~/.vscode/extensions`
-* **Linux**: `~/.vscode/extensions`
-
 ## 💻 How to use
 
 You simply need to instantiate a `Toolkit` with the name of the MELGEN file to manipulate and call those functions. For example:
 
 ```python
 from melkit.toolkit import Toolkit
 
 toolkit = Toolkit(filename)
 
 cvs = toolkit.read_cvs()
 fls = toolkit.read_fls()
 ```
 
+## ➕ Extensions
+
+Includes **MELCOR Language Support** (`mls`): a MELCOR 1.8.6 syntax highlighter for Visual Studio Code.
+
+Just copy the [`mls` folder](https://github.com/manjavacas/melkit/tree/main/vscode/mls) in `.vscode/extensions` for an improved MELCOR coding experience. 
+
+You can find the Visual Studio Code installation folder in the following paths:
+
+* **Windows**: `%USERPROFILE%\.vscode\extensions`
+* **macOS**: `~/.vscode/extensions`
+* **Linux**: `~/.vscode/extensions`
+
 ## 👐 Contributing
 
 Feel free to contribute via _issues_ and _pull requests_.
```

### Comparing `melkit-0.1.3/melkit/inputs.py` & `melkit-0.1.4/melkit/inputs.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,14 +28,23 @@
     def update_field(self, field_name: str, new_val: str) -> None:
         for record in self.records:
             if field_name in self.records[record]:
                 self.records[record][field_name] = new_val
 
     def __eq__(self, other):
         return self.get_id() == other.get_id()
+    
+    def __str__(self):
+        obj_str = []
+        for record, fields in self.records.items():
+            obj_str.append(f'{record}\t')
+            for value in fields.values():
+                obj_str.append(f'{value}\t')
+            obj_str.append('\n')
+        return ''.join(obj_str)
 
 
 class CV(Object):
     '''
     Control Volume class (CVH package).
     '''
     def __str__(self):
@@ -51,15 +60,12 @@
         return ''.join(cv_str)
 
 
 class FL(Object):
     '''
     Flow Path class (FL package).
     '''
-    def __str__(self):
-        fl_str = []
-        for record, fields in self.records.items():
-            fl_str.append(f'{record}\t')
-            for value in fields.values():
-                fl_str.append(f'{value}\t')
-            fl_str.append('\n')
-        return ''.join(fl_str)
+
+class CF(Object):
+    '''
+    Control Function class (CF package).
+    '''
```

### Comparing `melkit-0.1.3/melkit/toolkit.py` & `melkit-0.1.4/melkit/toolkit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 '''
 MELGEN/MELCOR file manipulation tools.
 '''
 
 from pandas import DataFrame, read_csv
 
 from os import remove
-from re import search, match
+from re import search, match, findall
+from json import dumps
 
 from typing import List, Union
 
 from .exceptions import ParseException
-from .inputs import Object, CV, FL
+from .inputs import Object, CV, FL, CF
 from .constants import CV_KEYS
 
 
 class Toolkit:
     '''
     Multi-purpose file manipulator.
     '''
 
     def __init__(self, filename: str):
         self._filename = filename
 
         self._cv_list = self._read_cvs()
         self._fl_list = self._read_fls()
+        self._cf_list = self._read_cfs()
 
 #------------------------ OBJECT MANIPULATION TOOLS -----------------------#
 
     def _read_object(self, id_regex: str) -> List[Object]:
         '''
         Looks for objects in the input file according to a given ID regex
         '''
@@ -36,27 +38,35 @@
             for line in file:
                 id = search(id_regex, line)
                 if id and id not in ids:
                     if 'CV' in id_regex:
                         objs.append(self.get_cv(id.group()[:-2]))
                     elif 'FL' in id_regex:
                         objs.append(self.get_fl(id.group()[:-2]))
+                    elif 'CF' in id_regex:
+                        objs.append(self.get_cf(id.group()[:-2]))
         return objs
 
     def _read_cvs(self) -> List[CV]:
         '''
         Looks for CVs in the input file and returns them as a list of CV objects.
         '''
         return self._read_object(r'\bCV\d{3}00\b')
 
     def _read_fls(self) -> List[FL]:
         '''
         Looks for FLs in the input file and returns them as a list of FL objects.
         '''
         return self._read_object(r'\bFL\d{3}00\b')
+    
+    def _read_cfs(self) -> List[CF]:
+        '''
+        Looks for CFs in the input file and returns them as a list of CF objects.
+        '''
+        return self._read_object(r'\bCF\d{3,8}00\b')
 
     def get_cv(self, cv_id: str) -> CV:
         '''
         Searches for a CV in the input file and returns it as a CV object.
         '''
         cv_data = {}
 
@@ -179,25 +189,89 @@
                     except:
                         raise ParseException(
                             fl_id, f'Invalid number of attributes for record {record_id}')
                     fl_data[record_id] = record_data
 
         return FL(fl_data)
 
+    def get_cf(self, cf_id: str) -> CF:
+        '''
+        Searches for a CF in the input file and returns it as a CF object.
+        '''
+        cf_data = {}
+        
+        arg_c = 0   # arg counter
+
+        with open(self._filename, 'r') as file:
+            for line in file:
+                if line.startswith(cf_id):
+                    record = line.split()
+                    record_id = record[0]
+                    record_data = {}
+
+                    termination = record_id[-2:]
+
+                    try:
+                        if termination == '00':
+                            record_data['CFNAME'] = record[1]
+                            record_data['CFTYPE'] = record[2]
+                            record_data['NCFARG'] = record[3]
+                            record_data['CFSCAL'] = record[4]
+                            record_data['CFADCN'] = record[5] if len(record) > 5 else 0.0
+                        elif termination == '01':
+                            if record[1] in ['.TRUE.', '.FALSE.']:
+                                record_data['LCFVAL'] = record[1]
+                            else:
+                                record_data['CFVALR'] = record[1] 
+                        elif termination == '02':
+                            record_data['ICFLIM'] = record[1]
+                            if int(record[1]) in [1, 2, 3]:
+                                record_data['CFLIML'] = record[2]
+                            if int(record[1]) in [2, 3]:
+                                record_data['CFLIMU'] = record[3]
+                        elif match(r'0[3-4]', termination):
+                            record_data['FIELDS'] = record[1] # Fixable
+                        elif termination == '05':
+                            record_data['CLASS'] = record[1]
+                        elif termination == '06':
+                            record_data['MSGFIL'] = record[1]
+                            if int(record[1]) in [1, 2]:
+                                record_data['SWTMSG'] = record[2]
+                        elif match(r'[10-99]', termination):
+                            record_data['ARSCAL_' + str(arg_c)] = record[1]
+                            record_data['ARADCN_' + str(arg_c)] = record[2]
+                            record_data['CHARG_' + str(arg_c)] = record[3]
+                            arg_c += 1
+                        else:
+                            raise ParseException(
+                                cf_id, f'Unknown record: {record_id}')
+                    except:
+                        raise ParseException(
+                            cf_id, f'Invalid number of attributes for record {record_id}')
+                    cf_data[record_id] = record_data
+
+        return CF(cf_data)
+
     def get_cv_list(self) -> List[CV]:
         '''
         Return the list of CVs in parsed file.
         '''
         return self._cv_list
 
     def get_fl_list(self) -> List[FL]:
         '''
         Return the list of CVs in parsed file.
         '''
         return self._fl_list
+    
+    def get_cf_list(self) -> List[CF]:
+        '''
+        Return the list of CFs in parsed file.
+        '''
+        return self._cf_list
 
     def remove_object(self, obj_id: str, src_file: str = None, new_file: str = None) -> None:
         '''
         Deletes an object from the input file.
         '''
 
         src_file = src_file or self._filename
@@ -372,14 +446,45 @@
             if cv_id[2:] == fl.get_field('KCVFM'):
                 cv_connected.append(self.id_search(
                     self._cv_list, 'CV' + fl.get_field('KCVTO')))
             elif cv_id[2:] == fl.get_field('KCVTO'):
                 cv_connected.append(self.id_search(
                     self._cv_list, 'CV' + fl.get_field('KCVFM')))
         return cv_connected
+    
+
+    def get_connected_cfs(self, obj_id: str) -> List[CF]:
+        '''
+        Get those CFs directly or indirectly connected to a given Object.
+        - If the Object is an FL, the CF associated with the CFnnnTk record is returned and, recursively, all CFs on which this CF depends are added.
+        - If the object is a CF, that CF and its dependencies are returned.
+        '''
+        cf_connected = []
+
+        # Get a CF specified in the FL Tk record
+        if obj_id.startswith('FL'):
+            fl = self.get_fl(obj_id)
+            for key in fl.records.keys():
+                if match(obj_id + r'T[0-9]$', key) and fl.records[key]['NTFLAG'] == '2':
+                    cf_id = 'CF' + fl.records[key]['NFUN']
+                    cf_connected.append(self.get_cf(cf_id))
+                    # Recursion for interdependent CFs
+                    cf_connected += self.get_connected_cfs(cf_id)
+        # Get those CFs related to a given CF
+        elif obj_id.startswith('CF'):
+            cf = self.get_cf(obj_id)
+            cf_values = findall(r'\bCFVALU\.\d+\b', dumps(cf.records))
+            for value in cf_values: 
+                dot_pos = value.find('.')
+                cf_id = 'CF' + value[dot_pos + 1:]
+                cf_connected.append(self.get_cf(cf_id))
+                cf_connected += self.get_connected_cfs(cf_id)
+
+        return cf_connected
+
 
     def create_submodel(self, cv_id: str, new_file: str = None) -> Union[List[CV], List[FL]]:
         '''
         Creates a submodel related to a given CV. Those neighbour CVs are made time-independent.
         '''
 
         new_file = new_file or self._filename + '_SUB'
```

### Comparing `melkit-0.1.3/setup.py` & `melkit-0.1.4/setup.py`

 * *Files identical despite different names*


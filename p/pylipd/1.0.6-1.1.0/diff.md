# Comparing `tmp/pylipd-1.0.6.tar.gz` & `tmp/pylipd-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylipd-1.0.6.tar", last modified: Fri Apr  7 06:13:27 2023, max compression
+gzip compressed data, was "pylipd-1.1.0.tar", last modified: Mon Apr 10 19:07:34 2023, max compression
```

## Comparing `pylipd-1.0.6.tar` & `pylipd-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-07 06:13:27.903817 pylipd-1.0.6/
--rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.0.6/LICENSE
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-07 06:13:27.903864 pylipd-1.0.6/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.0.6/README.md
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-07 06:13:27.902426 pylipd-1.0.6/pylipd/
--rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-07 06:13:24.000000 pylipd-1.0.6/pylipd/__init__.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-07 06:13:27.902854 pylipd-1.0.6/pylipd/globals/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.0.6/pylipd/globals/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)      383 2022-11-15 21:36:42.000000 pylipd-1.0.6/pylipd/globals/blacklist.py
--rw-r--r--   0 varun      (502) staff       (20)    14564 2023-03-06 15:30:09.000000 pylipd-1.0.6/pylipd/globals/schema.py
--rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.0.6/pylipd/globals/urls.py
--rw-r--r--   0 varun      (502) staff       (20)    15901 2023-04-07 06:12:11.000000 pylipd-1.0.6/pylipd/legacy_utils.py
--rw-r--r--   0 varun      (502) staff       (20)    28677 2023-04-07 04:11:12.000000 pylipd-1.0.6/pylipd/lipd.py
--rw-r--r--   0 varun      (502) staff       (20)    42808 2023-03-31 15:11:12.000000 pylipd-1.0.6/pylipd/lipd_to_rdf.py
--rw-r--r--   0 varun      (502) staff       (20)     1742 2023-04-07 05:39:21.000000 pylipd-1.0.6/pylipd/multi_processing.py
--rw-r--r--   0 varun      (502) staff       (20)    17140 2023-02-23 13:16:36.000000 pylipd-1.0.6/pylipd/rdf_to_lipd.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-07 06:13:27.903050 pylipd-1.0.6/pylipd/series/
--rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.0.6/pylipd/series/__init__.py
--rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.0.6/pylipd/series/regexes.py
--rw-r--r--   0 varun      (502) staff       (20)     2270 2023-03-22 17:52:14.000000 pylipd-1.0.6/pylipd/test.py
--rw-r--r--   0 varun      (502) staff       (20)     4141 2023-04-07 05:57:19.000000 pylipd-1.0.6/pylipd/usage.py
--rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.0.6/pylipd/utils.py
-drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-07 06:13:27.903707 pylipd-1.0.6/pylipd.egg-info/
--rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-07 06:13:27.000000 pylipd-1.0.6/pylipd.egg-info/PKG-INFO
--rw-r--r--   0 varun      (502) staff       (20)      588 2023-04-07 06:13:27.000000 pylipd-1.0.6/pylipd.egg-info/SOURCES.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-04-07 06:13:27.000000 pylipd-1.0.6/pylipd.egg-info/dependency_links.txt
--rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.0.6/pylipd.egg-info/not-zip-safe
--rw-r--r--   0 varun      (502) staff       (20)       29 2023-04-07 06:13:27.000000 pylipd-1.0.6/pylipd.egg-info/requires.txt
--rw-r--r--   0 varun      (502) staff       (20)        7 2023-04-07 06:13:27.000000 pylipd-1.0.6/pylipd.egg-info/top_level.txt
--rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.0.6/pyproject.toml
--rw-r--r--   0 varun      (502) staff       (20)      686 2023-04-07 06:13:27.904103 pylipd-1.0.6/setup.cfg
--rw-r--r--   0 varun      (502) staff       (20)      956 2023-04-07 06:13:22.000000 pylipd-1.0.6/setup.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-10 19:07:34.477273 pylipd-1.1.0/
+-rw-r--r--   0 varun      (502) staff       (20)    11357 2022-09-22 13:14:27.000000 pylipd-1.1.0/LICENSE
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-10 19:07:34.477335 pylipd-1.1.0/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      630 2023-03-22 12:37:06.000000 pylipd-1.1.0/README.md
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-10 19:07:34.474853 pylipd-1.1.0/pylipd/
+-rw-r--r--   0 varun      (502) staff       (20)       22 2023-04-10 12:31:16.000000 pylipd-1.1.0/pylipd/__init__.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-10 19:07:34.475643 pylipd-1.1.0/pylipd/globals/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:18.000000 pylipd-1.1.0/pylipd/globals/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)      409 2023-04-10 19:03:17.000000 pylipd-1.1.0/pylipd/globals/blacklist.py
+-rw-r--r--   0 varun      (502) staff       (20)    14643 2023-04-10 19:06:28.000000 pylipd-1.1.0/pylipd/globals/schema.py
+-rw-r--r--   0 varun      (502) staff       (20)      197 2022-11-14 07:40:00.000000 pylipd-1.1.0/pylipd/globals/urls.py
+-rw-r--r--   0 varun      (502) staff       (20)    15901 2023-04-10 05:47:05.000000 pylipd-1.1.0/pylipd/legacy_utils.py
+-rw-r--r--   0 varun      (502) staff       (20)    30545 2023-04-10 07:14:07.000000 pylipd-1.1.0/pylipd/lipd.py
+-rw-r--r--   0 varun      (502) staff       (20)    43704 2023-04-10 19:04:22.000000 pylipd-1.1.0/pylipd/lipd_to_rdf.py
+-rw-r--r--   0 varun      (502) staff       (20)     1742 2023-04-07 05:39:21.000000 pylipd-1.1.0/pylipd/multi_processing.py
+-rw-r--r--   0 varun      (502) staff       (20)    22294 2023-04-10 19:05:37.000000 pylipd-1.1.0/pylipd/rdf_to_lipd.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-10 19:07:34.475994 pylipd-1.1.0/pylipd/series/
+-rw-r--r--   0 varun      (502) staff       (20)        0 2023-01-10 17:13:31.000000 pylipd-1.1.0/pylipd/series/__init__.py
+-rw-r--r--   0 varun      (502) staff       (20)     3223 2022-11-15 20:06:27.000000 pylipd-1.1.0/pylipd/series/regexes.py
+-rw-r--r--   0 varun      (502) staff       (20)     2270 2023-03-22 17:52:14.000000 pylipd-1.1.0/pylipd/test.py
+-rw-r--r--   0 varun      (502) staff       (20)     5054 2023-04-10 12:38:55.000000 pylipd-1.1.0/pylipd/usage.py
+-rw-r--r--   0 varun      (502) staff       (20)     2602 2023-02-23 10:01:04.000000 pylipd-1.1.0/pylipd/utils.py
+drwxr-xr-x   0 varun      (502) staff       (20)        0 2023-04-10 19:07:34.477177 pylipd-1.1.0/pylipd.egg-info/
+-rw-r--r--   0 varun      (502) staff       (20)     1282 2023-04-10 19:07:34.000000 pylipd-1.1.0/pylipd.egg-info/PKG-INFO
+-rw-r--r--   0 varun      (502) staff       (20)      588 2023-04-10 19:07:34.000000 pylipd-1.1.0/pylipd.egg-info/SOURCES.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-04-10 19:07:34.000000 pylipd-1.1.0/pylipd.egg-info/dependency_links.txt
+-rw-r--r--   0 varun      (502) staff       (20)        1 2023-02-24 09:46:52.000000 pylipd-1.1.0/pylipd.egg-info/not-zip-safe
+-rw-r--r--   0 varun      (502) staff       (20)       35 2023-04-10 19:07:34.000000 pylipd-1.1.0/pylipd.egg-info/requires.txt
+-rw-r--r--   0 varun      (502) staff       (20)        7 2023-04-10 19:07:34.000000 pylipd-1.1.0/pylipd.egg-info/top_level.txt
+-rw-r--r--   0 varun      (502) staff       (20)      104 2023-02-10 17:39:16.000000 pylipd-1.1.0/pyproject.toml
+-rw-r--r--   0 varun      (502) staff       (20)      693 2023-04-10 19:07:34.477604 pylipd-1.1.0/setup.cfg
+-rw-r--r--   0 varun      (502) staff       (20)      973 2023-04-10 12:31:07.000000 pylipd-1.1.0/setup.py
```

### Comparing `pylipd-1.0.6/LICENSE` & `pylipd-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylipd-1.0.6/PKG-INFO` & `pylipd-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.0.6
+Version: 1.1.0
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.0.6
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.1.0
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.0.6/README.md` & `pylipd-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pylipd-1.0.6/pylipd/globals/schema.py` & `pylipd-1.1.0/pylipd/globals/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,16 +237,15 @@
             'name': 'name' 
         }
     },
     'DataTable': {
         '@id': ['{filename}', '_trunc(4)'],
         '@fromJson': ['_set_inter_variable_links'],
         'filename': { 
-            'name': 'hasFileName', 
-            'type': 'File' 
+            'name': 'hasFileName'
         },
         'columns': {
             'name': 'includesVariable',
             'multiple': True,
             'schema': 'Variable'
         },
         'missingValue': { 
@@ -265,20 +264,22 @@
             '_set_variable_category',
             '_wrap_uncertainty',
             '_create_proxy_system',
             '_add_found_in_table',
             '_add_variable_values',
             '_stringify_column_numbers_array'
         ],
+        '@toJson_pre': [
+            '_remove_found_in_table',
+            #'_remove_depth_property'
+        ],
         '@toJson': [
             '_set_variable_type',
             '_unwrap_uncertainty',
             '_extract_from_proxy_system',
-            '_remove_found_in_table',
-            '_remove_depth_property',
             '_extract_variable_values',
             '_unarray_column_number'
         ],
         'number': { 
             'name': 'hasColumnNumber', 
             'type': 'integer'
         },
@@ -343,14 +344,17 @@
             'alternates': ['resolution'],
             'name': 'hasResolution',
             'category': 'Resolution',
             'schema': 'Resolution',
             'type': 'Individual',
             'alternates': ['hasResolution']
         },
+        'physicalSample': {
+            'type': 'Individual',
+        },
         'inferredFrom': { 
             'schema': 'Variable', 
             'category': 'MeasuredVariable',
             'type': 'Individual'
         },
         'hasUncertainty': { 
             'schema': 'Uncertainty',
```

### Comparing `pylipd-1.0.6/pylipd/legacy_utils.py` & `pylipd-1.1.0/pylipd/legacy_utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.0.6/pylipd/lipd.py` & `pylipd-1.1.0/pylipd/lipd.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import os.path
 import tempfile
 import pandas as pd
 import random
 import string
 import io
 
-from rdflib import ConjunctiveGraph, Namespace
+from rdflib import ConjunctiveGraph, Namespace, URIRef
 from pylipd.multi_processing import multi_convert_to_pickle, multi_convert_to_rdf
 
 from pylipd.rdf_to_lipd import RDFToLiPD
 from pylipd.legacy_utils import LiPD_Legacy
 from pylipd.utils import sanitizeId, sparql_results_to_df
 
 #import bibtexparser
@@ -76,14 +76,34 @@
         pylipd.LiPD
             a copy of the original object
 
         '''
         
         return deepcopy(self)
 
+    def merge(self, lipd):
+        '''
+        Merges the current LiPD object with another LiPD object
+
+        Parameters
+        ----------
+        lipd : pylipd.LiPD
+            LiPD object to merge with
+
+        Returns
+        -------
+        pylipd.LiPD
+            merged LiPD object
+
+        '''
+
+        merged = self.copy()
+        merged.graph.addN(lipd.graph.quads())
+        return merged
+    
     def load_from_dir(self, dir_path, parallel=False, collection_id=None):
         '''Load LiPD files from a directory
         Note: This function creates multiple process to process lipd files in parallel, therefore it is important that this call be made under the "__main__" process
 
         Parameters
         ----------
 
@@ -604,23 +624,23 @@
         '''
         ts = self._get_timeseries(dsnames)
         return ts
 
     def _get_timeseries(self, dsnames):
         timeseries = {}
         for dsname in dsnames:
-            converter = RDFToLiPD()
-            d = converter.convert(dsname, self.graph)
+            converter = RDFToLiPD(self.graph)
+            d = converter.convert_to_json(dsname)
             print("Extracting timeseries from dataset: " + dsname + " ...")
             if len(d.items()):
                 tss = LiPD_Legacy().extract(d)
                 timeseries[dsname] = tss
         return timeseries
 
-    def get_lipd(self, dsname):
+    def get_lipd(self, dsname, lipdfile):
         '''Get LiPD json for a dataset
 
         Parameters
         ----------
 
         dsname : str
             dataset id
@@ -638,25 +658,56 @@
             lipd_remote = LiPD()
             lipd_remote.set_endpoint("https://linkedearth.graphdb.mint.isi.edu/repositories/LiPDVerse2")
             dsname = "Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001"
             lipd_remote.load_remote_datasets([dsname])
             lipd_json = lipd_remote.get_lipd(dsname)
             print(lipd_json)
         '''           
-        converter = RDFToLiPD()            
-        return converter.convert(dsname, self.graph)
+        converter = RDFToLiPD(self.graph)
+        return converter.convert_to_json(dsname, lipdfile)
+
+    def create_lipd(self, dsname, lipdfile):
+        '''Create LiPD file for a dataset
+
+        Parameters
+        ----------
 
-    def pop(self, dsname, collection_id=None):
+        dsname : str
+            dataset id
+
+        lipdfile: str
+            path to LiPD file
+
+        Examples
+        --------
+
+        .. ipython:: python
+            :okwarning:
+            :okexcept:
+
+            from pylipd.lipd import LiPD
+
+            # Fetch LiPD data from remote RDF Graph
+            lipd_remote = LiPD()
+            lipd_remote.set_endpoint("https://linkedearth.graphdb.mint.isi.edu/repositories/LiPDVerse2")
+            dsname = "Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001"
+            lipd_remote.load_remote_datasets([dsname])
+            lipd_remote.create_lipd(dsname, "test.lpd")
+        '''           
+        converter = RDFToLiPD(self.graph)
+        return converter.convert(dsname, lipdfile)
+    
+    def pop(self, dsname=None, collection_id=None):
         '''Removes a dataset from the graph and returns a LiPD object
 
         Parameters
         ----------
 
         dsname : str
-            Path to the directory containing lipd files
+            (Optional) Name of the dataset (Set to None to pop all datasets in a collection)
 
         collection_id : str
             (Optional) collection id for the dataset
 
         Examples
         --------
 
@@ -673,21 +724,40 @@
                 "../examples/data/MD98_2181.Stott.2007.lpd"
             ])
             all_datasets = lipd.get_all_dataset_names()
             print("Loaded datasets: " + str(all_datasets))
             popped = lipd.pop(all_datasets[0])
             print("Loaded datasets after pop: " + str(lipd.get_all_dataset_names()))
             print("Popped dataset: " + str(popped.get_all_dataset_names()))       
-        '''        
-        graphurl = NSURL + "/" + dsname
-        if collection_id:
-            graphurl = NSURL + "/" + collection_id + "/" + dsname
-        subgraph = copy.deepcopy(self.graph.get_context(graphurl))
-        self.graph.remove((None, None, None, graphurl))
-        return LiPD(subgraph)
+        '''
+
+        popped = LiPD()
+
+        if dsname:
+            graphurl = NSURL + "/" + dsname
+            if collection_id:
+                graphurl = NSURL + "/" + collection_id + "/" + dsname
+        elif collection_id:
+            graphurl = NSURL + "/" + collection_id
+
+        # Match subgraphs
+        for ctx in self.graph.contexts():
+            id = ctx.identifier
+            if id.startswith(graphurl):
+                subgraph = copy.deepcopy(self.graph.get_context(id))
+                for triple in subgraph.triples((None, None, None)):
+                    popped.graph.add((
+                        triple[0],
+                        triple[1],
+                        triple[2],
+                        URIRef(id)))
+
+                self.graph.remove((None, None, None, id))
+        
+        return popped
 
     def remove(self, dsname, collection_id=None):
         '''Removes a dataset from the graph
 
         Parameters
         ----------
```

### Comparing `pylipd-1.0.6/pylipd/lipd_to_rdf.py` & `pylipd-1.1.0/pylipd/lipd_to_rdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,17 @@
         
         if "properties" in geo and isinstance(geo["properties"], dict) :
             for key,value in geo["properties"].items() :
                 ngeo[key] = value
         elif isinstance(geo, dict) :
             for key,value in geo.items() :
                 if key != "geometry":
-                    ngeo[key] = value
+                    # Do not add lat long if they are already added
+                    if f"wgs84:{key}" not in ngeo:
+                        ngeo[key] = value
         return ngeo
 
 
     def _get_uncertainty(self, val, parent = None) :
         uncertainty = {}
         uncertainty["hasValue"] = val
         uncertainty["analytical"] = val
@@ -354,15 +356,15 @@
         return camelCase(observation)
 
     def _get_variable_id(self, obj, parentid) :
         iobj = dict((k.lower(), v) for k, v in obj.items())
         if "tsid" not in iobj:
             iobj["tsid"] = uniqid()
         id =  parentid + "." + iobj["tsid"]
-        id += "." + str(iobj["variablename"])
+        id += "." + str(iobj.get("variablename", ""))
         return id
     
     def _set_inter_variable_links(self, obj, objhash) :
         depthcol = None
         vobjhash = {}
         if "columns" not in obj:
             return [obj, objhash, []]
@@ -373,17 +375,19 @@
         depthcol =  vobjhash["depth"] if ("depth" in vobjhash) else None
         for col in obj["columns"] : 
             thiscol = self._get_variable_id(col, obj["@id"])
             if (("inferredFrom" in col)) :
                 infcol = col["inferredFrom"].lower()
                 if ((infcol in vobjhash)) :
                     col["inferredFrom"] = vobjhash[infcol]
-                
-            if (depthcol and thiscol != depthcol) :
-                col["takenAtDepth"] = depthcol
+
+            # FIXME: Adding takenAtDepth is messing stuff up   
+            #if (depthcol and thiscol != depthcol) :
+            #    col["takenAtDepth"] = depthcol
+
         return [obj, objhash, []]
     
     # proxy (could be specific)
     # proxyGeneral (more general than proxy)
     # proxyDetail (more specific than proxy)
     # proxyLumps ?
     # archiveType -> keep at dataset level ?
@@ -411,30 +415,36 @@
             proxyobs = obj["proxy"]
             #del obj["proxy"]
         elif ("OnProxyObservationProperty" in obj and obj["OnProxyObservationProperty"]) :
             proxyobs = obj["OnProxyObservationProperty"]
             del obj["OnProxyObservationProperty"]
         elif ("ProxyObservationType" in obj and obj["ProxyObservationType"]) :
             proxyobs = obj["ProxyObservationType"]
-            if "name" in obj and obj["name"] :
-                obj["name"] = obj["name"] + "." + proxyobs
+            if "variableName" in obj and obj["variableName"] :
+                varname = str(obj["variableName"])
+                if varname.lower() != proxyobs.lower() :
+                    obj["variableName"] = obj["variableName"] + "." + proxyobs
             else:
-                obj["name"] = proxyobs
+                obj["variableName"] = proxyobs
         elif ("proxyObservationType" in obj and obj["proxyObservationType"]) :
             proxyobs = obj["proxyObservationType"]
-            if "name" in obj and obj["name"] :
-                obj["name"] = obj["name"] + "." + proxyobs
+            if "variableName" in obj and obj["variableName"] :
+                varname = str(obj["variableName"])
+                if varname.lower() != proxyobs.lower() :
+                    obj["variableName"] = obj["variableName"] + "." + proxyobs
             else:
-                obj["name"] = proxyobs
+                obj["variableName"] = proxyobs
         elif ("inferredVariableType" in obj and obj["inferredVariableType"]) :
             infvar = obj["inferredVariableType"]
-            if "name" in obj and obj["name"] :
-                obj["name"] = obj["name"] + "." + infvar
+            if "variableName" in obj and obj["variableName"] :
+                varname = str(obj["variableName"])
+                if varname.lower() != infvar.lower() :
+                    obj["variableName"] = varname + "." + infvar
             else:
-                obj["name"] = infvar
+                obj["variableName"] = infvar
 
         vartype = obj["@category"]
         if (vartype and vartype == "MeasuredVariable") :
             # Get the archive type
             dsname = self._get_parent_property(obj, "dataSetName")
             geo = self._get_parent_property(obj, "geo")
             latitude = 0
@@ -941,23 +951,23 @@
         return self.namespace + sanitizeId(objid)
     
     # Create class
     def _create_class(self, category) :
         return ONTONS + sanitizeId(category)
     
     # Create property
-    def _create_property(self, prop, dtype, cat, icon, multiple) :
+    def _create_property(self, prop, dtype, cat, multiple) :
         nsprop = prop.split(":", 2)
         ns = ONTONS
         if len(nsprop) > 1 :
             prefix = nsprop[0]
             if prefix in NAMESPACES:
                 ns = NAMESPACES[prefix]
             prop = nsprop[1]
-        return [ ns + lcfirst(sanitizeId(prop)), dtype ]
+        return [ ns + lcfirst(sanitizeId(prop)), dtype, cat, multiple ]
     
     # Set individual classes
     def _set_individual_classes(self, objid, category, extracats) :
         if objid and category:
             self.graph.add((
                 URIRef(objid),
                 RDF.type,
@@ -970,21 +980,21 @@
                     URIRef(objid),
                     RDF.type,
                     URIRef(self._create_class(ecat)),
                     URIRef(self.graphurl)
                 ))
     
     # Set property value
-    def _set_property( self, objid, prop, value ):
+    def _set_property_value( self, objid, prop, value ):
         if (type(value) is list) :
             for subvalue in value : 
-                self._set_property(objid, prop, subvalue)
+                self._set_property_value(objid, prop, subvalue)
             return
 
-        (propid, dtype) = prop
+        (propid, dtype, cat, multiple) = prop
         if objid and value:
             objitem = None
 
             if dtype == "float" or dtype == "integer":
                 if re.search("^.*[^a-zA-Z]?nan[^a-zA-Z]?.*$", str(value).lower()):
                     return
                 if re.search("^.*[^a-zA-Z]?na[^a-zA-Z]?.*$", str(value).lower()):
@@ -1018,14 +1028,20 @@
             
             elif dtype == "List":
                 objitem = value
             
             else:
                 objitem = Literal(value, datatype=(XSD[dtype] if dtype in XSD else None))
 
+            # FIXME: Do not add if property doesn't allow multiple values and a value already exists
+            if not multiple:
+                existing = list(self.graph.triples((URIRef(objid), URIRef(propid), None)))
+                if len(existing) > 0:
+                    return
+            
             self.graph.add((
                 URIRef(objid),
                 URIRef(propid),
                 objitem,
                 URIRef(self.graphurl)
             ))
     
@@ -1051,44 +1067,43 @@
         for key,value in obj.items() :
             if (key[0] == "@") :
                 continue
             
             details = self._get_property_details(key, schema, value)
             prop = details["name"]
             dtype = details["type"]
-            icon =  details["icon"] if ("icon" in details) else None
             cat =  details["category"] if ("category" in details) else None
             sch =  details["schema"] if ("schema" in details) else None
             if (sch and not cat) :
                 cat = sch
             
             fromJson =  details["fromJson"] if ("fromJson" in details) else None
             multiple =  details["multiple"] if ("multiple" in details) else False
             subobject =  details["subobject"] if ("subobject" in details) else False
             if (not prop) :
                 continue
                 
             # Create Property
-            propDI = self._create_property(prop, dtype, cat, icon, multiple)
+            propDI = self._create_property(prop, dtype, cat, multiple)
 
             # Set property value
             if (dtype == "Individual" or type(value) is dict) :
-                self._set_property(objid, propDI, value)
+                self._set_property_value(objid, propDI, value)
             else : 
                 if (dtype == "File") :
                     # Enable this ?
                     """
                     fileid = uploadFile(value)
                     if (fileid) :
                         protectIndividual(fileid)
                         data = set_property(data, propDI, fileid)
                     """
 
                 else : 
-                    self._set_property(objid, propDI, value)
+                    self._set_property_value(objid, propDI, value)
 
     def _find_files_with_extension(self, directory, extension):
         myregexobj = re.compile('\.'+extension+'$')
         try: 
             for entry in os.scandir(directory):
                 if entry.is_file() and myregexobj.search(entry.path): 
                     yield entry.path, entry.name
```

### Comparing `pylipd-1.0.6/pylipd/multi_processing.py` & `pylipd-1.1.0/pylipd/multi_processing.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.0.6/pylipd/rdf_to_lipd.py` & `pylipd-1.1.0/pylipd/rdf_to_lipd.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 """
 The RDFToLiPD class helps in converting an RDF Graph to a LiPD file.
 It uses the SCHEMA dictionary (from globals/schema.py) to do the conversion
 """
 
 import copy
+import os
 import re
+import csv
+import bagit
 import json
+import tempfile
+import zipfile
 
 from rdflib.graph import ConjunctiveGraph, URIRef
 
 from .globals.urls import NSURL
 from .globals.blacklist import REVERSE_BLACKLIST
 from .globals.schema import SCHEMA
 
@@ -21,44 +26,171 @@
     It uses the SCHEMA dictionary (from globals/schema.py) to do the conversion
 
     Parameters
     ----------
     collection_id : str
         (Optional) set a collection id for the lipd file    
     """    
-    def __init__(self, collection_id=None):
-        self.graph = ConjunctiveGraph()
+    def __init__(self, graph, collection_id=None):
+        self.graph = graph
         self.lipd_csvs = {}
         self.collection_id = collection_id
         self.graphurl = NSURL
         self.namespace = NSURL + "#"
         if self.collection_id:
             self.namespace = NSURL + "/" + collection_id + "#"
 
-    def convert(self, id, graph):
-        '''Convert RDF graph to LiPD json
+    def convert(self, dsname, lipdfile):
+        '''Convert RDF graph to a LiPD file
+
+        Parameters
+        ----------
+
+        graph : rdflib.ConjunctiveGraph
+            the RDF graph object
+
+        '''
+        lipd = self.convert_to_json(dsname)
+
+        with tempfile.TemporaryDirectory(prefix="rdf_to_lipd_") as tmpdir:
+            # Create a temporary data directory
+            datadir = f"{tmpdir}/{dsname}"
+            os.makedirs(datadir)
+
+            # Create the csv files and metadata jsonld
+            self._create_csvs(lipd, datadir)
+            with(open(f"{datadir}/metadata.jsonld", "w")) as f:
+                json.dump(lipd, f, indent=4, default=str)
+            
+            # Convert data directory to a bag
+            bagit.make_bag(datadir, checksums=['md5'])
+
+            # Zip the bag
+            self._zip_directory(datadir, lipdfile)
+
+        return lipd
+
+    def convert_to_json(self, dsname):
+        '''Convert RDF graph to a LiPD file
 
         Parameters
         ----------
 
         graph : rdflib.ConjunctiveGraph
             the RDF graph object
 
         '''
-        self.graph = graph
         self.schema = copy.deepcopy(SCHEMA)
         self.rschema = self._get_schema_reverse_map()
 
         self.allfacts = {}
-        self._get_indexed_facts(self.namespace + id)
+        self._get_indexed_facts(self.namespace + dsname)
         
-        lipd = self._convert_to_lipd(self.namespace + id, "Dataset", "Dataset", pagesdone=[])
+        lipd = self._convert_to_lipd(self.namespace + dsname, "Dataset", "Dataset", pagesdone={})
         lipd = self._post_processing(lipd)
         return lipd
 
+    def _get_table_data(self, table):
+        csvdata = []
+        numrows = 0
+        
+        table["columns"] = sorted(table["columns"], key=lambda x: x["number"] if ("number" in x and type(x["number"]) is int) else 99999)
+
+        for col in table["columns"]:
+            if "values" in col:
+                numrows = len(col["values"])
+                break
+        
+        for rowidx in range(numrows):
+            row = []
+            for col in table["columns"]:
+                if "values" in col:
+                    colindices = []
+                    if "number" in col:
+                        colnum = col["number"]
+                        colindices.append(colnum)
+                    else:
+                        colindices.append(1)
+                    
+                    for colindex in colindices:
+                        if type(colindex) is list:
+                            sorted(colindex)
+                            firstidx = colindex[0]
+                            for subindex in colindex:
+                                idx = subindex - 1
+                                if idx >= len(row):
+                                    row.extend([""] * (idx - len(row) + 1))
+                                row[idx] = col["values"][rowidx][subindex-firstidx]
+
+                        else:
+                            idx = colindex - 1
+                            if idx >= len(row):
+                                row.extend([""] * (idx - len(row) + 1))
+                            row[idx] = col["values"][rowidx]
+
+            csvdata.append(row)
+
+        # Delete the values field (since we've extracted the csv data)
+        for col in table["columns"]:
+            if "values" in col:
+                del col["values"]
+
+        return csvdata
+    
+    def _create_csvs(self, lipd, datadir):
+        csvs = {}
+        datakeys = ["paleoData", "chronData"]
+        for datakey in datakeys:
+            if datakey in lipd:
+                for data in lipd[datakey]:
+                    if "measurementTable" in data:
+                        for table in data["measurementTable"]:
+                            csvs[table["filename"]] = self._get_table_data(table)
+                    if "model" in data:
+                        for model in data["model"]:
+                            if "ensembleTable" in model:
+                                for table in model["ensembleTable"]:
+                                    csvs[table["filename"]] = self._get_table_data(table)
+                            if "summaryTable" in model:
+                                for table in model["summaryTable"]:
+                                    csvs[table["filename"]] = self._get_table_data(table)
+
+        for csvname, csvdata in csvs.items():
+            # writing to csv file 
+            with open(f"{datadir}/{csvname}", 'w') as csvfile: 
+                csvwriter = csv.writer(csvfile) 
+                csvwriter.writerows(csvdata)
+
+
+    def _zip_directory(self, datadir, lipdfile):
+        # Zip the bag
+        with zipfile.ZipFile(lipdfile, 'w') as zipf:
+            for root, dirs, files in os.walk(datadir):
+                for file in files:
+                    zipf.write(os.path.join(root, file), os.path.relpath(os.path.join(root, file), os.path.join(datadir, '..')))
+
+    '''
+    def _zip_lipd_dir(self, lipddir, lipdfile):
+        if lipdfile.startswith("http"):
+            # If this is a URL
+            # Handle special characters in url (if any)
+            res = urlparse(lipdfile)
+            lipdurl = urlunparse(res._replace(path=quote(res.path)))
+
+            # Open url and unzip
+            resp = urlopen(lipdurl)
+            with zipfile.ZipFile(BytesIO(resp.read())) as zip_ref:
+                zip_ref.extractall(unzipdir)
+        else:
+            # If this is a local file
+            # Unzip file
+            with zipfile.ZipFile(lipdfile, 'r') as zip_ref:
+                zip_ref.extractall(unzipdir)
+    '''
+    
     def _get_property_details(self, pname, schema) :
         details = { "name": pname }
         # Create property
         if schema and (pname in schema) :
             for skey,svalue in schema[pname].items() :
                 details[skey] = svalue
         return details
@@ -142,21 +274,20 @@
         for pname, pfacts in facts.items():
             for pfact in pfacts:
                 if pfact["@type"] == "uri":
                     if pname != "type":
                         self._get_indexed_facts(pfact["@id"])
 
 
-    def _convert_to_lipd(self, id, category, schemaname, pagesdone=[]) :
+    def _convert_to_lipd(self, id, category, schemaname, pagesdone={}) :
         if id in self.allfacts:
             facts = self.allfacts[id]
 
             if id in pagesdone:
-                return {}
-            pagesdone.append(id)
+                return pagesdone[id]
             
             schema =  self.rschema[schemaname] if (schemaname in self.rschema) else None
             if (schemaname and not category) :
                 category = schemaname
             
             if "type" in facts:
                 cats = facts["type"]
@@ -167,14 +298,16 @@
             
             obj = {
                 "@id":id,
                 "@category":category,
                 "@schema":schemaname
             }
 
+            pagesdone[id] = obj
+
             for pname, pfacts in facts.items() :
                 if pname in REVERSE_BLACKLIST:
                     continue
                 prop = pname
                 prop = re.sub("/\\s/", "_", prop)
                 # Get a sample value page category, and use to make a property key
                 propkey = prop
@@ -210,60 +343,63 @@
                             val = self._convert_to_lipd(pfact["@id"], cat, sch, pagesdone)
                         else:
                             val = pfact["@value"]
                         
                         if (toJson) :
                             fn = getattr(self, toJson)
                             val = fn(val)
-                        
-                        # TODO: Handle hasValues :: Convert to File ?
-                        
+                                                
                         # If there is already a value present
                         # - Then this need to be marked as "multiple"
                         if (not multiple) and (name in obj) and (not type(obj[name]) is list):
                             multiple = True
                             obj[name] = [obj[name]]
                         
                         if (multiple) :
                             obj[name].append(val)
                         else : 
                             obj[name] = val
 
-            # TODO: Fix the empty case ?
-            #if (empty(Settlement.array_keys([obj]))) :
-            #    return preg_replace("/_/", " ", id)
-            
             return obj
         else : 
             return re.sub("/_/", " ", id)
 
 
     def _post_processing(self, obj, parent=None):
         if not(type(obj) is dict):
             return obj
 		
         if not("@schema" in obj):
             return obj
 
+        # FIXME: Hack to avoid recursion
+        schemaname = obj["@schema"]
+        tschema = self.schema[schemaname] if schemaname in self.schema else None
+
+        if tschema and "@toJson_pre" in tschema:
+            for func in tschema["@toJson_pre"]:
+                fn = getattr(self, func)
+                obj = fn(obj, parent)        
+
         for key,value in obj.items():
             if type(value) is list:
                 for i in range(len(value)):
                     obj[key][i] = self._post_processing(value[i], obj)
             else:
                 obj[key] = self._post_processing(value, obj)
 
-        schemaname = obj["@schema"]
-        tschema = self.schema[schemaname] if schemaname in self.schema else None
         if tschema and "@toJson" in tschema:
             for func in tschema["@toJson"]:
                 fn = getattr(self, func)
                 obj = fn(obj, parent)
 
+        # FIXME: Only remove hasValues.. LiPD CSVs should be created outside this function beforehand
         if "hasValues" in obj:
-            obj["values"] = json.loads(obj["hasValues"])
+            valuestr = obj["hasValues"]
+            obj["values"] = json.loads(valuestr)
             del obj["hasValues"]
         
         del obj["@id"]
         del obj["@schema"]
         del obj["@category"]
         if "type" in obj:
             del obj["type"] 
@@ -305,25 +441,27 @@
                 if prop == "coordinates" or prop == "coordinatesFor":
                     # Ignore
                     pass
                 else : 
                     if re.search(r"^(geo|wgs84):", prop) :
                         # Ignore
                         pass
+                    elif prop in ["long", "lat", "alt"] :
+                        pass
                     else : 
                         geojson["properties"][prop] = value
         
         return geojson
 
 
     def _get_google_spreadsheet_key(self, url:str, parent = None) :
         return url.replace("https://docs.google.com/spreadsheets/d/", "")
 
     def _remove_found_in_table(self, var, parent = None) :
-        if (("foundInTable" in var)) :
+        if "foundInTable" in var :
             del var["foundInTable"]
         return var
 
     def __get_variable_archive_types(self, item, atypes) :
         if type(item) is dict:
             nitem = {}
             for key,value in item.items() :
@@ -421,15 +559,15 @@
             var["variableType"] = "measured"
         
         if (var["@category"] == "InferredVariable") :
             var["variableType"] = "inferred"
         return var
 
     def _remove_depth_property(self, val, parent = None) :
-        if (("takenAtDepth" in val)) :
+        if "takenAtDepth" in val :
             del val["takenAtDepth"]
         return val
 
     def _create_publication_identifier(self, pub, parent = None) :
         identifiers = []
         if (("hasDOI" in pub)) :
             identifier = {}
@@ -466,12 +604,13 @@
             var["number"] = var["number"][0]
         if ("number" in var) and (type(var["number"]) is str) :
             var["number"] = json.loads(var["number"])
         return var
 
     def _extract_variable_values(self, var, parent = None) :
         if "hasValues" in var:
-            values = json.loads(var["hasValues"])
+            valuestr = var["hasValues"]
+            values = json.loads(valuestr)
             if type(values) is dict and "base64_zlib" in values:
                 values = unzip_string(values["base64_zlib"])
                 var["hasValues"] = values
         return var
```

### Comparing `pylipd-1.0.6/pylipd/series/regexes.py` & `pylipd-1.1.0/pylipd/series/regexes.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.0.6/pylipd/test.py` & `pylipd-1.1.0/pylipd/test.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.0.6/pylipd/usage.py` & `pylipd-1.1.0/pylipd/usage.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 from pylipd.lipd import LiPD
+import json
 from pylipd.multi_processing import convert_to_rdf
 
 ####################
 # TODO:
 # - Edit local LiPD & update endpoint
 ####################
 
 
 local_lipd_dir = "/Users/varun/git/LiPD/PyLiPD/data/lpd.latest"
 remote_lipd_endpoint = "https://linkedearth.graphdb.mint.isi.edu/repositories/LiPDVerse2"
 
-url = 'https://lipdverse.org/data/RRh3T4NCsf4MgrxhXbJq/1_0_0//Ocn-Philippines.Stott.2007.lpd'
-        
-lipd = LiPD()
-lipd.load(url)
-ts_list=lipd.get_timeseries(lipd.get_all_dataset_names())
-
-exit()
-
 '''
 lipd = LiPD()
 # Convert LiPD files to RDF    
 lipd.convert_lipd_dir_to_rdf(
     local_lipd_dir,
     local_lipd_dir+".nq", 
     parallel=False)
@@ -69,46 +62,79 @@
 '''
 
 # Load from local
 lipd = LiPD()
 lipdfiles = [local_lipd_dir + "/" + dsname + ".lpd" for dsname in dsnames]
 #print(lipdfiles)
 
-lipd.load(lipdfiles)
-#lipd.load_from_dir(local_lipd_dir)
+#lipd.load(lipdfiles)
+#lipd.load_from_dir("examples/data")
+lipd.load(["/Users/varun/Downloads/ODP846.Lawrence.2006.lpd"])
 print(lipd.get_all_dataset_names())
 print(lipd.get_all_dataset_ids())
 
 #lipd.load(["/Users/varun/Downloads/Arc-LakeNataujärvi.Ojala.2005.lpd"])
 #print(lipd.get_all_dataset_names())
 
 ts_list = lipd.get_timeseries(lipd.get_all_dataset_names())
 for dsname, tsos in ts_list.items():
     for tso in tsos:
         if 'paleoData_variableName' in tso:
-            print(dsname+': '+tso['paleoData_variableName']+': '+tso['archiveType'])
+            print(dsname+': '+str(tso['paleoData_variableName'])+': '+tso['archiveType'])
 
 
 # Fetch LiPD data from remote RDF Graph
 lipd.set_endpoint(remote_lipd_endpoint)
-lipd.load_remote_datasets(remote_dsnames)
+#lipd.load_remote_datasets(remote_dsnames)
 
 # Convert to TSO object (as before)
+'''
 ts_list_remote = lipd.get_timeseries(lipd.get_all_dataset_names())
 for dsname, tsos in ts_list_remote.items():
     for tso in tsos:
-        print(dsname+': '+tso['paleoData_variableName']+': '+tso['archiveType'])
+        print(dsname+': '+str(tso['paleoData_variableName'])+': '+tso['archiveType'])
+'''
+
+print("Popping ...")
+poplipd = lipd.pop(lipd.get_all_dataset_names()[0])
+
+print("Creating separate lipd file for popped")
+dsname = poplipd.get_all_dataset_names()[0]
+lipdfile = f"{dsname}.lpd"
+poplipd.create_lipd(dsname, lipdfile)
+
+print("Loading .. created lipd file: "+lipdfile)
+lpd2 = LiPD()
+lpd2.load([lipdfile])
+ts_list_remote = lpd2.get_timeseries(lpd2.get_all_dataset_names())
+for dsname, tsos in ts_list_remote.items():
+    for tso in tsos:
+        print(dsname+': '+str(tso['paleoData_variableName'])+': '+tso['archiveType'])
+
+exit()
 
-print(lipd.get_all_dataset_names())
-poplipd = lipd.pop(remote_dsnames[0])
 print("After popping..")
 print(lipd.get_all_dataset_names())
+ts_list_remote = lipd.get_timeseries(lipd.get_all_dataset_names())
+for dsname, tsos in ts_list_remote.items():
+    for tso in tsos:
+        print(dsname+': '+str(tso['paleoData_variableName'])+': '+tso['archiveType'])
+
 print("Popped..")
 print(poplipd.get_all_dataset_names())
 
+print("Merging back..")
+mergelipd = lipd.merge(poplipd)
+print(mergelipd.get_all_dataset_names())
+
+ts_list_remote = mergelipd.get_timeseries(mergelipd.get_all_dataset_names())
+for dsname, tsos in ts_list_remote.items():
+    for tso in tsos:
+        print(dsname+': '+str(tso['paleoData_variableName'])+': '+tso['archiveType'])
+
 '''
 print(lipd.get_all_dataset_names())    
 datasets = lipd.get_datasets(dsnames=dsnames)
 print("Fetched..")
 for ds in datasets:
     print(ds['id'])
     #print(json.dumps(ds, indent=3))
```

### Comparing `pylipd-1.0.6/pylipd/utils.py` & `pylipd-1.1.0/pylipd/utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.0.6/pylipd.egg-info/PKG-INFO` & `pylipd-1.1.0/pylipd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.0.6
+Version: 1.1.0
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.0.6
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.1.0
 Author: Varun Ratnakar
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pylipd-1.0.6/pylipd.egg-info/SOURCES.txt` & `pylipd-1.1.0/pylipd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylipd-1.0.6/setup.cfg` & `pylipd-1.1.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pylipd
-version = 1.0.6
+version = 1.1.0
 author = Varun Ratnakar
 author_email = varunratnakar@gmail.com
 description = Python utilities for handling LiPD data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/linkedearth/pylipd
 project_urls = 
@@ -20,14 +20,15 @@
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	rdflib
 	pandas
 	doi2bib
 	pybtex
+	bagit
 
 [options.packages.find]
 where = .
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pylipd-1.0.6/setup.py` & `pylipd-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import setup, find_packages
 
 
-version = '1.0.6'
+version = '1.1.0'
 
 # Read the readme file contents into variable
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='pylipd',
@@ -26,11 +26,12 @@
     keywords=['Paleoclimate, Data Analysis, LiPD'],
     package_dir = {'':'.'},
     classifiers=[],
     install_requires=[
         "rdflib",
         "pandas",
         "doi2bib",
-        "pybtex"
+        "pybtex",
+        "bagit"
     ],
     python_requires=">=3.9.0"
 )
```


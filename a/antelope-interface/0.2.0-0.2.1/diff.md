# Comparing `tmp/antelope_interface-0.2.0.tar.gz` & `tmp/antelope_interface-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antelope_interface-0.2.0.tar", last modified: Fri Apr  7 05:30:14 2023, max compression
+gzip compressed data, was "antelope_interface-0.2.1.tar", last modified: Mon Apr 10 21:38:40 2023, max compression
```

## Comparing `antelope_interface-0.2.0.tar` & `antelope_interface-0.2.1.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:14.609516 antelope_interface-0.2.0/
--rw-r--r--   0 b          (500) b          (506)     1520 2020-05-28 23:57:28.000000 antelope_interface-0.2.0/LICENSE
--rw-r--r--   0 b          (500) b          (506)       44 2022-04-09 17:53:58.000000 antelope_interface-0.2.0/MANIFEST.in
--rw-r--r--   0 b          (500) b          (506)     1617 2023-04-07 05:30:14.609516 antelope_interface-0.2.0/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)     1013 2020-12-30 20:52:39.000000 antelope_interface-0.2.0/README.md
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:14.606182 antelope_interface-0.2.0/antelope/
--rw-r--r--   0 b          (500) b          (506)     7381 2023-02-06 20:32:15.000000 antelope_interface-0.2.0/antelope/__init__.py
--rw-r--r--   0 b          (500) b          (506)     7128 2022-06-11 08:41:11.000000 antelope_interface-0.2.0/antelope/exchanges_from_spreadsheet.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:14.606182 antelope_interface-0.2.0/antelope/flows/
--rw-r--r--   0 b          (500) b          (506)       89 2022-12-31 00:07:14.000000 antelope_interface-0.2.0/antelope/flows/__init__.py
--rw-r--r--   0 b          (500) b          (506)     8689 2023-03-29 01:31:42.000000 antelope_interface-0.2.0/antelope/flows/flow.py
--rw-r--r--   0 b          (500) b          (506)     3751 2022-12-31 00:07:14.000000 antelope_interface-0.2.0/antelope/flows/flow_interface.py
--rw-r--r--   0 b          (500) b          (506)    13903 2022-04-09 17:53:58.000000 antelope_interface-0.2.0/antelope/flows/openlca_locales.json
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:14.606182 antelope_interface-0.2.0/antelope/interfaces/
--rw-r--r--   0 b          (500) b          (506)      111 2020-09-25 19:28:16.000000 antelope_interface-0.2.0/antelope/interfaces/__init__.py
--rw-r--r--   0 b          (500) b          (506)     3307 2023-03-30 22:44:53.000000 antelope_interface-0.2.0/antelope/interfaces/abstract_query.py
--rw-r--r--   0 b          (500) b          (506)    10849 2023-04-05 15:49:48.000000 antelope_interface-0.2.0/antelope/interfaces/ibackground.py
--rw-r--r--   0 b          (500) b          (506)     4333 2020-09-24 22:08:18.000000 antelope_interface-0.2.0/antelope/interfaces/iconfigure.py
--rw-r--r--   0 b          (500) b          (506)     5947 2022-12-31 00:07:14.000000 antelope_interface-0.2.0/antelope/interfaces/iexchange.py
--rw-r--r--   0 b          (500) b          (506)     6797 2022-12-31 00:07:14.000000 antelope_interface-0.2.0/antelope/interfaces/iforeground.py
--rw-r--r--   0 b          (500) b          (506)     7077 2021-10-30 03:46:20.000000 antelope_interface-0.2.0/antelope/interfaces/iindex.py
--rw-r--r--   0 b          (500) b          (506)    15250 2023-01-12 06:14:41.000000 antelope_interface-0.2.0/antelope/interfaces/iquantity.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:14.609516 antelope_interface-0.2.0/antelope/refs/
--rw-r--r--   0 b          (500) b          (506)       81 2022-04-09 17:53:58.000000 antelope_interface-0.2.0/antelope/refs/__init__.py
--rw-r--r--   0 b          (500) b          (506)    13561 2023-01-07 00:12:58.000000 antelope_interface-0.2.0/antelope/refs/base.py
--rw-r--r--   0 b          (500) b          (506)     4326 2022-01-22 08:03:17.000000 antelope_interface-0.2.0/antelope/refs/catalog_ref.py
--rw-r--r--   0 b          (500) b          (506)     8254 2022-04-09 17:53:58.000000 antelope_interface-0.2.0/antelope/refs/exchange_ref.py
--rw-r--r--   0 b          (500) b          (506)     4753 2022-04-09 17:53:58.000000 antelope_interface-0.2.0/antelope/refs/flow_ref.py
--rw-r--r--   0 b          (500) b          (506)    11560 2023-04-05 08:50:18.000000 antelope_interface-0.2.0/antelope/refs/process_ref.py
--rw-r--r--   0 b          (500) b          (506)     8662 2023-02-06 20:32:15.000000 antelope_interface-0.2.0/antelope/refs/quantity_ref.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:14.609516 antelope_interface-0.2.0/antelope/refs/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2022-04-09 17:53:58.000000 antelope_interface-0.2.0/antelope/refs/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     1150 2022-04-09 17:53:58.000000 antelope_interface-0.2.0/antelope/refs/tests/test_flows.py
--rw-r--r--   0 b          (500) b          (506)     4605 2023-01-11 06:29:16.000000 antelope_interface-0.2.0/antelope/xdb_tokens.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-07 05:30:14.609516 antelope_interface-0.2.0/antelope_interface.egg-info/
--rw-r--r--   0 b          (500) b          (506)     1617 2023-04-07 05:30:14.000000 antelope_interface-0.2.0/antelope_interface.egg-info/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)      977 2023-04-07 05:30:14.000000 antelope_interface-0.2.0/antelope_interface.egg-info/SOURCES.txt
--rw-r--r--   0 b          (500) b          (506)        1 2023-04-07 05:30:14.000000 antelope_interface-0.2.0/antelope_interface.egg-info/dependency_links.txt
--rw-r--r--   0 b          (500) b          (506)       36 2023-04-07 05:30:14.000000 antelope_interface-0.2.0/antelope_interface.egg-info/requires.txt
--rw-r--r--   0 b          (500) b          (506)        9 2023-04-07 05:30:14.000000 antelope_interface-0.2.0/antelope_interface.egg-info/top_level.txt
--rw-r--r--   0 b          (500) b          (506)       38 2023-04-07 05:30:14.609516 antelope_interface-0.2.0/setup.cfg
--rw-r--r--   0 b          (500) b          (506)     2437 2023-04-06 23:21:36.000000 antelope_interface-0.2.0/setup.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:38:40.243899 antelope_interface-0.2.1/
+-rw-r--r--   0 b          (500) b          (506)     1520 2020-05-28 23:57:28.000000 antelope_interface-0.2.1/LICENSE
+-rw-r--r--   0 b          (500) b          (506)       44 2022-04-09 17:53:58.000000 antelope_interface-0.2.1/MANIFEST.in
+-rw-r--r--   0 b          (500) b          (506)     1617 2023-04-10 21:38:40.243899 antelope_interface-0.2.1/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)     1013 2020-12-30 20:52:39.000000 antelope_interface-0.2.1/README.md
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:38:40.243899 antelope_interface-0.2.1/antelope/
+-rw-r--r--   0 b          (500) b          (506)     7381 2023-02-06 20:32:15.000000 antelope_interface-0.2.1/antelope/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     7128 2022-06-11 08:41:11.000000 antelope_interface-0.2.1/antelope/exchanges_from_spreadsheet.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:38:40.243899 antelope_interface-0.2.1/antelope/flows/
+-rw-r--r--   0 b          (500) b          (506)       89 2022-12-31 00:07:14.000000 antelope_interface-0.2.1/antelope/flows/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     8689 2023-04-07 06:23:50.000000 antelope_interface-0.2.1/antelope/flows/flow.py
+-rw-r--r--   0 b          (500) b          (506)     3751 2022-12-31 00:07:14.000000 antelope_interface-0.2.1/antelope/flows/flow_interface.py
+-rw-r--r--   0 b          (500) b          (506)    13903 2022-04-09 17:53:58.000000 antelope_interface-0.2.1/antelope/flows/openlca_locales.json
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:38:40.243899 antelope_interface-0.2.1/antelope/interfaces/
+-rw-r--r--   0 b          (500) b          (506)      111 2020-09-25 19:28:16.000000 antelope_interface-0.2.1/antelope/interfaces/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     3307 2023-04-10 05:50:06.000000 antelope_interface-0.2.1/antelope/interfaces/abstract_query.py
+-rw-r--r--   0 b          (500) b          (506)    10480 2023-04-10 06:01:03.000000 antelope_interface-0.2.1/antelope/interfaces/ibackground.py
+-rw-r--r--   0 b          (500) b          (506)     4333 2020-09-24 22:08:18.000000 antelope_interface-0.2.1/antelope/interfaces/iconfigure.py
+-rw-r--r--   0 b          (500) b          (506)     5947 2023-04-08 00:18:01.000000 antelope_interface-0.2.1/antelope/interfaces/iexchange.py
+-rw-r--r--   0 b          (500) b          (506)     6797 2022-12-31 00:07:14.000000 antelope_interface-0.2.1/antelope/interfaces/iforeground.py
+-rw-r--r--   0 b          (500) b          (506)     7077 2021-10-30 03:46:20.000000 antelope_interface-0.2.1/antelope/interfaces/iindex.py
+-rw-r--r--   0 b          (500) b          (506)    15438 2023-04-10 21:02:48.000000 antelope_interface-0.2.1/antelope/interfaces/iquantity.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:38:40.243899 antelope_interface-0.2.1/antelope/models/
+-rw-r--r--   0 b          (500) b          (506)    16203 2023-04-08 00:29:06.000000 antelope_interface-0.2.1/antelope/models/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     4223 2023-04-07 19:23:32.000000 antelope_interface-0.2.1/antelope/models/auth.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:38:40.243899 antelope_interface-0.2.1/antelope/refs/
+-rw-r--r--   0 b          (500) b          (506)       81 2022-04-09 17:53:58.000000 antelope_interface-0.2.1/antelope/refs/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    13561 2023-01-07 00:12:58.000000 antelope_interface-0.2.1/antelope/refs/base.py
+-rw-r--r--   0 b          (500) b          (506)     4326 2022-01-22 08:03:17.000000 antelope_interface-0.2.1/antelope/refs/catalog_ref.py
+-rw-r--r--   0 b          (500) b          (506)     8254 2022-04-09 17:53:58.000000 antelope_interface-0.2.1/antelope/refs/exchange_ref.py
+-rw-r--r--   0 b          (500) b          (506)     4753 2022-04-09 17:53:58.000000 antelope_interface-0.2.1/antelope/refs/flow_ref.py
+-rw-r--r--   0 b          (500) b          (506)    11808 2023-04-10 20:48:27.000000 antelope_interface-0.2.1/antelope/refs/process_ref.py
+-rw-r--r--   0 b          (500) b          (506)     8662 2023-02-06 20:32:15.000000 antelope_interface-0.2.1/antelope/refs/quantity_ref.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:38:40.243899 antelope_interface-0.2.1/antelope/refs/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2022-04-09 17:53:58.000000 antelope_interface-0.2.1/antelope/refs/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     1150 2022-04-09 17:53:58.000000 antelope_interface-0.2.1/antelope/refs/tests/test_flows.py
+-rw-r--r--   0 b          (500) b          (506)     4605 2023-01-11 06:29:16.000000 antelope_interface-0.2.1/antelope/xdb_tokens.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2023-04-10 21:38:40.243899 antelope_interface-0.2.1/antelope_interface.egg-info/
+-rw-r--r--   0 b          (500) b          (506)     1617 2023-04-10 21:38:40.000000 antelope_interface-0.2.1/antelope_interface.egg-info/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)     1029 2023-04-10 21:38:40.000000 antelope_interface-0.2.1/antelope_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 b          (500) b          (506)        1 2023-04-10 21:38:40.000000 antelope_interface-0.2.1/antelope_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 b          (500) b          (506)       36 2023-04-10 21:38:40.000000 antelope_interface-0.2.1/antelope_interface.egg-info/requires.txt
+-rw-r--r--   0 b          (500) b          (506)        9 2023-04-10 21:38:40.000000 antelope_interface-0.2.1/antelope_interface.egg-info/top_level.txt
+-rw-r--r--   0 b          (500) b          (506)       38 2023-04-10 21:38:40.243899 antelope_interface-0.2.1/setup.cfg
+-rw-r--r--   0 b          (500) b          (506)     2625 2023-04-10 21:38:30.000000 antelope_interface-0.2.1/setup.py
```

### Comparing `antelope_interface-0.2.0/LICENSE` & `antelope_interface-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.0/PKG-INFO` & `antelope_interface-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antelope_interface
-Version: 0.2.0
+Version: 0.2.1
 Home-page: https://github.com/AntelopeLCA/antelope
 Author: Brandon Kuczenski
 Author-email: bkuczenski@ucsb.edu
 License: BSD 3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `antelope_interface-0.2.0/README.md` & `antelope_interface-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.0/antelope/__init__.py` & `antelope_interface-0.2.1/antelope/__init__.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.0/antelope/exchanges_from_spreadsheet.py` & `antelope_interface-0.2.1/antelope/exchanges_from_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.0/antelope/flows/flow.py` & `antelope_interface-0.2.1/antelope/flows/flow.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.0/antelope/flows/flow_interface.py` & `antelope_interface-0.2.1/antelope/flows/flow_interface.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.0/antelope/flows/openlca_locales.json` & `antelope_interface-0.2.1/antelope/flows/openlca_locales.json`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.0/antelope/interfaces/abstract_query.py` & `antelope_interface-0.2.1/antelope/interfaces/abstract_query.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.0/antelope/interfaces/ibackground.py` & `antelope_interface-0.2.1/antelope/interfaces/ibackground.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 The (as yet hypothetical) antelope_brightway2 plugin can provide index, inventory, and background data for a bw2
 database.
 
 More plugins are yet imagined.
 """
 
 from .abstract_query import AbstractQuery
+from ..refs import ExchangeRef
 from itertools import chain
 
 
 class BackgroundRequired(Exception):
     pass
 
 
@@ -130,60 +131,51 @@
         :param process:
         :param ref_flow:
         :return:
         """
         return self._perform_query(_interface, 'lci', BackgroundRequired,
                                    process, ref_flow=ref_flow, **kwargs)
 
+    def _make_sys_lci_exchange(self, x):
+        return ExchangeRef(self.get(x.process), self.make_ref(x.flow), x.direction, value=x.value,
+                           termination=x.termination, comment='SYS LCI', is_reference=False)
+
     def sys_lci(self, demand, **kwargs):
         """
-        Perform LCI on an arbitrary demand vector, which should be supplied as an iterable of exchanges whose
-        terminations can be found in the background database.
+        Perform LCI on an arbitrary demand vector, which should be supplied as an iterable of UnallocatedExchange
+        models whose terminations can be found in the background database.
 
-        Terminations to foreground, background, and exterior flows are allowed.
+        Terminations to foreground and background are allowed. Exterior flows are just passed through but contexts
+        may be transformed in the process and thus should be excluded.  See bg_lcia() for recommended implementation.
 
         sys_lci(process_ref.dependencies()) + process_ref.emissions() should equal process_ref.lci()
         although the sum of iterables would not be straightforward to compute... the correct approach is:
         sys_lci(itertools.chain(process_ref.dependencies(), process_ref.emissions(), process_ref.cutoffs()))
 
         sys_lci(process_ref.inventory()) should equal process_ref.lci() directly, up to a normalization, assuming
         the individual exchanges are properly terminated.
         :param demand: an iterable of exchanges with terminations that can be found in the background database.
         :param kwargs:
         :return:
         """
-        return self._perform_query(_interface, 'sys_lci', BackgroundRequired,
-                                   demand, **kwargs)
+        for i in self._perform_query(_interface, 'sys_lci', BackgroundRequired, demand, **kwargs):
+            yield self._make_sys_lci_exchange(i)
 
     def bg_lcia(self, process, query_qty, observed=None, ref_flow=None, **kwargs):
         """
-        returns an LciaResult object, aggregated as appropriate depending on the interface's privacy level.
-        This is an ensemble function that stitches together bg functions with quantity access.
 
         :param process:
-        :param query_qty: must be an operable quantity_ref. the process must have exchange access
-        :param observed: iterable of DirectedFlows (flow: FlowSpec, direction: str)
+        :param query_qty:
+        :param observed:
         :param ref_flow:
         :param kwargs:
         :return:
         """
-        p_ref = self.make_ref(self.get(process))  # a ref
-        if observed is None:
-            observed = ()
-        obs = set((x.flow.external_ref, x.direction) for x in observed)
-        if len(obs) > 0:
-            inventory = chain(p_ref.dependencies(ref_flow=ref_flow),
-                              p_ref.emissions(ref_flow=ref_flow),
-                              p_ref.cutoffs(ref_flow=ref_flow))
-            incl = (k for k in inventory if (k.flow.external_ref, k.direction) not in obs)
-            lci = self.sys_lci(incl)
-        else:
-            lci = p_ref.lci(ref_flow=ref_flow)
-        # aggregation
-        return query_qty.do_lcia(lci, **kwargs)
+        return self._perform_query(_interface, 'bg_lcia', BackgroundRequired,
+                                   process, query_qty, observed=observed, ref_flow=ref_flow, **kwargs)
 
     '''
     Methods requiring a partial ordering (implemented by antelope_background)
     '''
     def foreground_flows(self, search=None, **kwargs):
         """
         Yield a list of Reference Exchanges that make up the foreground (e.g. rows/columns of Af).
```

### Comparing `antelope_interface-0.2.0/antelope/interfaces/iconfigure.py` & `antelope_interface-0.2.1/antelope/interfaces/iconfigure.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.0/antelope/interfaces/iexchange.py` & `antelope_interface-0.2.1/antelope/interfaces/iexchange.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.0/antelope/interfaces/iforeground.py` & `antelope_interface-0.2.1/antelope/interfaces/iforeground.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.0/antelope/interfaces/iindex.py` & `antelope_interface-0.2.1/antelope/interfaces/iindex.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.0/antelope/interfaces/iquantity.py` & `antelope_interface-0.2.1/antelope/interfaces/iquantity.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,16 @@
         """
         return self._perform_query(_interface, 'quantity_relation', QuantityRequired,
                                    flowable, ref_quantity, query_quantity, context, locale=locale, **kwargs)
 
     def do_lcia(self, quantity, inventory, locale='GLO', **kwargs):
         """
         Successively implement the quantity relation over an iterable of exchanges.
+        we should probably generalize this to automatically expect a list of results, to support running whole
+        methodologies. This is now supported in antelope_foreground and xdb.
 
         :param quantity:
         :param inventory:
         :param locale:
         :param kwargs:
         :return: an LciaResult whose components are processes encountered in the inventory
         """
```

### Comparing `antelope_interface-0.2.0/antelope/refs/base.py` & `antelope_interface-0.2.1/antelope/refs/base.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.0/antelope/refs/catalog_ref.py` & `antelope_interface-0.2.1/antelope/refs/catalog_ref.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.0/antelope/refs/exchange_ref.py` & `antelope_interface-0.2.1/antelope/refs/exchange_ref.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.0/antelope/refs/flow_ref.py` & `antelope_interface-0.2.1/antelope/refs/flow_ref.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.0/antelope/refs/process_ref.py` & `antelope_interface-0.2.1/antelope/refs/process_ref.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,16 +154,15 @@
                 flow = flow.external_ref
         for x in self._query.exchange_values(self.external_ref, flow, direction,
                                              termination=termination, reference=reference, **kwargs):
             yield self._to_exch_ref(x, value=x.values)
 
     def inventory(self, ref_flow=None, **kwargs):
         # ref_flow = self._use_ref_exch(ref_flow)  # ref_flow=None returns unallocated inventory
-        inv = [ExchangeRef(self, self._query.make_ref(x.flow), x.direction, value=x.value, termination=x.termination,
-                           comment=x.comment, is_reference=x.is_reference)
+        inv = [self._to_exch_ref(x, x.value)
                for x in self._query.inventory(self.external_ref, ref_flow=ref_flow, **kwargs)]
         return sorted(inv, key=lambda t: (not t.is_reference, t.direction, t.type == 'context', t.type == 'cutoff'))
 
     def exchange_relation(self, ref_flow, exch_flow, direction, termination=None, **kwargs):
         ref_flow = self._use_ref_exch(ref_flow)
         if hasattr(exch_flow, 'external_ref'):
             exch_flow = exch_flow.external_ref
@@ -219,35 +218,40 @@
 
     def consumers(self, ref_flow=None, **kwargs):
         ref_flow = self._use_ref_exch(ref_flow)
         return self._query.consumers(self.external_ref, ref_flow=ref_flow, **kwargs)
 
     def dependencies(self, ref_flow=None, **kwargs):
         ref_flow = self._use_ref_exch(ref_flow)
-        return self._query.dependencies(self.external_ref, ref_flow=ref_flow, **kwargs)
+        return [self._to_exch_ref(x, x.value) for x in
+                self._query.dependencies(self.external_ref, ref_flow=ref_flow, **kwargs)]
 
     def emissions(self, ref_flow=None, **kwargs):
         ref_flow = self._use_ref_exch(ref_flow)
-        return self._query.emissions(self.external_ref, ref_flow=ref_flow, **kwargs)
+        return [self._to_exch_ref(x, x.value) for x in
+                self._query.emissions(self.external_ref, ref_flow=ref_flow, **kwargs)]
 
     def cutoffs(self, ref_flow=None, **kwargs):
         ref_flow = self._use_ref_exch(ref_flow)
-        return self._query.cutoffs(self.external_ref, ref_flow=ref_flow, **kwargs)
+        return [self._to_exch_ref(x, x.value) for x in
+                self._query.cutoffs(self.external_ref, ref_flow=ref_flow, **kwargs)]
 
     def is_in_background(self, ref_flow=None, **kwargs):
         ref_flow = self._use_ref_exch(ref_flow)
         return self._query.is_in_background(self.external_ref, ref_flow=ref_flow, **kwargs)
 
     def ad(self, ref_flow=None, **kwargs):
         ref_flow = self._use_ref_exch(ref_flow)
-        return self._query.ad(self.external_ref, ref_flow, **kwargs)
+        return [self._to_exch_ref(x, x.value) for x in
+                self._query.ad(self.external_ref, ref_flow, **kwargs)]
 
     def bf(self, ref_flow=None, **kwargs):
         ref_flow = self._use_ref_exch(ref_flow)
-        return self._query.bf(self.external_ref, ref_flow, **kwargs)
+        return [self._to_exch_ref(x, x.value) for x in
+                self._query.bf(self.external_ref, ref_flow, **kwargs)]
 
     def lci(self, ref_flow=None, refresh=False, **kwargs):
         """
         Caches LCI results
         :param ref_flow:
         :param refresh:
         :param kwargs:
@@ -275,24 +279,26 @@
         more appropriate to use the combined dependencies and emissions rather than inventory.
 
         :param observed: iterable of exchanges or child flows, having a flow (with external_ref) and direction
         :param ref_flow:
         :param kwargs:
         :return:
         """
-        excl = set((k.flow.external_ref, k.direction) for k in observed)
-        if len(excl) == 0:
-            return self.lci(ref_flow=ref_flow, **kwargs)
-        ref_flow = self._use_ref_exch(ref_flow)
-        inventory = chain(self.dependencies(ref_flow=ref_flow),
-                          self.emissions(ref_flow=ref_flow),
-                          self.cutoffs(ref_flow=ref_flow))
-        incl = (k for k in inventory if (k.flow.external_ref, k.direction) not in excl)
-        for i in self._query.sys_lci(incl, **kwargs):
-            yield self._to_exch_ref(i, i.value)
+        obs = set((k.flow.external_ref, k.direction) for k in observed)
+        if len(obs) == 0:
+            yield from self.lci(ref_flow=ref_flow, **kwargs)
+        else:
+            ref_flow = self._use_ref_exch(ref_flow)
+            exts = chain(self.emissions(ref_flow=ref_flow),
+                         self.cutoffs(ref_flow=ref_flow))
+            incl = (k for k in self.dependencies(ref_flow=ref_flow) if (k.flow.external_ref, k.direction) not in obs)
+            ext = (k for k in exts if (k.flow.external_ref, k.direction) not in obs)
+            lci = chain(self._query.sys_lci(incl, **kwargs), ext)
+            for i in lci:
+                yield self._to_exch_ref(i, i.value)
 
     def bg_lcia(self, lcia_qty, observed=None, ref_flow=None, **kwargs):
         """
         :param lcia_qty: should be a quantity ref (or qty), not an external ID
         :param observed: see unobserved_lci
         :param ref_flow:
         :param kwargs:
```

### Comparing `antelope_interface-0.2.0/antelope/refs/quantity_ref.py` & `antelope_interface-0.2.1/antelope/refs/quantity_ref.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.0/antelope/refs/tests/test_flows.py` & `antelope_interface-0.2.1/antelope/refs/tests/test_flows.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.0/antelope/xdb_tokens.py` & `antelope_interface-0.2.1/antelope/xdb_tokens.py`

 * *Files identical despite different names*

### Comparing `antelope_interface-0.2.0/antelope_interface.egg-info/PKG-INFO` & `antelope_interface-0.2.1/antelope_interface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antelope-interface
-Version: 0.2.0
+Version: 0.2.1
 Home-page: https://github.com/AntelopeLCA/antelope
 Author: Brandon Kuczenski
 Author-email: bkuczenski@ucsb.edu
 License: BSD 3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `antelope_interface-0.2.0/antelope_interface.egg-info/SOURCES.txt` & `antelope_interface-0.2.1/antelope_interface.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 antelope/interfaces/abstract_query.py
 antelope/interfaces/ibackground.py
 antelope/interfaces/iconfigure.py
 antelope/interfaces/iexchange.py
 antelope/interfaces/iforeground.py
 antelope/interfaces/iindex.py
 antelope/interfaces/iquantity.py
+antelope/models/__init__.py
+antelope/models/auth.py
 antelope/refs/__init__.py
 antelope/refs/base.py
 antelope/refs/catalog_ref.py
 antelope/refs/exchange_ref.py
 antelope/refs/flow_ref.py
 antelope/refs/process_ref.py
 antelope/refs/quantity_ref.py
```

### Comparing `antelope_interface-0.2.0/setup.py` & `antelope_interface-0.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from setuptools import setup, find_packages
 
-ANTELOPE_VERSION = '0.2.0'
+ANTELOPE_VERSION = '0.2.1'
 
 requires = [
     "synonym_dict>=0.2.0",
     "pydantic>=1.8.2"
 ]
 
 """
 Version History:
+0.2.1-virtualize - 2023/04/10 xdb passes benchmarks.
+                   pydantic models moved into interface
+                   sys_lci and bg_lcia operational, both locally and remotely
+
 0.2.0-virtualize - in progress, with xdb
                    minimal complete foreground spec
                    add xdb token spec
                    
 0.1.8 2022/04/08 - Minor changes, to go along with 0.1.8 core release
  - support None in exchanges_from_spreadsheet (this will still not work until xls_tools is out)
  - add comp_sense function to relate Sink-Output and Source-Input
```


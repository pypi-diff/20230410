# Comparing `tmp/datrafilcha-1.0.0.tar.gz` & `tmp/datrafilcha-1.0.1.tar.gz`

## Comparing `datrafilcha-1.0.0.tar` & `datrafilcha-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 datrafilcha-1.0.0/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datrafilcha-1.0.0/datrafilcha/__init__.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 datrafilcha-1.0.0/datrafilcha/facade.py
--rw-r--r--   0        0        0     5569 2020-02-02 00:00:00.000000 datrafilcha-1.0.0/datrafilcha/graph_functions.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 datrafilcha-1.0.0/LICENSE
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 datrafilcha-1.0.0/README.md
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 datrafilcha-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 datrafilcha-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 datrafilcha-1.0.1/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datrafilcha-1.0.1/datrafilcha/__init__.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 datrafilcha-1.0.1/datrafilcha/facade.py
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 datrafilcha-1.0.1/datrafilcha/graph_functions.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 datrafilcha-1.0.1/LICENSE
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 datrafilcha-1.0.1/README.md
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 datrafilcha-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 datrafilcha-1.0.1/PKG-INFO
```

### Comparing `datrafilcha-1.0.0/datrafilcha/facade.py` & `datrafilcha-1.0.1/datrafilcha/facade.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from os import path
 
 from . import graph_functions
-from .graph_functions import FactoryManager, ColumnDataFromCSV
+from .graph_functions import _FactoryManager, _ColumnDataFromCSV
 
 
 class DataFiltersFacade:
     def __init__(self):
-        self.factory_manager = FactoryManager
+        self.factory_manager = _FactoryManager
 
     def csv_column(self, function_cfg: dict, data_source_file: str, column: str):
         """
         Process column based data from CSV based on configuration
         """
 
         # Setup
@@ -21,15 +21,15 @@
             raise NameError("Graphing function doesn't exists! ")
 
         # Check data exists
         if not path.exists(data_source_file):
             raise NameError("Data source doesn't exists")
 
         # Factory - loads data, filter/process data
-        factory = self.factory_manager(ColumnDataFromCSV, data_source_file, column)
+        factory = self.factory_manager(_ColumnDataFromCSV, data_source_file, column)
 
         data_processing_function = getattr(graph_functions, function_type)
 
         cfg_of_function = {}
         if len(function_cfg) > 1:
             cfg_of_function = {k: v for k, v in function_cfg.items() if k != 'id'}
```

### Comparing `datrafilcha-1.0.0/datrafilcha/graph_functions.py` & `datrafilcha-1.0.1/datrafilcha/graph_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class Data(ABC):
     """Interface"""
     def load(self):
         pass
 
 
-class ColumnDataFromCSV(Data):
+class _ColumnDataFromCSV(Data):
     """Get column from CSV and return pandas data frame"""
 
     def load(self, path: str, column_name: str, sep=',') -> pd.DataFrame:
         df = pd.read_csv(path, sep=sep)
         self.data_frame = pd.DataFrame(df.get(column_name))
 
         if self.data_frame is None:
@@ -47,37 +47,37 @@
     def new(self):
         pass
 
     def produce(self):
         pass
 
 
-class FactoryManager():
+class _FactoryManager():
     """Manage data init and processing."""
     def __init__(self, data_loader: Data, path_to_data: str, cname: str) -> None:
         self.dframe = data_loader().load(path=path_to_data, column_name=cname, sep=',')
 
         return None
 
     def job(self, data_process_factory: Factory, configuration: dict) -> px:
         figure = data_process_factory.produce_result(configuration, self.dframe)
 
         return figure
 
 
-class UniqValues(Factory):
+class _UniqValues(Factory):
     def create(self, data, *args):
         c = args
         d = data
-        uniq_values_producer = UniqValuesProducer().new(d, c)
+        uniq_values_producer = _UniqValuesProducer().new(d, c)
 
         return uniq_values_producer
 
 
-class UniqValuesProducer(Producer):
+class _UniqValuesProducer(Producer):
     """
     Report repeated lines and it's number of occurrences, Eq. GNU command uniq -c
     """
 
     def new(self, data, *args):
         """Init and configure uniq_values method"""
 
@@ -137,23 +137,23 @@
                      y="Number of occurrences",
                      hover_data=["Value"]
                      )
 
         return fig
 
 
-class FrequencyOfOccurrences(Factory):
+class _FrequencyOfOccurrences(Factory):
     def create(self, data, *args):
         cfg = args
-        foop = FrequencyOfOccurrencesProducer().new(data, cfg)
+        foop = _FrequencyOfOccurrencesProducer().new(data, cfg)
 
         return foop
 
 
-class FrequencyOfOccurrencesProducer(Producer):
+class _FrequencyOfOccurrencesProducer(Producer):
     """
     Suppose you want to know how often you will meet the value when reading list of values line by line expressed as histogram.
     For example in the following set:
         a,b,a,b,a,b,a,b
     We have 8 items and we want to know the frequency of occurrences of letter b.
     X axe value = number of items - sequence
     Y axe value = for each x - y is either 0 b is not present or 1 b is present
```

### Comparing `datrafilcha-1.0.0/LICENSE` & `datrafilcha-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datrafilcha-1.0.0/README.md` & `datrafilcha-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `datrafilcha-1.0.0/PKG-INFO` & `datrafilcha-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datrafilcha
-Version: 1.0.0
+Version: 1.0.1
 Project-URL: Homepage, https://gitlab.com/gitm1993/datrafilcha
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```


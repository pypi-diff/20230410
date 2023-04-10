# Comparing `tmp/pavan_housing-0.1.tar.gz` & `tmp/pavan_housing-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pavan_housing-0.1.tar", last modified: Tue Jan 31 08:34:40 2023, max compression
+gzip compressed data, was "pavan_housing-0.2.tar", last modified: Mon Apr 10 20:13:41 2023, max compression
```

## Comparing `pavan_housing-0.1.tar` & `pavan_housing-0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 08:34:40.075805 pavan_housing-0.1/
--rw-r--r--   0 root         (0) root         (0)     1638 2023-01-31 08:34:40.075805 pavan_housing-0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1200 2023-01-23 09:12:10.000000 pavan_housing-0.1/README.md
--rw-r--r--   0 root         (0) root         (0)      764 2023-01-31 08:34:07.000000 pavan_housing-0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-31 08:34:40.075805 pavan_housing-0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-31 06:45:03.000000 pavan_housing-0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 08:34:40.075805 pavan_housing-0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 08:34:40.075805 pavan_housing-0.1/src/pavan_housing/
--rw-r--r--   0 root         (0) root         (0)       44 2023-01-31 06:41:38.000000 pavan_housing-0.1/src/pavan_housing/__init__.py
--rw-r--r--   0 root         (0) root         (0)      263 2023-01-27 14:43:09.000000 pavan_housing-0.1/src/pavan_housing/config.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-01-27 14:43:09.000000 pavan_housing-0.1/src/pavan_housing/ingest_data.py
--rw-r--r--   0 root         (0) root         (0)      987 2023-01-31 08:20:29.000000 pavan_housing-0.1/src/pavan_housing/logger.py
--rw-r--r--   0 root         (0) root         (0)     1801 2023-01-27 14:43:09.000000 pavan_housing-0.1/src/pavan_housing/methods.py
--rw-r--r--   0 root         (0) root         (0)      468 2023-01-23 08:41:42.000000 pavan_housing-0.1/src/pavan_housing/mlflow_exp.py
--rw-r--r--   0 root         (0) root         (0)     3549 2023-01-31 08:32:39.000000 pavan_housing-0.1/src/pavan_housing/train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 08:34:40.075805 pavan_housing-0.1/src/pavan_housing.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1638 2023-01-31 08:34:40.000000 pavan_housing-0.1/src/pavan_housing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      404 2023-01-31 08:34:40.000000 pavan_housing-0.1/src/pavan_housing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-31 08:34:40.000000 pavan_housing-0.1/src/pavan_housing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-01-31 08:34:40.000000 pavan_housing-0.1/src/pavan_housing.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 20:13:41.251172 pavan_housing-0.2/
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-04-10 20:13:41.251172 pavan_housing-0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1217 2023-04-10 20:00:43.000000 pavan_housing-0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      764 2023-04-10 20:13:29.000000 pavan_housing-0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 20:13:41.251172 pavan_housing-0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-01-31 06:45:03.000000 pavan_housing-0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 20:13:41.241172 pavan_housing-0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 20:13:41.251172 pavan_housing-0.2/src/pavan_housing/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-03-11 07:29:40.000000 pavan_housing-0.2/src/pavan_housing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      395 2023-04-10 18:10:42.000000 pavan_housing-0.2/src/pavan_housing/config.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-04-10 17:28:40.000000 pavan_housing-0.2/src/pavan_housing/ingest_data.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-01-31 08:41:50.000000 pavan_housing-0.2/src/pavan_housing/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2023-01-27 14:43:09.000000 pavan_housing-0.2/src/pavan_housing/methods.py
+-rw-r--r--   0 root         (0) root         (0)      807 2023-04-10 18:56:45.000000 pavan_housing-0.2/src/pavan_housing/predict.py
+-rw-r--r--   0 root         (0) root         (0)     3837 2023-04-10 18:16:50.000000 pavan_housing-0.2/src/pavan_housing/train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 20:13:41.251172 pavan_housing-0.2/src/pavan_housing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-04-10 20:13:41.000000 pavan_housing-0.2/src/pavan_housing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      401 2023-04-10 20:13:41.000000 pavan_housing-0.2/src/pavan_housing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 20:13:41.000000 pavan_housing-0.2/src/pavan_housing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-10 20:13:41.000000 pavan_housing-0.2/src/pavan_housing.egg-info/top_level.txt
```

### Comparing `pavan_housing-0.1/PKG-INFO` & `pavan_housing-0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pavan_housing
-Version: 0.1
+Version: 0.2
 Summary: 'A housing package to predict the price of houses in california'
 Author-email: Pavan Bongu <pavan.bongu@tigeranalytics.com>
 Project-URL: Homepage, https://github.com/pavanbongu7/mle-training
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -33,9 +33,10 @@
 ```
 conda activate mle-dev
 ```
 ## Installing the Package
 To install the package, you can use the following command:
 ```
 pip install .
-pip install housing_package
+
 ```
+The dot(.) here denotes the current folder
```

### Comparing `pavan_housing-0.1/README.md` & `pavan_housing-0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,9 +21,10 @@
 ```
 conda activate mle-dev
 ```
 ## Installing the Package
 To install the package, you can use the following command:
 ```
 pip install .
-pip install housing_package
-```
+
+```
+The dot(.) here denotes the current folder
```

### Comparing `pavan_housing-0.1/pyproject.toml` & `pavan_housing-0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pavan_housing"
-version = "0.1"
+version = "0.2"
 authors = [
   { name="Pavan Bongu", email="pavan.bongu@tigeranalytics.com" },
 ]
 description = "'A housing package to predict the price of houses in california'"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pavan_housing-0.1/src/pavan_housing/ingest_data.py` & `pavan_housing-0.2/src/pavan_housing/ingest_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,38 +3,36 @@
 import os
 import tarfile
 
 import pandas as pd
 import requests
 from sklearn.model_selection import train_test_split
 
-from housing.config import *
+from pavan_housing.config import *
 
 parser = argparse.ArgumentParser()
 parser.add_argument(
     "--path", help="Path to store the data files", default=DEFAULT_HOUSING_PATH
 )
 args = parser.parse_args()
 
 HOUSING_PATH = args.path
 
 logging.basicConfig(level=logging.WARN)
 logger = logging.getLogger(__name__)
 
-
-with requests.get(HOUSING_URL, stream=True) as rx, tarfile.open(
-    fileobj=rx.raw, mode="r:gz"
-) as tarobj:
-    tarobj.extractall(HOUSING_PATH)
-
-
 def load_housing_data(housing_path=HOUSING_PATH):
     csv_path = os.path.join(housing_path, "housing.csv")
     return pd.read_csv(csv_path)
 
-
-housing = load_housing_data()
+try:
+    with requests.get(HOUSING_URL, stream=True) as rx, tarfile.open(
+        fileobj=rx.raw, mode="r:gz"
+    ) as tarobj:
+        tarobj.extractall(HOUSING_PATH)
+except:
+    housing = load_housing_data()
 
 train_set, test_set = train_test_split(housing, test_size=0.2, random_state=42)
 
-train_set.to_csv(os.path.join(HOUSING_PATH, "train.csv"))
-test_set.to_csv(os.path.join(HOUSING_PATH, "test.csv"))
+train_set.to_csv(os.path.join(HOUSING_PATH, "train.csv"),index=False)
+test_set.to_csv(os.path.join(HOUSING_PATH, "test.csv"),index=False)
```

### Comparing `pavan_housing-0.1/src/pavan_housing/logger.py` & `pavan_housing-0.2/src/pavan_housing/logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from housing.config import LOGS_PATH
+from pavan_housing.config import LOGS_PATH
 
 
 def get_logger(logger_name):
     """
     get_logger : Generate logger object which will log the events in the module during the runtime
 
     Arguments:
```

### Comparing `pavan_housing-0.1/src/pavan_housing/methods.py` & `pavan_housing-0.2/src/pavan_housing/methods.py`

 * *Files identical despite different names*

### Comparing `pavan_housing-0.1/src/pavan_housing.egg-info/PKG-INFO` & `pavan_housing-0.2/src/pavan_housing.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pavan-housing
-Version: 0.1
+Version: 0.2
 Summary: 'A housing package to predict the price of houses in california'
 Author-email: Pavan Bongu <pavan.bongu@tigeranalytics.com>
 Project-URL: Homepage, https://github.com/pavanbongu7/mle-training
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -33,9 +33,10 @@
 ```
 conda activate mle-dev
 ```
 ## Installing the Package
 To install the package, you can use the following command:
 ```
 pip install .
-pip install housing_package
+
 ```
+The dot(.) here denotes the current folder
```


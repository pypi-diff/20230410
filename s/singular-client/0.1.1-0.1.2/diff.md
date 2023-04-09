# Comparing `tmp/singular_client-0.1.1.tar.gz` & `tmp/singular_client-0.1.2.tar.gz`

## Comparing `singular_client-0.1.1.tar` & `singular_client-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/__init__.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/_utils.py
--rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/api.py
--rwxr-xr-x   0        0        0     6543 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/arguments.py
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/documents.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/processing.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/endpoints/__init__.py
--rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/endpoints/_bases.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/endpoints/governance.py
--rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/endpoints/links.py
--rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/endpoints/links_legacy.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/endpoints/monetization.py
--rw-r--r--   0        0        0     8387 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/endpoints/reporting.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 singular_client-0.1.1/singular_client/endpoints/skan.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 singular_client-0.1.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 singular_client-0.1.1/README.md
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 singular_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 singular_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/__init__.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/_utils.py
+-rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/api.py
+-rwxr-xr-x   0        0        0     6543 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/arguments.py
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/documents.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/processing.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/endpoints/__init__.py
+-rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/endpoints/_bases.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/endpoints/governance.py
+-rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/endpoints/links.py
+-rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/endpoints/links_legacy.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/endpoints/monetization.py
+-rw-r--r--   0        0        0     8387 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/endpoints/reporting.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 singular_client-0.1.2/singular_client/endpoints/skan.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 singular_client-0.1.2/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 singular_client-0.1.2/README.md
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 singular_client-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 singular_client-0.1.2/PKG-INFO
```

### Comparing `singular_client-0.1.1/singular_client/_utils.py` & `singular_client-0.1.2/singular_client/_utils.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.1/singular_client/api.py` & `singular_client-0.1.2/singular_client/api.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.1/singular_client/arguments.py` & `singular_client-0.1.2/singular_client/arguments.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.1/singular_client/documents.py` & `singular_client-0.1.2/singular_client/documents.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.1/singular_client/endpoints/_bases.py` & `singular_client-0.1.2/singular_client/endpoints/_bases.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.1/singular_client/endpoints/links.py` & `singular_client-0.1.2/singular_client/endpoints/links.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.1/singular_client/endpoints/links_legacy.py` & `singular_client-0.1.2/singular_client/endpoints/links_legacy.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.1/singular_client/endpoints/monetization.py` & `singular_client-0.1.2/singular_client/endpoints/monetization.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.1/singular_client/endpoints/reporting.py` & `singular_client-0.1.2/singular_client/endpoints/reporting.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.1/singular_client/endpoints/skan.py` & `singular_client-0.1.2/singular_client/endpoints/skan.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.1/pyproject.toml` & `singular_client-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "singular-client"
-version = "0.1.1"
+version = "0.1.2"
 python_requires = ">=3.8"
 description = "Singular API client"
 authors = [
     {name = "Ryan Young", email = "dev@ryayoung.com"}
 ]
 readme = "README.md"
 license = "MIT"
@@ -20,10 +20,9 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries"
 ]
 dependencies = [
-    'pandas',
     'requests',
 ]
```


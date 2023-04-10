# Comparing `tmp/almonaut-0.1.0.tar.gz` & `tmp/almonaut-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almonaut-0.1.0.tar", last modified: Fri Sep 30 18:37:09 2022, max compression
+gzip compressed data, was "almonaut-0.2.0.tar", last modified: Mon Apr 10 19:58:57 2023, max compression
```

## Comparing `almonaut-0.1.0.tar` & `almonaut-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2022-09-30 18:37:09.495626 almonaut-0.1.0/
--rw-r--r--   0 john      (1000) john      (1000)    11357 2022-09-30 18:23:32.000000 almonaut-0.1.0/LICENSE
--rw-r--r--   0 john      (1000) john      (1000)     2539 2022-09-30 18:37:09.495626 almonaut-0.1.0/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     1801 2022-09-30 18:23:32.000000 almonaut-0.1.0/README.md
--rw-r--r--   0 john      (1000) john      (1000)      893 2022-09-30 18:23:32.000000 almonaut-0.1.0/pyproject.toml
--rw-r--r--   0 john      (1000) john      (1000)       38 2022-09-30 18:37:09.495626 almonaut-0.1.0/setup.cfg
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2022-09-30 18:37:09.491626 almonaut-0.1.0/src/
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2022-09-30 18:37:09.493626 almonaut-0.1.0/src/almonaut/
--rw-r--r--   0 john      (1000) john      (1000)        0 2022-09-30 18:23:32.000000 almonaut-0.1.0/src/almonaut/__init__.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2022-09-30 18:37:09.494626 almonaut-0.1.0/src/almonaut/acquisitions/
--rw-r--r--   0 john      (1000) john      (1000)        0 2022-09-30 18:23:32.000000 almonaut-0.1.0/src/almonaut/acquisitions/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)    19414 2022-09-30 18:23:32.000000 almonaut-0.1.0/src/almonaut/acquisitions/acquisitions_models.py
--rw-r--r--   0 john      (1000) john      (1000)    21728 2022-09-30 18:23:32.000000 almonaut-0.1.0/src/almonaut/client.py
--rw-r--r--   0 john      (1000) john      (1000)      719 2022-09-30 18:23:32.000000 almonaut-0.1.0/src/almonaut/common_validators.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2022-09-30 18:37:09.494626 almonaut-0.1.0/src/almonaut/electronic_resources/
--rw-r--r--   0 john      (1000) john      (1000)        0 2022-09-30 18:23:32.000000 almonaut-0.1.0/src/almonaut/electronic_resources/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)    16185 2022-09-30 18:23:32.000000 almonaut-0.1.0/src/almonaut/electronic_resources/electronic_resources_models.py
--rw-r--r--   0 john      (1000) john      (1000)     2221 2022-09-30 18:23:32.000000 almonaut-0.1.0/src/almonaut/exceptions.py
--rw-r--r--   0 john      (1000) john      (1000)      937 2022-09-30 18:23:32.000000 almonaut-0.1.0/src/almonaut/session.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2022-09-30 18:37:09.494626 almonaut-0.1.0/src/almonaut.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)     2539 2022-09-30 18:37:09.000000 almonaut-0.1.0/src/almonaut.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)      542 2022-09-30 18:37:09.000000 almonaut-0.1.0/src/almonaut.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) john      (1000)        1 2022-09-30 18:37:09.000000 almonaut-0.1.0/src/almonaut.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) john      (1000)       34 2022-09-30 18:37:09.000000 almonaut-0.1.0/src/almonaut.egg-info/requires.txt
--rw-r--r--   0 john      (1000) john      (1000)        9 2022-09-30 18:37:09.000000 almonaut-0.1.0/src/almonaut.egg-info/top_level.txt
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-10 19:58:57.328113 almonaut-0.2.0/
+-rw-r--r--   0 john      (1000) john      (1000)    11357 2023-04-10 18:58:10.000000 almonaut-0.2.0/LICENSE
+-rw-r--r--   0 john      (1000) john      (1000)     2539 2023-04-10 19:58:57.328113 almonaut-0.2.0/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     1801 2023-04-10 18:58:10.000000 almonaut-0.2.0/README.md
+-rw-r--r--   0 john      (1000) john      (1000)      893 2023-04-10 19:15:28.000000 almonaut-0.2.0/pyproject.toml
+-rw-r--r--   0 john      (1000) john      (1000)       38 2023-04-10 19:58:57.328113 almonaut-0.2.0/setup.cfg
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-10 19:58:57.328113 almonaut-0.2.0/src/
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-10 19:58:57.328113 almonaut-0.2.0/src/almonaut/
+-rw-r--r--   0 john      (1000) john      (1000)        0 2023-04-10 18:58:10.000000 almonaut-0.2.0/src/almonaut/__init__.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-10 19:58:57.328113 almonaut-0.2.0/src/almonaut/acquisitions/
+-rw-r--r--   0 john      (1000) john      (1000)        0 2023-04-10 18:58:10.000000 almonaut-0.2.0/src/almonaut/acquisitions/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)    19394 2023-04-10 19:10:34.000000 almonaut-0.2.0/src/almonaut/acquisitions/acquisitions_models.py
+-rw-r--r--   0 john      (1000) john      (1000)    21728 2023-04-10 18:58:10.000000 almonaut-0.2.0/src/almonaut/client.py
+-rw-r--r--   0 john      (1000) john      (1000)      719 2023-04-10 18:58:10.000000 almonaut-0.2.0/src/almonaut/common_validators.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-10 19:58:57.328113 almonaut-0.2.0/src/almonaut/electronic_resources/
+-rw-r--r--   0 john      (1000) john      (1000)        0 2023-04-10 18:58:10.000000 almonaut-0.2.0/src/almonaut/electronic_resources/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)    16185 2023-04-10 18:58:10.000000 almonaut-0.2.0/src/almonaut/electronic_resources/electronic_resources_models.py
+-rw-r--r--   0 john      (1000) john      (1000)     2221 2023-04-10 18:58:10.000000 almonaut-0.2.0/src/almonaut/exceptions.py
+-rw-r--r--   0 john      (1000) john      (1000)      937 2023-04-10 18:58:10.000000 almonaut-0.2.0/src/almonaut/session.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-10 19:58:57.328113 almonaut-0.2.0/src/almonaut.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)     2539 2023-04-10 19:58:57.000000 almonaut-0.2.0/src/almonaut.egg-info/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)      542 2023-04-10 19:58:57.000000 almonaut-0.2.0/src/almonaut.egg-info/SOURCES.txt
+-rw-r--r--   0 john      (1000) john      (1000)        1 2023-04-10 19:58:57.000000 almonaut-0.2.0/src/almonaut.egg-info/dependency_links.txt
+-rw-r--r--   0 john      (1000) john      (1000)       34 2023-04-10 19:58:57.000000 almonaut-0.2.0/src/almonaut.egg-info/requires.txt
+-rw-r--r--   0 john      (1000) john      (1000)        9 2023-04-10 19:58:57.000000 almonaut-0.2.0/src/almonaut.egg-info/top_level.txt
```

### Comparing `almonaut-0.1.0/LICENSE` & `almonaut-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `almonaut-0.1.0/PKG-INFO` & `almonaut-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almonaut
-Version: 0.1.0
+Version: 0.2.0
 Summary: A library to interact with the Ex Libris Alma(c) API
 Author: University of Waterloo Library
 Maintainer: University of Waterloo Library
 License: Apache-2.0
 Project-URL: Home Page, https://uwatlib.github.io/almonaut/
 Project-URL: Bug Tracker, https://github.com/uwatlib/almonaut/issues
 Project-URL: Changelog, https://github.com/uwatlib/almonaut/blob/master/CHANGELOG.md
```

### Comparing `almonaut-0.1.0/README.md` & `almonaut-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `almonaut-0.1.0/pyproject.toml` & `almonaut-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "almonaut"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="University of Waterloo Library" },
 ]
 maintainers = [
   { name="University of Waterloo Library" }
 ]
 license = {text = "Apache-2.0"}
@@ -17,16 +17,16 @@
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "pydantic>=1.10.2",
-    "requests>=2.28.1",
+    "pydantic>=1.10.7",
+    "requests>=2.28.2",
 ]
 
 [project.urls]
 "Home Page" = "https://uwatlib.github.io/almonaut/"
 "Bug Tracker" = "https://github.com/uwatlib/almonaut/issues"
 "Changelog" = "https://github.com/uwatlib/almonaut/blob/master/CHANGELOG.md"
 "Documentation" = "https://uwatlib.github.io/almonaut/"
```

### Comparing `almonaut-0.1.0/src/almonaut/acquisitions/acquisitions_models.py` & `almonaut-0.2.0/src/almonaut/acquisitions/acquisitions_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,15 +319,15 @@
 
 class Fund(BaseModel):
     id_: str = Field(..., alias='id')
     link: str
     code: str
     name: str
     external_id: Optional[str] = None
-    type_: Optional[Type1] = Field(..., alias='type')
+    type_: Optional[Type1] = Field(alias='type')
     entity_type: EntityType
     owner: Owner1
     status: Status1
     description: Optional[str] = None
     fiscal_period: FiscalPeriod
     currency: Currency1
     allocated_balance: float
@@ -434,15 +434,15 @@
 
 class Price(BaseModel):
     sum_: float = Field(..., alias='sum')
     currency: Currency2
 
 
 class Amount(BaseModel):
-    sum_: Optional[float] = Field(..., alias='sum')
+    sum_: Optional[float] = Field(alias='sum')
     currency: Currency4
 
     @validator('sum_', pre=True)
     def empty_string(value, field):
         if value == "":
             return None
         return value
@@ -531,15 +531,15 @@
     fifth_reporting_code: Optional[str] = None
     vendor_note: Optional[str] = None
     receiving_note: Optional[str] = None
     alerts: Optional[List[Alert]] = Field(alias='alert')
     notes: Optional[List[Note1]] = Field(alias='note')
     locations: Optional[List[Location1]] = Field(alias='location')
     interested_users: Optional[List[InterestedUser]] = Field(alias='interested_user')
-    license_: Optional[License2] = Field(..., alias='license')
+    license_: Optional[License2] = Field(alias='license')
     access_model: Optional[str] = None
     url: Optional[str] = None
     base_status: Optional[str] = None
     access_provider: Optional[str] = None
     manual_renewal: Optional[bool] = None
     renewal_cycle: Optional[RenewalCycle] = None
     subscription_from_date: Optional[date] = None
@@ -771,39 +771,39 @@
 
 
 class Term(BaseModel):
     code: Code
     value: Value
 
 
-class Type6(BaseModel):
+class Type7(BaseModel):
     # used by class Resource
     value: str
     desc: str
 
 
 class Resource(BaseModel):
     pid: str
     name: str
-    type_: Type6 = Field(..., alias='type')
+    type_: Type7 = Field(..., alias='type')
     link: str
 
 
-class Type7(BaseModel):
+class Type8(BaseModel):
     # used by class Note3
     value: str
     desc: str
 
 
 class Note3(BaseModel):
     # used by class License
     content: Optional[str] = None
     creation_date: date
     created_by: str
-    type_: Optional[Type7] = Field(..., alias='type')
+    type_: Optional[Type8] = Field(alias='type')
 
     _strip_gmt_date_z = validator('creation_date', pre=True, allow_reuse=True)(
         common_validators._strip_gmt_date_z
     )
 
 
 class License(BaseModel):
```

### Comparing `almonaut-0.1.0/src/almonaut/client.py` & `almonaut-0.2.0/src/almonaut/client.py`

 * *Files identical despite different names*

### Comparing `almonaut-0.1.0/src/almonaut/common_validators.py` & `almonaut-0.2.0/src/almonaut/common_validators.py`

 * *Files identical despite different names*

### Comparing `almonaut-0.1.0/src/almonaut/electronic_resources/electronic_resources_models.py` & `almonaut-0.2.0/src/almonaut/electronic_resources/electronic_resources_models.py`

 * *Files identical despite different names*

### Comparing `almonaut-0.1.0/src/almonaut/exceptions.py` & `almonaut-0.2.0/src/almonaut/exceptions.py`

 * *Files identical despite different names*

### Comparing `almonaut-0.1.0/src/almonaut/session.py` & `almonaut-0.2.0/src/almonaut/session.py`

 * *Files identical despite different names*

### Comparing `almonaut-0.1.0/src/almonaut.egg-info/PKG-INFO` & `almonaut-0.2.0/src/almonaut.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almonaut
-Version: 0.1.0
+Version: 0.2.0
 Summary: A library to interact with the Ex Libris Alma(c) API
 Author: University of Waterloo Library
 Maintainer: University of Waterloo Library
 License: Apache-2.0
 Project-URL: Home Page, https://uwatlib.github.io/almonaut/
 Project-URL: Bug Tracker, https://github.com/uwatlib/almonaut/issues
 Project-URL: Changelog, https://github.com/uwatlib/almonaut/blob/master/CHANGELOG.md
```

### Comparing `almonaut-0.1.0/src/almonaut.egg-info/SOURCES.txt` & `almonaut-0.2.0/src/almonaut.egg-info/SOURCES.txt`

 * *Files identical despite different names*


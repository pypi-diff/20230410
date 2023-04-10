# Comparing `tmp/deutsche-bahn-api-1.0.4.tar.gz` & `tmp/deutsche-bahn-api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deutsche-bahn-api-1.0.4.tar", last modified: Sun Jan 15 20:09:07 2023, max compression
+gzip compressed data, was "deutsche-bahn-api-1.0.5.tar", last modified: Mon Apr 10 20:05:19 2023, max compression
```

## Comparing `deutsche-bahn-api-1.0.4.tar` & `deutsche-bahn-api-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-01-15 20:09:07.593373 deutsche-bahn-api-1.0.4/
--rw-r--r--   0 manuel     (501) staff       (20)    35148 2023-01-15 14:31:50.000000 deutsche-bahn-api-1.0.4/LICENSE
--rw-r--r--   0 manuel     (501) staff       (20)     2860 2023-01-15 20:09:07.593209 deutsche-bahn-api-1.0.4/PKG-INFO
--rw-r--r--   0 manuel     (501) staff       (20)     2400 2023-01-15 15:19:26.000000 deutsche-bahn-api-1.0.4/README.md
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-01-15 20:09:07.588463 deutsche-bahn-api-1.0.4/deutsche_bahn_api/
--rw-r--r--   0 manuel     (501) staff       (20)        0 2023-01-15 18:07:45.000000 deutsche-bahn-api-1.0.4/deutsche_bahn_api/__init__.py
--rw-r--r--   0 manuel     (501) staff       (20)      711 2023-01-15 14:31:50.000000 deutsche-bahn-api-1.0.4/deutsche_bahn_api/api_authentication.py
--rw-r--r--   0 manuel     (501) staff       (20)        0 2023-01-15 14:31:50.000000 deutsche-bahn-api-1.0.4/deutsche_bahn_api/deutsche_bahn_api.py
--rw-r--r--   0 manuel     (501) staff       (20)      382 2023-01-15 19:50:15.000000 deutsche-bahn-api-1.0.4/deutsche_bahn_api/message.py
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-01-15 20:09:07.589617 deutsche-bahn-api-1.0.4/deutsche_bahn_api/static/
--rw-r--r--   0 manuel     (501) staff       (20)     6919 2023-01-15 14:31:50.000000 deutsche-bahn-api-1.0.4/deutsche_bahn_api/static/message_codes.json
--rw-r--r--   0 manuel     (501) staff       (20)  1850222 2023-01-15 14:31:50.000000 deutsche-bahn-api-1.0.4/deutsche_bahn_api/static/train_stations_list.json
--rw-r--r--   0 manuel     (501) staff       (20)      230 2023-01-15 14:31:50.000000 deutsche-bahn-api-1.0.4/deutsche_bahn_api/station.py
--rw-r--r--   0 manuel     (501) staff       (20)     1442 2023-01-15 19:48:42.000000 deutsche-bahn-api-1.0.4/deutsche_bahn_api/station_helper.py
--rw-r--r--   0 manuel     (501) staff       (20)     5001 2023-01-15 14:31:50.000000 deutsche-bahn-api-1.0.4/deutsche_bahn_api/timetable_helper.py
--rw-r--r--   0 manuel     (501) staff       (20)      365 2023-01-15 14:31:50.000000 deutsche-bahn-api-1.0.4/deutsche_bahn_api/train.py
--rw-r--r--   0 manuel     (501) staff       (20)      253 2023-01-15 14:31:50.000000 deutsche-bahn-api-1.0.4/deutsche_bahn_api/train_changes.py
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-01-15 20:09:07.589254 deutsche-bahn-api-1.0.4/deutsche_bahn_api.egg-info/
--rw-r--r--   0 manuel     (501) staff       (20)     2860 2023-01-15 20:09:07.000000 deutsche-bahn-api-1.0.4/deutsche_bahn_api.egg-info/PKG-INFO
--rw-r--r--   0 manuel     (501) staff       (20)      627 2023-01-15 20:09:07.000000 deutsche-bahn-api-1.0.4/deutsche_bahn_api.egg-info/SOURCES.txt
--rw-r--r--   0 manuel     (501) staff       (20)        1 2023-01-15 20:09:07.000000 deutsche-bahn-api-1.0.4/deutsche_bahn_api.egg-info/dependency_links.txt
--rw-r--r--   0 manuel     (501) staff       (20)       13 2023-01-15 20:09:07.000000 deutsche-bahn-api-1.0.4/deutsche_bahn_api.egg-info/requires.txt
--rw-r--r--   0 manuel     (501) staff       (20)       18 2023-01-15 20:09:07.000000 deutsche-bahn-api-1.0.4/deutsche_bahn_api.egg-info/top_level.txt
--rw-r--r--   0 manuel     (501) staff       (20)       38 2023-01-15 20:09:07.593437 deutsche-bahn-api-1.0.4/setup.cfg
--rw-r--r--   0 manuel     (501) staff       (20)      786 2023-01-15 20:09:04.000000 deutsche-bahn-api-1.0.4/setup.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-04-10 20:05:19.516141 deutsche-bahn-api-1.0.5/
+-rw-r--r--   0 manuel     (501) staff       (20)    35148 2023-04-10 19:09:31.000000 deutsche-bahn-api-1.0.5/LICENSE
+-rw-r--r--   0 manuel     (501) staff       (20)     2860 2023-04-10 20:05:19.515998 deutsche-bahn-api-1.0.5/PKG-INFO
+-rw-r--r--   0 manuel     (501) staff       (20)     2400 2023-04-10 19:09:31.000000 deutsche-bahn-api-1.0.5/README.md
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-04-10 20:05:19.512397 deutsche-bahn-api-1.0.5/deutsche_bahn_api/
+-rw-r--r--   0 manuel     (501) staff       (20)        0 2023-04-10 19:09:31.000000 deutsche-bahn-api-1.0.5/deutsche_bahn_api/__init__.py
+-rw-r--r--   0 manuel     (501) staff       (20)      711 2023-04-10 19:14:38.000000 deutsche-bahn-api-1.0.5/deutsche_bahn_api/api_authentication.py
+-rw-r--r--   0 manuel     (501) staff       (20)        0 2023-04-10 19:09:31.000000 deutsche-bahn-api-1.0.5/deutsche_bahn_api/deutsche_bahn_api.py
+-rw-r--r--   0 manuel     (501) staff       (20)      382 2023-04-10 19:09:31.000000 deutsche-bahn-api-1.0.5/deutsche_bahn_api/message.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-04-10 20:05:19.513444 deutsche-bahn-api-1.0.5/deutsche_bahn_api/static/
+-rw-r--r--   0 manuel     (501) staff       (20)     6919 2023-04-10 19:09:31.000000 deutsche-bahn-api-1.0.5/deutsche_bahn_api/static/message_codes.json
+-rw-r--r--   0 manuel     (501) staff       (20)  1850222 2023-04-10 19:09:31.000000 deutsche-bahn-api-1.0.5/deutsche_bahn_api/static/train_stations_list.json
+-rw-r--r--   0 manuel     (501) staff       (20)      230 2023-04-10 19:09:31.000000 deutsche-bahn-api-1.0.5/deutsche_bahn_api/station.py
+-rw-r--r--   0 manuel     (501) staff       (20)     1442 2023-04-10 19:09:31.000000 deutsche-bahn-api-1.0.5/deutsche_bahn_api/station_helper.py
+-rw-r--r--   0 manuel     (501) staff       (20)     5720 2023-04-10 20:00:31.000000 deutsche-bahn-api-1.0.5/deutsche_bahn_api/timetable_helper.py
+-rw-r--r--   0 manuel     (501) staff       (20)      365 2023-04-10 19:09:31.000000 deutsche-bahn-api-1.0.5/deutsche_bahn_api/train.py
+-rw-r--r--   0 manuel     (501) staff       (20)      253 2023-04-10 19:09:31.000000 deutsche-bahn-api-1.0.5/deutsche_bahn_api/train_changes.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2023-04-10 20:05:19.513150 deutsche-bahn-api-1.0.5/deutsche_bahn_api.egg-info/
+-rw-r--r--   0 manuel     (501) staff       (20)     2860 2023-04-10 20:05:19.000000 deutsche-bahn-api-1.0.5/deutsche_bahn_api.egg-info/PKG-INFO
+-rw-r--r--   0 manuel     (501) staff       (20)      627 2023-04-10 20:05:19.000000 deutsche-bahn-api-1.0.5/deutsche_bahn_api.egg-info/SOURCES.txt
+-rw-r--r--   0 manuel     (501) staff       (20)        1 2023-04-10 20:05:19.000000 deutsche-bahn-api-1.0.5/deutsche_bahn_api.egg-info/dependency_links.txt
+-rw-r--r--   0 manuel     (501) staff       (20)       13 2023-04-10 20:05:19.000000 deutsche-bahn-api-1.0.5/deutsche_bahn_api.egg-info/requires.txt
+-rw-r--r--   0 manuel     (501) staff       (20)       18 2023-04-10 20:05:19.000000 deutsche-bahn-api-1.0.5/deutsche_bahn_api.egg-info/top_level.txt
+-rw-r--r--   0 manuel     (501) staff       (20)       38 2023-04-10 20:05:19.516197 deutsche-bahn-api-1.0.5/setup.cfg
+-rw-r--r--   0 manuel     (501) staff       (20)      786 2023-04-10 20:04:07.000000 deutsche-bahn-api-1.0.5/setup.py
```

### Comparing `deutsche-bahn-api-1.0.4/LICENSE` & `deutsche-bahn-api-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `deutsche-bahn-api-1.0.4/PKG-INFO` & `deutsche-bahn-api-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deutsche-bahn-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: A small package to work with the Deutsche Bahn timetables api
 Home-page: https://github.com/Tutorialwork/deutsche_bahn_api
 Author: Tutorialwork
 Author-email: mail@manuelschuler.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deutsche-bahn-api-1.0.4/README.md` & `deutsche-bahn-api-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `deutsche-bahn-api-1.0.4/deutsche_bahn_api/api_authentication.py` & `deutsche-bahn-api-1.0.5/deutsche_bahn_api/api_authentication.py`

 * *Files identical despite different names*

### Comparing `deutsche-bahn-api-1.0.4/deutsche_bahn_api/static/message_codes.json` & `deutsche-bahn-api-1.0.5/deutsche_bahn_api/static/message_codes.json`

 * *Files identical despite different names*

### Comparing `deutsche-bahn-api-1.0.4/deutsche_bahn_api/static/train_stations_list.json` & `deutsche-bahn-api-1.0.5/deutsche_bahn_api/static/train_stations_list.json`

 * *Files identical despite different names*

### Comparing `deutsche-bahn-api-1.0.4/deutsche_bahn_api/station_helper.py` & `deutsche-bahn-api-1.0.5/deutsche_bahn_api/station_helper.py`

 * *Files identical despite different names*

### Comparing `deutsche-bahn-api-1.0.4/deutsche_bahn_api/timetable_helper.py` & `deutsche-bahn-api-1.0.5/deutsche_bahn_api/timetable_helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from datetime import datetime
+from datetime import datetime, timedelta
 from typing import Optional
 
 import requests
 import xml.etree.ElementTree as elementTree
 
 from deutsche_bahn_api.api_authentication import ApiAuthentication
 from deutsche_bahn_api.message import Message, resolve_message_by_code
@@ -17,25 +17,35 @@
     station: Station
     api_authentication: ApiAuthentication
 
     def __init__(self, station: Station, api_authentication: ApiAuthentication) -> None:
         self.station = station
         self.api_authentication = api_authentication
 
-    def get_timetable_xml(self, hour: Optional[int] = None) -> str:
+    def get_timetable_xml(self, hour: Optional[int] = None, date: Optional[datetime] = None) -> str:
         hour_date: datetime = datetime.now()
         if hour:
             hour_date = datetime.strptime(str(hour), "%H")
-        date: str = datetime.now().strftime("%y%m%d")
+        date_string: str = datetime.now().strftime("%y%m%d")
+        if date is not None:
+            date_string = date.strftime("%y%m%d")
         hour: str = hour_date.strftime("%H")
         response = requests.get(
             f"https://apis.deutschebahn.com/db-api-marketplace/apis/timetables/v1"
-            f"/plan/{self.station.EVA_NR}/{date}/{hour}",
+            f"/plan/{self.station.EVA_NR}/{date_string}/{hour}",
             headers=self.api_authentication.get_headers()
         )
+        if response.status_code == 410:
+            return self.get_timetable_xml(int(hour), datetime.now() + timedelta(days=1))
+        elif response.status_code == 401:
+            raise Exception("Can't request timetable because the credentials are not correct. Please make sure that "
+                            "you providing the correct credentials.")
+        elif response.status_code != 200:
+            raise Exception("Can't request timetable! The request failed with the HTTP status code {}: {}"
+                            .format(response.status_code, response.text))
         return response.text
 
     def get_timetable(self, hour: Optional[int] = None) -> list[Train]:
         train_list: list[Train] = []
         trains = elementTree.fromstringlist(self.get_timetable_xml(hour))
         for train in trains:
             trip_label_object: dict[str, str] | None = None
```

### Comparing `deutsche-bahn-api-1.0.4/deutsche_bahn_api.egg-info/PKG-INFO` & `deutsche-bahn-api-1.0.5/deutsche_bahn_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deutsche-bahn-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: A small package to work with the Deutsche Bahn timetables api
 Home-page: https://github.com/Tutorialwork/deutsche_bahn_api
 Author: Tutorialwork
 Author-email: mail@manuelschuler.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deutsche-bahn-api-1.0.4/deutsche_bahn_api.egg-info/SOURCES.txt` & `deutsche-bahn-api-1.0.5/deutsche_bahn_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deutsche-bahn-api-1.0.4/setup.py` & `deutsche-bahn-api-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="deutsche-bahn-api",
-    version="1.0.4",
+    version="1.0.5",
     author="Tutorialwork",
     author_email="mail@manuelschuler.dev",
     description="A small package to work with the Deutsche Bahn timetables api",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tutorialwork/deutsche_bahn_api",
     packages=find_packages(),
```


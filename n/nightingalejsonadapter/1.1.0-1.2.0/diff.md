# Comparing `tmp/nightingalejsonadapter-1.1.0.tar.gz` & `tmp/nightingalejsonadapter-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nightingalejsonadapter-1.1.0.tar", last modified: Tue Apr  4 16:27:37 2023, max compression
+gzip compressed data, was "nightingalejsonadapter-1.2.0.tar", last modified: Mon Apr 10 14:33:10 2023, max compression
```

## Comparing `nightingalejsonadapter-1.1.0.tar` & `nightingalejsonadapter-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2023-04-04 16:27:37.721688 nightingalejsonadapter-1.1.0/
--rw-r--r--   0 nuno      (1000) nuno      (1000)      246 2023-04-04 16:27:37.721688 nightingalejsonadapter-1.1.0/PKG-INFO
-drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2023-04-04 16:27:37.721688 nightingalejsonadapter-1.1.0/nightingalejsonadapter/
--rw-r--r--   0 nuno      (1000) nuno      (1000)        0 2023-04-04 16:22:01.000000 nightingalejsonadapter-1.1.0/nightingalejsonadapter/__init__.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      560 2023-04-03 16:31:02.000000 nightingalejsonadapter-1.1.0/nightingalejsonadapter/patient_info_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      516 2023-03-15 15:22:55.000000 nightingalejsonadapter-1.1.0/nightingalejsonadapter/uuid_generator.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      581 2023-04-03 15:47:00.000000 nightingalejsonadapter-1.1.0/nightingalejsonadapter/vital_kafka_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      596 2023-03-16 11:54:47.000000 nightingalejsonadapter-1.1.0/nightingalejsonadapter/vitals_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)     1170 2023-03-16 11:52:53.000000 nightingalejsonadapter-1.1.0/nightingalejsonadapter/vitals_response.py
-drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2023-04-04 16:27:37.721688 nightingalejsonadapter-1.1.0/nightingalejsonadapter.egg-info/
--rw-r--r--   0 nuno      (1000) nuno      (1000)      246 2023-04-04 16:27:37.000000 nightingalejsonadapter-1.1.0/nightingalejsonadapter.egg-info/PKG-INFO
--rw-r--r--   0 nuno      (1000) nuno      (1000)      489 2023-04-04 16:27:37.000000 nightingalejsonadapter-1.1.0/nightingalejsonadapter.egg-info/SOURCES.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)        1 2023-04-04 16:27:37.000000 nightingalejsonadapter-1.1.0/nightingalejsonadapter.egg-info/dependency_links.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)        9 2023-04-04 16:27:37.000000 nightingalejsonadapter-1.1.0/nightingalejsonadapter.egg-info/requires.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)       23 2023-04-04 16:27:37.000000 nightingalejsonadapter-1.1.0/nightingalejsonadapter.egg-info/top_level.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)       38 2023-04-04 16:27:37.721688 nightingalejsonadapter-1.1.0/setup.cfg
--rw-r--r--   0 nuno      (1000) nuno      (1000)      715 2023-04-04 16:27:35.000000 nightingalejsonadapter-1.1.0/setup.py
+drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2023-04-10 14:33:10.436648 nightingalejsonadapter-1.2.0/
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      246 2023-04-10 14:33:10.436648 nightingalejsonadapter-1.2.0/PKG-INFO
+drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2023-04-10 14:33:10.436648 nightingalejsonadapter-1.2.0/nightingalejsonadapter/
+-rw-r--r--   0 nuno      (1000) nuno      (1000)        0 2023-04-04 16:22:01.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter/__init__.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      452 2023-04-05 17:04:25.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter/intervention_adapter.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      560 2023-04-03 16:31:02.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter/patient_info_adapter.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      516 2023-03-15 15:22:55.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter/uuid_generator.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      622 2023-04-05 17:04:56.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter/vital_kafka_adapter.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      601 2023-04-05 17:04:40.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter/vitals_adapter.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)     1180 2023-04-05 17:05:24.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter/vitals_response.py
+drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2023-04-10 14:33:10.436648 nightingalejsonadapter-1.2.0/nightingalejsonadapter.egg-info/
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      246 2023-04-10 14:33:10.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter.egg-info/PKG-INFO
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      536 2023-04-10 14:33:10.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter.egg-info/SOURCES.txt
+-rw-r--r--   0 nuno      (1000) nuno      (1000)        1 2023-04-10 14:33:10.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter.egg-info/dependency_links.txt
+-rw-r--r--   0 nuno      (1000) nuno      (1000)        9 2023-04-10 14:33:10.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter.egg-info/requires.txt
+-rw-r--r--   0 nuno      (1000) nuno      (1000)       23 2023-04-10 14:33:10.000000 nightingalejsonadapter-1.2.0/nightingalejsonadapter.egg-info/top_level.txt
+-rw-r--r--   0 nuno      (1000) nuno      (1000)       38 2023-04-10 14:33:10.436648 nightingalejsonadapter-1.2.0/setup.cfg
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      715 2023-04-05 17:01:48.000000 nightingalejsonadapter-1.2.0/setup.py
```

### Comparing `nightingalejsonadapter-1.1.0/nightingalejsonadapter/patient_info_adapter.py` & `nightingalejsonadapter-1.2.0/nightingalejsonadapter/patient_info_adapter.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-1.1.0/nightingalejsonadapter/uuid_generator.py` & `nightingalejsonadapter-1.2.0/nightingalejsonadapter/uuid_generator.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-1.1.0/nightingalejsonadapter/vitals_adapter.py` & `nightingalejsonadapter-1.2.0/nightingalejsonadapter/vitals_adapter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from typing import List
 from pydantic import BaseModel
 from enum import Enum
-import datetime
+from datetime import datetime
 
 class triageColour(Enum):
     red = 1
     yellow = 2
     green = 3
     purple = 4
 
@@ -18,12 +18,12 @@
     respiratoryRate: int
     temperature: int
     heartRateVariability: int
     GCS: int
     glucose: int
     treatment: str
     triageColour: triageColour
-    date: datetime.datetime
+    date: datetime
 
 class Model(BaseModel):
     victimID: str
     vitals: List[vitals]
```

### Comparing `nightingalejsonadapter-1.1.0/nightingalejsonadapter/vitals_response.py` & `nightingalejsonadapter-1.2.0/nightingalejsonadapter/vitals_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,22 +36,22 @@
 class ProcedureMessagesABC(BaseModel):
     a: ProcedureMessage
     b: ProcedureMessage
     c: ProcedureMessage
 
 
 class Prediction(BaseModel):
-    Timestamp: str
+    Timestamp: datetime
     VitalPredictions: VitalPredictions
     VitalEarlyWarningScore: VitalEarlyWarningScore
     ShockIndex: ShockIndex
     ProcedureMessagesABC: ProcedureMessagesABC
 
 
 class Model(BaseModel):
     UUID: str
-    LastMeasurementTimestamp: str
+    LastMeasurementTimestamp: datetime
     PredictionTimestampId: str
     PredictionTimeDeltaMinutes: int
     PatientId: str
     ProcedureMessageCount: int
     Predictions: List[Prediction]
```

### Comparing `nightingalejsonadapter-1.1.0/setup.py` & `nightingalejsonadapter-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.0' 
+VERSION = '1.2.0' 
 DESCRIPTION = 'JSON adapter'
 LONG_DESCRIPTION = 'JSON adapters and validators for Nightingale Communication and Integration'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="nightingalejsonadapter",
```


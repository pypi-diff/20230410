# Comparing `tmp/sqlalchemy-spanner-1.3.0.tar.gz` & `tmp/sqlalchemy-spanner-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-spanner-1.3.0.tar", last modified: Tue Mar 21 05:23:50 2023, max compression
+gzip compressed data, was "sqlalchemy-spanner-1.4.0.tar", last modified: Mon Apr 10 05:40:20 2023, max compression
```

## Comparing `sqlalchemy-spanner-1.3.0.tar` & `sqlalchemy-spanner-1.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-21 05:23:50.486317 sqlalchemy-spanner-1.3.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-21 05:21:53.000000 sqlalchemy-spanner-1.3.0/LICENSE
--rw-r--r--   0 root         (0)     1003    17361 2023-03-21 05:23:50.486317 sqlalchemy-spanner-1.3.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003    16988 2023-03-21 05:21:53.000000 sqlalchemy-spanner-1.3.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-21 05:23:50.482317 sqlalchemy-spanner-1.3.0/google/
--rw-rw-r--   0 root         (0)     1003      747 2023-03-21 05:21:53.000000 sqlalchemy-spanner-1.3.0/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-21 05:23:50.482317 sqlalchemy-spanner-1.3.0/google/cloud/
--rw-rw-r--   0 root         (0)     1003      747 2023-03-21 05:21:53.000000 sqlalchemy-spanner-1.3.0/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-21 05:23:50.482317 sqlalchemy-spanner-1.3.0/google/cloud/sqlalchemy_spanner/
--rw-rw-r--   0 root         (0)     1003      651 2023-03-21 05:21:53.000000 sqlalchemy-spanner-1.3.0/google/cloud/sqlalchemy_spanner/__init__.py
--rw-rw-r--   0 root         (0)     1003     1988 2023-03-21 05:21:53.000000 sqlalchemy-spanner-1.3.0/google/cloud/sqlalchemy_spanner/_opentelemetry_tracing.py
--rw-rw-r--   0 root         (0)     1003      792 2023-03-21 05:21:53.000000 sqlalchemy-spanner-1.3.0/google/cloud/sqlalchemy_spanner/provision.py
--rw-rw-r--   0 root         (0)     1003     2675 2023-03-21 05:21:53.000000 sqlalchemy-spanner-1.3.0/google/cloud/sqlalchemy_spanner/requirements.py
--rw-rw-r--   0 root         (0)     1003    35544 2023-03-21 05:21:53.000000 sqlalchemy-spanner-1.3.0/google/cloud/sqlalchemy_spanner/sqlalchemy_spanner.py
--rw-rw-r--   0 root         (0)     1003      261 2023-03-21 05:23:50.486317 sqlalchemy-spanner-1.3.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2431 2023-03-21 05:21:53.000000 sqlalchemy-spanner-1.3.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-21 05:23:50.486317 sqlalchemy-spanner-1.3.0/sqlalchemy_spanner.egg-info/
--rw-r--r--   0 root         (0)     1003    17361 2023-03-21 05:23:50.000000 sqlalchemy-spanner-1.3.0/sqlalchemy_spanner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      720 2023-03-21 05:23:50.000000 sqlalchemy-spanner-1.3.0/sqlalchemy_spanner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-21 05:23:50.000000 sqlalchemy-spanner-1.3.0/sqlalchemy_spanner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       87 2023-03-21 05:23:50.000000 sqlalchemy-spanner-1.3.0/sqlalchemy_spanner.egg-info/entry_points.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-21 05:23:50.000000 sqlalchemy-spanner-1.3.0/sqlalchemy_spanner.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-21 05:23:50.000000 sqlalchemy-spanner-1.3.0/sqlalchemy_spanner.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      155 2023-03-21 05:23:50.000000 sqlalchemy-spanner-1.3.0/sqlalchemy_spanner.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-21 05:23:50.000000 sqlalchemy-spanner-1.3.0/sqlalchemy_spanner.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-21 05:23:50.486317 sqlalchemy-spanner-1.3.0/test/
--rw-rw-r--   0 root         (0)     1003    65384 2023-03-21 05:21:53.000000 sqlalchemy-spanner-1.3.0/test/test_suite_13.py
--rw-rw-r--   0 root         (0)     1003    74431 2023-03-21 05:21:53.000000 sqlalchemy-spanner-1.3.0/test/test_suite_14.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-10 05:40:20.883465 sqlalchemy-spanner-1.4.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/LICENSE
+-rw-r--r--   0 root         (0)     1003    17665 2023-04-10 05:40:20.883465 sqlalchemy-spanner-1.4.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003    17292 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-10 05:40:20.879465 sqlalchemy-spanner-1.4.0/google/
+-rw-rw-r--   0 root         (0)     1003      747 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-10 05:40:20.879465 sqlalchemy-spanner-1.4.0/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      747 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-10 05:40:20.883465 sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/
+-rw-rw-r--   0 root         (0)     1003      651 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1988 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/_opentelemetry_tracing.py
+-rw-rw-r--   0 root         (0)     1003      792 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/provision.py
+-rw-rw-r--   0 root         (0)     1003     2675 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/requirements.py
+-rw-rw-r--   0 root         (0)     1003    35544 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/sqlalchemy_spanner.py
+-rw-rw-r--   0 root         (0)     1003      261 2023-04-10 05:40:20.887465 sqlalchemy-spanner-1.4.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2431 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-10 05:40:20.883465 sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/
+-rw-r--r--   0 root         (0)     1003    17665 2023-04-10 05:40:20.000000 sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      720 2023-04-10 05:40:20.000000 sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-10 05:40:20.000000 sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       87 2023-04-10 05:40:20.000000 sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-04-10 05:40:20.000000 sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-10 05:40:20.000000 sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      155 2023-04-10 05:40:20.000000 sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-04-10 05:40:20.000000 sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-10 05:40:20.883465 sqlalchemy-spanner-1.4.0/test/
+-rw-rw-r--   0 root         (0)     1003    66314 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/test/test_suite_13.py
+-rw-rw-r--   0 root         (0)     1003    75361 2023-04-10 05:38:19.000000 sqlalchemy-spanner-1.4.0/test/test_suite_14.py
```

### Comparing `sqlalchemy-spanner-1.3.0/LICENSE` & `sqlalchemy-spanner-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.3.0/PKG-INFO` & `sqlalchemy-spanner-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-spanner
-Version: 1.3.0
+Version: 1.4.0
 Summary: SQLAlchemy dialect integrated into Cloud Spanner database
 Home-page: https://github.com/cloudspannerecosystem/python-spanner-sqlalchemy
 Author: Google LLC
 Author-email: cloud-spanner-developers@googlegroups.com
 Classifier: Intended Audience :: Developers
 Provides-Extra: tracing
 License-File: LICENSE
@@ -83,14 +83,23 @@
 
    # for SQLAlchemy 1.3:
    spanner:///projects/project-id/instances/instance-id/databases/database-id
 
    # for SQLAlchemy 1.4:
    spanner+spanner:///projects/project-id/instances/instance-id/databases/database-id
 
+To pass your custom client object directly to be be used, create engine as following:
+
+.. code:: python
+
+    engine = create_engine(
+        "spanner+spanner:///projects/project-id/instances/instance-id/databases/database-id",
+        connect_args={'client': spanner.Client(project="project-id")}
+    )
+
 Create a table
 ~~~~~~~~~~~~~~
 
 .. code:: python
 
    from sqlalchemy import (
        Column,
```

### Comparing `sqlalchemy-spanner-1.3.0/README.rst` & `sqlalchemy-spanner-1.4.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,23 @@
 
    # for SQLAlchemy 1.3:
    spanner:///projects/project-id/instances/instance-id/databases/database-id
 
    # for SQLAlchemy 1.4:
    spanner+spanner:///projects/project-id/instances/instance-id/databases/database-id
 
+To pass your custom client object directly to be be used, create engine as following:
+
+.. code:: python
+
+    engine = create_engine(
+        "spanner+spanner:///projects/project-id/instances/instance-id/databases/database-id",
+        connect_args={'client': spanner.Client(project="project-id")}
+    )
+
 Create a table
 ~~~~~~~~~~~~~~
 
 .. code:: python
 
    from sqlalchemy import (
        Column,
```

### Comparing `sqlalchemy-spanner-1.3.0/google/__init__.py` & `sqlalchemy-spanner-1.4.0/google/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.3.0/google/cloud/__init__.py` & `sqlalchemy-spanner-1.4.0/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.3.0/google/cloud/sqlalchemy_spanner/__init__.py` & `sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.3.0/google/cloud/sqlalchemy_spanner/_opentelemetry_tracing.py` & `sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/_opentelemetry_tracing.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.3.0/google/cloud/sqlalchemy_spanner/provision.py` & `sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/provision.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.3.0/google/cloud/sqlalchemy_spanner/requirements.py` & `sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/requirements.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.3.0/google/cloud/sqlalchemy_spanner/sqlalchemy_spanner.py` & `sqlalchemy-spanner-1.4.0/google/cloud/sqlalchemy_spanner/sqlalchemy_spanner.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.3.0/setup.py` & `sqlalchemy-spanner-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.3.0/sqlalchemy_spanner.egg-info/PKG-INFO` & `sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-spanner
-Version: 1.3.0
+Version: 1.4.0
 Summary: SQLAlchemy dialect integrated into Cloud Spanner database
 Home-page: https://github.com/cloudspannerecosystem/python-spanner-sqlalchemy
 Author: Google LLC
 Author-email: cloud-spanner-developers@googlegroups.com
 Classifier: Intended Audience :: Developers
 Provides-Extra: tracing
 License-File: LICENSE
@@ -83,14 +83,23 @@
 
    # for SQLAlchemy 1.3:
    spanner:///projects/project-id/instances/instance-id/databases/database-id
 
    # for SQLAlchemy 1.4:
    spanner+spanner:///projects/project-id/instances/instance-id/databases/database-id
 
+To pass your custom client object directly to be be used, create engine as following:
+
+.. code:: python
+
+    engine = create_engine(
+        "spanner+spanner:///projects/project-id/instances/instance-id/databases/database-id",
+        connect_args={'client': spanner.Client(project="project-id")}
+    )
+
 Create a table
 ~~~~~~~~~~~~~~
 
 .. code:: python
 
    from sqlalchemy import (
        Column,
```

### Comparing `sqlalchemy-spanner-1.3.0/sqlalchemy_spanner.egg-info/SOURCES.txt` & `sqlalchemy-spanner-1.4.0/sqlalchemy_spanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.3.0/test/test_suite_13.py` & `sqlalchemy-spanner-1.4.0/test/test_suite_13.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 import pkg_resources
 import pytest
 import random
 import time
 from unittest import mock
 
-from google.cloud.spanner_v1 import RequestOptions
+from google.cloud.spanner_v1 import RequestOptions, Client
 
 import sqlalchemy
 from sqlalchemy import create_engine
 from sqlalchemy import inspect
 from sqlalchemy import testing
 from sqlalchemy import ForeignKey
 from sqlalchemy import MetaData
@@ -116,15 +116,15 @@
     TextTest as _TextTest,
     TimeTest as _TimeTest,
     TimeMicrosecondsTest as _TimeMicrosecondsTest,
     TimestampMicrosecondsTest,
     UnicodeVarcharTest as _UnicodeVarcharTest,
     UnicodeTextTest as _UnicodeTextTest,
 )
-from test._helpers import get_db_url
+from test._helpers import get_db_url, get_project
 
 config.test_schema = ""
 
 
 class EscapingTest(_EscapingTest):
     @provide_metadata
     def test_percent_sign_round_trip(self):
@@ -1957,7 +1957,34 @@
         pass
 
     @pytest.mark.skip(
         "Spanner doesn't support type casts inside JSON_VALUE() function."
     )
     def test_round_trip_none_as_sql_null(self):
         pass
+
+
+class CreateEngineWithClientObjectTest(fixtures.TestBase):
+    def test_create_engine_w_valid_client_object(self):
+        """
+        SPANNER TEST:
+
+        Check that we can connect to SqlAlchemy
+        by passing custom Client object.
+        """
+        client = Client(project=get_project())
+        engine = create_engine(get_db_url(), connect_args={"client": client})
+        with engine.connect() as connection:
+            assert connection.connection.instance._client == client
+
+    def test_create_engine_w_invalid_client_object(self):
+        """
+        SPANNER TEST:
+
+        Check that if project id in url and custom Client
+        Object passed to enginer mismatch, error is thrown.
+        """
+        client = Client(project="project_id")
+        engine = create_engine(get_db_url(), connect_args={"client": client})
+
+        with pytest.raises(ValueError):
+            engine.connect()
```

### Comparing `sqlalchemy-spanner-1.3.0/test/test_suite_14.py` & `sqlalchemy-spanner-1.4.0/test/test_suite_14.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,4609 +44,4668 @@
 000002b0: 7572 6365 730a 696d 706f 7274 2070 7974  urces.import pyt
 000002c0: 6573 740a 696d 706f 7274 2072 616e 646f  est.import rando
 000002d0: 6d0a 696d 706f 7274 2074 696d 650a 6672  m.import time.fr
 000002e0: 6f6d 2075 6e69 7474 6573 7420 696d 706f  om unittest impo
 000002f0: 7274 206d 6f63 6b0a 0a66 726f 6d20 676f  rt mock..from go
 00000300: 6f67 6c65 2e63 6c6f 7564 2e73 7061 6e6e  ogle.cloud.spann
 00000310: 6572 5f76 3120 696d 706f 7274 2052 6571  er_v1 import Req
-00000320: 7565 7374 4f70 7469 6f6e 730a 0a69 6d70  uestOptions..imp
-00000330: 6f72 7420 7371 6c61 6c63 6865 6d79 0a66  ort sqlalchemy.f
-00000340: 726f 6d20 7371 6c61 6c63 6865 6d79 2069  rom sqlalchemy i
-00000350: 6d70 6f72 7420 6372 6561 7465 5f65 6e67  mport create_eng
-00000360: 696e 650a 6672 6f6d 2073 716c 616c 6368  ine.from sqlalch
-00000370: 656d 7920 696d 706f 7274 2069 6e73 7065  emy import inspe
-00000380: 6374 0a66 726f 6d20 7371 6c61 6c63 6865  ct.from sqlalche
-00000390: 6d79 2069 6d70 6f72 7420 7465 7374 696e  my import testin
-000003a0: 670a 6672 6f6d 2073 716c 616c 6368 656d  g.from sqlalchem
-000003b0: 7920 696d 706f 7274 2046 6f72 6569 676e  y import Foreign
-000003c0: 4b65 790a 6672 6f6d 2073 716c 616c 6368  Key.from sqlalch
-000003d0: 656d 7920 696d 706f 7274 204d 6574 6144  emy import MetaD
-000003e0: 6174 610a 6672 6f6d 2073 716c 616c 6368  ata.from sqlalch
-000003f0: 656d 792e 7363 6865 6d61 2069 6d70 6f72  emy.schema impor
-00000400: 7420 4444 4c0a 6672 6f6d 2073 716c 616c  t DDL.from sqlal
-00000410: 6368 656d 792e 7363 6865 6d61 2069 6d70  chemy.schema imp
-00000420: 6f72 7420 436f 6d70 7574 6564 0a66 726f  ort Computed.fro
-00000430: 6d20 7371 6c61 6c63 6865 6d79 2e74 6573  m sqlalchemy.tes
-00000440: 7469 6e67 2069 6d70 6f72 7420 636f 6e66  ting import conf
-00000450: 6967 0a66 726f 6d20 7371 6c61 6c63 6865  ig.from sqlalche
-00000460: 6d79 2e74 6573 7469 6e67 2069 6d70 6f72  my.testing impor
-00000470: 7420 656e 6769 6e65 730a 6672 6f6d 2073  t engines.from s
-00000480: 716c 616c 6368 656d 792e 7465 7374 696e  qlalchemy.testin
-00000490: 6720 696d 706f 7274 2065 715f 0a66 726f  g import eq_.fro
-000004a0: 6d20 7371 6c61 6c63 6865 6d79 2e74 6573  m sqlalchemy.tes
-000004b0: 7469 6e67 2069 6d70 6f72 7420 7072 6f76  ting import prov
-000004c0: 6964 655f 6d65 7461 6461 7461 2c20 656d  ide_metadata, em
-000004d0: 6974 735f 7761 726e 696e 670a 6672 6f6d  its_warning.from
-000004e0: 2073 716c 616c 6368 656d 792e 7465 7374   sqlalchemy.test
-000004f0: 696e 6720 696d 706f 7274 2066 6978 7475  ing import fixtu
-00000500: 7265 730a 6672 6f6d 2073 716c 616c 6368  res.from sqlalch
-00000510: 656d 792e 7465 7374 696e 672e 7072 6f76  emy.testing.prov
-00000520: 6973 696f 6e20 696d 706f 7274 2074 656d  ision import tem
-00000530: 705f 7461 626c 655f 6b65 7977 6f72 645f  p_table_keyword_
-00000540: 6172 6773 0a66 726f 6d20 7371 6c61 6c63  args.from sqlalc
-00000550: 6865 6d79 2e74 6573 7469 6e67 2e73 6368  hemy.testing.sch
-00000560: 656d 6120 696d 706f 7274 2043 6f6c 756d  ema import Colum
-00000570: 6e0a 6672 6f6d 2073 716c 616c 6368 656d  n.from sqlalchem
-00000580: 792e 7465 7374 696e 672e 7363 6865 6d61  y.testing.schema
-00000590: 2069 6d70 6f72 7420 5461 626c 650a 6672   import Table.fr
-000005a0: 6f6d 2073 716c 616c 6368 656d 7920 696d  om sqlalchemy im
-000005b0: 706f 7274 206c 6974 6572 616c 5f63 6f6c  port literal_col
-000005c0: 756d 6e0a 6672 6f6d 2073 716c 616c 6368  umn.from sqlalch
-000005d0: 656d 7920 696d 706f 7274 2073 656c 6563  emy import selec
-000005e0: 740a 6672 6f6d 2073 716c 616c 6368 656d  t.from sqlalchem
-000005f0: 7920 696d 706f 7274 2075 7469 6c0a 6672  y import util.fr
-00000600: 6f6d 2073 716c 616c 6368 656d 7920 696d  om sqlalchemy im
-00000610: 706f 7274 2075 6e69 6f6e 0a66 726f 6d20  port union.from 
-00000620: 7371 6c61 6c63 6865 6d79 2069 6d70 6f72  sqlalchemy impor
-00000630: 7420 6576 656e 740a 6672 6f6d 2073 716c  t event.from sql
-00000640: 616c 6368 656d 7920 696d 706f 7274 2065  alchemy import e
-00000650: 7869 7374 730a 6672 6f6d 2073 716c 616c  xists.from sqlal
-00000660: 6368 656d 7920 696d 706f 7274 2042 6f6f  chemy import Boo
-00000670: 6c65 616e 0a66 726f 6d20 7371 6c61 6c63  lean.from sqlalc
-00000680: 6865 6d79 2069 6d70 6f72 7420 466c 6f61  hemy import Floa
-00000690: 740a 6672 6f6d 2073 716c 616c 6368 656d  t.from sqlalchem
-000006a0: 7920 696d 706f 7274 204c 6172 6765 4269  y import LargeBi
-000006b0: 6e61 7279 0a66 726f 6d20 7371 6c61 6c63  nary.from sqlalc
-000006c0: 6865 6d79 2069 6d70 6f72 7420 5374 7269  hemy import Stri
-000006d0: 6e67 0a66 726f 6d20 7371 6c61 6c63 6865  ng.from sqlalche
-000006e0: 6d79 2e65 7874 2e64 6563 6c61 7261 7469  my.ext.declarati
-000006f0: 7665 2069 6d70 6f72 7420 6465 636c 6172  ve import declar
-00000700: 6174 6976 655f 6261 7365 0a66 726f 6d20  ative_base.from 
-00000710: 7371 6c61 6c63 6865 6d79 2e6f 726d 2069  sqlalchemy.orm i
-00000720: 6d70 6f72 7420 7265 6c61 7469 6f6e 0a66  mport relation.f
-00000730: 726f 6d20 7371 6c61 6c63 6865 6d79 2e6f  rom sqlalchemy.o
-00000740: 726d 2069 6d70 6f72 7420 5365 7373 696f  rm import Sessio
-00000750: 6e0a 6672 6f6d 2073 716c 616c 6368 656d  n.from sqlalchem
-00000760: 792e 7479 7065 7320 696d 706f 7274 2049  y.types import I
-00000770: 6e74 6567 6572 0a66 726f 6d20 7371 6c61  nteger.from sqla
-00000780: 6c63 6865 6d79 2e74 7970 6573 2069 6d70  lchemy.types imp
-00000790: 6f72 7420 4e75 6d65 7269 630a 6672 6f6d  ort Numeric.from
-000007a0: 2073 716c 616c 6368 656d 792e 7479 7065   sqlalchemy.type
-000007b0: 7320 696d 706f 7274 2054 6578 740a 6672  s import Text.fr
-000007c0: 6f6d 2073 716c 616c 6368 656d 792e 7465  om sqlalchemy.te
-000007d0: 7374 696e 6720 696d 706f 7274 2072 6571  sting import req
-000007e0: 7569 7265 730a 6672 6f6d 2073 716c 616c  uires.from sqlal
-000007f0: 6368 656d 792e 7465 7374 696e 6720 696d  chemy.testing im
-00000800: 706f 7274 2069 735f 7472 7565 0a66 726f  port is_true.fro
-00000810: 6d20 7371 6c61 6c63 6865 6d79 2e74 6573  m sqlalchemy.tes
-00000820: 7469 6e67 2e66 6978 7475 7265 7320 696d  ting.fixtures im
-00000830: 706f 7274 2028 0a20 2020 2043 6f6d 7075  port (.    Compu
-00000840: 7465 6452 6566 6c65 6374 696f 6e46 6978  tedReflectionFix
-00000850: 7475 7265 5465 7374 2061 7320 5f43 6f6d  tureTest as _Com
-00000860: 7075 7465 6452 6566 6c65 6374 696f 6e46  putedReflectionF
-00000870: 6978 7475 7265 5465 7374 2c0a 290a 0a66  ixtureTest,.)..f
-00000880: 726f 6d20 676f 6f67 6c65 2e61 7069 5f63  rom google.api_c
-00000890: 6f72 652e 6461 7465 7469 6d65 5f68 656c  ore.datetime_hel
-000008a0: 7065 7273 2069 6d70 6f72 7420 4461 7465  pers import Date
-000008b0: 7469 6d65 5769 7468 4e61 6e6f 7365 636f  timeWithNanoseco
-000008c0: 6e64 730a 0a66 726f 6d20 676f 6f67 6c65  nds..from google
-000008d0: 2e63 6c6f 7564 2069 6d70 6f72 7420 7370  .cloud import sp
-000008e0: 616e 6e65 725f 6462 6170 690a 0a66 726f  anner_dbapi..fro
-000008f0: 6d20 7371 6c61 6c63 6865 6d79 2e74 6573  m sqlalchemy.tes
-00000900: 7469 6e67 2e73 7569 7465 2e74 6573 745f  ting.suite.test_
-00000910: 6374 6520 696d 706f 7274 202a 2020 2320  cte import *  # 
-00000920: 6e6f 7161 3a20 4634 3031 2c20 4634 3033  noqa: F401, F403
-00000930: 0a66 726f 6d20 7371 6c61 6c63 6865 6d79  .from sqlalchemy
-00000940: 2e74 6573 7469 6e67 2e73 7569 7465 2e74  .testing.suite.t
-00000950: 6573 745f 6464 6c20 696d 706f 7274 202a  est_ddl import *
-00000960: 2020 2320 6e6f 7161 3a20 4634 3031 2c20    # noqa: F401, 
-00000970: 4634 3033 0a66 726f 6d20 7371 6c61 6c63  F403.from sqlalc
-00000980: 6865 6d79 2e74 6573 7469 6e67 2e73 7569  hemy.testing.sui
-00000990: 7465 2e74 6573 745f 6469 616c 6563 7420  te.test_dialect 
-000009a0: 696d 706f 7274 202a 2020 2320 6e6f 7161  import *  # noqa
-000009b0: 3a20 4634 3031 2c20 4634 3033 0a66 726f  : F401, F403.fro
-000009c0: 6d20 7371 6c61 6c63 6865 6d79 2e74 6573  m sqlalchemy.tes
-000009d0: 7469 6e67 2e73 7569 7465 2e74 6573 745f  ting.suite.test_
-000009e0: 696e 7365 7274 2069 6d70 6f72 7420 2a20  insert import * 
-000009f0: 2023 206e 6f71 613a 2046 3430 312c 2046   # noqa: F401, F
-00000a00: 3430 330a 6672 6f6d 2073 716c 616c 6368  403.from sqlalch
-00000a10: 656d 792e 7465 7374 696e 672e 7375 6974  emy.testing.suit
-00000a20: 652e 7465 7374 5f72 6566 6c65 6374 696f  e.test_reflectio
-00000a30: 6e20 696d 706f 7274 202a 2020 2320 6e6f  n import *  # no
-00000a40: 7161 3a20 4634 3031 2c20 4634 3033 0a66  qa: F401, F403.f
-00000a50: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
-00000a60: 6573 7469 6e67 2e73 7569 7465 2e74 6573  esting.suite.tes
-00000a70: 745f 7265 7375 6c74 7320 696d 706f 7274  t_results import
-00000a80: 202a 2020 2320 6e6f 7161 3a20 4634 3031   *  # noqa: F401
-00000a90: 2c20 4634 3033 0a66 726f 6d20 7371 6c61  , F403.from sqla
-00000aa0: 6c63 6865 6d79 2e74 6573 7469 6e67 2e73  lchemy.testing.s
-00000ab0: 7569 7465 2e74 6573 745f 7365 6c65 6374  uite.test_select
-00000ac0: 2069 6d70 6f72 7420 2a20 2023 206e 6f71   import *  # noq
-00000ad0: 613a 2046 3430 312c 2046 3430 330a 6672  a: F401, F403.fr
-00000ae0: 6f6d 2073 716c 616c 6368 656d 792e 7465  om sqlalchemy.te
-00000af0: 7374 696e 672e 7375 6974 652e 7465 7374  sting.suite.test
-00000b00: 5f73 6571 7565 6e63 6520 696d 706f 7274  _sequence import
-00000b10: 202a 2020 2320 6e6f 7161 3a20 4634 3031   *  # noqa: F401
-00000b20: 2c20 4634 3033 0a66 726f 6d20 7371 6c61  , F403.from sqla
-00000b30: 6c63 6865 6d79 2e74 6573 7469 6e67 2e73  lchemy.testing.s
-00000b40: 7569 7465 2e74 6573 745f 7570 6461 7465  uite.test_update
-00000b50: 5f64 656c 6574 6520 696d 706f 7274 202a  _delete import *
-00000b60: 2020 2320 6e6f 7161 3a20 4634 3031 2c20    # noqa: F401, 
-00000b70: 4634 3033 0a66 726f 6d20 7371 6c61 6c63  F403.from sqlalc
-00000b80: 6865 6d79 2e74 6573 7469 6e67 2e73 7569  hemy.testing.sui
-00000b90: 7465 2e74 6573 745f 6374 6520 696d 706f  te.test_cte impo
-00000ba0: 7274 2043 5445 5465 7374 2061 7320 5f43  rt CTETest as _C
-00000bb0: 5445 5465 7374 0a66 726f 6d20 7371 6c61  TETest.from sqla
-00000bc0: 6c63 6865 6d79 2e74 6573 7469 6e67 2e73  lchemy.testing.s
-00000bd0: 7569 7465 2e74 6573 745f 6464 6c20 696d  uite.test_ddl im
-00000be0: 706f 7274 2054 6162 6c65 4444 4c54 6573  port TableDDLTes
-00000bf0: 7420 6173 205f 5461 626c 6544 444c 5465  t as _TableDDLTe
-00000c00: 7374 0a66 726f 6d20 7371 6c61 6c63 6865  st.from sqlalche
-00000c10: 6d79 2e74 6573 7469 6e67 2e73 7569 7465  my.testing.suite
-00000c20: 2e74 6573 745f 6464 6c20 696d 706f 7274  .test_ddl import
-00000c30: 2028 0a20 2020 2046 7574 7572 6554 6162   (.    FutureTab
-00000c40: 6c65 4444 4c54 6573 7420 6173 205f 4675  leDDLTest as _Fu
-00000c50: 7475 7265 5461 626c 6544 444c 5465 7374  tureTableDDLTest
-00000c60: 2c0a 2020 2020 4c6f 6e67 4e61 6d65 426c  ,.    LongNameBl
-00000c70: 6f77 6f75 7454 6573 7420 6173 205f 4c6f  owoutTest as _Lo
-00000c80: 6e67 4e61 6d65 426c 6f77 6f75 7454 6573  ngNameBlowoutTes
-00000c90: 742c 0a29 0a66 726f 6d20 7371 6c61 6c63  t,.).from sqlalc
-00000ca0: 6865 6d79 2e74 6573 7469 6e67 2e73 7569  hemy.testing.sui
-00000cb0: 7465 2e74 6573 745f 7570 6461 7465 5f64  te.test_update_d
-00000cc0: 656c 6574 6520 696d 706f 7274 2028 0a20  elete import (. 
-00000cd0: 2020 2053 696d 706c 6555 7064 6174 6544     SimpleUpdateD
-00000ce0: 656c 6574 6554 6573 7420 6173 205f 5369  eleteTest as _Si
-00000cf0: 6d70 6c65 5570 6461 7465 4465 6c65 7465  mpleUpdateDelete
-00000d00: 5465 7374 2c0a 290a 6672 6f6d 2073 716c  Test,.).from sql
-00000d10: 616c 6368 656d 792e 7465 7374 696e 672e  alchemy.testing.
-00000d20: 7375 6974 652e 7465 7374 5f64 6961 6c65  suite.test_diale
-00000d30: 6374 2069 6d70 6f72 7420 280a 2020 2020  ct import (.    
-00000d40: 4469 6666 6963 756c 7450 6172 616d 6574  DifficultParamet
-00000d50: 6572 7354 6573 7420 6173 205f 4469 6666  ersTest as _Diff
-00000d60: 6963 756c 7450 6172 616d 6574 6572 7354  icultParametersT
-00000d70: 6573 742c 0a20 2020 2045 7363 6170 696e  est,.    Escapin
-00000d80: 6754 6573 7420 6173 205f 4573 6361 7069  gTest as _Escapi
-00000d90: 6e67 5465 7374 2c0a 290a 6672 6f6d 2073  ngTest,.).from s
-00000da0: 716c 616c 6368 656d 792e 7465 7374 696e  qlalchemy.testin
-00000db0: 672e 7375 6974 652e 7465 7374 5f69 6e73  g.suite.test_ins
-00000dc0: 6572 7420 696d 706f 7274 2028 0a20 2020  ert import (.   
-00000dd0: 2049 6e73 6572 7442 6568 6176 696f 7254   InsertBehaviorT
-00000de0: 6573 7420 6173 205f 496e 7365 7274 4265  est as _InsertBe
-00000df0: 6861 7669 6f72 5465 7374 2c0a 290a 6672  haviorTest,.).fr
-00000e00: 6f6d 2073 716c 616c 6368 656d 792e 7465  om sqlalchemy.te
-00000e10: 7374 696e 672e 7375 6974 652e 7465 7374  sting.suite.test
-00000e20: 5f73 656c 6563 7420 696d 706f 7274 2028  _select import (
-00000e30: 2020 2320 6e6f 7161 3a20 4634 3031 2c20    # noqa: F401, 
-00000e40: 4634 3033 0a20 2020 2043 6f6d 706f 756e  F403.    Compoun
-00000e50: 6453 656c 6563 7454 6573 7420 6173 205f  dSelectTest as _
-00000e60: 436f 6d70 6f75 6e64 5365 6c65 6374 5465  CompoundSelectTe
-00000e70: 7374 2c0a 2020 2020 4578 6973 7473 5465  st,.    ExistsTe
-00000e80: 7374 2061 7320 5f45 7869 7374 7354 6573  st as _ExistsTes
-00000e90: 742c 0a20 2020 2046 6574 6368 4c69 6d69  t,.    FetchLimi
-00000ea0: 744f 6666 7365 7454 6573 7420 6173 205f  tOffsetTest as _
-00000eb0: 4665 7463 684c 696d 6974 4f66 6673 6574  FetchLimitOffset
-00000ec0: 5465 7374 2c0a 2020 2020 4964 656e 7469  Test,.    Identi
-00000ed0: 7479 4175 746f 696e 6372 656d 656e 7454  tyAutoincrementT
-00000ee0: 6573 7420 6173 205f 4964 656e 7469 7479  est as _Identity
-00000ef0: 4175 746f 696e 6372 656d 656e 7454 6573  AutoincrementTes
-00000f00: 742c 0a20 2020 2049 734f 7249 734e 6f74  t,.    IsOrIsNot
-00000f10: 4469 7374 696e 6374 4672 6f6d 5465 7374  DistinctFromTest
-00000f20: 2061 7320 5f49 734f 7249 734e 6f74 4469   as _IsOrIsNotDi
-00000f30: 7374 696e 6374 4672 6f6d 5465 7374 2c0a  stinctFromTest,.
-00000f40: 2020 2020 4c69 6b65 4675 6e63 7469 6f6e      LikeFunction
-00000f50: 7354 6573 7420 6173 205f 4c69 6b65 4675  sTest as _LikeFu
-00000f60: 6e63 7469 6f6e 7354 6573 742c 0a20 2020  nctionsTest,.   
-00000f70: 204f 7264 6572 4279 4c61 6265 6c54 6573   OrderByLabelTes
-00000f80: 7420 6173 205f 4f72 6465 7242 794c 6162  t as _OrderByLab
-00000f90: 656c 5465 7374 2c0a 2020 2020 506f 7374  elTest,.    Post
-00000fa0: 436f 6d70 696c 6550 6172 616d 7354 6573  CompileParamsTes
-00000fb0: 7420 6173 205f 506f 7374 436f 6d70 696c  t as _PostCompil
-00000fc0: 6550 6172 616d 7354 6573 742c 0a29 0a66  eParamsTest,.).f
-00000fd0: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
-00000fe0: 6573 7469 6e67 2e73 7569 7465 2e74 6573  esting.suite.tes
-00000ff0: 745f 7265 666c 6563 7469 6f6e 2069 6d70  t_reflection imp
-00001000: 6f72 7420 280a 2020 2020 436f 6d70 6f6e  ort (.    Compon
-00001010: 656e 7452 6566 6c65 6374 696f 6e54 6573  entReflectionTes
-00001020: 7445 7874 7261 2061 7320 5f43 6f6d 706f  tExtra as _Compo
-00001030: 6e65 6e74 5265 666c 6563 7469 6f6e 5465  nentReflectionTe
-00001040: 7374 4578 7472 612c 0a20 2020 2051 756f  stExtra,.    Quo
-00001050: 7465 644e 616d 6541 7267 756d 656e 7454  tedNameArgumentT
-00001060: 6573 7420 6173 205f 5175 6f74 6564 4e61  est as _QuotedNa
-00001070: 6d65 4172 6775 6d65 6e74 5465 7374 2c0a  meArgumentTest,.
-00001080: 2020 2020 436f 6d70 6f6e 656e 7452 6566      ComponentRef
-00001090: 6c65 6374 696f 6e54 6573 7420 6173 205f  lectionTest as _
-000010a0: 436f 6d70 6f6e 656e 7452 6566 6c65 6374  ComponentReflect
-000010b0: 696f 6e54 6573 742c 0a20 2020 2043 6f6d  ionTest,.    Com
-000010c0: 706f 7369 7465 4b65 7952 6566 6c65 6374  positeKeyReflect
-000010d0: 696f 6e54 6573 7420 6173 205f 436f 6d70  ionTest as _Comp
-000010e0: 6f73 6974 654b 6579 5265 666c 6563 7469  ositeKeyReflecti
-000010f0: 6f6e 5465 7374 2c0a 2020 2020 436f 6d70  onTest,.    Comp
-00001100: 7574 6564 5265 666c 6563 7469 6f6e 5465  utedReflectionTe
-00001110: 7374 2061 7320 5f43 6f6d 7075 7465 6452  st as _ComputedR
-00001120: 6566 6c65 6374 696f 6e54 6573 742c 0a20  eflectionTest,. 
-00001130: 2020 2048 6173 496e 6465 7854 6573 7420     HasIndexTest 
-00001140: 6173 205f 4861 7349 6e64 6578 5465 7374  as _HasIndexTest
-00001150: 2c0a 2020 2020 4861 7354 6162 6c65 5465  ,.    HasTableTe
-00001160: 7374 2061 7320 5f48 6173 5461 626c 6554  st as _HasTableT
-00001170: 6573 742c 0a29 0a66 726f 6d20 7371 6c61  est,.).from sqla
-00001180: 6c63 6865 6d79 2e74 6573 7469 6e67 2e73  lchemy.testing.s
-00001190: 7569 7465 2e74 6573 745f 7265 7375 6c74  uite.test_result
-000011a0: 7320 696d 706f 7274 2052 6f77 4665 7463  s import RowFetc
-000011b0: 6854 6573 7420 6173 205f 526f 7746 6574  hTest as _RowFet
-000011c0: 6368 5465 7374 0a66 726f 6d20 7371 6c61  chTest.from sqla
-000011d0: 6c63 6865 6d79 2e74 6573 7469 6e67 2e73  lchemy.testing.s
-000011e0: 7569 7465 2e74 6573 745f 7479 7065 7320  uite.test_types 
-000011f0: 696d 706f 7274 2028 2020 2320 6e6f 7161  import (  # noqa
-00001200: 3a20 4634 3031 2c20 4634 3033 0a20 2020  : F401, F403.   
-00001210: 2042 6f6f 6c65 616e 5465 7374 2061 7320   BooleanTest as 
-00001220: 5f42 6f6f 6c65 616e 5465 7374 2c0a 2020  _BooleanTest,.  
-00001230: 2020 4461 7465 5465 7374 2061 7320 5f44    DateTest as _D
-00001240: 6174 6554 6573 742c 0a20 2020 205f 4461  ateTest,.    _Da
-00001250: 7465 4669 7874 7572 6520 6173 205f 5f44  teFixture as __D
-00001260: 6174 6546 6978 7475 7265 2c0a 2020 2020  ateFixture,.    
-00001270: 4461 7465 5469 6d65 4869 7374 6f72 6963  DateTimeHistoric
-00001280: 5465 7374 2c0a 2020 2020 4461 7465 5469  Test,.    DateTi
-00001290: 6d65 436f 6572 6365 6454 6f44 6174 6554  meCoercedToDateT
-000012a0: 696d 6554 6573 7420 6173 205f 4461 7465  imeTest as _Date
-000012b0: 5469 6d65 436f 6572 6365 6454 6f44 6174  TimeCoercedToDat
-000012c0: 6554 696d 6554 6573 742c 0a20 2020 2044  eTimeTest,.    D
-000012d0: 6174 6554 696d 654d 6963 726f 7365 636f  ateTimeMicroseco
-000012e0: 6e64 7354 6573 7420 6173 205f 4461 7465  ndsTest as _Date
-000012f0: 5469 6d65 4d69 6372 6f73 6563 6f6e 6473  TimeMicroseconds
-00001300: 5465 7374 2c0a 2020 2020 4461 7465 5469  Test,.    DateTi
-00001310: 6d65 5465 7374 2061 7320 5f44 6174 6554  meTest as _DateT
-00001320: 696d 6554 6573 742c 0a20 2020 2049 6e74  imeTest,.    Int
-00001330: 6567 6572 5465 7374 2061 7320 5f49 6e74  egerTest as _Int
-00001340: 6567 6572 5465 7374 2c0a 2020 2020 4a53  egerTest,.    JS
-00001350: 4f4e 5465 7374 2061 7320 5f4a 534f 4e54  ONTest as _JSONT
-00001360: 6573 742c 0a20 2020 205f 4c69 7465 7261  est,.    _Litera
-00001370: 6c52 6f75 6e64 5472 6970 4669 7874 7572  lRoundTripFixtur
-00001380: 652c 0a20 2020 204e 756d 6572 6963 5465  e,.    NumericTe
-00001390: 7374 2061 7320 5f4e 756d 6572 6963 5465  st as _NumericTe
-000013a0: 7374 2c0a 2020 2020 5374 7269 6e67 5465  st,.    StringTe
-000013b0: 7374 2061 7320 5f53 7472 696e 6754 6573  st as _StringTes
-000013c0: 742c 0a20 2020 2054 6578 7454 6573 7420  t,.    TextTest 
-000013d0: 6173 205f 5465 7874 5465 7374 2c0a 2020  as _TextTest,.  
-000013e0: 2020 5469 6d65 5465 7374 2061 7320 5f54    TimeTest as _T
-000013f0: 696d 6554 6573 742c 0a20 2020 2054 696d  imeTest,.    Tim
-00001400: 654d 6963 726f 7365 636f 6e64 7354 6573  eMicrosecondsTes
-00001410: 7420 6173 205f 5469 6d65 4d69 6372 6f73  t as _TimeMicros
-00001420: 6563 6f6e 6473 5465 7374 2c0a 2020 2020  econdsTest,.    
-00001430: 5469 6d65 7374 616d 704d 6963 726f 7365  TimestampMicrose
-00001440: 636f 6e64 7354 6573 742c 0a20 2020 2055  condsTest,.    U
-00001450: 6e69 636f 6465 5661 7263 6861 7254 6573  nicodeVarcharTes
-00001460: 7420 6173 205f 556e 6963 6f64 6556 6172  t as _UnicodeVar
-00001470: 6368 6172 5465 7374 2c0a 2020 2020 556e  charTest,.    Un
-00001480: 6963 6f64 6554 6578 7454 6573 7420 6173  icodeTextTest as
-00001490: 205f 556e 6963 6f64 6554 6578 7454 6573   _UnicodeTextTes
-000014a0: 742c 0a20 2020 205f 556e 6963 6f64 6546  t,.    _UnicodeF
-000014b0: 6978 7475 7265 2061 7320 5f5f 556e 6963  ixture as __Unic
-000014c0: 6f64 6546 6978 7475 7265 2c0a 290a 6672  odeFixture,.).fr
-000014d0: 6f6d 2074 6573 742e 5f68 656c 7065 7273  om test._helpers
-000014e0: 2069 6d70 6f72 7420 6765 745f 6462 5f75   import get_db_u
-000014f0: 726c 0a0a 636f 6e66 6967 2e74 6573 745f  rl..config.test_
-00001500: 7363 6865 6d61 203d 2022 220a 0a0a 636c  schema = ""...cl
-00001510: 6173 7320 426f 6f6c 6561 6e54 6573 7428  ass BooleanTest(
-00001520: 5f42 6f6f 6c65 616e 5465 7374 293a 0a20  _BooleanTest):. 
-00001530: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-00001540: 736b 6970 280a 2020 2020 2020 2020 2254  skip(.        "T
-00001550: 6865 206f 7269 6769 6e61 6c20 7465 7374  he original test
-00001560: 2063 6173 6520 7761 7320 7370 6c69 7420   case was split 
-00001570: 696e 746f 2032 2070 6172 7473 3a20 220a  into 2 parts: ".
-00001580: 2020 2020 2020 2020 2274 6573 745f 7265          "test_re
-00001590: 6e64 6572 5f6c 6974 6572 616c 5f62 6f6f  nder_literal_boo
-000015a0: 6c5f 7472 7565 2061 6e64 2074 6573 745f  l_true and test_
-000015b0: 7265 6e64 6572 5f6c 6974 6572 616c 5f62  render_literal_b
-000015c0: 6f6f 6c5f 6661 6c73 6522 0a20 2020 2029  ool_false".    )
-000015d0: 0a20 2020 2064 6566 2074 6573 745f 7265  .    def test_re
-000015e0: 6e64 6572 5f6c 6974 6572 616c 5f62 6f6f  nder_literal_boo
-000015f0: 6c28 7365 6c66 293a 0a20 2020 2020 2020  l(self):.       
-00001600: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
-00001610: 6573 745f 7265 6e64 6572 5f6c 6974 6572  est_render_liter
-00001620: 616c 5f62 6f6f 6c5f 7472 7565 2873 656c  al_bool_true(sel
-00001630: 662c 206c 6974 6572 616c 5f72 6f75 6e64  f, literal_round
-00001640: 5f74 7269 7029 3a0a 2020 2020 2020 2020  _trip):.        
-00001650: 2222 220a 2020 2020 2020 2020 5350 414e  """.        SPAN
-00001660: 4e45 5220 4f56 4552 5249 4445 3a0a 0a20  NER OVERRIDE:.. 
-00001670: 2020 2020 2020 2043 6c6f 7564 2053 7061         Cloud Spa
-00001680: 6e6e 6572 2073 7570 706f 7274 7320 7461  nner supports ta
-00001690: 626c 6573 2077 6974 6820 616e 2065 6d70  bles with an emp
-000016a0: 7479 2070 7269 6d61 7279 206b 6579 2c20  ty primary key, 
-000016b0: 6275 740a 2020 2020 2020 2020 6f6e 6c79  but.        only
-000016c0: 2061 2073 696e 676c 6520 726f 7720 6361   a single row ca
-000016d0: 6e20 6265 2069 6e73 6572 7465 6420 696e  n be inserted in
-000016e0: 746f 2073 7563 6820 6120 7461 626c 6520  to such a table 
-000016f0: 2d0a 2020 2020 2020 2020 666f 6c6c 6f77  -.        follow
-00001700: 696e 6720 696e 7365 7274 696f 6e73 2077  ing insertions w
-00001710: 696c 6c20 6661 696c 2077 6974 6820 6052  ill fail with `R
-00001720: 6f77 205b 5d20 616c 7265 6164 7920 6578  ow [] already ex
-00001730: 6973 7473 222e 0a20 2020 2020 2020 204f  ists"..        O
-00001740: 7665 7272 6964 696e 6720 7468 6520 7465  verriding the te
-00001750: 7374 2074 6f20 6176 6f69 6420 7468 6520  st to avoid the 
-00001760: 7361 6d65 2066 6169 6c75 7265 2e0a 2020  same failure..  
-00001770: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00001780: 2020 6c69 7465 7261 6c5f 726f 756e 645f    literal_round_
-00001790: 7472 6970 2842 6f6f 6c65 616e 2829 2c20  trip(Boolean(), 
-000017a0: 5b54 7275 655d 2c20 5b54 7275 655d 290a  [True], [True]).
-000017b0: 0a20 2020 2064 6566 2074 6573 745f 7265  .    def test_re
-000017c0: 6e64 6572 5f6c 6974 6572 616c 5f62 6f6f  nder_literal_boo
-000017d0: 6c5f 6661 6c73 6528 7365 6c66 2c20 6c69  l_false(self, li
-000017e0: 7465 7261 6c5f 726f 756e 645f 7472 6970  teral_round_trip
-000017f0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00001800: 2020 2020 2020 2053 5041 4e4e 4552 204f         SPANNER O
-00001810: 5645 5252 4944 453a 0a0a 2020 2020 2020  VERRIDE:..      
-00001820: 2020 436c 6f75 6420 5370 616e 6e65 7220    Cloud Spanner 
-00001830: 7375 7070 6f72 7473 2074 6162 6c65 7320  supports tables 
-00001840: 7769 7468 2061 6e20 656d 7074 7920 7072  with an empty pr
-00001850: 696d 6172 7920 6b65 792c 2062 7574 0a20  imary key, but. 
-00001860: 2020 2020 2020 206f 6e6c 7920 6120 7369         only a si
-00001870: 6e67 6c65 2072 6f77 2063 616e 2062 6520  ngle row can be 
-00001880: 696e 7365 7274 6564 2069 6e74 6f20 7375  inserted into su
-00001890: 6368 2061 2074 6162 6c65 202d 0a20 2020  ch a table -.   
-000018a0: 2020 2020 2066 6f6c 6c6f 7769 6e67 2069       following i
-000018b0: 6e73 6572 7469 6f6e 7320 7769 6c6c 2066  nsertions will f
-000018c0: 6169 6c20 7769 7468 2060 526f 7720 5b5d  ail with `Row []
-000018d0: 2061 6c72 6561 6479 2065 7869 7374 7322   already exists"
-000018e0: 2e0a 2020 2020 2020 2020 4f76 6572 7269  ..        Overri
-000018f0: 6469 6e67 2074 6865 2074 6573 7420 746f  ding the test to
-00001900: 2061 766f 6964 2074 6865 2073 616d 6520   avoid the same 
-00001910: 6661 696c 7572 652e 0a20 2020 2020 2020  failure..       
-00001920: 2022 2222 0a20 2020 2020 2020 206c 6974   """.        lit
-00001930: 6572 616c 5f72 6f75 6e64 5f74 7269 7028  eral_round_trip(
-00001940: 426f 6f6c 6561 6e28 292c 205b 4661 6c73  Boolean(), [Fals
-00001950: 655d 2c20 5b46 616c 7365 5d29 0a0a 2020  e], [False])..  
-00001960: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
-00001970: 6b69 7028 224e 6f74 2073 7570 706f 7274  kip("Not support
-00001980: 6564 2062 7920 436c 6f75 6420 5370 616e  ed by Cloud Span
-00001990: 6e65 7222 290a 2020 2020 6465 6620 7465  ner").    def te
-000019a0: 7374 5f77 6865 7265 636c 6175 7365 2873  st_whereclause(s
-000019b0: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-000019c0: 7373 0a0a 0a63 6c61 7373 2043 6f6d 706f  ss...class Compo
-000019d0: 6e65 6e74 5265 666c 6563 7469 6f6e 5465  nentReflectionTe
-000019e0: 7374 4578 7472 6128 5f43 6f6d 706f 6e65  stExtra(_Compone
-000019f0: 6e74 5265 666c 6563 7469 6f6e 5465 7374  ntReflectionTest
-00001a00: 4578 7472 6129 3a0a 2020 2020 4074 6573  Extra):.    @tes
-00001a10: 7469 6e67 2e72 6571 7569 7265 732e 7461  ting.requires.ta
-00001a20: 626c 655f 7265 666c 6563 7469 6f6e 0a20  ble_reflection. 
-00001a30: 2020 2064 6566 2074 6573 745f 6e75 6c6c     def test_null
-00001a40: 6162 6c65 5f72 6566 6c65 6374 696f 6e28  able_reflection(
-00001a50: 7365 6c66 2c20 636f 6e6e 6563 7469 6f6e  self, connection
-00001a60: 2c20 6d65 7461 6461 7461 293a 0a20 2020  , metadata):.   
-00001a70: 2020 2020 2074 203d 2054 6162 6c65 280a       t = Table(.
-00001a80: 2020 2020 2020 2020 2020 2020 2274 222c              "t",
-00001a90: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
-00001aa0: 6164 6174 612c 0a20 2020 2020 2020 2020  adata,.         
-00001ab0: 2020 2043 6f6c 756d 6e28 2261 222c 2049     Column("a", I
-00001ac0: 6e74 6567 6572 2c20 6e75 6c6c 6162 6c65  nteger, nullable
-00001ad0: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
-00001ae0: 2020 2020 436f 6c75 6d6e 2822 6222 2c20      Column("b", 
-00001af0: 496e 7465 6765 722c 206e 756c 6c61 626c  Integer, nullabl
-00001b00: 653d 4661 6c73 6529 2c0a 2020 2020 2020  e=False),.      
-00001b10: 2020 290a 2020 2020 2020 2020 742e 6372    ).        t.cr
-00001b20: 6561 7465 2863 6f6e 6e65 6374 696f 6e29  eate(connection)
-00001b30: 0a20 2020 2020 2020 2063 6f6e 6e65 6374  .        connect
-00001b40: 696f 6e2e 636f 6e6e 6563 7469 6f6e 2e63  ion.connection.c
-00001b50: 6f6d 6d69 7428 290a 2020 2020 2020 2020  ommit().        
-00001b60: 6571 5f28 0a20 2020 2020 2020 2020 2020  eq_(.           
-00001b70: 2064 6963 7428 0a20 2020 2020 2020 2020   dict(.         
-00001b80: 2020 2020 2020 2028 636f 6c5b 226e 616d         (col["nam
-00001b90: 6522 5d2c 2063 6f6c 5b22 6e75 6c6c 6162  e"], col["nullab
-00001ba0: 6c65 225d 290a 2020 2020 2020 2020 2020  le"]).          
-00001bb0: 2020 2020 2020 666f 7220 636f 6c20 696e        for col in
-00001bc0: 2069 6e73 7065 6374 2863 6f6e 6e65 6374   inspect(connect
-00001bd0: 696f 6e29 2e67 6574 5f63 6f6c 756d 6e73  ion).get_columns
-00001be0: 2822 7422 290a 2020 2020 2020 2020 2020  ("t").          
-00001bf0: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-00001c00: 207b 2261 223a 2054 7275 652c 2022 6222   {"a": True, "b"
-00001c10: 3a20 4661 6c73 657d 2c0a 2020 2020 2020  : False},.      
-00001c20: 2020 290a 0a20 2020 2064 6566 205f 7479    )..    def _ty
-00001c30: 7065 5f72 6f75 6e64 5f74 7269 7028 7365  pe_round_trip(se
-00001c40: 6c66 2c20 636f 6e6e 6563 7469 6f6e 2c20  lf, connection, 
-00001c50: 6d65 7461 6461 7461 2c20 2a74 7970 6573  metadata, *types
-00001c60: 293a 0a20 2020 2020 2020 2074 203d 2054  ):.        t = T
-00001c70: 6162 6c65 280a 2020 2020 2020 2020 2020  able(.          
-00001c80: 2020 2274 222c 206d 6574 6164 6174 612c    "t", metadata,
-00001c90: 202a 5b43 6f6c 756d 6e28 2274 2564 2220   *[Column("t%d" 
-00001ca0: 2520 692c 2074 7970 655f 2920 666f 7220  % i, type_) for 
-00001cb0: 692c 2074 7970 655f 2069 6e20 656e 756d  i, type_ in enum
-00001cc0: 6572 6174 6528 7479 7065 7329 5d0a 2020  erate(types)].  
-00001cd0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00001ce0: 742e 6372 6561 7465 2863 6f6e 6e65 6374  t.create(connect
-00001cf0: 696f 6e29 0a20 2020 2020 2020 2063 6f6e  ion).        con
-00001d00: 6e65 6374 696f 6e2e 636f 6e6e 6563 7469  nection.connecti
-00001d10: 6f6e 2e63 6f6d 6d69 7428 290a 0a20 2020  on.commit()..   
-00001d20: 2020 2020 2072 6574 7572 6e20 5b63 5b22       return [c["
-00001d30: 7479 7065 225d 2066 6f72 2063 2069 6e20  type"] for c in 
-00001d40: 696e 7370 6563 7428 636f 6e6e 6563 7469  inspect(connecti
-00001d50: 6f6e 292e 6765 745f 636f 6c75 6d6e 7328  on).get_columns(
-00001d60: 2274 2229 5d0a 0a20 2020 2040 7465 7374  "t")]..    @test
-00001d70: 696e 672e 7265 7175 6972 6573 2e74 6162  ing.requires.tab
-00001d80: 6c65 5f72 6566 6c65 6374 696f 6e0a 2020  le_reflection.  
-00001d90: 2020 6465 6620 7465 7374 5f6e 756d 6572    def test_numer
-00001da0: 6963 5f72 6566 6c65 6374 696f 6e28 7365  ic_reflection(se
-00001db0: 6c66 2c20 636f 6e6e 6563 7469 6f6e 2c20  lf, connection, 
-00001dc0: 6d65 7461 6461 7461 293a 0a20 2020 2020  metadata):.     
-00001dd0: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
-00001de0: 5041 4e4e 4552 204f 5645 5252 4944 453a  PANNER OVERRIDE:
-00001df0: 0a0a 2020 2020 2020 2020 5370 616e 6e65  ..        Spanne
-00001e00: 7220 6465 6669 6e65 7320 4e55 4d45 5249  r defines NUMERI
-00001e10: 4320 7479 7065 2077 6974 6820 7468 6520  C type with the 
-00001e20: 636f 6e73 7461 6e74 2070 7265 6369 7369  constant precisi
-00001e30: 6f6e 3d33 380a 2020 2020 2020 2020 616e  on=38.        an
-00001e40: 6420 7363 616c 653d 392e 204f 7665 7272  d scale=9. Overr
-00001e50: 6964 696e 6720 7468 6520 7465 7374 2074  iding the test t
-00001e60: 6f20 6368 6563 6b20 6966 2074 6865 204e  o check if the N
-00001e70: 554d 4552 4943 0a20 2020 2020 2020 2063  UMERIC.        c
-00001e80: 6f6c 756d 6e20 6973 2073 7563 6365 7373  olumn is success
-00001e90: 6675 6c6c 7920 6372 6561 7465 6420 616e  fully created an
-00001ea0: 6420 6861 7320 6469 6d65 6e73 696f 6e73  d has dimensions
-00001eb0: 0a20 2020 2020 2020 2063 6f72 7265 6374  .        correct
-00001ec0: 2066 6f72 2043 6c6f 7564 2053 7061 6e6e   for Cloud Spann
-00001ed0: 6572 2e0a 2020 2020 2020 2020 2222 220a  er..        """.
-00001ee0: 2020 2020 2020 2020 666f 7220 7479 7020          for typ 
-00001ef0: 696e 2073 656c 662e 5f74 7970 655f 726f  in self._type_ro
-00001f00: 756e 645f 7472 6970 2863 6f6e 6e65 6374  und_trip(connect
-00001f10: 696f 6e2c 206d 6574 6164 6174 612c 204e  ion, metadata, N
-00001f20: 756d 6572 6963 2831 382c 2035 2929 3a0a  umeric(18, 5)):.
-00001f30: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00001f40: 7274 2069 7369 6e73 7461 6e63 6528 7479  rt isinstance(ty
-00001f50: 702c 204e 756d 6572 6963 290a 2020 2020  p, Numeric).    
-00001f60: 2020 2020 2020 2020 6571 5f28 7479 702e          eq_(typ.
-00001f70: 7072 6563 6973 696f 6e2c 2033 3829 0a20  precision, 38). 
-00001f80: 2020 2020 2020 2020 2020 2065 715f 2874             eq_(t
-00001f90: 7970 2e73 6361 6c65 2c20 3929 0a0a 2020  yp.scale, 9)..  
-00001fa0: 2020 4074 6573 7469 6e67 2e72 6571 7569    @testing.requi
-00001fb0: 7265 732e 7461 626c 655f 7265 666c 6563  res.table_reflec
-00001fc0: 7469 6f6e 0a20 2020 2064 6566 2074 6573  tion.    def tes
-00001fd0: 745f 6269 6e61 7279 5f72 6566 6c65 6374  t_binary_reflect
-00001fe0: 696f 6e28 7365 6c66 2c20 636f 6e6e 6563  ion(self, connec
-00001ff0: 7469 6f6e 2c20 6d65 7461 6461 7461 293a  tion, metadata):
-00002000: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00002010: 2020 2020 2043 6865 636b 2074 6861 7420       Check that 
-00002020: 6120 4259 5445 5320 636f 6c75 6d6e 2077  a BYTES column w
-00002030: 6974 6820 616e 2065 7870 6c69 6369 746c  ith an explicitl
-00002040: 790a 2020 2020 2020 2020 7365 7420 7369  y.        set si
-00002050: 7a65 2069 7320 636f 7272 6563 746c 7920  ze is correctly 
-00002060: 7265 666c 6563 7465 642e 0a20 2020 2020  reflected..     
-00002070: 2020 2022 2222 0a20 2020 2020 2020 2066     """.        f
-00002080: 6f72 2074 7970 2069 6e20 7365 6c66 2e5f  or typ in self._
-00002090: 7479 7065 5f72 6f75 6e64 5f74 7269 7028  type_round_trip(
-000020a0: 636f 6e6e 6563 7469 6f6e 2c20 6d65 7461  connection, meta
-000020b0: 6461 7461 2c20 4c61 7267 6542 696e 6172  data, LargeBinar
-000020c0: 7928 3230 2929 3a0a 2020 2020 2020 2020  y(20)):.        
-000020d0: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
-000020e0: 7461 6e63 6528 7479 702c 204c 6172 6765  tance(typ, Large
-000020f0: 4269 6e61 7279 290a 2020 2020 2020 2020  Binary).        
-00002100: 2020 2020 6571 5f28 7479 702e 6c65 6e67      eq_(typ.leng
-00002110: 7468 2c20 3230 290a 0a0a 636c 6173 7320  th, 20)...class 
-00002120: 436f 6d70 6f6e 656e 7452 6566 6c65 6374  ComponentReflect
-00002130: 696f 6e54 6573 7428 5f43 6f6d 706f 6e65  ionTest(_Compone
-00002140: 6e74 5265 666c 6563 7469 6f6e 5465 7374  ntReflectionTest
-00002150: 293a 0a20 2020 2040 636c 6173 736d 6574  ):.    @classmet
-00002160: 686f 640a 2020 2020 6465 6620 6465 6669  hod.    def defi
-00002170: 6e65 5f74 6162 6c65 7328 636c 732c 206d  ne_tables(cls, m
-00002180: 6574 6164 6174 6129 3a0a 2020 2020 2020  etadata):.      
-00002190: 2020 636c 732e 6465 6669 6e65 5f72 6566    cls.define_ref
-000021a0: 6c65 6374 6564 5f74 6162 6c65 7328 6d65  lected_tables(me
-000021b0: 7461 6461 7461 2c20 4e6f 6e65 290a 0a20  tadata, None).. 
-000021c0: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-000021d0: 2020 2020 6465 6620 6465 6669 6e65 5f72      def define_r
-000021e0: 6566 6c65 6374 6564 5f74 6162 6c65 7328  eflected_tables(
-000021f0: 636c 732c 206d 6574 6164 6174 612c 2073  cls, metadata, s
-00002200: 6368 656d 6129 3a0a 2020 2020 2020 2020  chema):.        
-00002210: 6966 2073 6368 656d 613a 0a20 2020 2020  if schema:.     
-00002220: 2020 2020 2020 2073 6368 656d 615f 7072         schema_pr
-00002230: 6566 6978 203d 2073 6368 656d 6120 2b20  efix = schema + 
-00002240: 222e 220a 2020 2020 2020 2020 656c 7365  ".".        else
-00002250: 3a0a 2020 2020 2020 2020 2020 2020 7363  :.            sc
-00002260: 6865 6d61 5f70 7265 6669 7820 3d20 2222  hema_prefix = ""
-00002270: 0a0a 2020 2020 2020 2020 6966 2074 6573  ..        if tes
-00002280: 7469 6e67 2e72 6571 7569 7265 732e 7365  ting.requires.se
-00002290: 6c66 5f72 6566 6572 656e 7469 616c 5f66  lf_referential_f
-000022a0: 6f72 6569 676e 5f6b 6579 732e 656e 6162  oreign_keys.enab
-000022b0: 6c65 643a 0a20 2020 2020 2020 2020 2020  led:.           
-000022c0: 2075 7365 7273 203d 2054 6162 6c65 280a   users = Table(.
-000022d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022e0: 2275 7365 7273 222c 0a20 2020 2020 2020  "users",.       
-000022f0: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
-00002300: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
-00002310: 2020 2043 6f6c 756d 6e28 2275 7365 725f     Column("user_
-00002320: 6964 222c 2073 716c 616c 6368 656d 792e  id", sqlalchemy.
-00002330: 494e 542c 2070 7269 6d61 7279 5f6b 6579  INT, primary_key
-00002340: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
-00002350: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
-00002360: 7465 7374 3122 2c20 7371 6c61 6c63 6865  test1", sqlalche
-00002370: 6d79 2e43 4841 5228 3529 2c20 6e75 6c6c  my.CHAR(5), null
-00002380: 6162 6c65 3d46 616c 7365 292c 0a20 2020  able=False),.   
-00002390: 2020 2020 2020 2020 2020 2020 2043 6f6c               Col
-000023a0: 756d 6e28 2274 6573 7432 222c 2073 716c  umn("test2", sql
-000023b0: 616c 6368 656d 792e 466c 6f61 7428 3529  alchemy.Float(5)
-000023c0: 2c20 6e75 6c6c 6162 6c65 3d46 616c 7365  , nullable=False
-000023d0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-000023e0: 2020 2043 6f6c 756d 6e28 0a20 2020 2020     Column(.     
-000023f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002400: 7061 7265 6e74 5f75 7365 725f 6964 222c  parent_user_id",
-00002410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002420: 2020 2020 2073 716c 616c 6368 656d 792e       sqlalchemy.
-00002430: 496e 7465 6765 722c 0a20 2020 2020 2020  Integer,.       
-00002440: 2020 2020 2020 2020 2020 2020 2073 716c               sql
-00002450: 616c 6368 656d 792e 466f 7265 6967 6e4b  alchemy.ForeignK
-00002460: 6579 280a 2020 2020 2020 2020 2020 2020  ey(.            
-00002470: 2020 2020 2020 2020 2020 2020 2225 7375              "%su
-00002480: 7365 7273 2e75 7365 725f 6964 2220 2520  sers.user_id" % 
-00002490: 7363 6865 6d61 5f70 7265 6669 782c 206e  schema_prefix, n
-000024a0: 616d 653d 2275 7365 725f 6964 5f66 6b22  ame="user_id_fk"
-000024b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000024c0: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-000024d0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-000024e0: 2020 2020 2020 2020 2020 2073 6368 656d             schem
-000024f0: 613d 7363 6865 6d61 2c0a 2020 2020 2020  a=schema,.      
-00002500: 2020 2020 2020 2020 2020 7465 7374 5f6e            test_n
-00002510: 6565 6473 5f66 6b3d 5472 7565 2c0a 2020  eeds_fk=True,.  
-00002520: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00002530: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00002540: 2020 2020 2020 7573 6572 7320 3d20 5461        users = Ta
-00002550: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
-00002560: 2020 2020 2022 7573 6572 7322 2c0a 2020       "users",.  
-00002570: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-00002580: 7461 6461 7461 2c0a 2020 2020 2020 2020  tadata,.        
-00002590: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
-000025a0: 7573 6572 5f69 6422 2c20 7371 6c61 6c63  user_id", sqlalc
-000025b0: 6865 6d79 2e49 4e54 2c20 7072 696d 6172  hemy.INT, primar
-000025c0: 795f 6b65 793d 5472 7565 292c 0a20 2020  y_key=True),.   
-000025d0: 2020 2020 2020 2020 2020 2020 2043 6f6c               Col
-000025e0: 756d 6e28 2274 6573 7431 222c 2073 716c  umn("test1", sql
-000025f0: 616c 6368 656d 792e 4348 4152 2835 292c  alchemy.CHAR(5),
-00002600: 206e 756c 6c61 626c 653d 4661 6c73 6529   nullable=False)
-00002610: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002620: 2020 436f 6c75 6d6e 2822 7465 7374 3222    Column("test2"
-00002630: 2c20 7371 6c61 6c63 6865 6d79 2e46 6c6f  , sqlalchemy.Flo
-00002640: 6174 2835 292c 206e 756c 6c61 626c 653d  at(5), nullable=
-00002650: 4661 6c73 6529 2c0a 2020 2020 2020 2020  False),.        
-00002660: 2020 2020 2020 2020 7363 6865 6d61 3d73          schema=s
-00002670: 6368 656d 612c 0a20 2020 2020 2020 2020  chema,.         
-00002680: 2020 2020 2020 2074 6573 745f 6e65 6564         test_need
-00002690: 735f 666b 3d54 7275 652c 0a20 2020 2020  s_fk=True,.     
-000026a0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-000026b0: 2020 5461 626c 6528 0a20 2020 2020 2020    Table(.       
-000026c0: 2020 2020 2022 6469 6e67 616c 696e 6773       "dingalings
-000026d0: 222c 0a20 2020 2020 2020 2020 2020 206d  ",.            m
-000026e0: 6574 6164 6174 612c 0a20 2020 2020 2020  etadata,.       
-000026f0: 2020 2020 2043 6f6c 756d 6e28 2264 696e       Column("din
-00002700: 6761 6c69 6e67 5f69 6422 2c20 7371 6c61  galing_id", sqla
-00002710: 6c63 6865 6d79 2e49 6e74 6567 6572 2c20  lchemy.Integer, 
-00002720: 7072 696d 6172 795f 6b65 793d 5472 7565  primary_key=True
-00002730: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
-00002740: 6f6c 756d 6e28 0a20 2020 2020 2020 2020  olumn(.         
-00002750: 2020 2020 2020 2022 6164 6472 6573 735f         "address_
-00002760: 6964 222c 0a20 2020 2020 2020 2020 2020  id",.           
-00002770: 2020 2020 2073 716c 616c 6368 656d 792e       sqlalchemy.
-00002780: 496e 7465 6765 722c 0a20 2020 2020 2020  Integer,.       
-00002790: 2020 2020 2020 2020 2073 716c 616c 6368           sqlalch
-000027a0: 656d 792e 466f 7265 6967 6e4b 6579 2822  emy.ForeignKey("
-000027b0: 2573 656d 6169 6c5f 6164 6472 6573 7365  %semail_addresse
-000027c0: 732e 6164 6472 6573 735f 6964 2220 2520  s.address_id" % 
-000027d0: 7363 6865 6d61 5f70 7265 6669 7829 2c0a  schema_prefix),.
-000027e0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-000027f0: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
-00002800: 6e28 2264 6174 6122 2c20 7371 6c61 6c63  n("data", sqlalc
-00002810: 6865 6d79 2e53 7472 696e 6728 3330 2929  hemy.String(30))
-00002820: 2c0a 2020 2020 2020 2020 2020 2020 7363  ,.            sc
-00002830: 6865 6d61 3d73 6368 656d 612c 0a20 2020  hema=schema,.   
-00002840: 2020 2020 2020 2020 2074 6573 745f 6e65           test_ne
-00002850: 6564 735f 666b 3d54 7275 652c 0a20 2020  eds_fk=True,.   
-00002860: 2020 2020 2029 0a20 2020 2020 2020 2054       ).        T
-00002870: 6162 6c65 280a 2020 2020 2020 2020 2020  able(.          
-00002880: 2020 2265 6d61 696c 5f61 6464 7265 7373    "email_address
-00002890: 6573 222c 0a20 2020 2020 2020 2020 2020  es",.           
-000028a0: 206d 6574 6164 6174 612c 0a20 2020 2020   metadata,.     
-000028b0: 2020 2020 2020 2043 6f6c 756d 6e28 2261         Column("a
-000028c0: 6464 7265 7373 5f69 6422 2c20 7371 6c61  ddress_id", sqla
-000028d0: 6c63 6865 6d79 2e49 6e74 6567 6572 2c20  lchemy.Integer, 
-000028e0: 7072 696d 6172 795f 6b65 793d 5472 7565  primary_key=True
-000028f0: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
-00002900: 6f6c 756d 6e28 0a20 2020 2020 2020 2020  olumn(.         
-00002910: 2020 2020 2020 2022 7265 6d6f 7465 5f75         "remote_u
-00002920: 7365 725f 6964 222c 0a20 2020 2020 2020  ser_id",.       
-00002930: 2020 2020 2020 2020 2073 716c 616c 6368           sqlalch
-00002940: 656d 792e 496e 7465 6765 722c 0a20 2020  emy.Integer,.   
-00002950: 2020 2020 2020 2020 2020 2020 2073 716c               sql
-00002960: 616c 6368 656d 792e 466f 7265 6967 6e4b  alchemy.ForeignK
-00002970: 6579 2875 7365 7273 2e63 2e75 7365 725f  ey(users.c.user_
-00002980: 6964 292c 0a20 2020 2020 2020 2020 2020  id),.           
-00002990: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-000029a0: 436f 6c75 6d6e 2822 656d 6169 6c5f 6164  Column("email_ad
-000029b0: 6472 6573 7322 2c20 7371 6c61 6c63 6865  dress", sqlalche
-000029c0: 6d79 2e53 7472 696e 6728 3230 2929 2c0a  my.String(20)),.
-000029d0: 2020 2020 2020 2020 2020 2020 7371 6c61              sqla
-000029e0: 6c63 6865 6d79 2e50 7269 6d61 7279 4b65  lchemy.PrimaryKe
-000029f0: 7943 6f6e 7374 7261 696e 7428 2261 6464  yConstraint("add
-00002a00: 7265 7373 5f69 6422 2c20 6e61 6d65 3d22  ress_id", name="
-00002a10: 656d 6169 6c5f 6164 5f70 6b22 292c 0a20  email_ad_pk"),. 
-00002a20: 2020 2020 2020 2020 2020 2073 6368 656d             schem
-00002a30: 613d 7363 6865 6d61 2c0a 2020 2020 2020  a=schema,.      
-00002a40: 2020 2020 2020 7465 7374 5f6e 6565 6473        test_needs
-00002a50: 5f66 6b3d 5472 7565 2c0a 2020 2020 2020  _fk=True,.      
-00002a60: 2020 290a 2020 2020 2020 2020 5461 626c    ).        Tabl
-00002a70: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
-00002a80: 636f 6d6d 656e 745f 7465 7374 222c 0a20  comment_test",. 
-00002a90: 2020 2020 2020 2020 2020 206d 6574 6164             metad
-00002aa0: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-00002ab0: 2043 6f6c 756d 6e28 2269 6422 2c20 7371   Column("id", sq
-00002ac0: 6c61 6c63 6865 6d79 2e49 6e74 6567 6572  lalchemy.Integer
-00002ad0: 2c20 7072 696d 6172 795f 6b65 793d 5472  , primary_key=Tr
-00002ae0: 7565 2c20 636f 6d6d 656e 743d 2269 6420  ue, comment="id 
-00002af0: 636f 6d6d 656e 7422 292c 0a20 2020 2020  comment"),.     
-00002b00: 2020 2020 2020 2043 6f6c 756d 6e28 2264         Column("d
-00002b10: 6174 6122 2c20 7371 6c61 6c63 6865 6d79  ata", sqlalchemy
-00002b20: 2e53 7472 696e 6728 3230 292c 2063 6f6d  .String(20), com
-00002b30: 6d65 6e74 3d22 6461 7461 2025 2063 6f6d  ment="data % com
-00002b40: 6d65 6e74 2229 2c0a 2020 2020 2020 2020  ment"),.        
-00002b50: 2020 2020 436f 6c75 6d6e 280a 2020 2020      Column(.    
-00002b60: 2020 2020 2020 2020 2020 2020 2264 3222              "d2"
-00002b70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002b80: 2020 7371 6c61 6c63 6865 6d79 2e53 7472    sqlalchemy.Str
-00002b90: 696e 6728 3230 292c 0a20 2020 2020 2020  ing(20),.       
-00002ba0: 2020 2020 2020 2020 2063 6f6d 6d65 6e74           comment
-00002bb0: 3d72 2222 2243 6f6d 6d65 6e74 2074 7970  =r"""Comment typ
-00002bc0: 6573 2074 7970 6520 7370 6565 6469 6c79  es type speedily
-00002bd0: 2027 2022 205c 2027 2720 4675 6e21 2222   ' " \ '' Fun!""
-00002be0: 222c 0a20 2020 2020 2020 2020 2020 2029  ",.            )
-00002bf0: 2c0a 2020 2020 2020 2020 2020 2020 7363  ,.            sc
-00002c00: 6865 6d61 3d73 6368 656d 612c 0a20 2020  hema=schema,.   
-00002c10: 2020 2020 2020 2020 2063 6f6d 6d65 6e74           comment
-00002c20: 3d72 2222 2274 6865 2074 6573 7420 2520  =r"""the test % 
-00002c30: 2720 2220 5c20 7461 626c 6520 636f 6d6d  ' " \ table comm
-00002c40: 656e 7422 2222 2c0a 2020 2020 2020 2020  ent""",.        
-00002c50: 290a 0a20 2020 2020 2020 2069 6620 7465  )..        if te
-00002c60: 7374 696e 672e 7265 7175 6972 6573 2e63  sting.requires.c
-00002c70: 726f 7373 5f73 6368 656d 615f 666b 5f72  ross_schema_fk_r
-00002c80: 6566 6c65 6374 696f 6e2e 656e 6162 6c65  eflection.enable
-00002c90: 643a 0a20 2020 2020 2020 2020 2020 2069  d:.            i
-00002ca0: 6620 7363 6865 6d61 2069 7320 4e6f 6e65  f schema is None
-00002cb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002cc0: 2020 5461 626c 6528 0a20 2020 2020 2020    Table(.       
-00002cd0: 2020 2020 2020 2020 2020 2020 2022 6c6f               "lo
-00002ce0: 6361 6c5f 7461 626c 6522 2c0a 2020 2020  cal_table",.    
-00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d00: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
-00002d10: 2020 2020 2020 2020 2020 2020 2020 436f                Co
-00002d20: 6c75 6d6e 2822 6964 222c 2073 716c 616c  lumn("id", sqlal
-00002d30: 6368 656d 792e 496e 7465 6765 722c 2070  chemy.Integer, p
-00002d40: 7269 6d61 7279 5f6b 6579 3d54 7275 6529  rimary_key=True)
-00002d50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002d60: 2020 2020 2020 436f 6c75 6d6e 2822 6461        Column("da
-00002d70: 7461 222c 2073 716c 616c 6368 656d 792e  ta", sqlalchemy.
-00002d80: 5374 7269 6e67 2832 3029 292c 0a20 2020  String(20)),.   
-00002d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002da0: 2043 6f6c 756d 6e28 0a20 2020 2020 2020   Column(.       
-00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002dc0: 2022 7265 6d6f 7465 5f69 6422 2c0a 2020   "remote_id",.  
-00002dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002de0: 2020 2020 2020 466f 7265 6967 6e4b 6579        ForeignKey
-00002df0: 2822 2573 2e72 656d 6f74 655f 7461 626c  ("%s.remote_tabl
-00002e00: 655f 322e 6964 2220 2520 7465 7374 696e  e_2.id" % testin
-00002e10: 672e 636f 6e66 6967 2e74 6573 745f 7363  g.config.test_sc
-00002e20: 6865 6d61 292c 0a20 2020 2020 2020 2020  hema),.         
-00002e30: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
+00000320: 7565 7374 4f70 7469 6f6e 732c 2043 6c69  uestOptions, Cli
+00000330: 656e 740a 0a69 6d70 6f72 7420 7371 6c61  ent..import sqla
+00000340: 6c63 6865 6d79 0a66 726f 6d20 7371 6c61  lchemy.from sqla
+00000350: 6c63 6865 6d79 2069 6d70 6f72 7420 6372  lchemy import cr
+00000360: 6561 7465 5f65 6e67 696e 650a 6672 6f6d  eate_engine.from
+00000370: 2073 716c 616c 6368 656d 7920 696d 706f   sqlalchemy impo
+00000380: 7274 2069 6e73 7065 6374 0a66 726f 6d20  rt inspect.from 
+00000390: 7371 6c61 6c63 6865 6d79 2069 6d70 6f72  sqlalchemy impor
+000003a0: 7420 7465 7374 696e 670a 6672 6f6d 2073  t testing.from s
+000003b0: 716c 616c 6368 656d 7920 696d 706f 7274  qlalchemy import
+000003c0: 2046 6f72 6569 676e 4b65 790a 6672 6f6d   ForeignKey.from
+000003d0: 2073 716c 616c 6368 656d 7920 696d 706f   sqlalchemy impo
+000003e0: 7274 204d 6574 6144 6174 610a 6672 6f6d  rt MetaData.from
+000003f0: 2073 716c 616c 6368 656d 792e 7363 6865   sqlalchemy.sche
+00000400: 6d61 2069 6d70 6f72 7420 4444 4c0a 6672  ma import DDL.fr
+00000410: 6f6d 2073 716c 616c 6368 656d 792e 7363  om sqlalchemy.sc
+00000420: 6865 6d61 2069 6d70 6f72 7420 436f 6d70  hema import Comp
+00000430: 7574 6564 0a66 726f 6d20 7371 6c61 6c63  uted.from sqlalc
+00000440: 6865 6d79 2e74 6573 7469 6e67 2069 6d70  hemy.testing imp
+00000450: 6f72 7420 636f 6e66 6967 0a66 726f 6d20  ort config.from 
+00000460: 7371 6c61 6c63 6865 6d79 2e74 6573 7469  sqlalchemy.testi
+00000470: 6e67 2069 6d70 6f72 7420 656e 6769 6e65  ng import engine
+00000480: 730a 6672 6f6d 2073 716c 616c 6368 656d  s.from sqlalchem
+00000490: 792e 7465 7374 696e 6720 696d 706f 7274  y.testing import
+000004a0: 2065 715f 0a66 726f 6d20 7371 6c61 6c63   eq_.from sqlalc
+000004b0: 6865 6d79 2e74 6573 7469 6e67 2069 6d70  hemy.testing imp
+000004c0: 6f72 7420 7072 6f76 6964 655f 6d65 7461  ort provide_meta
+000004d0: 6461 7461 2c20 656d 6974 735f 7761 726e  data, emits_warn
+000004e0: 696e 670a 6672 6f6d 2073 716c 616c 6368  ing.from sqlalch
+000004f0: 656d 792e 7465 7374 696e 6720 696d 706f  emy.testing impo
+00000500: 7274 2066 6978 7475 7265 730a 6672 6f6d  rt fixtures.from
+00000510: 2073 716c 616c 6368 656d 792e 7465 7374   sqlalchemy.test
+00000520: 696e 672e 7072 6f76 6973 696f 6e20 696d  ing.provision im
+00000530: 706f 7274 2074 656d 705f 7461 626c 655f  port temp_table_
+00000540: 6b65 7977 6f72 645f 6172 6773 0a66 726f  keyword_args.fro
+00000550: 6d20 7371 6c61 6c63 6865 6d79 2e74 6573  m sqlalchemy.tes
+00000560: 7469 6e67 2e73 6368 656d 6120 696d 706f  ting.schema impo
+00000570: 7274 2043 6f6c 756d 6e0a 6672 6f6d 2073  rt Column.from s
+00000580: 716c 616c 6368 656d 792e 7465 7374 696e  qlalchemy.testin
+00000590: 672e 7363 6865 6d61 2069 6d70 6f72 7420  g.schema import 
+000005a0: 5461 626c 650a 6672 6f6d 2073 716c 616c  Table.from sqlal
+000005b0: 6368 656d 7920 696d 706f 7274 206c 6974  chemy import lit
+000005c0: 6572 616c 5f63 6f6c 756d 6e0a 6672 6f6d  eral_column.from
+000005d0: 2073 716c 616c 6368 656d 7920 696d 706f   sqlalchemy impo
+000005e0: 7274 2073 656c 6563 740a 6672 6f6d 2073  rt select.from s
+000005f0: 716c 616c 6368 656d 7920 696d 706f 7274  qlalchemy import
+00000600: 2075 7469 6c0a 6672 6f6d 2073 716c 616c   util.from sqlal
+00000610: 6368 656d 7920 696d 706f 7274 2075 6e69  chemy import uni
+00000620: 6f6e 0a66 726f 6d20 7371 6c61 6c63 6865  on.from sqlalche
+00000630: 6d79 2069 6d70 6f72 7420 6576 656e 740a  my import event.
+00000640: 6672 6f6d 2073 716c 616c 6368 656d 7920  from sqlalchemy 
+00000650: 696d 706f 7274 2065 7869 7374 730a 6672  import exists.fr
+00000660: 6f6d 2073 716c 616c 6368 656d 7920 696d  om sqlalchemy im
+00000670: 706f 7274 2042 6f6f 6c65 616e 0a66 726f  port Boolean.fro
+00000680: 6d20 7371 6c61 6c63 6865 6d79 2069 6d70  m sqlalchemy imp
+00000690: 6f72 7420 466c 6f61 740a 6672 6f6d 2073  ort Float.from s
+000006a0: 716c 616c 6368 656d 7920 696d 706f 7274  qlalchemy import
+000006b0: 204c 6172 6765 4269 6e61 7279 0a66 726f   LargeBinary.fro
+000006c0: 6d20 7371 6c61 6c63 6865 6d79 2069 6d70  m sqlalchemy imp
+000006d0: 6f72 7420 5374 7269 6e67 0a66 726f 6d20  ort String.from 
+000006e0: 7371 6c61 6c63 6865 6d79 2e65 7874 2e64  sqlalchemy.ext.d
+000006f0: 6563 6c61 7261 7469 7665 2069 6d70 6f72  eclarative impor
+00000700: 7420 6465 636c 6172 6174 6976 655f 6261  t declarative_ba
+00000710: 7365 0a66 726f 6d20 7371 6c61 6c63 6865  se.from sqlalche
+00000720: 6d79 2e6f 726d 2069 6d70 6f72 7420 7265  my.orm import re
+00000730: 6c61 7469 6f6e 0a66 726f 6d20 7371 6c61  lation.from sqla
+00000740: 6c63 6865 6d79 2e6f 726d 2069 6d70 6f72  lchemy.orm impor
+00000750: 7420 5365 7373 696f 6e0a 6672 6f6d 2073  t Session.from s
+00000760: 716c 616c 6368 656d 792e 7479 7065 7320  qlalchemy.types 
+00000770: 696d 706f 7274 2049 6e74 6567 6572 0a66  import Integer.f
+00000780: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
+00000790: 7970 6573 2069 6d70 6f72 7420 4e75 6d65  ypes import Nume
+000007a0: 7269 630a 6672 6f6d 2073 716c 616c 6368  ric.from sqlalch
+000007b0: 656d 792e 7479 7065 7320 696d 706f 7274  emy.types import
+000007c0: 2054 6578 740a 6672 6f6d 2073 716c 616c   Text.from sqlal
+000007d0: 6368 656d 792e 7465 7374 696e 6720 696d  chemy.testing im
+000007e0: 706f 7274 2072 6571 7569 7265 730a 6672  port requires.fr
+000007f0: 6f6d 2073 716c 616c 6368 656d 792e 7465  om sqlalchemy.te
+00000800: 7374 696e 6720 696d 706f 7274 2069 735f  sting import is_
+00000810: 7472 7565 0a66 726f 6d20 7371 6c61 6c63  true.from sqlalc
+00000820: 6865 6d79 2e74 6573 7469 6e67 2e66 6978  hemy.testing.fix
+00000830: 7475 7265 7320 696d 706f 7274 2028 0a20  tures import (. 
+00000840: 2020 2043 6f6d 7075 7465 6452 6566 6c65     ComputedRefle
+00000850: 6374 696f 6e46 6978 7475 7265 5465 7374  ctionFixtureTest
+00000860: 2061 7320 5f43 6f6d 7075 7465 6452 6566   as _ComputedRef
+00000870: 6c65 6374 696f 6e46 6978 7475 7265 5465  lectionFixtureTe
+00000880: 7374 2c0a 290a 0a66 726f 6d20 676f 6f67  st,.)..from goog
+00000890: 6c65 2e61 7069 5f63 6f72 652e 6461 7465  le.api_core.date
+000008a0: 7469 6d65 5f68 656c 7065 7273 2069 6d70  time_helpers imp
+000008b0: 6f72 7420 4461 7465 7469 6d65 5769 7468  ort DatetimeWith
+000008c0: 4e61 6e6f 7365 636f 6e64 730a 0a66 726f  Nanoseconds..fro
+000008d0: 6d20 676f 6f67 6c65 2e63 6c6f 7564 2069  m google.cloud i
+000008e0: 6d70 6f72 7420 7370 616e 6e65 725f 6462  mport spanner_db
+000008f0: 6170 690a 0a66 726f 6d20 7371 6c61 6c63  api..from sqlalc
+00000900: 6865 6d79 2e74 6573 7469 6e67 2e73 7569  hemy.testing.sui
+00000910: 7465 2e74 6573 745f 6374 6520 696d 706f  te.test_cte impo
+00000920: 7274 202a 2020 2320 6e6f 7161 3a20 4634  rt *  # noqa: F4
+00000930: 3031 2c20 4634 3033 0a66 726f 6d20 7371  01, F403.from sq
+00000940: 6c61 6c63 6865 6d79 2e74 6573 7469 6e67  lalchemy.testing
+00000950: 2e73 7569 7465 2e74 6573 745f 6464 6c20  .suite.test_ddl 
+00000960: 696d 706f 7274 202a 2020 2320 6e6f 7161  import *  # noqa
+00000970: 3a20 4634 3031 2c20 4634 3033 0a66 726f  : F401, F403.fro
+00000980: 6d20 7371 6c61 6c63 6865 6d79 2e74 6573  m sqlalchemy.tes
+00000990: 7469 6e67 2e73 7569 7465 2e74 6573 745f  ting.suite.test_
+000009a0: 6469 616c 6563 7420 696d 706f 7274 202a  dialect import *
+000009b0: 2020 2320 6e6f 7161 3a20 4634 3031 2c20    # noqa: F401, 
+000009c0: 4634 3033 0a66 726f 6d20 7371 6c61 6c63  F403.from sqlalc
+000009d0: 6865 6d79 2e74 6573 7469 6e67 2e73 7569  hemy.testing.sui
+000009e0: 7465 2e74 6573 745f 696e 7365 7274 2069  te.test_insert i
+000009f0: 6d70 6f72 7420 2a20 2023 206e 6f71 613a  mport *  # noqa:
+00000a00: 2046 3430 312c 2046 3430 330a 6672 6f6d   F401, F403.from
+00000a10: 2073 716c 616c 6368 656d 792e 7465 7374   sqlalchemy.test
+00000a20: 696e 672e 7375 6974 652e 7465 7374 5f72  ing.suite.test_r
+00000a30: 6566 6c65 6374 696f 6e20 696d 706f 7274  eflection import
+00000a40: 202a 2020 2320 6e6f 7161 3a20 4634 3031   *  # noqa: F401
+00000a50: 2c20 4634 3033 0a66 726f 6d20 7371 6c61  , F403.from sqla
+00000a60: 6c63 6865 6d79 2e74 6573 7469 6e67 2e73  lchemy.testing.s
+00000a70: 7569 7465 2e74 6573 745f 7265 7375 6c74  uite.test_result
+00000a80: 7320 696d 706f 7274 202a 2020 2320 6e6f  s import *  # no
+00000a90: 7161 3a20 4634 3031 2c20 4634 3033 0a66  qa: F401, F403.f
+00000aa0: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
+00000ab0: 6573 7469 6e67 2e73 7569 7465 2e74 6573  esting.suite.tes
+00000ac0: 745f 7365 6c65 6374 2069 6d70 6f72 7420  t_select import 
+00000ad0: 2a20 2023 206e 6f71 613a 2046 3430 312c  *  # noqa: F401,
+00000ae0: 2046 3430 330a 6672 6f6d 2073 716c 616c   F403.from sqlal
+00000af0: 6368 656d 792e 7465 7374 696e 672e 7375  chemy.testing.su
+00000b00: 6974 652e 7465 7374 5f73 6571 7565 6e63  ite.test_sequenc
+00000b10: 6520 696d 706f 7274 202a 2020 2320 6e6f  e import *  # no
+00000b20: 7161 3a20 4634 3031 2c20 4634 3033 0a66  qa: F401, F403.f
+00000b30: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
+00000b40: 6573 7469 6e67 2e73 7569 7465 2e74 6573  esting.suite.tes
+00000b50: 745f 7570 6461 7465 5f64 656c 6574 6520  t_update_delete 
+00000b60: 696d 706f 7274 202a 2020 2320 6e6f 7161  import *  # noqa
+00000b70: 3a20 4634 3031 2c20 4634 3033 0a66 726f  : F401, F403.fro
+00000b80: 6d20 7371 6c61 6c63 6865 6d79 2e74 6573  m sqlalchemy.tes
+00000b90: 7469 6e67 2e73 7569 7465 2e74 6573 745f  ting.suite.test_
+00000ba0: 6374 6520 696d 706f 7274 2043 5445 5465  cte import CTETe
+00000bb0: 7374 2061 7320 5f43 5445 5465 7374 0a66  st as _CTETest.f
+00000bc0: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
+00000bd0: 6573 7469 6e67 2e73 7569 7465 2e74 6573  esting.suite.tes
+00000be0: 745f 6464 6c20 696d 706f 7274 2054 6162  t_ddl import Tab
+00000bf0: 6c65 4444 4c54 6573 7420 6173 205f 5461  leDDLTest as _Ta
+00000c00: 626c 6544 444c 5465 7374 0a66 726f 6d20  bleDDLTest.from 
+00000c10: 7371 6c61 6c63 6865 6d79 2e74 6573 7469  sqlalchemy.testi
+00000c20: 6e67 2e73 7569 7465 2e74 6573 745f 6464  ng.suite.test_dd
+00000c30: 6c20 696d 706f 7274 2028 0a20 2020 2046  l import (.    F
+00000c40: 7574 7572 6554 6162 6c65 4444 4c54 6573  utureTableDDLTes
+00000c50: 7420 6173 205f 4675 7475 7265 5461 626c  t as _FutureTabl
+00000c60: 6544 444c 5465 7374 2c0a 2020 2020 4c6f  eDDLTest,.    Lo
+00000c70: 6e67 4e61 6d65 426c 6f77 6f75 7454 6573  ngNameBlowoutTes
+00000c80: 7420 6173 205f 4c6f 6e67 4e61 6d65 426c  t as _LongNameBl
+00000c90: 6f77 6f75 7454 6573 742c 0a29 0a66 726f  owoutTest,.).fro
+00000ca0: 6d20 7371 6c61 6c63 6865 6d79 2e74 6573  m sqlalchemy.tes
+00000cb0: 7469 6e67 2e73 7569 7465 2e74 6573 745f  ting.suite.test_
+00000cc0: 7570 6461 7465 5f64 656c 6574 6520 696d  update_delete im
+00000cd0: 706f 7274 2028 0a20 2020 2053 696d 706c  port (.    Simpl
+00000ce0: 6555 7064 6174 6544 656c 6574 6554 6573  eUpdateDeleteTes
+00000cf0: 7420 6173 205f 5369 6d70 6c65 5570 6461  t as _SimpleUpda
+00000d00: 7465 4465 6c65 7465 5465 7374 2c0a 290a  teDeleteTest,.).
+00000d10: 6672 6f6d 2073 716c 616c 6368 656d 792e  from sqlalchemy.
+00000d20: 7465 7374 696e 672e 7375 6974 652e 7465  testing.suite.te
+00000d30: 7374 5f64 6961 6c65 6374 2069 6d70 6f72  st_dialect impor
+00000d40: 7420 280a 2020 2020 4469 6666 6963 756c  t (.    Difficul
+00000d50: 7450 6172 616d 6574 6572 7354 6573 7420  tParametersTest 
+00000d60: 6173 205f 4469 6666 6963 756c 7450 6172  as _DifficultPar
+00000d70: 616d 6574 6572 7354 6573 742c 0a20 2020  ametersTest,.   
+00000d80: 2045 7363 6170 696e 6754 6573 7420 6173   EscapingTest as
+00000d90: 205f 4573 6361 7069 6e67 5465 7374 2c0a   _EscapingTest,.
+00000da0: 290a 6672 6f6d 2073 716c 616c 6368 656d  ).from sqlalchem
+00000db0: 792e 7465 7374 696e 672e 7375 6974 652e  y.testing.suite.
+00000dc0: 7465 7374 5f69 6e73 6572 7420 696d 706f  test_insert impo
+00000dd0: 7274 2028 0a20 2020 2049 6e73 6572 7442  rt (.    InsertB
+00000de0: 6568 6176 696f 7254 6573 7420 6173 205f  ehaviorTest as _
+00000df0: 496e 7365 7274 4265 6861 7669 6f72 5465  InsertBehaviorTe
+00000e00: 7374 2c0a 290a 6672 6f6d 2073 716c 616c  st,.).from sqlal
+00000e10: 6368 656d 792e 7465 7374 696e 672e 7375  chemy.testing.su
+00000e20: 6974 652e 7465 7374 5f73 656c 6563 7420  ite.test_select 
+00000e30: 696d 706f 7274 2028 2020 2320 6e6f 7161  import (  # noqa
+00000e40: 3a20 4634 3031 2c20 4634 3033 0a20 2020  : F401, F403.   
+00000e50: 2043 6f6d 706f 756e 6453 656c 6563 7454   CompoundSelectT
+00000e60: 6573 7420 6173 205f 436f 6d70 6f75 6e64  est as _Compound
+00000e70: 5365 6c65 6374 5465 7374 2c0a 2020 2020  SelectTest,.    
+00000e80: 4578 6973 7473 5465 7374 2061 7320 5f45  ExistsTest as _E
+00000e90: 7869 7374 7354 6573 742c 0a20 2020 2046  xistsTest,.    F
+00000ea0: 6574 6368 4c69 6d69 744f 6666 7365 7454  etchLimitOffsetT
+00000eb0: 6573 7420 6173 205f 4665 7463 684c 696d  est as _FetchLim
+00000ec0: 6974 4f66 6673 6574 5465 7374 2c0a 2020  itOffsetTest,.  
+00000ed0: 2020 4964 656e 7469 7479 4175 746f 696e    IdentityAutoin
+00000ee0: 6372 656d 656e 7454 6573 7420 6173 205f  crementTest as _
+00000ef0: 4964 656e 7469 7479 4175 746f 696e 6372  IdentityAutoincr
+00000f00: 656d 656e 7454 6573 742c 0a20 2020 2049  ementTest,.    I
+00000f10: 734f 7249 734e 6f74 4469 7374 696e 6374  sOrIsNotDistinct
+00000f20: 4672 6f6d 5465 7374 2061 7320 5f49 734f  FromTest as _IsO
+00000f30: 7249 734e 6f74 4469 7374 696e 6374 4672  rIsNotDistinctFr
+00000f40: 6f6d 5465 7374 2c0a 2020 2020 4c69 6b65  omTest,.    Like
+00000f50: 4675 6e63 7469 6f6e 7354 6573 7420 6173  FunctionsTest as
+00000f60: 205f 4c69 6b65 4675 6e63 7469 6f6e 7354   _LikeFunctionsT
+00000f70: 6573 742c 0a20 2020 204f 7264 6572 4279  est,.    OrderBy
+00000f80: 4c61 6265 6c54 6573 7420 6173 205f 4f72  LabelTest as _Or
+00000f90: 6465 7242 794c 6162 656c 5465 7374 2c0a  derByLabelTest,.
+00000fa0: 2020 2020 506f 7374 436f 6d70 696c 6550      PostCompileP
+00000fb0: 6172 616d 7354 6573 7420 6173 205f 506f  aramsTest as _Po
+00000fc0: 7374 436f 6d70 696c 6550 6172 616d 7354  stCompileParamsT
+00000fd0: 6573 742c 0a29 0a66 726f 6d20 7371 6c61  est,.).from sqla
+00000fe0: 6c63 6865 6d79 2e74 6573 7469 6e67 2e73  lchemy.testing.s
+00000ff0: 7569 7465 2e74 6573 745f 7265 666c 6563  uite.test_reflec
+00001000: 7469 6f6e 2069 6d70 6f72 7420 280a 2020  tion import (.  
+00001010: 2020 436f 6d70 6f6e 656e 7452 6566 6c65    ComponentRefle
+00001020: 6374 696f 6e54 6573 7445 7874 7261 2061  ctionTestExtra a
+00001030: 7320 5f43 6f6d 706f 6e65 6e74 5265 666c  s _ComponentRefl
+00001040: 6563 7469 6f6e 5465 7374 4578 7472 612c  ectionTestExtra,
+00001050: 0a20 2020 2051 756f 7465 644e 616d 6541  .    QuotedNameA
+00001060: 7267 756d 656e 7454 6573 7420 6173 205f  rgumentTest as _
+00001070: 5175 6f74 6564 4e61 6d65 4172 6775 6d65  QuotedNameArgume
+00001080: 6e74 5465 7374 2c0a 2020 2020 436f 6d70  ntTest,.    Comp
+00001090: 6f6e 656e 7452 6566 6c65 6374 696f 6e54  onentReflectionT
+000010a0: 6573 7420 6173 205f 436f 6d70 6f6e 656e  est as _Componen
+000010b0: 7452 6566 6c65 6374 696f 6e54 6573 742c  tReflectionTest,
+000010c0: 0a20 2020 2043 6f6d 706f 7369 7465 4b65  .    CompositeKe
+000010d0: 7952 6566 6c65 6374 696f 6e54 6573 7420  yReflectionTest 
+000010e0: 6173 205f 436f 6d70 6f73 6974 654b 6579  as _CompositeKey
+000010f0: 5265 666c 6563 7469 6f6e 5465 7374 2c0a  ReflectionTest,.
+00001100: 2020 2020 436f 6d70 7574 6564 5265 666c      ComputedRefl
+00001110: 6563 7469 6f6e 5465 7374 2061 7320 5f43  ectionTest as _C
+00001120: 6f6d 7075 7465 6452 6566 6c65 6374 696f  omputedReflectio
+00001130: 6e54 6573 742c 0a20 2020 2048 6173 496e  nTest,.    HasIn
+00001140: 6465 7854 6573 7420 6173 205f 4861 7349  dexTest as _HasI
+00001150: 6e64 6578 5465 7374 2c0a 2020 2020 4861  ndexTest,.    Ha
+00001160: 7354 6162 6c65 5465 7374 2061 7320 5f48  sTableTest as _H
+00001170: 6173 5461 626c 6554 6573 742c 0a29 0a66  asTableTest,.).f
+00001180: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
+00001190: 6573 7469 6e67 2e73 7569 7465 2e74 6573  esting.suite.tes
+000011a0: 745f 7265 7375 6c74 7320 696d 706f 7274  t_results import
+000011b0: 2052 6f77 4665 7463 6854 6573 7420 6173   RowFetchTest as
+000011c0: 205f 526f 7746 6574 6368 5465 7374 0a66   _RowFetchTest.f
+000011d0: 726f 6d20 7371 6c61 6c63 6865 6d79 2e74  rom sqlalchemy.t
+000011e0: 6573 7469 6e67 2e73 7569 7465 2e74 6573  esting.suite.tes
+000011f0: 745f 7479 7065 7320 696d 706f 7274 2028  t_types import (
+00001200: 2020 2320 6e6f 7161 3a20 4634 3031 2c20    # noqa: F401, 
+00001210: 4634 3033 0a20 2020 2042 6f6f 6c65 616e  F403.    Boolean
+00001220: 5465 7374 2061 7320 5f42 6f6f 6c65 616e  Test as _Boolean
+00001230: 5465 7374 2c0a 2020 2020 4461 7465 5465  Test,.    DateTe
+00001240: 7374 2061 7320 5f44 6174 6554 6573 742c  st as _DateTest,
+00001250: 0a20 2020 205f 4461 7465 4669 7874 7572  .    _DateFixtur
+00001260: 6520 6173 205f 5f44 6174 6546 6978 7475  e as __DateFixtu
+00001270: 7265 2c0a 2020 2020 4461 7465 5469 6d65  re,.    DateTime
+00001280: 4869 7374 6f72 6963 5465 7374 2c0a 2020  HistoricTest,.  
+00001290: 2020 4461 7465 5469 6d65 436f 6572 6365    DateTimeCoerce
+000012a0: 6454 6f44 6174 6554 696d 6554 6573 7420  dToDateTimeTest 
+000012b0: 6173 205f 4461 7465 5469 6d65 436f 6572  as _DateTimeCoer
+000012c0: 6365 6454 6f44 6174 6554 696d 6554 6573  cedToDateTimeTes
+000012d0: 742c 0a20 2020 2044 6174 6554 696d 654d  t,.    DateTimeM
+000012e0: 6963 726f 7365 636f 6e64 7354 6573 7420  icrosecondsTest 
+000012f0: 6173 205f 4461 7465 5469 6d65 4d69 6372  as _DateTimeMicr
+00001300: 6f73 6563 6f6e 6473 5465 7374 2c0a 2020  osecondsTest,.  
+00001310: 2020 4461 7465 5469 6d65 5465 7374 2061    DateTimeTest a
+00001320: 7320 5f44 6174 6554 696d 6554 6573 742c  s _DateTimeTest,
+00001330: 0a20 2020 2049 6e74 6567 6572 5465 7374  .    IntegerTest
+00001340: 2061 7320 5f49 6e74 6567 6572 5465 7374   as _IntegerTest
+00001350: 2c0a 2020 2020 4a53 4f4e 5465 7374 2061  ,.    JSONTest a
+00001360: 7320 5f4a 534f 4e54 6573 742c 0a20 2020  s _JSONTest,.   
+00001370: 205f 4c69 7465 7261 6c52 6f75 6e64 5472   _LiteralRoundTr
+00001380: 6970 4669 7874 7572 652c 0a20 2020 204e  ipFixture,.    N
+00001390: 756d 6572 6963 5465 7374 2061 7320 5f4e  umericTest as _N
+000013a0: 756d 6572 6963 5465 7374 2c0a 2020 2020  umericTest,.    
+000013b0: 5374 7269 6e67 5465 7374 2061 7320 5f53  StringTest as _S
+000013c0: 7472 696e 6754 6573 742c 0a20 2020 2054  tringTest,.    T
+000013d0: 6578 7454 6573 7420 6173 205f 5465 7874  extTest as _Text
+000013e0: 5465 7374 2c0a 2020 2020 5469 6d65 5465  Test,.    TimeTe
+000013f0: 7374 2061 7320 5f54 696d 6554 6573 742c  st as _TimeTest,
+00001400: 0a20 2020 2054 696d 654d 6963 726f 7365  .    TimeMicrose
+00001410: 636f 6e64 7354 6573 7420 6173 205f 5469  condsTest as _Ti
+00001420: 6d65 4d69 6372 6f73 6563 6f6e 6473 5465  meMicrosecondsTe
+00001430: 7374 2c0a 2020 2020 5469 6d65 7374 616d  st,.    Timestam
+00001440: 704d 6963 726f 7365 636f 6e64 7354 6573  pMicrosecondsTes
+00001450: 742c 0a20 2020 2055 6e69 636f 6465 5661  t,.    UnicodeVa
+00001460: 7263 6861 7254 6573 7420 6173 205f 556e  rcharTest as _Un
+00001470: 6963 6f64 6556 6172 6368 6172 5465 7374  icodeVarcharTest
+00001480: 2c0a 2020 2020 556e 6963 6f64 6554 6578  ,.    UnicodeTex
+00001490: 7454 6573 7420 6173 205f 556e 6963 6f64  tTest as _Unicod
+000014a0: 6554 6578 7454 6573 742c 0a20 2020 205f  eTextTest,.    _
+000014b0: 556e 6963 6f64 6546 6978 7475 7265 2061  UnicodeFixture a
+000014c0: 7320 5f5f 556e 6963 6f64 6546 6978 7475  s __UnicodeFixtu
+000014d0: 7265 2c0a 290a 6672 6f6d 2074 6573 742e  re,.).from test.
+000014e0: 5f68 656c 7065 7273 2069 6d70 6f72 7420  _helpers import 
+000014f0: 6765 745f 6462 5f75 726c 2c20 6765 745f  get_db_url, get_
+00001500: 7072 6f6a 6563 740a 0a63 6f6e 6669 672e  project..config.
+00001510: 7465 7374 5f73 6368 656d 6120 3d20 2222  test_schema = ""
+00001520: 0a0a 0a63 6c61 7373 2042 6f6f 6c65 616e  ...class Boolean
+00001530: 5465 7374 285f 426f 6f6c 6561 6e54 6573  Test(_BooleanTes
+00001540: 7429 3a0a 2020 2020 4070 7974 6573 742e  t):.    @pytest.
+00001550: 6d61 726b 2e73 6b69 7028 0a20 2020 2020  mark.skip(.     
+00001560: 2020 2022 5468 6520 6f72 6967 696e 616c     "The original
+00001570: 2074 6573 7420 6361 7365 2077 6173 2073   test case was s
+00001580: 706c 6974 2069 6e74 6f20 3220 7061 7274  plit into 2 part
+00001590: 733a 2022 0a20 2020 2020 2020 2022 7465  s: ".        "te
+000015a0: 7374 5f72 656e 6465 725f 6c69 7465 7261  st_render_litera
+000015b0: 6c5f 626f 6f6c 5f74 7275 6520 616e 6420  l_bool_true and 
+000015c0: 7465 7374 5f72 656e 6465 725f 6c69 7465  test_render_lite
+000015d0: 7261 6c5f 626f 6f6c 5f66 616c 7365 220a  ral_bool_false".
+000015e0: 2020 2020 290a 2020 2020 6465 6620 7465      ).    def te
+000015f0: 7374 5f72 656e 6465 725f 6c69 7465 7261  st_render_litera
+00001600: 6c5f 626f 6f6c 2873 656c 6629 3a0a 2020  l_bool(self):.  
+00001610: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00001620: 6465 6620 7465 7374 5f72 656e 6465 725f  def test_render_
+00001630: 6c69 7465 7261 6c5f 626f 6f6c 5f74 7275  literal_bool_tru
+00001640: 6528 7365 6c66 2c20 6c69 7465 7261 6c5f  e(self, literal_
+00001650: 726f 756e 645f 7472 6970 293a 0a20 2020  round_trip):.   
+00001660: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00001670: 2053 5041 4e4e 4552 204f 5645 5252 4944   SPANNER OVERRID
+00001680: 453a 0a0a 2020 2020 2020 2020 436c 6f75  E:..        Clou
+00001690: 6420 5370 616e 6e65 7220 7375 7070 6f72  d Spanner suppor
+000016a0: 7473 2074 6162 6c65 7320 7769 7468 2061  ts tables with a
+000016b0: 6e20 656d 7074 7920 7072 696d 6172 7920  n empty primary 
+000016c0: 6b65 792c 2062 7574 0a20 2020 2020 2020  key, but.       
+000016d0: 206f 6e6c 7920 6120 7369 6e67 6c65 2072   only a single r
+000016e0: 6f77 2063 616e 2062 6520 696e 7365 7274  ow can be insert
+000016f0: 6564 2069 6e74 6f20 7375 6368 2061 2074  ed into such a t
+00001700: 6162 6c65 202d 0a20 2020 2020 2020 2066  able -.        f
+00001710: 6f6c 6c6f 7769 6e67 2069 6e73 6572 7469  ollowing inserti
+00001720: 6f6e 7320 7769 6c6c 2066 6169 6c20 7769  ons will fail wi
+00001730: 7468 2060 526f 7720 5b5d 2061 6c72 6561  th `Row [] alrea
+00001740: 6479 2065 7869 7374 7322 2e0a 2020 2020  dy exists"..    
+00001750: 2020 2020 4f76 6572 7269 6469 6e67 2074      Overriding t
+00001760: 6865 2074 6573 7420 746f 2061 766f 6964  he test to avoid
+00001770: 2074 6865 2073 616d 6520 6661 696c 7572   the same failur
+00001780: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
+00001790: 2020 2020 2020 206c 6974 6572 616c 5f72         literal_r
+000017a0: 6f75 6e64 5f74 7269 7028 426f 6f6c 6561  ound_trip(Boolea
+000017b0: 6e28 292c 205b 5472 7565 5d2c 205b 5472  n(), [True], [Tr
+000017c0: 7565 5d29 0a0a 2020 2020 6465 6620 7465  ue])..    def te
+000017d0: 7374 5f72 656e 6465 725f 6c69 7465 7261  st_render_litera
+000017e0: 6c5f 626f 6f6c 5f66 616c 7365 2873 656c  l_bool_false(sel
+000017f0: 662c 206c 6974 6572 616c 5f72 6f75 6e64  f, literal_round
+00001800: 5f74 7269 7029 3a0a 2020 2020 2020 2020  _trip):.        
+00001810: 2222 220a 2020 2020 2020 2020 5350 414e  """.        SPAN
+00001820: 4e45 5220 4f56 4552 5249 4445 3a0a 0a20  NER OVERRIDE:.. 
+00001830: 2020 2020 2020 2043 6c6f 7564 2053 7061         Cloud Spa
+00001840: 6e6e 6572 2073 7570 706f 7274 7320 7461  nner supports ta
+00001850: 626c 6573 2077 6974 6820 616e 2065 6d70  bles with an emp
+00001860: 7479 2070 7269 6d61 7279 206b 6579 2c20  ty primary key, 
+00001870: 6275 740a 2020 2020 2020 2020 6f6e 6c79  but.        only
+00001880: 2061 2073 696e 676c 6520 726f 7720 6361   a single row ca
+00001890: 6e20 6265 2069 6e73 6572 7465 6420 696e  n be inserted in
+000018a0: 746f 2073 7563 6820 6120 7461 626c 6520  to such a table 
+000018b0: 2d0a 2020 2020 2020 2020 666f 6c6c 6f77  -.        follow
+000018c0: 696e 6720 696e 7365 7274 696f 6e73 2077  ing insertions w
+000018d0: 696c 6c20 6661 696c 2077 6974 6820 6052  ill fail with `R
+000018e0: 6f77 205b 5d20 616c 7265 6164 7920 6578  ow [] already ex
+000018f0: 6973 7473 222e 0a20 2020 2020 2020 204f  ists"..        O
+00001900: 7665 7272 6964 696e 6720 7468 6520 7465  verriding the te
+00001910: 7374 2074 6f20 6176 6f69 6420 7468 6520  st to avoid the 
+00001920: 7361 6d65 2066 6169 6c75 7265 2e0a 2020  same failure..  
+00001930: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00001940: 2020 6c69 7465 7261 6c5f 726f 756e 645f    literal_round_
+00001950: 7472 6970 2842 6f6f 6c65 616e 2829 2c20  trip(Boolean(), 
+00001960: 5b46 616c 7365 5d2c 205b 4661 6c73 655d  [False], [False]
+00001970: 290a 0a20 2020 2040 7079 7465 7374 2e6d  )..    @pytest.m
+00001980: 6172 6b2e 736b 6970 2822 4e6f 7420 7375  ark.skip("Not su
+00001990: 7070 6f72 7465 6420 6279 2043 6c6f 7564  pported by Cloud
+000019a0: 2053 7061 6e6e 6572 2229 0a20 2020 2064   Spanner").    d
+000019b0: 6566 2074 6573 745f 7768 6572 6563 6c61  ef test_wherecla
+000019c0: 7573 6528 7365 6c66 293a 0a20 2020 2020  use(self):.     
+000019d0: 2020 2070 6173 730a 0a0a 636c 6173 7320     pass...class 
+000019e0: 436f 6d70 6f6e 656e 7452 6566 6c65 6374  ComponentReflect
+000019f0: 696f 6e54 6573 7445 7874 7261 285f 436f  ionTestExtra(_Co
+00001a00: 6d70 6f6e 656e 7452 6566 6c65 6374 696f  mponentReflectio
+00001a10: 6e54 6573 7445 7874 7261 293a 0a20 2020  nTestExtra):.   
+00001a20: 2040 7465 7374 696e 672e 7265 7175 6972   @testing.requir
+00001a30: 6573 2e74 6162 6c65 5f72 6566 6c65 6374  es.table_reflect
+00001a40: 696f 6e0a 2020 2020 6465 6620 7465 7374  ion.    def test
+00001a50: 5f6e 756c 6c61 626c 655f 7265 666c 6563  _nullable_reflec
+00001a60: 7469 6f6e 2873 656c 662c 2063 6f6e 6e65  tion(self, conne
+00001a70: 6374 696f 6e2c 206d 6574 6164 6174 6129  ction, metadata)
+00001a80: 3a0a 2020 2020 2020 2020 7420 3d20 5461  :.        t = Ta
+00001a90: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
+00001aa0: 2022 7422 2c0a 2020 2020 2020 2020 2020   "t",.          
+00001ab0: 2020 6d65 7461 6461 7461 2c0a 2020 2020    metadata,.    
+00001ac0: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
+00001ad0: 6122 2c20 496e 7465 6765 722c 206e 756c  a", Integer, nul
+00001ae0: 6c61 626c 653d 5472 7565 292c 0a20 2020  lable=True),.   
+00001af0: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
+00001b00: 2262 222c 2049 6e74 6567 6572 2c20 6e75  "b", Integer, nu
+00001b10: 6c6c 6162 6c65 3d46 616c 7365 292c 0a20  llable=False),. 
+00001b20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00001b30: 2074 2e63 7265 6174 6528 636f 6e6e 6563   t.create(connec
+00001b40: 7469 6f6e 290a 2020 2020 2020 2020 636f  tion).        co
+00001b50: 6e6e 6563 7469 6f6e 2e63 6f6e 6e65 6374  nnection.connect
+00001b60: 696f 6e2e 636f 6d6d 6974 2829 0a20 2020  ion.commit().   
+00001b70: 2020 2020 2065 715f 280a 2020 2020 2020       eq_(.      
+00001b80: 2020 2020 2020 6469 6374 280a 2020 2020        dict(.    
+00001b90: 2020 2020 2020 2020 2020 2020 2863 6f6c              (col
+00001ba0: 5b22 6e61 6d65 225d 2c20 636f 6c5b 226e  ["name"], col["n
+00001bb0: 756c 6c61 626c 6522 5d29 0a20 2020 2020  ullable"]).     
+00001bc0: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
+00001bd0: 6f6c 2069 6e20 696e 7370 6563 7428 636f  ol in inspect(co
+00001be0: 6e6e 6563 7469 6f6e 292e 6765 745f 636f  nnection).get_co
+00001bf0: 6c75 6d6e 7328 2274 2229 0a20 2020 2020  lumns("t").     
+00001c00: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+00001c10: 2020 2020 2020 7b22 6122 3a20 5472 7565        {"a": True
+00001c20: 2c20 2262 223a 2046 616c 7365 7d2c 0a20  , "b": False},. 
+00001c30: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+00001c40: 6620 5f74 7970 655f 726f 756e 645f 7472  f _type_round_tr
+00001c50: 6970 2873 656c 662c 2063 6f6e 6e65 6374  ip(self, connect
+00001c60: 696f 6e2c 206d 6574 6164 6174 612c 202a  ion, metadata, *
+00001c70: 7479 7065 7329 3a0a 2020 2020 2020 2020  types):.        
+00001c80: 7420 3d20 5461 626c 6528 0a20 2020 2020  t = Table(.     
+00001c90: 2020 2020 2020 2022 7422 2c20 6d65 7461         "t", meta
+00001ca0: 6461 7461 2c20 2a5b 436f 6c75 6d6e 2822  data, *[Column("
+00001cb0: 7425 6422 2025 2069 2c20 7479 7065 5f29  t%d" % i, type_)
+00001cc0: 2066 6f72 2069 2c20 7479 7065 5f20 696e   for i, type_ in
+00001cd0: 2065 6e75 6d65 7261 7465 2874 7970 6573   enumerate(types
+00001ce0: 295d 0a20 2020 2020 2020 2029 0a20 2020  )].        ).   
+00001cf0: 2020 2020 2074 2e63 7265 6174 6528 636f       t.create(co
+00001d00: 6e6e 6563 7469 6f6e 290a 2020 2020 2020  nnection).      
+00001d10: 2020 636f 6e6e 6563 7469 6f6e 2e63 6f6e    connection.con
+00001d20: 6e65 6374 696f 6e2e 636f 6d6d 6974 2829  nection.commit()
+00001d30: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00001d40: 205b 635b 2274 7970 6522 5d20 666f 7220   [c["type"] for 
+00001d50: 6320 696e 2069 6e73 7065 6374 2863 6f6e  c in inspect(con
+00001d60: 6e65 6374 696f 6e29 2e67 6574 5f63 6f6c  nection).get_col
+00001d70: 756d 6e73 2822 7422 295d 0a0a 2020 2020  umns("t")]..    
+00001d80: 4074 6573 7469 6e67 2e72 6571 7569 7265  @testing.require
+00001d90: 732e 7461 626c 655f 7265 666c 6563 7469  s.table_reflecti
+00001da0: 6f6e 0a20 2020 2064 6566 2074 6573 745f  on.    def test_
+00001db0: 6e75 6d65 7269 635f 7265 666c 6563 7469  numeric_reflecti
+00001dc0: 6f6e 2873 656c 662c 2063 6f6e 6e65 6374  on(self, connect
+00001dd0: 696f 6e2c 206d 6574 6164 6174 6129 3a0a  ion, metadata):.
+00001de0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00001df0: 2020 2020 5350 414e 4e45 5220 4f56 4552      SPANNER OVER
+00001e00: 5249 4445 3a0a 0a20 2020 2020 2020 2053  RIDE:..        S
+00001e10: 7061 6e6e 6572 2064 6566 696e 6573 204e  panner defines N
+00001e20: 554d 4552 4943 2074 7970 6520 7769 7468  UMERIC type with
+00001e30: 2074 6865 2063 6f6e 7374 616e 7420 7072   the constant pr
+00001e40: 6563 6973 696f 6e3d 3338 0a20 2020 2020  ecision=38.     
+00001e50: 2020 2061 6e64 2073 6361 6c65 3d39 2e20     and scale=9. 
+00001e60: 4f76 6572 7269 6469 6e67 2074 6865 2074  Overriding the t
+00001e70: 6573 7420 746f 2063 6865 636b 2069 6620  est to check if 
+00001e80: 7468 6520 4e55 4d45 5249 430a 2020 2020  the NUMERIC.    
+00001e90: 2020 2020 636f 6c75 6d6e 2069 7320 7375      column is su
+00001ea0: 6363 6573 7366 756c 6c79 2063 7265 6174  ccessfully creat
+00001eb0: 6564 2061 6e64 2068 6173 2064 696d 656e  ed and has dimen
+00001ec0: 7369 6f6e 730a 2020 2020 2020 2020 636f  sions.        co
+00001ed0: 7272 6563 7420 666f 7220 436c 6f75 6420  rrect for Cloud 
+00001ee0: 5370 616e 6e65 722e 0a20 2020 2020 2020  Spanner..       
+00001ef0: 2022 2222 0a20 2020 2020 2020 2066 6f72   """.        for
+00001f00: 2074 7970 2069 6e20 7365 6c66 2e5f 7479   typ in self._ty
+00001f10: 7065 5f72 6f75 6e64 5f74 7269 7028 636f  pe_round_trip(co
+00001f20: 6e6e 6563 7469 6f6e 2c20 6d65 7461 6461  nnection, metada
+00001f30: 7461 2c20 4e75 6d65 7269 6328 3138 2c20  ta, Numeric(18, 
+00001f40: 3529 293a 0a20 2020 2020 2020 2020 2020  5)):.           
+00001f50: 2061 7373 6572 7420 6973 696e 7374 616e   assert isinstan
+00001f60: 6365 2874 7970 2c20 4e75 6d65 7269 6329  ce(typ, Numeric)
+00001f70: 0a20 2020 2020 2020 2020 2020 2065 715f  .            eq_
+00001f80: 2874 7970 2e70 7265 6369 7369 6f6e 2c20  (typ.precision, 
+00001f90: 3338 290a 2020 2020 2020 2020 2020 2020  38).            
+00001fa0: 6571 5f28 7479 702e 7363 616c 652c 2039  eq_(typ.scale, 9
+00001fb0: 290a 0a20 2020 2040 7465 7374 696e 672e  )..    @testing.
+00001fc0: 7265 7175 6972 6573 2e74 6162 6c65 5f72  requires.table_r
+00001fd0: 6566 6c65 6374 696f 6e0a 2020 2020 6465  eflection.    de
+00001fe0: 6620 7465 7374 5f62 696e 6172 795f 7265  f test_binary_re
+00001ff0: 666c 6563 7469 6f6e 2873 656c 662c 2063  flection(self, c
+00002000: 6f6e 6e65 6374 696f 6e2c 206d 6574 6164  onnection, metad
+00002010: 6174 6129 3a0a 2020 2020 2020 2020 2222  ata):.        ""
+00002020: 220a 2020 2020 2020 2020 4368 6563 6b20  ".        Check 
+00002030: 7468 6174 2061 2042 5954 4553 2063 6f6c  that a BYTES col
+00002040: 756d 6e20 7769 7468 2061 6e20 6578 706c  umn with an expl
+00002050: 6963 6974 6c79 0a20 2020 2020 2020 2073  icitly.        s
+00002060: 6574 2073 697a 6520 6973 2063 6f72 7265  et size is corre
+00002070: 6374 6c79 2072 6566 6c65 6374 6564 2e0a  ctly reflected..
+00002080: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00002090: 2020 2020 666f 7220 7479 7020 696e 2073      for typ in s
+000020a0: 656c 662e 5f74 7970 655f 726f 756e 645f  elf._type_round_
+000020b0: 7472 6970 2863 6f6e 6e65 6374 696f 6e2c  trip(connection,
+000020c0: 206d 6574 6164 6174 612c 204c 6172 6765   metadata, Large
+000020d0: 4269 6e61 7279 2832 3029 293a 0a20 2020  Binary(20)):.   
+000020e0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+000020f0: 6973 696e 7374 616e 6365 2874 7970 2c20  isinstance(typ, 
+00002100: 4c61 7267 6542 696e 6172 7929 0a20 2020  LargeBinary).   
+00002110: 2020 2020 2020 2020 2065 715f 2874 7970           eq_(typ
+00002120: 2e6c 656e 6774 682c 2032 3029 0a0a 0a63  .length, 20)...c
+00002130: 6c61 7373 2043 6f6d 706f 6e65 6e74 5265  lass ComponentRe
+00002140: 666c 6563 7469 6f6e 5465 7374 285f 436f  flectionTest(_Co
+00002150: 6d70 6f6e 656e 7452 6566 6c65 6374 696f  mponentReflectio
+00002160: 6e54 6573 7429 3a0a 2020 2020 4063 6c61  nTest):.    @cla
+00002170: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
+00002180: 2064 6566 696e 655f 7461 626c 6573 2863   define_tables(c
+00002190: 6c73 2c20 6d65 7461 6461 7461 293a 0a20  ls, metadata):. 
+000021a0: 2020 2020 2020 2063 6c73 2e64 6566 696e         cls.defin
+000021b0: 655f 7265 666c 6563 7465 645f 7461 626c  e_reflected_tabl
+000021c0: 6573 286d 6574 6164 6174 612c 204e 6f6e  es(metadata, Non
+000021d0: 6529 0a0a 2020 2020 4063 6c61 7373 6d65  e)..    @classme
+000021e0: 7468 6f64 0a20 2020 2064 6566 2064 6566  thod.    def def
+000021f0: 696e 655f 7265 666c 6563 7465 645f 7461  ine_reflected_ta
+00002200: 626c 6573 2863 6c73 2c20 6d65 7461 6461  bles(cls, metada
+00002210: 7461 2c20 7363 6865 6d61 293a 0a20 2020  ta, schema):.   
+00002220: 2020 2020 2069 6620 7363 6865 6d61 3a0a       if schema:.
+00002230: 2020 2020 2020 2020 2020 2020 7363 6865              sche
+00002240: 6d61 5f70 7265 6669 7820 3d20 7363 6865  ma_prefix = sche
+00002250: 6d61 202b 2022 2e22 0a20 2020 2020 2020  ma + ".".       
+00002260: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00002270: 2020 2073 6368 656d 615f 7072 6566 6978     schema_prefix
+00002280: 203d 2022 220a 0a20 2020 2020 2020 2069   = ""..        i
+00002290: 6620 7465 7374 696e 672e 7265 7175 6972  f testing.requir
+000022a0: 6573 2e73 656c 665f 7265 6665 7265 6e74  es.self_referent
+000022b0: 6961 6c5f 666f 7265 6967 6e5f 6b65 7973  ial_foreign_keys
+000022c0: 2e65 6e61 626c 6564 3a0a 2020 2020 2020  .enabled:.      
+000022d0: 2020 2020 2020 7573 6572 7320 3d20 5461        users = Ta
+000022e0: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
+000022f0: 2020 2020 2022 7573 6572 7322 2c0a 2020       "users",.  
+00002300: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00002310: 7461 6461 7461 2c0a 2020 2020 2020 2020  tadata,.        
+00002320: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
+00002330: 7573 6572 5f69 6422 2c20 7371 6c61 6c63  user_id", sqlalc
+00002340: 6865 6d79 2e49 4e54 2c20 7072 696d 6172  hemy.INT, primar
+00002350: 795f 6b65 793d 5472 7565 292c 0a20 2020  y_key=True),.   
+00002360: 2020 2020 2020 2020 2020 2020 2043 6f6c               Col
+00002370: 756d 6e28 2274 6573 7431 222c 2073 716c  umn("test1", sql
+00002380: 616c 6368 656d 792e 4348 4152 2835 292c  alchemy.CHAR(5),
+00002390: 206e 756c 6c61 626c 653d 4661 6c73 6529   nullable=False)
+000023a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000023b0: 2020 436f 6c75 6d6e 2822 7465 7374 3222    Column("test2"
+000023c0: 2c20 7371 6c61 6c63 6865 6d79 2e46 6c6f  , sqlalchemy.Flo
+000023d0: 6174 2835 292c 206e 756c 6c61 626c 653d  at(5), nullable=
+000023e0: 4661 6c73 6529 2c0a 2020 2020 2020 2020  False),.        
+000023f0: 2020 2020 2020 2020 436f 6c75 6d6e 280a          Column(.
+00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002410: 2020 2020 2270 6172 656e 745f 7573 6572      "parent_user
+00002420: 5f69 6422 2c0a 2020 2020 2020 2020 2020  _id",.          
+00002430: 2020 2020 2020 2020 2020 7371 6c61 6c63            sqlalc
+00002440: 6865 6d79 2e49 6e74 6567 6572 2c0a 2020  hemy.Integer,.  
+00002450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002460: 2020 7371 6c61 6c63 6865 6d79 2e46 6f72    sqlalchemy.For
+00002470: 6569 676e 4b65 7928 0a20 2020 2020 2020  eignKey(.       
+00002480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002490: 2022 2573 7573 6572 732e 7573 6572 5f69   "%susers.user_i
+000024a0: 6422 2025 2073 6368 656d 615f 7072 6566  d" % schema_pref
+000024b0: 6978 2c20 6e61 6d65 3d22 7573 6572 5f69  ix, name="user_i
+000024c0: 645f 666b 220a 2020 2020 2020 2020 2020  d_fk".          
+000024d0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+000024e0: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
+000024f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002500: 7363 6865 6d61 3d73 6368 656d 612c 0a20  schema=schema,. 
+00002510: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00002520: 6573 745f 6e65 6564 735f 666b 3d54 7275  est_needs_fk=Tru
+00002530: 652c 0a20 2020 2020 2020 2020 2020 2029  e,.            )
+00002540: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00002550: 2020 2020 2020 2020 2020 2075 7365 7273             users
+00002560: 203d 2054 6162 6c65 280a 2020 2020 2020   = Table(.      
+00002570: 2020 2020 2020 2020 2020 2275 7365 7273            "users
+00002580: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002590: 2020 206d 6574 6164 6174 612c 0a20 2020     metadata,.   
+000025a0: 2020 2020 2020 2020 2020 2020 2043 6f6c               Col
+000025b0: 756d 6e28 2275 7365 725f 6964 222c 2073  umn("user_id", s
+000025c0: 716c 616c 6368 656d 792e 494e 542c 2070  qlalchemy.INT, p
+000025d0: 7269 6d61 7279 5f6b 6579 3d54 7275 6529  rimary_key=True)
+000025e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000025f0: 2020 436f 6c75 6d6e 2822 7465 7374 3122    Column("test1"
+00002600: 2c20 7371 6c61 6c63 6865 6d79 2e43 4841  , sqlalchemy.CHA
+00002610: 5228 3529 2c20 6e75 6c6c 6162 6c65 3d46  R(5), nullable=F
+00002620: 616c 7365 292c 0a20 2020 2020 2020 2020  alse),.         
+00002630: 2020 2020 2020 2043 6f6c 756d 6e28 2274         Column("t
+00002640: 6573 7432 222c 2073 716c 616c 6368 656d  est2", sqlalchem
+00002650: 792e 466c 6f61 7428 3529 2c20 6e75 6c6c  y.Float(5), null
+00002660: 6162 6c65 3d46 616c 7365 292c 0a20 2020  able=False),.   
+00002670: 2020 2020 2020 2020 2020 2020 2073 6368               sch
+00002680: 656d 613d 7363 6865 6d61 2c0a 2020 2020  ema=schema,.    
+00002690: 2020 2020 2020 2020 2020 2020 7465 7374              test
+000026a0: 5f6e 6565 6473 5f66 6b3d 5472 7565 2c0a  _needs_fk=True,.
+000026b0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+000026c0: 2020 2020 2020 2054 6162 6c65 280a 2020         Table(.  
+000026d0: 2020 2020 2020 2020 2020 2264 696e 6761            "dinga
+000026e0: 6c69 6e67 7322 2c0a 2020 2020 2020 2020  lings",.        
+000026f0: 2020 2020 6d65 7461 6461 7461 2c0a 2020      metadata,.  
+00002700: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
+00002710: 2822 6469 6e67 616c 696e 675f 6964 222c  ("dingaling_id",
+00002720: 2073 716c 616c 6368 656d 792e 496e 7465   sqlalchemy.Inte
+00002730: 6765 722c 2070 7269 6d61 7279 5f6b 6579  ger, primary_key
+00002740: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
+00002750: 2020 2020 436f 6c75 6d6e 280a 2020 2020      Column(.    
+00002760: 2020 2020 2020 2020 2020 2020 2261 6464              "add
+00002770: 7265 7373 5f69 6422 2c0a 2020 2020 2020  ress_id",.      
+00002780: 2020 2020 2020 2020 2020 7371 6c61 6c63            sqlalc
+00002790: 6865 6d79 2e49 6e74 6567 6572 2c0a 2020  hemy.Integer,.  
+000027a0: 2020 2020 2020 2020 2020 2020 2020 7371                sq
+000027b0: 6c61 6c63 6865 6d79 2e46 6f72 6569 676e  lalchemy.Foreign
+000027c0: 4b65 7928 2225 7365 6d61 696c 5f61 6464  Key("%semail_add
+000027d0: 7265 7373 6573 2e61 6464 7265 7373 5f69  resses.address_i
+000027e0: 6422 2025 2073 6368 656d 615f 7072 6566  d" % schema_pref
+000027f0: 6978 292c 0a20 2020 2020 2020 2020 2020  ix),.           
+00002800: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00002810: 436f 6c75 6d6e 2822 6461 7461 222c 2073  Column("data", s
+00002820: 716c 616c 6368 656d 792e 5374 7269 6e67  qlalchemy.String
+00002830: 2833 3029 292c 0a20 2020 2020 2020 2020  (30)),.         
+00002840: 2020 2073 6368 656d 613d 7363 6865 6d61     schema=schema
+00002850: 2c0a 2020 2020 2020 2020 2020 2020 7465  ,.            te
+00002860: 7374 5f6e 6565 6473 5f66 6b3d 5472 7565  st_needs_fk=True
+00002870: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00002880: 2020 2020 5461 626c 6528 0a20 2020 2020      Table(.     
+00002890: 2020 2020 2020 2022 656d 6169 6c5f 6164         "email_ad
+000028a0: 6472 6573 7365 7322 2c0a 2020 2020 2020  dresses",.      
+000028b0: 2020 2020 2020 6d65 7461 6461 7461 2c0a        metadata,.
+000028c0: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
+000028d0: 6d6e 2822 6164 6472 6573 735f 6964 222c  mn("address_id",
+000028e0: 2073 716c 616c 6368 656d 792e 496e 7465   sqlalchemy.Inte
+000028f0: 6765 722c 2070 7269 6d61 7279 5f6b 6579  ger, primary_key
+00002900: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
+00002910: 2020 2020 436f 6c75 6d6e 280a 2020 2020      Column(.    
+00002920: 2020 2020 2020 2020 2020 2020 2272 656d              "rem
+00002930: 6f74 655f 7573 6572 5f69 6422 2c0a 2020  ote_user_id",.  
+00002940: 2020 2020 2020 2020 2020 2020 2020 7371                sq
+00002950: 6c61 6c63 6865 6d79 2e49 6e74 6567 6572  lalchemy.Integer
+00002960: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002970: 2020 7371 6c61 6c63 6865 6d79 2e46 6f72    sqlalchemy.For
+00002980: 6569 676e 4b65 7928 7573 6572 732e 632e  eignKey(users.c.
+00002990: 7573 6572 5f69 6429 2c0a 2020 2020 2020  user_id),.      
+000029a0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+000029b0: 2020 2020 2043 6f6c 756d 6e28 2265 6d61       Column("ema
+000029c0: 696c 5f61 6464 7265 7373 222c 2073 716c  il_address", sql
+000029d0: 616c 6368 656d 792e 5374 7269 6e67 2832  alchemy.String(2
+000029e0: 3029 292c 0a20 2020 2020 2020 2020 2020  0)),.           
+000029f0: 2073 716c 616c 6368 656d 792e 5072 696d   sqlalchemy.Prim
+00002a00: 6172 794b 6579 436f 6e73 7472 6169 6e74  aryKeyConstraint
+00002a10: 2822 6164 6472 6573 735f 6964 222c 206e  ("address_id", n
+00002a20: 616d 653d 2265 6d61 696c 5f61 645f 706b  ame="email_ad_pk
+00002a30: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+00002a40: 7363 6865 6d61 3d73 6368 656d 612c 0a20  schema=schema,. 
+00002a50: 2020 2020 2020 2020 2020 2074 6573 745f             test_
+00002a60: 6e65 6564 735f 666b 3d54 7275 652c 0a20  needs_fk=True,. 
+00002a70: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00002a80: 2054 6162 6c65 280a 2020 2020 2020 2020   Table(.        
+00002a90: 2020 2020 2263 6f6d 6d65 6e74 5f74 6573      "comment_tes
+00002aa0: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+00002ab0: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
+00002ac0: 2020 2020 2020 436f 6c75 6d6e 2822 6964        Column("id
+00002ad0: 222c 2073 716c 616c 6368 656d 792e 496e  ", sqlalchemy.In
+00002ae0: 7465 6765 722c 2070 7269 6d61 7279 5f6b  teger, primary_k
+00002af0: 6579 3d54 7275 652c 2063 6f6d 6d65 6e74  ey=True, comment
+00002b00: 3d22 6964 2063 6f6d 6d65 6e74 2229 2c0a  ="id comment"),.
+00002b10: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
+00002b20: 6d6e 2822 6461 7461 222c 2073 716c 616c  mn("data", sqlal
+00002b30: 6368 656d 792e 5374 7269 6e67 2832 3029  chemy.String(20)
+00002b40: 2c20 636f 6d6d 656e 743d 2264 6174 6120  , comment="data 
+00002b50: 2520 636f 6d6d 656e 7422 292c 0a20 2020  % comment"),.   
+00002b60: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
+00002b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002b80: 2022 6432 222c 0a20 2020 2020 2020 2020   "d2",.         
+00002b90: 2020 2020 2020 2073 716c 616c 6368 656d         sqlalchem
+00002ba0: 792e 5374 7269 6e67 2832 3029 2c0a 2020  y.String(20),.  
+00002bb0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00002bc0: 6d6d 656e 743d 7222 2222 436f 6d6d 656e  mment=r"""Commen
+00002bd0: 7420 7479 7065 7320 7479 7065 2073 7065  t types type spe
+00002be0: 6564 696c 7920 2720 2220 5c20 2727 2046  edily ' " \ '' F
+00002bf0: 756e 2122 2222 2c0a 2020 2020 2020 2020  un!""",.        
+00002c00: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00002c10: 2020 2073 6368 656d 613d 7363 6865 6d61     schema=schema
+00002c20: 2c0a 2020 2020 2020 2020 2020 2020 636f  ,.            co
+00002c30: 6d6d 656e 743d 7222 2222 7468 6520 7465  mment=r"""the te
+00002c40: 7374 2025 2027 2022 205c 2074 6162 6c65  st % ' " \ table
+00002c50: 2063 6f6d 6d65 6e74 2222 222c 0a20 2020   comment""",.   
+00002c60: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00002c70: 6966 2074 6573 7469 6e67 2e72 6571 7569  if testing.requi
+00002c80: 7265 732e 6372 6f73 735f 7363 6865 6d61  res.cross_schema
+00002c90: 5f66 6b5f 7265 666c 6563 7469 6f6e 2e65  _fk_reflection.e
+00002ca0: 6e61 626c 6564 3a0a 2020 2020 2020 2020  nabled:.        
+00002cb0: 2020 2020 6966 2073 6368 656d 6120 6973      if schema is
+00002cc0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00002cd0: 2020 2020 2020 2054 6162 6c65 280a 2020         Table(.  
+00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cf0: 2020 226c 6f63 616c 5f74 6162 6c65 222c    "local_table",
+00002d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002d10: 2020 2020 206d 6574 6164 6174 612c 0a20       metadata,. 
+00002d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d30: 2020 2043 6f6c 756d 6e28 2269 6422 2c20     Column("id", 
+00002d40: 7371 6c61 6c63 6865 6d79 2e49 6e74 6567  sqlalchemy.Integ
+00002d50: 6572 2c20 7072 696d 6172 795f 6b65 793d  er, primary_key=
+00002d60: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
+00002d70: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
+00002d80: 6e28 2264 6174 6122 2c20 7371 6c61 6c63  n("data", sqlalc
+00002d90: 6865 6d79 2e53 7472 696e 6728 3230 2929  hemy.String(20))
+00002da0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002db0: 2020 2020 2020 436f 6c75 6d6e 280a 2020        Column(.  
+00002dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002dd0: 2020 2020 2020 2272 656d 6f74 655f 6964        "remote_id
+00002de0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002df0: 2020 2020 2020 2020 2020 2046 6f72 6569             Forei
+00002e00: 676e 4b65 7928 2225 732e 7265 6d6f 7465  gnKey("%s.remote
+00002e10: 5f74 6162 6c65 5f32 2e69 6422 2025 2074  _table_2.id" % t
+00002e20: 6573 7469 6e67 2e63 6f6e 6669 672e 7465  esting.config.te
+00002e30: 7374 5f73 6368 656d 6129 2c0a 2020 2020  st_schema),.    
 00002e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e50: 2020 7465 7374 5f6e 6565 6473 5f66 6b3d    test_needs_fk=
-00002e60: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-00002e70: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
-00002e80: 3d63 6f6e 6669 672e 6462 2e64 6961 6c65  =config.db.diale
-00002e90: 6374 2e64 6566 6175 6c74 5f73 6368 656d  ct.default_schem
-00002ea0: 615f 6e61 6d65 2c0a 2020 2020 2020 2020  a_name,.        
-00002eb0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00002ec0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00002ed0: 2020 2020 2020 2020 2020 2020 5461 626c              Tabl
-00002ee0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00002ef0: 2020 2020 2020 2022 7265 6d6f 7465 5f74         "remote_t
-00002f00: 6162 6c65 222c 0a20 2020 2020 2020 2020  able",.         
-00002f10: 2020 2020 2020 2020 2020 206d 6574 6164             metad
-00002f20: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-00002f30: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-00002f40: 2269 6422 2c20 7371 6c61 6c63 6865 6d79  "id", sqlalchemy
-00002f50: 2e49 6e74 6567 6572 2c20 7072 696d 6172  .Integer, primar
-00002f60: 795f 6b65 793d 5472 7565 292c 0a20 2020  y_key=True),.   
-00002f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f80: 2043 6f6c 756d 6e28 0a20 2020 2020 2020   Column(.       
-00002f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fa0: 2022 6c6f 6361 6c5f 6964 222c 0a20 2020   "local_id",.   
-00002fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fc0: 2020 2020 2046 6f72 6569 676e 4b65 7928       ForeignKey(
-00002fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002fe0: 2020 2020 2020 2020 2020 2020 2022 2573               "%s
-00002ff0: 2e6c 6f63 616c 5f74 6162 6c65 2e69 6422  .local_table.id"
-00003000: 2025 2063 6f6e 6669 672e 6462 2e64 6961   % config.db.dia
-00003010: 6c65 6374 2e64 6566 6175 6c74 5f73 6368  lect.default_sch
-00003020: 656d 615f 6e61 6d65 0a20 2020 2020 2020  ema_name.       
-00003030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003040: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-00003050: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-00003060: 2020 2020 2020 2020 2020 2020 2020 2043                 C
-00003070: 6f6c 756d 6e28 2264 6174 6122 2c20 7371  olumn("data", sq
-00003080: 6c61 6c63 6865 6d79 2e53 7472 696e 6728  lalchemy.String(
-00003090: 3230 2929 2c0a 2020 2020 2020 2020 2020  20)),.          
-000030a0: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
-000030b0: 3d73 6368 656d 612c 0a20 2020 2020 2020  =schema,.       
-000030c0: 2020 2020 2020 2020 2020 2020 2074 6573               tes
-000030d0: 745f 6e65 6564 735f 666b 3d54 7275 652c  t_needs_fk=True,
-000030e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000030f0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00003100: 2020 2054 6162 6c65 280a 2020 2020 2020     Table(.      
-00003110: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00003120: 656d 6f74 655f 7461 626c 655f 3222 2c0a  emote_table_2",.
-00003130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003140: 2020 2020 6d65 7461 6461 7461 2c0a 2020      metadata,.  
-00003150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003160: 2020 436f 6c75 6d6e 2822 6964 222c 2073    Column("id", s
-00003170: 716c 616c 6368 656d 792e 496e 7465 6765  qlalchemy.Intege
-00003180: 722c 2070 7269 6d61 7279 5f6b 6579 3d54  r, primary_key=T
-00003190: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
-000031a0: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
-000031b0: 2822 6461 7461 222c 2073 716c 616c 6368  ("data", sqlalch
-000031c0: 656d 792e 5374 7269 6e67 2832 3029 292c  emy.String(20)),
-000031d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000031e0: 2020 2020 2073 6368 656d 613d 7363 6865       schema=sche
-000031f0: 6d61 2c0a 2020 2020 2020 2020 2020 2020  ma,.            
-00003200: 2020 2020 2020 2020 7465 7374 5f6e 6565          test_nee
-00003210: 6473 5f66 6b3d 5472 7565 2c0a 2020 2020  ds_fk=True,.    
-00003220: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00003230: 2020 2020 2020 2069 6620 7465 7374 696e         if testin
-00003240: 672e 7265 7175 6972 6573 2e69 6e64 6578  g.requires.index
-00003250: 5f72 6566 6c65 6374 696f 6e2e 656e 6162  _reflection.enab
-00003260: 6c65 643a 0a20 2020 2020 2020 2020 2020  led:.           
-00003270: 2063 6c73 2e64 6566 696e 655f 696e 6465   cls.define_inde
-00003280: 7828 6d65 7461 6461 7461 2c20 7573 6572  x(metadata, user
-00003290: 7329 0a0a 2020 2020 2020 2020 2020 2020  s)..            
-000032a0: 6966 206e 6f74 2073 6368 656d 613a 0a20  if not schema:. 
-000032b0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000032c0: 2074 6573 745f 6e65 6564 735f 666b 2069   test_needs_fk i
-000032d0: 7320 6174 2074 6865 206d 6f6d 656e 7420  s at the moment 
-000032e0: 746f 2066 6f72 6365 204d 7953 514c 2049  to force MySQL I
-000032f0: 6e6e 6f44 420a 2020 2020 2020 2020 2020  nnoDB.          
-00003300: 2020 2020 2020 6e6f 6e63 6f6c 5f69 6478        noncol_idx
-00003310: 5f74 6573 745f 6e6f 706b 203d 2054 6162  _test_nopk = Tab
-00003320: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
-00003330: 2020 2020 2020 2020 226e 6f6e 636f 6c5f          "noncol_
-00003340: 6964 785f 7465 7374 5f6e 6f70 6b22 2c0a  idx_test_nopk",.
-00003350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003360: 2020 2020 6d65 7461 6461 7461 2c0a 2020      metadata,.  
-00003370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003380: 2020 436f 6c75 6d6e 2822 6964 222c 2073    Column("id", s
-00003390: 716c 616c 6368 656d 792e 496e 7465 6765  qlalchemy.Intege
-000033a0: 722c 2070 7269 6d61 7279 5f6b 6579 3d54  r, primary_key=T
-000033b0: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
-000033c0: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
-000033d0: 2822 7122 2c20 7371 6c61 6c63 6865 6d79  ("q", sqlalchemy
-000033e0: 2e53 7472 696e 6728 3529 292c 0a20 2020  .String(5)),.   
-000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003400: 2074 6573 745f 6e65 6564 735f 666b 3d54   test_needs_fk=T
-00003410: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00003420: 2020 2020 2020 2020 2065 7874 656e 645f           extend_
-00003430: 6578 6973 7469 6e67 3d54 7275 652c 0a20  existing=True,. 
-00003440: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00003450: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003460: 2020 6e6f 6e63 6f6c 5f69 6478 5f74 6573    noncol_idx_tes
-00003470: 745f 706b 203d 2054 6162 6c65 280a 2020  t_pk = Table(.  
-00003480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003490: 2020 226e 6f6e 636f 6c5f 6964 785f 7465    "noncol_idx_te
-000034a0: 7374 5f70 6b22 2c0a 2020 2020 2020 2020  st_pk",.        
-000034b0: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
-000034c0: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
-000034d0: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
-000034e0: 2822 6964 222c 2073 716c 616c 6368 656d  ("id", sqlalchem
-000034f0: 792e 496e 7465 6765 722c 2070 7269 6d61  y.Integer, prima
-00003500: 7279 5f6b 6579 3d54 7275 6529 2c0a 2020  ry_key=True),.  
-00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003520: 2020 436f 6c75 6d6e 2822 7122 2c20 7371    Column("q", sq
-00003530: 6c61 6c63 6865 6d79 2e53 7472 696e 6728  lalchemy.String(
-00003540: 3529 292c 0a20 2020 2020 2020 2020 2020  5)),.           
-00003550: 2020 2020 2020 2020 2074 6573 745f 6e65           test_ne
-00003560: 6564 735f 666b 3d54 7275 652c 0a20 2020  eds_fk=True,.   
-00003570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003580: 2065 7874 656e 645f 6578 6973 7469 6e67   extend_existing
-00003590: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
-000035a0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-000035b0: 2020 2020 2020 2020 2020 6966 2074 6573            if tes
-000035c0: 7469 6e67 2e72 6571 7569 7265 732e 696e  ting.requires.in
-000035d0: 6465 7865 735f 7769 7468 5f61 7363 6465  dexes_with_ascde
-000035e0: 7363 2e65 6e61 626c 6564 3a0a 2020 2020  sc.enabled:.    
-000035f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003600: 7371 6c61 6c63 6865 6d79 2e49 6e64 6578  sqlalchemy.Index
-00003610: 2822 6e6f 6e63 6f6c 5f69 6478 5f6e 6f70  ("noncol_idx_nop
-00003620: 6b22 2c20 6e6f 6e63 6f6c 5f69 6478 5f74  k", noncol_idx_t
-00003630: 6573 745f 6e6f 706b 2e63 2e71 2e64 6573  est_nopk.c.q.des
-00003640: 6328 2929 0a20 2020 2020 2020 2020 2020  c()).           
-00003650: 2020 2020 2020 2020 2073 716c 616c 6368           sqlalch
-00003660: 656d 792e 496e 6465 7828 226e 6f6e 636f  emy.Index("nonco
-00003670: 6c5f 6964 785f 706b 222c 206e 6f6e 636f  l_idx_pk", nonco
-00003680: 6c5f 6964 785f 7465 7374 5f70 6b2e 632e  l_idx_test_pk.c.
-00003690: 712e 6465 7363 2829 290a 0a20 2020 2020  q.desc())..     
-000036a0: 2020 2069 6620 7465 7374 696e 672e 7265     if testing.re
-000036b0: 7175 6972 6573 2e76 6965 775f 636f 6c75  quires.view_colu
-000036c0: 6d6e 5f72 6566 6c65 6374 696f 6e2e 656e  mn_reflection.en
-000036d0: 6162 6c65 643a 0a20 2020 2020 2020 2020  abled:.         
-000036e0: 2020 2063 6c73 2e64 6566 696e 655f 7669     cls.define_vi
-000036f0: 6577 7328 6d65 7461 6461 7461 2c20 7363  ews(metadata, sc
-00003700: 6865 6d61 290a 0a20 2020 2040 7465 7374  hema)..    @test
-00003710: 696e 672e 636f 6d62 696e 6174 696f 6e73  ing.combinations
-00003720: 2828 4661 6c73 652c 292c 2061 7267 6e61  ((False,), argna
-00003730: 6d65 733d 2275 7365 5f73 6368 656d 6122  mes="use_schema"
-00003740: 290a 2020 2020 4074 6573 7469 6e67 2e72  ).    @testing.r
-00003750: 6571 7569 7265 732e 666f 7265 6967 6e5f  equires.foreign_
-00003760: 6b65 795f 636f 6e73 7472 6169 6e74 5f72  key_constraint_r
-00003770: 6566 6c65 6374 696f 6e0a 2020 2020 6465  eflection.    de
-00003780: 6620 7465 7374 5f67 6574 5f66 6f72 6569  f test_get_forei
-00003790: 676e 5f6b 6579 7328 7365 6c66 2c20 636f  gn_keys(self, co
-000037a0: 6e6e 6563 7469 6f6e 2c20 7573 655f 7363  nnection, use_sc
-000037b0: 6865 6d61 293a 0a20 2020 2020 2020 2069  hema):.        i
-000037c0: 6620 7573 655f 7363 6865 6d61 3a0a 2020  f use_schema:.  
-000037d0: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
-000037e0: 203d 2063 6f6e 6669 672e 7465 7374 5f73   = config.test_s
-000037f0: 6368 656d 610a 2020 2020 2020 2020 656c  chema.        el
-00003800: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00003810: 7363 6865 6d61 203d 204e 6f6e 650a 0a20  schema = None.. 
-00003820: 2020 2020 2020 2075 7365 7273 2c20 6164         users, ad
-00003830: 6472 6573 7365 7320 3d20 2873 656c 662e  dresses = (self.
-00003840: 7461 626c 6573 2e75 7365 7273 2c20 7365  tables.users, se
-00003850: 6c66 2e74 6162 6c65 732e 656d 6169 6c5f  lf.tables.email_
-00003860: 6164 6472 6573 7365 7329 0a20 2020 2020  addresses).     
-00003870: 2020 2069 6e73 7020 3d20 696e 7370 6563     insp = inspec
-00003880: 7428 636f 6e6e 6563 7469 6f6e 290a 2020  t(connection).  
-00003890: 2020 2020 2020 6578 7065 6374 6564 5f73        expected_s
-000038a0: 6368 656d 6120 3d20 7363 6865 6d61 0a20  chema = schema. 
-000038b0: 2020 2020 2020 2023 2075 7365 7273 0a0a         # users..
-000038c0: 2020 2020 2020 2020 6966 2074 6573 7469          if testi
-000038d0: 6e67 2e72 6571 7569 7265 732e 7365 6c66  ng.requires.self
-000038e0: 5f72 6566 6572 656e 7469 616c 5f66 6f72  _referential_for
-000038f0: 6569 676e 5f6b 6579 732e 656e 6162 6c65  eign_keys.enable
-00003900: 643a 0a20 2020 2020 2020 2020 2020 2075  d:.            u
-00003910: 7365 7273 5f66 6b65 7973 203d 2069 6e73  sers_fkeys = ins
-00003920: 702e 6765 745f 666f 7265 6967 6e5f 6b65  p.get_foreign_ke
-00003930: 7973 2875 7365 7273 2e6e 616d 652c 2073  ys(users.name, s
-00003940: 6368 656d 613d 7363 6865 6d61 290a 2020  chema=schema).  
-00003950: 2020 2020 2020 2020 2020 666b 6579 3120            fkey1 
-00003960: 3d20 7573 6572 735f 666b 6579 735b 305d  = users_fkeys[0]
-00003970: 0a0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
-00003980: 7468 2074 6573 7469 6e67 2e72 6571 7569  th testing.requi
-00003990: 7265 732e 6e61 6d65 645f 636f 6e73 7472  res.named_constr
-000039a0: 6169 6e74 732e 6661 696c 5f69 6628 293a  aints.fail_if():
-000039b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000039c0: 2065 715f 2866 6b65 7931 5b22 6e61 6d65   eq_(fkey1["name
-000039d0: 225d 2c20 2275 7365 725f 6964 5f66 6b22  "], "user_id_fk"
-000039e0: 290a 0a20 2020 2020 2020 2020 2020 2065  )..            e
-000039f0: 715f 2866 6b65 7931 5b22 7265 6665 7272  q_(fkey1["referr
-00003a00: 6564 5f73 6368 656d 6122 5d2c 2065 7870  ed_schema"], exp
-00003a10: 6563 7465 645f 7363 6865 6d61 290a 2020  ected_schema).  
-00003a20: 2020 2020 2020 2020 2020 6571 5f28 666b            eq_(fk
-00003a30: 6579 315b 2272 6566 6572 7265 645f 7461  ey1["referred_ta
-00003a40: 626c 6522 5d2c 2075 7365 7273 2e6e 616d  ble"], users.nam
-00003a50: 6529 0a20 2020 2020 2020 2020 2020 2065  e).            e
-00003a60: 715f 2866 6b65 7931 5b22 7265 6665 7272  q_(fkey1["referr
-00003a70: 6564 5f63 6f6c 756d 6e73 225d 2c20 5b22  ed_columns"], ["
-00003a80: 7573 6572 5f69 6422 5d29 0a20 2020 2020  user_id"]).     
-00003a90: 2020 2020 2020 2069 6620 7465 7374 696e         if testin
-00003aa0: 672e 7265 7175 6972 6573 2e73 656c 665f  g.requires.self_
-00003ab0: 7265 6665 7265 6e74 6961 6c5f 666f 7265  referential_fore
-00003ac0: 6967 6e5f 6b65 7973 2e65 6e61 626c 6564  ign_keys.enabled
-00003ad0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003ae0: 2020 6571 5f28 666b 6579 315b 2263 6f6e    eq_(fkey1["con
-00003af0: 7374 7261 696e 6564 5f63 6f6c 756d 6e73  strained_columns
-00003b00: 225d 2c20 5b22 7061 7265 6e74 5f75 7365  "], ["parent_use
-00003b10: 725f 6964 225d 290a 0a20 2020 2020 2020  r_id"])..       
-00003b20: 2023 2061 6464 7265 7373 6573 0a20 2020   # addresses.   
-00003b30: 2020 2020 2061 6464 725f 666b 6579 7320       addr_fkeys 
-00003b40: 3d20 696e 7370 2e67 6574 5f66 6f72 6569  = insp.get_forei
-00003b50: 676e 5f6b 6579 7328 6164 6472 6573 7365  gn_keys(addresse
-00003b60: 732e 6e61 6d65 2c20 7363 6865 6d61 3d73  s.name, schema=s
-00003b70: 6368 656d 6129 0a20 2020 2020 2020 2066  chema).        f
-00003b80: 6b65 7931 203d 2061 6464 725f 666b 6579  key1 = addr_fkey
-00003b90: 735b 305d 0a0a 2020 2020 2020 2020 7769  s[0]..        wi
-00003ba0: 7468 2074 6573 7469 6e67 2e72 6571 7569  th testing.requi
-00003bb0: 7265 732e 696d 706c 6963 6974 6c79 5f6e  res.implicitly_n
-00003bc0: 616d 6564 5f63 6f6e 7374 7261 696e 7473  amed_constraints
-00003bd0: 2e66 6169 6c5f 6966 2829 3a0a 2020 2020  .fail_if():.    
-00003be0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00003bf0: 6572 745f 2866 6b65 7931 5b22 6e61 6d65  ert_(fkey1["name
-00003c00: 225d 2069 7320 6e6f 7420 4e6f 6e65 290a  "] is not None).
-00003c10: 0a20 2020 2020 2020 2065 715f 2866 6b65  .        eq_(fke
-00003c20: 7931 5b22 7265 6665 7272 6564 5f73 6368  y1["referred_sch
-00003c30: 656d 6122 5d2c 2065 7870 6563 7465 645f  ema"], expected_
-00003c40: 7363 6865 6d61 290a 2020 2020 2020 2020  schema).        
-00003c50: 6571 5f28 666b 6579 315b 2272 6566 6572  eq_(fkey1["refer
-00003c60: 7265 645f 7461 626c 6522 5d2c 2075 7365  red_table"], use
-00003c70: 7273 2e6e 616d 6529 0a20 2020 2020 2020  rs.name).       
-00003c80: 2065 715f 2866 6b65 7931 5b22 7265 6665   eq_(fkey1["refe
-00003c90: 7272 6564 5f63 6f6c 756d 6e73 225d 2c20  rred_columns"], 
-00003ca0: 5b22 7573 6572 5f69 6422 5d29 0a20 2020  ["user_id"]).   
-00003cb0: 2020 2020 2065 715f 2866 6b65 7931 5b22       eq_(fkey1["
-00003cc0: 636f 6e73 7472 6169 6e65 645f 636f 6c75  constrained_colu
-00003cd0: 6d6e 7322 5d2c 205b 2272 656d 6f74 655f  mns"], ["remote_
-00003ce0: 7573 6572 5f69 6422 5d29 0a0a 2020 2020  user_id"])..    
-00003cf0: 4074 6573 7469 6e67 2e72 6571 7569 7265  @testing.require
-00003d00: 732e 666f 7265 6967 6e5f 6b65 795f 636f  s.foreign_key_co
-00003d10: 6e73 7472 6169 6e74 5f72 6566 6c65 6374  nstraint_reflect
-00003d20: 696f 6e0a 2020 2020 4074 6573 7469 6e67  ion.    @testing
-00003d30: 2e63 6f6d 6269 6e61 7469 6f6e 7328 0a20  .combinations(. 
-00003d40: 2020 2020 2020 2028 4e6f 6e65 2c20 5472         (None, Tr
-00003d50: 7565 2c20 4661 6c73 652c 2046 616c 7365  ue, False, False
-00003d60: 292c 0a20 2020 2020 2020 2028 4e6f 6e65  ),.        (None
-00003d70: 2c20 5472 7565 2c20 4661 6c73 652c 2054  , True, False, T
-00003d80: 7275 652c 2074 6573 7469 6e67 2e72 6571  rue, testing.req
-00003d90: 7569 7265 732e 7363 6865 6d61 7329 2c0a  uires.schemas),.
-00003da0: 2020 2020 2020 2020 2822 666f 7265 6967          ("foreig
-00003db0: 6e5f 6b65 7922 2c20 5472 7565 2c20 4661  n_key", True, Fa
-00003dc0: 6c73 652c 2046 616c 7365 292c 0a20 2020  lse, False),.   
-00003dd0: 2020 2020 2028 4e6f 6e65 2c20 4661 6c73       (None, Fals
-00003de0: 652c 2046 616c 7365 2c20 4661 6c73 6529  e, False, False)
-00003df0: 2c0a 2020 2020 2020 2020 284e 6f6e 652c  ,.        (None,
-00003e00: 2046 616c 7365 2c20 4661 6c73 652c 2054   False, False, T
-00003e10: 7275 652c 2074 6573 7469 6e67 2e72 6571  rue, testing.req
-00003e20: 7569 7265 732e 7363 6865 6d61 7329 2c0a  uires.schemas),.
-00003e30: 2020 2020 2020 2020 284e 6f6e 652c 2054          (None, T
-00003e40: 7275 652c 2046 616c 7365 2c20 4661 6c73  rue, False, Fals
-00003e50: 6529 2c0a 2020 2020 2020 2020 284e 6f6e  e),.        (Non
-00003e60: 652c 2054 7275 652c 2046 616c 7365 2c20  e, True, False, 
-00003e70: 5472 7565 2c20 7465 7374 696e 672e 7265  True, testing.re
-00003e80: 7175 6972 6573 2e73 6368 656d 6173 292c  quires.schemas),
-00003e90: 0a20 2020 2020 2020 2061 7267 6e61 6d65  .        argname
-00003ea0: 733d 226f 7264 6572 5f62 792c 696e 636c  s="order_by,incl
-00003eb0: 7564 655f 706c 6169 6e2c 696e 636c 7564  ude_plain,includ
-00003ec0: 655f 7669 6577 732c 7573 655f 7363 6865  e_views,use_sche
-00003ed0: 6d61 222c 0a20 2020 2029 0a20 2020 2064  ma",.    ).    d
-00003ee0: 6566 2074 6573 745f 6765 745f 7461 626c  ef test_get_tabl
-00003ef0: 655f 6e61 6d65 7328 0a20 2020 2020 2020  e_names(.       
-00003f00: 2073 656c 662c 2063 6f6e 6e65 6374 696f   self, connectio
-00003f10: 6e2c 206f 7264 6572 5f62 792c 2069 6e63  n, order_by, inc
-00003f20: 6c75 6465 5f70 6c61 696e 2c20 696e 636c  lude_plain, incl
-00003f30: 7564 655f 7669 6577 732c 2075 7365 5f73  ude_views, use_s
-00003f40: 6368 656d 610a 2020 2020 293a 0a0a 2020  chema.    ):..  
-00003f50: 2020 2020 2020 6966 2075 7365 5f73 6368        if use_sch
-00003f60: 656d 613a 0a20 2020 2020 2020 2020 2020  ema:.           
-00003f70: 2073 6368 656d 6120 3d20 636f 6e66 6967   schema = config
-00003f80: 2e74 6573 745f 7363 6865 6d61 0a20 2020  .test_schema.   
-00003f90: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00003fa0: 2020 2020 2020 2073 6368 656d 6120 3d20         schema = 
-00003fb0: 4e6f 6e65 0a0a 2020 2020 2020 2020 5f69  None..        _i
-00003fc0: 676e 6f72 655f 7461 626c 6573 203d 205b  gnore_tables = [
-00003fd0: 0a20 2020 2020 2020 2020 2020 2022 6163  .            "ac
-00003fe0: 636f 756e 7422 2c0a 2020 2020 2020 2020  count",.        
-00003ff0: 2020 2020 2261 6c65 6d62 6963 5f76 6572      "alembic_ver
-00004000: 7369 6f6e 222c 0a20 2020 2020 2020 2020  sion",.         
-00004010: 2020 2022 6279 7465 735f 7461 626c 6522     "bytes_table"
-00004020: 2c0a 2020 2020 2020 2020 2020 2020 2263  ,.            "c
-00004030: 6f6d 6d65 6e74 5f74 6573 7422 2c0a 2020  omment_test",.  
-00004040: 2020 2020 2020 2020 2020 2264 6174 655f            "date_
-00004050: 7461 626c 6522 2c0a 2020 2020 2020 2020  table",.        
-00004060: 2020 2020 226e 6f6e 636f 6c5f 6964 785f      "noncol_idx_
-00004070: 7465 7374 5f70 6b22 2c0a 2020 2020 2020  test_pk",.      
-00004080: 2020 2020 2020 226e 6f6e 636f 6c5f 6964        "noncol_id
-00004090: 785f 7465 7374 5f6e 6f70 6b22 2c0a 2020  x_test_nopk",.  
-000040a0: 2020 2020 2020 2020 2020 226c 6f63 616c            "local
-000040b0: 5f74 6162 6c65 222c 0a20 2020 2020 2020  _table",.       
-000040c0: 2020 2020 2022 7265 6d6f 7465 5f74 6162       "remote_tab
-000040d0: 6c65 222c 0a20 2020 2020 2020 2020 2020  le",.           
-000040e0: 2022 7265 6d6f 7465 5f74 6162 6c65 5f32   "remote_table_2
-000040f0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00004100: 7465 7874 5f74 6162 6c65 222c 0a20 2020  text_table",.   
-00004110: 2020 2020 2020 2020 2022 7573 6572 5f74           "user_t
-00004120: 6d70 222c 0a20 2020 2020 2020 205d 0a0a  mp",.        ]..
-00004130: 2020 2020 2020 2020 696e 7370 203d 2069          insp = i
-00004140: 6e73 7065 6374 2863 6f6e 6e65 6374 696f  nspect(connectio
-00004150: 6e29 0a0a 2020 2020 2020 2020 6966 2069  n)..        if i
-00004160: 6e63 6c75 6465 5f76 6965 7773 3a0a 2020  nclude_views:.  
-00004170: 2020 2020 2020 2020 2020 7461 626c 655f            table_
-00004180: 6e61 6d65 7320 3d20 696e 7370 2e67 6574  names = insp.get
-00004190: 5f76 6965 775f 6e61 6d65 7328 7363 6865  _view_names(sche
-000041a0: 6d61 290a 2020 2020 2020 2020 2020 2020  ma).            
-000041b0: 7461 626c 655f 6e61 6d65 732e 736f 7274  table_names.sort
-000041c0: 2829 0a20 2020 2020 2020 2020 2020 2061  ().            a
-000041d0: 6e73 7765 7220 3d20 5b22 656d 6169 6c5f  nswer = ["email_
-000041e0: 6164 6472 6573 7365 735f 7622 2c20 2275  addresses_v", "u
-000041f0: 7365 7273 5f76 225d 0a20 2020 2020 2020  sers_v"].       
-00004200: 2020 2020 2065 715f 2873 6f72 7465 6428       eq_(sorted(
-00004210: 7461 626c 655f 6e61 6d65 7329 2c20 616e  table_names), an
-00004220: 7377 6572 290a 0a20 2020 2020 2020 2069  swer)..        i
-00004230: 6620 696e 636c 7564 655f 706c 6169 6e3a  f include_plain:
-00004240: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00004250: 6f72 6465 725f 6279 3a0a 2020 2020 2020  order_by:.      
-00004260: 2020 2020 2020 2020 2020 7461 626c 6573            tables
-00004270: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-00004280: 2020 2020 2020 2020 2072 6563 5b30 5d0a           rec[0].
-00004290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042a0: 2020 2020 666f 7220 7265 6320 696e 2069      for rec in i
-000042b0: 6e73 702e 6765 745f 736f 7274 6564 5f74  nsp.get_sorted_t
-000042c0: 6162 6c65 5f61 6e64 5f66 6b63 5f6e 616d  able_and_fkc_nam
-000042d0: 6573 2873 6368 656d 6129 0a20 2020 2020  es(schema).     
-000042e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000042f0: 6620 7265 635b 305d 0a20 2020 2020 2020  f rec[0].       
-00004300: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00004310: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00004320: 2020 2020 2020 2020 2020 2020 2074 6162               tab
-00004330: 6c65 7320 3d20 696e 7370 2e67 6574 5f74  les = insp.get_t
-00004340: 6162 6c65 5f6e 616d 6573 2873 6368 656d  able_names(schem
-00004350: 6129 0a20 2020 2020 2020 2020 2020 2074  a).            t
-00004360: 6162 6c65 5f6e 616d 6573 203d 205b 7420  able_names = [t 
-00004370: 666f 7220 7420 696e 2074 6162 6c65 7320  for t in tables 
-00004380: 6966 2074 206e 6f74 2069 6e20 5f69 676e  if t not in _ign
-00004390: 6f72 655f 7461 626c 6573 5d0a 0a20 2020  ore_tables]..   
-000043a0: 2020 2020 2020 2020 2069 6620 6f72 6465           if orde
-000043b0: 725f 6279 203d 3d20 2266 6f72 6569 676e  r_by == "foreign
-000043c0: 5f6b 6579 223a 0a20 2020 2020 2020 2020  _key":.         
-000043d0: 2020 2020 2020 2061 6e73 7765 7220 3d20         answer = 
-000043e0: 5b22 7573 6572 7322 2c20 2265 6d61 696c  ["users", "email
-000043f0: 5f61 6464 7265 7373 6573 222c 2022 6469  _addresses", "di
-00004400: 6e67 616c 696e 6773 225d 0a20 2020 2020  ngalings"].     
-00004410: 2020 2020 2020 2020 2020 2065 715f 2874             eq_(t
-00004420: 6162 6c65 5f6e 616d 6573 2c20 616e 7377  able_names, answ
-00004430: 6572 290a 2020 2020 2020 2020 2020 2020  er).            
-00004440: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00004450: 2020 2020 2020 616e 7377 6572 203d 205b        answer = [
-00004460: 2264 696e 6761 6c69 6e67 7322 2c20 2265  "dingalings", "e
-00004470: 6d61 696c 5f61 6464 7265 7373 6573 222c  mail_addresses",
-00004480: 2022 7573 6572 7322 5d0a 2020 2020 2020   "users"].      
-00004490: 2020 2020 2020 2020 2020 6571 5f28 736f            eq_(so
-000044a0: 7274 6564 2874 6162 6c65 5f6e 616d 6573  rted(table_names
-000044b0: 292c 2061 6e73 7765 7229 0a0a 2020 2020  ), answer)..    
-000044c0: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-000044d0: 2064 6566 2064 6566 696e 655f 7465 6d70   def define_temp
-000044e0: 5f74 6162 6c65 7328 636c 732c 206d 6574  _tables(cls, met
-000044f0: 6164 6174 6129 3a0a 2020 2020 2020 2020  adata):.        
-00004500: 2222 220a 2020 2020 2020 2020 5350 414e  """.        SPAN
-00004510: 4e45 5220 4f56 4552 5249 4445 3a0a 0a20  NER OVERRIDE:.. 
-00004520: 2020 2020 2020 2049 6e20 436c 6f75 6420         In Cloud 
-00004530: 5370 616e 6e65 7220 756e 6971 7565 2069  Spanner unique i
-00004540: 6e64 6578 6573 2061 7265 2075 7365 6420  ndexes are used 
-00004550: 696e 7374 6561 6420 6f66 2064 6972 6563  instead of direc
-00004560: 746c 790a 2020 2020 2020 2020 6372 6561  tly.        crea
-00004570: 7469 6e67 2075 6e69 7175 6520 636f 6e73  ting unique cons
-00004580: 7472 6169 6e74 732e 204f 7665 7272 6964  traints. Overrid
-00004590: 696e 6720 7468 6520 7465 7374 2074 6f20  ing the test to 
-000045a0: 7265 706c 6163 650a 2020 2020 2020 2020  replace.        
-000045b0: 636f 6e73 7472 6169 6e74 7320 7769 7468  constraints with
-000045c0: 2069 6e64 6578 6573 2069 6e20 7465 7374   indexes in test
-000045d0: 696e 6720 6461 7461 2e0a 2020 2020 2020  ing data..      
-000045e0: 2020 2222 220a 2020 2020 2020 2020 6b77    """.        kw
-000045f0: 203d 2074 656d 705f 7461 626c 655f 6b65   = temp_table_ke
-00004600: 7977 6f72 645f 6172 6773 2863 6f6e 6669  yword_args(confi
-00004610: 672c 2063 6f6e 6669 672e 6462 290a 2020  g, config.db).  
-00004620: 2020 2020 2020 7573 6572 5f74 6d70 203d        user_tmp =
-00004630: 2054 6162 6c65 280a 2020 2020 2020 2020   Table(.        
-00004640: 2020 2020 2275 7365 725f 746d 7022 2c0a      "user_tmp",.
-00004650: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
-00004660: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
-00004670: 2020 436f 6c75 6d6e 2822 6964 222c 2073    Column("id", s
-00004680: 716c 616c 6368 656d 792e 494e 542c 2070  qlalchemy.INT, p
-00004690: 7269 6d61 7279 5f6b 6579 3d54 7275 6529  rimary_key=True)
-000046a0: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
-000046b0: 6c75 6d6e 2822 6e61 6d65 222c 2073 716c  lumn("name", sql
-000046c0: 616c 6368 656d 792e 5641 5243 4841 5228  alchemy.VARCHAR(
-000046d0: 3530 2929 2c0a 2020 2020 2020 2020 2020  50)),.          
-000046e0: 2020 436f 6c75 6d6e 2822 666f 6f22 2c20    Column("foo", 
-000046f0: 7371 6c61 6c63 6865 6d79 2e49 4e54 292c  sqlalchemy.INT),
-00004700: 0a20 2020 2020 2020 2020 2020 2073 716c  .            sql
-00004710: 616c 6368 656d 792e 496e 6465 7828 2275  alchemy.Index("u
-00004720: 7365 725f 746d 705f 7571 222c 2022 6e61  ser_tmp_uq", "na
-00004730: 6d65 222c 2075 6e69 7175 653d 5472 7565  me", unique=True
-00004740: 292c 0a20 2020 2020 2020 2020 2020 2073  ),.            s
-00004750: 716c 616c 6368 656d 792e 496e 6465 7828  qlalchemy.Index(
-00004760: 2275 7365 725f 746d 705f 6978 222c 2022  "user_tmp_ix", "
-00004770: 666f 6f22 292c 0a20 2020 2020 2020 2020  foo"),.         
-00004780: 2020 2065 7874 656e 645f 6578 6973 7469     extend_existi
-00004790: 6e67 3d54 7275 652c 0a20 2020 2020 2020  ng=True,.       
-000047a0: 2020 2020 202a 2a6b 772c 0a20 2020 2020       **kw,.     
-000047b0: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
-000047c0: 280a 2020 2020 2020 2020 2020 2020 7465  (.            te
-000047d0: 7374 696e 672e 7265 7175 6972 6573 2e76  sting.requires.v
-000047e0: 6965 775f 7265 666c 6563 7469 6f6e 2e65  iew_reflection.e
-000047f0: 6e61 626c 6564 0a20 2020 2020 2020 2020  nabled.         
-00004800: 2020 2061 6e64 2074 6573 7469 6e67 2e72     and testing.r
-00004810: 6571 7569 7265 732e 7465 6d70 6f72 6172  equires.temporar
-00004820: 795f 7669 6577 732e 656e 6162 6c65 640a  y_views.enabled.
-00004830: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-00004840: 2020 2020 2020 2065 7665 6e74 2e6c 6973         event.lis
-00004850: 7465 6e28 0a20 2020 2020 2020 2020 2020  ten(.           
-00004860: 2020 2020 2075 7365 725f 746d 702c 0a20       user_tmp,. 
-00004870: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004880: 6166 7465 725f 6372 6561 7465 222c 0a20  after_create",. 
-00004890: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-000048a0: 444c 2822 6372 6561 7465 2074 656d 706f  DL("create tempo
-000048b0: 7261 7279 2076 6965 7720 7573 6572 5f74  rary view user_t
-000048c0: 6d70 5f76 2061 7320 2220 2273 656c 6563  mp_v as " "selec
-000048d0: 7420 2a20 6672 6f6d 2075 7365 725f 746d  t * from user_tm
-000048e0: 7022 292c 0a20 2020 2020 2020 2020 2020  p"),.           
-000048f0: 2029 0a20 2020 2020 2020 2020 2020 2065   ).            e
-00004900: 7665 6e74 2e6c 6973 7465 6e28 7573 6572  vent.listen(user
-00004910: 5f74 6d70 2c20 2262 6566 6f72 655f 6472  _tmp, "before_dr
-00004920: 6f70 222c 2044 444c 2822 6472 6f70 2076  op", DDL("drop v
-00004930: 6965 7720 7573 6572 5f74 6d70 5f76 2229  iew user_tmp_v")
-00004940: 290a 0a20 2020 2040 7465 7374 696e 672e  )..    @testing.
-00004950: 7072 6f76 6964 655f 6d65 7461 6461 7461  provide_metadata
-00004960: 0a20 2020 2064 6566 2074 6573 745f 7265  .    def test_re
-00004970: 666c 6563 745f 7374 7269 6e67 5f63 6f6c  flect_string_col
-00004980: 756d 6e5f 6d61 785f 6c65 6e28 7365 6c66  umn_max_len(self
-00004990: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-000049a0: 2020 2020 2020 2053 5041 4e4e 4552 2053         SPANNER S
-000049b0: 5045 4349 4649 4320 5445 5354 3a0a 0a20  PECIFIC TEST:.. 
-000049c0: 2020 2020 2020 2049 6e20 5370 616e 6e65         In Spanne
-000049d0: 7220 636f 6c75 6d6e 206f 6620 7468 6520  r column of the 
-000049e0: 5354 5249 4e47 2074 7970 6520 6361 6e20  STRING type can 
-000049f0: 6265 0a20 2020 2020 2020 2063 7265 6174  be.        creat
-00004a00: 6564 2077 6974 6820 7369 7a65 2064 6566  ed with size def
-00004a10: 696e 6564 2061 7320 4d41 582e 2054 6865  ined as MAX. The
-00004a20: 2074 6573 740a 2020 2020 2020 2020 6368   test.        ch
-00004a30: 6563 6b73 2074 6861 7420 7375 6368 2061  ecks that such a
-00004a40: 2063 6f6c 756d 6e20 6973 2063 6f72 7265   column is corre
-00004a50: 6374 6c79 2072 6566 6c65 6374 6564 2e0a  ctly reflected..
-00004a60: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00004a70: 2020 2020 6d65 7461 6461 7461 203d 204d      metadata = M
-00004a80: 6574 6144 6174 6128 7365 6c66 2e62 696e  etaData(self.bin
-00004a90: 6429 0a20 2020 2020 2020 2054 6162 6c65  d).        Table
-00004aa0: 2822 7465 7874 5f74 6162 6c65 222c 206d  ("text_table", m
-00004ab0: 6574 6164 6174 612c 2043 6f6c 756d 6e28  etadata, Column(
-00004ac0: 2254 6573 7443 6f6c 756d 6e22 2c20 5465  "TestColumn", Te
-00004ad0: 7874 2c20 6e75 6c6c 6162 6c65 3d46 616c  xt, nullable=Fal
-00004ae0: 7365 2929 0a20 2020 2020 2020 206d 6574  se)).        met
-00004af0: 6164 6174 612e 6372 6561 7465 5f61 6c6c  adata.create_all
-00004b00: 2829 0a0a 2020 2020 2020 2020 5461 626c  ()..        Tabl
-00004b10: 6528 2274 6578 745f 7461 626c 6522 2c20  e("text_table", 
-00004b20: 6d65 7461 6461 7461 2c20 6175 746f 6c6f  metadata, autolo
-00004b30: 6164 3d54 7275 6529 0a0a 2020 2020 6465  ad=True)..    de
-00004b40: 6620 7465 7374 5f72 6566 6c65 6374 5f62  f test_reflect_b
-00004b50: 7974 6573 5f63 6f6c 756d 6e5f 6d61 785f  ytes_column_max_
-00004b60: 6c65 6e28 7365 6c66 293a 0a20 2020 2020  len(self):.     
-00004b70: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
-00004b80: 5041 4e4e 4552 2053 5045 4349 4649 4320  PANNER SPECIFIC 
-00004b90: 5445 5354 3a0a 0a20 2020 2020 2020 2049  TEST:..        I
-00004ba0: 6e20 5370 616e 6e65 7220 636f 6c75 6d6e  n Spanner column
-00004bb0: 206f 6620 7468 6520 4259 5445 5320 7479   of the BYTES ty
-00004bc0: 7065 2063 616e 2062 650a 2020 2020 2020  pe can be.      
-00004bd0: 2020 6372 6561 7465 6420 7769 7468 2073    created with s
-00004be0: 697a 6520 6465 6669 6e65 6420 6173 204d  ize defined as M
-00004bf0: 4158 2e20 5468 6520 7465 7374 0a20 2020  AX. The test.   
-00004c00: 2020 2020 2063 6865 636b 7320 7468 6174       checks that
-00004c10: 2073 7563 6820 6120 636f 6c75 6d6e 2069   such a column i
-00004c20: 7320 636f 7272 6563 746c 7920 7265 666c  s correctly refl
-00004c30: 6563 7465 642e 0a20 2020 2020 2020 2022  ected..        "
-00004c40: 2222 0a20 2020 2020 2020 206d 6574 6164  "".        metad
-00004c50: 6174 6120 3d20 4d65 7461 4461 7461 2873  ata = MetaData(s
-00004c60: 656c 662e 6269 6e64 290a 2020 2020 2020  elf.bind).      
-00004c70: 2020 5461 626c 6528 0a20 2020 2020 2020    Table(.       
-00004c80: 2020 2020 2022 6279 7465 735f 7461 626c       "bytes_tabl
-00004c90: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00004ca0: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
-00004cb0: 2020 2020 2020 436f 6c75 6d6e 2822 5465        Column("Te
-00004cc0: 7374 436f 6c75 6d6e 222c 204c 6172 6765  stColumn", Large
-00004cd0: 4269 6e61 7279 2c20 6e75 6c6c 6162 6c65  Binary, nullable
-00004ce0: 3d46 616c 7365 292c 0a20 2020 2020 2020  =False),.       
-00004cf0: 2029 0a20 2020 2020 2020 206d 6574 6164   ).        metad
-00004d00: 6174 612e 6372 6561 7465 5f61 6c6c 2829  ata.create_all()
-00004d10: 0a0a 2020 2020 2020 2020 5461 626c 6528  ..        Table(
-00004d20: 2262 7974 6573 5f74 6162 6c65 222c 206d  "bytes_table", m
-00004d30: 6574 6164 6174 612c 2061 7574 6f6c 6f61  etadata, autoloa
-00004d40: 643d 5472 7565 290a 0a20 2020 2040 7465  d=True)..    @te
-00004d50: 7374 696e 672e 636f 6d62 696e 6174 696f  sting.combinatio
-00004d60: 6e73 280a 2020 2020 2020 2020 2854 7275  ns(.        (Tru
-00004d70: 652c 2074 6573 7469 6e67 2e72 6571 7569  e, testing.requi
-00004d80: 7265 732e 7363 6865 6d61 7329 2c20 2846  res.schemas), (F
-00004d90: 616c 7365 2c29 2c20 6172 676e 616d 6573  alse,), argnames
-00004da0: 3d22 7573 655f 7363 6865 6d61 220a 2020  ="use_schema".  
-00004db0: 2020 290a 2020 2020 4074 6573 7469 6e67    ).    @testing
-00004dc0: 2e72 6571 7569 7265 732e 756e 6971 7565  .requires.unique
-00004dd0: 5f63 6f6e 7374 7261 696e 745f 7265 666c  _constraint_refl
-00004de0: 6563 7469 6f6e 0a20 2020 2064 6566 2074  ection.    def t
-00004df0: 6573 745f 6765 745f 756e 6971 7565 5f63  est_get_unique_c
-00004e00: 6f6e 7374 7261 696e 7473 2873 656c 662c  onstraints(self,
-00004e10: 206d 6574 6164 6174 612c 2063 6f6e 6e65   metadata, conne
-00004e20: 6374 696f 6e2c 2075 7365 5f73 6368 656d  ction, use_schem
-00004e30: 6129 3a0a 2020 2020 2020 2020 2320 5351  a):.        # SQ
-00004e40: 4c69 7465 2064 6961 6c65 6374 206e 6565  Lite dialect nee
-00004e50: 6473 2074 6f20 7061 7273 6520 7468 6520  ds to parse the 
-00004e60: 6e61 6d65 7320 6f66 2074 6865 2063 6f6e  names of the con
-00004e70: 7374 7261 696e 7473 0a20 2020 2020 2020  straints.       
-00004e80: 2023 2073 6570 6172 6174 656c 7920 6672   # separately fr
-00004e90: 6f6d 2077 6861 7420 6974 2067 6574 7320  om what it gets 
-00004ea0: 6672 6f6d 2050 5241 474d 4120 696e 6465  from PRAGMA inde
-00004eb0: 785f 6c69 7374 2829 2c20 616e 640a 2020  x_list(), and.  
-00004ec0: 2020 2020 2020 2320 7468 656e 206d 6174        # then mat
-00004ed0: 6368 6573 2074 6865 6d20 7570 2e20 2073  ches them up.  s
-00004ee0: 6f20 7361 6d65 2073 6574 206f 6620 636f  o same set of co
-00004ef0: 6c75 6d6e 5f6e 616d 6573 2069 6e20 7477  lumn_names in tw
-00004f00: 6f0a 2020 2020 2020 2020 2320 636f 6e73  o.        # cons
-00004f10: 7472 6169 6e74 7320 7769 6c6c 2063 6f6e  traints will con
-00004f20: 6675 7365 2069 742e 2020 2020 5065 7268  fuse it.    Perh
-00004f30: 6170 7320 7765 2073 686f 756c 6420 6e6f  aps we should no
-00004f40: 206c 6f6e 6765 720a 2020 2020 2020 2020   longer.        
-00004f50: 2320 626f 7468 6572 2077 6974 6820 696e  # bother with in
-00004f60: 6465 785f 6c69 7374 2829 2068 6572 6520  dex_list() here 
-00004f70: 7369 6e63 6520 7765 2068 6176 6520 7468  since we have th
-00004f80: 6520 7768 6f6c 650a 2020 2020 2020 2020  e whole.        
-00004f90: 2320 4352 4541 5445 2054 4142 4c45 3f0a  # CREATE TABLE?.
-00004fa0: 0a20 2020 2020 2020 2069 6620 7573 655f  .        if use_
-00004fb0: 7363 6865 6d61 3a0a 2020 2020 2020 2020  schema:.        
-00004fc0: 2020 2020 7363 6865 6d61 203d 2063 6f6e      schema = con
-00004fd0: 6669 672e 7465 7374 5f73 6368 656d 610a  fig.test_schema.
-00004fe0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00004ff0: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
-00005000: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-00005010: 756e 6971 7565 7320 3d20 736f 7274 6564  uniques = sorted
-00005020: 280a 2020 2020 2020 2020 2020 2020 5b0a  (.            [.
-00005030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005040: 7b22 6e61 6d65 223a 2022 756e 6971 7565  {"name": "unique
-00005050: 5f61 222c 2022 636f 6c75 6d6e 5f6e 616d  _a", "column_nam
-00005060: 6573 223a 205b 2261 225d 7d2c 0a20 2020  es": ["a"]},.   
-00005070: 2020 2020 2020 2020 2020 2020 207b 226e               {"n
-00005080: 616d 6522 3a20 2275 6e69 7175 655f 615f  ame": "unique_a_
-00005090: 625f 6322 2c20 2263 6f6c 756d 6e5f 6e61  b_c", "column_na
-000050a0: 6d65 7322 3a20 5b22 6122 2c20 2262 222c  mes": ["a", "b",
-000050b0: 2022 6322 5d7d 2c0a 2020 2020 2020 2020   "c"]},.        
-000050c0: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
-000050d0: 2022 756e 6971 7565 5f63 5f61 5f62 222c   "unique_c_a_b",
-000050e0: 2022 636f 6c75 6d6e 5f6e 616d 6573 223a   "column_names":
-000050f0: 205b 2263 222c 2022 6122 2c20 2262 225d   ["c", "a", "b"]
-00005100: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00005110: 2020 207b 226e 616d 6522 3a20 2275 6e69     {"name": "uni
-00005120: 7175 655f 6173 635f 6b65 7922 2c20 2263  que_asc_key", "c
-00005130: 6f6c 756d 6e5f 6e61 6d65 7322 3a20 5b22  olumn_names": ["
-00005140: 6173 6322 2c20 226b 6579 225d 7d2c 0a20  asc", "key"]},. 
-00005150: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00005160: 226e 616d 6522 3a20 2269 2e68 6176 652e  "name": "i.have.
-00005170: 646f 7473 222c 2022 636f 6c75 6d6e 5f6e  dots", "column_n
-00005180: 616d 6573 223a 205b 2262 225d 7d2c 0a20  ames": ["b"]},. 
-00005190: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000051a0: 226e 616d 6522 3a20 2269 2068 6176 6520  "name": "i have 
-000051b0: 7370 6163 6573 222c 2022 636f 6c75 6d6e  spaces", "column
-000051c0: 5f6e 616d 6573 223a 205b 2263 225d 7d2c  _names": ["c"]},
-000051d0: 0a20 2020 2020 2020 2020 2020 205d 2c0a  .            ],.
-000051e0: 2020 2020 2020 2020 2020 2020 6b65 793d              key=
-000051f0: 6f70 6572 6174 6f72 2e69 7465 6d67 6574  operator.itemget
-00005200: 7465 7228 226e 616d 6522 292c 0a20 2020  ter("name"),.   
-00005210: 2020 2020 2029 0a20 2020 2020 2020 2074       ).        t
-00005220: 6162 6c65 203d 2054 6162 6c65 280a 2020  able = Table(.  
-00005230: 2020 2020 2020 2020 2020 2274 6573 7474            "testt
-00005240: 626c 222c 0a20 2020 2020 2020 2020 2020  bl",.           
-00005250: 206d 6574 6164 6174 612c 0a20 2020 2020   metadata,.     
-00005260: 2020 2020 2020 2043 6f6c 756d 6e28 2269         Column("i
-00005270: 6422 2c20 7371 6c61 6c63 6865 6d79 2e49  d", sqlalchemy.I
-00005280: 4e54 2c20 7072 696d 6172 795f 6b65 793d  NT, primary_key=
-00005290: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
-000052a0: 2020 2043 6f6c 756d 6e28 2261 222c 2053     Column("a", S
-000052b0: 7472 696e 6728 3230 2929 2c0a 2020 2020  tring(20)),.    
-000052c0: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
-000052d0: 6222 2c20 5374 7269 6e67 2833 3029 292c  b", String(30)),
-000052e0: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
-000052f0: 756d 6e28 2263 222c 2049 6e74 6567 6572  umn("c", Integer
-00005300: 292c 0a20 2020 2020 2020 2020 2020 2023  ),.            #
-00005310: 2072 6573 6572 7665 6420 6964 656e 7469   reserved identi
-00005320: 6669 6572 730a 2020 2020 2020 2020 2020  fiers.          
-00005330: 2020 436f 6c75 6d6e 2822 6173 6322 2c20    Column("asc", 
-00005340: 5374 7269 6e67 2833 3029 292c 0a20 2020  String(30)),.   
-00005350: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-00005360: 226b 6579 222c 2053 7472 696e 6728 3330  "key", String(30
-00005370: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-00005380: 7371 6c61 6c63 6865 6d79 2e49 6e64 6578  sqlalchemy.Index
-00005390: 2822 756e 6971 7565 5f61 222c 2022 6122  ("unique_a", "a"
-000053a0: 2c20 756e 6971 7565 3d54 7275 6529 2c0a  , unique=True),.
-000053b0: 2020 2020 2020 2020 2020 2020 7371 6c61              sqla
-000053c0: 6c63 6865 6d79 2e49 6e64 6578 2822 756e  lchemy.Index("un
-000053d0: 6971 7565 5f61 5f62 5f63 222c 2022 6122  ique_a_b_c", "a"
-000053e0: 2c20 2262 222c 2022 6322 2c20 756e 6971  , "b", "c", uniq
-000053f0: 7565 3d54 7275 6529 2c0a 2020 2020 2020  ue=True),.      
-00005400: 2020 2020 2020 7371 6c61 6c63 6865 6d79        sqlalchemy
-00005410: 2e49 6e64 6578 2822 756e 6971 7565 5f63  .Index("unique_c
-00005420: 5f61 5f62 222c 2022 6322 2c20 2261 222c  _a_b", "c", "a",
-00005430: 2022 6222 2c20 756e 6971 7565 3d54 7275   "b", unique=Tru
-00005440: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-00005450: 7371 6c61 6c63 6865 6d79 2e49 6e64 6578  sqlalchemy.Index
-00005460: 2822 756e 6971 7565 5f61 7363 5f6b 6579  ("unique_asc_key
-00005470: 222c 2022 6173 6322 2c20 226b 6579 222c  ", "asc", "key",
-00005480: 2075 6e69 7175 653d 5472 7565 292c 0a20   unique=True),. 
-00005490: 2020 2020 2020 2020 2020 2073 6368 656d             schem
-000054a0: 613d 7363 6865 6d61 2c0a 2020 2020 2020  a=schema,.      
-000054b0: 2020 290a 2020 2020 2020 2020 7461 626c    ).        tabl
-000054c0: 652e 6372 6561 7465 2863 6f6e 6e65 6374  e.create(connect
-000054d0: 696f 6e29 0a20 2020 2020 2020 2063 6f6e  ion).        con
-000054e0: 6e65 6374 696f 6e2e 636f 6e6e 6563 7469  nection.connecti
-000054f0: 6f6e 2e63 6f6d 6d69 7428 290a 0a20 2020  on.commit()..   
-00005500: 2020 2020 2069 6e73 7065 6374 6f72 203d       inspector =
-00005510: 2069 6e73 7065 6374 2863 6f6e 6e65 6374   inspect(connect
-00005520: 696f 6e29 0a20 2020 2020 2020 2072 6566  ion).        ref
-00005530: 6c65 6374 6564 203d 2073 6f72 7465 6428  lected = sorted(
-00005540: 0a20 2020 2020 2020 2020 2020 2069 6e73  .            ins
-00005550: 7065 6374 6f72 2e67 6574 5f75 6e69 7175  pector.get_uniqu
-00005560: 655f 636f 6e73 7472 6169 6e74 7328 2274  e_constraints("t
-00005570: 6573 7474 626c 222c 2073 6368 656d 613d  esttbl", schema=
-00005580: 7363 6865 6d61 292c 0a20 2020 2020 2020  schema),.       
-00005590: 2020 2020 206b 6579 3d6f 7065 7261 746f       key=operato
-000055a0: 722e 6974 656d 6765 7474 6572 2822 6e61  r.itemgetter("na
-000055b0: 6d65 2229 2c0a 2020 2020 2020 2020 290a  me"),.        ).
-000055c0: 0a20 2020 2020 2020 206e 616d 6573 5f74  .        names_t
-000055d0: 6861 745f 6475 706c 6963 6174 655f 696e  hat_duplicate_in
-000055e0: 6465 7820 3d20 7365 7428 290a 0a20 2020  dex = set()..   
-000055f0: 2020 2020 2066 6f72 206f 7269 672c 2072       for orig, r
-00005600: 6566 6c20 696e 207a 6970 2875 6e69 7175  efl in zip(uniqu
-00005610: 6573 2c20 7265 666c 6563 7465 6429 3a0a  es, reflected):.
-00005620: 2020 2020 2020 2020 2020 2020 2320 4469              # Di
-00005630: 6666 6572 656e 7420 6469 616c 6563 7473  fferent dialects
-00005640: 2068 616e 646c 6520 6475 706c 6963 6174   handle duplicat
-00005650: 6520 696e 6465 7820 616e 6420 636f 6e73  e index and cons
-00005660: 7472 6169 6e74 730a 2020 2020 2020 2020  traints.        
-00005670: 2020 2020 2320 6469 6666 6572 656e 746c      # differentl
-00005680: 792c 2073 6f20 6967 6e6f 7265 2074 6869  y, so ignore thi
-00005690: 7320 666c 6167 0a20 2020 2020 2020 2020  s flag.         
-000056a0: 2020 2064 7570 6520 3d20 7265 666c 2e70     dupe = refl.p
-000056b0: 6f70 2822 6475 706c 6963 6174 6573 5f69  op("duplicates_i
-000056c0: 6e64 6578 222c 204e 6f6e 6529 0a20 2020  ndex", None).   
-000056d0: 2020 2020 2020 2020 2069 6620 6475 7065           if dupe
-000056e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000056f0: 2020 6e61 6d65 735f 7468 6174 5f64 7570    names_that_dup
-00005700: 6c69 6361 7465 5f69 6e64 6578 2e61 6464  licate_index.add
-00005710: 2864 7570 6529 0a20 2020 2020 2020 2020  (dupe).         
-00005720: 2020 2065 715f 286f 7269 672c 2072 6566     eq_(orig, ref
-00005730: 6c29 0a0a 2020 2020 2020 2020 7265 666c  l)..        refl
-00005740: 6563 7465 645f 6d65 7461 6461 7461 203d  ected_metadata =
-00005750: 204d 6574 6144 6174 6128 290a 2020 2020   MetaData().    
-00005760: 2020 2020 7265 666c 6563 7465 6420 3d20      reflected = 
-00005770: 5461 626c 6528 0a20 2020 2020 2020 2020  Table(.         
-00005780: 2020 2022 7465 7374 7462 6c22 2c0a 2020     "testtbl",.  
-00005790: 2020 2020 2020 2020 2020 7265 666c 6563            reflec
-000057a0: 7465 645f 6d65 7461 6461 7461 2c0a 2020  ted_metadata,.  
-000057b0: 2020 2020 2020 2020 2020 6175 746f 6c6f            autolo
-000057c0: 6164 5f77 6974 683d 636f 6e6e 6563 7469  ad_with=connecti
-000057d0: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-000057e0: 7363 6865 6d61 3d73 6368 656d 612c 0a20  schema=schema,. 
-000057f0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00005800: 2020 2320 7465 7374 2022 6465 6475 706c    # test "dedupl
-00005810: 6963 6174 6573 2066 6f72 2069 6e64 6578  icates for index
-00005820: 2220 6c6f 6769 632e 2020 204d 7953 514c  " logic.   MySQL
-00005830: 2061 6e64 204f 7261 636c 650a 2020 2020   and Oracle.    
-00005840: 2020 2020 2320 2275 6e69 7175 6520 636f      # "unique co
-00005850: 6e73 7472 6169 6e74 7322 2061 7265 2061  nstraints" are a
-00005860: 6374 7561 6c6c 7920 756e 6971 7565 2069  ctually unique i
-00005870: 6e64 6578 6573 2028 7769 7468 2070 6f73  ndexes (with pos
-00005880: 7369 626c 650a 2020 2020 2020 2020 2320  sible.        # 
-00005890: 6578 6365 7074 696f 6e20 6f66 2061 2075  exception of a u
-000058a0: 6e69 7175 6520 7468 6174 2069 7320 6120  nique that is a 
-000058b0: 6475 7065 206f 6620 616e 6f74 6865 7220  dupe of another 
-000058c0: 6f6e 6520 696e 2074 6865 2063 6173 650a  one in the case.
-000058d0: 2020 2020 2020 2020 2320 6f66 204f 7261          # of Ora
-000058e0: 636c 6529 2e20 206d 616b 6520 7375 7265  cle).  make sure
-000058f0: 2023 2074 6865 7920 6172 656e 2774 2064   # they aren't d
-00005900: 7570 6c69 6361 7465 642e 0a20 2020 2020  uplicated..     
-00005910: 2020 2069 6478 5f6e 616d 6573 203d 2073     idx_names = s
-00005920: 6574 285b 6964 782e 6e61 6d65 2066 6f72  et([idx.name for
-00005930: 2069 6478 2069 6e20 7265 666c 6563 7465   idx in reflecte
-00005940: 642e 696e 6465 7865 735d 290a 2020 2020  d.indexes]).    
-00005950: 2020 2020 7571 5f6e 616d 6573 203d 2073      uq_names = s
-00005960: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
-00005970: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-00005980: 2020 7571 2e6e 616d 650a 2020 2020 2020    uq.name.      
-00005990: 2020 2020 2020 2020 2020 666f 7220 7571            for uq
-000059a0: 2069 6e20 7265 666c 6563 7465 642e 636f   in reflected.co
-000059b0: 6e73 7472 6169 6e74 730a 2020 2020 2020  nstraints.      
-000059c0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-000059d0: 6e73 7461 6e63 6528 7571 2c20 7371 6c61  nstance(uq, sqla
-000059e0: 6c63 6865 6d79 2e55 6e69 7175 6543 6f6e  lchemy.UniqueCon
-000059f0: 7374 7261 696e 7429 0a20 2020 2020 2020  straint).       
-00005a00: 2020 2020 205d 0a20 2020 2020 2020 2029       ].        )
-00005a10: 2e64 6966 6665 7265 6e63 6528 5b22 756e  .difference(["un
-00005a20: 6971 7565 5f63 5f61 5f62 225d 290a 0a20  ique_c_a_b"]).. 
-00005a30: 2020 2020 2020 2061 7373 6572 7420 6e6f         assert no
-00005a40: 7420 6964 785f 6e61 6d65 732e 696e 7465  t idx_names.inte
-00005a50: 7273 6563 7469 6f6e 2875 715f 6e61 6d65  rsection(uq_name
-00005a60: 7329 0a20 2020 2020 2020 2069 6620 6e61  s).        if na
-00005a70: 6d65 735f 7468 6174 5f64 7570 6c69 6361  mes_that_duplica
-00005a80: 7465 5f69 6e64 6578 3a0a 2020 2020 2020  te_index:.      
-00005a90: 2020 2020 2020 6571 5f28 6e61 6d65 735f        eq_(names_
-00005aa0: 7468 6174 5f64 7570 6c69 6361 7465 5f69  that_duplicate_i
-00005ab0: 6e64 6578 2c20 6964 785f 6e61 6d65 7329  ndex, idx_names)
-00005ac0: 0a20 2020 2020 2020 2020 2020 2065 715f  .            eq_
-00005ad0: 2875 715f 6e61 6d65 732c 2073 6574 2829  (uq_names, set()
-00005ae0: 290a 0a20 2020 2040 7465 7374 696e 672e  )..    @testing.
-00005af0: 7072 6f76 6964 655f 6d65 7461 6461 7461  provide_metadata
-00005b00: 0a20 2020 2064 6566 2074 6573 745f 756e  .    def test_un
-00005b10: 6971 7565 5f63 6f6e 7374 7261 696e 745f  ique_constraint_
-00005b20: 7261 6973 6573 2873 656c 6629 3a0a 2020  raises(self):.  
-00005b30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00005b40: 2020 4368 6563 6b69 6e67 2074 6861 7420    Checking that 
-00005b50: 756e 6971 7565 2063 6f6e 7374 7261 696e  unique constrain
-00005b60: 7420 6372 6561 7469 6f6e 0a20 2020 2020  t creation.     
-00005b70: 2020 2066 6169 6c73 2064 7565 2074 6f20     fails due to 
-00005b80: 6120 5072 6f67 7261 6d6d 696e 6745 7272  a ProgrammingErr
-00005b90: 6f72 2e0a 2020 2020 2020 2020 2222 220a  or..        """.
-00005ba0: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
-00005bb0: 203d 204d 6574 6144 6174 6128 7365 6c66   = MetaData(self
-00005bc0: 2e62 696e 6429 0a20 2020 2020 2020 2054  .bind).        T
-00005bd0: 6162 6c65 280a 2020 2020 2020 2020 2020  able(.          
-00005be0: 2020 2275 7365 725f 746d 705f 6661 696c    "user_tmp_fail
-00005bf0: 7572 6522 2c0a 2020 2020 2020 2020 2020  ure",.          
-00005c00: 2020 6d65 7461 6461 7461 2c0a 2020 2020    metadata,.    
-00005c10: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
-00005c20: 6964 222c 2073 716c 616c 6368 656d 792e  id", sqlalchemy.
-00005c30: 494e 542c 2070 7269 6d61 7279 5f6b 6579  INT, primary_key
-00005c40: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
-00005c50: 2020 2020 436f 6c75 6d6e 2822 6e61 6d65      Column("name
-00005c60: 222c 2073 716c 616c 6368 656d 792e 5641  ", sqlalchemy.VA
-00005c70: 5243 4841 5228 3530 2929 2c0a 2020 2020  RCHAR(50)),.    
-00005c80: 2020 2020 2020 2020 7371 6c61 6c63 6865          sqlalche
-00005c90: 6d79 2e55 6e69 7175 6543 6f6e 7374 7261  my.UniqueConstra
-00005ca0: 696e 7428 226e 616d 6522 2c20 6e61 6d65  int("name", name
-00005cb0: 3d22 7573 6572 5f74 6d70 5f75 7122 292c  ="user_tmp_uq"),
-00005cc0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00005cd0: 2020 2020 7769 7468 2070 7974 6573 742e      with pytest.
-00005ce0: 7261 6973 6573 2873 7061 6e6e 6572 5f64  raises(spanner_d
-00005cf0: 6261 7069 2e65 7863 6570 7469 6f6e 732e  bapi.exceptions.
-00005d00: 5072 6f67 7261 6d6d 696e 6745 7272 6f72  ProgrammingError
-00005d10: 293a 0a20 2020 2020 2020 2020 2020 206d  ):.            m
-00005d20: 6574 6164 6174 612e 6372 6561 7465 5f61  etadata.create_a
-00005d30: 6c6c 2829 0a0a 2020 2020 4074 6573 7469  ll()..    @testi
-00005d40: 6e67 2e70 726f 7669 6465 5f6d 6574 6164  ng.provide_metad
-00005d50: 6174 610a 2020 2020 6465 6620 5f74 6573  ata.    def _tes
-00005d60: 745f 6765 745f 7461 626c 655f 6e61 6d65  t_get_table_name
-00005d70: 7328 7365 6c66 2c20 7363 6865 6d61 3d4e  s(self, schema=N
-00005d80: 6f6e 652c 2074 6162 6c65 5f74 7970 653d  one, table_type=
-00005d90: 2274 6162 6c65 222c 206f 7264 6572 5f62  "table", order_b
-00005da0: 793d 4e6f 6e65 293a 0a20 2020 2020 2020  y=None):.       
-00005db0: 2022 2222 0a20 2020 2020 2020 2053 5041   """.        SPA
-00005dc0: 4e4e 4552 204f 5645 5252 4944 453a 0a0a  NNER OVERRIDE:..
-00005dd0: 2020 2020 2020 2020 5370 616e 6e65 7220          Spanner 
-00005de0: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
-00005df0: 7465 6d70 6f72 6172 7920 7461 626c 6573  temporary tables
-00005e00: 2c20 736f 2072 6561 6c20 7461 626c 6573  , so real tables
-00005e10: 2061 7265 0a20 2020 2020 2020 2075 7365   are.        use
-00005e20: 6420 666f 7220 7465 7374 696e 672e 2041  d for testing. A
-00005e30: 7320 7468 6520 6f72 6967 696e 616c 2074  s the original t
-00005e40: 6573 7420 6578 7065 6374 7320 6f6e 6c79  est expects only
-00005e50: 2072 6561 6c0a 2020 2020 2020 2020 7461   real.        ta
-00005e60: 626c 6573 2074 6f20 6265 2072 6561 642c  bles to be read,
-00005e70: 2061 6e64 2069 6e20 5370 616e 6e65 7220   and in Spanner 
-00005e80: 616c 6c20 7468 6520 7461 626c 6573 2061  all the tables a
-00005e90: 7265 2072 6561 6c2c 0a20 2020 2020 2020  re real,.       
-00005ea0: 2065 7870 6563 7465 6420 7265 7375 6c74   expected result
-00005eb0: 7320 6f76 6572 7269 6465 2069 7320 7265  s override is re
-00005ec0: 7175 6972 6564 2e0a 2020 2020 2020 2020  quired..        
-00005ed0: 2222 220a 2020 2020 2020 2020 5f69 676e  """.        _ign
-00005ee0: 6f72 655f 7461 626c 6573 203d 205b 0a20  ore_tables = [. 
-00005ef0: 2020 2020 2020 2020 2020 2022 636f 6d6d             "comm
-00005f00: 656e 745f 7465 7374 222c 0a20 2020 2020  ent_test",.     
-00005f10: 2020 2020 2020 2022 6e6f 6e63 6f6c 5f69         "noncol_i
-00005f20: 6478 5f74 6573 745f 706b 222c 0a20 2020  dx_test_pk",.   
-00005f30: 2020 2020 2020 2020 2022 6e6f 6e63 6f6c           "noncol
-00005f40: 5f69 6478 5f74 6573 745f 6e6f 706b 222c  _idx_test_nopk",
-00005f50: 0a20 2020 2020 2020 2020 2020 2022 6c6f  .            "lo
-00005f60: 6361 6c5f 7461 626c 6522 2c0a 2020 2020  cal_table",.    
-00005f70: 2020 2020 2020 2020 2272 656d 6f74 655f          "remote_
-00005f80: 7461 626c 6522 2c0a 2020 2020 2020 2020  table",.        
-00005f90: 2020 2020 2272 656d 6f74 655f 7461 626c      "remote_tabl
-00005fa0: 655f 3222 2c0a 2020 2020 2020 2020 5d0a  e_2",.        ].
-00005fb0: 2020 2020 2020 2020 6d65 7461 203d 2073          meta = s
-00005fc0: 656c 662e 6d65 7461 6461 7461 0a0a 2020  elf.metadata..  
-00005fd0: 2020 2020 2020 696e 7370 203d 2069 6e73        insp = ins
-00005fe0: 7065 6374 286d 6574 612e 6269 6e64 290a  pect(meta.bind).
-00005ff0: 0a20 2020 2020 2020 2069 6620 7461 626c  .        if tabl
-00006000: 655f 7479 7065 203d 3d20 2276 6965 7722  e_type == "view"
-00006010: 3a0a 2020 2020 2020 2020 2020 2020 7461  :.            ta
-00006020: 626c 655f 6e61 6d65 7320 3d20 696e 7370  ble_names = insp
-00006030: 2e67 6574 5f76 6965 775f 6e61 6d65 7328  .get_view_names(
-00006040: 7363 6865 6d61 290a 2020 2020 2020 2020  schema).        
-00006050: 2020 2020 7461 626c 655f 6e61 6d65 732e      table_names.
-00006060: 736f 7274 2829 0a20 2020 2020 2020 2020  sort().         
-00006070: 2020 2061 6e73 7765 7220 3d20 5b22 656d     answer = ["em
-00006080: 6169 6c5f 6164 6472 6573 7365 735f 7622  ail_addresses_v"
-00006090: 2c20 2275 7365 7273 5f76 225d 0a20 2020  , "users_v"].   
-000060a0: 2020 2020 2020 2020 2065 715f 2873 6f72           eq_(sor
-000060b0: 7465 6428 7461 626c 655f 6e61 6d65 7329  ted(table_names)
-000060c0: 2c20 616e 7377 6572 290a 2020 2020 2020  , answer).      
-000060d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000060e0: 2020 2020 6966 206f 7264 6572 5f62 793a      if order_by:
-000060f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006100: 2074 6162 6c65 7320 3d20 5b0a 2020 2020   tables = [.    
-00006110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006120: 7265 635b 305d 0a20 2020 2020 2020 2020  rec[0].         
-00006130: 2020 2020 2020 2020 2020 2066 6f72 2072             for r
-00006140: 6563 2069 6e20 696e 7370 2e67 6574 5f73  ec in insp.get_s
-00006150: 6f72 7465 645f 7461 626c 655f 616e 645f  orted_table_and_
-00006160: 666b 635f 6e61 6d65 7328 7363 6865 6d61  fkc_names(schema
-00006170: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00006180: 2020 2020 2020 6966 2072 6563 5b30 5d0a        if rec[0].
-00006190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061a0: 5d0a 2020 2020 2020 2020 2020 2020 656c  ].            el
-000061b0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000061c0: 2020 2020 7461 626c 6573 203d 2069 6e73      tables = ins
-000061d0: 702e 6765 745f 7461 626c 655f 6e61 6d65  p.get_table_name
-000061e0: 7328 7363 6865 6d61 290a 2020 2020 2020  s(schema).      
-000061f0: 2020 2020 2020 7461 626c 655f 6e61 6d65        table_name
-00006200: 7320 3d20 5b74 2066 6f72 2074 2069 6e20  s = [t for t in 
-00006210: 7461 626c 6573 2069 6620 7420 6e6f 7420  tables if t not 
-00006220: 696e 205f 6967 6e6f 7265 5f74 6162 6c65  in _ignore_table
-00006230: 735d 0a0a 2020 2020 2020 2020 2020 2020  s]..            
-00006240: 6966 206f 7264 6572 5f62 7920 3d3d 2022  if order_by == "
-00006250: 666f 7265 6967 6e5f 6b65 7922 3a0a 2020  foreign_key":.  
-00006260: 2020 2020 2020 2020 2020 2020 2020 616e                an
-00006270: 7377 6572 203d 207b 2264 696e 6761 6c69  swer = {"dingali
-00006280: 6e67 7322 2c20 2265 6d61 696c 5f61 6464  ngs", "email_add
-00006290: 7265 7373 6573 222c 2022 7573 6572 5f74  resses", "user_t
-000062a0: 6d70 222c 2022 7573 6572 7322 7d0a 2020  mp", "users"}.  
-000062b0: 2020 2020 2020 2020 2020 2020 2020 6571                eq
-000062c0: 5f28 7365 7428 7461 626c 655f 6e61 6d65  _(set(table_name
-000062d0: 7329 2c20 616e 7377 6572 290a 2020 2020  s), answer).    
-000062e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000062f0: 2020 2020 2020 2020 2020 2020 2020 616e                an
-00006300: 7377 6572 203d 205b 2264 696e 6761 6c69  swer = ["dingali
-00006310: 6e67 7322 2c20 2265 6d61 696c 5f61 6464  ngs", "email_add
-00006320: 7265 7373 6573 222c 2022 7573 6572 5f74  resses", "user_t
-00006330: 6d70 222c 2022 7573 6572 7322 5d0a 2020  mp", "users"].  
-00006340: 2020 2020 2020 2020 2020 2020 2020 6571                eq
-00006350: 5f28 736f 7274 6564 2874 6162 6c65 5f6e  _(sorted(table_n
-00006360: 616d 6573 292c 2061 6e73 7765 7229 0a0a  ames), answer)..
-00006370: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-00006380: 2e73 6b69 7028 2253 7061 6e6e 6572 2064  .skip("Spanner d
-00006390: 6f65 736e 2774 2073 7570 706f 7274 2074  oesn't support t
-000063a0: 656d 706f 7261 7279 2074 6162 6c65 7322  emporary tables"
-000063b0: 290a 2020 2020 6465 6620 7465 7374 5f67  ).    def test_g
-000063c0: 6574 5f74 656d 705f 7461 626c 655f 696e  et_temp_table_in
-000063d0: 6465 7865 7328 7365 6c66 293a 0a20 2020  dexes(self):.   
-000063e0: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
-000063f0: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
-00006400: 2822 5370 616e 6e65 7220 646f 6573 6e27  ("Spanner doesn'
-00006410: 7420 7375 7070 6f72 7420 7465 6d70 6f72  t support tempor
-00006420: 6172 7920 7461 626c 6573 2229 0a20 2020  ary tables").   
-00006430: 2064 6566 2074 6573 745f 6765 745f 7465   def test_get_te
-00006440: 6d70 5f74 6162 6c65 5f75 6e69 7175 655f  mp_table_unique_
-00006450: 636f 6e73 7472 6169 6e74 7328 7365 6c66  constraints(self
-00006460: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-00006470: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
-00006480: 6b2e 736b 6970 2822 5370 616e 6e65 7220  k.skip("Spanner 
-00006490: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
-000064a0: 7465 6d70 6f72 6172 7920 7461 626c 6573  temporary tables
-000064b0: 2229 0a20 2020 2064 6566 2074 6573 745f  ").    def test_
-000064c0: 6765 745f 7465 6d70 5f74 6162 6c65 5f63  get_temp_table_c
-000064d0: 6f6c 756d 6e73 2873 656c 6629 3a0a 2020  olumns(self):.  
-000064e0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-000064f0: 6465 6620 5f61 7373 6572 745f 696e 7370  def _assert_insp
-00006500: 5f69 6e64 6578 6573 2873 656c 662c 2069  _indexes(self, i
-00006510: 6e64 6578 6573 2c20 6578 7065 6374 6564  ndexes, expected
-00006520: 5f69 6e64 6578 6573 293a 0a20 2020 2020  _indexes):.     
-00006530: 2020 2065 7870 6563 7465 645f 696e 6465     expected_inde
-00006540: 7865 732e 736f 7274 286b 6579 3d6c 616d  xes.sort(key=lam
-00006550: 6264 6120 6974 656d 3a20 6974 656d 5b22  bda item: item["
-00006560: 6e61 6d65 225d 290a 0a20 2020 2020 2020  name"])..       
-00006570: 2069 6e64 6578 5f6e 616d 6573 203d 205b   index_names = [
-00006580: 645b 226e 616d 6522 5d20 666f 7220 6420  d["name"] for d 
-00006590: 696e 2069 6e64 6578 6573 5d0a 2020 2020  in indexes].    
-000065a0: 2020 2020 6578 705f 696e 6465 785f 6e61      exp_index_na
-000065b0: 6d65 7320 3d20 5b64 5b22 6e61 6d65 225d  mes = [d["name"]
-000065c0: 2066 6f72 2064 2069 6e20 6578 7065 6374   for d in expect
-000065d0: 6564 5f69 6e64 6578 6573 5d0a 2020 2020  ed_indexes].    
-000065e0: 2020 2020 6173 7365 7274 2073 6f72 7465      assert sorte
-000065f0: 6428 696e 6465 785f 6e61 6d65 7329 203d  d(index_names) =
-00006600: 3d20 736f 7274 6564 2865 7870 5f69 6e64  = sorted(exp_ind
-00006610: 6578 5f6e 616d 6573 290a 0a0a 636c 6173  ex_names)...clas
-00006620: 7320 436f 6d70 6f73 6974 654b 6579 5265  s CompositeKeyRe
-00006630: 666c 6563 7469 6f6e 5465 7374 285f 436f  flectionTest(_Co
-00006640: 6d70 6f73 6974 654b 6579 5265 666c 6563  mpositeKeyReflec
-00006650: 7469 6f6e 5465 7374 293a 0a20 2020 2040  tionTest):.    @
-00006660: 7465 7374 696e 672e 7265 7175 6972 6573  testing.requires
-00006670: 2e66 6f72 6569 676e 5f6b 6579 5f63 6f6e  .foreign_key_con
-00006680: 7374 7261 696e 745f 7265 666c 6563 7469  straint_reflecti
-00006690: 6f6e 0a20 2020 2064 6566 2074 6573 745f  on.    def test_
-000066a0: 666b 5f63 6f6c 756d 6e5f 6f72 6465 7228  fk_column_order(
-000066b0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-000066c0: 2222 0a20 2020 2020 2020 2053 5041 4e4e  "".        SPANN
-000066d0: 4552 204f 5645 5252 4944 453a 0a0a 2020  ER OVERRIDE:..  
-000066e0: 2020 2020 2020 5370 616e 6e65 7220 636f        Spanner co
-000066f0: 6c75 6d6e 2075 7361 6765 2072 6566 6c65  lumn usage refle
-00006700: 6374 696f 6e20 646f 6573 6e27 7420 7375  ction doesn't su
-00006710: 7070 6f72 7420 6465 7465 726d 656e 6973  pport determenis
-00006720: 7469 630a 2020 2020 2020 2020 6f72 6465  tic.        orde
-00006730: 7269 6e67 2e20 4f76 6572 7269 6469 6e67  ring. Overriding
-00006740: 2074 6865 2074 6573 7420 746f 2063 6865   the test to che
-00006750: 636b 2074 6861 7420 636f 6c75 6d6e 7320  ck that columns 
-00006760: 6172 650a 2020 2020 2020 2020 7265 666c  are.        refl
-00006770: 6563 7465 6420 636f 7272 6563 746c 792c  ected correctly,
-00006780: 2077 6974 686f 7574 2063 6f6e 7369 6465   without conside
-00006790: 7269 6e67 2074 6865 6972 206f 7264 6572  ring their order
-000067a0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-000067b0: 2020 2020 2020 2320 7465 7374 2066 6f72        # test for
-000067c0: 2069 7373 7565 2023 3536 3631 0a20 2020   issue #5661.   
-000067d0: 2020 2020 2069 6e73 7020 3d20 696e 7370       insp = insp
-000067e0: 6563 7428 7365 6c66 2e62 696e 6429 0a20  ect(self.bind). 
-000067f0: 2020 2020 2020 2066 6f72 6569 676e 5f6b         foreign_k
-00006800: 6579 7320 3d20 696e 7370 2e67 6574 5f66  eys = insp.get_f
-00006810: 6f72 6569 676e 5f6b 6579 7328 7365 6c66  oreign_keys(self
-00006820: 2e74 6162 6c65 732e 7462 322e 6e61 6d65  .tables.tb2.name
-00006830: 290a 2020 2020 2020 2020 6571 5f28 6c65  ).        eq_(le
-00006840: 6e28 666f 7265 6967 6e5f 6b65 7973 292c  n(foreign_keys),
-00006850: 2031 290a 2020 2020 2020 2020 666b 6579   1).        fkey
-00006860: 3120 3d20 666f 7265 6967 6e5f 6b65 7973  1 = foreign_keys
-00006870: 5b30 5d0a 2020 2020 2020 2020 6571 5f28  [0].        eq_(
-00006880: 7365 7428 666b 6579 312e 6765 7428 2272  set(fkey1.get("r
-00006890: 6566 6572 7265 645f 636f 6c75 6d6e 7322  eferred_columns"
-000068a0: 2929 2c20 7b22 6e61 6d65 222c 2022 6964  )), {"name", "id
-000068b0: 222c 2022 6174 7472 227d 290a 2020 2020  ", "attr"}).    
-000068c0: 2020 2020 6571 5f28 7365 7428 666b 6579      eq_(set(fkey
-000068d0: 312e 6765 7428 2263 6f6e 7374 7261 696e  1.get("constrain
-000068e0: 6564 5f63 6f6c 756d 6e73 2229 292c 207b  ed_columns")), {
-000068f0: 2270 6e61 6d65 222c 2022 7069 6422 2c20  "pname", "pid", 
-00006900: 2270 6174 7472 227d 290a 0a0a 4070 7974  "pattr"})...@pyt
-00006910: 6573 742e 6d61 726b 2e73 6b69 7028 2253  est.mark.skip("S
-00006920: 7061 6e6e 6572 2064 6f65 736e 2774 2073  panner doesn't s
-00006930: 7570 706f 7274 2071 756f 7465 7320 696e  upport quotes in
-00006940: 2074 6162 6c65 206e 616d 6573 2e22 290a   table names.").
-00006950: 636c 6173 7320 5175 6f74 6564 4e61 6d65  class QuotedName
-00006960: 4172 6775 6d65 6e74 5465 7374 285f 5175  ArgumentTest(_Qu
-00006970: 6f74 6564 4e61 6d65 4172 6775 6d65 6e74  otedNameArgument
-00006980: 5465 7374 293a 0a20 2020 2070 6173 730a  Test):.    pass.
-00006990: 0a0a 636c 6173 7320 5f44 6174 6546 6978  ..class _DateFix
-000069a0: 7475 7265 285f 5f44 6174 6546 6978 7475  ture(__DateFixtu
-000069b0: 7265 293a 0a20 2020 2063 6f6d 7061 7265  re):.    compare
-000069c0: 203d 204e 6f6e 650a 0a20 2020 2040 636c   = None..    @cl
-000069d0: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-000069e0: 6620 6465 6669 6e65 5f74 6162 6c65 7328  f define_tables(
-000069f0: 636c 732c 206d 6574 6164 6174 6129 3a0a  cls, metadata):.
-00006a00: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00006a10: 2020 2020 5350 414e 4e45 5220 4f56 4552      SPANNER OVER
-00006a20: 5249 4445 3a0a 0a20 2020 2020 2020 2043  RIDE:..        C
-00006a30: 6c6f 7564 2053 7061 6e6e 6572 2064 6f65  loud Spanner doe
-00006a40: 736e 2774 2073 7570 706f 7274 2061 7574  sn't support aut
-00006a50: 6f20 696e 6372 656d 656e 7469 6e67 2069  o incrementing i
-00006a60: 6473 2066 6561 7475 7265 2c0a 2020 2020  ds feature,.    
-00006a70: 2020 2020 7768 6963 6820 6973 2075 7365      which is use
-00006a80: 6420 6279 2074 6865 206f 7269 6769 6e61  d by the origina
-00006a90: 6c20 7465 7374 2e20 4f76 6572 7269 6469  l test. Overridi
-00006aa0: 6e67 2074 6865 2074 6573 7420 6461 7461  ng the test data
-00006ab0: 0a20 2020 2020 2020 2063 7265 6174 696f  .        creatio
-00006ac0: 6e20 6d65 7468 6f64 2074 6f20 6469 7361  n method to disa
-00006ad0: 626c 6520 6175 746f 696e 6372 656d 656e  ble autoincremen
-00006ae0: 7420 616e 6420 6d61 6b65 2069 6420 636f  t and make id co
-00006af0: 6c75 6d6e 0a20 2020 2020 2020 206e 756c  lumn.        nul
-00006b00: 6c61 626c 652e 0a20 2020 2020 2020 2022  lable..        "
-00006b10: 2222 0a0a 2020 2020 2020 2020 636c 6173  ""..        clas
-00006b20: 7320 4465 636f 7261 7465 6428 7371 6c61  s Decorated(sqla
-00006b30: 6c63 6865 6d79 2e54 7970 6544 6563 6f72  lchemy.TypeDecor
-00006b40: 6174 6f72 293a 0a20 2020 2020 2020 2020  ator):.         
-00006b50: 2020 2069 6d70 6c20 3d20 636c 732e 6461     impl = cls.da
-00006b60: 7461 7479 7065 0a20 2020 2020 2020 2020  tatype.         
-00006b70: 2020 2063 6163 6865 5f6f 6b20 3d20 5472     cache_ok = Tr
-00006b80: 7565 0a0a 2020 2020 2020 2020 5461 626c  ue..        Tabl
-00006b90: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
-00006ba0: 6461 7465 5f74 6162 6c65 222c 0a20 2020  date_table",.   
-00006bb0: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
-00006bc0: 612c 0a20 2020 2020 2020 2020 2020 2043  a,.            C
-00006bd0: 6f6c 756d 6e28 2269 6422 2c20 496e 7465  olumn("id", Inte
-00006be0: 6765 722c 2070 7269 6d61 7279 5f6b 6579  ger, primary_key
-00006bf0: 3d54 7275 652c 206e 756c 6c61 626c 653d  =True, nullable=
-00006c00: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
-00006c10: 2020 2043 6f6c 756d 6e28 2264 6174 655f     Column("date_
-00006c20: 6461 7461 222c 2063 6c73 2e64 6174 6174  data", cls.datat
-00006c30: 7970 6529 2c0a 2020 2020 2020 2020 2020  ype),.          
-00006c40: 2020 436f 6c75 6d6e 2822 6465 636f 7261    Column("decora
-00006c50: 7465 645f 6461 7465 5f64 6174 6122 2c20  ted_date_data", 
-00006c60: 4465 636f 7261 7465 6429 2c0a 2020 2020  Decorated),.    
-00006c70: 2020 2020 290a 0a0a 636c 6173 7320 4461      )...class Da
-00006c80: 7465 5465 7374 285f 4461 7465 5465 7374  teTest(_DateTest
-00006c90: 293a 0a20 2020 2022 2222 0a20 2020 2053  ):.    """.    S
-00006ca0: 5041 4e4e 4552 204f 5645 5252 4944 453a  PANNER OVERRIDE:
-00006cb0: 0a0a 2020 2020 4461 7465 5465 7374 2074  ..    DateTest t
-00006cc0: 6573 7473 2075 7365 6420 7361 6d65 2063  ests used same c
-00006cd0: 6c61 7373 206d 6574 686f 6420 746f 2063  lass method to c
-00006ce0: 7265 6174 6520 7461 626c 652c 2073 6f20  reate table, so 
-00006cf0: 746f 2061 766f 6964 2074 686f 7365 2066  to avoid those f
-00006d00: 6169 6c75 7265 730a 2020 2020 616e 6420  ailures.    and 
-00006d10: 6d61 696e 7461 696e 2044 5259 2063 6f6e  maintain DRY con
-00006d20: 6365 7074 206a 7573 7420 696e 6865 7269  cept just inheri
-00006d30: 7420 7468 6520 636c 6173 7320 746f 2072  t the class to r
-00006d40: 756e 2074 6573 7473 2073 7563 6365 7373  un tests success
-00006d50: 6675 6c6c 792e 0a20 2020 2022 2222 0a0a  fully..    """..
-00006d60: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-00006d70: 2e73 6b69 7069 6628 0a20 2020 2020 2020  .skipif(.       
-00006d80: 2062 6f6f 6c28 6f73 2e65 6e76 6972 6f6e   bool(os.environ
-00006d90: 2e67 6574 2822 5350 414e 4e45 525f 454d  .get("SPANNER_EM
-00006da0: 554c 4154 4f52 5f48 4f53 5422 2929 2c20  ULATOR_HOST")), 
-00006db0: 7265 6173 6f6e 3d22 536b 6970 7065 6420  reason="Skipped 
-00006dc0: 6f6e 2065 6d75 6c61 746f 7222 0a20 2020  on emulator".   
-00006dd0: 2029 0a20 2020 2064 6566 2074 6573 745f   ).    def test_
-00006de0: 6e75 6c6c 5f62 6f75 6e64 5f63 6f6d 7061  null_bound_compa
-00006df0: 7269 736f 6e28 7365 6c66 293a 0a20 2020  rison(self):.   
-00006e00: 2020 2020 2073 7570 6572 2829 2e74 6573       super().tes
-00006e10: 745f 6e75 6c6c 5f62 6f75 6e64 5f63 6f6d  t_null_bound_com
-00006e20: 7061 7269 736f 6e28 290a 0a20 2020 2040  parison()..    @
-00006e30: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
-00006e40: 6966 280a 2020 2020 2020 2020 626f 6f6c  if(.        bool
-00006e50: 286f 732e 656e 7669 726f 6e2e 6765 7428  (os.environ.get(
-00006e60: 2253 5041 4e4e 4552 5f45 4d55 4c41 544f  "SPANNER_EMULATO
-00006e70: 525f 484f 5354 2229 292c 2072 6561 736f  R_HOST")), reaso
-00006e80: 6e3d 2253 6b69 7070 6564 206f 6e20 656d  n="Skipped on em
-00006e90: 756c 6174 6f72 220a 2020 2020 290a 2020  ulator".    ).  
-00006ea0: 2020 6465 6620 7465 7374 5f6e 756c 6c28    def test_null(
-00006eb0: 7365 6c66 2c20 636f 6e6e 6563 7469 6f6e  self, connection
-00006ec0: 293a 0a20 2020 2020 2020 2073 7570 6572  ):.        super
-00006ed0: 2829 2e74 6573 745f 6e75 6c6c 2863 6f6e  ().test_null(con
-00006ee0: 6e65 6374 696f 6e29 0a0a 0a63 6c61 7373  nection)...class
-00006ef0: 2043 5445 5465 7374 285f 4354 4554 6573   CTETest(_CTETes
-00006f00: 7429 3a0a 2020 2020 4063 6c61 7373 6d65  t):.    @classme
-00006f10: 7468 6f64 0a20 2020 2064 6566 2064 6566  thod.    def def
-00006f20: 696e 655f 7461 626c 6573 2863 6c73 2c20  ine_tables(cls, 
-00006f30: 6d65 7461 6461 7461 293a 0a20 2020 2020  metadata):.     
-00006f40: 2020 2022 2222 0a20 2020 2020 2020 2054     """.        T
-00006f50: 6865 206f 7269 6769 6e61 6c20 6d65 7468  he original meth
-00006f60: 6f64 2063 7265 6174 6573 2061 2066 6f72  od creates a for
-00006f70: 6569 676e 206b 6579 2077 6974 686f 7574  eign key without
-00006f80: 2061 206e 616d 652c 0a20 2020 2020 2020   a name,.       
-00006f90: 2077 6869 6368 2063 6175 7365 7320 7472   which causes tr
-00006fa0: 6f75 626c 6573 206f 6e20 7465 7374 2063  oubles on test c
-00006fb0: 6c65 616e 7570 2e20 4f76 6572 7269 6469  leanup. Overridi
-00006fc0: 6e67 2074 6865 0a20 2020 2020 2020 206d  ng the.        m
-00006fd0: 6574 686f 6420 746f 2065 7870 6c69 6369  ethod to explici
-00006fe0: 746c 7920 7365 7420 6120 666f 7265 6967  tly set a foreig
-00006ff0: 6e20 6b65 7920 6e61 6d65 2e0a 2020 2020  n key name..    
-00007000: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00007010: 5461 626c 6528 0a20 2020 2020 2020 2020  Table(.         
-00007020: 2020 2022 736f 6d65 5f74 6162 6c65 222c     "some_table",
-00007030: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
-00007040: 6164 6174 612c 0a20 2020 2020 2020 2020  adata,.         
-00007050: 2020 2043 6f6c 756d 6e28 2269 6422 2c20     Column("id", 
-00007060: 496e 7465 6765 722c 2070 7269 6d61 7279  Integer, primary
-00007070: 5f6b 6579 3d54 7275 6529 2c0a 2020 2020  _key=True),.    
-00007080: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
-00007090: 6461 7461 222c 2053 7472 696e 6728 3530  data", String(50
-000070a0: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-000070b0: 436f 6c75 6d6e 2822 7061 7265 6e74 5f69  Column("parent_i
-000070c0: 6422 2c20 466f 7265 6967 6e4b 6579 2822  d", ForeignKey("
-000070d0: 736f 6d65 5f74 6162 6c65 2e69 6422 2c20  some_table.id", 
-000070e0: 6e61 6d65 3d22 666b 5f73 6f6d 655f 7461  name="fk_some_ta
-000070f0: 626c 6522 2929 2c0a 2020 2020 2020 2020  ble")),.        
-00007100: 290a 0a20 2020 2020 2020 2054 6162 6c65  )..        Table
-00007110: 280a 2020 2020 2020 2020 2020 2020 2273  (.            "s
-00007120: 6f6d 655f 6f74 6865 725f 7461 626c 6522  ome_other_table"
-00007130: 2c0a 2020 2020 2020 2020 2020 2020 6d65  ,.            me
-00007140: 7461 6461 7461 2c0a 2020 2020 2020 2020  tadata,.        
-00007150: 2020 2020 436f 6c75 6d6e 2822 6964 222c      Column("id",
-00007160: 2049 6e74 6567 6572 2c20 7072 696d 6172   Integer, primar
-00007170: 795f 6b65 793d 5472 7565 292c 0a20 2020  y_key=True),.   
-00007180: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-00007190: 2264 6174 6122 2c20 5374 7269 6e67 2835  "data", String(5
-000071a0: 3029 292c 0a20 2020 2020 2020 2020 2020  0)),.           
-000071b0: 2043 6f6c 756d 6e28 2270 6172 656e 745f   Column("parent_
-000071c0: 6964 222c 2049 6e74 6567 6572 292c 0a20  id", Integer),. 
-000071d0: 2020 2020 2020 2029 0a0a 2020 2020 4070         )..    @p
-000071e0: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
-000071f0: 2249 4e53 4552 5420 6672 6f6d 2057 4954  "INSERT from WIT
-00007200: 4820 7375 6271 7565 7279 2069 7320 6e6f  H subquery is no
-00007210: 7420 7375 7070 6f72 7465 6422 290a 2020  t supported").  
-00007220: 2020 6465 6620 7465 7374 5f69 6e73 6572    def test_inser
-00007230: 745f 6672 6f6d 5f73 656c 6563 745f 726f  t_from_select_ro
-00007240: 756e 645f 7472 6970 2873 656c 6629 3a0a  und_trip(self):.
-00007250: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00007260: 2020 2020 5468 6520 7465 7374 2063 6865      The test che
-00007270: 636b 7320 6966 2061 6e20 494e 5345 5254  cks if an INSERT
-00007280: 2063 616e 2062 6520 646f 6e65 2066 726f   can be done fro
-00007290: 6d20 6120 6374 652c 206c 696b 653a 0a0a  m a cte, like:..
-000072a0: 2020 2020 2020 2020 5749 5448 2073 6f6d          WITH som
-000072b0: 655f 6374 6520 4153 2028 2e2e 2e29 0a20  e_cte AS (...). 
-000072c0: 2020 2020 2020 2049 4e53 4552 5420 494e         INSERT IN
-000072d0: 544f 2073 6f6d 655f 6f74 6865 725f 7461  TO some_other_ta
-000072e0: 626c 6520 282e 2e2e 2053 454c 4543 5420  ble (... SELECT 
-000072f0: 2a20 4652 4f4d 2073 6f6d 655f 6374 6529  * FROM some_cte)
-00007300: 0a0a 2020 2020 2020 2020 5375 6368 2071  ..        Such q
-00007310: 7565 7269 6573 2061 7265 206e 6f74 2073  ueries are not s
-00007320: 7570 706f 7274 6564 2062 7920 5370 616e  upported by Span
-00007330: 6e65 722e 0a20 2020 2020 2020 2022 2222  ner..        """
-00007340: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00007350: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-00007360: 736b 6970 2822 4445 4c45 5445 2066 726f  skip("DELETE fro
-00007370: 6d20 5749 5448 2073 7562 7175 6572 7920  m WITH subquery 
-00007380: 6973 206e 6f74 2073 7570 706f 7274 6564  is not supported
-00007390: 2229 0a20 2020 2064 6566 2074 6573 745f  ").    def test_
-000073a0: 6465 6c65 7465 5f73 6361 6c61 725f 7375  delete_scalar_su
-000073b0: 6271 5f72 6f75 6e64 5f74 7269 7028 7365  bq_round_trip(se
-000073c0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-000073d0: 0a20 2020 2020 2020 2054 6865 2074 6573  .        The tes
-000073e0: 7420 6368 6563 6b73 2069 6620 6120 4445  t checks if a DE
-000073f0: 4c45 5445 2063 616e 2062 6520 646f 6e65  LETE can be done
-00007400: 2066 726f 6d20 6120 6374 652c 206c 696b   from a cte, lik
-00007410: 653a 0a0a 2020 2020 2020 2020 5749 5448  e:..        WITH
-00007420: 2073 6f6d 655f 6374 6520 4153 2028 2e2e   some_cte AS (..
-00007430: 2e29 0a20 2020 2020 2020 2044 454c 4554  .).        DELET
-00007440: 4520 4652 4f4d 2073 6f6d 655f 6f74 6865  E FROM some_othe
-00007450: 725f 7461 626c 6520 282e 2e2e 2053 454c  r_table (... SEL
-00007460: 4543 5420 2a20 4652 4f4d 2073 6f6d 655f  ECT * FROM some_
-00007470: 6374 6529 0a0a 2020 2020 2020 2020 5375  cte)..        Su
-00007480: 6368 2071 7565 7269 6573 2061 7265 206e  ch queries are n
-00007490: 6f74 2073 7570 706f 7274 6564 2062 7920  ot supported by 
-000074a0: 5370 616e 6e65 722e 0a20 2020 2020 2020  Spanner..       
-000074b0: 2022 2222 0a20 2020 2020 2020 2070 6173   """.        pas
-000074c0: 730a 0a20 2020 2040 7079 7465 7374 2e6d  s..    @pytest.m
-000074d0: 6172 6b2e 736b 6970 2822 4445 4c45 5445  ark.skip("DELETE
-000074e0: 2066 726f 6d20 5749 5448 2073 7562 7175   from WITH subqu
-000074f0: 6572 7920 6973 206e 6f74 2073 7570 706f  ery is not suppo
-00007500: 7274 6564 2229 0a20 2020 2064 6566 2074  rted").    def t
-00007510: 6573 745f 6465 6c65 7465 5f66 726f 6d5f  est_delete_from_
-00007520: 726f 756e 645f 7472 6970 2873 656c 6629  round_trip(self)
-00007530: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00007540: 2020 2020 2020 5468 6520 7465 7374 2063        The test c
-00007550: 6865 636b 7320 6966 2061 2044 454c 4554  hecks if a DELET
-00007560: 4520 6361 6e20 6265 2064 6f6e 6520 6672  E can be done fr
-00007570: 6f6d 2061 2063 7465 2c20 6c69 6b65 3a0a  om a cte, like:.
-00007580: 0a20 2020 2020 2020 2057 4954 4820 736f  .        WITH so
-00007590: 6d65 5f63 7465 2041 5320 282e 2e2e 290a  me_cte AS (...).
-000075a0: 2020 2020 2020 2020 4445 4c45 5445 2046          DELETE F
-000075b0: 524f 4d20 736f 6d65 5f6f 7468 6572 5f74  ROM some_other_t
-000075c0: 6162 6c65 2028 2e2e 2e20 5345 4c45 4354  able (... SELECT
-000075d0: 202a 2046 524f 4d20 736f 6d65 5f63 7465   * FROM some_cte
-000075e0: 290a 0a20 2020 2020 2020 2053 7563 6820  )..        Such 
-000075f0: 7175 6572 6965 7320 6172 6520 6e6f 7420  queries are not 
-00007600: 7375 7070 6f72 7465 6420 6279 2053 7061  supported by Spa
-00007610: 6e6e 6572 2e0a 2020 2020 2020 2020 2222  nner..        ""
-00007620: 220a 2020 2020 2020 2020 7061 7373 0a0a  ".        pass..
-00007630: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-00007640: 2e73 6b69 7028 2255 5044 4154 4520 6672  .skip("UPDATE fr
-00007650: 6f6d 2057 4954 4820 7375 6271 7565 7279  om WITH subquery
-00007660: 2069 7320 6e6f 7420 7375 7070 6f72 7465   is not supporte
-00007670: 6422 290a 2020 2020 6465 6620 7465 7374  d").    def test
-00007680: 5f75 7064 6174 655f 6672 6f6d 5f72 6f75  _update_from_rou
-00007690: 6e64 5f74 7269 7028 7365 6c66 293a 0a20  nd_trip(self):. 
-000076a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000076b0: 2020 2054 6865 2074 6573 7420 6368 6563     The test chec
-000076c0: 6b73 2069 6620 616e 2055 5044 4154 4520  ks if an UPDATE 
-000076d0: 6361 6e20 6265 2064 6f6e 6520 6672 6f6d  can be done from
-000076e0: 2061 2063 7465 2c20 6c69 6b65 3a0a 0a20   a cte, like:.. 
-000076f0: 2020 2020 2020 2057 4954 4820 736f 6d65         WITH some
-00007700: 5f63 7465 2041 5320 282e 2e2e 290a 2020  _cte AS (...).  
-00007710: 2020 2020 2020 5550 4441 5445 2073 6f6d        UPDATE som
-00007720: 655f 6f74 6865 725f 7461 626c 650a 2020  e_other_table.  
-00007730: 2020 2020 2020 5345 5420 282e 2e2e 2053        SET (... S
-00007740: 454c 4543 5420 2a20 4652 4f4d 2073 6f6d  ELECT * FROM som
-00007750: 655f 6374 6529 0a0a 2020 2020 2020 2020  e_cte)..        
-00007760: 5375 6368 2071 7565 7269 6573 2061 7265  Such queries are
-00007770: 206e 6f74 2073 7570 706f 7274 6564 2062   not supported b
-00007780: 7920 5370 616e 6e65 722e 0a20 2020 2020  y Spanner..     
-00007790: 2020 2022 2222 0a20 2020 2020 2020 2070     """.        p
-000077a0: 6173 730a 0a20 2020 2040 7079 7465 7374  ass..    @pytest
-000077b0: 2e6d 6172 6b2e 736b 6970 2822 5749 5448  .mark.skip("WITH
-000077c0: 2052 4543 5552 5349 5645 2073 7562 7175   RECURSIVE subqu
-000077d0: 6572 6965 7320 6172 6520 6e6f 7420 7375  eries are not su
-000077e0: 7070 6f72 7465 6422 290a 2020 2020 6465  pported").    de
-000077f0: 6620 7465 7374 5f73 656c 6563 745f 7265  f test_select_re
-00007800: 6375 7273 6976 655f 726f 756e 645f 7472  cursive_round_tr
-00007810: 6970 2873 656c 6629 3a0a 2020 2020 2020  ip(self):.      
-00007820: 2020 7061 7373 0a0a 0a63 6c61 7373 2044    pass...class D
-00007830: 6174 6554 696d 654d 6963 726f 7365 636f  ateTimeMicroseco
-00007840: 6e64 7354 6573 7428 5f44 6174 6554 696d  ndsTest(_DateTim
-00007850: 654d 6963 726f 7365 636f 6e64 7354 6573  eMicrosecondsTes
-00007860: 742c 2044 6174 6554 6573 7429 3a0a 2020  t, DateTest):.  
-00007870: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
-00007880: 6b69 7028 2253 7061 6e6e 6572 2064 6174  kip("Spanner dat
-00007890: 6573 2061 7265 2074 696d 6520 7a6f 6e65  es are time zone
-000078a0: 2069 6e64 6570 656e 6465 6e74 2229 0a20   independent"). 
-000078b0: 2020 2064 6566 2074 6573 745f 7365 6c65     def test_sele
-000078c0: 6374 5f64 6972 6563 7428 7365 6c66 293a  ct_direct(self):
-000078d0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-000078e0: 2020 2064 6566 2074 6573 745f 726f 756e     def test_roun
-000078f0: 645f 7472 6970 2873 656c 6629 3a0a 2020  d_trip(self):.  
-00007900: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00007910: 2020 5350 414e 4e45 5220 4f56 4552 5249    SPANNER OVERRI
-00007920: 4445 3a0a 0a20 2020 2020 2020 2053 7061  DE:..        Spa
-00007930: 6e6e 6572 2063 6f6e 7665 7274 7320 7469  nner converts ti
-00007940: 6d65 7374 616d 7020 696e 746f 2060 2559  mestamp into `%Y
-00007950: 2d25 6d2d 2564 5425 483a 254d 3a25 532e  -%m-%dT%H:%M:%S.
-00007960: 2566 5a60 2066 6f72 6d61 742c 2073 6f20  %fZ` format, so 
-00007970: 746f 2061 766f 6964 0a20 2020 2020 2020  to avoid.       
-00007980: 2061 7373 6572 7420 6661 696c 7572 6573   assert failures
-00007990: 2063 6f6e 7665 7274 2064 6174 6574 696d   convert datetim
-000079a0: 6520 696e 7075 7420 746f 2074 6865 2064  e input to the d
-000079b0: 6573 6972 6520 7469 6d65 7374 616d 7020  esire timestamp 
-000079c0: 666f 726d 6174 2e0a 2020 2020 2020 2020  format..        
-000079d0: 2222 220a 2020 2020 2020 2020 6461 7465  """.        date
-000079e0: 5f74 6162 6c65 203d 2073 656c 662e 7461  _table = self.ta
-000079f0: 626c 6573 2e64 6174 655f 7461 626c 650a  bles.date_table.
-00007a00: 2020 2020 2020 2020 636f 6e66 6967 2e64          config.d
-00007a10: 622e 6578 6563 7574 6528 6461 7465 5f74  b.execute(date_t
-00007a20: 6162 6c65 2e69 6e73 6572 7428 292c 207b  able.insert(), {
-00007a30: 2264 6174 655f 6461 7461 223a 2073 656c  "date_data": sel
-00007a40: 662e 6461 7461 2c20 2269 6422 3a20 3235  f.data, "id": 25
-00007a50: 307d 290a 0a20 2020 2020 2020 2072 6f77  0})..        row
-00007a60: 203d 2063 6f6e 6669 672e 6462 2e65 7865   = config.db.exe
-00007a70: 6375 7465 2873 656c 6563 7428 5b64 6174  cute(select([dat
-00007a80: 655f 7461 626c 652e 632e 6461 7465 5f64  e_table.c.date_d
-00007a90: 6174 615d 2929 2e66 6972 7374 2829 0a20  ata])).first(). 
-00007aa0: 2020 2020 2020 2063 6f6d 7061 7265 203d         compare =
-00007ab0: 2073 656c 662e 636f 6d70 6172 6520 6f72   self.compare or
-00007ac0: 2073 656c 662e 6461 7461 0a20 2020 2020   self.data.     
-00007ad0: 2020 2063 6f6d 7061 7265 203d 2063 6f6d     compare = com
-00007ae0: 7061 7265 2e73 7472 6674 696d 6528 2225  pare.strftime("%
-00007af0: 592d 256d 2d25 6454 2548 3a25 4d3a 2553  Y-%m-%dT%H:%M:%S
-00007b00: 2e25 665a 2229 0a20 2020 2020 2020 2065  .%fZ").        e
-00007b10: 715f 2872 6f77 5b30 5d2e 7266 6333 3333  q_(row[0].rfc333
-00007b20: 3928 292c 2063 6f6d 7061 7265 290a 2020  9(), compare).  
-00007b30: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
-00007b40: 6e73 7461 6e63 6528 726f 775b 305d 2c20  nstance(row[0], 
-00007b50: 4461 7465 7469 6d65 5769 7468 4e61 6e6f  DatetimeWithNano
-00007b60: 7365 636f 6e64 7329 0a0a 2020 2020 6465  seconds)..    de
-00007b70: 6620 7465 7374 5f72 6f75 6e64 5f74 7269  f test_round_tri
-00007b80: 705f 6465 636f 7261 7465 6428 7365 6c66  p_decorated(self
-00007b90: 2c20 636f 6e6e 6563 7469 6f6e 293a 0a20  , connection):. 
-00007ba0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00007bb0: 2020 2053 5041 4e4e 4552 204f 5645 5252     SPANNER OVERR
-00007bc0: 4944 453a 0a0a 2020 2020 2020 2020 5370  IDE:..        Sp
-00007bd0: 616e 6e65 7220 636f 6e76 6572 7473 2074  anner converts t
-00007be0: 696d 6573 7461 6d70 2069 6e74 6f20 6025  imestamp into `%
-00007bf0: 592d 256d 2d25 6454 2548 3a25 4d3a 2553  Y-%m-%dT%H:%M:%S
-00007c00: 2e25 665a 6020 666f 726d 6174 2c20 736f  .%fZ` format, so
-00007c10: 2074 6f20 6176 6f69 640a 2020 2020 2020   to avoid.      
-00007c20: 2020 6173 7365 7274 2066 6169 6c75 7265    assert failure
-00007c30: 7320 636f 6e76 6572 7420 6461 7465 7469  s convert dateti
-00007c40: 6d65 2069 6e70 7574 2074 6f20 7468 6520  me input to the 
-00007c50: 6465 7369 7265 2074 696d 6573 7461 6d70  desire timestamp
-00007c60: 2066 6f72 6d61 742e 0a20 2020 2020 2020   format..       
-00007c70: 2022 2222 0a20 2020 2020 2020 2064 6174   """.        dat
-00007c80: 655f 7461 626c 6520 3d20 7365 6c66 2e74  e_table = self.t
-00007c90: 6162 6c65 732e 6461 7465 5f74 6162 6c65  ables.date_table
-00007ca0: 0a0a 2020 2020 2020 2020 636f 6e6e 6563  ..        connec
-00007cb0: 7469 6f6e 2e65 7865 6375 7465 280a 2020  tion.execute(.  
-00007cc0: 2020 2020 2020 2020 2020 6461 7465 5f74            date_t
-00007cd0: 6162 6c65 2e69 6e73 6572 7428 292c 207b  able.insert(), {
-00007ce0: 2269 6422 3a20 312c 2022 6465 636f 7261  "id": 1, "decora
-00007cf0: 7465 645f 6461 7465 5f64 6174 6122 3a20  ted_date_data": 
-00007d00: 7365 6c66 2e64 6174 617d 0a20 2020 2020  self.data}.     
-00007d10: 2020 2029 0a0a 2020 2020 2020 2020 726f     )..        ro
-00007d20: 7720 3d20 636f 6e6e 6563 7469 6f6e 2e65  w = connection.e
-00007d30: 7865 6375 7465 2873 656c 6563 7428 6461  xecute(select(da
-00007d40: 7465 5f74 6162 6c65 2e63 2e64 6563 6f72  te_table.c.decor
-00007d50: 6174 6564 5f64 6174 655f 6461 7461 2929  ated_date_data))
-00007d60: 2e66 6972 7374 2829 0a0a 2020 2020 2020  .first()..      
-00007d70: 2020 636f 6d70 6172 6520 3d20 7365 6c66    compare = self
-00007d80: 2e63 6f6d 7061 7265 206f 7220 7365 6c66  .compare or self
-00007d90: 2e64 6174 610a 2020 2020 2020 2020 636f  .data.        co
-00007da0: 6d70 6172 6520 3d20 636f 6d70 6172 652e  mpare = compare.
-00007db0: 7374 7266 7469 6d65 2822 2559 2d25 6d2d  strftime("%Y-%m-
-00007dc0: 2564 5425 483a 254d 3a25 532e 2566 5a22  %dT%H:%M:%S.%fZ"
-00007dd0: 290a 2020 2020 2020 2020 6571 5f28 726f  ).        eq_(ro
-00007de0: 775b 305d 2e72 6663 3333 3339 2829 2c20  w[0].rfc3339(), 
-00007df0: 636f 6d70 6172 6529 0a20 2020 2020 2020  compare).       
-00007e00: 2061 7373 6572 7420 6973 696e 7374 616e   assert isinstan
-00007e10: 6365 2872 6f77 5b30 5d2c 2044 6174 6574  ce(row[0], Datet
-00007e20: 696d 6557 6974 684e 616e 6f73 6563 6f6e  imeWithNanosecon
-00007e30: 6473 290a 0a20 2020 2040 7079 7465 7374  ds)..    @pytest
-00007e40: 2e6d 6172 6b2e 736b 6970 6966 280a 2020  .mark.skipif(.  
-00007e50: 2020 2020 2020 626f 6f6c 286f 732e 656e        bool(os.en
-00007e60: 7669 726f 6e2e 6765 7428 2253 5041 4e4e  viron.get("SPANN
-00007e70: 4552 5f45 4d55 4c41 544f 525f 484f 5354  ER_EMULATOR_HOST
-00007e80: 2229 292c 2072 6561 736f 6e3d 2253 6b69  ")), reason="Ski
-00007e90: 7070 6564 206f 6e20 656d 756c 6174 6f72  pped on emulator
-00007ea0: 220a 2020 2020 290a 2020 2020 6465 6620  ".    ).    def 
-00007eb0: 7465 7374 5f6e 756c 6c5f 626f 756e 645f  test_null_bound_
-00007ec0: 636f 6d70 6172 6973 6f6e 2873 656c 6629  comparison(self)
-00007ed0: 3a0a 2020 2020 2020 2020 7375 7065 7228  :.        super(
-00007ee0: 292e 7465 7374 5f6e 756c 6c5f 626f 756e  ).test_null_boun
-00007ef0: 645f 636f 6d70 6172 6973 6f6e 2829 0a0a  d_comparison()..
-00007f00: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-00007f10: 2e73 6b69 7069 6628 0a20 2020 2020 2020  .skipif(.       
-00007f20: 2062 6f6f 6c28 6f73 2e65 6e76 6972 6f6e   bool(os.environ
-00007f30: 2e67 6574 2822 5350 414e 4e45 525f 454d  .get("SPANNER_EM
-00007f40: 554c 4154 4f52 5f48 4f53 5422 2929 2c20  ULATOR_HOST")), 
-00007f50: 7265 6173 6f6e 3d22 536b 6970 7065 6420  reason="Skipped 
-00007f60: 6f6e 2065 6d75 6c61 746f 7222 0a20 2020  on emulator".   
-00007f70: 2029 0a20 2020 2064 6566 2074 6573 745f   ).    def test_
-00007f80: 6e75 6c6c 2873 656c 662c 2063 6f6e 6e65  null(self, conne
-00007f90: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
-00007fa0: 7375 7065 7228 292e 7465 7374 5f6e 756c  super().test_nul
-00007fb0: 6c28 636f 6e6e 6563 7469 6f6e 290a 0a0a  l(connection)...
-00007fc0: 636c 6173 7320 4461 7465 5469 6d65 5465  class DateTimeTe
-00007fd0: 7374 285f 4461 7465 5469 6d65 5465 7374  st(_DateTimeTest
-00007fe0: 2c20 4461 7465 5469 6d65 4d69 6372 6f73  , DateTimeMicros
-00007ff0: 6563 6f6e 6473 5465 7374 293a 0a20 2020  econdsTest):.   
-00008000: 2022 2222 0a20 2020 2053 5041 4e4e 4552   """.    SPANNER
-00008010: 204f 5645 5252 4944 453a 0a0a 2020 2020   OVERRIDE:..    
-00008020: 4461 7465 5469 6d65 5465 7374 2074 6573  DateTimeTest tes
-00008030: 7473 2068 6176 6520 7468 6520 7361 6d65  ts have the same
-00008040: 2066 6169 6c75 7265 7320 7361 6d65 2061   failures same a
-00008050: 7320 4461 7465 5469 6d65 4d69 6372 6f73  s DateTimeMicros
-00008060: 6563 6f6e 6473 5465 7374 2074 6573 7473  econdsTest tests
-00008070: 2c0a 2020 2020 736f 2074 6f20 6176 6f69  ,.    so to avoi
-00008080: 6420 7468 6f73 6520 6661 696c 7572 6573  d those failures
-00008090: 2061 6e64 206d 6169 6e74 6169 6e20 4452   and maintain DR
-000080a0: 5920 636f 6e63 6570 7420 6a75 7374 2069  Y concept just i
-000080b0: 6e68 6572 6974 2074 6865 2063 6c61 7373  nherit the class
-000080c0: 2074 6f20 7275 6e0a 2020 2020 7465 7374   to run.    test
-000080d0: 7320 7375 6363 6573 7366 756c 6c79 2e0a  s successfully..
-000080e0: 2020 2020 2222 220a 0a20 2020 2040 7079      """..    @py
-000080f0: 7465 7374 2e6d 6172 6b2e 736b 6970 6966  test.mark.skipif
-00008100: 280a 2020 2020 2020 2020 626f 6f6c 286f  (.        bool(o
-00008110: 732e 656e 7669 726f 6e2e 6765 7428 2253  s.environ.get("S
-00008120: 5041 4e4e 4552 5f45 4d55 4c41 544f 525f  PANNER_EMULATOR_
-00008130: 484f 5354 2229 292c 2072 6561 736f 6e3d  HOST")), reason=
-00008140: 2253 6b69 7070 6564 206f 6e20 656d 756c  "Skipped on emul
-00008150: 6174 6f72 220a 2020 2020 290a 2020 2020  ator".    ).    
-00008160: 6465 6620 7465 7374 5f6e 756c 6c5f 626f  def test_null_bo
-00008170: 756e 645f 636f 6d70 6172 6973 6f6e 2873  und_comparison(s
-00008180: 656c 6629 3a0a 2020 2020 2020 2020 7375  elf):.        su
-00008190: 7065 7228 292e 7465 7374 5f6e 756c 6c5f  per().test_null_
-000081a0: 626f 756e 645f 636f 6d70 6172 6973 6f6e  bound_comparison
-000081b0: 2829 0a0a 2020 2020 4070 7974 6573 742e  ()..    @pytest.
-000081c0: 6d61 726b 2e73 6b69 7069 6628 0a20 2020  mark.skipif(.   
-000081d0: 2020 2020 2062 6f6f 6c28 6f73 2e65 6e76       bool(os.env
-000081e0: 6972 6f6e 2e67 6574 2822 5350 414e 4e45  iron.get("SPANNE
-000081f0: 525f 454d 554c 4154 4f52 5f48 4f53 5422  R_EMULATOR_HOST"
-00008200: 2929 2c20 7265 6173 6f6e 3d22 536b 6970  )), reason="Skip
-00008210: 7065 6420 6f6e 2065 6d75 6c61 746f 7222  ped on emulator"
-00008220: 0a20 2020 2029 0a20 2020 2064 6566 2074  .    ).    def t
-00008230: 6573 745f 6e75 6c6c 2873 656c 662c 2063  est_null(self, c
-00008240: 6f6e 6e65 6374 696f 6e29 3a0a 2020 2020  onnection):.    
-00008250: 2020 2020 7375 7065 7228 292e 7465 7374      super().test
-00008260: 5f6e 756c 6c28 636f 6e6e 6563 7469 6f6e  _null(connection
-00008270: 290a 0a20 2020 2040 7079 7465 7374 2e6d  )..    @pytest.m
-00008280: 6172 6b2e 736b 6970 2822 5370 616e 6e65  ark.skip("Spanne
-00008290: 7220 6461 7465 7320 6172 6520 7469 6d65  r dates are time
-000082a0: 207a 6f6e 6520 696e 6465 7065 6e64 656e   zone independen
-000082b0: 7422 290a 2020 2020 6465 6620 7465 7374  t").    def test
-000082c0: 5f73 656c 6563 745f 6469 7265 6374 2873  _select_direct(s
-000082d0: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-000082e0: 7373 0a0a 0a40 7079 7465 7374 2e6d 6172  ss...@pytest.mar
-000082f0: 6b2e 736b 6970 2822 4e6f 7420 7375 7070  k.skip("Not supp
-00008300: 6f72 7465 6420 6279 2053 7061 6e6e 6572  orted by Spanner
-00008310: 2229 0a63 6c61 7373 2044 6966 6669 6375  ").class Difficu
-00008320: 6c74 5061 7261 6d65 7465 7273 5465 7374  ltParametersTest
-00008330: 285f 4469 6666 6963 756c 7450 6172 616d  (_DifficultParam
-00008340: 6574 6572 7354 6573 7429 3a0a 2020 2020  etersTest):.    
-00008350: 7061 7373 0a0a 0a63 6c61 7373 2046 6574  pass...class Fet
-00008360: 6368 4c69 6d69 744f 6666 7365 7454 6573  chLimitOffsetTes
-00008370: 7428 5f46 6574 6368 4c69 6d69 744f 6666  t(_FetchLimitOff
-00008380: 7365 7454 6573 7429 3a0a 2020 2020 4070  setTest):.    @p
-00008390: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
-000083a0: 2253 7061 6e6e 6572 2064 6f65 736e 2774  "Spanner doesn't
-000083b0: 2073 7570 706f 7274 2063 6f6d 706f 7369   support composi
-000083c0: 7465 204c 494d 4954 2061 6e64 204f 4646  te LIMIT and OFF
-000083d0: 5345 5420 636c 6175 7365 7322 290a 2020  SET clauses").  
-000083e0: 2020 6465 6620 7465 7374 5f65 7870 725f    def test_expr_
-000083f0: 6c69 6d69 7428 7365 6c66 2c20 636f 6e6e  limit(self, conn
-00008400: 6563 7469 6f6e 293a 0a20 2020 2020 2020  ection):.       
-00008410: 2070 6173 730a 0a20 2020 2040 7079 7465   pass..    @pyte
-00008420: 7374 2e6d 6172 6b2e 736b 6970 2822 5370  st.mark.skip("Sp
-00008430: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
-00008440: 7070 6f72 7420 636f 6d70 6f73 6974 6520  pport composite 
-00008450: 4c49 4d49 5420 616e 6420 4f46 4653 4554  LIMIT and OFFSET
-00008460: 2063 6c61 7573 6573 2229 0a20 2020 2064   clauses").    d
-00008470: 6566 2074 6573 745f 6578 7072 5f6f 6666  ef test_expr_off
-00008480: 7365 7428 7365 6c66 2c20 636f 6e6e 6563  set(self, connec
-00008490: 7469 6f6e 293a 0a20 2020 2020 2020 2070  tion):.        p
-000084a0: 6173 730a 0a20 2020 2040 7079 7465 7374  ass..    @pytest
-000084b0: 2e6d 6172 6b2e 736b 6970 2822 5370 616e  .mark.skip("Span
-000084c0: 6e65 7220 646f 6573 6e27 7420 7375 7070  ner doesn't supp
-000084d0: 6f72 7420 636f 6d70 6f73 6974 6520 4c49  ort composite LI
-000084e0: 4d49 5420 616e 6420 4f46 4653 4554 2063  MIT and OFFSET c
-000084f0: 6c61 7573 6573 2229 0a20 2020 2064 6566  lauses").    def
-00008500: 2074 6573 745f 6578 7072 5f6c 696d 6974   test_expr_limit
-00008510: 5f6f 6666 7365 7428 7365 6c66 2c20 636f  _offset(self, co
-00008520: 6e6e 6563 7469 6f6e 293a 0a20 2020 2020  nnection):.     
-00008530: 2020 2070 6173 730a 0a20 2020 2040 7079     pass..    @py
-00008540: 7465 7374 2e6d 6172 6b2e 736b 6970 2822  test.mark.skip("
-00008550: 5370 616e 6e65 7220 646f 6573 6e27 7420  Spanner doesn't 
-00008560: 7375 7070 6f72 7420 636f 6d70 6f73 6974  support composit
-00008570: 6520 4c49 4d49 5420 616e 6420 4f46 4653  e LIMIT and OFFS
-00008580: 4554 2063 6c61 7573 6573 2229 0a20 2020  ET clauses").   
-00008590: 2064 6566 2074 6573 745f 6578 7072 5f6c   def test_expr_l
-000085a0: 696d 6974 5f73 696d 706c 655f 6f66 6673  imit_simple_offs
-000085b0: 6574 2873 656c 662c 2063 6f6e 6e65 6374  et(self, connect
-000085c0: 696f 6e29 3a0a 2020 2020 2020 2020 7061  ion):.        pa
-000085d0: 7373 0a0a 2020 2020 4070 7974 6573 742e  ss..    @pytest.
-000085e0: 6d61 726b 2e73 6b69 7028 2253 7061 6e6e  mark.skip("Spann
-000085f0: 6572 2064 6f65 736e 2774 2073 7570 706f  er doesn't suppo
-00008600: 7274 2063 6f6d 706f 7369 7465 204c 494d  rt composite LIM
-00008610: 4954 2061 6e64 204f 4646 5345 5420 636c  IT and OFFSET cl
-00008620: 6175 7365 7322 290a 2020 2020 6465 6620  auses").    def 
-00008630: 7465 7374 5f73 696d 706c 655f 6c69 6d69  test_simple_limi
-00008640: 745f 6578 7072 5f6f 6666 7365 7428 7365  t_expr_offset(se
-00008650: 6c66 2c20 636f 6e6e 6563 7469 6f6e 293a  lf, connection):
-00008660: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00008670: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-00008680: 736b 6970 2822 5370 616e 6e65 7220 646f  skip("Spanner do
-00008690: 6573 6e27 7420 7375 7070 6f72 7420 636f  esn't support co
-000086a0: 6d70 6f73 6974 6520 4c49 4d49 5420 616e  mposite LIMIT an
-000086b0: 6420 4f46 4653 4554 2063 6c61 7573 6573  d OFFSET clauses
-000086c0: 2229 0a20 2020 2064 6566 2074 6573 745f  ").    def test_
-000086d0: 626f 756e 645f 6f66 6673 6574 2873 656c  bound_offset(sel
-000086e0: 662c 2063 6f6e 6e65 6374 696f 6e29 3a0a  f, connection):.
-000086f0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00008700: 2020 6465 6620 7465 7374 5f6c 696d 6974    def test_limit
-00008710: 5f72 656e 6465 725f 6d75 6c74 6970 6c65  _render_multiple
-00008720: 5f74 696d 6573 2873 656c 662c 2063 6f6e  _times(self, con
-00008730: 6e65 6374 696f 6e29 3a0a 2020 2020 2020  nection):.      
-00008740: 2020 7461 626c 6520 3d20 7365 6c66 2e74    table = self.t
-00008750: 6162 6c65 732e 736f 6d65 5f74 6162 6c65  ables.some_table
-00008760: 0a20 2020 2020 2020 2073 746d 7420 3d20  .        stmt = 
-00008770: 7365 6c65 6374 2874 6162 6c65 2e63 2e69  select(table.c.i
-00008780: 6429 2e6c 696d 6974 2831 292e 7363 616c  d).limit(1).scal
-00008790: 6172 5f73 7562 7175 6572 7928 290a 0a20  ar_subquery().. 
-000087a0: 2020 2020 2020 2075 203d 2075 6e69 6f6e         u = union
-000087b0: 2873 656c 6563 7428 7374 6d74 292c 2073  (select(stmt), s
-000087c0: 656c 6563 7428 7374 6d74 2929 2e73 7562  elect(stmt)).sub
-000087d0: 7175 6572 7928 292e 7365 6c65 6374 2829  query().select()
-000087e0: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-000087f0: 6173 7365 7274 5f72 6573 756c 7428 0a20  assert_result(. 
-00008800: 2020 2020 2020 2020 2020 2063 6f6e 6e65             conne
-00008810: 6374 696f 6e2c 0a20 2020 2020 2020 2020  ction,.         
-00008820: 2020 2075 2c0a 2020 2020 2020 2020 2020     u,.          
-00008830: 2020 5b28 322c 295d 2c0a 2020 2020 2020    [(2,)],.      
-00008840: 2020 290a 0a0a 4070 7974 6573 742e 6d61    )...@pytest.ma
-00008850: 726b 2e73 6b69 7028 2253 7061 6e6e 6572  rk.skip("Spanner
-00008860: 2064 6f65 736e 2774 2073 7570 706f 7274   doesn't support
-00008870: 2061 7574 6f69 6e63 7265 6d65 6e74 2229   autoincrement")
-00008880: 0a63 6c61 7373 2049 6465 6e74 6974 7941  .class IdentityA
-00008890: 7574 6f69 6e63 7265 6d65 6e74 5465 7374  utoincrementTest
-000088a0: 285f 4964 656e 7469 7479 4175 746f 696e  (_IdentityAutoin
-000088b0: 6372 656d 656e 7454 6573 7429 3a0a 2020  crementTest):.  
-000088c0: 2020 7061 7373 0a0a 0a63 6c61 7373 2045    pass...class E
-000088d0: 7363 6170 696e 6754 6573 7428 5f45 7363  scapingTest(_Esc
-000088e0: 6170 696e 6754 6573 7429 3a0a 2020 2020  apingTest):.    
-000088f0: 4070 726f 7669 6465 5f6d 6574 6164 6174  @provide_metadat
-00008900: 610a 2020 2020 6465 6620 7465 7374 5f70  a.    def test_p
-00008910: 6572 6365 6e74 5f73 6967 6e5f 726f 756e  ercent_sign_roun
-00008920: 645f 7472 6970 2873 656c 6629 3a0a 2020  d_trip(self):.  
-00008930: 2020 2020 2020 2222 2254 6573 7420 7468        """Test th
-00008940: 6174 2074 6865 2044 4241 5049 2061 6363  at the DBAPI acc
-00008950: 6f6d 6d6f 6461 7465 7320 666f 7220 6573  ommodates for es
-00008960: 6361 7065 6420 2f20 6e6f 6e65 7363 6170  caped / nonescap
-00008970: 6564 0a20 2020 2020 2020 2070 6572 6365  ed.        perce
-00008980: 6e74 2073 6967 6e73 2069 6e20 6120 7761  nt signs in a wa
-00008990: 7920 7468 6174 206d 6174 6368 6573 2074  y that matches t
-000089a0: 6865 2063 6f6d 7069 6c65 720a 0a20 2020  he compiler..   
-000089b0: 2020 2020 2053 5041 4e4e 4552 204f 5645       SPANNER OVE
-000089c0: 5252 4944 450a 2020 2020 2020 2020 436c  RRIDE.        Cl
-000089d0: 6f75 6420 5370 616e 6e65 7220 7375 7070  oud Spanner supp
-000089e0: 6f72 7473 2074 6162 6c65 7320 7769 7468  orts tables with
-000089f0: 2065 6d70 7479 2070 7269 6d61 7279 206b   empty primary k
-00008a00: 6579 2c20 6275 740a 2020 2020 2020 2020  ey, but.        
-00008a10: 6f6e 6c79 2073 696e 676c 6520 6f6e 6520  only single one 
-00008a20: 726f 7720 6361 6e20 6265 2069 6e73 6572  row can be inser
-00008a30: 7465 6420 696e 746f 2073 7563 6820 6120  ted into such a 
-00008a40: 7461 626c 6520 2d0a 2020 2020 2020 2020  table -.        
-00008a50: 666f 6c6c 6f77 696e 6720 696e 7365 7274  following insert
-00008a60: 696f 6e73 2077 696c 6c20 6661 696c 2077  ions will fail w
-00008a70: 6974 6820 6052 6f77 205b 5d20 616c 7265  ith `Row [] alre
-00008a80: 6164 7920 6578 6973 7473 222e 0a20 2020  ady exists"..   
-00008a90: 2020 2020 204f 7665 7272 6964 696e 6720       Overriding 
-00008aa0: 7468 6520 7465 7374 2074 6f20 6176 6f69  the test to avoi
-00008ab0: 6420 7468 6520 7361 6d65 2066 6169 6c75  d the same failu
-00008ac0: 7265 2e0a 2020 2020 2020 2020 2222 220a  re..        """.
-00008ad0: 2020 2020 2020 2020 6d20 3d20 7365 6c66          m = self
-00008ae0: 2e6d 6574 6164 6174 610a 2020 2020 2020  .metadata.      
-00008af0: 2020 7420 3d20 5461 626c 6528 2274 222c    t = Table("t",
-00008b00: 206d 2c20 436f 6c75 6d6e 2822 6461 7461   m, Column("data
-00008b10: 222c 2053 7472 696e 6728 3530 2929 290a  ", String(50))).
-00008b20: 2020 2020 2020 2020 742e 6372 6561 7465          t.create
-00008b30: 2863 6f6e 6669 672e 6462 290a 2020 2020  (config.db).    
-00008b40: 2020 2020 7769 7468 2063 6f6e 6669 672e      with config.
-00008b50: 6462 2e62 6567 696e 2829 2061 7320 636f  db.begin() as co
-00008b60: 6e6e 3a0a 2020 2020 2020 2020 2020 2020  nn:.            
-00008b70: 636f 6e6e 2e65 7865 6375 7465 2874 2e69  conn.execute(t.i
-00008b80: 6e73 6572 7428 292c 2064 6963 7428 6461  nsert(), dict(da
-00008b90: 7461 3d22 736f 6d65 2025 2076 616c 7565  ta="some % value
-00008ba0: 2229 290a 0a20 2020 2020 2020 2020 2020  "))..           
-00008bb0: 2065 715f 280a 2020 2020 2020 2020 2020   eq_(.          
-00008bc0: 2020 2020 2020 636f 6e6e 2e73 6361 6c61        conn.scala
-00008bd0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-00008be0: 2020 2020 2020 2073 656c 6563 7428 5b74         select([t
-00008bf0: 2e63 2e64 6174 615d 292e 7768 6572 6528  .c.data]).where(
-00008c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008c10: 2020 2020 2020 2020 2074 2e63 2e64 6174           t.c.dat
-00008c20: 6120 3d3d 206c 6974 6572 616c 5f63 6f6c  a == literal_col
-00008c30: 756d 6e28 2227 736f 6d65 2025 2076 616c  umn("'some % val
-00008c40: 7565 2722 290a 2020 2020 2020 2020 2020  ue'").          
-00008c50: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00008c60: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-00008c70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00008c80: 736f 6d65 2025 2076 616c 7565 222c 0a20  some % value",. 
-00008c90: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00008ca0: 2020 2020 2020 2020 2020 636f 6e6e 2e65            conn.e
-00008cb0: 7865 6375 7465 2874 2e64 656c 6574 6528  xecute(t.delete(
-00008cc0: 2929 0a20 2020 2020 2020 2020 2020 2063  )).            c
-00008cd0: 6f6e 6e2e 6578 6563 7574 6528 742e 696e  onn.execute(t.in
-00008ce0: 7365 7274 2829 2c20 6469 6374 2864 6174  sert(), dict(dat
-00008cf0: 613d 2273 6f6d 6520 2525 206f 7468 6572  a="some %% other
-00008d00: 2076 616c 7565 2229 290a 2020 2020 2020   value")).      
-00008d10: 2020 2020 2020 6571 5f28 0a20 2020 2020        eq_(.     
-00008d20: 2020 2020 2020 2020 2020 2063 6f6e 6e2e             conn.
-00008d30: 7363 616c 6172 280a 2020 2020 2020 2020  scalar(.        
-00008d40: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
-00008d50: 6374 285b 742e 632e 6461 7461 5d29 2e77  ct([t.c.data]).w
-00008d60: 6865 7265 280a 2020 2020 2020 2020 2020  here(.          
-00008d70: 2020 2020 2020 2020 2020 2020 2020 742e                t.
-00008d80: 632e 6461 7461 203d 3d20 6c69 7465 7261  c.data == litera
-00008d90: 6c5f 636f 6c75 6d6e 2822 2773 6f6d 6520  l_column("'some 
-00008da0: 2525 206f 7468 6572 2076 616c 7565 2722  %% other value'"
-00008db0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00008dc0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00008dd0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-00008de0: 2020 2020 2020 2020 2020 2022 736f 6d65             "some
-00008df0: 2025 2520 6f74 6865 7220 7661 6c75 6522   %% other value"
-00008e00: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00008e10: 0a0a 636c 6173 7320 4578 6973 7473 5465  ..class ExistsTe
-00008e20: 7374 285f 4578 6973 7473 5465 7374 293a  st(_ExistsTest):
-00008e30: 0a20 2020 2064 6566 2074 6573 745f 7365  .    def test_se
-00008e40: 6c65 6374 5f65 7869 7374 7328 7365 6c66  lect_exists(self
-00008e50: 2c20 636f 6e6e 6563 7469 6f6e 293a 0a20  , connection):. 
-00008e60: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00008e70: 2020 2053 5041 4e4e 4552 204f 5645 5252     SPANNER OVERR
-00008e80: 4944 453a 0a0a 2020 2020 2020 2020 5468  IDE:..        Th
-00008e90: 6520 6f72 6967 696e 616c 2074 6573 7420  e original test 
-00008ea0: 6973 2074 7279 696e 6720 746f 2065 7865  is trying to exe
-00008eb0: 6375 7465 2061 2071 7565 7279 206c 696b  cute a query lik
-00008ec0: 653a 0a0a 2020 2020 2020 2020 5345 4c45  e:..        SELE
-00008ed0: 4354 202e 2e2e 0a20 2020 2020 2020 2057  CT ....        W
-00008ee0: 4845 5245 2045 5849 5354 5320 2853 454c  HERE EXISTS (SEL
-00008ef0: 4543 5420 2e2e 2e29 0a0a 2020 2020 2020  ECT ...)..      
-00008f00: 2020 5345 4c45 4354 2057 4845 5245 2077    SELECT WHERE w
-00008f10: 6974 686f 7574 2046 524f 4d20 636c 6175  ithout FROM clau
-00008f20: 7365 2069 7320 6e6f 7420 7375 7070 6f72  se is not suppor
-00008f30: 7465 6420 6279 2053 7061 6e6e 6572 2e0a  ted by Spanner..
-00008f40: 2020 2020 2020 2020 5265 7772 6974 696e          Rewritin
-00008f50: 6720 7468 6520 7465 7374 2074 6f20 666f  g the test to fo
-00008f60: 7263 6520 6974 2074 6f20 6765 6e65 7261  rce it to genera
-00008f70: 7465 2061 2071 7565 7279 206c 696b 653a  te a query like:
-00008f80: 0a0a 2020 2020 2020 2020 5345 4c45 4354  ..        SELECT
-00008f90: 2045 5849 5354 5320 2853 454c 4543 5420   EXISTS (SELECT 
-00008fa0: 2e2e 2e29 0a20 2020 2020 2020 2022 2222  ...).        """
-00008fb0: 0a20 2020 2020 2020 2073 7475 6666 203d  .        stuff =
-00008fc0: 2073 656c 662e 7461 626c 6573 2e73 7475   self.tables.stu
-00008fd0: 6666 0a20 2020 2020 2020 2065 715f 280a  ff.        eq_(.
-00008fe0: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
-00008ff0: 6563 7469 6f6e 2e65 7865 6375 7465 280a  ection.execute(.
-00009000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009010: 7365 6c65 6374 2828 6578 6973 7473 2829  select((exists()
-00009020: 2e77 6865 7265 2873 7475 6666 2e63 2e64  .where(stuff.c.d
-00009030: 6174 6120 3d3d 2022 736f 6d65 2064 6174  ata == "some dat
-00009040: 6122 292c 2929 0a20 2020 2020 2020 2020  a"),)).         
-00009050: 2020 2029 2e66 6574 6368 616c 6c28 292c     ).fetchall(),
-00009060: 0a20 2020 2020 2020 2020 2020 205b 2854  .            [(T
-00009070: 7275 652c 295d 2c0a 2020 2020 2020 2020  rue,)],.        
-00009080: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00009090: 7365 6c65 6374 5f65 7869 7374 735f 6661  select_exists_fa
-000090a0: 6c73 6528 7365 6c66 2c20 636f 6e6e 6563  lse(self, connec
-000090b0: 7469 6f6e 293a 0a20 2020 2020 2020 2022  tion):.        "
-000090c0: 2222 0a20 2020 2020 2020 2053 5041 4e4e  "".        SPANN
-000090d0: 4552 204f 5645 5252 4944 453a 0a0a 2020  ER OVERRIDE:..  
-000090e0: 2020 2020 2020 5468 6520 6f72 6967 696e        The origin
-000090f0: 616c 2074 6573 7420 6973 2074 7279 696e  al test is tryin
-00009100: 6720 746f 2065 7865 6375 7465 2061 2071  g to execute a q
-00009110: 7565 7279 206c 696b 653a 0a0a 2020 2020  uery like:..    
-00009120: 2020 2020 5345 4c45 4354 202e 2e2e 0a20      SELECT .... 
-00009130: 2020 2020 2020 2057 4845 5245 2045 5849         WHERE EXI
-00009140: 5354 5320 2853 454c 4543 5420 2e2e 2e29  STS (SELECT ...)
-00009150: 0a0a 2020 2020 2020 2020 5345 4c45 4354  ..        SELECT
-00009160: 2057 4845 5245 2077 6974 686f 7574 2046   WHERE without F
-00009170: 524f 4d20 636c 6175 7365 2069 7320 6e6f  ROM clause is no
-00009180: 7420 7375 7070 6f72 7465 6420 6279 2053  t supported by S
-00009190: 7061 6e6e 6572 2e0a 2020 2020 2020 2020  panner..        
-000091a0: 5265 7772 6974 696e 6720 7468 6520 7465  Rewriting the te
-000091b0: 7374 2074 6f20 666f 7263 6520 6974 2074  st to force it t
-000091c0: 6f20 6765 6e65 7261 7465 2061 2071 7565  o generate a que
-000091d0: 7279 206c 696b 653a 0a0a 2020 2020 2020  ry like:..      
-000091e0: 2020 5345 4c45 4354 2045 5849 5354 5320    SELECT EXISTS 
-000091f0: 2853 454c 4543 5420 2e2e 2e29 0a20 2020  (SELECT ...).   
-00009200: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00009210: 2073 7475 6666 203d 2073 656c 662e 7461   stuff = self.ta
-00009220: 626c 6573 2e73 7475 6666 0a20 2020 2020  bles.stuff.     
-00009230: 2020 2065 715f 280a 2020 2020 2020 2020     eq_(.        
-00009240: 2020 2020 636f 6e6e 6563 7469 6f6e 2e65      connection.e
-00009250: 7865 6375 7465 280a 2020 2020 2020 2020  xecute(.        
-00009260: 2020 2020 2020 2020 7365 6c65 6374 2828          select((
-00009270: 6578 6973 7473 2829 2e77 6865 7265 2873  exists().where(s
-00009280: 7475 6666 2e63 2e64 6174 6120 3d3d 2022  tuff.c.data == "
-00009290: 6e6f 2064 6174 6122 292c 2929 0a20 2020  no data"),)).   
-000092a0: 2020 2020 2020 2020 2029 2e66 6574 6368           ).fetch
-000092b0: 616c 6c28 292c 0a20 2020 2020 2020 2020  all(),.         
-000092c0: 2020 205b 2846 616c 7365 2c29 5d2c 0a20     [(False,)],. 
-000092d0: 2020 2020 2020 2029 0a0a 0a63 6c61 7373         )...class
-000092e0: 2054 6162 6c65 4444 4c54 6573 7428 5f54   TableDDLTest(_T
-000092f0: 6162 6c65 4444 4c54 6573 7429 3a0a 2020  ableDDLTest):.  
-00009300: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
-00009310: 6b69 7028 0a20 2020 2020 2020 2022 5370  kip(.        "Sp
-00009320: 616e 6e65 7220 7461 626c 6520 6e61 6d65  anner table name
-00009330: 206d 7573 7420 7374 6172 7420 7769 7468   must start with
-00009340: 2061 6e20 7570 7065 7263 6173 6520 6f72   an uppercase or
-00009350: 206c 6f77 6572 6361 7365 206c 6574 7465   lowercase lette
-00009360: 7222 0a20 2020 2029 0a20 2020 2064 6566  r".    ).    def
-00009370: 2074 6573 745f 756e 6465 7273 636f 7265   test_underscore
-00009380: 5f6e 616d 6573 2873 656c 6629 3a0a 2020  _names(self):.  
-00009390: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-000093a0: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
-000093b0: 7028 2254 6162 6c65 206e 616d 6573 2069  p("Table names i
-000093c0: 6e63 7564 696e 6720 7363 6865 6d61 7320  ncuding schemas 
-000093d0: 6172 6520 6e6f 7420 7375 7070 6f72 7465  are not supporte
-000093e0: 6420 6279 2053 7061 6e6e 6572 2229 0a20  d by Spanner"). 
-000093f0: 2020 2064 6566 2074 6573 745f 6372 6561     def test_crea
-00009400: 7465 5f74 6162 6c65 5f73 6368 656d 6128  te_table_schema(
-00009410: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00009420: 6173 730a 0a0a 636c 6173 7320 4675 7475  ass...class Futu
-00009430: 7265 5461 626c 6544 444c 5465 7374 285f  reTableDDLTest(_
-00009440: 4675 7475 7265 5461 626c 6544 444c 5465  FutureTableDDLTe
-00009450: 7374 293a 0a20 2020 2040 7079 7465 7374  st):.    @pytest
-00009460: 2e6d 6172 6b2e 736b 6970 2822 5461 626c  .mark.skip("Tabl
-00009470: 6520 6e61 6d65 7320 696e 6375 6469 6e67  e names incuding
-00009480: 2073 6368 656d 6173 2061 7265 206e 6f74   schemas are not
-00009490: 2073 7570 706f 7274 6564 2062 7920 5370   supported by Sp
-000094a0: 616e 6e65 7222 290a 2020 2020 6465 6620  anner").    def 
-000094b0: 7465 7374 5f63 7265 6174 655f 7461 626c  test_create_tabl
-000094c0: 655f 7363 6865 6d61 2873 656c 6629 3a0a  e_schema(self):.
-000094d0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-000094e0: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
-000094f0: 6b69 7028 0a20 2020 2020 2020 2022 5370  kip(.        "Sp
-00009500: 616e 6e65 7220 7461 626c 6520 6e61 6d65  anner table name
-00009510: 206d 7573 7420 7374 6172 7420 7769 7468   must start with
-00009520: 2061 6e20 7570 7065 7263 6173 6520 6f72   an uppercase or
-00009530: 206c 6f77 6572 6361 7365 206c 6574 7465   lowercase lette
-00009540: 7222 0a20 2020 2029 0a20 2020 2064 6566  r".    ).    def
-00009550: 2074 6573 745f 756e 6465 7273 636f 7265   test_underscore
-00009560: 5f6e 616d 6573 2873 656c 6629 3a0a 2020  _names(self):.  
-00009570: 2020 2020 2020 7061 7373 0a0a 0a40 7079        pass...@py
-00009580: 7465 7374 2e6d 6172 6b2e 736b 6970 2822  test.mark.skip("
-00009590: 4d61 7820 6964 656e 7469 6669 6572 206c  Max identifier l
-000095a0: 656e 6774 6820 696e 2053 7061 6e6e 6572  ength in Spanner
-000095b0: 2069 7320 3132 3822 290a 636c 6173 7320   is 128").class 
-000095c0: 4c6f 6e67 4e61 6d65 426c 6f77 6f75 7454  LongNameBlowoutT
-000095d0: 6573 7428 5f4c 6f6e 674e 616d 6542 6c6f  est(_LongNameBlo
-000095e0: 776f 7574 5465 7374 293a 0a20 2020 2070  woutTest):.    p
-000095f0: 6173 730a 0a0a 4070 7974 6573 742e 6d61  ass...@pytest.ma
-00009600: 726b 2e73 6b69 7028 2253 7061 6e6e 6572  rk.skip("Spanner
-00009610: 2064 6f65 736e 2774 2073 7570 706f 7274   doesn't support
-00009620: 2054 696d 6520 6461 7461 2074 7970 652e   Time data type.
-00009630: 2229 0a63 6c61 7373 2054 696d 6554 6573  ").class TimeTes
-00009640: 7473 285f 5469 6d65 4d69 6372 6f73 6563  ts(_TimeMicrosec
-00009650: 6f6e 6473 5465 7374 2c20 5f54 696d 6554  ondsTest, _TimeT
-00009660: 6573 7429 3a0a 2020 2020 7061 7373 0a0a  est):.    pass..
-00009670: 0a40 7079 7465 7374 2e6d 6172 6b2e 736b  .@pytest.mark.sk
-00009680: 6970 2822 5370 616e 6e65 7220 646f 6573  ip("Spanner does
-00009690: 6e27 7420 636f 6572 6365 2064 6174 6573  n't coerce dates
-000096a0: 2066 726f 6d20 6461 7465 7469 6d65 2e22   from datetime."
-000096b0: 290a 636c 6173 7320 4461 7465 5469 6d65  ).class DateTime
-000096c0: 436f 6572 6365 6454 6f44 6174 6554 696d  CoercedToDateTim
-000096d0: 6554 6573 7428 5f44 6174 6554 696d 6543  eTest(_DateTimeC
-000096e0: 6f65 7263 6564 546f 4461 7465 5469 6d65  oercedToDateTime
-000096f0: 5465 7374 293a 0a20 2020 2070 6173 730a  Test):.    pass.
-00009700: 0a0a 636c 6173 7320 496e 7465 6765 7254  ..class IntegerT
-00009710: 6573 7428 5f49 6e74 6567 6572 5465 7374  est(_IntegerTest
-00009720: 293a 0a20 2020 2040 7072 6f76 6964 655f  ):.    @provide_
-00009730: 6d65 7461 6461 7461 0a20 2020 2064 6566  metadata.    def
-00009740: 205f 726f 756e 645f 7472 6970 2873 656c   _round_trip(sel
-00009750: 662c 2064 6174 6174 7970 652c 2064 6174  f, datatype, dat
-00009760: 6129 3a0a 2020 2020 2020 2020 2222 220a  a):.        """.
-00009770: 2020 2020 2020 2020 5350 414e 4e45 5220          SPANNER 
-00009780: 4f56 4552 5249 4445 3a0a 0a20 2020 2020  OVERRIDE:..     
-00009790: 2020 2054 6869 7320 6973 2074 6865 2068     This is the h
-000097a0: 656c 7065 7220 6d65 7468 6f64 2066 6f72  elper method for
-000097b0: 2069 6e74 6567 6572 2063 6c61 7373 2074   integer class t
-000097c0: 6573 7473 2077 6869 6368 2063 7265 6174  ests which creat
-000097d0: 6573 2061 2074 6162 6c65 2061 6e64 0a20  es a table and. 
-000097e0: 2020 2020 2020 2070 6572 666f 726d 7320         performs 
-000097f0: 616e 2069 6e73 6572 7420 6f70 6572 6174  an insert operat
-00009800: 696f 6e2e 0a20 2020 2020 2020 2043 6c6f  ion..        Clo
-00009810: 7564 2053 7061 6e6e 6572 2073 7570 706f  ud Spanner suppo
-00009820: 7274 7320 7461 626c 6573 2077 6974 6820  rts tables with 
-00009830: 616e 2065 6d70 7479 2070 7269 6d61 7279  an empty primary
-00009840: 206b 6579 2c20 6275 7420 6f6e 6c79 206f   key, but only o
-00009850: 6e65 0a20 2020 2020 2020 2072 6f77 2063  ne.        row c
-00009860: 616e 2062 6520 696e 7365 7274 6564 2069  an be inserted i
-00009870: 6e74 6f20 7375 6368 2061 2074 6162 6c65  nto such a table
-00009880: 202d 2066 6f6c 6c6f 7769 6e67 2069 6e73   - following ins
-00009890: 6572 7469 6f6e 7320 7769 6c6c 2066 6169  ertions will fai
-000098a0: 6c20 7769 7468 0a20 2020 2020 2020 2060  l with.        `
-000098b0: 3430 3020 6964 206d 7573 7420 6e6f 7420  400 id must not 
-000098c0: 6265 204e 554c 4c20 696e 2074 6162 6c65  be NULL in table
-000098d0: 2064 6174 655f 7461 626c 6560 2e0a 2020   date_table`..  
-000098e0: 2020 2020 2020 4f76 6572 7269 6469 6e67        Overriding
-000098f0: 2074 6865 2074 6573 7473 2061 6e64 2061   the tests and a
-00009900: 6464 696e 6720 6120 6d61 6e75 616c 2070  dding a manual p
-00009910: 7269 6d61 7279 206b 6579 2076 616c 7565  rimary key value
-00009920: 2074 6f20 6176 6f69 6420 7468 6520 7361   to avoid the sa
-00009930: 6d65 0a20 2020 2020 2020 2066 6169 6c75  me.        failu
-00009940: 7265 732e 0a20 2020 2020 2020 2022 2222  res..        """
-00009950: 0a20 2020 2020 2020 206d 6574 6164 6174  .        metadat
-00009960: 6120 3d20 7365 6c66 2e6d 6574 6164 6174  a = self.metadat
-00009970: 610a 2020 2020 2020 2020 696e 745f 7461  a.        int_ta
-00009980: 626c 6520 3d20 5461 626c 6528 0a20 2020  ble = Table(.   
-00009990: 2020 2020 2020 2020 2022 696e 7465 6765           "intege
-000099a0: 725f 7461 626c 6522 2c0a 2020 2020 2020  r_table",.      
-000099b0: 2020 2020 2020 6d65 7461 6461 7461 2c0a        metadata,.
-000099c0: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
-000099d0: 6d6e 2822 6964 222c 2049 6e74 6567 6572  mn("id", Integer
-000099e0: 2c20 7072 696d 6172 795f 6b65 793d 5472  , primary_key=Tr
-000099f0: 7565 2c20 7465 7374 5f6e 6565 6473 5f61  ue, test_needs_a
-00009a00: 7574 6f69 6e63 7265 6d65 6e74 3d54 7275  utoincrement=Tru
-00009a10: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-00009a20: 436f 6c75 6d6e 2822 696e 7465 6765 725f  Column("integer_
-00009a30: 6461 7461 222c 2064 6174 6174 7970 6529  data", datatype)
-00009a40: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-00009a50: 2020 2020 206d 6574 6164 6174 612e 6372       metadata.cr
-00009a60: 6561 7465 5f61 6c6c 2863 6f6e 6669 672e  eate_all(config.
-00009a70: 6462 290a 0a20 2020 2020 2020 2063 6f6e  db)..        con
-00009a80: 6669 672e 6462 2e65 7865 6375 7465 2869  fig.db.execute(i
-00009a90: 6e74 5f74 6162 6c65 2e69 6e73 6572 7428  nt_table.insert(
-00009aa0: 292c 207b 2269 6422 3a20 312c 2022 696e  ), {"id": 1, "in
-00009ab0: 7465 6765 725f 6461 7461 223a 2064 6174  teger_data": dat
-00009ac0: 617d 290a 0a20 2020 2020 2020 2072 6f77  a})..        row
-00009ad0: 203d 2063 6f6e 6669 672e 6462 2e65 7865   = config.db.exe
-00009ae0: 6375 7465 2873 656c 6563 7428 5b69 6e74  cute(select([int
-00009af0: 5f74 6162 6c65 2e63 2e69 6e74 6567 6572  _table.c.integer
-00009b00: 5f64 6174 615d 2929 2e66 6972 7374 2829  _data])).first()
-00009b10: 0a0a 2020 2020 2020 2020 6571 5f28 726f  ..        eq_(ro
-00009b20: 772c 2028 6461 7461 2c29 290a 0a20 2020  w, (data,))..   
-00009b30: 2020 2020 2069 6620 7574 696c 2e70 7933       if util.py3
-00009b40: 6b3a 0a20 2020 2020 2020 2020 2020 2061  k:.            a
-00009b50: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
-00009b60: 2872 6f77 5b30 5d2c 2069 6e74 290a 2020  (row[0], int).  
-00009b70: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00009b80: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
-00009b90: 7369 6e73 7461 6e63 6528 726f 775b 305d  sinstance(row[0]
-00009ba0: 2c20 286c 6f6e 672c 2069 6e74 2929 2020  , (long, int))  
-00009bb0: 2320 6e6f 7161 0a0a 0a63 6c61 7373 205f  # noqa...class _
-00009bc0: 556e 6963 6f64 6546 6978 7475 7265 285f  UnicodeFixture(_
-00009bd0: 5f55 6e69 636f 6465 4669 7874 7572 6529  _UnicodeFixture)
-00009be0: 3a0a 2020 2020 4063 6c61 7373 6d65 7468  :.    @classmeth
-00009bf0: 6f64 0a20 2020 2064 6566 2064 6566 696e  od.    def defin
-00009c00: 655f 7461 626c 6573 2863 6c73 2c20 6d65  e_tables(cls, me
-00009c10: 7461 6461 7461 293a 0a20 2020 2020 2020  tadata):.       
-00009c20: 2022 2222 0a20 2020 2020 2020 2053 5041   """.        SPA
-00009c30: 4e4e 4552 204f 5645 5252 4944 453a 0a0a  NNER OVERRIDE:..
-00009c40: 2020 2020 2020 2020 436c 6f75 6420 5370          Cloud Sp
-00009c50: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
-00009c60: 7070 6f72 7420 6175 746f 2069 6e63 7265  pport auto incre
-00009c70: 6d65 6e74 696e 6720 6964 7320 6665 6174  menting ids feat
-00009c80: 7572 652c 0a20 2020 2020 2020 2077 6869  ure,.        whi
-00009c90: 6368 2069 7320 7573 6564 2062 7920 7468  ch is used by th
-00009ca0: 6520 6f72 6967 696e 616c 2074 6573 742e  e original test.
-00009cb0: 204f 7665 7272 6964 696e 6720 7468 6520   Overriding the 
-00009cc0: 7465 7374 2064 6174 610a 2020 2020 2020  test data.      
-00009cd0: 2020 6372 6561 7469 6f6e 206d 6574 686f    creation metho
-00009ce0: 6420 746f 2064 6973 6162 6c65 2061 7574  d to disable aut
-00009cf0: 6f69 6e63 7265 6d65 6e74 2061 6e64 206d  oincrement and m
-00009d00: 616b 6520 6964 2063 6f6c 756d 6e0a 2020  ake id column.  
-00009d10: 2020 2020 2020 6e75 6c6c 6162 6c65 2e0a        nullable..
-00009d20: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00009d30: 2020 2020 5461 626c 6528 0a20 2020 2020      Table(.     
-00009d40: 2020 2020 2020 2022 756e 6963 6f64 655f         "unicode_
-00009d50: 7461 626c 6522 2c0a 2020 2020 2020 2020  table",.        
-00009d60: 2020 2020 6d65 7461 6461 7461 2c0a 2020      metadata,.  
-00009d70: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
-00009d80: 2822 6964 222c 2049 6e74 6567 6572 2c20  ("id", Integer, 
-00009d90: 7072 696d 6172 795f 6b65 793d 5472 7565  primary_key=True
-00009da0: 2c20 6e75 6c6c 6162 6c65 3d54 7275 6529  , nullable=True)
-00009db0: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
-00009dc0: 6c75 6d6e 2822 756e 6963 6f64 655f 6461  lumn("unicode_da
-00009dd0: 7461 222c 2063 6c73 2e64 6174 6174 7970  ta", cls.datatyp
-00009de0: 6529 2c0a 2020 2020 2020 2020 290a 0a20  e),.        ).. 
-00009df0: 2020 2064 6566 2074 6573 745f 726f 756e     def test_roun
-00009e00: 645f 7472 6970 5f65 7865 6375 7465 6d61  d_trip_executema
-00009e10: 6e79 2873 656c 6629 3a0a 2020 2020 2020  ny(self):.      
-00009e20: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
-00009e30: 414e 4e45 5220 4f56 4552 5249 4445 0a0a  ANNER OVERRIDE..
-00009e40: 2020 2020 2020 2020 436c 6f75 6420 5370          Cloud Sp
-00009e50: 616e 6e65 7220 7375 7070 6f72 7473 2074  anner supports t
-00009e60: 6162 6c65 7320 7769 7468 2065 6d70 7479  ables with empty
-00009e70: 2070 7269 6d61 7279 206b 6579 2c20 6275   primary key, bu
-00009e80: 740a 2020 2020 2020 2020 6f6e 6c79 2073  t.        only s
-00009e90: 696e 676c 6520 6f6e 6520 726f 7720 6361  ingle one row ca
-00009ea0: 6e20 6265 2069 6e73 6572 7465 6420 696e  n be inserted in
-00009eb0: 746f 2073 7563 6820 6120 7461 626c 6520  to such a table 
-00009ec0: 2d0a 2020 2020 2020 2020 666f 6c6c 6f77  -.        follow
-00009ed0: 696e 6720 696e 7365 7274 696f 6e73 2077  ing insertions w
-00009ee0: 696c 6c20 6661 696c 2077 6974 6820 6052  ill fail with `R
-00009ef0: 6f77 205b 5d20 616c 7265 6164 7920 6578  ow [] already ex
-00009f00: 6973 7473 222e 0a20 2020 2020 2020 204f  ists"..        O
-00009f10: 7665 7272 6964 696e 6720 7468 6520 7465  verriding the te
-00009f20: 7374 2074 6f20 6176 6f69 6420 7468 6520  st to avoid the 
-00009f30: 7361 6d65 2066 6169 6c75 7265 2e0a 2020  same failure..  
-00009f40: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00009f50: 2020 756e 6963 6f64 655f 7461 626c 6520    unicode_table 
-00009f60: 3d20 7365 6c66 2e74 6162 6c65 732e 756e  = self.tables.un
-00009f70: 6963 6f64 655f 7461 626c 650a 0a20 2020  icode_table..   
-00009f80: 2020 2020 2063 6f6e 6669 672e 6462 2e65       config.db.e
-00009f90: 7865 6375 7465 280a 2020 2020 2020 2020  xecute(.        
-00009fa0: 2020 2020 756e 6963 6f64 655f 7461 626c      unicode_tabl
-00009fb0: 652e 696e 7365 7274 2829 2c0a 2020 2020  e.insert(),.    
-00009fc0: 2020 2020 2020 2020 5b7b 2269 6422 3a20          [{"id": 
-00009fd0: 692c 2022 756e 6963 6f64 655f 6461 7461  i, "unicode_data
-00009fe0: 223a 2073 656c 662e 6461 7461 7d20 666f  ": self.data} fo
-00009ff0: 7220 6920 696e 2072 616e 6765 2833 295d  r i in range(3)]
-0000a000: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-0000a010: 2020 2020 2072 6f77 7320 3d20 636f 6e66       rows = conf
-0000a020: 6967 2e64 622e 6578 6563 7574 6528 7365  ig.db.execute(se
-0000a030: 6c65 6374 285b 756e 6963 6f64 655f 7461  lect([unicode_ta
-0000a040: 626c 652e 632e 756e 6963 6f64 655f 6461  ble.c.unicode_da
-0000a050: 7461 5d29 292e 6665 7463 6861 6c6c 2829  ta])).fetchall()
-0000a060: 0a20 2020 2020 2020 2065 715f 2872 6f77  .        eq_(row
-0000a070: 732c 205b 2873 656c 662e 6461 7461 2c29  s, [(self.data,)
-0000a080: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-0000a090: 3329 5d29 0a20 2020 2020 2020 2066 6f72  3)]).        for
-0000a0a0: 2072 6f77 2069 6e20 726f 7773 3a0a 2020   row in rows:.  
-0000a0b0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-0000a0c0: 2069 7369 6e73 7461 6e63 6528 726f 775b   isinstance(row[
-0000a0d0: 305d 2c20 7574 696c 2e74 6578 745f 7479  0], util.text_ty
-0000a0e0: 7065 290a 0a20 2020 2040 7079 7465 7374  pe)..    @pytest
-0000a0f0: 2e6d 6172 6b2e 736b 6970 2822 5370 616e  .mark.skip("Span
-0000a100: 6e65 7220 646f 6573 6e27 7420 7375 7070  ner doesn't supp
-0000a110: 6f72 7420 6e6f 6e2d 6173 6369 6920 6368  ort non-ascii ch
-0000a120: 6172 6163 7465 7273 2229 0a20 2020 2064  aracters").    d
-0000a130: 6566 2074 6573 745f 6c69 7465 7261 6c28  ef test_literal(
-0000a140: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-0000a150: 6173 730a 0a20 2020 2040 7079 7465 7374  ass..    @pytest
-0000a160: 2e6d 6172 6b2e 736b 6970 2822 5370 616e  .mark.skip("Span
-0000a170: 6e65 7220 646f 6573 6e27 7420 7375 7070  ner doesn't supp
-0000a180: 6f72 7420 6e6f 6e2d 6173 6369 6920 6368  ort non-ascii ch
-0000a190: 6172 6163 7465 7273 2229 0a20 2020 2064  aracters").    d
-0000a1a0: 6566 2074 6573 745f 6c69 7465 7261 6c5f  ef test_literal_
-0000a1b0: 6e6f 6e5f 6173 6369 6928 7365 6c66 293a  non_ascii(self):
-0000a1c0: 0a20 2020 2020 2020 2070 6173 730a 0a0a  .        pass...
-0000a1d0: 636c 6173 7320 556e 6963 6f64 6556 6172  class UnicodeVar
-0000a1e0: 6368 6172 5465 7374 285f 556e 6963 6f64  charTest(_Unicod
-0000a1f0: 6546 6978 7475 7265 2c20 5f55 6e69 636f  eFixture, _Unico
-0000a200: 6465 5661 7263 6861 7254 6573 7429 3a0a  deVarcharTest):.
-0000a210: 2020 2020 2222 220a 2020 2020 5350 414e      """.    SPAN
-0000a220: 4e45 5220 4f56 4552 5249 4445 3a0a 0a20  NER OVERRIDE:.. 
-0000a230: 2020 2055 6e69 636f 6465 5661 7263 6861     UnicodeVarcha
-0000a240: 7254 6573 7420 636c 6173 7320 696e 6865  rTest class inhe
-0000a250: 7269 7473 2074 6865 205f 5f55 6e69 636f  rits the __Unico
-0000a260: 6465 4669 7874 7572 6520 636c 6173 7327  deFixture class'
-0000a270: 7320 7465 7374 732c 0a20 2020 2073 6f20  s tests,.    so 
-0000a280: 746f 2061 766f 6964 2074 686f 7365 2066  to avoid those f
-0000a290: 6169 6c75 7265 7320 616e 6420 6d61 696e  ailures and main
-0000a2a0: 7461 696e 2044 5259 2063 6f6e 6365 7074  tain DRY concept
-0000a2b0: 206a 7573 7420 696e 6865 7269 7420 7468   just inherit th
-0000a2c0: 6520 636c 6173 7320 746f 2072 756e 0a20  e class to run. 
-0000a2d0: 2020 2074 6573 7473 2073 7563 6365 7373     tests success
-0000a2e0: 6675 6c6c 792e 0a20 2020 2022 2222 0a0a  fully..    """..
-0000a2f0: 2020 2020 7061 7373 0a0a 0a63 6c61 7373      pass...class
-0000a300: 2055 6e69 636f 6465 5465 7874 5465 7374   UnicodeTextTest
-0000a310: 285f 556e 6963 6f64 6546 6978 7475 7265  (_UnicodeFixture
-0000a320: 2c20 5f55 6e69 636f 6465 5465 7874 5465  , _UnicodeTextTe
-0000a330: 7374 293a 0a20 2020 2022 2222 0a20 2020  st):.    """.   
-0000a340: 2053 5041 4e4e 4552 204f 5645 5252 4944   SPANNER OVERRID
-0000a350: 453a 0a0a 2020 2020 556e 6963 6f64 6554  E:..    UnicodeT
-0000a360: 6578 7454 6573 7420 636c 6173 7320 696e  extTest class in
-0000a370: 6865 7269 7473 2074 6865 205f 5f55 6e69  herits the __Uni
-0000a380: 636f 6465 4669 7874 7572 6520 636c 6173  codeFixture clas
-0000a390: 7327 7320 7465 7374 732c 0a20 2020 2073  s's tests,.    s
-0000a3a0: 6f20 746f 2061 766f 6964 2074 686f 7365  o to avoid those
-0000a3b0: 2066 6169 6c75 7265 7320 616e 6420 6d61   failures and ma
-0000a3c0: 696e 7461 696e 2044 5259 2063 6f6e 6365  intain DRY conce
-0000a3d0: 7074 206a 7573 7420 696e 6865 7269 7420  pt just inherit 
-0000a3e0: 7468 6520 636c 6173 7320 746f 2072 756e  the class to run
-0000a3f0: 0a20 2020 2074 6573 7473 2073 7563 6365  .    tests succe
-0000a400: 7373 6675 6c6c 792e 0a20 2020 2022 2222  ssfully..    """
-0000a410: 0a0a 2020 2020 7061 7373 0a0a 0a63 6c61  ..    pass...cla
-0000a420: 7373 2052 6f77 4665 7463 6854 6573 7428  ss RowFetchTest(
-0000a430: 5f52 6f77 4665 7463 6854 6573 7429 3a0a  _RowFetchTest):.
-0000a440: 2020 2020 6465 6620 7465 7374 5f72 6f77      def test_row
-0000a450: 5f77 5f73 6361 6c61 725f 7365 6c65 6374  _w_scalar_select
-0000a460: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000a470: 2222 220a 2020 2020 2020 2020 5350 414e  """.        SPAN
-0000a480: 4e45 5220 4f56 4552 5249 4445 3a0a 0a20  NER OVERRIDE:.. 
-0000a490: 2020 2020 2020 2043 6c6f 7564 2053 7061         Cloud Spa
-0000a4a0: 6e6e 6572 2072 6574 7572 6e73 2061 2044  nner returns a D
-0000a4b0: 6174 6574 696d 6557 6974 684e 616e 6f73  atetimeWithNanos
-0000a4c0: 6563 6f6e 6473 2829 2066 6f72 2064 6174  econds() for dat
-0000a4d0: 650a 2020 2020 2020 2020 6461 7461 2074  e.        data t
-0000a4e0: 7970 6573 2e20 4f76 6572 7269 6469 6e67  ypes. Overriding
-0000a4f0: 2074 6865 2074 6573 7420 746f 2075 7365   the test to use
-0000a500: 2061 2044 6174 6574 696d 6557 6974 684e   a DatetimeWithN
-0000a510: 616e 6f73 6563 6f6e 6473 0a20 2020 2020  anoseconds.     
-0000a520: 2020 2074 7970 6520 7661 6c75 6520 6173     type value as
-0000a530: 2061 6e20 6578 7065 6374 6564 2072 6573   an expected res
-0000a540: 756c 742e 0a20 2020 2020 2020 202d 2d2d  ult..        ---
-0000a550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020  -----------..   
-0000a560: 2020 2020 2074 6573 7420 7468 6174 2061       test that a
-0000a570: 2073 6361 6c61 7220 7365 6c65 6374 2061   scalar select a
-0000a580: 7320 6120 636f 6c75 6d6e 2069 7320 7265  s a column is re
-0000a590: 7475 726e 6564 2061 7320 7375 6368 0a20  turned as such. 
-0000a5a0: 2020 2020 2020 2061 6e64 2074 6861 7420         and that 
-0000a5b0: 7479 7065 2063 6f6e 7665 7273 696f 6e20  type conversion 
-0000a5c0: 776f 726b 7320 4f4b 2e0a 0a20 2020 2020  works OK...     
-0000a5d0: 2020 2028 7468 6973 2069 7320 6861 6c66     (this is half
-0000a5e0: 2061 2053 514c 416c 6368 656d 7920 436f   a SQLAlchemy Co
-0000a5f0: 7265 2074 6573 7420 616e 6420 6861 6c66  re test and half
-0000a600: 2074 6f20 6361 7463 6820 6461 7461 6261   to catch databa
-0000a610: 7365 0a20 2020 2020 2020 2062 6163 6b65  se.        backe
-0000a620: 6e64 7320 7468 6174 206d 6179 2068 6176  nds that may hav
-0000a630: 6520 756e 7573 7561 6c20 6265 6861 7669  e unusual behavi
-0000a640: 6f72 2077 6974 6820 7363 616c 6172 2073  or with scalar s
-0000a650: 656c 6563 7473 2e29 0a20 2020 2020 2020  elects.).       
-0000a660: 2022 2222 0a20 2020 2020 2020 2064 6174   """.        dat
-0000a670: 6574 6162 6c65 203d 2073 656c 662e 7461  etable = self.ta
-0000a680: 626c 6573 2e68 6173 5f64 6174 6573 0a20  bles.has_dates. 
-0000a690: 2020 2020 2020 2073 203d 2073 656c 6563         s = selec
-0000a6a0: 7428 5b64 6174 6574 6162 6c65 2e61 6c69  t([datetable.ali
-0000a6b0: 6173 2822 7822 292e 632e 746f 6461 795d  as("x").c.today]
-0000a6c0: 292e 7363 616c 6172 5f73 7562 7175 6572  ).scalar_subquer
-0000a6d0: 7928 290a 2020 2020 2020 2020 7332 203d  y().        s2 =
-0000a6e0: 2073 656c 6563 7428 5b64 6174 6574 6162   select([datetab
-0000a6f0: 6c65 2e63 2e69 642c 2073 2e6c 6162 656c  le.c.id, s.label
-0000a700: 2822 736f 6d65 6c61 6265 6c22 295d 290a  ("somelabel")]).
-0000a710: 2020 2020 2020 2020 726f 7720 3d20 636f          row = co
-0000a720: 6e66 6967 2e64 622e 6578 6563 7574 6528  nfig.db.execute(
-0000a730: 7332 292e 6669 7273 7428 290a 0a20 2020  s2).first()..   
-0000a740: 2020 2020 2065 715f 280a 2020 2020 2020       eq_(.      
-0000a750: 2020 2020 2020 726f 775b 2273 6f6d 656c        row["somel
-0000a760: 6162 656c 225d 2c0a 2020 2020 2020 2020  abel"],.        
-0000a770: 2020 2020 4461 7465 7469 6d65 5769 7468      DatetimeWith
-0000a780: 4e61 6e6f 7365 636f 6e64 7328 3230 3036  Nanoseconds(2006
-0000a790: 2c20 352c 2031 322c 2031 322c 2030 2c20  , 5, 12, 12, 0, 
-0000a7a0: 302c 2074 7a69 6e66 6f3d 7469 6d65 7a6f  0, tzinfo=timezo
-0000a7b0: 6e65 2e75 7463 292c 0a20 2020 2020 2020  ne.utc),.       
-0000a7c0: 2029 0a0a 0a63 6c61 7373 2049 6e73 6572   )...class Inser
-0000a7d0: 7442 6568 6176 696f 7254 6573 7428 5f49  tBehaviorTest(_I
-0000a7e0: 6e73 6572 7442 6568 6176 696f 7254 6573  nsertBehaviorTes
-0000a7f0: 7429 3a0a 2020 2020 4070 7974 6573 742e  t):.    @pytest.
-0000a800: 6d61 726b 2e73 6b69 7028 2253 7061 6e6e  mark.skip("Spann
-0000a810: 6572 2064 6f65 736e 2774 2073 7570 706f  er doesn't suppo
-0000a820: 7274 2065 6d70 7479 2069 6e73 6572 7473  rt empty inserts
-0000a830: 2229 0a20 2020 2064 6566 2074 6573 745f  ").    def test_
-0000a840: 656d 7074 795f 696e 7365 7274 2873 656c  empty_insert(sel
-0000a850: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-0000a860: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
-0000a870: 726b 2e73 6b69 7028 2253 7061 6e6e 6572  rk.skip("Spanner
-0000a880: 2064 6f65 736e 2774 2073 7570 706f 7274   doesn't support
-0000a890: 2065 6d70 7479 2069 6e73 6572 7473 2229   empty inserts")
-0000a8a0: 0a20 2020 2064 6566 2074 6573 745f 656d  .    def test_em
-0000a8b0: 7074 795f 696e 7365 7274 5f6d 756c 7469  pty_insert_multi
-0000a8c0: 706c 6528 7365 6c66 293a 0a20 2020 2020  ple(self):.     
-0000a8d0: 2020 2070 6173 730a 0a20 2020 2040 7079     pass..    @py
-0000a8e0: 7465 7374 2e6d 6172 6b2e 736b 6970 2822  test.mark.skip("
-0000a8f0: 5370 616e 6e65 7220 646f 6573 6e27 7420  Spanner doesn't 
-0000a900: 7375 7070 6f72 7420 6175 746f 2069 6e63  support auto inc
-0000a910: 7265 6d65 6e74 2229 0a20 2020 2064 6566  rement").    def
-0000a920: 2074 6573 745f 696e 7365 7274 5f66 726f   test_insert_fro
-0000a930: 6d5f 7365 6c65 6374 5f61 7574 6f69 6e63  m_select_autoinc
-0000a940: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000a950: 7061 7373 0a0a 2020 2020 6465 6620 7465  pass..    def te
-0000a960: 7374 5f61 7574 6f63 6c6f 7365 5f6f 6e5f  st_autoclose_on_
-0000a970: 696e 7365 7274 2873 656c 6629 3a0a 2020  insert(self):.  
-0000a980: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000a990: 2020 5350 414e 4e45 5220 4f56 4552 5249    SPANNER OVERRI
-0000a9a0: 4445 3a0a 0a20 2020 2020 2020 2043 6c6f  DE:..        Clo
-0000a9b0: 7564 2053 7061 6e6e 6572 2064 6f65 736e  ud Spanner doesn
-0000a9c0: 2774 2073 7570 706f 7274 2074 6162 6c65  't support table
-0000a9d0: 7320 7769 7468 2061 6e20 6175 746f 2069  s with an auto i
-0000a9e0: 6e63 7265 6d65 6e74 2070 7269 6d61 7279  ncrement primary
-0000a9f0: 206b 6579 2c0a 2020 2020 2020 2020 666f   key,.        fo
-0000aa00: 6c6c 6f77 696e 6720 696e 7365 7274 696f  llowing insertio
-0000aa10: 6e73 2077 696c 6c20 6661 696c 2077 6974  ns will fail wit
-0000aa20: 6820 6034 3030 2069 6420 6d75 7374 206e  h `400 id must n
-0000aa30: 6f74 2062 6520 4e55 4c4c 2069 6e20 7461  ot be NULL in ta
-0000aa40: 626c 650a 2020 2020 2020 2020 6175 746f  ble.        auto
-0000aa50: 696e 635f 706b 602e 0a0a 2020 2020 2020  inc_pk`...      
-0000aa60: 2020 4f76 6572 7269 6469 6e67 2074 6865    Overriding the
-0000aa70: 2074 6573 7473 2061 6e64 2061 6464 696e   tests and addin
-0000aa80: 6720 6120 6d61 6e75 616c 2070 7269 6d61  g a manual prima
-0000aa90: 7279 206b 6579 2076 616c 7565 2074 6f20  ry key value to 
-0000aaa0: 6176 6f69 6420 7468 6520 7361 6d65 0a20  avoid the same. 
-0000aab0: 2020 2020 2020 2066 6169 6c75 7265 732e         failures.
-0000aac0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000aad0: 2020 2020 2069 6620 636f 6e66 6967 2e72       if config.r
-0000aae0: 6571 7569 7265 6d65 6e74 732e 7265 7475  equirements.retu
-0000aaf0: 726e 696e 672e 656e 6162 6c65 643a 0a20  rning.enabled:. 
-0000ab00: 2020 2020 2020 2020 2020 2065 6e67 696e             engin
-0000ab10: 6520 3d20 656e 6769 6e65 732e 7465 7374  e = engines.test
-0000ab20: 696e 675f 656e 6769 6e65 286f 7074 696f  ing_engine(optio
-0000ab30: 6e73 3d7b 2269 6d70 6c69 6369 745f 7265  ns={"implicit_re
-0000ab40: 7475 726e 696e 6722 3a20 4661 6c73 657d  turning": False}
-0000ab50: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0000ab60: 2020 2020 2020 2020 2020 2020 656e 6769              engi
-0000ab70: 6e65 203d 2063 6f6e 6669 672e 6462 0a0a  ne = config.db..
-0000ab80: 2020 2020 2020 2020 7769 7468 2065 6e67          with eng
-0000ab90: 696e 652e 6265 6769 6e28 2920 6173 2063  ine.begin() as c
-0000aba0: 6f6e 6e3a 0a20 2020 2020 2020 2020 2020  onn:.           
-0000abb0: 2072 203d 2063 6f6e 6e2e 6578 6563 7574   r = conn.execut
-0000abc0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-0000abd0: 2020 2073 656c 662e 7461 626c 6573 2e61     self.tables.a
-0000abe0: 7574 6f69 6e63 5f70 6b2e 696e 7365 7274  utoinc_pk.insert
-0000abf0: 2829 2c20 6469 6374 2869 643d 312c 2064  (), dict(id=1, d
-0000ac00: 6174 613d 2273 6f6d 6520 6461 7461 2229  ata="some data")
-0000ac10: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-0000ac20: 2020 2020 2020 2020 6173 7365 7274 2072          assert r
-0000ac30: 2e5f 736f 6674 5f63 6c6f 7365 640a 2020  ._soft_closed.  
-0000ac40: 2020 2020 2020 6173 7365 7274 206e 6f74        assert not
-0000ac50: 2072 2e63 6c6f 7365 640a 2020 2020 2020   r.closed.      
-0000ac60: 2020 6173 7365 7274 2072 2e69 735f 696e    assert r.is_in
-0000ac70: 7365 7274 0a20 2020 2020 2020 2061 7373  sert.        ass
-0000ac80: 6572 7420 6e6f 7420 722e 7265 7475 726e  ert not r.return
-0000ac90: 735f 726f 7773 0a0a 0a63 6c61 7373 2042  s_rows...class B
-0000aca0: 7974 6573 5465 7374 285f 4c69 7465 7261  ytesTest(_Litera
-0000acb0: 6c52 6f75 6e64 5472 6970 4669 7874 7572  lRoundTripFixtur
-0000acc0: 652c 2066 6978 7475 7265 732e 5465 7374  e, fixtures.Test
-0000acd0: 4261 7365 293a 0a20 2020 205f 5f62 6163  Base):.    __bac
-0000ace0: 6b65 6e64 5f5f 203d 2054 7275 650a 0a20  kend__ = True.. 
-0000acf0: 2020 2064 6566 2074 6573 745f 6e6f 6c65     def test_nole
-0000ad00: 6e67 7468 5f62 696e 6172 7928 7365 6c66  ngth_binary(self
-0000ad10: 293a 0a20 2020 2020 2020 206d 6574 6164  ):.        metad
-0000ad20: 6174 6120 3d20 4d65 7461 4461 7461 2829  ata = MetaData()
-0000ad30: 0a20 2020 2020 2020 2066 6f6f 203d 2054  .        foo = T
-0000ad40: 6162 6c65 2822 666f 6f22 2c20 6d65 7461  able("foo", meta
-0000ad50: 6461 7461 2c20 436f 6c75 6d6e 2822 6f6e  data, Column("on
-0000ad60: 6522 2c20 4c61 7267 6542 696e 6172 7929  e", LargeBinary)
-0000ad70: 290a 0a20 2020 2020 2020 2066 6f6f 2e63  )..        foo.c
-0000ad80: 7265 6174 6528 636f 6e66 6967 2e64 6229  reate(config.db)
-0000ad90: 0a20 2020 2020 2020 2066 6f6f 2e64 726f  .        foo.dro
-0000ada0: 7028 636f 6e66 6967 2e64 6229 0a0a 0a63  p(config.db)...c
-0000adb0: 6c61 7373 2053 7472 696e 6754 6573 7428  lass StringTest(
-0000adc0: 5f53 7472 696e 6754 6573 7429 3a0a 2020  _StringTest):.  
-0000add0: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
-0000ade0: 6b69 7028 2253 7061 6e6e 6572 2064 6f65  kip("Spanner doe
-0000adf0: 736e 2774 2073 7570 706f 7274 206e 6f6e  sn't support non
-0000ae00: 2d61 7363 6969 2063 6861 7261 6374 6572  -ascii character
-0000ae10: 7322 290a 2020 2020 6465 6620 7465 7374  s").    def test
-0000ae20: 5f6c 6974 6572 616c 5f6e 6f6e 5f61 7363  _literal_non_asc
-0000ae30: 6969 2873 656c 6629 3a0a 2020 2020 2020  ii(self):.      
-0000ae40: 2020 7061 7373 0a0a 0a63 6c61 7373 2054    pass...class T
-0000ae50: 6578 7454 6573 7428 5f54 6578 7454 6573  extTest(_TextTes
-0000ae60: 7429 3a0a 2020 2020 4063 6c61 7373 6d65  t):.    @classme
-0000ae70: 7468 6f64 0a20 2020 2064 6566 2064 6566  thod.    def def
-0000ae80: 696e 655f 7461 626c 6573 2863 6c73 2c20  ine_tables(cls, 
-0000ae90: 6d65 7461 6461 7461 293a 0a20 2020 2020  metadata):.     
-0000aea0: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
-0000aeb0: 5041 4e4e 4552 204f 5645 5252 4944 453a  PANNER OVERRIDE:
-0000aec0: 0a0a 2020 2020 2020 2020 436c 6f75 6420  ..        Cloud 
-0000aed0: 5370 616e 6e65 7220 646f 6573 6e27 7420  Spanner doesn't 
-0000aee0: 7375 7070 6f72 7420 6175 746f 2069 6e63  support auto inc
-0000aef0: 7265 6d65 6e74 696e 6720 6964 7320 6665  rementing ids fe
-0000af00: 6174 7572 652c 0a20 2020 2020 2020 2077  ature,.        w
-0000af10: 6869 6368 2069 7320 7573 6564 2062 7920  hich is used by 
-0000af20: 7468 6520 6f72 6967 696e 616c 2074 6573  the original tes
-0000af30: 742e 204f 7665 7272 6964 696e 6720 7468  t. Overriding th
-0000af40: 6520 7465 7374 2064 6174 610a 2020 2020  e test data.    
-0000af50: 2020 2020 6372 6561 7469 6f6e 206d 6574      creation met
-0000af60: 686f 6420 746f 2064 6973 6162 6c65 2061  hod to disable a
-0000af70: 7574 6f69 6e63 7265 6d65 6e74 2061 6e64  utoincrement and
-0000af80: 206d 616b 6520 6964 2063 6f6c 756d 6e0a   make id column.
-0000af90: 2020 2020 2020 2020 6e75 6c6c 6162 6c65          nullable
-0000afa0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000afb0: 2020 2020 2020 5461 626c 6528 0a20 2020        Table(.   
-0000afc0: 2020 2020 2020 2020 2022 7465 7874 5f74           "text_t
-0000afd0: 6162 6c65 222c 0a20 2020 2020 2020 2020  able",.         
-0000afe0: 2020 206d 6574 6164 6174 612c 0a20 2020     metadata,.   
-0000aff0: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-0000b000: 2269 6422 2c20 496e 7465 6765 722c 2070  "id", Integer, p
-0000b010: 7269 6d61 7279 5f6b 6579 3d54 7275 652c  rimary_key=True,
-0000b020: 206e 756c 6c61 626c 653d 5472 7565 292c   nullable=True),
-0000b030: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
-0000b040: 756d 6e28 2274 6578 745f 6461 7461 222c  umn("text_data",
-0000b050: 2054 6578 7429 2c0a 2020 2020 2020 2020   Text),.        
-0000b060: 290a 0a20 2020 2040 7079 7465 7374 2e6d  )..    @pytest.m
-0000b070: 6172 6b2e 736b 6970 2822 5370 616e 6e65  ark.skip("Spanne
-0000b080: 7220 646f 6573 6e27 7420 7375 7070 6f72  r doesn't suppor
-0000b090: 7420 6e6f 6e2d 6173 6369 6920 6368 6172  t non-ascii char
-0000b0a0: 6163 7465 7273 2229 0a20 2020 2064 6566  acters").    def
-0000b0b0: 2074 6573 745f 6c69 7465 7261 6c5f 6e6f   test_literal_no
-0000b0c0: 6e5f 6173 6369 6928 7365 6c66 293a 0a20  n_ascii(self):. 
-0000b0d0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-0000b0e0: 2040 7079 7465 7374 2e6d 6172 6b2e 736b   @pytest.mark.sk
-0000b0f0: 6970 2822 4e6f 7420 7375 7070 6f72 7465  ip("Not supporte
-0000b100: 6420 6279 2053 7061 6e6e 6572 2229 0a20  d by Spanner"). 
-0000b110: 2020 2064 6566 2074 6573 745f 7465 7874     def test_text
-0000b120: 5f72 6f75 6e64 7472 6970 2873 656c 662c  _roundtrip(self,
-0000b130: 2063 6f6e 6e65 6374 696f 6e29 3a0a 2020   connection):.  
-0000b140: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-0000b150: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
-0000b160: 7028 224e 6f74 2073 7570 706f 7274 6564  p("Not supported
-0000b170: 2062 7920 5370 616e 6e65 7222 290a 2020   by Spanner").  
-0000b180: 2020 6465 6620 7465 7374 5f74 6578 745f    def test_text_
-0000b190: 656d 7074 795f 7374 7269 6e67 7328 7365  empty_strings(se
-0000b1a0: 6c66 2c20 636f 6e6e 6563 7469 6f6e 293a  lf, connection):
-0000b1b0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-0000b1c0: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-0000b1d0: 736b 6970 2822 4e6f 7420 7375 7070 6f72  skip("Not suppor
-0000b1e0: 7465 6420 6279 2053 7061 6e6e 6572 2229  ted by Spanner")
-0000b1f0: 0a20 2020 2064 6566 2074 6573 745f 7465  .    def test_te
-0000b200: 7874 5f6e 756c 6c5f 7374 7269 6e67 7328  xt_null_strings(
-0000b210: 7365 6c66 2c20 636f 6e6e 6563 7469 6f6e  self, connection
-0000b220: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-0000b230: 0a0a 636c 6173 7320 4e75 6d65 7269 6354  ..class NumericT
-0000b240: 6573 7428 5f4e 756d 6572 6963 5465 7374  est(_NumericTest
-0000b250: 293a 0a20 2020 2040 7465 7374 696e 672e  ):.    @testing.
-0000b260: 6669 7874 7572 650a 2020 2020 6465 6620  fixture.    def 
-0000b270: 646f 5f6e 756d 6572 6963 5f74 6573 7428  do_numeric_test(
-0000b280: 7365 6c66 2c20 6d65 7461 6461 7461 2c20  self, metadata, 
-0000b290: 636f 6e6e 6563 7469 6f6e 293a 0a20 2020  connection):.   
-0000b2a0: 2020 2020 2040 7465 7374 696e 672e 656d       @testing.em
-0000b2b0: 6974 735f 7761 726e 696e 6728 7222 2e2a  its_warning(r".*
-0000b2c0: 646f 6573 205c 2a6e 6f74 5c2a 2073 7570  does \*not\* sup
-0000b2d0: 706f 7274 2044 6563 696d 616c 206f 626a  port Decimal obj
-0000b2e0: 6563 7473 206e 6174 6976 656c 7922 290a  ects natively").
-0000b2f0: 2020 2020 2020 2020 6465 6620 7275 6e28          def run(
-0000b300: 7479 7065 5f2c 2069 6e70 7574 5f2c 206f  type_, input_, o
-0000b310: 7574 7075 742c 2066 696c 7465 725f 3d4e  utput, filter_=N
-0000b320: 6f6e 652c 2063 6865 636b 5f73 6361 6c65  one, check_scale
-0000b330: 3d46 616c 7365 293a 0a20 2020 2020 2020  =False):.       
-0000b340: 2020 2020 2074 203d 2054 6162 6c65 280a       t = Table(.
-0000b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b360: 2274 222c 0a20 2020 2020 2020 2020 2020  "t",.           
-0000b370: 2020 2020 206d 6574 6164 6174 612c 0a20       metadata,. 
-0000b380: 2020 2020 2020 2020 2020 2020 2020 2043                 C
-0000b390: 6f6c 756d 6e28 2278 222c 2074 7970 655f  olumn("x", type_
-0000b3a0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000b3b0: 2020 2043 6f6c 756d 6e28 2269 6422 2c20     Column("id", 
-0000b3c0: 496e 7465 6765 722c 2070 7269 6d61 7279  Integer, primary
-0000b3d0: 5f6b 6579 3d54 7275 6529 2c0a 2020 2020  _key=True),.    
-0000b3e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000b3f0: 2020 2020 2020 742e 6372 6561 7465 2863        t.create(c
-0000b400: 6f6e 6e65 6374 696f 6e29 0a20 2020 2020  onnection).     
-0000b410: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
-0000b420: 6e2e 636f 6e6e 6563 7469 6f6e 2e63 6f6d  n.connection.com
-0000b430: 6d69 7428 290a 2020 2020 2020 2020 2020  mit().          
-0000b440: 2020 636f 6e6e 6563 7469 6f6e 2e65 7865    connection.exe
-0000b450: 6375 7465 280a 2020 2020 2020 2020 2020  cute(.          
-0000b460: 2020 2020 2020 742e 696e 7365 7274 2829        t.insert()
-0000b470: 2c20 5b7b 2278 223a 2078 2c20 2269 6422  , [{"x": x, "id"
-0000b480: 3a20 697d 2066 6f72 2069 2c20 7820 696e  : i} for i, x in
-0000b490: 2065 6e75 6d65 7261 7465 2869 6e70 7574   enumerate(input
-0000b4a0: 5f29 5d0a 2020 2020 2020 2020 2020 2020  _)].            
-0000b4b0: 290a 0a20 2020 2020 2020 2020 2020 2072  )..            r
-0000b4c0: 6573 756c 7420 3d20 7b72 6f77 5b30 5d20  esult = {row[0] 
-0000b4d0: 666f 7220 726f 7720 696e 2063 6f6e 6e65  for row in conne
-0000b4e0: 6374 696f 6e2e 6578 6563 7574 6528 742e  ction.execute(t.
-0000b4f0: 7365 6c65 6374 2829 297d 0a20 2020 2020  select())}.     
-0000b500: 2020 2020 2020 206f 7574 7075 7420 3d20         output = 
-0000b510: 7365 7428 6f75 7470 7574 290a 2020 2020  set(output).    
-0000b520: 2020 2020 2020 2020 6966 2066 696c 7465          if filte
-0000b530: 725f 3a0a 2020 2020 2020 2020 2020 2020  r_:.            
-0000b540: 2020 2020 7265 7375 6c74 203d 2073 6574      result = set
-0000b550: 2866 696c 7465 725f 2878 2920 666f 7220  (filter_(x) for 
-0000b560: 7820 696e 2072 6573 756c 7429 0a20 2020  x in result).   
-0000b570: 2020 2020 2020 2020 2020 2020 206f 7574               out
-0000b580: 7075 7420 3d20 7365 7428 6669 6c74 6572  put = set(filter
-0000b590: 5f28 7829 2066 6f72 2078 2069 6e20 6f75  _(x) for x in ou
-0000b5a0: 7470 7574 290a 2020 2020 2020 2020 2020  tput).          
-0000b5b0: 2020 6571 5f28 7265 7375 6c74 2c20 6f75    eq_(result, ou
-0000b5c0: 7470 7574 290a 2020 2020 2020 2020 2020  tput).          
-0000b5d0: 2020 6966 2063 6865 636b 5f73 6361 6c65    if check_scale
-0000b5e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b5f0: 2020 6571 5f28 5b73 7472 2878 2920 666f    eq_([str(x) fo
-0000b600: 7220 7820 696e 2072 6573 756c 745d 2c20  r x in result], 
-0000b610: 5b73 7472 2878 2920 666f 7220 7820 696e  [str(x) for x in
-0000b620: 206f 7574 7075 745d 290a 0a20 2020 2020   output])..     
-0000b630: 2020 2072 6574 7572 6e20 7275 6e0a 0a20     return run.. 
-0000b640: 2020 2040 656d 6974 735f 7761 726e 696e     @emits_warnin
-0000b650: 6728 7222 2e2a 646f 6573 205c 2a6e 6f74  g(r".*does \*not
-0000b660: 5c2a 2073 7570 706f 7274 2044 6563 696d  \* support Decim
-0000b670: 616c 206f 626a 6563 7473 206e 6174 6976  al objects nativ
-0000b680: 656c 7922 290a 2020 2020 6465 6620 7465  ely").    def te
-0000b690: 7374 5f72 656e 6465 725f 6c69 7465 7261  st_render_litera
-0000b6a0: 6c5f 6e75 6d65 7269 6328 7365 6c66 2c20  l_numeric(self, 
-0000b6b0: 6c69 7465 7261 6c5f 726f 756e 645f 7472  literal_round_tr
-0000b6c0: 6970 293a 0a20 2020 2020 2020 2022 2222  ip):.        """
-0000b6d0: 0a20 2020 2020 2020 2053 5041 4e4e 4552  .        SPANNER
-0000b6e0: 204f 5645 5252 4944 453a 0a0a 2020 2020   OVERRIDE:..    
-0000b6f0: 2020 2020 436c 6f75 6420 5370 616e 6e65      Cloud Spanne
-0000b700: 7220 7375 7070 6f72 7473 2074 6162 6c65  r supports table
-0000b710: 7320 7769 7468 2061 6e20 656d 7074 7920  s with an empty 
-0000b720: 7072 696d 6172 7920 6b65 792c 2062 7574  primary key, but
-0000b730: 0a20 2020 2020 2020 206f 6e6c 7920 6120  .        only a 
-0000b740: 7369 6e67 6c65 2072 6f77 2063 616e 2062  single row can b
-0000b750: 6520 696e 7365 7274 6564 2069 6e74 6f20  e inserted into 
-0000b760: 7375 6368 2061 2074 6162 6c65 202d 0a20  such a table -. 
-0000b770: 2020 2020 2020 2066 6f6c 6c6f 7769 6e67         following
-0000b780: 2069 6e73 6572 7469 6f6e 7320 7769 6c6c   insertions will
-0000b790: 2066 6169 6c20 7769 7468 2060 526f 7720   fail with `Row 
-0000b7a0: 5b5d 2061 6c72 6561 6479 2065 7869 7374  [] already exist
-0000b7b0: 7322 2e0a 2020 2020 2020 2020 4f76 6572  s"..        Over
-0000b7c0: 7269 6469 6e67 2074 6865 2074 6573 7420  riding the test 
-0000b7d0: 746f 2061 766f 6964 2074 6865 2073 616d  to avoid the sam
-0000b7e0: 6520 6661 696c 7572 652e 0a20 2020 2020  e failure..     
-0000b7f0: 2020 2022 2222 0a20 2020 2020 2020 206c     """.        l
-0000b800: 6974 6572 616c 5f72 6f75 6e64 5f74 7269  iteral_round_tri
-0000b810: 7028 0a20 2020 2020 2020 2020 2020 204e  p(.            N
-0000b820: 756d 6572 6963 2870 7265 6369 7369 6f6e  umeric(precision
-0000b830: 3d38 2c20 7363 616c 653d 3429 2c0a 2020  =8, scale=4),.  
-0000b840: 2020 2020 2020 2020 2020 5b64 6563 696d            [decim
-0000b850: 616c 2e44 6563 696d 616c 2822 3135 2e37  al.Decimal("15.7
-0000b860: 3536 3322 295d 2c0a 2020 2020 2020 2020  563")],.        
-0000b870: 2020 2020 5b64 6563 696d 616c 2e44 6563      [decimal.Dec
-0000b880: 696d 616c 2822 3135 2e37 3536 3322 295d  imal("15.7563")]
-0000b890: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-0000b8a0: 2040 656d 6974 735f 7761 726e 696e 6728   @emits_warning(
-0000b8b0: 7222 2e2a 646f 6573 205c 2a6e 6f74 5c2a  r".*does \*not\*
-0000b8c0: 2073 7570 706f 7274 2044 6563 696d 616c   support Decimal
-0000b8d0: 206f 626a 6563 7473 206e 6174 6976 656c   objects nativel
-0000b8e0: 7922 290a 2020 2020 6465 6620 7465 7374  y").    def test
-0000b8f0: 5f72 656e 6465 725f 6c69 7465 7261 6c5f  _render_literal_
-0000b900: 6e75 6d65 7269 635f 6173 666c 6f61 7428  numeric_asfloat(
-0000b910: 7365 6c66 2c20 6c69 7465 7261 6c5f 726f  self, literal_ro
-0000b920: 756e 645f 7472 6970 293a 0a20 2020 2020  und_trip):.     
-0000b930: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
-0000b940: 5041 4e4e 4552 204f 5645 5252 4944 453a  PANNER OVERRIDE:
-0000b950: 0a0a 2020 2020 2020 2020 436c 6f75 6420  ..        Cloud 
-0000b960: 5370 616e 6e65 7220 7375 7070 6f72 7473  Spanner supports
-0000b970: 2074 6162 6c65 7320 7769 7468 2061 6e20   tables with an 
-0000b980: 656d 7074 7920 7072 696d 6172 7920 6b65  empty primary ke
-0000b990: 792c 2062 7574 0a20 2020 2020 2020 206f  y, but.        o
-0000b9a0: 6e6c 7920 6120 7369 6e67 6c65 2072 6f77  nly a single row
-0000b9b0: 2063 616e 2062 6520 696e 7365 7274 6564   can be inserted
-0000b9c0: 2069 6e74 6f20 7375 6368 2061 2074 6162   into such a tab
-0000b9d0: 6c65 202d 0a20 2020 2020 2020 2066 6f6c  le -.        fol
-0000b9e0: 6c6f 7769 6e67 2069 6e73 6572 7469 6f6e  lowing insertion
-0000b9f0: 7320 7769 6c6c 2066 6169 6c20 7769 7468  s will fail with
-0000ba00: 2060 526f 7720 5b5d 2061 6c72 6561 6479   `Row [] already
-0000ba10: 2065 7869 7374 7322 2e0a 2020 2020 2020   exists"..      
-0000ba20: 2020 4f76 6572 7269 6469 6e67 2074 6865    Overriding the
-0000ba30: 2074 6573 7420 746f 2061 766f 6964 2074   test to avoid t
-0000ba40: 6865 2073 616d 6520 6661 696c 7572 652e  he same failure.
-0000ba50: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000ba60: 2020 2020 206c 6974 6572 616c 5f72 6f75       literal_rou
-0000ba70: 6e64 5f74 7269 7028 0a20 2020 2020 2020  nd_trip(.       
-0000ba80: 2020 2020 204e 756d 6572 6963 2870 7265       Numeric(pre
-0000ba90: 6369 7369 6f6e 3d38 2c20 7363 616c 653d  cision=8, scale=
-0000baa0: 342c 2061 7364 6563 696d 616c 3d46 616c  4, asdecimal=Fal
-0000bab0: 7365 292c 0a20 2020 2020 2020 2020 2020  se),.           
-0000bac0: 205b 6465 6369 6d61 6c2e 4465 6369 6d61   [decimal.Decima
-0000bad0: 6c28 2231 352e 3735 3633 2229 5d2c 0a20  l("15.7563")],. 
-0000bae0: 2020 2020 2020 2020 2020 205b 3135 2e37             [15.7
-0000baf0: 3536 335d 2c0a 2020 2020 2020 2020 290a  563],.        ).
-0000bb00: 0a20 2020 2064 6566 2074 6573 745f 7265  .    def test_re
-0000bb10: 6e64 6572 5f6c 6974 6572 616c 5f66 6c6f  nder_literal_flo
-0000bb20: 6174 2873 656c 662c 206c 6974 6572 616c  at(self, literal
-0000bb30: 5f72 6f75 6e64 5f74 7269 7029 3a0a 2020  _round_trip):.  
-0000bb40: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000bb50: 2020 5350 414e 4e45 5220 4f56 4552 5249    SPANNER OVERRI
-0000bb60: 4445 3a0a 0a20 2020 2020 2020 2043 6c6f  DE:..        Clo
-0000bb70: 7564 2053 7061 6e6e 6572 2073 7570 706f  ud Spanner suppo
-0000bb80: 7274 7320 7461 626c 6573 2077 6974 6820  rts tables with 
-0000bb90: 616e 2065 6d70 7479 2070 7269 6d61 7279  an empty primary
-0000bba0: 206b 6579 2c20 6275 740a 2020 2020 2020   key, but.      
-0000bbb0: 2020 6f6e 6c79 2061 2073 696e 676c 6520    only a single 
-0000bbc0: 726f 7720 6361 6e20 6265 2069 6e73 6572  row can be inser
-0000bbd0: 7465 6420 696e 746f 2073 7563 6820 6120  ted into such a 
-0000bbe0: 7461 626c 6520 2d0a 2020 2020 2020 2020  table -.        
-0000bbf0: 666f 6c6c 6f77 696e 6720 696e 7365 7274  following insert
-0000bc00: 696f 6e73 2077 696c 6c20 6661 696c 2077  ions will fail w
-0000bc10: 6974 6820 6052 6f77 205b 5d20 616c 7265  ith `Row [] alre
-0000bc20: 6164 7920 6578 6973 7473 222e 0a20 2020  ady exists"..   
-0000bc30: 2020 2020 204f 7665 7272 6964 696e 6720       Overriding 
-0000bc40: 7468 6520 7465 7374 2074 6f20 6176 6f69  the test to avoi
-0000bc50: 6420 7468 6520 7361 6d65 2066 6169 6c75  d the same failu
-0000bc60: 7265 2e0a 2020 2020 2020 2020 2222 220a  re..        """.
-0000bc70: 2020 2020 2020 2020 6c69 7465 7261 6c5f          literal_
-0000bc80: 726f 756e 645f 7472 6970 280a 2020 2020  round_trip(.    
-0000bc90: 2020 2020 2020 2020 466c 6f61 7428 3429          Float(4)
-0000bca0: 2c0a 2020 2020 2020 2020 2020 2020 5b64  ,.            [d
-0000bcb0: 6563 696d 616c 2e44 6563 696d 616c 2822  ecimal.Decimal("
-0000bcc0: 3135 2e37 3536 3322 295d 2c0a 2020 2020  15.7563")],.    
-0000bcd0: 2020 2020 2020 2020 5b31 352e 3735 3633          [15.7563
-0000bce0: 5d2c 0a20 2020 2020 2020 2020 2020 2066  ],.            f
-0000bcf0: 696c 7465 725f 3d6c 616d 6264 6120 6e3a  ilter_=lambda n:
-0000bd00: 206e 2069 7320 6e6f 7420 4e6f 6e65 2061   n is not None a
-0000bd10: 6e64 2072 6f75 6e64 286e 2c20 3529 206f  nd round(n, 5) o
-0000bd20: 7220 4e6f 6e65 2c0a 2020 2020 2020 2020  r None,.        
-0000bd30: 290a 0a20 2020 2040 7265 7175 6972 6573  )..    @requires
-0000bd40: 2e70 7265 6369 7369 6f6e 5f67 656e 6572  .precision_gener
-0000bd50: 6963 5f66 6c6f 6174 5f74 7970 650a 2020  ic_float_type.  
-0000bd60: 2020 6465 6620 7465 7374 5f66 6c6f 6174    def test_float
-0000bd70: 5f63 7573 746f 6d5f 7363 616c 6528 7365  _custom_scale(se
-0000bd80: 6c66 2c20 646f 5f6e 756d 6572 6963 5f74  lf, do_numeric_t
-0000bd90: 6573 7429 3a0a 2020 2020 2020 2020 2222  est):.        ""
-0000bda0: 220a 2020 2020 2020 2020 5350 414e 4e45  ".        SPANNE
-0000bdb0: 5220 4f56 4552 5249 4445 3a0a 0a20 2020  R OVERRIDE:..   
-0000bdc0: 2020 2020 2043 6c6f 7564 2053 7061 6e6e       Cloud Spann
-0000bdd0: 6572 2073 7570 706f 7274 7320 7461 626c  er supports tabl
-0000bde0: 6573 2077 6974 6820 616e 2065 6d70 7479  es with an empty
-0000bdf0: 2070 7269 6d61 7279 206b 6579 2c20 6275   primary key, bu
-0000be00: 740a 2020 2020 2020 2020 6f6e 6c79 2061  t.        only a
-0000be10: 2073 696e 676c 6520 726f 7720 6361 6e20   single row can 
-0000be20: 6265 2069 6e73 6572 7465 6420 696e 746f  be inserted into
-0000be30: 2073 7563 6820 6120 7461 626c 6520 2d0a   such a table -.
-0000be40: 2020 2020 2020 2020 666f 6c6c 6f77 696e          followin
-0000be50: 6720 696e 7365 7274 696f 6e73 2077 696c  g insertions wil
-0000be60: 6c20 6661 696c 2077 6974 6820 6052 6f77  l fail with `Row
-0000be70: 205b 5d20 616c 7265 6164 7920 6578 6973   [] already exis
-0000be80: 7473 222e 0a20 2020 2020 2020 204f 7665  ts"..        Ove
-0000be90: 7272 6964 696e 6720 7468 6520 7465 7374  rriding the test
-0000bea0: 2074 6f20 6176 6f69 6420 7468 6520 7361   to avoid the sa
-0000beb0: 6d65 2066 6169 6c75 7265 2e0a 2020 2020  me failure..    
-0000bec0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000bed0: 646f 5f6e 756d 6572 6963 5f74 6573 7428  do_numeric_test(
-0000bee0: 0a20 2020 2020 2020 2020 2020 2046 6c6f  .            Flo
-0000bef0: 6174 284e 6f6e 652c 2064 6563 696d 616c  at(None, decimal
-0000bf00: 5f72 6574 7572 6e5f 7363 616c 653d 372c  _return_scale=7,
-0000bf10: 2061 7364 6563 696d 616c 3d54 7275 6529   asdecimal=True)
-0000bf20: 2c0a 2020 2020 2020 2020 2020 2020 5b64  ,.            [d
-0000bf30: 6563 696d 616c 2e44 6563 696d 616c 2822  ecimal.Decimal("
-0000bf40: 3135 2e37 3536 3338 3237 2229 2c20 6465  15.7563827"), de
-0000bf50: 6369 6d61 6c2e 4465 6369 6d61 6c28 2231  cimal.Decimal("1
-0000bf60: 352e 3735 3633 3832 3722 295d 2c0a 2020  5.7563827")],.  
-0000bf70: 2020 2020 2020 2020 2020 5b64 6563 696d            [decim
-0000bf80: 616c 2e44 6563 696d 616c 2822 3135 2e37  al.Decimal("15.7
-0000bf90: 3536 3338 3237 2229 5d2c 0a20 2020 2020  563827")],.     
-0000bfa0: 2020 2020 2020 2063 6865 636b 5f73 6361         check_sca
-0000bfb0: 6c65 3d54 7275 652c 0a20 2020 2020 2020  le=True,.       
-0000bfc0: 2029 0a0a 2020 2020 6465 6620 7465 7374   )..    def test
-0000bfd0: 5f6e 756d 6572 6963 5f61 735f 6465 6369  _numeric_as_deci
-0000bfe0: 6d61 6c28 7365 6c66 2c20 646f 5f6e 756d  mal(self, do_num
-0000bff0: 6572 6963 5f74 6573 7429 3a0a 2020 2020  eric_test):.    
-0000c000: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000c010: 5350 414e 4e45 5220 4f56 4552 5249 4445  SPANNER OVERRIDE
-0000c020: 3a0a 0a20 2020 2020 2020 2053 7061 6e6e  :..        Spann
-0000c030: 6572 2074 6872 6f77 7320 616e 2065 7272  er throws an err
-0000c040: 6f72 2034 3030 2056 616c 7565 2068 6173  or 400 Value has
-0000c050: 2074 7970 6520 464c 4f41 5436 3420 7768   type FLOAT64 wh
-0000c060: 6963 6820 6361 6e6e 6f74 2062 650a 2020  ich cannot be.  
-0000c070: 2020 2020 2020 696e 7365 7274 6564 2069        inserted i
-0000c080: 6e74 6f20 636f 6c75 6d6e 2078 2c20 7768  nto column x, wh
-0000c090: 6963 6820 6861 7320 7479 7065 204e 554d  ich has type NUM
-0000c0a0: 4552 4943 2066 6f72 2076 616c 7565 2031  ERIC for value 1
-0000c0b0: 352e 3735 3633 2e0a 2020 2020 2020 2020  5.7563..        
-0000c0c0: 4f76 6572 7269 6469 6e67 2074 6865 2074  Overriding the t
-0000c0d0: 6573 7420 746f 2072 656d 6f76 6520 7468  est to remove th
-0000c0e0: 6520 6661 696c 7572 6520 6361 7365 2e0a  e failure case..
-0000c0f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000c100: 2020 2020 646f 5f6e 756d 6572 6963 5f74      do_numeric_t
-0000c110: 6573 7428 0a20 2020 2020 2020 2020 2020  est(.           
-0000c120: 204e 756d 6572 6963 2870 7265 6369 7369   Numeric(precisi
-0000c130: 6f6e 3d38 2c20 7363 616c 653d 3429 2c0a  on=8, scale=4),.
-0000c140: 2020 2020 2020 2020 2020 2020 5b64 6563              [dec
-0000c150: 696d 616c 2e44 6563 696d 616c 2822 3135  imal.Decimal("15
-0000c160: 2e37 3536 3322 292c 2064 6563 696d 616c  .7563"), decimal
-0000c170: 2e44 6563 696d 616c 2822 3135 2e37 3536  .Decimal("15.756
-0000c180: 3322 295d 2c0a 2020 2020 2020 2020 2020  3")],.          
-0000c190: 2020 5b64 6563 696d 616c 2e44 6563 696d    [decimal.Decim
-0000c1a0: 616c 2822 3135 2e37 3536 3322 295d 2c0a  al("15.7563")],.
-0000c1b0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-0000c1c0: 6566 2074 6573 745f 6e75 6d65 7269 635f  ef test_numeric_
-0000c1d0: 6173 5f66 6c6f 6174 2873 656c 662c 2064  as_float(self, d
-0000c1e0: 6f5f 6e75 6d65 7269 635f 7465 7374 293a  o_numeric_test):
-0000c1f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c200: 2020 2020 2053 5041 4e4e 4552 204f 5645       SPANNER OVE
-0000c210: 5252 4944 453a 0a0a 2020 2020 2020 2020  RRIDE:..        
-0000c220: 5370 616e 6e65 7220 7468 726f 7773 2061  Spanner throws a
-0000c230: 6e20 6572 726f 7220 3430 3020 5661 6c75  n error 400 Valu
-0000c240: 6520 6861 7320 7479 7065 2046 4c4f 4154  e has type FLOAT
-0000c250: 3634 2077 6869 6368 2063 616e 6e6f 7420  64 which cannot 
-0000c260: 6265 0a20 2020 2020 2020 2069 6e73 6572  be.        inser
-0000c270: 7465 6420 696e 746f 2063 6f6c 756d 6e20  ted into column 
-0000c280: 782c 2077 6869 6368 2068 6173 2074 7970  x, which has typ
-0000c290: 6520 4e55 4d45 5249 4320 666f 7220 7661  e NUMERIC for va
-0000c2a0: 6c75 6520 3135 2e37 3536 332e 0a20 2020  lue 15.7563..   
-0000c2b0: 2020 2020 204f 7665 7272 6964 696e 6720       Overriding 
-0000c2c0: 7468 6520 7465 7374 2074 6f20 7265 6d6f  the test to remo
-0000c2d0: 7665 2074 6865 2066 6169 6c75 7265 2063  ve the failure c
-0000c2e0: 6173 652e 0a20 2020 2020 2020 2022 2222  ase..        """
-0000c2f0: 0a20 2020 2020 2020 2064 6f5f 6e75 6d65  .        do_nume
-0000c300: 7269 635f 7465 7374 280a 2020 2020 2020  ric_test(.      
-0000c310: 2020 2020 2020 4e75 6d65 7269 6328 7072        Numeric(pr
-0000c320: 6563 6973 696f 6e3d 382c 2073 6361 6c65  ecision=8, scale
-0000c330: 3d34 2c20 6173 6465 6369 6d61 6c3d 4661  =4, asdecimal=Fa
-0000c340: 6c73 6529 2c0a 2020 2020 2020 2020 2020  lse),.          
-0000c350: 2020 5b64 6563 696d 616c 2e44 6563 696d    [decimal.Decim
-0000c360: 616c 2822 3135 2e37 3536 3322 292c 2064  al("15.7563"), d
-0000c370: 6563 696d 616c 2e44 6563 696d 616c 2822  ecimal.Decimal("
-0000c380: 3135 2e37 3536 3322 295d 2c0a 2020 2020  15.7563")],.    
-0000c390: 2020 2020 2020 2020 5b31 352e 3735 3633          [15.7563
-0000c3a0: 5d2c 0a20 2020 2020 2020 2029 0a0a 2020  ],.        )..  
-0000c3b0: 2020 4072 6571 7569 7265 732e 666c 6f61    @requires.floa
-0000c3c0: 7473 5f74 6f5f 666f 7572 5f64 6563 696d  ts_to_four_decim
-0000c3d0: 616c 730a 2020 2020 6465 6620 7465 7374  als.    def test
-0000c3e0: 5f66 6c6f 6174 5f61 735f 6465 6369 6d61  _float_as_decima
-0000c3f0: 6c28 7365 6c66 2c20 646f 5f6e 756d 6572  l(self, do_numer
-0000c400: 6963 5f74 6573 7429 3a0a 2020 2020 2020  ic_test):.      
-0000c410: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
-0000c420: 414e 4e45 5220 4f56 4552 5249 4445 3a0a  ANNER OVERRIDE:.
-0000c430: 0a20 2020 2020 2020 2043 6c6f 7564 2053  .        Cloud S
-0000c440: 7061 6e6e 6572 2073 7570 706f 7274 7320  panner supports 
-0000c450: 7461 626c 6573 2077 6974 6820 616e 2065  tables with an e
-0000c460: 6d70 7479 2070 7269 6d61 7279 206b 6579  mpty primary key
-0000c470: 2c20 6275 740a 2020 2020 2020 2020 6f6e  , but.        on
-0000c480: 6c79 2061 2073 696e 676c 6520 726f 7720  ly a single row 
-0000c490: 6361 6e20 6265 2069 6e73 6572 7465 6420  can be inserted 
-0000c4a0: 696e 746f 2073 7563 6820 6120 7461 626c  into such a tabl
-0000c4b0: 6520 2d0a 2020 2020 2020 2020 666f 6c6c  e -.        foll
-0000c4c0: 6f77 696e 6720 696e 7365 7274 696f 6e73  owing insertions
-0000c4d0: 2077 696c 6c20 6661 696c 2077 6974 6820   will fail with 
-0000c4e0: 6052 6f77 205b 5d20 616c 7265 6164 7920  `Row [] already 
-0000c4f0: 6578 6973 7473 222e 0a20 2020 2020 2020  exists"..       
-0000c500: 204f 7665 7272 6964 696e 6720 7468 6520   Overriding the 
-0000c510: 7465 7374 2074 6f20 6176 6f69 6420 7468  test to avoid th
-0000c520: 6520 7361 6d65 2066 6169 6c75 7265 2e0a  e same failure..
-0000c530: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000c540: 2020 2020 646f 5f6e 756d 6572 6963 5f74      do_numeric_t
-0000c550: 6573 7428 0a20 2020 2020 2020 2020 2020  est(.           
-0000c560: 2046 6c6f 6174 2870 7265 6369 7369 6f6e   Float(precision
-0000c570: 3d38 2c20 6173 6465 6369 6d61 6c3d 5472  =8, asdecimal=Tr
-0000c580: 7565 292c 0a20 2020 2020 2020 2020 2020  ue),.           
-0000c590: 205b 6465 6369 6d61 6c2e 4465 6369 6d61   [decimal.Decima
-0000c5a0: 6c28 2231 352e 3735 3633 2229 2c20 6465  l("15.7563"), de
-0000c5b0: 6369 6d61 6c2e 4465 6369 6d61 6c28 2231  cimal.Decimal("1
-0000c5c0: 352e 3735 3633 2229 2c20 4e6f 6e65 5d2c  5.7563"), None],
-0000c5d0: 0a20 2020 2020 2020 2020 2020 205b 6465  .            [de
-0000c5e0: 6369 6d61 6c2e 4465 6369 6d61 6c28 2231  cimal.Decimal("1
-0000c5f0: 352e 3735 3633 2229 2c20 4e6f 6e65 5d2c  5.7563"), None],
-0000c600: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
-0000c610: 7465 725f 3d6c 616d 6264 6120 6e3a 206e  ter_=lambda n: n
-0000c620: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-0000c630: 2072 6f75 6e64 286e 2c20 3429 206f 7220   round(n, 4) or 
-0000c640: 4e6f 6e65 2c0a 2020 2020 2020 2020 290a  None,.        ).
-0000c650: 0a20 2020 2064 6566 2074 6573 745f 666c  .    def test_fl
-0000c660: 6f61 745f 6173 5f66 6c6f 6174 2873 656c  oat_as_float(sel
-0000c670: 662c 2064 6f5f 6e75 6d65 7269 635f 7465  f, do_numeric_te
-0000c680: 7374 293a 0a20 2020 2020 2020 2022 2222  st):.        """
-0000c690: 0a20 2020 2020 2020 2053 5041 4e4e 4552  .        SPANNER
-0000c6a0: 204f 5645 5252 4944 453a 0a0a 2020 2020   OVERRIDE:..    
-0000c6b0: 2020 2020 436c 6f75 6420 5370 616e 6e65      Cloud Spanne
-0000c6c0: 7220 7375 7070 6f72 7473 2074 6162 6c65  r supports table
-0000c6d0: 7320 7769 7468 2061 6e20 656d 7074 7920  s with an empty 
-0000c6e0: 7072 696d 6172 7920 6b65 792c 2062 7574  primary key, but
-0000c6f0: 0a20 2020 2020 2020 206f 6e6c 7920 6120  .        only a 
-0000c700: 7369 6e67 6c65 2072 6f77 2063 616e 2062  single row can b
-0000c710: 6520 696e 7365 7274 6564 2069 6e74 6f20  e inserted into 
-0000c720: 7375 6368 2061 2074 6162 6c65 202d 0a20  such a table -. 
-0000c730: 2020 2020 2020 2066 6f6c 6c6f 7769 6e67         following
-0000c740: 2069 6e73 6572 7469 6f6e 7320 7769 6c6c   insertions will
-0000c750: 2066 6169 6c20 7769 7468 2060 526f 7720   fail with `Row 
-0000c760: 5b5d 2061 6c72 6561 6479 2065 7869 7374  [] already exist
-0000c770: 7322 2e0a 2020 2020 2020 2020 4f76 6572  s"..        Over
-0000c780: 7269 6469 6e67 2074 6865 2074 6573 7420  riding the test 
-0000c790: 746f 2061 766f 6964 2074 6865 2073 616d  to avoid the sam
-0000c7a0: 6520 6661 696c 7572 652e 0a20 2020 2020  e failure..     
-0000c7b0: 2020 2022 2222 0a20 2020 2020 2020 2064     """.        d
-0000c7c0: 6f5f 6e75 6d65 7269 635f 7465 7374 280a  o_numeric_test(.
-0000c7d0: 2020 2020 2020 2020 2020 2020 466c 6f61              Floa
-0000c7e0: 7428 7072 6563 6973 696f 6e3d 3829 2c0a  t(precision=8),.
-0000c7f0: 2020 2020 2020 2020 2020 2020 5b64 6563              [dec
-0000c800: 696d 616c 2e44 6563 696d 616c 2822 3135  imal.Decimal("15
-0000c810: 2e37 3536 3322 292c 2064 6563 696d 616c  .7563"), decimal
-0000c820: 2e44 6563 696d 616c 2822 3135 2e37 3536  .Decimal("15.756
-0000c830: 3322 295d 2c0a 2020 2020 2020 2020 2020  3")],.          
-0000c840: 2020 5b31 352e 3735 3633 5d2c 0a20 2020    [15.7563],.   
-0000c850: 2020 2020 2020 2020 2066 696c 7465 725f           filter_
-0000c860: 3d6c 616d 6264 6120 6e3a 206e 2069 7320  =lambda n: n is 
-0000c870: 6e6f 7420 4e6f 6e65 2061 6e64 2072 6f75  not None and rou
-0000c880: 6e64 286e 2c20 3529 206f 7220 4e6f 6e65  nd(n, 5) or None
-0000c890: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-0000c8a0: 2040 7265 7175 6972 6573 2e70 7265 6369   @requires.preci
-0000c8b0: 7369 6f6e 5f6e 756d 6572 6963 735f 6765  sion_numerics_ge
-0000c8c0: 6e65 7261 6c0a 2020 2020 6465 6620 7465  neral.    def te
-0000c8d0: 7374 5f70 7265 6369 7369 6f6e 5f64 6563  st_precision_dec
-0000c8e0: 696d 616c 2873 656c 662c 2064 6f5f 6e75  imal(self, do_nu
-0000c8f0: 6d65 7269 635f 7465 7374 293a 0a20 2020  meric_test):.   
-0000c900: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000c910: 2053 5041 4e4e 4552 204f 5645 5252 4944   SPANNER OVERRID
-0000c920: 453a 0a0a 2020 2020 2020 2020 436c 6f75  E:..        Clou
-0000c930: 6420 5370 616e 6e65 7220 7375 7070 6f72  d Spanner suppor
-0000c940: 7473 2074 6162 6c65 7320 7769 7468 2061  ts tables with a
-0000c950: 6e20 656d 7074 7920 7072 696d 6172 7920  n empty primary 
-0000c960: 6b65 792c 2062 7574 0a20 2020 2020 2020  key, but.       
-0000c970: 206f 6e6c 7920 6120 7369 6e67 6c65 2072   only a single r
-0000c980: 6f77 2063 616e 2062 6520 696e 7365 7274  ow can be insert
-0000c990: 6564 2069 6e74 6f20 7375 6368 2061 2074  ed into such a t
-0000c9a0: 6162 6c65 202d 0a20 2020 2020 2020 2066  able -.        f
-0000c9b0: 6f6c 6c6f 7769 6e67 2069 6e73 6572 7469  ollowing inserti
-0000c9c0: 6f6e 7320 7769 6c6c 2066 6169 6c20 7769  ons will fail wi
-0000c9d0: 7468 2060 526f 7720 5b5d 2061 6c72 6561  th `Row [] alrea
-0000c9e0: 6479 2065 7869 7374 7322 2e0a 2020 2020  dy exists"..    
-0000c9f0: 2020 2020 4f76 6572 7269 6469 6e67 2074      Overriding t
-0000ca00: 6865 2074 6573 7420 746f 2061 766f 6964  he test to avoid
-0000ca10: 2074 6865 2073 616d 6520 6661 696c 7572   the same failur
-0000ca20: 652e 0a0a 2020 2020 2020 2020 5265 6d6f  e...        Remo
-0000ca30: 7665 2061 6e20 6578 7472 6120 6469 6769  ve an extra digi
-0000ca40: 7473 2061 6674 6572 2064 6563 696d 616c  ts after decimal
-0000ca50: 2070 6f69 6e74 2061 7320 636c 6f75 6420   point as cloud 
-0000ca60: 7370 616e 6e65 7220 6973 0a20 2020 2020  spanner is.     
-0000ca70: 2020 2063 6170 6162 6c65 206f 6620 7265     capable of re
-0000ca80: 7072 6573 656e 7469 6e67 2061 6e20 6578  presenting an ex
-0000ca90: 6163 7420 6e75 6d65 7269 6320 7661 6c75  act numeric valu
-0000caa0: 6520 7769 7468 2061 2070 7265 6369 7369  e with a precisi
-0000cab0: 6f6e 0a20 2020 2020 2020 206f 6620 3338  on.        of 38
-0000cac0: 2061 6e64 2073 6361 6c65 206f 6620 392e   and scale of 9.
-0000cad0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000cae0: 2020 2020 206e 756d 6265 7273 203d 2073       numbers = s
-0000caf0: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
-0000cb00: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-0000cb10: 2020 6465 6369 6d61 6c2e 4465 6369 6d61    decimal.Decima
-0000cb20: 6c28 2235 342e 3234 3634 3531 3635 3022  l("54.246451650"
-0000cb30: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000cb40: 2020 2064 6563 696d 616c 2e44 6563 696d     decimal.Decim
-0000cb50: 616c 2822 302e 3030 3433 3534 2229 2c0a  al("0.004354"),.
-0000cb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb70: 6465 6369 6d61 6c2e 4465 6369 6d61 6c28  decimal.Decimal(
-0000cb80: 2239 3030 2e30 2229 2c0a 2020 2020 2020  "900.0"),.      
-0000cb90: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-0000cba0: 290a 2020 2020 2020 2020 646f 5f6e 756d  ).        do_num
-0000cbb0: 6572 6963 5f74 6573 7428 4e75 6d65 7269  eric_test(Numeri
-0000cbc0: 6328 7072 6563 6973 696f 6e3d 3138 2c20  c(precision=18, 
-0000cbd0: 7363 616c 653d 3929 2c20 6e75 6d62 6572  scale=9), number
-0000cbe0: 732c 206e 756d 6265 7273 290a 0a20 2020  s, numbers)..   
-0000cbf0: 2040 7465 7374 696e 672e 7265 7175 6972   @testing.requir
-0000cc00: 6573 2e70 7265 6369 7369 6f6e 5f6e 756d  es.precision_num
-0000cc10: 6572 6963 735f 656e 6f74 6174 696f 6e5f  erics_enotation_
-0000cc20: 6c61 7267 650a 2020 2020 6465 6620 7465  large.    def te
-0000cc30: 7374 5f65 6e6f 7461 7469 6f6e 5f64 6563  st_enotation_dec
-0000cc40: 696d 616c 5f6c 6172 6765 2873 656c 662c  imal_large(self,
-0000cc50: 2064 6f5f 6e75 6d65 7269 635f 7465 7374   do_numeric_test
-0000cc60: 293a 0a20 2020 2020 2020 2022 2222 7465  ):.        """te
-0000cc70: 7374 2065 7863 6565 6469 6e67 6c79 206c  st exceedingly l
-0000cc80: 6172 6765 2064 6563 696d 616c 732e 0a0a  arge decimals...
-0000cc90: 2020 2020 2020 2020 5350 414e 4e45 5220          SPANNER 
-0000cca0: 4f56 4552 5249 4445 3a0a 0a20 2020 2020  OVERRIDE:..     
-0000ccb0: 2020 2043 6c6f 7564 2053 7061 6e6e 6572     Cloud Spanner
-0000ccc0: 2073 7570 706f 7274 7320 7461 626c 6573   supports tables
-0000ccd0: 2077 6974 6820 616e 2065 6d70 7479 2070   with an empty p
-0000cce0: 7269 6d61 7279 206b 6579 2c20 6275 740a  rimary key, but.
-0000ccf0: 2020 2020 2020 2020 6f6e 6c79 2061 2073          only a s
-0000cd00: 696e 676c 6520 726f 7720 6361 6e20 6265  ingle row can be
-0000cd10: 2069 6e73 6572 7465 6420 696e 746f 2073   inserted into s
-0000cd20: 7563 6820 6120 7461 626c 6520 2d0a 2020  uch a table -.  
-0000cd30: 2020 2020 2020 666f 6c6c 6f77 696e 6720        following 
-0000cd40: 696e 7365 7274 696f 6e73 2077 696c 6c20  insertions will 
-0000cd50: 6661 696c 2077 6974 6820 6052 6f77 205b  fail with `Row [
-0000cd60: 5d20 616c 7265 6164 7920 6578 6973 7473  ] already exists
-0000cd70: 222e 0a20 2020 2020 2020 204f 7665 7272  "..        Overr
-0000cd80: 6964 696e 6720 7468 6520 7465 7374 2074  iding the test t
-0000cd90: 6f20 6176 6f69 6420 7468 6520 7361 6d65  o avoid the same
-0000cda0: 2066 6169 6c75 7265 2e0a 2020 2020 2020   failure..      
-0000cdb0: 2020 2222 220a 2020 2020 2020 2020 6e75    """.        nu
-0000cdc0: 6d62 6572 7320 3d20 7365 7428 0a20 2020  mbers = set(.   
-0000cdd0: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
-0000cde0: 2020 2020 2020 2020 2020 2064 6563 696d             decim
-0000cdf0: 616c 2e44 6563 696d 616c 2822 3445 2b38  al.Decimal("4E+8
-0000ce00: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-0000ce10: 2020 2020 6465 6369 6d61 6c2e 4465 6369      decimal.Deci
-0000ce20: 6d61 6c28 2235 3734 3845 2b31 3522 292c  mal("5748E+15"),
-0000ce30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ce40: 2064 6563 696d 616c 2e44 6563 696d 616c   decimal.Decimal
-0000ce50: 2822 312e 3532 3145 2b31 3522 292c 0a20  ("1.521E+15"),. 
-0000ce60: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000ce70: 6563 696d 616c 2e44 6563 696d 616c 2822  ecimal.Decimal("
-0000ce80: 3030 3030 3030 3030 302e 3145 2b39 2229  000000000.1E+9")
-0000ce90: 2c0a 2020 2020 2020 2020 2020 2020 5d0a  ,.            ].
-0000cea0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000ceb0: 2020 646f 5f6e 756d 6572 6963 5f74 6573    do_numeric_tes
-0000cec0: 7428 4e75 6d65 7269 6328 7072 6563 6973  t(Numeric(precis
-0000ced0: 696f 6e3d 3235 2c20 7363 616c 653d 3229  ion=25, scale=2)
-0000cee0: 2c20 6e75 6d62 6572 732c 206e 756d 6265  , numbers, numbe
-0000cef0: 7273 290a 0a20 2020 2040 7465 7374 696e  rs)..    @testin
-0000cf00: 672e 7265 7175 6972 6573 2e70 7265 6369  g.requires.preci
-0000cf10: 7369 6f6e 5f6e 756d 6572 6963 735f 656e  sion_numerics_en
-0000cf20: 6f74 6174 696f 6e5f 6c61 7267 650a 2020  otation_large.  
-0000cf30: 2020 6465 6620 7465 7374 5f65 6e6f 7461    def test_enota
-0000cf40: 7469 6f6e 5f64 6563 696d 616c 2873 656c  tion_decimal(sel
-0000cf50: 662c 2064 6f5f 6e75 6d65 7269 635f 7465  f, do_numeric_te
-0000cf60: 7374 293a 0a20 2020 2020 2020 2022 2222  st):.        """
-0000cf70: 7465 7374 2065 7863 6565 6469 6e67 6c79  test exceedingly
-0000cf80: 2073 6d61 6c6c 2064 6563 696d 616c 732e   small decimals.
-0000cf90: 0a0a 2020 2020 2020 2020 4465 6369 6d61  ..        Decima
-0000cfa0: 6c20 7265 706f 7274 7320 7661 6c75 6573  l reports values
-0000cfb0: 2077 6974 6820 4520 6e6f 7461 7469 6f6e   with E notation
-0000cfc0: 2077 6865 6e20 7468 6520 6578 706f 6e65   when the expone
-0000cfd0: 6e74 0a20 2020 2020 2020 2069 7320 6772  nt.        is gr
-0000cfe0: 6561 7465 7220 7468 616e 2036 2e0a 0a20  eater than 6... 
-0000cff0: 2020 2020 2020 2053 5041 4e4e 4552 204f         SPANNER O
-0000d000: 5645 5252 4944 453a 0a0a 2020 2020 2020  VERRIDE:..      
-0000d010: 2020 5265 6d6f 7665 2065 7874 7261 2064    Remove extra d
-0000d020: 6967 6974 7320 6166 7465 7220 6465 6369  igits after deci
-0000d030: 6d61 6c20 706f 696e 7420 6173 2043 6c6f  mal point as Clo
-0000d040: 7564 2053 7061 6e6e 6572 2069 730a 2020  ud Spanner is.  
-0000d050: 2020 2020 2020 6361 7061 626c 6520 6f66        capable of
-0000d060: 2072 6570 7265 7365 6e74 696e 6720 616e   representing an
-0000d070: 2065 7861 6374 206e 756d 6572 6963 2076   exact numeric v
-0000d080: 616c 7565 2077 6974 6820 6120 7072 6563  alue with a prec
-0000d090: 6973 696f 6e0a 2020 2020 2020 2020 6f66  ision.        of
-0000d0a0: 2033 3820 616e 6420 7363 616c 6520 6f66   38 and scale of
-0000d0b0: 2039 2e0a 2020 2020 2020 2020 2222 220a   9..        """.
-0000d0c0: 2020 2020 2020 2020 6e75 6d62 6572 7320          numbers 
-0000d0d0: 3d20 7365 7428 0a20 2020 2020 2020 2020  = set(.         
-0000d0e0: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
-0000d0f0: 2020 2020 2064 6563 696d 616c 2e44 6563       decimal.Dec
-0000d100: 696d 616c 2822 3145 2d32 2229 2c0a 2020  imal("1E-2"),.  
-0000d110: 2020 2020 2020 2020 2020 2020 2020 6465                de
-0000d120: 6369 6d61 6c2e 4465 6369 6d61 6c28 2231  cimal.Decimal("1
-0000d130: 452d 3322 292c 0a20 2020 2020 2020 2020  E-3"),.         
-0000d140: 2020 2020 2020 2064 6563 696d 616c 2e44         decimal.D
-0000d150: 6563 696d 616c 2822 3145 2d34 2229 2c0a  ecimal("1E-4"),.
-0000d160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d170: 6465 6369 6d61 6c2e 4465 6369 6d61 6c28  decimal.Decimal(
-0000d180: 2231 452d 3522 292c 0a20 2020 2020 2020  "1E-5"),.       
-0000d190: 2020 2020 2020 2020 2064 6563 696d 616c           decimal
-0000d1a0: 2e44 6563 696d 616c 2822 3145 2d36 2229  .Decimal("1E-6")
-0000d1b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d1c0: 2020 6465 6369 6d61 6c2e 4465 6369 6d61    decimal.Decima
-0000d1d0: 6c28 2231 452d 3722 292c 0a20 2020 2020  l("1E-7"),.     
-0000d1e0: 2020 2020 2020 2020 2020 2064 6563 696d             decim
-0000d1f0: 616c 2e44 6563 696d 616c 2822 3145 2d38  al.Decimal("1E-8
-0000d200: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-0000d210: 2020 2020 6465 6369 6d61 6c2e 4465 6369      decimal.Deci
-0000d220: 6d61 6c28 2230 2e31 3035 3934 3036 3936  mal("0.105940696
-0000d230: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-0000d240: 2020 2020 6465 6369 6d61 6c2e 4465 6369      decimal.Deci
-0000d250: 6d61 6c28 2230 2e30 3035 3934 3036 3936  mal("0.005940696
-0000d260: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-0000d270: 2020 2020 6465 6369 6d61 6c2e 4465 6369      decimal.Deci
-0000d280: 6d61 6c28 2230 2e30 3030 3030 3036 3936  mal("0.000000696
-0000d290: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-0000d2a0: 2020 2020 6465 6369 6d61 6c2e 4465 6369      decimal.Deci
-0000d2b0: 6d61 6c28 2230 2e37 3030 3030 3036 3936  mal("0.700000696
-0000d2c0: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-0000d2d0: 2020 2020 6465 6369 6d61 6c2e 4465 6369      decimal.Deci
-0000d2e0: 6d61 6c28 2236 3936 452d 3922 292c 0a20  mal("696E-9"),. 
-0000d2f0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-0000d300: 2020 2020 2029 0a20 2020 2020 2020 2064       ).        d
-0000d310: 6f5f 6e75 6d65 7269 635f 7465 7374 284e  o_numeric_test(N
-0000d320: 756d 6572 6963 2870 7265 6369 7369 6f6e  umeric(precision
-0000d330: 3d33 382c 2073 6361 6c65 3d39 292c 206e  =38, scale=9), n
-0000d340: 756d 6265 7273 2c20 6e75 6d62 6572 7329  umbers, numbers)
-0000d350: 0a0a 0a63 6c61 7373 204c 696b 6546 756e  ...class LikeFun
-0000d360: 6374 696f 6e73 5465 7374 285f 4c69 6b65  ctionsTest(_Like
-0000d370: 4675 6e63 7469 6f6e 7354 6573 7429 3a0a  FunctionsTest):.
-0000d380: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-0000d390: 2e73 6b69 7028 2253 7061 6e6e 6572 2064  .skip("Spanner d
-0000d3a0: 6f65 736e 2774 2073 7570 706f 7274 204c  oesn't support L
-0000d3b0: 494b 4520 4553 4341 5045 2063 6c61 7573  IKE ESCAPE claus
-0000d3c0: 6522 290a 2020 2020 6465 6620 7465 7374  e").    def test
-0000d3d0: 5f63 6f6e 7461 696e 735f 6175 746f 6573  _contains_autoes
-0000d3e0: 6361 7065 2873 656c 6629 3a0a 2020 2020  cape(self):.    
-0000d3f0: 2020 2020 7061 7373 0a0a 2020 2020 4070      pass..    @p
-0000d400: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
-0000d410: 2253 7061 6e6e 6572 2064 6f65 736e 2774  "Spanner doesn't
-0000d420: 2073 7570 706f 7274 204c 494b 4520 4553   support LIKE ES
-0000d430: 4341 5045 2063 6c61 7573 6522 290a 2020  CAPE clause").  
-0000d440: 2020 6465 6620 7465 7374 5f63 6f6e 7461    def test_conta
-0000d450: 696e 735f 6175 746f 6573 6361 7065 5f65  ins_autoescape_e
-0000d460: 7363 6170 6528 7365 6c66 293a 0a20 2020  scape(self):.   
-0000d470: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
-0000d480: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
-0000d490: 2822 5370 616e 6e65 7220 646f 6573 6e27  ("Spanner doesn'
-0000d4a0: 7420 7375 7070 6f72 7420 4c49 4b45 2045  t support LIKE E
-0000d4b0: 5343 4150 4520 636c 6175 7365 2229 0a20  SCAPE clause"). 
-0000d4c0: 2020 2064 6566 2074 6573 745f 636f 6e74     def test_cont
-0000d4d0: 6169 6e73 5f65 7363 6170 6528 7365 6c66  ains_escape(self
-0000d4e0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-0000d4f0: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
-0000d500: 6b2e 736b 6970 2822 5370 616e 6e65 7220  k.skip("Spanner 
-0000d510: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
-0000d520: 4c49 4b45 2045 5343 4150 4520 636c 6175  LIKE ESCAPE clau
-0000d530: 7365 2229 0a20 2020 2064 6566 2074 6573  se").    def tes
-0000d540: 745f 656e 6473 7769 7468 5f61 7574 6f65  t_endswith_autoe
-0000d550: 7363 6170 6528 7365 6c66 293a 0a20 2020  scape(self):.   
-0000d560: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
-0000d570: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
-0000d580: 2822 5370 616e 6e65 7220 646f 6573 6e27  ("Spanner doesn'
-0000d590: 7420 7375 7070 6f72 7420 4c49 4b45 2045  t support LIKE E
-0000d5a0: 5343 4150 4520 636c 6175 7365 2229 0a20  SCAPE clause"). 
-0000d5b0: 2020 2064 6566 2074 6573 745f 656e 6473     def test_ends
-0000d5c0: 7769 7468 5f65 7363 6170 6528 7365 6c66  with_escape(self
-0000d5d0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-0000d5e0: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
-0000d5f0: 6b2e 736b 6970 2822 5370 616e 6e65 7220  k.skip("Spanner 
-0000d600: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
-0000d610: 4c49 4b45 2045 5343 4150 4520 636c 6175  LIKE ESCAPE clau
-0000d620: 7365 2229 0a20 2020 2064 6566 2074 6573  se").    def tes
-0000d630: 745f 656e 6473 7769 7468 5f61 7574 6f65  t_endswith_autoe
-0000d640: 7363 6170 655f 6573 6361 7065 2873 656c  scape_escape(sel
-0000d650: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-0000d660: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
-0000d670: 726b 2e73 6b69 7028 2253 7061 6e6e 6572  rk.skip("Spanner
-0000d680: 2064 6f65 736e 2774 2073 7570 706f 7274   doesn't support
-0000d690: 204c 494b 4520 4553 4341 5045 2063 6c61   LIKE ESCAPE cla
-0000d6a0: 7573 6522 290a 2020 2020 6465 6620 7465  use").    def te
-0000d6b0: 7374 5f73 7461 7274 7377 6974 685f 6175  st_startswith_au
-0000d6c0: 746f 6573 6361 7065 2873 656c 6629 3a0a  toescape(self):.
-0000d6d0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-0000d6e0: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
-0000d6f0: 6b69 7028 2253 7061 6e6e 6572 2064 6f65  kip("Spanner doe
-0000d700: 736e 2774 2073 7570 706f 7274 204c 494b  sn't support LIK
-0000d710: 4520 4553 4341 5045 2063 6c61 7573 6522  E ESCAPE clause"
-0000d720: 290a 2020 2020 6465 6620 7465 7374 5f73  ).    def test_s
-0000d730: 7461 7274 7377 6974 685f 6573 6361 7065  tartswith_escape
-0000d740: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000d750: 7061 7373 0a0a 2020 2020 4070 7974 6573  pass..    @pytes
-0000d760: 742e 6d61 726b 2e73 6b69 7028 2253 7061  t.mark.skip("Spa
-0000d770: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
-0000d780: 706f 7274 204c 494b 4520 4553 4341 5045  port LIKE ESCAPE
-0000d790: 2063 6c61 7573 6522 290a 2020 2020 6465   clause").    de
-0000d7a0: 6620 7465 7374 5f73 7461 7274 7377 6974  f test_startswit
-0000d7b0: 685f 6175 746f 6573 6361 7065 5f65 7363  h_autoescape_esc
-0000d7c0: 6170 6528 7365 6c66 293a 0a20 2020 2020  ape(self):.     
-0000d7d0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-0000d7e0: 2074 6573 745f 6573 6361 7065 5f6b 6579   test_escape_key
-0000d7f0: 776f 7264 5f72 6169 7365 7328 7365 6c66  word_raises(self
-0000d800: 293a 0a20 2020 2020 2020 2022 2222 4368  ):.        """Ch
-0000d810: 6563 6b20 7468 6174 2045 5343 4150 4520  eck that ESCAPE 
-0000d820: 6b65 7977 6f72 6420 6361 7573 6573 2061  keyword causes a
-0000d830: 6e20 6578 6365 7074 696f 6e20 7768 656e  n exception when
-0000d840: 2075 7365 642e 2222 220a 2020 2020 2020   used.""".      
-0000d850: 2020 7769 7468 2070 7974 6573 742e 7261    with pytest.ra
-0000d860: 6973 6573 284e 6f74 496d 706c 656d 656e  ises(NotImplemen
-0000d870: 7465 6445 7272 6f72 293a 0a20 2020 2020  tedError):.     
-0000d880: 2020 2020 2020 2063 6f6c 203d 2073 656c         col = sel
-0000d890: 662e 7461 626c 6573 2e73 6f6d 655f 7461  f.tables.some_ta
-0000d8a0: 626c 652e 632e 6461 7461 0a20 2020 2020  ble.c.data.     
-0000d8b0: 2020 2020 2020 2073 656c 662e 5f74 6573         self._tes
-0000d8c0: 7428 636f 6c2e 636f 6e74 6169 6e73 2822  t(col.contains("
-0000d8d0: 6223 2363 6465 222c 2065 7363 6170 653d  b##cde", escape=
-0000d8e0: 2223 2229 2c20 7b37 7d29 0a0a 0a40 7079  "#"), {7})...@py
-0000d8f0: 7465 7374 2e6d 6172 6b2e 736b 6970 2822  test.mark.skip("
-0000d900: 5370 616e 6e65 7220 646f 6573 6e27 7420  Spanner doesn't 
-0000d910: 7375 7070 6f72 7420 4953 2044 4953 5449  support IS DISTI
-0000d920: 4e43 5420 4652 4f4d 2063 6c61 7573 6522  NCT FROM clause"
-0000d930: 290a 636c 6173 7320 4973 4f72 4973 4e6f  ).class IsOrIsNo
-0000d940: 7444 6973 7469 6e63 7446 726f 6d54 6573  tDistinctFromTes
-0000d950: 7428 5f49 734f 7249 734e 6f74 4469 7374  t(_IsOrIsNotDist
-0000d960: 696e 6374 4672 6f6d 5465 7374 293a 0a20  inctFromTest):. 
-0000d970: 2020 2070 6173 730a 0a0a 636c 6173 7320     pass...class 
-0000d980: 4f72 6465 7242 794c 6162 656c 5465 7374  OrderByLabelTest
-0000d990: 285f 4f72 6465 7242 794c 6162 656c 5465  (_OrderByLabelTe
-0000d9a0: 7374 293a 0a20 2020 2040 7079 7465 7374  st):.    @pytest
-0000d9b0: 2e6d 6172 6b2e 736b 6970 280a 2020 2020  .mark.skip(.    
-0000d9c0: 2020 2020 2253 7061 6e6e 6572 2072 6571      "Spanner req
-0000d9d0: 7569 7265 7320 616e 2061 6c69 6173 2066  uires an alias f
-0000d9e0: 6f72 2074 6865 2047 524f 5550 2042 5920  or the GROUP BY 
-0000d9f0: 6c69 7374 2077 6865 6e20 7370 6563 6966  list when specif
-0000da00: 7969 6e67 2064 6572 6976 6564 2022 0a20  ying derived ". 
-0000da10: 2020 2020 2020 2022 636f 6c75 6d6e 7320         "columns 
-0000da20: 616c 736f 2075 7365 6420 696e 2053 454c  also used in SEL
-0000da30: 4543 5422 0a20 2020 2029 0a20 2020 2064  ECT".    ).    d
-0000da40: 6566 2074 6573 745f 6772 6f75 705f 6279  ef test_group_by
-0000da50: 5f63 6f6d 706f 7365 6428 7365 6c66 293a  _composed(self):
-0000da60: 0a20 2020 2020 2020 2070 6173 730a 0a0a  .        pass...
-0000da70: 636c 6173 7320 436f 6d70 6f75 6e64 5365  class CompoundSe
-0000da80: 6c65 6374 5465 7374 285f 436f 6d70 6f75  lectTest(_Compou
-0000da90: 6e64 5365 6c65 6374 5465 7374 293a 0a20  ndSelectTest):. 
-0000daa0: 2020 2022 2222 0a20 2020 2053 6565 3a20     """.    See: 
-0000dab0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000dac0: 6f6d 2f67 6f6f 676c 6561 7069 732f 7079  om/googleapis/py
-0000dad0: 7468 6f6e 2d73 7061 6e6e 6572 2f69 7373  thon-spanner/iss
-0000dae0: 7565 732f 3334 370a 2020 2020 2222 220a  ues/347.    """.
-0000daf0: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
-0000db00: 6b2e 736b 6970 280a 2020 2020 2020 2020  k.skip(.        
-0000db10: 2253 7061 6e6e 6572 2044 4241 5049 2069  "Spanner DBAPI i
-0000db20: 6e63 6f72 7265 6374 6c79 2063 6c61 7373  ncorrectly class
-0000db30: 6966 7920 7468 6520 7374 6174 656d 656e  ify the statemen
-0000db40: 7420 7374 6172 7469 6e67 2077 6974 6820  t starting with 
-0000db50: 6272 6163 6b65 7473 2e22 0a20 2020 2029  brackets.".    )
-0000db60: 0a20 2020 2064 6566 2074 6573 745f 6c69  .    def test_li
-0000db70: 6d69 745f 6f66 6673 6574 5f73 656c 6563  mit_offset_selec
-0000db80: 7461 626c 655f 696e 5f75 6e69 6f6e 7328  table_in_unions(
-0000db90: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-0000dba0: 6173 730a 0a20 2020 2040 7079 7465 7374  ass..    @pytest
-0000dbb0: 2e6d 6172 6b2e 736b 6970 280a 2020 2020  .mark.skip(.    
-0000dbc0: 2020 2020 2253 7061 6e6e 6572 2044 4241      "Spanner DBA
-0000dbd0: 5049 2069 6e63 6f72 7265 6374 6c79 2063  PI incorrectly c
-0000dbe0: 6c61 7373 6966 7920 7468 6520 7374 6174  lassify the stat
-0000dbf0: 656d 656e 7420 7374 6172 7469 6e67 2077  ement starting w
-0000dc00: 6974 6820 6272 6163 6b65 7473 2e22 0a20  ith brackets.". 
-0000dc10: 2020 2029 0a20 2020 2064 6566 2074 6573     ).    def tes
-0000dc20: 745f 6f72 6465 725f 6279 5f73 656c 6563  t_order_by_selec
-0000dc30: 7461 626c 655f 696e 5f75 6e69 6f6e 7328  table_in_unions(
-0000dc40: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-0000dc50: 6173 730a 0a0a 636c 6173 7320 5465 7374  ass...class Test
-0000dc60: 5175 6572 7948 696e 7473 2866 6978 7475  QueryHints(fixtu
-0000dc70: 7265 732e 5461 626c 6573 5465 7374 293a  res.TablesTest):
-0000dc80: 0a20 2020 2022 2222 0a20 2020 2043 6f6d  .    """.    Com
-0000dc90: 7069 6c65 2061 2063 6f6d 706c 6578 2071  pile a complex q
-0000dca0: 7565 7279 2077 6974 6820 4a4f 494e 2061  uery with JOIN a
-0000dcb0: 6e64 2063 6865 636b 2074 6861 740a 2020  nd check that.  
-0000dcc0: 2020 7468 6520 7461 626c 6520 6869 6e74    the table hint
-0000dcd0: 2077 6173 2073 6574 2069 6e74 6f20 7468   was set into th
-0000dce0: 6520 7269 6768 7420 706c 6163 652e 0a20  e right place.. 
-0000dcf0: 2020 2022 2222 0a0a 2020 2020 5f5f 6261     """..    __ba
-0000dd00: 636b 656e 645f 5f20 3d20 5472 7565 0a0a  ckend__ = True..
-0000dd10: 2020 2020 6465 6620 7465 7374 5f63 6f6d      def test_com
-0000dd20: 706c 6578 5f71 7565 7279 5f74 6162 6c65  plex_query_table
-0000dd30: 5f68 696e 7473 2873 656c 6629 3a0a 2020  _hints(self):.  
-0000dd40: 2020 2020 2020 4558 5045 4354 4544 5f51        EXPECTED_Q
-0000dd50: 5545 5259 203d 2028 0a20 2020 2020 2020  UERY = (.       
-0000dd60: 2020 2020 2022 5345 4c45 4354 2075 7365       "SELECT use
-0000dd70: 7273 2e69 642c 2075 7365 7273 2e6e 616d  rs.id, users.nam
-0000dd80: 6520 5c6e 4652 4f4d 2075 7365 7273 2040  e \nFROM users @
-0000dd90: 7b46 4f52 4345 5f49 4e44 4558 3d74 6162  {FORCE_INDEX=tab
-0000dda0: 6c65 5f31 5f62 795f 696e 745f 6964 787d  le_1_by_int_idx}
-0000ddb0: 220a 2020 2020 2020 2020 2020 2020 2220  ".            " 
-0000ddc0: 4a4f 494e 2061 6464 7265 7373 6573 204f  JOIN addresses O
-0000ddd0: 4e20 7573 6572 732e 6964 203d 2061 6464  N users.id = add
-0000dde0: 7265 7373 6573 2e75 7365 725f 6964 2022  resses.user_id "
-0000ddf0: 0a20 2020 2020 2020 2020 2020 2022 5c6e  .            "\n
-0000de00: 5748 4552 4520 7573 6572 732e 6e61 6d65  WHERE users.name
-0000de10: 2049 4e20 285f 5f5b 504f 5354 434f 4d50   IN (__[POSTCOMP
-0000de20: 494c 455f 6e61 6d65 5f31 5d29 220a 2020  ILE_name_1])".  
-0000de30: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0000de40: 2042 6173 6520 3d20 6465 636c 6172 6174   Base = declarat
-0000de50: 6976 655f 6261 7365 2829 0a20 2020 2020  ive_base().     
-0000de60: 2020 2065 6e67 696e 6520 3d20 6372 6561     engine = crea
-0000de70: 7465 5f65 6e67 696e 6528 0a20 2020 2020  te_engine(.     
-0000de80: 2020 2020 2020 2022 7370 616e 6e65 723a         "spanner:
-0000de90: 2f2f 2f70 726f 6a65 6374 732f 7072 6f6a  ///projects/proj
-0000dea0: 6563 742d 6964 2f69 6e73 7461 6e63 6573  ect-id/instances
-0000deb0: 2f69 6e73 7461 6e63 652d 6964 2f64 6174  /instance-id/dat
-0000dec0: 6162 6173 6573 2f64 6174 6162 6173 652d  abases/database-
-0000ded0: 6964 220a 2020 2020 2020 2020 290a 0a20  id".        ).. 
-0000dee0: 2020 2020 2020 2063 6c61 7373 2055 7365         class Use
-0000def0: 7228 4261 7365 293a 0a20 2020 2020 2020  r(Base):.       
-0000df00: 2020 2020 205f 5f74 6162 6c65 6e61 6d65       __tablename
-0000df10: 5f5f 203d 2022 7573 6572 7322 0a20 2020  __ = "users".   
-0000df20: 2020 2020 2020 2020 2069 6420 3d20 436f           id = Co
-0000df30: 6c75 6d6e 2849 6e74 6567 6572 2c20 7072  lumn(Integer, pr
-0000df40: 696d 6172 795f 6b65 793d 5472 7565 290a  imary_key=True).
-0000df50: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-0000df60: 203d 2043 6f6c 756d 6e28 5374 7269 6e67   = Column(String
-0000df70: 2835 3029 290a 2020 2020 2020 2020 2020  (50)).          
-0000df80: 2020 6164 6472 6573 7365 7320 3d20 7265    addresses = re
-0000df90: 6c61 7469 6f6e 2822 4164 6472 6573 7322  lation("Address"
-0000dfa0: 2c20 6261 636b 7265 663d 2275 7365 7222  , backref="user"
-0000dfb0: 290a 0a20 2020 2020 2020 2063 6c61 7373  )..        class
-0000dfc0: 2041 6464 7265 7373 2842 6173 6529 3a0a   Address(Base):.
-0000dfd0: 2020 2020 2020 2020 2020 2020 5f5f 7461              __ta
-0000dfe0: 626c 656e 616d 655f 5f20 3d20 2261 6464  blename__ = "add
-0000dff0: 7265 7373 6573 220a 2020 2020 2020 2020  resses".        
-0000e000: 2020 2020 6964 203d 2043 6f6c 756d 6e28      id = Column(
-0000e010: 496e 7465 6765 722c 2070 7269 6d61 7279  Integer, primary
-0000e020: 5f6b 6579 3d54 7275 6529 0a20 2020 2020  _key=True).     
-0000e030: 2020 2020 2020 2065 6d61 696c 203d 2043         email = C
-0000e040: 6f6c 756d 6e28 5374 7269 6e67 2835 3029  olumn(String(50)
-0000e050: 290a 2020 2020 2020 2020 2020 2020 7573  ).            us
-0000e060: 6572 5f69 6420 3d20 436f 6c75 6d6e 2849  er_id = Column(I
-0000e070: 6e74 6567 6572 2c20 466f 7265 6967 6e4b  nteger, ForeignK
-0000e080: 6579 2822 7573 6572 732e 6964 2229 290a  ey("users.id")).
-0000e090: 0a20 2020 2020 2020 2073 6573 7369 6f6e  .        session
-0000e0a0: 203d 2053 6573 7369 6f6e 2865 6e67 696e   = Session(engin
-0000e0b0: 6529 0a0a 2020 2020 2020 2020 7175 6572  e)..        quer
-0000e0c0: 7920 3d20 7365 7373 696f 6e2e 7175 6572  y = session.quer
-0000e0d0: 7928 5573 6572 290a 2020 2020 2020 2020  y(User).        
-0000e0e0: 7175 6572 7920 3d20 7175 6572 792e 7769  query = query.wi
-0000e0f0: 7468 5f68 696e 7428 0a20 2020 2020 2020  th_hint(.       
-0000e100: 2020 2020 2073 656c 6563 7461 626c 653d       selectable=
-0000e110: 5573 6572 2c20 7465 7874 3d22 407b 464f  User, text="@{FO
-0000e120: 5243 455f 494e 4445 583d 7461 626c 655f  RCE_INDEX=table_
-0000e130: 315f 6279 5f69 6e74 5f69 6478 7d22 0a20  1_by_int_idx}". 
-0000e140: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000e150: 2020 7175 6572 7920 3d20 7175 6572 792e    query = query.
-0000e160: 6669 6c74 6572 2855 7365 722e 6e61 6d65  filter(User.name
-0000e170: 2e69 6e5f 285b 2276 616c 3122 2c20 2276  .in_(["val1", "v
-0000e180: 616c 3222 5d29 290a 2020 2020 2020 2020  al2"])).        
-0000e190: 7175 6572 7920 3d20 7175 6572 792e 6a6f  query = query.jo
-0000e1a0: 696e 2841 6464 7265 7373 290a 0a20 2020  in(Address)..   
-0000e1b0: 2020 2020 2061 7373 6572 7420 7374 7228       assert str(
-0000e1c0: 7175 6572 792e 7374 6174 656d 656e 742e  query.statement.
-0000e1d0: 636f 6d70 696c 6528 7365 7373 696f 6e2e  compile(session.
-0000e1e0: 6269 6e64 2929 203d 3d20 4558 5045 4354  bind)) == EXPECT
-0000e1f0: 4544 5f51 5545 5259 0a0a 0a63 6c61 7373  ED_QUERY...class
-0000e200: 2049 6e74 6572 6c65 6176 6564 5461 626c   InterleavedTabl
-0000e210: 6573 5465 7374 2866 6978 7475 7265 732e  esTest(fixtures.
-0000e220: 5465 7374 4261 7365 293a 0a20 2020 2022  TestBase):.    "
-0000e230: 2222 0a20 2020 2043 6865 636b 2074 6861  "".    Check tha
-0000e240: 7420 4352 4541 5445 2054 4142 4c45 2073  t CREATE TABLE s
-0000e250: 7461 7465 6d65 6e74 7320 666f 7220 696e  tatements for in
-0000e260: 7465 726c 6561 7665 6420 7461 626c 6573  terleaved tables
-0000e270: 2061 7265 2063 6f72 7265 6374 6c79 0a20   are correctly. 
-0000e280: 2020 2067 656e 6572 6174 6564 2e0a 2020     generated..  
-0000e290: 2020 2222 220a 0a20 2020 2064 6566 2073    """..    def s
-0000e2a0: 6574 5570 2873 656c 6629 3a0a 2020 2020  etUp(self):.    
-0000e2b0: 2020 2020 7365 6c66 2e5f 656e 6769 6e65      self._engine
-0000e2c0: 203d 2063 7265 6174 655f 656e 6769 6e65   = create_engine
-0000e2d0: 280a 2020 2020 2020 2020 2020 2020 2273  (.            "s
-0000e2e0: 7061 6e6e 6572 3a2f 2f2f 7072 6f6a 6563  panner:///projec
-0000e2f0: 7473 2f61 7070 6465 762d 736f 6461 2d73  ts/appdev-soda-s
-0000e300: 7061 6e6e 6572 2d73 7461 6769 6e67 2f69  panner-staging/i
-0000e310: 6e73 7461 6e63 6573 2f22 0a20 2020 2020  nstances/".     
-0000e320: 2020 2020 2020 2022 7371 6c61 6c63 6865         "sqlalche
-0000e330: 6d79 2d64 6961 6c65 6374 2d74 6573 742f  my-dialect-test/
-0000e340: 6461 7461 6261 7365 732f 636f 6d70 6c69  databases/compli
-0000e350: 616e 6365 2d74 6573 7422 0a20 2020 2020  ance-test".     
-0000e360: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-0000e370: 662e 5f6d 6574 6164 6174 6120 3d20 4d65  f._metadata = Me
-0000e380: 7461 4461 7461 2862 696e 643d 7365 6c66  taData(bind=self
-0000e390: 2e5f 656e 6769 6e65 290a 0a20 2020 2064  ._engine)..    d
-0000e3a0: 6566 2074 6573 745f 696e 7465 726c 6561  ef test_interlea
-0000e3b0: 7665 2873 656c 6629 3a0a 2020 2020 2020  ve(self):.      
-0000e3c0: 2020 4558 505f 5155 4552 5920 3d20 280a    EXP_QUERY = (.
-0000e3d0: 2020 2020 2020 2020 2020 2020 225c 6e43              "\nC
-0000e3e0: 5245 4154 4520 5441 424c 4520 636c 6965  REATE TABLE clie
-0000e3f0: 6e74 2028 5c6e 5c74 7465 616d 5f69 6420  nt (\n\tteam_id 
-0000e400: 494e 5436 3420 4e4f 5420 4e55 4c4c 2c20  INT64 NOT NULL, 
-0000e410: 220a 2020 2020 2020 2020 2020 2020 225c  ".            "\
-0000e420: 6e5c 7463 6c69 656e 745f 6964 2049 4e54  n\tclient_id INT
-0000e430: 3634 204e 4f54 204e 554c 4c2c 2022 0a20  64 NOT NULL, ". 
-0000e440: 2020 2020 2020 2020 2020 2022 5c6e 5c74             "\n\t
-0000e450: 636c 6965 6e74 5f6e 616d 6520 5354 5249  client_name STRI
-0000e460: 4e47 2831 3629 204e 4f54 204e 554c 4c22  NG(16) NOT NULL"
-0000e470: 0a20 2020 2020 2020 2020 2020 2022 5c6e  .            "\n
-0000e480: 2920 5052 494d 4152 5920 4b45 5920 2874  ) PRIMARY KEY (t
-0000e490: 6561 6d5f 6964 2c20 636c 6965 6e74 5f69  eam_id, client_i
-0000e4a0: 6429 2c22 0a20 2020 2020 2020 2020 2020  d),".           
-0000e4b0: 2022 5c6e 494e 5445 524c 4541 5645 2049   "\nINTERLEAVE I
-0000e4c0: 4e20 5041 5245 4e54 2074 6561 6d5c 6e5c  N PARENT team\n\
-0000e4d0: 6e22 0a20 2020 2020 2020 2029 0a20 2020  n".        ).   
-0000e4e0: 2020 2020 2063 6c69 656e 7420 3d20 5461       client = Ta
-0000e4f0: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
-0000e500: 2022 636c 6965 6e74 222c 0a20 2020 2020   "client",.     
-0000e510: 2020 2020 2020 2073 656c 662e 5f6d 6574         self._met
-0000e520: 6164 6174 612c 0a20 2020 2020 2020 2020  adata,.         
-0000e530: 2020 2043 6f6c 756d 6e28 2274 6561 6d5f     Column("team_
-0000e540: 6964 222c 2049 6e74 6567 6572 2c20 7072  id", Integer, pr
-0000e550: 696d 6172 795f 6b65 793d 5472 7565 292c  imary_key=True),
-0000e560: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
-0000e570: 756d 6e28 2263 6c69 656e 745f 6964 222c  umn("client_id",
-0000e580: 2049 6e74 6567 6572 2c20 7072 696d 6172   Integer, primar
-0000e590: 795f 6b65 793d 5472 7565 292c 0a20 2020  y_key=True),.   
-0000e5a0: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
-0000e5b0: 2263 6c69 656e 745f 6e61 6d65 222c 2053  "client_name", S
-0000e5c0: 7472 696e 6728 3136 292c 206e 756c 6c61  tring(16), nulla
-0000e5d0: 626c 653d 4661 6c73 6529 2c0a 2020 2020  ble=False),.    
-0000e5e0: 2020 2020 2020 2020 7370 616e 6e65 725f          spanner_
-0000e5f0: 696e 7465 726c 6561 7665 5f69 6e3d 2274  interleave_in="t
-0000e600: 6561 6d22 2c0a 2020 2020 2020 2020 290a  eam",.        ).
-0000e610: 2020 2020 2020 2020 7769 7468 206d 6f63          with moc
-0000e620: 6b2e 7061 7463 6828 2267 6f6f 676c 652e  k.patch("google.
-0000e630: 636c 6f75 642e 7370 616e 6e65 725f 6462  cloud.spanner_db
-0000e640: 6170 692e 6375 7273 6f72 2e43 7572 736f  api.cursor.Curso
-0000e650: 722e 6578 6563 7574 6522 2920 6173 2065  r.execute") as e
-0000e660: 7865 6375 7465 3a0a 2020 2020 2020 2020  xecute:.        
-0000e670: 2020 2020 636c 6965 6e74 2e63 7265 6174      client.creat
-0000e680: 6528 7365 6c66 2e5f 656e 6769 6e65 290a  e(self._engine).
-0000e690: 2020 2020 2020 2020 2020 2020 6578 6563              exec
-0000e6a0: 7574 652e 6173 7365 7274 5f63 616c 6c65  ute.assert_calle
-0000e6b0: 645f 6f6e 6365 5f77 6974 6828 4558 505f  d_once_with(EXP_
-0000e6c0: 5155 4552 592c 205b 5d29 0a0a 2020 2020  QUERY, [])..    
-0000e6d0: 6465 6620 7465 7374 5f69 6e74 6572 6c65  def test_interle
-0000e6e0: 6176 655f 6f6e 5f64 656c 6574 655f 6361  ave_on_delete_ca
-0000e6f0: 7363 6164 6528 7365 6c66 293a 0a20 2020  scade(self):.   
-0000e700: 2020 2020 2045 5850 5f51 5545 5259 203d       EXP_QUERY =
-0000e710: 2028 0a20 2020 2020 2020 2020 2020 2022   (.            "
-0000e720: 5c6e 4352 4541 5445 2054 4142 4c45 2063  \nCREATE TABLE c
-0000e730: 6c69 656e 7420 285c 6e5c 7474 6561 6d5f  lient (\n\tteam_
-0000e740: 6964 2049 4e54 3634 204e 4f54 204e 554c  id INT64 NOT NUL
-0000e750: 4c2c 2022 0a20 2020 2020 2020 2020 2020  L, ".           
-0000e760: 2022 5c6e 5c74 636c 6965 6e74 5f69 6420   "\n\tclient_id 
-0000e770: 494e 5436 3420 4e4f 5420 4e55 4c4c 2c20  INT64 NOT NULL, 
-0000e780: 220a 2020 2020 2020 2020 2020 2020 225c  ".            "\
-0000e790: 6e5c 7463 6c69 656e 745f 6e61 6d65 2053  n\tclient_name S
-0000e7a0: 5452 494e 4728 3136 2920 4e4f 5420 4e55  TRING(16) NOT NU
-0000e7b0: 4c4c 220a 2020 2020 2020 2020 2020 2020  LL".            
-0000e7c0: 225c 6e29 2050 5249 4d41 5259 204b 4559  "\n) PRIMARY KEY
-0000e7d0: 2028 7465 616d 5f69 642c 2063 6c69 656e   (team_id, clien
-0000e7e0: 745f 6964 292c 220a 2020 2020 2020 2020  t_id),".        
-0000e7f0: 2020 2020 225c 6e49 4e54 4552 4c45 4156      "\nINTERLEAV
-0000e800: 4520 494e 2050 4152 454e 5420 7465 616d  E IN PARENT team
-0000e810: 204f 4e20 4445 4c45 5445 2043 4153 4341   ON DELETE CASCA
-0000e820: 4445 5c6e 5c6e 220a 2020 2020 2020 2020  DE\n\n".        
-0000e830: 290a 2020 2020 2020 2020 636c 6965 6e74  ).        client
-0000e840: 203d 2054 6162 6c65 280a 2020 2020 2020   = Table(.      
-0000e850: 2020 2020 2020 2263 6c69 656e 7422 2c0a        "client",.
-0000e860: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e870: 2e5f 6d65 7461 6461 7461 2c0a 2020 2020  ._metadata,.    
-0000e880: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
-0000e890: 7465 616d 5f69 6422 2c20 496e 7465 6765  team_id", Intege
-0000e8a0: 722c 2070 7269 6d61 7279 5f6b 6579 3d54  r, primary_key=T
-0000e8b0: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
-0000e8c0: 2020 436f 6c75 6d6e 2822 636c 6965 6e74    Column("client
-0000e8d0: 5f69 6422 2c20 496e 7465 6765 722c 2070  _id", Integer, p
-0000e8e0: 7269 6d61 7279 5f6b 6579 3d54 7275 6529  rimary_key=True)
-0000e8f0: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
-0000e900: 6c75 6d6e 2822 636c 6965 6e74 5f6e 616d  lumn("client_nam
-0000e910: 6522 2c20 5374 7269 6e67 2831 3629 2c20  e", String(16), 
-0000e920: 6e75 6c6c 6162 6c65 3d46 616c 7365 292c  nullable=False),
-0000e930: 0a20 2020 2020 2020 2020 2020 2073 7061  .            spa
-0000e940: 6e6e 6572 5f69 6e74 6572 6c65 6176 655f  nner_interleave_
-0000e950: 696e 3d22 7465 616d 222c 0a20 2020 2020  in="team",.     
-0000e960: 2020 2020 2020 2073 7061 6e6e 6572 5f69         spanner_i
-0000e970: 6e74 6572 6c65 6176 655f 6f6e 5f64 656c  nterleave_on_del
-0000e980: 6574 655f 6361 7363 6164 653d 5472 7565  ete_cascade=True
-0000e990: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-0000e9a0: 2020 2020 7769 7468 206d 6f63 6b2e 7061      with mock.pa
-0000e9b0: 7463 6828 2267 6f6f 676c 652e 636c 6f75  tch("google.clou
-0000e9c0: 642e 7370 616e 6e65 725f 6462 6170 692e  d.spanner_dbapi.
-0000e9d0: 6375 7273 6f72 2e43 7572 736f 722e 6578  cursor.Cursor.ex
-0000e9e0: 6563 7574 6522 2920 6173 2065 7865 6375  ecute") as execu
-0000e9f0: 7465 3a0a 2020 2020 2020 2020 2020 2020  te:.            
-0000ea00: 636c 6965 6e74 2e63 7265 6174 6528 7365  client.create(se
-0000ea10: 6c66 2e5f 656e 6769 6e65 290a 2020 2020  lf._engine).    
-0000ea20: 2020 2020 2020 2020 6578 6563 7574 652e          execute.
-0000ea30: 6173 7365 7274 5f63 616c 6c65 645f 6f6e  assert_called_on
-0000ea40: 6365 5f77 6974 6828 4558 505f 5155 4552  ce_with(EXP_QUER
-0000ea50: 592c 205b 5d29 0a0a 0a63 6c61 7373 2055  Y, [])...class U
-0000ea60: 7365 7241 6765 6e74 5465 7374 2866 6978  serAgentTest(fix
-0000ea70: 7475 7265 732e 5465 7374 4261 7365 293a  tures.TestBase):
-0000ea80: 0a20 2020 2022 2222 4368 6563 6b20 7468  .    """Check th
-0000ea90: 6174 2053 514c 416c 6368 656d 7920 6469  at SQLAlchemy di
-0000eaa0: 616c 6563 7420 7573 6573 2063 6f72 7265  alect uses corre
-0000eab0: 6374 2075 7365 7220 6167 656e 742e 2222  ct user agent.""
-0000eac0: 220a 0a20 2020 2064 6566 2073 6574 5570  "..    def setUp
-0000ead0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000eae0: 7365 6c66 2e5f 656e 6769 6e65 203d 2063  self._engine = c
-0000eaf0: 7265 6174 655f 656e 6769 6e65 280a 2020  reate_engine(.  
-0000eb00: 2020 2020 2020 2020 2020 2273 7061 6e6e            "spann
-0000eb10: 6572 3a2f 2f2f 7072 6f6a 6563 7473 2f61  er:///projects/a
-0000eb20: 7070 6465 762d 736f 6461 2d73 7061 6e6e  ppdev-soda-spann
-0000eb30: 6572 2d73 7461 6769 6e67 2f69 6e73 7461  er-staging/insta
-0000eb40: 6e63 6573 2f22 0a20 2020 2020 2020 2020  nces/".         
-0000eb50: 2020 2022 7371 6c61 6c63 6865 6d79 2d64     "sqlalchemy-d
-0000eb60: 6961 6c65 6374 2d74 6573 742f 6461 7461  ialect-test/data
-0000eb70: 6261 7365 732f 636f 6d70 6c69 616e 6365  bases/compliance
-0000eb80: 2d74 6573 7422 0a20 2020 2020 2020 2029  -test".        )
-0000eb90: 0a20 2020 2020 2020 2073 656c 662e 5f6d  .        self._m
-0000eba0: 6574 6164 6174 6120 3d20 4d65 7461 4461  etadata = MetaDa
-0000ebb0: 7461 2862 696e 643d 7365 6c66 2e5f 656e  ta(bind=self._en
-0000ebc0: 6769 6e65 290a 0a20 2020 2064 6566 2074  gine)..    def t
-0000ebd0: 6573 745f 7573 6572 5f61 6765 6e74 2873  est_user_agent(s
-0000ebe0: 656c 6629 3a0a 2020 2020 2020 2020 6469  elf):.        di
-0000ebf0: 7374 203d 2070 6b67 5f72 6573 6f75 7263  st = pkg_resourc
-0000ec00: 6573 2e67 6574 5f64 6973 7472 6962 7574  es.get_distribut
-0000ec10: 696f 6e28 2273 716c 616c 6368 656d 792d  ion("sqlalchemy-
-0000ec20: 7370 616e 6e65 7222 290a 0a20 2020 2020  spanner")..     
-0000ec30: 2020 2077 6974 6820 7365 6c66 2e5f 656e     with self._en
-0000ec40: 6769 6e65 2e63 6f6e 6e65 6374 2829 2061  gine.connect() a
-0000ec50: 7320 636f 6e6e 6563 7469 6f6e 3a0a 2020  s connection:.  
-0000ec60: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-0000ec70: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-0000ec80: 2020 2063 6f6e 6e65 6374 696f 6e2e 636f     connection.co
-0000ec90: 6e6e 6563 7469 6f6e 2e69 6e73 7461 6e63  nnection.instanc
-0000eca0: 652e 5f63 6c69 656e 742e 5f63 6c69 656e  e._client._clien
-0000ecb0: 745f 696e 666f 2e75 7365 725f 6167 656e  t_info.user_agen
-0000ecc0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-0000ecd0: 2020 3d3d 2022 676c 2d22 202b 2064 6973    == "gl-" + dis
-0000ece0: 742e 7072 6f6a 6563 745f 6e61 6d65 202b  t.project_name +
-0000ecf0: 2022 2f22 202b 2064 6973 742e 7665 7273   "/" + dist.vers
-0000ed00: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-0000ed10: 290a 0a0a 636c 6173 7320 5369 6d70 6c65  )...class Simple
-0000ed20: 5570 6461 7465 4465 6c65 7465 5465 7374  UpdateDeleteTest
-0000ed30: 285f 5369 6d70 6c65 5570 6461 7465 4465  (_SimpleUpdateDe
-0000ed40: 6c65 7465 5465 7374 293a 0a20 2020 2022  leteTest):.    "
-0000ed50: 2222 0a20 2020 2053 5041 4e4e 4552 204f  "".    SPANNER O
-0000ed60: 5645 5252 4944 453a 0a0a 2020 2020 5370  VERRIDE:..    Sp
-0000ed70: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
-0000ed80: 7070 6f72 7420 6072 6f77 636f 756e 7460  pport `rowcount`
-0000ed90: 2070 726f 7065 7274 792e 2054 6865 7365   property. These
-0000eda0: 0a20 2020 2074 6573 7420 6361 7365 7320  .    test cases 
-0000edb0: 6f76 6572 7269 6465 7320 6f6d 6974 2060  overrides omit `
-0000edc0: 726f 7763 6f75 6e74 6020 6368 6563 6b73  rowcount` checks
-0000edd0: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
-0000ede0: 6566 2074 6573 745f 6465 6c65 7465 2873  ef test_delete(s
-0000edf0: 656c 662c 2063 6f6e 6e65 6374 696f 6e29  elf, connection)
-0000ee00: 3a0a 2020 2020 2020 2020 7420 3d20 7365  :.        t = se
-0000ee10: 6c66 2e74 6162 6c65 732e 706c 6169 6e5f  lf.tables.plain_
-0000ee20: 706b 0a20 2020 2020 2020 2072 203d 2063  pk.        r = c
-0000ee30: 6f6e 6e65 6374 696f 6e2e 6578 6563 7574  onnection.execut
-0000ee40: 6528 742e 6465 6c65 7465 2829 2e77 6865  e(t.delete().whe
-0000ee50: 7265 2874 2e63 2e69 6420 3d3d 2032 2929  re(t.c.id == 2))
-0000ee60: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0000ee70: 6e6f 7420 722e 6973 5f69 6e73 6572 740a  not r.is_insert.
-0000ee80: 2020 2020 2020 2020 6173 7365 7274 206e          assert n
-0000ee90: 6f74 2072 2e72 6574 7572 6e73 5f72 6f77  ot r.returns_row
-0000eea0: 730a 2020 2020 2020 2020 6571 5f28 0a20  s.        eq_(. 
-0000eeb0: 2020 2020 2020 2020 2020 2063 6f6e 6e65             conne
-0000eec0: 6374 696f 6e2e 6578 6563 7574 6528 742e  ction.execute(t.
-0000eed0: 7365 6c65 6374 2829 2e6f 7264 6572 5f62  select().order_b
-0000eee0: 7928 742e 632e 6964 2929 2e66 6574 6368  y(t.c.id)).fetch
-0000eef0: 616c 6c28 292c 0a20 2020 2020 2020 2020  all(),.         
-0000ef00: 2020 205b 2831 2c20 2264 3122 292c 2028     [(1, "d1"), (
-0000ef10: 332c 2022 6433 2229 5d2c 0a20 2020 2020  3, "d3")],.     
-0000ef20: 2020 2029 0a0a 2020 2020 6465 6620 7465     )..    def te
-0000ef30: 7374 5f75 7064 6174 6528 7365 6c66 2c20  st_update(self, 
-0000ef40: 636f 6e6e 6563 7469 6f6e 293a 0a20 2020  connection):.   
-0000ef50: 2020 2020 2074 203d 2073 656c 662e 7461       t = self.ta
-0000ef60: 626c 6573 2e70 6c61 696e 5f70 6b0a 2020  bles.plain_pk.  
-0000ef70: 2020 2020 2020 7220 3d20 636f 6e6e 6563        r = connec
-0000ef80: 7469 6f6e 2e65 7865 6375 7465 2874 2e75  tion.execute(t.u
-0000ef90: 7064 6174 6528 292e 7768 6572 6528 742e  pdate().where(t.
-0000efa0: 632e 6964 203d 3d20 3229 2c20 6469 6374  c.id == 2), dict
-0000efb0: 2864 6174 613d 2264 325f 6e65 7722 2929  (data="d2_new"))
-0000efc0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0000efd0: 6e6f 7420 722e 6973 5f69 6e73 6572 740a  not r.is_insert.
-0000efe0: 2020 2020 2020 2020 6173 7365 7274 206e          assert n
-0000eff0: 6f74 2072 2e72 6574 7572 6e73 5f72 6f77  ot r.returns_row
-0000f000: 730a 0a20 2020 2020 2020 2065 715f 280a  s..        eq_(.
-0000f010: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
-0000f020: 6563 7469 6f6e 2e65 7865 6375 7465 2874  ection.execute(t
-0000f030: 2e73 656c 6563 7428 292e 6f72 6465 725f  .select().order_
-0000f040: 6279 2874 2e63 2e69 6429 292e 6665 7463  by(t.c.id)).fetc
-0000f050: 6861 6c6c 2829 2c0a 2020 2020 2020 2020  hall(),.        
-0000f060: 2020 2020 5b28 312c 2022 6431 2229 2c20      [(1, "d1"), 
-0000f070: 2832 2c20 2264 325f 6e65 7722 292c 2028  (2, "d2_new"), (
-0000f080: 332c 2022 6433 2229 5d2c 0a20 2020 2020  3, "d3")],.     
-0000f090: 2020 2029 0a0a 0a63 6c61 7373 2048 6173     )...class Has
-0000f0a0: 496e 6465 7854 6573 7428 5f48 6173 496e  IndexTest(_HasIn
-0000f0b0: 6465 7854 6573 7429 3a0a 2020 2020 4063  dexTest):.    @c
-0000f0c0: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-0000f0d0: 6566 2064 6566 696e 655f 7461 626c 6573  ef define_tables
-0000f0e0: 2863 6c73 2c20 6d65 7461 6461 7461 293a  (cls, metadata):
-0000f0f0: 0a20 2020 2020 2020 2074 7420 3d20 5461  .        tt = Ta
-0000f100: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
-0000f110: 2022 7465 7374 5f74 6162 6c65 222c 0a20   "test_table",. 
-0000f120: 2020 2020 2020 2020 2020 206d 6574 6164             metad
-0000f130: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-0000f140: 2043 6f6c 756d 6e28 2269 6422 2c20 496e   Column("id", In
-0000f150: 7465 6765 722c 2070 7269 6d61 7279 5f6b  teger, primary_k
-0000f160: 6579 3d54 7275 6529 2c0a 2020 2020 2020  ey=True),.      
-0000f170: 2020 2020 2020 436f 6c75 6d6e 2822 6461        Column("da
-0000f180: 7461 222c 2053 7472 696e 6728 3530 2929  ta", String(50))
-0000f190: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-0000f1a0: 2020 2020 7371 6c61 6c63 6865 6d79 2e49      sqlalchemy.I
-0000f1b0: 6e64 6578 2822 6d79 5f69 6478 222c 2074  ndex("my_idx", t
-0000f1c0: 742e 632e 6461 7461 290a 0a20 2020 2040  t.c.data)..    @
-0000f1d0: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
-0000f1e0: 2822 4e6f 7420 7375 7070 6f72 7465 6420  ("Not supported 
-0000f1f0: 6279 2043 6c6f 7564 2053 7061 6e6e 6572  by Cloud Spanner
-0000f200: 2229 0a20 2020 2064 6566 2074 6573 745f  ").    def test_
-0000f210: 6861 735f 696e 6465 785f 7363 6865 6d61  has_index_schema
-0000f220: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000f230: 7061 7373 0a0a 0a63 6c61 7373 2048 6173  pass...class Has
-0000f240: 5461 626c 6554 6573 7428 5f48 6173 5461  TableTest(_HasTa
-0000f250: 626c 6554 6573 7429 3a0a 2020 2020 4063  bleTest):.    @c
-0000f260: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-0000f270: 6566 2064 6566 696e 655f 7461 626c 6573  ef define_tables
-0000f280: 2863 6c73 2c20 6d65 7461 6461 7461 293a  (cls, metadata):
-0000f290: 0a20 2020 2020 2020 2054 6162 6c65 280a  .        Table(.
-0000f2a0: 2020 2020 2020 2020 2020 2020 2274 6573              "tes
-0000f2b0: 745f 7461 626c 6522 2c0a 2020 2020 2020  t_table",.      
-0000f2c0: 2020 2020 2020 6d65 7461 6461 7461 2c0a        metadata,.
-0000f2d0: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
-0000f2e0: 6d6e 2822 6964 222c 2049 6e74 6567 6572  mn("id", Integer
-0000f2f0: 2c20 7072 696d 6172 795f 6b65 793d 5472  , primary_key=Tr
-0000f300: 7565 292c 0a20 2020 2020 2020 2020 2020  ue),.           
-0000f310: 2043 6f6c 756d 6e28 2264 6174 6122 2c20   Column("data", 
-0000f320: 5374 7269 6e67 2835 3029 292c 0a20 2020  String(50)),.   
-0000f330: 2020 2020 2029 0a0a 2020 2020 4070 7974       )..    @pyt
-0000f340: 6573 742e 6d61 726b 2e73 6b69 7028 224e  est.mark.skip("N
-0000f350: 6f74 2073 7570 706f 7274 6564 2062 7920  ot supported by 
-0000f360: 436c 6f75 6420 5370 616e 6e65 7222 290a  Cloud Spanner").
-0000f370: 2020 2020 6465 6620 7465 7374 5f68 6173      def test_has
-0000f380: 5f74 6162 6c65 5f73 6368 656d 6128 7365  _table_schema(se
-0000f390: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
-0000f3a0: 730a 0a0a 636c 6173 7320 506f 7374 436f  s...class PostCo
-0000f3b0: 6d70 696c 6550 6172 616d 7354 6573 7428  mpileParamsTest(
-0000f3c0: 5f50 6f73 7443 6f6d 7069 6c65 5061 7261  _PostCompilePara
-0000f3d0: 6d73 5465 7374 293a 0a20 2020 2064 6566  msTest):.    def
-0000f3e0: 2074 6573 745f 6578 6563 7574 6528 7365   test_execute(se
-0000f3f0: 6c66 293a 0a20 2020 2020 2020 2074 6162  lf):.        tab
-0000f400: 6c65 203d 2073 656c 662e 7461 626c 6573  le = self.tables
-0000f410: 2e73 6f6d 655f 7461 626c 650a 0a20 2020  .some_table..   
-0000f420: 2020 2020 2073 746d 7420 3d20 7365 6c65       stmt = sele
-0000f430: 6374 2874 6162 6c65 2e63 2e69 6429 2e77  ct(table.c.id).w
-0000f440: 6865 7265 280a 2020 2020 2020 2020 2020  here(.          
-0000f450: 2020 7461 626c 652e 632e 7820 3d3d 2073    table.c.x == s
-0000f460: 716c 616c 6368 656d 792e 6269 6e64 7061  qlalchemy.bindpa
-0000f470: 7261 6d28 2271 222c 206c 6974 6572 616c  ram("q", literal
-0000f480: 5f65 7865 6375 7465 3d54 7275 6529 0a20  _execute=True). 
-0000f490: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000f4a0: 2020 7769 7468 2073 656c 662e 7371 6c5f    with self.sql_
-0000f4b0: 6578 6563 7574 696f 6e5f 6173 7365 7274  execution_assert
-0000f4c0: 6572 2829 2061 7320 6173 7365 7274 6572  er() as asserter
-0000f4d0: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
-0000f4e0: 7468 2063 6f6e 6669 672e 6462 2e63 6f6e  th config.db.con
-0000f4f0: 6e65 6374 2829 2061 7320 636f 6e6e 3a0a  nect() as conn:.
-0000f500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f510: 636f 6e6e 2e65 7865 6375 7465 2873 746d  conn.execute(stm
-0000f520: 742c 2064 6963 7428 713d 3130 2929 0a0a  t, dict(q=10))..
-0000f530: 2020 2020 2020 2020 6173 7365 7274 6572          asserter
-0000f540: 2e61 7373 6572 745f 280a 2020 2020 2020  .assert_(.      
-0000f550: 2020 2020 2020 7371 6c61 6c63 6865 6d79        sqlalchemy
-0000f560: 2e74 6573 7469 6e67 2e61 7373 6572 7473  .testing.asserts
-0000f570: 716c 2e43 7572 736f 7253 514c 280a 2020  ql.CursorSQL(.  
-0000f580: 2020 2020 2020 2020 2020 2020 2020 2253                "S
-0000f590: 454c 4543 5420 736f 6d65 5f74 6162 6c65  ELECT some_table
-0000f5a0: 2e69 6420 5c6e 4652 4f4d 2073 6f6d 655f  .id \nFROM some_
-0000f5b0: 7461 626c 6520 2220 225c 6e57 4845 5245  table " "\nWHERE
-0000f5c0: 2073 6f6d 655f 7461 626c 652e 7820 3d20   some_table.x = 
-0000f5d0: 3130 222c 0a20 2020 2020 2020 2020 2020  10",.           
-0000f5e0: 2020 2020 205b 5d20 6966 2063 6f6e 6669       [] if confi
-0000f5f0: 672e 6462 2e64 6961 6c65 6374 2e70 6f73  g.db.dialect.pos
-0000f600: 6974 696f 6e61 6c20 656c 7365 207b 7d2c  itional else {},
-0000f610: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000f620: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-0000f630: 6620 7465 7374 5f65 7865 6375 7465 5f65  f test_execute_e
-0000f640: 7870 616e 6469 6e67 5f70 6c75 735f 6c69  xpanding_plus_li
-0000f650: 7465 7261 6c5f 6578 6563 7574 6528 7365  teral_execute(se
-0000f660: 6c66 293a 0a20 2020 2020 2020 2074 6162  lf):.        tab
-0000f670: 6c65 203d 2073 656c 662e 7461 626c 6573  le = self.tables
-0000f680: 2e73 6f6d 655f 7461 626c 650a 0a20 2020  .some_table..   
-0000f690: 2020 2020 2073 746d 7420 3d20 7365 6c65       stmt = sele
-0000f6a0: 6374 2874 6162 6c65 2e63 2e69 6429 2e77  ct(table.c.id).w
-0000f6b0: 6865 7265 280a 2020 2020 2020 2020 2020  here(.          
-0000f6c0: 2020 7461 626c 652e 632e 782e 696e 5f28    table.c.x.in_(
-0000f6d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f6e0: 2073 716c 616c 6368 656d 792e 6269 6e64   sqlalchemy.bind
-0000f6f0: 7061 7261 6d28 2271 222c 2065 7870 616e  param("q", expan
-0000f700: 6469 6e67 3d54 7275 652c 206c 6974 6572  ding=True, liter
-0000f710: 616c 5f65 7865 6375 7465 3d54 7275 6529  al_execute=True)
-0000f720: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000f730: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000f740: 2020 7769 7468 2073 656c 662e 7371 6c5f    with self.sql_
-0000f750: 6578 6563 7574 696f 6e5f 6173 7365 7274  execution_assert
-0000f760: 6572 2829 2061 7320 6173 7365 7274 6572  er() as asserter
-0000f770: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
-0000f780: 7468 2063 6f6e 6669 672e 6462 2e63 6f6e  th config.db.con
-0000f790: 6e65 6374 2829 2061 7320 636f 6e6e 3a0a  nect() as conn:.
-0000f7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7b0: 636f 6e6e 2e65 7865 6375 7465 2873 746d  conn.execute(stm
-0000f7c0: 742c 2064 6963 7428 713d 5b35 2c20 362c  t, dict(q=[5, 6,
-0000f7d0: 2037 5d29 290a 0a20 2020 2020 2020 2061   7]))..        a
-0000f7e0: 7373 6572 7465 722e 6173 7365 7274 5f28  sserter.assert_(
-0000f7f0: 0a20 2020 2020 2020 2020 2020 2073 716c  .            sql
-0000f800: 616c 6368 656d 792e 7465 7374 696e 672e  alchemy.testing.
-0000f810: 6173 7365 7274 7371 6c2e 4375 7273 6f72  assertsql.Cursor
-0000f820: 5351 4c28 0a20 2020 2020 2020 2020 2020  SQL(.           
-0000f830: 2020 2020 2022 5345 4c45 4354 2073 6f6d       "SELECT som
-0000f840: 655f 7461 626c 652e 6964 205c 6e46 524f  e_table.id \nFRO
-0000f850: 4d20 736f 6d65 5f74 6162 6c65 2022 0a20  M some_table ". 
-0000f860: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000f870: 5c6e 5748 4552 4520 736f 6d65 5f74 6162  \nWHERE some_tab
-0000f880: 6c65 2e78 2049 4e20 2835 2c20 362c 2037  le.x IN (5, 6, 7
-0000f890: 2922 2c0a 2020 2020 2020 2020 2020 2020  )",.            
-0000f8a0: 2020 2020 5b5d 2069 6620 636f 6e66 6967      [] if config
-0000f8b0: 2e64 622e 6469 616c 6563 742e 706f 7369  .db.dialect.posi
-0000f8c0: 7469 6f6e 616c 2065 6c73 6520 7b7d 2c0a  tional else {},.
-0000f8d0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000f8e0: 2020 2020 2020 290a 0a20 2020 2040 7465        )..    @te
-0000f8f0: 7374 696e 672e 7265 7175 6972 6573 2e74  sting.requires.t
-0000f900: 7570 6c65 5f69 6e0a 2020 2020 6465 6620  uple_in.    def 
-0000f910: 7465 7374 5f65 7865 6375 7465 5f74 7570  test_execute_tup
-0000f920: 6c65 5f65 7870 616e 6469 6e67 5f70 6c75  le_expanding_plu
-0000f930: 735f 6c69 7465 7261 6c5f 6578 6563 7574  s_literal_execut
-0000f940: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-0000f950: 2074 6162 6c65 203d 2073 656c 662e 7461   table = self.ta
-0000f960: 626c 6573 2e73 6f6d 655f 7461 626c 650a  bles.some_table.
-0000f970: 0a20 2020 2020 2020 2073 746d 7420 3d20  .        stmt = 
-0000f980: 7365 6c65 6374 2874 6162 6c65 2e63 2e69  select(table.c.i
-0000f990: 6429 2e77 6865 7265 280a 2020 2020 2020  d).where(.      
-0000f9a0: 2020 2020 2020 7371 6c61 6c63 6865 6d79        sqlalchemy
-0000f9b0: 2e74 7570 6c65 5f28 7461 626c 652e 632e  .tuple_(table.c.
-0000f9c0: 782c 2074 6162 6c65 2e63 2e79 292e 696e  x, table.c.y).in
-0000f9d0: 5f28 0a20 2020 2020 2020 2020 2020 2020  _(.             
-0000f9e0: 2020 2073 716c 616c 6368 656d 792e 6269     sqlalchemy.bi
-0000f9f0: 6e64 7061 7261 6d28 2271 222c 2065 7870  ndparam("q", exp
-0000fa00: 616e 6469 6e67 3d54 7275 652c 206c 6974  anding=True, lit
-0000fa10: 6572 616c 5f65 7865 6375 7465 3d54 7275  eral_execute=Tru
-0000fa20: 6529 0a20 2020 2020 2020 2020 2020 2029  e).            )
-0000fa30: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0000fa40: 2020 2020 7769 7468 2073 656c 662e 7371      with self.sq
-0000fa50: 6c5f 6578 6563 7574 696f 6e5f 6173 7365  l_execution_asse
-0000fa60: 7274 6572 2829 2061 7320 6173 7365 7274  rter() as assert
-0000fa70: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
-0000fa80: 7769 7468 2063 6f6e 6669 672e 6462 2e63  with config.db.c
-0000fa90: 6f6e 6e65 6374 2829 2061 7320 636f 6e6e  onnect() as conn
-0000faa0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000fab0: 2020 636f 6e6e 2e65 7865 6375 7465 2873    conn.execute(s
-0000fac0: 746d 742c 2064 6963 7428 713d 5b28 352c  tmt, dict(q=[(5,
-0000fad0: 2031 3029 2c20 2831 322c 2031 3829 5d29   10), (12, 18)])
-0000fae0: 290a 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-0000faf0: 7465 722e 6173 7365 7274 5f28 0a20 2020  ter.assert_(.   
-0000fb00: 2020 2020 2020 2020 2073 716c 616c 6368           sqlalch
-0000fb10: 656d 792e 7465 7374 696e 672e 6173 7365  emy.testing.asse
-0000fb20: 7274 7371 6c2e 4375 7273 6f72 5351 4c28  rtsql.CursorSQL(
-0000fb30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fb40: 2022 5345 4c45 4354 2073 6f6d 655f 7461   "SELECT some_ta
-0000fb50: 626c 652e 6964 205c 6e46 524f 4d20 736f  ble.id \nFROM so
-0000fb60: 6d65 5f74 6162 6c65 2022 0a20 2020 2020  me_table ".     
-0000fb70: 2020 2020 2020 2020 2020 2022 5c6e 5748             "\nWH
-0000fb80: 4552 4520 2873 6f6d 655f 7461 626c 652e  ERE (some_table.
-0000fb90: 782c 2073 6f6d 655f 7461 626c 652e 7929  x, some_table.y)
-0000fba0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-0000fbb0: 2020 2022 494e 2028 2573 2835 2c20 3130     "IN (%s(5, 10
-0000fbc0: 292c 2028 3132 2c20 3138 2929 220a 2020  ), (12, 18))".  
-0000fbd0: 2020 2020 2020 2020 2020 2020 2020 2520                % 
-0000fbe0: 2822 5641 4c55 4553 2022 2069 6620 636f  ("VALUES " if co
-0000fbf0: 6e66 6967 2e64 622e 6469 616c 6563 742e  nfig.db.dialect.
-0000fc00: 7475 706c 655f 696e 5f76 616c 7565 7320  tuple_in_values 
-0000fc10: 656c 7365 2022 2229 2c0a 2020 2020 2020  else ""),.      
-0000fc20: 2020 2020 2020 2020 2020 2829 2069 6620            () if 
-0000fc30: 636f 6e66 6967 2e64 622e 6469 616c 6563  config.db.dialec
-0000fc40: 742e 706f 7369 7469 6f6e 616c 2065 6c73  t.positional els
-0000fc50: 6520 7b7d 2c0a 2020 2020 2020 2020 2020  e {},.          
-0000fc60: 2020 290a 2020 2020 2020 2020 290a 0a20    ).        ).. 
-0000fc70: 2020 2040 7465 7374 696e 672e 7265 7175     @testing.requ
-0000fc80: 6972 6573 2e74 7570 6c65 5f69 6e0a 2020  ires.tuple_in.  
-0000fc90: 2020 6465 6620 7465 7374 5f65 7865 6375    def test_execu
-0000fca0: 7465 5f74 7570 6c65 5f65 7870 616e 6469  te_tuple_expandi
-0000fcb0: 6e67 5f70 6c75 735f 6c69 7465 7261 6c5f  ng_plus_literal_
-0000fcc0: 6865 7465 726f 6765 6e65 6f75 735f 6578  heterogeneous_ex
-0000fcd0: 6563 7574 6528 7365 6c66 293a 0a20 2020  ecute(self):.   
-0000fce0: 2020 2020 2074 6162 6c65 203d 2073 656c       table = sel
-0000fcf0: 662e 7461 626c 6573 2e73 6f6d 655f 7461  f.tables.some_ta
-0000fd00: 626c 650a 0a20 2020 2020 2020 2073 746d  ble..        stm
-0000fd10: 7420 3d20 7365 6c65 6374 2874 6162 6c65  t = select(table
-0000fd20: 2e63 2e69 6429 2e77 6865 7265 280a 2020  .c.id).where(.  
-0000fd30: 2020 2020 2020 2020 2020 7371 6c61 6c63            sqlalc
-0000fd40: 6865 6d79 2e74 7570 6c65 5f28 7461 626c  hemy.tuple_(tabl
-0000fd50: 652e 632e 782c 2074 6162 6c65 2e63 2e7a  e.c.x, table.c.z
-0000fd60: 292e 696e 5f28 0a20 2020 2020 2020 2020  ).in_(.         
-0000fd70: 2020 2020 2020 2073 716c 616c 6368 656d         sqlalchem
-0000fd80: 792e 6269 6e64 7061 7261 6d28 2271 222c  y.bindparam("q",
-0000fd90: 2065 7870 616e 6469 6e67 3d54 7275 652c   expanding=True,
-0000fda0: 206c 6974 6572 616c 5f65 7865 6375 7465   literal_execute
-0000fdb0: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-0000fdc0: 2020 2029 0a20 2020 2020 2020 2029 0a0a     ).        )..
-0000fdd0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-0000fde0: 662e 7371 6c5f 6578 6563 7574 696f 6e5f  f.sql_execution_
-0000fdf0: 6173 7365 7274 6572 2829 2061 7320 6173  asserter() as as
-0000fe00: 7365 7274 6572 3a0a 2020 2020 2020 2020  serter:.        
-0000fe10: 2020 2020 7769 7468 2063 6f6e 6669 672e      with config.
-0000fe20: 6462 2e63 6f6e 6e65 6374 2829 2061 7320  db.connect() as 
-0000fe30: 636f 6e6e 3a0a 2020 2020 2020 2020 2020  conn:.          
-0000fe40: 2020 2020 2020 636f 6e6e 2e65 7865 6375        conn.execu
-0000fe50: 7465 2873 746d 742c 2064 6963 7428 713d  te(stmt, dict(q=
-0000fe60: 5b28 352c 2022 7a31 2229 2c20 2831 322c  [(5, "z1"), (12,
-0000fe70: 2022 7a33 2229 5d29 290a 0a20 2020 2020   "z3")]))..     
-0000fe80: 2020 2061 7373 6572 7465 722e 6173 7365     asserter.asse
-0000fe90: 7274 5f28 0a20 2020 2020 2020 2020 2020  rt_(.           
-0000fea0: 2073 716c 616c 6368 656d 792e 7465 7374   sqlalchemy.test
-0000feb0: 696e 672e 6173 7365 7274 7371 6c2e 4375  ing.assertsql.Cu
-0000fec0: 7273 6f72 5351 4c28 0a20 2020 2020 2020  rsorSQL(.       
-0000fed0: 2020 2020 2020 2020 2022 5345 4c45 4354           "SELECT
-0000fee0: 2073 6f6d 655f 7461 626c 652e 6964 205c   some_table.id \
-0000fef0: 6e46 524f 4d20 736f 6d65 5f74 6162 6c65  nFROM some_table
-0000ff00: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-0000ff10: 2020 2022 5c6e 5748 4552 4520 2873 6f6d     "\nWHERE (som
-0000ff20: 655f 7461 626c 652e 782c 2073 6f6d 655f  e_table.x, some_
-0000ff30: 7461 626c 652e 7a29 2022 0a20 2020 2020  table.z) ".     
-0000ff40: 2020 2020 2020 2020 2020 2022 494e 2028             "IN (
-0000ff50: 2573 2835 2c20 277a 3127 292c 2028 3132  %s(5, 'z1'), (12
-0000ff60: 2c20 277a 3327 2929 220a 2020 2020 2020  , 'z3'))".      
-0000ff70: 2020 2020 2020 2020 2020 2520 2822 5641            % ("VA
-0000ff80: 4c55 4553 2022 2069 6620 636f 6e66 6967  LUES " if config
-0000ff90: 2e64 622e 6469 616c 6563 742e 7475 706c  .db.dialect.tupl
-0000ffa0: 655f 696e 5f76 616c 7565 7320 656c 7365  e_in_values else
-0000ffb0: 2022 2229 2c0a 2020 2020 2020 2020 2020   ""),.          
-0000ffc0: 2020 2020 2020 2829 2069 6620 636f 6e66        () if conf
-0000ffd0: 6967 2e64 622e 6469 616c 6563 742e 706f  ig.db.dialect.po
-0000ffe0: 7369 7469 6f6e 616c 2065 6c73 6520 7b7d  sitional else {}
-0000fff0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00010000: 2020 2020 2020 2020 290a 0a0a 636c 6173          )...clas
-00010010: 7320 436f 6d70 7574 6564 5265 666c 6563  s ComputedReflec
-00010020: 7469 6f6e 4669 7874 7572 6554 6573 7428  tionFixtureTest(
-00010030: 5f43 6f6d 7075 7465 6452 6566 6c65 6374  _ComputedReflect
-00010040: 696f 6e46 6978 7475 7265 5465 7374 293a  ionFixtureTest):
-00010050: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00010060: 640a 2020 2020 6465 6620 6465 6669 6e65  d.    def define
-00010070: 5f74 6162 6c65 7328 636c 732c 206d 6574  _tables(cls, met
-00010080: 6164 6174 6129 3a0a 2020 2020 2020 2020  adata):.        
-00010090: 2222 2253 5041 4e4e 4552 204f 5645 5252  """SPANNER OVERR
-000100a0: 4944 453a 0a0a 2020 2020 2020 2020 4176  IDE:..        Av
-000100b0: 6f69 6420 7573 696e 6720 6465 6661 756c  oid using defaul
-000100c0: 7420 7661 6c75 6573 2066 6f72 2063 6f6d  t values for com
-000100d0: 7075 7465 6420 636f 6c75 6d6e 732e 0a20  puted columns.. 
-000100e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000100f0: 2020 2054 6162 6c65 280a 2020 2020 2020     Table(.      
-00010100: 2020 2020 2020 2263 6f6d 7075 7465 645f        "computed_
-00010110: 6465 6661 756c 745f 7461 626c 6522 2c0a  default_table",.
-00010120: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
-00010130: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
-00010140: 2020 436f 6c75 6d6e 2822 6964 222c 2049    Column("id", I
-00010150: 6e74 6567 6572 2c20 7072 696d 6172 795f  nteger, primary_
-00010160: 6b65 793d 5472 7565 292c 0a20 2020 2020  key=True),.     
-00010170: 2020 2020 2020 2043 6f6c 756d 6e28 226e         Column("n
-00010180: 6f72 6d61 6c22 2c20 496e 7465 6765 7229  ormal", Integer)
-00010190: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
-000101a0: 6c75 6d6e 2822 636f 6d70 7574 6564 5f63  lumn("computed_c
-000101b0: 6f6c 222c 2049 6e74 6567 6572 2c20 436f  ol", Integer, Co
-000101c0: 6d70 7574 6564 2822 6e6f 726d 616c 202b  mputed("normal +
-000101d0: 2034 3222 2929 2c0a 2020 2020 2020 2020   42")),.        
-000101e0: 2020 2020 436f 6c75 6d6e 2822 7769 7468      Column("with
-000101f0: 5f64 6566 6175 6c74 222c 2049 6e74 6567  _default", Integ
-00010200: 6572 292c 0a20 2020 2020 2020 2029 0a0a  er),.        )..
-00010210: 2020 2020 2020 2020 7420 3d20 5461 626c          t = Tabl
-00010220: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
-00010230: 636f 6d70 7574 6564 5f63 6f6c 756d 6e5f  computed_column_
-00010240: 7461 626c 6522 2c0a 2020 2020 2020 2020  table",.        
-00010250: 2020 2020 6d65 7461 6461 7461 2c0a 2020      metadata,.  
-00010260: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
-00010270: 2822 6964 222c 2049 6e74 6567 6572 2c20  ("id", Integer, 
-00010280: 7072 696d 6172 795f 6b65 793d 5472 7565  primary_key=True
-00010290: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
-000102a0: 6f6c 756d 6e28 226e 6f72 6d61 6c22 2c20  olumn("normal", 
-000102b0: 496e 7465 6765 7229 2c0a 2020 2020 2020  Integer),.      
-000102c0: 2020 2020 2020 436f 6c75 6d6e 2822 636f        Column("co
-000102d0: 6d70 7574 6564 5f6e 6f5f 666c 6167 222c  mputed_no_flag",
-000102e0: 2049 6e74 6567 6572 2c20 436f 6d70 7574   Integer, Comput
-000102f0: 6564 2822 6e6f 726d 616c 202b 2034 3222  ed("normal + 42"
-00010300: 2929 2c0a 2020 2020 2020 2020 290a 0a20  )),.        ).. 
-00010310: 2020 2020 2020 2069 6620 7465 7374 696e         if testin
-00010320: 672e 7265 7175 6972 6573 2e63 6f6d 7075  g.requires.compu
-00010330: 7465 645f 636f 6c75 6d6e 735f 7669 7274  ted_columns_virt
-00010340: 7561 6c2e 656e 6162 6c65 643a 0a20 2020  ual.enabled:.   
-00010350: 2020 2020 2020 2020 2074 2e61 7070 656e           t.appen
-00010360: 645f 636f 6c75 6d6e 280a 2020 2020 2020  d_column(.      
-00010370: 2020 2020 2020 2020 2020 436f 6c75 6d6e            Column
-00010380: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00010390: 2020 2020 2020 2263 6f6d 7075 7465 645f        "computed_
-000103a0: 7669 7274 7561 6c22 2c0a 2020 2020 2020  virtual",.      
-000103b0: 2020 2020 2020 2020 2020 2020 2020 496e                In
-000103c0: 7465 6765 722c 0a20 2020 2020 2020 2020  teger,.         
-000103d0: 2020 2020 2020 2020 2020 2043 6f6d 7075             Compu
-000103e0: 7465 6428 226e 6f72 6d61 6c20 2b20 3222  ted("normal + 2"
-000103f0: 2c20 7065 7273 6973 7465 643d 4661 6c73  , persisted=Fals
-00010400: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-00010410: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00010420: 2020 290a 2020 2020 2020 2020 6966 2074    ).        if t
-00010430: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
-00010440: 636f 6d70 7574 6564 5f63 6f6c 756d 6e73  computed_columns
-00010450: 5f73 746f 7265 642e 656e 6162 6c65 643a  _stored.enabled:
-00010460: 0a20 2020 2020 2020 2020 2020 2074 2e61  .            t.a
-00010470: 7070 656e 645f 636f 6c75 6d6e 280a 2020  ppend_column(.  
-00010480: 2020 2020 2020 2020 2020 2020 2020 436f                Co
-00010490: 6c75 6d6e 280a 2020 2020 2020 2020 2020  lumn(.          
-000104a0: 2020 2020 2020 2020 2020 2263 6f6d 7075            "compu
-000104b0: 7465 645f 7374 6f72 6564 222c 0a20 2020  ted_stored",.   
-000104c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104d0: 2049 6e74 6567 6572 2c0a 2020 2020 2020   Integer,.      
-000104e0: 2020 2020 2020 2020 2020 2020 2020 436f                Co
-000104f0: 6d70 7574 6564 2822 6e6f 726d 616c 202d  mputed("normal -
-00010500: 2034 3222 2c20 7065 7273 6973 7465 643d   42", persisted=
-00010510: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
-00010520: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00010530: 2020 2020 2029 0a0a 0a63 6c61 7373 2043       )...class C
-00010540: 6f6d 7075 7465 6452 6566 6c65 6374 696f  omputedReflectio
-00010550: 6e54 6573 7428 5f43 6f6d 7075 7465 6452  nTest(_ComputedR
-00010560: 6566 6c65 6374 696f 6e54 6573 742c 2043  eflectionTest, C
-00010570: 6f6d 7075 7465 6452 6566 6c65 6374 696f  omputedReflectio
-00010580: 6e46 6978 7475 7265 5465 7374 293a 0a20  nFixtureTest):. 
-00010590: 2020 2040 7465 7374 696e 672e 7265 7175     @testing.requ
-000105a0: 6972 6573 2e73 6368 656d 6173 0a20 2020  ires.schemas.   
-000105b0: 2064 6566 2074 6573 745f 6765 745f 636f   def test_get_co
-000105c0: 6c75 6d6e 5f72 6574 7572 6e73 5f70 6572  lumn_returns_per
-000105d0: 7369 7374 6564 5f77 6974 685f 7363 6865  sisted_with_sche
-000105e0: 6d61 2873 656c 6629 3a0a 2020 2020 2020  ma(self):.      
-000105f0: 2020 696e 7370 203d 2069 6e73 7065 6374    insp = inspect
-00010600: 2863 6f6e 6669 672e 6462 290a 0a20 2020  (config.db)..   
-00010610: 2020 2020 2063 6f6c 7320 3d20 696e 7370       cols = insp
-00010620: 2e67 6574 5f63 6f6c 756d 6e73 2822 636f  .get_columns("co
-00010630: 6d70 7574 6564 5f63 6f6c 756d 6e5f 7461  mputed_column_ta
-00010640: 626c 6522 2c20 7363 6865 6d61 3d63 6f6e  ble", schema=con
-00010650: 6669 672e 7465 7374 5f73 6368 656d 6129  fig.test_schema)
-00010660: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00010670: 7b63 5b22 6e61 6d65 225d 3a20 6320 666f  {c["name"]: c fo
-00010680: 7220 6320 696e 2063 6f6c 737d 0a0a 2020  r c in cols}..  
-00010690: 2020 2020 2020 7365 6c66 2e63 6865 636b        self.check
-000106a0: 5f63 6f6c 756d 6e28 0a20 2020 2020 2020  _column(.       
-000106b0: 2020 2020 2064 6174 612c 0a20 2020 2020       data,.     
-000106c0: 2020 2020 2020 2022 636f 6d70 7574 6564         "computed
-000106d0: 5f6e 6f5f 666c 6167 222c 0a20 2020 2020  _no_flag",.     
-000106e0: 2020 2020 2020 2022 6e6f 726d 616c 2b34         "normal+4
-000106f0: 3222 2c0a 2020 2020 2020 2020 2020 2020  2",.            
-00010700: 7465 7374 696e 672e 7265 7175 6972 6573  testing.requires
-00010710: 2e63 6f6d 7075 7465 645f 636f 6c75 6d6e  .computed_column
-00010720: 735f 6465 6661 756c 745f 7065 7273 6973  s_default_persis
-00010730: 7465 642e 656e 6162 6c65 642c 0a20 2020  ted.enabled,.   
-00010740: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
-00010750: 6620 7465 7374 696e 672e 7265 7175 6972  f testing.requir
-00010760: 6573 2e63 6f6d 7075 7465 645f 636f 6c75  es.computed_colu
-00010770: 6d6e 735f 7669 7274 7561 6c2e 656e 6162  mns_virtual.enab
-00010780: 6c65 643a 0a20 2020 2020 2020 2020 2020  led:.           
-00010790: 2073 656c 662e 6368 6563 6b5f 636f 6c75   self.check_colu
-000107a0: 6d6e 280a 2020 2020 2020 2020 2020 2020  mn(.            
-000107b0: 2020 2020 6461 7461 2c0a 2020 2020 2020      data,.      
-000107c0: 2020 2020 2020 2020 2020 2263 6f6d 7075            "compu
-000107d0: 7465 645f 7669 7274 7561 6c22 2c0a 2020  ted_virtual",.  
-000107e0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-000107f0: 6f72 6d61 6c2f 3222 2c0a 2020 2020 2020  ormal/2",.      
-00010800: 2020 2020 2020 2020 2020 4661 6c73 652c            False,
-00010810: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00010820: 2020 2020 2020 2069 6620 7465 7374 696e         if testin
-00010830: 672e 7265 7175 6972 6573 2e63 6f6d 7075  g.requires.compu
-00010840: 7465 645f 636f 6c75 6d6e 735f 7374 6f72  ted_columns_stor
-00010850: 6564 2e65 6e61 626c 6564 3a0a 2020 2020  ed.enabled:.    
-00010860: 2020 2020 2020 2020 7365 6c66 2e63 6865          self.che
-00010870: 636b 5f63 6f6c 756d 6e28 0a20 2020 2020  ck_column(.     
-00010880: 2020 2020 2020 2020 2020 2064 6174 612c             data,
-00010890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000108a0: 2022 636f 6d70 7574 6564 5f73 746f 7265   "computed_store
-000108b0: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
-000108c0: 2020 2020 226e 6f72 6d61 6c2d 3432 222c      "normal-42",
-000108d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000108e0: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
-000108f0: 2020 2029 0a0a 2020 2020 4070 7974 6573     )..    @pytes
-00010900: 742e 6d61 726b 2e73 6b69 7028 2244 6566  t.mark.skip("Def
-00010910: 6175 6c74 2076 616c 7565 7320 6172 6520  ault values are 
-00010920: 6e6f 7420 7375 7070 6f72 7465 642e 2229  not supported.")
-00010930: 0a20 2020 2064 6566 2074 6573 745f 636f  .    def test_co
-00010940: 6d70 7574 6564 5f63 6f6c 5f64 6566 6175  mputed_col_defau
-00010950: 6c74 5f6e 6f74 5f73 6574 2873 656c 6629  lt_not_set(self)
-00010960: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-00010970: 2020 2020 6465 6620 7465 7374 5f67 6574      def test_get
-00010980: 5f63 6f6c 756d 6e5f 7265 7475 726e 735f  _column_returns_
-00010990: 636f 6d70 7574 6564 2873 656c 6629 3a0a  computed(self):.
-000109a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000109b0: 2020 2020 5350 414e 4e45 5220 4f56 4552      SPANNER OVER
-000109c0: 5249 4445 3a0a 0a20 2020 2020 2020 2049  RIDE:..        I
-000109d0: 6e20 5370 616e 6e65 7220 616c 6c20 7468  n Spanner all th
-000109e0: 6520 6765 6e65 7261 7465 6420 636f 6c75  e generated colu
-000109f0: 6d6e 7320 6172 6520 5354 4f52 4544 2c0a  mns are STORED,.
-00010a00: 2020 2020 2020 2020 6d65 616e 696e 6720          meaning 
-00010a10: 7468 6572 6520 6172 6520 6e6f 2070 6572  there are no per
-00010a20: 7369 7374 6564 2061 6e64 206e 6f74 2070  sisted and not p
-00010a30: 6572 7369 7374 6564 0a20 2020 2020 2020  ersisted.       
-00010a40: 2028 696e 2074 6865 2074 6572 6d73 206f   (in the terms o
-00010a50: 6620 7468 6520 5351 4c41 6c63 6865 6d79  f the SQLAlchemy
-00010a60: 2920 636f 6c75 6d6e 732e 2054 6865 0a20  ) columns. The. 
-00010a70: 2020 2020 2020 206d 6574 686f 6420 6f76         method ov
-00010a80: 6572 7269 6465 206f 6d69 7473 2074 6865  erride omits the
-00010a90: 2070 6572 7369 7374 656e 6365 2072 6566   persistence ref
-00010aa0: 6c65 6374 696f 6e20 6368 6563 6b73 2e0a  lection checks..
-00010ab0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00010ac0: 2020 2020 696e 7370 203d 2069 6e73 7065      insp = inspe
-00010ad0: 6374 2863 6f6e 6669 672e 6462 290a 0a20  ct(config.db).. 
-00010ae0: 2020 2020 2020 2063 6f6c 7320 3d20 696e         cols = in
-00010af0: 7370 2e67 6574 5f63 6f6c 756d 6e73 2822  sp.get_columns("
-00010b00: 636f 6d70 7574 6564 5f64 6566 6175 6c74  computed_default
-00010b10: 5f74 6162 6c65 2229 0a20 2020 2020 2020  _table").       
-00010b20: 2064 6174 6120 3d20 7b63 5b22 6e61 6d65   data = {c["name
-00010b30: 225d 3a20 6320 666f 7220 6320 696e 2063  "]: c for c in c
-00010b40: 6f6c 737d 0a20 2020 2020 2020 2066 6f72  ols}.        for
-00010b50: 206b 6579 2069 6e20 2822 6964 222c 2022   key in ("id", "
-00010b60: 6e6f 726d 616c 222c 2022 7769 7468 5f64  normal", "with_d
-00010b70: 6566 6175 6c74 2229 3a0a 2020 2020 2020  efault"):.      
-00010b80: 2020 2020 2020 6973 5f74 7275 6528 2263        is_true("c
-00010b90: 6f6d 7075 7465 6422 206e 6f74 2069 6e20  omputed" not in 
-00010ba0: 6461 7461 5b6b 6579 5d29 0a20 2020 2020  data[key]).     
-00010bb0: 2020 2063 6f6d 7044 6174 6120 3d20 6461     compData = da
-00010bc0: 7461 5b22 636f 6d70 7574 6564 5f63 6f6c  ta["computed_col
-00010bd0: 225d 0a20 2020 2020 2020 2069 735f 7472  "].        is_tr
-00010be0: 7565 2822 636f 6d70 7574 6564 2220 696e  ue("computed" in
-00010bf0: 2063 6f6d 7044 6174 6129 0a20 2020 2020   compData).     
-00010c00: 2020 2069 735f 7472 7565 2822 7371 6c74     is_true("sqlt
-00010c10: 6578 7422 2069 6e20 636f 6d70 4461 7461  ext" in compData
-00010c20: 5b22 636f 6d70 7574 6564 225d 290a 2020  ["computed"]).  
-00010c30: 2020 2020 2020 6571 5f28 7365 6c66 2e6e        eq_(self.n
-00010c40: 6f72 6d61 6c69 7a65 2863 6f6d 7044 6174  ormalize(compDat
-00010c50: 615b 2263 6f6d 7075 7465 6422 5d5b 2273  a["computed"]["s
-00010c60: 716c 7465 7874 225d 292c 2022 6e6f 726d  qltext"]), "norm
-00010c70: 616c 2b34 3222 290a 0a20 2020 2064 6566  al+42")..    def
-00010c80: 2074 6573 745f 6372 6561 7465 5f6e 6f74   test_create_not
-00010c90: 5f6e 756c 6c5f 636f 6d70 7574 6564 5f63  _null_computed_c
-00010ca0: 6f6c 756d 6e28 7365 6c66 293a 0a20 2020  olumn(self):.   
-00010cb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00010cc0: 2053 5041 4e4e 4552 2054 4553 543a 0a0a   SPANNER TEST:..
-00010cd0: 2020 2020 2020 2020 4368 6563 6b20 7468          Check th
-00010ce0: 6174 206f 6e20 6372 6561 7469 6e67 2061  at on creating a
-00010cf0: 2063 6f6d 7075 7465 6420 636f 6c75 6d6e   computed column
-00010d00: 2077 6974 6820 6120 4e4f 5420 4e55 4c4c   with a NOT NULL
-00010d10: 0a20 2020 2020 2020 2063 6c61 7573 6520  .        clause 
-00010d20: 7468 6520 636c 6175 7365 2069 7320 7365  the clause is se
-00010d30: 7420 696e 2066 726f 6e74 206f 6620 7468  t in front of th
-00010d40: 6520 636f 6d70 7574 6564 2063 6f6c 756d  e computed colum
-00010d50: 6e0a 2020 2020 2020 2020 7374 6174 656d  n.        statem
-00010d60: 656e 7420 6465 6669 6e69 7469 6f6e 2061  ent definition a
-00010d70: 6e64 2064 6f65 736e 2774 2063 6175 7365  nd doesn't cause
-00010d80: 2066 6169 6c75 7265 732e 0a20 2020 2020   failures..     
-00010d90: 2020 2022 2222 0a20 2020 2020 2020 2065     """.        e
-00010da0: 6e67 696e 6520 3d20 6372 6561 7465 5f65  ngine = create_e
-00010db0: 6e67 696e 6528 6765 745f 6462 5f75 726c  ngine(get_db_url
-00010dc0: 2829 290a 2020 2020 2020 2020 6d65 7461  ()).        meta
-00010dd0: 6461 7461 203d 204d 6574 6144 6174 6128  data = MetaData(
-00010de0: 6269 6e64 3d65 6e67 696e 6529 0a0a 2020  bind=engine)..  
-00010df0: 2020 2020 2020 5461 626c 6528 0a20 2020        Table(.   
-00010e00: 2020 2020 2020 2020 2022 5369 6e67 6572           "Singer
-00010e10: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-00010e20: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
-00010e30: 2020 2020 2020 436f 6c75 6d6e 2822 5369        Column("Si
-00010e40: 6e67 6572 4964 222c 2053 7472 696e 6728  ngerId", String(
-00010e50: 3336 292c 2070 7269 6d61 7279 5f6b 6579  36), primary_key
-00010e60: 3d54 7275 652c 206e 756c 6c61 626c 653d  =True, nullable=
-00010e70: 4661 6c73 6529 2c0a 2020 2020 2020 2020  False),.        
-00010e80: 2020 2020 436f 6c75 6d6e 2822 4669 7273      Column("Firs
-00010e90: 744e 616d 6522 2c20 5374 7269 6e67 2832  tName", String(2
-00010ea0: 3030 2929 2c0a 2020 2020 2020 2020 2020  00)),.          
-00010eb0: 2020 436f 6c75 6d6e 2822 4c61 7374 4e61    Column("LastNa
-00010ec0: 6d65 222c 2053 7472 696e 6728 3230 3029  me", String(200)
-00010ed0: 2c20 6e75 6c6c 6162 6c65 3d46 616c 7365  , nullable=False
-00010ee0: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
-00010ef0: 6f6c 756d 6e28 0a20 2020 2020 2020 2020  olumn(.         
-00010f00: 2020 2020 2020 2022 4675 6c6c 4e61 6d65         "FullName
-00010f10: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00010f20: 2020 2053 7472 696e 6728 3430 3029 2c0a     String(400),.
-00010f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f40: 436f 6d70 7574 6564 2822 434f 414c 4553  Computed("COALES
-00010f50: 4345 2846 6972 7374 4e61 6d65 207c 7c20  CE(FirstName || 
-00010f60: 2720 272c 2027 2729 207c 7c20 4c61 7374  ' ', '') || Last
-00010f70: 4e61 6d65 2229 2c0a 2020 2020 2020 2020  Name"),.        
-00010f80: 2020 2020 2020 2020 6e75 6c6c 6162 6c65          nullable
-00010f90: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-00010fa0: 2020 2020 292c 0a20 2020 2020 2020 2029      ),.        )
-00010fb0: 0a0a 2020 2020 2020 2020 6d65 7461 6461  ..        metada
-00010fc0: 7461 2e63 7265 6174 655f 616c 6c28 656e  ta.create_all(en
-00010fd0: 6769 6e65 290a 0a0a 4070 7974 6573 742e  gine)...@pytest.
-00010fe0: 6d61 726b 2e73 6b69 7069 6628 0a20 2020  mark.skipif(.   
-00010ff0: 2062 6f6f 6c28 6f73 2e65 6e76 6972 6f6e   bool(os.environ
-00011000: 2e67 6574 2822 5350 414e 4e45 525f 454d  .get("SPANNER_EM
-00011010: 554c 4154 4f52 5f48 4f53 5422 2929 2c20  ULATOR_HOST")), 
-00011020: 7265 6173 6f6e 3d22 536b 6970 7065 6420  reason="Skipped 
-00011030: 6f6e 2065 6d75 6c61 746f 7222 0a29 0a63  on emulator".).c
-00011040: 6c61 7373 204a 534f 4e54 6573 7428 5f4a  lass JSONTest(_J
-00011050: 534f 4e54 6573 7429 3a0a 2020 2020 4070  SONTest):.    @p
-00011060: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
-00011070: 2256 616c 7565 7320 7769 7468 6f75 7420  "Values without 
-00011080: 6b65 7973 2061 7265 206e 6f74 2073 7570  keys are not sup
-00011090: 706f 7274 6564 2e22 290a 2020 2020 6465  ported.").    de
-000110a0: 6620 7465 7374 5f73 696e 676c 655f 656c  f test_single_el
-000110b0: 656d 656e 745f 726f 756e 645f 7472 6970  ement_round_trip
-000110c0: 2873 656c 662c 2065 6c65 6d65 6e74 293a  (self, element):
-000110d0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-000110e0: 2020 2064 6566 205f 7465 7374 5f72 6f75     def _test_rou
-000110f0: 6e64 5f74 7269 7028 7365 6c66 2c20 6461  nd_trip(self, da
-00011100: 7461 5f65 6c65 6d65 6e74 293a 0a20 2020  ta_element):.   
-00011110: 2020 2020 2064 6174 615f 7461 626c 6520       data_table 
-00011120: 3d20 7365 6c66 2e74 6162 6c65 732e 6461  = self.tables.da
-00011130: 7461 5f74 6162 6c65 0a0a 2020 2020 2020  ta_table..      
-00011140: 2020 636f 6e66 6967 2e64 622e 6578 6563    config.db.exec
-00011150: 7574 6528 0a20 2020 2020 2020 2020 2020  ute(.           
-00011160: 2064 6174 615f 7461 626c 652e 696e 7365   data_table.inse
-00011170: 7274 2829 2c0a 2020 2020 2020 2020 2020  rt(),.          
-00011180: 2020 7b22 6964 223a 2072 616e 646f 6d2e    {"id": random.
-00011190: 7261 6e64 696e 7428 312c 2031 3030 3030  randint(1, 10000
-000111a0: 3030 3030 292c 2022 6e61 6d65 223a 2022  0000), "name": "
-000111b0: 726f 7731 222c 2022 6461 7461 223a 2064  row1", "data": d
-000111c0: 6174 615f 656c 656d 656e 747d 2c0a 2020  ata_element},.  
-000111d0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-000111e0: 2072 6f77 203d 2063 6f6e 6669 672e 6462   row = config.db
-000111f0: 2e65 7865 6375 7465 2873 656c 6563 7428  .execute(select(
-00011200: 5b64 6174 615f 7461 626c 652e 632e 6461  [data_table.c.da
-00011210: 7461 5d29 292e 6669 7273 7428 290a 0a20  ta])).first().. 
-00011220: 2020 2020 2020 2065 715f 2872 6f77 2c20         eq_(row, 
-00011230: 2864 6174 615f 656c 656d 656e 742c 2929  (data_element,))
-00011240: 0a0a 2020 2020 6465 6620 7465 7374 5f75  ..    def test_u
-00011250: 6e69 636f 6465 5f72 6f75 6e64 5f74 7269  nicode_round_tri
-00011260: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-00011270: 2023 206e 6f74 6520 7765 2069 6e63 6c75   # note we inclu
-00011280: 6465 2055 6e69 636f 6465 2073 7570 706c  de Unicode suppl
-00011290: 656d 656e 7461 7279 2063 6861 7261 6374  ementary charact
-000112a0: 6572 7320 6173 2077 656c 6c0a 2020 2020  ers as well.    
-000112b0: 2020 2020 7769 7468 2063 6f6e 6669 672e      with config.
-000112c0: 6462 2e63 6f6e 6e65 6374 2829 2061 7320  db.connect() as 
-000112d0: 636f 6e6e 3a0a 2020 2020 2020 2020 2020  conn:.          
-000112e0: 2020 636f 6e6e 2e65 7865 6375 7465 280a    conn.execute(.
-000112f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011300: 7365 6c66 2e74 6162 6c65 732e 6461 7461  self.tables.data
-00011310: 5f74 6162 6c65 2e69 6e73 6572 7428 292c  _table.insert(),
-00011320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011330: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00011340: 2020 2020 2020 2022 6964 223a 2072 616e         "id": ran
-00011350: 646f 6d2e 7261 6e64 696e 7428 312c 2031  dom.randint(1, 1
-00011360: 3030 3030 3030 3030 292c 0a20 2020 2020  00000000),.     
-00011370: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00011380: 6e61 6d65 223a 2022 7231 222c 0a20 2020  name": "r1",.   
-00011390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113a0: 2022 6461 7461 223a 207b 0a20 2020 2020   "data": {.     
-000113b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113c0: 2020 2075 7469 6c2e 7528 2272 c3a9 7665     util.u("r..ve
-000113d0: f09f 908d 2069 6c6c c3a9 2229 3a20 7574  .... ill.."): ut
-000113e0: 696c 2e75 2822 72c3 a976 65f0 9f90 8d20  il.u("r..ve.... 
-000113f0: 696c 6cc3 a922 292c 0a20 2020 2020 2020  ill.."),.       
-00011400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011410: 2022 6461 7461 223a 207b 226b 3122 3a20   "data": {"k1": 
-00011420: 7574 696c 2e75 2822 6472 c3b4 6cf0 9f90  util.u("dr..l...
-00011430: 8d65 2229 7d2c 0a20 2020 2020 2020 2020  .e")},.         
-00011440: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00011450: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-00011460: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00011470: 2020 2020 2020 2020 2020 2020 6571 5f28              eq_(
-00011480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011490: 2063 6f6e 6e2e 7363 616c 6172 2873 656c   conn.scalar(sel
-000114a0: 6563 7428 5b73 656c 662e 7461 626c 6573  ect([self.tables
-000114b0: 2e64 6174 615f 7461 626c 652e 632e 6461  .data_table.c.da
-000114c0: 7461 5d29 292c 0a20 2020 2020 2020 2020  ta])),.         
-000114d0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-000114e0: 2020 2020 2020 2020 2020 2020 2075 7469               uti
-000114f0: 6c2e 7528 2272 c3a9 7665 f09f 908d 2069  l.u("r..ve.... i
-00011500: 6c6c c3a9 2229 3a20 7574 696c 2e75 2822  ll.."): util.u("
-00011510: 72c3 a976 65f0 9f90 8d20 696c 6cc3 a922  r..ve.... ill.."
-00011520: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00011530: 2020 2020 2020 2022 6461 7461 223a 207b         "data": {
-00011540: 226b 3122 3a20 7574 696c 2e75 2822 6472  "k1": util.u("dr
-00011550: c3b4 6cf0 9f90 8d65 2229 7d2c 0a20 2020  ..l....e")},.   
-00011560: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
-00011570: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00011580: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-00011590: 736b 6970 2822 5061 7261 6d65 7465 7269  skip("Parameteri
-000115a0: 7a65 6420 7479 7065 7320 6172 6520 6e6f  zed types are no
-000115b0: 7420 7375 7070 6f72 7465 642e 2229 0a20  t supported."). 
-000115c0: 2020 2064 6566 2074 6573 745f 6576 616c     def test_eval
-000115d0: 5f6e 6f6e 655f 666c 6167 5f6f 726d 2873  _none_flag_orm(s
-000115e0: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-000115f0: 7373 0a0a 2020 2020 4070 7974 6573 742e  ss..    @pytest.
-00011600: 6d61 726b 2e73 6b69 7028 0a20 2020 2020  mark.skip(.     
-00011610: 2020 2022 5370 616e 6e65 7220 4a53 4f4e     "Spanner JSON
-00011620: 5f56 414c 5545 2829 2061 6c77 6179 7320  _VALUE() always 
-00011630: 7265 7475 726e 7320 5354 5249 4e47 2c22  returns STRING,"
-00011640: 0a20 2020 2020 2020 2022 7468 7573 2c20  .        "thus, 
-00011650: 7468 6973 2074 6573 7420 6361 7365 2063  this test case c
-00011660: 616e 2774 2062 6520 6578 6563 7574 6564  an't be executed
-00011670: 2e22 0a20 2020 2029 0a20 2020 2064 6566  .".    ).    def
-00011680: 2074 6573 745f 696e 6465 785f 7479 7065   test_index_type
-00011690: 645f 636f 6d70 6172 6973 6f6e 2873 656c  d_comparison(sel
-000116a0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-000116b0: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
-000116c0: 726b 2e73 6b69 7028 0a20 2020 2020 2020  rk.skip(.       
-000116d0: 2022 5370 616e 6e65 7220 4a53 4f4e 5f56   "Spanner JSON_V
-000116e0: 414c 5545 2829 2061 6c77 6179 7320 7265  ALUE() always re
-000116f0: 7475 726e 7320 5354 5249 4e47 2c22 0a20  turns STRING,". 
-00011700: 2020 2020 2020 2022 7468 7573 2c20 7468         "thus, th
-00011710: 6973 2074 6573 7420 6361 7365 2063 616e  is test case can
-00011720: 2774 2062 6520 6578 6563 7574 6564 2e22  't be executed."
-00011730: 0a20 2020 2029 0a20 2020 2064 6566 2074  .    ).    def t
-00011740: 6573 745f 7061 7468 5f74 7970 6564 5f63  est_path_typed_c
-00011750: 6f6d 7061 7269 736f 6e28 7365 6c66 293a  omparison(self):
-00011760: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00011770: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-00011780: 736b 6970 2822 4375 7374 6f6d 204a 534f  skip("Custom JSO
-00011790: 4e20 6465 2d2f 7365 7269 616c 697a 6572  N de-/serializer
-000117a0: 7320 6172 6520 6e6f 7420 7375 7070 6f72  s are not suppor
-000117b0: 7465 642e 2229 0a20 2020 2064 6566 2074  ted.").    def t
-000117c0: 6573 745f 726f 756e 645f 7472 6970 5f63  est_round_trip_c
-000117d0: 7573 746f 6d5f 6a73 6f6e 2873 656c 6629  ustom_json(self)
-000117e0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-000117f0: 2020 2020 6465 6620 5f69 6e64 6578 5f66      def _index_f
-00011800: 6978 7475 7265 7328 666e 293a 0a20 2020  ixtures(fn):.   
-00011810: 2020 2020 2066 6e20 3d20 7465 7374 696e       fn = testin
-00011820: 672e 636f 6d62 696e 6174 696f 6e73 280a  g.combinations(.
-00011830: 2020 2020 2020 2020 2020 2020 2822 626f              ("bo
-00011840: 6f6c 6561 6e22 2c20 5472 7565 292c 0a20  olean", True),. 
-00011850: 2020 2020 2020 2020 2020 2028 2262 6f6f             ("boo
-00011860: 6c65 616e 222c 2046 616c 7365 292c 0a20  lean", False),. 
-00011870: 2020 2020 2020 2020 2020 2028 2262 6f6f             ("boo
-00011880: 6c65 616e 222c 204e 6f6e 6529 2c0a 2020  lean", None),.  
-00011890: 2020 2020 2020 2020 2020 2822 7374 7269            ("stri
-000118a0: 6e67 222c 2022 736f 6d65 2073 7472 696e  ng", "some strin
-000118b0: 6722 292c 0a20 2020 2020 2020 2020 2020  g"),.           
-000118c0: 2028 2273 7472 696e 6722 2c20 4e6f 6e65   ("string", None
-000118d0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-000118e0: 2269 6e74 6567 6572 222c 2031 3529 2c0a  "integer", 15),.
-000118f0: 2020 2020 2020 2020 2020 2020 2822 696e              ("in
-00011900: 7465 6765 7222 2c20 3129 2c0a 2020 2020  teger", 1),.    
-00011910: 2020 2020 2020 2020 2822 696e 7465 6765          ("intege
-00011920: 7222 2c20 3029 2c0a 2020 2020 2020 2020  r", 0),.        
-00011930: 2020 2020 2822 696e 7465 6765 7222 2c20      ("integer", 
-00011940: 4e6f 6e65 292c 0a20 2020 2020 2020 2020  None),.         
-00011950: 2020 2028 2266 6c6f 6174 222c 2032 382e     ("float", 28.
-00011960: 3529 2c0a 2020 2020 2020 2020 2020 2020  5),.            
-00011970: 2822 666c 6f61 7422 2c20 4e6f 6e65 292c  ("float", None),
-00011980: 0a20 2020 2020 2020 2020 2020 2069 645f  .            id_
-00011990: 3d22 7361 222c 0a20 2020 2020 2020 2029  ="sa",.        )
-000119a0: 2866 6e29 0a20 2020 2020 2020 2072 6574  (fn).        ret
-000119b0: 7572 6e20 666e 0a0a 2020 2020 405f 696e  urn fn..    @_in
-000119c0: 6465 785f 6669 7874 7572 6573 0a20 2020  dex_fixtures.   
-000119d0: 2064 6566 2074 6573 745f 696e 6465 785f   def test_index_
-000119e0: 7479 7065 645f 6163 6365 7373 2873 656c  typed_access(sel
-000119f0: 662c 2064 6174 6174 7970 652c 2076 616c  f, datatype, val
-00011a00: 7565 293a 0a20 2020 2020 2020 2064 6174  ue):.        dat
-00011a10: 615f 7461 626c 6520 3d20 7365 6c66 2e74  a_table = self.t
-00011a20: 6162 6c65 732e 6461 7461 5f74 6162 6c65  ables.data_table
-00011a30: 0a20 2020 2020 2020 2064 6174 615f 656c  .        data_el
-00011a40: 656d 656e 7420 3d20 7b22 6b65 7931 223a  ement = {"key1":
-00011a50: 2076 616c 7565 7d0a 2020 2020 2020 2020   value}.        
-00011a60: 7769 7468 2063 6f6e 6669 672e 6462 2e63  with config.db.c
-00011a70: 6f6e 6e65 6374 2829 2061 7320 636f 6e6e  onnect() as conn
-00011a80: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-00011a90: 6e6e 2e65 7865 6375 7465 280a 2020 2020  nn.execute(.    
-00011aa0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00011ab0: 5f74 6162 6c65 2e69 6e73 6572 7428 292c  _table.insert(),
-00011ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011ad0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00011ae0: 2020 2020 2020 2022 6964 223a 2072 616e         "id": ran
-00011af0: 646f 6d2e 7261 6e64 696e 7428 312c 2031  dom.randint(1, 1
-00011b00: 3030 3030 3030 3030 292c 0a20 2020 2020  00000000),.     
-00011b10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00011b20: 6e61 6d65 223a 2022 726f 7731 222c 0a20  name": "row1",. 
-00011b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b40: 2020 2022 6461 7461 223a 2064 6174 615f     "data": data_
-00011b50: 656c 656d 656e 742c 0a20 2020 2020 2020  element,.       
-00011b60: 2020 2020 2020 2020 2020 2020 2022 6e75               "nu
-00011b70: 6c6c 6461 7461 223a 2064 6174 615f 656c  lldata": data_el
-00011b80: 656d 656e 742c 0a20 2020 2020 2020 2020  ement,.         
-00011b90: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00011ba0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00011bb0: 2020 2020 2065 7870 7220 3d20 6461 7461       expr = data
-00011bc0: 5f74 6162 6c65 2e63 2e64 6174 615b 226b  _table.c.data["k
-00011bd0: 6579 3122 5d0a 2020 2020 2020 2020 2020  ey1"].          
-00011be0: 2020 6578 7072 203d 2067 6574 6174 7472    expr = getattr
-00011bf0: 2865 7870 722c 2022 6173 5f25 7322 2025  (expr, "as_%s" %
-00011c00: 2064 6174 6174 7970 6529 2829 0a0a 2020   datatype)()..  
-00011c10: 2020 2020 2020 2020 2020 726f 756e 6474            roundt
-00011c20: 7269 7020 3d20 636f 6e6e 2e73 6361 6c61  rip = conn.scala
-00011c30: 7228 7365 6c65 6374 285b 6578 7072 5d29  r(select([expr])
-00011c40: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00011c50: 2072 6f75 6e64 7472 6970 2069 6e20 2822   roundtrip in ("
-00011c60: 7472 7565 222c 2022 6661 6c73 6522 2c20  true", "false", 
-00011c70: 4e6f 6e65 293a 0a20 2020 2020 2020 2020  None):.         
-00011c80: 2020 2020 2020 2072 6f75 6e64 7472 6970         roundtrip
-00011c90: 203d 2073 7472 2872 6f75 6e64 7472 6970   = str(roundtrip
-00011ca0: 292e 6361 7069 7461 6c69 7a65 2829 0a0a  ).capitalize()..
-00011cb0: 2020 2020 2020 2020 2020 2020 6571 5f28              eq_(
-00011cc0: 7374 7228 726f 756e 6474 7269 7029 2c20  str(roundtrip), 
-00011cd0: 7374 7228 7661 6c75 6529 290a 0a20 2020  str(value))..   
-00011ce0: 2040 7079 7465 7374 2e6d 6172 6b2e 736b   @pytest.mark.sk
-00011cf0: 6970 280a 2020 2020 2020 2020 2253 7061  ip(.        "Spa
-00011d00: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
-00011d10: 706f 7274 2074 7970 6520 6361 7374 7320  port type casts 
-00011d20: 696e 7369 6465 204a 534f 4e5f 5641 4c55  inside JSON_VALU
-00011d30: 4528 2920 6675 6e63 7469 6f6e 2e22 0a20  E() function.". 
-00011d40: 2020 2029 0a20 2020 2064 6566 2074 6573     ).    def tes
-00011d50: 745f 726f 756e 645f 7472 6970 5f6a 736f  t_round_trip_jso
-00011d60: 6e5f 6e75 6c6c 5f61 735f 6a73 6f6e 5f6e  n_null_as_json_n
-00011d70: 756c 6c28 7365 6c66 293a 0a20 2020 2020  ull(self):.     
-00011d80: 2020 2070 6173 730a 0a20 2020 2040 7079     pass..    @py
-00011d90: 7465 7374 2e6d 6172 6b2e 736b 6970 280a  test.mark.skip(.
-00011da0: 2020 2020 2020 2020 2253 7061 6e6e 6572          "Spanner
-00011db0: 2064 6f65 736e 2774 2073 7570 706f 7274   doesn't support
-00011dc0: 2074 7970 6520 6361 7374 7320 696e 7369   type casts insi
-00011dd0: 6465 204a 534f 4e5f 5641 4c55 4528 2920  de JSON_VALUE() 
-00011de0: 6675 6e63 7469 6f6e 2e22 0a20 2020 2029  function.".    )
-00011df0: 0a20 2020 2064 6566 2074 6573 745f 726f  .    def test_ro
-00011e00: 756e 645f 7472 6970 5f6e 6f6e 655f 6173  und_trip_none_as
-00011e10: 5f6a 736f 6e5f 6e75 6c6c 2873 656c 6629  _json_null(self)
-00011e20: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-00011e30: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-00011e40: 2e73 6b69 7028 0a20 2020 2020 2020 2022  .skip(.        "
-00011e50: 5370 616e 6e65 7220 646f 6573 6e27 7420  Spanner doesn't 
-00011e60: 7375 7070 6f72 7420 7479 7065 2063 6173  support type cas
-00011e70: 7473 2069 6e73 6964 6520 4a53 4f4e 5f56  ts inside JSON_V
-00011e80: 414c 5545 2829 2066 756e 6374 696f 6e2e  ALUE() function.
-00011e90: 220a 2020 2020 290a 2020 2020 6465 6620  ".    ).    def 
-00011ea0: 7465 7374 5f72 6f75 6e64 5f74 7269 705f  test_round_trip_
-00011eb0: 6e6f 6e65 5f61 735f 7371 6c5f 6e75 6c6c  none_as_sql_null
-00011ec0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00011ed0: 7061 7373 0a0a 0a63 6c61 7373 2045 7865  pass...class Exe
-00011ee0: 6375 7469 6f6e 4f70 7469 6f6e 7352 6571  cutionOptionsReq
-00011ef0: 7565 7374 5072 696f 726f 7479 5465 7374  uestPriorotyTest
-00011f00: 2866 6978 7475 7265 732e 5465 7374 4261  (fixtures.TestBa
-00011f10: 7365 293a 0a20 2020 2064 6566 2073 6574  se):.    def set
-00011f20: 5570 2873 656c 6629 3a0a 2020 2020 2020  Up(self):.      
-00011f30: 2020 7365 6c66 2e5f 656e 6769 6e65 203d    self._engine =
-00011f40: 2063 7265 6174 655f 656e 6769 6e65 2867   create_engine(g
-00011f50: 6574 5f64 625f 7572 6c28 292c 2070 6f6f  et_db_url(), poo
-00011f60: 6c5f 7369 7a65 3d31 290a 2020 2020 2020  l_size=1).      
-00011f70: 2020 6d65 7461 6461 7461 203d 204d 6574    metadata = Met
-00011f80: 6144 6174 6128 6269 6e64 3d73 656c 662e  aData(bind=self.
-00011f90: 5f65 6e67 696e 6529 0a0a 2020 2020 2020  _engine)..      
-00011fa0: 2020 7365 6c66 2e5f 7461 626c 6520 3d20    self._table = 
-00011fb0: 5461 626c 6528 0a20 2020 2020 2020 2020  Table(.         
-00011fc0: 2020 2022 6578 6563 7574 696f 6e5f 6f70     "execution_op
-00011fd0: 7469 6f6e 7332 222c 0a20 2020 2020 2020  tions2",.       
-00011fe0: 2020 2020 206d 6574 6164 6174 612c 0a20       metadata,. 
-00011ff0: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
-00012000: 6e28 226f 7074 5f69 6422 2c20 496e 7465  n("opt_id", Inte
-00012010: 6765 722c 2070 7269 6d61 7279 5f6b 6579  ger, primary_key
-00012020: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
-00012030: 2020 2020 436f 6c75 6d6e 2822 6f70 745f      Column("opt_
-00012040: 6e61 6d65 222c 2053 7472 696e 6728 3136  name", String(16
-00012050: 292c 206e 756c 6c61 626c 653d 4661 6c73  ), nullable=Fals
-00012060: 6529 2c0a 2020 2020 2020 2020 290a 0a20  e),.        ).. 
-00012070: 2020 2020 2020 206d 6574 6164 6174 612e         metadata.
-00012080: 6372 6561 7465 5f61 6c6c 2873 656c 662e  create_all(self.
-00012090: 5f65 6e67 696e 6529 0a20 2020 2020 2020  _engine).       
-000120a0: 2074 696d 652e 736c 6565 7028 3129 0a0a   time.sleep(1)..
-000120b0: 2020 2020 6465 6620 7465 7374 5f72 6571      def test_req
-000120c0: 7565 7374 5f70 7269 6f72 6974 7928 7365  uest_priority(se
-000120d0: 6c66 293a 0a20 2020 2020 2020 2050 5249  lf):.        PRI
-000120e0: 4f52 4954 5920 3d20 5265 7175 6573 744f  ORITY = RequestO
-000120f0: 7074 696f 6e73 2e50 7269 6f72 6974 792e  ptions.Priority.
-00012100: 5052 494f 5249 5459 5f4d 4544 4955 4d0a  PRIORITY_MEDIUM.
-00012110: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00012120: 662e 5f65 6e67 696e 652e 636f 6e6e 6563  f._engine.connec
-00012130: 7428 292e 6578 6563 7574 696f 6e5f 6f70  t().execution_op
-00012140: 7469 6f6e 7328 0a20 2020 2020 2020 2020  tions(.         
-00012150: 2020 2072 6571 7565 7374 5f70 7269 6f72     request_prior
-00012160: 6974 793d 5052 494f 5249 5459 0a20 2020  ity=PRIORITY.   
-00012170: 2020 2020 2029 2061 7320 636f 6e6e 6563       ) as connec
-00012180: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
-00012190: 2020 636f 6e6e 6563 7469 6f6e 2e65 7865    connection.exe
-000121a0: 6375 7465 2873 656c 6563 7428 5b22 2a22  cute(select(["*"
-000121b0: 5d2c 2066 726f 6d5f 6f62 6a3d 7365 6c66  ], from_obj=self
-000121c0: 2e5f 7461 626c 6529 292e 6665 7463 6861  ._table)).fetcha
-000121d0: 6c6c 2829 0a0a 2020 2020 2020 2020 7769  ll()..        wi
-000121e0: 7468 2073 656c 662e 5f65 6e67 696e 652e  th self._engine.
-000121f0: 636f 6e6e 6563 7428 2920 6173 2063 6f6e  connect() as con
-00012200: 6e65 6374 696f 6e3a 0a20 2020 2020 2020  nection:.       
-00012210: 2020 2020 2061 7373 6572 7420 636f 6e6e       assert conn
-00012220: 6563 7469 6f6e 2e63 6f6e 6e65 6374 696f  ection.connectio
-00012230: 6e2e 7265 7175 6573 745f 7072 696f 7269  n.request_priori
-00012240: 7479 2069 7320 4e6f 6e65 0a0a 2020 2020  ty is None..    
-00012250: 2020 2020 656e 6769 6e65 203d 2063 7265      engine = cre
-00012260: 6174 655f 656e 6769 6e65 2822 7371 6c69  ate_engine("sqli
-00012270: 7465 3a2f 2f2f 6461 7461 6261 7365 2229  te:///database")
-00012280: 0a20 2020 2020 2020 2077 6974 6820 656e  .        with en
-00012290: 6769 6e65 2e63 6f6e 6e65 6374 2829 2061  gine.connect() a
-000122a0: 7320 636f 6e6e 6563 7469 6f6e 3a0a 2020  s connection:.  
-000122b0: 2020 2020 2020 2020 2020 7061 7373 0a              pass.
+00002e50: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00002e60: 2020 2020 2020 2074 6573 745f 6e65 6564         test_need
+00002e70: 735f 666b 3d54 7275 652c 0a20 2020 2020  s_fk=True,.     
+00002e80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002e90: 6368 656d 613d 636f 6e66 6967 2e64 622e  chema=config.db.
+00002ea0: 6469 616c 6563 742e 6465 6661 756c 745f  dialect.default_
+00002eb0: 7363 6865 6d61 5f6e 616d 652c 0a20 2020  schema_name,.   
+00002ec0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00002ed0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00002ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002ef0: 2054 6162 6c65 280a 2020 2020 2020 2020   Table(.        
+00002f00: 2020 2020 2020 2020 2020 2020 2272 656d              "rem
+00002f10: 6f74 655f 7461 626c 6522 2c0a 2020 2020  ote_table",.    
+00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f30: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
+00002f40: 2020 2020 2020 2020 2020 2020 2020 436f                Co
+00002f50: 6c75 6d6e 2822 6964 222c 2073 716c 616c  lumn("id", sqlal
+00002f60: 6368 656d 792e 496e 7465 6765 722c 2070  chemy.Integer, p
+00002f70: 7269 6d61 7279 5f6b 6579 3d54 7275 6529  rimary_key=True)
+00002f80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002f90: 2020 2020 2020 436f 6c75 6d6e 280a 2020        Column(.  
+00002fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fb0: 2020 2020 2020 226c 6f63 616c 5f69 6422        "local_id"
+00002fc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002fd0: 2020 2020 2020 2020 2020 466f 7265 6967            Foreig
+00002fe0: 6e4b 6579 280a 2020 2020 2020 2020 2020  nKey(.          
+00002ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003000: 2020 2225 732e 6c6f 6361 6c5f 7461 626c    "%s.local_tabl
+00003010: 652e 6964 2220 2520 636f 6e66 6967 2e64  e.id" % config.d
+00003020: 622e 6469 616c 6563 742e 6465 6661 756c  b.dialect.defaul
+00003030: 745f 7363 6865 6d61 5f6e 616d 650a 2020  t_schema_name.  
+00003040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003050: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+00003060: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
+00003070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003080: 2020 2020 436f 6c75 6d6e 2822 6461 7461      Column("data
+00003090: 222c 2073 716c 616c 6368 656d 792e 5374  ", sqlalchemy.St
+000030a0: 7269 6e67 2832 3029 292c 0a20 2020 2020  ring(20)),.     
+000030b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000030c0: 6368 656d 613d 7363 6865 6d61 2c0a 2020  chema=schema,.  
+000030d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030e0: 2020 7465 7374 5f6e 6565 6473 5f66 6b3d    test_needs_fk=
+000030f0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00003100: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00003110: 2020 2020 2020 2020 5461 626c 6528 0a20          Table(. 
+00003120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003130: 2020 2022 7265 6d6f 7465 5f74 6162 6c65     "remote_table
+00003140: 5f32 222c 0a20 2020 2020 2020 2020 2020  _2",.           
+00003150: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
+00003160: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
+00003170: 2020 2020 2020 2043 6f6c 756d 6e28 2269         Column("i
+00003180: 6422 2c20 7371 6c61 6c63 6865 6d79 2e49  d", sqlalchemy.I
+00003190: 6e74 6567 6572 2c20 7072 696d 6172 795f  nteger, primary_
+000031a0: 6b65 793d 5472 7565 292c 0a20 2020 2020  key=True),.     
+000031b0: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+000031c0: 6f6c 756d 6e28 2264 6174 6122 2c20 7371  olumn("data", sq
+000031d0: 6c61 6c63 6865 6d79 2e53 7472 696e 6728  lalchemy.String(
+000031e0: 3230 2929 2c0a 2020 2020 2020 2020 2020  20)),.          
+000031f0: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
+00003200: 3d73 6368 656d 612c 0a20 2020 2020 2020  =schema,.       
+00003210: 2020 2020 2020 2020 2020 2020 2074 6573               tes
+00003220: 745f 6e65 6564 735f 666b 3d54 7275 652c  t_needs_fk=True,
+00003230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003240: 2029 0a0a 2020 2020 2020 2020 6966 2074   )..        if t
+00003250: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
+00003260: 696e 6465 785f 7265 666c 6563 7469 6f6e  index_reflection
+00003270: 2e65 6e61 626c 6564 3a0a 2020 2020 2020  .enabled:.      
+00003280: 2020 2020 2020 636c 732e 6465 6669 6e65        cls.define
+00003290: 5f69 6e64 6578 286d 6574 6164 6174 612c  _index(metadata,
+000032a0: 2075 7365 7273 290a 0a20 2020 2020 2020   users)..       
+000032b0: 2020 2020 2069 6620 6e6f 7420 7363 6865       if not sche
+000032c0: 6d61 3a0a 2020 2020 2020 2020 2020 2020  ma:.            
+000032d0: 2020 2020 2320 7465 7374 5f6e 6565 6473      # test_needs
+000032e0: 5f66 6b20 6973 2061 7420 7468 6520 6d6f  _fk is at the mo
+000032f0: 6d65 6e74 2074 6f20 666f 7263 6520 4d79  ment to force My
+00003300: 5351 4c20 496e 6e6f 4442 0a20 2020 2020  SQL InnoDB.     
+00003310: 2020 2020 2020 2020 2020 206e 6f6e 636f             nonco
+00003320: 6c5f 6964 785f 7465 7374 5f6e 6f70 6b20  l_idx_test_nopk 
+00003330: 3d20 5461 626c 6528 0a20 2020 2020 2020  = Table(.       
+00003340: 2020 2020 2020 2020 2020 2020 2022 6e6f               "no
+00003350: 6e63 6f6c 5f69 6478 5f74 6573 745f 6e6f  ncol_idx_test_no
+00003360: 706b 222c 0a20 2020 2020 2020 2020 2020  pk",.           
+00003370: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
+00003380: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
+00003390: 2020 2020 2020 2043 6f6c 756d 6e28 2269         Column("i
+000033a0: 6422 2c20 7371 6c61 6c63 6865 6d79 2e49  d", sqlalchemy.I
+000033b0: 6e74 6567 6572 2c20 7072 696d 6172 795f  nteger, primary_
+000033c0: 6b65 793d 5472 7565 292c 0a20 2020 2020  key=True),.     
+000033d0: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+000033e0: 6f6c 756d 6e28 2271 222c 2073 716c 616c  olumn("q", sqlal
+000033f0: 6368 656d 792e 5374 7269 6e67 2835 2929  chemy.String(5))
+00003400: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003410: 2020 2020 2020 7465 7374 5f6e 6565 6473        test_needs
+00003420: 5f66 6b3d 5472 7565 2c0a 2020 2020 2020  _fk=True,.      
+00003430: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+00003440: 7465 6e64 5f65 7869 7374 696e 673d 5472  tend_existing=Tr
+00003450: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00003460: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
+00003470: 2020 2020 2020 206e 6f6e 636f 6c5f 6964         noncol_id
+00003480: 785f 7465 7374 5f70 6b20 3d20 5461 626c  x_test_pk = Tabl
+00003490: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+000034a0: 2020 2020 2020 2022 6e6f 6e63 6f6c 5f69         "noncol_i
+000034b0: 6478 5f74 6573 745f 706b 222c 0a20 2020  dx_test_pk",.   
+000034c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034d0: 206d 6574 6164 6174 612c 0a20 2020 2020   metadata,.     
+000034e0: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+000034f0: 6f6c 756d 6e28 2269 6422 2c20 7371 6c61  olumn("id", sqla
+00003500: 6c63 6865 6d79 2e49 6e74 6567 6572 2c20  lchemy.Integer, 
+00003510: 7072 696d 6172 795f 6b65 793d 5472 7565  primary_key=True
+00003520: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00003530: 2020 2020 2020 2043 6f6c 756d 6e28 2271         Column("q
+00003540: 222c 2073 716c 616c 6368 656d 792e 5374  ", sqlalchemy.St
+00003550: 7269 6e67 2835 2929 2c0a 2020 2020 2020  ring(5)),.      
+00003560: 2020 2020 2020 2020 2020 2020 2020 7465                te
+00003570: 7374 5f6e 6565 6473 5f66 6b3d 5472 7565  st_needs_fk=True
+00003580: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003590: 2020 2020 2020 6578 7465 6e64 5f65 7869        extend_exi
+000035a0: 7374 696e 673d 5472 7565 2c0a 2020 2020  sting=True,.    
+000035b0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+000035c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000035d0: 6620 7465 7374 696e 672e 7265 7175 6972  f testing.requir
+000035e0: 6573 2e69 6e64 6578 6573 5f77 6974 685f  es.indexes_with_
+000035f0: 6173 6364 6573 632e 656e 6162 6c65 643a  ascdesc.enabled:
+00003600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003610: 2020 2020 2073 716c 616c 6368 656d 792e       sqlalchemy.
+00003620: 496e 6465 7828 226e 6f6e 636f 6c5f 6964  Index("noncol_id
+00003630: 785f 6e6f 706b 222c 206e 6f6e 636f 6c5f  x_nopk", noncol_
+00003640: 6964 785f 7465 7374 5f6e 6f70 6b2e 632e  idx_test_nopk.c.
+00003650: 712e 6465 7363 2829 290a 2020 2020 2020  q.desc()).      
+00003660: 2020 2020 2020 2020 2020 2020 2020 7371                sq
+00003670: 6c61 6c63 6865 6d79 2e49 6e64 6578 2822  lalchemy.Index("
+00003680: 6e6f 6e63 6f6c 5f69 6478 5f70 6b22 2c20  noncol_idx_pk", 
+00003690: 6e6f 6e63 6f6c 5f69 6478 5f74 6573 745f  noncol_idx_test_
+000036a0: 706b 2e63 2e71 2e64 6573 6328 2929 0a0a  pk.c.q.desc())..
+000036b0: 2020 2020 2020 2020 6966 2074 6573 7469          if testi
+000036c0: 6e67 2e72 6571 7569 7265 732e 7669 6577  ng.requires.view
+000036d0: 5f63 6f6c 756d 6e5f 7265 666c 6563 7469  _column_reflecti
+000036e0: 6f6e 2e65 6e61 626c 6564 3a0a 2020 2020  on.enabled:.    
+000036f0: 2020 2020 2020 2020 636c 732e 6465 6669          cls.defi
+00003700: 6e65 5f76 6965 7773 286d 6574 6164 6174  ne_views(metadat
+00003710: 612c 2073 6368 656d 6129 0a0a 2020 2020  a, schema)..    
+00003720: 4074 6573 7469 6e67 2e63 6f6d 6269 6e61  @testing.combina
+00003730: 7469 6f6e 7328 2846 616c 7365 2c29 2c20  tions((False,), 
+00003740: 6172 676e 616d 6573 3d22 7573 655f 7363  argnames="use_sc
+00003750: 6865 6d61 2229 0a20 2020 2040 7465 7374  hema").    @test
+00003760: 696e 672e 7265 7175 6972 6573 2e66 6f72  ing.requires.for
+00003770: 6569 676e 5f6b 6579 5f63 6f6e 7374 7261  eign_key_constra
+00003780: 696e 745f 7265 666c 6563 7469 6f6e 0a20  int_reflection. 
+00003790: 2020 2064 6566 2074 6573 745f 6765 745f     def test_get_
+000037a0: 666f 7265 6967 6e5f 6b65 7973 2873 656c  foreign_keys(sel
+000037b0: 662c 2063 6f6e 6e65 6374 696f 6e2c 2075  f, connection, u
+000037c0: 7365 5f73 6368 656d 6129 3a0a 2020 2020  se_schema):.    
+000037d0: 2020 2020 6966 2075 7365 5f73 6368 656d      if use_schem
+000037e0: 613a 0a20 2020 2020 2020 2020 2020 2073  a:.            s
+000037f0: 6368 656d 6120 3d20 636f 6e66 6967 2e74  chema = config.t
+00003800: 6573 745f 7363 6865 6d61 0a20 2020 2020  est_schema.     
+00003810: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00003820: 2020 2020 2073 6368 656d 6120 3d20 4e6f       schema = No
+00003830: 6e65 0a0a 2020 2020 2020 2020 7573 6572  ne..        user
+00003840: 732c 2061 6464 7265 7373 6573 203d 2028  s, addresses = (
+00003850: 7365 6c66 2e74 6162 6c65 732e 7573 6572  self.tables.user
+00003860: 732c 2073 656c 662e 7461 626c 6573 2e65  s, self.tables.e
+00003870: 6d61 696c 5f61 6464 7265 7373 6573 290a  mail_addresses).
+00003880: 2020 2020 2020 2020 696e 7370 203d 2069          insp = i
+00003890: 6e73 7065 6374 2863 6f6e 6e65 6374 696f  nspect(connectio
+000038a0: 6e29 0a20 2020 2020 2020 2065 7870 6563  n).        expec
+000038b0: 7465 645f 7363 6865 6d61 203d 2073 6368  ted_schema = sch
+000038c0: 656d 610a 2020 2020 2020 2020 2320 7573  ema.        # us
+000038d0: 6572 730a 0a20 2020 2020 2020 2069 6620  ers..        if 
+000038e0: 7465 7374 696e 672e 7265 7175 6972 6573  testing.requires
+000038f0: 2e73 656c 665f 7265 6665 7265 6e74 6961  .self_referentia
+00003900: 6c5f 666f 7265 6967 6e5f 6b65 7973 2e65  l_foreign_keys.e
+00003910: 6e61 626c 6564 3a0a 2020 2020 2020 2020  nabled:.        
+00003920: 2020 2020 7573 6572 735f 666b 6579 7320      users_fkeys 
+00003930: 3d20 696e 7370 2e67 6574 5f66 6f72 6569  = insp.get_forei
+00003940: 676e 5f6b 6579 7328 7573 6572 732e 6e61  gn_keys(users.na
+00003950: 6d65 2c20 7363 6865 6d61 3d73 6368 656d  me, schema=schem
+00003960: 6129 0a20 2020 2020 2020 2020 2020 2066  a).            f
+00003970: 6b65 7931 203d 2075 7365 7273 5f66 6b65  key1 = users_fke
+00003980: 7973 5b30 5d0a 0a20 2020 2020 2020 2020  ys[0]..         
+00003990: 2020 2077 6974 6820 7465 7374 696e 672e     with testing.
+000039a0: 7265 7175 6972 6573 2e6e 616d 6564 5f63  requires.named_c
+000039b0: 6f6e 7374 7261 696e 7473 2e66 6169 6c5f  onstraints.fail_
+000039c0: 6966 2829 3a0a 2020 2020 2020 2020 2020  if():.          
+000039d0: 2020 2020 2020 6571 5f28 666b 6579 315b        eq_(fkey1[
+000039e0: 226e 616d 6522 5d2c 2022 7573 6572 5f69  "name"], "user_i
+000039f0: 645f 666b 2229 0a0a 2020 2020 2020 2020  d_fk")..        
+00003a00: 2020 2020 6571 5f28 666b 6579 315b 2272      eq_(fkey1["r
+00003a10: 6566 6572 7265 645f 7363 6865 6d61 225d  eferred_schema"]
+00003a20: 2c20 6578 7065 6374 6564 5f73 6368 656d  , expected_schem
+00003a30: 6129 0a20 2020 2020 2020 2020 2020 2065  a).            e
+00003a40: 715f 2866 6b65 7931 5b22 7265 6665 7272  q_(fkey1["referr
+00003a50: 6564 5f74 6162 6c65 225d 2c20 7573 6572  ed_table"], user
+00003a60: 732e 6e61 6d65 290a 2020 2020 2020 2020  s.name).        
+00003a70: 2020 2020 6571 5f28 666b 6579 315b 2272      eq_(fkey1["r
+00003a80: 6566 6572 7265 645f 636f 6c75 6d6e 7322  eferred_columns"
+00003a90: 5d2c 205b 2275 7365 725f 6964 225d 290a  ], ["user_id"]).
+00003aa0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+00003ab0: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
+00003ac0: 7365 6c66 5f72 6566 6572 656e 7469 616c  self_referential
+00003ad0: 5f66 6f72 6569 676e 5f6b 6579 732e 656e  _foreign_keys.en
+00003ae0: 6162 6c65 643a 0a20 2020 2020 2020 2020  abled:.         
+00003af0: 2020 2020 2020 2065 715f 2866 6b65 7931         eq_(fkey1
+00003b00: 5b22 636f 6e73 7472 6169 6e65 645f 636f  ["constrained_co
+00003b10: 6c75 6d6e 7322 5d2c 205b 2270 6172 656e  lumns"], ["paren
+00003b20: 745f 7573 6572 5f69 6422 5d29 0a0a 2020  t_user_id"])..  
+00003b30: 2020 2020 2020 2320 6164 6472 6573 7365        # addresse
+00003b40: 730a 2020 2020 2020 2020 6164 6472 5f66  s.        addr_f
+00003b50: 6b65 7973 203d 2069 6e73 702e 6765 745f  keys = insp.get_
+00003b60: 666f 7265 6967 6e5f 6b65 7973 2861 6464  foreign_keys(add
+00003b70: 7265 7373 6573 2e6e 616d 652c 2073 6368  resses.name, sch
+00003b80: 656d 613d 7363 6865 6d61 290a 2020 2020  ema=schema).    
+00003b90: 2020 2020 666b 6579 3120 3d20 6164 6472      fkey1 = addr
+00003ba0: 5f66 6b65 7973 5b30 5d0a 0a20 2020 2020  _fkeys[0]..     
+00003bb0: 2020 2077 6974 6820 7465 7374 696e 672e     with testing.
+00003bc0: 7265 7175 6972 6573 2e69 6d70 6c69 6369  requires.implici
+00003bd0: 746c 795f 6e61 6d65 645f 636f 6e73 7472  tly_named_constr
+00003be0: 6169 6e74 732e 6661 696c 5f69 6628 293a  aints.fail_if():
+00003bf0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00003c00: 662e 6173 7365 7274 5f28 666b 6579 315b  f.assert_(fkey1[
+00003c10: 226e 616d 6522 5d20 6973 206e 6f74 204e  "name"] is not N
+00003c20: 6f6e 6529 0a0a 2020 2020 2020 2020 6571  one)..        eq
+00003c30: 5f28 666b 6579 315b 2272 6566 6572 7265  _(fkey1["referre
+00003c40: 645f 7363 6865 6d61 225d 2c20 6578 7065  d_schema"], expe
+00003c50: 6374 6564 5f73 6368 656d 6129 0a20 2020  cted_schema).   
+00003c60: 2020 2020 2065 715f 2866 6b65 7931 5b22       eq_(fkey1["
+00003c70: 7265 6665 7272 6564 5f74 6162 6c65 225d  referred_table"]
+00003c80: 2c20 7573 6572 732e 6e61 6d65 290a 2020  , users.name).  
+00003c90: 2020 2020 2020 6571 5f28 666b 6579 315b        eq_(fkey1[
+00003ca0: 2272 6566 6572 7265 645f 636f 6c75 6d6e  "referred_column
+00003cb0: 7322 5d2c 205b 2275 7365 725f 6964 225d  s"], ["user_id"]
+00003cc0: 290a 2020 2020 2020 2020 6571 5f28 666b  ).        eq_(fk
+00003cd0: 6579 315b 2263 6f6e 7374 7261 696e 6564  ey1["constrained
+00003ce0: 5f63 6f6c 756d 6e73 225d 2c20 5b22 7265  _columns"], ["re
+00003cf0: 6d6f 7465 5f75 7365 725f 6964 225d 290a  mote_user_id"]).
+00003d00: 0a20 2020 2040 7465 7374 696e 672e 7265  .    @testing.re
+00003d10: 7175 6972 6573 2e66 6f72 6569 676e 5f6b  quires.foreign_k
+00003d20: 6579 5f63 6f6e 7374 7261 696e 745f 7265  ey_constraint_re
+00003d30: 666c 6563 7469 6f6e 0a20 2020 2040 7465  flection.    @te
+00003d40: 7374 696e 672e 636f 6d62 696e 6174 696f  sting.combinatio
+00003d50: 6e73 280a 2020 2020 2020 2020 284e 6f6e  ns(.        (Non
+00003d60: 652c 2054 7275 652c 2046 616c 7365 2c20  e, True, False, 
+00003d70: 4661 6c73 6529 2c0a 2020 2020 2020 2020  False),.        
+00003d80: 284e 6f6e 652c 2054 7275 652c 2046 616c  (None, True, Fal
+00003d90: 7365 2c20 5472 7565 2c20 7465 7374 696e  se, True, testin
+00003da0: 672e 7265 7175 6972 6573 2e73 6368 656d  g.requires.schem
+00003db0: 6173 292c 0a20 2020 2020 2020 2028 2266  as),.        ("f
+00003dc0: 6f72 6569 676e 5f6b 6579 222c 2054 7275  oreign_key", Tru
+00003dd0: 652c 2046 616c 7365 2c20 4661 6c73 6529  e, False, False)
+00003de0: 2c0a 2020 2020 2020 2020 284e 6f6e 652c  ,.        (None,
+00003df0: 2046 616c 7365 2c20 4661 6c73 652c 2046   False, False, F
+00003e00: 616c 7365 292c 0a20 2020 2020 2020 2028  alse),.        (
+00003e10: 4e6f 6e65 2c20 4661 6c73 652c 2046 616c  None, False, Fal
+00003e20: 7365 2c20 5472 7565 2c20 7465 7374 696e  se, True, testin
+00003e30: 672e 7265 7175 6972 6573 2e73 6368 656d  g.requires.schem
+00003e40: 6173 292c 0a20 2020 2020 2020 2028 4e6f  as),.        (No
+00003e50: 6e65 2c20 5472 7565 2c20 4661 6c73 652c  ne, True, False,
+00003e60: 2046 616c 7365 292c 0a20 2020 2020 2020   False),.       
+00003e70: 2028 4e6f 6e65 2c20 5472 7565 2c20 4661   (None, True, Fa
+00003e80: 6c73 652c 2054 7275 652c 2074 6573 7469  lse, True, testi
+00003e90: 6e67 2e72 6571 7569 7265 732e 7363 6865  ng.requires.sche
+00003ea0: 6d61 7329 2c0a 2020 2020 2020 2020 6172  mas),.        ar
+00003eb0: 676e 616d 6573 3d22 6f72 6465 725f 6279  gnames="order_by
+00003ec0: 2c69 6e63 6c75 6465 5f70 6c61 696e 2c69  ,include_plain,i
+00003ed0: 6e63 6c75 6465 5f76 6965 7773 2c75 7365  nclude_views,use
+00003ee0: 5f73 6368 656d 6122 2c0a 2020 2020 290a  _schema",.    ).
+00003ef0: 2020 2020 6465 6620 7465 7374 5f67 6574      def test_get
+00003f00: 5f74 6162 6c65 5f6e 616d 6573 280a 2020  _table_names(.  
+00003f10: 2020 2020 2020 7365 6c66 2c20 636f 6e6e        self, conn
+00003f20: 6563 7469 6f6e 2c20 6f72 6465 725f 6279  ection, order_by
+00003f30: 2c20 696e 636c 7564 655f 706c 6169 6e2c  , include_plain,
+00003f40: 2069 6e63 6c75 6465 5f76 6965 7773 2c20   include_views, 
+00003f50: 7573 655f 7363 6865 6d61 0a20 2020 2029  use_schema.    )
+00003f60: 3a0a 0a20 2020 2020 2020 2069 6620 7573  :..        if us
+00003f70: 655f 7363 6865 6d61 3a0a 2020 2020 2020  e_schema:.      
+00003f80: 2020 2020 2020 7363 6865 6d61 203d 2063        schema = c
+00003f90: 6f6e 6669 672e 7465 7374 5f73 6368 656d  onfig.test_schem
+00003fa0: 610a 2020 2020 2020 2020 656c 7365 3a0a  a.        else:.
+00003fb0: 2020 2020 2020 2020 2020 2020 7363 6865              sche
+00003fc0: 6d61 203d 204e 6f6e 650a 0a20 2020 2020  ma = None..     
+00003fd0: 2020 205f 6967 6e6f 7265 5f74 6162 6c65     _ignore_table
+00003fe0: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
+00003ff0: 2020 2261 6363 6f75 6e74 222c 0a20 2020    "account",.   
+00004000: 2020 2020 2020 2020 2022 616c 656d 6269           "alembi
+00004010: 635f 7665 7273 696f 6e22 2c0a 2020 2020  c_version",.    
+00004020: 2020 2020 2020 2020 2262 7974 6573 5f74          "bytes_t
+00004030: 6162 6c65 222c 0a20 2020 2020 2020 2020  able",.         
+00004040: 2020 2022 636f 6d6d 656e 745f 7465 7374     "comment_test
+00004050: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00004060: 6461 7465 5f74 6162 6c65 222c 0a20 2020  date_table",.   
+00004070: 2020 2020 2020 2020 2022 6e6f 6e63 6f6c           "noncol
+00004080: 5f69 6478 5f74 6573 745f 706b 222c 0a20  _idx_test_pk",. 
+00004090: 2020 2020 2020 2020 2020 2022 6e6f 6e63             "nonc
+000040a0: 6f6c 5f69 6478 5f74 6573 745f 6e6f 706b  ol_idx_test_nopk
+000040b0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000040c0: 6c6f 6361 6c5f 7461 626c 6522 2c0a 2020  local_table",.  
+000040d0: 2020 2020 2020 2020 2020 2272 656d 6f74            "remot
+000040e0: 655f 7461 626c 6522 2c0a 2020 2020 2020  e_table",.      
+000040f0: 2020 2020 2020 2272 656d 6f74 655f 7461        "remote_ta
+00004100: 626c 655f 3222 2c0a 2020 2020 2020 2020  ble_2",.        
+00004110: 2020 2020 2274 6578 745f 7461 626c 6522      "text_table"
+00004120: 2c0a 2020 2020 2020 2020 2020 2020 2275  ,.            "u
+00004130: 7365 725f 746d 7022 2c0a 2020 2020 2020  ser_tmp",.      
+00004140: 2020 5d0a 0a20 2020 2020 2020 2069 6e73    ]..        ins
+00004150: 7020 3d20 696e 7370 6563 7428 636f 6e6e  p = inspect(conn
+00004160: 6563 7469 6f6e 290a 0a20 2020 2020 2020  ection)..       
+00004170: 2069 6620 696e 636c 7564 655f 7669 6577   if include_view
+00004180: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
+00004190: 6162 6c65 5f6e 616d 6573 203d 2069 6e73  able_names = ins
+000041a0: 702e 6765 745f 7669 6577 5f6e 616d 6573  p.get_view_names
+000041b0: 2873 6368 656d 6129 0a20 2020 2020 2020  (schema).       
+000041c0: 2020 2020 2074 6162 6c65 5f6e 616d 6573       table_names
+000041d0: 2e73 6f72 7428 290a 2020 2020 2020 2020  .sort().        
+000041e0: 2020 2020 616e 7377 6572 203d 205b 2265      answer = ["e
+000041f0: 6d61 696c 5f61 6464 7265 7373 6573 5f76  mail_addresses_v
+00004200: 222c 2022 7573 6572 735f 7622 5d0a 2020  ", "users_v"].  
+00004210: 2020 2020 2020 2020 2020 6571 5f28 736f            eq_(so
+00004220: 7274 6564 2874 6162 6c65 5f6e 616d 6573  rted(table_names
+00004230: 292c 2061 6e73 7765 7229 0a0a 2020 2020  ), answer)..    
+00004240: 2020 2020 6966 2069 6e63 6c75 6465 5f70      if include_p
+00004250: 6c61 696e 3a0a 2020 2020 2020 2020 2020  lain:.          
+00004260: 2020 6966 206f 7264 6572 5f62 793a 0a20    if order_by:. 
+00004270: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00004280: 6162 6c65 7320 3d20 5b0a 2020 2020 2020  ables = [.      
+00004290: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000042a0: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
+000042b0: 2020 2020 2020 2020 2066 6f72 2072 6563           for rec
+000042c0: 2069 6e20 696e 7370 2e67 6574 5f73 6f72   in insp.get_sor
+000042d0: 7465 645f 7461 626c 655f 616e 645f 666b  ted_table_and_fk
+000042e0: 635f 6e61 6d65 7328 7363 6865 6d61 290a  c_names(schema).
+000042f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004300: 2020 2020 6966 2072 6563 5b30 5d0a 2020      if rec[0].  
+00004310: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
+00004320: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00004330: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004340: 2020 7461 626c 6573 203d 2069 6e73 702e    tables = insp.
+00004350: 6765 745f 7461 626c 655f 6e61 6d65 7328  get_table_names(
+00004360: 7363 6865 6d61 290a 2020 2020 2020 2020  schema).        
+00004370: 2020 2020 7461 626c 655f 6e61 6d65 7320      table_names 
+00004380: 3d20 5b74 2066 6f72 2074 2069 6e20 7461  = [t for t in ta
+00004390: 626c 6573 2069 6620 7420 6e6f 7420 696e  bles if t not in
+000043a0: 205f 6967 6e6f 7265 5f74 6162 6c65 735d   _ignore_tables]
+000043b0: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+000043c0: 206f 7264 6572 5f62 7920 3d3d 2022 666f   order_by == "fo
+000043d0: 7265 6967 6e5f 6b65 7922 3a0a 2020 2020  reign_key":.    
+000043e0: 2020 2020 2020 2020 2020 2020 616e 7377              answ
+000043f0: 6572 203d 205b 2275 7365 7273 222c 2022  er = ["users", "
+00004400: 656d 6169 6c5f 6164 6472 6573 7365 7322  email_addresses"
+00004410: 2c20 2264 696e 6761 6c69 6e67 7322 5d0a  , "dingalings"].
+00004420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004430: 6571 5f28 7461 626c 655f 6e61 6d65 732c  eq_(table_names,
+00004440: 2061 6e73 7765 7229 0a20 2020 2020 2020   answer).       
+00004450: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00004460: 2020 2020 2020 2020 2020 2061 6e73 7765             answe
+00004470: 7220 3d20 5b22 6469 6e67 616c 696e 6773  r = ["dingalings
+00004480: 222c 2022 656d 6169 6c5f 6164 6472 6573  ", "email_addres
+00004490: 7365 7322 2c20 2275 7365 7273 225d 0a20  ses", "users"]. 
+000044a0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000044b0: 715f 2873 6f72 7465 6428 7461 626c 655f  q_(sorted(table_
+000044c0: 6e61 6d65 7329 2c20 616e 7377 6572 290a  names), answer).
+000044d0: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+000044e0: 640a 2020 2020 6465 6620 6465 6669 6e65  d.    def define
+000044f0: 5f74 656d 705f 7461 626c 6573 2863 6c73  _temp_tables(cls
+00004500: 2c20 6d65 7461 6461 7461 293a 0a20 2020  , metadata):.   
+00004510: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00004520: 2053 5041 4e4e 4552 204f 5645 5252 4944   SPANNER OVERRID
+00004530: 453a 0a0a 2020 2020 2020 2020 496e 2043  E:..        In C
+00004540: 6c6f 7564 2053 7061 6e6e 6572 2075 6e69  loud Spanner uni
+00004550: 7175 6520 696e 6465 7865 7320 6172 6520  que indexes are 
+00004560: 7573 6564 2069 6e73 7465 6164 206f 6620  used instead of 
+00004570: 6469 7265 6374 6c79 0a20 2020 2020 2020  directly.       
+00004580: 2063 7265 6174 696e 6720 756e 6971 7565   creating unique
+00004590: 2063 6f6e 7374 7261 696e 7473 2e20 4f76   constraints. Ov
+000045a0: 6572 7269 6469 6e67 2074 6865 2074 6573  erriding the tes
+000045b0: 7420 746f 2072 6570 6c61 6365 0a20 2020  t to replace.   
+000045c0: 2020 2020 2063 6f6e 7374 7261 696e 7473       constraints
+000045d0: 2077 6974 6820 696e 6465 7865 7320 696e   with indexes in
+000045e0: 2074 6573 7469 6e67 2064 6174 612e 0a20   testing data.. 
+000045f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00004600: 2020 206b 7720 3d20 7465 6d70 5f74 6162     kw = temp_tab
+00004610: 6c65 5f6b 6579 776f 7264 5f61 7267 7328  le_keyword_args(
+00004620: 636f 6e66 6967 2c20 636f 6e66 6967 2e64  config, config.d
+00004630: 6229 0a20 2020 2020 2020 2075 7365 725f  b).        user_
+00004640: 746d 7020 3d20 5461 626c 6528 0a20 2020  tmp = Table(.   
+00004650: 2020 2020 2020 2020 2022 7573 6572 5f74           "user_t
+00004660: 6d70 222c 0a20 2020 2020 2020 2020 2020  mp",.           
+00004670: 206d 6574 6164 6174 612c 0a20 2020 2020   metadata,.     
+00004680: 2020 2020 2020 2043 6f6c 756d 6e28 2269         Column("i
+00004690: 6422 2c20 7371 6c61 6c63 6865 6d79 2e49  d", sqlalchemy.I
+000046a0: 4e54 2c20 7072 696d 6172 795f 6b65 793d  NT, primary_key=
+000046b0: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
+000046c0: 2020 2043 6f6c 756d 6e28 226e 616d 6522     Column("name"
+000046d0: 2c20 7371 6c61 6c63 6865 6d79 2e56 4152  , sqlalchemy.VAR
+000046e0: 4348 4152 2835 3029 292c 0a20 2020 2020  CHAR(50)),.     
+000046f0: 2020 2020 2020 2043 6f6c 756d 6e28 2266         Column("f
+00004700: 6f6f 222c 2073 716c 616c 6368 656d 792e  oo", sqlalchemy.
+00004710: 494e 5429 2c0a 2020 2020 2020 2020 2020  INT),.          
+00004720: 2020 7371 6c61 6c63 6865 6d79 2e49 6e64    sqlalchemy.Ind
+00004730: 6578 2822 7573 6572 5f74 6d70 5f75 7122  ex("user_tmp_uq"
+00004740: 2c20 226e 616d 6522 2c20 756e 6971 7565  , "name", unique
+00004750: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
+00004760: 2020 2020 7371 6c61 6c63 6865 6d79 2e49      sqlalchemy.I
+00004770: 6e64 6578 2822 7573 6572 5f74 6d70 5f69  ndex("user_tmp_i
+00004780: 7822 2c20 2266 6f6f 2229 2c0a 2020 2020  x", "foo"),.    
+00004790: 2020 2020 2020 2020 6578 7465 6e64 5f65          extend_e
+000047a0: 7869 7374 696e 673d 5472 7565 2c0a 2020  xisting=True,.  
+000047b0: 2020 2020 2020 2020 2020 2a2a 6b77 2c0a            **kw,.
+000047c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000047d0: 2020 6966 2028 0a20 2020 2020 2020 2020    if (.         
+000047e0: 2020 2074 6573 7469 6e67 2e72 6571 7569     testing.requi
+000047f0: 7265 732e 7669 6577 5f72 6566 6c65 6374  res.view_reflect
+00004800: 696f 6e2e 656e 6162 6c65 640a 2020 2020  ion.enabled.    
+00004810: 2020 2020 2020 2020 616e 6420 7465 7374          and test
+00004820: 696e 672e 7265 7175 6972 6573 2e74 656d  ing.requires.tem
+00004830: 706f 7261 7279 5f76 6965 7773 2e65 6e61  porary_views.ena
+00004840: 626c 6564 0a20 2020 2020 2020 2029 3a0a  bled.        ):.
+00004850: 2020 2020 2020 2020 2020 2020 6576 656e              even
+00004860: 742e 6c69 7374 656e 280a 2020 2020 2020  t.listen(.      
+00004870: 2020 2020 2020 2020 2020 7573 6572 5f74            user_t
+00004880: 6d70 2c0a 2020 2020 2020 2020 2020 2020  mp,.            
+00004890: 2020 2020 2261 6674 6572 5f63 7265 6174      "after_creat
+000048a0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+000048b0: 2020 2020 4444 4c28 2263 7265 6174 6520      DDL("create 
+000048c0: 7465 6d70 6f72 6172 7920 7669 6577 2075  temporary view u
+000048d0: 7365 725f 746d 705f 7620 6173 2022 2022  ser_tmp_v as " "
+000048e0: 7365 6c65 6374 202a 2066 726f 6d20 7573  select * from us
+000048f0: 6572 5f74 6d70 2229 2c0a 2020 2020 2020  er_tmp"),.      
+00004900: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00004910: 2020 2020 6576 656e 742e 6c69 7374 656e      event.listen
+00004920: 2875 7365 725f 746d 702c 2022 6265 666f  (user_tmp, "befo
+00004930: 7265 5f64 726f 7022 2c20 4444 4c28 2264  re_drop", DDL("d
+00004940: 726f 7020 7669 6577 2075 7365 725f 746d  rop view user_tm
+00004950: 705f 7622 2929 0a0a 2020 2020 4074 6573  p_v"))..    @tes
+00004960: 7469 6e67 2e70 726f 7669 6465 5f6d 6574  ting.provide_met
+00004970: 6164 6174 610a 2020 2020 6465 6620 7465  adata.    def te
+00004980: 7374 5f72 6566 6c65 6374 5f73 7472 696e  st_reflect_strin
+00004990: 675f 636f 6c75 6d6e 5f6d 6178 5f6c 656e  g_column_max_len
+000049a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000049b0: 2222 220a 2020 2020 2020 2020 5350 414e  """.        SPAN
+000049c0: 4e45 5220 5350 4543 4946 4943 2054 4553  NER SPECIFIC TES
+000049d0: 543a 0a0a 2020 2020 2020 2020 496e 2053  T:..        In S
+000049e0: 7061 6e6e 6572 2063 6f6c 756d 6e20 6f66  panner column of
+000049f0: 2074 6865 2053 5452 494e 4720 7479 7065   the STRING type
+00004a00: 2063 616e 2062 650a 2020 2020 2020 2020   can be.        
+00004a10: 6372 6561 7465 6420 7769 7468 2073 697a  created with siz
+00004a20: 6520 6465 6669 6e65 6420 6173 204d 4158  e defined as MAX
+00004a30: 2e20 5468 6520 7465 7374 0a20 2020 2020  . The test.     
+00004a40: 2020 2063 6865 636b 7320 7468 6174 2073     checks that s
+00004a50: 7563 6820 6120 636f 6c75 6d6e 2069 7320  uch a column is 
+00004a60: 636f 7272 6563 746c 7920 7265 666c 6563  correctly reflec
+00004a70: 7465 642e 0a20 2020 2020 2020 2022 2222  ted..        """
+00004a80: 0a20 2020 2020 2020 206d 6574 6164 6174  .        metadat
+00004a90: 6120 3d20 4d65 7461 4461 7461 2873 656c  a = MetaData(sel
+00004aa0: 662e 6269 6e64 290a 2020 2020 2020 2020  f.bind).        
+00004ab0: 5461 626c 6528 2274 6578 745f 7461 626c  Table("text_tabl
+00004ac0: 6522 2c20 6d65 7461 6461 7461 2c20 436f  e", metadata, Co
+00004ad0: 6c75 6d6e 2822 5465 7374 436f 6c75 6d6e  lumn("TestColumn
+00004ae0: 222c 2054 6578 742c 206e 756c 6c61 626c  ", Text, nullabl
+00004af0: 653d 4661 6c73 6529 290a 2020 2020 2020  e=False)).      
+00004b00: 2020 6d65 7461 6461 7461 2e63 7265 6174    metadata.creat
+00004b10: 655f 616c 6c28 290a 0a20 2020 2020 2020  e_all()..       
+00004b20: 2054 6162 6c65 2822 7465 7874 5f74 6162   Table("text_tab
+00004b30: 6c65 222c 206d 6574 6164 6174 612c 2061  le", metadata, a
+00004b40: 7574 6f6c 6f61 643d 5472 7565 290a 0a20  utoload=True).. 
+00004b50: 2020 2064 6566 2074 6573 745f 7265 666c     def test_refl
+00004b60: 6563 745f 6279 7465 735f 636f 6c75 6d6e  ect_bytes_column
+00004b70: 5f6d 6178 5f6c 656e 2873 656c 6629 3a0a  _max_len(self):.
+00004b80: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00004b90: 2020 2020 5350 414e 4e45 5220 5350 4543      SPANNER SPEC
+00004ba0: 4946 4943 2054 4553 543a 0a0a 2020 2020  IFIC TEST:..    
+00004bb0: 2020 2020 496e 2053 7061 6e6e 6572 2063      In Spanner c
+00004bc0: 6f6c 756d 6e20 6f66 2074 6865 2042 5954  olumn of the BYT
+00004bd0: 4553 2074 7970 6520 6361 6e20 6265 0a20  ES type can be. 
+00004be0: 2020 2020 2020 2063 7265 6174 6564 2077         created w
+00004bf0: 6974 6820 7369 7a65 2064 6566 696e 6564  ith size defined
+00004c00: 2061 7320 4d41 582e 2054 6865 2074 6573   as MAX. The tes
+00004c10: 740a 2020 2020 2020 2020 6368 6563 6b73  t.        checks
+00004c20: 2074 6861 7420 7375 6368 2061 2063 6f6c   that such a col
+00004c30: 756d 6e20 6973 2063 6f72 7265 6374 6c79  umn is correctly
+00004c40: 2072 6566 6c65 6374 6564 2e0a 2020 2020   reflected..    
+00004c50: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00004c60: 6d65 7461 6461 7461 203d 204d 6574 6144  metadata = MetaD
+00004c70: 6174 6128 7365 6c66 2e62 696e 6429 0a20  ata(self.bind). 
+00004c80: 2020 2020 2020 2054 6162 6c65 280a 2020         Table(.  
+00004c90: 2020 2020 2020 2020 2020 2262 7974 6573            "bytes
+00004ca0: 5f74 6162 6c65 222c 0a20 2020 2020 2020  _table",.       
+00004cb0: 2020 2020 206d 6574 6164 6174 612c 0a20       metadata,. 
+00004cc0: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
+00004cd0: 6e28 2254 6573 7443 6f6c 756d 6e22 2c20  n("TestColumn", 
+00004ce0: 4c61 7267 6542 696e 6172 792c 206e 756c  LargeBinary, nul
+00004cf0: 6c61 626c 653d 4661 6c73 6529 2c0a 2020  lable=False),.  
+00004d00: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00004d10: 6d65 7461 6461 7461 2e63 7265 6174 655f  metadata.create_
+00004d20: 616c 6c28 290a 0a20 2020 2020 2020 2054  all()..        T
+00004d30: 6162 6c65 2822 6279 7465 735f 7461 626c  able("bytes_tabl
+00004d40: 6522 2c20 6d65 7461 6461 7461 2c20 6175  e", metadata, au
+00004d50: 746f 6c6f 6164 3d54 7275 6529 0a0a 2020  toload=True)..  
+00004d60: 2020 4074 6573 7469 6e67 2e63 6f6d 6269    @testing.combi
+00004d70: 6e61 7469 6f6e 7328 0a20 2020 2020 2020  nations(.       
+00004d80: 2028 5472 7565 2c20 7465 7374 696e 672e   (True, testing.
+00004d90: 7265 7175 6972 6573 2e73 6368 656d 6173  requires.schemas
+00004da0: 292c 2028 4661 6c73 652c 292c 2061 7267  ), (False,), arg
+00004db0: 6e61 6d65 733d 2275 7365 5f73 6368 656d  names="use_schem
+00004dc0: 6122 0a20 2020 2029 0a20 2020 2040 7465  a".    ).    @te
+00004dd0: 7374 696e 672e 7265 7175 6972 6573 2e75  sting.requires.u
+00004de0: 6e69 7175 655f 636f 6e73 7472 6169 6e74  nique_constraint
+00004df0: 5f72 6566 6c65 6374 696f 6e0a 2020 2020  _reflection.    
+00004e00: 6465 6620 7465 7374 5f67 6574 5f75 6e69  def test_get_uni
+00004e10: 7175 655f 636f 6e73 7472 6169 6e74 7328  que_constraints(
+00004e20: 7365 6c66 2c20 6d65 7461 6461 7461 2c20  self, metadata, 
+00004e30: 636f 6e6e 6563 7469 6f6e 2c20 7573 655f  connection, use_
+00004e40: 7363 6865 6d61 293a 0a20 2020 2020 2020  schema):.       
+00004e50: 2023 2053 514c 6974 6520 6469 616c 6563   # SQLite dialec
+00004e60: 7420 6e65 6564 7320 746f 2070 6172 7365  t needs to parse
+00004e70: 2074 6865 206e 616d 6573 206f 6620 7468   the names of th
+00004e80: 6520 636f 6e73 7472 6169 6e74 730a 2020  e constraints.  
+00004e90: 2020 2020 2020 2320 7365 7061 7261 7465        # separate
+00004ea0: 6c79 2066 726f 6d20 7768 6174 2069 7420  ly from what it 
+00004eb0: 6765 7473 2066 726f 6d20 5052 4147 4d41  gets from PRAGMA
+00004ec0: 2069 6e64 6578 5f6c 6973 7428 292c 2061   index_list(), a
+00004ed0: 6e64 0a20 2020 2020 2020 2023 2074 6865  nd.        # the
+00004ee0: 6e20 6d61 7463 6865 7320 7468 656d 2075  n matches them u
+00004ef0: 702e 2020 736f 2073 616d 6520 7365 7420  p.  so same set 
+00004f00: 6f66 2063 6f6c 756d 6e5f 6e61 6d65 7320  of column_names 
+00004f10: 696e 2074 776f 0a20 2020 2020 2020 2023  in two.        #
+00004f20: 2063 6f6e 7374 7261 696e 7473 2077 696c   constraints wil
+00004f30: 6c20 636f 6e66 7573 6520 6974 2e20 2020  l confuse it.   
+00004f40: 2050 6572 6861 7073 2077 6520 7368 6f75   Perhaps we shou
+00004f50: 6c64 206e 6f20 6c6f 6e67 6572 0a20 2020  ld no longer.   
+00004f60: 2020 2020 2023 2062 6f74 6865 7220 7769       # bother wi
+00004f70: 7468 2069 6e64 6578 5f6c 6973 7428 2920  th index_list() 
+00004f80: 6865 7265 2073 696e 6365 2077 6520 6861  here since we ha
+00004f90: 7665 2074 6865 2077 686f 6c65 0a20 2020  ve the whole.   
+00004fa0: 2020 2020 2023 2043 5245 4154 4520 5441       # CREATE TA
+00004fb0: 424c 453f 0a0a 2020 2020 2020 2020 6966  BLE?..        if
+00004fc0: 2075 7365 5f73 6368 656d 613a 0a20 2020   use_schema:.   
+00004fd0: 2020 2020 2020 2020 2073 6368 656d 6120           schema 
+00004fe0: 3d20 636f 6e66 6967 2e74 6573 745f 7363  = config.test_sc
+00004ff0: 6865 6d61 0a20 2020 2020 2020 2065 6c73  hema.        els
+00005000: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00005010: 6368 656d 6120 3d20 4e6f 6e65 0a20 2020  chema = None.   
+00005020: 2020 2020 2075 6e69 7175 6573 203d 2073       uniques = s
+00005030: 6f72 7465 6428 0a20 2020 2020 2020 2020  orted(.         
+00005040: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
+00005050: 2020 2020 207b 226e 616d 6522 3a20 2275       {"name": "u
+00005060: 6e69 7175 655f 6122 2c20 2263 6f6c 756d  nique_a", "colum
+00005070: 6e5f 6e61 6d65 7322 3a20 5b22 6122 5d7d  n_names": ["a"]}
+00005080: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005090: 2020 7b22 6e61 6d65 223a 2022 756e 6971    {"name": "uniq
+000050a0: 7565 5f61 5f62 5f63 222c 2022 636f 6c75  ue_a_b_c", "colu
+000050b0: 6d6e 5f6e 616d 6573 223a 205b 2261 222c  mn_names": ["a",
+000050c0: 2022 6222 2c20 2263 225d 7d2c 0a20 2020   "b", "c"]},.   
+000050d0: 2020 2020 2020 2020 2020 2020 207b 226e               {"n
+000050e0: 616d 6522 3a20 2275 6e69 7175 655f 635f  ame": "unique_c_
+000050f0: 615f 6222 2c20 2263 6f6c 756d 6e5f 6e61  a_b", "column_na
+00005100: 6d65 7322 3a20 5b22 6322 2c20 2261 222c  mes": ["c", "a",
+00005110: 2022 6222 5d7d 2c0a 2020 2020 2020 2020   "b"]},.        
+00005120: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
+00005130: 2022 756e 6971 7565 5f61 7363 5f6b 6579   "unique_asc_key
+00005140: 222c 2022 636f 6c75 6d6e 5f6e 616d 6573  ", "column_names
+00005150: 223a 205b 2261 7363 222c 2022 6b65 7922  ": ["asc", "key"
+00005160: 5d7d 2c0a 2020 2020 2020 2020 2020 2020  ]},.            
+00005170: 2020 2020 7b22 6e61 6d65 223a 2022 692e      {"name": "i.
+00005180: 6861 7665 2e64 6f74 7322 2c20 2263 6f6c  have.dots", "col
+00005190: 756d 6e5f 6e61 6d65 7322 3a20 5b22 6222  umn_names": ["b"
+000051a0: 5d7d 2c0a 2020 2020 2020 2020 2020 2020  ]},.            
+000051b0: 2020 2020 7b22 6e61 6d65 223a 2022 6920      {"name": "i 
+000051c0: 6861 7665 2073 7061 6365 7322 2c20 2263  have spaces", "c
+000051d0: 6f6c 756d 6e5f 6e61 6d65 7322 3a20 5b22  olumn_names": ["
+000051e0: 6322 5d7d 2c0a 2020 2020 2020 2020 2020  c"]},.          
+000051f0: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
+00005200: 206b 6579 3d6f 7065 7261 746f 722e 6974   key=operator.it
+00005210: 656d 6765 7474 6572 2822 6e61 6d65 2229  emgetter("name")
+00005220: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00005230: 2020 2020 7461 626c 6520 3d20 5461 626c      table = Tabl
+00005240: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
+00005250: 7465 7374 7462 6c22 2c0a 2020 2020 2020  testtbl",.      
+00005260: 2020 2020 2020 6d65 7461 6461 7461 2c0a        metadata,.
+00005270: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
+00005280: 6d6e 2822 6964 222c 2073 716c 616c 6368  mn("id", sqlalch
+00005290: 656d 792e 494e 542c 2070 7269 6d61 7279  emy.INT, primary
+000052a0: 5f6b 6579 3d54 7275 6529 2c0a 2020 2020  _key=True),.    
+000052b0: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
+000052c0: 6122 2c20 5374 7269 6e67 2832 3029 292c  a", String(20)),
+000052d0: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
+000052e0: 756d 6e28 2262 222c 2053 7472 696e 6728  umn("b", String(
+000052f0: 3330 2929 2c0a 2020 2020 2020 2020 2020  30)),.          
+00005300: 2020 436f 6c75 6d6e 2822 6322 2c20 496e    Column("c", In
+00005310: 7465 6765 7229 2c0a 2020 2020 2020 2020  teger),.        
+00005320: 2020 2020 2320 7265 7365 7276 6564 2069      # reserved i
+00005330: 6465 6e74 6966 6965 7273 0a20 2020 2020  dentifiers.     
+00005340: 2020 2020 2020 2043 6f6c 756d 6e28 2261         Column("a
+00005350: 7363 222c 2053 7472 696e 6728 3330 2929  sc", String(30))
+00005360: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
+00005370: 6c75 6d6e 2822 6b65 7922 2c20 5374 7269  lumn("key", Stri
+00005380: 6e67 2833 3029 292c 0a20 2020 2020 2020  ng(30)),.       
+00005390: 2020 2020 2073 716c 616c 6368 656d 792e       sqlalchemy.
+000053a0: 496e 6465 7828 2275 6e69 7175 655f 6122  Index("unique_a"
+000053b0: 2c20 2261 222c 2075 6e69 7175 653d 5472  , "a", unique=Tr
+000053c0: 7565 292c 0a20 2020 2020 2020 2020 2020  ue),.           
+000053d0: 2073 716c 616c 6368 656d 792e 496e 6465   sqlalchemy.Inde
+000053e0: 7828 2275 6e69 7175 655f 615f 625f 6322  x("unique_a_b_c"
+000053f0: 2c20 2261 222c 2022 6222 2c20 2263 222c  , "a", "b", "c",
+00005400: 2075 6e69 7175 653d 5472 7565 292c 0a20   unique=True),. 
+00005410: 2020 2020 2020 2020 2020 2073 716c 616c             sqlal
+00005420: 6368 656d 792e 496e 6465 7828 2275 6e69  chemy.Index("uni
+00005430: 7175 655f 635f 615f 6222 2c20 2263 222c  que_c_a_b", "c",
+00005440: 2022 6122 2c20 2262 222c 2075 6e69 7175   "a", "b", uniqu
+00005450: 653d 5472 7565 292c 0a20 2020 2020 2020  e=True),.       
+00005460: 2020 2020 2073 716c 616c 6368 656d 792e       sqlalchemy.
+00005470: 496e 6465 7828 2275 6e69 7175 655f 6173  Index("unique_as
+00005480: 635f 6b65 7922 2c20 2261 7363 222c 2022  c_key", "asc", "
+00005490: 6b65 7922 2c20 756e 6971 7565 3d54 7275  key", unique=Tru
+000054a0: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+000054b0: 7363 6865 6d61 3d73 6368 656d 612c 0a20  schema=schema,. 
+000054c0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000054d0: 2074 6162 6c65 2e63 7265 6174 6528 636f   table.create(co
+000054e0: 6e6e 6563 7469 6f6e 290a 2020 2020 2020  nnection).      
+000054f0: 2020 636f 6e6e 6563 7469 6f6e 2e63 6f6e    connection.con
+00005500: 6e65 6374 696f 6e2e 636f 6d6d 6974 2829  nection.commit()
+00005510: 0a0a 2020 2020 2020 2020 696e 7370 6563  ..        inspec
+00005520: 746f 7220 3d20 696e 7370 6563 7428 636f  tor = inspect(co
+00005530: 6e6e 6563 7469 6f6e 290a 2020 2020 2020  nnection).      
+00005540: 2020 7265 666c 6563 7465 6420 3d20 736f    reflected = so
+00005550: 7274 6564 280a 2020 2020 2020 2020 2020  rted(.          
+00005560: 2020 696e 7370 6563 746f 722e 6765 745f    inspector.get_
+00005570: 756e 6971 7565 5f63 6f6e 7374 7261 696e  unique_constrain
+00005580: 7473 2822 7465 7374 7462 6c22 2c20 7363  ts("testtbl", sc
+00005590: 6865 6d61 3d73 6368 656d 6129 2c0a 2020  hema=schema),.  
+000055a0: 2020 2020 2020 2020 2020 6b65 793d 6f70            key=op
+000055b0: 6572 6174 6f72 2e69 7465 6d67 6574 7465  erator.itemgette
+000055c0: 7228 226e 616d 6522 292c 0a20 2020 2020  r("name"),.     
+000055d0: 2020 2029 0a0a 2020 2020 2020 2020 6e61     )..        na
+000055e0: 6d65 735f 7468 6174 5f64 7570 6c69 6361  mes_that_duplica
+000055f0: 7465 5f69 6e64 6578 203d 2073 6574 2829  te_index = set()
+00005600: 0a0a 2020 2020 2020 2020 666f 7220 6f72  ..        for or
+00005610: 6967 2c20 7265 666c 2069 6e20 7a69 7028  ig, refl in zip(
+00005620: 756e 6971 7565 732c 2072 6566 6c65 6374  uniques, reflect
+00005630: 6564 293a 0a20 2020 2020 2020 2020 2020  ed):.           
+00005640: 2023 2044 6966 6665 7265 6e74 2064 6961   # Different dia
+00005650: 6c65 6374 7320 6861 6e64 6c65 2064 7570  lects handle dup
+00005660: 6c69 6361 7465 2069 6e64 6578 2061 6e64  licate index and
+00005670: 2063 6f6e 7374 7261 696e 7473 0a20 2020   constraints.   
+00005680: 2020 2020 2020 2020 2023 2064 6966 6665           # diffe
+00005690: 7265 6e74 6c79 2c20 736f 2069 676e 6f72  rently, so ignor
+000056a0: 6520 7468 6973 2066 6c61 670a 2020 2020  e this flag.    
+000056b0: 2020 2020 2020 2020 6475 7065 203d 2072          dupe = r
+000056c0: 6566 6c2e 706f 7028 2264 7570 6c69 6361  efl.pop("duplica
+000056d0: 7465 735f 696e 6465 7822 2c20 4e6f 6e65  tes_index", None
+000056e0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+000056f0: 2064 7570 653a 0a20 2020 2020 2020 2020   dupe:.         
+00005700: 2020 2020 2020 206e 616d 6573 5f74 6861         names_tha
+00005710: 745f 6475 706c 6963 6174 655f 696e 6465  t_duplicate_inde
+00005720: 782e 6164 6428 6475 7065 290a 2020 2020  x.add(dupe).    
+00005730: 2020 2020 2020 2020 6571 5f28 6f72 6967          eq_(orig
+00005740: 2c20 7265 666c 290a 0a20 2020 2020 2020  , refl)..       
+00005750: 2072 6566 6c65 6374 6564 5f6d 6574 6164   reflected_metad
+00005760: 6174 6120 3d20 4d65 7461 4461 7461 2829  ata = MetaData()
+00005770: 0a20 2020 2020 2020 2072 6566 6c65 6374  .        reflect
+00005780: 6564 203d 2054 6162 6c65 280a 2020 2020  ed = Table(.    
+00005790: 2020 2020 2020 2020 2274 6573 7474 626c          "testtbl
+000057a0: 222c 0a20 2020 2020 2020 2020 2020 2072  ",.            r
+000057b0: 6566 6c65 6374 6564 5f6d 6574 6164 6174  eflected_metadat
+000057c0: 612c 0a20 2020 2020 2020 2020 2020 2061  a,.            a
+000057d0: 7574 6f6c 6f61 645f 7769 7468 3d63 6f6e  utoload_with=con
+000057e0: 6e65 6374 696f 6e2c 0a20 2020 2020 2020  nection,.       
+000057f0: 2020 2020 2073 6368 656d 613d 7363 6865       schema=sche
+00005800: 6d61 2c0a 2020 2020 2020 2020 290a 0a20  ma,.        ).. 
+00005810: 2020 2020 2020 2023 2074 6573 7420 2264         # test "d
+00005820: 6564 7570 6c69 6361 7465 7320 666f 7220  eduplicates for 
+00005830: 696e 6465 7822 206c 6f67 6963 2e20 2020  index" logic.   
+00005840: 4d79 5351 4c20 616e 6420 4f72 6163 6c65  MySQL and Oracle
+00005850: 0a20 2020 2020 2020 2023 2022 756e 6971  .        # "uniq
+00005860: 7565 2063 6f6e 7374 7261 696e 7473 2220  ue constraints" 
+00005870: 6172 6520 6163 7475 616c 6c79 2075 6e69  are actually uni
+00005880: 7175 6520 696e 6465 7865 7320 2877 6974  que indexes (wit
+00005890: 6820 706f 7373 6962 6c65 0a20 2020 2020  h possible.     
+000058a0: 2020 2023 2065 7863 6570 7469 6f6e 206f     # exception o
+000058b0: 6620 6120 756e 6971 7565 2074 6861 7420  f a unique that 
+000058c0: 6973 2061 2064 7570 6520 6f66 2061 6e6f  is a dupe of ano
+000058d0: 7468 6572 206f 6e65 2069 6e20 7468 6520  ther one in the 
+000058e0: 6361 7365 0a20 2020 2020 2020 2023 206f  case.        # o
+000058f0: 6620 4f72 6163 6c65 292e 2020 6d61 6b65  f Oracle).  make
+00005900: 2073 7572 6520 2320 7468 6579 2061 7265   sure # they are
+00005910: 6e27 7420 6475 706c 6963 6174 6564 2e0a  n't duplicated..
+00005920: 2020 2020 2020 2020 6964 785f 6e61 6d65          idx_name
+00005930: 7320 3d20 7365 7428 5b69 6478 2e6e 616d  s = set([idx.nam
+00005940: 6520 666f 7220 6964 7820 696e 2072 6566  e for idx in ref
+00005950: 6c65 6374 6564 2e69 6e64 6578 6573 5d29  lected.indexes])
+00005960: 0a20 2020 2020 2020 2075 715f 6e61 6d65  .        uq_name
+00005970: 7320 3d20 7365 7428 0a20 2020 2020 2020  s = set(.       
+00005980: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+00005990: 2020 2020 2020 2075 712e 6e61 6d65 0a20         uq.name. 
+000059a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000059b0: 6f72 2075 7120 696e 2072 6566 6c65 6374  or uq in reflect
+000059c0: 6564 2e63 6f6e 7374 7261 696e 7473 0a20  ed.constraints. 
+000059d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000059e0: 6620 6973 696e 7374 616e 6365 2875 712c  f isinstance(uq,
+000059f0: 2073 716c 616c 6368 656d 792e 556e 6971   sqlalchemy.Uniq
+00005a00: 7565 436f 6e73 7472 6169 6e74 290a 2020  ueConstraint).  
+00005a10: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+00005a20: 2020 2020 292e 6469 6666 6572 656e 6365      ).difference
+00005a30: 285b 2275 6e69 7175 655f 635f 615f 6222  (["unique_c_a_b"
+00005a40: 5d29 0a0a 2020 2020 2020 2020 6173 7365  ])..        asse
+00005a50: 7274 206e 6f74 2069 6478 5f6e 616d 6573  rt not idx_names
+00005a60: 2e69 6e74 6572 7365 6374 696f 6e28 7571  .intersection(uq
+00005a70: 5f6e 616d 6573 290a 2020 2020 2020 2020  _names).        
+00005a80: 6966 206e 616d 6573 5f74 6861 745f 6475  if names_that_du
+00005a90: 706c 6963 6174 655f 696e 6465 783a 0a20  plicate_index:. 
+00005aa0: 2020 2020 2020 2020 2020 2065 715f 286e             eq_(n
+00005ab0: 616d 6573 5f74 6861 745f 6475 706c 6963  ames_that_duplic
+00005ac0: 6174 655f 696e 6465 782c 2069 6478 5f6e  ate_index, idx_n
+00005ad0: 616d 6573 290a 2020 2020 2020 2020 2020  ames).          
+00005ae0: 2020 6571 5f28 7571 5f6e 616d 6573 2c20    eq_(uq_names, 
+00005af0: 7365 7428 2929 0a0a 2020 2020 4074 6573  set())..    @tes
+00005b00: 7469 6e67 2e70 726f 7669 6465 5f6d 6574  ting.provide_met
+00005b10: 6164 6174 610a 2020 2020 6465 6620 7465  adata.    def te
+00005b20: 7374 5f75 6e69 7175 655f 636f 6e73 7472  st_unique_constr
+00005b30: 6169 6e74 5f72 6169 7365 7328 7365 6c66  aint_raises(self
+00005b40: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00005b50: 2020 2020 2020 2043 6865 636b 696e 6720         Checking 
+00005b60: 7468 6174 2075 6e69 7175 6520 636f 6e73  that unique cons
+00005b70: 7472 6169 6e74 2063 7265 6174 696f 6e0a  traint creation.
+00005b80: 2020 2020 2020 2020 6661 696c 7320 6475          fails du
+00005b90: 6520 746f 2061 2050 726f 6772 616d 6d69  e to a Programmi
+00005ba0: 6e67 4572 726f 722e 0a20 2020 2020 2020  ngError..       
+00005bb0: 2022 2222 0a20 2020 2020 2020 206d 6574   """.        met
+00005bc0: 6164 6174 6120 3d20 4d65 7461 4461 7461  adata = MetaData
+00005bd0: 2873 656c 662e 6269 6e64 290a 2020 2020  (self.bind).    
+00005be0: 2020 2020 5461 626c 6528 0a20 2020 2020      Table(.     
+00005bf0: 2020 2020 2020 2022 7573 6572 5f74 6d70         "user_tmp
+00005c00: 5f66 6169 6c75 7265 222c 0a20 2020 2020  _failure",.     
+00005c10: 2020 2020 2020 206d 6574 6164 6174 612c         metadata,
+00005c20: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
+00005c30: 756d 6e28 2269 6422 2c20 7371 6c61 6c63  umn("id", sqlalc
+00005c40: 6865 6d79 2e49 4e54 2c20 7072 696d 6172  hemy.INT, primar
+00005c50: 795f 6b65 793d 5472 7565 292c 0a20 2020  y_key=True),.   
+00005c60: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
+00005c70: 226e 616d 6522 2c20 7371 6c61 6c63 6865  "name", sqlalche
+00005c80: 6d79 2e56 4152 4348 4152 2835 3029 292c  my.VARCHAR(50)),
+00005c90: 0a20 2020 2020 2020 2020 2020 2073 716c  .            sql
+00005ca0: 616c 6368 656d 792e 556e 6971 7565 436f  alchemy.UniqueCo
+00005cb0: 6e73 7472 6169 6e74 2822 6e61 6d65 222c  nstraint("name",
+00005cc0: 206e 616d 653d 2275 7365 725f 746d 705f   name="user_tmp_
+00005cd0: 7571 2229 2c0a 2020 2020 2020 2020 290a  uq"),.        ).
+00005ce0: 0a20 2020 2020 2020 2077 6974 6820 7079  .        with py
+00005cf0: 7465 7374 2e72 6169 7365 7328 7370 616e  test.raises(span
+00005d00: 6e65 725f 6462 6170 692e 6578 6365 7074  ner_dbapi.except
+00005d10: 696f 6e73 2e50 726f 6772 616d 6d69 6e67  ions.Programming
+00005d20: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
+00005d30: 2020 2020 6d65 7461 6461 7461 2e63 7265      metadata.cre
+00005d40: 6174 655f 616c 6c28 290a 0a20 2020 2040  ate_all()..    @
+00005d50: 7465 7374 696e 672e 7072 6f76 6964 655f  testing.provide_
+00005d60: 6d65 7461 6461 7461 0a20 2020 2064 6566  metadata.    def
+00005d70: 205f 7465 7374 5f67 6574 5f74 6162 6c65   _test_get_table
+00005d80: 5f6e 616d 6573 2873 656c 662c 2073 6368  _names(self, sch
+00005d90: 656d 613d 4e6f 6e65 2c20 7461 626c 655f  ema=None, table_
+00005da0: 7479 7065 3d22 7461 626c 6522 2c20 6f72  type="table", or
+00005db0: 6465 725f 6279 3d4e 6f6e 6529 3a0a 2020  der_by=None):.  
+00005dc0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00005dd0: 2020 5350 414e 4e45 5220 4f56 4552 5249    SPANNER OVERRI
+00005de0: 4445 3a0a 0a20 2020 2020 2020 2053 7061  DE:..        Spa
+00005df0: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
+00005e00: 706f 7274 2074 656d 706f 7261 7279 2074  port temporary t
+00005e10: 6162 6c65 732c 2073 6f20 7265 616c 2074  ables, so real t
+00005e20: 6162 6c65 7320 6172 650a 2020 2020 2020  ables are.      
+00005e30: 2020 7573 6564 2066 6f72 2074 6573 7469    used for testi
+00005e40: 6e67 2e20 4173 2074 6865 206f 7269 6769  ng. As the origi
+00005e50: 6e61 6c20 7465 7374 2065 7870 6563 7473  nal test expects
+00005e60: 206f 6e6c 7920 7265 616c 0a20 2020 2020   only real.     
+00005e70: 2020 2074 6162 6c65 7320 746f 2062 6520     tables to be 
+00005e80: 7265 6164 2c20 616e 6420 696e 2053 7061  read, and in Spa
+00005e90: 6e6e 6572 2061 6c6c 2074 6865 2074 6162  nner all the tab
+00005ea0: 6c65 7320 6172 6520 7265 616c 2c0a 2020  les are real,.  
+00005eb0: 2020 2020 2020 6578 7065 6374 6564 2072        expected r
+00005ec0: 6573 756c 7473 206f 7665 7272 6964 6520  esults override 
+00005ed0: 6973 2072 6571 7569 7265 642e 0a20 2020  is required..   
+00005ee0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00005ef0: 205f 6967 6e6f 7265 5f74 6162 6c65 7320   _ignore_tables 
+00005f00: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00005f10: 2263 6f6d 6d65 6e74 5f74 6573 7422 2c0a  "comment_test",.
+00005f20: 2020 2020 2020 2020 2020 2020 226e 6f6e              "non
+00005f30: 636f 6c5f 6964 785f 7465 7374 5f70 6b22  col_idx_test_pk"
+00005f40: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
+00005f50: 6f6e 636f 6c5f 6964 785f 7465 7374 5f6e  oncol_idx_test_n
+00005f60: 6f70 6b22 2c0a 2020 2020 2020 2020 2020  opk",.          
+00005f70: 2020 226c 6f63 616c 5f74 6162 6c65 222c    "local_table",
+00005f80: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
+00005f90: 6d6f 7465 5f74 6162 6c65 222c 0a20 2020  mote_table",.   
+00005fa0: 2020 2020 2020 2020 2022 7265 6d6f 7465           "remote
+00005fb0: 5f74 6162 6c65 5f32 222c 0a20 2020 2020  _table_2",.     
+00005fc0: 2020 205d 0a20 2020 2020 2020 206d 6574     ].        met
+00005fd0: 6120 3d20 7365 6c66 2e6d 6574 6164 6174  a = self.metadat
+00005fe0: 610a 0a20 2020 2020 2020 2069 6e73 7020  a..        insp 
+00005ff0: 3d20 696e 7370 6563 7428 6d65 7461 2e62  = inspect(meta.b
+00006000: 696e 6429 0a0a 2020 2020 2020 2020 6966  ind)..        if
+00006010: 2074 6162 6c65 5f74 7970 6520 3d3d 2022   table_type == "
+00006020: 7669 6577 223a 0a20 2020 2020 2020 2020  view":.         
+00006030: 2020 2074 6162 6c65 5f6e 616d 6573 203d     table_names =
+00006040: 2069 6e73 702e 6765 745f 7669 6577 5f6e   insp.get_view_n
+00006050: 616d 6573 2873 6368 656d 6129 0a20 2020  ames(schema).   
+00006060: 2020 2020 2020 2020 2074 6162 6c65 5f6e           table_n
+00006070: 616d 6573 2e73 6f72 7428 290a 2020 2020  ames.sort().    
+00006080: 2020 2020 2020 2020 616e 7377 6572 203d          answer =
+00006090: 205b 2265 6d61 696c 5f61 6464 7265 7373   ["email_address
+000060a0: 6573 5f76 222c 2022 7573 6572 735f 7622  es_v", "users_v"
+000060b0: 5d0a 2020 2020 2020 2020 2020 2020 6571  ].            eq
+000060c0: 5f28 736f 7274 6564 2874 6162 6c65 5f6e  _(sorted(table_n
+000060d0: 616d 6573 292c 2061 6e73 7765 7229 0a20  ames), answer). 
+000060e0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000060f0: 2020 2020 2020 2020 2069 6620 6f72 6465           if orde
+00006100: 725f 6279 3a0a 2020 2020 2020 2020 2020  r_by:.          
+00006110: 2020 2020 2020 7461 626c 6573 203d 205b        tables = [
+00006120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006130: 2020 2020 2072 6563 5b30 5d0a 2020 2020       rec[0].    
+00006140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006150: 666f 7220 7265 6320 696e 2069 6e73 702e  for rec in insp.
+00006160: 6765 745f 736f 7274 6564 5f74 6162 6c65  get_sorted_table
+00006170: 5f61 6e64 5f66 6b63 5f6e 616d 6573 2873  _and_fkc_names(s
+00006180: 6368 656d 6129 0a20 2020 2020 2020 2020  chema).         
+00006190: 2020 2020 2020 2020 2020 2069 6620 7265             if re
+000061a0: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
+000061b0: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
+000061c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000061d0: 2020 2020 2020 2020 2074 6162 6c65 7320           tables 
+000061e0: 3d20 696e 7370 2e67 6574 5f74 6162 6c65  = insp.get_table
+000061f0: 5f6e 616d 6573 2873 6368 656d 6129 0a20  _names(schema). 
+00006200: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+00006210: 5f6e 616d 6573 203d 205b 7420 666f 7220  _names = [t for 
+00006220: 7420 696e 2074 6162 6c65 7320 6966 2074  t in tables if t
+00006230: 206e 6f74 2069 6e20 5f69 676e 6f72 655f   not in _ignore_
+00006240: 7461 626c 6573 5d0a 0a20 2020 2020 2020  tables]..       
+00006250: 2020 2020 2069 6620 6f72 6465 725f 6279       if order_by
+00006260: 203d 3d20 2266 6f72 6569 676e 5f6b 6579   == "foreign_key
+00006270: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00006280: 2020 2061 6e73 7765 7220 3d20 7b22 6469     answer = {"di
+00006290: 6e67 616c 696e 6773 222c 2022 656d 6169  ngalings", "emai
+000062a0: 6c5f 6164 6472 6573 7365 7322 2c20 2275  l_addresses", "u
+000062b0: 7365 725f 746d 7022 2c20 2275 7365 7273  ser_tmp", "users
+000062c0: 227d 0a20 2020 2020 2020 2020 2020 2020  "}.             
+000062d0: 2020 2065 715f 2873 6574 2874 6162 6c65     eq_(set(table
+000062e0: 5f6e 616d 6573 292c 2061 6e73 7765 7229  _names), answer)
+000062f0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00006300: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00006310: 2020 2061 6e73 7765 7220 3d20 5b22 6469     answer = ["di
+00006320: 6e67 616c 696e 6773 222c 2022 656d 6169  ngalings", "emai
+00006330: 6c5f 6164 6472 6573 7365 7322 2c20 2275  l_addresses", "u
+00006340: 7365 725f 746d 7022 2c20 2275 7365 7273  ser_tmp", "users
+00006350: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00006360: 2020 2065 715f 2873 6f72 7465 6428 7461     eq_(sorted(ta
+00006370: 626c 655f 6e61 6d65 7329 2c20 616e 7377  ble_names), answ
+00006380: 6572 290a 0a20 2020 2040 7079 7465 7374  er)..    @pytest
+00006390: 2e6d 6172 6b2e 736b 6970 2822 5370 616e  .mark.skip("Span
+000063a0: 6e65 7220 646f 6573 6e27 7420 7375 7070  ner doesn't supp
+000063b0: 6f72 7420 7465 6d70 6f72 6172 7920 7461  ort temporary ta
+000063c0: 626c 6573 2229 0a20 2020 2064 6566 2074  bles").    def t
+000063d0: 6573 745f 6765 745f 7465 6d70 5f74 6162  est_get_temp_tab
+000063e0: 6c65 5f69 6e64 6578 6573 2873 656c 6629  le_indexes(self)
+000063f0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+00006400: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+00006410: 2e73 6b69 7028 2253 7061 6e6e 6572 2064  .skip("Spanner d
+00006420: 6f65 736e 2774 2073 7570 706f 7274 2074  oesn't support t
+00006430: 656d 706f 7261 7279 2074 6162 6c65 7322  emporary tables"
+00006440: 290a 2020 2020 6465 6620 7465 7374 5f67  ).    def test_g
+00006450: 6574 5f74 656d 705f 7461 626c 655f 756e  et_temp_table_un
+00006460: 6971 7565 5f63 6f6e 7374 7261 696e 7473  ique_constraints
+00006470: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00006480: 7061 7373 0a0a 2020 2020 4070 7974 6573  pass..    @pytes
+00006490: 742e 6d61 726b 2e73 6b69 7028 2253 7061  t.mark.skip("Spa
+000064a0: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
+000064b0: 706f 7274 2074 656d 706f 7261 7279 2074  port temporary t
+000064c0: 6162 6c65 7322 290a 2020 2020 6465 6620  ables").    def 
+000064d0: 7465 7374 5f67 6574 5f74 656d 705f 7461  test_get_temp_ta
+000064e0: 626c 655f 636f 6c75 6d6e 7328 7365 6c66  ble_columns(self
+000064f0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+00006500: 0a20 2020 2064 6566 205f 6173 7365 7274  .    def _assert
+00006510: 5f69 6e73 705f 696e 6465 7865 7328 7365  _insp_indexes(se
+00006520: 6c66 2c20 696e 6465 7865 732c 2065 7870  lf, indexes, exp
+00006530: 6563 7465 645f 696e 6465 7865 7329 3a0a  ected_indexes):.
+00006540: 2020 2020 2020 2020 6578 7065 6374 6564          expected
+00006550: 5f69 6e64 6578 6573 2e73 6f72 7428 6b65  _indexes.sort(ke
+00006560: 793d 6c61 6d62 6461 2069 7465 6d3a 2069  y=lambda item: i
+00006570: 7465 6d5b 226e 616d 6522 5d29 0a0a 2020  tem["name"])..  
+00006580: 2020 2020 2020 696e 6465 785f 6e61 6d65        index_name
+00006590: 7320 3d20 5b64 5b22 6e61 6d65 225d 2066  s = [d["name"] f
+000065a0: 6f72 2064 2069 6e20 696e 6465 7865 735d  or d in indexes]
+000065b0: 0a20 2020 2020 2020 2065 7870 5f69 6e64  .        exp_ind
+000065c0: 6578 5f6e 616d 6573 203d 205b 645b 226e  ex_names = [d["n
+000065d0: 616d 6522 5d20 666f 7220 6420 696e 2065  ame"] for d in e
+000065e0: 7870 6563 7465 645f 696e 6465 7865 735d  xpected_indexes]
+000065f0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00006600: 736f 7274 6564 2869 6e64 6578 5f6e 616d  sorted(index_nam
+00006610: 6573 2920 3d3d 2073 6f72 7465 6428 6578  es) == sorted(ex
+00006620: 705f 696e 6465 785f 6e61 6d65 7329 0a0a  p_index_names)..
+00006630: 0a63 6c61 7373 2043 6f6d 706f 7369 7465  .class Composite
+00006640: 4b65 7952 6566 6c65 6374 696f 6e54 6573  KeyReflectionTes
+00006650: 7428 5f43 6f6d 706f 7369 7465 4b65 7952  t(_CompositeKeyR
+00006660: 6566 6c65 6374 696f 6e54 6573 7429 3a0a  eflectionTest):.
+00006670: 2020 2020 4074 6573 7469 6e67 2e72 6571      @testing.req
+00006680: 7569 7265 732e 666f 7265 6967 6e5f 6b65  uires.foreign_ke
+00006690: 795f 636f 6e73 7472 6169 6e74 5f72 6566  y_constraint_ref
+000066a0: 6c65 6374 696f 6e0a 2020 2020 6465 6620  lection.    def 
+000066b0: 7465 7374 5f66 6b5f 636f 6c75 6d6e 5f6f  test_fk_column_o
+000066c0: 7264 6572 2873 656c 6629 3a0a 2020 2020  rder(self):.    
+000066d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000066e0: 5350 414e 4e45 5220 4f56 4552 5249 4445  SPANNER OVERRIDE
+000066f0: 3a0a 0a20 2020 2020 2020 2053 7061 6e6e  :..        Spann
+00006700: 6572 2063 6f6c 756d 6e20 7573 6167 6520  er column usage 
+00006710: 7265 666c 6563 7469 6f6e 2064 6f65 736e  reflection doesn
+00006720: 2774 2073 7570 706f 7274 2064 6574 6572  't support deter
+00006730: 6d65 6e69 7374 6963 0a20 2020 2020 2020  menistic.       
+00006740: 206f 7264 6572 696e 672e 204f 7665 7272   ordering. Overr
+00006750: 6964 696e 6720 7468 6520 7465 7374 2074  iding the test t
+00006760: 6f20 6368 6563 6b20 7468 6174 2063 6f6c  o check that col
+00006770: 756d 6e73 2061 7265 0a20 2020 2020 2020  umns are.       
+00006780: 2072 6566 6c65 6374 6564 2063 6f72 7265   reflected corre
+00006790: 6374 6c79 2c20 7769 7468 6f75 7420 636f  ctly, without co
+000067a0: 6e73 6964 6572 696e 6720 7468 6569 7220  nsidering their 
+000067b0: 6f72 6465 722e 0a20 2020 2020 2020 2022  order..        "
+000067c0: 2222 0a20 2020 2020 2020 2023 2074 6573  "".        # tes
+000067d0: 7420 666f 7220 6973 7375 6520 2335 3636  t for issue #566
+000067e0: 310a 2020 2020 2020 2020 696e 7370 203d  1.        insp =
+000067f0: 2069 6e73 7065 6374 2873 656c 662e 6269   inspect(self.bi
+00006800: 6e64 290a 2020 2020 2020 2020 666f 7265  nd).        fore
+00006810: 6967 6e5f 6b65 7973 203d 2069 6e73 702e  ign_keys = insp.
+00006820: 6765 745f 666f 7265 6967 6e5f 6b65 7973  get_foreign_keys
+00006830: 2873 656c 662e 7461 626c 6573 2e74 6232  (self.tables.tb2
+00006840: 2e6e 616d 6529 0a20 2020 2020 2020 2065  .name).        e
+00006850: 715f 286c 656e 2866 6f72 6569 676e 5f6b  q_(len(foreign_k
+00006860: 6579 7329 2c20 3129 0a20 2020 2020 2020  eys), 1).       
+00006870: 2066 6b65 7931 203d 2066 6f72 6569 676e   fkey1 = foreign
+00006880: 5f6b 6579 735b 305d 0a20 2020 2020 2020  _keys[0].       
+00006890: 2065 715f 2873 6574 2866 6b65 7931 2e67   eq_(set(fkey1.g
+000068a0: 6574 2822 7265 6665 7272 6564 5f63 6f6c  et("referred_col
+000068b0: 756d 6e73 2229 292c 207b 226e 616d 6522  umns")), {"name"
+000068c0: 2c20 2269 6422 2c20 2261 7474 7222 7d29  , "id", "attr"})
+000068d0: 0a20 2020 2020 2020 2065 715f 2873 6574  .        eq_(set
+000068e0: 2866 6b65 7931 2e67 6574 2822 636f 6e73  (fkey1.get("cons
+000068f0: 7472 6169 6e65 645f 636f 6c75 6d6e 7322  trained_columns"
+00006900: 2929 2c20 7b22 706e 616d 6522 2c20 2270  )), {"pname", "p
+00006910: 6964 222c 2022 7061 7474 7222 7d29 0a0a  id", "pattr"})..
+00006920: 0a40 7079 7465 7374 2e6d 6172 6b2e 736b  .@pytest.mark.sk
+00006930: 6970 2822 5370 616e 6e65 7220 646f 6573  ip("Spanner does
+00006940: 6e27 7420 7375 7070 6f72 7420 7175 6f74  n't support quot
+00006950: 6573 2069 6e20 7461 626c 6520 6e61 6d65  es in table name
+00006960: 732e 2229 0a63 6c61 7373 2051 756f 7465  s.").class Quote
+00006970: 644e 616d 6541 7267 756d 656e 7454 6573  dNameArgumentTes
+00006980: 7428 5f51 756f 7465 644e 616d 6541 7267  t(_QuotedNameArg
+00006990: 756d 656e 7454 6573 7429 3a0a 2020 2020  umentTest):.    
+000069a0: 7061 7373 0a0a 0a63 6c61 7373 205f 4461  pass...class _Da
+000069b0: 7465 4669 7874 7572 6528 5f5f 4461 7465  teFixture(__Date
+000069c0: 4669 7874 7572 6529 3a0a 2020 2020 636f  Fixture):.    co
+000069d0: 6d70 6172 6520 3d20 4e6f 6e65 0a0a 2020  mpare = None..  
+000069e0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+000069f0: 2020 2064 6566 2064 6566 696e 655f 7461     def define_ta
+00006a00: 626c 6573 2863 6c73 2c20 6d65 7461 6461  bles(cls, metada
+00006a10: 7461 293a 0a20 2020 2020 2020 2022 2222  ta):.        """
+00006a20: 0a20 2020 2020 2020 2053 5041 4e4e 4552  .        SPANNER
+00006a30: 204f 5645 5252 4944 453a 0a0a 2020 2020   OVERRIDE:..    
+00006a40: 2020 2020 436c 6f75 6420 5370 616e 6e65      Cloud Spanne
+00006a50: 7220 646f 6573 6e27 7420 7375 7070 6f72  r doesn't suppor
+00006a60: 7420 6175 746f 2069 6e63 7265 6d65 6e74  t auto increment
+00006a70: 696e 6720 6964 7320 6665 6174 7572 652c  ing ids feature,
+00006a80: 0a20 2020 2020 2020 2077 6869 6368 2069  .        which i
+00006a90: 7320 7573 6564 2062 7920 7468 6520 6f72  s used by the or
+00006aa0: 6967 696e 616c 2074 6573 742e 204f 7665  iginal test. Ove
+00006ab0: 7272 6964 696e 6720 7468 6520 7465 7374  rriding the test
+00006ac0: 2064 6174 610a 2020 2020 2020 2020 6372   data.        cr
+00006ad0: 6561 7469 6f6e 206d 6574 686f 6420 746f  eation method to
+00006ae0: 2064 6973 6162 6c65 2061 7574 6f69 6e63   disable autoinc
+00006af0: 7265 6d65 6e74 2061 6e64 206d 616b 6520  rement and make 
+00006b00: 6964 2063 6f6c 756d 6e0a 2020 2020 2020  id column.      
+00006b10: 2020 6e75 6c6c 6162 6c65 2e0a 2020 2020    nullable..    
+00006b20: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00006b30: 2063 6c61 7373 2044 6563 6f72 6174 6564   class Decorated
+00006b40: 2873 716c 616c 6368 656d 792e 5479 7065  (sqlalchemy.Type
+00006b50: 4465 636f 7261 746f 7229 3a0a 2020 2020  Decorator):.    
+00006b60: 2020 2020 2020 2020 696d 706c 203d 2063          impl = c
+00006b70: 6c73 2e64 6174 6174 7970 650a 2020 2020  ls.datatype.    
+00006b80: 2020 2020 2020 2020 6361 6368 655f 6f6b          cache_ok
+00006b90: 203d 2054 7275 650a 0a20 2020 2020 2020   = True..       
+00006ba0: 2054 6162 6c65 280a 2020 2020 2020 2020   Table(.        
+00006bb0: 2020 2020 2264 6174 655f 7461 626c 6522      "date_table"
+00006bc0: 2c0a 2020 2020 2020 2020 2020 2020 6d65  ,.            me
+00006bd0: 7461 6461 7461 2c0a 2020 2020 2020 2020  tadata,.        
+00006be0: 2020 2020 436f 6c75 6d6e 2822 6964 222c      Column("id",
+00006bf0: 2049 6e74 6567 6572 2c20 7072 696d 6172   Integer, primar
+00006c00: 795f 6b65 793d 5472 7565 2c20 6e75 6c6c  y_key=True, null
+00006c10: 6162 6c65 3d54 7275 6529 2c0a 2020 2020  able=True),.    
+00006c20: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
+00006c30: 6461 7465 5f64 6174 6122 2c20 636c 732e  date_data", cls.
+00006c40: 6461 7461 7479 7065 292c 0a20 2020 2020  datatype),.     
+00006c50: 2020 2020 2020 2043 6f6c 756d 6e28 2264         Column("d
+00006c60: 6563 6f72 6174 6564 5f64 6174 655f 6461  ecorated_date_da
+00006c70: 7461 222c 2044 6563 6f72 6174 6564 292c  ta", Decorated),
+00006c80: 0a20 2020 2020 2020 2029 0a0a 0a63 6c61  .        )...cla
+00006c90: 7373 2044 6174 6554 6573 7428 5f44 6174  ss DateTest(_Dat
+00006ca0: 6554 6573 7429 3a0a 2020 2020 2222 220a  eTest):.    """.
+00006cb0: 2020 2020 5350 414e 4e45 5220 4f56 4552      SPANNER OVER
+00006cc0: 5249 4445 3a0a 0a20 2020 2044 6174 6554  RIDE:..    DateT
+00006cd0: 6573 7420 7465 7374 7320 7573 6564 2073  est tests used s
+00006ce0: 616d 6520 636c 6173 7320 6d65 7468 6f64  ame class method
+00006cf0: 2074 6f20 6372 6561 7465 2074 6162 6c65   to create table
+00006d00: 2c20 736f 2074 6f20 6176 6f69 6420 7468  , so to avoid th
+00006d10: 6f73 6520 6661 696c 7572 6573 0a20 2020  ose failures.   
+00006d20: 2061 6e64 206d 6169 6e74 6169 6e20 4452   and maintain DR
+00006d30: 5920 636f 6e63 6570 7420 6a75 7374 2069  Y concept just i
+00006d40: 6e68 6572 6974 2074 6865 2063 6c61 7373  nherit the class
+00006d50: 2074 6f20 7275 6e20 7465 7374 7320 7375   to run tests su
+00006d60: 6363 6573 7366 756c 6c79 2e0a 2020 2020  ccessfully..    
+00006d70: 2222 220a 0a20 2020 2040 7079 7465 7374  """..    @pytest
+00006d80: 2e6d 6172 6b2e 736b 6970 6966 280a 2020  .mark.skipif(.  
+00006d90: 2020 2020 2020 626f 6f6c 286f 732e 656e        bool(os.en
+00006da0: 7669 726f 6e2e 6765 7428 2253 5041 4e4e  viron.get("SPANN
+00006db0: 4552 5f45 4d55 4c41 544f 525f 484f 5354  ER_EMULATOR_HOST
+00006dc0: 2229 292c 2072 6561 736f 6e3d 2253 6b69  ")), reason="Ski
+00006dd0: 7070 6564 206f 6e20 656d 756c 6174 6f72  pped on emulator
+00006de0: 220a 2020 2020 290a 2020 2020 6465 6620  ".    ).    def 
+00006df0: 7465 7374 5f6e 756c 6c5f 626f 756e 645f  test_null_bound_
+00006e00: 636f 6d70 6172 6973 6f6e 2873 656c 6629  comparison(self)
+00006e10: 3a0a 2020 2020 2020 2020 7375 7065 7228  :.        super(
+00006e20: 292e 7465 7374 5f6e 756c 6c5f 626f 756e  ).test_null_boun
+00006e30: 645f 636f 6d70 6172 6973 6f6e 2829 0a0a  d_comparison()..
+00006e40: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+00006e50: 2e73 6b69 7069 6628 0a20 2020 2020 2020  .skipif(.       
+00006e60: 2062 6f6f 6c28 6f73 2e65 6e76 6972 6f6e   bool(os.environ
+00006e70: 2e67 6574 2822 5350 414e 4e45 525f 454d  .get("SPANNER_EM
+00006e80: 554c 4154 4f52 5f48 4f53 5422 2929 2c20  ULATOR_HOST")), 
+00006e90: 7265 6173 6f6e 3d22 536b 6970 7065 6420  reason="Skipped 
+00006ea0: 6f6e 2065 6d75 6c61 746f 7222 0a20 2020  on emulator".   
+00006eb0: 2029 0a20 2020 2064 6566 2074 6573 745f   ).    def test_
+00006ec0: 6e75 6c6c 2873 656c 662c 2063 6f6e 6e65  null(self, conne
+00006ed0: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
+00006ee0: 7375 7065 7228 292e 7465 7374 5f6e 756c  super().test_nul
+00006ef0: 6c28 636f 6e6e 6563 7469 6f6e 290a 0a0a  l(connection)...
+00006f00: 636c 6173 7320 4354 4554 6573 7428 5f43  class CTETest(_C
+00006f10: 5445 5465 7374 293a 0a20 2020 2040 636c  TETest):.    @cl
+00006f20: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
+00006f30: 6620 6465 6669 6e65 5f74 6162 6c65 7328  f define_tables(
+00006f40: 636c 732c 206d 6574 6164 6174 6129 3a0a  cls, metadata):.
+00006f50: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00006f60: 2020 2020 5468 6520 6f72 6967 696e 616c      The original
+00006f70: 206d 6574 686f 6420 6372 6561 7465 7320   method creates 
+00006f80: 6120 666f 7265 6967 6e20 6b65 7920 7769  a foreign key wi
+00006f90: 7468 6f75 7420 6120 6e61 6d65 2c0a 2020  thout a name,.  
+00006fa0: 2020 2020 2020 7768 6963 6820 6361 7573        which caus
+00006fb0: 6573 2074 726f 7562 6c65 7320 6f6e 2074  es troubles on t
+00006fc0: 6573 7420 636c 6561 6e75 702e 204f 7665  est cleanup. Ove
+00006fd0: 7272 6964 696e 6720 7468 650a 2020 2020  rriding the.    
+00006fe0: 2020 2020 6d65 7468 6f64 2074 6f20 6578      method to ex
+00006ff0: 706c 6963 6974 6c79 2073 6574 2061 2066  plicitly set a f
+00007000: 6f72 6569 676e 206b 6579 206e 616d 652e  oreign key name.
+00007010: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00007020: 2020 2020 2054 6162 6c65 280a 2020 2020       Table(.    
+00007030: 2020 2020 2020 2020 2273 6f6d 655f 7461          "some_ta
+00007040: 626c 6522 2c0a 2020 2020 2020 2020 2020  ble",.          
+00007050: 2020 6d65 7461 6461 7461 2c0a 2020 2020    metadata,.    
+00007060: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
+00007070: 6964 222c 2049 6e74 6567 6572 2c20 7072  id", Integer, pr
+00007080: 696d 6172 795f 6b65 793d 5472 7565 292c  imary_key=True),
+00007090: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
+000070a0: 756d 6e28 2264 6174 6122 2c20 5374 7269  umn("data", Stri
+000070b0: 6e67 2835 3029 292c 0a20 2020 2020 2020  ng(50)),.       
+000070c0: 2020 2020 2043 6f6c 756d 6e28 2270 6172       Column("par
+000070d0: 656e 745f 6964 222c 2046 6f72 6569 676e  ent_id", Foreign
+000070e0: 4b65 7928 2273 6f6d 655f 7461 626c 652e  Key("some_table.
+000070f0: 6964 222c 206e 616d 653d 2266 6b5f 736f  id", name="fk_so
+00007100: 6d65 5f74 6162 6c65 2229 292c 0a20 2020  me_table")),.   
+00007110: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00007120: 5461 626c 6528 0a20 2020 2020 2020 2020  Table(.         
+00007130: 2020 2022 736f 6d65 5f6f 7468 6572 5f74     "some_other_t
+00007140: 6162 6c65 222c 0a20 2020 2020 2020 2020  able",.         
+00007150: 2020 206d 6574 6164 6174 612c 0a20 2020     metadata,.   
+00007160: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
+00007170: 2269 6422 2c20 496e 7465 6765 722c 2070  "id", Integer, p
+00007180: 7269 6d61 7279 5f6b 6579 3d54 7275 6529  rimary_key=True)
+00007190: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
+000071a0: 6c75 6d6e 2822 6461 7461 222c 2053 7472  lumn("data", Str
+000071b0: 696e 6728 3530 2929 2c0a 2020 2020 2020  ing(50)),.      
+000071c0: 2020 2020 2020 436f 6c75 6d6e 2822 7061        Column("pa
+000071d0: 7265 6e74 5f69 6422 2c20 496e 7465 6765  rent_id", Intege
+000071e0: 7229 2c0a 2020 2020 2020 2020 290a 0a20  r),.        ).. 
+000071f0: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
+00007200: 736b 6970 2822 494e 5345 5254 2066 726f  skip("INSERT fro
+00007210: 6d20 5749 5448 2073 7562 7175 6572 7920  m WITH subquery 
+00007220: 6973 206e 6f74 2073 7570 706f 7274 6564  is not supported
+00007230: 2229 0a20 2020 2064 6566 2074 6573 745f  ").    def test_
+00007240: 696e 7365 7274 5f66 726f 6d5f 7365 6c65  insert_from_sele
+00007250: 6374 5f72 6f75 6e64 5f74 7269 7028 7365  ct_round_trip(se
+00007260: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00007270: 0a20 2020 2020 2020 2054 6865 2074 6573  .        The tes
+00007280: 7420 6368 6563 6b73 2069 6620 616e 2049  t checks if an I
+00007290: 4e53 4552 5420 6361 6e20 6265 2064 6f6e  NSERT can be don
+000072a0: 6520 6672 6f6d 2061 2063 7465 2c20 6c69  e from a cte, li
+000072b0: 6b65 3a0a 0a20 2020 2020 2020 2057 4954  ke:..        WIT
+000072c0: 4820 736f 6d65 5f63 7465 2041 5320 282e  H some_cte AS (.
+000072d0: 2e2e 290a 2020 2020 2020 2020 494e 5345  ..).        INSE
+000072e0: 5254 2049 4e54 4f20 736f 6d65 5f6f 7468  RT INTO some_oth
+000072f0: 6572 5f74 6162 6c65 2028 2e2e 2e20 5345  er_table (... SE
+00007300: 4c45 4354 202a 2046 524f 4d20 736f 6d65  LECT * FROM some
+00007310: 5f63 7465 290a 0a20 2020 2020 2020 2053  _cte)..        S
+00007320: 7563 6820 7175 6572 6965 7320 6172 6520  uch queries are 
+00007330: 6e6f 7420 7375 7070 6f72 7465 6420 6279  not supported by
+00007340: 2053 7061 6e6e 6572 2e0a 2020 2020 2020   Spanner..      
+00007350: 2020 2222 220a 2020 2020 2020 2020 7061    """.        pa
+00007360: 7373 0a0a 2020 2020 4070 7974 6573 742e  ss..    @pytest.
+00007370: 6d61 726b 2e73 6b69 7028 2244 454c 4554  mark.skip("DELET
+00007380: 4520 6672 6f6d 2057 4954 4820 7375 6271  E from WITH subq
+00007390: 7565 7279 2069 7320 6e6f 7420 7375 7070  uery is not supp
+000073a0: 6f72 7465 6422 290a 2020 2020 6465 6620  orted").    def 
+000073b0: 7465 7374 5f64 656c 6574 655f 7363 616c  test_delete_scal
+000073c0: 6172 5f73 7562 715f 726f 756e 645f 7472  ar_subq_round_tr
+000073d0: 6970 2873 656c 6629 3a0a 2020 2020 2020  ip(self):.      
+000073e0: 2020 2222 220a 2020 2020 2020 2020 5468    """.        Th
+000073f0: 6520 7465 7374 2063 6865 636b 7320 6966  e test checks if
+00007400: 2061 2044 454c 4554 4520 6361 6e20 6265   a DELETE can be
+00007410: 2064 6f6e 6520 6672 6f6d 2061 2063 7465   done from a cte
+00007420: 2c20 6c69 6b65 3a0a 0a20 2020 2020 2020  , like:..       
+00007430: 2057 4954 4820 736f 6d65 5f63 7465 2041   WITH some_cte A
+00007440: 5320 282e 2e2e 290a 2020 2020 2020 2020  S (...).        
+00007450: 4445 4c45 5445 2046 524f 4d20 736f 6d65  DELETE FROM some
+00007460: 5f6f 7468 6572 5f74 6162 6c65 2028 2e2e  _other_table (..
+00007470: 2e20 5345 4c45 4354 202a 2046 524f 4d20  . SELECT * FROM 
+00007480: 736f 6d65 5f63 7465 290a 0a20 2020 2020  some_cte)..     
+00007490: 2020 2053 7563 6820 7175 6572 6965 7320     Such queries 
+000074a0: 6172 6520 6e6f 7420 7375 7070 6f72 7465  are not supporte
+000074b0: 6420 6279 2053 7061 6e6e 6572 2e0a 2020  d by Spanner..  
+000074c0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000074d0: 2020 7061 7373 0a0a 2020 2020 4070 7974    pass..    @pyt
+000074e0: 6573 742e 6d61 726b 2e73 6b69 7028 2244  est.mark.skip("D
+000074f0: 454c 4554 4520 6672 6f6d 2057 4954 4820  ELETE from WITH 
+00007500: 7375 6271 7565 7279 2069 7320 6e6f 7420  subquery is not 
+00007510: 7375 7070 6f72 7465 6422 290a 2020 2020  supported").    
+00007520: 6465 6620 7465 7374 5f64 656c 6574 655f  def test_delete_
+00007530: 6672 6f6d 5f72 6f75 6e64 5f74 7269 7028  from_round_trip(
+00007540: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00007550: 2222 0a20 2020 2020 2020 2054 6865 2074  "".        The t
+00007560: 6573 7420 6368 6563 6b73 2069 6620 6120  est checks if a 
+00007570: 4445 4c45 5445 2063 616e 2062 6520 646f  DELETE can be do
+00007580: 6e65 2066 726f 6d20 6120 6374 652c 206c  ne from a cte, l
+00007590: 696b 653a 0a0a 2020 2020 2020 2020 5749  ike:..        WI
+000075a0: 5448 2073 6f6d 655f 6374 6520 4153 2028  TH some_cte AS (
+000075b0: 2e2e 2e29 0a20 2020 2020 2020 2044 454c  ...).        DEL
+000075c0: 4554 4520 4652 4f4d 2073 6f6d 655f 6f74  ETE FROM some_ot
+000075d0: 6865 725f 7461 626c 6520 282e 2e2e 2053  her_table (... S
+000075e0: 454c 4543 5420 2a20 4652 4f4d 2073 6f6d  ELECT * FROM som
+000075f0: 655f 6374 6529 0a0a 2020 2020 2020 2020  e_cte)..        
+00007600: 5375 6368 2071 7565 7269 6573 2061 7265  Such queries are
+00007610: 206e 6f74 2073 7570 706f 7274 6564 2062   not supported b
+00007620: 7920 5370 616e 6e65 722e 0a20 2020 2020  y Spanner..     
+00007630: 2020 2022 2222 0a20 2020 2020 2020 2070     """.        p
+00007640: 6173 730a 0a20 2020 2040 7079 7465 7374  ass..    @pytest
+00007650: 2e6d 6172 6b2e 736b 6970 2822 5550 4441  .mark.skip("UPDA
+00007660: 5445 2066 726f 6d20 5749 5448 2073 7562  TE from WITH sub
+00007670: 7175 6572 7920 6973 206e 6f74 2073 7570  query is not sup
+00007680: 706f 7274 6564 2229 0a20 2020 2064 6566  ported").    def
+00007690: 2074 6573 745f 7570 6461 7465 5f66 726f   test_update_fro
+000076a0: 6d5f 726f 756e 645f 7472 6970 2873 656c  m_round_trip(sel
+000076b0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+000076c0: 2020 2020 2020 2020 5468 6520 7465 7374          The test
+000076d0: 2063 6865 636b 7320 6966 2061 6e20 5550   checks if an UP
+000076e0: 4441 5445 2063 616e 2062 6520 646f 6e65  DATE can be done
+000076f0: 2066 726f 6d20 6120 6374 652c 206c 696b   from a cte, lik
+00007700: 653a 0a0a 2020 2020 2020 2020 5749 5448  e:..        WITH
+00007710: 2073 6f6d 655f 6374 6520 4153 2028 2e2e   some_cte AS (..
+00007720: 2e29 0a20 2020 2020 2020 2055 5044 4154  .).        UPDAT
+00007730: 4520 736f 6d65 5f6f 7468 6572 5f74 6162  E some_other_tab
+00007740: 6c65 0a20 2020 2020 2020 2053 4554 2028  le.        SET (
+00007750: 2e2e 2e20 5345 4c45 4354 202a 2046 524f  ... SELECT * FRO
+00007760: 4d20 736f 6d65 5f63 7465 290a 0a20 2020  M some_cte)..   
+00007770: 2020 2020 2053 7563 6820 7175 6572 6965       Such querie
+00007780: 7320 6172 6520 6e6f 7420 7375 7070 6f72  s are not suppor
+00007790: 7465 6420 6279 2053 7061 6e6e 6572 2e0a  ted by Spanner..
+000077a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000077b0: 2020 2020 7061 7373 0a0a 2020 2020 4070      pass..    @p
+000077c0: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
+000077d0: 2257 4954 4820 5245 4355 5253 4956 4520  "WITH RECURSIVE 
+000077e0: 7375 6271 7565 7269 6573 2061 7265 206e  subqueries are n
+000077f0: 6f74 2073 7570 706f 7274 6564 2229 0a20  ot supported"). 
+00007800: 2020 2064 6566 2074 6573 745f 7365 6c65     def test_sele
+00007810: 6374 5f72 6563 7572 7369 7665 5f72 6f75  ct_recursive_rou
+00007820: 6e64 5f74 7269 7028 7365 6c66 293a 0a20  nd_trip(self):. 
+00007830: 2020 2020 2020 2070 6173 730a 0a0a 636c         pass...cl
+00007840: 6173 7320 4461 7465 5469 6d65 4d69 6372  ass DateTimeMicr
+00007850: 6f73 6563 6f6e 6473 5465 7374 285f 4461  osecondsTest(_Da
+00007860: 7465 5469 6d65 4d69 6372 6f73 6563 6f6e  teTimeMicrosecon
+00007870: 6473 5465 7374 2c20 4461 7465 5465 7374  dsTest, DateTest
+00007880: 293a 0a20 2020 2040 7079 7465 7374 2e6d  ):.    @pytest.m
+00007890: 6172 6b2e 736b 6970 2822 5370 616e 6e65  ark.skip("Spanne
+000078a0: 7220 6461 7465 7320 6172 6520 7469 6d65  r dates are time
+000078b0: 207a 6f6e 6520 696e 6465 7065 6e64 656e   zone independen
+000078c0: 7422 290a 2020 2020 6465 6620 7465 7374  t").    def test
+000078d0: 5f73 656c 6563 745f 6469 7265 6374 2873  _select_direct(s
+000078e0: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+000078f0: 7373 0a0a 2020 2020 6465 6620 7465 7374  ss..    def test
+00007900: 5f72 6f75 6e64 5f74 7269 7028 7365 6c66  _round_trip(self
+00007910: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00007920: 2020 2020 2020 2053 5041 4e4e 4552 204f         SPANNER O
+00007930: 5645 5252 4944 453a 0a0a 2020 2020 2020  VERRIDE:..      
+00007940: 2020 5370 616e 6e65 7220 636f 6e76 6572    Spanner conver
+00007950: 7473 2074 696d 6573 7461 6d70 2069 6e74  ts timestamp int
+00007960: 6f20 6025 592d 256d 2d25 6454 2548 3a25  o `%Y-%m-%dT%H:%
+00007970: 4d3a 2553 2e25 665a 6020 666f 726d 6174  M:%S.%fZ` format
+00007980: 2c20 736f 2074 6f20 6176 6f69 640a 2020  , so to avoid.  
+00007990: 2020 2020 2020 6173 7365 7274 2066 6169        assert fai
+000079a0: 6c75 7265 7320 636f 6e76 6572 7420 6461  lures convert da
+000079b0: 7465 7469 6d65 2069 6e70 7574 2074 6f20  tetime input to 
+000079c0: 7468 6520 6465 7369 7265 2074 696d 6573  the desire times
+000079d0: 7461 6d70 2066 6f72 6d61 742e 0a20 2020  tamp format..   
+000079e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000079f0: 2064 6174 655f 7461 626c 6520 3d20 7365   date_table = se
+00007a00: 6c66 2e74 6162 6c65 732e 6461 7465 5f74  lf.tables.date_t
+00007a10: 6162 6c65 0a20 2020 2020 2020 2063 6f6e  able.        con
+00007a20: 6669 672e 6462 2e65 7865 6375 7465 2864  fig.db.execute(d
+00007a30: 6174 655f 7461 626c 652e 696e 7365 7274  ate_table.insert
+00007a40: 2829 2c20 7b22 6461 7465 5f64 6174 6122  (), {"date_data"
+00007a50: 3a20 7365 6c66 2e64 6174 612c 2022 6964  : self.data, "id
+00007a60: 223a 2032 3530 7d29 0a0a 2020 2020 2020  ": 250})..      
+00007a70: 2020 726f 7720 3d20 636f 6e66 6967 2e64    row = config.d
+00007a80: 622e 6578 6563 7574 6528 7365 6c65 6374  b.execute(select
+00007a90: 285b 6461 7465 5f74 6162 6c65 2e63 2e64  ([date_table.c.d
+00007aa0: 6174 655f 6461 7461 5d29 292e 6669 7273  ate_data])).firs
+00007ab0: 7428 290a 2020 2020 2020 2020 636f 6d70  t().        comp
+00007ac0: 6172 6520 3d20 7365 6c66 2e63 6f6d 7061  are = self.compa
+00007ad0: 7265 206f 7220 7365 6c66 2e64 6174 610a  re or self.data.
+00007ae0: 2020 2020 2020 2020 636f 6d70 6172 6520          compare 
+00007af0: 3d20 636f 6d70 6172 652e 7374 7266 7469  = compare.strfti
+00007b00: 6d65 2822 2559 2d25 6d2d 2564 5425 483a  me("%Y-%m-%dT%H:
+00007b10: 254d 3a25 532e 2566 5a22 290a 2020 2020  %M:%S.%fZ").    
+00007b20: 2020 2020 6571 5f28 726f 775b 305d 2e72      eq_(row[0].r
+00007b30: 6663 3333 3339 2829 2c20 636f 6d70 6172  fc3339(), compar
+00007b40: 6529 0a20 2020 2020 2020 2061 7373 6572  e).        asser
+00007b50: 7420 6973 696e 7374 616e 6365 2872 6f77  t isinstance(row
+00007b60: 5b30 5d2c 2044 6174 6574 696d 6557 6974  [0], DatetimeWit
+00007b70: 684e 616e 6f73 6563 6f6e 6473 290a 0a20  hNanoseconds).. 
+00007b80: 2020 2064 6566 2074 6573 745f 726f 756e     def test_roun
+00007b90: 645f 7472 6970 5f64 6563 6f72 6174 6564  d_trip_decorated
+00007ba0: 2873 656c 662c 2063 6f6e 6e65 6374 696f  (self, connectio
+00007bb0: 6e29 3a0a 2020 2020 2020 2020 2222 220a  n):.        """.
+00007bc0: 2020 2020 2020 2020 5350 414e 4e45 5220          SPANNER 
+00007bd0: 4f56 4552 5249 4445 3a0a 0a20 2020 2020  OVERRIDE:..     
+00007be0: 2020 2053 7061 6e6e 6572 2063 6f6e 7665     Spanner conve
+00007bf0: 7274 7320 7469 6d65 7374 616d 7020 696e  rts timestamp in
+00007c00: 746f 2060 2559 2d25 6d2d 2564 5425 483a  to `%Y-%m-%dT%H:
+00007c10: 254d 3a25 532e 2566 5a60 2066 6f72 6d61  %M:%S.%fZ` forma
+00007c20: 742c 2073 6f20 746f 2061 766f 6964 0a20  t, so to avoid. 
+00007c30: 2020 2020 2020 2061 7373 6572 7420 6661         assert fa
+00007c40: 696c 7572 6573 2063 6f6e 7665 7274 2064  ilures convert d
+00007c50: 6174 6574 696d 6520 696e 7075 7420 746f  atetime input to
+00007c60: 2074 6865 2064 6573 6972 6520 7469 6d65   the desire time
+00007c70: 7374 616d 7020 666f 726d 6174 2e0a 2020  stamp format..  
+00007c80: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00007c90: 2020 6461 7465 5f74 6162 6c65 203d 2073    date_table = s
+00007ca0: 656c 662e 7461 626c 6573 2e64 6174 655f  elf.tables.date_
+00007cb0: 7461 626c 650a 0a20 2020 2020 2020 2063  table..        c
+00007cc0: 6f6e 6e65 6374 696f 6e2e 6578 6563 7574  onnection.execut
+00007cd0: 6528 0a20 2020 2020 2020 2020 2020 2064  e(.            d
+00007ce0: 6174 655f 7461 626c 652e 696e 7365 7274  ate_table.insert
+00007cf0: 2829 2c20 7b22 6964 223a 2031 2c20 2264  (), {"id": 1, "d
+00007d00: 6563 6f72 6174 6564 5f64 6174 655f 6461  ecorated_date_da
+00007d10: 7461 223a 2073 656c 662e 6461 7461 7d0a  ta": self.data}.
+00007d20: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00007d30: 2020 2072 6f77 203d 2063 6f6e 6e65 6374     row = connect
+00007d40: 696f 6e2e 6578 6563 7574 6528 7365 6c65  ion.execute(sele
+00007d50: 6374 2864 6174 655f 7461 626c 652e 632e  ct(date_table.c.
+00007d60: 6465 636f 7261 7465 645f 6461 7465 5f64  decorated_date_d
+00007d70: 6174 6129 292e 6669 7273 7428 290a 0a20  ata)).first().. 
+00007d80: 2020 2020 2020 2063 6f6d 7061 7265 203d         compare =
+00007d90: 2073 656c 662e 636f 6d70 6172 6520 6f72   self.compare or
+00007da0: 2073 656c 662e 6461 7461 0a20 2020 2020   self.data.     
+00007db0: 2020 2063 6f6d 7061 7265 203d 2063 6f6d     compare = com
+00007dc0: 7061 7265 2e73 7472 6674 696d 6528 2225  pare.strftime("%
+00007dd0: 592d 256d 2d25 6454 2548 3a25 4d3a 2553  Y-%m-%dT%H:%M:%S
+00007de0: 2e25 665a 2229 0a20 2020 2020 2020 2065  .%fZ").        e
+00007df0: 715f 2872 6f77 5b30 5d2e 7266 6333 3333  q_(row[0].rfc333
+00007e00: 3928 292c 2063 6f6d 7061 7265 290a 2020  9(), compare).  
+00007e10: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
+00007e20: 6e73 7461 6e63 6528 726f 775b 305d 2c20  nstance(row[0], 
+00007e30: 4461 7465 7469 6d65 5769 7468 4e61 6e6f  DatetimeWithNano
+00007e40: 7365 636f 6e64 7329 0a0a 2020 2020 4070  seconds)..    @p
+00007e50: 7974 6573 742e 6d61 726b 2e73 6b69 7069  ytest.mark.skipi
+00007e60: 6628 0a20 2020 2020 2020 2062 6f6f 6c28  f(.        bool(
+00007e70: 6f73 2e65 6e76 6972 6f6e 2e67 6574 2822  os.environ.get("
+00007e80: 5350 414e 4e45 525f 454d 554c 4154 4f52  SPANNER_EMULATOR
+00007e90: 5f48 4f53 5422 2929 2c20 7265 6173 6f6e  _HOST")), reason
+00007ea0: 3d22 536b 6970 7065 6420 6f6e 2065 6d75  ="Skipped on emu
+00007eb0: 6c61 746f 7222 0a20 2020 2029 0a20 2020  lator".    ).   
+00007ec0: 2064 6566 2074 6573 745f 6e75 6c6c 5f62   def test_null_b
+00007ed0: 6f75 6e64 5f63 6f6d 7061 7269 736f 6e28  ound_comparison(
+00007ee0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+00007ef0: 7570 6572 2829 2e74 6573 745f 6e75 6c6c  uper().test_null
+00007f00: 5f62 6f75 6e64 5f63 6f6d 7061 7269 736f  _bound_compariso
+00007f10: 6e28 290a 0a20 2020 2040 7079 7465 7374  n()..    @pytest
+00007f20: 2e6d 6172 6b2e 736b 6970 6966 280a 2020  .mark.skipif(.  
+00007f30: 2020 2020 2020 626f 6f6c 286f 732e 656e        bool(os.en
+00007f40: 7669 726f 6e2e 6765 7428 2253 5041 4e4e  viron.get("SPANN
+00007f50: 4552 5f45 4d55 4c41 544f 525f 484f 5354  ER_EMULATOR_HOST
+00007f60: 2229 292c 2072 6561 736f 6e3d 2253 6b69  ")), reason="Ski
+00007f70: 7070 6564 206f 6e20 656d 756c 6174 6f72  pped on emulator
+00007f80: 220a 2020 2020 290a 2020 2020 6465 6620  ".    ).    def 
+00007f90: 7465 7374 5f6e 756c 6c28 7365 6c66 2c20  test_null(self, 
+00007fa0: 636f 6e6e 6563 7469 6f6e 293a 0a20 2020  connection):.   
+00007fb0: 2020 2020 2073 7570 6572 2829 2e74 6573       super().tes
+00007fc0: 745f 6e75 6c6c 2863 6f6e 6e65 6374 696f  t_null(connectio
+00007fd0: 6e29 0a0a 0a63 6c61 7373 2044 6174 6554  n)...class DateT
+00007fe0: 696d 6554 6573 7428 5f44 6174 6554 696d  imeTest(_DateTim
+00007ff0: 6554 6573 742c 2044 6174 6554 696d 654d  eTest, DateTimeM
+00008000: 6963 726f 7365 636f 6e64 7354 6573 7429  icrosecondsTest)
+00008010: 3a0a 2020 2020 2222 220a 2020 2020 5350  :.    """.    SP
+00008020: 414e 4e45 5220 4f56 4552 5249 4445 3a0a  ANNER OVERRIDE:.
+00008030: 0a20 2020 2044 6174 6554 696d 6554 6573  .    DateTimeTes
+00008040: 7420 7465 7374 7320 6861 7665 2074 6865  t tests have the
+00008050: 2073 616d 6520 6661 696c 7572 6573 2073   same failures s
+00008060: 616d 6520 6173 2044 6174 6554 696d 654d  ame as DateTimeM
+00008070: 6963 726f 7365 636f 6e64 7354 6573 7420  icrosecondsTest 
+00008080: 7465 7374 732c 0a20 2020 2073 6f20 746f  tests,.    so to
+00008090: 2061 766f 6964 2074 686f 7365 2066 6169   avoid those fai
+000080a0: 6c75 7265 7320 616e 6420 6d61 696e 7461  lures and mainta
+000080b0: 696e 2044 5259 2063 6f6e 6365 7074 206a  in DRY concept j
+000080c0: 7573 7420 696e 6865 7269 7420 7468 6520  ust inherit the 
+000080d0: 636c 6173 7320 746f 2072 756e 0a20 2020  class to run.   
+000080e0: 2074 6573 7473 2073 7563 6365 7373 6675   tests successfu
+000080f0: 6c6c 792e 0a20 2020 2022 2222 0a0a 2020  lly..    """..  
+00008100: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
+00008110: 6b69 7069 6628 0a20 2020 2020 2020 2062  kipif(.        b
+00008120: 6f6f 6c28 6f73 2e65 6e76 6972 6f6e 2e67  ool(os.environ.g
+00008130: 6574 2822 5350 414e 4e45 525f 454d 554c  et("SPANNER_EMUL
+00008140: 4154 4f52 5f48 4f53 5422 2929 2c20 7265  ATOR_HOST")), re
+00008150: 6173 6f6e 3d22 536b 6970 7065 6420 6f6e  ason="Skipped on
+00008160: 2065 6d75 6c61 746f 7222 0a20 2020 2029   emulator".    )
+00008170: 0a20 2020 2064 6566 2074 6573 745f 6e75  .    def test_nu
+00008180: 6c6c 5f62 6f75 6e64 5f63 6f6d 7061 7269  ll_bound_compari
+00008190: 736f 6e28 7365 6c66 293a 0a20 2020 2020  son(self):.     
+000081a0: 2020 2073 7570 6572 2829 2e74 6573 745f     super().test_
+000081b0: 6e75 6c6c 5f62 6f75 6e64 5f63 6f6d 7061  null_bound_compa
+000081c0: 7269 736f 6e28 290a 0a20 2020 2040 7079  rison()..    @py
+000081d0: 7465 7374 2e6d 6172 6b2e 736b 6970 6966  test.mark.skipif
+000081e0: 280a 2020 2020 2020 2020 626f 6f6c 286f  (.        bool(o
+000081f0: 732e 656e 7669 726f 6e2e 6765 7428 2253  s.environ.get("S
+00008200: 5041 4e4e 4552 5f45 4d55 4c41 544f 525f  PANNER_EMULATOR_
+00008210: 484f 5354 2229 292c 2072 6561 736f 6e3d  HOST")), reason=
+00008220: 2253 6b69 7070 6564 206f 6e20 656d 756c  "Skipped on emul
+00008230: 6174 6f72 220a 2020 2020 290a 2020 2020  ator".    ).    
+00008240: 6465 6620 7465 7374 5f6e 756c 6c28 7365  def test_null(se
+00008250: 6c66 2c20 636f 6e6e 6563 7469 6f6e 293a  lf, connection):
+00008260: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+00008270: 2e74 6573 745f 6e75 6c6c 2863 6f6e 6e65  .test_null(conne
+00008280: 6374 696f 6e29 0a0a 2020 2020 4070 7974  ction)..    @pyt
+00008290: 6573 742e 6d61 726b 2e73 6b69 7028 2253  est.mark.skip("S
+000082a0: 7061 6e6e 6572 2064 6174 6573 2061 7265  panner dates are
+000082b0: 2074 696d 6520 7a6f 6e65 2069 6e64 6570   time zone indep
+000082c0: 656e 6465 6e74 2229 0a20 2020 2064 6566  endent").    def
+000082d0: 2074 6573 745f 7365 6c65 6374 5f64 6972   test_select_dir
+000082e0: 6563 7428 7365 6c66 293a 0a20 2020 2020  ect(self):.     
+000082f0: 2020 2070 6173 730a 0a0a 4070 7974 6573     pass...@pytes
+00008300: 742e 6d61 726b 2e73 6b69 7028 224e 6f74  t.mark.skip("Not
+00008310: 2073 7570 706f 7274 6564 2062 7920 5370   supported by Sp
+00008320: 616e 6e65 7222 290a 636c 6173 7320 4469  anner").class Di
+00008330: 6666 6963 756c 7450 6172 616d 6574 6572  fficultParameter
+00008340: 7354 6573 7428 5f44 6966 6669 6375 6c74  sTest(_Difficult
+00008350: 5061 7261 6d65 7465 7273 5465 7374 293a  ParametersTest):
+00008360: 0a20 2020 2070 6173 730a 0a0a 636c 6173  .    pass...clas
+00008370: 7320 4665 7463 684c 696d 6974 4f66 6673  s FetchLimitOffs
+00008380: 6574 5465 7374 285f 4665 7463 684c 696d  etTest(_FetchLim
+00008390: 6974 4f66 6673 6574 5465 7374 293a 0a20  itOffsetTest):. 
+000083a0: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
+000083b0: 736b 6970 2822 5370 616e 6e65 7220 646f  skip("Spanner do
+000083c0: 6573 6e27 7420 7375 7070 6f72 7420 636f  esn't support co
+000083d0: 6d70 6f73 6974 6520 4c49 4d49 5420 616e  mposite LIMIT an
+000083e0: 6420 4f46 4653 4554 2063 6c61 7573 6573  d OFFSET clauses
+000083f0: 2229 0a20 2020 2064 6566 2074 6573 745f  ").    def test_
+00008400: 6578 7072 5f6c 696d 6974 2873 656c 662c  expr_limit(self,
+00008410: 2063 6f6e 6e65 6374 696f 6e29 3a0a 2020   connection):.  
+00008420: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00008430: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+00008440: 7028 2253 7061 6e6e 6572 2064 6f65 736e  p("Spanner doesn
+00008450: 2774 2073 7570 706f 7274 2063 6f6d 706f  't support compo
+00008460: 7369 7465 204c 494d 4954 2061 6e64 204f  site LIMIT and O
+00008470: 4646 5345 5420 636c 6175 7365 7322 290a  FFSET clauses").
+00008480: 2020 2020 6465 6620 7465 7374 5f65 7870      def test_exp
+00008490: 725f 6f66 6673 6574 2873 656c 662c 2063  r_offset(self, c
+000084a0: 6f6e 6e65 6374 696f 6e29 3a0a 2020 2020  onnection):.    
+000084b0: 2020 2020 7061 7373 0a0a 2020 2020 4070      pass..    @p
+000084c0: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
+000084d0: 2253 7061 6e6e 6572 2064 6f65 736e 2774  "Spanner doesn't
+000084e0: 2073 7570 706f 7274 2063 6f6d 706f 7369   support composi
+000084f0: 7465 204c 494d 4954 2061 6e64 204f 4646  te LIMIT and OFF
+00008500: 5345 5420 636c 6175 7365 7322 290a 2020  SET clauses").  
+00008510: 2020 6465 6620 7465 7374 5f65 7870 725f    def test_expr_
+00008520: 6c69 6d69 745f 6f66 6673 6574 2873 656c  limit_offset(sel
+00008530: 662c 2063 6f6e 6e65 6374 696f 6e29 3a0a  f, connection):.
+00008540: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00008550: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
+00008560: 6b69 7028 2253 7061 6e6e 6572 2064 6f65  kip("Spanner doe
+00008570: 736e 2774 2073 7570 706f 7274 2063 6f6d  sn't support com
+00008580: 706f 7369 7465 204c 494d 4954 2061 6e64  posite LIMIT and
+00008590: 204f 4646 5345 5420 636c 6175 7365 7322   OFFSET clauses"
+000085a0: 290a 2020 2020 6465 6620 7465 7374 5f65  ).    def test_e
+000085b0: 7870 725f 6c69 6d69 745f 7369 6d70 6c65  xpr_limit_simple
+000085c0: 5f6f 6666 7365 7428 7365 6c66 2c20 636f  _offset(self, co
+000085d0: 6e6e 6563 7469 6f6e 293a 0a20 2020 2020  nnection):.     
+000085e0: 2020 2070 6173 730a 0a20 2020 2040 7079     pass..    @py
+000085f0: 7465 7374 2e6d 6172 6b2e 736b 6970 2822  test.mark.skip("
+00008600: 5370 616e 6e65 7220 646f 6573 6e27 7420  Spanner doesn't 
+00008610: 7375 7070 6f72 7420 636f 6d70 6f73 6974  support composit
+00008620: 6520 4c49 4d49 5420 616e 6420 4f46 4653  e LIMIT and OFFS
+00008630: 4554 2063 6c61 7573 6573 2229 0a20 2020  ET clauses").   
+00008640: 2064 6566 2074 6573 745f 7369 6d70 6c65   def test_simple
+00008650: 5f6c 696d 6974 5f65 7870 725f 6f66 6673  _limit_expr_offs
+00008660: 6574 2873 656c 662c 2063 6f6e 6e65 6374  et(self, connect
+00008670: 696f 6e29 3a0a 2020 2020 2020 2020 7061  ion):.        pa
+00008680: 7373 0a0a 2020 2020 4070 7974 6573 742e  ss..    @pytest.
+00008690: 6d61 726b 2e73 6b69 7028 2253 7061 6e6e  mark.skip("Spann
+000086a0: 6572 2064 6f65 736e 2774 2073 7570 706f  er doesn't suppo
+000086b0: 7274 2063 6f6d 706f 7369 7465 204c 494d  rt composite LIM
+000086c0: 4954 2061 6e64 204f 4646 5345 5420 636c  IT and OFFSET cl
+000086d0: 6175 7365 7322 290a 2020 2020 6465 6620  auses").    def 
+000086e0: 7465 7374 5f62 6f75 6e64 5f6f 6666 7365  test_bound_offse
+000086f0: 7428 7365 6c66 2c20 636f 6e6e 6563 7469  t(self, connecti
+00008700: 6f6e 293a 0a20 2020 2020 2020 2070 6173  on):.        pas
+00008710: 730a 0a20 2020 2064 6566 2074 6573 745f  s..    def test_
+00008720: 6c69 6d69 745f 7265 6e64 6572 5f6d 756c  limit_render_mul
+00008730: 7469 706c 655f 7469 6d65 7328 7365 6c66  tiple_times(self
+00008740: 2c20 636f 6e6e 6563 7469 6f6e 293a 0a20  , connection):. 
+00008750: 2020 2020 2020 2074 6162 6c65 203d 2073         table = s
+00008760: 656c 662e 7461 626c 6573 2e73 6f6d 655f  elf.tables.some_
+00008770: 7461 626c 650a 2020 2020 2020 2020 7374  table.        st
+00008780: 6d74 203d 2073 656c 6563 7428 7461 626c  mt = select(tabl
+00008790: 652e 632e 6964 292e 6c69 6d69 7428 3129  e.c.id).limit(1)
+000087a0: 2e73 6361 6c61 725f 7375 6271 7565 7279  .scalar_subquery
+000087b0: 2829 0a0a 2020 2020 2020 2020 7520 3d20  ()..        u = 
+000087c0: 756e 696f 6e28 7365 6c65 6374 2873 746d  union(select(stm
+000087d0: 7429 2c20 7365 6c65 6374 2873 746d 7429  t), select(stmt)
+000087e0: 292e 7375 6271 7565 7279 2829 2e73 656c  ).subquery().sel
+000087f0: 6563 7428 290a 0a20 2020 2020 2020 2073  ect()..        s
+00008800: 656c 662e 5f61 7373 6572 745f 7265 7375  elf._assert_resu
+00008810: 6c74 280a 2020 2020 2020 2020 2020 2020  lt(.            
+00008820: 636f 6e6e 6563 7469 6f6e 2c0a 2020 2020  connection,.    
+00008830: 2020 2020 2020 2020 752c 0a20 2020 2020          u,.     
+00008840: 2020 2020 2020 205b 2832 2c29 5d2c 0a20         [(2,)],. 
+00008850: 2020 2020 2020 2029 0a0a 0a40 7079 7465         )...@pyte
+00008860: 7374 2e6d 6172 6b2e 736b 6970 2822 5370  st.mark.skip("Sp
+00008870: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
+00008880: 7070 6f72 7420 6175 746f 696e 6372 656d  pport autoincrem
+00008890: 656e 7422 290a 636c 6173 7320 4964 656e  ent").class Iden
+000088a0: 7469 7479 4175 746f 696e 6372 656d 656e  tityAutoincremen
+000088b0: 7454 6573 7428 5f49 6465 6e74 6974 7941  tTest(_IdentityA
+000088c0: 7574 6f69 6e63 7265 6d65 6e74 5465 7374  utoincrementTest
+000088d0: 293a 0a20 2020 2070 6173 730a 0a0a 636c  ):.    pass...cl
+000088e0: 6173 7320 4573 6361 7069 6e67 5465 7374  ass EscapingTest
+000088f0: 285f 4573 6361 7069 6e67 5465 7374 293a  (_EscapingTest):
+00008900: 0a20 2020 2040 7072 6f76 6964 655f 6d65  .    @provide_me
+00008910: 7461 6461 7461 0a20 2020 2064 6566 2074  tadata.    def t
+00008920: 6573 745f 7065 7263 656e 745f 7369 676e  est_percent_sign
+00008930: 5f72 6f75 6e64 5f74 7269 7028 7365 6c66  _round_trip(self
+00008940: 293a 0a20 2020 2020 2020 2022 2222 5465  ):.        """Te
+00008950: 7374 2074 6861 7420 7468 6520 4442 4150  st that the DBAP
+00008960: 4920 6163 636f 6d6d 6f64 6174 6573 2066  I accommodates f
+00008970: 6f72 2065 7363 6170 6564 202f 206e 6f6e  or escaped / non
+00008980: 6573 6361 7065 640a 2020 2020 2020 2020  escaped.        
+00008990: 7065 7263 656e 7420 7369 676e 7320 696e  percent signs in
+000089a0: 2061 2077 6179 2074 6861 7420 6d61 7463   a way that matc
+000089b0: 6865 7320 7468 6520 636f 6d70 696c 6572  hes the compiler
+000089c0: 0a0a 2020 2020 2020 2020 5350 414e 4e45  ..        SPANNE
+000089d0: 5220 4f56 4552 5249 4445 0a20 2020 2020  R OVERRIDE.     
+000089e0: 2020 2043 6c6f 7564 2053 7061 6e6e 6572     Cloud Spanner
+000089f0: 2073 7570 706f 7274 7320 7461 626c 6573   supports tables
+00008a00: 2077 6974 6820 656d 7074 7920 7072 696d   with empty prim
+00008a10: 6172 7920 6b65 792c 2062 7574 0a20 2020  ary key, but.   
+00008a20: 2020 2020 206f 6e6c 7920 7369 6e67 6c65       only single
+00008a30: 206f 6e65 2072 6f77 2063 616e 2062 6520   one row can be 
+00008a40: 696e 7365 7274 6564 2069 6e74 6f20 7375  inserted into su
+00008a50: 6368 2061 2074 6162 6c65 202d 0a20 2020  ch a table -.   
+00008a60: 2020 2020 2066 6f6c 6c6f 7769 6e67 2069       following i
+00008a70: 6e73 6572 7469 6f6e 7320 7769 6c6c 2066  nsertions will f
+00008a80: 6169 6c20 7769 7468 2060 526f 7720 5b5d  ail with `Row []
+00008a90: 2061 6c72 6561 6479 2065 7869 7374 7322   already exists"
+00008aa0: 2e0a 2020 2020 2020 2020 4f76 6572 7269  ..        Overri
+00008ab0: 6469 6e67 2074 6865 2074 6573 7420 746f  ding the test to
+00008ac0: 2061 766f 6964 2074 6865 2073 616d 6520   avoid the same 
+00008ad0: 6661 696c 7572 652e 0a20 2020 2020 2020  failure..       
+00008ae0: 2022 2222 0a20 2020 2020 2020 206d 203d   """.        m =
+00008af0: 2073 656c 662e 6d65 7461 6461 7461 0a20   self.metadata. 
+00008b00: 2020 2020 2020 2074 203d 2054 6162 6c65         t = Table
+00008b10: 2822 7422 2c20 6d2c 2043 6f6c 756d 6e28  ("t", m, Column(
+00008b20: 2264 6174 6122 2c20 5374 7269 6e67 2835  "data", String(5
+00008b30: 3029 2929 0a20 2020 2020 2020 2074 2e63  0))).        t.c
+00008b40: 7265 6174 6528 636f 6e66 6967 2e64 6229  reate(config.db)
+00008b50: 0a20 2020 2020 2020 2077 6974 6820 636f  .        with co
+00008b60: 6e66 6967 2e64 622e 6265 6769 6e28 2920  nfig.db.begin() 
+00008b70: 6173 2063 6f6e 6e3a 0a20 2020 2020 2020  as conn:.       
+00008b80: 2020 2020 2063 6f6e 6e2e 6578 6563 7574       conn.execut
+00008b90: 6528 742e 696e 7365 7274 2829 2c20 6469  e(t.insert(), di
+00008ba0: 6374 2864 6174 613d 2273 6f6d 6520 2520  ct(data="some % 
+00008bb0: 7661 6c75 6522 2929 0a0a 2020 2020 2020  value"))..      
+00008bc0: 2020 2020 2020 6571 5f28 0a20 2020 2020        eq_(.     
+00008bd0: 2020 2020 2020 2020 2020 2063 6f6e 6e2e             conn.
+00008be0: 7363 616c 6172 280a 2020 2020 2020 2020  scalar(.        
+00008bf0: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
+00008c00: 6374 285b 742e 632e 6461 7461 5d29 2e77  ct([t.c.data]).w
+00008c10: 6865 7265 280a 2020 2020 2020 2020 2020  here(.          
+00008c20: 2020 2020 2020 2020 2020 2020 2020 742e                t.
+00008c30: 632e 6461 7461 203d 3d20 6c69 7465 7261  c.data == litera
+00008c40: 6c5f 636f 6c75 6d6e 2822 2773 6f6d 6520  l_column("'some 
+00008c50: 2520 7661 6c75 6527 2229 0a20 2020 2020  % value'").     
+00008c60: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00008c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008c80: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00008c90: 2020 2020 2273 6f6d 6520 2520 7661 6c75      "some % valu
+00008ca0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00008cb0: 290a 0a20 2020 2020 2020 2020 2020 2063  )..            c
+00008cc0: 6f6e 6e2e 6578 6563 7574 6528 742e 6465  onn.execute(t.de
+00008cd0: 6c65 7465 2829 290a 2020 2020 2020 2020  lete()).        
+00008ce0: 2020 2020 636f 6e6e 2e65 7865 6375 7465      conn.execute
+00008cf0: 2874 2e69 6e73 6572 7428 292c 2064 6963  (t.insert(), dic
+00008d00: 7428 6461 7461 3d22 736f 6d65 2025 2520  t(data="some %% 
+00008d10: 6f74 6865 7220 7661 6c75 6522 2929 0a20  other value")). 
+00008d20: 2020 2020 2020 2020 2020 2065 715f 280a             eq_(.
+00008d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d40: 636f 6e6e 2e73 6361 6c61 7228 0a20 2020  conn.scalar(.   
+00008d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d60: 2073 656c 6563 7428 5b74 2e63 2e64 6174   select([t.c.dat
+00008d70: 615d 292e 7768 6572 6528 0a20 2020 2020  a]).where(.     
+00008d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d90: 2020 2074 2e63 2e64 6174 6120 3d3d 206c     t.c.data == l
+00008da0: 6974 6572 616c 5f63 6f6c 756d 6e28 2227  iteral_column("'
+00008db0: 736f 6d65 2025 2520 6f74 6865 7220 7661  some %% other va
+00008dc0: 6c75 6527 2229 0a20 2020 2020 2020 2020  lue'").         
+00008dd0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00008de0: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
+00008df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e00: 2273 6f6d 6520 2525 206f 7468 6572 2076  "some %% other v
+00008e10: 616c 7565 222c 0a20 2020 2020 2020 2020  alue",.         
+00008e20: 2020 2029 0a0a 0a63 6c61 7373 2045 7869     )...class Exi
+00008e30: 7374 7354 6573 7428 5f45 7869 7374 7354  stsTest(_ExistsT
+00008e40: 6573 7429 3a0a 2020 2020 6465 6620 7465  est):.    def te
+00008e50: 7374 5f73 656c 6563 745f 6578 6973 7473  st_select_exists
+00008e60: 2873 656c 662c 2063 6f6e 6e65 6374 696f  (self, connectio
+00008e70: 6e29 3a0a 2020 2020 2020 2020 2222 220a  n):.        """.
+00008e80: 2020 2020 2020 2020 5350 414e 4e45 5220          SPANNER 
+00008e90: 4f56 4552 5249 4445 3a0a 0a20 2020 2020  OVERRIDE:..     
+00008ea0: 2020 2054 6865 206f 7269 6769 6e61 6c20     The original 
+00008eb0: 7465 7374 2069 7320 7472 7969 6e67 2074  test is trying t
+00008ec0: 6f20 6578 6563 7574 6520 6120 7175 6572  o execute a quer
+00008ed0: 7920 6c69 6b65 3a0a 0a20 2020 2020 2020  y like:..       
+00008ee0: 2053 454c 4543 5420 2e2e 2e0a 2020 2020   SELECT ....    
+00008ef0: 2020 2020 5748 4552 4520 4558 4953 5453      WHERE EXISTS
+00008f00: 2028 5345 4c45 4354 202e 2e2e 290a 0a20   (SELECT ...).. 
+00008f10: 2020 2020 2020 2053 454c 4543 5420 5748         SELECT WH
+00008f20: 4552 4520 7769 7468 6f75 7420 4652 4f4d  ERE without FROM
+00008f30: 2063 6c61 7573 6520 6973 206e 6f74 2073   clause is not s
+00008f40: 7570 706f 7274 6564 2062 7920 5370 616e  upported by Span
+00008f50: 6e65 722e 0a20 2020 2020 2020 2052 6577  ner..        Rew
+00008f60: 7269 7469 6e67 2074 6865 2074 6573 7420  riting the test 
+00008f70: 746f 2066 6f72 6365 2069 7420 746f 2067  to force it to g
+00008f80: 656e 6572 6174 6520 6120 7175 6572 7920  enerate a query 
+00008f90: 6c69 6b65 3a0a 0a20 2020 2020 2020 2053  like:..        S
+00008fa0: 454c 4543 5420 4558 4953 5453 2028 5345  ELECT EXISTS (SE
+00008fb0: 4c45 4354 202e 2e2e 290a 2020 2020 2020  LECT ...).      
+00008fc0: 2020 2222 220a 2020 2020 2020 2020 7374    """.        st
+00008fd0: 7566 6620 3d20 7365 6c66 2e74 6162 6c65  uff = self.table
+00008fe0: 732e 7374 7566 660a 2020 2020 2020 2020  s.stuff.        
+00008ff0: 6571 5f28 0a20 2020 2020 2020 2020 2020  eq_(.           
+00009000: 2063 6f6e 6e65 6374 696f 6e2e 6578 6563   connection.exec
+00009010: 7574 6528 0a20 2020 2020 2020 2020 2020  ute(.           
+00009020: 2020 2020 2073 656c 6563 7428 2865 7869       select((exi
+00009030: 7374 7328 292e 7768 6572 6528 7374 7566  sts().where(stuf
+00009040: 662e 632e 6461 7461 203d 3d20 2273 6f6d  f.c.data == "som
+00009050: 6520 6461 7461 2229 2c29 290a 2020 2020  e data"),)).    
+00009060: 2020 2020 2020 2020 292e 6665 7463 6861          ).fetcha
+00009070: 6c6c 2829 2c0a 2020 2020 2020 2020 2020  ll(),.          
+00009080: 2020 5b28 5472 7565 2c29 5d2c 0a20 2020    [(True,)],.   
+00009090: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+000090a0: 7465 7374 5f73 656c 6563 745f 6578 6973  test_select_exis
+000090b0: 7473 5f66 616c 7365 2873 656c 662c 2063  ts_false(self, c
+000090c0: 6f6e 6e65 6374 696f 6e29 3a0a 2020 2020  onnection):.    
+000090d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000090e0: 5350 414e 4e45 5220 4f56 4552 5249 4445  SPANNER OVERRIDE
+000090f0: 3a0a 0a20 2020 2020 2020 2054 6865 206f  :..        The o
+00009100: 7269 6769 6e61 6c20 7465 7374 2069 7320  riginal test is 
+00009110: 7472 7969 6e67 2074 6f20 6578 6563 7574  trying to execut
+00009120: 6520 6120 7175 6572 7920 6c69 6b65 3a0a  e a query like:.
+00009130: 0a20 2020 2020 2020 2053 454c 4543 5420  .        SELECT 
+00009140: 2e2e 2e0a 2020 2020 2020 2020 5748 4552  ....        WHER
+00009150: 4520 4558 4953 5453 2028 5345 4c45 4354  E EXISTS (SELECT
+00009160: 202e 2e2e 290a 0a20 2020 2020 2020 2053   ...)..        S
+00009170: 454c 4543 5420 5748 4552 4520 7769 7468  ELECT WHERE with
+00009180: 6f75 7420 4652 4f4d 2063 6c61 7573 6520  out FROM clause 
+00009190: 6973 206e 6f74 2073 7570 706f 7274 6564  is not supported
+000091a0: 2062 7920 5370 616e 6e65 722e 0a20 2020   by Spanner..   
+000091b0: 2020 2020 2052 6577 7269 7469 6e67 2074       Rewriting t
+000091c0: 6865 2074 6573 7420 746f 2066 6f72 6365  he test to force
+000091d0: 2069 7420 746f 2067 656e 6572 6174 6520   it to generate 
+000091e0: 6120 7175 6572 7920 6c69 6b65 3a0a 0a20  a query like:.. 
+000091f0: 2020 2020 2020 2053 454c 4543 5420 4558         SELECT EX
+00009200: 4953 5453 2028 5345 4c45 4354 202e 2e2e  ISTS (SELECT ...
+00009210: 290a 2020 2020 2020 2020 2222 220a 2020  ).        """.  
+00009220: 2020 2020 2020 7374 7566 6620 3d20 7365        stuff = se
+00009230: 6c66 2e74 6162 6c65 732e 7374 7566 660a  lf.tables.stuff.
+00009240: 2020 2020 2020 2020 6571 5f28 0a20 2020          eq_(.   
+00009250: 2020 2020 2020 2020 2063 6f6e 6e65 6374           connect
+00009260: 696f 6e2e 6578 6563 7574 6528 0a20 2020  ion.execute(.   
+00009270: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00009280: 6563 7428 2865 7869 7374 7328 292e 7768  ect((exists().wh
+00009290: 6572 6528 7374 7566 662e 632e 6461 7461  ere(stuff.c.data
+000092a0: 203d 3d20 226e 6f20 6461 7461 2229 2c29   == "no data"),)
+000092b0: 290a 2020 2020 2020 2020 2020 2020 292e  ).            ).
+000092c0: 6665 7463 6861 6c6c 2829 2c0a 2020 2020  fetchall(),.    
+000092d0: 2020 2020 2020 2020 5b28 4661 6c73 652c          [(False,
+000092e0: 295d 2c0a 2020 2020 2020 2020 290a 0a0a  )],.        )...
+000092f0: 636c 6173 7320 5461 626c 6544 444c 5465  class TableDDLTe
+00009300: 7374 285f 5461 626c 6544 444c 5465 7374  st(_TableDDLTest
+00009310: 293a 0a20 2020 2040 7079 7465 7374 2e6d  ):.    @pytest.m
+00009320: 6172 6b2e 736b 6970 280a 2020 2020 2020  ark.skip(.      
+00009330: 2020 2253 7061 6e6e 6572 2074 6162 6c65    "Spanner table
+00009340: 206e 616d 6520 6d75 7374 2073 7461 7274   name must start
+00009350: 2077 6974 6820 616e 2075 7070 6572 6361   with an upperca
+00009360: 7365 206f 7220 6c6f 7765 7263 6173 6520  se or lowercase 
+00009370: 6c65 7474 6572 220a 2020 2020 290a 2020  letter".    ).  
+00009380: 2020 6465 6620 7465 7374 5f75 6e64 6572    def test_under
+00009390: 7363 6f72 655f 6e61 6d65 7328 7365 6c66  score_names(self
+000093a0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+000093b0: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
+000093c0: 6b2e 736b 6970 2822 5461 626c 6520 6e61  k.skip("Table na
+000093d0: 6d65 7320 696e 6375 6469 6e67 2073 6368  mes incuding sch
+000093e0: 656d 6173 2061 7265 206e 6f74 2073 7570  emas are not sup
+000093f0: 706f 7274 6564 2062 7920 5370 616e 6e65  ported by Spanne
+00009400: 7222 290a 2020 2020 6465 6620 7465 7374  r").    def test
+00009410: 5f63 7265 6174 655f 7461 626c 655f 7363  _create_table_sc
+00009420: 6865 6d61 2873 656c 6629 3a0a 2020 2020  hema(self):.    
+00009430: 2020 2020 7061 7373 0a0a 0a63 6c61 7373      pass...class
+00009440: 2046 7574 7572 6554 6162 6c65 4444 4c54   FutureTableDDLT
+00009450: 6573 7428 5f46 7574 7572 6554 6162 6c65  est(_FutureTable
+00009460: 4444 4c54 6573 7429 3a0a 2020 2020 4070  DDLTest):.    @p
+00009470: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
+00009480: 2254 6162 6c65 206e 616d 6573 2069 6e63  "Table names inc
+00009490: 7564 696e 6720 7363 6865 6d61 7320 6172  uding schemas ar
+000094a0: 6520 6e6f 7420 7375 7070 6f72 7465 6420  e not supported 
+000094b0: 6279 2053 7061 6e6e 6572 2229 0a20 2020  by Spanner").   
+000094c0: 2064 6566 2074 6573 745f 6372 6561 7465   def test_create
+000094d0: 5f74 6162 6c65 5f73 6368 656d 6128 7365  _table_schema(se
+000094e0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+000094f0: 730a 0a20 2020 2040 7079 7465 7374 2e6d  s..    @pytest.m
+00009500: 6172 6b2e 736b 6970 280a 2020 2020 2020  ark.skip(.      
+00009510: 2020 2253 7061 6e6e 6572 2074 6162 6c65    "Spanner table
+00009520: 206e 616d 6520 6d75 7374 2073 7461 7274   name must start
+00009530: 2077 6974 6820 616e 2075 7070 6572 6361   with an upperca
+00009540: 7365 206f 7220 6c6f 7765 7263 6173 6520  se or lowercase 
+00009550: 6c65 7474 6572 220a 2020 2020 290a 2020  letter".    ).  
+00009560: 2020 6465 6620 7465 7374 5f75 6e64 6572    def test_under
+00009570: 7363 6f72 655f 6e61 6d65 7328 7365 6c66  score_names(self
+00009580: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+00009590: 0a0a 4070 7974 6573 742e 6d61 726b 2e73  ..@pytest.mark.s
+000095a0: 6b69 7028 224d 6178 2069 6465 6e74 6966  kip("Max identif
+000095b0: 6965 7220 6c65 6e67 7468 2069 6e20 5370  ier length in Sp
+000095c0: 616e 6e65 7220 6973 2031 3238 2229 0a63  anner is 128").c
+000095d0: 6c61 7373 204c 6f6e 674e 616d 6542 6c6f  lass LongNameBlo
+000095e0: 776f 7574 5465 7374 285f 4c6f 6e67 4e61  woutTest(_LongNa
+000095f0: 6d65 426c 6f77 6f75 7454 6573 7429 3a0a  meBlowoutTest):.
+00009600: 2020 2020 7061 7373 0a0a 0a40 7079 7465      pass...@pyte
+00009610: 7374 2e6d 6172 6b2e 736b 6970 2822 5370  st.mark.skip("Sp
+00009620: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
+00009630: 7070 6f72 7420 5469 6d65 2064 6174 6120  pport Time data 
+00009640: 7479 7065 2e22 290a 636c 6173 7320 5469  type.").class Ti
+00009650: 6d65 5465 7374 7328 5f54 696d 654d 6963  meTests(_TimeMic
+00009660: 726f 7365 636f 6e64 7354 6573 742c 205f  rosecondsTest, _
+00009670: 5469 6d65 5465 7374 293a 0a20 2020 2070  TimeTest):.    p
+00009680: 6173 730a 0a0a 4070 7974 6573 742e 6d61  ass...@pytest.ma
+00009690: 726b 2e73 6b69 7028 2253 7061 6e6e 6572  rk.skip("Spanner
+000096a0: 2064 6f65 736e 2774 2063 6f65 7263 6520   doesn't coerce 
+000096b0: 6461 7465 7320 6672 6f6d 2064 6174 6574  dates from datet
+000096c0: 696d 652e 2229 0a63 6c61 7373 2044 6174  ime.").class Dat
+000096d0: 6554 696d 6543 6f65 7263 6564 546f 4461  eTimeCoercedToDa
+000096e0: 7465 5469 6d65 5465 7374 285f 4461 7465  teTimeTest(_Date
+000096f0: 5469 6d65 436f 6572 6365 6454 6f44 6174  TimeCoercedToDat
+00009700: 6554 696d 6554 6573 7429 3a0a 2020 2020  eTimeTest):.    
+00009710: 7061 7373 0a0a 0a63 6c61 7373 2049 6e74  pass...class Int
+00009720: 6567 6572 5465 7374 285f 496e 7465 6765  egerTest(_Intege
+00009730: 7254 6573 7429 3a0a 2020 2020 4070 726f  rTest):.    @pro
+00009740: 7669 6465 5f6d 6574 6164 6174 610a 2020  vide_metadata.  
+00009750: 2020 6465 6620 5f72 6f75 6e64 5f74 7269    def _round_tri
+00009760: 7028 7365 6c66 2c20 6461 7461 7479 7065  p(self, datatype
+00009770: 2c20 6461 7461 293a 0a20 2020 2020 2020  , data):.       
+00009780: 2022 2222 0a20 2020 2020 2020 2053 5041   """.        SPA
+00009790: 4e4e 4552 204f 5645 5252 4944 453a 0a0a  NNER OVERRIDE:..
+000097a0: 2020 2020 2020 2020 5468 6973 2069 7320          This is 
+000097b0: 7468 6520 6865 6c70 6572 206d 6574 686f  the helper metho
+000097c0: 6420 666f 7220 696e 7465 6765 7220 636c  d for integer cl
+000097d0: 6173 7320 7465 7374 7320 7768 6963 6820  ass tests which 
+000097e0: 6372 6561 7465 7320 6120 7461 626c 6520  creates a table 
+000097f0: 616e 640a 2020 2020 2020 2020 7065 7266  and.        perf
+00009800: 6f72 6d73 2061 6e20 696e 7365 7274 206f  orms an insert o
+00009810: 7065 7261 7469 6f6e 2e0a 2020 2020 2020  peration..      
+00009820: 2020 436c 6f75 6420 5370 616e 6e65 7220    Cloud Spanner 
+00009830: 7375 7070 6f72 7473 2074 6162 6c65 7320  supports tables 
+00009840: 7769 7468 2061 6e20 656d 7074 7920 7072  with an empty pr
+00009850: 696d 6172 7920 6b65 792c 2062 7574 206f  imary key, but o
+00009860: 6e6c 7920 6f6e 650a 2020 2020 2020 2020  nly one.        
+00009870: 726f 7720 6361 6e20 6265 2069 6e73 6572  row can be inser
+00009880: 7465 6420 696e 746f 2073 7563 6820 6120  ted into such a 
+00009890: 7461 626c 6520 2d20 666f 6c6c 6f77 696e  table - followin
+000098a0: 6720 696e 7365 7274 696f 6e73 2077 696c  g insertions wil
+000098b0: 6c20 6661 696c 2077 6974 680a 2020 2020  l fail with.    
+000098c0: 2020 2020 6034 3030 2069 6420 6d75 7374      `400 id must
+000098d0: 206e 6f74 2062 6520 4e55 4c4c 2069 6e20   not be NULL in 
+000098e0: 7461 626c 6520 6461 7465 5f74 6162 6c65  table date_table
+000098f0: 602e 0a20 2020 2020 2020 204f 7665 7272  `..        Overr
+00009900: 6964 696e 6720 7468 6520 7465 7374 7320  iding the tests 
+00009910: 616e 6420 6164 6469 6e67 2061 206d 616e  and adding a man
+00009920: 7561 6c20 7072 696d 6172 7920 6b65 7920  ual primary key 
+00009930: 7661 6c75 6520 746f 2061 766f 6964 2074  value to avoid t
+00009940: 6865 2073 616d 650a 2020 2020 2020 2020  he same.        
+00009950: 6661 696c 7572 6573 2e0a 2020 2020 2020  failures..      
+00009960: 2020 2222 220a 2020 2020 2020 2020 6d65    """.        me
+00009970: 7461 6461 7461 203d 2073 656c 662e 6d65  tadata = self.me
+00009980: 7461 6461 7461 0a20 2020 2020 2020 2069  tadata.        i
+00009990: 6e74 5f74 6162 6c65 203d 2054 6162 6c65  nt_table = Table
+000099a0: 280a 2020 2020 2020 2020 2020 2020 2269  (.            "i
+000099b0: 6e74 6567 6572 5f74 6162 6c65 222c 0a20  nteger_table",. 
+000099c0: 2020 2020 2020 2020 2020 206d 6574 6164             metad
+000099d0: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
+000099e0: 2043 6f6c 756d 6e28 2269 6422 2c20 496e   Column("id", In
+000099f0: 7465 6765 722c 2070 7269 6d61 7279 5f6b  teger, primary_k
+00009a00: 6579 3d54 7275 652c 2074 6573 745f 6e65  ey=True, test_ne
+00009a10: 6564 735f 6175 746f 696e 6372 656d 656e  eds_autoincremen
+00009a20: 743d 5472 7565 292c 0a20 2020 2020 2020  t=True),.       
+00009a30: 2020 2020 2043 6f6c 756d 6e28 2269 6e74       Column("int
+00009a40: 6567 6572 5f64 6174 6122 2c20 6461 7461  eger_data", data
+00009a50: 7479 7065 292c 0a20 2020 2020 2020 2029  type),.        )
+00009a60: 0a0a 2020 2020 2020 2020 6d65 7461 6461  ..        metada
+00009a70: 7461 2e63 7265 6174 655f 616c 6c28 636f  ta.create_all(co
+00009a80: 6e66 6967 2e64 6229 0a0a 2020 2020 2020  nfig.db)..      
+00009a90: 2020 636f 6e66 6967 2e64 622e 6578 6563    config.db.exec
+00009aa0: 7574 6528 696e 745f 7461 626c 652e 696e  ute(int_table.in
+00009ab0: 7365 7274 2829 2c20 7b22 6964 223a 2031  sert(), {"id": 1
+00009ac0: 2c20 2269 6e74 6567 6572 5f64 6174 6122  , "integer_data"
+00009ad0: 3a20 6461 7461 7d29 0a0a 2020 2020 2020  : data})..      
+00009ae0: 2020 726f 7720 3d20 636f 6e66 6967 2e64    row = config.d
+00009af0: 622e 6578 6563 7574 6528 7365 6c65 6374  b.execute(select
+00009b00: 285b 696e 745f 7461 626c 652e 632e 696e  ([int_table.c.in
+00009b10: 7465 6765 725f 6461 7461 5d29 292e 6669  teger_data])).fi
+00009b20: 7273 7428 290a 0a20 2020 2020 2020 2065  rst()..        e
+00009b30: 715f 2872 6f77 2c20 2864 6174 612c 2929  q_(row, (data,))
+00009b40: 0a0a 2020 2020 2020 2020 6966 2075 7469  ..        if uti
+00009b50: 6c2e 7079 336b 3a0a 2020 2020 2020 2020  l.py3k:.        
+00009b60: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
+00009b70: 7461 6e63 6528 726f 775b 305d 2c20 696e  tance(row[0], in
+00009b80: 7429 0a20 2020 2020 2020 2065 6c73 653a  t).        else:
+00009b90: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+00009ba0: 6572 7420 6973 696e 7374 616e 6365 2872  ert isinstance(r
+00009bb0: 6f77 5b30 5d2c 2028 6c6f 6e67 2c20 696e  ow[0], (long, in
+00009bc0: 7429 2920 2023 206e 6f71 610a 0a0a 636c  t))  # noqa...cl
+00009bd0: 6173 7320 5f55 6e69 636f 6465 4669 7874  ass _UnicodeFixt
+00009be0: 7572 6528 5f5f 556e 6963 6f64 6546 6978  ure(__UnicodeFix
+00009bf0: 7475 7265 293a 0a20 2020 2040 636c 6173  ture):.    @clas
+00009c00: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
+00009c10: 6465 6669 6e65 5f74 6162 6c65 7328 636c  define_tables(cl
+00009c20: 732c 206d 6574 6164 6174 6129 3a0a 2020  s, metadata):.  
+00009c30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00009c40: 2020 5350 414e 4e45 5220 4f56 4552 5249    SPANNER OVERRI
+00009c50: 4445 3a0a 0a20 2020 2020 2020 2043 6c6f  DE:..        Clo
+00009c60: 7564 2053 7061 6e6e 6572 2064 6f65 736e  ud Spanner doesn
+00009c70: 2774 2073 7570 706f 7274 2061 7574 6f20  't support auto 
+00009c80: 696e 6372 656d 656e 7469 6e67 2069 6473  incrementing ids
+00009c90: 2066 6561 7475 7265 2c0a 2020 2020 2020   feature,.      
+00009ca0: 2020 7768 6963 6820 6973 2075 7365 6420    which is used 
+00009cb0: 6279 2074 6865 206f 7269 6769 6e61 6c20  by the original 
+00009cc0: 7465 7374 2e20 4f76 6572 7269 6469 6e67  test. Overriding
+00009cd0: 2074 6865 2074 6573 7420 6461 7461 0a20   the test data. 
+00009ce0: 2020 2020 2020 2063 7265 6174 696f 6e20         creation 
+00009cf0: 6d65 7468 6f64 2074 6f20 6469 7361 626c  method to disabl
+00009d00: 6520 6175 746f 696e 6372 656d 656e 7420  e autoincrement 
+00009d10: 616e 6420 6d61 6b65 2069 6420 636f 6c75  and make id colu
+00009d20: 6d6e 0a20 2020 2020 2020 206e 756c 6c61  mn.        nulla
+00009d30: 626c 652e 0a20 2020 2020 2020 2022 2222  ble..        """
+00009d40: 0a20 2020 2020 2020 2054 6162 6c65 280a  .        Table(.
+00009d50: 2020 2020 2020 2020 2020 2020 2275 6e69              "uni
+00009d60: 636f 6465 5f74 6162 6c65 222c 0a20 2020  code_table",.   
+00009d70: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
+00009d80: 612c 0a20 2020 2020 2020 2020 2020 2043  a,.            C
+00009d90: 6f6c 756d 6e28 2269 6422 2c20 496e 7465  olumn("id", Inte
+00009da0: 6765 722c 2070 7269 6d61 7279 5f6b 6579  ger, primary_key
+00009db0: 3d54 7275 652c 206e 756c 6c61 626c 653d  =True, nullable=
+00009dc0: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
+00009dd0: 2020 2043 6f6c 756d 6e28 2275 6e69 636f     Column("unico
+00009de0: 6465 5f64 6174 6122 2c20 636c 732e 6461  de_data", cls.da
+00009df0: 7461 7479 7065 292c 0a20 2020 2020 2020  tatype),.       
+00009e00: 2029 0a0a 2020 2020 6465 6620 7465 7374   )..    def test
+00009e10: 5f72 6f75 6e64 5f74 7269 705f 6578 6563  _round_trip_exec
+00009e20: 7574 656d 616e 7928 7365 6c66 293a 0a20  utemany(self):. 
+00009e30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00009e40: 2020 2053 5041 4e4e 4552 204f 5645 5252     SPANNER OVERR
+00009e50: 4944 450a 0a20 2020 2020 2020 2043 6c6f  IDE..        Clo
+00009e60: 7564 2053 7061 6e6e 6572 2073 7570 706f  ud Spanner suppo
+00009e70: 7274 7320 7461 626c 6573 2077 6974 6820  rts tables with 
+00009e80: 656d 7074 7920 7072 696d 6172 7920 6b65  empty primary ke
+00009e90: 792c 2062 7574 0a20 2020 2020 2020 206f  y, but.        o
+00009ea0: 6e6c 7920 7369 6e67 6c65 206f 6e65 2072  nly single one r
+00009eb0: 6f77 2063 616e 2062 6520 696e 7365 7274  ow can be insert
+00009ec0: 6564 2069 6e74 6f20 7375 6368 2061 2074  ed into such a t
+00009ed0: 6162 6c65 202d 0a20 2020 2020 2020 2066  able -.        f
+00009ee0: 6f6c 6c6f 7769 6e67 2069 6e73 6572 7469  ollowing inserti
+00009ef0: 6f6e 7320 7769 6c6c 2066 6169 6c20 7769  ons will fail wi
+00009f00: 7468 2060 526f 7720 5b5d 2061 6c72 6561  th `Row [] alrea
+00009f10: 6479 2065 7869 7374 7322 2e0a 2020 2020  dy exists"..    
+00009f20: 2020 2020 4f76 6572 7269 6469 6e67 2074      Overriding t
+00009f30: 6865 2074 6573 7420 746f 2061 766f 6964  he test to avoid
+00009f40: 2074 6865 2073 616d 6520 6661 696c 7572   the same failur
+00009f50: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
+00009f60: 2020 2020 2020 2075 6e69 636f 6465 5f74         unicode_t
+00009f70: 6162 6c65 203d 2073 656c 662e 7461 626c  able = self.tabl
+00009f80: 6573 2e75 6e69 636f 6465 5f74 6162 6c65  es.unicode_table
+00009f90: 0a0a 2020 2020 2020 2020 636f 6e66 6967  ..        config
+00009fa0: 2e64 622e 6578 6563 7574 6528 0a20 2020  .db.execute(.   
+00009fb0: 2020 2020 2020 2020 2075 6e69 636f 6465           unicode
+00009fc0: 5f74 6162 6c65 2e69 6e73 6572 7428 292c  _table.insert(),
+00009fd0: 0a20 2020 2020 2020 2020 2020 205b 7b22  .            [{"
+00009fe0: 6964 223a 2069 2c20 2275 6e69 636f 6465  id": i, "unicode
+00009ff0: 5f64 6174 6122 3a20 7365 6c66 2e64 6174  _data": self.dat
+0000a000: 617d 2066 6f72 2069 2069 6e20 7261 6e67  a} for i in rang
+0000a010: 6528 3329 5d2c 0a20 2020 2020 2020 2029  e(3)],.        )
+0000a020: 0a0a 2020 2020 2020 2020 726f 7773 203d  ..        rows =
+0000a030: 2063 6f6e 6669 672e 6462 2e65 7865 6375   config.db.execu
+0000a040: 7465 2873 656c 6563 7428 5b75 6e69 636f  te(select([unico
+0000a050: 6465 5f74 6162 6c65 2e63 2e75 6e69 636f  de_table.c.unico
+0000a060: 6465 5f64 6174 615d 2929 2e66 6574 6368  de_data])).fetch
+0000a070: 616c 6c28 290a 2020 2020 2020 2020 6571  all().        eq
+0000a080: 5f28 726f 7773 2c20 5b28 7365 6c66 2e64  _(rows, [(self.d
+0000a090: 6174 612c 2920 666f 7220 6920 696e 2072  ata,) for i in r
+0000a0a0: 616e 6765 2833 295d 290a 2020 2020 2020  ange(3)]).      
+0000a0b0: 2020 666f 7220 726f 7720 696e 2072 6f77    for row in row
+0000a0c0: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
+0000a0d0: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
+0000a0e0: 2872 6f77 5b30 5d2c 2075 7469 6c2e 7465  (row[0], util.te
+0000a0f0: 7874 5f74 7970 6529 0a0a 2020 2020 4070  xt_type)..    @p
+0000a100: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
+0000a110: 2253 7061 6e6e 6572 2064 6f65 736e 2774  "Spanner doesn't
+0000a120: 2073 7570 706f 7274 206e 6f6e 2d61 7363   support non-asc
+0000a130: 6969 2063 6861 7261 6374 6572 7322 290a  ii characters").
+0000a140: 2020 2020 6465 6620 7465 7374 5f6c 6974      def test_lit
+0000a150: 6572 616c 2873 656c 6629 3a0a 2020 2020  eral(self):.    
+0000a160: 2020 2020 7061 7373 0a0a 2020 2020 4070      pass..    @p
+0000a170: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
+0000a180: 2253 7061 6e6e 6572 2064 6f65 736e 2774  "Spanner doesn't
+0000a190: 2073 7570 706f 7274 206e 6f6e 2d61 7363   support non-asc
+0000a1a0: 6969 2063 6861 7261 6374 6572 7322 290a  ii characters").
+0000a1b0: 2020 2020 6465 6620 7465 7374 5f6c 6974      def test_lit
+0000a1c0: 6572 616c 5f6e 6f6e 5f61 7363 6969 2873  eral_non_ascii(s
+0000a1d0: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+0000a1e0: 7373 0a0a 0a63 6c61 7373 2055 6e69 636f  ss...class Unico
+0000a1f0: 6465 5661 7263 6861 7254 6573 7428 5f55  deVarcharTest(_U
+0000a200: 6e69 636f 6465 4669 7874 7572 652c 205f  nicodeFixture, _
+0000a210: 556e 6963 6f64 6556 6172 6368 6172 5465  UnicodeVarcharTe
+0000a220: 7374 293a 0a20 2020 2022 2222 0a20 2020  st):.    """.   
+0000a230: 2053 5041 4e4e 4552 204f 5645 5252 4944   SPANNER OVERRID
+0000a240: 453a 0a0a 2020 2020 556e 6963 6f64 6556  E:..    UnicodeV
+0000a250: 6172 6368 6172 5465 7374 2063 6c61 7373  archarTest class
+0000a260: 2069 6e68 6572 6974 7320 7468 6520 5f5f   inherits the __
+0000a270: 556e 6963 6f64 6546 6978 7475 7265 2063  UnicodeFixture c
+0000a280: 6c61 7373 2773 2074 6573 7473 2c0a 2020  lass's tests,.  
+0000a290: 2020 736f 2074 6f20 6176 6f69 6420 7468    so to avoid th
+0000a2a0: 6f73 6520 6661 696c 7572 6573 2061 6e64  ose failures and
+0000a2b0: 206d 6169 6e74 6169 6e20 4452 5920 636f   maintain DRY co
+0000a2c0: 6e63 6570 7420 6a75 7374 2069 6e68 6572  ncept just inher
+0000a2d0: 6974 2074 6865 2063 6c61 7373 2074 6f20  it the class to 
+0000a2e0: 7275 6e0a 2020 2020 7465 7374 7320 7375  run.    tests su
+0000a2f0: 6363 6573 7366 756c 6c79 2e0a 2020 2020  ccessfully..    
+0000a300: 2222 220a 0a20 2020 2070 6173 730a 0a0a  """..    pass...
+0000a310: 636c 6173 7320 556e 6963 6f64 6554 6578  class UnicodeTex
+0000a320: 7454 6573 7428 5f55 6e69 636f 6465 4669  tTest(_UnicodeFi
+0000a330: 7874 7572 652c 205f 556e 6963 6f64 6554  xture, _UnicodeT
+0000a340: 6578 7454 6573 7429 3a0a 2020 2020 2222  extTest):.    ""
+0000a350: 220a 2020 2020 5350 414e 4e45 5220 4f56  ".    SPANNER OV
+0000a360: 4552 5249 4445 3a0a 0a20 2020 2055 6e69  ERRIDE:..    Uni
+0000a370: 636f 6465 5465 7874 5465 7374 2063 6c61  codeTextTest cla
+0000a380: 7373 2069 6e68 6572 6974 7320 7468 6520  ss inherits the 
+0000a390: 5f5f 556e 6963 6f64 6546 6978 7475 7265  __UnicodeFixture
+0000a3a0: 2063 6c61 7373 2773 2074 6573 7473 2c0a   class's tests,.
+0000a3b0: 2020 2020 736f 2074 6f20 6176 6f69 6420      so to avoid 
+0000a3c0: 7468 6f73 6520 6661 696c 7572 6573 2061  those failures a
+0000a3d0: 6e64 206d 6169 6e74 6169 6e20 4452 5920  nd maintain DRY 
+0000a3e0: 636f 6e63 6570 7420 6a75 7374 2069 6e68  concept just inh
+0000a3f0: 6572 6974 2074 6865 2063 6c61 7373 2074  erit the class t
+0000a400: 6f20 7275 6e0a 2020 2020 7465 7374 7320  o run.    tests 
+0000a410: 7375 6363 6573 7366 756c 6c79 2e0a 2020  successfully..  
+0000a420: 2020 2222 220a 0a20 2020 2070 6173 730a    """..    pass.
+0000a430: 0a0a 636c 6173 7320 526f 7746 6574 6368  ..class RowFetch
+0000a440: 5465 7374 285f 526f 7746 6574 6368 5465  Test(_RowFetchTe
+0000a450: 7374 293a 0a20 2020 2064 6566 2074 6573  st):.    def tes
+0000a460: 745f 726f 775f 775f 7363 616c 6172 5f73  t_row_w_scalar_s
+0000a470: 656c 6563 7428 7365 6c66 293a 0a20 2020  elect(self):.   
+0000a480: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000a490: 2053 5041 4e4e 4552 204f 5645 5252 4944   SPANNER OVERRID
+0000a4a0: 453a 0a0a 2020 2020 2020 2020 436c 6f75  E:..        Clou
+0000a4b0: 6420 5370 616e 6e65 7220 7265 7475 726e  d Spanner return
+0000a4c0: 7320 6120 4461 7465 7469 6d65 5769 7468  s a DatetimeWith
+0000a4d0: 4e61 6e6f 7365 636f 6e64 7328 2920 666f  Nanoseconds() fo
+0000a4e0: 7220 6461 7465 0a20 2020 2020 2020 2064  r date.        d
+0000a4f0: 6174 6120 7479 7065 732e 204f 7665 7272  ata types. Overr
+0000a500: 6964 696e 6720 7468 6520 7465 7374 2074  iding the test t
+0000a510: 6f20 7573 6520 6120 4461 7465 7469 6d65  o use a Datetime
+0000a520: 5769 7468 4e61 6e6f 7365 636f 6e64 730a  WithNanoseconds.
+0000a530: 2020 2020 2020 2020 7479 7065 2076 616c          type val
+0000a540: 7565 2061 7320 616e 2065 7870 6563 7465  ue as an expecte
+0000a550: 6420 7265 7375 6c74 2e0a 2020 2020 2020  d result..      
+0000a560: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+0000a570: 0a0a 2020 2020 2020 2020 7465 7374 2074  ..        test t
+0000a580: 6861 7420 6120 7363 616c 6172 2073 656c  hat a scalar sel
+0000a590: 6563 7420 6173 2061 2063 6f6c 756d 6e20  ect as a column 
+0000a5a0: 6973 2072 6574 7572 6e65 6420 6173 2073  is returned as s
+0000a5b0: 7563 680a 2020 2020 2020 2020 616e 6420  uch.        and 
+0000a5c0: 7468 6174 2074 7970 6520 636f 6e76 6572  that type conver
+0000a5d0: 7369 6f6e 2077 6f72 6b73 204f 4b2e 0a0a  sion works OK...
+0000a5e0: 2020 2020 2020 2020 2874 6869 7320 6973          (this is
+0000a5f0: 2068 616c 6620 6120 5351 4c41 6c63 6865   half a SQLAlche
+0000a600: 6d79 2043 6f72 6520 7465 7374 2061 6e64  my Core test and
+0000a610: 2068 616c 6620 746f 2063 6174 6368 2064   half to catch d
+0000a620: 6174 6162 6173 650a 2020 2020 2020 2020  atabase.        
+0000a630: 6261 636b 656e 6473 2074 6861 7420 6d61  backends that ma
+0000a640: 7920 6861 7665 2075 6e75 7375 616c 2062  y have unusual b
+0000a650: 6568 6176 696f 7220 7769 7468 2073 6361  ehavior with sca
+0000a660: 6c61 7220 7365 6c65 6374 732e 290a 2020  lar selects.).  
+0000a670: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000a680: 2020 6461 7465 7461 626c 6520 3d20 7365    datetable = se
+0000a690: 6c66 2e74 6162 6c65 732e 6861 735f 6461  lf.tables.has_da
+0000a6a0: 7465 730a 2020 2020 2020 2020 7320 3d20  tes.        s = 
+0000a6b0: 7365 6c65 6374 285b 6461 7465 7461 626c  select([datetabl
+0000a6c0: 652e 616c 6961 7328 2278 2229 2e63 2e74  e.alias("x").c.t
+0000a6d0: 6f64 6179 5d29 2e73 6361 6c61 725f 7375  oday]).scalar_su
+0000a6e0: 6271 7565 7279 2829 0a20 2020 2020 2020  bquery().       
+0000a6f0: 2073 3220 3d20 7365 6c65 6374 285b 6461   s2 = select([da
+0000a700: 7465 7461 626c 652e 632e 6964 2c20 732e  tetable.c.id, s.
+0000a710: 6c61 6265 6c28 2273 6f6d 656c 6162 656c  label("somelabel
+0000a720: 2229 5d29 0a20 2020 2020 2020 2072 6f77  ")]).        row
+0000a730: 203d 2063 6f6e 6669 672e 6462 2e65 7865   = config.db.exe
+0000a740: 6375 7465 2873 3229 2e66 6972 7374 2829  cute(s2).first()
+0000a750: 0a0a 2020 2020 2020 2020 6571 5f28 0a20  ..        eq_(. 
+0000a760: 2020 2020 2020 2020 2020 2072 6f77 5b22             row["
+0000a770: 736f 6d65 6c61 6265 6c22 5d2c 0a20 2020  somelabel"],.   
+0000a780: 2020 2020 2020 2020 2044 6174 6574 696d           Datetim
+0000a790: 6557 6974 684e 616e 6f73 6563 6f6e 6473  eWithNanoseconds
+0000a7a0: 2832 3030 362c 2035 2c20 3132 2c20 3132  (2006, 5, 12, 12
+0000a7b0: 2c20 302c 2030 2c20 747a 696e 666f 3d74  , 0, 0, tzinfo=t
+0000a7c0: 696d 657a 6f6e 652e 7574 6329 2c0a 2020  imezone.utc),.  
+0000a7d0: 2020 2020 2020 290a 0a0a 636c 6173 7320        )...class 
+0000a7e0: 496e 7365 7274 4265 6861 7669 6f72 5465  InsertBehaviorTe
+0000a7f0: 7374 285f 496e 7365 7274 4265 6861 7669  st(_InsertBehavi
+0000a800: 6f72 5465 7374 293a 0a20 2020 2040 7079  orTest):.    @py
+0000a810: 7465 7374 2e6d 6172 6b2e 736b 6970 2822  test.mark.skip("
+0000a820: 5370 616e 6e65 7220 646f 6573 6e27 7420  Spanner doesn't 
+0000a830: 7375 7070 6f72 7420 656d 7074 7920 696e  support empty in
+0000a840: 7365 7274 7322 290a 2020 2020 6465 6620  serts").    def 
+0000a850: 7465 7374 5f65 6d70 7479 5f69 6e73 6572  test_empty_inser
+0000a860: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+0000a870: 2070 6173 730a 0a20 2020 2040 7079 7465   pass..    @pyte
+0000a880: 7374 2e6d 6172 6b2e 736b 6970 2822 5370  st.mark.skip("Sp
+0000a890: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
+0000a8a0: 7070 6f72 7420 656d 7074 7920 696e 7365  pport empty inse
+0000a8b0: 7274 7322 290a 2020 2020 6465 6620 7465  rts").    def te
+0000a8c0: 7374 5f65 6d70 7479 5f69 6e73 6572 745f  st_empty_insert_
+0000a8d0: 6d75 6c74 6970 6c65 2873 656c 6629 3a0a  multiple(self):.
+0000a8e0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+0000a8f0: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
+0000a900: 6b69 7028 2253 7061 6e6e 6572 2064 6f65  kip("Spanner doe
+0000a910: 736e 2774 2073 7570 706f 7274 2061 7574  sn't support aut
+0000a920: 6f20 696e 6372 656d 656e 7422 290a 2020  o increment").  
+0000a930: 2020 6465 6620 7465 7374 5f69 6e73 6572    def test_inser
+0000a940: 745f 6672 6f6d 5f73 656c 6563 745f 6175  t_from_select_au
+0000a950: 746f 696e 6328 7365 6c66 293a 0a20 2020  toinc(self):.   
+0000a960: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+0000a970: 6566 2074 6573 745f 6175 746f 636c 6f73  ef test_autoclos
+0000a980: 655f 6f6e 5f69 6e73 6572 7428 7365 6c66  e_on_insert(self
+0000a990: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000a9a0: 2020 2020 2020 2053 5041 4e4e 4552 204f         SPANNER O
+0000a9b0: 5645 5252 4944 453a 0a0a 2020 2020 2020  VERRIDE:..      
+0000a9c0: 2020 436c 6f75 6420 5370 616e 6e65 7220    Cloud Spanner 
+0000a9d0: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
+0000a9e0: 7461 626c 6573 2077 6974 6820 616e 2061  tables with an a
+0000a9f0: 7574 6f20 696e 6372 656d 656e 7420 7072  uto increment pr
+0000aa00: 696d 6172 7920 6b65 792c 0a20 2020 2020  imary key,.     
+0000aa10: 2020 2066 6f6c 6c6f 7769 6e67 2069 6e73     following ins
+0000aa20: 6572 7469 6f6e 7320 7769 6c6c 2066 6169  ertions will fai
+0000aa30: 6c20 7769 7468 2060 3430 3020 6964 206d  l with `400 id m
+0000aa40: 7573 7420 6e6f 7420 6265 204e 554c 4c20  ust not be NULL 
+0000aa50: 696e 2074 6162 6c65 0a20 2020 2020 2020  in table.       
+0000aa60: 2061 7574 6f69 6e63 5f70 6b60 2e0a 0a20   autoinc_pk`... 
+0000aa70: 2020 2020 2020 204f 7665 7272 6964 696e         Overridin
+0000aa80: 6720 7468 6520 7465 7374 7320 616e 6420  g the tests and 
+0000aa90: 6164 6469 6e67 2061 206d 616e 7561 6c20  adding a manual 
+0000aaa0: 7072 696d 6172 7920 6b65 7920 7661 6c75  primary key valu
+0000aab0: 6520 746f 2061 766f 6964 2074 6865 2073  e to avoid the s
+0000aac0: 616d 650a 2020 2020 2020 2020 6661 696c  ame.        fail
+0000aad0: 7572 6573 2e0a 2020 2020 2020 2020 2222  ures..        ""
+0000aae0: 220a 2020 2020 2020 2020 6966 2063 6f6e  ".        if con
+0000aaf0: 6669 672e 7265 7175 6972 656d 656e 7473  fig.requirements
+0000ab00: 2e72 6574 7572 6e69 6e67 2e65 6e61 626c  .returning.enabl
+0000ab10: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
+0000ab20: 656e 6769 6e65 203d 2065 6e67 696e 6573  engine = engines
+0000ab30: 2e74 6573 7469 6e67 5f65 6e67 696e 6528  .testing_engine(
+0000ab40: 6f70 7469 6f6e 733d 7b22 696d 706c 6963  options={"implic
+0000ab50: 6974 5f72 6574 7572 6e69 6e67 223a 2046  it_returning": F
+0000ab60: 616c 7365 7d29 0a20 2020 2020 2020 2065  alse}).        e
+0000ab70: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000ab80: 2065 6e67 696e 6520 3d20 636f 6e66 6967   engine = config
+0000ab90: 2e64 620a 0a20 2020 2020 2020 2077 6974  .db..        wit
+0000aba0: 6820 656e 6769 6e65 2e62 6567 696e 2829  h engine.begin()
+0000abb0: 2061 7320 636f 6e6e 3a0a 2020 2020 2020   as conn:.      
+0000abc0: 2020 2020 2020 7220 3d20 636f 6e6e 2e65        r = conn.e
+0000abd0: 7865 6375 7465 280a 2020 2020 2020 2020  xecute(.        
+0000abe0: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
+0000abf0: 6c65 732e 6175 746f 696e 635f 706b 2e69  les.autoinc_pk.i
+0000ac00: 6e73 6572 7428 292c 2064 6963 7428 6964  nsert(), dict(id
+0000ac10: 3d31 2c20 6461 7461 3d22 736f 6d65 2064  =1, data="some d
+0000ac20: 6174 6122 290a 2020 2020 2020 2020 2020  ata").          
+0000ac30: 2020 290a 0a20 2020 2020 2020 2061 7373    )..        ass
+0000ac40: 6572 7420 722e 5f73 6f66 745f 636c 6f73  ert r._soft_clos
+0000ac50: 6564 0a20 2020 2020 2020 2061 7373 6572  ed.        asser
+0000ac60: 7420 6e6f 7420 722e 636c 6f73 6564 0a20  t not r.closed. 
+0000ac70: 2020 2020 2020 2061 7373 6572 7420 722e         assert r.
+0000ac80: 6973 5f69 6e73 6572 740a 2020 2020 2020  is_insert.      
+0000ac90: 2020 6173 7365 7274 206e 6f74 2072 2e72    assert not r.r
+0000aca0: 6574 7572 6e73 5f72 6f77 730a 0a0a 636c  eturns_rows...cl
+0000acb0: 6173 7320 4279 7465 7354 6573 7428 5f4c  ass BytesTest(_L
+0000acc0: 6974 6572 616c 526f 756e 6454 7269 7046  iteralRoundTripF
+0000acd0: 6978 7475 7265 2c20 6669 7874 7572 6573  ixture, fixtures
+0000ace0: 2e54 6573 7442 6173 6529 3a0a 2020 2020  .TestBase):.    
+0000acf0: 5f5f 6261 636b 656e 645f 5f20 3d20 5472  __backend__ = Tr
+0000ad00: 7565 0a0a 2020 2020 6465 6620 7465 7374  ue..    def test
+0000ad10: 5f6e 6f6c 656e 6774 685f 6269 6e61 7279  _nolength_binary
+0000ad20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000ad30: 6d65 7461 6461 7461 203d 204d 6574 6144  metadata = MetaD
+0000ad40: 6174 6128 290a 2020 2020 2020 2020 666f  ata().        fo
+0000ad50: 6f20 3d20 5461 626c 6528 2266 6f6f 222c  o = Table("foo",
+0000ad60: 206d 6574 6164 6174 612c 2043 6f6c 756d   metadata, Colum
+0000ad70: 6e28 226f 6e65 222c 204c 6172 6765 4269  n("one", LargeBi
+0000ad80: 6e61 7279 2929 0a0a 2020 2020 2020 2020  nary))..        
+0000ad90: 666f 6f2e 6372 6561 7465 2863 6f6e 6669  foo.create(confi
+0000ada0: 672e 6462 290a 2020 2020 2020 2020 666f  g.db).        fo
+0000adb0: 6f2e 6472 6f70 2863 6f6e 6669 672e 6462  o.drop(config.db
+0000adc0: 290a 0a0a 636c 6173 7320 5374 7269 6e67  )...class String
+0000add0: 5465 7374 285f 5374 7269 6e67 5465 7374  Test(_StringTest
+0000ade0: 293a 0a20 2020 2040 7079 7465 7374 2e6d  ):.    @pytest.m
+0000adf0: 6172 6b2e 736b 6970 2822 5370 616e 6e65  ark.skip("Spanne
+0000ae00: 7220 646f 6573 6e27 7420 7375 7070 6f72  r doesn't suppor
+0000ae10: 7420 6e6f 6e2d 6173 6369 6920 6368 6172  t non-ascii char
+0000ae20: 6163 7465 7273 2229 0a20 2020 2064 6566  acters").    def
+0000ae30: 2074 6573 745f 6c69 7465 7261 6c5f 6e6f   test_literal_no
+0000ae40: 6e5f 6173 6369 6928 7365 6c66 293a 0a20  n_ascii(self):. 
+0000ae50: 2020 2020 2020 2070 6173 730a 0a0a 636c         pass...cl
+0000ae60: 6173 7320 5465 7874 5465 7374 285f 5465  ass TextTest(_Te
+0000ae70: 7874 5465 7374 293a 0a20 2020 2040 636c  xtTest):.    @cl
+0000ae80: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
+0000ae90: 6620 6465 6669 6e65 5f74 6162 6c65 7328  f define_tables(
+0000aea0: 636c 732c 206d 6574 6164 6174 6129 3a0a  cls, metadata):.
+0000aeb0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000aec0: 2020 2020 5350 414e 4e45 5220 4f56 4552      SPANNER OVER
+0000aed0: 5249 4445 3a0a 0a20 2020 2020 2020 2043  RIDE:..        C
+0000aee0: 6c6f 7564 2053 7061 6e6e 6572 2064 6f65  loud Spanner doe
+0000aef0: 736e 2774 2073 7570 706f 7274 2061 7574  sn't support aut
+0000af00: 6f20 696e 6372 656d 656e 7469 6e67 2069  o incrementing i
+0000af10: 6473 2066 6561 7475 7265 2c0a 2020 2020  ds feature,.    
+0000af20: 2020 2020 7768 6963 6820 6973 2075 7365      which is use
+0000af30: 6420 6279 2074 6865 206f 7269 6769 6e61  d by the origina
+0000af40: 6c20 7465 7374 2e20 4f76 6572 7269 6469  l test. Overridi
+0000af50: 6e67 2074 6865 2074 6573 7420 6461 7461  ng the test data
+0000af60: 0a20 2020 2020 2020 2063 7265 6174 696f  .        creatio
+0000af70: 6e20 6d65 7468 6f64 2074 6f20 6469 7361  n method to disa
+0000af80: 626c 6520 6175 746f 696e 6372 656d 656e  ble autoincremen
+0000af90: 7420 616e 6420 6d61 6b65 2069 6420 636f  t and make id co
+0000afa0: 6c75 6d6e 0a20 2020 2020 2020 206e 756c  lumn.        nul
+0000afb0: 6c61 626c 652e 0a20 2020 2020 2020 2022  lable..        "
+0000afc0: 2222 0a20 2020 2020 2020 2054 6162 6c65  "".        Table
+0000afd0: 280a 2020 2020 2020 2020 2020 2020 2274  (.            "t
+0000afe0: 6578 745f 7461 626c 6522 2c0a 2020 2020  ext_table",.    
+0000aff0: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
+0000b000: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
+0000b010: 6c75 6d6e 2822 6964 222c 2049 6e74 6567  lumn("id", Integ
+0000b020: 6572 2c20 7072 696d 6172 795f 6b65 793d  er, primary_key=
+0000b030: 5472 7565 2c20 6e75 6c6c 6162 6c65 3d54  True, nullable=T
+0000b040: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
+0000b050: 2020 436f 6c75 6d6e 2822 7465 7874 5f64    Column("text_d
+0000b060: 6174 6122 2c20 5465 7874 292c 0a20 2020  ata", Text),.   
+0000b070: 2020 2020 2029 0a0a 2020 2020 4070 7974       )..    @pyt
+0000b080: 6573 742e 6d61 726b 2e73 6b69 7028 2253  est.mark.skip("S
+0000b090: 7061 6e6e 6572 2064 6f65 736e 2774 2073  panner doesn't s
+0000b0a0: 7570 706f 7274 206e 6f6e 2d61 7363 6969  upport non-ascii
+0000b0b0: 2063 6861 7261 6374 6572 7322 290a 2020   characters").  
+0000b0c0: 2020 6465 6620 7465 7374 5f6c 6974 6572    def test_liter
+0000b0d0: 616c 5f6e 6f6e 5f61 7363 6969 2873 656c  al_non_ascii(sel
+0000b0e0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+0000b0f0: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
+0000b100: 726b 2e73 6b69 7028 224e 6f74 2073 7570  rk.skip("Not sup
+0000b110: 706f 7274 6564 2062 7920 5370 616e 6e65  ported by Spanne
+0000b120: 7222 290a 2020 2020 6465 6620 7465 7374  r").    def test
+0000b130: 5f74 6578 745f 726f 756e 6474 7269 7028  _text_roundtrip(
+0000b140: 7365 6c66 2c20 636f 6e6e 6563 7469 6f6e  self, connection
+0000b150: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+0000b160: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
+0000b170: 6b2e 736b 6970 2822 4e6f 7420 7375 7070  k.skip("Not supp
+0000b180: 6f72 7465 6420 6279 2053 7061 6e6e 6572  orted by Spanner
+0000b190: 2229 0a20 2020 2064 6566 2074 6573 745f  ").    def test_
+0000b1a0: 7465 7874 5f65 6d70 7479 5f73 7472 696e  text_empty_strin
+0000b1b0: 6773 2873 656c 662c 2063 6f6e 6e65 6374  gs(self, connect
+0000b1c0: 696f 6e29 3a0a 2020 2020 2020 2020 7061  ion):.        pa
+0000b1d0: 7373 0a0a 2020 2020 4070 7974 6573 742e  ss..    @pytest.
+0000b1e0: 6d61 726b 2e73 6b69 7028 224e 6f74 2073  mark.skip("Not s
+0000b1f0: 7570 706f 7274 6564 2062 7920 5370 616e  upported by Span
+0000b200: 6e65 7222 290a 2020 2020 6465 6620 7465  ner").    def te
+0000b210: 7374 5f74 6578 745f 6e75 6c6c 5f73 7472  st_text_null_str
+0000b220: 696e 6773 2873 656c 662c 2063 6f6e 6e65  ings(self, conne
+0000b230: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
+0000b240: 7061 7373 0a0a 0a63 6c61 7373 204e 756d  pass...class Num
+0000b250: 6572 6963 5465 7374 285f 4e75 6d65 7269  ericTest(_Numeri
+0000b260: 6354 6573 7429 3a0a 2020 2020 4074 6573  cTest):.    @tes
+0000b270: 7469 6e67 2e66 6978 7475 7265 0a20 2020  ting.fixture.   
+0000b280: 2064 6566 2064 6f5f 6e75 6d65 7269 635f   def do_numeric_
+0000b290: 7465 7374 2873 656c 662c 206d 6574 6164  test(self, metad
+0000b2a0: 6174 612c 2063 6f6e 6e65 6374 696f 6e29  ata, connection)
+0000b2b0: 3a0a 2020 2020 2020 2020 4074 6573 7469  :.        @testi
+0000b2c0: 6e67 2e65 6d69 7473 5f77 6172 6e69 6e67  ng.emits_warning
+0000b2d0: 2872 222e 2a64 6f65 7320 5c2a 6e6f 745c  (r".*does \*not\
+0000b2e0: 2a20 7375 7070 6f72 7420 4465 6369 6d61  * support Decima
+0000b2f0: 6c20 6f62 6a65 6374 7320 6e61 7469 7665  l objects native
+0000b300: 6c79 2229 0a20 2020 2020 2020 2064 6566  ly").        def
+0000b310: 2072 756e 2874 7970 655f 2c20 696e 7075   run(type_, inpu
+0000b320: 745f 2c20 6f75 7470 7574 2c20 6669 6c74  t_, output, filt
+0000b330: 6572 5f3d 4e6f 6e65 2c20 6368 6563 6b5f  er_=None, check_
+0000b340: 7363 616c 653d 4661 6c73 6529 3a0a 2020  scale=False):.  
+0000b350: 2020 2020 2020 2020 2020 7420 3d20 5461            t = Ta
+0000b360: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
+0000b370: 2020 2020 2022 7422 2c0a 2020 2020 2020       "t",.      
+0000b380: 2020 2020 2020 2020 2020 6d65 7461 6461            metada
+0000b390: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
+0000b3a0: 2020 2020 436f 6c75 6d6e 2822 7822 2c20      Column("x", 
+0000b3b0: 7479 7065 5f29 2c0a 2020 2020 2020 2020  type_),.        
+0000b3c0: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
+0000b3d0: 6964 222c 2049 6e74 6567 6572 2c20 7072  id", Integer, pr
+0000b3e0: 696d 6172 795f 6b65 793d 5472 7565 292c  imary_key=True),
+0000b3f0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0000b400: 2020 2020 2020 2020 2020 2074 2e63 7265             t.cre
+0000b410: 6174 6528 636f 6e6e 6563 7469 6f6e 290a  ate(connection).
+0000b420: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
+0000b430: 6563 7469 6f6e 2e63 6f6e 6e65 6374 696f  ection.connectio
+0000b440: 6e2e 636f 6d6d 6974 2829 0a20 2020 2020  n.commit().     
+0000b450: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
+0000b460: 6e2e 6578 6563 7574 6528 0a20 2020 2020  n.execute(.     
+0000b470: 2020 2020 2020 2020 2020 2074 2e69 6e73             t.ins
+0000b480: 6572 7428 292c 205b 7b22 7822 3a20 782c  ert(), [{"x": x,
+0000b490: 2022 6964 223a 2069 7d20 666f 7220 692c   "id": i} for i,
+0000b4a0: 2078 2069 6e20 656e 756d 6572 6174 6528   x in enumerate(
+0000b4b0: 696e 7075 745f 295d 0a20 2020 2020 2020  input_)].       
+0000b4c0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000b4d0: 2020 2020 7265 7375 6c74 203d 207b 726f      result = {ro
+0000b4e0: 775b 305d 2066 6f72 2072 6f77 2069 6e20  w[0] for row in 
+0000b4f0: 636f 6e6e 6563 7469 6f6e 2e65 7865 6375  connection.execu
+0000b500: 7465 2874 2e73 656c 6563 7428 2929 7d0a  te(t.select())}.
+0000b510: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+0000b520: 7574 203d 2073 6574 286f 7574 7075 7429  ut = set(output)
+0000b530: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000b540: 6669 6c74 6572 5f3a 0a20 2020 2020 2020  filter_:.       
+0000b550: 2020 2020 2020 2020 2072 6573 756c 7420           result 
+0000b560: 3d20 7365 7428 6669 6c74 6572 5f28 7829  = set(filter_(x)
+0000b570: 2066 6f72 2078 2069 6e20 7265 7375 6c74   for x in result
+0000b580: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000b590: 2020 6f75 7470 7574 203d 2073 6574 2866    output = set(f
+0000b5a0: 696c 7465 725f 2878 2920 666f 7220 7820  ilter_(x) for x 
+0000b5b0: 696e 206f 7574 7075 7429 0a20 2020 2020  in output).     
+0000b5c0: 2020 2020 2020 2065 715f 2872 6573 756c         eq_(resul
+0000b5d0: 742c 206f 7574 7075 7429 0a20 2020 2020  t, output).     
+0000b5e0: 2020 2020 2020 2069 6620 6368 6563 6b5f         if check_
+0000b5f0: 7363 616c 653a 0a20 2020 2020 2020 2020  scale:.         
+0000b600: 2020 2020 2020 2065 715f 285b 7374 7228         eq_([str(
+0000b610: 7829 2066 6f72 2078 2069 6e20 7265 7375  x) for x in resu
+0000b620: 6c74 5d2c 205b 7374 7228 7829 2066 6f72  lt], [str(x) for
+0000b630: 2078 2069 6e20 6f75 7470 7574 5d29 0a0a   x in output])..
+0000b640: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0000b650: 756e 0a0a 2020 2020 4065 6d69 7473 5f77  un..    @emits_w
+0000b660: 6172 6e69 6e67 2872 222e 2a64 6f65 7320  arning(r".*does 
+0000b670: 5c2a 6e6f 745c 2a20 7375 7070 6f72 7420  \*not\* support 
+0000b680: 4465 6369 6d61 6c20 6f62 6a65 6374 7320  Decimal objects 
+0000b690: 6e61 7469 7665 6c79 2229 0a20 2020 2064  natively").    d
+0000b6a0: 6566 2074 6573 745f 7265 6e64 6572 5f6c  ef test_render_l
+0000b6b0: 6974 6572 616c 5f6e 756d 6572 6963 2873  iteral_numeric(s
+0000b6c0: 656c 662c 206c 6974 6572 616c 5f72 6f75  elf, literal_rou
+0000b6d0: 6e64 5f74 7269 7029 3a0a 2020 2020 2020  nd_trip):.      
+0000b6e0: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
+0000b6f0: 414e 4e45 5220 4f56 4552 5249 4445 3a0a  ANNER OVERRIDE:.
+0000b700: 0a20 2020 2020 2020 2043 6c6f 7564 2053  .        Cloud S
+0000b710: 7061 6e6e 6572 2073 7570 706f 7274 7320  panner supports 
+0000b720: 7461 626c 6573 2077 6974 6820 616e 2065  tables with an e
+0000b730: 6d70 7479 2070 7269 6d61 7279 206b 6579  mpty primary key
+0000b740: 2c20 6275 740a 2020 2020 2020 2020 6f6e  , but.        on
+0000b750: 6c79 2061 2073 696e 676c 6520 726f 7720  ly a single row 
+0000b760: 6361 6e20 6265 2069 6e73 6572 7465 6420  can be inserted 
+0000b770: 696e 746f 2073 7563 6820 6120 7461 626c  into such a tabl
+0000b780: 6520 2d0a 2020 2020 2020 2020 666f 6c6c  e -.        foll
+0000b790: 6f77 696e 6720 696e 7365 7274 696f 6e73  owing insertions
+0000b7a0: 2077 696c 6c20 6661 696c 2077 6974 6820   will fail with 
+0000b7b0: 6052 6f77 205b 5d20 616c 7265 6164 7920  `Row [] already 
+0000b7c0: 6578 6973 7473 222e 0a20 2020 2020 2020  exists"..       
+0000b7d0: 204f 7665 7272 6964 696e 6720 7468 6520   Overriding the 
+0000b7e0: 7465 7374 2074 6f20 6176 6f69 6420 7468  test to avoid th
+0000b7f0: 6520 7361 6d65 2066 6169 6c75 7265 2e0a  e same failure..
+0000b800: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000b810: 2020 2020 6c69 7465 7261 6c5f 726f 756e      literal_roun
+0000b820: 645f 7472 6970 280a 2020 2020 2020 2020  d_trip(.        
+0000b830: 2020 2020 4e75 6d65 7269 6328 7072 6563      Numeric(prec
+0000b840: 6973 696f 6e3d 382c 2073 6361 6c65 3d34  ision=8, scale=4
+0000b850: 292c 0a20 2020 2020 2020 2020 2020 205b  ),.            [
+0000b860: 6465 6369 6d61 6c2e 4465 6369 6d61 6c28  decimal.Decimal(
+0000b870: 2231 352e 3735 3633 2229 5d2c 0a20 2020  "15.7563")],.   
+0000b880: 2020 2020 2020 2020 205b 6465 6369 6d61           [decima
+0000b890: 6c2e 4465 6369 6d61 6c28 2231 352e 3735  l.Decimal("15.75
+0000b8a0: 3633 2229 5d2c 0a20 2020 2020 2020 2029  63")],.        )
+0000b8b0: 0a0a 2020 2020 4065 6d69 7473 5f77 6172  ..    @emits_war
+0000b8c0: 6e69 6e67 2872 222e 2a64 6f65 7320 5c2a  ning(r".*does \*
+0000b8d0: 6e6f 745c 2a20 7375 7070 6f72 7420 4465  not\* support De
+0000b8e0: 6369 6d61 6c20 6f62 6a65 6374 7320 6e61  cimal objects na
+0000b8f0: 7469 7665 6c79 2229 0a20 2020 2064 6566  tively").    def
+0000b900: 2074 6573 745f 7265 6e64 6572 5f6c 6974   test_render_lit
+0000b910: 6572 616c 5f6e 756d 6572 6963 5f61 7366  eral_numeric_asf
+0000b920: 6c6f 6174 2873 656c 662c 206c 6974 6572  loat(self, liter
+0000b930: 616c 5f72 6f75 6e64 5f74 7269 7029 3a0a  al_round_trip):.
+0000b940: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000b950: 2020 2020 5350 414e 4e45 5220 4f56 4552      SPANNER OVER
+0000b960: 5249 4445 3a0a 0a20 2020 2020 2020 2043  RIDE:..        C
+0000b970: 6c6f 7564 2053 7061 6e6e 6572 2073 7570  loud Spanner sup
+0000b980: 706f 7274 7320 7461 626c 6573 2077 6974  ports tables wit
+0000b990: 6820 616e 2065 6d70 7479 2070 7269 6d61  h an empty prima
+0000b9a0: 7279 206b 6579 2c20 6275 740a 2020 2020  ry key, but.    
+0000b9b0: 2020 2020 6f6e 6c79 2061 2073 696e 676c      only a singl
+0000b9c0: 6520 726f 7720 6361 6e20 6265 2069 6e73  e row can be ins
+0000b9d0: 6572 7465 6420 696e 746f 2073 7563 6820  erted into such 
+0000b9e0: 6120 7461 626c 6520 2d0a 2020 2020 2020  a table -.      
+0000b9f0: 2020 666f 6c6c 6f77 696e 6720 696e 7365    following inse
+0000ba00: 7274 696f 6e73 2077 696c 6c20 6661 696c  rtions will fail
+0000ba10: 2077 6974 6820 6052 6f77 205b 5d20 616c   with `Row [] al
+0000ba20: 7265 6164 7920 6578 6973 7473 222e 0a20  ready exists".. 
+0000ba30: 2020 2020 2020 204f 7665 7272 6964 696e         Overridin
+0000ba40: 6720 7468 6520 7465 7374 2074 6f20 6176  g the test to av
+0000ba50: 6f69 6420 7468 6520 7361 6d65 2066 6169  oid the same fai
+0000ba60: 6c75 7265 2e0a 2020 2020 2020 2020 2222  lure..        ""
+0000ba70: 220a 2020 2020 2020 2020 6c69 7465 7261  ".        litera
+0000ba80: 6c5f 726f 756e 645f 7472 6970 280a 2020  l_round_trip(.  
+0000ba90: 2020 2020 2020 2020 2020 4e75 6d65 7269            Numeri
+0000baa0: 6328 7072 6563 6973 696f 6e3d 382c 2073  c(precision=8, s
+0000bab0: 6361 6c65 3d34 2c20 6173 6465 6369 6d61  cale=4, asdecima
+0000bac0: 6c3d 4661 6c73 6529 2c0a 2020 2020 2020  l=False),.      
+0000bad0: 2020 2020 2020 5b64 6563 696d 616c 2e44        [decimal.D
+0000bae0: 6563 696d 616c 2822 3135 2e37 3536 3322  ecimal("15.7563"
+0000baf0: 295d 2c0a 2020 2020 2020 2020 2020 2020  )],.            
+0000bb00: 5b31 352e 3735 3633 5d2c 0a20 2020 2020  [15.7563],.     
+0000bb10: 2020 2029 0a0a 2020 2020 6465 6620 7465     )..    def te
+0000bb20: 7374 5f72 656e 6465 725f 6c69 7465 7261  st_render_litera
+0000bb30: 6c5f 666c 6f61 7428 7365 6c66 2c20 6c69  l_float(self, li
+0000bb40: 7465 7261 6c5f 726f 756e 645f 7472 6970  teral_round_trip
+0000bb50: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000bb60: 2020 2020 2020 2053 5041 4e4e 4552 204f         SPANNER O
+0000bb70: 5645 5252 4944 453a 0a0a 2020 2020 2020  VERRIDE:..      
+0000bb80: 2020 436c 6f75 6420 5370 616e 6e65 7220    Cloud Spanner 
+0000bb90: 7375 7070 6f72 7473 2074 6162 6c65 7320  supports tables 
+0000bba0: 7769 7468 2061 6e20 656d 7074 7920 7072  with an empty pr
+0000bbb0: 696d 6172 7920 6b65 792c 2062 7574 0a20  imary key, but. 
+0000bbc0: 2020 2020 2020 206f 6e6c 7920 6120 7369         only a si
+0000bbd0: 6e67 6c65 2072 6f77 2063 616e 2062 6520  ngle row can be 
+0000bbe0: 696e 7365 7274 6564 2069 6e74 6f20 7375  inserted into su
+0000bbf0: 6368 2061 2074 6162 6c65 202d 0a20 2020  ch a table -.   
+0000bc00: 2020 2020 2066 6f6c 6c6f 7769 6e67 2069       following i
+0000bc10: 6e73 6572 7469 6f6e 7320 7769 6c6c 2066  nsertions will f
+0000bc20: 6169 6c20 7769 7468 2060 526f 7720 5b5d  ail with `Row []
+0000bc30: 2061 6c72 6561 6479 2065 7869 7374 7322   already exists"
+0000bc40: 2e0a 2020 2020 2020 2020 4f76 6572 7269  ..        Overri
+0000bc50: 6469 6e67 2074 6865 2074 6573 7420 746f  ding the test to
+0000bc60: 2061 766f 6964 2074 6865 2073 616d 6520   avoid the same 
+0000bc70: 6661 696c 7572 652e 0a20 2020 2020 2020  failure..       
+0000bc80: 2022 2222 0a20 2020 2020 2020 206c 6974   """.        lit
+0000bc90: 6572 616c 5f72 6f75 6e64 5f74 7269 7028  eral_round_trip(
+0000bca0: 0a20 2020 2020 2020 2020 2020 2046 6c6f  .            Flo
+0000bcb0: 6174 2834 292c 0a20 2020 2020 2020 2020  at(4),.         
+0000bcc0: 2020 205b 6465 6369 6d61 6c2e 4465 6369     [decimal.Deci
+0000bcd0: 6d61 6c28 2231 352e 3735 3633 2229 5d2c  mal("15.7563")],
+0000bce0: 0a20 2020 2020 2020 2020 2020 205b 3135  .            [15
+0000bcf0: 2e37 3536 335d 2c0a 2020 2020 2020 2020  .7563],.        
+0000bd00: 2020 2020 6669 6c74 6572 5f3d 6c61 6d62      filter_=lamb
+0000bd10: 6461 206e 3a20 6e20 6973 206e 6f74 204e  da n: n is not N
+0000bd20: 6f6e 6520 616e 6420 726f 756e 6428 6e2c  one and round(n,
+0000bd30: 2035 2920 6f72 204e 6f6e 652c 0a20 2020   5) or None,.   
+0000bd40: 2020 2020 2029 0a0a 2020 2020 4072 6571       )..    @req
+0000bd50: 7569 7265 732e 7072 6563 6973 696f 6e5f  uires.precision_
+0000bd60: 6765 6e65 7269 635f 666c 6f61 745f 7479  generic_float_ty
+0000bd70: 7065 0a20 2020 2064 6566 2074 6573 745f  pe.    def test_
+0000bd80: 666c 6f61 745f 6375 7374 6f6d 5f73 6361  float_custom_sca
+0000bd90: 6c65 2873 656c 662c 2064 6f5f 6e75 6d65  le(self, do_nume
+0000bda0: 7269 635f 7465 7374 293a 0a20 2020 2020  ric_test):.     
+0000bdb0: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
+0000bdc0: 5041 4e4e 4552 204f 5645 5252 4944 453a  PANNER OVERRIDE:
+0000bdd0: 0a0a 2020 2020 2020 2020 436c 6f75 6420  ..        Cloud 
+0000bde0: 5370 616e 6e65 7220 7375 7070 6f72 7473  Spanner supports
+0000bdf0: 2074 6162 6c65 7320 7769 7468 2061 6e20   tables with an 
+0000be00: 656d 7074 7920 7072 696d 6172 7920 6b65  empty primary ke
+0000be10: 792c 2062 7574 0a20 2020 2020 2020 206f  y, but.        o
+0000be20: 6e6c 7920 6120 7369 6e67 6c65 2072 6f77  nly a single row
+0000be30: 2063 616e 2062 6520 696e 7365 7274 6564   can be inserted
+0000be40: 2069 6e74 6f20 7375 6368 2061 2074 6162   into such a tab
+0000be50: 6c65 202d 0a20 2020 2020 2020 2066 6f6c  le -.        fol
+0000be60: 6c6f 7769 6e67 2069 6e73 6572 7469 6f6e  lowing insertion
+0000be70: 7320 7769 6c6c 2066 6169 6c20 7769 7468  s will fail with
+0000be80: 2060 526f 7720 5b5d 2061 6c72 6561 6479   `Row [] already
+0000be90: 2065 7869 7374 7322 2e0a 2020 2020 2020   exists"..      
+0000bea0: 2020 4f76 6572 7269 6469 6e67 2074 6865    Overriding the
+0000beb0: 2074 6573 7420 746f 2061 766f 6964 2074   test to avoid t
+0000bec0: 6865 2073 616d 6520 6661 696c 7572 652e  he same failure.
+0000bed0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000bee0: 2020 2020 2064 6f5f 6e75 6d65 7269 635f       do_numeric_
+0000bef0: 7465 7374 280a 2020 2020 2020 2020 2020  test(.          
+0000bf00: 2020 466c 6f61 7428 4e6f 6e65 2c20 6465    Float(None, de
+0000bf10: 6369 6d61 6c5f 7265 7475 726e 5f73 6361  cimal_return_sca
+0000bf20: 6c65 3d37 2c20 6173 6465 6369 6d61 6c3d  le=7, asdecimal=
+0000bf30: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
+0000bf40: 2020 205b 6465 6369 6d61 6c2e 4465 6369     [decimal.Deci
+0000bf50: 6d61 6c28 2231 352e 3735 3633 3832 3722  mal("15.7563827"
+0000bf60: 292c 2064 6563 696d 616c 2e44 6563 696d  ), decimal.Decim
+0000bf70: 616c 2822 3135 2e37 3536 3338 3237 2229  al("15.7563827")
+0000bf80: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+0000bf90: 6465 6369 6d61 6c2e 4465 6369 6d61 6c28  decimal.Decimal(
+0000bfa0: 2231 352e 3735 3633 3832 3722 295d 2c0a  "15.7563827")],.
+0000bfb0: 2020 2020 2020 2020 2020 2020 6368 6563              chec
+0000bfc0: 6b5f 7363 616c 653d 5472 7565 2c0a 2020  k_scale=True,.  
+0000bfd0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+0000bfe0: 2074 6573 745f 6e75 6d65 7269 635f 6173   test_numeric_as
+0000bff0: 5f64 6563 696d 616c 2873 656c 662c 2064  _decimal(self, d
+0000c000: 6f5f 6e75 6d65 7269 635f 7465 7374 293a  o_numeric_test):
+0000c010: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000c020: 2020 2020 2053 5041 4e4e 4552 204f 5645       SPANNER OVE
+0000c030: 5252 4944 453a 0a0a 2020 2020 2020 2020  RRIDE:..        
+0000c040: 5370 616e 6e65 7220 7468 726f 7773 2061  Spanner throws a
+0000c050: 6e20 6572 726f 7220 3430 3020 5661 6c75  n error 400 Valu
+0000c060: 6520 6861 7320 7479 7065 2046 4c4f 4154  e has type FLOAT
+0000c070: 3634 2077 6869 6368 2063 616e 6e6f 7420  64 which cannot 
+0000c080: 6265 0a20 2020 2020 2020 2069 6e73 6572  be.        inser
+0000c090: 7465 6420 696e 746f 2063 6f6c 756d 6e20  ted into column 
+0000c0a0: 782c 2077 6869 6368 2068 6173 2074 7970  x, which has typ
+0000c0b0: 6520 4e55 4d45 5249 4320 666f 7220 7661  e NUMERIC for va
+0000c0c0: 6c75 6520 3135 2e37 3536 332e 0a20 2020  lue 15.7563..   
+0000c0d0: 2020 2020 204f 7665 7272 6964 696e 6720       Overriding 
+0000c0e0: 7468 6520 7465 7374 2074 6f20 7265 6d6f  the test to remo
+0000c0f0: 7665 2074 6865 2066 6169 6c75 7265 2063  ve the failure c
+0000c100: 6173 652e 0a20 2020 2020 2020 2022 2222  ase..        """
+0000c110: 0a20 2020 2020 2020 2064 6f5f 6e75 6d65  .        do_nume
+0000c120: 7269 635f 7465 7374 280a 2020 2020 2020  ric_test(.      
+0000c130: 2020 2020 2020 4e75 6d65 7269 6328 7072        Numeric(pr
+0000c140: 6563 6973 696f 6e3d 382c 2073 6361 6c65  ecision=8, scale
+0000c150: 3d34 292c 0a20 2020 2020 2020 2020 2020  =4),.           
+0000c160: 205b 6465 6369 6d61 6c2e 4465 6369 6d61   [decimal.Decima
+0000c170: 6c28 2231 352e 3735 3633 2229 2c20 6465  l("15.7563"), de
+0000c180: 6369 6d61 6c2e 4465 6369 6d61 6c28 2231  cimal.Decimal("1
+0000c190: 352e 3735 3633 2229 5d2c 0a20 2020 2020  5.7563")],.     
+0000c1a0: 2020 2020 2020 205b 6465 6369 6d61 6c2e         [decimal.
+0000c1b0: 4465 6369 6d61 6c28 2231 352e 3735 3633  Decimal("15.7563
+0000c1c0: 2229 5d2c 0a20 2020 2020 2020 2029 0a0a  ")],.        )..
+0000c1d0: 2020 2020 6465 6620 7465 7374 5f6e 756d      def test_num
+0000c1e0: 6572 6963 5f61 735f 666c 6f61 7428 7365  eric_as_float(se
+0000c1f0: 6c66 2c20 646f 5f6e 756d 6572 6963 5f74  lf, do_numeric_t
+0000c200: 6573 7429 3a0a 2020 2020 2020 2020 2222  est):.        ""
+0000c210: 220a 2020 2020 2020 2020 5350 414e 4e45  ".        SPANNE
+0000c220: 5220 4f56 4552 5249 4445 3a0a 0a20 2020  R OVERRIDE:..   
+0000c230: 2020 2020 2053 7061 6e6e 6572 2074 6872       Spanner thr
+0000c240: 6f77 7320 616e 2065 7272 6f72 2034 3030  ows an error 400
+0000c250: 2056 616c 7565 2068 6173 2074 7970 6520   Value has type 
+0000c260: 464c 4f41 5436 3420 7768 6963 6820 6361  FLOAT64 which ca
+0000c270: 6e6e 6f74 2062 650a 2020 2020 2020 2020  nnot be.        
+0000c280: 696e 7365 7274 6564 2069 6e74 6f20 636f  inserted into co
+0000c290: 6c75 6d6e 2078 2c20 7768 6963 6820 6861  lumn x, which ha
+0000c2a0: 7320 7479 7065 204e 554d 4552 4943 2066  s type NUMERIC f
+0000c2b0: 6f72 2076 616c 7565 2031 352e 3735 3633  or value 15.7563
+0000c2c0: 2e0a 2020 2020 2020 2020 4f76 6572 7269  ..        Overri
+0000c2d0: 6469 6e67 2074 6865 2074 6573 7420 746f  ding the test to
+0000c2e0: 2072 656d 6f76 6520 7468 6520 6661 696c   remove the fail
+0000c2f0: 7572 6520 6361 7365 2e0a 2020 2020 2020  ure case..      
+0000c300: 2020 2222 220a 2020 2020 2020 2020 646f    """.        do
+0000c310: 5f6e 756d 6572 6963 5f74 6573 7428 0a20  _numeric_test(. 
+0000c320: 2020 2020 2020 2020 2020 204e 756d 6572             Numer
+0000c330: 6963 2870 7265 6369 7369 6f6e 3d38 2c20  ic(precision=8, 
+0000c340: 7363 616c 653d 342c 2061 7364 6563 696d  scale=4, asdecim
+0000c350: 616c 3d46 616c 7365 292c 0a20 2020 2020  al=False),.     
+0000c360: 2020 2020 2020 205b 6465 6369 6d61 6c2e         [decimal.
+0000c370: 4465 6369 6d61 6c28 2231 352e 3735 3633  Decimal("15.7563
+0000c380: 2229 2c20 6465 6369 6d61 6c2e 4465 6369  "), decimal.Deci
+0000c390: 6d61 6c28 2231 352e 3735 3633 2229 5d2c  mal("15.7563")],
+0000c3a0: 0a20 2020 2020 2020 2020 2020 205b 3135  .            [15
+0000c3b0: 2e37 3536 335d 2c0a 2020 2020 2020 2020  .7563],.        
+0000c3c0: 290a 0a20 2020 2040 7265 7175 6972 6573  )..    @requires
+0000c3d0: 2e66 6c6f 6174 735f 746f 5f66 6f75 725f  .floats_to_four_
+0000c3e0: 6465 6369 6d61 6c73 0a20 2020 2064 6566  decimals.    def
+0000c3f0: 2074 6573 745f 666c 6f61 745f 6173 5f64   test_float_as_d
+0000c400: 6563 696d 616c 2873 656c 662c 2064 6f5f  ecimal(self, do_
+0000c410: 6e75 6d65 7269 635f 7465 7374 293a 0a20  numeric_test):. 
+0000c420: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000c430: 2020 2053 5041 4e4e 4552 204f 5645 5252     SPANNER OVERR
+0000c440: 4944 453a 0a0a 2020 2020 2020 2020 436c  IDE:..        Cl
+0000c450: 6f75 6420 5370 616e 6e65 7220 7375 7070  oud Spanner supp
+0000c460: 6f72 7473 2074 6162 6c65 7320 7769 7468  orts tables with
+0000c470: 2061 6e20 656d 7074 7920 7072 696d 6172   an empty primar
+0000c480: 7920 6b65 792c 2062 7574 0a20 2020 2020  y key, but.     
+0000c490: 2020 206f 6e6c 7920 6120 7369 6e67 6c65     only a single
+0000c4a0: 2072 6f77 2063 616e 2062 6520 696e 7365   row can be inse
+0000c4b0: 7274 6564 2069 6e74 6f20 7375 6368 2061  rted into such a
+0000c4c0: 2074 6162 6c65 202d 0a20 2020 2020 2020   table -.       
+0000c4d0: 2066 6f6c 6c6f 7769 6e67 2069 6e73 6572   following inser
+0000c4e0: 7469 6f6e 7320 7769 6c6c 2066 6169 6c20  tions will fail 
+0000c4f0: 7769 7468 2060 526f 7720 5b5d 2061 6c72  with `Row [] alr
+0000c500: 6561 6479 2065 7869 7374 7322 2e0a 2020  eady exists"..  
+0000c510: 2020 2020 2020 4f76 6572 7269 6469 6e67        Overriding
+0000c520: 2074 6865 2074 6573 7420 746f 2061 766f   the test to avo
+0000c530: 6964 2074 6865 2073 616d 6520 6661 696c  id the same fail
+0000c540: 7572 652e 0a20 2020 2020 2020 2022 2222  ure..        """
+0000c550: 0a20 2020 2020 2020 2064 6f5f 6e75 6d65  .        do_nume
+0000c560: 7269 635f 7465 7374 280a 2020 2020 2020  ric_test(.      
+0000c570: 2020 2020 2020 466c 6f61 7428 7072 6563        Float(prec
+0000c580: 6973 696f 6e3d 382c 2061 7364 6563 696d  ision=8, asdecim
+0000c590: 616c 3d54 7275 6529 2c0a 2020 2020 2020  al=True),.      
+0000c5a0: 2020 2020 2020 5b64 6563 696d 616c 2e44        [decimal.D
+0000c5b0: 6563 696d 616c 2822 3135 2e37 3536 3322  ecimal("15.7563"
+0000c5c0: 292c 2064 6563 696d 616c 2e44 6563 696d  ), decimal.Decim
+0000c5d0: 616c 2822 3135 2e37 3536 3322 292c 204e  al("15.7563"), N
+0000c5e0: 6f6e 655d 2c0a 2020 2020 2020 2020 2020  one],.          
+0000c5f0: 2020 5b64 6563 696d 616c 2e44 6563 696d    [decimal.Decim
+0000c600: 616c 2822 3135 2e37 3536 3322 292c 204e  al("15.7563"), N
+0000c610: 6f6e 655d 2c0a 2020 2020 2020 2020 2020  one],.          
+0000c620: 2020 6669 6c74 6572 5f3d 6c61 6d62 6461    filter_=lambda
+0000c630: 206e 3a20 6e20 6973 206e 6f74 204e 6f6e   n: n is not Non
+0000c640: 6520 616e 6420 726f 756e 6428 6e2c 2034  e and round(n, 4
+0000c650: 2920 6f72 204e 6f6e 652c 0a20 2020 2020  ) or None,.     
+0000c660: 2020 2029 0a0a 2020 2020 6465 6620 7465     )..    def te
+0000c670: 7374 5f66 6c6f 6174 5f61 735f 666c 6f61  st_float_as_floa
+0000c680: 7428 7365 6c66 2c20 646f 5f6e 756d 6572  t(self, do_numer
+0000c690: 6963 5f74 6573 7429 3a0a 2020 2020 2020  ic_test):.      
+0000c6a0: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
+0000c6b0: 414e 4e45 5220 4f56 4552 5249 4445 3a0a  ANNER OVERRIDE:.
+0000c6c0: 0a20 2020 2020 2020 2043 6c6f 7564 2053  .        Cloud S
+0000c6d0: 7061 6e6e 6572 2073 7570 706f 7274 7320  panner supports 
+0000c6e0: 7461 626c 6573 2077 6974 6820 616e 2065  tables with an e
+0000c6f0: 6d70 7479 2070 7269 6d61 7279 206b 6579  mpty primary key
+0000c700: 2c20 6275 740a 2020 2020 2020 2020 6f6e  , but.        on
+0000c710: 6c79 2061 2073 696e 676c 6520 726f 7720  ly a single row 
+0000c720: 6361 6e20 6265 2069 6e73 6572 7465 6420  can be inserted 
+0000c730: 696e 746f 2073 7563 6820 6120 7461 626c  into such a tabl
+0000c740: 6520 2d0a 2020 2020 2020 2020 666f 6c6c  e -.        foll
+0000c750: 6f77 696e 6720 696e 7365 7274 696f 6e73  owing insertions
+0000c760: 2077 696c 6c20 6661 696c 2077 6974 6820   will fail with 
+0000c770: 6052 6f77 205b 5d20 616c 7265 6164 7920  `Row [] already 
+0000c780: 6578 6973 7473 222e 0a20 2020 2020 2020  exists"..       
+0000c790: 204f 7665 7272 6964 696e 6720 7468 6520   Overriding the 
+0000c7a0: 7465 7374 2074 6f20 6176 6f69 6420 7468  test to avoid th
+0000c7b0: 6520 7361 6d65 2066 6169 6c75 7265 2e0a  e same failure..
+0000c7c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000c7d0: 2020 2020 646f 5f6e 756d 6572 6963 5f74      do_numeric_t
+0000c7e0: 6573 7428 0a20 2020 2020 2020 2020 2020  est(.           
+0000c7f0: 2046 6c6f 6174 2870 7265 6369 7369 6f6e   Float(precision
+0000c800: 3d38 292c 0a20 2020 2020 2020 2020 2020  =8),.           
+0000c810: 205b 6465 6369 6d61 6c2e 4465 6369 6d61   [decimal.Decima
+0000c820: 6c28 2231 352e 3735 3633 2229 2c20 6465  l("15.7563"), de
+0000c830: 6369 6d61 6c2e 4465 6369 6d61 6c28 2231  cimal.Decimal("1
+0000c840: 352e 3735 3633 2229 5d2c 0a20 2020 2020  5.7563")],.     
+0000c850: 2020 2020 2020 205b 3135 2e37 3536 335d         [15.7563]
+0000c860: 2c0a 2020 2020 2020 2020 2020 2020 6669  ,.            fi
+0000c870: 6c74 6572 5f3d 6c61 6d62 6461 206e 3a20  lter_=lambda n: 
+0000c880: 6e20 6973 206e 6f74 204e 6f6e 6520 616e  n is not None an
+0000c890: 6420 726f 756e 6428 6e2c 2035 2920 6f72  d round(n, 5) or
+0000c8a0: 204e 6f6e 652c 0a20 2020 2020 2020 2029   None,.        )
+0000c8b0: 0a0a 2020 2020 4072 6571 7569 7265 732e  ..    @requires.
+0000c8c0: 7072 6563 6973 696f 6e5f 6e75 6d65 7269  precision_numeri
+0000c8d0: 6373 5f67 656e 6572 616c 0a20 2020 2064  cs_general.    d
+0000c8e0: 6566 2074 6573 745f 7072 6563 6973 696f  ef test_precisio
+0000c8f0: 6e5f 6465 6369 6d61 6c28 7365 6c66 2c20  n_decimal(self, 
+0000c900: 646f 5f6e 756d 6572 6963 5f74 6573 7429  do_numeric_test)
+0000c910: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000c920: 2020 2020 2020 5350 414e 4e45 5220 4f56        SPANNER OV
+0000c930: 4552 5249 4445 3a0a 0a20 2020 2020 2020  ERRIDE:..       
+0000c940: 2043 6c6f 7564 2053 7061 6e6e 6572 2073   Cloud Spanner s
+0000c950: 7570 706f 7274 7320 7461 626c 6573 2077  upports tables w
+0000c960: 6974 6820 616e 2065 6d70 7479 2070 7269  ith an empty pri
+0000c970: 6d61 7279 206b 6579 2c20 6275 740a 2020  mary key, but.  
+0000c980: 2020 2020 2020 6f6e 6c79 2061 2073 696e        only a sin
+0000c990: 676c 6520 726f 7720 6361 6e20 6265 2069  gle row can be i
+0000c9a0: 6e73 6572 7465 6420 696e 746f 2073 7563  nserted into suc
+0000c9b0: 6820 6120 7461 626c 6520 2d0a 2020 2020  h a table -.    
+0000c9c0: 2020 2020 666f 6c6c 6f77 696e 6720 696e      following in
+0000c9d0: 7365 7274 696f 6e73 2077 696c 6c20 6661  sertions will fa
+0000c9e0: 696c 2077 6974 6820 6052 6f77 205b 5d20  il with `Row [] 
+0000c9f0: 616c 7265 6164 7920 6578 6973 7473 222e  already exists".
+0000ca00: 0a20 2020 2020 2020 204f 7665 7272 6964  .        Overrid
+0000ca10: 696e 6720 7468 6520 7465 7374 2074 6f20  ing the test to 
+0000ca20: 6176 6f69 6420 7468 6520 7361 6d65 2066  avoid the same f
+0000ca30: 6169 6c75 7265 2e0a 0a20 2020 2020 2020  ailure...       
+0000ca40: 2052 656d 6f76 6520 616e 2065 7874 7261   Remove an extra
+0000ca50: 2064 6967 6974 7320 6166 7465 7220 6465   digits after de
+0000ca60: 6369 6d61 6c20 706f 696e 7420 6173 2063  cimal point as c
+0000ca70: 6c6f 7564 2073 7061 6e6e 6572 2069 730a  loud spanner is.
+0000ca80: 2020 2020 2020 2020 6361 7061 626c 6520          capable 
+0000ca90: 6f66 2072 6570 7265 7365 6e74 696e 6720  of representing 
+0000caa0: 616e 2065 7861 6374 206e 756d 6572 6963  an exact numeric
+0000cab0: 2076 616c 7565 2077 6974 6820 6120 7072   value with a pr
+0000cac0: 6563 6973 696f 6e0a 2020 2020 2020 2020  ecision.        
+0000cad0: 6f66 2033 3820 616e 6420 7363 616c 6520  of 38 and scale 
+0000cae0: 6f66 2039 2e0a 2020 2020 2020 2020 2222  of 9..        ""
+0000caf0: 220a 2020 2020 2020 2020 6e75 6d62 6572  ".        number
+0000cb00: 7320 3d20 7365 7428 0a20 2020 2020 2020  s = set(.       
+0000cb10: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+0000cb20: 2020 2020 2020 2064 6563 696d 616c 2e44         decimal.D
+0000cb30: 6563 696d 616c 2822 3534 2e32 3436 3435  ecimal("54.24645
+0000cb40: 3136 3530 2229 2c0a 2020 2020 2020 2020  1650"),.        
+0000cb50: 2020 2020 2020 2020 6465 6369 6d61 6c2e          decimal.
+0000cb60: 4465 6369 6d61 6c28 2230 2e30 3034 3335  Decimal("0.00435
+0000cb70: 3422 292c 0a20 2020 2020 2020 2020 2020  4"),.           
+0000cb80: 2020 2020 2064 6563 696d 616c 2e44 6563       decimal.Dec
+0000cb90: 696d 616c 2822 3930 302e 3022 292c 0a20  imal("900.0"),. 
+0000cba0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+0000cbb0: 2020 2020 2029 0a20 2020 2020 2020 2064       ).        d
+0000cbc0: 6f5f 6e75 6d65 7269 635f 7465 7374 284e  o_numeric_test(N
+0000cbd0: 756d 6572 6963 2870 7265 6369 7369 6f6e  umeric(precision
+0000cbe0: 3d31 382c 2073 6361 6c65 3d39 292c 206e  =18, scale=9), n
+0000cbf0: 756d 6265 7273 2c20 6e75 6d62 6572 7329  umbers, numbers)
+0000cc00: 0a0a 2020 2020 4074 6573 7469 6e67 2e72  ..    @testing.r
+0000cc10: 6571 7569 7265 732e 7072 6563 6973 696f  equires.precisio
+0000cc20: 6e5f 6e75 6d65 7269 6373 5f65 6e6f 7461  n_numerics_enota
+0000cc30: 7469 6f6e 5f6c 6172 6765 0a20 2020 2064  tion_large.    d
+0000cc40: 6566 2074 6573 745f 656e 6f74 6174 696f  ef test_enotatio
+0000cc50: 6e5f 6465 6369 6d61 6c5f 6c61 7267 6528  n_decimal_large(
+0000cc60: 7365 6c66 2c20 646f 5f6e 756d 6572 6963  self, do_numeric
+0000cc70: 5f74 6573 7429 3a0a 2020 2020 2020 2020  _test):.        
+0000cc80: 2222 2274 6573 7420 6578 6365 6564 696e  """test exceedin
+0000cc90: 676c 7920 6c61 7267 6520 6465 6369 6d61  gly large decima
+0000cca0: 6c73 2e0a 0a20 2020 2020 2020 2053 5041  ls...        SPA
+0000ccb0: 4e4e 4552 204f 5645 5252 4944 453a 0a0a  NNER OVERRIDE:..
+0000ccc0: 2020 2020 2020 2020 436c 6f75 6420 5370          Cloud Sp
+0000ccd0: 616e 6e65 7220 7375 7070 6f72 7473 2074  anner supports t
+0000cce0: 6162 6c65 7320 7769 7468 2061 6e20 656d  ables with an em
+0000ccf0: 7074 7920 7072 696d 6172 7920 6b65 792c  pty primary key,
+0000cd00: 2062 7574 0a20 2020 2020 2020 206f 6e6c   but.        onl
+0000cd10: 7920 6120 7369 6e67 6c65 2072 6f77 2063  y a single row c
+0000cd20: 616e 2062 6520 696e 7365 7274 6564 2069  an be inserted i
+0000cd30: 6e74 6f20 7375 6368 2061 2074 6162 6c65  nto such a table
+0000cd40: 202d 0a20 2020 2020 2020 2066 6f6c 6c6f   -.        follo
+0000cd50: 7769 6e67 2069 6e73 6572 7469 6f6e 7320  wing insertions 
+0000cd60: 7769 6c6c 2066 6169 6c20 7769 7468 2060  will fail with `
+0000cd70: 526f 7720 5b5d 2061 6c72 6561 6479 2065  Row [] already e
+0000cd80: 7869 7374 7322 2e0a 2020 2020 2020 2020  xists"..        
+0000cd90: 4f76 6572 7269 6469 6e67 2074 6865 2074  Overriding the t
+0000cda0: 6573 7420 746f 2061 766f 6964 2074 6865  est to avoid the
+0000cdb0: 2073 616d 6520 6661 696c 7572 652e 0a20   same failure.. 
+0000cdc0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000cdd0: 2020 206e 756d 6265 7273 203d 2073 6574     numbers = set
+0000cde0: 280a 2020 2020 2020 2020 2020 2020 5b0a  (.            [.
+0000cdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce00: 6465 6369 6d61 6c2e 4465 6369 6d61 6c28  decimal.Decimal(
+0000ce10: 2234 452b 3822 292c 0a20 2020 2020 2020  "4E+8"),.       
+0000ce20: 2020 2020 2020 2020 2064 6563 696d 616c           decimal
+0000ce30: 2e44 6563 696d 616c 2822 3537 3438 452b  .Decimal("5748E+
+0000ce40: 3135 2229 2c0a 2020 2020 2020 2020 2020  15"),.          
+0000ce50: 2020 2020 2020 6465 6369 6d61 6c2e 4465        decimal.De
+0000ce60: 6369 6d61 6c28 2231 2e35 3231 452b 3135  cimal("1.521E+15
+0000ce70: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+0000ce80: 2020 2020 6465 6369 6d61 6c2e 4465 6369      decimal.Deci
+0000ce90: 6d61 6c28 2230 3030 3030 3030 3030 2e31  mal("000000000.1
+0000cea0: 452b 3922 292c 0a20 2020 2020 2020 2020  E+9"),.         
+0000ceb0: 2020 205d 0a20 2020 2020 2020 2029 0a20     ].        ). 
+0000cec0: 2020 2020 2020 2064 6f5f 6e75 6d65 7269         do_numeri
+0000ced0: 635f 7465 7374 284e 756d 6572 6963 2870  c_test(Numeric(p
+0000cee0: 7265 6369 7369 6f6e 3d32 352c 2073 6361  recision=25, sca
+0000cef0: 6c65 3d32 292c 206e 756d 6265 7273 2c20  le=2), numbers, 
+0000cf00: 6e75 6d62 6572 7329 0a0a 2020 2020 4074  numbers)..    @t
+0000cf10: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
+0000cf20: 7072 6563 6973 696f 6e5f 6e75 6d65 7269  precision_numeri
+0000cf30: 6373 5f65 6e6f 7461 7469 6f6e 5f6c 6172  cs_enotation_lar
+0000cf40: 6765 0a20 2020 2064 6566 2074 6573 745f  ge.    def test_
+0000cf50: 656e 6f74 6174 696f 6e5f 6465 6369 6d61  enotation_decima
+0000cf60: 6c28 7365 6c66 2c20 646f 5f6e 756d 6572  l(self, do_numer
+0000cf70: 6963 5f74 6573 7429 3a0a 2020 2020 2020  ic_test):.      
+0000cf80: 2020 2222 2274 6573 7420 6578 6365 6564    """test exceed
+0000cf90: 696e 676c 7920 736d 616c 6c20 6465 6369  ingly small deci
+0000cfa0: 6d61 6c73 2e0a 0a20 2020 2020 2020 2044  mals...        D
+0000cfb0: 6563 696d 616c 2072 6570 6f72 7473 2076  ecimal reports v
+0000cfc0: 616c 7565 7320 7769 7468 2045 206e 6f74  alues with E not
+0000cfd0: 6174 696f 6e20 7768 656e 2074 6865 2065  ation when the e
+0000cfe0: 7870 6f6e 656e 740a 2020 2020 2020 2020  xponent.        
+0000cff0: 6973 2067 7265 6174 6572 2074 6861 6e20  is greater than 
+0000d000: 362e 0a0a 2020 2020 2020 2020 5350 414e  6...        SPAN
+0000d010: 4e45 5220 4f56 4552 5249 4445 3a0a 0a20  NER OVERRIDE:.. 
+0000d020: 2020 2020 2020 2052 656d 6f76 6520 6578         Remove ex
+0000d030: 7472 6120 6469 6769 7473 2061 6674 6572  tra digits after
+0000d040: 2064 6563 696d 616c 2070 6f69 6e74 2061   decimal point a
+0000d050: 7320 436c 6f75 6420 5370 616e 6e65 7220  s Cloud Spanner 
+0000d060: 6973 0a20 2020 2020 2020 2063 6170 6162  is.        capab
+0000d070: 6c65 206f 6620 7265 7072 6573 656e 7469  le of representi
+0000d080: 6e67 2061 6e20 6578 6163 7420 6e75 6d65  ng an exact nume
+0000d090: 7269 6320 7661 6c75 6520 7769 7468 2061  ric value with a
+0000d0a0: 2070 7265 6369 7369 6f6e 0a20 2020 2020   precision.     
+0000d0b0: 2020 206f 6620 3338 2061 6e64 2073 6361     of 38 and sca
+0000d0c0: 6c65 206f 6620 392e 0a20 2020 2020 2020  le of 9..       
+0000d0d0: 2022 2222 0a20 2020 2020 2020 206e 756d   """.        num
+0000d0e0: 6265 7273 203d 2073 6574 280a 2020 2020  bers = set(.    
+0000d0f0: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
+0000d100: 2020 2020 2020 2020 2020 6465 6369 6d61            decima
+0000d110: 6c2e 4465 6369 6d61 6c28 2231 452d 3222  l.Decimal("1E-2"
+0000d120: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0000d130: 2020 2064 6563 696d 616c 2e44 6563 696d     decimal.Decim
+0000d140: 616c 2822 3145 2d33 2229 2c0a 2020 2020  al("1E-3"),.    
+0000d150: 2020 2020 2020 2020 2020 2020 6465 6369              deci
+0000d160: 6d61 6c2e 4465 6369 6d61 6c28 2231 452d  mal.Decimal("1E-
+0000d170: 3422 292c 0a20 2020 2020 2020 2020 2020  4"),.           
+0000d180: 2020 2020 2064 6563 696d 616c 2e44 6563       decimal.Dec
+0000d190: 696d 616c 2822 3145 2d35 2229 2c0a 2020  imal("1E-5"),.  
+0000d1a0: 2020 2020 2020 2020 2020 2020 2020 6465                de
+0000d1b0: 6369 6d61 6c2e 4465 6369 6d61 6c28 2231  cimal.Decimal("1
+0000d1c0: 452d 3622 292c 0a20 2020 2020 2020 2020  E-6"),.         
+0000d1d0: 2020 2020 2020 2064 6563 696d 616c 2e44         decimal.D
+0000d1e0: 6563 696d 616c 2822 3145 2d37 2229 2c0a  ecimal("1E-7"),.
+0000d1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d200: 6465 6369 6d61 6c2e 4465 6369 6d61 6c28  decimal.Decimal(
+0000d210: 2231 452d 3822 292c 0a20 2020 2020 2020  "1E-8"),.       
+0000d220: 2020 2020 2020 2020 2064 6563 696d 616c           decimal
+0000d230: 2e44 6563 696d 616c 2822 302e 3130 3539  .Decimal("0.1059
+0000d240: 3430 3639 3622 292c 0a20 2020 2020 2020  40696"),.       
+0000d250: 2020 2020 2020 2020 2064 6563 696d 616c           decimal
+0000d260: 2e44 6563 696d 616c 2822 302e 3030 3539  .Decimal("0.0059
+0000d270: 3430 3639 3622 292c 0a20 2020 2020 2020  40696"),.       
+0000d280: 2020 2020 2020 2020 2064 6563 696d 616c           decimal
+0000d290: 2e44 6563 696d 616c 2822 302e 3030 3030  .Decimal("0.0000
+0000d2a0: 3030 3639 3622 292c 0a20 2020 2020 2020  00696"),.       
+0000d2b0: 2020 2020 2020 2020 2064 6563 696d 616c           decimal
+0000d2c0: 2e44 6563 696d 616c 2822 302e 3730 3030  .Decimal("0.7000
+0000d2d0: 3030 3639 3622 292c 0a20 2020 2020 2020  00696"),.       
+0000d2e0: 2020 2020 2020 2020 2064 6563 696d 616c           decimal
+0000d2f0: 2e44 6563 696d 616c 2822 3639 3645 2d39  .Decimal("696E-9
+0000d300: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+0000d310: 5d0a 2020 2020 2020 2020 290a 2020 2020  ].        ).    
+0000d320: 2020 2020 646f 5f6e 756d 6572 6963 5f74      do_numeric_t
+0000d330: 6573 7428 4e75 6d65 7269 6328 7072 6563  est(Numeric(prec
+0000d340: 6973 696f 6e3d 3338 2c20 7363 616c 653d  ision=38, scale=
+0000d350: 3929 2c20 6e75 6d62 6572 732c 206e 756d  9), numbers, num
+0000d360: 6265 7273 290a 0a0a 636c 6173 7320 4c69  bers)...class Li
+0000d370: 6b65 4675 6e63 7469 6f6e 7354 6573 7428  keFunctionsTest(
+0000d380: 5f4c 696b 6546 756e 6374 696f 6e73 5465  _LikeFunctionsTe
+0000d390: 7374 293a 0a20 2020 2040 7079 7465 7374  st):.    @pytest
+0000d3a0: 2e6d 6172 6b2e 736b 6970 2822 5370 616e  .mark.skip("Span
+0000d3b0: 6e65 7220 646f 6573 6e27 7420 7375 7070  ner doesn't supp
+0000d3c0: 6f72 7420 4c49 4b45 2045 5343 4150 4520  ort LIKE ESCAPE 
+0000d3d0: 636c 6175 7365 2229 0a20 2020 2064 6566  clause").    def
+0000d3e0: 2074 6573 745f 636f 6e74 6169 6e73 5f61   test_contains_a
+0000d3f0: 7574 6f65 7363 6170 6528 7365 6c66 293a  utoescape(self):
+0000d400: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+0000d410: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
+0000d420: 736b 6970 2822 5370 616e 6e65 7220 646f  skip("Spanner do
+0000d430: 6573 6e27 7420 7375 7070 6f72 7420 4c49  esn't support LI
+0000d440: 4b45 2045 5343 4150 4520 636c 6175 7365  KE ESCAPE clause
+0000d450: 2229 0a20 2020 2064 6566 2074 6573 745f  ").    def test_
+0000d460: 636f 6e74 6169 6e73 5f61 7574 6f65 7363  contains_autoesc
+0000d470: 6170 655f 6573 6361 7065 2873 656c 6629  ape_escape(self)
+0000d480: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+0000d490: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+0000d4a0: 2e73 6b69 7028 2253 7061 6e6e 6572 2064  .skip("Spanner d
+0000d4b0: 6f65 736e 2774 2073 7570 706f 7274 204c  oesn't support L
+0000d4c0: 494b 4520 4553 4341 5045 2063 6c61 7573  IKE ESCAPE claus
+0000d4d0: 6522 290a 2020 2020 6465 6620 7465 7374  e").    def test
+0000d4e0: 5f63 6f6e 7461 696e 735f 6573 6361 7065  _contains_escape
+0000d4f0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000d500: 7061 7373 0a0a 2020 2020 4070 7974 6573  pass..    @pytes
+0000d510: 742e 6d61 726b 2e73 6b69 7028 2253 7061  t.mark.skip("Spa
+0000d520: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
+0000d530: 706f 7274 204c 494b 4520 4553 4341 5045  port LIKE ESCAPE
+0000d540: 2063 6c61 7573 6522 290a 2020 2020 6465   clause").    de
+0000d550: 6620 7465 7374 5f65 6e64 7377 6974 685f  f test_endswith_
+0000d560: 6175 746f 6573 6361 7065 2873 656c 6629  autoescape(self)
+0000d570: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+0000d580: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+0000d590: 2e73 6b69 7028 2253 7061 6e6e 6572 2064  .skip("Spanner d
+0000d5a0: 6f65 736e 2774 2073 7570 706f 7274 204c  oesn't support L
+0000d5b0: 494b 4520 4553 4341 5045 2063 6c61 7573  IKE ESCAPE claus
+0000d5c0: 6522 290a 2020 2020 6465 6620 7465 7374  e").    def test
+0000d5d0: 5f65 6e64 7377 6974 685f 6573 6361 7065  _endswith_escape
+0000d5e0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000d5f0: 7061 7373 0a0a 2020 2020 4070 7974 6573  pass..    @pytes
+0000d600: 742e 6d61 726b 2e73 6b69 7028 2253 7061  t.mark.skip("Spa
+0000d610: 6e6e 6572 2064 6f65 736e 2774 2073 7570  nner doesn't sup
+0000d620: 706f 7274 204c 494b 4520 4553 4341 5045  port LIKE ESCAPE
+0000d630: 2063 6c61 7573 6522 290a 2020 2020 6465   clause").    de
+0000d640: 6620 7465 7374 5f65 6e64 7377 6974 685f  f test_endswith_
+0000d650: 6175 746f 6573 6361 7065 5f65 7363 6170  autoescape_escap
+0000d660: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+0000d670: 2070 6173 730a 0a20 2020 2040 7079 7465   pass..    @pyte
+0000d680: 7374 2e6d 6172 6b2e 736b 6970 2822 5370  st.mark.skip("Sp
+0000d690: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
+0000d6a0: 7070 6f72 7420 4c49 4b45 2045 5343 4150  pport LIKE ESCAP
+0000d6b0: 4520 636c 6175 7365 2229 0a20 2020 2064  E clause").    d
+0000d6c0: 6566 2074 6573 745f 7374 6172 7473 7769  ef test_startswi
+0000d6d0: 7468 5f61 7574 6f65 7363 6170 6528 7365  th_autoescape(se
+0000d6e0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+0000d6f0: 730a 0a20 2020 2040 7079 7465 7374 2e6d  s..    @pytest.m
+0000d700: 6172 6b2e 736b 6970 2822 5370 616e 6e65  ark.skip("Spanne
+0000d710: 7220 646f 6573 6e27 7420 7375 7070 6f72  r doesn't suppor
+0000d720: 7420 4c49 4b45 2045 5343 4150 4520 636c  t LIKE ESCAPE cl
+0000d730: 6175 7365 2229 0a20 2020 2064 6566 2074  ause").    def t
+0000d740: 6573 745f 7374 6172 7473 7769 7468 5f65  est_startswith_e
+0000d750: 7363 6170 6528 7365 6c66 293a 0a20 2020  scape(self):.   
+0000d760: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
+0000d770: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
+0000d780: 2822 5370 616e 6e65 7220 646f 6573 6e27  ("Spanner doesn'
+0000d790: 7420 7375 7070 6f72 7420 4c49 4b45 2045  t support LIKE E
+0000d7a0: 5343 4150 4520 636c 6175 7365 2229 0a20  SCAPE clause"). 
+0000d7b0: 2020 2064 6566 2074 6573 745f 7374 6172     def test_star
+0000d7c0: 7473 7769 7468 5f61 7574 6f65 7363 6170  tswith_autoescap
+0000d7d0: 655f 6573 6361 7065 2873 656c 6629 3a0a  e_escape(self):.
+0000d7e0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+0000d7f0: 2020 6465 6620 7465 7374 5f65 7363 6170    def test_escap
+0000d800: 655f 6b65 7977 6f72 645f 7261 6973 6573  e_keyword_raises
+0000d810: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000d820: 2222 2243 6865 636b 2074 6861 7420 4553  """Check that ES
+0000d830: 4341 5045 206b 6579 776f 7264 2063 6175  CAPE keyword cau
+0000d840: 7365 7320 616e 2065 7863 6570 7469 6f6e  ses an exception
+0000d850: 2077 6865 6e20 7573 6564 2e22 2222 0a20   when used.""". 
+0000d860: 2020 2020 2020 2077 6974 6820 7079 7465         with pyte
+0000d870: 7374 2e72 6169 7365 7328 4e6f 7449 6d70  st.raises(NotImp
+0000d880: 6c65 6d65 6e74 6564 4572 726f 7229 3a0a  lementedError):.
+0000d890: 2020 2020 2020 2020 2020 2020 636f 6c20              col 
+0000d8a0: 3d20 7365 6c66 2e74 6162 6c65 732e 736f  = self.tables.so
+0000d8b0: 6d65 5f74 6162 6c65 2e63 2e64 6174 610a  me_table.c.data.
+0000d8c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d8d0: 2e5f 7465 7374 2863 6f6c 2e63 6f6e 7461  ._test(col.conta
+0000d8e0: 696e 7328 2262 2323 6364 6522 2c20 6573  ins("b##cde", es
+0000d8f0: 6361 7065 3d22 2322 292c 207b 377d 290a  cape="#"), {7}).
+0000d900: 0a0a 4070 7974 6573 742e 6d61 726b 2e73  ..@pytest.mark.s
+0000d910: 6b69 7028 2253 7061 6e6e 6572 2064 6f65  kip("Spanner doe
+0000d920: 736e 2774 2073 7570 706f 7274 2049 5320  sn't support IS 
+0000d930: 4449 5354 494e 4354 2046 524f 4d20 636c  DISTINCT FROM cl
+0000d940: 6175 7365 2229 0a63 6c61 7373 2049 734f  ause").class IsO
+0000d950: 7249 734e 6f74 4469 7374 696e 6374 4672  rIsNotDistinctFr
+0000d960: 6f6d 5465 7374 285f 4973 4f72 4973 4e6f  omTest(_IsOrIsNo
+0000d970: 7444 6973 7469 6e63 7446 726f 6d54 6573  tDistinctFromTes
+0000d980: 7429 3a0a 2020 2020 7061 7373 0a0a 0a63  t):.    pass...c
+0000d990: 6c61 7373 204f 7264 6572 4279 4c61 6265  lass OrderByLabe
+0000d9a0: 6c54 6573 7428 5f4f 7264 6572 4279 4c61  lTest(_OrderByLa
+0000d9b0: 6265 6c54 6573 7429 3a0a 2020 2020 4070  belTest):.    @p
+0000d9c0: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
+0000d9d0: 0a20 2020 2020 2020 2022 5370 616e 6e65  .        "Spanne
+0000d9e0: 7220 7265 7175 6972 6573 2061 6e20 616c  r requires an al
+0000d9f0: 6961 7320 666f 7220 7468 6520 4752 4f55  ias for the GROU
+0000da00: 5020 4259 206c 6973 7420 7768 656e 2073  P BY list when s
+0000da10: 7065 6369 6679 696e 6720 6465 7269 7665  pecifying derive
+0000da20: 6420 220a 2020 2020 2020 2020 2263 6f6c  d ".        "col
+0000da30: 756d 6e73 2061 6c73 6f20 7573 6564 2069  umns also used i
+0000da40: 6e20 5345 4c45 4354 220a 2020 2020 290a  n SELECT".    ).
+0000da50: 2020 2020 6465 6620 7465 7374 5f67 726f      def test_gro
+0000da60: 7570 5f62 795f 636f 6d70 6f73 6564 2873  up_by_composed(s
+0000da70: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+0000da80: 7373 0a0a 0a63 6c61 7373 2043 6f6d 706f  ss...class Compo
+0000da90: 756e 6453 656c 6563 7454 6573 7428 5f43  undSelectTest(_C
+0000daa0: 6f6d 706f 756e 6453 656c 6563 7454 6573  ompoundSelectTes
+0000dab0: 7429 3a0a 2020 2020 2222 220a 2020 2020  t):.    """.    
+0000dac0: 5365 653a 2068 7474 7073 3a2f 2f67 6974  See: https://git
+0000dad0: 6875 622e 636f 6d2f 676f 6f67 6c65 6170  hub.com/googleap
+0000dae0: 6973 2f70 7974 686f 6e2d 7370 616e 6e65  is/python-spanne
+0000daf0: 722f 6973 7375 6573 2f33 3437 0a20 2020  r/issues/347.   
+0000db00: 2022 2222 0a0a 2020 2020 4070 7974 6573   """..    @pytes
+0000db10: 742e 6d61 726b 2e73 6b69 7028 0a20 2020  t.mark.skip(.   
+0000db20: 2020 2020 2022 5370 616e 6e65 7220 4442       "Spanner DB
+0000db30: 4150 4920 696e 636f 7272 6563 746c 7920  API incorrectly 
+0000db40: 636c 6173 7369 6679 2074 6865 2073 7461  classify the sta
+0000db50: 7465 6d65 6e74 2073 7461 7274 696e 6720  tement starting 
+0000db60: 7769 7468 2062 7261 636b 6574 732e 220a  with brackets.".
+0000db70: 2020 2020 290a 2020 2020 6465 6620 7465      ).    def te
+0000db80: 7374 5f6c 696d 6974 5f6f 6666 7365 745f  st_limit_offset_
+0000db90: 7365 6c65 6374 6162 6c65 5f69 6e5f 756e  selectable_in_un
+0000dba0: 696f 6e73 2873 656c 6629 3a0a 2020 2020  ions(self):.    
+0000dbb0: 2020 2020 7061 7373 0a0a 2020 2020 4070      pass..    @p
+0000dbc0: 7974 6573 742e 6d61 726b 2e73 6b69 7028  ytest.mark.skip(
+0000dbd0: 0a20 2020 2020 2020 2022 5370 616e 6e65  .        "Spanne
+0000dbe0: 7220 4442 4150 4920 696e 636f 7272 6563  r DBAPI incorrec
+0000dbf0: 746c 7920 636c 6173 7369 6679 2074 6865  tly classify the
+0000dc00: 2073 7461 7465 6d65 6e74 2073 7461 7274   statement start
+0000dc10: 696e 6720 7769 7468 2062 7261 636b 6574  ing with bracket
+0000dc20: 732e 220a 2020 2020 290a 2020 2020 6465  s.".    ).    de
+0000dc30: 6620 7465 7374 5f6f 7264 6572 5f62 795f  f test_order_by_
+0000dc40: 7365 6c65 6374 6162 6c65 5f69 6e5f 756e  selectable_in_un
+0000dc50: 696f 6e73 2873 656c 6629 3a0a 2020 2020  ions(self):.    
+0000dc60: 2020 2020 7061 7373 0a0a 0a63 6c61 7373      pass...class
+0000dc70: 2054 6573 7451 7565 7279 4869 6e74 7328   TestQueryHints(
+0000dc80: 6669 7874 7572 6573 2e54 6162 6c65 7354  fixtures.TablesT
+0000dc90: 6573 7429 3a0a 2020 2020 2222 220a 2020  est):.    """.  
+0000dca0: 2020 436f 6d70 696c 6520 6120 636f 6d70    Compile a comp
+0000dcb0: 6c65 7820 7175 6572 7920 7769 7468 204a  lex query with J
+0000dcc0: 4f49 4e20 616e 6420 6368 6563 6b20 7468  OIN and check th
+0000dcd0: 6174 0a20 2020 2074 6865 2074 6162 6c65  at.    the table
+0000dce0: 2068 696e 7420 7761 7320 7365 7420 696e   hint was set in
+0000dcf0: 746f 2074 6865 2072 6967 6874 2070 6c61  to the right pla
+0000dd00: 6365 2e0a 2020 2020 2222 220a 0a20 2020  ce..    """..   
+0000dd10: 205f 5f62 6163 6b65 6e64 5f5f 203d 2054   __backend__ = T
+0000dd20: 7275 650a 0a20 2020 2064 6566 2074 6573  rue..    def tes
+0000dd30: 745f 636f 6d70 6c65 785f 7175 6572 795f  t_complex_query_
+0000dd40: 7461 626c 655f 6869 6e74 7328 7365 6c66  table_hints(self
+0000dd50: 293a 0a20 2020 2020 2020 2045 5850 4543  ):.        EXPEC
+0000dd60: 5445 445f 5155 4552 5920 3d20 280a 2020  TED_QUERY = (.  
+0000dd70: 2020 2020 2020 2020 2020 2253 454c 4543            "SELEC
+0000dd80: 5420 7573 6572 732e 6964 2c20 7573 6572  T users.id, user
+0000dd90: 732e 6e61 6d65 205c 6e46 524f 4d20 7573  s.name \nFROM us
+0000dda0: 6572 7320 407b 464f 5243 455f 494e 4445  ers @{FORCE_INDE
+0000ddb0: 583d 7461 626c 655f 315f 6279 5f69 6e74  X=table_1_by_int
+0000ddc0: 5f69 6478 7d22 0a20 2020 2020 2020 2020  _idx}".         
+0000ddd0: 2020 2022 204a 4f49 4e20 6164 6472 6573     " JOIN addres
+0000dde0: 7365 7320 4f4e 2075 7365 7273 2e69 6420  ses ON users.id 
+0000ddf0: 3d20 6164 6472 6573 7365 732e 7573 6572  = addresses.user
+0000de00: 5f69 6420 220a 2020 2020 2020 2020 2020  _id ".          
+0000de10: 2020 225c 6e57 4845 5245 2075 7365 7273    "\nWHERE users
+0000de20: 2e6e 616d 6520 494e 2028 5f5f 5b50 4f53  .name IN (__[POS
+0000de30: 5443 4f4d 5049 4c45 5f6e 616d 655f 315d  TCOMPILE_name_1]
+0000de40: 2922 0a20 2020 2020 2020 2029 0a0a 2020  )".        )..  
+0000de50: 2020 2020 2020 4261 7365 203d 2064 6563        Base = dec
+0000de60: 6c61 7261 7469 7665 5f62 6173 6528 290a  larative_base().
+0000de70: 2020 2020 2020 2020 656e 6769 6e65 203d          engine =
+0000de80: 2063 7265 6174 655f 656e 6769 6e65 280a   create_engine(.
+0000de90: 2020 2020 2020 2020 2020 2020 2273 7061              "spa
+0000dea0: 6e6e 6572 3a2f 2f2f 7072 6f6a 6563 7473  nner:///projects
+0000deb0: 2f70 726f 6a65 6374 2d69 642f 696e 7374  /project-id/inst
+0000dec0: 616e 6365 732f 696e 7374 616e 6365 2d69  ances/instance-i
+0000ded0: 642f 6461 7461 6261 7365 732f 6461 7461  d/databases/data
+0000dee0: 6261 7365 2d69 6422 0a20 2020 2020 2020  base-id".       
+0000def0: 2029 0a0a 2020 2020 2020 2020 636c 6173   )..        clas
+0000df00: 7320 5573 6572 2842 6173 6529 3a0a 2020  s User(Base):.  
+0000df10: 2020 2020 2020 2020 2020 5f5f 7461 626c            __tabl
+0000df20: 656e 616d 655f 5f20 3d20 2275 7365 7273  ename__ = "users
+0000df30: 220a 2020 2020 2020 2020 2020 2020 6964  ".            id
+0000df40: 203d 2043 6f6c 756d 6e28 496e 7465 6765   = Column(Intege
+0000df50: 722c 2070 7269 6d61 7279 5f6b 6579 3d54  r, primary_key=T
+0000df60: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+0000df70: 206e 616d 6520 3d20 436f 6c75 6d6e 2853   name = Column(S
+0000df80: 7472 696e 6728 3530 2929 0a20 2020 2020  tring(50)).     
+0000df90: 2020 2020 2020 2061 6464 7265 7373 6573         addresses
+0000dfa0: 203d 2072 656c 6174 696f 6e28 2241 6464   = relation("Add
+0000dfb0: 7265 7373 222c 2062 6163 6b72 6566 3d22  ress", backref="
+0000dfc0: 7573 6572 2229 0a0a 2020 2020 2020 2020  user")..        
+0000dfd0: 636c 6173 7320 4164 6472 6573 7328 4261  class Address(Ba
+0000dfe0: 7365 293a 0a20 2020 2020 2020 2020 2020  se):.           
+0000dff0: 205f 5f74 6162 6c65 6e61 6d65 5f5f 203d   __tablename__ =
+0000e000: 2022 6164 6472 6573 7365 7322 0a20 2020   "addresses".   
+0000e010: 2020 2020 2020 2020 2069 6420 3d20 436f           id = Co
+0000e020: 6c75 6d6e 2849 6e74 6567 6572 2c20 7072  lumn(Integer, pr
+0000e030: 696d 6172 795f 6b65 793d 5472 7565 290a  imary_key=True).
+0000e040: 2020 2020 2020 2020 2020 2020 656d 6169              emai
+0000e050: 6c20 3d20 436f 6c75 6d6e 2853 7472 696e  l = Column(Strin
+0000e060: 6728 3530 2929 0a20 2020 2020 2020 2020  g(50)).         
+0000e070: 2020 2075 7365 725f 6964 203d 2043 6f6c     user_id = Col
+0000e080: 756d 6e28 496e 7465 6765 722c 2046 6f72  umn(Integer, For
+0000e090: 6569 676e 4b65 7928 2275 7365 7273 2e69  eignKey("users.i
+0000e0a0: 6422 2929 0a0a 2020 2020 2020 2020 7365  d"))..        se
+0000e0b0: 7373 696f 6e20 3d20 5365 7373 696f 6e28  ssion = Session(
+0000e0c0: 656e 6769 6e65 290a 0a20 2020 2020 2020  engine)..       
+0000e0d0: 2071 7565 7279 203d 2073 6573 7369 6f6e   query = session
+0000e0e0: 2e71 7565 7279 2855 7365 7229 0a20 2020  .query(User).   
+0000e0f0: 2020 2020 2071 7565 7279 203d 2071 7565       query = que
+0000e100: 7279 2e77 6974 685f 6869 6e74 280a 2020  ry.with_hint(.  
+0000e110: 2020 2020 2020 2020 2020 7365 6c65 6374            select
+0000e120: 6162 6c65 3d55 7365 722c 2074 6578 743d  able=User, text=
+0000e130: 2240 7b46 4f52 4345 5f49 4e44 4558 3d74  "@{FORCE_INDEX=t
+0000e140: 6162 6c65 5f31 5f62 795f 696e 745f 6964  able_1_by_int_id
+0000e150: 787d 220a 2020 2020 2020 2020 290a 0a20  x}".        ).. 
+0000e160: 2020 2020 2020 2071 7565 7279 203d 2071         query = q
+0000e170: 7565 7279 2e66 696c 7465 7228 5573 6572  uery.filter(User
+0000e180: 2e6e 616d 652e 696e 5f28 5b22 7661 6c31  .name.in_(["val1
+0000e190: 222c 2022 7661 6c32 225d 2929 0a20 2020  ", "val2"])).   
+0000e1a0: 2020 2020 2071 7565 7279 203d 2071 7565       query = que
+0000e1b0: 7279 2e6a 6f69 6e28 4164 6472 6573 7329  ry.join(Address)
+0000e1c0: 0a0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+0000e1d0: 2073 7472 2871 7565 7279 2e73 7461 7465   str(query.state
+0000e1e0: 6d65 6e74 2e63 6f6d 7069 6c65 2873 6573  ment.compile(ses
+0000e1f0: 7369 6f6e 2e62 696e 6429 2920 3d3d 2045  sion.bind)) == E
+0000e200: 5850 4543 5445 445f 5155 4552 590a 0a0a  XPECTED_QUERY...
+0000e210: 636c 6173 7320 496e 7465 726c 6561 7665  class Interleave
+0000e220: 6454 6162 6c65 7354 6573 7428 6669 7874  dTablesTest(fixt
+0000e230: 7572 6573 2e54 6573 7442 6173 6529 3a0a  ures.TestBase):.
+0000e240: 2020 2020 2222 220a 2020 2020 4368 6563      """.    Chec
+0000e250: 6b20 7468 6174 2043 5245 4154 4520 5441  k that CREATE TA
+0000e260: 424c 4520 7374 6174 656d 656e 7473 2066  BLE statements f
+0000e270: 6f72 2069 6e74 6572 6c65 6176 6564 2074  or interleaved t
+0000e280: 6162 6c65 7320 6172 6520 636f 7272 6563  ables are correc
+0000e290: 746c 790a 2020 2020 6765 6e65 7261 7465  tly.    generate
+0000e2a0: 642e 0a20 2020 2022 2222 0a0a 2020 2020  d..    """..    
+0000e2b0: 6465 6620 7365 7455 7028 7365 6c66 293a  def setUp(self):
+0000e2c0: 0a20 2020 2020 2020 2073 656c 662e 5f65  .        self._e
+0000e2d0: 6e67 696e 6520 3d20 6372 6561 7465 5f65  ngine = create_e
+0000e2e0: 6e67 696e 6528 0a20 2020 2020 2020 2020  ngine(.         
+0000e2f0: 2020 2022 7370 616e 6e65 723a 2f2f 2f70     "spanner:///p
+0000e300: 726f 6a65 6374 732f 6170 7064 6576 2d73  rojects/appdev-s
+0000e310: 6f64 612d 7370 616e 6e65 722d 7374 6167  oda-spanner-stag
+0000e320: 696e 672f 696e 7374 616e 6365 732f 220a  ing/instances/".
+0000e330: 2020 2020 2020 2020 2020 2020 2273 716c              "sql
+0000e340: 616c 6368 656d 792d 6469 616c 6563 742d  alchemy-dialect-
+0000e350: 7465 7374 2f64 6174 6162 6173 6573 2f63  test/databases/c
+0000e360: 6f6d 706c 6961 6e63 652d 7465 7374 220a  ompliance-test".
+0000e370: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000e380: 2020 7365 6c66 2e5f 6d65 7461 6461 7461    self._metadata
+0000e390: 203d 204d 6574 6144 6174 6128 6269 6e64   = MetaData(bind
+0000e3a0: 3d73 656c 662e 5f65 6e67 696e 6529 0a0a  =self._engine)..
+0000e3b0: 2020 2020 6465 6620 7465 7374 5f69 6e74      def test_int
+0000e3c0: 6572 6c65 6176 6528 7365 6c66 293a 0a20  erleave(self):. 
+0000e3d0: 2020 2020 2020 2045 5850 5f51 5545 5259         EXP_QUERY
+0000e3e0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+0000e3f0: 2022 5c6e 4352 4541 5445 2054 4142 4c45   "\nCREATE TABLE
+0000e400: 2063 6c69 656e 7420 285c 6e5c 7474 6561   client (\n\ttea
+0000e410: 6d5f 6964 2049 4e54 3634 204e 4f54 204e  m_id INT64 NOT N
+0000e420: 554c 4c2c 2022 0a20 2020 2020 2020 2020  ULL, ".         
+0000e430: 2020 2022 5c6e 5c74 636c 6965 6e74 5f69     "\n\tclient_i
+0000e440: 6420 494e 5436 3420 4e4f 5420 4e55 4c4c  d INT64 NOT NULL
+0000e450: 2c20 220a 2020 2020 2020 2020 2020 2020  , ".            
+0000e460: 225c 6e5c 7463 6c69 656e 745f 6e61 6d65  "\n\tclient_name
+0000e470: 2053 5452 494e 4728 3136 2920 4e4f 5420   STRING(16) NOT 
+0000e480: 4e55 4c4c 220a 2020 2020 2020 2020 2020  NULL".          
+0000e490: 2020 225c 6e29 2050 5249 4d41 5259 204b    "\n) PRIMARY K
+0000e4a0: 4559 2028 7465 616d 5f69 642c 2063 6c69  EY (team_id, cli
+0000e4b0: 656e 745f 6964 292c 220a 2020 2020 2020  ent_id),".      
+0000e4c0: 2020 2020 2020 225c 6e49 4e54 4552 4c45        "\nINTERLE
+0000e4d0: 4156 4520 494e 2050 4152 454e 5420 7465  AVE IN PARENT te
+0000e4e0: 616d 5c6e 5c6e 220a 2020 2020 2020 2020  am\n\n".        
+0000e4f0: 290a 2020 2020 2020 2020 636c 6965 6e74  ).        client
+0000e500: 203d 2054 6162 6c65 280a 2020 2020 2020   = Table(.      
+0000e510: 2020 2020 2020 2263 6c69 656e 7422 2c0a        "client",.
+0000e520: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e530: 2e5f 6d65 7461 6461 7461 2c0a 2020 2020  ._metadata,.    
+0000e540: 2020 2020 2020 2020 436f 6c75 6d6e 2822          Column("
+0000e550: 7465 616d 5f69 6422 2c20 496e 7465 6765  team_id", Intege
+0000e560: 722c 2070 7269 6d61 7279 5f6b 6579 3d54  r, primary_key=T
+0000e570: 7275 6529 2c0a 2020 2020 2020 2020 2020  rue),.          
+0000e580: 2020 436f 6c75 6d6e 2822 636c 6965 6e74    Column("client
+0000e590: 5f69 6422 2c20 496e 7465 6765 722c 2070  _id", Integer, p
+0000e5a0: 7269 6d61 7279 5f6b 6579 3d54 7275 6529  rimary_key=True)
+0000e5b0: 2c0a 2020 2020 2020 2020 2020 2020 436f  ,.            Co
+0000e5c0: 6c75 6d6e 2822 636c 6965 6e74 5f6e 616d  lumn("client_nam
+0000e5d0: 6522 2c20 5374 7269 6e67 2831 3629 2c20  e", String(16), 
+0000e5e0: 6e75 6c6c 6162 6c65 3d46 616c 7365 292c  nullable=False),
+0000e5f0: 0a20 2020 2020 2020 2020 2020 2073 7061  .            spa
+0000e600: 6e6e 6572 5f69 6e74 6572 6c65 6176 655f  nner_interleave_
+0000e610: 696e 3d22 7465 616d 222c 0a20 2020 2020  in="team",.     
+0000e620: 2020 2029 0a20 2020 2020 2020 2077 6974     ).        wit
+0000e630: 6820 6d6f 636b 2e70 6174 6368 2822 676f  h mock.patch("go
+0000e640: 6f67 6c65 2e63 6c6f 7564 2e73 7061 6e6e  ogle.cloud.spann
+0000e650: 6572 5f64 6261 7069 2e63 7572 736f 722e  er_dbapi.cursor.
+0000e660: 4375 7273 6f72 2e65 7865 6375 7465 2229  Cursor.execute")
+0000e670: 2061 7320 6578 6563 7574 653a 0a20 2020   as execute:.   
+0000e680: 2020 2020 2020 2020 2063 6c69 656e 742e           client.
+0000e690: 6372 6561 7465 2873 656c 662e 5f65 6e67  create(self._eng
+0000e6a0: 696e 6529 0a20 2020 2020 2020 2020 2020  ine).           
+0000e6b0: 2065 7865 6375 7465 2e61 7373 6572 745f   execute.assert_
+0000e6c0: 6361 6c6c 6564 5f6f 6e63 655f 7769 7468  called_once_with
+0000e6d0: 2845 5850 5f51 5545 5259 2c20 5b5d 290a  (EXP_QUERY, []).
+0000e6e0: 0a20 2020 2064 6566 2074 6573 745f 696e  .    def test_in
+0000e6f0: 7465 726c 6561 7665 5f6f 6e5f 6465 6c65  terleave_on_dele
+0000e700: 7465 5f63 6173 6361 6465 2873 656c 6629  te_cascade(self)
+0000e710: 3a0a 2020 2020 2020 2020 4558 505f 5155  :.        EXP_QU
+0000e720: 4552 5920 3d20 280a 2020 2020 2020 2020  ERY = (.        
+0000e730: 2020 2020 225c 6e43 5245 4154 4520 5441      "\nCREATE TA
+0000e740: 424c 4520 636c 6965 6e74 2028 5c6e 5c74  BLE client (\n\t
+0000e750: 7465 616d 5f69 6420 494e 5436 3420 4e4f  team_id INT64 NO
+0000e760: 5420 4e55 4c4c 2c20 220a 2020 2020 2020  T NULL, ".      
+0000e770: 2020 2020 2020 225c 6e5c 7463 6c69 656e        "\n\tclien
+0000e780: 745f 6964 2049 4e54 3634 204e 4f54 204e  t_id INT64 NOT N
+0000e790: 554c 4c2c 2022 0a20 2020 2020 2020 2020  ULL, ".         
+0000e7a0: 2020 2022 5c6e 5c74 636c 6965 6e74 5f6e     "\n\tclient_n
+0000e7b0: 616d 6520 5354 5249 4e47 2831 3629 204e  ame STRING(16) N
+0000e7c0: 4f54 204e 554c 4c22 0a20 2020 2020 2020  OT NULL".       
+0000e7d0: 2020 2020 2022 5c6e 2920 5052 494d 4152       "\n) PRIMAR
+0000e7e0: 5920 4b45 5920 2874 6561 6d5f 6964 2c20  Y KEY (team_id, 
+0000e7f0: 636c 6965 6e74 5f69 6429 2c22 0a20 2020  client_id),".   
+0000e800: 2020 2020 2020 2020 2022 5c6e 494e 5445           "\nINTE
+0000e810: 524c 4541 5645 2049 4e20 5041 5245 4e54  RLEAVE IN PARENT
+0000e820: 2074 6561 6d20 4f4e 2044 454c 4554 4520   team ON DELETE 
+0000e830: 4341 5343 4144 455c 6e5c 6e22 0a20 2020  CASCADE\n\n".   
+0000e840: 2020 2020 2029 0a20 2020 2020 2020 2063       ).        c
+0000e850: 6c69 656e 7420 3d20 5461 626c 6528 0a20  lient = Table(. 
+0000e860: 2020 2020 2020 2020 2020 2022 636c 6965             "clie
+0000e870: 6e74 222c 0a20 2020 2020 2020 2020 2020  nt",.           
+0000e880: 2073 656c 662e 5f6d 6574 6164 6174 612c   self._metadata,
+0000e890: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
+0000e8a0: 756d 6e28 2274 6561 6d5f 6964 222c 2049  umn("team_id", I
+0000e8b0: 6e74 6567 6572 2c20 7072 696d 6172 795f  nteger, primary_
+0000e8c0: 6b65 793d 5472 7565 292c 0a20 2020 2020  key=True),.     
+0000e8d0: 2020 2020 2020 2043 6f6c 756d 6e28 2263         Column("c
+0000e8e0: 6c69 656e 745f 6964 222c 2049 6e74 6567  lient_id", Integ
+0000e8f0: 6572 2c20 7072 696d 6172 795f 6b65 793d  er, primary_key=
+0000e900: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
+0000e910: 2020 2043 6f6c 756d 6e28 2263 6c69 656e     Column("clien
+0000e920: 745f 6e61 6d65 222c 2053 7472 696e 6728  t_name", String(
+0000e930: 3136 292c 206e 756c 6c61 626c 653d 4661  16), nullable=Fa
+0000e940: 6c73 6529 2c0a 2020 2020 2020 2020 2020  lse),.          
+0000e950: 2020 7370 616e 6e65 725f 696e 7465 726c    spanner_interl
+0000e960: 6561 7665 5f69 6e3d 2274 6561 6d22 2c0a  eave_in="team",.
+0000e970: 2020 2020 2020 2020 2020 2020 7370 616e              span
+0000e980: 6e65 725f 696e 7465 726c 6561 7665 5f6f  ner_interleave_o
+0000e990: 6e5f 6465 6c65 7465 5f63 6173 6361 6465  n_delete_cascade
+0000e9a0: 3d54 7275 652c 0a20 2020 2020 2020 2029  =True,.        )
+0000e9b0: 0a20 2020 2020 2020 2077 6974 6820 6d6f  .        with mo
+0000e9c0: 636b 2e70 6174 6368 2822 676f 6f67 6c65  ck.patch("google
+0000e9d0: 2e63 6c6f 7564 2e73 7061 6e6e 6572 5f64  .cloud.spanner_d
+0000e9e0: 6261 7069 2e63 7572 736f 722e 4375 7273  bapi.cursor.Curs
+0000e9f0: 6f72 2e65 7865 6375 7465 2229 2061 7320  or.execute") as 
+0000ea00: 6578 6563 7574 653a 0a20 2020 2020 2020  execute:.       
+0000ea10: 2020 2020 2063 6c69 656e 742e 6372 6561       client.crea
+0000ea20: 7465 2873 656c 662e 5f65 6e67 696e 6529  te(self._engine)
+0000ea30: 0a20 2020 2020 2020 2020 2020 2065 7865  .            exe
+0000ea40: 6375 7465 2e61 7373 6572 745f 6361 6c6c  cute.assert_call
+0000ea50: 6564 5f6f 6e63 655f 7769 7468 2845 5850  ed_once_with(EXP
+0000ea60: 5f51 5545 5259 2c20 5b5d 290a 0a0a 636c  _QUERY, [])...cl
+0000ea70: 6173 7320 5573 6572 4167 656e 7454 6573  ass UserAgentTes
+0000ea80: 7428 6669 7874 7572 6573 2e54 6573 7442  t(fixtures.TestB
+0000ea90: 6173 6529 3a0a 2020 2020 2222 2243 6865  ase):.    """Che
+0000eaa0: 636b 2074 6861 7420 5351 4c41 6c63 6865  ck that SQLAlche
+0000eab0: 6d79 2064 6961 6c65 6374 2075 7365 7320  my dialect uses 
+0000eac0: 636f 7272 6563 7420 7573 6572 2061 6765  correct user age
+0000ead0: 6e74 2e22 2222 0a0a 2020 2020 6465 6620  nt."""..    def 
+0000eae0: 7365 7455 7028 7365 6c66 293a 0a20 2020  setUp(self):.   
+0000eaf0: 2020 2020 2073 656c 662e 5f65 6e67 696e       self._engin
+0000eb00: 6520 3d20 6372 6561 7465 5f65 6e67 696e  e = create_engin
+0000eb10: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
+0000eb20: 7370 616e 6e65 723a 2f2f 2f70 726f 6a65  spanner:///proje
+0000eb30: 6374 732f 6170 7064 6576 2d73 6f64 612d  cts/appdev-soda-
+0000eb40: 7370 616e 6e65 722d 7374 6167 696e 672f  spanner-staging/
+0000eb50: 696e 7374 616e 6365 732f 220a 2020 2020  instances/".    
+0000eb60: 2020 2020 2020 2020 2273 716c 616c 6368          "sqlalch
+0000eb70: 656d 792d 6469 616c 6563 742d 7465 7374  emy-dialect-test
+0000eb80: 2f64 6174 6162 6173 6573 2f63 6f6d 706c  /databases/compl
+0000eb90: 6961 6e63 652d 7465 7374 220a 2020 2020  iance-test".    
+0000eba0: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+0000ebb0: 6c66 2e5f 6d65 7461 6461 7461 203d 204d  lf._metadata = M
+0000ebc0: 6574 6144 6174 6128 6269 6e64 3d73 656c  etaData(bind=sel
+0000ebd0: 662e 5f65 6e67 696e 6529 0a0a 2020 2020  f._engine)..    
+0000ebe0: 6465 6620 7465 7374 5f75 7365 725f 6167  def test_user_ag
+0000ebf0: 656e 7428 7365 6c66 293a 0a20 2020 2020  ent(self):.     
+0000ec00: 2020 2064 6973 7420 3d20 706b 675f 7265     dist = pkg_re
+0000ec10: 736f 7572 6365 732e 6765 745f 6469 7374  sources.get_dist
+0000ec20: 7269 6275 7469 6f6e 2822 7371 6c61 6c63  ribution("sqlalc
+0000ec30: 6865 6d79 2d73 7061 6e6e 6572 2229 0a0a  hemy-spanner")..
+0000ec40: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+0000ec50: 662e 5f65 6e67 696e 652e 636f 6e6e 6563  f._engine.connec
+0000ec60: 7428 2920 6173 2063 6f6e 6e65 6374 696f  t() as connectio
+0000ec70: 6e3a 0a20 2020 2020 2020 2020 2020 2061  n:.            a
+0000ec80: 7373 6572 7420 280a 2020 2020 2020 2020  ssert (.        
+0000ec90: 2020 2020 2020 2020 636f 6e6e 6563 7469          connecti
+0000eca0: 6f6e 2e63 6f6e 6e65 6374 696f 6e2e 696e  on.connection.in
+0000ecb0: 7374 616e 6365 2e5f 636c 6965 6e74 2e5f  stance._client._
+0000ecc0: 636c 6965 6e74 5f69 6e66 6f2e 7573 6572  client_info.user
+0000ecd0: 5f61 6765 6e74 0a20 2020 2020 2020 2020  _agent.         
+0000ece0: 2020 2020 2020 203d 3d20 2267 6c2d 2220         == "gl-" 
+0000ecf0: 2b20 6469 7374 2e70 726f 6a65 6374 5f6e  + dist.project_n
+0000ed00: 616d 6520 2b20 222f 2220 2b20 6469 7374  ame + "/" + dist
+0000ed10: 2e76 6572 7369 6f6e 0a20 2020 2020 2020  .version.       
+0000ed20: 2020 2020 2029 0a0a 0a63 6c61 7373 2053       )...class S
+0000ed30: 696d 706c 6555 7064 6174 6544 656c 6574  impleUpdateDelet
+0000ed40: 6554 6573 7428 5f53 696d 706c 6555 7064  eTest(_SimpleUpd
+0000ed50: 6174 6544 656c 6574 6554 6573 7429 3a0a  ateDeleteTest):.
+0000ed60: 2020 2020 2222 220a 2020 2020 5350 414e      """.    SPAN
+0000ed70: 4e45 5220 4f56 4552 5249 4445 3a0a 0a20  NER OVERRIDE:.. 
+0000ed80: 2020 2053 7061 6e6e 6572 2064 6f65 736e     Spanner doesn
+0000ed90: 2774 2073 7570 706f 7274 2060 726f 7763  't support `rowc
+0000eda0: 6f75 6e74 6020 7072 6f70 6572 7479 2e20  ount` property. 
+0000edb0: 5468 6573 650a 2020 2020 7465 7374 2063  These.    test c
+0000edc0: 6173 6573 206f 7665 7272 6964 6573 206f  ases overrides o
+0000edd0: 6d69 7420 6072 6f77 636f 756e 7460 2063  mit `rowcount` c
+0000ede0: 6865 636b 732e 0a20 2020 2022 2222 0a0a  hecks..    """..
+0000edf0: 2020 2020 6465 6620 7465 7374 5f64 656c      def test_del
+0000ee00: 6574 6528 7365 6c66 2c20 636f 6e6e 6563  ete(self, connec
+0000ee10: 7469 6f6e 293a 0a20 2020 2020 2020 2074  tion):.        t
+0000ee20: 203d 2073 656c 662e 7461 626c 6573 2e70   = self.tables.p
+0000ee30: 6c61 696e 5f70 6b0a 2020 2020 2020 2020  lain_pk.        
+0000ee40: 7220 3d20 636f 6e6e 6563 7469 6f6e 2e65  r = connection.e
+0000ee50: 7865 6375 7465 2874 2e64 656c 6574 6528  xecute(t.delete(
+0000ee60: 292e 7768 6572 6528 742e 632e 6964 203d  ).where(t.c.id =
+0000ee70: 3d20 3229 290a 2020 2020 2020 2020 6173  = 2)).        as
+0000ee80: 7365 7274 206e 6f74 2072 2e69 735f 696e  sert not r.is_in
+0000ee90: 7365 7274 0a20 2020 2020 2020 2061 7373  sert.        ass
+0000eea0: 6572 7420 6e6f 7420 722e 7265 7475 726e  ert not r.return
+0000eeb0: 735f 726f 7773 0a20 2020 2020 2020 2065  s_rows.        e
+0000eec0: 715f 280a 2020 2020 2020 2020 2020 2020  q_(.            
+0000eed0: 636f 6e6e 6563 7469 6f6e 2e65 7865 6375  connection.execu
+0000eee0: 7465 2874 2e73 656c 6563 7428 292e 6f72  te(t.select().or
+0000eef0: 6465 725f 6279 2874 2e63 2e69 6429 292e  der_by(t.c.id)).
+0000ef00: 6665 7463 6861 6c6c 2829 2c0a 2020 2020  fetchall(),.    
+0000ef10: 2020 2020 2020 2020 5b28 312c 2022 6431          [(1, "d1
+0000ef20: 2229 2c20 2833 2c20 2264 3322 295d 2c0a  "), (3, "d3")],.
+0000ef30: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+0000ef40: 6566 2074 6573 745f 7570 6461 7465 2873  ef test_update(s
+0000ef50: 656c 662c 2063 6f6e 6e65 6374 696f 6e29  elf, connection)
+0000ef60: 3a0a 2020 2020 2020 2020 7420 3d20 7365  :.        t = se
+0000ef70: 6c66 2e74 6162 6c65 732e 706c 6169 6e5f  lf.tables.plain_
+0000ef80: 706b 0a20 2020 2020 2020 2072 203d 2063  pk.        r = c
+0000ef90: 6f6e 6e65 6374 696f 6e2e 6578 6563 7574  onnection.execut
+0000efa0: 6528 742e 7570 6461 7465 2829 2e77 6865  e(t.update().whe
+0000efb0: 7265 2874 2e63 2e69 6420 3d3d 2032 292c  re(t.c.id == 2),
+0000efc0: 2064 6963 7428 6461 7461 3d22 6432 5f6e   dict(data="d2_n
+0000efd0: 6577 2229 290a 2020 2020 2020 2020 6173  ew")).        as
+0000efe0: 7365 7274 206e 6f74 2072 2e69 735f 696e  sert not r.is_in
+0000eff0: 7365 7274 0a20 2020 2020 2020 2061 7373  sert.        ass
+0000f000: 6572 7420 6e6f 7420 722e 7265 7475 726e  ert not r.return
+0000f010: 735f 726f 7773 0a0a 2020 2020 2020 2020  s_rows..        
+0000f020: 6571 5f28 0a20 2020 2020 2020 2020 2020  eq_(.           
+0000f030: 2063 6f6e 6e65 6374 696f 6e2e 6578 6563   connection.exec
+0000f040: 7574 6528 742e 7365 6c65 6374 2829 2e6f  ute(t.select().o
+0000f050: 7264 6572 5f62 7928 742e 632e 6964 2929  rder_by(t.c.id))
+0000f060: 2e66 6574 6368 616c 6c28 292c 0a20 2020  .fetchall(),.   
+0000f070: 2020 2020 2020 2020 205b 2831 2c20 2264           [(1, "d
+0000f080: 3122 292c 2028 322c 2022 6432 5f6e 6577  1"), (2, "d2_new
+0000f090: 2229 2c20 2833 2c20 2264 3322 295d 2c0a  "), (3, "d3")],.
+0000f0a0: 2020 2020 2020 2020 290a 0a0a 636c 6173          )...clas
+0000f0b0: 7320 4861 7349 6e64 6578 5465 7374 285f  s HasIndexTest(_
+0000f0c0: 4861 7349 6e64 6578 5465 7374 293a 0a20  HasIndexTest):. 
+0000f0d0: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+0000f0e0: 2020 2020 6465 6620 6465 6669 6e65 5f74      def define_t
+0000f0f0: 6162 6c65 7328 636c 732c 206d 6574 6164  ables(cls, metad
+0000f100: 6174 6129 3a0a 2020 2020 2020 2020 7474  ata):.        tt
+0000f110: 203d 2054 6162 6c65 280a 2020 2020 2020   = Table(.      
+0000f120: 2020 2020 2020 2274 6573 745f 7461 626c        "test_tabl
+0000f130: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+0000f140: 6d65 7461 6461 7461 2c0a 2020 2020 2020  metadata,.      
+0000f150: 2020 2020 2020 436f 6c75 6d6e 2822 6964        Column("id
+0000f160: 222c 2049 6e74 6567 6572 2c20 7072 696d  ", Integer, prim
+0000f170: 6172 795f 6b65 793d 5472 7565 292c 0a20  ary_key=True),. 
+0000f180: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
+0000f190: 6e28 2264 6174 6122 2c20 5374 7269 6e67  n("data", String
+0000f1a0: 2835 3029 292c 0a20 2020 2020 2020 2029  (50)),.        )
+0000f1b0: 0a20 2020 2020 2020 2073 716c 616c 6368  .        sqlalch
+0000f1c0: 656d 792e 496e 6465 7828 226d 795f 6964  emy.Index("my_id
+0000f1d0: 7822 2c20 7474 2e63 2e64 6174 6129 0a0a  x", tt.c.data)..
+0000f1e0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+0000f1f0: 2e73 6b69 7028 224e 6f74 2073 7570 706f  .skip("Not suppo
+0000f200: 7274 6564 2062 7920 436c 6f75 6420 5370  rted by Cloud Sp
+0000f210: 616e 6e65 7222 290a 2020 2020 6465 6620  anner").    def 
+0000f220: 7465 7374 5f68 6173 5f69 6e64 6578 5f73  test_has_index_s
+0000f230: 6368 656d 6128 7365 6c66 293a 0a20 2020  chema(self):.   
+0000f240: 2020 2020 2070 6173 730a 0a0a 636c 6173       pass...clas
+0000f250: 7320 4861 7354 6162 6c65 5465 7374 285f  s HasTableTest(_
+0000f260: 4861 7354 6162 6c65 5465 7374 293a 0a20  HasTableTest):. 
+0000f270: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+0000f280: 2020 2020 6465 6620 6465 6669 6e65 5f74      def define_t
+0000f290: 6162 6c65 7328 636c 732c 206d 6574 6164  ables(cls, metad
+0000f2a0: 6174 6129 3a0a 2020 2020 2020 2020 5461  ata):.        Ta
+0000f2b0: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
+0000f2c0: 2022 7465 7374 5f74 6162 6c65 222c 0a20   "test_table",. 
+0000f2d0: 2020 2020 2020 2020 2020 206d 6574 6164             metad
+0000f2e0: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
+0000f2f0: 2043 6f6c 756d 6e28 2269 6422 2c20 496e   Column("id", In
+0000f300: 7465 6765 722c 2070 7269 6d61 7279 5f6b  teger, primary_k
+0000f310: 6579 3d54 7275 6529 2c0a 2020 2020 2020  ey=True),.      
+0000f320: 2020 2020 2020 436f 6c75 6d6e 2822 6461        Column("da
+0000f330: 7461 222c 2053 7472 696e 6728 3530 2929  ta", String(50))
+0000f340: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+0000f350: 2040 7079 7465 7374 2e6d 6172 6b2e 736b   @pytest.mark.sk
+0000f360: 6970 2822 4e6f 7420 7375 7070 6f72 7465  ip("Not supporte
+0000f370: 6420 6279 2043 6c6f 7564 2053 7061 6e6e  d by Cloud Spann
+0000f380: 6572 2229 0a20 2020 2064 6566 2074 6573  er").    def tes
+0000f390: 745f 6861 735f 7461 626c 655f 7363 6865  t_has_table_sche
+0000f3a0: 6d61 2873 656c 6629 3a0a 2020 2020 2020  ma(self):.      
+0000f3b0: 2020 7061 7373 0a0a 0a63 6c61 7373 2050    pass...class P
+0000f3c0: 6f73 7443 6f6d 7069 6c65 5061 7261 6d73  ostCompileParams
+0000f3d0: 5465 7374 285f 506f 7374 436f 6d70 696c  Test(_PostCompil
+0000f3e0: 6550 6172 616d 7354 6573 7429 3a0a 2020  eParamsTest):.  
+0000f3f0: 2020 6465 6620 7465 7374 5f65 7865 6375    def test_execu
+0000f400: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+0000f410: 2020 7461 626c 6520 3d20 7365 6c66 2e74    table = self.t
+0000f420: 6162 6c65 732e 736f 6d65 5f74 6162 6c65  ables.some_table
+0000f430: 0a0a 2020 2020 2020 2020 7374 6d74 203d  ..        stmt =
+0000f440: 2073 656c 6563 7428 7461 626c 652e 632e   select(table.c.
+0000f450: 6964 292e 7768 6572 6528 0a20 2020 2020  id).where(.     
+0000f460: 2020 2020 2020 2074 6162 6c65 2e63 2e78         table.c.x
+0000f470: 203d 3d20 7371 6c61 6c63 6865 6d79 2e62   == sqlalchemy.b
+0000f480: 696e 6470 6172 616d 2822 7122 2c20 6c69  indparam("q", li
+0000f490: 7465 7261 6c5f 6578 6563 7574 653d 5472  teral_execute=Tr
+0000f4a0: 7565 290a 2020 2020 2020 2020 290a 0a20  ue).        ).. 
+0000f4b0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+0000f4c0: 2e73 716c 5f65 7865 6375 7469 6f6e 5f61  .sql_execution_a
+0000f4d0: 7373 6572 7465 7228 2920 6173 2061 7373  sserter() as ass
+0000f4e0: 6572 7465 723a 0a20 2020 2020 2020 2020  erter:.         
+0000f4f0: 2020 2077 6974 6820 636f 6e66 6967 2e64     with config.d
+0000f500: 622e 636f 6e6e 6563 7428 2920 6173 2063  b.connect() as c
+0000f510: 6f6e 6e3a 0a20 2020 2020 2020 2020 2020  onn:.           
+0000f520: 2020 2020 2063 6f6e 6e2e 6578 6563 7574       conn.execut
+0000f530: 6528 7374 6d74 2c20 6469 6374 2871 3d31  e(stmt, dict(q=1
+0000f540: 3029 290a 0a20 2020 2020 2020 2061 7373  0))..        ass
+0000f550: 6572 7465 722e 6173 7365 7274 5f28 0a20  erter.assert_(. 
+0000f560: 2020 2020 2020 2020 2020 2073 716c 616c             sqlal
+0000f570: 6368 656d 792e 7465 7374 696e 672e 6173  chemy.testing.as
+0000f580: 7365 7274 7371 6c2e 4375 7273 6f72 5351  sertsql.CursorSQ
+0000f590: 4c28 0a20 2020 2020 2020 2020 2020 2020  L(.             
+0000f5a0: 2020 2022 5345 4c45 4354 2073 6f6d 655f     "SELECT some_
+0000f5b0: 7461 626c 652e 6964 205c 6e46 524f 4d20  table.id \nFROM 
+0000f5c0: 736f 6d65 5f74 6162 6c65 2022 2022 5c6e  some_table " "\n
+0000f5d0: 5748 4552 4520 736f 6d65 5f74 6162 6c65  WHERE some_table
+0000f5e0: 2e78 203d 2031 3022 2c0a 2020 2020 2020  .x = 10",.      
+0000f5f0: 2020 2020 2020 2020 2020 5b5d 2069 6620            [] if 
+0000f600: 636f 6e66 6967 2e64 622e 6469 616c 6563  config.db.dialec
+0000f610: 742e 706f 7369 7469 6f6e 616c 2065 6c73  t.positional els
+0000f620: 6520 7b7d 2c0a 2020 2020 2020 2020 2020  e {},.          
+0000f630: 2020 290a 2020 2020 2020 2020 290a 0a20    ).        ).. 
+0000f640: 2020 2064 6566 2074 6573 745f 6578 6563     def test_exec
+0000f650: 7574 655f 6578 7061 6e64 696e 675f 706c  ute_expanding_pl
+0000f660: 7573 5f6c 6974 6572 616c 5f65 7865 6375  us_literal_execu
+0000f670: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+0000f680: 2020 7461 626c 6520 3d20 7365 6c66 2e74    table = self.t
+0000f690: 6162 6c65 732e 736f 6d65 5f74 6162 6c65  ables.some_table
+0000f6a0: 0a0a 2020 2020 2020 2020 7374 6d74 203d  ..        stmt =
+0000f6b0: 2073 656c 6563 7428 7461 626c 652e 632e   select(table.c.
+0000f6c0: 6964 292e 7768 6572 6528 0a20 2020 2020  id).where(.     
+0000f6d0: 2020 2020 2020 2074 6162 6c65 2e63 2e78         table.c.x
+0000f6e0: 2e69 6e5f 280a 2020 2020 2020 2020 2020  .in_(.          
+0000f6f0: 2020 2020 2020 7371 6c61 6c63 6865 6d79        sqlalchemy
+0000f700: 2e62 696e 6470 6172 616d 2822 7122 2c20  .bindparam("q", 
+0000f710: 6578 7061 6e64 696e 673d 5472 7565 2c20  expanding=True, 
+0000f720: 6c69 7465 7261 6c5f 6578 6563 7574 653d  literal_execute=
+0000f730: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+0000f740: 2020 290a 2020 2020 2020 2020 290a 0a20    ).        ).. 
+0000f750: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+0000f760: 2e73 716c 5f65 7865 6375 7469 6f6e 5f61  .sql_execution_a
+0000f770: 7373 6572 7465 7228 2920 6173 2061 7373  sserter() as ass
+0000f780: 6572 7465 723a 0a20 2020 2020 2020 2020  erter:.         
+0000f790: 2020 2077 6974 6820 636f 6e66 6967 2e64     with config.d
+0000f7a0: 622e 636f 6e6e 6563 7428 2920 6173 2063  b.connect() as c
+0000f7b0: 6f6e 6e3a 0a20 2020 2020 2020 2020 2020  onn:.           
+0000f7c0: 2020 2020 2063 6f6e 6e2e 6578 6563 7574       conn.execut
+0000f7d0: 6528 7374 6d74 2c20 6469 6374 2871 3d5b  e(stmt, dict(q=[
+0000f7e0: 352c 2036 2c20 375d 2929 0a0a 2020 2020  5, 6, 7]))..    
+0000f7f0: 2020 2020 6173 7365 7274 6572 2e61 7373      asserter.ass
+0000f800: 6572 745f 280a 2020 2020 2020 2020 2020  ert_(.          
+0000f810: 2020 7371 6c61 6c63 6865 6d79 2e74 6573    sqlalchemy.tes
+0000f820: 7469 6e67 2e61 7373 6572 7473 716c 2e43  ting.assertsql.C
+0000f830: 7572 736f 7253 514c 280a 2020 2020 2020  ursorSQL(.      
+0000f840: 2020 2020 2020 2020 2020 2253 454c 4543            "SELEC
+0000f850: 5420 736f 6d65 5f74 6162 6c65 2e69 6420  T some_table.id 
+0000f860: 5c6e 4652 4f4d 2073 6f6d 655f 7461 626c  \nFROM some_tabl
+0000f870: 6520 220a 2020 2020 2020 2020 2020 2020  e ".            
+0000f880: 2020 2020 225c 6e57 4845 5245 2073 6f6d      "\nWHERE som
+0000f890: 655f 7461 626c 652e 7820 494e 2028 352c  e_table.x IN (5,
+0000f8a0: 2036 2c20 3729 222c 0a20 2020 2020 2020   6, 7)",.       
+0000f8b0: 2020 2020 2020 2020 205b 5d20 6966 2063           [] if c
+0000f8c0: 6f6e 6669 672e 6462 2e64 6961 6c65 6374  onfig.db.dialect
+0000f8d0: 2e70 6f73 6974 696f 6e61 6c20 656c 7365  .positional else
+0000f8e0: 207b 7d2c 0a20 2020 2020 2020 2020 2020   {},.           
+0000f8f0: 2029 0a20 2020 2020 2020 2029 0a0a 2020   ).        )..  
+0000f900: 2020 4074 6573 7469 6e67 2e72 6571 7569    @testing.requi
+0000f910: 7265 732e 7475 706c 655f 696e 0a20 2020  res.tuple_in.   
+0000f920: 2064 6566 2074 6573 745f 6578 6563 7574   def test_execut
+0000f930: 655f 7475 706c 655f 6578 7061 6e64 696e  e_tuple_expandin
+0000f940: 675f 706c 7573 5f6c 6974 6572 616c 5f65  g_plus_literal_e
+0000f950: 7865 6375 7465 2873 656c 6629 3a0a 2020  xecute(self):.  
+0000f960: 2020 2020 2020 7461 626c 6520 3d20 7365        table = se
+0000f970: 6c66 2e74 6162 6c65 732e 736f 6d65 5f74  lf.tables.some_t
+0000f980: 6162 6c65 0a0a 2020 2020 2020 2020 7374  able..        st
+0000f990: 6d74 203d 2073 656c 6563 7428 7461 626c  mt = select(tabl
+0000f9a0: 652e 632e 6964 292e 7768 6572 6528 0a20  e.c.id).where(. 
+0000f9b0: 2020 2020 2020 2020 2020 2073 716c 616c             sqlal
+0000f9c0: 6368 656d 792e 7475 706c 655f 2874 6162  chemy.tuple_(tab
+0000f9d0: 6c65 2e63 2e78 2c20 7461 626c 652e 632e  le.c.x, table.c.
+0000f9e0: 7929 2e69 6e5f 280a 2020 2020 2020 2020  y).in_(.        
+0000f9f0: 2020 2020 2020 2020 7371 6c61 6c63 6865          sqlalche
+0000fa00: 6d79 2e62 696e 6470 6172 616d 2822 7122  my.bindparam("q"
+0000fa10: 2c20 6578 7061 6e64 696e 673d 5472 7565  , expanding=True
+0000fa20: 2c20 6c69 7465 7261 6c5f 6578 6563 7574  , literal_execut
+0000fa30: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
+0000fa40: 2020 2020 290a 2020 2020 2020 2020 290a      ).        ).
+0000fa50: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+0000fa60: 6c66 2e73 716c 5f65 7865 6375 7469 6f6e  lf.sql_execution
+0000fa70: 5f61 7373 6572 7465 7228 2920 6173 2061  _asserter() as a
+0000fa80: 7373 6572 7465 723a 0a20 2020 2020 2020  sserter:.       
+0000fa90: 2020 2020 2077 6974 6820 636f 6e66 6967       with config
+0000faa0: 2e64 622e 636f 6e6e 6563 7428 2920 6173  .db.connect() as
+0000fab0: 2063 6f6e 6e3a 0a20 2020 2020 2020 2020   conn:.         
+0000fac0: 2020 2020 2020 2063 6f6e 6e2e 6578 6563         conn.exec
+0000fad0: 7574 6528 7374 6d74 2c20 6469 6374 2871  ute(stmt, dict(q
+0000fae0: 3d5b 2835 2c20 3130 292c 2028 3132 2c20  =[(5, 10), (12, 
+0000faf0: 3138 295d 2929 0a0a 2020 2020 2020 2020  18)]))..        
+0000fb00: 6173 7365 7274 6572 2e61 7373 6572 745f  asserter.assert_
+0000fb10: 280a 2020 2020 2020 2020 2020 2020 7371  (.            sq
+0000fb20: 6c61 6c63 6865 6d79 2e74 6573 7469 6e67  lalchemy.testing
+0000fb30: 2e61 7373 6572 7473 716c 2e43 7572 736f  .assertsql.Curso
+0000fb40: 7253 514c 280a 2020 2020 2020 2020 2020  rSQL(.          
+0000fb50: 2020 2020 2020 2253 454c 4543 5420 736f        "SELECT so
+0000fb60: 6d65 5f74 6162 6c65 2e69 6420 5c6e 4652  me_table.id \nFR
+0000fb70: 4f4d 2073 6f6d 655f 7461 626c 6520 220a  OM some_table ".
+0000fb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb90: 225c 6e57 4845 5245 2028 736f 6d65 5f74  "\nWHERE (some_t
+0000fba0: 6162 6c65 2e78 2c20 736f 6d65 5f74 6162  able.x, some_tab
+0000fbb0: 6c65 2e79 2920 220a 2020 2020 2020 2020  le.y) ".        
+0000fbc0: 2020 2020 2020 2020 2249 4e20 2825 7328          "IN (%s(
+0000fbd0: 352c 2031 3029 2c20 2831 322c 2031 3829  5, 10), (12, 18)
+0000fbe0: 2922 0a20 2020 2020 2020 2020 2020 2020  )".             
+0000fbf0: 2020 2025 2028 2256 414c 5545 5320 2220     % ("VALUES " 
+0000fc00: 6966 2063 6f6e 6669 672e 6462 2e64 6961  if config.db.dia
+0000fc10: 6c65 6374 2e74 7570 6c65 5f69 6e5f 7661  lect.tuple_in_va
+0000fc20: 6c75 6573 2065 6c73 6520 2222 292c 0a20  lues else ""),. 
+0000fc30: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+0000fc40: 2920 6966 2063 6f6e 6669 672e 6462 2e64  ) if config.db.d
+0000fc50: 6961 6c65 6374 2e70 6f73 6974 696f 6e61  ialect.positiona
+0000fc60: 6c20 656c 7365 207b 7d2c 0a20 2020 2020  l else {},.     
+0000fc70: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000fc80: 2029 0a0a 2020 2020 4074 6573 7469 6e67   )..    @testing
+0000fc90: 2e72 6571 7569 7265 732e 7475 706c 655f  .requires.tuple_
+0000fca0: 696e 0a20 2020 2064 6566 2074 6573 745f  in.    def test_
+0000fcb0: 6578 6563 7574 655f 7475 706c 655f 6578  execute_tuple_ex
+0000fcc0: 7061 6e64 696e 675f 706c 7573 5f6c 6974  panding_plus_lit
+0000fcd0: 6572 616c 5f68 6574 6572 6f67 656e 656f  eral_heterogeneo
+0000fce0: 7573 5f65 7865 6375 7465 2873 656c 6629  us_execute(self)
+0000fcf0: 3a0a 2020 2020 2020 2020 7461 626c 6520  :.        table 
+0000fd00: 3d20 7365 6c66 2e74 6162 6c65 732e 736f  = self.tables.so
+0000fd10: 6d65 5f74 6162 6c65 0a0a 2020 2020 2020  me_table..      
+0000fd20: 2020 7374 6d74 203d 2073 656c 6563 7428    stmt = select(
+0000fd30: 7461 626c 652e 632e 6964 292e 7768 6572  table.c.id).wher
+0000fd40: 6528 0a20 2020 2020 2020 2020 2020 2073  e(.            s
+0000fd50: 716c 616c 6368 656d 792e 7475 706c 655f  qlalchemy.tuple_
+0000fd60: 2874 6162 6c65 2e63 2e78 2c20 7461 626c  (table.c.x, tabl
+0000fd70: 652e 632e 7a29 2e69 6e5f 280a 2020 2020  e.c.z).in_(.    
+0000fd80: 2020 2020 2020 2020 2020 2020 7371 6c61              sqla
+0000fd90: 6c63 6865 6d79 2e62 696e 6470 6172 616d  lchemy.bindparam
+0000fda0: 2822 7122 2c20 6578 7061 6e64 696e 673d  ("q", expanding=
+0000fdb0: 5472 7565 2c20 6c69 7465 7261 6c5f 6578  True, literal_ex
+0000fdc0: 6563 7574 653d 5472 7565 290a 2020 2020  ecute=True).    
+0000fdd0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000fde0: 2020 290a 0a20 2020 2020 2020 2077 6974    )..        wit
+0000fdf0: 6820 7365 6c66 2e73 716c 5f65 7865 6375  h self.sql_execu
+0000fe00: 7469 6f6e 5f61 7373 6572 7465 7228 2920  tion_asserter() 
+0000fe10: 6173 2061 7373 6572 7465 723a 0a20 2020  as asserter:.   
+0000fe20: 2020 2020 2020 2020 2077 6974 6820 636f           with co
+0000fe30: 6e66 6967 2e64 622e 636f 6e6e 6563 7428  nfig.db.connect(
+0000fe40: 2920 6173 2063 6f6e 6e3a 0a20 2020 2020  ) as conn:.     
+0000fe50: 2020 2020 2020 2020 2020 2063 6f6e 6e2e             conn.
+0000fe60: 6578 6563 7574 6528 7374 6d74 2c20 6469  execute(stmt, di
+0000fe70: 6374 2871 3d5b 2835 2c20 227a 3122 292c  ct(q=[(5, "z1"),
+0000fe80: 2028 3132 2c20 227a 3322 295d 2929 0a0a   (12, "z3")]))..
+0000fe90: 2020 2020 2020 2020 6173 7365 7274 6572          asserter
+0000fea0: 2e61 7373 6572 745f 280a 2020 2020 2020  .assert_(.      
+0000feb0: 2020 2020 2020 7371 6c61 6c63 6865 6d79        sqlalchemy
+0000fec0: 2e74 6573 7469 6e67 2e61 7373 6572 7473  .testing.asserts
+0000fed0: 716c 2e43 7572 736f 7253 514c 280a 2020  ql.CursorSQL(.  
+0000fee0: 2020 2020 2020 2020 2020 2020 2020 2253                "S
+0000fef0: 454c 4543 5420 736f 6d65 5f74 6162 6c65  ELECT some_table
+0000ff00: 2e69 6420 5c6e 4652 4f4d 2073 6f6d 655f  .id \nFROM some_
+0000ff10: 7461 626c 6520 220a 2020 2020 2020 2020  table ".        
+0000ff20: 2020 2020 2020 2020 225c 6e57 4845 5245          "\nWHERE
+0000ff30: 2028 736f 6d65 5f74 6162 6c65 2e78 2c20   (some_table.x, 
+0000ff40: 736f 6d65 5f74 6162 6c65 2e7a 2920 220a  some_table.z) ".
+0000ff50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff60: 2249 4e20 2825 7328 352c 2027 7a31 2729  "IN (%s(5, 'z1')
+0000ff70: 2c20 2831 322c 2027 7a33 2729 2922 0a20  , (12, 'z3'))". 
+0000ff80: 2020 2020 2020 2020 2020 2020 2020 2025                 %
+0000ff90: 2028 2256 414c 5545 5320 2220 6966 2063   ("VALUES " if c
+0000ffa0: 6f6e 6669 672e 6462 2e64 6961 6c65 6374  onfig.db.dialect
+0000ffb0: 2e74 7570 6c65 5f69 6e5f 7661 6c75 6573  .tuple_in_values
+0000ffc0: 2065 6c73 6520 2222 292c 0a20 2020 2020   else ""),.     
+0000ffd0: 2020 2020 2020 2020 2020 2028 2920 6966             () if
+0000ffe0: 2063 6f6e 6669 672e 6462 2e64 6961 6c65   config.db.diale
+0000fff0: 6374 2e70 6f73 6974 696f 6e61 6c20 656c  ct.positional el
+00010000: 7365 207b 7d2c 0a20 2020 2020 2020 2020  se {},.         
+00010010: 2020 2029 0a20 2020 2020 2020 2029 0a0a     ).        )..
+00010020: 0a63 6c61 7373 2043 6f6d 7075 7465 6452  .class ComputedR
+00010030: 6566 6c65 6374 696f 6e46 6978 7475 7265  eflectionFixture
+00010040: 5465 7374 285f 436f 6d70 7574 6564 5265  Test(_ComputedRe
+00010050: 666c 6563 7469 6f6e 4669 7874 7572 6554  flectionFixtureT
+00010060: 6573 7429 3a0a 2020 2020 4063 6c61 7373  est):.    @class
+00010070: 6d65 7468 6f64 0a20 2020 2064 6566 2064  method.    def d
+00010080: 6566 696e 655f 7461 626c 6573 2863 6c73  efine_tables(cls
+00010090: 2c20 6d65 7461 6461 7461 293a 0a20 2020  , metadata):.   
+000100a0: 2020 2020 2022 2222 5350 414e 4e45 5220       """SPANNER 
+000100b0: 4f56 4552 5249 4445 3a0a 0a20 2020 2020  OVERRIDE:..     
+000100c0: 2020 2041 766f 6964 2075 7369 6e67 2064     Avoid using d
+000100d0: 6566 6175 6c74 2076 616c 7565 7320 666f  efault values fo
+000100e0: 7220 636f 6d70 7574 6564 2063 6f6c 756d  r computed colum
+000100f0: 6e73 2e0a 2020 2020 2020 2020 2222 220a  ns..        """.
+00010100: 2020 2020 2020 2020 5461 626c 6528 0a20          Table(. 
+00010110: 2020 2020 2020 2020 2020 2022 636f 6d70             "comp
+00010120: 7574 6564 5f64 6566 6175 6c74 5f74 6162  uted_default_tab
+00010130: 6c65 222c 0a20 2020 2020 2020 2020 2020  le",.           
+00010140: 206d 6574 6164 6174 612c 0a20 2020 2020   metadata,.     
+00010150: 2020 2020 2020 2043 6f6c 756d 6e28 2269         Column("i
+00010160: 6422 2c20 496e 7465 6765 722c 2070 7269  d", Integer, pri
+00010170: 6d61 7279 5f6b 6579 3d54 7275 6529 2c0a  mary_key=True),.
+00010180: 2020 2020 2020 2020 2020 2020 436f 6c75              Colu
+00010190: 6d6e 2822 6e6f 726d 616c 222c 2049 6e74  mn("normal", Int
+000101a0: 6567 6572 292c 0a20 2020 2020 2020 2020  eger),.         
+000101b0: 2020 2043 6f6c 756d 6e28 2263 6f6d 7075     Column("compu
+000101c0: 7465 645f 636f 6c22 2c20 496e 7465 6765  ted_col", Intege
+000101d0: 722c 2043 6f6d 7075 7465 6428 226e 6f72  r, Computed("nor
+000101e0: 6d61 6c20 2b20 3432 2229 292c 0a20 2020  mal + 42")),.   
+000101f0: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
+00010200: 2277 6974 685f 6465 6661 756c 7422 2c20  "with_default", 
+00010210: 496e 7465 6765 7229 2c0a 2020 2020 2020  Integer),.      
+00010220: 2020 290a 0a20 2020 2020 2020 2074 203d    )..        t =
+00010230: 2054 6162 6c65 280a 2020 2020 2020 2020   Table(.        
+00010240: 2020 2020 2263 6f6d 7075 7465 645f 636f      "computed_co
+00010250: 6c75 6d6e 5f74 6162 6c65 222c 0a20 2020  lumn_table",.   
+00010260: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
+00010270: 612c 0a20 2020 2020 2020 2020 2020 2043  a,.            C
+00010280: 6f6c 756d 6e28 2269 6422 2c20 496e 7465  olumn("id", Inte
+00010290: 6765 722c 2070 7269 6d61 7279 5f6b 6579  ger, primary_key
+000102a0: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
+000102b0: 2020 2020 436f 6c75 6d6e 2822 6e6f 726d      Column("norm
+000102c0: 616c 222c 2049 6e74 6567 6572 292c 0a20  al", Integer),. 
+000102d0: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
+000102e0: 6e28 2263 6f6d 7075 7465 645f 6e6f 5f66  n("computed_no_f
+000102f0: 6c61 6722 2c20 496e 7465 6765 722c 2043  lag", Integer, C
+00010300: 6f6d 7075 7465 6428 226e 6f72 6d61 6c20  omputed("normal 
+00010310: 2b20 3432 2229 292c 0a20 2020 2020 2020  + 42")),.       
+00010320: 2029 0a0a 2020 2020 2020 2020 6966 2074   )..        if t
+00010330: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
+00010340: 636f 6d70 7574 6564 5f63 6f6c 756d 6e73  computed_columns
+00010350: 5f76 6972 7475 616c 2e65 6e61 626c 6564  _virtual.enabled
+00010360: 3a0a 2020 2020 2020 2020 2020 2020 742e  :.            t.
+00010370: 6170 7065 6e64 5f63 6f6c 756d 6e28 0a20  append_column(. 
+00010380: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+00010390: 6f6c 756d 6e28 0a20 2020 2020 2020 2020  olumn(.         
+000103a0: 2020 2020 2020 2020 2020 2022 636f 6d70             "comp
+000103b0: 7574 6564 5f76 6972 7475 616c 222c 0a20  uted_virtual",. 
+000103c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103d0: 2020 2049 6e74 6567 6572 2c0a 2020 2020     Integer,.    
+000103e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103f0: 436f 6d70 7574 6564 2822 6e6f 726d 616c  Computed("normal
+00010400: 202b 2032 222c 2070 6572 7369 7374 6564   + 2", persisted
+00010410: 3d46 616c 7365 292c 0a20 2020 2020 2020  =False),.       
+00010420: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00010430: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00010440: 2069 6620 7465 7374 696e 672e 7265 7175   if testing.requ
+00010450: 6972 6573 2e63 6f6d 7075 7465 645f 636f  ires.computed_co
+00010460: 6c75 6d6e 735f 7374 6f72 6564 2e65 6e61  lumns_stored.ena
+00010470: 626c 6564 3a0a 2020 2020 2020 2020 2020  bled:.          
+00010480: 2020 742e 6170 7065 6e64 5f63 6f6c 756d    t.append_colum
+00010490: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+000104a0: 2020 2043 6f6c 756d 6e28 0a20 2020 2020     Column(.     
+000104b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000104c0: 636f 6d70 7574 6564 5f73 746f 7265 6422  computed_stored"
+000104d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000104e0: 2020 2020 2020 496e 7465 6765 722c 0a20        Integer,. 
+000104f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010500: 2020 2043 6f6d 7075 7465 6428 226e 6f72     Computed("nor
+00010510: 6d61 6c20 2d20 3432 222c 2070 6572 7369  mal - 42", persi
+00010520: 7374 6564 3d54 7275 6529 2c0a 2020 2020  sted=True),.    
+00010530: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00010540: 2020 2020 2020 2020 2020 290a 0a0a 636c            )...cl
+00010550: 6173 7320 436f 6d70 7574 6564 5265 666c  ass ComputedRefl
+00010560: 6563 7469 6f6e 5465 7374 285f 436f 6d70  ectionTest(_Comp
+00010570: 7574 6564 5265 666c 6563 7469 6f6e 5465  utedReflectionTe
+00010580: 7374 2c20 436f 6d70 7574 6564 5265 666c  st, ComputedRefl
+00010590: 6563 7469 6f6e 4669 7874 7572 6554 6573  ectionFixtureTes
+000105a0: 7429 3a0a 2020 2020 4074 6573 7469 6e67  t):.    @testing
+000105b0: 2e72 6571 7569 7265 732e 7363 6865 6d61  .requires.schema
+000105c0: 730a 2020 2020 6465 6620 7465 7374 5f67  s.    def test_g
+000105d0: 6574 5f63 6f6c 756d 6e5f 7265 7475 726e  et_column_return
+000105e0: 735f 7065 7273 6973 7465 645f 7769 7468  s_persisted_with
+000105f0: 5f73 6368 656d 6128 7365 6c66 293a 0a20  _schema(self):. 
+00010600: 2020 2020 2020 2069 6e73 7020 3d20 696e         insp = in
+00010610: 7370 6563 7428 636f 6e66 6967 2e64 6229  spect(config.db)
+00010620: 0a0a 2020 2020 2020 2020 636f 6c73 203d  ..        cols =
+00010630: 2069 6e73 702e 6765 745f 636f 6c75 6d6e   insp.get_column
+00010640: 7328 2263 6f6d 7075 7465 645f 636f 6c75  s("computed_colu
+00010650: 6d6e 5f74 6162 6c65 222c 2073 6368 656d  mn_table", schem
+00010660: 613d 636f 6e66 6967 2e74 6573 745f 7363  a=config.test_sc
+00010670: 6865 6d61 290a 2020 2020 2020 2020 6461  hema).        da
+00010680: 7461 203d 207b 635b 226e 616d 6522 5d3a  ta = {c["name"]:
+00010690: 2063 2066 6f72 2063 2069 6e20 636f 6c73   c for c in cols
+000106a0: 7d0a 0a20 2020 2020 2020 2073 656c 662e  }..        self.
+000106b0: 6368 6563 6b5f 636f 6c75 6d6e 280a 2020  check_column(.  
+000106c0: 2020 2020 2020 2020 2020 6461 7461 2c0a            data,.
+000106d0: 2020 2020 2020 2020 2020 2020 2263 6f6d              "com
+000106e0: 7075 7465 645f 6e6f 5f66 6c61 6722 2c0a  puted_no_flag",.
+000106f0: 2020 2020 2020 2020 2020 2020 226e 6f72              "nor
+00010700: 6d61 6c2b 3432 222c 0a20 2020 2020 2020  mal+42",.       
+00010710: 2020 2020 2074 6573 7469 6e67 2e72 6571       testing.req
+00010720: 7569 7265 732e 636f 6d70 7574 6564 5f63  uires.computed_c
+00010730: 6f6c 756d 6e73 5f64 6566 6175 6c74 5f70  olumns_default_p
+00010740: 6572 7369 7374 6564 2e65 6e61 626c 6564  ersisted.enabled
+00010750: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00010760: 2020 2020 6966 2074 6573 7469 6e67 2e72      if testing.r
+00010770: 6571 7569 7265 732e 636f 6d70 7574 6564  equires.computed
+00010780: 5f63 6f6c 756d 6e73 5f76 6972 7475 616c  _columns_virtual
+00010790: 2e65 6e61 626c 6564 3a0a 2020 2020 2020  .enabled:.      
+000107a0: 2020 2020 2020 7365 6c66 2e63 6865 636b        self.check
+000107b0: 5f63 6f6c 756d 6e28 0a20 2020 2020 2020  _column(.       
+000107c0: 2020 2020 2020 2020 2064 6174 612c 0a20           data,. 
+000107d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000107e0: 636f 6d70 7574 6564 5f76 6972 7475 616c  computed_virtual
+000107f0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00010800: 2020 2022 6e6f 726d 616c 2f32 222c 0a20     "normal/2",. 
+00010810: 2020 2020 2020 2020 2020 2020 2020 2046                 F
+00010820: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+00010830: 2020 290a 2020 2020 2020 2020 6966 2074    ).        if t
+00010840: 6573 7469 6e67 2e72 6571 7569 7265 732e  esting.requires.
+00010850: 636f 6d70 7574 6564 5f63 6f6c 756d 6e73  computed_columns
+00010860: 5f73 746f 7265 642e 656e 6162 6c65 643a  _stored.enabled:
+00010870: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00010880: 662e 6368 6563 6b5f 636f 6c75 6d6e 280a  f.check_column(.
+00010890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108a0: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
+000108b0: 2020 2020 2020 2263 6f6d 7075 7465 645f        "computed_
+000108c0: 7374 6f72 6564 222c 0a20 2020 2020 2020  stored",.       
+000108d0: 2020 2020 2020 2020 2022 6e6f 726d 616c           "normal
+000108e0: 2d34 3222 2c0a 2020 2020 2020 2020 2020  -42",.          
+000108f0: 2020 2020 2020 5472 7565 2c0a 2020 2020        True,.    
+00010900: 2020 2020 2020 2020 290a 0a20 2020 2040          )..    @
+00010910: 7079 7465 7374 2e6d 6172 6b2e 736b 6970  pytest.mark.skip
+00010920: 2822 4465 6661 756c 7420 7661 6c75 6573  ("Default values
+00010930: 2061 7265 206e 6f74 2073 7570 706f 7274   are not support
+00010940: 6564 2e22 290a 2020 2020 6465 6620 7465  ed.").    def te
+00010950: 7374 5f63 6f6d 7075 7465 645f 636f 6c5f  st_computed_col_
+00010960: 6465 6661 756c 745f 6e6f 745f 7365 7428  default_not_set(
+00010970: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+00010980: 6173 730a 0a20 2020 2064 6566 2074 6573  ass..    def tes
+00010990: 745f 6765 745f 636f 6c75 6d6e 5f72 6574  t_get_column_ret
+000109a0: 7572 6e73 5f63 6f6d 7075 7465 6428 7365  urns_computed(se
+000109b0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+000109c0: 0a20 2020 2020 2020 2053 5041 4e4e 4552  .        SPANNER
+000109d0: 204f 5645 5252 4944 453a 0a0a 2020 2020   OVERRIDE:..    
+000109e0: 2020 2020 496e 2053 7061 6e6e 6572 2061      In Spanner a
+000109f0: 6c6c 2074 6865 2067 656e 6572 6174 6564  ll the generated
+00010a00: 2063 6f6c 756d 6e73 2061 7265 2053 544f   columns are STO
+00010a10: 5245 442c 0a20 2020 2020 2020 206d 6561  RED,.        mea
+00010a20: 6e69 6e67 2074 6865 7265 2061 7265 206e  ning there are n
+00010a30: 6f20 7065 7273 6973 7465 6420 616e 6420  o persisted and 
+00010a40: 6e6f 7420 7065 7273 6973 7465 640a 2020  not persisted.  
+00010a50: 2020 2020 2020 2869 6e20 7468 6520 7465        (in the te
+00010a60: 726d 7320 6f66 2074 6865 2053 514c 416c  rms of the SQLAl
+00010a70: 6368 656d 7929 2063 6f6c 756d 6e73 2e20  chemy) columns. 
+00010a80: 5468 650a 2020 2020 2020 2020 6d65 7468  The.        meth
+00010a90: 6f64 206f 7665 7272 6964 6520 6f6d 6974  od override omit
+00010aa0: 7320 7468 6520 7065 7273 6973 7465 6e63  s the persistenc
+00010ab0: 6520 7265 666c 6563 7469 6f6e 2063 6865  e reflection che
+00010ac0: 636b 732e 0a20 2020 2020 2020 2022 2222  cks..        """
+00010ad0: 0a20 2020 2020 2020 2069 6e73 7020 3d20  .        insp = 
+00010ae0: 696e 7370 6563 7428 636f 6e66 6967 2e64  inspect(config.d
+00010af0: 6229 0a0a 2020 2020 2020 2020 636f 6c73  b)..        cols
+00010b00: 203d 2069 6e73 702e 6765 745f 636f 6c75   = insp.get_colu
+00010b10: 6d6e 7328 2263 6f6d 7075 7465 645f 6465  mns("computed_de
+00010b20: 6661 756c 745f 7461 626c 6522 290a 2020  fault_table").  
+00010b30: 2020 2020 2020 6461 7461 203d 207b 635b        data = {c[
+00010b40: 226e 616d 6522 5d3a 2063 2066 6f72 2063  "name"]: c for c
+00010b50: 2069 6e20 636f 6c73 7d0a 2020 2020 2020   in cols}.      
+00010b60: 2020 666f 7220 6b65 7920 696e 2028 2269    for key in ("i
+00010b70: 6422 2c20 226e 6f72 6d61 6c22 2c20 2277  d", "normal", "w
+00010b80: 6974 685f 6465 6661 756c 7422 293a 0a20  ith_default"):. 
+00010b90: 2020 2020 2020 2020 2020 2069 735f 7472             is_tr
+00010ba0: 7565 2822 636f 6d70 7574 6564 2220 6e6f  ue("computed" no
+00010bb0: 7420 696e 2064 6174 615b 6b65 795d 290a  t in data[key]).
+00010bc0: 2020 2020 2020 2020 636f 6d70 4461 7461          compData
+00010bd0: 203d 2064 6174 615b 2263 6f6d 7075 7465   = data["compute
+00010be0: 645f 636f 6c22 5d0a 2020 2020 2020 2020  d_col"].        
+00010bf0: 6973 5f74 7275 6528 2263 6f6d 7075 7465  is_true("compute
+00010c00: 6422 2069 6e20 636f 6d70 4461 7461 290a  d" in compData).
+00010c10: 2020 2020 2020 2020 6973 5f74 7275 6528          is_true(
+00010c20: 2273 716c 7465 7874 2220 696e 2063 6f6d  "sqltext" in com
+00010c30: 7044 6174 615b 2263 6f6d 7075 7465 6422  pData["computed"
+00010c40: 5d29 0a20 2020 2020 2020 2065 715f 2873  ]).        eq_(s
+00010c50: 656c 662e 6e6f 726d 616c 697a 6528 636f  elf.normalize(co
+00010c60: 6d70 4461 7461 5b22 636f 6d70 7574 6564  mpData["computed
+00010c70: 225d 5b22 7371 6c74 6578 7422 5d29 2c20  "]["sqltext"]), 
+00010c80: 226e 6f72 6d61 6c2b 3432 2229 0a0a 2020  "normal+42")..  
+00010c90: 2020 6465 6620 7465 7374 5f63 7265 6174    def test_creat
+00010ca0: 655f 6e6f 745f 6e75 6c6c 5f63 6f6d 7075  e_not_null_compu
+00010cb0: 7465 645f 636f 6c75 6d6e 2873 656c 6629  ted_column(self)
+00010cc0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00010cd0: 2020 2020 2020 5350 414e 4e45 5220 5445        SPANNER TE
+00010ce0: 5354 3a0a 0a20 2020 2020 2020 2043 6865  ST:..        Che
+00010cf0: 636b 2074 6861 7420 6f6e 2063 7265 6174  ck that on creat
+00010d00: 696e 6720 6120 636f 6d70 7574 6564 2063  ing a computed c
+00010d10: 6f6c 756d 6e20 7769 7468 2061 204e 4f54  olumn with a NOT
+00010d20: 204e 554c 4c0a 2020 2020 2020 2020 636c   NULL.        cl
+00010d30: 6175 7365 2074 6865 2063 6c61 7573 6520  ause the clause 
+00010d40: 6973 2073 6574 2069 6e20 6672 6f6e 7420  is set in front 
+00010d50: 6f66 2074 6865 2063 6f6d 7075 7465 6420  of the computed 
+00010d60: 636f 6c75 6d6e 0a20 2020 2020 2020 2073  column.        s
+00010d70: 7461 7465 6d65 6e74 2064 6566 696e 6974  tatement definit
+00010d80: 696f 6e20 616e 6420 646f 6573 6e27 7420  ion and doesn't 
+00010d90: 6361 7573 6520 6661 696c 7572 6573 2e0a  cause failures..
+00010da0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010db0: 2020 2020 656e 6769 6e65 203d 2063 7265      engine = cre
+00010dc0: 6174 655f 656e 6769 6e65 2867 6574 5f64  ate_engine(get_d
+00010dd0: 625f 7572 6c28 2929 0a20 2020 2020 2020  b_url()).       
+00010de0: 206d 6574 6164 6174 6120 3d20 4d65 7461   metadata = Meta
+00010df0: 4461 7461 2862 696e 643d 656e 6769 6e65  Data(bind=engine
+00010e00: 290a 0a20 2020 2020 2020 2054 6162 6c65  )..        Table
+00010e10: 280a 2020 2020 2020 2020 2020 2020 2253  (.            "S
+00010e20: 696e 6765 7273 222c 0a20 2020 2020 2020  ingers",.       
+00010e30: 2020 2020 206d 6574 6164 6174 612c 0a20       metadata,. 
+00010e40: 2020 2020 2020 2020 2020 2043 6f6c 756d             Colum
+00010e50: 6e28 2253 696e 6765 7249 6422 2c20 5374  n("SingerId", St
+00010e60: 7269 6e67 2833 3629 2c20 7072 696d 6172  ring(36), primar
+00010e70: 795f 6b65 793d 5472 7565 2c20 6e75 6c6c  y_key=True, null
+00010e80: 6162 6c65 3d46 616c 7365 292c 0a20 2020  able=False),.   
+00010e90: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
+00010ea0: 2246 6972 7374 4e61 6d65 222c 2053 7472  "FirstName", Str
+00010eb0: 696e 6728 3230 3029 292c 0a20 2020 2020  ing(200)),.     
+00010ec0: 2020 2020 2020 2043 6f6c 756d 6e28 224c         Column("L
+00010ed0: 6173 744e 616d 6522 2c20 5374 7269 6e67  astName", String
+00010ee0: 2832 3030 292c 206e 756c 6c61 626c 653d  (200), nullable=
+00010ef0: 4661 6c73 6529 2c0a 2020 2020 2020 2020  False),.        
+00010f00: 2020 2020 436f 6c75 6d6e 280a 2020 2020      Column(.    
+00010f10: 2020 2020 2020 2020 2020 2020 2246 756c              "Ful
+00010f20: 6c4e 616d 6522 2c0a 2020 2020 2020 2020  lName",.        
+00010f30: 2020 2020 2020 2020 5374 7269 6e67 2834          String(4
+00010f40: 3030 292c 0a20 2020 2020 2020 2020 2020  00),.           
+00010f50: 2020 2020 2043 6f6d 7075 7465 6428 2243       Computed("C
+00010f60: 4f41 4c45 5343 4528 4669 7273 744e 616d  OALESCE(FirstNam
+00010f70: 6520 7c7c 2027 2027 2c20 2727 2920 7c7c  e || ' ', '') ||
+00010f80: 204c 6173 744e 616d 6522 292c 0a20 2020   LastName"),.   
+00010f90: 2020 2020 2020 2020 2020 2020 206e 756c               nul
+00010fa0: 6c61 626c 653d 4661 6c73 652c 0a20 2020  lable=False,.   
+00010fb0: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
+00010fc0: 2020 2020 290a 0a20 2020 2020 2020 206d      )..        m
+00010fd0: 6574 6164 6174 612e 6372 6561 7465 5f61  etadata.create_a
+00010fe0: 6c6c 2865 6e67 696e 6529 0a0a 0a40 7079  ll(engine)...@py
+00010ff0: 7465 7374 2e6d 6172 6b2e 736b 6970 6966  test.mark.skipif
+00011000: 280a 2020 2020 626f 6f6c 286f 732e 656e  (.    bool(os.en
+00011010: 7669 726f 6e2e 6765 7428 2253 5041 4e4e  viron.get("SPANN
+00011020: 4552 5f45 4d55 4c41 544f 525f 484f 5354  ER_EMULATOR_HOST
+00011030: 2229 292c 2072 6561 736f 6e3d 2253 6b69  ")), reason="Ski
+00011040: 7070 6564 206f 6e20 656d 756c 6174 6f72  pped on emulator
+00011050: 220a 290a 636c 6173 7320 4a53 4f4e 5465  ".).class JSONTe
+00011060: 7374 285f 4a53 4f4e 5465 7374 293a 0a20  st(_JSONTest):. 
+00011070: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
+00011080: 736b 6970 2822 5661 6c75 6573 2077 6974  skip("Values wit
+00011090: 686f 7574 206b 6579 7320 6172 6520 6e6f  hout keys are no
+000110a0: 7420 7375 7070 6f72 7465 642e 2229 0a20  t supported."). 
+000110b0: 2020 2064 6566 2074 6573 745f 7369 6e67     def test_sing
+000110c0: 6c65 5f65 6c65 6d65 6e74 5f72 6f75 6e64  le_element_round
+000110d0: 5f74 7269 7028 7365 6c66 2c20 656c 656d  _trip(self, elem
+000110e0: 656e 7429 3a0a 2020 2020 2020 2020 7061  ent):.        pa
+000110f0: 7373 0a0a 2020 2020 6465 6620 5f74 6573  ss..    def _tes
+00011100: 745f 726f 756e 645f 7472 6970 2873 656c  t_round_trip(sel
+00011110: 662c 2064 6174 615f 656c 656d 656e 7429  f, data_element)
+00011120: 3a0a 2020 2020 2020 2020 6461 7461 5f74  :.        data_t
+00011130: 6162 6c65 203d 2073 656c 662e 7461 626c  able = self.tabl
+00011140: 6573 2e64 6174 615f 7461 626c 650a 0a20  es.data_table.. 
+00011150: 2020 2020 2020 2063 6f6e 6669 672e 6462         config.db
+00011160: 2e65 7865 6375 7465 280a 2020 2020 2020  .execute(.      
+00011170: 2020 2020 2020 6461 7461 5f74 6162 6c65        data_table
+00011180: 2e69 6e73 6572 7428 292c 0a20 2020 2020  .insert(),.     
+00011190: 2020 2020 2020 207b 2269 6422 3a20 7261         {"id": ra
+000111a0: 6e64 6f6d 2e72 616e 6469 6e74 2831 2c20  ndom.randint(1, 
+000111b0: 3130 3030 3030 3030 3029 2c20 226e 616d  100000000), "nam
+000111c0: 6522 3a20 2272 6f77 3122 2c20 2264 6174  e": "row1", "dat
+000111d0: 6122 3a20 6461 7461 5f65 6c65 6d65 6e74  a": data_element
+000111e0: 7d2c 0a20 2020 2020 2020 2029 0a0a 2020  },.        )..  
+000111f0: 2020 2020 2020 726f 7720 3d20 636f 6e66        row = conf
+00011200: 6967 2e64 622e 6578 6563 7574 6528 7365  ig.db.execute(se
+00011210: 6c65 6374 285b 6461 7461 5f74 6162 6c65  lect([data_table
+00011220: 2e63 2e64 6174 615d 2929 2e66 6972 7374  .c.data])).first
+00011230: 2829 0a0a 2020 2020 2020 2020 6571 5f28  ()..        eq_(
+00011240: 726f 772c 2028 6461 7461 5f65 6c65 6d65  row, (data_eleme
+00011250: 6e74 2c29 290a 0a20 2020 2064 6566 2074  nt,))..    def t
+00011260: 6573 745f 756e 6963 6f64 655f 726f 756e  est_unicode_roun
+00011270: 645f 7472 6970 2873 656c 6629 3a0a 2020  d_trip(self):.  
+00011280: 2020 2020 2020 2320 6e6f 7465 2077 6520        # note we 
+00011290: 696e 636c 7564 6520 556e 6963 6f64 6520  include Unicode 
+000112a0: 7375 7070 6c65 6d65 6e74 6172 7920 6368  supplementary ch
+000112b0: 6172 6163 7465 7273 2061 7320 7765 6c6c  aracters as well
+000112c0: 0a20 2020 2020 2020 2077 6974 6820 636f  .        with co
+000112d0: 6e66 6967 2e64 622e 636f 6e6e 6563 7428  nfig.db.connect(
+000112e0: 2920 6173 2063 6f6e 6e3a 0a20 2020 2020  ) as conn:.     
+000112f0: 2020 2020 2020 2063 6f6e 6e2e 6578 6563         conn.exec
+00011300: 7574 6528 0a20 2020 2020 2020 2020 2020  ute(.           
+00011310: 2020 2020 2073 656c 662e 7461 626c 6573       self.tables
+00011320: 2e64 6174 615f 7461 626c 652e 696e 7365  .data_table.inse
+00011330: 7274 2829 2c0a 2020 2020 2020 2020 2020  rt(),.          
+00011340: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00011350: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+00011360: 3a20 7261 6e64 6f6d 2e72 616e 6469 6e74  : random.randint
+00011370: 2831 2c20 3130 3030 3030 3030 3029 2c0a  (1, 100000000),.
+00011380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011390: 2020 2020 226e 616d 6522 3a20 2272 3122      "name": "r1"
+000113a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000113b0: 2020 2020 2020 2264 6174 6122 3a20 7b0a        "data": {.
+000113c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113d0: 2020 2020 2020 2020 7574 696c 2e75 2822          util.u("
+000113e0: 72c3 a976 65f0 9f90 8d20 696c 6cc3 a922  r..ve.... ill.."
+000113f0: 293a 2075 7469 6c2e 7528 2272 c3a9 7665  ): util.u("r..ve
+00011400: f09f 908d 2069 6c6c c3a9 2229 2c0a 2020  .... ill.."),.  
+00011410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011420: 2020 2020 2020 2264 6174 6122 3a20 7b22        "data": {"
+00011430: 6b31 223a 2075 7469 6c2e 7528 2264 72c3  k1": util.u("dr.
+00011440: b46c f09f 908d 6522 297d 2c0a 2020 2020  .l....e")},.    
+00011450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011460: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+00011470: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00011480: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+00011490: 2065 715f 280a 2020 2020 2020 2020 2020   eq_(.          
+000114a0: 2020 2020 2020 636f 6e6e 2e73 6361 6c61        conn.scala
+000114b0: 7228 7365 6c65 6374 285b 7365 6c66 2e74  r(select([self.t
+000114c0: 6162 6c65 732e 6461 7461 5f74 6162 6c65  ables.data_table
+000114d0: 2e63 2e64 6174 615d 2929 2c0a 2020 2020  .c.data])),.    
+000114e0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+000114f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011500: 2020 7574 696c 2e75 2822 72c3 a976 65f0    util.u("r..ve.
+00011510: 9f90 8d20 696c 6cc3 a922 293a 2075 7469  ... ill.."): uti
+00011520: 6c2e 7528 2272 c3a9 7665 f09f 908d 2069  l.u("r..ve.... i
+00011530: 6c6c c3a9 2229 2c0a 2020 2020 2020 2020  ll.."),.        
+00011540: 2020 2020 2020 2020 2020 2020 2264 6174              "dat
+00011550: 6122 3a20 7b22 6b31 223a 2075 7469 6c2e  a": {"k1": util.
+00011560: 7528 2264 72c3 b46c f09f 908d 6522 297d  u("dr..l....e")}
+00011570: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011580: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00011590: 2029 0a0a 2020 2020 4070 7974 6573 742e   )..    @pytest.
+000115a0: 6d61 726b 2e73 6b69 7028 2250 6172 616d  mark.skip("Param
+000115b0: 6574 6572 697a 6564 2074 7970 6573 2061  eterized types a
+000115c0: 7265 206e 6f74 2073 7570 706f 7274 6564  re not supported
+000115d0: 2e22 290a 2020 2020 6465 6620 7465 7374  .").    def test
+000115e0: 5f65 7661 6c5f 6e6f 6e65 5f66 6c61 675f  _eval_none_flag_
+000115f0: 6f72 6d28 7365 6c66 293a 0a20 2020 2020  orm(self):.     
+00011600: 2020 2070 6173 730a 0a20 2020 2040 7079     pass..    @py
+00011610: 7465 7374 2e6d 6172 6b2e 736b 6970 280a  test.mark.skip(.
+00011620: 2020 2020 2020 2020 2253 7061 6e6e 6572          "Spanner
+00011630: 204a 534f 4e5f 5641 4c55 4528 2920 616c   JSON_VALUE() al
+00011640: 7761 7973 2072 6574 7572 6e73 2053 5452  ways returns STR
+00011650: 494e 472c 220a 2020 2020 2020 2020 2274  ING,".        "t
+00011660: 6875 732c 2074 6869 7320 7465 7374 2063  hus, this test c
+00011670: 6173 6520 6361 6e27 7420 6265 2065 7865  ase can't be exe
+00011680: 6375 7465 642e 220a 2020 2020 290a 2020  cuted.".    ).  
+00011690: 2020 6465 6620 7465 7374 5f69 6e64 6578    def test_index
+000116a0: 5f74 7970 6564 5f63 6f6d 7061 7269 736f  _typed_compariso
+000116b0: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
+000116c0: 2070 6173 730a 0a20 2020 2040 7079 7465   pass..    @pyte
+000116d0: 7374 2e6d 6172 6b2e 736b 6970 280a 2020  st.mark.skip(.  
+000116e0: 2020 2020 2020 2253 7061 6e6e 6572 204a        "Spanner J
+000116f0: 534f 4e5f 5641 4c55 4528 2920 616c 7761  SON_VALUE() alwa
+00011700: 7973 2072 6574 7572 6e73 2053 5452 494e  ys returns STRIN
+00011710: 472c 220a 2020 2020 2020 2020 2274 6875  G,".        "thu
+00011720: 732c 2074 6869 7320 7465 7374 2063 6173  s, this test cas
+00011730: 6520 6361 6e27 7420 6265 2065 7865 6375  e can't be execu
+00011740: 7465 642e 220a 2020 2020 290a 2020 2020  ted.".    ).    
+00011750: 6465 6620 7465 7374 5f70 6174 685f 7479  def test_path_ty
+00011760: 7065 645f 636f 6d70 6172 6973 6f6e 2873  ped_comparison(s
+00011770: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+00011780: 7373 0a0a 2020 2020 4070 7974 6573 742e  ss..    @pytest.
+00011790: 6d61 726b 2e73 6b69 7028 2243 7573 746f  mark.skip("Custo
+000117a0: 6d20 4a53 4f4e 2064 652d 2f73 6572 6961  m JSON de-/seria
+000117b0: 6c69 7a65 7273 2061 7265 206e 6f74 2073  lizers are not s
+000117c0: 7570 706f 7274 6564 2e22 290a 2020 2020  upported.").    
+000117d0: 6465 6620 7465 7374 5f72 6f75 6e64 5f74  def test_round_t
+000117e0: 7269 705f 6375 7374 6f6d 5f6a 736f 6e28  rip_custom_json(
+000117f0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+00011800: 6173 730a 0a20 2020 2064 6566 205f 696e  ass..    def _in
+00011810: 6465 785f 6669 7874 7572 6573 2866 6e29  dex_fixtures(fn)
+00011820: 3a0a 2020 2020 2020 2020 666e 203d 2074  :.        fn = t
+00011830: 6573 7469 6e67 2e63 6f6d 6269 6e61 7469  esting.combinati
+00011840: 6f6e 7328 0a20 2020 2020 2020 2020 2020  ons(.           
+00011850: 2028 2262 6f6f 6c65 616e 222c 2054 7275   ("boolean", Tru
+00011860: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+00011870: 2822 626f 6f6c 6561 6e22 2c20 4661 6c73  ("boolean", Fals
+00011880: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+00011890: 2822 626f 6f6c 6561 6e22 2c20 4e6f 6e65  ("boolean", None
+000118a0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+000118b0: 2273 7472 696e 6722 2c20 2273 6f6d 6520  "string", "some 
+000118c0: 7374 7269 6e67 2229 2c0a 2020 2020 2020  string"),.      
+000118d0: 2020 2020 2020 2822 7374 7269 6e67 222c        ("string",
+000118e0: 204e 6f6e 6529 2c0a 2020 2020 2020 2020   None),.        
+000118f0: 2020 2020 2822 696e 7465 6765 7222 2c20      ("integer", 
+00011900: 3135 292c 0a20 2020 2020 2020 2020 2020  15),.           
+00011910: 2028 2269 6e74 6567 6572 222c 2031 292c   ("integer", 1),
+00011920: 0a20 2020 2020 2020 2020 2020 2028 2269  .            ("i
+00011930: 6e74 6567 6572 222c 2030 292c 0a20 2020  nteger", 0),.   
+00011940: 2020 2020 2020 2020 2028 2269 6e74 6567           ("integ
+00011950: 6572 222c 204e 6f6e 6529 2c0a 2020 2020  er", None),.    
+00011960: 2020 2020 2020 2020 2822 666c 6f61 7422          ("float"
+00011970: 2c20 3238 2e35 292c 0a20 2020 2020 2020  , 28.5),.       
+00011980: 2020 2020 2028 2266 6c6f 6174 222c 204e       ("float", N
+00011990: 6f6e 6529 2c0a 2020 2020 2020 2020 2020  one),.          
+000119a0: 2020 6964 5f3d 2273 6122 2c0a 2020 2020    id_="sa",.    
+000119b0: 2020 2020 2928 666e 290a 2020 2020 2020      )(fn).      
+000119c0: 2020 7265 7475 726e 2066 6e0a 0a20 2020    return fn..   
+000119d0: 2040 5f69 6e64 6578 5f66 6978 7475 7265   @_index_fixture
+000119e0: 730a 2020 2020 6465 6620 7465 7374 5f69  s.    def test_i
+000119f0: 6e64 6578 5f74 7970 6564 5f61 6363 6573  ndex_typed_acces
+00011a00: 7328 7365 6c66 2c20 6461 7461 7479 7065  s(self, datatype
+00011a10: 2c20 7661 6c75 6529 3a0a 2020 2020 2020  , value):.      
+00011a20: 2020 6461 7461 5f74 6162 6c65 203d 2073    data_table = s
+00011a30: 656c 662e 7461 626c 6573 2e64 6174 615f  elf.tables.data_
+00011a40: 7461 626c 650a 2020 2020 2020 2020 6461  table.        da
+00011a50: 7461 5f65 6c65 6d65 6e74 203d 207b 226b  ta_element = {"k
+00011a60: 6579 3122 3a20 7661 6c75 657d 0a20 2020  ey1": value}.   
+00011a70: 2020 2020 2077 6974 6820 636f 6e66 6967       with config
+00011a80: 2e64 622e 636f 6e6e 6563 7428 2920 6173  .db.connect() as
+00011a90: 2063 6f6e 6e3a 0a20 2020 2020 2020 2020   conn:.         
+00011aa0: 2020 2063 6f6e 6e2e 6578 6563 7574 6528     conn.execute(
+00011ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011ac0: 2064 6174 615f 7461 626c 652e 696e 7365   data_table.inse
+00011ad0: 7274 2829 2c0a 2020 2020 2020 2020 2020  rt(),.          
+00011ae0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00011af0: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+00011b00: 3a20 7261 6e64 6f6d 2e72 616e 6469 6e74  : random.randint
+00011b10: 2831 2c20 3130 3030 3030 3030 3029 2c0a  (1, 100000000),.
+00011b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b30: 2020 2020 226e 616d 6522 3a20 2272 6f77      "name": "row
+00011b40: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
+00011b50: 2020 2020 2020 2020 2264 6174 6122 3a20          "data": 
+00011b60: 6461 7461 5f65 6c65 6d65 6e74 2c0a 2020  data_element,.  
+00011b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b80: 2020 226e 756c 6c64 6174 6122 3a20 6461    "nulldata": da
+00011b90: 7461 5f65 6c65 6d65 6e74 2c0a 2020 2020  ta_element,.    
+00011ba0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00011bb0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00011bc0: 2020 2020 2020 2020 2020 6578 7072 203d            expr =
+00011bd0: 2064 6174 615f 7461 626c 652e 632e 6461   data_table.c.da
+00011be0: 7461 5b22 6b65 7931 225d 0a20 2020 2020  ta["key1"].     
+00011bf0: 2020 2020 2020 2065 7870 7220 3d20 6765         expr = ge
+00011c00: 7461 7474 7228 6578 7072 2c20 2261 735f  tattr(expr, "as_
+00011c10: 2573 2220 2520 6461 7461 7479 7065 2928  %s" % datatype)(
+00011c20: 290a 0a20 2020 2020 2020 2020 2020 2072  )..            r
+00011c30: 6f75 6e64 7472 6970 203d 2063 6f6e 6e2e  oundtrip = conn.
+00011c40: 7363 616c 6172 2873 656c 6563 7428 5b65  scalar(select([e
+00011c50: 7870 725d 2929 0a20 2020 2020 2020 2020  xpr])).         
+00011c60: 2020 2069 6620 726f 756e 6474 7269 7020     if roundtrip 
+00011c70: 696e 2028 2274 7275 6522 2c20 2266 616c  in ("true", "fal
+00011c80: 7365 222c 204e 6f6e 6529 3a0a 2020 2020  se", None):.    
+00011c90: 2020 2020 2020 2020 2020 2020 726f 756e              roun
+00011ca0: 6474 7269 7020 3d20 7374 7228 726f 756e  dtrip = str(roun
+00011cb0: 6474 7269 7029 2e63 6170 6974 616c 697a  dtrip).capitaliz
+00011cc0: 6528 290a 0a20 2020 2020 2020 2020 2020  e()..           
+00011cd0: 2065 715f 2873 7472 2872 6f75 6e64 7472   eq_(str(roundtr
+00011ce0: 6970 292c 2073 7472 2876 616c 7565 2929  ip), str(value))
+00011cf0: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
+00011d00: 726b 2e73 6b69 7028 0a20 2020 2020 2020  rk.skip(.       
+00011d10: 2022 5370 616e 6e65 7220 646f 6573 6e27   "Spanner doesn'
+00011d20: 7420 7375 7070 6f72 7420 7479 7065 2063  t support type c
+00011d30: 6173 7473 2069 6e73 6964 6520 4a53 4f4e  asts inside JSON
+00011d40: 5f56 414c 5545 2829 2066 756e 6374 696f  _VALUE() functio
+00011d50: 6e2e 220a 2020 2020 290a 2020 2020 6465  n.".    ).    de
+00011d60: 6620 7465 7374 5f72 6f75 6e64 5f74 7269  f test_round_tri
+00011d70: 705f 6a73 6f6e 5f6e 756c 6c5f 6173 5f6a  p_json_null_as_j
+00011d80: 736f 6e5f 6e75 6c6c 2873 656c 6629 3a0a  son_null(self):.
+00011d90: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00011da0: 2020 4070 7974 6573 742e 6d61 726b 2e73    @pytest.mark.s
+00011db0: 6b69 7028 0a20 2020 2020 2020 2022 5370  kip(.        "Sp
+00011dc0: 616e 6e65 7220 646f 6573 6e27 7420 7375  anner doesn't su
+00011dd0: 7070 6f72 7420 7479 7065 2063 6173 7473  pport type casts
+00011de0: 2069 6e73 6964 6520 4a53 4f4e 5f56 414c   inside JSON_VAL
+00011df0: 5545 2829 2066 756e 6374 696f 6e2e 220a  UE() function.".
+00011e00: 2020 2020 290a 2020 2020 6465 6620 7465      ).    def te
+00011e10: 7374 5f72 6f75 6e64 5f74 7269 705f 6e6f  st_round_trip_no
+00011e20: 6e65 5f61 735f 6a73 6f6e 5f6e 756c 6c28  ne_as_json_null(
+00011e30: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+00011e40: 6173 730a 0a20 2020 2040 7079 7465 7374  ass..    @pytest
+00011e50: 2e6d 6172 6b2e 736b 6970 280a 2020 2020  .mark.skip(.    
+00011e60: 2020 2020 2253 7061 6e6e 6572 2064 6f65      "Spanner doe
+00011e70: 736e 2774 2073 7570 706f 7274 2074 7970  sn't support typ
+00011e80: 6520 6361 7374 7320 696e 7369 6465 204a  e casts inside J
+00011e90: 534f 4e5f 5641 4c55 4528 2920 6675 6e63  SON_VALUE() func
+00011ea0: 7469 6f6e 2e22 0a20 2020 2029 0a20 2020  tion.".    ).   
+00011eb0: 2064 6566 2074 6573 745f 726f 756e 645f   def test_round_
+00011ec0: 7472 6970 5f6e 6f6e 655f 6173 5f73 716c  trip_none_as_sql
+00011ed0: 5f6e 756c 6c28 7365 6c66 293a 0a20 2020  _null(self):.   
+00011ee0: 2020 2020 2070 6173 730a 0a0a 636c 6173       pass...clas
+00011ef0: 7320 4578 6563 7574 696f 6e4f 7074 696f  s ExecutionOptio
+00011f00: 6e73 5265 7175 6573 7450 7269 6f72 6f74  nsRequestPriorot
+00011f10: 7954 6573 7428 6669 7874 7572 6573 2e54  yTest(fixtures.T
+00011f20: 6573 7442 6173 6529 3a0a 2020 2020 6465  estBase):.    de
+00011f30: 6620 7365 7455 7028 7365 6c66 293a 0a20  f setUp(self):. 
+00011f40: 2020 2020 2020 2073 656c 662e 5f65 6e67         self._eng
+00011f50: 696e 6520 3d20 6372 6561 7465 5f65 6e67  ine = create_eng
+00011f60: 696e 6528 6765 745f 6462 5f75 726c 2829  ine(get_db_url()
+00011f70: 2c20 706f 6f6c 5f73 697a 653d 3129 0a20  , pool_size=1). 
+00011f80: 2020 2020 2020 206d 6574 6164 6174 6120         metadata 
+00011f90: 3d20 4d65 7461 4461 7461 2862 696e 643d  = MetaData(bind=
+00011fa0: 7365 6c66 2e5f 656e 6769 6e65 290a 0a20  self._engine).. 
+00011fb0: 2020 2020 2020 2073 656c 662e 5f74 6162         self._tab
+00011fc0: 6c65 203d 2054 6162 6c65 280a 2020 2020  le = Table(.    
+00011fd0: 2020 2020 2020 2020 2265 7865 6375 7469          "executi
+00011fe0: 6f6e 5f6f 7074 696f 6e73 3222 2c0a 2020  on_options2",.  
+00011ff0: 2020 2020 2020 2020 2020 6d65 7461 6461            metada
+00012000: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
+00012010: 436f 6c75 6d6e 2822 6f70 745f 6964 222c  Column("opt_id",
+00012020: 2049 6e74 6567 6572 2c20 7072 696d 6172   Integer, primar
+00012030: 795f 6b65 793d 5472 7565 292c 0a20 2020  y_key=True),.   
+00012040: 2020 2020 2020 2020 2043 6f6c 756d 6e28           Column(
+00012050: 226f 7074 5f6e 616d 6522 2c20 5374 7269  "opt_name", Stri
+00012060: 6e67 2831 3629 2c20 6e75 6c6c 6162 6c65  ng(16), nullable
+00012070: 3d46 616c 7365 292c 0a20 2020 2020 2020  =False),.       
+00012080: 2029 0a0a 2020 2020 2020 2020 6d65 7461   )..        meta
+00012090: 6461 7461 2e63 7265 6174 655f 616c 6c28  data.create_all(
+000120a0: 7365 6c66 2e5f 656e 6769 6e65 290a 2020  self._engine).  
+000120b0: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
+000120c0: 2831 290a 0a20 2020 2064 6566 2074 6573  (1)..    def tes
+000120d0: 745f 7265 7175 6573 745f 7072 696f 7269  t_request_priori
+000120e0: 7479 2873 656c 6629 3a0a 2020 2020 2020  ty(self):.      
+000120f0: 2020 5052 494f 5249 5459 203d 2052 6571    PRIORITY = Req
+00012100: 7565 7374 4f70 7469 6f6e 732e 5072 696f  uestOptions.Prio
+00012110: 7269 7479 2e50 5249 4f52 4954 595f 4d45  rity.PRIORITY_ME
+00012120: 4449 554d 0a20 2020 2020 2020 2077 6974  DIUM.        wit
+00012130: 6820 7365 6c66 2e5f 656e 6769 6e65 2e63  h self._engine.c
+00012140: 6f6e 6e65 6374 2829 2e65 7865 6375 7469  onnect().executi
+00012150: 6f6e 5f6f 7074 696f 6e73 280a 2020 2020  on_options(.    
+00012160: 2020 2020 2020 2020 7265 7175 6573 745f          request_
+00012170: 7072 696f 7269 7479 3d50 5249 4f52 4954  priority=PRIORIT
+00012180: 590a 2020 2020 2020 2020 2920 6173 2063  Y.        ) as c
+00012190: 6f6e 6e65 6374 696f 6e3a 0a20 2020 2020  onnection:.     
+000121a0: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
+000121b0: 6e2e 6578 6563 7574 6528 7365 6c65 6374  n.execute(select
+000121c0: 285b 222a 225d 2c20 6672 6f6d 5f6f 626a  (["*"], from_obj
+000121d0: 3d73 656c 662e 5f74 6162 6c65 2929 2e66  =self._table)).f
+000121e0: 6574 6368 616c 6c28 290a 0a20 2020 2020  etchall()..     
+000121f0: 2020 2077 6974 6820 7365 6c66 2e5f 656e     with self._en
+00012200: 6769 6e65 2e63 6f6e 6e65 6374 2829 2061  gine.connect() a
+00012210: 7320 636f 6e6e 6563 7469 6f6e 3a0a 2020  s connection:.  
+00012220: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+00012230: 2063 6f6e 6e65 6374 696f 6e2e 636f 6e6e   connection.conn
+00012240: 6563 7469 6f6e 2e72 6571 7565 7374 5f70  ection.request_p
+00012250: 7269 6f72 6974 7920 6973 204e 6f6e 650a  riority is None.
+00012260: 0a20 2020 2020 2020 2065 6e67 696e 6520  .        engine 
+00012270: 3d20 6372 6561 7465 5f65 6e67 696e 6528  = create_engine(
+00012280: 2273 716c 6974 653a 2f2f 2f64 6174 6162  "sqlite:///datab
+00012290: 6173 6522 290a 2020 2020 2020 2020 7769  ase").        wi
+000122a0: 7468 2065 6e67 696e 652e 636f 6e6e 6563  th engine.connec
+000122b0: 7428 2920 6173 2063 6f6e 6e65 6374 696f  t() as connectio
+000122c0: 6e3a 0a20 2020 2020 2020 2020 2020 2070  n:.            p
+000122d0: 6173 730a 0a0a 636c 6173 7320 4372 6561  ass...class Crea
+000122e0: 7465 456e 6769 6e65 5769 7468 436c 6965  teEngineWithClie
+000122f0: 6e74 4f62 6a65 6374 5465 7374 2866 6978  ntObjectTest(fix
+00012300: 7475 7265 732e 5465 7374 4261 7365 293a  tures.TestBase):
+00012310: 0a20 2020 2064 6566 2074 6573 745f 6372  .    def test_cr
+00012320: 6561 7465 5f65 6e67 696e 655f 775f 7661  eate_engine_w_va
+00012330: 6c69 645f 636c 6965 6e74 5f6f 626a 6563  lid_client_objec
+00012340: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+00012350: 2022 2222 0a20 2020 2020 2020 2053 5041   """.        SPA
+00012360: 4e4e 4552 2054 4553 543a 0a0a 2020 2020  NNER TEST:..    
+00012370: 2020 2020 4368 6563 6b20 7468 6174 2077      Check that w
+00012380: 6520 6361 6e20 636f 6e6e 6563 7420 746f  e can connect to
+00012390: 2053 716c 416c 6368 656d 790a 2020 2020   SqlAlchemy.    
+000123a0: 2020 2020 6279 2070 6173 7369 6e67 2063      by passing c
+000123b0: 7573 746f 6d20 436c 6965 6e74 206f 626a  ustom Client obj
+000123c0: 6563 742e 0a20 2020 2020 2020 2022 2222  ect..        """
+000123d0: 0a20 2020 2020 2020 2063 6c69 656e 7420  .        client 
+000123e0: 3d20 436c 6965 6e74 2870 726f 6a65 6374  = Client(project
+000123f0: 3d67 6574 5f70 726f 6a65 6374 2829 290a  =get_project()).
+00012400: 2020 2020 2020 2020 656e 6769 6e65 203d          engine =
+00012410: 2063 7265 6174 655f 656e 6769 6e65 2867   create_engine(g
+00012420: 6574 5f64 625f 7572 6c28 292c 2063 6f6e  et_db_url(), con
+00012430: 6e65 6374 5f61 7267 733d 7b22 636c 6965  nect_args={"clie
+00012440: 6e74 223a 2063 6c69 656e 747d 290a 2020  nt": client}).  
+00012450: 2020 2020 2020 7769 7468 2065 6e67 696e        with engin
+00012460: 652e 636f 6e6e 6563 7428 2920 6173 2063  e.connect() as c
+00012470: 6f6e 6e65 6374 696f 6e3a 0a20 2020 2020  onnection:.     
+00012480: 2020 2020 2020 2061 7373 6572 7420 636f         assert co
+00012490: 6e6e 6563 7469 6f6e 2e63 6f6e 6e65 6374  nnection.connect
+000124a0: 696f 6e2e 696e 7374 616e 6365 2e5f 636c  ion.instance._cl
+000124b0: 6965 6e74 203d 3d20 636c 6965 6e74 0a0a  ient == client..
+000124c0: 2020 2020 6465 6620 7465 7374 5f63 7265      def test_cre
+000124d0: 6174 655f 656e 6769 6e65 5f77 5f69 6e76  ate_engine_w_inv
+000124e0: 616c 6964 5f63 6c69 656e 745f 6f62 6a65  alid_client_obje
+000124f0: 6374 2873 656c 6629 3a0a 2020 2020 2020  ct(self):.      
+00012500: 2020 2222 220a 2020 2020 2020 2020 5350    """.        SP
+00012510: 414e 4e45 5220 5445 5354 3a0a 0a20 2020  ANNER TEST:..   
+00012520: 2020 2020 2043 6865 636b 2074 6861 7420       Check that 
+00012530: 6966 2070 726f 6a65 6374 2069 6420 696e  if project id in
+00012540: 2075 726c 2061 6e64 2063 7573 746f 6d20   url and custom 
+00012550: 436c 6965 6e74 0a20 2020 2020 2020 204f  Client.        O
+00012560: 626a 6563 7420 7061 7373 6564 2074 6f20  bject passed to 
+00012570: 656e 6769 6e65 7220 6d69 736d 6174 6368  enginer mismatch
+00012580: 2c20 6572 726f 7220 6973 2074 6872 6f77  , error is throw
+00012590: 6e2e 0a20 2020 2020 2020 2022 2222 0a20  n..        """. 
+000125a0: 2020 2020 2020 2063 6c69 656e 7420 3d20         client = 
+000125b0: 436c 6965 6e74 2870 726f 6a65 6374 3d22  Client(project="
+000125c0: 7072 6f6a 6563 745f 6964 2229 0a20 2020  project_id").   
+000125d0: 2020 2020 2065 6e67 696e 6520 3d20 6372       engine = cr
+000125e0: 6561 7465 5f65 6e67 696e 6528 6765 745f  eate_engine(get_
+000125f0: 6462 5f75 726c 2829 2c20 636f 6e6e 6563  db_url(), connec
+00012600: 745f 6172 6773 3d7b 2263 6c69 656e 7422  t_args={"client"
+00012610: 3a20 636c 6965 6e74 7d29 0a0a 2020 2020  : client})..    
+00012620: 2020 2020 7769 7468 2070 7974 6573 742e      with pytest.
+00012630: 7261 6973 6573 2856 616c 7565 4572 726f  raises(ValueErro
+00012640: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00012650: 656e 6769 6e65 2e63 6f6e 6e65 6374 2829  engine.connect()
+00012660: 0a                                       .
```


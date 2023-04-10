# Comparing `tmp/moontour_common-1.0.8.tar.gz` & `tmp/moontour_common-1.0.9.tar.gz`

## Comparing `moontour_common-1.0.8.tar` & `moontour_common-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common/database/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common/database/clients/__init__.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common/database/clients/mongo.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common/database/clients/rabbitmq.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common/database/clients/redis.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common/models/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common/models/coordinates.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common/models/guess.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common/models/phase.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common/models/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common/models/rooms/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common/models/rooms/duel_room.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common/models/rooms/health_room.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common/models/rooms/room.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common/models/rooms/streak_room.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common/models/rooms/teams_room.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common.egg-info/PKG-INFO
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 moontour_common-1.0.8/moontour_common.egg-info/top_level.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 moontour_common-1.0.8/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 moontour_common-1.0.8/README.md
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 moontour_common-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 moontour_common-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common/database/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common/database/clients/__init__.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common/database/clients/mongo.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common/database/clients/rabbitmq.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common/database/clients/redis.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common/models/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common/models/coordinates.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common/models/guess.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common/models/phase.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common/models/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common/models/rooms/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common/models/rooms/duel_room.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common/models/rooms/health_room.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common/models/rooms/room.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common/models/rooms/streak_room.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common/models/rooms/teams_room.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 moontour_common-1.0.9/moontour_common.egg-info/top_level.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 moontour_common-1.0.9/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 moontour_common-1.0.9/README.md
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 moontour_common-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 moontour_common-1.0.9/PKG-INFO
```

### Comparing `moontour_common-1.0.8/moontour_common/models/__init__.py` & `moontour_common-1.0.9/moontour_common/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moontour_common-1.0.8/moontour_common/models/rooms/room.py` & `moontour_common-1.0.9/moontour_common/models/rooms/room.py`

 * *Files identical despite different names*

### Comparing `moontour_common-1.0.8/moontour_common/models/rooms/teams_room.py` & `moontour_common-1.0.9/moontour_common/models/rooms/teams_room.py`

 * *Files identical despite different names*

### Comparing `moontour_common-1.0.8/pyproject.toml` & `moontour_common-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "moontour-common"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
     { name = "Elai Corem", email = "elaicorem1@gmail.com" },
 ]
 description = "Common entities and utilities for Moontour services"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```


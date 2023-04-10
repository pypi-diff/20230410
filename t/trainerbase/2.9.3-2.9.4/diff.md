# Comparing `tmp/TrainerBase-2.9.3.tar.gz` & `tmp/TrainerBase-2.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrainerBase-2.9.3.tar", last modified: Mon Apr 10 21:21:18 2023, max compression
+gzip compressed data, was "TrainerBase-2.9.4.tar", last modified: Mon Apr 10 21:26:09 2023, max compression
```

## Comparing `TrainerBase-2.9.3.tar` & `TrainerBase-2.9.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rwxr-xr-x   0        0        0   117248 2022-02-21 09:32:45.418863 TrainerBase-2.9.3/fasm/FASM.EXE
--rw-r--r--   0        0        0     1103 2023-04-02 15:26:24.974155 TrainerBase-2.9.3/LICENSE
--rw-r--r--   0        0        0      788 2023-04-10 21:20:25.266891 TrainerBase-2.9.3/pyproject.toml
--rw-r--r--   0        0        0      170 2022-11-27 19:37:39.028579 TrainerBase-2.9.3/README.md
--rw-r--r--   0        0        0        0 2022-11-27 19:37:39.030089 TrainerBase-2.9.3/trainerbase/__init__.py
--rw-r--r--   0        0        0     3464 2023-04-10 20:48:57.586831 TrainerBase-2.9.3/trainerbase/codeinjection.py
--rw-r--r--   0        0        0     1019 2023-04-10 20:37:50.924352 TrainerBase-2.9.3/trainerbase/common.py
--rw-r--r--   0        0        0     2686 2022-12-07 20:27:21.445222 TrainerBase-2.9.3/trainerbase/gameobject.py
--rw-r--r--   0        0        0     6434 2023-04-10 21:02:16.760340 TrainerBase-2.9.3/trainerbase/gui.py
--rw-r--r--   0        0        0     1332 2023-04-10 20:47:38.678906 TrainerBase-2.9.3/trainerbase/memory.py
--rw-r--r--   0        0        0     2518 2022-12-09 12:40:11.890792 TrainerBase-2.9.3/trainerbase/scriptengine.py
--rw-r--r--   0        0        0        0 2022-11-27 19:37:39.031619 TrainerBase-2.9.3/trainerbase/template/__init__.py
--rw-r--r--   0        0        0       56 2022-12-03 21:05:33.189289 TrainerBase-2.9.3/trainerbase/template/config.py
--rw-r--r--   0        0        0      758 2022-12-03 21:05:33.189289 TrainerBase-2.9.3/trainerbase/template/gui.py
--rw-r--r--   0        0        0       95 2022-12-03 21:05:33.190297 TrainerBase-2.9.3/trainerbase/template/injections.py
--rw-r--r--   0        0        0      302 2022-12-07 20:41:59.080957 TrainerBase-2.9.3/trainerbase/template/main.py
--rw-r--r--   0        0        0      133 2022-12-04 16:32:33.988485 TrainerBase-2.9.3/trainerbase/template/objects.py
--rw-r--r--   0        0        0      233 2022-12-07 19:31:24.358010 TrainerBase-2.9.3/trainerbase/template/scripts.py
--rw-r--r--   0        0        0      256 2023-04-10 21:20:16.978879 TrainerBase-2.9.3/trainerbase/tts.py
--rw-r--r--   0        0        0      128 2022-12-03 21:05:33.192296 TrainerBase-2.9.3/trainerbase/use_trainer_template.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 TrainerBase-2.9.3/PKG-INFO
+-rwxr-xr-x   0        0        0   117248 2022-02-21 09:32:45.418863 TrainerBase-2.9.4/fasm/FASM.EXE
+-rw-r--r--   0        0        0     1103 2023-04-02 15:26:24.974155 TrainerBase-2.9.4/LICENSE
+-rw-r--r--   0        0        0      788 2023-04-10 21:25:00.299740 TrainerBase-2.9.4/pyproject.toml
+-rw-r--r--   0        0        0      170 2022-11-27 19:37:39.028579 TrainerBase-2.9.4/README.md
+-rw-r--r--   0        0        0        0 2022-11-27 19:37:39.030089 TrainerBase-2.9.4/trainerbase/__init__.py
+-rw-r--r--   0        0        0     3464 2023-04-10 20:48:57.586831 TrainerBase-2.9.4/trainerbase/codeinjection.py
+-rw-r--r--   0        0        0     1019 2023-04-10 20:37:50.924352 TrainerBase-2.9.4/trainerbase/common.py
+-rw-r--r--   0        0        0     2686 2022-12-07 20:27:21.445222 TrainerBase-2.9.4/trainerbase/gameobject.py
+-rw-r--r--   0        0        0     6434 2023-04-10 21:02:16.760340 TrainerBase-2.9.4/trainerbase/gui.py
+-rw-r--r--   0        0        0     1332 2023-04-10 20:47:38.678906 TrainerBase-2.9.4/trainerbase/memory.py
+-rw-r--r--   0        0        0     2518 2022-12-09 12:40:11.890792 TrainerBase-2.9.4/trainerbase/scriptengine.py
+-rw-r--r--   0        0        0        0 2022-11-27 19:37:39.031619 TrainerBase-2.9.4/trainerbase/template/__init__.py
+-rw-r--r--   0        0        0       56 2022-12-03 21:05:33.189289 TrainerBase-2.9.4/trainerbase/template/config.py
+-rw-r--r--   0        0        0      758 2022-12-03 21:05:33.189289 TrainerBase-2.9.4/trainerbase/template/gui.py
+-rw-r--r--   0        0        0       95 2022-12-03 21:05:33.190297 TrainerBase-2.9.4/trainerbase/template/injections.py
+-rw-r--r--   0        0        0      302 2022-12-07 20:41:59.080957 TrainerBase-2.9.4/trainerbase/template/main.py
+-rw-r--r--   0        0        0      133 2022-12-04 16:32:33.988485 TrainerBase-2.9.4/trainerbase/template/objects.py
+-rw-r--r--   0        0        0      233 2022-12-07 19:31:24.358010 TrainerBase-2.9.4/trainerbase/template/scripts.py
+-rw-r--r--   0        0        0      274 2023-04-10 21:24:56.178701 TrainerBase-2.9.4/trainerbase/tts.py
+-rw-r--r--   0        0        0      128 2022-12-03 21:05:33.192296 TrainerBase-2.9.4/trainerbase/use_trainer_template.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 TrainerBase-2.9.4/PKG-INFO
```

### Comparing `TrainerBase-2.9.3/fasm/FASM.EXE` & `TrainerBase-2.9.4/fasm/FASM.EXE`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.3/LICENSE` & `TrainerBase-2.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.3/pyproject.toml` & `TrainerBase-2.9.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 dev = [
     "black>=22.10.0",
     "pylint>=2.15.7",
 ]
 
 [project]
 name = "TrainerBase"
-version = "2.9.3"
+version = "2.9.4"
 description = "Template/Framework to create game trainers"
 authors = [
     { name = "v01d", email = "v01d@v01d.ru" },
     { name = "doomayka", email = "zd@doomayka.ru" },
 ]
 dependencies = [
     "pymem>=1.10.0",
```

### Comparing `TrainerBase-2.9.3/trainerbase/codeinjection.py` & `TrainerBase-2.9.4/trainerbase/codeinjection.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.3/trainerbase/common.py` & `TrainerBase-2.9.4/trainerbase/common.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.3/trainerbase/gameobject.py` & `TrainerBase-2.9.4/trainerbase/gameobject.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.3/trainerbase/gui.py` & `TrainerBase-2.9.4/trainerbase/gui.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.3/trainerbase/memory.py` & `TrainerBase-2.9.4/trainerbase/memory.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.3/trainerbase/scriptengine.py` & `TrainerBase-2.9.4/trainerbase/scriptengine.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.3/trainerbase/template/gui.py` & `TrainerBase-2.9.4/trainerbase/template/gui.py`

 * *Files identical despite different names*


# Comparing `tmp/TrainerBase-2.9.7.tar.gz` & `tmp/TrainerBase-2.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrainerBase-2.9.7.tar", last modified: Mon Apr 10 21:41:09 2023, max compression
+gzip compressed data, was "TrainerBase-2.9.8.tar", last modified: Mon Apr 10 21:46:04 2023, max compression
```

## Comparing `TrainerBase-2.9.7.tar` & `TrainerBase-2.9.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rwxr-xr-x   0        0        0   117248 2022-02-21 09:32:45.418863 TrainerBase-2.9.7/fasm/FASM.EXE
--rw-r--r--   0        0        0     1103 2023-04-02 15:26:24.974155 TrainerBase-2.9.7/LICENSE
--rw-r--r--   0        0        0      788 2023-04-10 21:40:37.373402 TrainerBase-2.9.7/pyproject.toml
--rw-r--r--   0        0        0      170 2022-11-27 19:37:39.028579 TrainerBase-2.9.7/README.md
--rw-r--r--   0        0        0        0 2022-11-27 19:37:39.030089 TrainerBase-2.9.7/trainerbase/__init__.py
--rw-r--r--   0        0        0     3464 2023-04-10 20:48:57.586831 TrainerBase-2.9.7/trainerbase/codeinjection.py
--rw-r--r--   0        0        0     1019 2023-04-10 20:37:50.924352 TrainerBase-2.9.7/trainerbase/common.py
--rw-r--r--   0        0        0     2686 2022-12-07 20:27:21.445222 TrainerBase-2.9.7/trainerbase/gameobject.py
--rw-r--r--   0        0        0     6434 2023-04-10 21:02:16.760340 TrainerBase-2.9.7/trainerbase/gui.py
--rw-r--r--   0        0        0     1332 2023-04-10 20:47:38.678906 TrainerBase-2.9.7/trainerbase/memory.py
--rw-r--r--   0        0        0     2518 2022-12-09 12:40:11.890792 TrainerBase-2.9.7/trainerbase/scriptengine.py
--rw-r--r--   0        0        0        0 2022-11-27 19:37:39.031619 TrainerBase-2.9.7/trainerbase/template/__init__.py
--rw-r--r--   0        0        0       56 2022-12-03 21:05:33.189289 TrainerBase-2.9.7/trainerbase/template/config.py
--rw-r--r--   0        0        0      758 2022-12-03 21:05:33.189289 TrainerBase-2.9.7/trainerbase/template/gui.py
--rw-r--r--   0        0        0       95 2022-12-03 21:05:33.190297 TrainerBase-2.9.7/trainerbase/template/injections.py
--rw-r--r--   0        0        0      302 2022-12-07 20:41:59.080957 TrainerBase-2.9.7/trainerbase/template/main.py
--rw-r--r--   0        0        0      133 2022-12-04 16:32:33.988485 TrainerBase-2.9.7/trainerbase/template/objects.py
--rw-r--r--   0        0        0      233 2022-12-07 19:31:24.358010 TrainerBase-2.9.7/trainerbase/template/scripts.py
--rw-r--r--   0        0        0      493 2023-04-10 21:40:22.796319 TrainerBase-2.9.7/trainerbase/tts.py
--rw-r--r--   0        0        0      128 2022-12-03 21:05:33.192296 TrainerBase-2.9.7/trainerbase/use_trainer_template.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 TrainerBase-2.9.7/PKG-INFO
+-rwxr-xr-x   0        0        0   117248 2022-02-21 09:32:45.418863 TrainerBase-2.9.8/fasm/FASM.EXE
+-rw-r--r--   0        0        0     1103 2023-04-02 15:26:24.974155 TrainerBase-2.9.8/LICENSE
+-rw-r--r--   0        0        0      788 2023-04-10 21:45:43.888196 TrainerBase-2.9.8/pyproject.toml
+-rw-r--r--   0        0        0      170 2022-11-27 19:37:39.028579 TrainerBase-2.9.8/README.md
+-rw-r--r--   0        0        0        0 2022-11-27 19:37:39.030089 TrainerBase-2.9.8/trainerbase/__init__.py
+-rw-r--r--   0        0        0     3464 2023-04-10 20:48:57.586831 TrainerBase-2.9.8/trainerbase/codeinjection.py
+-rw-r--r--   0        0        0     1019 2023-04-10 20:37:50.924352 TrainerBase-2.9.8/trainerbase/common.py
+-rw-r--r--   0        0        0     2686 2022-12-07 20:27:21.445222 TrainerBase-2.9.8/trainerbase/gameobject.py
+-rw-r--r--   0        0        0     6434 2023-04-10 21:02:16.760340 TrainerBase-2.9.8/trainerbase/gui.py
+-rw-r--r--   0        0        0     1332 2023-04-10 20:47:38.678906 TrainerBase-2.9.8/trainerbase/memory.py
+-rw-r--r--   0        0        0     2518 2022-12-09 12:40:11.890792 TrainerBase-2.9.8/trainerbase/scriptengine.py
+-rw-r--r--   0        0        0        0 2022-11-27 19:37:39.031619 TrainerBase-2.9.8/trainerbase/template/__init__.py
+-rw-r--r--   0        0        0       56 2022-12-03 21:05:33.189289 TrainerBase-2.9.8/trainerbase/template/config.py
+-rw-r--r--   0        0        0      758 2022-12-03 21:05:33.189289 TrainerBase-2.9.8/trainerbase/template/gui.py
+-rw-r--r--   0        0        0       95 2022-12-03 21:05:33.190297 TrainerBase-2.9.8/trainerbase/template/injections.py
+-rw-r--r--   0        0        0      302 2022-12-07 20:41:59.080957 TrainerBase-2.9.8/trainerbase/template/main.py
+-rw-r--r--   0        0        0      133 2022-12-04 16:32:33.988485 TrainerBase-2.9.8/trainerbase/template/objects.py
+-rw-r--r--   0        0        0      233 2022-12-07 19:31:24.358010 TrainerBase-2.9.8/trainerbase/template/scripts.py
+-rw-r--r--   0        0        0      545 2023-04-10 21:45:22.647705 TrainerBase-2.9.8/trainerbase/tts.py
+-rw-r--r--   0        0        0      128 2022-12-03 21:05:33.192296 TrainerBase-2.9.8/trainerbase/use_trainer_template.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 TrainerBase-2.9.8/PKG-INFO
```

### Comparing `TrainerBase-2.9.7/fasm/FASM.EXE` & `TrainerBase-2.9.8/fasm/FASM.EXE`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.7/LICENSE` & `TrainerBase-2.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.7/pyproject.toml` & `TrainerBase-2.9.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 dev = [
     "black>=22.10.0",
     "pylint>=2.15.7",
 ]
 
 [project]
 name = "TrainerBase"
-version = "2.9.7"
+version = "2.9.8"
 description = "Template/Framework to create game trainers"
 authors = [
     { name = "v01d", email = "v01d@v01d.ru" },
     { name = "doomayka", email = "zd@doomayka.ru" },
 ]
 dependencies = [
     "pymem>=1.10.0",
```

### Comparing `TrainerBase-2.9.7/trainerbase/codeinjection.py` & `TrainerBase-2.9.8/trainerbase/codeinjection.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.7/trainerbase/common.py` & `TrainerBase-2.9.8/trainerbase/common.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.7/trainerbase/gameobject.py` & `TrainerBase-2.9.8/trainerbase/gameobject.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.7/trainerbase/gui.py` & `TrainerBase-2.9.8/trainerbase/gui.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.7/trainerbase/memory.py` & `TrainerBase-2.9.8/trainerbase/memory.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.7/trainerbase/scriptengine.py` & `TrainerBase-2.9.8/trainerbase/scriptengine.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.7/trainerbase/template/gui.py` & `TrainerBase-2.9.8/trainerbase/template/gui.py`

 * *Files identical despite different names*


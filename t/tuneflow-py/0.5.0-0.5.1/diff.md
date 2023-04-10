# Comparing `tmp/tuneflow-py-0.5.0.tar.gz` & `tmp/tuneflow-py-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneflow-py-0.5.0.tar", last modified: Mon Apr 10 06:27:07 2023, max compression
+gzip compressed data, was "tuneflow-py-0.5.1.tar", last modified: Mon Apr 10 18:45:31 2023, max compression
```

## Comparing `tuneflow-py-0.5.0.tar` & `tuneflow-py-0.5.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 06:27:07.951477 tuneflow-py-0.5.0/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1065 2023-01-10 14:03:44.000000 tuneflow-py-0.5.0/LICENSE
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-10 06:27:07.951477 tuneflow-py-0.5.0/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3809 2023-03-06 23:39:23.000000 tuneflow-py-0.5.0/README.md
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1288 2023-04-10 06:26:23.000000 tuneflow-py-0.5.0/pyproject.toml
--rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-04-10 06:27:07.951477 tuneflow-py-0.5.0/setup.cfg
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 06:27:07.941477 tuneflow-py-0.5.0/src/
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 06:27:07.941477 tuneflow-py-0.5.0/src/tuneflow_py/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1155 2023-04-10 06:26:06.000000 tuneflow-py-0.5.0/src/tuneflow_py/__init__.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1987 2023-02-28 00:04:43.000000 tuneflow-py-0.5.0/src/tuneflow_py/base_plugin.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 06:27:07.951477 tuneflow-py-0.5.0/src/tuneflow_py/descriptors/
--rw-r--r--   0 panacea   (1000) panacea   (1000)      922 2023-03-30 21:40:36.000000 tuneflow-py-0.5.0/src/tuneflow_py/descriptors/audio_plugin_descriptor.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1579 2023-03-30 21:53:02.000000 tuneflow-py-0.5.0/src/tuneflow_py/descriptors/clip_descriptor.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      439 2023-03-30 21:53:05.000000 tuneflow-py-0.5.0/src/tuneflow_py/descriptors/common.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4221 2023-03-30 21:53:07.000000 tuneflow-py-0.5.0/src/tuneflow_py/descriptors/param.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4407 2023-03-30 21:53:10.000000 tuneflow-py-0.5.0/src/tuneflow_py/descriptors/plugin.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)       71 2023-03-30 21:53:12.000000 tuneflow-py-0.5.0/src/tuneflow_py/descriptors/text.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5575 2023-03-31 22:25:01.000000 tuneflow-py-0.5.0/src/tuneflow_py/descriptors/widget.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 06:27:07.951477 tuneflow-py-0.5.0/src/tuneflow_py/models/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3128 2023-03-01 03:02:02.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/audio_plugin.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    17158 2023-03-31 07:33:41.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/automation.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    23875 2023-03-31 07:45:07.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      979 2023-04-10 06:26:06.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/marker.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5275 2023-02-22 00:50:28.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/note.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 06:27:07.951477 tuneflow-py-0.5.0/src/tuneflow_py/models/protos/
--rw-r--r--   0 panacea   (1000) panacea   (1000)    69365 2023-04-10 06:26:06.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/protos/song_pb2.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    25532 2023-04-10 06:26:06.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/song.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      873 2023-03-01 22:09:14.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/tempo.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1093 2023-02-22 00:28:50.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/time_signature.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    16387 2023-03-31 16:53:25.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/track.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     6210 2023-03-29 01:48:05.000000 tuneflow-py-0.5.0/src/tuneflow_py/utils.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 06:27:07.941477 tuneflow-py-0.5.0/src/tuneflow_py.egg-info/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-10 06:27:07.000000 tuneflow-py-0.5.0/src/tuneflow_py.egg-info/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1113 2023-04-10 06:27:07.000000 tuneflow-py-0.5.0/src/tuneflow_py.egg-info/SOURCES.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-04-10 06:27:07.000000 tuneflow-py-0.5.0/src/tuneflow_py.egg-info/dependency_links.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       96 2023-04-10 06:27:07.000000 tuneflow-py-0.5.0/src/tuneflow_py.egg-info/requires.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       12 2023-04-10 06:27:07.000000 tuneflow-py-0.5.0/src/tuneflow_py.egg-info/top_level.txt
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 06:27:07.951477 tuneflow-py-0.5.0/test/
--rw-r--r--   0 panacea   (1000) panacea   (1000)    21690 2023-02-24 04:10:42.000000 tuneflow-py-0.5.0/test/test_audio_clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    24170 2023-03-31 07:02:16.000000 tuneflow-py-0.5.0/test/test_automation.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     6655 2023-04-10 06:26:06.000000 tuneflow-py-0.5.0/test/test_marker.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    33568 2023-03-09 18:17:16.000000 tuneflow-py-0.5.0/test/test_midi_clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    24300 2023-02-22 00:33:25.000000 tuneflow-py-0.5.0/test/test_note.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    14091 2023-03-31 16:54:59.000000 tuneflow-py-0.5.0/test/test_song.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3583 2023-03-31 08:05:14.000000 tuneflow-py-0.5.0/test/test_track.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2071 2023-02-16 23:10:13.000000 tuneflow-py-0.5.0/test/test_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1065 2023-01-10 14:03:44.000000 tuneflow-py-0.5.1/LICENSE
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3809 2023-03-06 23:39:23.000000 tuneflow-py-0.5.1/README.md
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1288 2023-04-10 18:44:50.000000 tuneflow-py-0.5.1/pyproject.toml
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/setup.cfg
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/src/
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/src/tuneflow_py/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1155 2023-04-10 06:26:06.000000 tuneflow-py-0.5.1/src/tuneflow_py/__init__.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1987 2023-02-28 00:04:43.000000 tuneflow-py-0.5.1/src/tuneflow_py/base_plugin.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/src/tuneflow_py/descriptors/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      922 2023-03-30 21:40:36.000000 tuneflow-py-0.5.1/src/tuneflow_py/descriptors/audio_plugin_descriptor.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1579 2023-03-30 21:53:02.000000 tuneflow-py-0.5.1/src/tuneflow_py/descriptors/clip_descriptor.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      439 2023-03-30 21:53:05.000000 tuneflow-py-0.5.1/src/tuneflow_py/descriptors/common.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4221 2023-03-30 21:53:07.000000 tuneflow-py-0.5.1/src/tuneflow_py/descriptors/param.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4407 2023-03-30 21:53:10.000000 tuneflow-py-0.5.1/src/tuneflow_py/descriptors/plugin.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       71 2023-03-30 21:53:12.000000 tuneflow-py-0.5.1/src/tuneflow_py/descriptors/text.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5575 2023-03-31 22:25:01.000000 tuneflow-py-0.5.1/src/tuneflow_py/descriptors/widget.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/src/tuneflow_py/models/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3128 2023-03-01 03:02:02.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/audio_plugin.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    17158 2023-03-31 07:33:41.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/automation.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    23875 2023-03-31 07:45:07.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1305 2023-04-10 18:15:27.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/marker.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5275 2023-02-22 00:50:28.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/note.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/src/tuneflow_py/models/protos/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    70682 2023-04-10 18:11:02.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/protos/song_pb2.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    25607 2023-04-10 18:24:50.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/song.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      873 2023-03-01 22:09:14.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/tempo.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1093 2023-02-22 00:28:50.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/time_signature.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    16387 2023-03-31 16:53:25.000000 tuneflow-py-0.5.1/src/tuneflow_py/models/track.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     6210 2023-03-29 01:48:05.000000 tuneflow-py-0.5.1/src/tuneflow_py/utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/src/tuneflow_py.egg-info/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-10 18:45:31.000000 tuneflow-py-0.5.1/src/tuneflow_py.egg-info/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1113 2023-04-10 18:45:31.000000 tuneflow-py-0.5.1/src/tuneflow_py.egg-info/SOURCES.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-04-10 18:45:31.000000 tuneflow-py-0.5.1/src/tuneflow_py.egg-info/dependency_links.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       96 2023-04-10 18:45:31.000000 tuneflow-py-0.5.1/src/tuneflow_py.egg-info/requires.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       12 2023-04-10 18:45:31.000000 tuneflow-py-0.5.1/src/tuneflow_py.egg-info/top_level.txt
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 18:45:31.446440 tuneflow-py-0.5.1/test/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    21690 2023-02-24 04:10:42.000000 tuneflow-py-0.5.1/test/test_audio_clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    24170 2023-03-31 07:02:16.000000 tuneflow-py-0.5.1/test/test_automation.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     8001 2023-04-10 18:37:18.000000 tuneflow-py-0.5.1/test/test_marker.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    33568 2023-03-09 18:17:16.000000 tuneflow-py-0.5.1/test/test_midi_clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    24300 2023-02-22 00:33:25.000000 tuneflow-py-0.5.1/test/test_note.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    14091 2023-03-31 16:54:59.000000 tuneflow-py-0.5.1/test/test_song.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3583 2023-03-31 08:05:14.000000 tuneflow-py-0.5.1/test/test_track.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2071 2023-02-16 23:10:13.000000 tuneflow-py-0.5.1/test/test_utils.py
```

### Comparing `tuneflow-py-0.5.0/LICENSE` & `tuneflow-py-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/PKG-INFO` & `tuneflow-py-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-py
-Version: 0.5.0
+Version: 0.5.1
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: TuneFlow <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-py-0.5.0/README.md` & `tuneflow-py-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/pyproject.toml` & `tuneflow-py-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "tuneflow-py"
-version = "0.5.0"
+version = "0.5.1"
 authors = [{ name = "TuneFlow", email = "contact@info.tuneflow.com" }]
 description = "Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [
   "AI",
   "music",
```

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py/__init__.py` & `tuneflow-py-0.5.1/src/tuneflow_py/__init__.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py/base_plugin.py` & `tuneflow-py-0.5.1/src/tuneflow_py/base_plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py/descriptors/audio_plugin_descriptor.py` & `tuneflow-py-0.5.1/src/tuneflow_py/descriptors/audio_plugin_descriptor.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py/descriptors/clip_descriptor.py` & `tuneflow-py-0.5.1/src/tuneflow_py/descriptors/clip_descriptor.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py/descriptors/param.py` & `tuneflow-py-0.5.1/src/tuneflow_py/descriptors/param.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py/descriptors/plugin.py` & `tuneflow-py-0.5.1/src/tuneflow_py/descriptors/plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py/descriptors/widget.py` & `tuneflow-py-0.5.1/src/tuneflow_py/descriptors/widget.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py/models/audio_plugin.py` & `tuneflow-py-0.5.1/src/tuneflow_py/models/audio_plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py/models/automation.py` & `tuneflow-py-0.5.1/src/tuneflow_py/models/automation.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py/models/clip.py` & `tuneflow-py-0.5.1/src/tuneflow_py/models/clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py/models/marker.py` & `tuneflow-py-0.5.1/src/tuneflow_py/models/marker.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,29 +2,37 @@
 from tuneflow_py.models.protos import song_pb2
 
 StructureType = song_pb2.StructureMarker.StructureType
 
 
 class StructureMarker:
     def __init__(self, song, tick:int=None, type: int | None = None,
-                 proto: song_pb2.StructureMarker | None = None) -> None:
+                 custom_name: str | None = None, proto: song_pb2.StructureMarker | None = None) -> None:
         if song is None:
             raise Exception('song must be provided when creating a track')
         self.song = song
         if proto is not None:
             self._proto = proto
             return
         self._proto = song_pb2.StructureMarker()
         self._proto.type = type if type is not None else StructureType.INTRO
         self._proto.tick = tick if tick is not None else 0
+        if type == StructureType.CUSTOM:
+            self._proto.custom_name = custom_name if custom_name is not None else ''
 
     def get_tick(self) -> int:
         return self._proto.tick
 
     def set_tick(self, tick: int):
         self._proto.tick = tick
 
     def get_type(self) -> StructureType:
         return self._proto.type
 
     def set_type(self, type: StructureType):
-        self._proto.type = type
+        self._proto.type = type
+    
+    def set_custom_name(self, name: str):
+        self._proto.custom_name = name
+    
+    def get_custom_name(self) -> str:
+        return self._proto.custom_name
```

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py/models/note.py` & `tuneflow-py-0.5.1/src/tuneflow_py/models/note.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py/models/protos/song_pb2.py` & `tuneflow-py-0.5.1/src/tuneflow_py/models/protos/song_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='song.proto',
   package='song',
   syntax='proto2',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\nsong.proto\x12\x04song\"\x7f\n\x04Note\x12\r\n\x05pitch\x18\x01 \x01(\x05\x12\x10\n\x08velocity\x18\x02 \x01(\x05\x12\x12\n\nstart_tick\x18\x03 \x01(\x05\x12\x12\n\nstart_time\x18\x04 \x01(\x02\x12\x10\n\x08\x65nd_tick\x18\x05 \x01(\x05\x12\x10\n\x08\x65nd_time\x18\x06 \x01(\x02\x12\n\n\x02id\x18\x07 \x01(\r\"6\n\nTempoEvent\x12\r\n\x05ticks\x18\x01 \x01(\x05\x12\x0b\n\x03\x62pm\x18\x02 \x01(\x02\x12\x0c\n\x04time\x18\x03 \x01(\x02\"K\n\x12TimeSignatureEvent\x12\r\n\x05ticks\x18\x01 \x01(\x05\x12\x11\n\tnumerator\x18\x02 \x01(\x05\x12\x13\n\x0b\x64\x65nominator\x18\x03 \x01(\x05\"2\n\x0eInstrumentInfo\x12\x0f\n\x07program\x18\x01 \x01(\x05\x12\x0f\n\x07is_drum\x18\x02 \x01(\x08\"f\n\x0f\x41udioPluginInfo\x12\r\n\x05tf_id\x18\x01 \x01(\t\x12\x12\n\nis_enabled\x18\x02 \x01(\x08\x12\x19\n\x11local_instance_id\x18\x03 \x01(\t\x12\x15\n\rbase64_states\x18\x04 \x01(\t\"\xb2\x01\n\x10\x41utomationTarget\x12/\n\x04type\x18\x01 \x01(\x0e\x32!.song.AutomationTarget.TargetType\x12\x17\n\x0f\x61udio_plugin_id\x18\x02 \x01(\t\x12\x10\n\x08param_id\x18\x03 \x01(\t\"B\n\nTargetType\x12\r\n\tUNDEFINED\x10\x00\x12\n\n\x06VOLUME\x10\x01\x12\x07\n\x03PAN\x10\x02\x12\x10\n\x0c\x41UDIO_PLUGIN\x10\x03\"\x8c\x01\n\x0f\x41utomationValue\x12\x30\n\x06points\x18\x01 \x03(\x0b\x32 .song.AutomationValue.ParamValue\x12\x10\n\x08\x64isabled\x18\x02 \x01(\x08\x1a\x35\n\nParamValue\x12\x0c\n\x04tick\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x02\x12\n\n\x02id\x18\x03 \x01(\x05\"\xc4\x01\n\x0e\x41utomationData\x12\'\n\x07targets\x18\x01 \x03(\x0b\x32\x16.song.AutomationTarget\x12=\n\rtarget_values\x18\x02 \x03(\x0b\x32&.song.AutomationData.TargetValuesEntry\x1aJ\n\x11TargetValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.song.AutomationValue:\x02\x38\x01\"\xef\x01\n\tTrackSend\x12\x17\n\x0foutput_bus_rank\x18\x01 \x01(\x05\x12\x12\n\ngain_level\x18\x02 \x01(\x02\x12\x33\n\x08position\x18\x03 \x01(\x0e\x32!.song.TrackSend.TrackSendPosition\x12\r\n\x05muted\x18\x04 \x01(\x08\"q\n\x11TrackSendPosition\x12!\n\x1dUNDEFINED_TRACK_SEND_POSITION\x10\x00\x12\x1b\n\x17SEND_POSITION_PRE_FADER\x10\x01\x12\x1c\n\x18SEND_POSITION_POST_FADER\x10\x02\"\xca\x01\n\x0bTrackOutput\x12/\n\x04type\x18\x01 \x01(\x0e\x32!.song.TrackOutput.TrackOutputType\x12\x10\n\x08track_id\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65vice_name\x18\x03 \x01(\t\"c\n\x0fTrackOutputType\x12\x1f\n\x1bUNDEFINED_TRACK_OUTPUT_TYPE\x10\x00\x12\x17\n\x13TRACK_OUTPUT_DEVICE\x10\x01\x12\x16\n\x12TRACK_OUTPUT_TRACK\x10\x02\"&\n\x0c\x41uxTrackData\x12\x16\n\x0einput_bus_rank\x18\x01 \x01(\x05\"\xe2\x05\n\x05Track\x12(\n\ninstrument\x18\x01 \x01(\x0b\x32\x14.song.InstrumentInfo\x12\x1d\n\x05notes\x18\x02 \x03(\x0b\x32\n.song.NoteB\x02\x18\x01\x12\x33\n\x15suggested_instruments\x18\x03 \x03(\x0b\x32\x14.song.InstrumentInfo\x12\x0c\n\x04uuid\x18\x04 \x01(\t\x12\x0e\n\x06volume\x18\x05 \x01(\x02\x12\x0c\n\x04solo\x18\x06 \x01(\x08\x12\r\n\x05muted\x18\x07 \x01(\x08\x12\x0c\n\x04rank\x18\x08 \x01(\x05\x12\x18\n\x10track_start_tick\x18\t \x01(\x05\x12\x16\n\x0etrack_end_tick\x18\n \x01(\x05\x12-\n\x0esampler_plugin\x18\x0b \x01(\x0b\x32\x15.song.AudioPluginInfo\x12\x32\n\x0c\x61udio_plugin\x18\x0c \x03(\x0b\x32\x1c.song.Track.AudioPluginEntry\x12\x19\n\x05\x63lips\x18\r \x03(\x0b\x32\n.song.Clip\x12\x0b\n\x03pan\x18\x0e \x01(\x05\x12\x0c\n\x04name\x18\x0f \x01(\t\x12(\n\nautomation\x18\x10 \x01(\x0b\x32\x14.song.AutomationData\x12\x1d\n\x04type\x18\x11 \x01(\x0e\x32\x0f.song.TrackType\x12*\n\x0e\x61ux_track_data\x18\x12 \x01(\x0b\x32\x12.song.AuxTrackData\x12%\n\x05sends\x18\x13 \x03(\x0b\x32\x16.song.Track.SendsEntry\x12!\n\x06output\x18\x14 \x01(\x0b\x32\x11.song.TrackOutput\x1aI\n\x10\x41udioPluginEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.song.AudioPluginInfo:\x02\x38\x01\x1a=\n\nSendsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.song.TrackSend:\x02\x38\x01\")\n\tAudioData\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\t\"s\n\rAudioClipData\x12\x17\n\x0f\x61udio_file_path\x18\x01 \x01(\t\x12\x12\n\nstart_tick\x18\x02 \x01(\x05\x12\x10\n\x08\x64uration\x18\x03 \x01(\x01\x12#\n\naudio_data\x18\x04 \x01(\x0b\x32\x0f.song.AudioData\"\xb7\x01\n\x04\x43lip\x12\n\n\x02id\x18\x01 \x01(\t\x12\x17\n\x0f\x63lip_start_tick\x18\x02 \x01(\x05\x12\x15\n\rclip_end_tick\x18\x03 \x01(\x05\x12\x19\n\x05notes\x18\x04 \x03(\x0b\x32\n.song.Note\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x1c\n\x04type\x18\x06 \x01(\x0e\x32\x0e.song.ClipType\x12,\n\x0f\x61udio_clip_data\x18\x07 \x01(\x0b\x32\x13.song.AudioClipData\"\xa9\x01\n\x0fStructureMarker\x12\x0c\n\x04tick\x18\x01 \x01(\x05\x12\x31\n\x04type\x18\x02 \x01(\x0e\x32#.song.StructureMarker.StructureType\"U\n\rStructureType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05INTRO\x10\x01\x12\t\n\x05VERSE\x10\x02\x12\n\n\x06\x43HORUS\x10\x03\x12\n\n\x06\x42RIDGE\x10\x04\x12\t\n\x05OUTRO\x10\x05\"!\n\x03\x42us\x12\x0c\n\x04rank\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x92\x02\n\x04Song\x12\x0b\n\x03PPQ\x18\x01 \x01(\x05\x12 \n\x06tempos\x18\x02 \x03(\x0b\x32\x10.song.TempoEvent\x12\x31\n\x0ftime_signatures\x18\x03 \x03(\x0b\x32\x18.song.TimeSignatureEvent\x12\x11\n\tlast_tick\x18\x04 \x01(\x05\x12\x10\n\x08\x64uration\x18\x05 \x01(\x02\x12\x1b\n\x06tracks\x18\x06 \x03(\x0b\x32\x0b.song.Track\x12!\n\x0cmaster_track\x18\x07 \x01(\x0b\x32\x0b.song.Track\x12)\n\nstructures\x18\x08 \x03(\x0b\x32\x15.song.StructureMarker\x12\x18\n\x05\x62uses\x18\t \x03(\x0b\x32\t.song.Bus*b\n\tTrackType\x12\x13\n\x0fUNDEFINED_TRACK\x10\x00\x12\x0e\n\nMIDI_TRACK\x10\x01\x12\x0f\n\x0b\x41UDIO_TRACK\x10\x02\x12\x10\n\x0cMASTER_TRACK\x10\x03\x12\r\n\tAUX_TRACK\x10\x04*=\n\x08\x43lipType\x12\x12\n\x0eUNDEFINED_CLIP\x10\x00\x12\r\n\tMIDI_CLIP\x10\x01\x12\x0e\n\nAUDIO_CLIP\x10\x02'
+  serialized_pb=b'\n\nsong.proto\x12\x04song\"\x7f\n\x04Note\x12\r\n\x05pitch\x18\x01 \x01(\x05\x12\x10\n\x08velocity\x18\x02 \x01(\x05\x12\x12\n\nstart_tick\x18\x03 \x01(\x05\x12\x12\n\nstart_time\x18\x04 \x01(\x02\x12\x10\n\x08\x65nd_tick\x18\x05 \x01(\x05\x12\x10\n\x08\x65nd_time\x18\x06 \x01(\x02\x12\n\n\x02id\x18\x07 \x01(\r\"6\n\nTempoEvent\x12\r\n\x05ticks\x18\x01 \x01(\x05\x12\x0b\n\x03\x62pm\x18\x02 \x01(\x02\x12\x0c\n\x04time\x18\x03 \x01(\x02\"K\n\x12TimeSignatureEvent\x12\r\n\x05ticks\x18\x01 \x01(\x05\x12\x11\n\tnumerator\x18\x02 \x01(\x05\x12\x13\n\x0b\x64\x65nominator\x18\x03 \x01(\x05\"2\n\x0eInstrumentInfo\x12\x0f\n\x07program\x18\x01 \x01(\x05\x12\x0f\n\x07is_drum\x18\x02 \x01(\x08\"f\n\x0f\x41udioPluginInfo\x12\r\n\x05tf_id\x18\x01 \x01(\t\x12\x12\n\nis_enabled\x18\x02 \x01(\x08\x12\x19\n\x11local_instance_id\x18\x03 \x01(\t\x12\x15\n\rbase64_states\x18\x04 \x01(\t\"\xb2\x01\n\x10\x41utomationTarget\x12/\n\x04type\x18\x01 \x01(\x0e\x32!.song.AutomationTarget.TargetType\x12\x17\n\x0f\x61udio_plugin_id\x18\x02 \x01(\t\x12\x10\n\x08param_id\x18\x03 \x01(\t\"B\n\nTargetType\x12\r\n\tUNDEFINED\x10\x00\x12\n\n\x06VOLUME\x10\x01\x12\x07\n\x03PAN\x10\x02\x12\x10\n\x0c\x41UDIO_PLUGIN\x10\x03\"\x8c\x01\n\x0f\x41utomationValue\x12\x30\n\x06points\x18\x01 \x03(\x0b\x32 .song.AutomationValue.ParamValue\x12\x10\n\x08\x64isabled\x18\x02 \x01(\x08\x1a\x35\n\nParamValue\x12\x0c\n\x04tick\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x02\x12\n\n\x02id\x18\x03 \x01(\x05\"\xc4\x01\n\x0e\x41utomationData\x12\'\n\x07targets\x18\x01 \x03(\x0b\x32\x16.song.AutomationTarget\x12=\n\rtarget_values\x18\x02 \x03(\x0b\x32&.song.AutomationData.TargetValuesEntry\x1aJ\n\x11TargetValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.song.AutomationValue:\x02\x38\x01\"\xef\x01\n\tTrackSend\x12\x17\n\x0foutput_bus_rank\x18\x01 \x01(\x05\x12\x12\n\ngain_level\x18\x02 \x01(\x02\x12\x33\n\x08position\x18\x03 \x01(\x0e\x32!.song.TrackSend.TrackSendPosition\x12\r\n\x05muted\x18\x04 \x01(\x08\"q\n\x11TrackSendPosition\x12!\n\x1dUNDEFINED_TRACK_SEND_POSITION\x10\x00\x12\x1b\n\x17SEND_POSITION_PRE_FADER\x10\x01\x12\x1c\n\x18SEND_POSITION_POST_FADER\x10\x02\"\xca\x01\n\x0bTrackOutput\x12/\n\x04type\x18\x01 \x01(\x0e\x32!.song.TrackOutput.TrackOutputType\x12\x10\n\x08track_id\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65vice_name\x18\x03 \x01(\t\"c\n\x0fTrackOutputType\x12\x1f\n\x1bUNDEFINED_TRACK_OUTPUT_TYPE\x10\x00\x12\x17\n\x13TRACK_OUTPUT_DEVICE\x10\x01\x12\x16\n\x12TRACK_OUTPUT_TRACK\x10\x02\"&\n\x0c\x41uxTrackData\x12\x16\n\x0einput_bus_rank\x18\x01 \x01(\x05\"\xe2\x05\n\x05Track\x12(\n\ninstrument\x18\x01 \x01(\x0b\x32\x14.song.InstrumentInfo\x12\x1d\n\x05notes\x18\x02 \x03(\x0b\x32\n.song.NoteB\x02\x18\x01\x12\x33\n\x15suggested_instruments\x18\x03 \x03(\x0b\x32\x14.song.InstrumentInfo\x12\x0c\n\x04uuid\x18\x04 \x01(\t\x12\x0e\n\x06volume\x18\x05 \x01(\x02\x12\x0c\n\x04solo\x18\x06 \x01(\x08\x12\r\n\x05muted\x18\x07 \x01(\x08\x12\x0c\n\x04rank\x18\x08 \x01(\x05\x12\x18\n\x10track_start_tick\x18\t \x01(\x05\x12\x16\n\x0etrack_end_tick\x18\n \x01(\x05\x12-\n\x0esampler_plugin\x18\x0b \x01(\x0b\x32\x15.song.AudioPluginInfo\x12\x32\n\x0c\x61udio_plugin\x18\x0c \x03(\x0b\x32\x1c.song.Track.AudioPluginEntry\x12\x19\n\x05\x63lips\x18\r \x03(\x0b\x32\n.song.Clip\x12\x0b\n\x03pan\x18\x0e \x01(\x05\x12\x0c\n\x04name\x18\x0f \x01(\t\x12(\n\nautomation\x18\x10 \x01(\x0b\x32\x14.song.AutomationData\x12\x1d\n\x04type\x18\x11 \x01(\x0e\x32\x0f.song.TrackType\x12*\n\x0e\x61ux_track_data\x18\x12 \x01(\x0b\x32\x12.song.AuxTrackData\x12%\n\x05sends\x18\x13 \x03(\x0b\x32\x16.song.Track.SendsEntry\x12!\n\x06output\x18\x14 \x01(\x0b\x32\x11.song.TrackOutput\x1aI\n\x10\x41udioPluginEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.song.AudioPluginInfo:\x02\x38\x01\x1a=\n\nSendsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.song.TrackSend:\x02\x38\x01\")\n\tAudioData\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\t\"s\n\rAudioClipData\x12\x17\n\x0f\x61udio_file_path\x18\x01 \x01(\t\x12\x12\n\nstart_tick\x18\x02 \x01(\x05\x12\x10\n\x08\x64uration\x18\x03 \x01(\x01\x12#\n\naudio_data\x18\x04 \x01(\x0b\x32\x0f.song.AudioData\"\xb7\x01\n\x04\x43lip\x12\n\n\x02id\x18\x01 \x01(\t\x12\x17\n\x0f\x63lip_start_tick\x18\x02 \x01(\x05\x12\x15\n\rclip_end_tick\x18\x03 \x01(\x05\x12\x19\n\x05notes\x18\x04 \x03(\x0b\x32\n.song.Note\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x1c\n\x04type\x18\x06 \x01(\x0e\x32\x0e.song.ClipType\x12,\n\x0f\x61udio_clip_data\x18\x07 \x01(\x0b\x32\x13.song.AudioClipData\"\xf6\x01\n\x0fStructureMarker\x12\x0c\n\x04tick\x18\x01 \x01(\x05\x12\x31\n\x04type\x18\x02 \x01(\x0e\x32#.song.StructureMarker.StructureType\x12\x13\n\x0b\x63ustom_name\x18\x03 \x01(\t\"\x8c\x01\n\rStructureType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05INTRO\x10\x01\x12\t\n\x05VERSE\x10\x02\x12\n\n\x06\x43HORUS\x10\x03\x12\n\n\x06\x42RIDGE\x10\x04\x12\t\n\x05OUTRO\x10\x05\x12\x0e\n\nPRE_CHORUS\x10\x06\x12\x0f\n\x0bPOST_CHORUS\x10\x07\x12\x08\n\x04\x46ILL\x10\x08\x12\n\n\x06\x43USTOM\x10\t\"!\n\x03\x42us\x12\x0c\n\x04rank\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x92\x02\n\x04Song\x12\x0b\n\x03PPQ\x18\x01 \x01(\x05\x12 \n\x06tempos\x18\x02 \x03(\x0b\x32\x10.song.TempoEvent\x12\x31\n\x0ftime_signatures\x18\x03 \x03(\x0b\x32\x18.song.TimeSignatureEvent\x12\x11\n\tlast_tick\x18\x04 \x01(\x05\x12\x10\n\x08\x64uration\x18\x05 \x01(\x02\x12\x1b\n\x06tracks\x18\x06 \x03(\x0b\x32\x0b.song.Track\x12!\n\x0cmaster_track\x18\x07 \x01(\x0b\x32\x0b.song.Track\x12)\n\nstructures\x18\x08 \x03(\x0b\x32\x15.song.StructureMarker\x12\x18\n\x05\x62uses\x18\t \x03(\x0b\x32\t.song.Bus*b\n\tTrackType\x12\x13\n\x0fUNDEFINED_TRACK\x10\x00\x12\x0e\n\nMIDI_TRACK\x10\x01\x12\x0f\n\x0b\x41UDIO_TRACK\x10\x02\x12\x10\n\x0cMASTER_TRACK\x10\x03\x12\r\n\tAUX_TRACK\x10\x04*=\n\x08\x43lipType\x12\x12\n\x0eUNDEFINED_CLIP\x10\x00\x12\r\n\tMIDI_CLIP\x10\x01\x12\x0e\n\nAUDIO_CLIP\x10\x02'
 )
 
 _TRACKTYPE = _descriptor.EnumDescriptor(
   name='TrackType',
   full_name='song.TrackType',
   filename=None,
   file=DESCRIPTOR,
@@ -54,16 +54,16 @@
       name='AUX_TRACK', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3019,
-  serialized_end=3117,
+  serialized_start=3096,
+  serialized_end=3194,
 )
 _sym_db.RegisterEnumDescriptor(_TRACKTYPE)
 
 TrackType = enum_type_wrapper.EnumTypeWrapper(_TRACKTYPE)
 _CLIPTYPE = _descriptor.EnumDescriptor(
   name='ClipType',
   full_name='song.ClipType',
@@ -85,16 +85,16 @@
       name='AUDIO_CLIP', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3119,
-  serialized_end=3180,
+  serialized_start=3196,
+  serialized_end=3257,
 )
 _sym_db.RegisterEnumDescriptor(_CLIPTYPE)
 
 ClipType = enum_type_wrapper.EnumTypeWrapper(_CLIPTYPE)
 UNDEFINED_TRACK = 0
 MIDI_TRACK = 1
 AUDIO_TRACK = 2
@@ -233,22 +233,43 @@
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='OUTRO', index=5, number=5,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='PRE_CHORUS', index=6, number=6,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='POST_CHORUS', index=7, number=7,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='FILL', index=8, number=8,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='CUSTOM', index=9, number=9,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2620,
-  serialized_end=2705,
+  serialized_start=2642,
+  serialized_end=2782,
 )
 _sym_db.RegisterEnumDescriptor(_STRUCTUREMARKER_STRUCTURETYPE)
 
+
 _NOTE = _descriptor.Descriptor(
   name='Note',
   full_name='song.Note',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
@@ -1269,29 +1290,36 @@
     _descriptor.FieldDescriptor(
       name='type', full_name='song.StructureMarker.type', index=1,
       number=2, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='custom_name', full_name='song.StructureMarker.custom_name', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
     _STRUCTUREMARKER_STRUCTURETYPE,
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=2536,
-  serialized_end=2705,
+  serialized_end=2782,
 )
 
 
 _BUS = _descriptor.Descriptor(
   name='Bus',
   full_name='song.Bus',
   filename=None,
@@ -1321,16 +1349,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2707,
-  serialized_end=2740,
+  serialized_start=2784,
+  serialized_end=2817,
 )
 
 
 _SONG = _descriptor.Descriptor(
   name='Song',
   full_name='song.Song',
   filename=None,
@@ -1409,16 +1437,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2743,
-  serialized_end=3017,
+  serialized_start=2820,
+  serialized_end=3094,
 )
 
 _AUTOMATIONTARGET.fields_by_name['type'].enum_type = _AUTOMATIONTARGET_TARGETTYPE
 _AUTOMATIONTARGET_TARGETTYPE.containing_type = _AUTOMATIONTARGET
 _AUTOMATIONVALUE_PARAMVALUE.containing_type = _AUTOMATIONVALUE
 _AUTOMATIONVALUE.fields_by_name['points'].message_type = _AUTOMATIONVALUE_PARAMVALUE
 _AUTOMATIONDATA_TARGETVALUESENTRY.fields_by_name['value'].message_type = _AUTOMATIONVALUE
```

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py/models/song.py` & `tuneflow-py-0.5.1/src/tuneflow_py/models/song.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,30 +113,30 @@
             index = len(self._proto.structures) - 1
 
         if index == -1:
             return None
 
         return StructureMarker(song=self, proto=self._proto.structures[index])
 
-    def create_structure(self, tick: int, type: StructureType):
-        structure = StructureMarker(song=self, tick=tick, type=type)
+    def create_structure(self, tick: int, type: StructureType, custom_name: str | None = None):
+        structure = StructureMarker(song=self, tick=tick, type=type, custom_name=custom_name)
         self._proto.structures.append(structure._proto)
         structure._proto = self._proto.structures[-1]
         if len(self._proto.structures) == 1:
             # If there is only 1 structure, move it to the start.
             structure.set_tick(0)
         self._proto.structures.sort(key=lambda x: x.tick)
 
     def move_structure(self, structure_index: int, move_to_tick: int):
         structure = self.get_structure_at_index(structure_index)
         if not structure:
             return
         if structure_index <= 0:
             return
-        prev_structure = self.get_structure_at_index(structure_index - 1)
+        prev_structure : StructureMarker = self.get_structure_at_index(structure_index - 1)
         if prev_structure.get_tick() == move_to_tick:
             # Moved to another structure, delete it.
             self.remove_structure(structure_index - 1)
         elif structure_index < len(self.get_structures()) - 1:
             next_structure = self.get_structure_at_index(structure_index + 1)
             if next_structure and next_structure.get_tick() == move_to_tick:
                 # Moved to another time signature, delete it.
```

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py/models/tempo.py` & `tuneflow-py-0.5.1/src/tuneflow_py/models/tempo.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py/models/time_signature.py` & `tuneflow-py-0.5.1/src/tuneflow_py/models/time_signature.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py/models/track.py` & `tuneflow-py-0.5.1/src/tuneflow_py/models/track.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py/utils.py` & `tuneflow-py-0.5.1/src/tuneflow_py/utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py.egg-info/PKG-INFO` & `tuneflow-py-0.5.1/src/tuneflow_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-py
-Version: 0.5.0
+Version: 0.5.1
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: TuneFlow <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-py-0.5.0/src/tuneflow_py.egg-info/SOURCES.txt` & `tuneflow-py-0.5.1/src/tuneflow_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/test/test_audio_clip.py` & `tuneflow-py-0.5.1/test/test_audio_clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/test/test_automation.py` & `tuneflow-py-0.5.1/test/test_automation.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/test/test_marker.py` & `tuneflow-py-0.5.1/test/test_marker.py`

 * *Files 13% similar despite different names*

```diff
@@ -116,15 +116,14 @@
         song.move_structure(1, 0)
         assert len(song.get_structures()) == 2
         assert song.get_structures()[0].get_type() == StructureType.VERSE
         assert song.get_structures()[0].get_tick() == 0
         assert song.get_structures()[1].get_type() == StructureType.CHORUS
         assert song.get_structures()[1].get_tick() == 960
 
-
     def test_remove_structure_correctly(self):
         song = create_song()
         song.create_structure(tick=0, type=StructureType.INTRO)
         song.create_structure(tick=480, type=StructureType.VERSE)
         song.create_structure(tick=960, type=StructureType.CHORUS)
         assert len(song.get_structures()) == 3
         song.remove_structure(1)
@@ -133,10 +132,31 @@
         assert song.get_structures()[0].get_tick() == 0
         assert song.get_structures()[1].get_type() == StructureType.CHORUS
         assert song.get_structures()[1].get_tick() == 960
         song.remove_structure(3)
         song.remove_structure(-1)
         assert song.get_tempo_event_count() == 2
 
+    def test_create_custom_marker(self):
+        song = create_song()
+        song.create_structure(tick=0, type=StructureType.INTRO)
+        song.create_structure(tick=480, type=StructureType.CUSTOM, custom_name='myStructure')
+        song.create_structure(tick=960, type=StructureType.OUTRO, custom_name='myStructure')
+        self.assertEqual(song.get_structure_at_index(0).get_type(), StructureType.INTRO)
+        self.assertEqual(song.get_structure_at_index(1).get_type(), StructureType.CUSTOM)
+        self.assertEqual(song.get_structure_at_index(1).get_custom_name(), 'myStructure')
+        self.assertEqual(song.get_structure_at_index(2).get_custom_name(), '')
+
+    def test_update_custom_marker(self):
+        song = create_song()
+        song.create_structure(tick=0, type=StructureType.INTRO)
+        song.create_structure(tick=480, type=StructureType.CUSTOM, custom_name='myStructure')
+        song.create_structure(tick=960, type=StructureType.OUTRO, custom_name='myStructure')
+        self.assertEqual(song.get_structure_at_index(1).get_type(), StructureType.CUSTOM)
+        self.assertEqual(song.get_structure_at_index(1).get_custom_name(), 'myStructure')
+
+        song.get_structure_at_index(1).set_custom_name('myNewStructureName')
+        self.assertEqual(song.get_structure_at_index(1).get_custom_name(), 'myNewStructureName')
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `tuneflow-py-0.5.0/test/test_midi_clip.py` & `tuneflow-py-0.5.1/test/test_midi_clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/test/test_note.py` & `tuneflow-py-0.5.1/test/test_note.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/test/test_song.py` & `tuneflow-py-0.5.1/test/test_song.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/test/test_track.py` & `tuneflow-py-0.5.1/test/test_track.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.5.0/test/test_utils.py` & `tuneflow-py-0.5.1/test/test_utils.py`

 * *Files identical despite different names*


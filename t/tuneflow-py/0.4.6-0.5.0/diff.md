# Comparing `tmp/tuneflow-py-0.4.6.tar.gz` & `tmp/tuneflow-py-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneflow-py-0.4.6.tar", last modified: Sun Apr  9 02:41:02 2023, max compression
+gzip compressed data, was "tuneflow-py-0.5.0.tar", last modified: Mon Apr 10 06:27:07 2023, max compression
```

## Comparing `tuneflow-py-0.4.6.tar` & `tuneflow-py-0.5.0.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1065 2023-01-10 14:03:44.000000 tuneflow-py-0.4.6/LICENSE
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3809 2023-03-06 23:39:23.000000 tuneflow-py-0.4.6/README.md
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1288 2023-04-09 02:35:25.000000 tuneflow-py-0.4.6/pyproject.toml
--rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/setup.cfg
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/src/
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/src/tuneflow_py/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1086 2023-03-31 16:35:25.000000 tuneflow-py-0.4.6/src/tuneflow_py/__init__.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1987 2023-02-28 00:04:43.000000 tuneflow-py-0.4.6/src/tuneflow_py/base_plugin.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/src/tuneflow_py/descriptors/
--rw-r--r--   0 panacea   (1000) panacea   (1000)      922 2023-03-30 21:40:36.000000 tuneflow-py-0.4.6/src/tuneflow_py/descriptors/audio_plugin_descriptor.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1579 2023-03-30 21:53:02.000000 tuneflow-py-0.4.6/src/tuneflow_py/descriptors/clip_descriptor.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      439 2023-03-30 21:53:05.000000 tuneflow-py-0.4.6/src/tuneflow_py/descriptors/common.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4221 2023-03-30 21:53:07.000000 tuneflow-py-0.4.6/src/tuneflow_py/descriptors/param.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4407 2023-03-30 21:53:10.000000 tuneflow-py-0.4.6/src/tuneflow_py/descriptors/plugin.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)       71 2023-03-30 21:53:12.000000 tuneflow-py-0.4.6/src/tuneflow_py/descriptors/text.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5575 2023-03-31 22:25:01.000000 tuneflow-py-0.4.6/src/tuneflow_py/descriptors/widget.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/src/tuneflow_py/models/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3128 2023-03-01 03:02:02.000000 tuneflow-py-0.4.6/src/tuneflow_py/models/audio_plugin.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    17158 2023-03-31 07:33:41.000000 tuneflow-py-0.4.6/src/tuneflow_py/models/automation.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    23875 2023-03-31 07:45:07.000000 tuneflow-py-0.4.6/src/tuneflow_py/models/clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5275 2023-02-22 00:50:28.000000 tuneflow-py-0.4.6/src/tuneflow_py/models/note.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/src/tuneflow_py/models/protos/
--rw-r--r--   0 panacea   (1000) panacea   (1000)    69366 2023-03-31 16:43:26.000000 tuneflow-py-0.4.6/src/tuneflow_py/models/protos/song_pb2.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    22269 2023-04-05 05:19:38.000000 tuneflow-py-0.4.6/src/tuneflow_py/models/song.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      873 2023-03-01 22:09:14.000000 tuneflow-py-0.4.6/src/tuneflow_py/models/tempo.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1093 2023-02-22 00:28:50.000000 tuneflow-py-0.4.6/src/tuneflow_py/models/time_signature.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    16387 2023-03-31 16:53:25.000000 tuneflow-py-0.4.6/src/tuneflow_py/models/track.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     6210 2023-03-29 01:48:05.000000 tuneflow-py-0.4.6/src/tuneflow_py/utils.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/src/tuneflow_py.egg-info/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-09 02:41:02.000000 tuneflow-py-0.4.6/src/tuneflow_py.egg-info/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1060 2023-04-09 02:41:02.000000 tuneflow-py-0.4.6/src/tuneflow_py.egg-info/SOURCES.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-04-09 02:41:02.000000 tuneflow-py-0.4.6/src/tuneflow_py.egg-info/dependency_links.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       96 2023-04-09 02:41:02.000000 tuneflow-py-0.4.6/src/tuneflow_py.egg-info/requires.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       12 2023-04-09 02:41:02.000000 tuneflow-py-0.4.6/src/tuneflow_py.egg-info/top_level.txt
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/test/
--rw-r--r--   0 panacea   (1000) panacea   (1000)    21690 2023-02-24 04:10:42.000000 tuneflow-py-0.4.6/test/test_audio_clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    24170 2023-03-31 07:02:16.000000 tuneflow-py-0.4.6/test/test_automation.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    33568 2023-03-09 18:17:16.000000 tuneflow-py-0.4.6/test/test_midi_clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    24300 2023-02-22 00:33:25.000000 tuneflow-py-0.4.6/test/test_note.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    14091 2023-03-31 16:54:59.000000 tuneflow-py-0.4.6/test/test_song.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3583 2023-03-31 08:05:14.000000 tuneflow-py-0.4.6/test/test_track.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2071 2023-02-16 23:10:13.000000 tuneflow-py-0.4.6/test/test_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 06:27:07.951477 tuneflow-py-0.5.0/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1065 2023-01-10 14:03:44.000000 tuneflow-py-0.5.0/LICENSE
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-10 06:27:07.951477 tuneflow-py-0.5.0/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3809 2023-03-06 23:39:23.000000 tuneflow-py-0.5.0/README.md
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1288 2023-04-10 06:26:23.000000 tuneflow-py-0.5.0/pyproject.toml
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-04-10 06:27:07.951477 tuneflow-py-0.5.0/setup.cfg
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 06:27:07.941477 tuneflow-py-0.5.0/src/
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 06:27:07.941477 tuneflow-py-0.5.0/src/tuneflow_py/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1155 2023-04-10 06:26:06.000000 tuneflow-py-0.5.0/src/tuneflow_py/__init__.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1987 2023-02-28 00:04:43.000000 tuneflow-py-0.5.0/src/tuneflow_py/base_plugin.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 06:27:07.951477 tuneflow-py-0.5.0/src/tuneflow_py/descriptors/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      922 2023-03-30 21:40:36.000000 tuneflow-py-0.5.0/src/tuneflow_py/descriptors/audio_plugin_descriptor.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1579 2023-03-30 21:53:02.000000 tuneflow-py-0.5.0/src/tuneflow_py/descriptors/clip_descriptor.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      439 2023-03-30 21:53:05.000000 tuneflow-py-0.5.0/src/tuneflow_py/descriptors/common.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4221 2023-03-30 21:53:07.000000 tuneflow-py-0.5.0/src/tuneflow_py/descriptors/param.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4407 2023-03-30 21:53:10.000000 tuneflow-py-0.5.0/src/tuneflow_py/descriptors/plugin.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       71 2023-03-30 21:53:12.000000 tuneflow-py-0.5.0/src/tuneflow_py/descriptors/text.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5575 2023-03-31 22:25:01.000000 tuneflow-py-0.5.0/src/tuneflow_py/descriptors/widget.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 06:27:07.951477 tuneflow-py-0.5.0/src/tuneflow_py/models/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3128 2023-03-01 03:02:02.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/audio_plugin.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    17158 2023-03-31 07:33:41.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/automation.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    23875 2023-03-31 07:45:07.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      979 2023-04-10 06:26:06.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/marker.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5275 2023-02-22 00:50:28.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/note.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 06:27:07.951477 tuneflow-py-0.5.0/src/tuneflow_py/models/protos/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    69365 2023-04-10 06:26:06.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/protos/song_pb2.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    25532 2023-04-10 06:26:06.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/song.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      873 2023-03-01 22:09:14.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/tempo.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1093 2023-02-22 00:28:50.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/time_signature.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    16387 2023-03-31 16:53:25.000000 tuneflow-py-0.5.0/src/tuneflow_py/models/track.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     6210 2023-03-29 01:48:05.000000 tuneflow-py-0.5.0/src/tuneflow_py/utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 06:27:07.941477 tuneflow-py-0.5.0/src/tuneflow_py.egg-info/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-10 06:27:07.000000 tuneflow-py-0.5.0/src/tuneflow_py.egg-info/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1113 2023-04-10 06:27:07.000000 tuneflow-py-0.5.0/src/tuneflow_py.egg-info/SOURCES.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-04-10 06:27:07.000000 tuneflow-py-0.5.0/src/tuneflow_py.egg-info/dependency_links.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       96 2023-04-10 06:27:07.000000 tuneflow-py-0.5.0/src/tuneflow_py.egg-info/requires.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       12 2023-04-10 06:27:07.000000 tuneflow-py-0.5.0/src/tuneflow_py.egg-info/top_level.txt
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-10 06:27:07.951477 tuneflow-py-0.5.0/test/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    21690 2023-02-24 04:10:42.000000 tuneflow-py-0.5.0/test/test_audio_clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    24170 2023-03-31 07:02:16.000000 tuneflow-py-0.5.0/test/test_automation.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     6655 2023-04-10 06:26:06.000000 tuneflow-py-0.5.0/test/test_marker.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    33568 2023-03-09 18:17:16.000000 tuneflow-py-0.5.0/test/test_midi_clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    24300 2023-02-22 00:33:25.000000 tuneflow-py-0.5.0/test/test_note.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    14091 2023-03-31 16:54:59.000000 tuneflow-py-0.5.0/test/test_song.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3583 2023-03-31 08:05:14.000000 tuneflow-py-0.5.0/test/test_track.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2071 2023-02-16 23:10:13.000000 tuneflow-py-0.5.0/test/test_utils.py
```

### Comparing `tuneflow-py-0.4.6/LICENSE` & `tuneflow-py-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/PKG-INFO` & `tuneflow-py-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-py
-Version: 0.4.6
+Version: 0.5.0
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: TuneFlow <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-py-0.4.6/README.md` & `tuneflow-py-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/pyproject.toml` & `tuneflow-py-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "tuneflow-py"
-version = "0.4.6"
+version = "0.5.0"
 authors = [{ name = "TuneFlow", email = "contact@info.tuneflow.com" }]
 description = "Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [
   "AI",
   "music",
```

### Comparing `tuneflow-py-0.4.6/src/tuneflow_py/__init__.py` & `tuneflow-py-0.5.0/src/tuneflow_py/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from tuneflow_py.base_plugin import TuneflowPlugin
 from tuneflow_py.models.audio_plugin import AudioPlugin, get_audio_plugin_tuneflow_id, are_tuneflow_ids_equal, are_tuneflow_ids_equal_ignore_version, decode_audio_plugin_tuneflow_id
 from tuneflow_py.models.automation import AutomationTarget, AutomationTargetType, AutomationData, AutomationPoint, AutomationValue
 from tuneflow_py.models.clip import ClipType, Clip
 from tuneflow_py.models.note import Note
 from tuneflow_py.models.song import Song
 from tuneflow_py.models.tempo import TempoEvent
+from tuneflow_py.models.marker import StructureMarker, StructureType
 from tuneflow_py.models.time_signature import TimeSignatureEvent
 from tuneflow_py.models.track import TrackType, Track, TrackOutputType
 from tuneflow_py.descriptors.widget import *
 from tuneflow_py.descriptors.text import *
 from tuneflow_py.descriptors.param import *
 from tuneflow_py.descriptors.common import *
 from tuneflow_py.descriptors.audio_plugin_descriptor import *
```

### Comparing `tuneflow-py-0.4.6/src/tuneflow_py/base_plugin.py` & `tuneflow-py-0.5.0/src/tuneflow_py/base_plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/src/tuneflow_py/descriptors/audio_plugin_descriptor.py` & `tuneflow-py-0.5.0/src/tuneflow_py/descriptors/audio_plugin_descriptor.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/src/tuneflow_py/descriptors/clip_descriptor.py` & `tuneflow-py-0.5.0/src/tuneflow_py/descriptors/clip_descriptor.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/src/tuneflow_py/descriptors/param.py` & `tuneflow-py-0.5.0/src/tuneflow_py/descriptors/param.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/src/tuneflow_py/descriptors/plugin.py` & `tuneflow-py-0.5.0/src/tuneflow_py/descriptors/plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/src/tuneflow_py/descriptors/widget.py` & `tuneflow-py-0.5.0/src/tuneflow_py/descriptors/widget.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/src/tuneflow_py/models/audio_plugin.py` & `tuneflow-py-0.5.0/src/tuneflow_py/models/audio_plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/src/tuneflow_py/models/automation.py` & `tuneflow-py-0.5.0/src/tuneflow_py/models/automation.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/src/tuneflow_py/models/clip.py` & `tuneflow-py-0.5.0/src/tuneflow_py/models/clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/src/tuneflow_py/models/note.py` & `tuneflow-py-0.5.0/src/tuneflow_py/models/note.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/src/tuneflow_py/models/protos/song_pb2.py` & `tuneflow-py-0.5.0/src/tuneflow_py/models/protos/song_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,14 @@
   containing_type=None,
   serialized_options=None,
   serialized_start=2620,
   serialized_end=2705,
 )
 _sym_db.RegisterEnumDescriptor(_STRUCTUREMARKER_STRUCTURETYPE)
 
-
 _NOTE = _descriptor.Descriptor(
   name='Note',
   full_name='song.Note',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
```

### Comparing `tuneflow-py-0.4.6/src/tuneflow_py/models/song.py` & `tuneflow-py-0.5.0/src/tuneflow_py/models/song.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 from base64 import b64encode, b64decode
 from tuneflow_py.models.protos import song_pb2
 from tuneflow_py.models.track import Track, TrackType, TrackOutputType
+from tuneflow_py.models.marker import StructureMarker, StructureType
 from tuneflow_py.models.clip import Clip, ClipType
 from tuneflow_py.models.tempo import TempoEvent
 from tuneflow_py.models.time_signature import TimeSignatureEvent
 from tuneflow_py.models.automation import AutomationTarget, AutomationTargetType
 from tuneflow_py.models.audio_plugin import AudioPlugin, decode_audio_plugin_tuneflow_id
 from tuneflow_py.utils import db_to_volume_value, greater_equal, lower_than, lower_equal
-from miditoolkit.midi import MidiFile, TempoChange as ToolkitTempoChange, TimeSignature as ToolkitTimeSignature, Instrument, Note as ToolkitNote
+from miditoolkit.midi import MidiFile, TempoChange as ToolkitTempoChange, TimeSignature as ToolkitTimeSignature, \
+    Instrument, Note as ToolkitNote
 from types import SimpleNamespace
 from typing import List
 
 
 class Song:
     def __init__(self, proto: song_pb2.Song | None = None) -> None:
         if proto is not None:
@@ -69,24 +71,100 @@
         '''
         Removes a track from the song and returns it.
         '''
         track = self.get_track_by_id(track_id=track_id)
         if not track:
             return None
 
-        for i in range(self.get_track_count()-1, -1, -1):
+        for i in range(self.get_track_count() - 1, -1, -1):
             if self.get_track_at(i).get_id() == track_id:
                 del self._proto.tracks[i]
         # Delete dependencies.
         for dep_track in self.get_tracks():
             track_output = dep_track.get_output()
             if track_output is not None and track_output.get_type() == TrackOutputType.TRACK_OUTPUT_TRACK and track_output.get_track_id() == track_id:
                 dep_track.remove_output()
         return track
 
+    def get_structures(self):
+        return [StructureMarker(song=self, proto=structure_proto) for structure_proto in self._proto.structures]
+
+    def get_structure_at_index(self, index: int):
+        if index < 0 or index >= len(self._proto.structures):
+            return None
+        return StructureMarker(song=self, proto=self._proto.structures[index])
+
+    def get_structure_at_tick(self, tick: int):
+        def tick_to_structure_fn(tick):
+            return StructureMarker(song=self, tick=tick, type=StructureType.UNKNOWN)
+
+        def structure_to_tick_fn(structure):
+            return structure.get_tick()
+
+        index = lower_equal(
+            self.get_structures(),
+            tick_to_structure_fn(tick),
+            key=lambda s: structure_to_tick_fn(s),
+        )
+
+        if index < 0:
+            index = 0
+
+        if index >= len(self._proto.structures):
+            index = len(self._proto.structures) - 1
+
+        if index == -1:
+            return None
+
+        return StructureMarker(song=self, proto=self._proto.structures[index])
+
+    def create_structure(self, tick: int, type: StructureType):
+        structure = StructureMarker(song=self, tick=tick, type=type)
+        self._proto.structures.append(structure._proto)
+        structure._proto = self._proto.structures[-1]
+        if len(self._proto.structures) == 1:
+            # If there is only 1 structure, move it to the start.
+            structure.set_tick(0)
+        self._proto.structures.sort(key=lambda x: x.tick)
+
+    def move_structure(self, structure_index: int, move_to_tick: int):
+        structure = self.get_structure_at_index(structure_index)
+        if not structure:
+            return
+        if structure_index <= 0:
+            return
+        prev_structure = self.get_structure_at_index(structure_index - 1)
+        if prev_structure.get_tick() == move_to_tick:
+            # Moved to another structure, delete it.
+            self.remove_structure(structure_index - 1)
+        elif structure_index < len(self.get_structures()) - 1:
+            next_structure = self.get_structure_at_index(structure_index + 1)
+            if next_structure and next_structure.get_tick() == move_to_tick:
+                # Moved to another time signature, delete it.
+                self.remove_structure(structure_index + 1)
+        structure.set_tick(move_to_tick)
+        self._proto.structures.sort(key=lambda x: x.tick)
+
+    def update_structure_at_tick(self, tick: int, type: StructureType):
+        existing_structure = self.get_structure_at_tick(tick)
+        if existing_structure:
+            existing_structure.set_type(type)
+        else:
+            self.create_structure(tick, type)
+
+    def remove_structure(self, index: int):
+        if index < 0 or index >= len(self._proto.structures):
+            return
+        self._proto.structures.pop(index)
+        if len(self._proto.structures) > 0 and self._proto.structures[0].tick > 0:
+            # If the first structure of the remaining ones does not start
+            # from 0, move it to 0.
+            self._proto.structures[0].tick = 0
+        self._proto.structures.sort(key=lambda x: x.tick)
+
     def serialize(self):
         return b64encode(self._proto.SerializeToString()).decode('ascii')
 
     def serialize_to_bytestring(self) -> str:
         '''
         Note here the returned string is essentially bytes, just using the str form for convenience.
         See https://protobuf.dev/getting-started/pythontutorial/#parsing-serialization
@@ -110,20 +188,22 @@
         return Song(proto=song_proto)
 
     @staticmethod
     def from_midi(midi_obj: MidiFile):
         '''
         TODO: Replace proto operations with builtin methods.
         '''
+
         def scale_int_by(value, scale_factor):
-            return round(value*scale_factor)
+            return round(value * scale_factor)
+
         song = Song()
         song_proto = song._proto
         ppq_scale_factor = float(song_proto.PPQ) / \
-            float(midi_obj.ticks_per_beat)
+                           float(midi_obj.ticks_per_beat)
         # Add tempos and time signatures
         song.overwrite_tempo_changes([TempoEvent(ticks=scale_int_by(
             tempo_change.time, ppq_scale_factor), bpm=tempo_change.tempo) for tempo_change in midi_obj.tempo_changes])
         song.overwrite_time_signature_changes([
             TimeSignatureEvent(
                 ticks=scale_int_by(time_signature_change.time, ppq_scale_factor),
                 numerator=time_signature_change.numerator,
@@ -161,26 +241,26 @@
                 if control_change.number == 7:
                     # Volume CC
                     volume_ccs.append(control_change)
                 elif control_change.number == 10:
                     # Pan CC
                     pan_ccs.append(control_change)
             if len(volume_ccs) == 1:
-                song_track_proto.volume = volume_ccs[0].value/127.0
+                song_track_proto.volume = volume_ccs[0].value / 127.0
             elif len(volume_ccs) > 1:
                 volume_target = AutomationTarget(AutomationTargetType.VOLUME)
                 volume_target_id = volume_target.to_tf_automation_target_id()
                 song_track_proto.automation.targets.append(
                     volume_target._proto)
                 volume_target._proto = song_track_proto.automation.targets[-1]
                 volume_target_value = song_pb2.AutomationValue()
                 song_track_proto.automation.target_values[volume_target_id] = volume_target_value
                 for index, cc in enumerate(sorted(volume_ccs, key=lambda x: x.time)):
                     volume_target_value.points.add(tick=scale_int_by(
-                        cc.time, ppq_scale_factor), value=cc.value/127.0, id=index+1)
+                        cc.time, ppq_scale_factor), value=cc.value / 127.0, id=index + 1)
             else:
                 # Volume data missing from midi, set it to default.
                 song_track_proto.volume = db_to_volume_value(0.0)
 
             if len(pan_ccs) == 1:
                 song_track_proto.pan = pan_ccs[0].value - 64
             elif len(pan_ccs) > 1:
@@ -188,15 +268,15 @@
                 pan_target_id = pan_target.to_tf_automation_target_id()
                 song_track_proto.automation.targets.append(pan_target._proto)
                 pan_target._proto = song_track_proto.automation.targets[-1]
                 pan_target_value = song_pb2.AutomationValue()
                 song_track_proto.automation.target_values[pan_target_id] = pan_target_value
                 for index, cc in enumerate(sorted(pan_ccs, key=lambda x: x.time)):
                     pan_target_value.points.add(tick=scale_int_by(
-                        cc.time, ppq_scale_factor), value=cc.value/127.0, id=index+1)
+                        cc.time, ppq_scale_factor), value=cc.value / 127.0, id=index + 1)
 
         song.last_tick = song_last_tick
         song.duration = song.tick_to_seconds(song_last_tick)
         return song
 
     def to_midi(self):
         '''
@@ -307,15 +387,15 @@
         prev_tempo = self.get_tempo_event_at(tempo_index - 1)
         if prev_tempo is None:
             return
         if (prev_tempo.get_ticks() == move_to_tick):
             # Moved to another tempo, delete it.
             self.remove_tempo_change_at(tempo_index - 1)
         elif (tempo_index < self.get_tempo_event_count() - 1):
-            next_tempo = self.get_tempo_event_at(tempo_index+1)
+            next_tempo = self.get_tempo_event_at(tempo_index + 1)
             if (next_tempo is not None and next_tempo.get_ticks() == move_to_tick):
                 # Moved to another tempo, delete it.
                 self.remove_tempo_change_at(tempo_index + 1)
 
         tempo.set_ticks(move_to_tick)
         self.retiming_tempo_events()
```

### Comparing `tuneflow-py-0.4.6/src/tuneflow_py/models/tempo.py` & `tuneflow-py-0.5.0/src/tuneflow_py/models/tempo.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/src/tuneflow_py/models/time_signature.py` & `tuneflow-py-0.5.0/src/tuneflow_py/models/time_signature.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/src/tuneflow_py/models/track.py` & `tuneflow-py-0.5.0/src/tuneflow_py/models/track.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/src/tuneflow_py/utils.py` & `tuneflow-py-0.5.0/src/tuneflow_py/utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/src/tuneflow_py.egg-info/PKG-INFO` & `tuneflow-py-0.5.0/src/tuneflow_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-py
-Version: 0.4.6
+Version: 0.5.0
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: TuneFlow <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-py-0.4.6/src/tuneflow_py.egg-info/SOURCES.txt` & `tuneflow-py-0.5.0/src/tuneflow_py.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,20 +15,22 @@
 src/tuneflow_py/descriptors/param.py
 src/tuneflow_py/descriptors/plugin.py
 src/tuneflow_py/descriptors/text.py
 src/tuneflow_py/descriptors/widget.py
 src/tuneflow_py/models/audio_plugin.py
 src/tuneflow_py/models/automation.py
 src/tuneflow_py/models/clip.py
+src/tuneflow_py/models/marker.py
 src/tuneflow_py/models/note.py
 src/tuneflow_py/models/song.py
 src/tuneflow_py/models/tempo.py
 src/tuneflow_py/models/time_signature.py
 src/tuneflow_py/models/track.py
 src/tuneflow_py/models/protos/song_pb2.py
 test/test_audio_clip.py
 test/test_automation.py
+test/test_marker.py
 test/test_midi_clip.py
 test/test_note.py
 test/test_song.py
 test/test_track.py
 test/test_utils.py
```

### Comparing `tuneflow-py-0.4.6/test/test_audio_clip.py` & `tuneflow-py-0.5.0/test/test_audio_clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/test/test_automation.py` & `tuneflow-py-0.5.0/test/test_automation.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/test/test_midi_clip.py` & `tuneflow-py-0.5.0/test/test_midi_clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/test/test_note.py` & `tuneflow-py-0.5.0/test/test_note.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/test/test_song.py` & `tuneflow-py-0.5.0/test/test_song.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/test/test_track.py` & `tuneflow-py-0.5.0/test/test_track.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.6/test/test_utils.py` & `tuneflow-py-0.5.0/test/test_utils.py`

 * *Files identical despite different names*


# Comparing `tmp/TrainerBase-2.9.0.tar.gz` & `tmp/TrainerBase-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrainerBase-2.9.0.tar", last modified: Mon Apr 10 20:53:25 2023, max compression
+gzip compressed data, was "TrainerBase-2.9.1.tar", last modified: Mon Apr 10 21:03:01 2023, max compression
```

## Comparing `TrainerBase-2.9.0.tar` & `TrainerBase-2.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rwxr-xr-x   0        0        0   117248 2022-02-21 09:32:45.418863 TrainerBase-2.9.0/fasm/FASM.EXE
--rw-r--r--   0        0        0     1103 2023-04-02 15:26:24.974155 TrainerBase-2.9.0/LICENSE
--rw-r--r--   0        0        0      788 2023-04-10 20:52:17.696085 TrainerBase-2.9.0/pyproject.toml
--rw-r--r--   0        0        0      170 2022-11-27 19:37:39.028579 TrainerBase-2.9.0/README.md
--rw-r--r--   0        0        0        0 2022-11-27 19:37:39.030089 TrainerBase-2.9.0/trainerbase/__init__.py
--rw-r--r--   0        0        0     3464 2023-04-10 20:48:57.586831 TrainerBase-2.9.0/trainerbase/codeinjection.py
--rw-r--r--   0        0        0     1019 2023-04-10 20:37:50.924352 TrainerBase-2.9.0/trainerbase/common.py
--rw-r--r--   0        0        0     2686 2022-12-07 20:27:21.445222 TrainerBase-2.9.0/trainerbase/gameobject.py
--rw-r--r--   0        0        0     6338 2023-04-10 20:52:25.869971 TrainerBase-2.9.0/trainerbase/gui.py
--rw-r--r--   0        0        0     1332 2023-04-10 20:47:38.678906 TrainerBase-2.9.0/trainerbase/memory.py
--rw-r--r--   0        0        0     2518 2022-12-09 12:40:11.890792 TrainerBase-2.9.0/trainerbase/scriptengine.py
--rw-r--r--   0        0        0        0 2022-11-27 19:37:39.031619 TrainerBase-2.9.0/trainerbase/template/__init__.py
--rw-r--r--   0        0        0       56 2022-12-03 21:05:33.189289 TrainerBase-2.9.0/trainerbase/template/config.py
--rw-r--r--   0        0        0      758 2022-12-03 21:05:33.189289 TrainerBase-2.9.0/trainerbase/template/gui.py
--rw-r--r--   0        0        0       95 2022-12-03 21:05:33.190297 TrainerBase-2.9.0/trainerbase/template/injections.py
--rw-r--r--   0        0        0      302 2022-12-07 20:41:59.080957 TrainerBase-2.9.0/trainerbase/template/main.py
--rw-r--r--   0        0        0      133 2022-12-04 16:32:33.988485 TrainerBase-2.9.0/trainerbase/template/objects.py
--rw-r--r--   0        0        0      233 2022-12-07 19:31:24.358010 TrainerBase-2.9.0/trainerbase/template/scripts.py
--rw-r--r--   0        0        0      256 2023-04-10 20:52:25.763039 TrainerBase-2.9.0/trainerbase/tts.py
--rw-r--r--   0        0        0      128 2022-12-03 21:05:33.192296 TrainerBase-2.9.0/trainerbase/use_trainer_template.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 TrainerBase-2.9.0/PKG-INFO
+-rwxr-xr-x   0        0        0   117248 2022-02-21 09:32:45.418863 TrainerBase-2.9.1/fasm/FASM.EXE
+-rw-r--r--   0        0        0     1103 2023-04-02 15:26:24.974155 TrainerBase-2.9.1/LICENSE
+-rw-r--r--   0        0        0      788 2023-04-10 21:02:38.660868 TrainerBase-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0      170 2022-11-27 19:37:39.028579 TrainerBase-2.9.1/README.md
+-rw-r--r--   0        0        0        0 2022-11-27 19:37:39.030089 TrainerBase-2.9.1/trainerbase/__init__.py
+-rw-r--r--   0        0        0     3464 2023-04-10 20:48:57.586831 TrainerBase-2.9.1/trainerbase/codeinjection.py
+-rw-r--r--   0        0        0     1019 2023-04-10 20:37:50.924352 TrainerBase-2.9.1/trainerbase/common.py
+-rw-r--r--   0        0        0     2686 2022-12-07 20:27:21.445222 TrainerBase-2.9.1/trainerbase/gameobject.py
+-rw-r--r--   0        0        0     6434 2023-04-10 21:02:16.760340 TrainerBase-2.9.1/trainerbase/gui.py
+-rw-r--r--   0        0        0     1332 2023-04-10 20:47:38.678906 TrainerBase-2.9.1/trainerbase/memory.py
+-rw-r--r--   0        0        0     2518 2022-12-09 12:40:11.890792 TrainerBase-2.9.1/trainerbase/scriptengine.py
+-rw-r--r--   0        0        0        0 2022-11-27 19:37:39.031619 TrainerBase-2.9.1/trainerbase/template/__init__.py
+-rw-r--r--   0        0        0       56 2022-12-03 21:05:33.189289 TrainerBase-2.9.1/trainerbase/template/config.py
+-rw-r--r--   0        0        0      758 2022-12-03 21:05:33.189289 TrainerBase-2.9.1/trainerbase/template/gui.py
+-rw-r--r--   0        0        0       95 2022-12-03 21:05:33.190297 TrainerBase-2.9.1/trainerbase/template/injections.py
+-rw-r--r--   0        0        0      302 2022-12-07 20:41:59.080957 TrainerBase-2.9.1/trainerbase/template/main.py
+-rw-r--r--   0        0        0      133 2022-12-04 16:32:33.988485 TrainerBase-2.9.1/trainerbase/template/objects.py
+-rw-r--r--   0        0        0      233 2022-12-07 19:31:24.358010 TrainerBase-2.9.1/trainerbase/template/scripts.py
+-rw-r--r--   0        0        0      256 2023-04-10 20:52:25.763039 TrainerBase-2.9.1/trainerbase/tts.py
+-rw-r--r--   0        0        0      128 2022-12-03 21:05:33.192296 TrainerBase-2.9.1/trainerbase/use_trainer_template.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 TrainerBase-2.9.1/PKG-INFO
```

### Comparing `TrainerBase-2.9.0/fasm/FASM.EXE` & `TrainerBase-2.9.1/fasm/FASM.EXE`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.0/LICENSE` & `TrainerBase-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.0/pyproject.toml` & `TrainerBase-2.9.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 dev = [
     "black>=22.10.0",
     "pylint>=2.15.7",
 ]
 
 [project]
 name = "TrainerBase"
-version = "2.9.0"
+version = "2.9.1"
 description = "Template/Framework to create game trainers"
 authors = [
     { name = "v01d", email = "v01d@v01d.ru" },
     { name = "doomayka", email = "zd@doomayka.ru" },
 ]
 dependencies = [
     "pymem>=1.10.0",
```

### Comparing `TrainerBase-2.9.0/trainerbase/codeinjection.py` & `TrainerBase-2.9.1/trainerbase/codeinjection.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.0/trainerbase/common.py` & `TrainerBase-2.9.1/trainerbase/common.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.0/trainerbase/gameobject.py` & `TrainerBase-2.9.1/trainerbase/gameobject.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.0/trainerbase/gui.py` & `TrainerBase-2.9.1/trainerbase/gui.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,21 +52,22 @@
     hotkey: str = None,
     tts_on_hotkey: bool = True,
 ):
     def on_script_state_change():
         script.enabled = dpg.get_value(script.dpg_tag)
 
     if hotkey is not None:
+        pure_label = label
 
         def on_hotkey_press():
             dpg.set_value(script.dpg_tag, not dpg.get_value(script.dpg_tag))
             on_script_state_change()
             if tts_on_hotkey:
                 status = "enabled" if script.enabled else "disabled"
-                say(f"Script {label} {status}")
+                say(f"Script {pure_label} {status}")
 
         keyboard.add_hotkey(hotkey, on_hotkey_press)
 
         label = f"[{hotkey}] {label}"
 
     dpg.add_checkbox(label=label, tag=script.dpg_tag, callback=on_script_state_change, default_value=script.enabled)
 
@@ -90,21 +91,22 @@
 
         if gameobject.frozen is None:
             gameobject.value = new_value
         else:
             gameobject.frozen = new_value
 
     if hotkey is not None:
+        pure_label = label
 
         def on_hotkey_press():
             dpg.set_value(gameobject.dpg_tag_frozen, not dpg.get_value(gameobject.dpg_tag_frozen))
             on_frozen_state_change()
             if tts_on_hotkey:
                 status = "released" if gameobject.frozen is None else "frozen"
-                say(f"GameObject {label} {status}")
+                say(f"GameObject {pure_label} {status}")
 
         keyboard.add_hotkey(hotkey, on_hotkey_press)
 
         label = f"[{hotkey}] {label}"
 
     with dpg.group(horizontal=True):
         dpg.add_checkbox(tag=gameobject.dpg_tag_frozen, callback=on_frozen_state_change)
@@ -123,21 +125,22 @@
     def on_codeinjection_state_change():
         if dpg.get_value(injection.dpg_tag):
             injection.inject()
         else:
             injection.eject()
 
     if hotkey is not None:
+        pure_label = label
 
         def on_hotkey_press():
             dpg.set_value(injection.dpg_tag, not dpg.get_value(injection.dpg_tag))
             on_codeinjection_state_change()
             if tts_on_hotkey:
                 status = "applied" if dpg.get_value(injection.dpg_tag) else "removed"
-                say(f"CodeInjection {label} {status}")
+                say(f"CodeInjection {pure_label} {status}")
 
         keyboard.add_hotkey(hotkey, on_hotkey_press)
 
         label = f"[{hotkey}] {label}"
 
     dpg.add_checkbox(label=label, tag=injection.dpg_tag, callback=on_codeinjection_state_change)
```

### Comparing `TrainerBase-2.9.0/trainerbase/memory.py` & `TrainerBase-2.9.1/trainerbase/memory.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.0/trainerbase/scriptengine.py` & `TrainerBase-2.9.1/trainerbase/scriptengine.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.9.0/trainerbase/template/gui.py` & `TrainerBase-2.9.1/trainerbase/template/gui.py`

 * *Files identical despite different names*


# Comparing `tmp/TrainerBase-2.8.2.tar.gz` & `tmp/TrainerBase-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrainerBase-2.8.2.tar", last modified: Wed Apr  5 11:12:18 2023, max compression
+gzip compressed data, was "TrainerBase-2.9.0.tar", last modified: Mon Apr 10 20:53:25 2023, max compression
```

## Comparing `TrainerBase-2.8.2.tar` & `TrainerBase-2.9.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rwxr-xr-x   0        0        0   117248 2022-02-21 09:32:45.418863 TrainerBase-2.8.2/fasm/FASM.EXE
--rw-r--r--   0        0        0     1103 2023-04-02 15:26:24.974155 TrainerBase-2.8.2/LICENSE
--rw-r--r--   0        0        0      767 2023-04-05 11:10:52.673299 TrainerBase-2.8.2/pyproject.toml
--rw-r--r--   0        0        0      170 2022-11-27 19:37:39.028579 TrainerBase-2.8.2/README.md
--rw-r--r--   0        0        0        0 2022-11-27 19:37:39.030089 TrainerBase-2.8.2/trainerbase/__init__.py
--rw-r--r--   0        0        0     3476 2023-04-02 15:40:55.182254 TrainerBase-2.8.2/trainerbase/codeinjection.py
--rw-r--r--   0        0        0     1019 2022-12-09 12:24:02.543792 TrainerBase-2.8.2/trainerbase/common.py
--rw-r--r--   0        0        0     2686 2022-12-07 20:27:21.445222 TrainerBase-2.8.2/trainerbase/gameobject.py
--rw-r--r--   0        0        0     5458 2023-04-05 11:11:44.488173 TrainerBase-2.8.2/trainerbase/gui.py
--rw-r--r--   0        0        0     1332 2022-12-17 20:33:10.668800 TrainerBase-2.8.2/trainerbase/memory.py
--rw-r--r--   0        0        0     2518 2022-12-09 12:40:11.890792 TrainerBase-2.8.2/trainerbase/scriptengine.py
--rw-r--r--   0        0        0        0 2022-11-27 19:37:39.031619 TrainerBase-2.8.2/trainerbase/template/__init__.py
--rw-r--r--   0        0        0       56 2022-12-03 21:05:33.189289 TrainerBase-2.8.2/trainerbase/template/config.py
--rw-r--r--   0        0        0      758 2022-12-03 21:05:33.189289 TrainerBase-2.8.2/trainerbase/template/gui.py
--rw-r--r--   0        0        0       95 2022-12-03 21:05:33.190297 TrainerBase-2.8.2/trainerbase/template/injections.py
--rw-r--r--   0        0        0      302 2022-12-07 20:41:59.080957 TrainerBase-2.8.2/trainerbase/template/main.py
--rw-r--r--   0        0        0      133 2022-12-04 16:32:33.988485 TrainerBase-2.8.2/trainerbase/template/objects.py
--rw-r--r--   0        0        0      233 2022-12-07 19:31:24.358010 TrainerBase-2.8.2/trainerbase/template/scripts.py
--rw-r--r--   0        0        0      128 2022-12-03 21:05:33.192296 TrainerBase-2.8.2/trainerbase/use_trainer_template.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 TrainerBase-2.8.2/PKG-INFO
+-rwxr-xr-x   0        0        0   117248 2022-02-21 09:32:45.418863 TrainerBase-2.9.0/fasm/FASM.EXE
+-rw-r--r--   0        0        0     1103 2023-04-02 15:26:24.974155 TrainerBase-2.9.0/LICENSE
+-rw-r--r--   0        0        0      788 2023-04-10 20:52:17.696085 TrainerBase-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0      170 2022-11-27 19:37:39.028579 TrainerBase-2.9.0/README.md
+-rw-r--r--   0        0        0        0 2022-11-27 19:37:39.030089 TrainerBase-2.9.0/trainerbase/__init__.py
+-rw-r--r--   0        0        0     3464 2023-04-10 20:48:57.586831 TrainerBase-2.9.0/trainerbase/codeinjection.py
+-rw-r--r--   0        0        0     1019 2023-04-10 20:37:50.924352 TrainerBase-2.9.0/trainerbase/common.py
+-rw-r--r--   0        0        0     2686 2022-12-07 20:27:21.445222 TrainerBase-2.9.0/trainerbase/gameobject.py
+-rw-r--r--   0        0        0     6338 2023-04-10 20:52:25.869971 TrainerBase-2.9.0/trainerbase/gui.py
+-rw-r--r--   0        0        0     1332 2023-04-10 20:47:38.678906 TrainerBase-2.9.0/trainerbase/memory.py
+-rw-r--r--   0        0        0     2518 2022-12-09 12:40:11.890792 TrainerBase-2.9.0/trainerbase/scriptengine.py
+-rw-r--r--   0        0        0        0 2022-11-27 19:37:39.031619 TrainerBase-2.9.0/trainerbase/template/__init__.py
+-rw-r--r--   0        0        0       56 2022-12-03 21:05:33.189289 TrainerBase-2.9.0/trainerbase/template/config.py
+-rw-r--r--   0        0        0      758 2022-12-03 21:05:33.189289 TrainerBase-2.9.0/trainerbase/template/gui.py
+-rw-r--r--   0        0        0       95 2022-12-03 21:05:33.190297 TrainerBase-2.9.0/trainerbase/template/injections.py
+-rw-r--r--   0        0        0      302 2022-12-07 20:41:59.080957 TrainerBase-2.9.0/trainerbase/template/main.py
+-rw-r--r--   0        0        0      133 2022-12-04 16:32:33.988485 TrainerBase-2.9.0/trainerbase/template/objects.py
+-rw-r--r--   0        0        0      233 2022-12-07 19:31:24.358010 TrainerBase-2.9.0/trainerbase/template/scripts.py
+-rw-r--r--   0        0        0      256 2023-04-10 20:52:25.763039 TrainerBase-2.9.0/trainerbase/tts.py
+-rw-r--r--   0        0        0      128 2022-12-03 21:05:33.192296 TrainerBase-2.9.0/trainerbase/use_trainer_template.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 TrainerBase-2.9.0/PKG-INFO
```

### Comparing `TrainerBase-2.8.2/fasm/FASM.EXE` & `TrainerBase-2.9.0/fasm/FASM.EXE`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.8.2/LICENSE` & `TrainerBase-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.8.2/pyproject.toml` & `TrainerBase-2.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -14,24 +14,25 @@
 dev = [
     "black>=22.10.0",
     "pylint>=2.15.7",
 ]
 
 [project]
 name = "TrainerBase"
-version = "2.8.2"
+version = "2.9.0"
 description = "Template/Framework to create game trainers"
 authors = [
     { name = "v01d", email = "v01d@v01d.ru" },
     { name = "doomayka", email = "zd@doomayka.ru" },
 ]
 dependencies = [
     "pymem>=1.10.0",
     "dearpygui>=1.8.0",
     "keyboard>=0.13.5",
+    "pyttsx3>=2.90",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `TrainerBase-2.8.2/trainerbase/codeinjection.py` & `TrainerBase-2.9.0/trainerbase/codeinjection.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,10 +105,10 @@
         raise TypeError("code must be bytes | str")
 
     return code
 
 
 def goto(address: int) -> str:
     return f"""
-            push {address}
-            ret
-        """
+        push {address}
+        ret
+    """
```

### Comparing `TrainerBase-2.8.2/trainerbase/common.py` & `TrainerBase-2.9.0/trainerbase/common.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.8.2/trainerbase/gameobject.py` & `TrainerBase-2.9.0/trainerbase/gameobject.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.8.2/trainerbase/gui.py` & `TrainerBase-2.9.0/trainerbase/gui.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import dearpygui.dearpygui as dpg
 import keyboard
 
 from trainerbase import scriptengine
 from trainerbase import gameobject
 from trainerbase import codeinjection
 from trainerbase.common import Teleport
+from trainerbase.tts import say
 
 
 def simple_trainerbase_menu(window_title: str, width, height):
     def menu_decorator(initializer: Callable):
         def run_menu_wrapper(on_initialized: Callable):
             dpg.create_context()
             dpg.create_viewport(
@@ -45,36 +46,41 @@
     return menu_decorator
 
 
 def add_script_to_gui(
     script: scriptengine.Script,
     label: str,
     hotkey: str = None,
+    tts_on_hotkey: bool = True,
 ):
     def on_script_state_change():
         script.enabled = dpg.get_value(script.dpg_tag)
 
     if hotkey is not None:
 
         def on_hotkey_press():
             dpg.set_value(script.dpg_tag, not dpg.get_value(script.dpg_tag))
             on_script_state_change()
+            if tts_on_hotkey:
+                status = "enabled" if script.enabled else "disabled"
+                say(f"Script {label} {status}")
 
         keyboard.add_hotkey(hotkey, on_hotkey_press)
 
         label = f"[{hotkey}] {label}"
 
     dpg.add_checkbox(label=label, tag=script.dpg_tag, callback=on_script_state_change, default_value=script.enabled)
 
 
 def add_gameobject_to_gui(
     gameobject: gameobject.GameObject,
     label: str,
     hotkey: str = None,
     before_set: Callable = int,
+    tts_on_hotkey: bool = True,
 ):
     def on_frozen_state_change():
         gameobject.frozen = gameobject.value if dpg.get_value(gameobject.dpg_tag_frozen) else None
 
     def on_value_set():
         raw_new_value = dpg.get_value(gameobject.dpg_tag_setter)
         if not raw_new_value:
@@ -88,14 +94,17 @@
             gameobject.frozen = new_value
 
     if hotkey is not None:
 
         def on_hotkey_press():
             dpg.set_value(gameobject.dpg_tag_frozen, not dpg.get_value(gameobject.dpg_tag_frozen))
             on_frozen_state_change()
+            if tts_on_hotkey:
+                status = "released" if gameobject.frozen is None else "frozen"
+                say(f"GameObject {label} {status}")
 
         keyboard.add_hotkey(hotkey, on_hotkey_press)
 
         label = f"[{hotkey}] {label}"
 
     with dpg.group(horizontal=True):
         dpg.add_checkbox(tag=gameobject.dpg_tag_frozen, callback=on_frozen_state_change)
@@ -105,35 +114,44 @@
         dpg.add_button(label="Set", callback=on_value_set)
 
 
 def add_codeinjection_to_gui(
     injection: codeinjection.CodeInjection,
     label: str,
     hotkey: str = None,
+    tts_on_hotkey: bool = True,
 ):
     def on_codeinjection_state_change():
         if dpg.get_value(injection.dpg_tag):
             injection.inject()
         else:
             injection.eject()
 
     if hotkey is not None:
 
         def on_hotkey_press():
             dpg.set_value(injection.dpg_tag, not dpg.get_value(injection.dpg_tag))
             on_codeinjection_state_change()
+            if tts_on_hotkey:
+                status = "applied" if dpg.get_value(injection.dpg_tag) else "removed"
+                say(f"CodeInjection {label} {status}")
 
         keyboard.add_hotkey(hotkey, on_hotkey_press)
 
         label = f"[{hotkey}] {label}"
 
     dpg.add_checkbox(label=label, tag=injection.dpg_tag, callback=on_codeinjection_state_change)
 
 
-def add_teleport_to_gui(tp: Teleport, hotkey_save_position: str = None, hotkey_set_saved_position: str = None):
+def add_teleport_to_gui(
+    tp: Teleport,
+    hotkey_save_position: str = None,
+    hotkey_set_saved_position: str = None,
+    tts_on_hotkey: bool = True,
+):
     tag_teleport_labels = "teleport_labels"
     should_add_save_set_position_hotkeys = hotkey_save_position is not None and hotkey_set_saved_position is not None
 
     def on_goto_label():
         tp.goto(dpg.get_value(tag_teleport_labels))
 
     def on_clip_coords():
@@ -141,19 +159,26 @@
 
     if should_add_save_set_position_hotkeys:
         saved_position = None
 
         def on_hotkey_save_position_press():
             nonlocal saved_position
             saved_position = tp.get_coords()
+            if tts_on_hotkey:
+                say("Position saved")
 
         def on_hotkey_set_saved_position_press():
             if saved_position is not None:
                 tp.set_coords(*saved_position)
 
+                if tts_on_hotkey:
+                    say("Position restored")
+            elif tts_on_hotkey:
+                say("Save position at first")
+
         keyboard.add_hotkey(hotkey_save_position, on_hotkey_save_position_press)
         keyboard.add_hotkey(hotkey_set_saved_position, on_hotkey_set_saved_position_press)
 
     with dpg.tab(label="Teleport", tag="tab_teleport"):
         if should_add_save_set_position_hotkeys:
             dpg.add_text(f"[{hotkey_save_position}] Save Position")
             dpg.add_text(f"[{hotkey_set_saved_position}] Set Saved Position")
```

### Comparing `TrainerBase-2.8.2/trainerbase/memory.py` & `TrainerBase-2.9.0/trainerbase/memory.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.8.2/trainerbase/scriptengine.py` & `TrainerBase-2.9.0/trainerbase/scriptengine.py`

 * *Files identical despite different names*

### Comparing `TrainerBase-2.8.2/trainerbase/template/gui.py` & `TrainerBase-2.9.0/trainerbase/template/gui.py`

 * *Files identical despite different names*


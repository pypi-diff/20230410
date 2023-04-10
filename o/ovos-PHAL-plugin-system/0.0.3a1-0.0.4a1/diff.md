# Comparing `tmp/ovos-PHAL-plugin-system-0.0.3a1.tar.gz` & `tmp/ovos-PHAL-plugin-system-0.0.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-system-0.0.3a1.tar", last modified: Sat Dec 31 02:15:44 2022, max compression
+gzip compressed data, was "ovos-PHAL-plugin-system-0.0.4a1.tar", last modified: Mon Apr 10 18:17:32 2023, max compression
```

## Comparing `ovos-PHAL-plugin-system-0.0.3a1.tar` & `ovos-PHAL-plugin-system-0.0.4a1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 02:15:44.821671 ovos-PHAL-plugin-system-0.0.3a1/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2022-12-31 02:15:44.821671 ovos-PHAL-plugin-system-0.0.3a1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 02:15:44.821671 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/
--rw-r--r--   0 runner    (1001) docker     (123)    11179 2022-12-31 02:15:36.000000 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 02:15:44.821671 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2022-12-31 02:15:36.000000 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/ui/Reboot.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2022-12-31 02:15:36.000000 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/ui/Restart.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2022-12-31 02:15:36.000000 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/ui/Shutdown.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2022-12-31 02:15:36.000000 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/ui/Status.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 02:15:44.821671 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/ui/animations/
--rw-r--r--   0 runner    (1001) docker     (123)    11056 2022-12-31 02:15:36.000000 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/ui/animations/loading.json
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2022-12-31 02:15:36.000000 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/ui/animations/status-fail.json
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2022-12-31 02:15:36.000000 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/ui/animations/status-success.json
--rw-r--r--   0 runner    (1001) docker     (123)      177 2022-12-31 02:15:39.000000 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 02:15:44.821671 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2022-12-31 02:15:44.000000 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2022-12-31 02:15:44.000000 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-31 02:15:44.000000 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-31 02:15:44.000000 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-31 02:15:44.000000 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-31 02:15:44.000000 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-31 02:15:44.000000 ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-31 02:15:44.821671 ovos-PHAL-plugin-system-0.0.3a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2736 2022-12-31 02:15:36.000000 ovos-PHAL-plugin-system-0.0.3a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:17:32.746103 ovos-PHAL-plugin-system-0.0.4a1/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-10 18:17:32.746103 ovos-PHAL-plugin-system-0.0.4a1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:17:32.746103 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-10 18:17:24.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:17:32.746103 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-10 18:17:24.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/Reboot.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-10 18:17:24.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/Restart.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-10 18:17:24.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/Shutdown.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-10 18:17:24.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/Status.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:17:32.746103 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/animations/
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-04-10 18:17:24.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/animations/loading.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-04-10 18:17:24.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/animations/status-fail.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-10 18:17:24.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/animations/status-success.json
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-10 18:17:26.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:17:32.746103 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-10 18:17:32.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-10 18:17:32.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:17:32.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-10 18:17:32.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-10 18:17:32.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 18:17:32.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:17:32.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:17:32.746103 ovos-PHAL-plugin-system-0.0.4a1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2736 2023-04-10 18:17:24.000000 ovos-PHAL-plugin-system-0.0.4a1/setup.py
```

### Comparing `ovos-PHAL-plugin-system-0.0.3a1/PKG-INFO` & `ovos-PHAL-plugin-system-0.0.4a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-system
-Version: 0.0.3a1
+Version: 0.0.4a1
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-system
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/__init__.py` & `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -198,21 +198,30 @@
             self.gui.show_page(page)
         self.bus.emit(message.reply('system.ntp.sync.complete'))
 
     def handle_reboot_request(self, message):
         if message.data.get("display", True):
             page = join(dirname(__file__), "ui", "Reboot.qml")
             self.gui.show_page(page, override_animations=True, override_idle=True)
-        system_reboot()
+
+        script = os.path.expanduser(self.config.get("reboot_script"))
+        if script and os.path.isfile(script):
+            subprocess.call(script, shell=True)
+        else:
+            system_reboot()
 
     def handle_shutdown_request(self, message):
         if message.data.get("display", True):
             page = join(dirname(__file__), "ui", "Shutdown.qml")
             self.gui.show_page(page, override_animations=True, override_idle=True)
-        system_shutdown()
+        script = os.path.expanduser(self.config.get("shutdown_script"))
+        if script and os.path.isfile(script):
+            subprocess.call(script, shell=True)
+        else:
+            system_reboot()
 
     def handle_configure_language_request(self, message):
         language_code = message.data.get('language_code', "en_US")
         with open(f"{os.environ['HOME']}/.bash_profile", "w") as bash_profile_file:
             bash_profile_file.write(f"export LANG={language_code}\n")
 
         language_code = language_code.lower().replace("_", "-")
```

### Comparing `ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/ui/Reboot.qml` & `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/Reboot.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/ui/Restart.qml` & `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/Restart.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/ui/Shutdown.qml` & `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/Shutdown.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/ui/Status.qml` & `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/Status.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/ui/animations/loading.json` & `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/animations/loading.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/ui/animations/status-fail.json` & `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/animations/status-fail.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system/ui/animations/status-success.json` & `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/animations/status-success.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system.egg-info/PKG-INFO` & `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-system
-Version: 0.0.3a1
+Version: 0.0.4a1
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-system
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-system-0.0.3a1/ovos_PHAL_plugin_system.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.3a1/setup.py` & `ovos-PHAL-plugin-system-0.0.4a1/setup.py`

 * *Files identical despite different names*


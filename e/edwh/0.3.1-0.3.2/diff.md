# Comparing `tmp/edwh-0.3.1.tar.gz` & `tmp/edwh-0.3.2.tar.gz`

## Comparing `edwh-0.3.1.tar` & `edwh-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 edwh-0.3.1/CHANGELOG.md
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 edwh-0.3.1/.idea/.gitignore
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 edwh-0.3.1/.idea/edwh.iml
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 edwh-0.3.1/.idea/jupyter-settings.xml
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 edwh-0.3.1/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 edwh-0.3.1/.idea/modules.xml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh-0.3.1/.idea/vcs.xml
--rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 edwh-0.3.1/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh-0.3.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     9468 2020-02-02 00:00:00.000000 edwh-0.3.1/c/edwh-0.3.0-py3-none-any.whl
--rw-r--r--   0        0        0    12057 2020-02-02 00:00:00.000000 edwh-0.3.1/c/edwh-0.3.0.tar.gz
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.3.1/src/edwh/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.3.1/src/edwh/__init__.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 edwh-0.3.1/src/edwh/cli.py
--rw-r--r--   0        0        0    17003 2020-02-02 00:00:00.000000 edwh-0.3.1/src/edwh/tasks.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.3.1/LICENSE.txt
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 edwh-0.3.1/README.md
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 edwh-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 edwh-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 edwh-0.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 edwh-0.3.2/.idea/.gitignore
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 edwh-0.3.2/.idea/edwh.iml
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 edwh-0.3.2/.idea/jupyter-settings.xml
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 edwh-0.3.2/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 edwh-0.3.2/.idea/modules.xml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh-0.3.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 edwh-0.3.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh-0.3.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     9468 2020-02-02 00:00:00.000000 edwh-0.3.2/c/edwh-0.3.0-py3-none-any.whl
+-rw-r--r--   0        0        0    12057 2020-02-02 00:00:00.000000 edwh-0.3.2/c/edwh-0.3.0.tar.gz
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.3.2/src/edwh/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.3.2/src/edwh/__init__.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 edwh-0.3.2/src/edwh/cli.py
+-rw-r--r--   0        0        0    16936 2020-02-02 00:00:00.000000 edwh-0.3.2/src/edwh/tasks.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.3.2/tests/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.3.2/LICENSE.txt
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 edwh-0.3.2/README.md
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 edwh-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 edwh-0.3.2/PKG-INFO
```

### Comparing `edwh-0.3.1/CHANGELOG.md` & `edwh-0.3.2/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.3.2 (2023-04-10)
+### Fix
+* Diceware was included as a dependency, but used as a pipx installed application. ([`2f6bc9f`](https://github.com/educationwarehouse/edwh/commit/2f6bc9f7c7aabafbab0b857d84905be13d3973f0))
+
 ## v0.3.1 (2023-04-10)
 ### Fix
 * Missing changelog entry ([`4fe91e4`](https://github.com/educationwarehouse/edwh/commit/4fe91e400a8b64197b7a1c7df55777c13787b2d7))
 
 ## v0.3.1 (2023-04-10)
 ### Feature
 * Added and upgraded: settings, up, ps, logs, stop, down, build, rebuild, docs, search_adjacent_setting, generate_password, settings, volumes and helpers. ([`9f80e25`](https://github.com/educationwarehouse/edwh/commit/9f80e25953a37a333ce4a0b73e355864d6c26fb1))
```

### Comparing `edwh-0.3.1/.idea/jupyter-settings.xml` & `edwh-0.3.2/.idea/jupyter-settings.xml`

 * *Files identical despite different names*

### Comparing `edwh-0.3.1/.idea/workspace.xml` & `edwh-0.3.2/.idea/workspace.xml`

 * *Files 16% similar despite different names*

#### Comparing `edwh-0.3.1/.idea/workspace.xml` & `edwh-0.3.2/.idea/workspace.xml`

```diff
@@ -1,21 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="BlackConnectSettings" triggerOnReformat="true"/>
   <component name="ChangeListManager">
-    <list default="true" id="a8ee968c-c8d6-4911-ae81-e260b5e9d9f0" name="Changes" comment="feat: added and upgraded: settings, up, ps, logs, stop, down, build, rebuild, docs, search_adjacent_setting, generate_password, settings, volumes and helpers.
-
-including new dependencies: tabulate, pyyaml, diceware and tomlkit
-
-Fixed some inspections.">
+    <list default="true" id="a8ee968c-c8d6-4911-ae81-e260b5e9d9f0" name="Changes" comment="fix: missing changelog entry">
       <change beforePath="$PROJECT_DIR$/.idea/vcs.xml" beforeDir="false" afterPath="$PROJECT_DIR$/.idea/vcs.xml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/CHANGELOG.md" beforeDir="false" afterPath="$PROJECT_DIR$/CHANGELOG.md" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/edwh/tasks.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/edwh/tasks.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
@@ -63,15 +59,15 @@
       <option name="presentableId" value="Default"/>
       <updated>1680722607644</updated>
       <workItem from="1680722608717" duration="182000"/>
       <workItem from="1680724415156" duration="2074000"/>
       <workItem from="1680965546116" duration="403000"/>
       <workItem from="1680967358935" duration="3652000"/>
       <workItem from="1681073068492" duration="64000"/>
-      <workItem from="1681073149934" duration="9132000"/>
+      <workItem from="1681073149934" duration="10495000"/>
     </task>
     <task id="LOCAL-00001" summary="feat: added `plugins` as an optional dependencies">
       <created>1680724520623</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1680724520623</updated>
@@ -104,15 +100,22 @@
 Fixed some inspections.">
       <created>1681082009694</created>
       <option name="number" value="00005"/>
       <option name="presentableId" value="LOCAL-00005"/>
       <option name="project" value="LOCAL"/>
       <updated>1681082009694</updated>
     </task>
-    <option name="localTasksCounter" value="6"/>
+    <task id="LOCAL-00006" summary="fix: missing changelog entry">
+      <created>1681082304271</created>
+      <option name="number" value="00006"/>
+      <option name="presentableId" value="LOCAL-00006"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1681082304271</updated>
+    </task>
+    <option name="localTasksCounter" value="7"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -131,14 +134,11 @@
     <MESSAGE value="build: version bump"/>
     <MESSAGE value="fix: added `tomlkit` dependency voor `omgeving`, changed the output of the discovered plugins list."/>
     <MESSAGE value="feat: added and upgraded: settings, up, ps, logs, stop, down, build, rebuild, docs, search_adjacent_setting, generate_password, settings, volumes and helpers.
 
 including new dependencies: tabulate, pyyaml, diceware and tomlkit
 
 Fixed some inspections."/>
-    <option name="LAST_COMMIT_MESSAGE" value="feat: added and upgraded: settings, up, ps, logs, stop, down, build, rebuild, docs, search_adjacent_setting, generate_password, settings, volumes and helpers.
-
-including new dependencies: tabulate, pyyaml, diceware and tomlkit
-
-Fixed some inspections."/>
+    <MESSAGE value="fix: missing changelog entry"/>
+    <option name="LAST_COMMIT_MESSAGE" value="fix: missing changelog entry"/>
   </component>
 </project>
```

### Comparing `edwh-0.3.1/c/edwh-0.3.0-py3-none-any.whl` & `edwh-0.3.2/c/edwh-0.3.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `edwh-0.3.1/c/edwh-0.3.0.tar.gz` & `edwh-0.3.2/c/edwh-0.3.0.tar.gz`

 * *Files identical despite different names*

### Comparing `edwh-0.3.1/src/edwh/cli.py` & `edwh-0.3.2/src/edwh/cli.py`

 * *Files identical despite different names*

### Comparing `edwh-0.3.1/src/edwh/tasks.py` & `edwh-0.3.2/src/edwh/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import diceware
+
 try:
     import glob
     import csv
     import shlex
     from statistics import median
     from invoke import task, Result, Context
     import datetime
@@ -269,18 +271,18 @@
         project = env_path.parent.name
         if not silent:
             print(f"{project :>20} : {value}")
         adjacent_settings[project] = value
     return adjacent_settings
 
 
-@task(help=dict(dice="how many dice to use", silent="do not echo the password"))
-def generate_password(c, dice=6, silent=False):
-    """Generate a diceware password using --dice (default 6) dice."""
-    password = c.run(f"diceware --num {dice}", hide=True).stdout.strip()
+@task(help=dict(silent="do not echo the password"))
+def generate_password(c, silent=False):
+    """Generate a diceware password using --dice 6."""
+    password = diceware.get_passphrase()
     if not silent:
         print("Password:", password)
     return password
 
 
 # noinspection PyUnusedLocal
 @task(help=dict(find="search for this specific setting"))
```

### Comparing `edwh-0.3.1/LICENSE.txt` & `edwh-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh-0.3.1/README.md` & `edwh-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `edwh-0.3.1/pyproject.toml` & `edwh-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh-0.3.1/PKG-INFO` & `edwh-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh
-Version: 0.3.1
+Version: 0.3.2
 Summary: Education Warehouse maintenance tools
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>, Romy Schöller <romy.s@educationwarehouse.nl>, Sven Keimpema <sven.k@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```


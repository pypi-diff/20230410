# Comparing `tmp/edwh-0.3.0.tar.gz` & `tmp/edwh-0.3.1.tar.gz`

## Comparing `edwh-0.3.0.tar` & `edwh-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 edwh-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 edwh-0.3.0/.idea/.gitignore
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 edwh-0.3.0/.idea/edwh.iml
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 edwh-0.3.0/.idea/jupyter-settings.xml
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 edwh-0.3.0/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 edwh-0.3.0/.idea/modules.xml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh-0.3.0/.idea/vcs.xml
--rw-r--r--   0        0        0     5801 2020-02-02 00:00:00.000000 edwh-0.3.0/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh-0.3.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     9468 2020-02-02 00:00:00.000000 edwh-0.3.0/c/edwh-0.3.0-py3-none-any.whl
--rw-r--r--   0        0        0    12057 2020-02-02 00:00:00.000000 edwh-0.3.0/c/edwh-0.3.0.tar.gz
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.3.0/src/edwh/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.3.0/src/edwh/__init__.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 edwh-0.3.0/src/edwh/cli.py
--rw-r--r--   0        0        0    17003 2020-02-02 00:00:00.000000 edwh-0.3.0/src/edwh/tasks.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 edwh-0.3.0/README.md
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 edwh-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 edwh-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 edwh-0.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 edwh-0.3.1/.idea/.gitignore
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 edwh-0.3.1/.idea/edwh.iml
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 edwh-0.3.1/.idea/jupyter-settings.xml
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 edwh-0.3.1/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 edwh-0.3.1/.idea/modules.xml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh-0.3.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 edwh-0.3.1/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh-0.3.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     9468 2020-02-02 00:00:00.000000 edwh-0.3.1/c/edwh-0.3.0-py3-none-any.whl
+-rw-r--r--   0        0        0    12057 2020-02-02 00:00:00.000000 edwh-0.3.1/c/edwh-0.3.0.tar.gz
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.3.1/src/edwh/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.3.1/src/edwh/__init__.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 edwh-0.3.1/src/edwh/cli.py
+-rw-r--r--   0        0        0    17003 2020-02-02 00:00:00.000000 edwh-0.3.1/src/edwh/tasks.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 edwh-0.3.1/README.md
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 edwh-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 edwh-0.3.1/PKG-INFO
```

### Comparing `edwh-0.3.0/.idea/jupyter-settings.xml` & `edwh-0.3.1/.idea/jupyter-settings.xml`

 * *Files identical despite different names*

### Comparing `edwh-0.3.0/.idea/workspace.xml` & `edwh-0.3.1/.idea/workspace.xml`

 * *Files 24% similar despite different names*

#### Comparing `edwh-0.3.0/.idea/workspace.xml` & `edwh-0.3.1/.idea/workspace.xml`

```diff
@@ -1,18 +1,21 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="BlackConnectSettings" triggerOnReformat="true"/>
   <component name="ChangeListManager">
-    <list default="true" id="a8ee968c-c8d6-4911-ae81-e260b5e9d9f0" name="Changes" comment="fix: added `tomlkit` dependency voor `omgeving`, changed the output of the discovered plugins list.">
+    <list default="true" id="a8ee968c-c8d6-4911-ae81-e260b5e9d9f0" name="Changes" comment="feat: added and upgraded: settings, up, ps, logs, stop, down, build, rebuild, docs, search_adjacent_setting, generate_password, settings, volumes and helpers.
+
+including new dependencies: tabulate, pyyaml, diceware and tomlkit
+
+Fixed some inspections.">
       <change beforePath="$PROJECT_DIR$/.idea/vcs.xml" beforeDir="false" afterPath="$PROJECT_DIR$/.idea/vcs.xml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/edwh/tasks.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/edwh/tasks.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/CHANGELOG.md" beforeDir="false" afterPath="$PROJECT_DIR$/CHANGELOG.md" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
@@ -60,15 +63,15 @@
       <option name="presentableId" value="Default"/>
       <updated>1680722607644</updated>
       <workItem from="1680722608717" duration="182000"/>
       <workItem from="1680724415156" duration="2074000"/>
       <workItem from="1680965546116" duration="403000"/>
       <workItem from="1680967358935" duration="3652000"/>
       <workItem from="1681073068492" duration="64000"/>
-      <workItem from="1681073149934" duration="8673000"/>
+      <workItem from="1681073149934" duration="9132000"/>
     </task>
     <task id="LOCAL-00001" summary="feat: added `plugins` as an optional dependencies">
       <created>1680724520623</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1680724520623</updated>
@@ -90,15 +93,26 @@
     <task id="LOCAL-00004" summary="fix: added `tomlkit` dependency voor `omgeving`, changed the output of the discovered plugins list.">
       <created>1680968678579</created>
       <option name="number" value="00004"/>
       <option name="presentableId" value="LOCAL-00004"/>
       <option name="project" value="LOCAL"/>
       <updated>1680968678579</updated>
     </task>
-    <option name="localTasksCounter" value="5"/>
+    <task id="LOCAL-00005" summary="feat: added and upgraded: settings, up, ps, logs, stop, down, build, rebuild, docs, search_adjacent_setting, generate_password, settings, volumes and helpers.
+
+including new dependencies: tabulate, pyyaml, diceware and tomlkit
+
+Fixed some inspections.">
+      <created>1681082009694</created>
+      <option name="number" value="00005"/>
+      <option name="presentableId" value="LOCAL-00005"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1681082009694</updated>
+    </task>
+    <option name="localTasksCounter" value="6"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -112,10 +126,19 @@
     </option>
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="feat: added `plugins` as an optional dependencies"/>
     <MESSAGE value="fix: added `edwh-demo-tasks-plugin` as a `plugins` optional dependency"/>
     <MESSAGE value="build: version bump"/>
     <MESSAGE value="fix: added `tomlkit` dependency voor `omgeving`, changed the output of the discovered plugins list."/>
-    <option name="LAST_COMMIT_MESSAGE" value="fix: added `tomlkit` dependency voor `omgeving`, changed the output of the discovered plugins list."/>
+    <MESSAGE value="feat: added and upgraded: settings, up, ps, logs, stop, down, build, rebuild, docs, search_adjacent_setting, generate_password, settings, volumes and helpers.
+
+including new dependencies: tabulate, pyyaml, diceware and tomlkit
+
+Fixed some inspections."/>
+    <option name="LAST_COMMIT_MESSAGE" value="feat: added and upgraded: settings, up, ps, logs, stop, down, build, rebuild, docs, search_adjacent_setting, generate_password, settings, volumes and helpers.
+
+including new dependencies: tabulate, pyyaml, diceware and tomlkit
+
+Fixed some inspections."/>
   </component>
 </project>
```

### Comparing `edwh-0.3.0/c/edwh-0.3.0-py3-none-any.whl` & `edwh-0.3.1/c/edwh-0.3.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `edwh-0.3.0/c/edwh-0.3.0.tar.gz` & `edwh-0.3.1/c/edwh-0.3.0.tar.gz`

 * *Files identical despite different names*

### Comparing `edwh-0.3.0/src/edwh/cli.py` & `edwh-0.3.1/src/edwh/cli.py`

 * *Files identical despite different names*

### Comparing `edwh-0.3.0/src/edwh/tasks.py` & `edwh-0.3.1/src/edwh/tasks.py`

 * *Files identical despite different names*

### Comparing `edwh-0.3.0/LICENSE.txt` & `edwh-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh-0.3.0/README.md` & `edwh-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `edwh-0.3.0/pyproject.toml` & `edwh-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh-0.3.0/PKG-INFO` & `edwh-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh
-Version: 0.3.0
+Version: 0.3.1
 Summary: Education Warehouse maintenance tools
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>, Romy Schöller <romy.s@educationwarehouse.nl>, Sven Keimpema <sven.k@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```


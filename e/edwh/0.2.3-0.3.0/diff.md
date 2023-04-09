# Comparing `tmp/edwh-0.2.3.tar.gz` & `tmp/edwh-0.3.0.tar.gz`

## Comparing `edwh-0.2.3.tar` & `edwh-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 edwh-0.2.3/CHANGELOG.md
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 edwh-0.2.3/.idea/.gitignore
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 edwh-0.2.3/.idea/edwh.iml
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 edwh-0.2.3/.idea/jupyter-settings.xml
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 edwh-0.2.3/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 edwh-0.2.3/.idea/modules.xml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh-0.2.3/.idea/vcs.xml
--rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 edwh-0.2.3/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh-0.2.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.2.3/src/edwh/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.2.3/src/edwh/__init__.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 edwh-0.2.3/src/edwh/cli.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 edwh-0.2.3/src/edwh/tasks.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.2.3/LICENSE.txt
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 edwh-0.2.3/README.md
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 edwh-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 edwh-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 edwh-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 edwh-0.3.0/.idea/.gitignore
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 edwh-0.3.0/.idea/edwh.iml
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 edwh-0.3.0/.idea/jupyter-settings.xml
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 edwh-0.3.0/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 edwh-0.3.0/.idea/modules.xml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh-0.3.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     5801 2020-02-02 00:00:00.000000 edwh-0.3.0/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh-0.3.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     9468 2020-02-02 00:00:00.000000 edwh-0.3.0/c/edwh-0.3.0-py3-none-any.whl
+-rw-r--r--   0        0        0    12057 2020-02-02 00:00:00.000000 edwh-0.3.0/c/edwh-0.3.0.tar.gz
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.3.0/src/edwh/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.3.0/src/edwh/__init__.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 edwh-0.3.0/src/edwh/cli.py
+-rw-r--r--   0        0        0    17003 2020-02-02 00:00:00.000000 edwh-0.3.0/src/edwh/tasks.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 edwh-0.3.0/README.md
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 edwh-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 edwh-0.3.0/PKG-INFO
```

### Comparing `edwh-0.2.3/CHANGELOG.md` & `edwh-0.3.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `edwh-0.2.3/.idea/jupyter-settings.xml` & `edwh-0.3.0/.idea/jupyter-settings.xml`

 * *Files identical despite different names*

### Comparing `edwh-0.2.3/.idea/workspace.xml` & `edwh-0.3.0/.idea/workspace.xml`

 * *Files 8% similar despite different names*

#### Comparing `edwh-0.2.3/.idea/workspace.xml` & `edwh-0.3.0/.idea/workspace.xml`

```diff
@@ -1,15 +1,18 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
+  <component name="BlackConnectSettings" triggerOnReformat="true"/>
   <component name="ChangeListManager">
     <list default="true" id="a8ee968c-c8d6-4911-ae81-e260b5e9d9f0" name="Changes" comment="fix: added `tomlkit` dependency voor `omgeving`, changed the output of the discovered plugins list.">
       <change beforePath="$PROJECT_DIR$/.idea/vcs.xml" beforeDir="false" afterPath="$PROJECT_DIR$/.idea/vcs.xml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/edwh/tasks.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/edwh/tasks.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
@@ -25,27 +28,28 @@
   </component>
   <component name="ProjectId" id="2O1KNWZ6CP36BVEqAMkUxvDRxX7"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showExcludedFiles" value="false"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent">{
-  &quot;keyToString&quot;: {
-    &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
-    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
-    &quot;SHARE_PROJECT_CONFIGURATION_FILES&quot;: &quot;true&quot;,
-    &quot;WebServerToolWindowFactoryState&quot;: &quot;false&quot;,
-    &quot;git-widget-placeholder&quot;: &quot;main&quot;,
-    &quot;node.js.detected.package.eslint&quot;: &quot;true&quot;,
-    &quot;node.js.selected.package.eslint&quot;: &quot;(autodetect)&quot;,
-    &quot;nodejs_package_manager_path&quot;: &quot;npm&quot;,
-    &quot;vue.rearranger.settings.migration&quot;: &quot;true&quot;
+  <component name="PropertiesComponent"><![CDATA[{
+  "keyToString": {
+    "RunOnceActivity.OpenProjectViewOnStart": "true",
+    "RunOnceActivity.ShowReadmeOnStart": "true",
+    "SHARE_PROJECT_CONFIGURATION_FILES": "true",
+    "WebServerToolWindowFactoryState": "false",
+    "git-widget-placeholder": "main",
+    "node.js.detected.package.eslint": "true",
+    "node.js.selected.package.eslint": "(autodetect)",
+    "nodejs_package_manager_path": "npm",
+    "settings.editor.selected.configurable": "me.lensvol.blackconnect.settings",
+    "vue.rearranger.settings.migration": "true"
   }
-}</component>
+}]]></component>
   <component name="RecentsManager">
     <key name="OPEN_URL_DIALOG">
       <recent name="https://github.com/educationwarehouse/edwh-demo-tasks-plugin"/>
     </key>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
@@ -56,15 +60,15 @@
       <option name="presentableId" value="Default"/>
       <updated>1680722607644</updated>
       <workItem from="1680722608717" duration="182000"/>
       <workItem from="1680724415156" duration="2074000"/>
       <workItem from="1680965546116" duration="403000"/>
       <workItem from="1680967358935" duration="3652000"/>
       <workItem from="1681073068492" duration="64000"/>
-      <workItem from="1681073149934" duration="817000"/>
+      <workItem from="1681073149934" duration="8673000"/>
     </task>
     <task id="LOCAL-00001" summary="feat: added `plugins` as an optional dependencies">
       <created>1680724520623</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1680724520623</updated>
```

### Comparing `edwh-0.2.3/src/edwh/cli.py` & `edwh-0.3.0/src/edwh/cli.py`

 * *Files identical despite different names*

### Comparing `edwh-0.2.3/LICENSE.txt` & `edwh-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh-0.2.3/README.md` & `edwh-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `edwh-0.2.3/pyproject.toml` & `edwh-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,26 +26,31 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   'invoke',
   'importlib_metadata >=3.6 ; python_version < "3.10"',
+  'tabulate',
+  'pyyaml',
+  'tomlkit',
+  'diceware',
 ]
 [project.optional-dependencies]
 omgeving = [
   'humanize',
   'tabulate',
   'pyyaml',
   'tomlkit'
 ]
 plugins = [
   'edwh-multipass-plugin',
   'edwh-demo-tasks-plugin',
   'edwh-restic-plugin',
+  #'edwh-pipcompile-plugin'
 ]
 
 [project.scripts]
 edwh = "edwh.cli:program.run"
 ew = "edwh.cli:program.run"
 
 [project.urls]
```

### Comparing `edwh-0.2.3/PKG-INFO` & `edwh-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh
-Version: 0.2.3
+Version: 0.3.0
 Summary: Education Warehouse maintenance tools
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>, Romy Schöller <romy.s@educationwarehouse.nl>, Sven Keimpema <sven.k@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -14,16 +14,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Requires-Dist: diceware
 Requires-Dist: importlib-metadata>=3.6; python_version < '3.10'
 Requires-Dist: invoke
+Requires-Dist: pyyaml
+Requires-Dist: tabulate
+Requires-Dist: tomlkit
 Provides-Extra: omgeving
 Requires-Dist: humanize; extra == 'omgeving'
 Requires-Dist: pyyaml; extra == 'omgeving'
 Requires-Dist: tabulate; extra == 'omgeving'
 Requires-Dist: tomlkit; extra == 'omgeving'
 Provides-Extra: plugins
 Requires-Dist: edwh-demo-tasks-plugin; extra == 'plugins'
```


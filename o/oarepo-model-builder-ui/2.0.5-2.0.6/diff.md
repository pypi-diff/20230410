# Comparing `tmp/oarepo-model-builder-ui-2.0.5.tar.gz` & `tmp/oarepo-model-builder-ui-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-ui-2.0.5.tar", last modified: Fri Apr  7 10:52:04 2023, max compression
+gzip compressed data, was "oarepo-model-builder-ui-2.0.6.tar", last modified: Mon Apr 10 12:04:04 2023, max compression
```

## Comparing `oarepo-model-builder-ui-2.0.5.tar` & `oarepo-model-builder-ui-2.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:52:04.414441 oarepo-model-builder-ui-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-07 10:52:04.414441 oarepo-model-builder-ui-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-07 10:49:53.000000 oarepo-model-builder-ui-2.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:52:04.414441 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 10:49:53.000000 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-07 10:49:53.000000 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:52:04.414441 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 10:49:53.000000 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-07 10:49:53.000000 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/invenio/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-07 10:49:53.000000 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/invenio/i18n_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-07 10:49:53.000000 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/invenio/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-07 10:49:53.000000 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/invenio/layout_setup_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:52:04.414441 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/model_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 10:49:53.000000 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/model_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-07 10:49:53.000000 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/model_preprocessors/layout_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:52:04.414441 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-07 10:49:53.000000 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/outputs/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-07 10:49:53.000000 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/outputs/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:52:04.414441 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-07 10:49:53.000000 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:52:04.414441 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-07 10:52:04.000000 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-07 10:52:04.000000 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 10:52:04.000000 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-07 10:52:04.000000 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-07 10:52:04.000000 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-07 10:52:04.000000 oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-07 10:49:53.000000 oarepo-model-builder-ui-2.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-07 10:52:04.414441 oarepo-model-builder-ui-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 10:49:53.000000 oarepo-model-builder-ui-2.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:52:04.414441 oarepo-model-builder-ui-2.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-07 10:49:53.000000 oarepo-model-builder-ui-2.0.5/tests/test_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/i18n_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/layout_setup_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/model_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/model_preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/model_preprocessors/layout_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/outputs/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/outputs/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-10 12:04:04.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-10 12:04:04.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:04:04.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-10 12:04:04.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-10 12:04:04.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 12:04:04.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/tests/test_translation.py
```

### Comparing `oarepo-model-builder-ui-2.0.5/PKG-INFO` & `oarepo-model-builder-ui-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-ui
-Version: 2.0.5
+Version: 2.0.6
 Summary: Model builder plugin for oarepo-ui
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 <!--
  Copyright (c) 2022 CESNET
```

### Comparing `oarepo-model-builder-ui-2.0.5/README.md` & `oarepo-model-builder-ui-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/invenio/i18n.py` & `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/invenio/i18n_setup_cfg.py` & `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/i18n_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/invenio/layout.py` & `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/layout.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/invenio/layout_setup_cfg.py` & `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/layout_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/model_preprocessors/layout_settings.py` & `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/model_preprocessors/layout_settings.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/outputs/i18n.py` & `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/outputs/i18n.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,18 +5,21 @@
 
 
 class POWrapper:
     """
     wrapper for polib.POFile that adds lookup dictionary for entries (to speed up adding new entries)
     """
 
-    def __init__(self, po) -> None:
+    def __init__(self, po, remove_empty=False) -> None:
         self.po = po
         self.lookup = {}
-        for entry in po:
+        for entry in list(po):
+            if remove_empty and not entry.msgstr:
+                po.remove(entry)
+                continue
             self.lookup[entry.msgid] = entry
 
     def add(self, key, value):
         if key in self.lookup:
             entry = self.lookup[key]
             if not entry.msgstr:
                 entry.msgstr = value
@@ -44,15 +47,17 @@
             lang_path = Path(self.path) / lang / "LC_MESSAGES" / "messages.po"
             self._init_lang_path(lang, lang_path)
         self._init_lang_path(None, Path(self.path) / "messages.pot")
 
     def _init_lang_path(self, lang, lang_path):
         if self.builder.filesystem.exists(lang_path):
             with self.builder.filesystem.open(lang_path) as f:
-                self.po_files[lang] = POWrapper(polib.pofile(f.read()))
+                self.po_files[lang] = POWrapper(
+                    polib.pofile(f.read()), remove_empty=True
+                )
         else:
             po_file = polib.POFile()
             po_file.metadata = {
                 "Project-Id-Version": "1.0",
                 "POT-Creation-Date": datetime.datetime.now().isoformat(),
                 "PO-Revision-Date": datetime.datetime.now().isoformat(),
                 "MIME-Version": "1.0",
```

### Comparing `oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/outputs/layout.py` & `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/outputs/layout.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui/validation/__init__.py` & `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui.egg-info/PKG-INFO` & `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-ui
-Version: 2.0.5
+Version: 2.0.6
 Summary: Model builder plugin for oarepo-ui
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 <!--
  Copyright (c) 2022 CESNET
```

### Comparing `oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui.egg-info/SOURCES.txt` & `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.5/oarepo_model_builder_ui.egg-info/entry_points.txt` & `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.5/setup.cfg` & `oarepo-model-builder-ui-2.0.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-ui
-version = 2.0.5
+version = 2.0.6
 description = Model builder plugin for oarepo-ui
 authors = 
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```


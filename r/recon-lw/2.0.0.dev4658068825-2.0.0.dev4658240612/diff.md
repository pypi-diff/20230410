# Comparing `tmp/recon_lw-2.0.0.dev4658068825.tar.gz` & `tmp/recon_lw-2.0.0.dev4658240612.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4658068825.tar", last modified: Mon Apr 10 14:00:13 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4658240612.tar", last modified: Mon Apr 10 14:19:48 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4658068825.tar` & `recon_lw-2.0.0.dev4658240612.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-10 13:59:38.000000 recon_lw-2.0.0.dev4658068825/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-10 13:59:38.000000 recon_lw-2.0.0.dev4658068825/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-10 14:00:01.000000 recon_lw-2.0.0.dev4658068825/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-10 13:59:38.000000 recon_lw-2.0.0.dev4658068825/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-10 13:59:38.000000 recon_lw-2.0.0.dev4658068825/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    13155 2023-04-10 13:59:38.000000 recon_lw-2.0.0.dev4658068825/recon_lw/recon_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-10 13:59:38.000000 recon_lw-2.0.0.dev4658068825/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-10 13:59:38.000000 recon_lw-2.0.0.dev4658068825/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-10 14:19:14.000000 recon_lw-2.0.0.dev4658240612/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-10 14:19:14.000000 recon_lw-2.0.0.dev4658240612/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-10 14:19:37.000000 recon_lw-2.0.0.dev4658240612/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-10 14:19:14.000000 recon_lw-2.0.0.dev4658240612/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-10 14:19:14.000000 recon_lw-2.0.0.dev4658240612/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13155 2023-04-10 14:19:14.000000 recon_lw-2.0.0.dev4658240612/recon_lw/recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-10 14:19:14.000000 recon_lw-2.0.0.dev4658240612/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 14:19:48.000000 recon_lw-2.0.0.dev4658240612/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-10 14:19:14.000000 recon_lw-2.0.0.dev4658240612/setup.py
```

### Comparing `recon_lw-2.0.0.dev4658068825/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4658240612/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4658068825/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4658240612/recon_lw/recon_ob.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
     n_processed = process_ob_rules(seq_batch,
                                    rule_settings["books_cache"],
                                    rule_settings["get_book_id"],
                                    rule_settings["update_book_rule"],
                                    rule_settings["check_book_rule"],
                                    event_sequence,
                                    save_events_func,
-                                   rule_settings["rule_root_event"].
+                                   rule_settings["rule_root_event"],
                                    rule_settings["initial_book_params"])
     ## Process duplicated
     duplicates = rule_settings["sequence_cache"]["duplicates"]
     n_dupl = len(duplicates)
     dupl_events = []
     for i in range(0,n_dupl):
         item = duplicates.pop(0)
```

### Comparing `recon_lw-2.0.0.dev4658068825/setup.py` & `recon_lw-2.0.0.dev4658240612/setup.py`

 * *Files identical despite different names*


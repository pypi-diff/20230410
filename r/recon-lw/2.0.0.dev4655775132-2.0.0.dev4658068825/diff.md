# Comparing `tmp/recon_lw-2.0.0.dev4655775132.tar.gz` & `tmp/recon_lw-2.0.0.dev4658068825.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4655775132.tar", last modified: Mon Apr 10 08:12:23 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4658068825.tar", last modified: Mon Apr 10 14:00:13 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4655775132.tar` & `recon_lw-2.0.0.dev4658068825.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-10 08:11:47.000000 recon_lw-2.0.0.dev4655775132/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-10 08:11:47.000000 recon_lw-2.0.0.dev4655775132/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-10 08:12:11.000000 recon_lw-2.0.0.dev4655775132/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-10 08:11:47.000000 recon_lw-2.0.0.dev4655775132/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-10 08:11:47.000000 recon_lw-2.0.0.dev4655775132/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    12936 2023-04-10 08:11:47.000000 recon_lw-2.0.0.dev4655775132/recon_lw/recon_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-10 08:11:47.000000 recon_lw-2.0.0.dev4655775132/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 08:12:23.000000 recon_lw-2.0.0.dev4655775132/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-10 08:11:47.000000 recon_lw-2.0.0.dev4655775132/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-10 13:59:38.000000 recon_lw-2.0.0.dev4658068825/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-10 13:59:38.000000 recon_lw-2.0.0.dev4658068825/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-10 14:00:01.000000 recon_lw-2.0.0.dev4658068825/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-10 13:59:38.000000 recon_lw-2.0.0.dev4658068825/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-10 13:59:38.000000 recon_lw-2.0.0.dev4658068825/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13155 2023-04-10 13:59:38.000000 recon_lw-2.0.0.dev4658068825/recon_lw/recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-10 13:59:38.000000 recon_lw-2.0.0.dev4658068825/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 14:00:13.000000 recon_lw-2.0.0.dev4658068825/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-10 13:59:38.000000 recon_lw-2.0.0.dev4658068825/setup.py
```

### Comparing `recon_lw-2.0.0.dev4655775132/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4658068825/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4655775132/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4658068825/recon_lw/recon_ob.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,27 +61,28 @@
 def flush_sequence_clear_cache(processed_len, sequence_cache):
     sequence = sequence_cache["sequence"]
     for i in range(0, processed_len):
         sequence.pop(0)
 
 
 def process_market_data_update(mess, events,  books_cache, get_book_id_func ,update_book_rule,
-                               check_book_rule, event_sequence, parent_event):
+                               check_book_rule, event_sequence, parent_event, initial_book_params):
     book_id, result = get_book_id_func(mess)
     if result is not None:
         book_id_event = recon_lw.create_event("GetBookEroor:" + parent_event["eventName"], "GetBookEroor", event_sequence,
                                               ok=False,
                                               body=result,
                                               parentId=parent_event["eventId"])
         book_id_event["attachedMessageIds"] = [mess["messageId"]]
         events.append(book_id_event)
 
     if book_id is not None:
         if book_id not in books_cache:
-            books_cache[book_id] = {"ask": {}, "bid": {}, "status": "?"}
+            books_cache[book_id] = copy.deepcopy(initial_book_params)            
+            #books_cache[book_id] = {"ask": {}, "bid": {}, "status": "?"}
         book = books_cache[book_id]
         initial_book = copy.deepcopy(book)
         operation, parameters = update_book_rule(book, mess)
         if operation is None:
             return 
         initial_parameters = copy.copy(parameters)
         parameters["order_book"] = book
@@ -108,30 +109,30 @@
                 r["body"]["book_id"] = book_id
                 r["parentEventId"] = parent_event["eventId"]
                 r["attachedMessageIds"] = [mess["messageId"]]
                 events.append(r)
 
 
 def process_ob_rules(sequenced_batch, books_cache, get_book_id_func ,update_book_rule,
-                     check_book_rule, event_sequence, send_events_func, parent_event):
+                     check_book_rule, event_sequence, send_events_func, parent_event, initial_book_params):
     events = []
     n_processed = 0
     for m in sequenced_batch:
         seq = m[0]
         mess = m[1]
         #process gaps
         if "gap" in mess:
             gap_event = recon_lw.create_event("SeqGap:" + parent_event["eventName"],"SeqGap",event_sequence,ok=False,
                                               body={"seq_num": seq} ,parentId=parent_event["eventId"])
             events.append(gap_event)
             continue
         chunk = message_utils.expand_message(mess)
         for m_upd in chunk:
             process_market_data_update(m_upd, events, books_cache, get_book_id_func, update_book_rule,
-                                       check_book_rule, event_sequence, parent_event)
+                                       check_book_rule, event_sequence, parent_event, initial_book_params)
         n_processed += 1
 
     send_events_func(events)
     return n_processed
 
 
 def init_ob_stream(rule_settings):
@@ -158,15 +159,16 @@
     n_processed = process_ob_rules(seq_batch,
                                    rule_settings["books_cache"],
                                    rule_settings["get_book_id"],
                                    rule_settings["update_book_rule"],
                                    rule_settings["check_book_rule"],
                                    event_sequence,
                                    save_events_func,
-                                   rule_settings["rule_root_event"])
+                                   rule_settings["rule_root_event"].
+                                   rule_settings["initial_book_params"])
     ## Process duplicated
     duplicates = rule_settings["sequence_cache"]["duplicates"]
     n_dupl = len(duplicates)
     dupl_events = []
     for i in range(0,n_dupl):
         item = duplicates.pop(0)
         d_ev = recon_lw.create_event("Duplicate:" + rule_settings["rule_root_event"]["eventName"],"Duplicate",
```

### Comparing `recon_lw-2.0.0.dev4655775132/setup.py` & `recon_lw-2.0.0.dev4658068825/setup.py`

 * *Files identical despite different names*


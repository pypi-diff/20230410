# Comparing `tmp/posthoganalytics-2.4.2.tar.gz` & `tmp/posthoganalytics-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posthoganalytics-2.4.2.tar", last modified: Thu Mar 30 14:35:51 2023, max compression
+gzip compressed data, was "posthoganalytics-2.5.0.tar", last modified: Mon Apr 10 19:14:07 2023, max compression
```

## Comparing `posthoganalytics-2.4.2.tar` & `posthoganalytics-2.5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:35:51.274401 posthoganalytics-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-03-30 14:35:22.000000 posthoganalytics-2.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-03-30 14:35:22.000000 posthoganalytics-2.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1224 2023-03-30 14:35:51.274401 posthoganalytics-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2207 2023-03-30 14:35:22.000000 posthoganalytics-2.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:35:51.270401 posthoganalytics-2.4.2/posthoganalytics/
--rw-r--r--   0 runner    (1001) docker     (122)    12342 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24681 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4315 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)    10578 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics/poller.py
--rw-r--r--   0 runner    (1001) docker     (122)     3554 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics/request.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:35:51.274401 posthoganalytics-2.4.2/posthoganalytics/sentry/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics/sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      780 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics/sentry/django.py
--rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics/sentry/posthog_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:35:51.274401 posthoganalytics-2.4.2/posthoganalytics/test/
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19772 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6352 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics/test/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)   125824 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics/test/test_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)      982 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics/test/test_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     1720 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics/test/test_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:35:51.274401 posthoganalytics-2.4.2/posthoganalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1224 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      891 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-03-30 14:35:51.000000 posthoganalytics-2.4.2/posthoganalytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-03-30 14:35:22.000000 posthoganalytics-2.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-03-30 14:35:51.274401 posthoganalytics-2.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-03-30 14:35:22.000000 posthoganalytics-2.4.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-03-30 14:35:22.000000 posthoganalytics-2.4.2/setup_analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:14:07.891819 posthoganalytics-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-04-10 19:13:52.000000 posthoganalytics-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-10 19:13:52.000000 posthoganalytics-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1224 2023-04-10 19:14:07.891819 posthoganalytics-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2207 2023-04-10 19:13:52.000000 posthoganalytics-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:14:07.887819 posthoganalytics-2.5.0/posthoganalytics/
+-rw-r--r--   0 runner    (1001) docker     (122)    12474 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24803 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4315 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10578 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics/poller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3554 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics/request.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:14:07.891819 posthoganalytics-2.5.0/posthoganalytics/sentry/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      780 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics/sentry/django.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics/sentry/posthog_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:14:07.891819 posthoganalytics-2.5.0/posthoganalytics/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20693 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6352 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics/test/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)   125824 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics/test/test_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics/test/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1720 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics/test/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:14:07.887819 posthoganalytics-2.5.0/posthoganalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1224 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      891 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-10 19:14:07.000000 posthoganalytics-2.5.0/posthoganalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-04-10 19:13:52.000000 posthoganalytics-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-04-10 19:14:07.891819 posthoganalytics-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-04-10 19:13:52.000000 posthoganalytics-2.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-04-10 19:13:52.000000 posthoganalytics-2.5.0/setup_analytics.py
```

### Comparing `posthoganalytics-2.4.2/LICENSE` & `posthoganalytics-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `posthoganalytics-2.4.2/PKG-INFO` & `posthoganalytics-2.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posthoganalytics
-Version: 2.4.2
+Version: 2.5.0
 Summary: Integrate PostHog into any python application.
 Home-page: https://github.com/posthog/posthog-python
 Author: Posthog
 Author-email: hey@posthog.com
 Maintainer: PostHog
 Maintainer-email: hey@posthog.com
 License: MIT License
```

### Comparing `posthoganalytics-2.4.2/README.md` & `posthoganalytics-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `posthoganalytics-2.4.2/posthoganalytics/__init__.py` & `posthoganalytics-2.5.0/posthoganalytics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         context=context,
         timestamp=timestamp,
         uuid=uuid,
     )
 
 
 def set(
-    distinct_id,  # type: str,
+    distinct_id,  # type: str
     properties=None,  # type: Optional[Dict]
     context=None,  # type: Optional[Dict]
     timestamp=None,  # type: Optional[datetime.datetime]
     uuid=None,  # type: Optional[str]
 ):
     # type: (...) -> None
     """
@@ -128,15 +128,15 @@
         context=context,
         timestamp=timestamp,
         uuid=uuid,
     )
 
 
 def set_once(
-    distinct_id,  # type: str,
+    distinct_id,  # type: str
     properties=None,  # type: Optional[Dict]
     context=None,  # type: Optional[Dict]
     timestamp=None,  # type: Optional[datetime.datetime]
     uuid=None,  # type: Optional[str]
 ):
     # type: (...) -> None
     """
@@ -196,16 +196,16 @@
         context=context,
         timestamp=timestamp,
         uuid=uuid,
     )
 
 
 def alias(
-    previous_id,  # type: str,
-    distinct_id,  # type: str,
+    previous_id,  # type: str
+    distinct_id,  # type: str
     context=None,  # type: Optional[Dict]
     timestamp=None,  # type: Optional[datetime.datetime]
     uuid=None,  # type: Optional[str]
 ):
     # type: (...) -> None
     """
     To marry up whatever a user does before they sign up or log in with what they do after you need to make an alias call. This will allow you to answer questions like "Which marketing channels leads to users churning after a month?" or "What do users do on our website before signing up?"
@@ -230,16 +230,16 @@
         context=context,
         timestamp=timestamp,
         uuid=uuid,
     )
 
 
 def feature_enabled(
-    key,  # type: str,
-    distinct_id,  # type: str,
+    key,  # type: str
+    distinct_id,  # type: str
     groups={},  # type: dict
     person_properties={},  # type: dict
     group_properties={},  # type: dict
     only_evaluate_locally=False,  # type: bool
     send_feature_flag_events=True,  # type: bool
 ):
     # type: (...) -> bool
@@ -265,16 +265,16 @@
         group_properties=group_properties,
         only_evaluate_locally=only_evaluate_locally,
         send_feature_flag_events=send_feature_flag_events,
     )
 
 
 def get_feature_flag(
-    key,  # type: str,
-    distinct_id,  # type: str,
+    key,  # type: str
+    distinct_id,  # type: str
     groups={},  # type: dict
     person_properties={},  # type: dict
     group_properties={},  # type: dict
     only_evaluate_locally=False,  # type: bool
     send_feature_flag_events=True,  # type: bool
 ):
     """
@@ -308,15 +308,15 @@
         group_properties=group_properties,
         only_evaluate_locally=only_evaluate_locally,
         send_feature_flag_events=send_feature_flag_events,
     )
 
 
 def get_all_flags(
-    distinct_id,  # type: str,
+    distinct_id,  # type: str
     groups={},  # type: dict
     person_properties={},  # type: dict
     group_properties={},  # type: dict
     only_evaluate_locally=False,  # type: bool
 ):
     """
     Get all flags for a given user.
@@ -402,24 +402,31 @@
     _proxy("flush")
     _proxy("join")
 
 
 def _proxy(method, *args, **kwargs):
     """Create an analytics client if one doesn't exist and send to it."""
     global default_client
-    if disabled:
-        return None
     if not default_client:
         default_client = Client(
             api_key,
             host=host,
             debug=debug,
             on_error=on_error,
             send=send,
             sync_mode=sync_mode,
             personal_api_key=personal_api_key,
             project_api_key=project_api_key,
             poll_interval=poll_interval,
+            disabled=disabled,
         )
 
+    # always set incase user changes it
+    default_client.disabled = disabled
+    default_client.debug = debug
+
     fn = getattr(default_client, method)
     return fn(*args, **kwargs)
+
+
+class Posthog(Client):
+    pass
```

### Comparing `posthoganalytics-2.4.2/posthoganalytics/client.py` & `posthoganalytics-2.5.0/posthoganalytics/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         max_retries=3,
         sync_mode=False,
         timeout=15,
         thread=1,
         poll_interval=30,
         personal_api_key=None,
         project_api_key=None,
+        disabled=False,
     ):
         self.queue = queue.Queue(max_queue_size)
 
         # api_key: This should be the Team API Key (token), public
         self.api_key = project_api_key or api_key
 
         require("api_key", self.api_key, string_types)
@@ -65,14 +66,15 @@
         self.feature_flags = None
         self.feature_flags_by_key = None
         self.group_type_mapping = None
         self.cohorts = None
         self.poll_interval = poll_interval
         self.poller = None
         self.distinct_ids_feature_flags_reported = SizeLimitedDict(MAX_DICT_SIZE, set)
+        self.disabled = disabled
 
         # personal_api_key: This should be a generated Personal API Key, private
         self.personal_api_key = personal_api_key
         if debug:
             # Ensures that debug level messages are logged when debug mode is on.
             # Otherwise, defaults to WARNING level. See https://docs.python.org/3/howto/logging.html#what-happens-if-no-configuration-is-provided
             logging.basicConfig()
@@ -295,14 +297,18 @@
             "uuid": uuid,
         }
 
         return self._enqueue(msg)
 
     def _enqueue(self, msg):
         """Push a new `msg` onto the queue, return `(success, msg)`"""
+
+        if self.disabled:
+            return False, "disabled"
+
         timestamp = msg["timestamp"]
         if timestamp is None:
             timestamp = datetime.utcnow().replace(tzinfo=tzutc())
 
         require("timestamp", timestamp, datetime)
         require("context", msg["context"], dict)
```

### Comparing `posthoganalytics-2.4.2/posthoganalytics/consumer.py` & `posthoganalytics-2.5.0/posthoganalytics/consumer.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-2.4.2/posthoganalytics/feature_flags.py` & `posthoganalytics-2.5.0/posthoganalytics/feature_flags.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-2.4.2/posthoganalytics/poller.py` & `posthoganalytics-2.5.0/posthoganalytics/poller.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-2.4.2/posthoganalytics/request.py` & `posthoganalytics-2.5.0/posthoganalytics/request.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-2.4.2/posthoganalytics/sentry/django.py` & `posthoganalytics-2.5.0/posthoganalytics/sentry/django.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-2.4.2/posthoganalytics/sentry/posthog_integration.py` & `posthoganalytics-2.5.0/posthoganalytics/sentry/posthog_integration.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-2.4.2/posthoganalytics/test/test_client.py` & `posthoganalytics-2.5.0/posthoganalytics/test/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,14 +464,40 @@
             self.assertEqual(consumer.timeout, 10)
 
     def test_default_timeout_15(self):
         client = Client(FAKE_TEST_API_KEY)
         for consumer in client.consumers:
             self.assertEqual(consumer.timeout, 15)
 
+    def test_disabled(self):
+        client = Client(FAKE_TEST_API_KEY, on_error=self.set_fail, disabled=True)
+        success, msg = client.capture("distinct_id", "python test event")
+        client.flush()
+        self.assertFalse(success)
+        self.assertFalse(self.failed)
+
+        self.assertEqual(msg, "disabled")
+
+    def test_enabled_to_disabled(self):
+        client = Client(FAKE_TEST_API_KEY, on_error=self.set_fail, disabled=False)
+        success, msg = client.capture("distinct_id", "python test event")
+        client.flush()
+
+        self.assertTrue(success)
+        self.assertFalse(self.failed)
+        self.assertEqual(msg["event"], "python test event")
+
+        client.disabled = True
+        success, msg = client.capture("distinct_id", "python test event")
+        client.flush()
+        self.assertFalse(success)
+        self.assertFalse(self.failed)
+
+        self.assertEqual(msg, "disabled")
+
     @mock.patch("posthog.client.Poller")
     @mock.patch("posthog.client.get")
     def test_call_identify_fails(self, patch_get, patch_poll):
         def raise_effect():
             raise Exception("http exception")
 
         patch_get.return_value.raiseError.side_effect = raise_effect
```

### Comparing `posthoganalytics-2.4.2/posthoganalytics/test/test_consumer.py` & `posthoganalytics-2.5.0/posthoganalytics/test/test_consumer.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-2.4.2/posthoganalytics/test/test_feature_flags.py` & `posthoganalytics-2.5.0/posthoganalytics/test/test_feature_flags.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-2.4.2/posthoganalytics/test/test_request.py` & `posthoganalytics-2.5.0/posthoganalytics/test/test_request.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-2.4.2/posthoganalytics/test/test_utils.py` & `posthoganalytics-2.5.0/posthoganalytics/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-2.4.2/posthoganalytics/utils.py` & `posthoganalytics-2.5.0/posthoganalytics/utils.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-2.4.2/posthoganalytics.egg-info/PKG-INFO` & `posthoganalytics-2.5.0/posthoganalytics.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posthoganalytics
-Version: 2.4.2
+Version: 2.5.0
 Summary: Integrate PostHog into any python application.
 Home-page: https://github.com/posthog/posthog-python
 Author: Posthog
 Author-email: hey@posthog.com
 Maintainer: PostHog
 Maintainer-email: hey@posthog.com
 License: MIT License
```

### Comparing `posthoganalytics-2.4.2/posthoganalytics.egg-info/SOURCES.txt` & `posthoganalytics-2.5.0/posthoganalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `posthoganalytics-2.4.2/setup.py` & `posthoganalytics-2.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `posthoganalytics-2.4.2/setup_analytics.py` & `posthoganalytics-2.5.0/setup_analytics.py`

 * *Files identical despite different names*


# Comparing `tmp/django_pgpubsub-1.0.3.tar.gz` & `tmp/django_pgpubsub-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pgpubsub-1.0.3.tar", max compression
+gzip compressed data, was "django_pgpubsub-1.0.4.tar", max compression
```

## Comparing `django_pgpubsub-1.0.3.tar` & `django_pgpubsub-1.0.4.tar`

### file list

```diff
@@ -1,28 +1,24 @@
--rw-r--r--   0        0        0     1456 2022-11-05 17:21:11.401611 django_pgpubsub-1.0.3/LICENSE
--rw-r--r--   0        0        0    25981 2023-01-10 19:35:52.721302 django_pgpubsub-1.0.3/README.md
--rw-r--r--   0        0        0      390 2022-11-05 17:21:11.403909 django_pgpubsub-1.0.3/pgpubsub/__init__.py
--rw-r--r--   0        0        0     5843 2023-04-08 10:44:01.456137 django_pgpubsub-1.0.3/pgpubsub/channel.py
--rw-r--r--   0        0        0     4980 2023-02-02 16:18:56.082239 django_pgpubsub-1.0.3/pgpubsub/listen.py
--rw-r--r--   0        0        0     2647 2023-01-10 17:48:32.840212 django_pgpubsub-1.0.3/pgpubsub/listeners.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.404451 django_pgpubsub-1.0.3/pgpubsub/management/__init__.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.404567 django_pgpubsub-1.0.3/pgpubsub/management/commands/__init__.py
--rw-r--r--   0        0        0     1288 2023-02-02 16:18:56.082808 django_pgpubsub-1.0.3/pgpubsub/management/commands/listen.py
--rw-r--r--   0        0        0      751 2023-04-08 10:44:01.456747 django_pgpubsub-1.0.3/pgpubsub/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.405068 django_pgpubsub-1.0.3/pgpubsub/migrations/__init__.py
--rw-r--r--   0        0        0      690 2023-04-08 10:44:01.457008 django_pgpubsub-1.0.3/pgpubsub/models.py
--rw-r--r--   0        0        0     2130 2022-11-05 17:21:11.405511 django_pgpubsub-1.0.3/pgpubsub/notify.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.405631 django_pgpubsub-1.0.3/pgpubsub/tests/__init__.py
--rw-r--r--   0        0        0      164 2022-11-05 17:21:11.405752 django_pgpubsub-1.0.3/pgpubsub/tests/apps.py
--rw-r--r--   0        0        0      640 2023-02-01 14:09:57.717907 django_pgpubsub-1.0.3/pgpubsub/tests/channels.py
--rw-r--r--   0        0        0     1938 2023-04-08 10:43:55.376913 django_pgpubsub-1.0.3/pgpubsub/tests/listeners.py
--rw-r--r--   0        0        0     2734 2022-11-05 17:21:11.406152 django_pgpubsub-1.0.3/pgpubsub/tests/migrations/0001_initial.py
--rw-r--r--   0        0        0     2869 2023-01-19 17:18:42.251074 django_pgpubsub-1.0.3/pgpubsub/tests/migrations/0002_author_pgpubsub_160cf_media_pgpubsub_a83de_and_more.py
--rw-r--r--   0        0        0      653 2023-01-19 18:43:55.169915 django_pgpubsub-1.0.3/pgpubsub/tests/migrations/0003_alter_author_user.py
--rw-r--r--   0        0        0      583 2023-02-02 13:53:06.887019 django_pgpubsub-1.0.3/pgpubsub/tests/migrations/0004_alter_author_user.py
--rw-r--r--   0        0        0     1257 2023-04-08 08:00:32.761709 django_pgpubsub-1.0.3/pgpubsub/tests/migrations/0005_remove_post_pgpubsub_72091_post_pgpubsub_72091.py
--rw-r--r--   0        0        0        0 2022-11-05 17:21:11.406217 django_pgpubsub-1.0.3/pgpubsub/tests/migrations/__init__.py
--rw-r--r--   0        0        0     1209 2023-02-02 13:52:43.296803 django_pgpubsub-1.0.3/pgpubsub/tests/models.py
--rw-r--r--   0        0        0     8890 2023-04-08 10:44:01.457320 django_pgpubsub-1.0.3/pgpubsub/tests/test_core.py
--rw-r--r--   0        0        0     1040 2023-04-08 10:44:01.457599 django_pgpubsub-1.0.3/pgpubsub/triggers.py
--rw-r--r--   0        0        0     2082 2023-04-08 10:45:43.484551 django_pgpubsub-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    27304 1970-01-01 00:00:00.000000 django_pgpubsub-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1456 2022-11-05 17:21:11.401611 django_pgpubsub-1.0.4/LICENSE
+-rw-r--r--   0        0        0    25976 2023-04-10 14:46:46.455426 django_pgpubsub-1.0.4/README.md
+-rw-r--r--   0        0        0      390 2022-11-05 17:21:11.403909 django_pgpubsub-1.0.4/pgpubsub/__init__.py
+-rw-r--r--   0        0        0     5843 2023-04-09 15:03:50.911492 django_pgpubsub-1.0.4/pgpubsub/channel.py
+-rw-r--r--   0        0        0     4980 2023-02-02 16:18:56.082239 django_pgpubsub-1.0.4/pgpubsub/listen.py
+-rw-r--r--   0        0        0     2647 2023-01-10 17:48:32.840212 django_pgpubsub-1.0.4/pgpubsub/listeners.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.404451 django_pgpubsub-1.0.4/pgpubsub/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.404567 django_pgpubsub-1.0.4/pgpubsub/management/commands/__init__.py
+-rw-r--r--   0        0        0     1288 2023-02-02 16:18:56.082808 django_pgpubsub-1.0.4/pgpubsub/management/commands/listen.py
+-rw-r--r--   0        0        0      751 2023-04-09 15:03:50.912029 django_pgpubsub-1.0.4/pgpubsub/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.405068 django_pgpubsub-1.0.4/pgpubsub/migrations/__init__.py
+-rw-r--r--   0        0        0      690 2023-04-09 15:03:50.912484 django_pgpubsub-1.0.4/pgpubsub/models.py
+-rw-r--r--   0        0        0     2130 2022-11-05 17:21:11.405511 django_pgpubsub-1.0.4/pgpubsub/notify.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.405631 django_pgpubsub-1.0.4/pgpubsub/tests/__init__.py
+-rw-r--r--   0        0        0      164 2022-11-05 17:21:11.405752 django_pgpubsub-1.0.4/pgpubsub/tests/apps.py
+-rw-r--r--   0        0        0      640 2023-02-01 14:09:57.717907 django_pgpubsub-1.0.4/pgpubsub/tests/channels.py
+-rw-r--r--   0        0        0     1938 2023-04-09 15:03:50.912969 django_pgpubsub-1.0.4/pgpubsub/tests/listeners.py
+-rw-r--r--   0        0        0     2734 2022-11-05 17:21:11.406152 django_pgpubsub-1.0.4/pgpubsub/tests/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-11-05 17:21:11.406217 django_pgpubsub-1.0.4/pgpubsub/tests/migrations/__init__.py
+-rw-r--r--   0        0        0     1209 2023-02-02 13:52:43.296803 django_pgpubsub-1.0.4/pgpubsub/tests/models.py
+-rw-r--r--   0        0        0     8890 2023-04-09 15:03:50.913480 django_pgpubsub-1.0.4/pgpubsub/tests/test_core.py
+-rw-r--r--   0        0        0     1040 2023-04-09 15:03:50.913993 django_pgpubsub-1.0.4/pgpubsub/triggers.py
+-rw-r--r--   0        0        0     2082 2023-04-10 14:46:01.186583 django_pgpubsub-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    27299 1970-01-01 00:00:00.000000 django_pgpubsub-1.0.4/PKG-INFO
```

### Comparing `django_pgpubsub-1.0.3/LICENSE` & `django_pgpubsub-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.3/README.md` & `django_pgpubsub-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 Highlights
 ==========
 
 - **Minimal Operational Infrastructure**: If you're already running a Django application
   on top of a Postgres database, the installation of this library is the sum total
   of the operational work required to implement a framework for a distributed
-  message processing framework. No additional servers or server configuration
-  is required.
+  message processing framework. No additional frameworks or technologies
+  are required.
 
 - **Integration with Postgres Triggers (via django-pgtrigger)**:
   To quote the [official](https://www.postgresql.org/docs/current/sql-notify.html)
   Postgres docs:
 
   *"When NOTIFY is used to signal the occurrence of changes to a particular table,
   a useful programming technique is to put the NOTIFY in a statement trigger that is triggered
@@ -82,15 +82,15 @@
   AMPQ queue.
 
 - If a message is sent using Postgres' ``NOTIFY`` and no process is listening at that time,
   the message is lost forever. As explained in the **Durability and Recovery** section above,
   pgpubsub can easily be configured so that we can replay "lost" messages, but this comes at the
   performance penalty of inserting a row into a table before sending each notification. This is the same
   penalty we must pay if we wish to have concurrent processes listening to the same channel without
-  duplicate notiifcation processing, as explained in the **Exactly-once notification processing** section above.
+  duplicate notifcation processing, as explained in the **Exactly-once notification processing** section above.
 
 
 Alternatives
 ============
 
 - [Celery](https://docs.celeryq.dev/en/stable/search.html?q=ampq): The canonical distributed message processing library for django based applications. This can handle large volumes of throughput and is well tested in production.
   It is however operationally quite heavy to maintain and set-up.
```

### Comparing `django_pgpubsub-1.0.3/pgpubsub/channel.py` & `django_pgpubsub-1.0.4/pgpubsub/channel.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.3/pgpubsub/listen.py` & `django_pgpubsub-1.0.4/pgpubsub/listen.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.3/pgpubsub/listeners.py` & `django_pgpubsub-1.0.4/pgpubsub/listeners.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.3/pgpubsub/management/commands/listen.py` & `django_pgpubsub-1.0.4/pgpubsub/management/commands/listen.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.3/pgpubsub/migrations/0001_initial.py` & `django_pgpubsub-1.0.4/pgpubsub/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.3/pgpubsub/models.py` & `django_pgpubsub-1.0.4/pgpubsub/models.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.3/pgpubsub/notify.py` & `django_pgpubsub-1.0.4/pgpubsub/notify.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.3/pgpubsub/tests/channels.py` & `django_pgpubsub-1.0.4/pgpubsub/tests/channels.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.3/pgpubsub/tests/listeners.py` & `django_pgpubsub-1.0.4/pgpubsub/tests/listeners.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.3/pgpubsub/tests/migrations/0001_initial.py` & `django_pgpubsub-1.0.4/pgpubsub/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.3/pgpubsub/tests/models.py` & `django_pgpubsub-1.0.4/pgpubsub/tests/models.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.3/pgpubsub/tests/test_core.py` & `django_pgpubsub-1.0.4/pgpubsub/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.3/pgpubsub/triggers.py` & `django_pgpubsub-1.0.4/pgpubsub/triggers.py`

 * *Files identical despite different names*

### Comparing `django_pgpubsub-1.0.3/pyproject.toml` & `django_pgpubsub-1.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 fail_under = 100
 
 [tool.poetry]
 name = "django-pgpubsub"
 packages = [
   { include = "pgpubsub" }
 ]
-version = "1.0.3"
+version = "1.0.4"
 description = "A distributed task processing framework for Django built on top of the Postgres NOTIFY/LISTEN protocol."
 authors = ["Opus 10 Engineering"]
 classifiers = [
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
```

### Comparing `django_pgpubsub-1.0.3/PKG-INFO` & `django_pgpubsub-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pgpubsub
-Version: 1.0.3
+Version: 1.0.4
 Summary: A distributed task processing framework for Django built on top of the Postgres NOTIFY/LISTEN protocol.
 Home-page: https://github.com/Opus10/django-pgpubsub
 License: BSD-3-Clause
 Author: Opus 10 Engineering
 Requires-Python: >=3.7.0,<4
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -52,16 +52,16 @@
 
 Highlights
 ==========
 
 - **Minimal Operational Infrastructure**: If you're already running a Django application
   on top of a Postgres database, the installation of this library is the sum total
   of the operational work required to implement a framework for a distributed
-  message processing framework. No additional servers or server configuration
-  is required.
+  message processing framework. No additional frameworks or technologies
+  are required.
 
 - **Integration with Postgres Triggers (via django-pgtrigger)**:
   To quote the [official](https://www.postgresql.org/docs/current/sql-notify.html)
   Postgres docs:
 
   *"When NOTIFY is used to signal the occurrence of changes to a particular table,
   a useful programming technique is to put the NOTIFY in a statement trigger that is triggered
@@ -112,15 +112,15 @@
   AMPQ queue.
 
 - If a message is sent using Postgres' ``NOTIFY`` and no process is listening at that time,
   the message is lost forever. As explained in the **Durability and Recovery** section above,
   pgpubsub can easily be configured so that we can replay "lost" messages, but this comes at the
   performance penalty of inserting a row into a table before sending each notification. This is the same
   penalty we must pay if we wish to have concurrent processes listening to the same channel without
-  duplicate notiifcation processing, as explained in the **Exactly-once notification processing** section above.
+  duplicate notifcation processing, as explained in the **Exactly-once notification processing** section above.
 
 
 Alternatives
 ============
 
 - [Celery](https://docs.celeryq.dev/en/stable/search.html?q=ampq): The canonical distributed message processing library for django based applications. This can handle large volumes of throughput and is well tested in production.
   It is however operationally quite heavy to maintain and set-up.
```


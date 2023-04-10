# Comparing `tmp/kustosz-22.8.0.tar.gz` & `tmp/kustosz-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kustosz-22.8.0.tar", max compression
+gzip compressed data, was "kustosz-23.4.0.tar", max compression
```

## Comparing `kustosz-22.8.0.tar` & `kustosz-23.4.0.tar`

### file list

```diff
@@ -1,71 +1,70 @@
--rw-r--r--   0        0        0    13829 2022-08-14 09:20:42.186907 kustosz-22.8.0/LICENSE
--rw-r--r--   0        0        0     2166 2022-08-14 09:20:42.186907 kustosz-22.8.0/README.md
--rw-r--r--   0        0        0       65 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/__init__.py
--rw-r--r--   0        0        0      305 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/admin.py
--rw-r--r--   0        0        0      149 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/apps.py
--rw-r--r--   0        0        0      390 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/asgi.py
--rw-r--r--   0        0        0      804 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/authentication.py
--rw-r--r--   0        0        0      618 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/celery.py
--rw-r--r--   0        0        0        0 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/cli/__init__.py
--rwxr-xr-x   0        0        0      663 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/cli/manage.py
--rw-r--r--   0        0        0      468 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/constants.py
--rw-r--r--   0        0        0     2383 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/enums.py
--rw-r--r--   0        0        0      376 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/exceptions.py
--rw-r--r--   0        0        0        0 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/fetchers/__init__.py
--rw-r--r--   0        0        0     7524 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/fetchers/feed.py
--rw-r--r--   0        0        0     4584 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/fetchers/url.py
--rw-r--r--   0        0        0     9052 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/filters.py
--rw-r--r--   0        0        0        0 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/forms/__init__.py
--rw-r--r--   0        0        0      181 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/forms/fields.py
--rw-r--r--   0        0        0        0 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/management/__init__.py
--rw-r--r--   0        0        0        0 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/management/commands/__init__.py
--rw-r--r--   0        0        0     2252 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/management/commands/add_entry.py
--rw-r--r--   0        0        0     1020 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/management/commands/export_channels.py
--rw-r--r--   0        0        0     1507 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/management/commands/fetch_new_content.py
--rw-r--r--   0        0        0     5143 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/management/commands/import_channels.py
--rw-r--r--   0        0        0    29539 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/managers.py
--rw-r--r--   0        0        0    18825 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/migrations/0001_initial.py
--rw-r--r--   0        0        0      570 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/migrations/0002_create_manual_channel_20210923_1906.py
--rw-r--r--   0        0        0     1055 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/migrations/0003_create_celery_beat_20220108_0935.py
--rw-r--r--   0        0        0     1821 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/migrations/0004_entry_mark_as_read_20220622_1219.py
--rw-r--r--   0        0        0        0 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/migrations/__init__.py
--rw-r--r--   0        0        0     9737 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/models.py
--rw-r--r--   0        0        0      231 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/renderers.py
--rw-r--r--   0        0        0    10299 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/serializers.py
--rw-r--r--   0        0        0      553 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/settings.py
--rw-r--r--   0        0        0      420 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/signals.py
--rw-r--r--   0        0        0     1060 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/tasks/__init__.py
--rw-r--r--   0        0        0      576 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/tasks/task_add_channels.py
--rw-r--r--   0        0        0      521 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/tasks/task_add_readability_contents.py
--rw-r--r--   0        0        0      696 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/tasks/task_autodetect_channel_content_from_url.py
--rw-r--r--   0        0        0      661 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/tasks/task_autodetect_channels_from_url.py
--rw-r--r--   0        0        0      752 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/tasks/task_autodetect_content_from_url.py
--rw-r--r--   0        0        0      686 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/tasks/task_autodetect_entry_content_from_url.py
--rw-r--r--   0        0        0      854 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/tasks/task_clean_feed_fetcher_cache.py
--rw-r--r--   0        0        0      351 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/tasks/task_clean_url_fetcher_cache.py
--rw-r--r--   0        0        0      456 2022-08-14 09:20:42.186907 kustosz-22.8.0/kustosz/tasks/task_deduplicate_entries.py
--rw-r--r--   0        0        0      459 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/tasks/task_fetch_channel_content.py
--rw-r--r--   0        0        0      958 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/tasks/task_fetch_feed_channel_content.py
--rw-r--r--   0        0        0      491 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/tasks/task_fetch_manual_entry_data.py
--rw-r--r--   0        0        0      531 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/tasks/task_fetch_manual_entry_metadata.py
--rw-r--r--   0        0        0      385 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/tasks/task_filter_action_run_script.py
--rw-r--r--   0        0        0      550 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/tasks/task_run_filters_on_entries.py
--rw-r--r--   0        0        0        0 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/third_party/__init__.py
--rw-r--r--   0        0        0       30 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/third_party/taggit_serializer/__init__.py
--rw-r--r--   0        0        0     3679 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/third_party/taggit_serializer/serializers.py
--rw-r--r--   0        0        0     6537 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/types.py
--rw-r--r--   0        0        0     2012 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/urls.py
--rw-r--r--   0        0        0     1492 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/utils/__init__.py
--rw-r--r--   0        0        0    14773 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/utils/autodetect_content.py
--rw-r--r--   0        0        0     2290 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/utils/duplicate_finder.py
--rw-r--r--   0        0        0     7806 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/utils/extract_metadata.py
--rw-r--r--   0        0        0     3908 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/utils/extract_readability.py
--rw-r--r--   0        0        0     1100 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/utils/filter_actions.py
--rw-r--r--   0        0        0     2602 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/utils/opml_exporter.py
--rw-r--r--   0        0        0     2011 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/utils/run_script.py
--rw-r--r--   0        0        0      768 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/validators.py
--rw-r--r--   0        0        0    11835 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/views.py
--rw-r--r--   0        0        0      390 2022-08-14 09:20:42.190907 kustosz-22.8.0/kustosz/wsgi.py
--rw-r--r--   0        0        0     2390 2022-08-14 09:20:42.190907 kustosz-22.8.0/pyproject.toml
--rw-r--r--   0        0        0     4401 2022-08-14 09:20:51.928542 kustosz-22.8.0/setup.py
--rw-r--r--   0        0        0     4740 2022-08-14 09:20:51.929079 kustosz-22.8.0/PKG-INFO
+-rw-r--r--   0        0        0    13829 2023-04-10 10:35:54.309193 kustosz-23.4.0/LICENSE
+-rw-r--r--   0        0        0     2190 2023-04-10 10:35:54.309193 kustosz-23.4.0/README.md
+-rw-r--r--   0        0        0       65 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/__init__.py
+-rw-r--r--   0        0        0      305 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/admin.py
+-rw-r--r--   0        0        0      149 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/apps.py
+-rw-r--r--   0        0        0      390 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/asgi.py
+-rw-r--r--   0        0        0      804 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/authentication.py
+-rw-r--r--   0        0        0      618 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/celery.py
+-rw-r--r--   0        0        0        0 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/cli/__init__.py
+-rwxr-xr-x   0        0        0      663 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/cli/manage.py
+-rw-r--r--   0        0        0      468 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/constants.py
+-rw-r--r--   0        0        0     2383 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/enums.py
+-rw-r--r--   0        0        0      376 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/fetchers/__init__.py
+-rw-r--r--   0        0        0     7532 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/fetchers/feed.py
+-rw-r--r--   0        0        0     4598 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/fetchers/url.py
+-rw-r--r--   0        0        0     9052 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/filters.py
+-rw-r--r--   0        0        0        0 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/forms/__init__.py
+-rw-r--r--   0        0        0      181 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/forms/fields.py
+-rw-r--r--   0        0        0        0 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/management/commands/__init__.py
+-rw-r--r--   0        0        0     2259 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/management/commands/add_entry.py
+-rw-r--r--   0        0        0     1020 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/management/commands/export_channels.py
+-rw-r--r--   0        0        0     1507 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/management/commands/fetch_new_content.py
+-rw-r--r--   0        0        0     5143 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/management/commands/import_channels.py
+-rw-r--r--   0        0        0    29531 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/managers.py
+-rw-r--r--   0        0        0    18825 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/migrations/0001_initial.py
+-rw-r--r--   0        0        0      570 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/migrations/0002_create_manual_channel_20210923_1906.py
+-rw-r--r--   0        0        0     1055 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/migrations/0003_create_celery_beat_20220108_0935.py
+-rw-r--r--   0        0        0     1821 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/migrations/0004_entry_mark_as_read_20220622_1219.py
+-rw-r--r--   0        0        0        0 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/migrations/__init__.py
+-rw-r--r--   0        0        0     9761 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/models.py
+-rw-r--r--   0        0        0      231 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/renderers.py
+-rw-r--r--   0        0        0    10306 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/serializers.py
+-rw-r--r--   0        0        0      553 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/settings.py
+-rw-r--r--   0        0        0      420 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/signals.py
+-rw-r--r--   0        0        0     1060 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/tasks/__init__.py
+-rw-r--r--   0        0        0      576 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/tasks/task_add_channels.py
+-rw-r--r--   0        0        0      521 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/tasks/task_add_readability_contents.py
+-rw-r--r--   0        0        0      696 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/tasks/task_autodetect_channel_content_from_url.py
+-rw-r--r--   0        0        0      661 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/tasks/task_autodetect_channels_from_url.py
+-rw-r--r--   0        0        0      752 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/tasks/task_autodetect_content_from_url.py
+-rw-r--r--   0        0        0      686 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/tasks/task_autodetect_entry_content_from_url.py
+-rw-r--r--   0        0        0      854 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/tasks/task_clean_feed_fetcher_cache.py
+-rw-r--r--   0        0        0      351 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/tasks/task_clean_url_fetcher_cache.py
+-rw-r--r--   0        0        0      456 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/tasks/task_deduplicate_entries.py
+-rw-r--r--   0        0        0      459 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/tasks/task_fetch_channel_content.py
+-rw-r--r--   0        0        0      958 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/tasks/task_fetch_feed_channel_content.py
+-rw-r--r--   0        0        0      491 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/tasks/task_fetch_manual_entry_data.py
+-rw-r--r--   0        0        0      531 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/tasks/task_fetch_manual_entry_metadata.py
+-rw-r--r--   0        0        0      385 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/tasks/task_filter_action_run_script.py
+-rw-r--r--   0        0        0      550 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/tasks/task_run_filters_on_entries.py
+-rw-r--r--   0        0        0        0 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/third_party/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/third_party/taggit_serializer/__init__.py
+-rw-r--r--   0        0        0     3679 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/third_party/taggit_serializer/serializers.py
+-rw-r--r--   0        0        0     6537 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/types.py
+-rw-r--r--   0        0        0     2012 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/urls.py
+-rw-r--r--   0        0        0     1492 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/utils/__init__.py
+-rw-r--r--   0        0        0    14773 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/utils/autodetect_content.py
+-rw-r--r--   0        0        0     2290 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/utils/duplicate_finder.py
+-rw-r--r--   0        0        0     7806 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/utils/extract_metadata.py
+-rw-r--r--   0        0        0     3908 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/utils/extract_readability.py
+-rw-r--r--   0        0        0     1100 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/utils/filter_actions.py
+-rw-r--r--   0        0        0     2602 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/utils/opml_exporter.py
+-rw-r--r--   0        0        0     2011 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/utils/run_script.py
+-rw-r--r--   0        0        0      768 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/validators.py
+-rw-r--r--   0        0        0    11842 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/views.py
+-rw-r--r--   0        0        0      390 2023-04-10 10:35:54.309193 kustosz-23.4.0/kustosz/wsgi.py
+-rw-r--r--   0        0        0     2391 2023-04-10 10:35:54.313193 kustosz-23.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4810 1970-01-01 00:00:00.000000 kustosz-23.4.0/PKG-INFO
```

### Comparing `kustosz-22.8.0/LICENSE` & `kustosz-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/README.md` & `kustosz-23.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![Kustosz](./kustosz_logo.svg)](https://www.kustosz.org)
 
-![GitHub](https://img.shields.io/github/license/KustoszApp/server?color=green) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kustosz?color=green) ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/KustoszApp/server/CI?label=CI) ![GitHub issues](https://img.shields.io/github/issues/KustoszApp/server?color=green) ![GitHub pull requests](https://img.shields.io/github/issues-pr/KustoszApp/server) ![GitHub Repo stars](https://img.shields.io/github/stars/KustoszApp/server?color=green) ![GitHub Release Date](https://img.shields.io/github/release-date/KustoszApp/server) ![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/KustoszApp/server/latest?color=green) ![GitHub last commit](https://img.shields.io/github/last-commit/KustoszApp/server)
+![GitHub](https://img.shields.io/github/license/KustoszApp/server?color=green) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kustosz?color=green) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/KustoszApp/server/ci.yml?branch=main&label=CI) ![GitHub issues](https://img.shields.io/github/issues/KustoszApp/server?color=green) ![GitHub pull requests](https://img.shields.io/github/issues-pr/KustoszApp/server) ![GitHub Repo stars](https://img.shields.io/github/stars/KustoszApp/server?color=green) ![GitHub Release Date](https://img.shields.io/github/release-date/KustoszApp/server) ![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/KustoszApp/server/latest?color=green) ![GitHub last commit](https://img.shields.io/github/last-commit/KustoszApp/server)
 
 # Kustosz - backend server repository
 
 Focus on the worthwhile content with Kustosz, open source self-hosted web application.
 
 This repository contains backend server.
```

### Comparing `kustosz-22.8.0/kustosz/authentication.py` & `kustosz-23.4.0/kustosz/authentication.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/celery.py` & `kustosz-23.4.0/kustosz/celery.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/cli/manage.py` & `kustosz-23.4.0/kustosz/cli/manage.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/enums.py` & `kustosz-23.4.0/kustosz/enums.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/fetchers/feed.py` & `kustosz-23.4.0/kustosz/fetchers/feed.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         if not ua:
             return None
 
         request.headers["User-Agent"] = ua
 
         return request
 
-    reader._parser.session_hooks.response.append(aggressive_ua_fallback_hook)
+    reader._parser.session_factory.response_hooks.append(aggressive_ua_fallback_hook)
 
 
 class FeedFetcherPurpose(enum.Enum):
     MAIN = enum.auto()
     FEED_DISCOVERY = enum.auto()
```

### Comparing `kustosz-22.8.0/kustosz/fetchers/url.py` & `kustosz-23.4.0/kustosz/fetchers/url.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,24 +92,24 @@
             requests_exceptions.Timeout,
             requests_exceptions.HTTPError,
             requests_exceptions.ConnectionError,
             requests_exceptions.TooManyRedirects,
             requests_exceptions.ChunkedEncodingError,
         ) as e:
             log.debug("url %s raised %s:", url, e.__class__.__name__, exc_info=True)
-            raise TransientFetcherError().with_traceback(e.__traceback__)
+            raise TransientFetcherError().with_traceback(e.__traceback__) from e
         except (
             requests_exceptions.MissingSchema,
             requests_exceptions.InvalidURL,
             requests_exceptions.InvalidHeader,
             requests_exceptions.InvalidProxyURL,
             requests_exceptions.ContentDecodingError,
         ) as e:
             log.debug("url %s raised %s:", url, e.__class__.__name__, exc_info=True)
-            raise PermanentFetcherError().with_traceback(e.__traceback__)
+            raise PermanentFetcherError().with_traceback(e.__traceback__) from e
 
         log.debug("url %s returned HTTP code %s", url, response.status_code)
 
         if not response.ok:
             msg = f"Error code {response.status_code}"
             if 400 <= response.status_code <= 499:
                 raise PermanentFetcherError(msg)
```

### Comparing `kustosz-22.8.0/kustosz/filters.py` & `kustosz-23.4.0/kustosz/filters.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/management/commands/add_entry.py` & `kustosz-23.4.0/kustosz/management/commands/add_entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,10 +53,10 @@
                 description = ", ".join([str(error) for error in errors])
                 msg.append(f" --{flag}: {description}")
             raise CommandError("\n".join(msg))
 
         try:
             Entry.objects.add_entry_from_manual_channel(serializer.validated_data)
         except InvalidDataException as e:
-            raise CommandError("\n".join(e.messages))
+            raise CommandError("\n".join(e.messages)) from e
 
         self.stdout.write(self.style.SUCCESS("DONE"))
```

### Comparing `kustosz-22.8.0/kustosz/management/commands/export_channels.py` & `kustosz-23.4.0/kustosz/management/commands/export_channels.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/management/commands/fetch_new_content.py` & `kustosz-23.4.0/kustosz/management/commands/fetch_new_content.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/management/commands/import_channels.py` & `kustosz-23.4.0/kustosz/management/commands/import_channels.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/managers.py` & `kustosz-23.4.0/kustosz/managers.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,15 +378,15 @@
             updated_time=django_now(),
             published_time_upstream=optional_make_aware(entry_data.published_time),
             updated_time_upstream=optional_make_aware(entry_data.updated_time),
         )
         try:
             entry.full_clean()
         except ValidationError as e:
-            raise InvalidDataException(e)
+            raise InvalidDataException(e) from e
         entry_exists = self.get_queryset().filter(
             channel=entry.channel_id, link__in=(entry.gid, entry.link)
         )
         if entry_exists.count():
             msg = "Entry with this Channel and Link already exists."
             raise InvalidDataException(msg)
         entry.save()
@@ -646,15 +646,15 @@
                     ),
                     channel_model.pk,
                     entry.gid,
                     e,
                     channel_model.url,
                 )
                 continue
-            EntryContent = entry.content_set.get_queryset().model
+            EntryContent = entry.content_set.model
             entry_contents = []
             for fetched_content in entry_data.content:
                 reading_time = estimate_reading_time(fetched_content.content)
                 content_obj = EntryContent(
                     updated_time=django_now(),
                     estimated_reading_time=reading_time,
                     **{
```

### Comparing `kustosz-22.8.0/kustosz/migrations/0001_initial.py` & `kustosz-23.4.0/kustosz/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/migrations/0002_create_manual_channel_20210923_1906.py` & `kustosz-23.4.0/kustosz/migrations/0002_create_manual_channel_20210923_1906.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/migrations/0003_create_celery_beat_20220108_0935.py` & `kustosz-23.4.0/kustosz/migrations/0003_create_celery_beat_20220108_0935.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/migrations/0004_entry_mark_as_read_20220622_1219.py` & `kustosz-23.4.0/kustosz/migrations/0004_entry_mark_as_read_20220622_1219.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/models.py` & `kustosz-23.4.0/kustosz/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,20 +199,20 @@
                 fields=["channel", "gid"], name="unique_channel_gid"
             )
         ]
 
     def set_new_preferred_content(self, new_preferred_content):
         try:
             found_content = self.content_set.get(pk=new_preferred_content.id)
-        except ObjectDoesNotExist:
+        except ObjectDoesNotExist as e:
             msg = "Could not find content matching provided criteria"
-            raise InvalidDataException(msg)
-        except MultipleObjectsReturned:
+            raise InvalidDataException(msg) from e
+        except MultipleObjectsReturned as e:
             msg = "Multiple content objects match provided criteria"
-            raise InvalidDataException(msg)
+            raise InvalidDataException(msg) from e
         self.selected_preferred_content = found_content
 
     @property
     def _published_time(self):
         if self.published_time_upstream:
             return self.published_time_upstream
         if self.updated_time_upstream:
```

### Comparing `kustosz-22.8.0/kustosz/serializers.py` & `kustosz-23.4.0/kustosz/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
     def update(self, instance, validated_data):
         new_preferred_content = validated_data.pop("preferred_content", None)
         if new_preferred_content:
             try:
                 instance.set_new_preferred_content(new_preferred_content)
             except InvalidDataException as e:
-                raise exceptions.ValidationError(e.message)
+                raise exceptions.ValidationError(e.message) from e
         instance.updated_time = django_now()
         return super().update(instance, validated_data)
 
 
 class EntriesArchiveSerializer(serializers.Serializer):
     archived_entries = serializers.ListField(
         child=serializers.IntegerField(), required=True
```

### Comparing `kustosz-22.8.0/kustosz/settings.py` & `kustosz-23.4.0/kustosz/settings.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/tasks/__init__.py` & `kustosz-23.4.0/kustosz/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/tasks/task_add_channels.py` & `kustosz-23.4.0/kustosz/tasks/task_add_channels.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/tasks/task_add_readability_contents.py` & `kustosz-23.4.0/kustosz/tasks/task_add_readability_contents.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/tasks/task_autodetect_channel_content_from_url.py` & `kustosz-23.4.0/kustosz/tasks/task_autodetect_channel_content_from_url.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/tasks/task_autodetect_channels_from_url.py` & `kustosz-23.4.0/kustosz/tasks/task_autodetect_channels_from_url.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/tasks/task_autodetect_content_from_url.py` & `kustosz-23.4.0/kustosz/tasks/task_autodetect_content_from_url.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/tasks/task_autodetect_entry_content_from_url.py` & `kustosz-23.4.0/kustosz/tasks/task_autodetect_entry_content_from_url.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/tasks/task_clean_feed_fetcher_cache.py` & `kustosz-23.4.0/kustosz/tasks/task_clean_feed_fetcher_cache.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/tasks/task_fetch_feed_channel_content.py` & `kustosz-23.4.0/kustosz/tasks/task_fetch_feed_channel_content.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/tasks/task_fetch_manual_entry_metadata.py` & `kustosz-23.4.0/kustosz/tasks/task_fetch_manual_entry_metadata.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/tasks/task_run_filters_on_entries.py` & `kustosz-23.4.0/kustosz/tasks/task_run_filters_on_entries.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/third_party/taggit_serializer/serializers.py` & `kustosz-23.4.0/kustosz/third_party/taggit_serializer/serializers.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/types.py` & `kustosz-23.4.0/kustosz/types.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/urls.py` & `kustosz-23.4.0/kustosz/urls.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/utils/__init__.py` & `kustosz-23.4.0/kustosz/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/utils/autodetect_content.py` & `kustosz-23.4.0/kustosz/utils/autodetect_content.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/utils/duplicate_finder.py` & `kustosz-23.4.0/kustosz/utils/duplicate_finder.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/utils/extract_metadata.py` & `kustosz-23.4.0/kustosz/utils/extract_metadata.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/utils/extract_readability.py` & `kustosz-23.4.0/kustosz/utils/extract_readability.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/utils/filter_actions.py` & `kustosz-23.4.0/kustosz/utils/filter_actions.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/utils/opml_exporter.py` & `kustosz-23.4.0/kustosz/utils/opml_exporter.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/utils/run_script.py` & `kustosz-23.4.0/kustosz/utils/run_script.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/validators.py` & `kustosz-23.4.0/kustosz/validators.py`

 * *Files identical despite different names*

### Comparing `kustosz-22.8.0/kustosz/views.py` & `kustosz-23.4.0/kustosz/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         serializer = serializers.EntryManualAddSerializer(data=request.data)
         serializer.is_valid(raise_exception=True)
         try:
             new_entry = models.Entry.objects.add_entry_from_manual_channel(
                 serializer.validated_data
             )
         except InvalidDataException as e:
-            raise ValidationError(e.messages)
+            raise ValidationError(e.messages) from e
         setattr(new_entry, "published_time", new_entry._published_time)
         serializer = self.get_serializer(new_entry)
         serializer.data
         headers = self.get_success_headers(serializer.data)
         return Response(
             serializer.data, status=status.HTTP_201_CREATED, headers=headers
         )
```

### Comparing `kustosz-22.8.0/pyproject.toml` & `kustosz-23.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kustosz"
-version = "22.08.0"
+version = "23.04.0"
 description = "Focus on the worthwhile content with Kustosz, open source self-hosted web application. This package contains backend server."
 license = "EUPL-1.2"
 authors = ["Mirek Długosz <mirek@mirekdlugosz.com>"]
 readme = "README.md"
 homepage = "https://www.kustosz.org/"
 repository = "https://github.com/KustoszApp/server/"
 documentation = "https://docs.kustosz.org/"
@@ -16,53 +16,58 @@
     "Intended Audience :: Science/Research",
     "Operating System :: POSIX :: Linux",
     "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-celery = "^5.2.6"
-dacite = "^1.6.0"
-Django = "^3.2.15"
-django-celery-beat = "^2.2.1"
-django-celery-results = "^2.3.1"
-django-cors-headers = "^3.12.0"
-django-extensions = "^3.2.0"
-django-filter = "^22.1"
-django-taggit = "^3.0.0"
+celery = "^5.2.7"
+dacite = "^1.8.0"
+Django = "^4.2"
+django-celery-beat = "^2.5.0"
+django-celery-results = "^2.5.0"
+django-cors-headers = "^3.14.0"
+django-extensions = "^3.2.1"
+django-filter = "^23.1"
+django-taggit = "^3.1.0"
 django-taggit-serializer = "^0.1.7"
-djangorestframework = "^3.13.1"
-dynaconf = { version = "^3.1.8", extras = ["yaml"] }
+djangorestframework = "^3.14.0"
+dynaconf = "^3.1.12"
 hyperlink = "^21.0.0"
 listparser = "^0.19"
 python-dateutil = "^2.8.2"
 readability-lxml = "^0.8.1"
-reader = "^2.17"
-requests-cache = "^0.9.4"
+reader = "^3.5"
+requests-cache = "^1.0.1"
 Unalix = "^0.9"
-dj-database-url = { version = "^0.5.0", optional = true }
+dj-database-url = { version = "^1.3.0", optional = true }
 gunicorn = { version = "^20.1.0", optional = true }
 supervisor = { version = "^4.2.4", optional = true }
-psycopg2 = { version = "^2.9.3", optional = true }
-psycopg2-binary = { version = "^2.9.3", optional = true }
-redis = { version = "^4.2.2", optional = true }
-whitenoise = { version = "^6.0.0", optional = true }
-
-[tool.poetry.dev-dependencies]
-# FIXME: make it two separate groups in poetry 1.2+
-# test dependencies
+psycopg2 = { version = "^2.9.6", optional = true }
+psycopg2-binary = { version = "^2.9.6", optional = true }
+redis = { version = "^4.5.4", optional = true }
+whitenoise = { version = "^6.4.0", optional = true }
+
+[tool.poetry.group.test]
+optional = true
+
+[tool.poetry.group.test.dependencies]
 dominate = "~2"
 factory-boy = "~3"
-Faker = "~13"
+Faker = "~18"
 freezegun = "~1"
 pytest = "~7"
 pytest-django = "~4"
 pytest-mock = "~3"
 pytest-factoryboy = "~2"
-# dev dependencies
+
+[tool.poetry.group.dev]
+optional = true
+
+[tool.poetry.group.dev.dependencies]
 black = "*"
 flake8 = "*"
 ipdb = "*"
 ipython = "*"
 pre-commit = "*"
 nox = "*"
```

### Comparing `kustosz-22.8.0/PKG-INFO` & `kustosz-23.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 Metadata-Version: 2.1
 Name: kustosz
-Version: 22.8.0
+Version: 23.4.0
 Summary: Focus on the worthwhile content with Kustosz, open source self-hosted web application. This package contains backend server.
 Home-page: https://www.kustosz.org/
 License: EUPL-1.2
 Author: Mirek Długosz
 Author-email: mirek@mirekdlugosz.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Provides-Extra: container
 Provides-Extra: heroku
 Provides-Extra: installer
-Requires-Dist: Django (>=3.2.15,<4.0.0)
+Requires-Dist: Django (>=4.2,<5.0)
 Requires-Dist: Unalix (>=0.9,<0.10)
-Requires-Dist: celery (>=5.2.6,<6.0.0)
-Requires-Dist: dacite (>=1.6.0,<2.0.0)
-Requires-Dist: dj-database-url (>=0.5.0,<0.6.0); extra == "heroku"
-Requires-Dist: django-celery-beat (>=2.2.1,<3.0.0)
-Requires-Dist: django-celery-results (>=2.3.1,<3.0.0)
-Requires-Dist: django-cors-headers (>=3.12.0,<4.0.0)
-Requires-Dist: django-extensions (>=3.2.0,<4.0.0)
-Requires-Dist: django-filter (>=22.1,<23.0)
-Requires-Dist: django-taggit (>=3.0.0,<4.0.0)
+Requires-Dist: celery (>=5.2.7,<6.0.0)
+Requires-Dist: dacite (>=1.8.0,<2.0.0)
+Requires-Dist: dj-database-url (>=1.3.0,<2.0.0) ; extra == "heroku"
+Requires-Dist: django-celery-beat (>=2.5.0,<3.0.0)
+Requires-Dist: django-celery-results (>=2.5.0,<3.0.0)
+Requires-Dist: django-cors-headers (>=3.14.0,<4.0.0)
+Requires-Dist: django-extensions (>=3.2.1,<4.0.0)
+Requires-Dist: django-filter (>=23.1,<24.0)
+Requires-Dist: django-taggit (>=3.1.0,<4.0.0)
 Requires-Dist: django-taggit-serializer (>=0.1.7,<0.2.0)
-Requires-Dist: djangorestframework (>=3.13.1,<4.0.0)
-Requires-Dist: dynaconf[yaml] (>=3.1.8,<4.0.0)
-Requires-Dist: gunicorn (>=20.1.0,<21.0.0); extra == "container" or extra == "installer" or extra == "heroku"
+Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
+Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
+Requires-Dist: gunicorn (>=20.1.0,<21.0.0) ; extra == "container" or extra == "installer" or extra == "heroku"
 Requires-Dist: hyperlink (>=21.0.0,<22.0.0)
 Requires-Dist: listparser (>=0.19,<0.20)
-Requires-Dist: psycopg2 (>=2.9.3,<3.0.0); extra == "container"
-Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0); extra == "heroku"
+Requires-Dist: psycopg2 (>=2.9.6,<3.0.0) ; extra == "container"
+Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0) ; extra == "heroku"
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: readability-lxml (>=0.8.1,<0.9.0)
-Requires-Dist: reader (>=2.17,<3.0)
-Requires-Dist: redis (>=4.2.2,<5.0.0); extra == "container" or extra == "installer" or extra == "heroku"
-Requires-Dist: requests-cache (>=0.9.4,<0.10.0)
-Requires-Dist: supervisor (>=4.2.4,<5.0.0); extra == "heroku"
-Requires-Dist: whitenoise (>=6.0.0,<7.0.0); extra == "container" or extra == "heroku"
+Requires-Dist: reader (>=3.5,<4.0)
+Requires-Dist: redis (>=4.5.4,<5.0.0) ; extra == "container" or extra == "installer" or extra == "heroku"
+Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
+Requires-Dist: supervisor (>=4.2.4,<5.0.0) ; extra == "heroku"
+Requires-Dist: whitenoise (>=6.4.0,<7.0.0) ; extra == "container" or extra == "heroku"
 Project-URL: Documentation, https://docs.kustosz.org/
 Project-URL: Repository, https://github.com/KustoszApp/server/
 Description-Content-Type: text/markdown
 
 [![Kustosz](./kustosz_logo.svg)](https://www.kustosz.org)
 
-![GitHub](https://img.shields.io/github/license/KustoszApp/server?color=green) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kustosz?color=green) ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/KustoszApp/server/CI?label=CI) ![GitHub issues](https://img.shields.io/github/issues/KustoszApp/server?color=green) ![GitHub pull requests](https://img.shields.io/github/issues-pr/KustoszApp/server) ![GitHub Repo stars](https://img.shields.io/github/stars/KustoszApp/server?color=green) ![GitHub Release Date](https://img.shields.io/github/release-date/KustoszApp/server) ![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/KustoszApp/server/latest?color=green) ![GitHub last commit](https://img.shields.io/github/last-commit/KustoszApp/server)
+![GitHub](https://img.shields.io/github/license/KustoszApp/server?color=green) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kustosz?color=green) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/KustoszApp/server/ci.yml?branch=main&label=CI) ![GitHub issues](https://img.shields.io/github/issues/KustoszApp/server?color=green) ![GitHub pull requests](https://img.shields.io/github/issues-pr/KustoszApp/server) ![GitHub Repo stars](https://img.shields.io/github/stars/KustoszApp/server?color=green) ![GitHub Release Date](https://img.shields.io/github/release-date/KustoszApp/server) ![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/KustoszApp/server/latest?color=green) ![GitHub last commit](https://img.shields.io/github/last-commit/KustoszApp/server)
 
 # Kustosz - backend server repository
 
 Focus on the worthwhile content with Kustosz, open source self-hosted web application.
 
 This repository contains backend server.
```


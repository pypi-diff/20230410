# Comparing `tmp/statefun-tasks-0.9.90.tar.gz` & `tmp/statefun-tasks-0.9.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statefun-tasks-0.9.90.tar", last modified: Fri Mar  3 19:15:53 2023, max compression
+gzip compressed data, was "statefun-tasks-0.9.91.tar", last modified: Mon Apr 10 17:02:11 2023, max compression
```

## Comparing `statefun-tasks-0.9.90.tar` & `statefun-tasks-0.9.91.tar`

### file list

```diff
@@ -1,63 +1,67 @@
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-03-03 19:15:53.661112 statefun-tasks-0.9.90/
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)    11357 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/LICENSE
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)     1330 2023-03-03 19:15:53.661112 statefun-tasks-0.9.90/PKG-INFO
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)      813 2022-11-27 19:05:43.000000 statefun-tasks-0.9.90/README.md
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)       38 2023-03-03 19:15:53.661112 statefun-tasks-0.9.90/setup.cfg
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      944 2023-03-03 19:15:45.000000 statefun-tasks-0.9.90/setup.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-03-03 19:15:53.551113 statefun-tasks-0.9.90/statefun_tasks/
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)      924 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/__init__.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      585 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/builtin.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1004 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/builtin_tasks.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-03-03 19:15:53.571113 statefun-tasks-0.9.90/statefun_tasks/client/
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)      151 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/client/__init__.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)    17395 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/client/tasks_client.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)      864 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/client/types.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)    10552 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/context.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-03-03 19:15:53.571113 statefun-tasks-0.9.90/statefun_tasks/events/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)       43 2022-11-27 19:05:41.000000 statefun-tasks-0.9.90/statefun_tasks/events/__init__.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6622 2022-11-27 19:05:41.000000 statefun-tasks-0.9.90/statefun_tasks/events/event_handlers.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-03-03 19:15:53.581113 statefun-tasks-0.9.90/statefun_tasks/extensions/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/extensions/__init__.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-03-03 19:15:53.581113 statefun-tasks-0.9.90/statefun_tasks/extensions/inline_tasks/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)       65 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/extensions/inline_tasks/__init__.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     5248 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/extensions/inline_tasks/inline_tasks_impl.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)   114816 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/messages_pb2.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     9212 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/pipeline.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    17896 2023-03-03 19:15:45.000000 statefun-tasks-0.9.90/statefun_tasks/pipeline_builder.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-03-03 19:15:53.581113 statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:41.000000 statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/__init__.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-03-03 19:15:53.601112 statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/handlers/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      298 2022-11-27 19:05:41.000000 statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/handlers/__init__.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6795 2022-11-27 19:05:41.000000 statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/handlers/begin_pipeline_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1926 2022-11-27 19:05:41.000000 statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/handlers/cancel_pipeline_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6768 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/handlers/continue_pipeline_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     2969 2022-11-27 19:05:41.000000 statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/handlers/end_pipeline_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1658 2022-11-27 19:05:41.000000 statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/handlers/pipeline_message_handler.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-03-03 19:15:53.621112 statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/helpers/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      186 2022-11-27 19:05:41.000000 statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/helpers/__init__.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    11000 2023-03-03 19:15:45.000000 statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/helpers/pipeline_graph.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6410 2022-11-27 19:05:41.000000 statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/helpers/result_aggregator.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1995 2022-11-27 19:05:41.000000 statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/helpers/result_emitter.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    12023 2022-11-29 16:51:28.000000 statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/helpers/task_submitter.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     7003 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/protobuf.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     9345 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/serialisation.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)    16385 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/task_builder.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-03-03 19:15:53.631112 statefun-tasks-0.9.90/statefun_tasks/task_impl/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:41.000000 statefun-tasks-0.9.90/statefun_tasks/task_impl/__init__.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-03-03 19:15:53.651112 statefun-tasks-0.9.90/statefun_tasks/task_impl/handlers/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      265 2022-11-27 19:05:41.000000 statefun-tasks-0.9.90/statefun_tasks/task_impl/handlers/__init__.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      858 2022-11-27 19:05:41.000000 statefun-tasks-0.9.90/statefun_tasks/task_impl/handlers/child_pipeline_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      537 2022-11-27 19:05:41.000000 statefun-tasks-0.9.90/statefun_tasks/task_impl/handlers/message_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     3983 2022-11-27 19:05:41.000000 statefun-tasks-0.9.90/statefun_tasks/task_impl/handlers/task_action_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     4382 2022-11-27 19:05:41.000000 statefun-tasks-0.9.90/statefun_tasks/task_impl/handlers/task_request_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1134 2022-11-27 19:05:41.000000 statefun-tasks-0.9.90/statefun_tasks/task_impl/handlers/task_response_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     7277 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/tasks.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     2483 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/type_helpers.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)    11331 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/types.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     1793 2022-11-27 19:05:40.000000 statefun-tasks-0.9.90/statefun_tasks/utils.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-03-03 19:15:53.561113 statefun-tasks-0.9.90/statefun_tasks.egg-info/
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     1330 2023-03-03 19:15:53.000000 statefun-tasks-0.9.90/statefun_tasks.egg-info/PKG-INFO
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     1995 2023-03-03 19:15:53.000000 statefun-tasks-0.9.90/statefun_tasks.egg-info/SOURCES.txt
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)        1 2023-03-03 19:15:53.000000 statefun-tasks-0.9.90/statefun_tasks.egg-info/dependency_links.txt
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)       42 2023-03-03 19:15:53.000000 statefun-tasks-0.9.90/statefun_tasks.egg-info/requires.txt
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)       15 2023-03-03 19:15:53.000000 statefun-tasks-0.9.90/statefun_tasks.egg-info/top_level.txt
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:11.090440 statefun-tasks-0.9.91/
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)    11357 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/LICENSE
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)     1386 2023-04-10 17:02:11.086439 statefun-tasks-0.9.91/PKG-INFO
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      869 2023-04-10 17:01:43.000000 statefun-tasks-0.9.91/README.md
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)       38 2023-04-10 17:02:11.090440 statefun-tasks-0.9.91/setup.cfg
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      944 2023-04-10 17:01:43.000000 statefun-tasks-0.9.91/setup.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:10.738443 statefun-tasks-0.9.91/statefun_tasks/
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)      924 2023-04-10 16:51:35.000000 statefun-tasks-0.9.91/statefun_tasks/__init__.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      585 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/builtin.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1004 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/builtin_tasks.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:10.798442 statefun-tasks-0.9.91/statefun_tasks/client/
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)      151 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/client/__init__.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)    17395 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/client/tasks_client.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)      864 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/client/types.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)    10552 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/context.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:10.822442 statefun-tasks-0.9.91/statefun_tasks/effects/
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)       84 2023-04-10 17:01:43.000000 statefun-tasks-0.9.91/statefun_tasks/effects/__init__.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)      339 2023-04-10 17:01:43.000000 statefun-tasks-0.9.91/statefun_tasks/effects/effect.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)      370 2023-04-10 17:01:43.000000 statefun-tasks-0.9.91/statefun_tasks/effects/pause_pipeline_effect.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:10.838442 statefun-tasks-0.9.91/statefun_tasks/events/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)       43 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/events/__init__.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6622 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/events/event_handlers.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:10.846442 statefun-tasks-0.9.91/statefun_tasks/extensions/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/extensions/__init__.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:10.866442 statefun-tasks-0.9.91/statefun_tasks/extensions/inline_tasks/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)       65 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/extensions/inline_tasks/__init__.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     5248 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/extensions/inline_tasks/inline_tasks_impl.py
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)   115734 2023-04-10 17:01:43.000000 statefun-tasks-0.9.91/statefun_tasks/messages_pb2.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)     9212 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    17896 2023-03-03 19:15:45.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_builder.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:10.878441 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/__init__.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:10.942441 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      298 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/__init__.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6795 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/begin_pipeline_handler.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1926 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/cancel_pipeline_handler.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     6799 2023-04-10 17:01:43.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/continue_pipeline_handler.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     2969 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/end_pipeline_handler.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1658 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/pipeline_message_handler.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:11.006440 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      186 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/__init__.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    11000 2023-03-03 19:15:45.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/pipeline_graph.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6410 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/result_aggregator.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1995 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/result_emitter.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    12023 2022-11-29 16:51:28.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/task_submitter.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)     7003 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/protobuf.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)     9345 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/serialisation.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)    16385 2023-04-10 12:06:04.000000 statefun-tasks-0.9.91/statefun_tasks/task_builder.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:11.022440 statefun-tasks-0.9.91/statefun_tasks/task_impl/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/task_impl/__init__.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:11.082440 statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      265 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/__init__.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      858 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/child_pipeline_handler.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      537 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/message_handler.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     3983 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/task_action_handler.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     4382 2023-04-10 17:01:43.000000 statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/task_request_handler.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1134 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/task_response_handler.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     7655 2023-04-10 17:01:43.000000 statefun-tasks-0.9.91/statefun_tasks/tasks.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     2483 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/type_helpers.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)    11331 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/types.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)     1793 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/utils.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:10.770442 statefun-tasks-0.9.91/statefun_tasks.egg-info/
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)     1386 2023-04-10 17:02:10.000000 statefun-tasks-0.9.91/statefun_tasks.egg-info/PKG-INFO
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)     2111 2023-04-10 17:02:10.000000 statefun-tasks-0.9.91/statefun_tasks.egg-info/SOURCES.txt
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)        1 2023-04-10 17:02:10.000000 statefun-tasks-0.9.91/statefun_tasks.egg-info/dependency_links.txt
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)       42 2023-04-10 17:02:10.000000 statefun-tasks-0.9.91/statefun_tasks.egg-info/requires.txt
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)       15 2023-04-10 17:02:10.000000 statefun-tasks-0.9.91/statefun_tasks.egg-info/top_level.txt
```

### Comparing `statefun-tasks-0.9.90/LICENSE` & `statefun-tasks-0.9.91/LICENSE`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/PKG-INFO` & `statefun-tasks-0.9.91/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statefun-tasks
-Version: 0.9.90
+Version: 0.9.91
 Summary: Tasks API for Stateful Functions on Flink
 Home-page: https://fransking.github.io/flink-statefun-tasks
 Author: Frans King & Luke Ashworth
 Author-email: frans.king@sbbsystems.com
 License: https://www.apache.org/licenses/LICENSE-2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
@@ -33,11 +33,12 @@
 
 
 @tasks.bind()
 def say_goodbye(greeting):
     return f'{greeting}.  So now I will say goodbye'
 ```
 
+Try the [demo](https://flink-demo-az.sbbsystems.co.uk).
 
 Additional documentation can be found [here](https://fransking.github.io/flink-statefun-tasks).
```

### Comparing `statefun-tasks-0.9.90/README.md` & `statefun-tasks-0.9.91/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -18,9 +18,10 @@
 
 
 @tasks.bind()
 def say_goodbye(greeting):
     return f'{greeting}.  So now I will say goodbye'
 ```
 
+Try the [demo](https://flink-demo-az.sbbsystems.co.uk).
 
 Additional documentation can be found [here](https://fransking.github.io/flink-statefun-tasks).
```

### Comparing `statefun-tasks-0.9.90/setup.py` & `statefun-tasks-0.9.91/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 install_requires = [
     'apache-flink-statefun>=3.2.0',
     'kafka-python'
 ]
 
 setuptools.setup(
     name="statefun-tasks",
-    version="0.9.90",
+    version="0.9.91",
     author="Frans King & Luke Ashworth",
     author_email="frans.king@sbbsystems.com",
     description="Tasks API for Stateful Functions on Flink",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://fransking.github.io/flink-statefun-tasks",
     packages=['statefun_tasks'] + [f'statefun_tasks.{package}' for package in setuptools.find_packages('statefun_tasks')],
```

### Comparing `statefun-tasks-0.9.90/statefun_tasks/__init__.py` & `statefun-tasks-0.9.91/statefun_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/builtin.py` & `statefun-tasks-0.9.91/statefun_tasks/builtin.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/builtin_tasks.py` & `statefun-tasks-0.9.91/statefun_tasks/builtin_tasks.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/client/tasks_client.py` & `statefun-tasks-0.9.91/statefun_tasks/client/tasks_client.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/client/types.py` & `statefun-tasks-0.9.91/statefun_tasks/client/types.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/context.py` & `statefun-tasks-0.9.91/statefun_tasks/context.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/events/event_handlers.py` & `statefun-tasks-0.9.91/statefun_tasks/events/event_handlers.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/extensions/inline_tasks/inline_tasks_impl.py` & `statefun-tasks-0.9.91/statefun_tasks/extensions/inline_tasks/inline_tasks_impl.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/messages_pb2.py` & `statefun-tasks-0.9.91/statefun_tasks/messages_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='messages.proto',
   package='statefun_tasks',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x0emessages.proto\x12\x0estatefun_tasks\x1a\x19google/protobuf/any.proto\"\x0b\n\tNoneValue\"6\n\x07\x41\x64\x64ress\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\"\x92\x01\n\x10MapOfStringToAny\x12:\n\x05items\x18\x01 \x03(\x0b\x32+.statefun_tasks.MapOfStringToAny.ItemsEntry\x1a\x42\n\nItemsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.Any:\x02\x38\x01\"1\n\nArrayOfAny\x12#\n\x05items\x18\x01 \x03(\x0b\x32\x14.google.protobuf.Any\"1\n\nTupleOfAny\x12#\n\x05items\x18\x01 \x03(\x0b\x32\x14.google.protobuf.Any\"\xd4\x02\n\tTaskEntry\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x11\n\ttask_type\x18\x02 \x01(\t\x12%\n\x07request\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x10\n\x08\x63omplete\x18\x04 \x01(\x08\x12\x12\n\nis_finally\x18\x05 \x01(\x08\x12\x11\n\tnamespace\x18\x06 \x01(\t\x12\x13\n\x0bworker_name\x18\x07 \x01(\t\x12\x13\n\x0bis_fruitful\x18\x08 \x01(\x08\x12\x35\n\x0cretry_policy\x18\t \x01(\x0b\x32\x1f.statefun_tasks.TaskRetryPolicy\x12\x19\n\x0c\x64isplay_name\x18\n \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x07is_wait\x18\x0b \x01(\x08\x12\x0b\n\x03uid\x18\x0c \x01(\t\x12\x18\n\x10is_exceptionally\x18\r \x01(\x08\x42\x0f\n\r_display_name\"\x8c\x01\n\nGroupEntry\x12\x10\n\x08group_id\x18\x01 \x01(\t\x12\'\n\x05group\x18\x02 \x03(\x0b\x32\x18.statefun_tasks.Pipeline\x12\x17\n\x0fmax_parallelism\x18\x03 \x01(\x05\x12\x0f\n\x07is_wait\x18\x04 \x01(\x08\x12\x19\n\x11return_exceptions\x18\x05 \x01(\x08\"|\n\rPipelineEntry\x12/\n\ntask_entry\x18\x01 \x01(\x0b\x32\x19.statefun_tasks.TaskEntryH\x00\x12\x31\n\x0bgroup_entry\x18\x02 \x01(\x0b\x32\x1a.statefun_tasks.GroupEntryH\x00\x42\x07\n\x05\x65ntry\"\xa2\x02\n\x08Pipeline\x12.\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x1d.statefun_tasks.PipelineEntry\x12\x0e\n\x06inline\x18\x02 \x01(\x08\x12/\n\x0cinitial_args\x18\x03 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x88\x01\x01\x12=\n\x0einitial_kwargs\x18\x04 \x01(\x0b\x32 .statefun_tasks.MapOfStringToAnyH\x01\x88\x01\x01\x12\x30\n\rinitial_state\x18\x05 \x01(\x0b\x32\x14.google.protobuf.AnyH\x02\x88\x01\x01\x42\x0f\n\r_initial_argsB\x11\n\x0f_initial_kwargsB\x10\n\x0e_initial_state\"i\n\x0fTaskRetryPolicy\x12\x11\n\tretry_for\x18\x01 \x03(\t\x12\x13\n\x0bmax_retries\x18\x02 \x01(\x05\x12\x10\n\x08\x64\x65lay_ms\x18\x03 \x01(\x02\x12\x1c\n\x14\x65xponential_back_off\x18\x04 \x01(\x08\"k\n\rArgsAndKwargs\x12(\n\x04\x61rgs\x18\x01 \x01(\x0b\x32\x1a.statefun_tasks.TupleOfAny\x12\x30\n\x06kwargs\x18\x02 \x01(\x0b\x32 .statefun_tasks.MapOfStringToAny\"\xc3\x03\n\x0bTaskRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x15\n\x0breply_topic\x18\x03 \x01(\tH\x00\x12\x30\n\rreply_address\x18\x04 \x01(\x0b\x32\x17.statefun_tasks.AddressH\x00\x12%\n\x07request\x18\x05 \x01(\x0b\x32\x14.google.protobuf.Any\x12#\n\x05state\x18\x06 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x35\n\x0cretry_policy\x18\x07 \x01(\x0b\x32\x1f.statefun_tasks.TaskRetryPolicy\x12\x33\n\x04meta\x18\x08 \x03(\x0b\x32%.statefun_tasks.TaskRequest.MetaEntry\x12\x18\n\x0bis_fruitful\x18\t \x01(\x08H\x01\x88\x01\x01\x12\x1a\n\rinvocation_id\x18\n \x01(\tH\x02\x88\x01\x01\x12\x0b\n\x03uid\x18\x0b \x01(\t\x1a+\n\tMetaEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x07\n\x05replyB\x0e\n\x0c_is_fruitfulB\x10\n\x0e_invocation_id\"\xac\x01\n\nTaskResult\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12$\n\x06result\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12#\n\x05state\x18\x04 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x1a\n\rinvocation_id\x18\x05 \x01(\tH\x00\x88\x01\x01\x12\x0b\n\x03uid\x18\x06 \x01(\tB\x10\n\x0e_invocation_id\"\x9c\x02\n\rTaskException\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x16\n\x0e\x65xception_type\x18\x03 \x01(\t\x12\x19\n\x11\x65xception_message\x18\x04 \x01(\t\x12\x12\n\nstacktrace\x18\x05 \x01(\t\x12#\n\x05state\x18\x06 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x13\n\x0bmaybe_retry\x18\x07 \x01(\x08\x12\x35\n\x0cretry_policy\x18\x08 \x01(\x0b\x32\x1f.statefun_tasks.TaskRetryPolicy\x12\x1a\n\rinvocation_id\x18\t \x01(\tH\x00\x88\x01\x01\x12\x0b\n\x03uid\x18\n \x01(\tB\x10\n\x0e_invocation_id\"\x9f\x01\n\x15TaskResultOrException\x12\x31\n\x0btask_result\x18\x01 \x01(\x0b\x32\x1a.statefun_tasks.TaskResultH\x00\x12\x37\n\x0etask_exception\x18\x02 \x01(\x0b\x32\x1d.statefun_tasks.TaskExceptionH\x00\x42\x1a\n\x18task_result_or_exception\"e\n\x11TaskSpecificState\x12\x13\n\x0bretry_count\x18\x01 \x01(\x05\x12\x1f\n\x17original_caller_address\x18\x02 \x01(\t\x12\x1a\n\x12original_caller_id\x18\x03 \x01(\t\"\xd8\x01\n\tTaskState\x12\x34\n\x06\x62y_uid\x18\x01 \x03(\x0b\x32$.statefun_tasks.TaskState.ByUidEntry\x12\x31\n\x0einternal_state\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x88\x01\x01\x1aO\n\nByUidEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x30\n\x05value\x18\x02 \x01(\x0b\x32!.statefun_tasks.TaskSpecificState:\x02\x38\x01\x42\x11\n\x0f_internal_state\"\x90\x02\n\x0cTaskDeferral\x12+\n\x05tasks\x18\x01 \x03(\x0b\x32\x1c.statefun_tasks.DeferredTask\x12 \n\x13parent_task_address\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x1b\n\x0eparent_task_id\x18\x03 \x01(\tH\x01\x88\x01\x01\x12L\n\x18task_result_or_exception\x18\x04 \x01(\x0b\x32%.statefun_tasks.TaskResultOrExceptionH\x02\x88\x01\x01\x42\x16\n\x14_parent_task_addressB\x11\n\x0f_parent_task_idB\x1b\n\x19_task_result_or_exception\":\n\x0c\x44\x65\x66\x65rredTask\x12\x10\n\x08task_uid\x18\x01 \x01(\t\x12\x18\n\x10has_initial_args\x18\x02 \x01(\x08\"T\n\nPausedTask\x12\x13\n\x0b\x64\x65stination\x18\x01 \x01(\t\x12\x31\n\x0ctask_request\x18\x02 \x01(\x0b\x32\x1b.statefun_tasks.TaskRequest\"\xdb\x07\n\rPipelineState\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x0f\n\x07root_id\x18\x03 \x01(\t\x12\x14\n\x0croot_address\x18\x04 \x01(\t\x12\x11\n\tcaller_id\x18\x05 \x01(\t\x12\x16\n\x0e\x63\x61ller_address\x18\x06 \x01(\t\x12*\n\x08pipeline\x18\x07 \x01(\x0b\x32\x18.statefun_tasks.Pipeline\x12\x31\n\x0ctask_results\x18\x08 \x01(\x0b\x32\x1b.statefun_tasks.TaskResults\x12;\n\x15result_before_finally\x18\t \x01(\x0b\x32\x1a.statefun_tasks.TaskResultH\x00\x12\x41\n\x18\x65xception_before_finally\x18\n \x01(\x0b\x32\x1d.statefun_tasks.TaskExceptionH\x00\x12\x13\n\x0bis_fruitful\x18\x0b \x01(\x08\x12(\n\ntask_state\x18\x0c \x01(\x0b\x32\x14.google.protobuf.Any\x12R\n\x14task_deferrals_by_id\x18\r \x03(\x0b\x32\x34.statefun_tasks.PipelineState.TaskDeferralsByIdEntry\x12\x62\n\x1dtask_deferral_ids_by_task_uid\x18\x0e \x03(\x0b\x32;.statefun_tasks.PipelineState.TaskDeferralIdsByTaskUidEntry\x12*\n\x06status\x18\x0f \x01(\x0b\x32\x1a.statefun_tasks.TaskStatus\x12\x30\n\x0cpaused_tasks\x18\x10 \x03(\x0b\x32\x1a.statefun_tasks.PausedTask\x12\x36\n\x0f\x63hild_pipelines\x18\x11 \x03(\x0b\x32\x1d.statefun_tasks.ChildPipeline\x12-\n\x0flast_task_state\x18\x12 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x15\n\rinvocation_id\x18\x13 \x01(\t\x1aV\n\x16TaskDeferralsByIdEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.statefun_tasks.TaskDeferral:\x02\x38\x01\x1a?\n\x1dTaskDeferralIdsByTaskUidEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x10\n\x0e\x62\x65\x66ore_finally\"\xbe\x01\n\rChildPipeline\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x0f\n\x07root_id\x18\x03 \x01(\t\x12\x14\n\x0croot_address\x18\x04 \x01(\t\x12\x11\n\tcaller_id\x18\x05 \x01(\t\x12\x16\n\x0e\x63\x61ller_address\x18\x06 \x01(\t\x12\'\n\x05tasks\x18\x07 \x03(\x0b\x32\x18.statefun_tasks.TaskInfo\x12\x15\n\rinvocation_id\x18\x08 \x01(\t\"h\n\x08TaskInfo\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x11\n\ttask_type\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x13\n\x0bworker_name\x18\x04 \x01(\t\x12\x10\n\x08task_uid\x18\x05 \x01(\t\"\x89\x01\n\x0bTaskResults\x12\x36\n\x06\x62y_uid\x18\x01 \x03(\x0b\x32&.statefun_tasks.TaskResults.ByUidEntry\x1a\x42\n\nByUidEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.Any:\x02\x38\x01\"\xaa\x01\n\x11TaskActionRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\x0breply_topic\x18\x02 \x01(\tH\x00\x12\x30\n\rreply_address\x18\x03 \x01(\x0b\x32\x17.statefun_tasks.AddressH\x00\x12*\n\x06\x61\x63tion\x18\x04 \x01(\x0e\x32\x1a.statefun_tasks.TaskAction\x12\x0b\n\x03uid\x18\x05 \x01(\tB\x07\n\x05reply\"}\n\x10TaskActionResult\x12\n\n\x02id\x18\x01 \x01(\t\x12*\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32\x1a.statefun_tasks.TaskAction\x12$\n\x06result\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x0b\n\x03uid\x18\x04 \x01(\t\"\xa1\x01\n\x13TaskActionException\x12\n\n\x02id\x18\x01 \x01(\t\x12*\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32\x1a.statefun_tasks.TaskAction\x12\x16\n\x0e\x65xception_type\x18\x03 \x01(\t\x12\x19\n\x11\x65xception_message\x18\x04 \x01(\t\x12\x12\n\nstacktrace\x18\x05 \x01(\t\x12\x0b\n\x03uid\x18\x06 \x01(\t\"\xa8\x01\n\nTaskStatus\x12\x30\n\x05value\x18\x01 \x01(\x0e\x32!.statefun_tasks.TaskStatus.Status\"h\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\x0b\n\x07RUNNING\x10\x01\x12\r\n\tCOMPLETED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\n\n\x06PAUSED\x10\x04\x12\x0e\n\nCANCELLING\x10\x05\x12\r\n\tCANCELLED\x10\x06*|\n\nTaskAction\x12\x0e\n\nGET_STATUS\x10\x00\x12\x0f\n\x0bGET_REQUEST\x10\x01\x12\x0e\n\nGET_RESULT\x10\x02\x12\x12\n\x0ePAUSE_PIPELINE\x10\x03\x12\x14\n\x10UNPAUSE_PIPELINE\x10\x04\x12\x13\n\x0f\x43\x41NCEL_PIPELINE\x10\x05\x62\x06proto3'
+  serialized_pb=b'\n\x0emessages.proto\x12\x0estatefun_tasks\x1a\x19google/protobuf/any.proto\"\x0b\n\tNoneValue\"6\n\x07\x41\x64\x64ress\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\"\x92\x01\n\x10MapOfStringToAny\x12:\n\x05items\x18\x01 \x03(\x0b\x32+.statefun_tasks.MapOfStringToAny.ItemsEntry\x1a\x42\n\nItemsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.Any:\x02\x38\x01\"1\n\nArrayOfAny\x12#\n\x05items\x18\x01 \x03(\x0b\x32\x14.google.protobuf.Any\"1\n\nTupleOfAny\x12#\n\x05items\x18\x01 \x03(\x0b\x32\x14.google.protobuf.Any\"\xd4\x02\n\tTaskEntry\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x11\n\ttask_type\x18\x02 \x01(\t\x12%\n\x07request\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x10\n\x08\x63omplete\x18\x04 \x01(\x08\x12\x12\n\nis_finally\x18\x05 \x01(\x08\x12\x11\n\tnamespace\x18\x06 \x01(\t\x12\x13\n\x0bworker_name\x18\x07 \x01(\t\x12\x13\n\x0bis_fruitful\x18\x08 \x01(\x08\x12\x35\n\x0cretry_policy\x18\t \x01(\x0b\x32\x1f.statefun_tasks.TaskRetryPolicy\x12\x19\n\x0c\x64isplay_name\x18\n \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x07is_wait\x18\x0b \x01(\x08\x12\x0b\n\x03uid\x18\x0c \x01(\t\x12\x18\n\x10is_exceptionally\x18\r \x01(\x08\x42\x0f\n\r_display_name\"\x8c\x01\n\nGroupEntry\x12\x10\n\x08group_id\x18\x01 \x01(\t\x12\'\n\x05group\x18\x02 \x03(\x0b\x32\x18.statefun_tasks.Pipeline\x12\x17\n\x0fmax_parallelism\x18\x03 \x01(\x05\x12\x0f\n\x07is_wait\x18\x04 \x01(\x08\x12\x19\n\x11return_exceptions\x18\x05 \x01(\x08\"|\n\rPipelineEntry\x12/\n\ntask_entry\x18\x01 \x01(\x0b\x32\x19.statefun_tasks.TaskEntryH\x00\x12\x31\n\x0bgroup_entry\x18\x02 \x01(\x0b\x32\x1a.statefun_tasks.GroupEntryH\x00\x42\x07\n\x05\x65ntry\"\xa2\x02\n\x08Pipeline\x12.\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x1d.statefun_tasks.PipelineEntry\x12\x0e\n\x06inline\x18\x02 \x01(\x08\x12/\n\x0cinitial_args\x18\x03 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x88\x01\x01\x12=\n\x0einitial_kwargs\x18\x04 \x01(\x0b\x32 .statefun_tasks.MapOfStringToAnyH\x01\x88\x01\x01\x12\x30\n\rinitial_state\x18\x05 \x01(\x0b\x32\x14.google.protobuf.AnyH\x02\x88\x01\x01\x42\x0f\n\r_initial_argsB\x11\n\x0f_initial_kwargsB\x10\n\x0e_initial_state\"i\n\x0fTaskRetryPolicy\x12\x11\n\tretry_for\x18\x01 \x03(\t\x12\x13\n\x0bmax_retries\x18\x02 \x01(\x05\x12\x10\n\x08\x64\x65lay_ms\x18\x03 \x01(\x02\x12\x1c\n\x14\x65xponential_back_off\x18\x04 \x01(\x08\"k\n\rArgsAndKwargs\x12(\n\x04\x61rgs\x18\x01 \x01(\x0b\x32\x1a.statefun_tasks.TupleOfAny\x12\x30\n\x06kwargs\x18\x02 \x01(\x0b\x32 .statefun_tasks.MapOfStringToAny\"\xc3\x03\n\x0bTaskRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x15\n\x0breply_topic\x18\x03 \x01(\tH\x00\x12\x30\n\rreply_address\x18\x04 \x01(\x0b\x32\x17.statefun_tasks.AddressH\x00\x12%\n\x07request\x18\x05 \x01(\x0b\x32\x14.google.protobuf.Any\x12#\n\x05state\x18\x06 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x35\n\x0cretry_policy\x18\x07 \x01(\x0b\x32\x1f.statefun_tasks.TaskRetryPolicy\x12\x33\n\x04meta\x18\x08 \x03(\x0b\x32%.statefun_tasks.TaskRequest.MetaEntry\x12\x18\n\x0bis_fruitful\x18\t \x01(\x08H\x01\x88\x01\x01\x12\x1a\n\rinvocation_id\x18\n \x01(\tH\x02\x88\x01\x01\x12\x0b\n\x03uid\x18\x0b \x01(\t\x1a+\n\tMetaEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x07\n\x05replyB\x0e\n\x0c_is_fruitfulB\x10\n\x0e_invocation_id\"\xbd\x01\n\nTaskResult\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12$\n\x06result\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12#\n\x05state\x18\x04 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x1a\n\rinvocation_id\x18\x05 \x01(\tH\x00\x88\x01\x01\x12\x0b\n\x03uid\x18\x06 \x01(\t\x12\x0f\n\x07is_wait\x18\x0b \x01(\x08\x42\x10\n\x0e_invocation_id\"\xad\x02\n\rTaskException\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x16\n\x0e\x65xception_type\x18\x03 \x01(\t\x12\x19\n\x11\x65xception_message\x18\x04 \x01(\t\x12\x12\n\nstacktrace\x18\x05 \x01(\t\x12#\n\x05state\x18\x06 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x13\n\x0bmaybe_retry\x18\x07 \x01(\x08\x12\x35\n\x0cretry_policy\x18\x08 \x01(\x0b\x32\x1f.statefun_tasks.TaskRetryPolicy\x12\x1a\n\rinvocation_id\x18\t \x01(\tH\x00\x88\x01\x01\x12\x0b\n\x03uid\x18\n \x01(\t\x12\x0f\n\x07is_wait\x18\x0b \x01(\x08\x42\x10\n\x0e_invocation_id\"\x9f\x01\n\x15TaskResultOrException\x12\x31\n\x0btask_result\x18\x01 \x01(\x0b\x32\x1a.statefun_tasks.TaskResultH\x00\x12\x37\n\x0etask_exception\x18\x02 \x01(\x0b\x32\x1d.statefun_tasks.TaskExceptionH\x00\x42\x1a\n\x18task_result_or_exception\"e\n\x11TaskSpecificState\x12\x13\n\x0bretry_count\x18\x01 \x01(\x05\x12\x1f\n\x17original_caller_address\x18\x02 \x01(\t\x12\x1a\n\x12original_caller_id\x18\x03 \x01(\t\"\xd8\x01\n\tTaskState\x12\x34\n\x06\x62y_uid\x18\x01 \x03(\x0b\x32$.statefun_tasks.TaskState.ByUidEntry\x12\x31\n\x0einternal_state\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x88\x01\x01\x1aO\n\nByUidEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x30\n\x05value\x18\x02 \x01(\x0b\x32!.statefun_tasks.TaskSpecificState:\x02\x38\x01\x42\x11\n\x0f_internal_state\"\x90\x02\n\x0cTaskDeferral\x12+\n\x05tasks\x18\x01 \x03(\x0b\x32\x1c.statefun_tasks.DeferredTask\x12 \n\x13parent_task_address\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x1b\n\x0eparent_task_id\x18\x03 \x01(\tH\x01\x88\x01\x01\x12L\n\x18task_result_or_exception\x18\x04 \x01(\x0b\x32%.statefun_tasks.TaskResultOrExceptionH\x02\x88\x01\x01\x42\x16\n\x14_parent_task_addressB\x11\n\x0f_parent_task_idB\x1b\n\x19_task_result_or_exception\":\n\x0c\x44\x65\x66\x65rredTask\x12\x10\n\x08task_uid\x18\x01 \x01(\t\x12\x18\n\x10has_initial_args\x18\x02 \x01(\x08\"T\n\nPausedTask\x12\x13\n\x0b\x64\x65stination\x18\x01 \x01(\t\x12\x31\n\x0ctask_request\x18\x02 \x01(\x0b\x32\x1b.statefun_tasks.TaskRequest\"\xdb\x07\n\rPipelineState\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x0f\n\x07root_id\x18\x03 \x01(\t\x12\x14\n\x0croot_address\x18\x04 \x01(\t\x12\x11\n\tcaller_id\x18\x05 \x01(\t\x12\x16\n\x0e\x63\x61ller_address\x18\x06 \x01(\t\x12*\n\x08pipeline\x18\x07 \x01(\x0b\x32\x18.statefun_tasks.Pipeline\x12\x31\n\x0ctask_results\x18\x08 \x01(\x0b\x32\x1b.statefun_tasks.TaskResults\x12;\n\x15result_before_finally\x18\t \x01(\x0b\x32\x1a.statefun_tasks.TaskResultH\x00\x12\x41\n\x18\x65xception_before_finally\x18\n \x01(\x0b\x32\x1d.statefun_tasks.TaskExceptionH\x00\x12\x13\n\x0bis_fruitful\x18\x0b \x01(\x08\x12(\n\ntask_state\x18\x0c \x01(\x0b\x32\x14.google.protobuf.Any\x12R\n\x14task_deferrals_by_id\x18\r \x03(\x0b\x32\x34.statefun_tasks.PipelineState.TaskDeferralsByIdEntry\x12\x62\n\x1dtask_deferral_ids_by_task_uid\x18\x0e \x03(\x0b\x32;.statefun_tasks.PipelineState.TaskDeferralIdsByTaskUidEntry\x12*\n\x06status\x18\x0f \x01(\x0b\x32\x1a.statefun_tasks.TaskStatus\x12\x30\n\x0cpaused_tasks\x18\x10 \x03(\x0b\x32\x1a.statefun_tasks.PausedTask\x12\x36\n\x0f\x63hild_pipelines\x18\x11 \x03(\x0b\x32\x1d.statefun_tasks.ChildPipeline\x12-\n\x0flast_task_state\x18\x12 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x15\n\rinvocation_id\x18\x13 \x01(\t\x1aV\n\x16TaskDeferralsByIdEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.statefun_tasks.TaskDeferral:\x02\x38\x01\x1a?\n\x1dTaskDeferralIdsByTaskUidEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x10\n\x0e\x62\x65\x66ore_finally\"\xbe\x01\n\rChildPipeline\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x0f\n\x07root_id\x18\x03 \x01(\t\x12\x14\n\x0croot_address\x18\x04 \x01(\t\x12\x11\n\tcaller_id\x18\x05 \x01(\t\x12\x16\n\x0e\x63\x61ller_address\x18\x06 \x01(\t\x12\'\n\x05tasks\x18\x07 \x03(\x0b\x32\x18.statefun_tasks.TaskInfo\x12\x15\n\rinvocation_id\x18\x08 \x01(\t\"h\n\x08TaskInfo\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x11\n\ttask_type\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x13\n\x0bworker_name\x18\x04 \x01(\t\x12\x10\n\x08task_uid\x18\x05 \x01(\t\"\x89\x01\n\x0bTaskResults\x12\x36\n\x06\x62y_uid\x18\x01 \x03(\x0b\x32&.statefun_tasks.TaskResults.ByUidEntry\x1a\x42\n\nByUidEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.Any:\x02\x38\x01\"\xaa\x01\n\x11TaskActionRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\x0breply_topic\x18\x02 \x01(\tH\x00\x12\x30\n\rreply_address\x18\x03 \x01(\x0b\x32\x17.statefun_tasks.AddressH\x00\x12*\n\x06\x61\x63tion\x18\x04 \x01(\x0e\x32\x1a.statefun_tasks.TaskAction\x12\x0b\n\x03uid\x18\x05 \x01(\tB\x07\n\x05reply\"}\n\x10TaskActionResult\x12\n\n\x02id\x18\x01 \x01(\t\x12*\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32\x1a.statefun_tasks.TaskAction\x12$\n\x06result\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x0b\n\x03uid\x18\x04 \x01(\t\"\xa1\x01\n\x13TaskActionException\x12\n\n\x02id\x18\x01 \x01(\t\x12*\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32\x1a.statefun_tasks.TaskAction\x12\x16\n\x0e\x65xception_type\x18\x03 \x01(\t\x12\x19\n\x11\x65xception_message\x18\x04 \x01(\t\x12\x12\n\nstacktrace\x18\x05 \x01(\t\x12\x0b\n\x03uid\x18\x06 \x01(\t\"\xa8\x01\n\nTaskStatus\x12\x30\n\x05value\x18\x01 \x01(\x0e\x32!.statefun_tasks.TaskStatus.Status\"h\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\x0b\n\x07RUNNING\x10\x01\x12\r\n\tCOMPLETED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\n\n\x06PAUSED\x10\x04\x12\x0e\n\nCANCELLING\x10\x05\x12\r\n\tCANCELLED\x10\x06*|\n\nTaskAction\x12\x0e\n\nGET_STATUS\x10\x00\x12\x0f\n\x0bGET_REQUEST\x10\x01\x12\x0e\n\nGET_RESULT\x10\x02\x12\x12\n\x0ePAUSE_PIPELINE\x10\x03\x12\x14\n\x10UNPAUSE_PIPELINE\x10\x04\x12\x13\n\x0f\x43\x41NCEL_PIPELINE\x10\x05\x62\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_any__pb2.DESCRIPTOR,])
 
 _TASKACTION = _descriptor.EnumDescriptor(
   name='TaskAction',
   full_name='statefun_tasks.TaskAction',
   filename=None,
@@ -61,16 +61,16 @@
       name='CANCEL_PIPELINE', index=5, number=5,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=5387,
-  serialized_end=5511,
+  serialized_start=5421,
+  serialized_end=5545,
 )
 _sym_db.RegisterEnumDescriptor(_TASKACTION)
 
 TaskAction = enum_type_wrapper.EnumTypeWrapper(_TASKACTION)
 GET_STATUS = 0
 GET_REQUEST = 1
 GET_RESULT = 2
@@ -120,16 +120,16 @@
       name='CANCELLED', index=6, number=6,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=5281,
-  serialized_end=5385,
+  serialized_start=5315,
+  serialized_end=5419,
 )
 _sym_db.RegisterEnumDescriptor(_TASKSTATUS_STATUS)
 
 
 _NONEVALUE = _descriptor.Descriptor(
   name='NoneValue',
   full_name='statefun_tasks.NoneValue',
@@ -928,14 +928,21 @@
     _descriptor.FieldDescriptor(
       name='uid', full_name='statefun_tasks.TaskResult.uid', index=5,
       number=6, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='is_wait', full_name='statefun_tasks.TaskResult.is_wait', index=6,
+      number=11, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -946,15 +953,15 @@
     _descriptor.OneofDescriptor(
       name='_invocation_id', full_name='statefun_tasks.TaskResult._invocation_id',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
   serialized_start=1957,
-  serialized_end=2129,
+  serialized_end=2146,
 )
 
 
 _TASKEXCEPTION = _descriptor.Descriptor(
   name='TaskException',
   full_name='statefun_tasks.TaskException',
   filename=None,
@@ -1028,14 +1035,21 @@
     _descriptor.FieldDescriptor(
       name='uid', full_name='statefun_tasks.TaskException.uid', index=9,
       number=10, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='is_wait', full_name='statefun_tasks.TaskException.is_wait', index=10,
+      number=11, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -1045,16 +1059,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='_invocation_id', full_name='statefun_tasks.TaskException._invocation_id',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=2132,
-  serialized_end=2416,
+  serialized_start=2149,
+  serialized_end=2450,
 )
 
 
 _TASKRESULTOREXCEPTION = _descriptor.Descriptor(
   name='TaskResultOrException',
   full_name='statefun_tasks.TaskResultOrException',
   filename=None,
@@ -1089,16 +1103,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='task_result_or_exception', full_name='statefun_tasks.TaskResultOrException.task_result_or_exception',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=2419,
-  serialized_end=2578,
+  serialized_start=2453,
+  serialized_end=2612,
 )
 
 
 _TASKSPECIFICSTATE = _descriptor.Descriptor(
   name='TaskSpecificState',
   full_name='statefun_tasks.TaskSpecificState',
   filename=None,
@@ -1135,16 +1149,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2580,
-  serialized_end=2681,
+  serialized_start=2614,
+  serialized_end=2715,
 )
 
 
 _TASKSTATE_BYUIDENTRY = _descriptor.Descriptor(
   name='ByUidEntry',
   full_name='statefun_tasks.TaskState.ByUidEntry',
   filename=None,
@@ -1174,16 +1188,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2802,
-  serialized_end=2881,
+  serialized_start=2836,
+  serialized_end=2915,
 )
 
 _TASKSTATE = _descriptor.Descriptor(
   name='TaskState',
   full_name='statefun_tasks.TaskState',
   filename=None,
   file=DESCRIPTOR,
@@ -1217,16 +1231,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='_internal_state', full_name='statefun_tasks.TaskState._internal_state',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=2684,
-  serialized_end=2900,
+  serialized_start=2718,
+  serialized_end=2934,
 )
 
 
 _TASKDEFERRAL = _descriptor.Descriptor(
   name='TaskDeferral',
   full_name='statefun_tasks.TaskDeferral',
   filename=None,
@@ -1285,16 +1299,16 @@
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_task_result_or_exception', full_name='statefun_tasks.TaskDeferral._task_result_or_exception',
       index=2, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=2903,
-  serialized_end=3175,
+  serialized_start=2937,
+  serialized_end=3209,
 )
 
 
 _DEFERREDTASK = _descriptor.Descriptor(
   name='DeferredTask',
   full_name='statefun_tasks.DeferredTask',
   filename=None,
@@ -1324,16 +1338,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3177,
-  serialized_end=3235,
+  serialized_start=3211,
+  serialized_end=3269,
 )
 
 
 _PAUSEDTASK = _descriptor.Descriptor(
   name='PausedTask',
   full_name='statefun_tasks.PausedTask',
   filename=None,
@@ -1363,16 +1377,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3237,
-  serialized_end=3321,
+  serialized_start=3271,
+  serialized_end=3355,
 )
 
 
 _PIPELINESTATE_TASKDEFERRALSBYIDENTRY = _descriptor.Descriptor(
   name='TaskDeferralsByIdEntry',
   full_name='statefun_tasks.PipelineState.TaskDeferralsByIdEntry',
   filename=None,
@@ -1402,16 +1416,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4142,
-  serialized_end=4228,
+  serialized_start=4176,
+  serialized_end=4262,
 )
 
 _PIPELINESTATE_TASKDEFERRALIDSBYTASKUIDENTRY = _descriptor.Descriptor(
   name='TaskDeferralIdsByTaskUidEntry',
   full_name='statefun_tasks.PipelineState.TaskDeferralIdsByTaskUidEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -1440,16 +1454,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4230,
-  serialized_end=4293,
+  serialized_start=4264,
+  serialized_end=4327,
 )
 
 _PIPELINESTATE = _descriptor.Descriptor(
   name='PipelineState',
   full_name='statefun_tasks.PipelineState',
   filename=None,
   file=DESCRIPTOR,
@@ -1602,16 +1616,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='before_finally', full_name='statefun_tasks.PipelineState.before_finally',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=3324,
-  serialized_end=4311,
+  serialized_start=3358,
+  serialized_end=4345,
 )
 
 
 _CHILDPIPELINE = _descriptor.Descriptor(
   name='ChildPipeline',
   full_name='statefun_tasks.ChildPipeline',
   filename=None,
@@ -1683,16 +1697,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4314,
-  serialized_end=4504,
+  serialized_start=4348,
+  serialized_end=4538,
 )
 
 
 _TASKINFO = _descriptor.Descriptor(
   name='TaskInfo',
   full_name='statefun_tasks.TaskInfo',
   filename=None,
@@ -1743,16 +1757,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4506,
-  serialized_end=4610,
+  serialized_start=4540,
+  serialized_end=4644,
 )
 
 
 _TASKRESULTS_BYUIDENTRY = _descriptor.Descriptor(
   name='ByUidEntry',
   full_name='statefun_tasks.TaskResults.ByUidEntry',
   filename=None,
@@ -1782,16 +1796,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4684,
-  serialized_end=4750,
+  serialized_start=4718,
+  serialized_end=4784,
 )
 
 _TASKRESULTS = _descriptor.Descriptor(
   name='TaskResults',
   full_name='statefun_tasks.TaskResults',
   filename=None,
   file=DESCRIPTOR,
@@ -1813,16 +1827,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4613,
-  serialized_end=4750,
+  serialized_start=4647,
+  serialized_end=4784,
 )
 
 
 _TASKACTIONREQUEST = _descriptor.Descriptor(
   name='TaskActionRequest',
   full_name='statefun_tasks.TaskActionRequest',
   filename=None,
@@ -1878,16 +1892,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='reply', full_name='statefun_tasks.TaskActionRequest.reply',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=4753,
-  serialized_end=4923,
+  serialized_start=4787,
+  serialized_end=4957,
 )
 
 
 _TASKACTIONRESULT = _descriptor.Descriptor(
   name='TaskActionResult',
   full_name='statefun_tasks.TaskActionResult',
   filename=None,
@@ -1931,16 +1945,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4925,
-  serialized_end=5050,
+  serialized_start=4959,
+  serialized_end=5084,
 )
 
 
 _TASKACTIONEXCEPTION = _descriptor.Descriptor(
   name='TaskActionException',
   full_name='statefun_tasks.TaskActionException',
   filename=None,
@@ -1998,16 +2012,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5053,
-  serialized_end=5214,
+  serialized_start=5087,
+  serialized_end=5248,
 )
 
 
 _TASKSTATUS = _descriptor.Descriptor(
   name='TaskStatus',
   full_name='statefun_tasks.TaskStatus',
   filename=None,
@@ -2031,16 +2045,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5217,
-  serialized_end=5385,
+  serialized_start=5251,
+  serialized_end=5419,
 )
 
 _MAPOFSTRINGTOANY_ITEMSENTRY.fields_by_name['value'].message_type = google_dot_protobuf_dot_any__pb2._ANY
 _MAPOFSTRINGTOANY_ITEMSENTRY.containing_type = _MAPOFSTRINGTOANY
 _MAPOFSTRINGTOANY.fields_by_name['items'].message_type = _MAPOFSTRINGTOANY_ITEMSENTRY
 _ARRAYOFANY.fields_by_name['items'].message_type = google_dot_protobuf_dot_any__pb2._ANY
 _TUPLEOFANY.fields_by_name['items'].message_type = google_dot_protobuf_dot_any__pb2._ANY
```

### Comparing `statefun-tasks-0.9.90/statefun_tasks/pipeline.py` & `statefun-tasks-0.9.91/statefun_tasks/pipeline.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/pipeline_builder.py` & `statefun-tasks-0.9.91/statefun_tasks/pipeline_builder.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/handlers/begin_pipeline_handler.py` & `statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/begin_pipeline_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/handlers/cancel_pipeline_handler.py` & `statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/cancel_pipeline_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/handlers/continue_pipeline_handler.py` & `statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/continue_pipeline_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,18 +55,18 @@
                 
                 # update last known task state in case we need to cancel later and call a finally task passing through the current state
                 context.pipeline_state.last_task_state.CopyFrom(task_result_or_exception.state)   
 
                 # pause the pipeline if this completed group is a wait
                 if group.is_wait:
                     await pipeline.pause(context)
-        else:
-            # pause the pipeline if this task is a wait
-            if current_step.is_wait:  
-                await pipeline.pause(context)
+
+        # pause the pipeline if this task entry or the response indicates we should wait
+        if current_step.is_wait or message.is_wait:  
+            await pipeline.pause(context)
 
         # notify event handlers of any skipped tasks such as exceptionally tasks that are passed over if we don't have a TaskException
         await pipeline.events.notify_pipeline_tasks_skipped(context, skipped_tasks)
 
         # if we got an exception then if we have an exceptionally, pass the exception as a result to this task
         if isinstance(task_result_or_exception, TaskException):
```

### Comparing `statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/handlers/end_pipeline_handler.py` & `statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/end_pipeline_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/handlers/pipeline_message_handler.py` & `statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/pipeline_message_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/helpers/pipeline_graph.py` & `statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/pipeline_graph.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/helpers/result_aggregator.py` & `statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/result_aggregator.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/helpers/result_emitter.py` & `statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/result_emitter.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/pipeline_impl/helpers/task_submitter.py` & `statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/task_submitter.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/protobuf.py` & `statefun-tasks-0.9.91/statefun_tasks/protobuf.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/serialisation.py` & `statefun-tasks-0.9.91/statefun_tasks/serialisation.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/task_builder.py` & `statefun-tasks-0.9.91/statefun_tasks/task_builder.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/task_impl/handlers/child_pipeline_handler.py` & `statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/child_pipeline_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/task_impl/handlers/message_handler.py` & `statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/task_impl/handlers/task_action_handler.py` & `statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/task_action_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/task_impl/handlers/task_request_handler.py` & `statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/task_request_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,20 +54,20 @@
             ()
 
         # else if we have an task exception, attempt retry or return the error
         elif task_exception is not None:
             if await self._attempt_retry(context, tasks, task_request, task_exception):
                 return  # we have triggered a retry so ignore the result of this invocation
 
-            context.storage.task_result = task_exception
+            context.storage.task_exception = task_exception
             await tasks.emit_result(context, task_request, task_exception)
 
         # else if we have a task result return it
         elif task_result is not None:
-            context.storage.task_exception = task_result
+            context.storage.task_result = task_result
             await tasks.emit_result(context, task_request, task_result)
 
     async def _attempt_retry(self, context, tasks, task_request, task_exception):
         task_state = context.task_state.by_uid[task_request.uid]
 
         if task_exception.maybe_retry and task_exception.retry_policy is not None:           
             if task_state.retry_count >= task_exception.retry_policy.max_retries:
```

### Comparing `statefun-tasks-0.9.90/statefun_tasks/task_impl/handlers/task_response_handler.py` & `statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/task_response_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/tasks.py` & `statefun-tasks-0.9.91/statefun_tasks/tasks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from statefun_tasks.context import TaskContext
 from statefun_tasks.events.event_handlers import EventHandlers
 from statefun_tasks.pipeline_builder import PipelineBuilder
 from statefun_tasks.utils import _is_tuple, _type_name, _annotated_protos_for
 from statefun_tasks.messages_pb2 import TaskRequest
 from statefun_tasks.type_helpers import _create_task_result, _create_task_exception
 from statefun_tasks.types import YieldTaskInvocation
+from statefun_tasks.effects import Effect
 
 from typing import AsyncGenerator, Generator
 import inspect
 import asyncio
 
 
 
@@ -37,15 +38,15 @@
     def function(self):
         """
         The Python function that this FlinkTask wraps
         """
         return self._fun
 
     async def run(self, task_context: TaskContext, task_request: TaskRequest):
-        task_result, task_exception, pipeline = None, None, None
+        task_result, task_exception, pipeline, effect = None, None, None, None
 
         task_args, kwargs, fn_state = self._to_task_args_and_kwargs(task_context, task_request)
 
         # run the flink task
         try:
             fn_result = self._fun(*task_args, **kwargs)
             
@@ -54,31 +55,39 @@
                 fn_result = list([x async for x in fn_result])
 
             elif isinstance(fn_result, Generator):
                 fn_result = list([x for x in fn_result])
 
             # await coros
             elif asyncio.iscoroutine(fn_result):
-                fn_result = await fn_result
+                fn_result = await fn_result               
 
+            # result of a task might be wrapped in an effect
+            if isinstance(fn_result, Effect):
+                effect = fn_result
+                fn_result = effect.fn_result
+                
             pipeline, task_result, fn_state = self._to_pipeline_or_task_result(task_context, task_request, fn_result, fn_state)
 
-        
+            # apply effects if we have them
+            if effect is not None:
+                effect.apply(task_result)
+
         except YieldTaskInvocation as e:
             # task yielded so we don't output anything
             ()
 
         except Exception as e:
             # we errored so return a task_exception instead
             task_exception = self._to_task_exception(task_request, e)
 
         return task_result, task_exception, pipeline, fn_state
 
     def _to_pipeline_or_task_result(self, task_context, task_request, fn_result, fn_state):
-        pipeline, task_result, is_fruitful = None, None, self._is_fruitful
+        pipeline, is_fruitful = None, self._is_fruitful
 
         if is_fruitful and task_request.HasField('is_fruitful'):
             is_fruitful = task_request.is_fruitful
 
         # if single result then wrap in tuple as this is the maximal case
         if not _is_tuple(fn_result):
             fn_result = (fn_result,)
```

### Comparing `statefun-tasks-0.9.90/statefun_tasks/type_helpers.py` & `statefun-tasks-0.9.91/statefun_tasks/type_helpers.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/types.py` & `statefun-tasks-0.9.91/statefun_tasks/types.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks/utils.py` & `statefun-tasks-0.9.91/statefun_tasks/utils.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.90/statefun_tasks.egg-info/PKG-INFO` & `statefun-tasks-0.9.91/statefun_tasks.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statefun-tasks
-Version: 0.9.90
+Version: 0.9.91
 Summary: Tasks API for Stateful Functions on Flink
 Home-page: https://fransking.github.io/flink-statefun-tasks
 Author: Frans King & Luke Ashworth
 Author-email: frans.king@sbbsystems.com
 License: https://www.apache.org/licenses/LICENSE-2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
@@ -33,11 +33,12 @@
 
 
 @tasks.bind()
 def say_goodbye(greeting):
     return f'{greeting}.  So now I will say goodbye'
 ```
 
+Try the [demo](https://flink-demo-az.sbbsystems.co.uk).
 
 Additional documentation can be found [here](https://fransking.github.io/flink-statefun-tasks).
```

### Comparing `statefun-tasks-0.9.90/statefun_tasks.egg-info/SOURCES.txt` & `statefun-tasks-0.9.91/statefun_tasks.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 statefun_tasks.egg-info/SOURCES.txt
 statefun_tasks.egg-info/dependency_links.txt
 statefun_tasks.egg-info/requires.txt
 statefun_tasks.egg-info/top_level.txt
 statefun_tasks/client/__init__.py
 statefun_tasks/client/tasks_client.py
 statefun_tasks/client/types.py
+statefun_tasks/effects/__init__.py
+statefun_tasks/effects/effect.py
+statefun_tasks/effects/pause_pipeline_effect.py
 statefun_tasks/events/__init__.py
 statefun_tasks/events/event_handlers.py
 statefun_tasks/extensions/__init__.py
 statefun_tasks/extensions/inline_tasks/__init__.py
 statefun_tasks/extensions/inline_tasks/inline_tasks_impl.py
 statefun_tasks/pipeline_impl/__init__.py
 statefun_tasks/pipeline_impl/handlers/__init__.py
```


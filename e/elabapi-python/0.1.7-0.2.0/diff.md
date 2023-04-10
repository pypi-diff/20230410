# Comparing `tmp/elabapi-python-0.1.7.tar.gz` & `tmp/elabapi-python-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elabapi-python-0.1.7.tar", last modified: Tue Mar  7 13:47:42 2023, max compression
+gzip compressed data, was "elabapi-python-0.2.0.tar", last modified: Mon Apr 10 15:18:54 2023, max compression
```

## Comparing `elabapi-python-0.1.7.tar` & `elabapi-python-0.2.0.tar`

### file list

```diff
@@ -1,188 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 13:47:42.470126 elabapi-python-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-07 13:47:42.470126 elabapi-python-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18635 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 13:47:42.434126 elabapi-python-0.1.7/elabapi_python/
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 13:47:42.438127 elabapi-python-0.1.7/elabapi_python/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/api_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23562 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/comments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14817 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/experiments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18664 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/experiments_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/favorite_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19746 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/items_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17478 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/items_types_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/links_to_experiments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14628 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/links_to_items_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/notifications_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20141 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18459 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/steps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22933 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20990 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/team_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20313 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/teamgroups_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14089 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/teams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/todolist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/unfinished_steps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28747 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/uploads_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14987 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25079 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 13:47:42.454126 elabapi-python-0.1.7/elabapi_python/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/elabapi_python/models/apikey.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/elabapi_python/models/apikeys_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/elabapi_python/models/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)    69462 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/elabapi_python/models/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    31781 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/elabapi_python/models/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/elabapi_python/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/elabapi_python/models/events_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/elabapi_python/models/events_id_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/elabapi_python/models/eventsid_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/elabapi_python/models/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/experiment_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/experiments_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/experiments_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/experiments_links_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/experiments_templates_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/experiments_templates_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/favtags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/id1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/id2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/id_comments_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/id_status_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/id_steps_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/id_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/id_teamgroups_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/id_uploads_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/inline_response200.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/inline_response2001.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/inline_response2002.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/inline_response2003.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/items_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/items_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/items_links_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/items_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/items_types_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/steps_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/tags_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/team_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/team_tags_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/team_tags_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/teamgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/teamgroup_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/teamgroups_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/elabapi_python/models/teams_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/models/todoitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/models/todolist_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/models/todolist_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/models/unfinished_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/models/unfinished_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/models/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/models/uploads_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/models/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/models/users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/models/users_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/elabapi_python/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 13:47:42.434126 elabapi-python-0.1.7/elabapi_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-07 13:47:42.000000 elabapi-python-0.1.7/elabapi_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-03-07 13:47:42.000000 elabapi-python-0.1.7/elabapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 13:47:42.000000 elabapi-python-0.1.7/elabapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-07 13:47:42.000000 elabapi-python-0.1.7/elabapi_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-07 13:47:42.000000 elabapi-python-0.1.7/elabapi_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 13:47:42.470126 elabapi-python-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 13:47:42.470126 elabapi-python-0.1.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_api_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/test/test_apikey.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/test/test_apikeys_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/test/test_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_comments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/test/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/test/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/test/test_events_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/test/test_events_id_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/test/test_eventsid_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-07 13:47:31.000000 elabapi-python-0.1.7/test/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_experiment_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_experiments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_experiments_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_experiments_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_experiments_links_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_experiments_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_experiments_templates_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_experiments_templates_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_favorite_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_favtags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_id1.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_id2.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_id_comments_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_id_status_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_id_steps_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_id_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_id_teamgroups_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_id_uploads_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_inline_response200.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_inline_response2001.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_inline_response2002.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_inline_response2003.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_items_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_items_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_items_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_items_links_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_items_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_items_types_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_items_types_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_links_to_experiments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_links_to_items_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_notifications_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_steps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_steps_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_tags_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_team_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_team_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_team_tags_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_team_tags_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_teamgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_teamgroup_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_teamgroups_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_teamgroups_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_teams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-07 13:47:32.000000 elabapi-python-0.1.7/test/test_teams_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_todoitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_todolist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_todolist_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_todolist_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_unfinished_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_unfinished_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_unfinished_steps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_uploads_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_uploads_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-07 13:47:33.000000 elabapi-python-0.1.7/test/test_users_id_body.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:54.564270 elabapi-python-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-10 15:18:54.564270 elabapi-python-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19244 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:54.532268 elabapi-python-0.2.0/elabapi_python/
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:54.536269 elabapi-python-0.2.0/elabapi_python/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/api_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23562 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/comments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14817 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/experiments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18664 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/experiments_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/favorite_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17373 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/idps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19746 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/items_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17478 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/items_types_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/links_to_experiments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14628 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/links_to_items_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20141 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18459 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/steps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22933 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20990 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/team_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20313 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/teamgroups_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/todolist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/unfinished_steps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28747 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/uploads_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25079 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:54.548269 elabapi-python-0.2.0/elabapi_python/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/elabapi_python/models/apikey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/elabapi_python/models/apikeys_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/elabapi_python/models/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72181 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/elabapi_python/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31781 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/elabapi_python/models/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/elabapi_python/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/elabapi_python/models/events_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/events_id_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/eventsid_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/experiment_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/experiments_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/experiments_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/experiments_links_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/experiments_templates_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/experiments_templates_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/favtags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id_comments_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id_status_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id_steps_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id_teamgroups_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/id_uploads_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/idp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/idps_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/idps_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/inline_response200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/inline_response2001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/inline_response2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/inline_response2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/items_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/items_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/items_links_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/items_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/items_types_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/steps_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/tags_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/team_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/team_tags_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/team_tags_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/teamgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/teamgroup_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/teamgroups_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/teams_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/todoitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/elabapi_python/models/todolist_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/todolist_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/unfinished_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/unfinished_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/uploads_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10577 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/users_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/models/users_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/elabapi_python/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:54.532268 elabapi-python-0.2.0/elabapi_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-10 15:18:54.000000 elabapi-python-0.2.0/elabapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-04-10 15:18:54.000000 elabapi-python-0.2.0/elabapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:18:54.000000 elabapi-python-0.2.0/elabapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-10 15:18:54.000000 elabapi-python-0.2.0/elabapi_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 15:18:54.000000 elabapi-python-0.2.0/elabapi_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:18:54.564270 elabapi-python-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:18:54.564270 elabapi-python-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_api_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/test/test_apikey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/test/test_apikeys_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/test/test_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_comments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/test/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-10 15:18:42.000000 elabapi-python-0.2.0/test/test_events_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_events_id_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_eventsid_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_experiment_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_experiments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_experiments_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_experiments_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_experiments_links_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_experiments_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_experiments_templates_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_experiments_templates_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_favorite_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_favtags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id_comments_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id_status_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id_steps_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id_teamgroups_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_id_uploads_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_idp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_idps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_idps_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_idps_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_inline_response200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_inline_response2001.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_inline_response2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_inline_response2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_items_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_items_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_items_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_items_links_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_items_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_items_types_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_items_types_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_links_to_experiments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_links_to_items_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_steps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_steps_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_tags_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_team_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_team_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_team_tags_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_team_tags_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_teamgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_teamgroup_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_teamgroups_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_teamgroups_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_teams_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_todoitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_todolist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-10 15:18:43.000000 elabapi-python-0.2.0/test/test_todolist_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_todolist_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_unfinished_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_unfinished_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_unfinished_steps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_uploads_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_uploads_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_users_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-10 15:18:44.000000 elabapi-python-0.2.0/test/test_users_teams.py
```

### Comparing `elabapi-python-0.1.7/README.md` & `elabapi-python-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # elabapi-python
 This document describes all available endpoints and methods for eLabFTW's API version 2. 
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 2.0.0
-- Package version: 0.1.7
+- Package version: 0.2.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -130,14 +130,19 @@
 *ExperimentsTemplatesApi* | [**get_experiment_template**](docs/ExperimentsTemplatesApi.md#get_experiment_template) | **GET** /experiments_templates/{id} | Read an experiment template
 *ExperimentsTemplatesApi* | [**patch_experiment_template**](docs/ExperimentsTemplatesApi.md#patch_experiment_template) | **PATCH** /experiments_templates/{id} | Modify an experiment template
 *ExperimentsTemplatesApi* | [**post_experiment_template**](docs/ExperimentsTemplatesApi.md#post_experiment_template) | **POST** /experiments_templates | Create an experiment template
 *ExperimentsTemplatesApi* | [**read_experiments_templates**](docs/ExperimentsTemplatesApi.md#read_experiments_templates) | **GET** /experiments_templates | Read all experiments_templates that are accessible
 *FavoriteTagsApi* | [**delete_favtag**](docs/FavoriteTagsApi.md#delete_favtag) | **DELETE** /favtags/{id} | Unfavorite a tag.
 *FavoriteTagsApi* | [**post_favtags**](docs/FavoriteTagsApi.md#post_favtags) | **POST** /favtags | Add a tag as favorite.
 *FavoriteTagsApi* | [**read_favtags**](docs/FavoriteTagsApi.md#read_favtags) | **GET** /favtags | Read all favorite tags for the user.
+*IdpsApi* | [**delete_idp**](docs/IdpsApi.md#delete_idp) | **DELETE** /idps/{id} | Delete an idp.
+*IdpsApi* | [**patch_idp**](docs/IdpsApi.md#patch_idp) | **PATCH** /idps/{id} | Actions on an idp.
+*IdpsApi* | [**post_idp**](docs/IdpsApi.md#post_idp) | **POST** /idps | Create an idp.
+*IdpsApi* | [**read_idp**](docs/IdpsApi.md#read_idp) | **GET** /idps/{id} | Read an idp.
+*IdpsApi* | [**read_idps**](docs/IdpsApi.md#read_idps) | **GET** /idps | Read all IDPs.
 *ItemsApi* | [**delete_item**](docs/ItemsApi.md#delete_item) | **DELETE** /items/{id} | Delete an item.
 *ItemsApi* | [**get_item**](docs/ItemsApi.md#get_item) | **GET** /items/{id} | Read an item
 *ItemsApi* | [**patch_item**](docs/ItemsApi.md#patch_item) | **PATCH** /items/{id} | Modify an item
 *ItemsApi* | [**post_item**](docs/ItemsApi.md#post_item) | **POST** /items | Create an item
 *ItemsApi* | [**read_items**](docs/ItemsApi.md#read_items) | **GET** /items | Read all items that are accessible
 *ItemsTypesApi* | [**delete_items_type**](docs/ItemsTypesApi.md#delete_items_type) | **DELETE** /items_types/{id} | Delete an item type.
 *ItemsTypesApi* | [**get_items_type**](docs/ItemsTypesApi.md#get_items_type) | **GET** /items_types/{id} | Read an items type
@@ -218,20 +223,24 @@
  - [ExperimentsLinksSubidBody](docs/ExperimentsLinksSubidBody.md)
  - [ExperimentsTemplatesBody](docs/ExperimentsTemplatesBody.md)
  - [ExperimentsTemplatesIdBody](docs/ExperimentsTemplatesIdBody.md)
  - [FavtagsBody](docs/FavtagsBody.md)
  - [Id](docs/Id.md)
  - [Id1](docs/Id1.md)
  - [Id2](docs/Id2.md)
+ - [Id3](docs/Id3.md)
  - [IdCommentsBody](docs/IdCommentsBody.md)
  - [IdStatusBody](docs/IdStatusBody.md)
  - [IdStepsBody](docs/IdStepsBody.md)
  - [IdTagsBody](docs/IdTagsBody.md)
  - [IdTeamgroupsBody](docs/IdTeamgroupsBody.md)
  - [IdUploadsBody](docs/IdUploadsBody.md)
+ - [Idp](docs/Idp.md)
+ - [IdpsBody](docs/IdpsBody.md)
+ - [IdpsIdBody](docs/IdpsIdBody.md)
  - [InlineResponse200](docs/InlineResponse200.md)
  - [InlineResponse2001](docs/InlineResponse2001.md)
  - [InlineResponse2002](docs/InlineResponse2002.md)
  - [InlineResponse2003](docs/InlineResponse2003.md)
  - [Item](docs/Item.md)
  - [ItemsBody](docs/ItemsBody.md)
  - [ItemsIdBody](docs/ItemsIdBody.md)
@@ -259,14 +268,15 @@
  - [UnfinishedStep](docs/UnfinishedStep.md)
  - [UnfinishedSteps](docs/UnfinishedSteps.md)
  - [Upload](docs/Upload.md)
  - [UploadsSubidBody](docs/UploadsSubidBody.md)
  - [Users](docs/Users.md)
  - [UsersBody](docs/UsersBody.md)
  - [UsersIdBody](docs/UsersIdBody.md)
+ - [UsersTeams](docs/UsersTeams.md)
 
 ## Documentation For Authorization
 
 
 ## token
 
 - **Type**: API key
```

### Comparing `elabapi-python-0.1.7/elabapi_python/__init__.py` & `elabapi-python-0.2.0/elabapi_python/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from elabapi_python.api.api_keys_api import ApiKeysApi
 from elabapi_python.api.comments_api import CommentsApi
 from elabapi_python.api.config_api import ConfigApi
 from elabapi_python.api.events_api import EventsApi
 from elabapi_python.api.experiments_api import ExperimentsApi
 from elabapi_python.api.experiments_templates_api import ExperimentsTemplatesApi
 from elabapi_python.api.favorite_tags_api import FavoriteTagsApi
+from elabapi_python.api.idps_api import IdpsApi
 from elabapi_python.api.items_api import ItemsApi
 from elabapi_python.api.items_types_api import ItemsTypesApi
 from elabapi_python.api.links_to_experiments_api import LinksToExperimentsApi
 from elabapi_python.api.links_to_items_api import LinksToItemsApi
 from elabapi_python.api.notifications_api import NotificationsApi
 from elabapi_python.api.status_api import StatusApi
 from elabapi_python.api.steps_api import StepsApi
@@ -57,20 +58,24 @@
 from elabapi_python.models.experiments_links_subid_body import ExperimentsLinksSubidBody
 from elabapi_python.models.experiments_templates_body import ExperimentsTemplatesBody
 from elabapi_python.models.experiments_templates_id_body import ExperimentsTemplatesIdBody
 from elabapi_python.models.favtags_body import FavtagsBody
 from elabapi_python.models.id import Id
 from elabapi_python.models.id1 import Id1
 from elabapi_python.models.id2 import Id2
+from elabapi_python.models.id3 import Id3
 from elabapi_python.models.id_comments_body import IdCommentsBody
 from elabapi_python.models.id_status_body import IdStatusBody
 from elabapi_python.models.id_steps_body import IdStepsBody
 from elabapi_python.models.id_tags_body import IdTagsBody
 from elabapi_python.models.id_teamgroups_body import IdTeamgroupsBody
 from elabapi_python.models.id_uploads_body import IdUploadsBody
+from elabapi_python.models.idp import Idp
+from elabapi_python.models.idps_body import IdpsBody
+from elabapi_python.models.idps_id_body import IdpsIdBody
 from elabapi_python.models.inline_response200 import InlineResponse200
 from elabapi_python.models.inline_response2001 import InlineResponse2001
 from elabapi_python.models.inline_response2002 import InlineResponse2002
 from elabapi_python.models.inline_response2003 import InlineResponse2003
 from elabapi_python.models.item import Item
 from elabapi_python.models.items_body import ItemsBody
 from elabapi_python.models.items_id_body import ItemsIdBody
@@ -98,7 +103,8 @@
 from elabapi_python.models.unfinished_step import UnfinishedStep
 from elabapi_python.models.unfinished_steps import UnfinishedSteps
 from elabapi_python.models.upload import Upload
 from elabapi_python.models.uploads_subid_body import UploadsSubidBody
 from elabapi_python.models.users import Users
 from elabapi_python.models.users_body import UsersBody
 from elabapi_python.models.users_id_body import UsersIdBody
+from elabapi_python.models.users_teams import UsersTeams
```

### Comparing `elabapi-python-0.1.7/elabapi_python/api/__init__.py` & `elabapi-python-0.2.0/elabapi_python/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from elabapi_python.api.api_keys_api import ApiKeysApi
 from elabapi_python.api.comments_api import CommentsApi
 from elabapi_python.api.config_api import ConfigApi
 from elabapi_python.api.events_api import EventsApi
 from elabapi_python.api.experiments_api import ExperimentsApi
 from elabapi_python.api.experiments_templates_api import ExperimentsTemplatesApi
 from elabapi_python.api.favorite_tags_api import FavoriteTagsApi
+from elabapi_python.api.idps_api import IdpsApi
 from elabapi_python.api.items_api import ItemsApi
 from elabapi_python.api.items_types_api import ItemsTypesApi
 from elabapi_python.api.links_to_experiments_api import LinksToExperimentsApi
 from elabapi_python.api.links_to_items_api import LinksToItemsApi
 from elabapi_python.api.notifications_api import NotificationsApi
 from elabapi_python.api.status_api import StatusApi
 from elabapi_python.api.steps_api import StepsApi
```

### Comparing `elabapi-python-0.1.7/elabapi_python/api/api_keys_api.py` & `elabapi-python-0.2.0/elabapi_python/api/api_keys_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/api/comments_api.py` & `elabapi-python-0.2.0/elabapi_python/api/comments_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/api/config_api.py` & `elabapi-python-0.2.0/elabapi_python/api/config_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/api/events_api.py` & `elabapi-python-0.2.0/elabapi_python/api/events_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/api/experiments_api.py` & `elabapi-python-0.2.0/elabapi_python/api/experiments_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/api/experiments_templates_api.py` & `elabapi-python-0.2.0/elabapi_python/api/experiments_templates_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/api/favorite_tags_api.py` & `elabapi-python-0.2.0/elabapi_python/api/favorite_tags_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/api/items_api.py` & `elabapi-python-0.2.0/elabapi_python/api/items_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/api/items_types_api.py` & `elabapi-python-0.2.0/elabapi_python/api/items_types_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/api/links_to_experiments_api.py` & `elabapi-python-0.2.0/elabapi_python/api/links_to_experiments_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/api/links_to_items_api.py` & `elabapi-python-0.2.0/elabapi_python/api/links_to_items_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/api/notifications_api.py` & `elabapi-python-0.2.0/elabapi_python/api/notifications_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         All notifications for the user are deleted.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete_notifications(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param Id1 id: ID of the user or `me`. (required)
+        :param Id2 id: ID of the user or `me`. (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.delete_notifications_with_http_info(id, **kwargs)  # noqa: E501
@@ -60,15 +60,15 @@
         All notifications for the user are deleted.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete_notifications_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param Id1 id: ID of the user or `me`. (required)
+        :param Id2 id: ID of the user or `me`. (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['id']  # noqa: E501
         all_params.append('async_req')
@@ -132,15 +132,15 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.patch_notification(id, subid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param Id2 id: ID of the user or `me`. (required)
+        :param Id3 id: ID of the user or `me`. (required)
         :param int subid: ID of the notification. (required)
         :return: Notification
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -154,15 +154,15 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.patch_notification_with_http_info(id, subid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param Id2 id: ID of the user or `me`. (required)
+        :param Id3 id: ID of the user or `me`. (required)
         :param int subid: ID of the notification. (required)
         :return: Notification
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['id', 'subid']  # noqa: E501
@@ -233,15 +233,15 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_notification(id, subid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param Id2 id: ID of the user or `me`. (required)
+        :param Id3 id: ID of the user or `me`. (required)
         :param int subid: ID of the notification. (required)
         :return: Notification
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -255,15 +255,15 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_notification_with_http_info(id, subid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param Id2 id: ID of the user or `me`. (required)
+        :param Id3 id: ID of the user or `me`. (required)
         :param int subid: ID of the notification. (required)
         :return: Notification
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['id', 'subid']  # noqa: E501
@@ -334,15 +334,15 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_notifications(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param Id1 id: ID of the user or `me`. (required)
+        :param Id2 id: ID of the user or `me`. (required)
         :return: InlineResponse2003
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.read_notifications_with_http_info(id, **kwargs)  # noqa: E501
@@ -355,15 +355,15 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_notifications_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param Id1 id: ID of the user or `me`. (required)
+        :param Id2 id: ID of the user or `me`. (required)
         :return: InlineResponse2003
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['id']  # noqa: E501
         all_params.append('async_req')
```

### Comparing `elabapi-python-0.1.7/elabapi_python/api/status_api.py` & `elabapi-python-0.2.0/elabapi_python/api/status_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/api/steps_api.py` & `elabapi-python-0.2.0/elabapi_python/api/steps_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/api/tags_api.py` & `elabapi-python-0.2.0/elabapi_python/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/api/team_tags_api.py` & `elabapi-python-0.2.0/elabapi_python/api/team_tags_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/api/teamgroups_api.py` & `elabapi-python-0.2.0/elabapi_python/api/teamgroups_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/api/teams_api.py` & `elabapi-python-0.2.0/elabapi_python/api/teams_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.patch_team(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param int id: ID of the team. (required)
+        :param Id id: ID of the team or `current`. (required)
         :param Team body: Parameters for modifying a team.
         :return: Team
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -59,15 +59,15 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.patch_team_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param int id: ID of the team. (required)
+        :param Id id: ID of the team or `current`. (required)
         :param Team body: Parameters for modifying a team.
         :return: Team
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['id', 'body']  # noqa: E501
@@ -227,15 +227,15 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_team(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param int id: ID of the team. (required)
+        :param Id id: ID of the team or `current`. (required)
         :return: Team
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.read_team_with_http_info(id, **kwargs)  # noqa: E501
@@ -248,15 +248,15 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_team_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param int id: ID of the team. (required)
+        :param Id id: ID of the team or `current`. (required)
         :return: Team
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['id']  # noqa: E501
         all_params.append('async_req')
```

### Comparing `elabapi-python-0.1.7/elabapi_python/api/todolist_api.py` & `elabapi-python-0.2.0/elabapi_python/api/todolist_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/api/unfinished_steps_api.py` & `elabapi-python-0.2.0/elabapi_python/api/unfinished_steps_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/api/uploads_api.py` & `elabapi-python-0.2.0/elabapi_python/api/uploads_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/api/users_api.py` & `elabapi-python-0.2.0/elabapi_python/api/users_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         Note: it is possible to use \"me\" instead of the userid to access the user of the API key.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.patch_user(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param Id id: ID of the user or `me`. (required)
+        :param Id1 id: ID of the user or `me`. (required)
         :param UsersIdBody body: Parameters for modifying a user.
         :return: Users
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -61,15 +61,15 @@
         Note: it is possible to use \"me\" instead of the userid to access the user of the API key.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.patch_user_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param Id id: ID of the user or `me`. (required)
+        :param Id1 id: ID of the user or `me`. (required)
         :param UsersIdBody body: Parameters for modifying a user.
         :return: Users
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['id', 'body']  # noqa: E501
@@ -232,15 +232,15 @@
         Note: it is possible to use \"me\" instead of the userid to access the user of the API key.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_user(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param Id id: ID of the user or `me`. (required)
+        :param Id1 id: ID of the user or `me`. (required)
         :return: Users
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.read_user_with_http_info(id, **kwargs)  # noqa: E501
@@ -254,15 +254,15 @@
         Note: it is possible to use \"me\" instead of the userid to access the user of the API key.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_user_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param Id id: ID of the user or `me`. (required)
+        :param Id1 id: ID of the user or `me`. (required)
         :return: Users
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['id']  # noqa: E501
         all_params.append('async_req')
```

### Comparing `elabapi-python-0.1.7/elabapi_python/api_client.py` & `elabapi-python-0.2.0/elabapi_python/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/0.1.7/python'
+        self.user_agent = 'Swagger-Codegen/0.2.0/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `elabapi-python-0.1.7/elabapi_python/configuration.py` & `elabapi-python-0.2.0/elabapi_python/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,9 +243,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2.0.0\n"\
-               "SDK Package Version: 0.1.7".\
+               "SDK Package Version: 0.2.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `elabapi-python-0.1.7/elabapi_python/models/__init__.py` & `elabapi-python-0.2.0/elabapi_python/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,20 +30,24 @@
 from elabapi_python.models.experiments_links_subid_body import ExperimentsLinksSubidBody
 from elabapi_python.models.experiments_templates_body import ExperimentsTemplatesBody
 from elabapi_python.models.experiments_templates_id_body import ExperimentsTemplatesIdBody
 from elabapi_python.models.favtags_body import FavtagsBody
 from elabapi_python.models.id import Id
 from elabapi_python.models.id1 import Id1
 from elabapi_python.models.id2 import Id2
+from elabapi_python.models.id3 import Id3
 from elabapi_python.models.id_comments_body import IdCommentsBody
 from elabapi_python.models.id_status_body import IdStatusBody
 from elabapi_python.models.id_steps_body import IdStepsBody
 from elabapi_python.models.id_tags_body import IdTagsBody
 from elabapi_python.models.id_teamgroups_body import IdTeamgroupsBody
 from elabapi_python.models.id_uploads_body import IdUploadsBody
+from elabapi_python.models.idp import Idp
+from elabapi_python.models.idps_body import IdpsBody
+from elabapi_python.models.idps_id_body import IdpsIdBody
 from elabapi_python.models.inline_response200 import InlineResponse200
 from elabapi_python.models.inline_response2001 import InlineResponse2001
 from elabapi_python.models.inline_response2002 import InlineResponse2002
 from elabapi_python.models.inline_response2003 import InlineResponse2003
 from elabapi_python.models.item import Item
 from elabapi_python.models.items_body import ItemsBody
 from elabapi_python.models.items_id_body import ItemsIdBody
@@ -71,7 +75,8 @@
 from elabapi_python.models.unfinished_step import UnfinishedStep
 from elabapi_python.models.unfinished_steps import UnfinishedSteps
 from elabapi_python.models.upload import Upload
 from elabapi_python.models.uploads_subid_body import UploadsSubidBody
 from elabapi_python.models.users import Users
 from elabapi_python.models.users_body import UsersBody
 from elabapi_python.models.users_id_body import UsersIdBody
+from elabapi_python.models.users_teams import UsersTeams
```

### Comparing `elabapi-python-0.1.7/elabapi_python/models/apikey.py` & `elabapi-python-0.2.0/elabapi_python/models/apikey.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/apikeys_body.py` & `elabapi-python-0.2.0/elabapi_python/models/apikeys_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/comment.py` & `elabapi-python-0.2.0/elabapi_python/models/comment.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/config.py` & `elabapi-python-0.2.0/elabapi_python/models/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,17 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'admin_validate': 'str',
         'admins_create_users': 'str',
+        'admins_create_users_remote_dir': 'str',
+        'admin_validate': 'str',
         'announcement': 'str',
         'anon_users': 'str',
         'autologout_time': 'str',
         'blox_anon': 'str',
         'blox_enabled': 'str',
         'debug': 'str',
         'deletable_xp': 'str',
@@ -65,14 +66,16 @@
         'max_revisions': 'str',
         'min_days_revisions': 'str',
         'min_delta_revisions': 'str',
         'open_science': 'str',
         'open_team': 'str',
         'privacy_policy': 'str',
         'proxy': 'str',
+        'remote_dir_config': 'str',
+        'remote_dir_service': 'str',
         's3_bucket_name': 'str',
         's3_endpoint': 'str',
         's3_path_prefix': 'str',
         's3_region': 'str',
         'saml_acs_binding': 'str',
         'saml_allowrepeatattributename': 'str',
         'saml_authnrequestssigned': 'str',
@@ -116,16 +119,17 @@
         'ts_login': 'str',
         'ts_password': 'str',
         'ts_url': 'str',
         'uploads_storage': 'str'
     }
 
     attribute_map = {
-        'admin_validate': 'admin_validate',
         'admins_create_users': 'admins_create_users',
+        'admins_create_users_remote_dir': 'admins_create_users_remote_dir',
+        'admin_validate': 'admin_validate',
         'announcement': 'announcement',
         'anon_users': 'anon_users',
         'autologout_time': 'autologout_time',
         'blox_anon': 'blox_anon',
         'blox_enabled': 'blox_enabled',
         'debug': 'debug',
         'deletable_xp': 'deletable_xp',
@@ -157,14 +161,16 @@
         'max_revisions': 'max_revisions',
         'min_days_revisions': 'min_days_revisions',
         'min_delta_revisions': 'min_delta_revisions',
         'open_science': 'open_science',
         'open_team': 'open_team',
         'privacy_policy': 'privacy_policy',
         'proxy': 'proxy',
+        'remote_dir_config': 'remote_dir_config',
+        'remote_dir_service': 'remote_dir_service',
         's3_bucket_name': 's3_bucket_name',
         's3_endpoint': 's3_endpoint',
         's3_path_prefix': 's3_path_prefix',
         's3_region': 's3_region',
         'saml_acs_binding': 'saml_acs_binding',
         'saml_allowrepeatattributename': 'saml_allowrepeatattributename',
         'saml_authnrequestssigned': 'saml_authnrequestssigned',
@@ -207,18 +213,19 @@
         'ts_limit': 'ts_limit',
         'ts_login': 'ts_login',
         'ts_password': 'ts_password',
         'ts_url': 'ts_url',
         'uploads_storage': 'uploads_storage'
     }
 
-    def __init__(self, admin_validate=None, admins_create_users=None, announcement=None, anon_users=None, autologout_time=None, blox_anon=None, blox_enabled=None, debug=None, deletable_xp=None, email_domain=None, extauth_email=None, extauth_firstname=None, extauth_lastname=None, extauth_remote_user=None, extauth_teams=None, lang=None, ldap_base_dn=None, ldap_search_attr=None, ldap_email=None, ldap_firstname=None, ldap_host=None, ldap_lastname=None, ldap_password=None, ldap_port=None, ldap_team=None, ldap_toggle=None, ldap_use_tls=None, ldap_username=None, local_login=None, local_register=None, login_announcement=None, login_tries=None, logout_url=None, mail_from=None, max_revisions=None, min_days_revisions=None, min_delta_revisions=None, open_science=None, open_team=None, privacy_policy=None, proxy=None, s3_bucket_name=None, s3_endpoint=None, s3_path_prefix=None, s3_region=None, saml_acs_binding=None, saml_allowrepeatattributename=None, saml_authnrequestssigned=None, saml_baseurl=None, saml_debug=None, saml_entityid=None, saml_logoutrequestsigned=None, saml_logoutresponsesigned=None, saml_lowercaseurlencoding=None, saml_nameidencrypted=None, saml_nameidformat=None, saml_privatekey=None, saml_relaxdestinationvalidation=None, saml_signmetadata=None, saml_slo_binding=None, saml_strict=None, saml_sync_teams=None, saml_team_create=None, saml_team_default=None, saml_toggle=None, saml_user_default=None, saml_wantassertionsencrypted=None, saml_wantassertionssigned=None, saml_wantmessagessigned=None, saml_wantnameid=None, saml_wantnameidencrypted=None, saml_wantxmlvalidation=None, saml_x509=None, saml_x509_new=None, schema=None, smtp_address=None, smtp_encryption=None, smtp_password=None, smtp_port=None, smtp_username=None, support_url=None, ts_authority=None, ts_cert=None, ts_hash=None, ts_limit=None, ts_login=None, ts_password=None, ts_url=None, uploads_storage=None):  # noqa: E501
+    def __init__(self, admins_create_users=None, admins_create_users_remote_dir=None, admin_validate=None, announcement=None, anon_users=None, autologout_time=None, blox_anon=None, blox_enabled=None, debug=None, deletable_xp=None, email_domain=None, extauth_email=None, extauth_firstname=None, extauth_lastname=None, extauth_remote_user=None, extauth_teams=None, lang=None, ldap_base_dn=None, ldap_search_attr=None, ldap_email=None, ldap_firstname=None, ldap_host=None, ldap_lastname=None, ldap_password=None, ldap_port=None, ldap_team=None, ldap_toggle=None, ldap_use_tls=None, ldap_username=None, local_login=None, local_register=None, login_announcement=None, login_tries=None, logout_url=None, mail_from=None, max_revisions=None, min_days_revisions=None, min_delta_revisions=None, open_science=None, open_team=None, privacy_policy=None, proxy=None, remote_dir_config=None, remote_dir_service=None, s3_bucket_name=None, s3_endpoint=None, s3_path_prefix=None, s3_region=None, saml_acs_binding=None, saml_allowrepeatattributename=None, saml_authnrequestssigned=None, saml_baseurl=None, saml_debug=None, saml_entityid=None, saml_logoutrequestsigned=None, saml_logoutresponsesigned=None, saml_lowercaseurlencoding=None, saml_nameidencrypted=None, saml_nameidformat=None, saml_privatekey=None, saml_relaxdestinationvalidation=None, saml_signmetadata=None, saml_slo_binding=None, saml_strict=None, saml_sync_teams=None, saml_team_create=None, saml_team_default=None, saml_toggle=None, saml_user_default=None, saml_wantassertionsencrypted=None, saml_wantassertionssigned=None, saml_wantmessagessigned=None, saml_wantnameid=None, saml_wantnameidencrypted=None, saml_wantxmlvalidation=None, saml_x509=None, saml_x509_new=None, schema=None, smtp_address=None, smtp_encryption=None, smtp_password=None, smtp_port=None, smtp_username=None, support_url=None, ts_authority=None, ts_cert=None, ts_hash=None, ts_limit=None, ts_login=None, ts_password=None, ts_url=None, uploads_storage=None):  # noqa: E501
         """Config - a model defined in Swagger"""  # noqa: E501
-        self._admin_validate = None
         self._admins_create_users = None
+        self._admins_create_users_remote_dir = None
+        self._admin_validate = None
         self._announcement = None
         self._anon_users = None
         self._autologout_time = None
         self._blox_anon = None
         self._blox_enabled = None
         self._debug = None
         self._deletable_xp = None
@@ -250,14 +257,16 @@
         self._max_revisions = None
         self._min_days_revisions = None
         self._min_delta_revisions = None
         self._open_science = None
         self._open_team = None
         self._privacy_policy = None
         self._proxy = None
+        self._remote_dir_config = None
+        self._remote_dir_service = None
         self._s3_bucket_name = None
         self._s3_endpoint = None
         self._s3_path_prefix = None
         self._s3_region = None
         self._saml_acs_binding = None
         self._saml_allowrepeatattributename = None
         self._saml_authnrequestssigned = None
@@ -299,18 +308,20 @@
         self._ts_hash = None
         self._ts_limit = None
         self._ts_login = None
         self._ts_password = None
         self._ts_url = None
         self._uploads_storage = None
         self.discriminator = None
-        if admin_validate is not None:
-            self.admin_validate = admin_validate
         if admins_create_users is not None:
             self.admins_create_users = admins_create_users
+        if admins_create_users_remote_dir is not None:
+            self.admins_create_users_remote_dir = admins_create_users_remote_dir
+        if admin_validate is not None:
+            self.admin_validate = admin_validate
         if announcement is not None:
             self.announcement = announcement
         if anon_users is not None:
             self.anon_users = anon_users
         if autologout_time is not None:
             self.autologout_time = autologout_time
         if blox_anon is not None:
@@ -381,14 +392,18 @@
             self.open_science = open_science
         if open_team is not None:
             self.open_team = open_team
         if privacy_policy is not None:
             self.privacy_policy = privacy_policy
         if proxy is not None:
             self.proxy = proxy
+        if remote_dir_config is not None:
+            self.remote_dir_config = remote_dir_config
+        if remote_dir_service is not None:
+            self.remote_dir_service = remote_dir_service
         if s3_bucket_name is not None:
             self.s3_bucket_name = s3_bucket_name
         if s3_endpoint is not None:
             self.s3_endpoint = s3_endpoint
         if s3_path_prefix is not None:
             self.s3_path_prefix = s3_path_prefix
         if s3_region is not None:
@@ -479,54 +494,75 @@
             self.ts_password = ts_password
         if ts_url is not None:
             self.ts_url = ts_url
         if uploads_storage is not None:
             self.uploads_storage = uploads_storage
 
     @property
-    def admin_validate(self):
-        """Gets the admin_validate of this Config.  # noqa: E501
+    def admins_create_users(self):
+        """Gets the admins_create_users of this Config.  # noqa: E501
 
 
-        :return: The admin_validate of this Config.  # noqa: E501
+        :return: The admins_create_users of this Config.  # noqa: E501
         :rtype: str
         """
-        return self._admin_validate
+        return self._admins_create_users
 
-    @admin_validate.setter
-    def admin_validate(self, admin_validate):
-        """Sets the admin_validate of this Config.
+    @admins_create_users.setter
+    def admins_create_users(self, admins_create_users):
+        """Sets the admins_create_users of this Config.
 
 
-        :param admin_validate: The admin_validate of this Config.  # noqa: E501
+        :param admins_create_users: The admins_create_users of this Config.  # noqa: E501
         :type: str
         """
 
-        self._admin_validate = admin_validate
+        self._admins_create_users = admins_create_users
 
     @property
-    def admins_create_users(self):
-        """Gets the admins_create_users of this Config.  # noqa: E501
+    def admins_create_users_remote_dir(self):
+        """Gets the admins_create_users_remote_dir of this Config.  # noqa: E501
 
 
-        :return: The admins_create_users of this Config.  # noqa: E501
+        :return: The admins_create_users_remote_dir of this Config.  # noqa: E501
         :rtype: str
         """
-        return self._admins_create_users
+        return self._admins_create_users_remote_dir
 
-    @admins_create_users.setter
-    def admins_create_users(self, admins_create_users):
-        """Sets the admins_create_users of this Config.
+    @admins_create_users_remote_dir.setter
+    def admins_create_users_remote_dir(self, admins_create_users_remote_dir):
+        """Sets the admins_create_users_remote_dir of this Config.
 
 
-        :param admins_create_users: The admins_create_users of this Config.  # noqa: E501
+        :param admins_create_users_remote_dir: The admins_create_users_remote_dir of this Config.  # noqa: E501
         :type: str
         """
 
-        self._admins_create_users = admins_create_users
+        self._admins_create_users_remote_dir = admins_create_users_remote_dir
+
+    @property
+    def admin_validate(self):
+        """Gets the admin_validate of this Config.  # noqa: E501
+
+
+        :return: The admin_validate of this Config.  # noqa: E501
+        :rtype: str
+        """
+        return self._admin_validate
+
+    @admin_validate.setter
+    def admin_validate(self, admin_validate):
+        """Sets the admin_validate of this Config.
+
+
+        :param admin_validate: The admin_validate of this Config.  # noqa: E501
+        :type: str
+        """
+
+        self._admin_validate = admin_validate
 
     @property
     def announcement(self):
         """Gets the announcement of this Config.  # noqa: E501
 
 
         :return: The announcement of this Config.  # noqa: E501
@@ -1340,14 +1376,56 @@
         :param proxy: The proxy of this Config.  # noqa: E501
         :type: str
         """
 
         self._proxy = proxy
 
     @property
+    def remote_dir_config(self):
+        """Gets the remote_dir_config of this Config.  # noqa: E501
+
+
+        :return: The remote_dir_config of this Config.  # noqa: E501
+        :rtype: str
+        """
+        return self._remote_dir_config
+
+    @remote_dir_config.setter
+    def remote_dir_config(self, remote_dir_config):
+        """Sets the remote_dir_config of this Config.
+
+
+        :param remote_dir_config: The remote_dir_config of this Config.  # noqa: E501
+        :type: str
+        """
+
+        self._remote_dir_config = remote_dir_config
+
+    @property
+    def remote_dir_service(self):
+        """Gets the remote_dir_service of this Config.  # noqa: E501
+
+
+        :return: The remote_dir_service of this Config.  # noqa: E501
+        :rtype: str
+        """
+        return self._remote_dir_service
+
+    @remote_dir_service.setter
+    def remote_dir_service(self, remote_dir_service):
+        """Sets the remote_dir_service of this Config.
+
+
+        :param remote_dir_service: The remote_dir_service of this Config.  # noqa: E501
+        :type: str
+        """
+
+        self._remote_dir_service = remote_dir_service
+
+    @property
     def s3_bucket_name(self):
         """Gets the s3_bucket_name of this Config.  # noqa: E501
 
 
         :return: The s3_bucket_name of this Config.  # noqa: E501
         :rtype: str
         """
```

### Comparing `elabapi-python-0.1.7/elabapi_python/models/entity.py` & `elabapi-python-0.2.0/elabapi_python/models/entity.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/event.py` & `elabapi-python-0.2.0/elabapi_python/models/event.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/events_id_body.py` & `elabapi-python-0.2.0/elabapi_python/models/events_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/events_id_body1.py` & `elabapi-python-0.2.0/elabapi_python/models/events_id_body1.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/eventsid_delta.py` & `elabapi-python-0.2.0/elabapi_python/models/eventsid_delta.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/experiment.py` & `elabapi-python-0.2.0/elabapi_python/models/experiment.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/experiment_template.py` & `elabapi-python-0.2.0/elabapi_python/models/experiment_template.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/experiments_body.py` & `elabapi-python-0.2.0/elabapi_python/models/experiments_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/experiments_id_body.py` & `elabapi-python-0.2.0/elabapi_python/models/experiments_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/experiments_links_subid_body.py` & `elabapi-python-0.2.0/elabapi_python/models/experiments_links_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/experiments_templates_body.py` & `elabapi-python-0.2.0/elabapi_python/models/experiments_templates_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/experiments_templates_id_body.py` & `elabapi-python-0.2.0/elabapi_python/models/experiments_templates_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/favtags_body.py` & `elabapi-python-0.2.0/elabapi_python/models/favtags_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/id.py` & `elabapi-python-0.2.0/elabapi_python/models/id.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/id1.py` & `elabapi-python-0.2.0/elabapi_python/models/id1.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/id2.py` & `elabapi-python-0.2.0/elabapi_python/models/id2.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/id_comments_body.py` & `elabapi-python-0.2.0/elabapi_python/models/id_comments_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/id_status_body.py` & `elabapi-python-0.2.0/elabapi_python/models/id_status_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/id_steps_body.py` & `elabapi-python-0.2.0/elabapi_python/models/id_steps_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/id_tags_body.py` & `elabapi-python-0.2.0/elabapi_python/models/id_tags_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/id_teamgroups_body.py` & `elabapi-python-0.2.0/elabapi_python/models/id_teamgroups_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/id_uploads_body.py` & `elabapi-python-0.2.0/elabapi_python/models/id_uploads_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/inline_response200.py` & `elabapi-python-0.2.0/elabapi_python/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/inline_response2001.py` & `elabapi-python-0.2.0/elabapi_python/models/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/inline_response2002.py` & `elabapi-python-0.2.0/elabapi_python/models/inline_response2002.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/inline_response2003.py` & `elabapi-python-0.2.0/elabapi_python/models/inline_response2003.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/item.py` & `elabapi-python-0.2.0/elabapi_python/models/item.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/items_body.py` & `elabapi-python-0.2.0/elabapi_python/models/items_body.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,40 +33,40 @@
     }
 
     attribute_map = {
         'category_id': 'category_id',
         'tags': 'tags'
     }
 
-    def __init__(self, category_id=-1, tags=None):  # noqa: E501
+    def __init__(self, category_id=None, tags=None):  # noqa: E501
         """ItemsBody - a model defined in Swagger"""  # noqa: E501
         self._category_id = None
         self._tags = None
         self.discriminator = None
         if category_id is not None:
             self.category_id = category_id
         if tags is not None:
             self.tags = tags
 
     @property
     def category_id(self):
         """Gets the category_id of this ItemsBody.  # noqa: E501
 
-        The template id to use, or 0 to use the common team template, or -1 to have an empty body.  # noqa: E501
+        Mandatory parameter, an ID corresponding to an items_types in the team.   # noqa: E501
 
         :return: The category_id of this ItemsBody.  # noqa: E501
         :rtype: int
         """
         return self._category_id
 
     @category_id.setter
     def category_id(self, category_id):
         """Sets the category_id of this ItemsBody.
 
-        The template id to use, or 0 to use the common team template, or -1 to have an empty body.  # noqa: E501
+        Mandatory parameter, an ID corresponding to an items_types in the team.   # noqa: E501
 
         :param category_id: The category_id of this ItemsBody.  # noqa: E501
         :type: int
         """
 
         self._category_id = category_id
```

### Comparing `elabapi-python-0.1.7/elabapi_python/models/items_id_body.py` & `elabapi-python-0.2.0/elabapi_python/models/items_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/items_links_subid_body.py` & `elabapi-python-0.2.0/elabapi_python/models/items_links_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/items_type.py` & `elabapi-python-0.2.0/elabapi_python/models/items_type.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/items_types_body.py` & `elabapi-python-0.2.0/elabapi_python/models/items_types_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/link.py` & `elabapi-python-0.2.0/elabapi_python/models/link.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/notification.py` & `elabapi-python-0.2.0/elabapi_python/models/notification.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/status.py` & `elabapi-python-0.2.0/elabapi_python/models/status.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/step.py` & `elabapi-python-0.2.0/elabapi_python/models/step.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/steps_subid_body.py` & `elabapi-python-0.2.0/elabapi_python/models/steps_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/tag.py` & `elabapi-python-0.2.0/elabapi_python/models/tag.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/tags_subid_body.py` & `elabapi-python-0.2.0/elabapi_python/models/tags_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/team.py` & `elabapi-python-0.2.0/elabapi_python/models/team.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/team_tags_body.py` & `elabapi-python-0.2.0/elabapi_python/models/team_tags_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/team_tags_body1.py` & `elabapi-python-0.2.0/elabapi_python/models/team_tags_body1.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/team_tags_id_body.py` & `elabapi-python-0.2.0/elabapi_python/models/team_tags_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/teamgroup.py` & `elabapi-python-0.2.0/elabapi_python/models/teamgroup.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/teamgroup_users.py` & `elabapi-python-0.2.0/elabapi_python/models/teamgroup_users.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/teamgroups_subid_body.py` & `elabapi-python-0.2.0/elabapi_python/models/teamgroups_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/teams_body.py` & `elabapi-python-0.2.0/elabapi_python/models/teams_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/todoitem.py` & `elabapi-python-0.2.0/elabapi_python/models/todoitem.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/todolist_body.py` & `elabapi-python-0.2.0/elabapi_python/models/todolist_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/todolist_id_body.py` & `elabapi-python-0.2.0/elabapi_python/models/todolist_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/unfinished_step.py` & `elabapi-python-0.2.0/elabapi_python/models/unfinished_step.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/unfinished_steps.py` & `elabapi-python-0.2.0/elabapi_python/models/unfinished_steps.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/upload.py` & `elabapi-python-0.2.0/elabapi_python/models/upload.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/uploads_subid_body.py` & `elabapi-python-0.2.0/elabapi_python/models/uploads_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/models/users.py` & `elabapi-python-0.2.0/elabapi_python/models/users.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,72 +29,82 @@
     """
     swagger_types = {
         'userid': 'int',
         'firstname': 'str',
         'lastname': 'str',
         'email': 'str',
         'validated': 'int',
-        'usergroup': 'int',
         'archived': 'int',
         'last_login': 'str',
         'fullname': 'str',
         'orcid': 'str',
-        'auth_service': 'int'
+        'orgid': 'str',
+        'auth_service': 'int',
+        'is_sysadmin': 'int',
+        'teams': 'list[UsersTeams]'
     }
 
     attribute_map = {
         'userid': 'userid',
         'firstname': 'firstname',
         'lastname': 'lastname',
         'email': 'email',
         'validated': 'validated',
-        'usergroup': 'usergroup',
         'archived': 'archived',
         'last_login': 'last_login',
         'fullname': 'fullname',
         'orcid': 'orcid',
-        'auth_service': 'auth_service'
+        'orgid': 'orgid',
+        'auth_service': 'auth_service',
+        'is_sysadmin': 'is_sysadmin',
+        'teams': 'teams'
     }
 
-    def __init__(self, userid=None, firstname=None, lastname=None, email=None, validated=None, usergroup=None, archived=None, last_login=None, fullname=None, orcid=None, auth_service=None):  # noqa: E501
+    def __init__(self, userid=None, firstname=None, lastname=None, email=None, validated=None, archived=None, last_login=None, fullname=None, orcid=None, orgid=None, auth_service=None, is_sysadmin=None, teams=None):  # noqa: E501
         """Users - a model defined in Swagger"""  # noqa: E501
         self._userid = None
         self._firstname = None
         self._lastname = None
         self._email = None
         self._validated = None
-        self._usergroup = None
         self._archived = None
         self._last_login = None
         self._fullname = None
         self._orcid = None
+        self._orgid = None
         self._auth_service = None
+        self._is_sysadmin = None
+        self._teams = None
         self.discriminator = None
         if userid is not None:
             self.userid = userid
         if firstname is not None:
             self.firstname = firstname
         if lastname is not None:
             self.lastname = lastname
         if email is not None:
             self.email = email
         if validated is not None:
             self.validated = validated
-        if usergroup is not None:
-            self.usergroup = usergroup
         if archived is not None:
             self.archived = archived
         if last_login is not None:
             self.last_login = last_login
         if fullname is not None:
             self.fullname = fullname
         if orcid is not None:
             self.orcid = orcid
+        if orgid is not None:
+            self.orgid = orgid
         if auth_service is not None:
             self.auth_service = auth_service
+        if is_sysadmin is not None:
+            self.is_sysadmin = is_sysadmin
+        if teams is not None:
+            self.teams = teams
 
     @property
     def userid(self):
         """Gets the userid of this Users.  # noqa: E501
 
 
         :return: The userid of this Users.  # noqa: E501
@@ -194,35 +204,14 @@
         :param validated: The validated of this Users.  # noqa: E501
         :type: int
         """
 
         self._validated = validated
 
     @property
-    def usergroup(self):
-        """Gets the usergroup of this Users.  # noqa: E501
-
-
-        :return: The usergroup of this Users.  # noqa: E501
-        :rtype: int
-        """
-        return self._usergroup
-
-    @usergroup.setter
-    def usergroup(self, usergroup):
-        """Sets the usergroup of this Users.
-
-
-        :param usergroup: The usergroup of this Users.  # noqa: E501
-        :type: int
-        """
-
-        self._usergroup = usergroup
-
-    @property
     def archived(self):
         """Gets the archived of this Users.  # noqa: E501
 
 
         :return: The archived of this Users.  # noqa: E501
         :rtype: int
         """
@@ -299,14 +288,35 @@
         :param orcid: The orcid of this Users.  # noqa: E501
         :type: str
         """
 
         self._orcid = orcid
 
     @property
+    def orgid(self):
+        """Gets the orgid of this Users.  # noqa: E501
+
+
+        :return: The orgid of this Users.  # noqa: E501
+        :rtype: str
+        """
+        return self._orgid
+
+    @orgid.setter
+    def orgid(self, orgid):
+        """Sets the orgid of this Users.
+
+
+        :param orgid: The orgid of this Users.  # noqa: E501
+        :type: str
+        """
+
+        self._orgid = orgid
+
+    @property
     def auth_service(self):
         """Gets the auth_service of this Users.  # noqa: E501
 
 
         :return: The auth_service of this Users.  # noqa: E501
         :rtype: int
         """
@@ -319,14 +329,56 @@
 
         :param auth_service: The auth_service of this Users.  # noqa: E501
         :type: int
         """
 
         self._auth_service = auth_service
 
+    @property
+    def is_sysadmin(self):
+        """Gets the is_sysadmin of this Users.  # noqa: E501
+
+
+        :return: The is_sysadmin of this Users.  # noqa: E501
+        :rtype: int
+        """
+        return self._is_sysadmin
+
+    @is_sysadmin.setter
+    def is_sysadmin(self, is_sysadmin):
+        """Sets the is_sysadmin of this Users.
+
+
+        :param is_sysadmin: The is_sysadmin of this Users.  # noqa: E501
+        :type: int
+        """
+
+        self._is_sysadmin = is_sysadmin
+
+    @property
+    def teams(self):
+        """Gets the teams of this Users.  # noqa: E501
+
+
+        :return: The teams of this Users.  # noqa: E501
+        :rtype: list[UsersTeams]
+        """
+        return self._teams
+
+    @teams.setter
+    def teams(self, teams):
+        """Sets the teams of this Users.
+
+
+        :param teams: The teams of this Users.  # noqa: E501
+        :type: list[UsersTeams]
+        """
+
+        self._teams = teams
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `elabapi-python-0.1.7/elabapi_python/models/users_body.py` & `elabapi-python-0.2.0/elabapi_python/models/users_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,46 +27,46 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'firstname': 'str',
         'lastname': 'str',
         'email': 'str',
-        'usergroup': 'str',
         'team': 'int',
-        'valid_until': 'str'
+        'valid_until': 'str',
+        'orgid': 'str'
     }
 
     attribute_map = {
         'firstname': 'firstname',
         'lastname': 'lastname',
         'email': 'email',
-        'usergroup': 'usergroup',
         'team': 'team',
-        'valid_until': 'valid_until'
+        'valid_until': 'valid_until',
+        'orgid': 'orgid'
     }
 
-    def __init__(self, firstname=None, lastname=None, email=None, usergroup=None, team=None, valid_until=None):  # noqa: E501
+    def __init__(self, firstname=None, lastname=None, email=None, team=None, valid_until=None, orgid=None):  # noqa: E501
         """UsersBody - a model defined in Swagger"""  # noqa: E501
         self._firstname = None
         self._lastname = None
         self._email = None
-        self._usergroup = None
         self._team = None
         self._valid_until = None
+        self._orgid = None
         self.discriminator = None
         self.firstname = firstname
         self.lastname = lastname
         self.email = email
-        if usergroup is not None:
-            self.usergroup = usergroup
         if team is not None:
             self.team = team
         if valid_until is not None:
             self.valid_until = valid_until
+        if orgid is not None:
+            self.orgid = orgid
 
     @property
     def firstname(self):
         """Gets the firstname of this UsersBody.  # noqa: E501
 
         User's first name.  # noqa: E501
 
@@ -136,43 +136,14 @@
         """
         if email is None:
             raise ValueError("Invalid value for `email`, must not be `None`")  # noqa: E501
 
         self._email = email
 
     @property
-    def usergroup(self):
-        """Gets the usergroup of this UsersBody.  # noqa: E501
-
-        1: Sysadmin, 2: Admin, 4: regular user.   # noqa: E501
-
-        :return: The usergroup of this UsersBody.  # noqa: E501
-        :rtype: str
-        """
-        return self._usergroup
-
-    @usergroup.setter
-    def usergroup(self, usergroup):
-        """Sets the usergroup of this UsersBody.
-
-        1: Sysadmin, 2: Admin, 4: regular user.   # noqa: E501
-
-        :param usergroup: The usergroup of this UsersBody.  # noqa: E501
-        :type: str
-        """
-        allowed_values = ["1", "2", "4"]  # noqa: E501
-        if usergroup not in allowed_values:
-            raise ValueError(
-                "Invalid value for `usergroup` ({0}), must be one of {1}"  # noqa: E501
-                .format(usergroup, allowed_values)
-            )
-
-        self._usergroup = usergroup
-
-    @property
     def team(self):
         """Gets the team of this UsersBody.  # noqa: E501
 
         The team id.  # noqa: E501
 
         :return: The team of this UsersBody.  # noqa: E501
         :rtype: int
@@ -210,14 +181,37 @@
 
         :param valid_until: The valid_until of this UsersBody.  # noqa: E501
         :type: str
         """
 
         self._valid_until = valid_until
 
+    @property
+    def orgid(self):
+        """Gets the orgid of this UsersBody.  # noqa: E501
+
+        Internal id.  # noqa: E501
+
+        :return: The orgid of this UsersBody.  # noqa: E501
+        :rtype: str
+        """
+        return self._orgid
+
+    @orgid.setter
+    def orgid(self, orgid):
+        """Sets the orgid of this UsersBody.
+
+        Internal id.  # noqa: E501
+
+        :param orgid: The orgid of this UsersBody.  # noqa: E501
+        :type: str
+        """
+
+        self._orgid = orgid
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `elabapi-python-0.1.7/elabapi_python/models/users_id_body.py` & `elabapi-python-0.2.0/elabapi_python/models/users_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python/rest.py` & `elabapi-python-0.2.0/elabapi_python/rest.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/elabapi_python.egg-info/SOURCES.txt` & `elabapi-python-0.2.0/elabapi_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 elabapi_python/api/api_keys_api.py
 elabapi_python/api/comments_api.py
 elabapi_python/api/config_api.py
 elabapi_python/api/events_api.py
 elabapi_python/api/experiments_api.py
 elabapi_python/api/experiments_templates_api.py
 elabapi_python/api/favorite_tags_api.py
+elabapi_python/api/idps_api.py
 elabapi_python/api/items_api.py
 elabapi_python/api/items_types_api.py
 elabapi_python/api/links_to_experiments_api.py
 elabapi_python/api/links_to_items_api.py
 elabapi_python/api/notifications_api.py
 elabapi_python/api/status_api.py
 elabapi_python/api/steps_api.py
@@ -49,20 +50,24 @@
 elabapi_python/models/experiments_links_subid_body.py
 elabapi_python/models/experiments_templates_body.py
 elabapi_python/models/experiments_templates_id_body.py
 elabapi_python/models/favtags_body.py
 elabapi_python/models/id.py
 elabapi_python/models/id1.py
 elabapi_python/models/id2.py
+elabapi_python/models/id3.py
 elabapi_python/models/id_comments_body.py
 elabapi_python/models/id_status_body.py
 elabapi_python/models/id_steps_body.py
 elabapi_python/models/id_tags_body.py
 elabapi_python/models/id_teamgroups_body.py
 elabapi_python/models/id_uploads_body.py
+elabapi_python/models/idp.py
+elabapi_python/models/idps_body.py
+elabapi_python/models/idps_id_body.py
 elabapi_python/models/inline_response200.py
 elabapi_python/models/inline_response2001.py
 elabapi_python/models/inline_response2002.py
 elabapi_python/models/inline_response2003.py
 elabapi_python/models/item.py
 elabapi_python/models/items_body.py
 elabapi_python/models/items_id_body.py
@@ -90,14 +95,15 @@
 elabapi_python/models/unfinished_step.py
 elabapi_python/models/unfinished_steps.py
 elabapi_python/models/upload.py
 elabapi_python/models/uploads_subid_body.py
 elabapi_python/models/users.py
 elabapi_python/models/users_body.py
 elabapi_python/models/users_id_body.py
+elabapi_python/models/users_teams.py
 test/__init__.py
 test/test_api_keys_api.py
 test/test_apikey.py
 test/test_apikeys_body.py
 test/test_comment.py
 test/test_comments_api.py
 test/test_config.py
@@ -118,20 +124,25 @@
 test/test_experiments_templates_body.py
 test/test_experiments_templates_id_body.py
 test/test_favorite_tags_api.py
 test/test_favtags_body.py
 test/test_id.py
 test/test_id1.py
 test/test_id2.py
+test/test_id3.py
 test/test_id_comments_body.py
 test/test_id_status_body.py
 test/test_id_steps_body.py
 test/test_id_tags_body.py
 test/test_id_teamgroups_body.py
 test/test_id_uploads_body.py
+test/test_idp.py
+test/test_idps_api.py
+test/test_idps_body.py
+test/test_idps_id_body.py
 test/test_inline_response200.py
 test/test_inline_response2001.py
 test/test_inline_response2002.py
 test/test_inline_response2003.py
 test/test_item.py
 test/test_items_api.py
 test/test_items_body.py
@@ -173,8 +184,9 @@
 test/test_unfinished_steps_api.py
 test/test_upload.py
 test/test_uploads_api.py
 test/test_uploads_subid_body.py
 test/test_users.py
 test/test_users_api.py
 test/test_users_body.py
-test/test_users_id_body.py
+test/test_users_id_body.py
+test/test_users_teams.py
```

### Comparing `elabapi-python-0.1.7/setup.py` & `elabapi-python-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "elabapi-python"
-VERSION = "0.1.7"
+VERSION = "0.2.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `elabapi-python-0.1.7/test/test_api_keys_api.py` & `elabapi-python-0.2.0/test/test_api_keys_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_apikey.py` & `elabapi-python-0.2.0/test/test_apikey.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_apikeys_body.py` & `elabapi-python-0.2.0/test/test_apikeys_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_comment.py` & `elabapi-python-0.2.0/test/test_comment.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_comments_api.py` & `elabapi-python-0.2.0/test/test_comments_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_config.py` & `elabapi-python-0.2.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_config_api.py` & `elabapi-python-0.2.0/test/test_config_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_entity.py` & `elabapi-python-0.2.0/test/test_entity.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_event.py` & `elabapi-python-0.2.0/test/test_event.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_events_api.py` & `elabapi-python-0.2.0/test/test_events_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_events_id_body.py` & `elabapi-python-0.2.0/test/test_events_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_events_id_body1.py` & `elabapi-python-0.2.0/test/test_events_id_body1.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_eventsid_delta.py` & `elabapi-python-0.2.0/test/test_eventsid_delta.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_experiment.py` & `elabapi-python-0.2.0/test/test_experiment.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_experiment_template.py` & `elabapi-python-0.2.0/test/test_experiment_template.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_experiments_api.py` & `elabapi-python-0.2.0/test/test_experiments_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_experiments_body.py` & `elabapi-python-0.2.0/test/test_experiments_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_experiments_id_body.py` & `elabapi-python-0.2.0/test/test_experiments_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_experiments_links_subid_body.py` & `elabapi-python-0.2.0/test/test_experiments_links_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_experiments_templates_api.py` & `elabapi-python-0.2.0/test/test_experiments_templates_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_experiments_templates_body.py` & `elabapi-python-0.2.0/test/test_experiments_templates_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_experiments_templates_id_body.py` & `elabapi-python-0.2.0/test/test_experiments_templates_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_favorite_tags_api.py` & `elabapi-python-0.2.0/test/test_favorite_tags_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_favtags_body.py` & `elabapi-python-0.2.0/test/test_favtags_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_id.py` & `elabapi-python-0.2.0/test/test_id.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_id1.py` & `elabapi-python-0.2.0/test/test_id1.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_id2.py` & `elabapi-python-0.2.0/test/test_id2.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_id_comments_body.py` & `elabapi-python-0.2.0/test/test_id_comments_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_id_status_body.py` & `elabapi-python-0.2.0/test/test_id_status_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_id_steps_body.py` & `elabapi-python-0.2.0/test/test_id_steps_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_id_tags_body.py` & `elabapi-python-0.2.0/test/test_id_tags_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_id_teamgroups_body.py` & `elabapi-python-0.2.0/test/test_id_teamgroups_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_id_uploads_body.py` & `elabapi-python-0.2.0/test/test_id_uploads_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_inline_response200.py` & `elabapi-python-0.2.0/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_inline_response2001.py` & `elabapi-python-0.2.0/test/test_inline_response2001.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_inline_response2002.py` & `elabapi-python-0.2.0/test/test_inline_response2002.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_inline_response2003.py` & `elabapi-python-0.2.0/test/test_inline_response2003.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_item.py` & `elabapi-python-0.2.0/test/test_item.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_items_api.py` & `elabapi-python-0.2.0/test/test_items_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_items_body.py` & `elabapi-python-0.2.0/test/test_items_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_items_id_body.py` & `elabapi-python-0.2.0/test/test_items_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_items_links_subid_body.py` & `elabapi-python-0.2.0/test/test_items_links_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_items_type.py` & `elabapi-python-0.2.0/test/test_items_type.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_items_types_api.py` & `elabapi-python-0.2.0/test/test_items_types_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_items_types_body.py` & `elabapi-python-0.2.0/test/test_items_types_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_link.py` & `elabapi-python-0.2.0/test/test_link.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_links_to_experiments_api.py` & `elabapi-python-0.2.0/test/test_links_to_experiments_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_links_to_items_api.py` & `elabapi-python-0.2.0/test/test_links_to_items_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_notification.py` & `elabapi-python-0.2.0/test/test_notification.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_notifications_api.py` & `elabapi-python-0.2.0/test/test_notifications_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_status.py` & `elabapi-python-0.2.0/test/test_status.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_status_api.py` & `elabapi-python-0.2.0/test/test_status_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_step.py` & `elabapi-python-0.2.0/test/test_step.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_steps_api.py` & `elabapi-python-0.2.0/test/test_steps_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_steps_subid_body.py` & `elabapi-python-0.2.0/test/test_steps_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_tag.py` & `elabapi-python-0.2.0/test/test_tag.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_tags_api.py` & `elabapi-python-0.2.0/test/test_tags_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_tags_subid_body.py` & `elabapi-python-0.2.0/test/test_tags_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_team.py` & `elabapi-python-0.2.0/test/test_team.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_team_tags_api.py` & `elabapi-python-0.2.0/test/test_team_tags_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_team_tags_body.py` & `elabapi-python-0.2.0/test/test_team_tags_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_team_tags_body1.py` & `elabapi-python-0.2.0/test/test_team_tags_body1.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_team_tags_id_body.py` & `elabapi-python-0.2.0/test/test_team_tags_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_teamgroup.py` & `elabapi-python-0.2.0/test/test_teamgroup.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_teamgroup_users.py` & `elabapi-python-0.2.0/test/test_teamgroup_users.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_teamgroups_api.py` & `elabapi-python-0.2.0/test/test_teamgroups_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_teamgroups_subid_body.py` & `elabapi-python-0.2.0/test/test_teamgroups_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_teams_api.py` & `elabapi-python-0.2.0/test/test_teams_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_teams_body.py` & `elabapi-python-0.2.0/test/test_teams_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_todoitem.py` & `elabapi-python-0.2.0/test/test_todoitem.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_todolist_api.py` & `elabapi-python-0.2.0/test/test_todolist_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_todolist_body.py` & `elabapi-python-0.2.0/test/test_todolist_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_todolist_id_body.py` & `elabapi-python-0.2.0/test/test_todolist_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_unfinished_step.py` & `elabapi-python-0.2.0/test/test_unfinished_step.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_unfinished_steps.py` & `elabapi-python-0.2.0/test/test_unfinished_steps.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_unfinished_steps_api.py` & `elabapi-python-0.2.0/test/test_unfinished_steps_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_upload.py` & `elabapi-python-0.2.0/test/test_upload.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_uploads_api.py` & `elabapi-python-0.2.0/test/test_uploads_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_uploads_subid_body.py` & `elabapi-python-0.2.0/test/test_uploads_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_users.py` & `elabapi-python-0.2.0/test/test_users.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_users_api.py` & `elabapi-python-0.2.0/test/test_users_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_users_body.py` & `elabapi-python-0.2.0/test/test_users_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.1.7/test/test_users_id_body.py` & `elabapi-python-0.2.0/test/test_users_id_body.py`

 * *Files identical despite different names*


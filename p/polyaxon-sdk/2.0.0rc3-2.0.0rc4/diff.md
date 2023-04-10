# Comparing `tmp/polyaxon-sdk-2.0.0rc3.tar.gz` & `tmp/polyaxon-sdk-2.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyaxon-sdk-2.0.0rc3.tar", last modified: Mon Apr 10 12:17:42 2023, max compression
+gzip compressed data, was "polyaxon-sdk-2.0.0rc4.tar", last modified: Mon Apr 10 20:44:35 2023, max compression
```

## Comparing `polyaxon-sdk-2.0.0rc3.tar` & `polyaxon-sdk-2.0.0rc4.tar`

### file list

```diff
@@ -1,266 +1,266 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:42.033174 polyaxon-sdk-2.0.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-10 12:17:42.033174 polyaxon-sdk-2.0.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    52213 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:41.997174 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)    16971 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:42.001174 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   109338 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/agents_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/artifacts_stores_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37184 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/auth_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    54224 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/connections_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53837 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/dashboards_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   272189 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/organizations_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    54821 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/presets_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    64667 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/project_dashboards_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    64247 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/project_searches_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   238883 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/projects_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    75735 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/queues_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   481783 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/runs_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/schemas_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53431 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/searches_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    99627 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/service_accounts_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    59827 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/tags_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    98300 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/teams_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    73195 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/users_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19823 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/versions_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30255 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:42.033174 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (123)    15335 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/agent_state_response_agent_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/mx_job_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/protobuf_any.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/protobuf_null_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/runtime_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/search_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/spark_deploy_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_agent_state_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_agent_status_body_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_analytics_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_artifact_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_artifact_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_artifacts_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_artifacts_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_auth_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_average_stopping_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_bayes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_bucket_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_claim_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_clean_pod_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_cloning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_cloning_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_compiled_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_connection_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_connection_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_connection_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_connection_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_cron_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_dag_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_dashboard_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_date_time_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_diff_stopping_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_dockerfile_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_entities_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_entities_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_entity_notification_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_entity_stage_body_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_entity_status_body_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_chart_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_curve_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_events_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_failure_early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_file_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_flink.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_gcs_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_git_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_git_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_grid_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_host_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_host_path_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_date_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_date_time_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_geom_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_lin_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_log_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_log_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_log_uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_p_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_q_log_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_q_log_uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_q_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_q_uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hub_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hyperband.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hyperopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hyperopt_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_interval_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_join_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_k8s_resource_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_k8s_resource_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_kf_replica.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_activities_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_agents_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_bookmarks_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_connections_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_dashboards_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_organization_members_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_organizations_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_presets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_project_versions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_projects_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_queues_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_run_artifacts_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_run_connections_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_run_edges_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_runs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_searches_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_service_accounts_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_tags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_team_members_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_teams_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_matrix_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_median_stopping_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_metric_early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_mpi_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_mx_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_operation_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_optimization_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_optimization_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_organization_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_paddle_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_password_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_patch_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_path_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_pipeline_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_polyaxon_init_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_polyaxon_sidecar_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_project_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_project_user_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_project_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_project_version_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_pytorch_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_random_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_ray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_resource_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_edge_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_reference_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_s3_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_schedule_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_scheduling_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_search_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_section_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_settings_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_spark_replica.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_spark_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_stage_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_stages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_status_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_team_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_team_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_tensorboard_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_termination.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_tf_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_trial_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_trigger_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_truncation_stopping_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_uri_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_url_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_user_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_user_singup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_uuids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_wasb_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_xg_boost_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:41.997174 polyaxon-sdk-2.0.0rc3/polyaxon_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-10 12:17:41.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-04-10 12:17:41.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:17:41.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 12:17:41.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 12:17:41.000000 polyaxon-sdk-2.0.0rc3/polyaxon_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-10 12:17:42.037174 polyaxon-sdk-2.0.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-10 12:17:33.000000 polyaxon-sdk-2.0.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:44:35.976585 polyaxon-sdk-2.0.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-10 20:44:35.976585 polyaxon-sdk-2.0.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    51978 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:44:35.932585 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)    16971 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:44:35.936585 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109338 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/agents_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/artifacts_stores_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37184 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/auth_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54224 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/connections_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53837 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/dashboards_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   272189 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/organizations_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54821 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/presets_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64667 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/project_dashboards_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64247 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/project_searches_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238883 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/projects_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75735 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/queues_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   474161 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/runs_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/schemas_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53431 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/searches_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99627 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/service_accounts_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59827 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/tags_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98300 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/teams_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73195 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/users_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19823 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/versions_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30255 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:44:35.976585 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    15335 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/agent_state_response_agent_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/mx_job_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/protobuf_any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/protobuf_null_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/runtime_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/search_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/spark_deploy_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_agent_state_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_agent_status_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_analytics_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_artifact_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_artifact_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_artifacts_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_artifacts_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_auth_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_average_stopping_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_bayes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_bucket_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_claim_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_clean_pod_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_cloning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_cloning_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_compiled_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_connection_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_connection_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_connection_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_connection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_cron_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_dag_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_dashboard_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_date_time_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_diff_stopping_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_dockerfile_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_entities_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_entities_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_entity_notification_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_entity_stage_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_entity_status_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_chart_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_curve_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_failure_early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_file_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_flink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_gcs_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_git_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_git_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_host_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_host_path_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_date_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_date_time_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_geom_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_lin_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_log_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_log_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_log_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_p_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_q_log_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_q_log_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_q_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_q_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hub_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hyperopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hyperopt_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_interval_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_join_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_k8s_resource_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_k8s_resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_kf_replica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_activities_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_agents_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_bookmarks_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_connections_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_dashboards_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_organization_members_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_organizations_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_presets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_project_versions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_projects_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_queues_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_run_artifacts_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_run_connections_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_run_edges_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_runs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_searches_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_service_accounts_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_tags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_team_members_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_teams_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_matrix_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_median_stopping_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_metric_early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_mpi_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_mx_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_operation_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_optimization_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_optimization_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_organization_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_paddle_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_password_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_patch_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_path_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_pipeline_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_polyaxon_init_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_polyaxon_sidecar_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_project_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_project_user_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_project_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_project_version_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_pytorch_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_random_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_ray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_edge_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_reference_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_s3_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_schedule_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_scheduling_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_search_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_section_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_settings_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_spark_replica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_spark_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_stage_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_stages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_status_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_team_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_tensorboard_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_termination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_tf_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_trial_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_trigger_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_truncation_stopping_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_uri_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_url_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_user_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_user_singup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_uuids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_wasb_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_xg_boost_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:44:35.932585 polyaxon-sdk-2.0.0rc4/polyaxon_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-10 20:44:35.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-04-10 20:44:35.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:44:35.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 20:44:35.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 20:44:35.000000 polyaxon-sdk-2.0.0rc4/polyaxon_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-10 20:44:35.976585 polyaxon-sdk-2.0.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-10 20:44:25.000000 polyaxon-sdk-2.0.0rc4/setup.py
```

### Comparing `polyaxon-sdk-2.0.0rc3/README.md` & `polyaxon-sdk-2.0.0rc4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # polyaxon-sdk
 Polyaxon SDKs and REST API specification.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2.0.0-rc3
-- Package version: 2.0.0-rc3
+- API version: 2.0.0-rc4
+- Package version: 2.0.0-rc4
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 For more information, please visit [https://github.com/polyaxon/polyaxon](https://github.com/polyaxon/polyaxon)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -245,15 +245,14 @@
 *RunsV1Api* | [**create_run_artifacts_lineage**](docs/RunsV1Api.md#create_run_artifacts_lineage) | **POST** /api/v1/{owner}/{project}/runs/{uuid}/lineage/artifacts | Create bulk run artifacts lineage
 *RunsV1Api* | [**create_run_status**](docs/RunsV1Api.md#create_run_status) | **POST** /api/v1/{owner}/{project}/runs/{uuid}/statuses | Create new run status
 *RunsV1Api* | [**delete_run**](docs/RunsV1Api.md#delete_run) | **DELETE** /api/v1/{owner}/{entity}/runs/{uuid} | Delete run
 *RunsV1Api* | [**delete_run_artifact**](docs/RunsV1Api.md#delete_run_artifact) | **DELETE** /streams/v1/{namespace}/{owner}/{project}/runs/{uuid}/artifact | Delete run artifact
 *RunsV1Api* | [**delete_run_artifact_lineage**](docs/RunsV1Api.md#delete_run_artifact_lineage) | **DELETE** /api/v1/{owner}/{project}/runs/{uuid}/lineage/artifacts/{name} | Delete run artifact lineage
 *RunsV1Api* | [**delete_run_artifacts**](docs/RunsV1Api.md#delete_run_artifacts) | **DELETE** /streams/v1/{namespace}/{owner}/{project}/runs/{uuid}/artifacts | Delete run artifacts
 *RunsV1Api* | [**delete_runs**](docs/RunsV1Api.md#delete_runs) | **DELETE** /api/v1/{owner}/{project}/runs/delete | Delete runs
-*RunsV1Api* | [**deprecated_collect_run_logs**](docs/RunsV1Api.md#deprecated_collect_run_logs) | **POST** /streams/v1/{namespace}/_internal/{owner}/{project}/runs/{uuid}/{kind}/logs | Deprecated Collect run logs (# TODO: Remove in v2)
 *RunsV1Api* | [**get_multi_run_events**](docs/RunsV1Api.md#get_multi_run_events) | **GET** /streams/v1/{namespace}/{owner}/{project}/runs/multi/events/{kind} | Get multi runs events
 *RunsV1Api* | [**get_run**](docs/RunsV1Api.md#get_run) | **GET** /api/v1/{owner}/{entity}/runs/{uuid} | Get run
 *RunsV1Api* | [**get_run_artifact**](docs/RunsV1Api.md#get_run_artifact) | **GET** /streams/v1/{namespace}/{owner}/{project}/runs/{uuid}/artifact | Get run artifact
 *RunsV1Api* | [**get_run_artifact_lineage**](docs/RunsV1Api.md#get_run_artifact_lineage) | **GET** /api/v1/{owner}/{project}/runs/{uuid}/lineage/artifacts/{name} | Get run artifacts lineage
 *RunsV1Api* | [**get_run_artifacts**](docs/RunsV1Api.md#get_run_artifacts) | **GET** /streams/v1/{namespace}/{owner}/{project}/runs/{uuid}/artifacts | Get run artifacts
 *RunsV1Api* | [**get_run_artifacts_lineage**](docs/RunsV1Api.md#get_run_artifacts_lineage) | **GET** /api/v1/{owner}/{entity}/runs/{uuid}/lineage/artifacts | Get run artifacts lineage
 *RunsV1Api* | [**get_run_artifacts_lineage_names**](docs/RunsV1Api.md#get_run_artifacts_lineage_names) | **GET** /api/v1/{owner}/{entity}/runs/{uuid}/lineage/artifacts/names | Get run artifacts lineage names
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/__init__.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 # flake8: noqa
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "2.0.0-rc3"
+__version__ = "2.0.0-rc4"
 
 # import apis into sdk package
 from polyaxon_sdk.api.agents_v1_api import AgentsV1Api
 from polyaxon_sdk.api.artifacts_stores_v1_api import ArtifactsStoresV1Api
 from polyaxon_sdk.api.auth_v1_api import AuthV1Api
 from polyaxon_sdk.api.connections_v1_api import ConnectionsV1Api
 from polyaxon_sdk.api.dashboards_v1_api import DashboardsV1Api
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/__init__.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/agents_v1_api.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/agents_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/artifacts_stores_v1_api.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/artifacts_stores_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/auth_v1_api.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/auth_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/connections_v1_api.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/connections_v1_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/dashboards_v1_api.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/dashboards_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/organizations_v1_api.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/organizations_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/presets_v1_api.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/presets_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/project_dashboards_v1_api.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/project_dashboards_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/project_searches_v1_api.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/project_searches_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/projects_v1_api.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/projects_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/queues_v1_api.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/queues_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/runs_v1_api.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/runs_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -2659,182 +2659,14 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get('async_req'),
-            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=_params.get('_preload_content', True),
-            _request_timeout=_params.get('_request_timeout'),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get('_request_auth'))
-
-    @validate_arguments
-    def deprecated_collect_run_logs(self, namespace : StrictStr, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project where the run will be assigned")], uuid : Annotated[StrictStr, Field(..., description="Uuid identifier of the entity")], kind : Annotated[StrictStr, Field(..., description="Kind of the entity")], **kwargs) -> None:  # noqa: E501
-        """Deprecated Collect run logs (# TODO: Remove in v2)  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.deprecated_collect_run_logs(namespace, owner, project, uuid, kind, async_req=True)
-        >>> result = thread.get()
-
-        :param namespace: (required)
-        :type namespace: str
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param project: Project where the run will be assigned (required)
-        :type project: str
-        :param uuid: Uuid identifier of the entity (required)
-        :type uuid: str
-        :param kind: Kind of the entity (required)
-        :type kind: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: None
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.deprecated_collect_run_logs_with_http_info(namespace, owner, project, uuid, kind, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def deprecated_collect_run_logs_with_http_info(self, namespace : StrictStr, owner : Annotated[StrictStr, Field(..., description="Owner of the namespace")], project : Annotated[StrictStr, Field(..., description="Project where the run will be assigned")], uuid : Annotated[StrictStr, Field(..., description="Uuid identifier of the entity")], kind : Annotated[StrictStr, Field(..., description="Kind of the entity")], **kwargs):  # noqa: E501
-        """Deprecated Collect run logs (# TODO: Remove in v2)  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.deprecated_collect_run_logs_with_http_info(namespace, owner, project, uuid, kind, async_req=True)
-        >>> result = thread.get()
-
-        :param namespace: (required)
-        :type namespace: str
-        :param owner: Owner of the namespace (required)
-        :type owner: str
-        :param project: Project where the run will be assigned (required)
-        :type project: str
-        :param uuid: Uuid identifier of the entity (required)
-        :type uuid: str
-        :param kind: Kind of the entity (required)
-        :type kind: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: None
-        """
-
-        _params = locals()
-
-        _all_params = [
-            'namespace',
-            'owner',
-            'project',
-            'uuid',
-            'kind'
-        ]
-        _all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params['kwargs'].items():
-            if _key not in _all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method deprecated_collect_run_logs" % _key
-                )
-            _params[_key] = _val
-        del _params['kwargs']
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
-        if _params['namespace']:
-            _path_params['namespace'] = _params['namespace']
-
-        if _params['owner']:
-            _path_params['owner'] = _params['owner']
-
-        if _params['project']:
-            _path_params['project'] = _params['project']
-
-        if _params['uuid']:
-            _path_params['uuid'] = _params['uuid']
-
-        if _params['kind']:
-            _path_params['kind'] = _params['kind']
-
-
-        # process the query parameters
-        _query_params = []
-        # process the header parameters
-        _header_params = dict(_params.get('_headers', {}))
-        # process the form parameters
-        _form_params = []
-        _files = {}
-        # process the body parameter
-        _body_params = None
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # authentication setting
-        _auth_settings = ['ApiKey']  # noqa: E501
-
-        _response_types_map = {}
-
-        return self.api_client.call_api(
-            '/streams/v1/{namespace}/_internal/{owner}/{project}/runs/{uuid}/{kind}/logs', 'POST',
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/schemas_v1_api.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/schemas_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/searches_v1_api.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/searches_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/service_accounts_v1_api.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/service_accounts_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/tags_v1_api.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/tags_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/teams_v1_api.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/teams_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/users_v1_api.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/users_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api/versions_v1_api.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api/versions_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/api_client.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -88,15 +88,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.0.0-rc3/python'
+        self.user_agent = 'OpenAPI-Generator/2.0.0-rc4/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/configuration.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -405,16 +405,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.0.0-rc3\n"\
-               "SDK Package Version: 2.0.0-rc3".\
+               "Version of the API: 2.0.0-rc4\n"\
+               "SDK Package Version: 2.0.0-rc4".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/exceptions.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/__init__.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 # flake8: noqa
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/agent_state_response_agent_state.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/agent_state_response_agent_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/mx_job_mode.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/mx_job_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/protobuf_any.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/protobuf_any.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/protobuf_null_value.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/protobuf_null_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/runtime_error.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/runtime_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/search_view.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/search_view.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/spark_deploy_mode.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/spark_deploy_mode.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_activity.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_activity.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_agent.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_agent_state_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_agent_state_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_agent_status_body_request.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_agent_status_body_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_analytics_spec.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_analytics_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_artifact_kind.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_artifact_kind.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_artifact_tree.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_artifact_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_artifacts_mount.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_artifacts_mount.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_artifacts_type.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_artifacts_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_auth.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_auth_type.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_auth_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_average_stopping_policy.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_average_stopping_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_bayes.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_bayes.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_bucket_connection.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_bucket_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_build.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_cache.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_claim_connection.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_claim_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_clean_pod_policy.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_clean_pod_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_cloning.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -34,23 +34,23 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictStr
-from polyaxon_sdk.models.v1_cloning_kind import V1CloningKind
+from polyaxon_sdk.models.v1_pipeline_kind import V1PipelineKind
 
-class V1Cloning(BaseModel):
+class V1Pipeline(BaseModel):
     """
-    V1Cloning
+    V1Pipeline
     """
     uuid: Optional[StrictStr] = None
     name: Optional[StrictStr] = None
-    kind: Optional[V1CloningKind] = None
+    kind: Optional[V1PipelineKind] = None
     __properties = ["uuid", "name", "kind"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -58,35 +58,35 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1Cloning:
-        """Create an instance of V1Cloning from a JSON string"""
+    def from_json(cls, json_str: str) -> V1Pipeline:
+        """Create an instance of V1Pipeline from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1Cloning:
-        """Create an instance of V1Cloning from a dict"""
+    def from_dict(cls, obj: dict) -> V1Pipeline:
+        """Create an instance of V1Pipeline from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return V1Cloning.parse_obj(obj)
+            return V1Pipeline.parse_obj(obj)
 
-        _obj = V1Cloning.parse_obj({
+        _obj = V1Pipeline.parse_obj({
             "uuid": obj.get("uuid"),
             "name": obj.get("name"),
             "kind": obj.get("kind")
         })
         return _obj
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_cloning_kind.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_cloning_kind.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_compatibility.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_compatibility.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_compiled_operation.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_compiled_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_component.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_component.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_connection_kind.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_connection_kind.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_connection_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_connection_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_connection_schema.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_connection_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_connection_type.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_connection_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_credentials.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_cron_schedule.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_cron_schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_dag.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_dag.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_dag_ref.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_dag_ref.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_dashboard.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_dashboard_spec.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_dashboard_spec.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_dask.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_dask.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_date_time_schedule.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_date_time_schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_diff_stopping_policy.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_diff_stopping_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_dockerfile_type.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_dockerfile_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_early_stopping.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_early_stopping.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_entities_tags.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_entities_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_entities_transfer.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_entities_transfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_entity_notification_body.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_entity_notification_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_entity_stage_body_request.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_entity_stage_body_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_entity_status_body_request.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_entity_status_body_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_environment.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_artifact.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_artifact.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_audio.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_audio.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_chart.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_chart_kind.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_chart_kind.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_confusion_matrix.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_confusion_matrix.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_curve.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_curve.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_curve_kind.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_curve_kind.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_dataframe.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_dataframe.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_histogram.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_histogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_image.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_kind.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_kind.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_model.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_trigger.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_trigger.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_type.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_event_video.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_event_video.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_events_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_events_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_failure_early_stopping.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_failure_early_stopping.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_file_type.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_file_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_flink.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_flink.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_gcs_type.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_gcs_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_git_connection.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_git_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_git_type.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_git_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_grid_search.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_grid_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hook.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hook.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_host_connection.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_host_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_host_path_connection.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_host_path_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_choice.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_choice.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_date_range.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_date_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_date_time_range.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_date_time_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_geom_space.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_geom_space.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_lin_space.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_lin_space.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_log_normal.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_log_normal.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_log_space.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_log_space.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_log_uniform.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_log_uniform.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_normal.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_q_normal.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -35,19 +35,19 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
 from pydantic import BaseModel, StrictStr
 
-class V1HpNormal(BaseModel):
+class V1HpQNormal(BaseModel):
     """
-    V1HpNormal
+    V1HpQNormal
     """
-    kind: Optional[StrictStr] = 'normal'
+    kind: Optional[StrictStr] = 'qnormal'
     value: Optional[Dict[str, Any]] = None
     __properties = ["kind", "value"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -56,34 +56,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1HpNormal:
-        """Create an instance of V1HpNormal from a JSON string"""
+    def from_json(cls, json_str: str) -> V1HpQNormal:
+        """Create an instance of V1HpQNormal from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1HpNormal:
-        """Create an instance of V1HpNormal from a dict"""
+    def from_dict(cls, obj: dict) -> V1HpQNormal:
+        """Create an instance of V1HpQNormal from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return V1HpNormal.parse_obj(obj)
+            return V1HpQNormal.parse_obj(obj)
 
-        _obj = V1HpNormal.parse_obj({
-            "kind": obj.get("kind") if obj.get("kind") is not None else 'normal',
+        _obj = V1HpQNormal.parse_obj({
+            "kind": obj.get("kind") if obj.get("kind") is not None else 'qnormal',
             "value": obj.get("value")
         })
         return _obj
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_p_choice.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_p_choice.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_params.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_q_log_normal.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_q_log_normal.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_q_log_uniform.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_q_log_uniform.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_q_normal.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_q_uniform.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -35,19 +35,19 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
 from pydantic import BaseModel, StrictStr
 
-class V1HpQNormal(BaseModel):
+class V1HpQUniform(BaseModel):
     """
-    V1HpQNormal
+    V1HpQUniform
     """
-    kind: Optional[StrictStr] = 'qnormal'
+    kind: Optional[StrictStr] = 'quniform'
     value: Optional[Dict[str, Any]] = None
     __properties = ["kind", "value"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -56,34 +56,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1HpQNormal:
-        """Create an instance of V1HpQNormal from a JSON string"""
+    def from_json(cls, json_str: str) -> V1HpQUniform:
+        """Create an instance of V1HpQUniform from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1HpQNormal:
-        """Create an instance of V1HpQNormal from a dict"""
+    def from_dict(cls, obj: dict) -> V1HpQUniform:
+        """Create an instance of V1HpQUniform from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return V1HpQNormal.parse_obj(obj)
+            return V1HpQUniform.parse_obj(obj)
 
-        _obj = V1HpQNormal.parse_obj({
-            "kind": obj.get("kind") if obj.get("kind") is not None else 'qnormal',
+        _obj = V1HpQUniform.parse_obj({
+            "kind": obj.get("kind") if obj.get("kind") is not None else 'quniform',
             "value": obj.get("value")
         })
         return _obj
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_q_uniform.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_uniform.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -35,19 +35,19 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
 from pydantic import BaseModel, StrictStr
 
-class V1HpQUniform(BaseModel):
+class V1HpUniform(BaseModel):
     """
-    V1HpQUniform
+    V1HpUniform
     """
-    kind: Optional[StrictStr] = 'quniform'
+    kind: Optional[StrictStr] = 'uniform'
     value: Optional[Dict[str, Any]] = None
     __properties = ["kind", "value"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -56,34 +56,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1HpQUniform:
-        """Create an instance of V1HpQUniform from a JSON string"""
+    def from_json(cls, json_str: str) -> V1HpUniform:
+        """Create an instance of V1HpUniform from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1HpQUniform:
-        """Create an instance of V1HpQUniform from a dict"""
+    def from_dict(cls, obj: dict) -> V1HpUniform:
+        """Create an instance of V1HpUniform from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return V1HpQUniform.parse_obj(obj)
+            return V1HpUniform.parse_obj(obj)
 
-        _obj = V1HpQUniform.parse_obj({
-            "kind": obj.get("kind") if obj.get("kind") is not None else 'quniform',
+        _obj = V1HpUniform.parse_obj({
+            "kind": obj.get("kind") if obj.get("kind") is not None else 'uniform',
             "value": obj.get("value")
         })
         return _obj
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_range.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hp_uniform.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hub_ref.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,73 +17,73 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict, Optional
+from typing import Optional
 from pydantic import BaseModel, StrictStr
 
-class V1HpUniform(BaseModel):
+class V1HubRef(BaseModel):
     """
-    V1HpUniform
+    V1HubRef
     """
-    kind: Optional[StrictStr] = 'uniform'
-    value: Optional[Dict[str, Any]] = None
-    __properties = ["kind", "value"]
+    kind: Optional[StrictStr] = 'hub_ref'
+    name: Optional[StrictStr] = None
+    __properties = ["kind", "name"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1HpUniform:
-        """Create an instance of V1HpUniform from a JSON string"""
+    def from_json(cls, json_str: str) -> V1HubRef:
+        """Create an instance of V1HubRef from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1HpUniform:
-        """Create an instance of V1HpUniform from a dict"""
+    def from_dict(cls, obj: dict) -> V1HubRef:
+        """Create an instance of V1HubRef from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return V1HpUniform.parse_obj(obj)
+            return V1HubRef.parse_obj(obj)
 
-        _obj = V1HpUniform.parse_obj({
-            "kind": obj.get("kind") if obj.get("kind") is not None else 'uniform',
-            "value": obj.get("value")
+        _obj = V1HubRef.parse_obj({
+            "kind": obj.get("kind") if obj.get("kind") is not None else 'hub_ref',
+            "name": obj.get("name")
         })
         return _obj
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hub_ref.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_url_ref.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -35,55 +35,55 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictStr
 
-class V1HubRef(BaseModel):
+class V1UrlRef(BaseModel):
     """
-    V1HubRef
+    V1UrlRef
     """
-    kind: Optional[StrictStr] = 'hub_ref'
-    name: Optional[StrictStr] = None
-    __properties = ["kind", "name"]
+    kind: Optional[StrictStr] = 'url_ref'
+    url: Optional[StrictStr] = None
+    __properties = ["kind", "url"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1HubRef:
-        """Create an instance of V1HubRef from a JSON string"""
+    def from_json(cls, json_str: str) -> V1UrlRef:
+        """Create an instance of V1UrlRef from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1HubRef:
-        """Create an instance of V1HubRef from a dict"""
+    def from_dict(cls, obj: dict) -> V1UrlRef:
+        """Create an instance of V1UrlRef from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return V1HubRef.parse_obj(obj)
+            return V1UrlRef.parse_obj(obj)
 
-        _obj = V1HubRef.parse_obj({
-            "kind": obj.get("kind") if obj.get("kind") is not None else 'hub_ref',
-            "name": obj.get("name")
+        _obj = V1UrlRef.parse_obj({
+            "kind": obj.get("kind") if obj.get("kind") is not None else 'url_ref',
+            "url": obj.get("url")
         })
         return _obj
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hyperband.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hyperband.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hyperopt.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hyperopt.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_hyperopt_algorithms.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hyperopt_algorithms.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_init.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_init.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_installation.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_installation.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_interval_schedule.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_interval_schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_io.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_iterative.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_iterative.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_job.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_join.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_join.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_join_param.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_join_param.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_k8s_resource_schema.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_k8s_resource_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_k8s_resource_type.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_k8s_resource_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_kf_replica.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_kf_replica.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_activities_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_activities_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_agents_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_agents_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_bookmarks_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_bookmarks_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_connections_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_connections_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_dashboards_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_dashboards_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_organization_members_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_organization_members_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_organizations_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_organizations_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_presets_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_presets_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_project_versions_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_project_versions_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_projects_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_projects_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_queues_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_queues_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_run_artifacts_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_run_artifacts_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_run_connections_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_run_connections_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_run_edges_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_run_edges_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_runs_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_runs_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_searches_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_searches_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_service_accounts_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_service_accounts_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_tags_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_tags_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_team_members_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_team_members_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_teams_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_teams_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_list_token_response.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_list_token_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_log.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_log_handler.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_log_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_logs.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_mapping.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_matrix.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_matrix_kind.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_matrix_kind.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_median_stopping_policy.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_median_stopping_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_metric_early_stopping.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_metric_early_stopping.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_mpi_job.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_mpi_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_mx_job.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_mx_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_notification.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_notification.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_operation.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_operation_body.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_operation_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_optimization.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_optimization.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_optimization_metric.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_optimization_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_optimization_resource.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_optimization_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_organization.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_organization.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_organization_member.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_organization_member.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_paddle_job.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_paddle_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_param.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_param.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_password_change.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_password_change.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_patch_strategy.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_patch_strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_path_ref.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_path_ref.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_pipeline.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_ray.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,76 +17,73 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Any, Dict, Optional
 from pydantic import BaseModel, StrictStr
-from polyaxon_sdk.models.v1_pipeline_kind import V1PipelineKind
 
-class V1Pipeline(BaseModel):
+class V1Ray(BaseModel):
     """
-    V1Pipeline
+    V1Ray
     """
-    uuid: Optional[StrictStr] = None
-    name: Optional[StrictStr] = None
-    kind: Optional[V1PipelineKind] = None
-    __properties = ["uuid", "name", "kind"]
+    kind: Optional[StrictStr] = None
+    spec: Optional[Dict[str, Any]] = None
+    __properties = ["kind", "spec"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1Pipeline:
-        """Create an instance of V1Pipeline from a JSON string"""
+    def from_json(cls, json_str: str) -> V1Ray:
+        """Create an instance of V1Ray from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1Pipeline:
-        """Create an instance of V1Pipeline from a dict"""
+    def from_dict(cls, obj: dict) -> V1Ray:
+        """Create an instance of V1Ray from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return V1Pipeline.parse_obj(obj)
+            return V1Ray.parse_obj(obj)
 
-        _obj = V1Pipeline.parse_obj({
-            "uuid": obj.get("uuid"),
-            "name": obj.get("name"),
-            "kind": obj.get("kind")
+        _obj = V1Ray.parse_obj({
+            "kind": obj.get("kind"),
+            "spec": obj.get("spec")
         })
         return _obj
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_pipeline_kind.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_pipeline_kind.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_plugins.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_polyaxon_init_container.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_polyaxon_init_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_polyaxon_sidecar_container.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_polyaxon_sidecar_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_preset.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_preset.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_project.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_project_settings.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_project_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_project_user_access.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_project_user_access.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_project_version.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_project_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_project_version_kind.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_project_version_kind.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_pytorch_job.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_pytorch_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_queue.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_random_search.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_random_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_ray.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_uuids.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,73 +17,71 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict, Optional
-from pydantic import BaseModel, StrictStr
+from typing import List, Optional
+from pydantic import BaseModel, StrictStr, conlist
 
-class V1Ray(BaseModel):
+class V1Uuids(BaseModel):
     """
-    V1Ray
+    V1Uuids
     """
-    kind: Optional[StrictStr] = None
-    spec: Optional[Dict[str, Any]] = None
-    __properties = ["kind", "spec"]
+    uuids: Optional[conlist(StrictStr)] = None
+    __properties = ["uuids"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1Ray:
-        """Create an instance of V1Ray from a JSON string"""
+    def from_json(cls, json_str: str) -> V1Uuids:
+        """Create an instance of V1Uuids from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1Ray:
-        """Create an instance of V1Ray from a dict"""
+    def from_dict(cls, obj: dict) -> V1Uuids:
+        """Create an instance of V1Uuids from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return V1Ray.parse_obj(obj)
+            return V1Uuids.parse_obj(obj)
 
-        _obj = V1Ray.parse_obj({
-            "kind": obj.get("kind"),
-            "spec": obj.get("spec")
+        _obj = V1Uuids.parse_obj({
+            "uuids": obj.get("uuids")
         })
         return _obj
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_reference.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_resource_type.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_resource_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_artifact.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_artifact.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_artifacts.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_artifacts.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_connection.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_edge.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_edge.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_edge_kind.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_edge_kind.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_kind.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_kind.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_pending.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_pending.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_reference_catalog.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_reference_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_resources.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_schema.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_run_settings.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_run_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_s3_type.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_s3_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_schedule.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_schedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_schedule_kind.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_schedule_kind.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_scheduling_policy.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_scheduling_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_schemas.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_search.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_search_spec.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_search_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_section_spec.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_section_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_service.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_service_account.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_service_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_settings_catalog.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_settings_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_spark.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_spark.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_spark_replica.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_spark_replica.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_spark_type.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_trigger_policy.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -34,20 +34,22 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1SparkType(str, Enum):
+class V1TriggerPolicy(str, Enum):
     """
-    V1SparkType
+    V1TriggerPolicy
     """
 
     """
     allowed enum values
     """
-    JAVA = 'java'
-    SCALA = 'scala'
-    PYTHON = 'python'
-    R = 'r'
+    ALL_SUCCEEDED = 'all_succeeded'
+    ALL_FAILED = 'all_failed'
+    ALL_DONE = 'all_done'
+    ONE_SUCCEEDED = 'one_succeeded'
+    ONE_FAILED = 'one_failed'
+    ONE_DONE = 'one_done'
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_stage.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_stage_condition.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_stage_condition.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_stages.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_stages.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_status.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_status_condition.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_status_condition.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_statuses.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_statuses.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_tag.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_tag.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_team.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_team.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_team_member.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_team_member.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_team_settings.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_team_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_template.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_tensorboard_type.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_tensorboard_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_termination.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_termination.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_tf_job.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_tf_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_token.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_trial_start.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_trial_start.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_trigger_policy.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_spark_type.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -34,22 +34,20 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1TriggerPolicy(str, Enum):
+class V1SparkType(str, Enum):
     """
-    V1TriggerPolicy
+    V1SparkType
     """
 
     """
     allowed enum values
     """
-    ALL_SUCCEEDED = 'all_succeeded'
-    ALL_FAILED = 'all_failed'
-    ALL_DONE = 'all_done'
-    ONE_SUCCEEDED = 'one_succeeded'
-    ONE_FAILED = 'one_failed'
-    ONE_DONE = 'one_done'
+    JAVA = 'java'
+    SCALA = 'scala'
+    PYTHON = 'python'
+    R = 'r'
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_truncation_stopping_policy.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_truncation_stopping_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_tuner.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_tuner.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_uri_type.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_uri_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_url_ref.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_cloning.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -34,56 +34,59 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictStr
+from polyaxon_sdk.models.v1_cloning_kind import V1CloningKind
 
-class V1UrlRef(BaseModel):
+class V1Cloning(BaseModel):
     """
-    V1UrlRef
+    V1Cloning
     """
-    kind: Optional[StrictStr] = 'url_ref'
-    url: Optional[StrictStr] = None
-    __properties = ["kind", "url"]
+    uuid: Optional[StrictStr] = None
+    name: Optional[StrictStr] = None
+    kind: Optional[V1CloningKind] = None
+    __properties = ["uuid", "name", "kind"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1UrlRef:
-        """Create an instance of V1UrlRef from a JSON string"""
+    def from_json(cls, json_str: str) -> V1Cloning:
+        """Create an instance of V1Cloning from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1UrlRef:
-        """Create an instance of V1UrlRef from a dict"""
+    def from_dict(cls, obj: dict) -> V1Cloning:
+        """Create an instance of V1Cloning from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return V1UrlRef.parse_obj(obj)
+            return V1Cloning.parse_obj(obj)
 
-        _obj = V1UrlRef.parse_obj({
-            "kind": obj.get("kind") if obj.get("kind") is not None else 'url_ref',
-            "url": obj.get("url")
+        _obj = V1Cloning.parse_obj({
+            "uuid": obj.get("uuid"),
+            "name": obj.get("name"),
+            "kind": obj.get("kind")
         })
         return _obj
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_user.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_user_email.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_user_email.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_user_singup.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_user_singup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_uuids.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,71 +17,73 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
-from pydantic import BaseModel, StrictStr, conlist
+from typing import Optional
+from pydantic import BaseModel, StrictStr
 
-class V1Uuids(BaseModel):
+class V1Version(BaseModel):
     """
-    V1Uuids
+    V1Version
     """
-    uuids: Optional[conlist(StrictStr)] = None
-    __properties = ["uuids"]
+    min: Optional[StrictStr] = None
+    latest: Optional[StrictStr] = None
+    __properties = ["min", "latest"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1Uuids:
-        """Create an instance of V1Uuids from a JSON string"""
+    def from_json(cls, json_str: str) -> V1Version:
+        """Create an instance of V1Version from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1Uuids:
-        """Create an instance of V1Uuids from a dict"""
+    def from_dict(cls, obj: dict) -> V1Version:
+        """Create an instance of V1Version from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return V1Uuids.parse_obj(obj)
+            return V1Version.parse_obj(obj)
 
-        _obj = V1Uuids.parse_obj({
-            "uuids": obj.get("uuids")
+        _obj = V1Version.parse_obj({
+            "min": obj.get("min"),
+            "latest": obj.get("latest")
         })
         return _obj
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_version.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_wasb_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -33,57 +33,59 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, Field, StrictBool, StrictStr
 
-class V1Version(BaseModel):
+class V1WasbType(BaseModel):
     """
-    V1Version
+    V1WasbType
     """
-    min: Optional[StrictStr] = None
-    latest: Optional[StrictStr] = None
-    __properties = ["min", "latest"]
+    container: Optional[StrictStr] = None
+    storage_account: Optional[StrictStr] = Field(None, alias="storageAccount")
+    path: Optional[StrictBool] = None
+    __properties = ["container", "storageAccount", "path"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1Version:
-        """Create an instance of V1Version from a JSON string"""
+    def from_json(cls, json_str: str) -> V1WasbType:
+        """Create an instance of V1WasbType from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1Version:
-        """Create an instance of V1Version from a dict"""
+    def from_dict(cls, obj: dict) -> V1WasbType:
+        """Create an instance of V1WasbType from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return V1Version.parse_obj(obj)
+            return V1WasbType.parse_obj(obj)
 
-        _obj = V1Version.parse_obj({
-            "min": obj.get("min"),
-            "latest": obj.get("latest")
+        _obj = V1WasbType.parse_obj({
+            "container": obj.get("container"),
+            "storage_account": obj.get("storageAccount"),
+            "path": obj.get("path")
         })
         return _obj
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_wasb_type.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_hp_normal.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,75 +17,73 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+from typing import Any, Dict, Optional
+from pydantic import BaseModel, StrictStr
 
-class V1WasbType(BaseModel):
+class V1HpNormal(BaseModel):
     """
-    V1WasbType
+    V1HpNormal
     """
-    container: Optional[StrictStr] = None
-    storage_account: Optional[StrictStr] = Field(None, alias="storageAccount")
-    path: Optional[StrictBool] = None
-    __properties = ["container", "storageAccount", "path"]
+    kind: Optional[StrictStr] = 'normal'
+    value: Optional[Dict[str, Any]] = None
+    __properties = ["kind", "value"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1WasbType:
-        """Create an instance of V1WasbType from a JSON string"""
+    def from_json(cls, json_str: str) -> V1HpNormal:
+        """Create an instance of V1HpNormal from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1WasbType:
-        """Create an instance of V1WasbType from a dict"""
+    def from_dict(cls, obj: dict) -> V1HpNormal:
+        """Create an instance of V1HpNormal from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return V1WasbType.parse_obj(obj)
+            return V1HpNormal.parse_obj(obj)
 
-        _obj = V1WasbType.parse_obj({
-            "container": obj.get("container"),
-            "storage_account": obj.get("storageAccount"),
-            "path": obj.get("path")
+        _obj = V1HpNormal.parse_obj({
+            "kind": obj.get("kind") if obj.get("kind") is not None else 'normal',
+            "value": obj.get("value")
         })
         return _obj
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/models/v1_xg_boost_job.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/models/v1_xg_boost_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk/rest.py` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `polyaxon-sdk-2.0.0rc3/polyaxon_sdk.egg-info/SOURCES.txt` & `polyaxon-sdk-2.0.0rc4/polyaxon_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polyaxon-sdk-2.0.0rc3/pyproject.toml` & `polyaxon-sdk-2.0.0rc4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polyaxon_sdk"
-version = "2.0.0-rc3"
+version = "2.0.0-rc4"
 description = "Polyaxon SDKs and REST API specification."
 authors = ["contact@polyaxon.com"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_REPO_ID/GIT_USER_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Polyaxon SDKs and REST API specification."]
```

### Comparing `polyaxon-sdk-2.0.0rc3/setup.py` & `polyaxon-sdk-2.0.0rc4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # coding: utf-8
 
 """
     Polyaxon SDKs and REST API specification.
 
     Polyaxon SDKs and REST API specification.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-rc3
+    The version of the OpenAPI document: 2.0.0-rc4
     Contact: contact@polyaxon.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -34,15 +34,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "polyaxon-sdk"
-VERSION = "2.0.0-rc3"
+VERSION = "2.0.0-rc4"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3",
     "python-dateutil",
     "pydantic",
     "aenum"
 ]
```


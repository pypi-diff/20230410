# Comparing `tmp/whylabs-client-0.4.4.tar.gz` & `tmp/whylabs-client-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylabs-client-0.4.4.tar", last modified: Fri Mar 24 20:52:29 2023, max compression
+gzip compressed data, was "whylabs-client-0.4.5.tar", last modified: Mon Apr 10 21:52:27 2023, max compression
```

## Comparing `whylabs-client-0.4.4.tar` & `whylabs-client-0.4.5.tar`

### file list

```diff
@@ -1,147 +1,148 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 20:52:29.308871 whylabs-client-0.4.4/
--rw-r--r--   0 root         (0) root         (0)      396 2023-03-24 20:52:29.308871 whylabs-client-0.4.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    20300 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-03-24 20:52:29.309872 whylabs-client-0.4.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1097 2023-03-24 20:52:28.000000 whylabs-client-0.4.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 20:52:29.264868 whylabs-client-0.4.4/whylabs_client/
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 20:52:29.269868 whylabs-client-0.4.4/whylabs_client/api/
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15394 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/api/dataset_metadata_api.py
--rw-rw-rw-   0 root         (0) root         (0)    12904 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/api/dataset_profile_api.py
--rw-rw-rw-   0 root         (0) root         (0)    10632 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/api/feature_weights_api.py
--rw-rw-rw-   0 root         (0) root         (0)    11520 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/api/log_api.py
--rw-rw-rw-   0 root         (0) root         (0)    20727 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/api/membership_api.py
--rw-rw-rw-   0 root         (0) root         (0)    52204 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/api/models_api.py
--rw-rw-rw-   0 root         (0) root         (0)    52337 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/api/monitor_api.py
--rw-rw-rw-   0 root         (0) root         (0)    42851 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/api/notification_settings_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5237 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/api/schema_api.py
--rw-rw-rw-   0 root         (0) root         (0)    14846 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/api/sessions_api.py
--rw-rw-rw-   0 root         (0) root         (0)    37575 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 20:52:29.270868 whylabs-client-0.4.4/whylabs_client/apis/
--rw-rw-rw-   0 root         (0) root         (0)     1038 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17084 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     5075 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 20:52:29.308871 whylabs-client-0.4.4/whylabs_client/model/
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11664 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/action_type.py
--rw-rw-rw-   0 root         (0) root         (0)    12110 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/add_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12005 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/async_log_response.py
--rw-rw-rw-   0 root         (0) root         (0)    13478 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/aws_marketplace_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    12443 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/column_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    11118 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/create_session_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11207 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/create_session_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11136 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/create_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13099 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/databricks_connection.py
--rw-rw-rw-   0 root         (0) root         (0)    11884 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/dataset_request_monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11114 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/datatype_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11061 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/delete_analyzer_results_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11061 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/delete_dataset_profiles_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11368 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/distribution_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11275 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/dto_auto_scale_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    13176 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/dto_aws_attributes_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11715 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/dto_aws_availability_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11665 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/dto_cluster_log_conf_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11338 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/dto_cron_schedule_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11082 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/dto_dbfs_storage_info_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11745 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/dto_ebs_volume_type_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11928 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/dto_job_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12392 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/dto_job_email_notifications_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    15918 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/dto_job_settings_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    14946 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/dto_new_cluster_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11591 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/dto_notebook_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11909 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/dto_spark_jar_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11493 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/dto_spark_python_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11281 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/dto_spark_submit_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12338 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/dtos3_storage_info_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11106 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/email_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    11739 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/entity_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    11862 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/entity_weight_record.py
--rw-rw-rw-   0 root         (0) root         (0)    11507 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/entity_weight_record_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11225 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/feature_flags.py
--rw-rw-rw-   0 root         (0) root         (0)    11574 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/get_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11411 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/get_connection_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11222 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/get_dataset_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11283 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/get_default_membership_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11431 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/get_marketplace_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11485 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/get_memberships_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11379 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/get_monitor_config_v2_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11417 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/get_notification_settings_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11334 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/get_session_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11559 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/list_jobs_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11260 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/list_jobs_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11496 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/list_models_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11530 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/list_organization_memberships_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11382 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/list_user_api_keys.py
--rw-rw-rw-   0 root         (0) root         (0)    11502 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/log_async_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11354 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/log_reference_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11858 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/log_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11441 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/log_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12015 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/marketplace_dimensions.py
--rw-rw-rw-   0 root         (0) root         (0)    12029 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/membership.py
--rw-rw-rw-   0 root         (0) root         (0)    11756 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/membership_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11120 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/missing_recent_data_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11132 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/missing_recent_profiles_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11938 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/missing_values_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    12527 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/model_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12219 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/model_type.py
--rw-rw-rw-   0 root         (0) root         (0)    13063 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11473 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/monitor_config_version.py
--rw-rw-rw-   0 root         (0) root         (0)    12120 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/monitor_request_reference.py
--rw-rw-rw-   0 root         (0) root         (0)    11689 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/monitor_request_reference_type.py
--rw-rw-rw-   0 root         (0) root         (0)    11783 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    11982 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/notification_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    11979 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/notification_settings_day.py
--rw-rw-rw-   0 root         (0) root         (0)    11751 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/notification_sqs_message_cadence.py
--rw-rw-rw-   0 root         (0) root         (0)    14425 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/organization_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    13737 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/organization_summary.py
--rw-rw-rw-   0 root         (0) root         (0)    11215 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/pager_duty_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    12319 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/provided_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11680 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/provision_databricks_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11657 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/provision_databricks_connection_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11882 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/provision_new_aws_marketplace_user_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12226 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/provision_new_marketplace_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12422 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/provision_new_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11574 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/provision_new_user_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12315 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/reference_profile_item_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11188 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/refresh_access_token_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11444 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/refresh_connection_by_org_id_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11586 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/refresh_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13668 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/register_databricks_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11112 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/register_databricks_connection_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11317 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/remove_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13372 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/request_feature_monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    15325 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/request_monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11070 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/response.py
--rw-rw-rw-   0 root         (0) root         (0)    11580 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/role.py
--rw-rw-rw-   0 root         (0) root         (0)    11922 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/run_job_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11089 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/run_job_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11471 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/schema_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11833 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/seasonal_arima_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11197 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/segment.py
--rw-rw-rw-   0 root         (0) root         (0)    11192 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/segment_tag.py
--rw-rw-rw-   0 root         (0) root         (0)    11505 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/segment_weight.py
--rw-rw-rw-   0 root         (0) root         (0)    11948 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/session_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11350 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/set_default_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11193 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/slack_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    11652 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/subscription_tier.py
--rw-rw-rw-   0 root         (0) root         (0)    11670 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/time_period.py
--rw-rw-rw-   0 root         (0) root         (0)    12934 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/uber_notification_schedule.py
--rw-rw-rw-   0 root         (0) root         (0)    11917 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/unique_values_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11548 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/update_connection_changes.py
--rw-rw-rw-   0 root         (0) root         (0)    11816 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/update_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11650 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/update_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11747 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/user.py
--rw-rw-rw-   0 root         (0) root         (0)    13667 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/user_api_key.py
--rw-rw-rw-   0 root         (0) root         (0)    11220 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/user_api_key_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11805 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model/why_logs_metric.py
--rw-rw-rw-   0 root         (0) root         (0)    81897 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 20:52:29.308871 whylabs-client-0.4.4/whylabs_client/models/
--rw-rw-rw-   0 root         (0) root         (0)     9159 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14199 2023-03-24 20:52:18.000000 whylabs-client-0.4.4/whylabs_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 20:52:29.265868 whylabs-client-0.4.4/whylabs_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      396 2023-03-24 20:52:28.000000 whylabs-client-0.4.4/whylabs_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6247 2023-03-24 20:52:28.000000 whylabs-client-0.4.4/whylabs_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 20:52:28.000000 whylabs-client-0.4.4/whylabs_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-03-24 20:52:28.000000 whylabs-client-0.4.4/whylabs_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-03-24 20:52:28.000000 whylabs-client-0.4.4/whylabs_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 21:52:27.841472 whylabs-client-0.4.5/
+-rw-r--r--   0 root         (0) root         (0)      396 2023-04-10 21:52:27.841472 whylabs-client-0.4.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    21762 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-10 21:52:27.841472 whylabs-client-0.4.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2023-04-10 21:52:26.000000 whylabs-client-0.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 21:52:27.788666 whylabs-client-0.4.5/whylabs_client/
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 21:52:27.795640 whylabs-client-0.4.5/whylabs_client/api/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15394 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/dataset_metadata_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    18502 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/dataset_profile_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    10632 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/feature_weights_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    11520 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/log_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    20727 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/membership_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    67177 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/models_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    52337 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/monitor_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    48204 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/notification_settings_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5237 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/schema_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    19879 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api/sessions_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    37575 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 21:52:27.795640 whylabs-client-0.4.5/whylabs_client/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17084 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5075 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 21:52:27.840476 whylabs-client-0.4.5/whylabs_client/model/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11664 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/action_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    12110 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/add_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12005 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/async_log_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    13478 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/aws_marketplace_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    12443 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/column_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    11118 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/create_session_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11207 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/create_session_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11136 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/create_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13099 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/databricks_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    11884 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dataset_request_monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11114 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/datatype_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11061 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/delete_analyzer_results_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11061 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/delete_dataset_profiles_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11368 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/distribution_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11275 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_auto_scale_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    13176 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_aws_attributes_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11715 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_aws_availability_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11665 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_cluster_log_conf_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11338 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_cron_schedule_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11082 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_dbfs_storage_info_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11745 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_ebs_volume_type_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11928 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_job_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12392 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_job_email_notifications_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    15918 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_job_settings_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    14946 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_new_cluster_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11591 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_notebook_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11909 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_spark_jar_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11493 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_spark_python_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11281 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dto_spark_submit_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12338 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/dtos3_storage_info_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11106 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/email_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    12313 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/entity_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    11862 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/entity_weight_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    11507 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/entity_weight_record_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11225 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/feature_flags.py
+-rw-rw-rw-   0 root         (0) root         (0)    11574 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/get_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11411 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/get_connection_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11222 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/get_dataset_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11283 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/get_default_membership_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11431 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/get_marketplace_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11485 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/get_memberships_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11379 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/get_monitor_config_v2_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11417 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/get_notification_settings_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11334 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/get_session_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11559 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/list_jobs_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11260 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/list_jobs_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11496 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/list_models_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11530 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/list_organization_memberships_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11382 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/list_user_api_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)    11502 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/log_async_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11354 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/log_reference_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11858 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/log_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11441 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/log_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12015 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/marketplace_dimensions.py
+-rw-rw-rw-   0 root         (0) root         (0)    12029 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/membership.py
+-rw-rw-rw-   0 root         (0) root         (0)    11756 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/membership_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    12260 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/metric_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    11120 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/missing_recent_data_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11132 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/missing_recent_profiles_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11938 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/missing_values_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    12569 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/model_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12219 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/model_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    13063 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11473 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/monitor_config_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    12120 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/monitor_request_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)    11689 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/monitor_request_reference_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    11783 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    11982 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/notification_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    11979 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/notification_settings_day.py
+-rw-rw-rw-   0 root         (0) root         (0)    11751 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/notification_sqs_message_cadence.py
+-rw-rw-rw-   0 root         (0) root         (0)    14425 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/organization_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    13737 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/organization_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)    11215 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/pager_duty_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    12319 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/provided_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11680 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/provision_databricks_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11657 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/provision_databricks_connection_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11882 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/provision_new_aws_marketplace_user_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12226 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/provision_new_marketplace_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12422 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/provision_new_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11574 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/provision_new_user_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12315 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/reference_profile_item_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11188 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/refresh_access_token_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11444 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/refresh_connection_by_org_id_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11586 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/refresh_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13668 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/register_databricks_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11112 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/register_databricks_connection_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11317 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/remove_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13372 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/request_feature_monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15325 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/request_monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11070 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11580 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/role.py
+-rw-rw-rw-   0 root         (0) root         (0)    11922 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/run_job_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11089 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/run_job_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11471 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/schema_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11833 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/seasonal_arima_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11197 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/segment.py
+-rw-rw-rw-   0 root         (0) root         (0)    11192 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/segment_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)    11505 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/segment_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)    11948 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/session_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11350 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/set_default_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11193 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/slack_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    11652 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/subscription_tier.py
+-rw-rw-rw-   0 root         (0) root         (0)    11670 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/time_period.py
+-rw-rw-rw-   0 root         (0) root         (0)    12934 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/uber_notification_schedule.py
+-rw-rw-rw-   0 root         (0) root         (0)    11917 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/unique_values_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11548 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/update_connection_changes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11816 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/update_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11650 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/update_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11747 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/user.py
+-rw-rw-rw-   0 root         (0) root         (0)    13667 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/user_api_key.py
+-rw-rw-rw-   0 root         (0) root         (0)    11220 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/user_api_key_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11805 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model/why_logs_metric.py
+-rw-rw-rw-   0 root         (0) root         (0)    81897 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 21:52:27.840476 whylabs-client-0.4.5/whylabs_client/models/
+-rw-rw-rw-   0 root         (0) root         (0)     9219 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14199 2023-04-10 21:52:15.000000 whylabs-client-0.4.5/whylabs_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 21:52:27.790658 whylabs-client-0.4.5/whylabs_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      396 2023-04-10 21:52:27.000000 whylabs-client-0.4.5/whylabs_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6285 2023-04-10 21:52:27.000000 whylabs-client-0.4.5/whylabs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 21:52:27.000000 whylabs-client-0.4.5/whylabs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-10 21:52:27.000000 whylabs-client-0.4.5/whylabs_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-10 21:52:27.000000 whylabs-client-0.4.5/whylabs_client.egg-info/top_level.txt
```

### Comparing `whylabs-client-0.4.4/README.md` & `whylabs-client-0.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # whylabs-client
 WhyLabs API that enables end-to-end AI observability
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1
-- Package version: 0.4.4
+- Package version: 0.4.5
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://whylabs.ai](https://whylabs.ai)
 
 ## Requirements.
 
 Python >= 3.6
 
@@ -49,14 +49,15 @@
 
 import time
 import whylabs_client
 from pprint import pprint
 from whylabs_client.api import dataset_profile_api
 from whylabs_client.model.delete_analyzer_results_response import DeleteAnalyzerResultsResponse
 from whylabs_client.model.delete_dataset_profiles_response import DeleteDatasetProfilesResponse
+from whylabs_client.model.reference_profile_item_response import ReferenceProfileItemResponse
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = whylabs_client.Configuration(
     host = "http://localhost"
 )
 
 # The client must configure the authentication and authorization parameters
@@ -92,56 +93,62 @@
 
 All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *DatasetProfileApi* | [**delete_analyzer_results**](docs/DatasetProfileApi.md#delete_analyzer_results) | **DELETE** /v0/organizations/{org_id}/dataset-profiles/models/{dataset_id}/analyzer-results | Deletes a set of analyzer results
 *DatasetProfileApi* | [**delete_dataset_profiles**](docs/DatasetProfileApi.md#delete_dataset_profiles) | **DELETE** /v0/organizations/{org_id}/dataset-profiles/models/{dataset_id} | Deletes a set of dataset profiles
+*DatasetProfileApi* | [**list_reference_profiles**](docs/DatasetProfileApi.md#list_reference_profiles) | **GET** /v0/organizations/{org_id}/dataset-profiles/models/{model_id}/reference-profiles | Returns a list for reference profiles
 *DatasetMetadataApi* | [**delete_dataset_metadata**](docs/DatasetMetadataApi.md#delete_dataset_metadata) | **DELETE** /v0/organizations/{org_id}/dataset/{dataset_id}/metadata | Delete dataset metadata for the specified dataset
 *DatasetMetadataApi* | [**get_dataset_metadata**](docs/DatasetMetadataApi.md#get_dataset_metadata) | **GET** /v0/organizations/{org_id}/dataset/{dataset_id}/metadata | Get dataset metadata for the specified dataset
 *DatasetMetadataApi* | [**put_dataset_metadata**](docs/DatasetMetadataApi.md#put_dataset_metadata) | **PUT** /v0/organizations/{org_id}/dataset/{dataset_id}/metadata | Put dataset metadata for the specified dataset
 *FeatureWeightsApi* | [**get_column_weights**](docs/FeatureWeightsApi.md#get_column_weights) | **GET** /v0/organizations/{org_id}/dataset/{dataset_id}/weights | Get column weights for the specified dataset
 *FeatureWeightsApi* | [**put_column_weights**](docs/FeatureWeightsApi.md#put_column_weights) | **PUT** /v0/organizations/{org_id}/dataset/{dataset_id}/weights | Put column weights for the specified dataset
 *LogApi* | [**log_async**](docs/LogApi.md#log_async) | **POST** /v0/organizations/{org_id}/log/async/{dataset_id} | Like /log, except this api doesn&#39;t take the actual profile content. It returns an upload link that can be used to upload the profile to.
 *LogApi* | [**log_reference**](docs/LogApi.md#log_reference) | **POST** /v0/organizations/{org_id}/log/reference/{model_id} | Returns a presigned URL for uploading the reference profile to.
 *MembershipApi* | [**create_organization_membership**](docs/MembershipApi.md#create_organization_membership) | **POST** /v0/organizations/{org_id}/membership | Create a membership for a user, making them apart of an organization. Uses the user&#39;s current email address.
 *MembershipApi* | [**list_organization_memberships**](docs/MembershipApi.md#list_organization_memberships) | **GET** /v0/organizations/{org_id}/membership | List organization memberships
 *MembershipApi* | [**remove_organization_membership**](docs/MembershipApi.md#remove_organization_membership) | **DELETE** /v0/organizations/{org_id}/membership | Removes membership in a given org from a user, using the user&#39;s email address.
 *MembershipApi* | [**update_organization_membership**](docs/MembershipApi.md#update_organization_membership) | **PUT** /v0/organizations/{org_id}/membership | Updates the role in an membership
 *ModelsApi* | [**create_model**](docs/ModelsApi.md#create_model) | **POST** /v0/organizations/{org_id}/models | Create a model with a given name and a time period
 *ModelsApi* | [**deactivate_model**](docs/ModelsApi.md#deactivate_model) | **DELETE** /v0/organizations/{org_id}/models/{model_id} | Mark a model as inactive
+*ModelsApi* | [**delete_entity_schema**](docs/ModelsApi.md#delete_entity_schema) | **DELETE** /v0/organizations/{org_id}/models/{dataset_id}/schema | Delete the entity schema config for a given dataset.
 *ModelsApi* | [**delete_entity_schema_column**](docs/ModelsApi.md#delete_entity_schema_column) | **DELETE** /v0/organizations/{org_id}/models/{dataset_id}/schema/column/{column_id} | Delete the entity schema of a single column for a given dataset.
+*ModelsApi* | [**delete_entity_schema_metric**](docs/ModelsApi.md#delete_entity_schema_metric) | **DELETE** /v0/organizations/{org_id}/models/{dataset_id}/schema/metric/{metric_label} | Delete the schema of a single metric for a given dataset.
 *ModelsApi* | [**get_entity_schema**](docs/ModelsApi.md#get_entity_schema) | **GET** /v0/organizations/{org_id}/models/{dataset_id}/schema | Get the entity schema config for a given dataset.
 *ModelsApi* | [**get_entity_schema_column**](docs/ModelsApi.md#get_entity_schema_column) | **GET** /v0/organizations/{org_id}/models/{dataset_id}/schema/column/{column_id} | Get the entity schema of a single column for a given dataset.
 *ModelsApi* | [**get_model**](docs/ModelsApi.md#get_model) | **GET** /v0/organizations/{org_id}/models/{model_id} | Get a model metadata
 *ModelsApi* | [**list_models**](docs/ModelsApi.md#list_models) | **GET** /v0/organizations/{org_id}/models | Get a list of all of the model ids for an organization.
 *ModelsApi* | [**put_entity_schema**](docs/ModelsApi.md#put_entity_schema) | **PUT** /v0/organizations/{org_id}/models/{dataset_id}/schema | Save the entity schema config for a given dataset.
 *ModelsApi* | [**put_entity_schema_column**](docs/ModelsApi.md#put_entity_schema_column) | **PUT** /v0/organizations/{org_id}/models/{dataset_id}/schema/column/{column_id} | Save the entity schema of a single column for a given dataset.
+*ModelsApi* | [**put_entity_schema_metric**](docs/ModelsApi.md#put_entity_schema_metric) | **PUT** /v0/organizations/{org_id}/models/{dataset_id}/schema/metric | Save the schema of a single metric for a given dataset.
 *ModelsApi* | [**update_model**](docs/ModelsApi.md#update_model) | **PUT** /v0/organizations/{org_id}/models/{model_id} | Update a model&#39;s metadata
 *MonitorApi* | [**delete_analyzer**](docs/MonitorApi.md#delete_analyzer) | **DELETE** /v0/organizations/{org_id}/models/{dataset_id}/monitor-config/analyzer/{analyzer_id} | Delete the analyzer config for a given dataset.
 *MonitorApi* | [**delete_monitor**](docs/MonitorApi.md#delete_monitor) | **DELETE** /v0/organizations/{org_id}/models/{dataset_id}/monitor-config/monitor/{monitor_id} | Delete the monitor for a given dataset.
 *MonitorApi* | [**get_analyzer**](docs/MonitorApi.md#get_analyzer) | **GET** /v0/organizations/{org_id}/models/{dataset_id}/monitor-config/analyzer/{analyzer_id} | Get the analyzer config for a given dataset.
 *MonitorApi* | [**get_monitor**](docs/MonitorApi.md#get_monitor) | **GET** /v0/organizations/{org_id}/models/{dataset_id}/monitor-config/monitor/{monitor_id} | Get the monitor config for a given dataset.
 *MonitorApi* | [**get_monitor_config_v3**](docs/MonitorApi.md#get_monitor_config_v3) | **GET** /v0/organizations/{org_id}/models/{dataset_id}/monitor-config/v3 | Get the monitor config document for a given dataset.
 *MonitorApi* | [**patch_monitor_config_v3**](docs/MonitorApi.md#patch_monitor_config_v3) | **PATCH** /v0/organizations/{org_id}/models/{dataset_id}/monitor-config/v3 | Patch an updated monitor config document for a given dataset.
 *MonitorApi* | [**put_analyzer**](docs/MonitorApi.md#put_analyzer) | **PUT** /v0/organizations/{org_id}/models/{dataset_id}/monitor-config/analyzer/{analyzer_id} | Save the analyzer config for a given dataset.
 *MonitorApi* | [**put_monitor**](docs/MonitorApi.md#put_monitor) | **PUT** /v0/organizations/{org_id}/models/{dataset_id}/monitor-config/monitor/{monitor_id} | Save the monitor for a given dataset.
 *MonitorApi* | [**put_monitor_config_v3**](docs/MonitorApi.md#put_monitor_config_v3) | **PUT** /v0/organizations/{org_id}/models/{dataset_id}/monitor-config/v3 | Save the monitor config document for a given dataset.
 *MonitorApi* | [**validate_monitor_config_v3**](docs/MonitorApi.md#validate_monitor_config_v3) | **PUT** /v0/organizations/{org_id}/models/{dataset_id}/monitor-config/v3/validate | Validate the monitor config document for a given dataset.
+*NotificationSettingsApi* | [**add_notification_action**](docs/NotificationSettingsApi.md#add_notification_action) | **POST** /v0/notification-settings/{org_id}/actions/{type}/{action_id} | Add new notification action
 *NotificationSettingsApi* | [**delete_notification_action**](docs/NotificationSettingsApi.md#delete_notification_action) | **DELETE** /v0/notification-settings/{org_id}/actions/{action_id} | Delete notification action
 *NotificationSettingsApi* | [**get_email_notification_action_payload**](docs/NotificationSettingsApi.md#get_email_notification_action_payload) | **GET** /v0/notification-settings/actions/email/payload | Get dummy notification action payload
 *NotificationSettingsApi* | [**get_notification_action**](docs/NotificationSettingsApi.md#get_notification_action) | **GET** /v0/notification-settings/{org_id}/actions/{action_id} | Get notification action for id
 *NotificationSettingsApi* | [**get_pager_duty_notification_action_payload**](docs/NotificationSettingsApi.md#get_pager_duty_notification_action_payload) | **GET** /v0/notification-settings/actions/pagerduty/payload | Get dummy notification action payload
 *NotificationSettingsApi* | [**get_slack_notification_action_payload**](docs/NotificationSettingsApi.md#get_slack_notification_action_payload) | **GET** /v0/notification-settings/actions/slack/payload | Get dummy notification action payload
 *NotificationSettingsApi* | [**list_notification_actions**](docs/NotificationSettingsApi.md#list_notification_actions) | **GET** /v0/notification-settings/{org_id}/actions | List notification actions for an org
 *NotificationSettingsApi* | [**put_notification_action**](docs/NotificationSettingsApi.md#put_notification_action) | **PUT** /v0/notification-settings/{org_id}/actions/{type}/{action_id} | Add new notification action
 *NotificationSettingsApi* | [**test_notification_action**](docs/NotificationSettingsApi.md#test_notification_action) | **POST** /v0/notification-settings/{org_id}/actions/{action_id}/test | Test a notification action
 *NotificationSettingsApi* | [**update_notification_action**](docs/NotificationSettingsApi.md#update_notification_action) | **PATCH** /v0/notification-settings/{org_id}/actions/{type}/{action_id} | Update notification action
 *SchemaApi* | [**get_monitor_config_schema**](docs/SchemaApi.md#get_monitor_config_schema) | **GET** /v0/organizations/{org_id}/schema/monitor-config | Get the current supported schema of the monitor configuration
 *SessionsApi* | [**create_dataset_profile_upload**](docs/SessionsApi.md#create_dataset_profile_upload) | **POST** /v0/sessions/{session_id}/upload | Create an upload for a given session.
+*SessionsApi* | [**create_reference_profile_upload**](docs/SessionsApi.md#create_reference_profile_upload) | **POST** /v0/sessions/{session_id}/reference | Create a reference profile upload for a given session.
 *SessionsApi* | [**create_session**](docs/SessionsApi.md#create_session) | **POST** /v0/sessions | Create a new session that can be used to upload dataset profiles from whylogs for display in whylabs.
 *SessionsApi* | [**get_session**](docs/SessionsApi.md#get_session) | **GET** /v0/sessions/{session_id} | Get information about a session.
 
 
 ## Documentation For Models
 
  - [AWSMarketplaceMetadata](docs/AWSMarketplaceMetadata.md)
@@ -196,14 +203,15 @@
  - [LogAsyncRequest](docs/LogAsyncRequest.md)
  - [LogReferenceRequest](docs/LogReferenceRequest.md)
  - [LogReferenceResponse](docs/LogReferenceResponse.md)
  - [LogResponse](docs/LogResponse.md)
  - [MarketplaceDimensions](docs/MarketplaceDimensions.md)
  - [Membership](docs/Membership.md)
  - [MembershipMetadata](docs/MembershipMetadata.md)
+ - [MetricSchema](docs/MetricSchema.md)
  - [MissingRecentDataRequestConfig](docs/MissingRecentDataRequestConfig.md)
  - [MissingRecentProfilesRequestConfig](docs/MissingRecentProfilesRequestConfig.md)
  - [MissingValuesMonitorRequestConfig](docs/MissingValuesMonitorRequestConfig.md)
  - [ModelMetadataResponse](docs/ModelMetadataResponse.md)
  - [ModelType](docs/ModelType.md)
  - [MonitorConfig](docs/MonitorConfig.md)
  - [MonitorConfigVersion](docs/MonitorConfigVersion.md)
```

### Comparing `whylabs-client-0.4.4/setup.py` & `whylabs-client-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "whylabs-client"
-VERSION = "0.4.4"
+VERSION = "0.4.5"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `whylabs-client-0.4.4/whylabs_client/__init__.py` & `whylabs-client-0.4.5/whylabs_client/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 0.1
     Contact: support@whylabs.ai
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.4.4"
+__version__ = "0.4.5"
 
 # import ApiClient
 from whylabs_client.api_client import ApiClient
 
 # import Configuration
 from whylabs_client.configuration import Configuration
```

### Comparing `whylabs-client-0.4.4/whylabs_client/api/dataset_metadata_api.py` & `whylabs-client-0.4.5/whylabs_client/api/dataset_metadata_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/api/dataset_profile_api.py` & `whylabs-client-0.4.5/whylabs_client/api/dataset_profile_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from whylabs_client.model.delete_analyzer_results_response import DeleteAnalyzerResultsResponse
 from whylabs_client.model.delete_dataset_profiles_response import DeleteDatasetProfilesResponse
+from whylabs_client.model.reference_profile_item_response import ReferenceProfileItemResponse
 
 
 class DatasetProfileApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -177,14 +178,83 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.list_reference_profiles_endpoint = _Endpoint(
+            settings={
+                'response_type': ([ReferenceProfileItemResponse],),
+                'auth': [
+                    'ApiKeyAuth'
+                ],
+                'endpoint_path': '/v0/organizations/{org_id}/dataset-profiles/models/{model_id}/reference-profiles',
+                'operation_id': 'list_reference_profiles',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'org_id',
+                    'model_id',
+                    'from_epoch',
+                    'to_epoch',
+                ],
+                'required': [
+                    'org_id',
+                    'model_id',
+                ],
+                'nullable': [
+                    'from_epoch',
+                    'to_epoch',
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'org_id':
+                        (str,),
+                    'model_id':
+                        (str,),
+                    'from_epoch':
+                        (int, none_type,),
+                    'to_epoch':
+                        (int, none_type,),
+                },
+                'attribute_map': {
+                    'org_id': 'org_id',
+                    'model_id': 'model_id',
+                    'from_epoch': 'from_epoch',
+                    'to_epoch': 'to_epoch',
+                },
+                'location_map': {
+                    'org_id': 'path',
+                    'model_id': 'path',
+                    'from_epoch': 'query',
+                    'to_epoch': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
 
     def delete_analyzer_results(
         self,
         org_id,
         dataset_id,
         **kwargs
     ):
@@ -333,7 +403,84 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['org_id'] = \
             org_id
         kwargs['dataset_id'] = \
             dataset_id
         return self.delete_dataset_profiles_endpoint.call_with_http_info(**kwargs)
 
+    def list_reference_profiles(
+        self,
+        org_id,
+        model_id,
+        **kwargs
+    ):
+        """Returns a list for reference profiles  # noqa: E501
+
+        Returns a list of Reference Profiles.            # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.list_reference_profiles(org_id, model_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            org_id (str): Your company's unique organization ID
+            model_id (str): The unique model ID in your company.
+
+        Keyword Args:
+            from_epoch (int, none_type): Milli epoch time that represents the end of the time range to query.. [optional]
+            to_epoch (int, none_type): Milli epoch time that represents the end of the time range to query.. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            [ReferenceProfileItemResponse]
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
+        kwargs['model_id'] = \
+            model_id
+        return self.list_reference_profiles_endpoint.call_with_http_info(**kwargs)
+
```

### Comparing `whylabs-client-0.4.4/whylabs_client/api/feature_weights_api.py` & `whylabs-client-0.4.5/whylabs_client/api/feature_weights_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/api/log_api.py` & `whylabs-client-0.4.5/whylabs_client/api/log_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/api/membership_api.py` & `whylabs-client-0.4.5/whylabs_client/api/membership_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/api/models_api.py` & `whylabs-client-0.4.5/whylabs_client/api/models_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     file_type,
     none_type,
     validate_and_convert_types
 )
 from whylabs_client.model.column_schema import ColumnSchema
 from whylabs_client.model.entity_schema import EntitySchema
 from whylabs_client.model.list_models_response import ListModelsResponse
+from whylabs_client.model.metric_schema import MetricSchema
 from whylabs_client.model.model_metadata_response import ModelMetadataResponse
 from whylabs_client.model.model_type import ModelType
 from whylabs_client.model.response import Response
 from whylabs_client.model.time_period import TimePeriod
 
 
 class ModelsApi(object):
@@ -186,14 +187,71 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.delete_entity_schema_endpoint = _Endpoint(
+            settings={
+                'response_type': (Response,),
+                'auth': [
+                    'ApiKeyAuth'
+                ],
+                'endpoint_path': '/v0/organizations/{org_id}/models/{dataset_id}/schema',
+                'operation_id': 'delete_entity_schema',
+                'http_method': 'DELETE',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'org_id',
+                    'dataset_id',
+                ],
+                'required': [
+                    'org_id',
+                    'dataset_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'org_id':
+                        (str,),
+                    'dataset_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'org_id': 'org_id',
+                    'dataset_id': 'dataset_id',
+                },
+                'location_map': {
+                    'org_id': 'path',
+                    'dataset_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.delete_entity_schema_column_endpoint = _Endpoint(
             settings={
                 'response_type': (Response,),
                 'auth': [
                     'ApiKeyAuth'
                 ],
                 'endpoint_path': '/v0/organizations/{org_id}/models/{dataset_id}/schema/column/{column_id}',
@@ -249,14 +307,77 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.delete_entity_schema_metric_endpoint = _Endpoint(
+            settings={
+                'response_type': (Response,),
+                'auth': [
+                    'ApiKeyAuth'
+                ],
+                'endpoint_path': '/v0/organizations/{org_id}/models/{dataset_id}/schema/metric/{metric_label}',
+                'operation_id': 'delete_entity_schema_metric',
+                'http_method': 'DELETE',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'org_id',
+                    'dataset_id',
+                    'metric_label',
+                ],
+                'required': [
+                    'org_id',
+                    'dataset_id',
+                    'metric_label',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'org_id':
+                        (str,),
+                    'dataset_id':
+                        (str,),
+                    'metric_label':
+                        (str,),
+                },
+                'attribute_map': {
+                    'org_id': 'org_id',
+                    'dataset_id': 'dataset_id',
+                    'metric_label': 'metric_label',
+                },
+                'location_map': {
+                    'org_id': 'path',
+                    'dataset_id': 'path',
+                    'metric_label': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.get_entity_schema_endpoint = _Endpoint(
             settings={
                 'response_type': (EntitySchema,),
                 'auth': [
                     'ApiKeyAuth'
                 ],
                 'endpoint_path': '/v0/organizations/{org_id}/models/{dataset_id}/schema',
@@ -611,14 +732,78 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.put_entity_schema_metric_endpoint = _Endpoint(
+            settings={
+                'response_type': (Response,),
+                'auth': [
+                    'ApiKeyAuth'
+                ],
+                'endpoint_path': '/v0/organizations/{org_id}/models/{dataset_id}/schema/metric',
+                'operation_id': 'put_entity_schema_metric',
+                'http_method': 'PUT',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'org_id',
+                    'dataset_id',
+                    'metric_schema',
+                ],
+                'required': [
+                    'org_id',
+                    'dataset_id',
+                    'metric_schema',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'org_id':
+                        (str,),
+                    'dataset_id':
+                        (str,),
+                    'metric_schema':
+                        (MetricSchema,),
+                },
+                'attribute_map': {
+                    'org_id': 'org_id',
+                    'dataset_id': 'dataset_id',
+                },
+                'location_map': {
+                    'org_id': 'path',
+                    'dataset_id': 'path',
+                    'metric_schema': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.update_model_endpoint = _Endpoint(
             settings={
                 'response_type': (ModelMetadataResponse,),
                 'auth': [
                     'ApiKeyAuth'
                 ],
                 'endpoint_path': '/v0/organizations/{org_id}/models/{model_id}',
@@ -842,14 +1027,89 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['org_id'] = \
             org_id
         kwargs['model_id'] = \
             model_id
         return self.deactivate_model_endpoint.call_with_http_info(**kwargs)
 
+    def delete_entity_schema(
+        self,
+        org_id,
+        dataset_id,
+        **kwargs
+    ):
+        """Delete the entity schema config for a given dataset.  # noqa: E501
+
+        Delete the entity schema config for a given dataset.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_entity_schema(org_id, dataset_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            org_id (str):
+            dataset_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
+        kwargs['dataset_id'] = \
+            dataset_id
+        return self.delete_entity_schema_endpoint.call_with_http_info(**kwargs)
+
     def delete_entity_schema_column(
         self,
         org_id,
         dataset_id,
         column_id,
         **kwargs
     ):
@@ -921,14 +1181,93 @@
             org_id
         kwargs['dataset_id'] = \
             dataset_id
         kwargs['column_id'] = \
             column_id
         return self.delete_entity_schema_column_endpoint.call_with_http_info(**kwargs)
 
+    def delete_entity_schema_metric(
+        self,
+        org_id,
+        dataset_id,
+        metric_label,
+        **kwargs
+    ):
+        """Delete the schema of a single metric for a given dataset.  # noqa: E501
+
+        Delete the schema of a single metric for a given dataset.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_entity_schema_metric(org_id, dataset_id, metric_label, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            org_id (str):
+            dataset_id (str):
+            metric_label (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
+        kwargs['dataset_id'] = \
+            dataset_id
+        kwargs['metric_label'] = \
+            metric_label
+        return self.delete_entity_schema_metric_endpoint.call_with_http_info(**kwargs)
+
     def get_entity_schema(
         self,
         org_id,
         dataset_id,
         **kwargs
     ):
         """Get the entity schema config for a given dataset.  # noqa: E501
@@ -1383,14 +1722,93 @@
             dataset_id
         kwargs['column_id'] = \
             column_id
         kwargs['column_schema'] = \
             column_schema
         return self.put_entity_schema_column_endpoint.call_with_http_info(**kwargs)
 
+    def put_entity_schema_metric(
+        self,
+        org_id,
+        dataset_id,
+        metric_schema,
+        **kwargs
+    ):
+        """Save the schema of a single metric for a given dataset.  # noqa: E501
+
+        Save the schema of a single metric for a given dataset.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.put_entity_schema_metric(org_id, dataset_id, metric_schema, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            org_id (str):
+            dataset_id (str):
+            metric_schema (MetricSchema):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
+        kwargs['dataset_id'] = \
+            dataset_id
+        kwargs['metric_schema'] = \
+            metric_schema
+        return self.put_entity_schema_metric_endpoint.call_with_http_info(**kwargs)
+
     def update_model(
         self,
         org_id,
         model_id,
         model_name,
         time_period,
         **kwargs
```

### Comparing `whylabs-client-0.4.4/whylabs_client/api/monitor_api.py` & `whylabs-client-0.4.5/whylabs_client/api/monitor_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/api/notification_settings_api.py` & `whylabs-client-0.4.5/whylabs_client/api/notification_settings_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,84 @@
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
+        self.add_notification_action_endpoint = _Endpoint(
+            settings={
+                'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
+                'auth': [
+                    'ApiKeyAuth'
+                ],
+                'endpoint_path': '/v0/notification-settings/{org_id}/actions/{type}/{action_id}',
+                'operation_id': 'add_notification_action',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'org_id',
+                    'type',
+                    'action_id',
+                    'body',
+                ],
+                'required': [
+                    'org_id',
+                    'type',
+                    'action_id',
+                    'body',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'org_id':
+                        (str,),
+                    'type':
+                        (ActionType,),
+                    'action_id':
+                        (str,),
+                    'body':
+                        (str,),
+                },
+                'attribute_map': {
+                    'org_id': 'org_id',
+                    'type': 'type',
+                    'action_id': 'action_id',
+                },
+                'location_map': {
+                    'org_id': 'path',
+                    'type': 'path',
+                    'action_id': 'path',
+                    'body': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.delete_notification_action_endpoint = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'ApiKeyAuth'
                 ],
                 'endpoint_path': '/v0/notification-settings/{org_id}/actions/{action_id}',
@@ -531,14 +601,97 @@
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
 
+    def add_notification_action(
+        self,
+        org_id,
+        type,
+        action_id,
+        body,
+        **kwargs
+    ):
+        """Add new notification action  # noqa: E501
+
+        Add new notification action  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.add_notification_action(org_id, type, action_id, body, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            org_id (str):
+            type (ActionType):
+            action_id (str):
+            body (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
+        kwargs['type'] = \
+            type
+        kwargs['action_id'] = \
+            action_id
+        kwargs['body'] = \
+            body
+        return self.add_notification_action_endpoint.call_with_http_info(**kwargs)
+
     def delete_notification_action(
         self,
         org_id,
         action_id,
         **kwargs
     ):
         """Delete notification action  # noqa: E501
```

### Comparing `whylabs-client-0.4.4/whylabs_client/api/schema_api.py` & `whylabs-client-0.4.5/whylabs_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/api/sessions_api.py` & `whylabs-client-0.4.5/whylabs_client/api/sessions_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     validate_and_convert_types
 )
 from whylabs_client.model.async_log_response import AsyncLogResponse
 from whylabs_client.model.create_session_request import CreateSessionRequest
 from whylabs_client.model.create_session_response import CreateSessionResponse
 from whylabs_client.model.get_session_response import GetSessionResponse
 from whylabs_client.model.log_async_request import LogAsyncRequest
+from whylabs_client.model.log_reference_request import LogReferenceRequest
+from whylabs_client.model.log_reference_response import LogReferenceResponse
 
 
 class SessionsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -92,14 +94,70 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.create_reference_profile_upload_endpoint = _Endpoint(
+            settings={
+                'response_type': (LogReferenceResponse,),
+                'auth': [],
+                'endpoint_path': '/v0/sessions/{session_id}/reference',
+                'operation_id': 'create_reference_profile_upload',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'session_id',
+                    'log_reference_request',
+                ],
+                'required': [
+                    'session_id',
+                    'log_reference_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'session_id':
+                        (str,),
+                    'log_reference_request':
+                        (LogReferenceRequest,),
+                },
+                'attribute_map': {
+                    'session_id': 'session_id',
+                },
+                'location_map': {
+                    'session_id': 'path',
+                    'log_reference_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.create_session_endpoint = _Endpoint(
             settings={
                 'response_type': (CreateSessionResponse,),
                 'auth': [],
                 'endpoint_path': '/v0/sessions',
                 'operation_id': 'create_session',
                 'http_method': 'POST',
@@ -269,14 +327,89 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['session_id'] = \
             session_id
         kwargs['log_async_request'] = \
             log_async_request
         return self.create_dataset_profile_upload_endpoint.call_with_http_info(**kwargs)
 
+    def create_reference_profile_upload(
+        self,
+        session_id,
+        log_reference_request,
+        **kwargs
+    ):
+        """Create a reference profile upload for a given session.  # noqa: E501
+
+        Create a reference profile upload for a given session.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_reference_profile_upload(session_id, log_reference_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            session_id (str):
+            log_reference_request (LogReferenceRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            LogReferenceResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['session_id'] = \
+            session_id
+        kwargs['log_reference_request'] = \
+            log_reference_request
+        return self.create_reference_profile_upload_endpoint.call_with_http_info(**kwargs)
+
     def create_session(
         self,
         create_session_request,
         **kwargs
     ):
         """Create a new session that can be used to upload dataset profiles from whylogs for display in whylabs.  # noqa: E501
```

### Comparing `whylabs-client-0.4.4/whylabs_client/api_client.py` & `whylabs-client-0.4.5/whylabs_client/api_client.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/apis/__init__.py` & `whylabs-client-0.4.5/whylabs_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/configuration.py` & `whylabs-client-0.4.5/whylabs_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -406,15 +406,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1\n"\
-               "SDK Package Version: 0.4.4".\
+               "SDK Package Version: 0.4.5".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `whylabs-client-0.4.4/whylabs_client/exceptions.py` & `whylabs-client-0.4.5/whylabs_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/action_type.py` & `whylabs-client-0.4.5/whylabs_client/model/action_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/add_membership_request.py` & `whylabs-client-0.4.5/whylabs_client/model/add_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/async_log_response.py` & `whylabs-client-0.4.5/whylabs_client/model/async_log_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/aws_marketplace_metadata.py` & `whylabs-client-0.4.5/whylabs_client/model/aws_marketplace_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/column_schema.py` & `whylabs-client-0.4.5/whylabs_client/model/column_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/create_session_request.py` & `whylabs-client-0.4.5/whylabs_client/model/create_session_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/create_session_response.py` & `whylabs-client-0.4.5/whylabs_client/model/create_session_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/create_user_request.py` & `whylabs-client-0.4.5/whylabs_client/model/create_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/databricks_connection.py` & `whylabs-client-0.4.5/whylabs_client/model/databricks_connection.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/dataset_request_monitor_config.py` & `whylabs-client-0.4.5/whylabs_client/model/dataset_request_monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/datatype_monitor_request_config.py` & `whylabs-client-0.4.5/whylabs_client/model/datatype_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/delete_analyzer_results_response.py` & `whylabs-client-0.4.5/whylabs_client/model/delete_analyzer_results_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/delete_dataset_profiles_response.py` & `whylabs-client-0.4.5/whylabs_client/model/delete_dataset_profiles_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/distribution_monitor_request_config.py` & `whylabs-client-0.4.5/whylabs_client/model/distribution_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/dto_auto_scale_dto.py` & `whylabs-client-0.4.5/whylabs_client/model/dto_auto_scale_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/dto_aws_attributes_dto.py` & `whylabs-client-0.4.5/whylabs_client/model/dto_aws_attributes_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/dto_aws_availability_dto.py` & `whylabs-client-0.4.5/whylabs_client/model/dto_aws_availability_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/dto_cluster_log_conf_dto.py` & `whylabs-client-0.4.5/whylabs_client/model/dto_cluster_log_conf_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/dto_cron_schedule_dto.py` & `whylabs-client-0.4.5/whylabs_client/model/dto_cron_schedule_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/dto_dbfs_storage_info_dto.py` & `whylabs-client-0.4.5/whylabs_client/model/dto_dbfs_storage_info_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/dto_ebs_volume_type_dto.py` & `whylabs-client-0.4.5/whylabs_client/model/dto_ebs_volume_type_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/dto_job_dto.py` & `whylabs-client-0.4.5/whylabs_client/model/dto_job_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/dto_job_email_notifications_dto.py` & `whylabs-client-0.4.5/whylabs_client/model/dto_job_email_notifications_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/dto_job_settings_dto.py` & `whylabs-client-0.4.5/whylabs_client/model/dto_job_settings_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/dto_new_cluster_dto.py` & `whylabs-client-0.4.5/whylabs_client/model/dto_new_cluster_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/dto_notebook_task_dto.py` & `whylabs-client-0.4.5/whylabs_client/model/dto_notebook_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/dto_spark_jar_task_dto.py` & `whylabs-client-0.4.5/whylabs_client/model/dto_spark_jar_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/dto_spark_python_task_dto.py` & `whylabs-client-0.4.5/whylabs_client/model/dto_spark_python_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/dto_spark_submit_task_dto.py` & `whylabs-client-0.4.5/whylabs_client/model/dto_spark_submit_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/dtos3_storage_info_dto.py` & `whylabs-client-0.4.5/whylabs_client/model/dtos3_storage_info_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/email_notification_action.py` & `whylabs-client-0.4.5/whylabs_client/model/email_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/entity_schema.py` & `whylabs-client-0.4.5/whylabs_client/model/get_dataset_metadata_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,22 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from whylabs_client.model.column_schema import ColumnSchema
-    from whylabs_client.model.schema_metadata import SchemaMetadata
-    globals()['ColumnSchema'] = ColumnSchema
-    globals()['SchemaMetadata'] = SchemaMetadata
 
-
-class EntitySchema(ModelNormal):
+class GetDatasetMetadataResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -69,57 +63,53 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'columns': ({str: (ColumnSchema,)},),  # noqa: E501
-            'metadata': (SchemaMetadata,),  # noqa: E501
+            'metadata': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'columns': 'columns',  # noqa: E501
         'metadata': 'metadata',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, columns, *args, **kwargs):  # noqa: E501
-        """EntitySchema - a model defined in OpenAPI
+    def _from_openapi_data(cls, metadata, *args, **kwargs):  # noqa: E501
+        """GetDatasetMetadataResponse - a model defined in OpenAPI
 
         Args:
-            columns ({str: (ColumnSchema,)}): Column schema for a given column
+            metadata (str): Metadata information for the dataset
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -144,15 +134,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            metadata (SchemaMetadata): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -172,15 +161,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.columns = columns
+        self.metadata = metadata
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -193,19 +182,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, columns, *args, **kwargs):  # noqa: E501
-        """EntitySchema - a model defined in OpenAPI
+    def __init__(self, metadata, *args, **kwargs):  # noqa: E501
+        """GetDatasetMetadataResponse - a model defined in OpenAPI
 
         Args:
-            columns ({str: (ColumnSchema,)}): Column schema for a given column
+            metadata (str): Metadata information for the dataset
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -230,15 +219,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            metadata (SchemaMetadata): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -256,15 +244,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.columns = columns
+        self.metadata = metadata
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.4.4/whylabs_client/model/entity_weight_record.py` & `whylabs-client-0.4.5/whylabs_client/model/entity_weight_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/entity_weight_record_metadata.py` & `whylabs-client-0.4.5/whylabs_client/model/entity_weight_record_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/feature_flags.py` & `whylabs-client-0.4.5/whylabs_client/model/feature_flags.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/get_connection_request.py` & `whylabs-client-0.4.5/whylabs_client/model/get_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/get_connection_response.py` & `whylabs-client-0.4.5/whylabs_client/model/get_connection_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/get_dataset_metadata_response.py` & `whylabs-client-0.4.5/whylabs_client/model/get_marketplace_metadata_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from whylabs_client.model.aws_marketplace_metadata import AWSMarketplaceMetadata
+    globals()['AWSMarketplaceMetadata'] = AWSMarketplaceMetadata
 
-class GetDatasetMetadataResponse(ModelNormal):
+
+class GetMarketplaceMetadataResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,30 +67,32 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'metadata': (str,),  # noqa: E501
+            'metadata': (AWSMarketplaceMetadata,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -98,18 +104,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, metadata, *args, **kwargs):  # noqa: E501
-        """GetDatasetMetadataResponse - a model defined in OpenAPI
+        """GetMarketplaceMetadataResponse - a model defined in OpenAPI
 
         Args:
-            metadata (str): Metadata information for the dataset
+            metadata (AWSMarketplaceMetadata):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -183,18 +189,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, metadata, *args, **kwargs):  # noqa: E501
-        """GetDatasetMetadataResponse - a model defined in OpenAPI
+        """GetMarketplaceMetadataResponse - a model defined in OpenAPI
 
         Args:
-            metadata (str): Metadata information for the dataset
+            metadata (AWSMarketplaceMetadata):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `whylabs-client-0.4.4/whylabs_client/model/get_default_membership_response.py` & `whylabs-client-0.4.5/whylabs_client/model/get_default_membership_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/get_marketplace_metadata_response.py` & `whylabs-client-0.4.5/whylabs_client/model/refresh_access_token_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from whylabs_client.model.aws_marketplace_metadata import AWSMarketplaceMetadata
-    globals()['AWSMarketplaceMetadata'] = AWSMarketplaceMetadata
 
-
-class GetMarketplaceMetadataResponse(ModelNormal):
+class RefreshAccessTokenRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,55 +63,53 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'metadata': (AWSMarketplaceMetadata,),  # noqa: E501
+            'workspace_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'metadata': 'metadata',  # noqa: E501
+        'workspace_id': 'workspaceId',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, metadata, *args, **kwargs):  # noqa: E501
-        """GetMarketplaceMetadataResponse - a model defined in OpenAPI
+    def _from_openapi_data(cls, workspace_id, *args, **kwargs):  # noqa: E501
+        """RefreshAccessTokenRequest - a model defined in OpenAPI
 
         Args:
-            metadata (AWSMarketplaceMetadata):
+            workspace_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -167,15 +161,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.metadata = metadata
+        self.workspace_id = workspace_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -188,19 +182,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, metadata, *args, **kwargs):  # noqa: E501
-        """GetMarketplaceMetadataResponse - a model defined in OpenAPI
+    def __init__(self, workspace_id, *args, **kwargs):  # noqa: E501
+        """RefreshAccessTokenRequest - a model defined in OpenAPI
 
         Args:
-            metadata (AWSMarketplaceMetadata):
+            workspace_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -250,15 +244,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.metadata = metadata
+        self.workspace_id = workspace_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.4.4/whylabs_client/model/get_memberships_response.py` & `whylabs-client-0.4.5/whylabs_client/model/get_memberships_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/get_monitor_config_v2_response.py` & `whylabs-client-0.4.5/whylabs_client/model/get_monitor_config_v2_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/get_notification_settings_response.py` & `whylabs-client-0.4.5/whylabs_client/model/get_notification_settings_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/get_session_response.py` & `whylabs-client-0.4.5/whylabs_client/model/get_session_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/list_jobs_request.py` & `whylabs-client-0.4.5/whylabs_client/model/list_jobs_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/list_jobs_response.py` & `whylabs-client-0.4.5/whylabs_client/model/list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/list_models_response.py` & `whylabs-client-0.4.5/whylabs_client/model/list_models_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/list_organization_memberships_response.py` & `whylabs-client-0.4.5/whylabs_client/model/list_organization_memberships_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/list_user_api_keys.py` & `whylabs-client-0.4.5/whylabs_client/model/list_user_api_keys.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/log_async_request.py` & `whylabs-client-0.4.5/whylabs_client/model/log_async_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/log_reference_request.py` & `whylabs-client-0.4.5/whylabs_client/model/log_reference_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/log_reference_response.py` & `whylabs-client-0.4.5/whylabs_client/model/log_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/log_response.py` & `whylabs-client-0.4.5/whylabs_client/model/log_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/marketplace_dimensions.py` & `whylabs-client-0.4.5/whylabs_client/model/marketplace_dimensions.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/membership.py` & `whylabs-client-0.4.5/whylabs_client/model/membership.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/membership_metadata.py` & `whylabs-client-0.4.5/whylabs_client/model/membership_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/missing_recent_data_request_config.py` & `whylabs-client-0.4.5/whylabs_client/model/missing_recent_data_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/missing_recent_profiles_request_config.py` & `whylabs-client-0.4.5/whylabs_client/model/missing_recent_profiles_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/missing_values_monitor_request_config.py` & `whylabs-client-0.4.5/whylabs_client/model/missing_values_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/model_metadata_response.py` & `whylabs-client-0.4.5/whylabs_client/model/reference_profile_item_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class ModelMetadataResponse(ModelNormal):
+class ReferenceProfileItemResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,49 +78,47 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str,),  # noqa: E501
             'org_id': (str,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'creation_time': (int,),  # noqa: E501
-            'time_period': (str,),  # noqa: E501
-            'model_type': (str, none_type,),  # noqa: E501
-            'model_category': (str,),  # noqa: E501
-            'active': (bool, none_type,),  # noqa: E501
+            'model_id': (str,),  # noqa: E501
+            'alias': (str,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'upload_timestamp': (int,),  # noqa: E501
+            'dataset_timestamp': (int, none_type,),  # noqa: E501
+            'path': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
         'org_id': 'orgId',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'creation_time': 'creationTime',  # noqa: E501
-        'time_period': 'timePeriod',  # noqa: E501
-        'model_type': 'modelType',  # noqa: E501
-        'model_category': 'modelCategory',  # noqa: E501
-        'active': 'active',  # noqa: E501
+        'model_id': 'modelId',  # noqa: E501
+        'alias': 'alias',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'upload_timestamp': 'uploadTimestamp',  # noqa: E501
+        'dataset_timestamp': 'datasetTimestamp',  # noqa: E501
+        'path': 'path',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ModelMetadataResponse - a model defined in OpenAPI
+        """ReferenceProfileItemResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -145,22 +143,21 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
             org_id (str): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            creation_time (int): [optional]  # noqa: E501
-            time_period (str): [optional]  # noqa: E501
-            model_type (str, none_type): [optional]  # noqa: E501
-            model_category (str): [optional]  # noqa: E501
-            active (bool, none_type): [optional]  # noqa: E501
+            model_id (str): [optional]  # noqa: E501
+            alias (str): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            upload_timestamp (int): [optional]  # noqa: E501
+            dataset_timestamp (int, none_type): [optional]  # noqa: E501
+            path (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -201,15 +198,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ModelMetadataResponse - a model defined in OpenAPI
+        """ReferenceProfileItemResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -234,22 +231,21 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
             org_id (str): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            creation_time (int): [optional]  # noqa: E501
-            time_period (str): [optional]  # noqa: E501
-            model_type (str, none_type): [optional]  # noqa: E501
-            model_category (str): [optional]  # noqa: E501
-            active (bool, none_type): [optional]  # noqa: E501
+            model_id (str): [optional]  # noqa: E501
+            alias (str): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            upload_timestamp (int): [optional]  # noqa: E501
+            dataset_timestamp (int, none_type): [optional]  # noqa: E501
+            path (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `whylabs-client-0.4.4/whylabs_client/model/model_type.py` & `whylabs-client-0.4.5/whylabs_client/model/model_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/monitor_config.py` & `whylabs-client-0.4.5/whylabs_client/model/monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/monitor_config_version.py` & `whylabs-client-0.4.5/whylabs_client/model/monitor_config_version.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/monitor_request_reference.py` & `whylabs-client-0.4.5/whylabs_client/model/monitor_request_reference.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/monitor_request_reference_type.py` & `whylabs-client-0.4.5/whylabs_client/model/monitor_request_reference_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/notification_action.py` & `whylabs-client-0.4.5/whylabs_client/model/notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/notification_settings.py` & `whylabs-client-0.4.5/whylabs_client/model/notification_settings.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/notification_settings_day.py` & `whylabs-client-0.4.5/whylabs_client/model/notification_settings_day.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/notification_sqs_message_cadence.py` & `whylabs-client-0.4.5/whylabs_client/model/notification_sqs_message_cadence.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/organization_metadata.py` & `whylabs-client-0.4.5/whylabs_client/model/organization_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/organization_summary.py` & `whylabs-client-0.4.5/whylabs_client/model/organization_summary.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/pager_duty_notification_action.py` & `whylabs-client-0.4.5/whylabs_client/model/pager_duty_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/provided_config.py` & `whylabs-client-0.4.5/whylabs_client/model/provided_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/provision_databricks_connection_request.py` & `whylabs-client-0.4.5/whylabs_client/model/provision_databricks_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/provision_databricks_connection_response.py` & `whylabs-client-0.4.5/whylabs_client/model/provision_databricks_connection_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/provision_new_aws_marketplace_user_response.py` & `whylabs-client-0.4.5/whylabs_client/model/provision_new_aws_marketplace_user_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/provision_new_marketplace_user_request.py` & `whylabs-client-0.4.5/whylabs_client/model/provision_new_marketplace_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/provision_new_user_request.py` & `whylabs-client-0.4.5/whylabs_client/model/provision_new_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/provision_new_user_response.py` & `whylabs-client-0.4.5/whylabs_client/model/provision_new_user_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/reference_profile_item_response.py` & `whylabs-client-0.4.5/whylabs_client/model/update_connection_changes.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class ReferenceProfileItemResponse(ModelNormal):
+class UpdateConnectionChanges(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,47 +78,39 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'org_id': (str,),  # noqa: E501
-            'model_id': (str,),  # noqa: E501
-            'alias': (str,),  # noqa: E501
-            'id': (str,),  # noqa: E501
-            'upload_timestamp': (int,),  # noqa: E501
-            'dataset_timestamp': (int, none_type,),  # noqa: E501
-            'path': (str,),  # noqa: E501
+            'org_id': (str, none_type,),  # noqa: E501
+            'connected': (bool, none_type,),  # noqa: E501
+            'demo': (bool, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'org_id': 'orgId',  # noqa: E501
-        'model_id': 'modelId',  # noqa: E501
-        'alias': 'alias',  # noqa: E501
-        'id': 'id',  # noqa: E501
-        'upload_timestamp': 'uploadTimestamp',  # noqa: E501
-        'dataset_timestamp': 'datasetTimestamp',  # noqa: E501
-        'path': 'path',  # noqa: E501
+        'connected': 'connected',  # noqa: E501
+        'demo': 'demo',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ReferenceProfileItemResponse - a model defined in OpenAPI
+        """UpdateConnectionChanges - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,21 +135,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            org_id (str): [optional]  # noqa: E501
-            model_id (str): [optional]  # noqa: E501
-            alias (str): [optional]  # noqa: E501
-            id (str): [optional]  # noqa: E501
-            upload_timestamp (int): [optional]  # noqa: E501
-            dataset_timestamp (int, none_type): [optional]  # noqa: E501
-            path (str): [optional]  # noqa: E501
+            org_id (str, none_type): [optional]  # noqa: E501
+            connected (bool, none_type): [optional]  # noqa: E501
+            demo (bool, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -198,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ReferenceProfileItemResponse - a model defined in OpenAPI
+        """UpdateConnectionChanges - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -231,21 +219,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            org_id (str): [optional]  # noqa: E501
-            model_id (str): [optional]  # noqa: E501
-            alias (str): [optional]  # noqa: E501
-            id (str): [optional]  # noqa: E501
-            upload_timestamp (int): [optional]  # noqa: E501
-            dataset_timestamp (int, none_type): [optional]  # noqa: E501
-            path (str): [optional]  # noqa: E501
+            org_id (str, none_type): [optional]  # noqa: E501
+            connected (bool, none_type): [optional]  # noqa: E501
+            demo (bool, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `whylabs-client-0.4.4/whylabs_client/model/refresh_access_token_request.py` & `whylabs-client-0.4.5/whylabs_client/model/run_job_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class RefreshAccessTokenRequest(ModelNormal):
+class RunJobResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,38 +78,38 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'workspace_id': (str,),  # noqa: E501
+            'run_id': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'workspace_id': 'workspaceId',  # noqa: E501
+        'run_id': 'runId',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, workspace_id, *args, **kwargs):  # noqa: E501
-        """RefreshAccessTokenRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, run_id, *args, **kwargs):  # noqa: E501
+        """RunJobResponse - a model defined in OpenAPI
 
         Args:
-            workspace_id (str):
+            run_id (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -161,15 +161,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.workspace_id = workspace_id
+        self.run_id = run_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -182,19 +182,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, workspace_id, *args, **kwargs):  # noqa: E501
-        """RefreshAccessTokenRequest - a model defined in OpenAPI
+    def __init__(self, run_id, *args, **kwargs):  # noqa: E501
+        """RunJobResponse - a model defined in OpenAPI
 
         Args:
-            workspace_id (str):
+            run_id (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -244,15 +244,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.workspace_id = workspace_id
+        self.run_id = run_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.4.4/whylabs_client/model/refresh_connection_by_org_id_response.py` & `whylabs-client-0.4.5/whylabs_client/model/refresh_connection_by_org_id_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/refresh_connection_request.py` & `whylabs-client-0.4.5/whylabs_client/model/refresh_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/register_databricks_connection_request.py` & `whylabs-client-0.4.5/whylabs_client/model/register_databricks_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/register_databricks_connection_response.py` & `whylabs-client-0.4.5/whylabs_client/model/register_databricks_connection_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/remove_membership_request.py` & `whylabs-client-0.4.5/whylabs_client/model/remove_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/request_feature_monitor_config.py` & `whylabs-client-0.4.5/whylabs_client/model/request_feature_monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/request_monitor_config.py` & `whylabs-client-0.4.5/whylabs_client/model/request_monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/response.py` & `whylabs-client-0.4.5/whylabs_client/model/response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/role.py` & `whylabs-client-0.4.5/whylabs_client/model/role.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/run_job_request.py` & `whylabs-client-0.4.5/whylabs_client/model/run_job_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/run_job_response.py` & `whylabs-client-0.4.5/whylabs_client/model/segment.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from whylabs_client.model.segment_tag import SegmentTag
+    globals()['SegmentTag'] = SegmentTag
 
-class RunJobResponse(ModelNormal):
+
+class Segment(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,53 +67,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'run_id': (int,),  # noqa: E501
+            'tags': ([SegmentTag],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'run_id': 'runId',  # noqa: E501
+        'tags': 'tags',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, run_id, *args, **kwargs):  # noqa: E501
-        """RunJobResponse - a model defined in OpenAPI
-
-        Args:
-            run_id (int):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """Segment - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,14 +137,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            tags ([SegmentTag]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -161,15 +165,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.run_id = run_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -182,19 +185,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, run_id, *args, **kwargs):  # noqa: E501
-        """RunJobResponse - a model defined in OpenAPI
-
-        Args:
-            run_id (int):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """Segment - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,14 +219,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            tags ([SegmentTag]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -244,15 +245,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.run_id = run_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.4.4/whylabs_client/model/schema_metadata.py` & `whylabs-client-0.4.5/whylabs_client/model/schema_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/seasonal_arima_request_config.py` & `whylabs-client-0.4.5/whylabs_client/model/seasonal_arima_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/segment.py` & `whylabs-client-0.4.5/whylabs_client/model/segment_weight.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from whylabs_client.model.segment_tag import SegmentTag
-    globals()['SegmentTag'] = SegmentTag
+    from whylabs_client.model.segment import Segment
+    globals()['Segment'] = Segment
 
 
-class Segment(ModelNormal):
+class SegmentWeight(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,35 +84,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'tags': ([SegmentTag],),  # noqa: E501
+            'segment': (Segment,),  # noqa: E501
+            'weights': ({str: (float,)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'tags': 'tags',  # noqa: E501
+        'segment': 'segment',  # noqa: E501
+        'weights': 'weights',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Segment - a model defined in OpenAPI
+        """SegmentWeight - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,15 +139,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            tags ([SegmentTag]): [optional]  # noqa: E501
+            segment (Segment): [optional]  # noqa: E501
+            weights ({str: (float,)}): Entity weight value for each entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +189,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Segment - a model defined in OpenAPI
+        """SegmentWeight - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,15 +222,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            tags ([SegmentTag]): [optional]  # noqa: E501
+            segment (Segment): [optional]  # noqa: E501
+            weights ({str: (float,)}): Entity weight value for each entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `whylabs-client-0.4.4/whylabs_client/model/segment_tag.py` & `whylabs-client-0.4.5/whylabs_client/model/segment_tag.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/segment_weight.py` & `whylabs-client-0.4.5/whylabs_client/model/set_default_membership_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from whylabs_client.model.segment import Segment
-    globals()['Segment'] = Segment
 
-
-class SegmentWeight(ModelNormal):
+class SetDefaultMembershipRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,54 +63,56 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'segment': (Segment,),  # noqa: E501
-            'weights': ({str: (float,)},),  # noqa: E501
+            'org_id': (str,),  # noqa: E501
+            'user_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'segment': 'segment',  # noqa: E501
-        'weights': 'weights',  # noqa: E501
+        'org_id': 'orgId',  # noqa: E501
+        'user_id': 'userId',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SegmentWeight - a model defined in OpenAPI
+    def _from_openapi_data(cls, org_id, user_id, *args, **kwargs):  # noqa: E501
+        """SetDefaultMembershipRequest - a model defined in OpenAPI
+
+        Args:
+            org_id (str):
+            user_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,16 +137,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            segment (Segment): [optional]  # noqa: E501
-            weights ({str: (float,)}): Entity weight value for each entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -168,14 +164,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.org_id = org_id
+        self.user_id = user_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -188,16 +186,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """SegmentWeight - a model defined in OpenAPI
+    def __init__(self, org_id, user_id, *args, **kwargs):  # noqa: E501
+        """SetDefaultMembershipRequest - a model defined in OpenAPI
+
+        Args:
+            org_id (str):
+            user_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,16 +224,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            segment (Segment): [optional]  # noqa: E501
-            weights ({str: (float,)}): Entity weight value for each entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -249,14 +249,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.org_id = org_id
+        self.user_id = user_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.4.4/whylabs_client/model/session_metadata.py` & `whylabs-client-0.4.5/whylabs_client/model/session_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/set_default_membership_request.py` & `whylabs-client-0.4.5/whylabs_client/model/update_membership_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from whylabs_client.model.role import Role
+    globals()['Role'] = Role
 
-class SetDefaultMembershipRequest(ModelNormal):
+
+class UpdateMembershipRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,56 +67,61 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
             'org_id': (str,),  # noqa: E501
-            'user_id': (str,),  # noqa: E501
+            'email': (str,),  # noqa: E501
+            'role': (Role,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'org_id': 'orgId',  # noqa: E501
-        'user_id': 'userId',  # noqa: E501
+        'email': 'email',  # noqa: E501
+        'role': 'role',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, org_id, user_id, *args, **kwargs):  # noqa: E501
-        """SetDefaultMembershipRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, org_id, email, role, *args, **kwargs):  # noqa: E501
+        """UpdateMembershipRequest - a model defined in OpenAPI
 
         Args:
             org_id (str):
-            user_id (str):
+            email (str):
+            role (Role):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -165,15 +174,16 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.org_id = org_id
-        self.user_id = user_id
+        self.email = email
+        self.role = role
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,20 +196,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, org_id, user_id, *args, **kwargs):  # noqa: E501
-        """SetDefaultMembershipRequest - a model defined in OpenAPI
+    def __init__(self, org_id, email, role, *args, **kwargs):  # noqa: E501
+        """UpdateMembershipRequest - a model defined in OpenAPI
 
         Args:
             org_id (str):
-            user_id (str):
+            email (str):
+            role (Role):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -250,15 +261,16 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.org_id = org_id
-        self.user_id = user_id
+        self.email = email
+        self.role = role
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.4.4/whylabs_client/model/slack_notification_action.py` & `whylabs-client-0.4.5/whylabs_client/model/slack_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/subscription_tier.py` & `whylabs-client-0.4.5/whylabs_client/model/subscription_tier.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/time_period.py` & `whylabs-client-0.4.5/whylabs_client/model/time_period.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/uber_notification_schedule.py` & `whylabs-client-0.4.5/whylabs_client/model/uber_notification_schedule.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/unique_values_monitor_request_config.py` & `whylabs-client-0.4.5/whylabs_client/model/unique_values_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/update_connection_changes.py` & `whylabs-client-0.4.5/whylabs_client/model/user_api_key_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from whylabs_client.model.user_api_key import UserApiKey
+    globals()['UserApiKey'] = UserApiKey
 
-class UpdateConnectionChanges(ModelNormal):
+
+class UserApiKeyResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,54 +67,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'org_id': (str, none_type,),  # noqa: E501
-            'connected': (bool, none_type,),  # noqa: E501
-            'demo': (bool, none_type,),  # noqa: E501
+            'key': (UserApiKey,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'org_id': 'orgId',  # noqa: E501
-        'connected': 'connected',  # noqa: E501
-        'demo': 'demo',  # noqa: E501
+        'key': 'key',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UpdateConnectionChanges - a model defined in OpenAPI
+        """UserApiKeyResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,17 +137,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            org_id (str, none_type): [optional]  # noqa: E501
-            connected (bool, none_type): [optional]  # noqa: E501
-            demo (bool, none_type): [optional]  # noqa: E501
+            key (UserApiKey): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """UpdateConnectionChanges - a model defined in OpenAPI
+        """UserApiKeyResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,17 +219,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            org_id (str, none_type): [optional]  # noqa: E501
-            connected (bool, none_type): [optional]  # noqa: E501
-            demo (bool, none_type): [optional]  # noqa: E501
+            key (UserApiKey): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `whylabs-client-0.4.4/whylabs_client/model/update_connection_request.py` & `whylabs-client-0.4.5/whylabs_client/model/update_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/update_membership_request.py` & `whylabs-client-0.4.5/whylabs_client/model/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from whylabs_client.model.role import Role
-    globals()['Role'] = Role
 
-
-class UpdateMembershipRequest(ModelNormal):
+class User(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,61 +63,58 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'org_id': (str,),  # noqa: E501
+            'user_id': (str,),  # noqa: E501
             'email': (str,),  # noqa: E501
-            'role': (Role,),  # noqa: E501
+            'preferences': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'org_id': 'orgId',  # noqa: E501
+        'user_id': 'userId',  # noqa: E501
         'email': 'email',  # noqa: E501
-        'role': 'role',  # noqa: E501
+        'preferences': 'preferences',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, org_id, email, role, *args, **kwargs):  # noqa: E501
-        """UpdateMembershipRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, user_id, email, *args, **kwargs):  # noqa: E501
+        """User - a model defined in OpenAPI
 
         Args:
-            org_id (str):
-            email (str):
-            role (Role):
+            user_id (str): The id of the user.
+            email (str): The user's email address.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -146,14 +139,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            preferences (str, none_type): The user's JSON serialized preferences. Schema defined in Dashbird.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -173,17 +167,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.org_id = org_id
+        self.user_id = user_id
         self.email = email
-        self.role = role
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -196,21 +189,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, org_id, email, role, *args, **kwargs):  # noqa: E501
-        """UpdateMembershipRequest - a model defined in OpenAPI
+    def __init__(self, user_id, email, *args, **kwargs):  # noqa: E501
+        """User - a model defined in OpenAPI
 
         Args:
-            org_id (str):
-            email (str):
-            role (Role):
+            user_id (str): The id of the user.
+            email (str): The user's email address.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -235,14 +227,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            preferences (str, none_type): The user's JSON serialized preferences. Schema defined in Dashbird.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -260,17 +253,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.org_id = org_id
+        self.user_id = user_id
         self.email = email
-        self.role = role
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.4.4/whylabs_client/model/user.py` & `whylabs-client-0.4.5/whylabs_client/model/entity_schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,16 +26,24 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from whylabs_client.model.column_schema import ColumnSchema
+    from whylabs_client.model.metric_schema import MetricSchema
+    from whylabs_client.model.schema_metadata import SchemaMetadata
+    globals()['ColumnSchema'] = ColumnSchema
+    globals()['MetricSchema'] = MetricSchema
+    globals()['SchemaMetadata'] = SchemaMetadata
 
-class User(ModelNormal):
+
+class EntitySchema(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,58 +71,59 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'user_id': (str,),  # noqa: E501
-            'email': (str,),  # noqa: E501
-            'preferences': (str, none_type,),  # noqa: E501
+            'columns': ({str: (ColumnSchema,)},),  # noqa: E501
+            'metadata': (SchemaMetadata,),  # noqa: E501
+            'metrics': ({str: (MetricSchema,)}, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'user_id': 'userId',  # noqa: E501
-        'email': 'email',  # noqa: E501
-        'preferences': 'preferences',  # noqa: E501
+        'columns': 'columns',  # noqa: E501
+        'metadata': 'metadata',  # noqa: E501
+        'metrics': 'metrics',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, user_id, email, *args, **kwargs):  # noqa: E501
-        """User - a model defined in OpenAPI
+    def _from_openapi_data(cls, columns, *args, **kwargs):  # noqa: E501
+        """EntitySchema - a model defined in OpenAPI
 
         Args:
-            user_id (str): The id of the user.
-            email (str): The user's email address.
+            columns ({str: (ColumnSchema,)}): Column schema for a given column
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,15 +148,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            preferences (str, none_type): The user's JSON serialized preferences. Schema defined in Dashbird.. [optional]  # noqa: E501
+            metadata (SchemaMetadata): [optional]  # noqa: E501
+            metrics ({str: (MetricSchema,)}, none_type): Schema for user-defined metrics (map of unique custom metric labels to their definitions). [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -167,16 +177,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.user_id = user_id
-        self.email = email
+        self.columns = columns
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -189,20 +198,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, user_id, email, *args, **kwargs):  # noqa: E501
-        """User - a model defined in OpenAPI
+    def __init__(self, columns, *args, **kwargs):  # noqa: E501
+        """EntitySchema - a model defined in OpenAPI
 
         Args:
-            user_id (str): The id of the user.
-            email (str): The user's email address.
+            columns ({str: (ColumnSchema,)}): Column schema for a given column
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -227,15 +235,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            preferences (str, none_type): The user's JSON serialized preferences. Schema defined in Dashbird.. [optional]  # noqa: E501
+            metadata (SchemaMetadata): [optional]  # noqa: E501
+            metrics ({str: (MetricSchema,)}, none_type): Schema for user-defined metrics (map of unique custom metric labels to their definitions). [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -253,16 +262,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.user_id = user_id
-        self.email = email
+        self.columns = columns
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.4.4/whylabs_client/model/user_api_key.py` & `whylabs-client-0.4.5/whylabs_client/model/user_api_key.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/model/user_api_key_response.py` & `whylabs-client-0.4.5/whylabs_client/model/why_logs_metric.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,95 +26,98 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from whylabs_client.model.user_api_key import UserApiKey
-    globals()['UserApiKey'] = UserApiKey
 
-
-class UserApiKeyResponse(ModelNormal):
+class WhyLogsMetric(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
       validations (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('value',): {
+            'TOTALCOUNT': "TotalCount",
+            'MEDIAN': "Median",
+            'MIN': "Min",
+            'MAX': "Max",
+            'STDDEV': "StdDev",
+            'MEAN': "Mean",
+        },
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'key': (UserApiKey,),  # noqa: E501
+            'value': (str,),
         }
 
     @cached_property
     def discriminator():
         return None
 
 
-    attribute_map = {
-        'key': 'key',  # noqa: E501
-    }
+    attribute_map = {}
 
-    read_only_vars = {
-    }
+    read_only_vars = set()
 
-    _composed_schemas = {}
+    _composed_schemas = None
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
 
-    @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UserApiKeyResponse - a model defined in OpenAPI
+    def __init__(self, *args, **kwargs):
+        """WhyLogsMetric - a model defined in OpenAPI
+
+        Note that value can be passed either in args or in kwargs, but not in both.
+
+        Args:
+            args[0] (str):, must be one of ["TotalCount", "Median", "Min", "Max", "StdDev", "Mean", ]  # noqa: E501
 
         Keyword Args:
+            value (str):, must be one of ["TotalCount", "Median", "Min", "Max", "StdDev", "Mean", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -137,25 +140,35 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            key (UserApiKey): [optional]  # noqa: E501
         """
+        # required up here when default value is not given
+        _path_to_item = kwargs.pop('_path_to_item', ())
+
+        if 'value' in kwargs:
+            value = kwargs.pop('value')
+        elif args:
+            args = list(args)
+            value = args.pop(0)
+        else:
+            raise ApiTypeError(
+                "value is required, but not passed in args or kwargs and doesn't have default",
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
-        self = super(OpenApiModel, cls).__new__(cls)
-
         if args:
             raise ApiTypeError(
                 "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
                     args,
                     self.__class__.__name__,
                 ),
                 path_to_item=_path_to_item,
@@ -164,39 +177,37 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+        self.value = value
+        if kwargs:
+            raise ApiTypeError(
+                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
+                    kwargs,
+                    self.__class__.__name__,
+                ),
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
 
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):
+        """WhyLogsMetric - a model defined in OpenAPI
 
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
+        Note that value can be passed either in args or in kwargs, but not in both.
 
-    @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """UserApiKeyResponse - a model defined in OpenAPI
+        Args:
+            args[0] (str):, must be one of ["TotalCount", "Median", "Min", "Max", "StdDev", "Mean", ]  # noqa: E501
 
         Keyword Args:
+            value (str):, must be one of ["TotalCount", "Median", "Min", "Max", "StdDev", "Mean", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -219,20 +230,34 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            key (UserApiKey): [optional]  # noqa: E501
         """
+        # required up here when default value is not given
+        _path_to_item = kwargs.pop('_path_to_item', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if 'value' in kwargs:
+            value = kwargs.pop('value')
+        elif args:
+            args = list(args)
+            value = args.pop(0)
+        else:
+            raise ApiTypeError(
+                "value is required, but not passed in args or kwargs and doesn't have default",
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             raise ApiTypeError(
                 "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
                     args,
@@ -244,19 +269,19 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+        self.value = value
+        if kwargs:
+            raise ApiTypeError(
+                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
+                    kwargs,
+                    self.__class__.__name__,
+                ),
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
 
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+        return self
```

### Comparing `whylabs-client-0.4.4/whylabs_client/model/why_logs_metric.py` & `whylabs-client-0.4.5/whylabs_client/model/metric_schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,97 +27,97 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class WhyLogsMetric(ModelSimple):
+class MetricSchema(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
       validations (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('value',): {
-            'TOTALCOUNT': "TotalCount",
-            'MEDIAN': "Median",
-            'MIN': "Min",
-            'MAX': "Max",
-            'STDDEV': "StdDev",
-            'MEAN': "Mean",
-        },
     }
 
     validations = {
     }
 
-    additional_properties_type = None
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'value': (str,),
+            'label': (str,),  # noqa: E501
+            'column': (str,),  # noqa: E501
+            'default_metric': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
-    attribute_map = {}
-
-    read_only_vars = set()
+    attribute_map = {
+        'label': 'label',  # noqa: E501
+        'column': 'column',  # noqa: E501
+        'default_metric': 'defaultMetric',  # noqa: E501
+    }
 
-    _composed_schemas = None
+    read_only_vars = {
+    }
 
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
+    _composed_schemas = {}
 
+    @classmethod
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):
-        """WhyLogsMetric - a model defined in OpenAPI
-
-        Note that value can be passed either in args or in kwargs, but not in both.
+    def _from_openapi_data(cls, label, column, default_metric, *args, **kwargs):  # noqa: E501
+        """MetricSchema - a model defined in OpenAPI
 
         Args:
-            args[0] (str):, must be one of ["TotalCount", "Median", "Min", "Max", "StdDev", "Mean", ]  # noqa: E501
+            label (str): User-friendly label for the metric. This should be a unique for the entity.
+            column (str): Entity column to extract the metric from
+            default_metric (str): whylogs metric to extract. Note that other metrics may be available for this column as well, this is the one to be used by default. Should match the values of the SimpleColumnMetric enum within the monitor config schema.
 
         Keyword Args:
-            value (str):, must be one of ["TotalCount", "Median", "Min", "Max", "StdDev", "Mean", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -141,34 +141,23 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            raise ApiTypeError(
-                "value is required, but not passed in args or kwargs and doesn't have default",
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
+        self = super(OpenApiModel, cls).__new__(cls)
+
         if args:
             raise ApiTypeError(
                 "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
                     args,
                     self.__class__.__name__,
                 ),
                 path_to_item=_path_to_item,
@@ -177,37 +166,47 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):
-        """WhyLogsMetric - a model defined in OpenAPI
+        self.label = label
+        self.column = column
+        self.default_metric = default_metric
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
 
-        Note that value can be passed either in args or in kwargs, but not in both.
+    @convert_js_args_to_python_args
+    def __init__(self, label, column, default_metric, *args, **kwargs):  # noqa: E501
+        """MetricSchema - a model defined in OpenAPI
 
         Args:
-            args[0] (str):, must be one of ["TotalCount", "Median", "Min", "Max", "StdDev", "Mean", ]  # noqa: E501
+            label (str): User-friendly label for the metric. This should be a unique for the entity.
+            column (str): Entity column to extract the metric from
+            default_metric (str): whylogs metric to extract. Note that other metrics may be available for this column as well, this is the one to be used by default. Should match the values of the SimpleColumnMetric enum within the monitor config schema.
 
         Keyword Args:
-            value (str):, must be one of ["TotalCount", "Median", "Min", "Max", "StdDev", "Mean", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -231,33 +230,18 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            raise ApiTypeError(
-                "value is required, but not passed in args or kwargs and doesn't have default",
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             raise ApiTypeError(
                 "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
                     args,
@@ -269,19 +253,22 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-        return self
+        self.label = label
+        self.column = column
+        self.default_metric = default_metric
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `whylabs-client-0.4.4/whylabs_client/model_utils.py` & `whylabs-client-0.4.5/whylabs_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client/models/__init__.py` & `whylabs-client-0.4.5/whylabs_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 from whylabs_client.model.log_async_request import LogAsyncRequest
 from whylabs_client.model.log_reference_request import LogReferenceRequest
 from whylabs_client.model.log_reference_response import LogReferenceResponse
 from whylabs_client.model.log_response import LogResponse
 from whylabs_client.model.marketplace_dimensions import MarketplaceDimensions
 from whylabs_client.model.membership import Membership
 from whylabs_client.model.membership_metadata import MembershipMetadata
+from whylabs_client.model.metric_schema import MetricSchema
 from whylabs_client.model.missing_recent_data_request_config import MissingRecentDataRequestConfig
 from whylabs_client.model.missing_recent_profiles_request_config import MissingRecentProfilesRequestConfig
 from whylabs_client.model.missing_values_monitor_request_config import MissingValuesMonitorRequestConfig
 from whylabs_client.model.model_metadata_response import ModelMetadataResponse
 from whylabs_client.model.model_type import ModelType
 from whylabs_client.model.monitor_config import MonitorConfig
 from whylabs_client.model.monitor_config_version import MonitorConfigVersion
```

### Comparing `whylabs-client-0.4.4/whylabs_client/rest.py` & `whylabs-client-0.4.5/whylabs_client/rest.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.4/whylabs_client.egg-info/SOURCES.txt` & `whylabs-client-0.4.5/whylabs_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 whylabs_client/model/log_async_request.py
 whylabs_client/model/log_reference_request.py
 whylabs_client/model/log_reference_response.py
 whylabs_client/model/log_response.py
 whylabs_client/model/marketplace_dimensions.py
 whylabs_client/model/membership.py
 whylabs_client/model/membership_metadata.py
+whylabs_client/model/metric_schema.py
 whylabs_client/model/missing_recent_data_request_config.py
 whylabs_client/model/missing_recent_profiles_request_config.py
 whylabs_client/model/missing_values_monitor_request_config.py
 whylabs_client/model/model_metadata_response.py
 whylabs_client/model/model_type.py
 whylabs_client/model/monitor_config.py
 whylabs_client/model/monitor_config_version.py
```


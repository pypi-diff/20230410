# Comparing `tmp/cdktf-cdktf-provider-newrelic-6.0.8.tar.gz` & `tmp/cdktf-cdktf-provider-newrelic-6.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-newrelic-6.0.8.tar", last modified: Thu Mar 23 03:19:24 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-newrelic-6.0.9.tar", last modified: Sat Mar 25 03:22:33 2023, max compression
```

## Comparing `cdktf-cdktf-provider-newrelic-6.0.8.tar` & `cdktf-cdktf-provider-newrelic-6.0.9.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.318463 cdktf-cdktf-provider-newrelic-6.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-03-23 03:19:24.318463 cdktf-cdktf-provider-newrelic-6.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 03:19:24.318463 cdktf-cdktf-provider-newrelic-6.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.282463 cdktf-cdktf-provider-newrelic-6.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.290463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/
--rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.290463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  3439202 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/_jsii/provider-newrelic@6.0.8.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.294463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/account_management/
--rw-r--r--   0 runner    (1001) docker     (123)    27495 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/account_management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.294463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/alert_channel/
--rw-r--r--   0 runner    (1001) docker     (123)    80427 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/alert_channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.298463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/alert_condition/
--rw-r--r--   0 runner    (1001) docker     (123)    68878 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/alert_condition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.298463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/alert_muting_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    74752 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/alert_muting_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.298463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/alert_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    25763 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/alert_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.298463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/alert_policy_channel/
--rw-r--r--   0 runner    (1001) docker     (123)    30810 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/alert_policy_channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.298463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/api_access_key/
--rw-r--r--   0 runner    (1001) docker     (123)    27951 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/api_access_key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.298463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/application_settings/
--rw-r--r--   0 runner    (1001) docker     (123)    25249 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/application_settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.298463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/browser_application/
--rw-r--r--   0 runner    (1001) docker     (123)    29413 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/browser_application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.298463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_integrations/
--rw-r--r--   0 runner    (1001) docker     (123)   386686 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.298463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_link_account/
--rw-r--r--   0 runner    (1001) docker     (123)    30048 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_link_account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.298463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_aws_integrations/
--rw-r--r--   0 runner    (1001) docker     (123)   109383 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_aws_integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.298463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_aws_link_account/
--rw-r--r--   0 runner    (1001) docker     (123)    32930 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_aws_link_account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.298463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_azure_integrations/
--rw-r--r--   0 runner    (1001) docker     (123)   392250 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_azure_integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.298463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_azure_link_account/
--rw-r--r--   0 runner    (1001) docker     (123)    29084 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_azure_link_account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.298463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_gcp_integrations/
--rw-r--r--   0 runner    (1001) docker     (123)   261951 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_gcp_integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.302463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_gcp_link_account/
--rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_gcp_link_account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.302463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_account/
--rw-r--r--   0 runner    (1001) docker     (123)    22272 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.302463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_channel/
--rw-r--r--   0 runner    (1001) docker     (123)    32758 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.302463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    23221 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.302463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_application/
--rw-r--r--   0 runner    (1001) docker     (123)    17737 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.302463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_cloud_account/
--rw-r--r--   0 runner    (1001) docker     (123)    22116 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_cloud_account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.302463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_entity/
--rw-r--r--   0 runner    (1001) docker     (123)    42812 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_entity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.302463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_key_transaction/
--rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_key_transaction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.302463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_notification_destination/
--rw-r--r--   0 runner    (1001) docker     (123)    28604 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_notification_destination/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.302463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_obfuscation_expression/
--rw-r--r--   0 runner    (1001) docker     (123)    20113 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_obfuscation_expression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.302463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_private_location/
--rw-r--r--   0 runner    (1001) docker     (123)    20306 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_private_location/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.302463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_secure_credential/
--rw-r--r--   0 runner    (1001) docker     (123)    21052 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_secure_credential/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.302463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_test_grok_pattern/
--rw-r--r--   0 runner    (1001) docker     (123)    41266 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_test_grok_pattern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.302463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_partition_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    38652 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_partition_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.302463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/entity_tags/
--rw-r--r--   0 runner    (1001) docker     (123)    41289 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/entity_tags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.302463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/events_to_metrics_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    27731 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/events_to_metrics_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.302463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/infra_alert_condition/
--rw-r--r--   0 runner    (1001) docker     (123)    74835 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/infra_alert_condition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.306463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/insights_event/
--rw-r--r--   0 runner    (1001) docker     (123)    50913 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/insights_event/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.306463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/log_parsing_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    34030 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/log_parsing_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.306463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/notification_channel/
--rw-r--r--   0 runner    (1001) docker     (123)    51065 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/notification_channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.306463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/notification_destination/
--rw-r--r--   0 runner    (1001) docker     (123)    67064 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/notification_destination/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.306463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/nrql_alert_condition/
--rw-r--r--   0 runner    (1001) docker     (123)   171356 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/nrql_alert_condition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.306463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/nrql_drop_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    24435 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/nrql_drop_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.306463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/obfuscation_expression/
--rw-r--r--   0 runner    (1001) docker     (123)    24315 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/obfuscation_expression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.306463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/obfuscation_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    45953 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/obfuscation_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.306463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/one_dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)  2234452 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/one_dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.310463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/one_dashboard_json/
--rw-r--r--   0 runner    (1001) docker     (123)    30482 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/one_dashboard_json/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.310463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/one_dashboard_raw/
--rw-r--r--   0 runner    (1001) docker     (123)    70768 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/one_dashboard_raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.310463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    37794 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.310463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/service_level/
--rw-r--r--   0 runner    (1001) docker     (123)   120291 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/service_level/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.310463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_alert_condition/
--rw-r--r--   0 runner    (1001) docker     (123)    27584 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_alert_condition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.310463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_broken_links_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)    50548 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_broken_links_monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.318463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_cert_check_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)    52548 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_cert_check_monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.318463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)    93855 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.318463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_multilocation_alert_condition/
--rw-r--r--   0 runner    (1001) docker     (123)    48868 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_multilocation_alert_condition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.318463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_private_location/
--rw-r--r--   0 runner    (1001) docker     (123)    26608 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_private_location/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.318463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_script_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)    80330 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_script_monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.318463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_secure_credential/
--rw-r--r--   0 runner    (1001) docker     (123)    36008 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_secure_credential/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.318463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_step_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)    86733 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_step_monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.318463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)   115291 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.318463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/workload/
--rw-r--r--   0 runner    (1001) docker     (123)   137480 2023-03-23 03:19:10.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/workload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:19:24.290463 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-03-23 03:19:24.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-03-23 03:19:24.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 03:19:24.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-23 03:19:24.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-23 03:19:24.000000 cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.184705 cdktf-cdktf-provider-newrelic-6.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-03-25 03:22:33.184705 cdktf-cdktf-provider-newrelic-6.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 03:22:33.184705 cdktf-cdktf-provider-newrelic-6.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.160704 cdktf-cdktf-provider-newrelic-6.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.164704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/
+-rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.164704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  3439169 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/_jsii/provider-newrelic@6.0.9.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.168704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/account_management/
+-rw-r--r--   0 runner    (1001) docker     (123)    27495 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/account_management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.168704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/alert_channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    80427 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/alert_channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.168704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/alert_condition/
+-rw-r--r--   0 runner    (1001) docker     (123)    68878 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/alert_condition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.168704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/alert_muting_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    74752 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/alert_muting_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.172704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/alert_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    25763 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/alert_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.172704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/alert_policy_channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    30810 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/alert_policy_channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.172704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/api_access_key/
+-rw-r--r--   0 runner    (1001) docker     (123)    27951 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/api_access_key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.172704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/application_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)    25249 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/application_settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.172704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/browser_application/
+-rw-r--r--   0 runner    (1001) docker     (123)    29413 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/browser_application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.172704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)   386686 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.172704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_link_account/
+-rw-r--r--   0 runner    (1001) docker     (123)    30048 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_link_account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.172704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_aws_integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)   109383 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_aws_integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.172704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_aws_link_account/
+-rw-r--r--   0 runner    (1001) docker     (123)    32930 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_aws_link_account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.172704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_azure_integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)   392250 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_azure_integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.172704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_azure_link_account/
+-rw-r--r--   0 runner    (1001) docker     (123)    29084 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_azure_link_account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.172704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_gcp_integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)   261951 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_gcp_integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.172704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_gcp_link_account/
+-rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_gcp_link_account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.172704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_account/
+-rw-r--r--   0 runner    (1001) docker     (123)    22272 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.172704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    32758 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.172704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    23221 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.172704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_application/
+-rw-r--r--   0 runner    (1001) docker     (123)    17737 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_cloud_account/
+-rw-r--r--   0 runner    (1001) docker     (123)    22116 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_cloud_account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_entity/
+-rw-r--r--   0 runner    (1001) docker     (123)    42812 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_entity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_key_transaction/
+-rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_key_transaction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_notification_destination/
+-rw-r--r--   0 runner    (1001) docker     (123)    28604 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_notification_destination/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_obfuscation_expression/
+-rw-r--r--   0 runner    (1001) docker     (123)    20113 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_obfuscation_expression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_private_location/
+-rw-r--r--   0 runner    (1001) docker     (123)    20306 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_private_location/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_secure_credential/
+-rw-r--r--   0 runner    (1001) docker     (123)    21052 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_secure_credential/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_test_grok_pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)    41266 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_test_grok_pattern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_partition_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    38652 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_partition_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/entity_tags/
+-rw-r--r--   0 runner    (1001) docker     (123)    41289 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/entity_tags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/events_to_metrics_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    27731 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/events_to_metrics_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/infra_alert_condition/
+-rw-r--r--   0 runner    (1001) docker     (123)    74835 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/infra_alert_condition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/insights_event/
+-rw-r--r--   0 runner    (1001) docker     (123)    50913 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/insights_event/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/log_parsing_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    34030 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/log_parsing_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/notification_channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    51065 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/notification_channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/notification_destination/
+-rw-r--r--   0 runner    (1001) docker     (123)    67064 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/notification_destination/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/nrql_alert_condition/
+-rw-r--r--   0 runner    (1001) docker     (123)   171356 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/nrql_alert_condition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/nrql_drop_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    24435 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/nrql_drop_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/obfuscation_expression/
+-rw-r--r--   0 runner    (1001) docker     (123)    24315 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/obfuscation_expression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/obfuscation_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    45953 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/obfuscation_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.176704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/one_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)  2234452 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/one_dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.180704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/one_dashboard_json/
+-rw-r--r--   0 runner    (1001) docker     (123)    30482 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/one_dashboard_json/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.180704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/one_dashboard_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)    70768 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/one_dashboard_raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.180704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    37794 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.180704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/service_level/
+-rw-r--r--   0 runner    (1001) docker     (123)   120291 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/service_level/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.180704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_alert_condition/
+-rw-r--r--   0 runner    (1001) docker     (123)    27584 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_alert_condition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.180704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_broken_links_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)    50548 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_broken_links_monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.180704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_cert_check_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)    52548 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_cert_check_monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.180704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)    93855 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.180704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_multilocation_alert_condition/
+-rw-r--r--   0 runner    (1001) docker     (123)    48868 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_multilocation_alert_condition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.184705 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_private_location/
+-rw-r--r--   0 runner    (1001) docker     (123)    26608 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_private_location/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.184705 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_script_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)    80330 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_script_monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.184705 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_secure_credential/
+-rw-r--r--   0 runner    (1001) docker     (123)    36008 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_secure_credential/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.184705 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_step_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)    86733 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_step_monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.184705 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)   115291 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.184705 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/workload/
+-rw-r--r--   0 runner    (1001) docker     (123)   137480 2023-03-25 03:22:20.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/workload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 03:22:33.164704 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-03-25 03:22:33.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-03-25 03:22:33.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 03:22:33.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-25 03:22:33.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-25 03:22:33.000000 cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/LICENSE` & `cdktf-cdktf-provider-newrelic-6.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/PKG-INFO` & `cdktf-cdktf-provider-newrelic-6.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-newrelic
-Version: 6.0.8
+Version: 6.0.9
 Summary: Prebuilt newrelic Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-newrelic.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-newrelic.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/README.md` & `cdktf-cdktf-provider-newrelic-6.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/setup.py` & `cdktf-cdktf-provider-newrelic-6.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-newrelic",
-    "version": "6.0.8",
+    "version": "6.0.9",
     "description": "Prebuilt newrelic Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-newrelic.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -79,15 +79,15 @@
         "cdktf_cdktf_provider_newrelic.synthetics_secure_credential",
         "cdktf_cdktf_provider_newrelic.synthetics_step_monitor",
         "cdktf_cdktf_provider_newrelic.workflow",
         "cdktf_cdktf_provider_newrelic.workload"
     ],
     "package_data": {
         "cdktf_cdktf_provider_newrelic._jsii": [
-            "provider-newrelic@6.0.8.jsii.tgz"
+            "provider-newrelic@6.0.9.jsii.tgz"
         ],
         "cdktf_cdktf_provider_newrelic": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/account_management/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/account_management/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/alert_channel/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/alert_channel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
         '''Create a new {@link https://www.terraform.io/docs/providers/newrelic/r/alert_channel newrelic_alert_channel} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
         :param name: (Required) The name of the channel. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_channel#name AlertChannel#name}
-        :param type: (Required) The type of channel. One of: (opsgenie, pagerduty, slack, user, victorops, webhook, email). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_channel#type AlertChannel#type}
+        :param type: (Required) The type of channel. One of: (webhook, email, opsgenie, pagerduty, slack, user, victorops). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_channel#type AlertChannel#type}
         :param account_id: The New Relic account ID where you want to create alert channels. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_channel#account_id AlertChannel#account_id}
         :param config: config block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_channel#config AlertChannel#config}
         :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_channel#id AlertChannel#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
@@ -299,15 +299,15 @@
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         :param name: (Required) The name of the channel. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_channel#name AlertChannel#name}
-        :param type: (Required) The type of channel. One of: (opsgenie, pagerduty, slack, user, victorops, webhook, email). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_channel#type AlertChannel#type}
+        :param type: (Required) The type of channel. One of: (webhook, email, opsgenie, pagerduty, slack, user, victorops). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_channel#type AlertChannel#type}
         :param account_id: The New Relic account ID where you want to create alert channels. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_channel#account_id AlertChannel#account_id}
         :param config: config block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_channel#config AlertChannel#config}
         :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_channel#id AlertChannel#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(config, dict):
@@ -421,15 +421,15 @@
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
-        '''(Required) The type of channel. One of: (opsgenie, pagerduty, slack, user, victorops, webhook, email).
+        '''(Required) The type of channel. One of: (webhook, email, opsgenie, pagerduty, slack, user, victorops).
 
         Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_channel#type AlertChannel#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
```

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/alert_condition/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/alert_condition/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
         :param entities: The instance IDs associated with this condition. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#entities AlertCondition#entities}
         :param metric: The metric field accepts parameters based on the type set. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#metric AlertCondition#metric}
         :param name: The title of the condition. Must be between 1 and 128 characters, inclusive. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#name AlertCondition#name}
         :param policy_id: The ID of the policy where this condition should be used. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#policy_id AlertCondition#policy_id}
         :param term: term block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#term AlertCondition#term}
-        :param type: The type of condition. One of: (mobile_metric, servers_metric, apm_app_metric, apm_jvm_metric, apm_kt_metric, browser_metric). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#type AlertCondition#type}
+        :param type: The type of condition. One of: (apm_app_metric, apm_jvm_metric, apm_kt_metric, browser_metric, mobile_metric, servers_metric). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#type AlertCondition#type}
         :param condition_scope: One of (application, instance). Choose application for most scenarios. If you are using the JVM plugin in New Relic, the instance setting allows your condition to trigger for specific app instances. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#condition_scope AlertCondition#condition_scope}
         :param enabled: Whether the condition is enabled. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#enabled AlertCondition#enabled}
         :param gc_metric: A valid Garbage Collection metric e.g. GC/G1 Young Generation. This is required if you are using apm_jvm_metric with gc_cpu_time condition type. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#gc_metric AlertCondition#gc_metric}
         :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#id AlertCondition#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param runbook_url: Runbook URL to display in notifications. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#runbook_url AlertCondition#runbook_url}
         :param user_defined_metric: A custom metric to be evaluated. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#user_defined_metric AlertCondition#user_defined_metric}
         :param user_defined_value_function: One of: (average, min, max, total, sample_size, percent, rate). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#user_defined_value_function AlertCondition#user_defined_value_function}
@@ -466,15 +466,15 @@
         :param provider: 
         :param provisioners: 
         :param entities: The instance IDs associated with this condition. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#entities AlertCondition#entities}
         :param metric: The metric field accepts parameters based on the type set. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#metric AlertCondition#metric}
         :param name: The title of the condition. Must be between 1 and 128 characters, inclusive. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#name AlertCondition#name}
         :param policy_id: The ID of the policy where this condition should be used. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#policy_id AlertCondition#policy_id}
         :param term: term block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#term AlertCondition#term}
-        :param type: The type of condition. One of: (mobile_metric, servers_metric, apm_app_metric, apm_jvm_metric, apm_kt_metric, browser_metric). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#type AlertCondition#type}
+        :param type: The type of condition. One of: (apm_app_metric, apm_jvm_metric, apm_kt_metric, browser_metric, mobile_metric, servers_metric). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#type AlertCondition#type}
         :param condition_scope: One of (application, instance). Choose application for most scenarios. If you are using the JVM plugin in New Relic, the instance setting allows your condition to trigger for specific app instances. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#condition_scope AlertCondition#condition_scope}
         :param enabled: Whether the condition is enabled. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#enabled AlertCondition#enabled}
         :param gc_metric: A valid Garbage Collection metric e.g. GC/G1 Young Generation. This is required if you are using apm_jvm_metric with gc_cpu_time condition type. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#gc_metric AlertCondition#gc_metric}
         :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#id AlertCondition#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param runbook_url: Runbook URL to display in notifications. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#runbook_url AlertCondition#runbook_url}
         :param user_defined_metric: A custom metric to be evaluated. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#user_defined_metric AlertCondition#user_defined_metric}
         :param user_defined_value_function: One of: (average, min, max, total, sample_size, percent, rate). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#user_defined_value_function AlertCondition#user_defined_value_function}
@@ -656,15 +656,15 @@
         '''
         result = self._values.get("term")
         assert result is not None, "Required property 'term' is missing"
         return typing.cast(typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["AlertConditionTerm"]], result)
 
     @builtins.property
     def type(self) -> builtins.str:
-        '''The type of condition. One of: (mobile_metric, servers_metric, apm_app_metric, apm_jvm_metric, apm_kt_metric, browser_metric).
+        '''The type of condition. One of: (apm_app_metric, apm_jvm_metric, apm_kt_metric, browser_metric, mobile_metric, servers_metric).
 
         Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/newrelic/r/alert_condition#type AlertCondition#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
```

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/alert_muting_rule/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/alert_muting_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/alert_policy/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/alert_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/alert_policy_channel/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/alert_policy_channel/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/api_access_key/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/api_access_key/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/application_settings/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/application_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/browser_application/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/browser_application/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_integrations/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_link_account/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_link_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_aws_integrations/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_aws_integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_aws_link_account/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_aws_link_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_azure_integrations/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_azure_integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_azure_link_account/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_azure_link_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_gcp_integrations/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_gcp_integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/cloud_gcp_link_account/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/cloud_gcp_link_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_account/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_channel/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_channel/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_policy/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_application/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_application/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_cloud_account/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_cloud_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_entity/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_entity/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_key_transaction/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_key_transaction/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_notification_destination/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_notification_destination/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_obfuscation_expression/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_obfuscation_expression/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_private_location/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_private_location/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_secure_credential/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_secure_credential/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_newrelic_test_grok_pattern/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_newrelic_test_grok_pattern/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/data_partition_rule/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/data_partition_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/entity_tags/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/entity_tags/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/events_to_metrics_rule/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/events_to_metrics_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/infra_alert_condition/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/infra_alert_condition/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/insights_event/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/insights_event/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/log_parsing_rule/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/log_parsing_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/notification_channel/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/notification_channel/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/notification_destination/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/notification_destination/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/nrql_alert_condition/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/nrql_alert_condition/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/nrql_drop_rule/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/nrql_drop_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/obfuscation_expression/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/obfuscation_expression/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/obfuscation_rule/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/obfuscation_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/one_dashboard/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/one_dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/one_dashboard_json/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/one_dashboard_json/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/one_dashboard_raw/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/one_dashboard_raw/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/provider/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/service_level/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/service_level/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_alert_condition/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_alert_condition/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_broken_links_monitor/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_broken_links_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_cert_check_monitor/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_cert_check_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_monitor/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_multilocation_alert_condition/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_multilocation_alert_condition/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_private_location/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_private_location/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_script_monitor/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_script_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_secure_credential/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_secure_credential/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/synthetics_step_monitor/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/synthetics_step_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/workflow/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic/workload/__init__.py` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic/workload/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic.egg-info/PKG-INFO` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-newrelic
-Version: 6.0.8
+Version: 6.0.9
 Summary: Prebuilt newrelic Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-newrelic.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-newrelic.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-newrelic-6.0.8/src/cdktf_cdktf_provider_newrelic.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-newrelic-6.0.9/src/cdktf_cdktf_provider_newrelic.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_newrelic/py.typed
 src/cdktf_cdktf_provider_newrelic.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_newrelic.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_newrelic.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_newrelic.egg-info/requires.txt
 src/cdktf_cdktf_provider_newrelic.egg-info/top_level.txt
 src/cdktf_cdktf_provider_newrelic/_jsii/__init__.py
-src/cdktf_cdktf_provider_newrelic/_jsii/provider-newrelic@6.0.8.jsii.tgz
+src/cdktf_cdktf_provider_newrelic/_jsii/provider-newrelic@6.0.9.jsii.tgz
 src/cdktf_cdktf_provider_newrelic/account_management/__init__.py
 src/cdktf_cdktf_provider_newrelic/alert_channel/__init__.py
 src/cdktf_cdktf_provider_newrelic/alert_condition/__init__.py
 src/cdktf_cdktf_provider_newrelic/alert_muting_rule/__init__.py
 src/cdktf_cdktf_provider_newrelic/alert_policy/__init__.py
 src/cdktf_cdktf_provider_newrelic/alert_policy_channel/__init__.py
 src/cdktf_cdktf_provider_newrelic/api_access_key/__init__.py
```


# Comparing `tmp/tcex-3.0.7.tar.gz` & `tmp/tcex-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcex-3.0.7.tar", last modified: Tue Feb  7 21:10:47 2023, max compression
+gzip compressed data, was "tcex-3.0.8.tar", last modified: Mon Apr 10 17:48:24 2023, max compression
```

## Comparing `tcex-3.0.7.tar` & `tcex-3.0.8.tar`

### file list

```diff
@@ -1,426 +1,426 @@
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.578763 tcex-3.0.7/
--rw-rw-r--   0 bsummers   (503) staff       (20)    11357 2019-02-12 17:08:25.000000 tcex-3.0.7/LICENSE
--rw-rw-r--   0 bsummers   (503) staff       (20)     3508 2023-02-07 21:10:47.578879 tcex-3.0.7/PKG-INFO
--rw-rw-r--   0 bsummers   (503) staff       (20)     2211 2022-11-14 21:07:06.000000 tcex-3.0.7/README.md
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.412173 tcex-3.0.7/bin/
--rw-rw-r--   0 bsummers   (503) staff       (20)    14118 2022-06-29 14:32:21.000000 tcex-3.0.7/bin/tcex
--rw-rw-r--   0 bsummers   (503) staff       (20)      984 2022-08-26 17:57:26.000000 tcex-3.0.7/pyproject.toml
--rw-rw-r--   0 bsummers   (503) staff       (20)      772 2023-02-07 21:10:47.579599 tcex-3.0.7/setup.cfg
--rw-rw-r--   0 bsummers   (503) staff       (20)     3028 2023-02-02 18:36:54.000000 tcex-3.0.7/setup.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.413900 tcex-3.0.7/tcex/
--rw-rw-r--   0 bsummers   (503) staff       (20)     1139 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      432 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/__metadata__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.417891 tcex-3.0.7/tcex/api/
--rw-rw-r--   0 bsummers   (503) staff       (20)       76 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      765 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/api.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.419025 tcex-3.0.7/tcex/api/tc/
--rw-rw-r--   0 bsummers   (503) staff       (20)       91 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/tc/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2052 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/tc/tc.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.420877 tcex-3.0.7/tcex/api/tc/ti_transform/
--rw-rw-r--   0 bsummers   (503) staff       (20)      141 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/tc/ti_transform/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      196 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/tc/ti_transform/formatters.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.422413 tcex-3.0.7/tcex/api/tc/ti_transform/model/
--rw-rw-r--   0 bsummers   (503) staff       (20)      353 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/tc/ti_transform/model/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7466 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/ti_transform/model/transform_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6377 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/tc/ti_transform/ti_transform.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    25560 2023-02-02 18:36:54.000000 tcex-3.0.7/tcex/api/tc/ti_transform/transform_abc.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.423337 tcex-3.0.7/tcex/api/tc/utils/
--rw-rw-r--   0 bsummers   (503) staff       (20)       39 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/utils/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    14736 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/utils/threat_intel_utils.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.424201 tcex-3.0.7/tcex/api/tc/v2/
--rw-rw-r--   0 bsummers   (503) staff       (20)      100 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.429602 tcex-3.0.7/tcex/api/tc/v2/batch/
--rw-rw-r--   0 bsummers   (503) staff       (20)      228 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/batch/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2671 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v2/batch/attribute.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    44500 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v2/batch/batch.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    18746 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/tc/v2/batch/batch_submit.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    51366 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/tc/v2/batch/batch_writer.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    23538 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v2/batch/group.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    29032 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/tc/v2/batch/indicator.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1768 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v2/batch/security_label.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1161 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v2/batch/tag.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.431022 tcex-3.0.7/tcex/api/tc/v2/datastore/
--rw-rw-r--   0 bsummers   (503) staff       (20)      114 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/datastore/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7077 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/datastore/cache.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    11000 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v2/datastore/datastore.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.431958 tcex-3.0.7/tcex/api/tc/v2/metrics/
--rw-rw-r--   0 bsummers   (503) staff       (20)       84 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/metrics/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6543 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/metrics/metrics.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.432737 tcex-3.0.7/tcex/api/tc/v2/notifications/
--rw-rw-r--   0 bsummers   (503) staff       (20)      102 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/notifications/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3187 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/notifications/notifications.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.434487 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/
--rw-rw-r--   0 bsummers   (503) staff       (20)      118 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.438009 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/
--rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2386 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/filters.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.438631 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/
--rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3731 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.444507 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/
--rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8796 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/adversary.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      947 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/attack_pattern.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1625 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/campaign.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      953 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/course_of_action.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4495 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/document.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1112 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/email.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2339 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/event.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2340 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/incident.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      951 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/intrusion_set.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      867 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/malware.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3710 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/report.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1564 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/signature.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      841 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/tactic.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      843 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/threat.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      831 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/tool.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      947 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/vulnerability.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.445043 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/indicator/
--rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/indicator/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    10357 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.447026 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/
--rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2166 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/address.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2041 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/email_address.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7612 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/file.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3127 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/host.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2103 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/url.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    22774 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/mappings.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2241 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/owner.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2945 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/security_label.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2545 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/tag.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1249 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/tags.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8676 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/task.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    15032 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/victim.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    57009 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/tcex_ti_tc_request.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    35065 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/threat_intelligence.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7064 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/tc/v2/v2.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.451227 tcex-3.0.7/tcex/api/tc/v3/
--rw-rw-r--   0 bsummers   (503) staff       (20)       53 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.454481 tcex-3.0.7/tcex/api/tc/v3/_gen/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/_gen/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     9764 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/_gen/_gen.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    18831 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/_gen/_gen_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3450 2023-02-02 18:36:54.000000 tcex-3.0.7/tcex/api/tc/v3/_gen/_gen_args_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    18924 2023-02-02 18:36:54.000000 tcex-3.0.7/tcex/api/tc/v3/_gen/_gen_filter_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    16667 2023-02-02 18:36:54.000000 tcex-3.0.7/tcex/api/tc/v3/_gen/_gen_model_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    38886 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/_gen/_gen_object_abc.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.456085 tcex-3.0.7/tcex/api/tc/v3/_gen/models/
--rw-rw-r--   0 bsummers   (503) staff       (20)      176 2023-02-02 18:36:54.000000 tcex-3.0.7/tcex/api/tc/v3/_gen/models/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4059 2023-02-02 18:36:54.000000 tcex-3.0.7/tcex/api/tc/v3/_gen/models/_filter_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    13541 2023-02-02 18:36:54.000000 tcex-3.0.7/tcex/api/tc/v3/_gen/models/_property_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.456641 tcex-3.0.7/tcex/api/tc/v3/adversary_assets/
--rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/adversary_assets/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1003 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/api_endpoints.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.459031 tcex-3.0.7/tcex/api/tc/v3/artifact_types/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/artifact_types/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3157 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/artifact_types/artifact_type.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2770 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/artifact_types/artifact_type_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2982 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/artifact_types/artifact_type_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.462062 tcex-3.0.7/tcex/api/tc/v3/artifacts/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/artifacts/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6810 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/artifacts/artifact.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6061 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/tc/v3/artifacts/artifact_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8747 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/artifacts/artifact_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.464154 tcex-3.0.7/tcex/api/tc/v3/attribute_types/
--rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/attribute_types/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3482 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/attribute_types/attribute_type.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3206 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/attribute_types/attribute_type_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3261 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/attribute_types/attribute_type_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.465169 tcex-3.0.7/tcex/api/tc/v3/attributes/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/attributes/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2234 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/attributes/attribute_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.467256 tcex-3.0.7/tcex/api/tc/v3/case_attributes/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/case_attributes/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4753 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/case_attributes/case_attribute.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6577 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/case_attributes/case_attribute_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4834 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/case_attributes/case_attribute_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.468321 tcex-3.0.7/tcex/api/tc/v3/case_management/
--rw-rw-r--   0 bsummers   (503) staff       (20)       63 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/case_management/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    22368 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/case_management/case_management.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.471338 tcex-3.0.7/tcex/api/tc/v3/cases/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/cases/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    12920 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/cases/case.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    15834 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/cases/case_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    11811 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/cases/case_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.472788 tcex-3.0.7/tcex/api/tc/v3/file_actions/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-08-26 17:57:26.000000 tcex-3.0.7/tcex/api/tc/v3/file_actions/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1797 2022-08-26 17:57:26.000000 tcex-3.0.7/tcex/api/tc/v3/file_actions/file_action_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.473870 tcex-3.0.7/tcex/api/tc/v3/file_occurrences/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-08-26 17:57:26.000000 tcex-3.0.7/tcex/api/tc/v3/file_occurrences/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1641 2022-08-26 17:57:26.000000 tcex-3.0.7/tcex/api/tc/v3/file_occurrences/file_occurrence_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1371 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/filter_abc.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.475690 tcex-3.0.7/tcex/api/tc/v3/group_attributes/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/group_attributes/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4781 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/group_attributes/group_attribute.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7370 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/group_attributes/group_attribute_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4856 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/group_attributes/group_attribute_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.477366 tcex-3.0.7/tcex/api/tc/v3/groups/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/groups/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    15307 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/groups/group.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    22344 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/groups/group_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    16801 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/groups/group_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.478828 tcex-3.0.7/tcex/api/tc/v3/indicator_attributes/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/indicator_attributes/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4893 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/indicator_attributes/indicator_attribute.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7466 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/indicator_attributes/indicator_attribute_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4944 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/indicator_attributes/indicator_attribute_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.480433 tcex-3.0.7/tcex/api/tc/v3/indicators/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/indicators/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    14868 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/indicators/indicator.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    20183 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/indicators/indicator_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    16897 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/indicators/indicator_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.482418 tcex-3.0.7/tcex/api/tc/v3/notes/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/notes/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3463 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/notes/note.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4852 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/tc/v3/notes/note_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6026 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/notes/note_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    12537 2023-02-02 18:36:54.000000 tcex-3.0.7/tcex/api/tc/v3/object_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8527 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/object_collection_abc.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.485449 tcex-3.0.7/tcex/api/tc/v3/security/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/security/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1393 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/security/assignee_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      741 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/security/assignee_user_group_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      716 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/security/assignee_user_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.487582 tcex-3.0.7/tcex/api/tc/v3/security/owner_roles/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/security/owner_roles/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2878 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/security/owner_roles/owner_role.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3600 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/security/owner_roles/owner_role_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3530 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/security/owner_roles/owner_role_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.489566 tcex-3.0.7/tcex/api/tc/v3/security/owners/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/security/owners/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2761 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/security/owners/owner.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    10858 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/security/owners/owner_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7508 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/security/owners/owner_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2266 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/security/security.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.491455 tcex-3.0.7/tcex/api/tc/v3/security/system_roles/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/security/system_roles/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2905 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/security/system_roles/system_role.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2052 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/security/system_roles/system_role_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2697 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/security/system_roles/system_role_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2650 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/security/task_assignee_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.493222 tcex-3.0.7/tcex/api/tc/v3/security/user_groups/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/security/user_groups/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2878 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/security/user_groups/user_group.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1411 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/security/user_groups/user_group_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2739 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/security/user_groups/user_group_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.495013 tcex-3.0.7/tcex/api/tc/v3/security/users/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/security/users/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2734 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/security/users/user.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7820 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/security/users/user_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2021 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/security/users/user_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.496565 tcex-3.0.7/tcex/api/tc/v3/security_labels/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/security_labels/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4337 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/security_labels/security_label.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6009 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/tc/v3/security_labels/security_label_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3134 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/tc/v3/security_labels/security_label_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.498123 tcex-3.0.7/tcex/api/tc/v3/tags/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/tags/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3980 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/tags/tag.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6091 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/tc/v3/tags/tag_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4349 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/tags/tag_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.499508 tcex-3.0.7/tcex/api/tc/v3/tasks/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/tasks/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6646 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/tasks/task.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     9537 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/tc/v3/tasks/task_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7442 2022-03-23 20:18:24.000000 tcex-3.0.7/tcex/api/tc/v3/tasks/task_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.500352 tcex-3.0.7/tcex/api/tc/v3/threat_intelligence/
--rw-rw-r--   0 bsummers   (503) staff       (20)       67 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/threat_intelligence/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    17553 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/threat_intelligence/threat_intelligence.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.502161 tcex-3.0.7/tcex/api/tc/v3/tql/
--rw-rw-r--   0 bsummers   (503) staff       (20)       51 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/tql/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2222 2023-02-02 18:36:54.000000 tcex-3.0.7/tcex/api/tc/v3/tql/tql.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      520 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/tql/tql_operator.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      251 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/tql/tql_type.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1321 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/tc/v3/v3.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    18104 2022-08-26 17:57:26.000000 tcex-3.0.7/tcex/api/tc/v3/v3_model_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1647 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/v3_types.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.503648 tcex-3.0.7/tcex/api/tc/v3/victim_assets/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/victim_assets/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5821 2022-08-26 17:57:26.000000 tcex-3.0.7/tcex/api/tc/v3/victim_assets/victim_asset.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5222 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/victim_assets/victim_asset_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5177 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/victim_assets/victim_asset_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.504884 tcex-3.0.7/tcex/api/tc/v3/victim_attributes/
--rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/victim_attributes/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4815 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/victim_attributes/victim_attribute.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7027 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/victim_attributes/victim_attribute_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4879 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/api/tc/v3/victim_attributes/victim_attribute_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.507182 tcex-3.0.7/tcex/api/tc/v3/victims/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/victims/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7916 2023-02-02 18:36:54.000000 tcex-3.0.7/tcex/api/tc/v3/victims/victim.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     9140 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/victims/victim_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6561 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/victims/victim_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.509626 tcex-3.0.7/tcex/api/tc/v3/workflow_events/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/workflow_events/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4550 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/workflow_events/workflow_event.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4075 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/api/tc/v3/workflow_events/workflow_event_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5484 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/workflow_events/workflow_event_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.512291 tcex-3.0.7/tcex/api/tc/v3/workflow_templates/
--rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/api/tc/v3/workflow_templates/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3611 2023-02-02 18:36:54.000000 tcex-3.0.7/tcex/api/tc/v3/workflow_templates/workflow_template.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3449 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/api/tc/v3/workflow_templates/workflow_template_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5159 2022-03-23 20:18:24.000000 tcex-3.0.7/tcex/api/tc/v3/workflow_templates/workflow_template_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.519188 tcex-3.0.7/tcex/app_config/
--rw-rw-r--   0 bsummers   (503) staff       (20)      327 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/app_config/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    21393 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/app_config/app_spec_yml.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     9324 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/app_config/install_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6004 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/app_config/install_json_update.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1485 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/app_config/install_json_validate.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2061 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/app_config/job_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4484 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/app_config/layout_json.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.523130 tcex-3.0.7/tcex/app_config/models/
--rw-rw-r--   0 bsummers   (503) staff       (20)      464 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/app_config/models/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    13834 2023-02-02 18:36:54.000000 tcex-3.0.7/tcex/app_config/models/app_spec_yml_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    29279 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/app_config/models/install_json_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2993 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/app_config/models/job_json_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2853 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/app_config/models/layout_json_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1833 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/app_config/models/tcex_json_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      914 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/app_config/models/template_config_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    20625 2022-08-26 17:57:26.000000 tcex-3.0.7/tcex/app_config/permutation.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2973 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/app_config/tcex_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3222 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/app_config/tcex_json_update.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.523988 tcex-3.0.7/tcex/app_feature/
--rw-rw-r--   0 bsummers   (503) staff       (20)      135 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/app_feature/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5615 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/app_feature/advanced_request.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.524464 tcex-3.0.7/tcex/backports/
--rw-rw-r--   0 bsummers   (503) staff       (20)     1066 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/backports/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.532036 tcex-3.0.7/tcex/bin/
--rw-rw-r--   0 bsummers   (503) staff       (20)      284 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/bin/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6525 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/bin/bin_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    16717 2022-08-26 17:57:26.000000 tcex-3.0.7/tcex/bin/dep.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5079 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/bin/deploy.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     9593 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/bin/package.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    11318 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/bin/spec_tool.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    22766 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/bin/spec_tool_app_input.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8530 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/bin/spec_tool_app_input_static.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    11155 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/bin/spec_tool_app_spec_yml.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5739 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/bin/spec_tool_install_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1587 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/bin/spec_tool_job_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      981 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/bin/spec_tool_layout_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    14062 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/bin/spec_tool_readme_md.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1057 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/bin/spec_tool_tcex_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    20422 2023-02-02 18:36:54.000000 tcex-3.0.7/tcex/bin/template.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    21765 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/bin/validate.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.535201 tcex-3.0.7/tcex/decorators/
--rw-rw-r--   0 bsummers   (503) staff       (20)      360 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/decorators/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2335 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/decorators/benchmark.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1558 2020-09-04 22:24:44.000000 tcex-3.0.7/tcex/decorators/debug.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4525 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/decorators/fail_on_output.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3681 2022-03-23 20:18:24.000000 tcex-3.0.7/tcex/decorators/on_exception.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1828 2020-09-04 22:24:44.000000 tcex-3.0.7/tcex/decorators/on_success.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3482 2020-09-04 22:24:44.000000 tcex-3.0.7/tcex/decorators/output.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.536555 tcex-3.0.7/tcex/exit/
--rw-rw-r--   0 bsummers   (503) staff       (20)      192 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/exit/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5374 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/exit/error_codes.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6516 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/exit/exit.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.537384 tcex-3.0.7/tcex/input/
--rw-rw-r--   0 bsummers   (503) staff       (20)       92 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.544199 tcex-3.0.7/tcex/input/field_types/
--rw-rw-r--   0 bsummers   (503) staff       (20)     1242 2022-03-23 20:18:24.000000 tcex-3.0.7/tcex/input/field_types/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3532 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/field_types/binary.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3129 2022-03-23 20:18:24.000000 tcex-3.0.7/tcex/input/field_types/case_management_entity.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1581 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/field_types/choice.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      866 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/field_types/datetime.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3764 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/field_types/edit_choice.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3073 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/field_types/exception.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2995 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/field_types/group_entity.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2725 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/field_types/indicator_entity.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3505 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/input/field_types/integer.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2336 2022-03-23 20:18:24.000000 tcex-3.0.7/tcex/input/field_types/ip_address.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1270 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/field_types/key_value.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5151 2023-02-02 18:36:54.000000 tcex-3.0.7/tcex/input/field_types/sensitive.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4111 2022-03-23 20:18:24.000000 tcex-3.0.7/tcex/input/field_types/string.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1251 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/field_types/tc_entity.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8590 2022-03-23 20:18:24.000000 tcex-3.0.7/tcex/input/field_types/validators.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    15693 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/input/input.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.550145 tcex-3.0.7/tcex/input/models/
--rw-rw-r--   0 bsummers   (503) staff       (20)     1012 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/models/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2575 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/input/models/advanced_request_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      999 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/models/aot_execution_enabled_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2935 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/input/models/api_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1525 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/models/batch_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      893 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/models/cal_settings_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1567 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/input/models/create_config_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1595 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/models/logging_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2736 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/input/models/model_map.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      428 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/models/organization_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1162 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/models/path_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1151 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/models/playbook_common_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      929 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/models/playbook_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1350 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/models/proxy_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2716 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/models/service_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1174 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/input/models/smtp_settings_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.552355 tcex-3.0.7/tcex/key_value_store/
--rw-rw-r--   0 bsummers   (503) staff       (20)      224 2022-08-26 17:57:26.000000 tcex-3.0.7/tcex/key_value_store/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      873 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/key_value_store/key_value_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2499 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/key_value_store/key_value_api.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1801 2022-08-26 17:57:26.000000 tcex-3.0.7/tcex/key_value_store/key_value_mock.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2777 2022-08-26 17:57:26.000000 tcex-3.0.7/tcex/key_value_store/key_value_redis.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1669 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/key_value_store/redis_client.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.556331 tcex-3.0.7/tcex/logger/
--rw-rw-r--   0 bsummers   (503) staff       (20)      293 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/logger/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3780 2022-08-26 17:57:26.000000 tcex-3.0.7/tcex/logger/api_handler.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      862 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/logger/cache_handler.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    13964 2023-02-02 18:36:54.000000 tcex-3.0.7/tcex/logger/logger.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3112 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/logger/pattern_file_handler.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2001 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/logger/rotating_file_handler_custom.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      974 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/logger/sensitive_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1822 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/logger/thread_file_handler.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1206 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/logger/trace_logger.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.560101 tcex-3.0.7/tcex/playbook/
--rw-rw-r--   0 bsummers   (503) staff       (20)       88 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/playbook/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3467 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/playbook/playbook.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    20899 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/playbook/playbook_create.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1027 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/playbook/playbook_delete.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      668 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/playbook/playbook_output.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    22857 2022-08-26 17:57:26.000000 tcex-3.0.7/tcex/playbook/playbook_read.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.565387 tcex-3.0.7/tcex/pleb/
--rw-rw-r--   0 bsummers   (503) staff       (20)       26 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/pleb/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1599 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/pleb/env_path.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      737 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/pleb/event.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      536 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/pleb/none_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1178 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/pleb/proxies.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7213 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/pleb/registry.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2311 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/pleb/scoped_property.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      412 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/pleb/singleton.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      731 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/pleb/threading.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.568643 tcex-3.0.7/tcex/services/
--rw-rw-r--   0 bsummers   (503) staff       (20)      324 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/services/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    11874 2023-02-02 18:36:54.000000 tcex-3.0.7/tcex/services/api_service.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    16230 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/services/common_service.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    17548 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/services/common_service_trigger.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    10563 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/services/mqtt_message_broker.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    15948 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/services/webhook_trigger_service.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.570925 tcex-3.0.7/tcex/sessions/
--rw-rw-r--   0 bsummers   (503) staff       (20)       40 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/sessions/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.572802 tcex-3.0.7/tcex/sessions/auth/
--rw-rw-r--   0 bsummers   (503) staff       (20)       31 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/sessions/auth/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1706 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/sessions/auth/hmac_auth.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1539 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/sessions/auth/tc_auth.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1835 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/sessions/auth/token_auth.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    12891 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/sessions/external_session.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4923 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/sessions/rate_limit_handler.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4420 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/sessions/tc_session.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    19749 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/tcex.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.573695 tcex-3.0.7/tcex/tokens/
--rw-rw-r--   0 bsummers   (503) staff       (20)       80 2020-09-04 22:24:44.000000 tcex-3.0.7/tcex/tokens/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    12245 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/tokens/tokens.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.577509 tcex-3.0.7/tcex/utils/
--rw-rw-r--   0 bsummers   (503) staff       (20)       78 2020-09-04 22:24:44.000000 tcex-3.0.7/tcex/utils/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1822 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/utils/aes_operations.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    10144 2022-06-29 14:32:21.000000 tcex-3.0.7/tcex/utils/datetime_operations.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7272 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/utils/file_operations.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.578352 tcex-3.0.7/tcex/utils/models/
--rw-rw-r--   0 bsummers   (503) staff       (20)      127 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/utils/models/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      667 2022-03-08 20:24:00.000000 tcex-3.0.7/tcex/utils/models/playbook_variable_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4889 2023-02-02 18:36:54.000000 tcex-3.0.7/tcex/utils/requests_to_curl.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7751 2023-02-07 21:10:46.000000 tcex-3.0.7/tcex/utils/string_operations.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6165 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/utils/utils.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7352 2022-11-14 21:07:06.000000 tcex-3.0.7/tcex/utils/variables.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-02-07 21:10:47.416980 tcex-3.0.7/tcex.egg-info/
--rw-rw-r--   0 bsummers   (503) staff       (20)     3508 2023-02-07 21:10:47.000000 tcex-3.0.7/tcex.egg-info/PKG-INFO
--rw-rw-r--   0 bsummers   (503) staff       (20)    14001 2023-02-07 21:10:47.000000 tcex-3.0.7/tcex.egg-info/SOURCES.txt
--rw-rw-r--   0 bsummers   (503) staff       (20)        1 2023-02-07 21:10:47.000000 tcex-3.0.7/tcex.egg-info/dependency_links.txt
--rw-rw-r--   0 bsummers   (503) staff       (20)      860 2023-02-07 21:10:47.000000 tcex-3.0.7/tcex.egg-info/requires.txt
--rw-rw-r--   0 bsummers   (503) staff       (20)        5 2023-02-07 21:10:47.000000 tcex-3.0.7/tcex.egg-info/top_level.txt
--rw-rw-r--   0 bsummers   (503) staff       (20)        1 2023-02-07 21:10:47.000000 tcex-3.0.7/tcex.egg-info/zip-safe
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.428491 tcex-3.0.8/
+-rw-rw-r--   0 bsummers   (503) staff       (20)    11357 2019-02-12 17:08:25.000000 tcex-3.0.8/LICENSE
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3508 2023-04-10 17:48:24.428624 tcex-3.0.8/PKG-INFO
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2211 2022-11-14 21:07:06.000000 tcex-3.0.8/README.md
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.266764 tcex-3.0.8/bin/
+-rw-rw-r--   0 bsummers   (503) staff       (20)    15774 2023-04-10 17:48:00.000000 tcex-3.0.8/bin/tcex
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1006 2023-04-10 17:48:00.000000 tcex-3.0.8/pyproject.toml
+-rw-rw-r--   0 bsummers   (503) staff       (20)      772 2023-04-10 17:48:24.429189 tcex-3.0.8/setup.cfg
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3081 2023-04-10 17:48:00.000000 tcex-3.0.8/setup.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.267810 tcex-3.0.8/tcex/
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1139 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      432 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/__metadata__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.270634 tcex-3.0.8/tcex/api/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       76 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      765 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/api.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.271340 tcex-3.0.8/tcex/api/tc/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       91 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2052 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/tc.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.272600 tcex-3.0.8/tcex/api/tc/ti_transform/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      141 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/ti_transform/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      196 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/ti_transform/formatters.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.273255 tcex-3.0.8/tcex/api/tc/ti_transform/model/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      353 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/ti_transform/model/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7541 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/ti_transform/model/transform_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6377 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/ti_transform/ti_transform.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    25131 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/ti_transform/transform_abc.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.274002 tcex-3.0.8/tcex/api/tc/utils/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       39 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/utils/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    14736 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/utils/threat_intel_utils.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.274944 tcex-3.0.8/tcex/api/tc/v2/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      100 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.279547 tcex-3.0.8/tcex/api/tc/v2/batch/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      228 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/batch/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2671 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v2/batch/attribute.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    44500 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v2/batch/batch.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    18746 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v2/batch/batch_submit.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    51366 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v2/batch/batch_writer.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    23538 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v2/batch/group.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    29032 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v2/batch/indicator.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1768 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v2/batch/security_label.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1161 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v2/batch/tag.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.280722 tcex-3.0.8/tcex/api/tc/v2/datastore/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      114 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/datastore/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7077 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/datastore/cache.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    11000 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v2/datastore/datastore.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.281589 tcex-3.0.8/tcex/api/tc/v2/metrics/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       84 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/metrics/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6543 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/metrics/metrics.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.282287 tcex-3.0.8/tcex/api/tc/v2/notifications/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      102 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/notifications/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3187 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/notifications/notifications.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.284247 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      118 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.287626 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/
+-rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2386 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/filters.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.288142 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/
+-rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3731 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.293445 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/
+-rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8796 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/adversary.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      947 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/attack_pattern.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1625 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/campaign.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      953 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/course_of_action.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4495 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/document.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1112 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/email.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2339 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/event.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2340 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/incident.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      951 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/intrusion_set.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      867 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/malware.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3710 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/report.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1564 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/signature.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      841 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/tactic.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      843 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/threat.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      831 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/tool.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      947 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/vulnerability.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.293961 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/
+-rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    10357 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.295909 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/
+-rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2166 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/address.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2041 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/email_address.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7612 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/file.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3127 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/host.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2103 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/url.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    22774 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/mappings.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2241 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/owner.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2945 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/security_label.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2545 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/tag.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1249 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/tags.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8676 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/task.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    15032 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/victim.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    57009 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/tcex_ti_tc_request.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    35065 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/threat_intelligence.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7064 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v2/v2.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.299481 tcex-3.0.8/tcex/api/tc/v3/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       53 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.303442 tcex-3.0.8/tcex/api/tc/v3/_gen/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     9764 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/_gen.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    19062 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3450 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_args_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    18924 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_filter_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    16667 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_model_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    38886 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_object_abc.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.305610 tcex-3.0.8/tcex/api/tc/v3/_gen/models/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      176 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/models/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4059 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/models/_filter_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    14547 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/_gen/models/_property_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.306174 tcex-3.0.8/tcex/api/tc/v3/adversary_assets/
+-rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/adversary_assets/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1003 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/api_endpoints.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.308694 tcex-3.0.8/tcex/api/tc/v3/artifact_types/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/artifact_types/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3157 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/artifact_types/artifact_type.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2770 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/artifact_types/artifact_type_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2982 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/artifact_types/artifact_type_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.311367 tcex-3.0.8/tcex/api/tc/v3/artifacts/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/artifacts/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6810 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/artifacts/artifact.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6061 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v3/artifacts/artifact_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8747 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/artifacts/artifact_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.313621 tcex-3.0.8/tcex/api/tc/v3/attribute_types/
+-rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/attribute_types/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3482 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/attribute_types/attribute_type.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3206 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/attribute_types/attribute_type_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3261 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/attribute_types/attribute_type_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.314731 tcex-3.0.8/tcex/api/tc/v3/attributes/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/attributes/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2234 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/attributes/attribute_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.316429 tcex-3.0.8/tcex/api/tc/v3/case_attributes/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/case_attributes/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4753 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/case_attributes/case_attribute.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6577 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/case_attributes/case_attribute_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4834 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/case_attributes/case_attribute_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.317595 tcex-3.0.8/tcex/api/tc/v3/case_management/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       63 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/case_management/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    22368 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/case_management/case_management.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.320006 tcex-3.0.8/tcex/api/tc/v3/cases/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/cases/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    12920 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/cases/case.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    16300 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/cases/case_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    12033 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/cases/case_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.321175 tcex-3.0.8/tcex/api/tc/v3/file_actions/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/api/tc/v3/file_actions/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1797 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/api/tc/v3/file_actions/file_action_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.322333 tcex-3.0.8/tcex/api/tc/v3/file_occurrences/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/api/tc/v3/file_occurrences/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1641 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/api/tc/v3/file_occurrences/file_occurrence_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1371 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/filter_abc.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.324563 tcex-3.0.8/tcex/api/tc/v3/group_attributes/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/group_attributes/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4856 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/group_attributes/group_attribute.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7370 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/group_attributes/group_attribute_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5255 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/group_attributes/group_attribute_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.326684 tcex-3.0.8/tcex/api/tc/v3/groups/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/groups/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    15307 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/groups/group.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    22742 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/groups/group_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    16799 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/groups/group_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.328321 tcex-3.0.8/tcex/api/tc/v3/indicator_attributes/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/indicator_attributes/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4980 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/indicator_attributes/indicator_attribute.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7466 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/indicator_attributes/indicator_attribute_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5383 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/indicator_attributes/indicator_attribute_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.330509 tcex-3.0.8/tcex/api/tc/v3/indicators/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/indicators/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    14868 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/indicators/indicator.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    20183 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/indicators/indicator_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    17137 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/indicators/indicator_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.332776 tcex-3.0.8/tcex/api/tc/v3/notes/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/notes/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3463 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/notes/note.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4852 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v3/notes/note_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6026 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/notes/note_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    12632 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/object_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8527 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/object_collection_abc.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.335300 tcex-3.0.8/tcex/api/tc/v3/security/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1393 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/assignee_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      741 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/assignee_user_group_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      716 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/assignee_user_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.336885 tcex-3.0.8/tcex/api/tc/v3/security/owner_roles/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/owner_roles/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2878 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/owner_roles/owner_role.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3600 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/owner_roles/owner_role_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3530 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/owner_roles/owner_role_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.338234 tcex-3.0.8/tcex/api/tc/v3/security/owners/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/owners/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2761 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/owners/owner.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    10858 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/owners/owner_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7508 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/owners/owner_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2266 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/security.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.339741 tcex-3.0.8/tcex/api/tc/v3/security/system_roles/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/system_roles/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2905 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/system_roles/system_role.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2052 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/system_roles/system_role_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2697 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/system_roles/system_role_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2650 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/task_assignee_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.340983 tcex-3.0.8/tcex/api/tc/v3/security/user_groups/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/user_groups/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2878 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/user_groups/user_group.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1411 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/user_groups/user_group_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2739 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/user_groups/user_group_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.342361 tcex-3.0.8/tcex/api/tc/v3/security/users/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/users/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2734 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security/users/user.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6970 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/api/tc/v3/security/users/user_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2021 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/security/users/user_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.343758 tcex-3.0.8/tcex/api/tc/v3/security_labels/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/security_labels/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4337 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/security_labels/security_label.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6009 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v3/security_labels/security_label_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3134 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v3/security_labels/security_label_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.345015 tcex-3.0.8/tcex/api/tc/v3/tags/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/tags/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3980 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/tags/tag.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6091 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v3/tags/tag_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4349 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/tags/tag_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.346187 tcex-3.0.8/tcex/api/tc/v3/tasks/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/tasks/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6646 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/tasks/task.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     9537 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v3/tasks/task_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7442 2022-03-23 20:18:24.000000 tcex-3.0.8/tcex/api/tc/v3/tasks/task_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.347004 tcex-3.0.8/tcex/api/tc/v3/threat_intelligence/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       67 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/threat_intelligence/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    17553 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/threat_intelligence/threat_intelligence.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.348438 tcex-3.0.8/tcex/api/tc/v3/tql/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       51 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/tql/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2222 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/api/tc/v3/tql/tql.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      520 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/tql/tql_operator.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      251 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/tql/tql_type.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1321 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v3/v3.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    18104 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/api/tc/v3/v3_model_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1647 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/v3_types.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.349700 tcex-3.0.8/tcex/api/tc/v3/victim_assets/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/victim_assets/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5821 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/api/tc/v3/victim_assets/victim_asset.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5222 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/victim_assets/victim_asset_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5177 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/victim_assets/victim_asset_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.350860 tcex-3.0.8/tcex/api/tc/v3/victim_attributes/
+-rw-rw-r--   0 bsummers   (503) staff       (20)        0 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/victim_attributes/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4815 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/victim_attributes/victim_attribute.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7027 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/victim_attributes/victim_attribute_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4879 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/api/tc/v3/victim_attributes/victim_attribute_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.352488 tcex-3.0.8/tcex/api/tc/v3/victims/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/victims/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7916 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/api/tc/v3/victims/victim.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     9140 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/victims/victim_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6561 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/victims/victim_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.355097 tcex-3.0.8/tcex/api/tc/v3/workflow_events/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/workflow_events/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4550 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/workflow_events/workflow_event.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4075 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/api/tc/v3/workflow_events/workflow_event_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5484 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/workflow_events/workflow_event_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.357693 tcex-3.0.8/tcex/api/tc/v3/workflow_templates/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       56 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/api/tc/v3/workflow_templates/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3611 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/api/tc/v3/workflow_templates/workflow_template.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3449 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/api/tc/v3/workflow_templates/workflow_template_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5159 2022-03-23 20:18:24.000000 tcex-3.0.8/tcex/api/tc/v3/workflow_templates/workflow_template_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.364794 tcex-3.0.8/tcex/app_config/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      327 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/app_config/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    21393 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/app_config/app_spec_yml.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     9324 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/app_config/install_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6004 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/app_config/install_json_update.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1485 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/app_config/install_json_validate.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2061 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/app_config/job_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4484 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/app_config/layout_json.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.368857 tcex-3.0.8/tcex/app_config/models/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      464 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/app_config/models/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    13834 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/app_config/models/app_spec_yml_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    29279 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/app_config/models/install_json_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2993 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/app_config/models/job_json_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2853 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/app_config/models/layout_json_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1833 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/app_config/models/tcex_json_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      914 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/app_config/models/template_config_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    20625 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/app_config/permutation.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2973 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/app_config/tcex_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3222 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/app_config/tcex_json_update.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.369779 tcex-3.0.8/tcex/app_feature/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      135 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/app_feature/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5615 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/app_feature/advanced_request.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.370248 tcex-3.0.8/tcex/backports/
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1066 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/backports/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.378474 tcex-3.0.8/tcex/bin/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      284 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/bin/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6525 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/bin/bin_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    17417 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/bin/dep.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5090 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/bin/deploy.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     9593 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/bin/package.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    11318 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/bin/spec_tool.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    22766 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/bin/spec_tool_app_input.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8530 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/bin/spec_tool_app_input_static.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    11155 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/bin/spec_tool_app_spec_yml.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5739 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/bin/spec_tool_install_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1587 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/bin/spec_tool_job_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      981 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/bin/spec_tool_layout_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    14062 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/bin/spec_tool_readme_md.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1057 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/bin/spec_tool_tcex_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    21485 2023-04-10 17:48:00.000000 tcex-3.0.8/tcex/bin/template.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    21765 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/bin/validate.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.382766 tcex-3.0.8/tcex/decorators/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      360 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/decorators/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2335 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/decorators/benchmark.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1558 2020-09-04 22:24:44.000000 tcex-3.0.8/tcex/decorators/debug.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4525 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/decorators/fail_on_output.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3681 2022-03-23 20:18:24.000000 tcex-3.0.8/tcex/decorators/on_exception.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1828 2020-09-04 22:24:44.000000 tcex-3.0.8/tcex/decorators/on_success.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3482 2020-09-04 22:24:44.000000 tcex-3.0.8/tcex/decorators/output.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.384490 tcex-3.0.8/tcex/exit/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      192 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/exit/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5374 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/exit/error_codes.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6516 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/exit/exit.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.385575 tcex-3.0.8/tcex/input/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       92 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.395011 tcex-3.0.8/tcex/input/field_types/
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1242 2022-03-23 20:18:24.000000 tcex-3.0.8/tcex/input/field_types/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3532 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/field_types/binary.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3129 2022-03-23 20:18:24.000000 tcex-3.0.8/tcex/input/field_types/case_management_entity.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1581 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/field_types/choice.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      866 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/field_types/datetime.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3764 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/field_types/edit_choice.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3073 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/field_types/exception.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2995 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/field_types/group_entity.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2725 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/field_types/indicator_entity.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3505 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/input/field_types/integer.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2336 2022-03-23 20:18:24.000000 tcex-3.0.8/tcex/input/field_types/ip_address.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1270 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/field_types/key_value.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5151 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/input/field_types/sensitive.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4111 2022-03-23 20:18:24.000000 tcex-3.0.8/tcex/input/field_types/string.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1251 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/field_types/tc_entity.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8590 2022-03-23 20:18:24.000000 tcex-3.0.8/tcex/input/field_types/validators.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    15693 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/input/input.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.402222 tcex-3.0.8/tcex/input/models/
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1012 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2575 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/input/models/advanced_request_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      999 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/aot_execution_enabled_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2935 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/input/models/api_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1525 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/batch_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      893 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/cal_settings_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1567 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/input/models/create_config_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1595 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/logging_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2736 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/input/models/model_map.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      428 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/organization_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1162 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/path_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1151 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/playbook_common_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      929 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/playbook_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1350 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/proxy_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2716 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/service_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1174 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/input/models/smtp_settings_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.405595 tcex-3.0.8/tcex/key_value_store/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      224 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/key_value_store/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      873 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/key_value_store/key_value_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2499 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/key_value_store/key_value_api.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1801 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/key_value_store/key_value_mock.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2777 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/key_value_store/key_value_redis.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1669 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/key_value_store/redis_client.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.410599 tcex-3.0.8/tcex/logger/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      293 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/logger/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3780 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/logger/api_handler.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      862 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/logger/cache_handler.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    13964 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/logger/logger.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3112 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/logger/pattern_file_handler.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2001 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/logger/rotating_file_handler_custom.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      974 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/logger/sensitive_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1822 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/logger/thread_file_handler.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1206 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/logger/trace_logger.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.414162 tcex-3.0.8/tcex/playbook/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       88 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/playbook/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3467 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/playbook/playbook.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    20899 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/playbook/playbook_create.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1027 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/playbook/playbook_delete.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      668 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/playbook/playbook_output.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    22857 2022-08-26 17:57:26.000000 tcex-3.0.8/tcex/playbook/playbook_read.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.417968 tcex-3.0.8/tcex/pleb/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       26 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/pleb/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1599 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/pleb/env_path.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      737 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/pleb/event.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      536 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/pleb/none_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1178 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/pleb/proxies.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7213 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/pleb/registry.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2311 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/pleb/scoped_property.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      412 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/pleb/singleton.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      731 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/pleb/threading.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.420337 tcex-3.0.8/tcex/services/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      324 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/services/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    11874 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/services/api_service.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    16230 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/services/common_service.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    17548 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/services/common_service_trigger.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    10563 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/services/mqtt_message_broker.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    15948 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/services/webhook_trigger_service.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.421797 tcex-3.0.8/tcex/sessions/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       40 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/sessions/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.423269 tcex-3.0.8/tcex/sessions/auth/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       31 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/sessions/auth/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1706 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/sessions/auth/hmac_auth.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1539 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/sessions/auth/tc_auth.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1835 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/sessions/auth/token_auth.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    12891 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/sessions/external_session.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4923 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/sessions/rate_limit_handler.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4420 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/sessions/tc_session.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    19749 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/tcex.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.424030 tcex-3.0.8/tcex/tokens/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       80 2020-09-04 22:24:44.000000 tcex-3.0.8/tcex/tokens/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    12245 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/tokens/tokens.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.427409 tcex-3.0.8/tcex/utils/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       78 2020-09-04 22:24:44.000000 tcex-3.0.8/tcex/utils/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1822 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/utils/aes_operations.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    10144 2022-06-29 14:32:21.000000 tcex-3.0.8/tcex/utils/datetime_operations.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7272 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/utils/file_operations.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.428128 tcex-3.0.8/tcex/utils/models/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      127 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/utils/models/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      667 2022-03-08 20:24:00.000000 tcex-3.0.8/tcex/utils/models/playbook_variable_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4889 2023-02-02 18:36:54.000000 tcex-3.0.8/tcex/utils/requests_to_curl.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7751 2023-02-07 21:10:46.000000 tcex-3.0.8/tcex/utils/string_operations.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6165 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/utils/utils.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7352 2022-11-14 21:07:06.000000 tcex-3.0.8/tcex/utils/variables.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-04-10 17:48:24.269885 tcex-3.0.8/tcex.egg-info/
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3508 2023-04-10 17:48:24.000000 tcex-3.0.8/tcex.egg-info/PKG-INFO
+-rw-rw-r--   0 bsummers   (503) staff       (20)    14001 2023-04-10 17:48:24.000000 tcex-3.0.8/tcex.egg-info/SOURCES.txt
+-rw-rw-r--   0 bsummers   (503) staff       (20)        1 2023-04-10 17:48:24.000000 tcex-3.0.8/tcex.egg-info/dependency_links.txt
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1019 2023-04-10 17:48:24.000000 tcex-3.0.8/tcex.egg-info/requires.txt
+-rw-rw-r--   0 bsummers   (503) staff       (20)        5 2023-04-10 17:48:24.000000 tcex-3.0.8/tcex.egg-info/top_level.txt
+-rw-rw-r--   0 bsummers   (503) staff       (20)        1 2023-04-10 17:48:24.000000 tcex-3.0.8/tcex.egg-info/zip-safe
```

### Comparing `tcex-3.0.7/LICENSE` & `tcex-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/PKG-INFO` & `tcex-3.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tcex
-Version: 3.0.7
+Version: 3.0.8
 Summary: ThreatConnect Exchange App Framework
 Home-page: https://github.com/ThreatConnect-Inc/tcex
-Download-URL: https://github.com/ThreatConnect-Inc/tcex/tarball/3.0.7
+Download-URL: https://github.com/ThreatConnect-Inc/tcex/tarball/3.0.8
 Author: ThreatConnect (support@threatconnect.com)
 Author-email: support@threatconnect.com
 License: Apache License, Version 2
 Project-URL: Documentation, https://github.com/ThreatConnect-Inc/tcex
 Project-URL: Source, https://github.com/ThreatConnect-Inc/tcex
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `tcex-3.0.7/README.md` & `tcex-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/bin/tcex` & `tcex-3.0.8/bin/tcex`

 * *Files 6% similar despite different names*

```diff
@@ -178,20 +178,37 @@
     force: bool = typer.Option(False, help='Force App init even if files exist in directory.'),
     branch: Optional[str] = typer.Option(
         'main', help='The git branch of the tcex-app-template repository to use.'
     ),
     app_builder: Optional[bool] = typer.Option(
         False, help='Include .appbuilderconfig file in template download.'
     ),
+    proxy_host: Optional[str] = typer.Option(
+        None, help='(Advanced) Hostname for the proxy server.'
+    ),
+    proxy_port: Optional[int] = typer.Option(
+        None, help='(Advanced) Port number for the proxy server.'
+    ),
+    proxy_user: Optional[str] = typer.Option(
+        None, help='(Advanced) Username for the proxy server.'
+    ),
+    proxy_pass: Optional[str] = typer.Option(
+        None, help='(Advanced) Password for the proxy server.'
+    ),
 ):
     """Initialize a new App from a template.
 
     Templates can be found at: https://github.com/ThreatConnect-Inc/tcex-app-templates
     """
-    tt = Template()
+    tt = Template(
+        proxy_host,
+        proxy_port,
+        proxy_user,
+        proxy_pass,
+    )
     if os.listdir(os.getcwd()) and force is False:
         tt.print_block(
             'The current directory does not appear to be empty. Apps should '
             'be initialized in an empty directory. If attempting to update an '
             'existing App then please try using the "tcex update" command instead.',
             fg_color='yellow',
         )
@@ -226,22 +243,39 @@
 
 @app.command('list')
 def _list(
     type_: Optional[str] = typer.Option(None, '--type', help='The App type being initialized.'),
     branch: Optional[str] = typer.Option(
         'main', help='The git branch of the tcex-app-template repository to use.'
     ),
+    proxy_host: Optional[str] = typer.Option(
+        None, help='(Advanced) Hostname for the proxy server.'
+    ),
+    proxy_port: Optional[int] = typer.Option(
+        None, help='(Advanced) Port number for the proxy server.'
+    ),
+    proxy_user: Optional[str] = typer.Option(
+        None, help='(Advanced) Username for the proxy server.'
+    ),
+    proxy_pass: Optional[str] = typer.Option(
+        None, help='(Advanced) Password for the proxy server.'
+    ),
 ):
     """List templates
 
     The template name will be pulled from tcex.json by default. If the template option
     is provided it will be used instead of the value in the tcex.json file. The tcex.json
     file will also be updated with new values.
     """
-    tt = Template()
+    tt = Template(
+        proxy_host,
+        proxy_port,
+        proxy_user,
+        proxy_pass,
+    )
     try:
         tt.list(branch, type_)
         tt.print_list(branch)
         tt.print_error_message()
     except Exception as ex:
         tt.log.error(traceback.format_exc())
         typer.echo(f'Failed getting App templates: {ex}', err=True)
@@ -308,14 +342,26 @@
     type_: str = typer.Option(None, '--type', help='The App type being initialized.'),
     branch: Optional[str] = typer.Option(
         'main', help='The git branch of the tcex-app-template repository to use.'
     ),
     force: bool = typer.Option(
         False, help="Update files from template even if they haven't changed."
     ),
+    proxy_host: Optional[str] = typer.Option(
+        None, help='(Advanced) Hostname for the proxy server.'
+    ),
+    proxy_port: Optional[int] = typer.Option(
+        None, help='(Advanced) Port number for the proxy server.'
+    ),
+    proxy_user: Optional[str] = typer.Option(
+        None, help='(Advanced) Username for the proxy server.'
+    ),
+    proxy_pass: Optional[str] = typer.Option(
+        None, help='(Advanced) Password for the proxy server.'
+    ),
 ):
     """Update a project with the latest template files.
 
     Templates can be found at: https://github.com/ThreatConnect-Inc/tcex-app-templates
 
     The template name will be pulled from tcex.json by default. If the template option
     is provided it will be used instead of the value in the tcex.json file. The tcex.json
@@ -325,15 +371,20 @@
     if not os.path.isfile('tcex.json'):
         typer.secho(
             'Update requires a tcex.json file, "external" App templates can not be update.',
             fg=typer.colors.RED,
         )
         raise typer.Exit(code=1)
 
-    tt = Template()
+    tt = Template(
+        proxy_host,
+        proxy_port,
+        proxy_user,
+        proxy_pass,
+    )
     try:
         downloads = tt.update(branch, template, type_, force)
         tt.print_title('Updating template files ...', divider=False, fg_color='white')
         if not downloads:
             typer.secho('\nNo files to update.', fg=typer.colors.GREEN)
         else:
             typer.echo('')  # add additional space before progress bar
```

### Comparing `tcex-3.0.7/pyproject.toml` & `tcex-3.0.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -23,11 +23,12 @@
 # W0707 - raise-missing-from
 # W1203 - logging-fstring-interpolation
 # W1514 - Using open without explicitly specifying an encoding (unspecified-encoding)
 disable = "C0103,C0302,C0330,C0415,E0401,R0205,R0801,R0902,R0903,R0904,R0912,R0913,R0914,R0915,R1702,W0212,W0511,W0703,W0707,W1203,W1514"
 extension-pkg-whitelist = "pydantic"
 
 [tool.pytest.ini_options]
+# addopts = "-n auto"
 junit_family = "xunit2"
 testpaths = [
   "tests",
 ]
```

### Comparing `tcex-3.0.7/setup.cfg` & `tcex-3.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/setup.py` & `tcex-3.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,29 +17,29 @@
 if not metadata:
     raise RuntimeError(f'Could not load metadata file ({metadata_file}).')
 
 with open('README.md') as f:
     readme = f.read()
 
 dev_packages = [
-    'black',
-    'codespell',
+    'black==22.8.0',
+    'codespell==2.2.1',
     'fakeredis==1.7.0',
-    'flake8',
-    'isort>=5.0.0',
-    'mako',
-    'pre-commit',
+    'flake8==5.0.4',
+    'isort==5.10.1',
+    'mako==1.1.6',
+    'pre-commit==2.17.0',
     'pydocstyle',
     'pylint>=2.5.0,<2.14.0',
-    'pytest',
+    'pytest==7.0.1',
     'pytest-cov',
     'pytest-html',
     'pytest-ordering',
-    'pytest-xdist>=2.5.0',
-    'pyupgrade',
+    'pytest-xdist==3.0.2',
+    'pyupgrade==2.31.0',
 ]
 if sys.version_info <= (3, 7):
     # these packages dropped support for 3.6
     dev_packages.extend(['bandit==1.7.1', 'deepdiff==5.7.0'])
 else:
     dev_packages.extend(['bandit', 'deepdiff'])
```

### Comparing `tcex-3.0.7/tcex/__init__.py` & `tcex-3.0.8/tcex/__init__.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/api.py` & `tcex-3.0.8/tcex/api/api.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/tc.py` & `tcex-3.0.8/tcex/api/tc/tc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/ti_transform/model/transform_model.py` & `tcex-3.0.8/tcex/api/tc/ti_transform/model/transform_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,15 @@
     value3: Optional[MetadataTransformModel] = Field(None, description='')
     # file
     file_occurrences: Optional[List[FileOccurrenceTransformModel]] = Field(None, description='')
     size: Optional[MetadataTransformModel] = Field(None, description='')
     # host
     dns_active: Optional[MetadataTransformModel] = Field(None, description='')
     whois_active: Optional[MetadataTransformModel] = Field(None, description='')
+    active: Optional[MetadataTransformModel] = Field(None, description='')
 
     # root validator that ensure at least one indicator value/summary is set
     @root_validator()
     def _one_indicator_value(cls, values):
         """Validate that one set of credentials is provided for the TC API."""
 
         if not any(
```

### Comparing `tcex-3.0.7/tcex/api/tc/ti_transform/ti_transform.py` & `tcex-3.0.8/tcex/api/tc/ti_transform/ti_transform.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/ti_transform/transform_abc.py` & `tcex-3.0.8/tcex/api/tc/ti_transform/transform_abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,25 +233,17 @@
             types = self._process_metadata_transform_model(attribute.type, len(values))
             source = self._process_metadata_transform_model(attribute.source, len(values))
             displayed = self._process_metadata_transform_model(attribute.displayed, len(values))
 
             param_keys = ['type_', 'value', 'displayed', 'source']
             params = [dict(zip(param_keys, p)) for p in zip(types, values, displayed, source)]
 
-            # self.log.trace(
-            #     f'feature=transform, action=process-attributes, values={values}, '
-            #     f'types={types}, source={source}, displayed={displayed}, params={params}'
-            # )
             for param in params:
                 param = self.utils.remove_none(param)
                 if 'value' not in param:
-                    self.log.warning(
-                        'feature=transform, action=process-attribute, '
-                        f'transform={attribute.dict(exclude_unset=True)}, error=no-value'
-                    )
                     continue
 
                 if 'type_' not in param:
                     self.log.warning(
                         'feature=transform, action=process-attribute, '
                         f'transform={attribute.dict(exclude_unset=True)}, error=no-type'
                     )
@@ -318,15 +310,15 @@
             self._process_metadata('password', self.transform.confidence)
 
         if self.transformed_item['type'] == 'Email':
             self._process_metadata('from', self.transform.from_addr)
             self._process_metadata('to', self.transform.to_addr)
 
         if self.transformed_item['type'] in ('Event', 'Incident'):
-            self._process_metadata('eventDate', self.transform.event_date)
+            self._process_metadata_datetime('eventDate', self.transform.event_date)
             self._process_metadata('status', self.transform.status)
 
         if self.transformed_item['type'] == 'Report':
             self._process_metadata('fileName', self.transform.file_name)
             self._process_metadata_datetime('publishDate', self.transform.publish_date)
 
         # Handle sig specific fields here
@@ -336,14 +328,17 @@
             self._process_metadata('fileText', self.transform.file_text)
 
     def _process_indicator(self):
         """Process Indicator Specific data."""
         # handle the 3 possible indicator fields
         self._process_indicator_values()
 
+        if self.transform.active:
+            self._process_metadata('active', self.transform.active)
+
         self._process_confidence(self.transform.confidence)
         self._process_rating(self.transform.rating)
 
         if self.transformed_item['type'] == 'File':
             self._process_metadata('size', self.transform.size)
             self._process_file_occurrences(self.transform.file_occurrences or [])
 
@@ -401,28 +396,26 @@
             if not names:
                 # self.log.info(f'No values found for security label transform {label.dict()}')
                 continue
 
             descriptions = self._process_metadata_transform_model(
                 label.description, expected_length=len(names)
             )
-            colors = self._process_metadata_transform_model(
-                label.colors, expected_length=len(names)
-            )
+            colors = self._process_metadata_transform_model(label.color, expected_length=len(names))
 
             param_keys = ['color', 'description', 'name']
             params = [dict(zip(param_keys, p)) for p in zip(colors, descriptions, names)]
 
             for kwargs in params:
+                kwargs = self.utils.remove_none(kwargs)
                 if 'name' not in kwargs:
-                    self.log.warning(f'Attribute transform {label.dict()} did not yield a name')
                     continue
                 # strip out None params so that required params are enforced and optional
                 # params with default values are respected.
-                self.add_security_label(**self.utils.remove_none(kwargs))
+                self.add_security_label(**kwargs)
 
     def _process_tags(self, tags: List['TagTransformModel']):
         """Process Tag data"""
         for tag in tags or []:
             for value in filter(bool, self._process_metadata_transform_model(tag.value)):
                 self.add_tag(name=value)
```

### Comparing `tcex-3.0.7/tcex/api/tc/utils/threat_intel_utils.py` & `tcex-3.0.8/tcex/api/tc/utils/threat_intel_utils.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/batch/attribute.py` & `tcex-3.0.8/tcex/api/tc/v2/batch/attribute.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/batch/batch.py` & `tcex-3.0.8/tcex/api/tc/v2/batch/batch.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/batch/batch_submit.py` & `tcex-3.0.8/tcex/api/tc/v2/batch/batch_submit.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/batch/batch_writer.py` & `tcex-3.0.8/tcex/api/tc/v2/batch/batch_writer.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/batch/group.py` & `tcex-3.0.8/tcex/api/tc/v2/batch/group.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/batch/indicator.py` & `tcex-3.0.8/tcex/api/tc/v2/batch/indicator.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/batch/security_label.py` & `tcex-3.0.8/tcex/api/tc/v2/batch/security_label.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/batch/tag.py` & `tcex-3.0.8/tcex/api/tc/v2/batch/tag.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/datastore/cache.py` & `tcex-3.0.8/tcex/api/tc/v2/datastore/cache.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/datastore/datastore.py` & `tcex-3.0.8/tcex/api/tc/v2/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/metrics/metrics.py` & `tcex-3.0.8/tcex/api/tc/v2/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/notifications/notifications.py` & `tcex-3.0.8/tcex/api/tc/v2/notifications/notifications.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/filters.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/filters.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/adversary.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/adversary.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/attack_pattern.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/attack_pattern.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/campaign.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/campaign.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/course_of_action.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/course_of_action.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/document.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/document.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/email.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/email.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/event.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/event.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/incident.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/incident.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/intrusion_set.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/intrusion_set.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/malware.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/malware.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/report.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/report.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/signature.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/signature.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/tactic.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/tactic.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/threat.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/threat.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/tool.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/tool.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/vulnerability.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/group/group_types/vulnerability.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/address.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/address.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/email_address.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/email_address.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/file.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/file.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/host.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/host.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/url.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/indicator/indicator_types/url.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/mappings.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/mappings.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/owner.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/owner.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/security_label.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/security_label.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/tag.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/tag.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/tags.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/tags.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/task.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/task.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/mappings/victim.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/mappings/victim.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/tcex_ti_tc_request.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/tcex_ti_tc_request.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/threat_intelligence/threat_intelligence.py` & `tcex-3.0.8/tcex/api/tc/v2/threat_intelligence/threat_intelligence.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v2/v2.py` & `tcex-3.0.8/tcex/api/tc/v2/v2.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/_gen/_gen.py` & `tcex-3.0.8/tcex/api/tc/v3/_gen/_gen.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/_gen/_gen_abc.py` & `tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_abc.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,14 +171,18 @@
 
         # remove unused fields, if any
         self._prop_content_remove_unused(_properties)
 
         # update "bad" data
         self._prop_content_update(_properties)
 
+        # Temp issue
+        if self.type_ == 'indicators':
+            _properties['enrichment']['data'][0]['type'] = 'Enrichment'
+
         # critical fix for breaking API change
         if self.type_ in [
             'case_attributes',
             'group_attributes',
             'indicator_attributes',
             'victim_attributes',
         ]:
@@ -377,16 +381,18 @@
                 if field in properties:
                     del properties[field]
 
     def _prop_content_update(self, properties: dict):
         """Update "bad" data in properties."""
         if self.type_ in ['groups']:
             # fixed fields that are missing readOnly property
-            properties['downVoteCount']['readOnly'] = True
-            properties['upVoteCount']['readOnly'] = True
+            if 'downVoteCount' in properties:
+                properties['downVoteCount']['readOnly'] = True
+            if 'upVoteCount' in properties:
+                properties['upVoteCount']['readOnly'] = True
 
         if self.type_ in ['victims']:
             # ownerName is readOnly, but readOnly is not defined in response from OPTIONS endpoint
             properties['ownerName']['readOnly'] = True
 
     @property
     def _prop_models(self) -> List[PropertyModel]:
```

### Comparing `tcex-3.0.7/tcex/api/tc/v3/_gen/_gen_args_abc.py` & `tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_args_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/_gen/_gen_filter_abc.py` & `tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_filter_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/_gen/_gen_model_abc.py` & `tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_model_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/_gen/_gen_object_abc.py` & `tcex-3.0.8/tcex/api/tc/v3/_gen/_gen_object_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/_gen/models/_filter_model.py` & `tcex-3.0.8/tcex/api/tc/v3/_gen/models/_filter_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/_gen/models/_property_model.py` & `tcex-3.0.8/tcex/api/tc/v3/_gen/models/_property_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,14 +137,19 @@
 
         # # process tc types
         self.__process_tc_types(self, extra)
 
         # process special types
         self.__process_special_types(self, extra)
 
+        if extra.get('typing_type') is None:
+            raise RuntimeError(
+                f'Unable to determine typing_type for name={self.name}, type={self.type}.'
+            )
+
         return extra
 
     def __calculate_methods(self):
         """Calculate the field methods."""
 
         # special case until core updates OPTIONS output
         methods = []
@@ -166,15 +171,15 @@
 
     @classmethod
     def __process_dict_types(cls, pm: 'PropertyModel', extra: Dict[str, str]):
         """Process standard type."""
         types = [
             'AttributeSource',
             'DNSResolutions',
-            'Enrichment',
+            'Enrichments',
             'GeoLocation',
             'InvestigationLinks',
             'Links',
             'Map',
             'ValidationRule',
             'WhoIs',
         ]
@@ -238,24 +243,44 @@
             extra.update(
                 {
                     'import_data': 'from datetime import datetime',
                     'import_source': 'standard library',
                     'typing_type': cls.__extra_format_type('datetime'),
                 }
             )
+        elif pm.type == 'Group':
+            bi += 'groups.group_model'
+            extra.update(
+                {
+                    'import_data': f'{bi} import GroupModel',
+                    'import_source': 'first-party-forward-reference',
+                    'model': f'{pm.type}Model',
+                    'typing_type': cls.__extra_format_type_model(pm.type),
+                }
+            )
         elif pm.type == 'GroupAttributes':
             bi += 'group_attributes.group_attribute_model'
             extra.update(
                 {
                     'import_data': f'{bi} import GroupAttributesModel',
                     'import_source': 'first-party-forward-reference',
                     'model': f'{pm.type}Model',
                     'typing_type': cls.__extra_format_type_model(pm.type),
                 }
             )
+        elif pm.type == 'Indicator':
+            bi += 'indicators.indicator_model'
+            extra.update(
+                {
+                    'import_data': f'{bi} import IndicatorModel',
+                    'import_source': 'first-party-forward-reference',
+                    'model': f'{pm.type}Model',
+                    'typing_type': cls.__extra_format_type_model(pm.type),
+                }
+            )
         elif pm.type == 'IndicatorAttributes':
             bi += 'indicator_attributes.indicator_attribute_model'
             extra.update(
                 {
                     'import_data': f'{bi} import IndicatorAttributesModel',
                     'import_source': 'first-party-forward-reference',
                     'model': f'{pm.type}Model',
```

### Comparing `tcex-3.0.7/tcex/api/tc/v3/api_endpoints.py` & `tcex-3.0.8/tcex/api/tc/v3/api_endpoints.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/artifact_types/artifact_type.py` & `tcex-3.0.8/tcex/api/tc/v3/artifact_types/artifact_type.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/artifact_types/artifact_type_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/artifact_types/artifact_type_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/artifact_types/artifact_type_model.py` & `tcex-3.0.8/tcex/api/tc/v3/artifact_types/artifact_type_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/artifacts/artifact.py` & `tcex-3.0.8/tcex/api/tc/v3/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/artifacts/artifact_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/artifacts/artifact_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/artifacts/artifact_model.py` & `tcex-3.0.8/tcex/api/tc/v3/artifacts/artifact_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/attribute_types/attribute_type.py` & `tcex-3.0.8/tcex/api/tc/v3/attribute_types/attribute_type.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/attribute_types/attribute_type_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/attribute_types/attribute_type_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/attribute_types/attribute_type_model.py` & `tcex-3.0.8/tcex/api/tc/v3/attribute_types/attribute_type_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/attributes/attribute_model.py` & `tcex-3.0.8/tcex/api/tc/v3/attributes/attribute_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/case_attributes/case_attribute.py` & `tcex-3.0.8/tcex/api/tc/v3/case_attributes/case_attribute.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/case_attributes/case_attribute_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/case_attributes/case_attribute_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/case_attributes/case_attribute_model.py` & `tcex-3.0.8/tcex/api/tc/v3/case_attributes/case_attribute_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/case_management/case_management.py` & `tcex-3.0.8/tcex/api/tc/v3/case_management/case_management.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/cases/case.py` & `tcex-3.0.8/tcex/api/tc/v3/cases/case.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/cases/case_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/cases/case_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,14 +285,24 @@
 
         Args:
             operator: The operator enum for the filter.
             id_as_string: The ID of the case as a String.
         """
         self._tql.add_filter('idAsString', operator, id_as_string, TqlType.STRING)
 
+    def last_updated(self, operator: Enum, last_updated: str):
+        """Filter Last Updated based on **lastUpdated** keyword.
+
+        Args:
+            operator: The operator enum for the filter.
+            last_updated: The date the case was last updated in the system.
+        """
+        last_updated = self.utils.any_to_datetime(last_updated).strftime('%Y-%m-%d %H:%M:%S')
+        self._tql.add_filter('lastUpdated', operator, last_updated, TqlType.STRING)
+
     def missing_artifact_count(self, operator: Enum, missing_artifact_count: int):
         """Filter Missing Artifact Count For Tasks based on **missingArtifactCount** keyword.
 
         Args:
             operator: The operator enum for the filter.
             missing_artifact_count: Missing Artifact Count for Case Tasks.
         """
```

### Comparing `tcex-3.0.7/tcex/api/tc/v3/cases/case_model.py` & `tcex-3.0.8/tcex/api/tc/v3/cases/case_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,21 @@
     )
     id: Optional[int] = Field(
         None,
         description='The ID of the item.',
         read_only=True,
         title='id',
     )
+    last_updated: Optional[datetime] = Field(
+        None,
+        allow_mutation=False,
+        description='The date and time that the Case was last updated.',
+        read_only=True,
+        title='lastUpdated',
+    )
     name: Optional[str] = Field(
         None,
         description='The name of the Case.',
         methods=['POST', 'PUT'],
         max_length=255,
         min_length=1,
         read_only=False,
```

### Comparing `tcex-3.0.7/tcex/api/tc/v3/file_actions/file_action_model.py` & `tcex-3.0.8/tcex/api/tc/v3/file_actions/file_action_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/file_occurrences/file_occurrence_model.py` & `tcex-3.0.8/tcex/api/tc/v3/file_occurrences/file_occurrence_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/filter_abc.py` & `tcex-3.0.8/tcex/api/tc/v3/filter_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/group_attributes/group_attribute.py` & `tcex-3.0.8/tcex/api/tc/v3/group_attributes/group_attribute.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 
 class GroupAttribute(ObjectABC):
     """GroupAttributes Object.
 
     Args:
         default (bool, kwargs): A flag indicating that this is the default attribute of its type
             within the object. Only applies to certain attribute and data types.
+        group (Group, kwargs): Details of group associated with attribute.
         group_id (int, kwargs): Group associated with attribute.
         pinned (bool, kwargs): A flag indicating that the attribute has been noted for importance.
         security_labels (SecurityLabels, kwargs): A list of Security Labels corresponding to the
             Intel item (NOTE: Setting this parameter will replace any existing tag(s) with
             the one(s) specified).
         source (str, kwargs): The attribute source.
         type (str, kwargs): The attribute type.
```

### Comparing `tcex-3.0.7/tcex/api/tc/v3/group_attributes/group_attribute_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/group_attributes/group_attribute_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/group_attributes/group_attribute_model.py` & `tcex-3.0.8/tcex/api/tc/v3/group_attributes/group_attribute_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -86,14 +86,21 @@
             'A flag indicating that this is the default attribute of its type within the object. '
             'Only applies to certain attribute and data types.'
         ),
         methods=['POST', 'PUT'],
         read_only=False,
         title='default',
     )
+    group: Optional['GroupModel'] = Field(
+        None,
+        description='Details of group associated with attribute.',
+        methods=['POST'],
+        read_only=False,
+        title='group',
+    )
     group_id: Optional[int] = Field(
         None,
         description='Group associated with attribute.',
         methods=['POST'],
         read_only=False,
         title='groupId',
     )
@@ -146,28 +153,35 @@
         description='The attribute value.',
         methods=['POST', 'PUT'],
         min_length=1,
         read_only=False,
         title='value',
     )
 
+    @validator('group', always=True)
+    def _validate_group(cls, v):
+        if not v:
+            return GroupModel()
+        return v
+
     @validator('security_labels', always=True)
     def _validate_security_labels(cls, v):
         if not v:
             return SecurityLabelsModel()
         return v
 
     @validator('created_by', always=True)
     def _validate_user(cls, v):
         if not v:
             return UserModel()
         return v
 
 
 # first-party
+from tcex.api.tc.v3.groups.group_model import GroupModel
 from tcex.api.tc.v3.security.users.user_model import UserModel
 from tcex.api.tc.v3.security_labels.security_label_model import SecurityLabelsModel
 
 # add forward references
 GroupAttributeDataModel.update_forward_refs()
 GroupAttributeModel.update_forward_refs()
 GroupAttributesModel.update_forward_refs()
```

### Comparing `tcex-3.0.7/tcex/api/tc/v3/groups/group.py` & `tcex-3.0.8/tcex/api/tc/v3/groups/group.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/groups/group_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/groups/group_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,14 +232,23 @@
         # first-party
         from tcex.api.tc.v3.indicators.indicator_filter import IndicatorFilter
 
         indicators = IndicatorFilter(Tql())
         self._tql.add_filter('hasIndicator', TqlOperator.EQ, indicators, TqlType.SUB_QUERY)
         return indicators
 
+    def has_intel_query(self, operator: Enum, has_intel_query: int):
+        """Filter Associated User Queries based on **hasIntelQuery** keyword.
+
+        Args:
+            operator: The operator enum for the filter.
+            has_intel_query: A nested query for association to User Queries.
+        """
+        self._tql.add_filter('hasIntelQuery', operator, has_intel_query, TqlType.INTEGER)
+
     @property
     def has_security_label(self):
         """Return **SecurityLabel** for further filtering."""
         # first-party
         from tcex.api.tc.v3.security_labels.security_label_filter import SecurityLabelFilter
 
         security_labels = SecurityLabelFilter(Tql())
```

### Comparing `tcex-3.0.7/tcex/api/tc/v3/groups/group_model.py` & `tcex-3.0.8/tcex/api/tc/v3/groups/group_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         description='The **created by** for the Group.',
         read_only=True,
         title='createdBy',
     )
     date_added: Optional[datetime] = Field(
         None,
         allow_mutation=False,
-        description='The date and time that the Entity was first created.',
+        description='The date and time that the item was first created.',
         read_only=True,
         title='dateAdded',
     )
     document_date_added: Optional[datetime] = Field(
         None,
         allow_mutation=False,
         applies_to=['Document', 'Report'],
```

### Comparing `tcex-3.0.7/tcex/api/tc/v3/indicator_attributes/indicator_attribute.py` & `tcex-3.0.8/tcex/api/tc/v3/indicator_attributes/indicator_attribute.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 
 class IndicatorAttribute(ObjectABC):
     """IndicatorAttributes Object.
 
     Args:
         default (bool, kwargs): A flag indicating that this is the default attribute of its type
             within the object. Only applies to certain attribute and data types.
+        indicator (Indicator, kwargs): Details of indicator associated with attribute.
         indicator_id (int, kwargs): Indicator associated with attribute.
         pinned (bool, kwargs): A flag indicating that the attribute has been noted for importance.
         security_labels (SecurityLabels, kwargs): A list of Security Labels corresponding to the
             Intel item (NOTE: Setting this parameter will replace any existing tag(s) with
             the one(s) specified).
         source (str, kwargs): The attribute source.
         type (str, kwargs): The attribute type.
```

### Comparing `tcex-3.0.7/tcex/api/tc/v3/indicator_attributes/indicator_attribute_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/indicator_attributes/indicator_attribute_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/indicator_attributes/indicator_attribute_model.py` & `tcex-3.0.8/tcex/api/tc/v3/indicator_attributes/indicator_attribute_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,14 +92,21 @@
     )
     id: Optional[int] = Field(
         None,
         description='The ID of the item.',
         read_only=True,
         title='id',
     )
+    indicator: Optional['IndicatorModel'] = Field(
+        None,
+        description='Details of indicator associated with attribute.',
+        methods=['POST'],
+        read_only=False,
+        title='indicator',
+    )
     indicator_id: Optional[int] = Field(
         None,
         description='Indicator associated with attribute.',
         methods=['POST'],
         read_only=False,
         title='indicatorId',
     )
@@ -146,28 +153,35 @@
         description='The attribute value.',
         methods=['POST', 'PUT'],
         min_length=1,
         read_only=False,
         title='value',
     )
 
+    @validator('indicator', always=True)
+    def _validate_indicator(cls, v):
+        if not v:
+            return IndicatorModel()
+        return v
+
     @validator('security_labels', always=True)
     def _validate_security_labels(cls, v):
         if not v:
             return SecurityLabelsModel()
         return v
 
     @validator('created_by', always=True)
     def _validate_user(cls, v):
         if not v:
             return UserModel()
         return v
 
 
 # first-party
+from tcex.api.tc.v3.indicators.indicator_model import IndicatorModel
 from tcex.api.tc.v3.security.users.user_model import UserModel
 from tcex.api.tc.v3.security_labels.security_label_model import SecurityLabelsModel
 
 # add forward references
 IndicatorAttributeDataModel.update_forward_refs()
 IndicatorAttributeModel.update_forward_refs()
 IndicatorAttributesModel.update_forward_refs()
```

### Comparing `tcex-3.0.7/tcex/api/tc/v3/indicators/indicator.py` & `tcex-3.0.8/tcex/api/tc/v3/indicators/indicator.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/indicators/indicator_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/indicators/indicator_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/indicators/indicator_model.py` & `tcex-3.0.8/tcex/api/tc/v3/indicators/indicator_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,14 +425,21 @@
     threat_assess_score_observed: Optional[int] = Field(
         None,
         allow_mutation=False,
         description='The Threat Assess score observed for this indicator.',
         read_only=True,
         title='threatAssessScoreObserved',
     )
+    tracked_users: Optional[dict] = Field(
+        None,
+        allow_mutation=False,
+        description='List of tracked users and their observation and false positive stats.',
+        read_only=True,
+        title='trackedUsers',
+    )
     type: Optional[str] = Field(
         None,
         description='The **type** for the Indicator.',
         methods=['POST', 'PUT'],
         min_length=1,
         read_only=False,
         title='type',
```

### Comparing `tcex-3.0.7/tcex/api/tc/v3/notes/note.py` & `tcex-3.0.8/tcex/api/tc/v3/notes/note.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/notes/note_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/notes/note_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/notes/note_model.py` & `tcex-3.0.8/tcex/api/tc/v3/notes/note_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/object_abc.py` & `tcex-3.0.8/tcex/api/tc/v3/object_abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,16 @@
     def create(self, params: Optional[dict] = None) -> 'Response':
         """Create or Update the Case Management object.
 
         This is determined based on if the id is already present in the object.
         """
         method = 'POST'
         body = self.model.gen_body_json(method=method)
+
+        params = self.gen_params(params or {})
         self._request(
             method,
             self.url(method),
             body,
             headers={'content-type': 'application/json'},
             params=params,
         )
@@ -341,14 +343,15 @@
 
         # get the unique id value for id, xid, summary, etc ...
         unique_id = self._calculate_unique_id().get('value')
 
         # validate an id is available
         self._validate_id(unique_id, self.url(method))
 
+        params = self.gen_params(params or {})
         self._request(
             method,
             self.url(method, unique_id=unique_id),
             body,
             headers={'content-type': 'application/json'},
             params=params,
         )
```

### Comparing `tcex-3.0.7/tcex/api/tc/v3/object_collection_abc.py` & `tcex-3.0.8/tcex/api/tc/v3/object_collection_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/assignee_model.py` & `tcex-3.0.8/tcex/api/tc/v3/security/assignee_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/assignee_user_group_model.py` & `tcex-3.0.8/tcex/api/tc/v3/security/assignee_user_group_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/assignee_user_model.py` & `tcex-3.0.8/tcex/api/tc/v3/security/assignee_user_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/owner_roles/owner_role.py` & `tcex-3.0.8/tcex/api/tc/v3/security/owner_roles/owner_role.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/owner_roles/owner_role_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/security/owner_roles/owner_role_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/owner_roles/owner_role_model.py` & `tcex-3.0.8/tcex/api/tc/v3/security/owner_roles/owner_role_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/owners/owner.py` & `tcex-3.0.8/tcex/api/tc/v3/security/owners/owner.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/owners/owner_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/security/owners/owner_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/owners/owner_model.py` & `tcex-3.0.8/tcex/api/tc/v3/security/owners/owner_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/security.py` & `tcex-3.0.8/tcex/api/tc/v3/security/security.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/system_roles/system_role.py` & `tcex-3.0.8/tcex/api/tc/v3/security/system_roles/system_role.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/system_roles/system_role_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/security/system_roles/system_role_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/system_roles/system_role_model.py` & `tcex-3.0.8/tcex/api/tc/v3/security/system_roles/system_role_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/task_assignee_model.py` & `tcex-3.0.8/tcex/api/tc/v3/security/task_assignee_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/user_groups/user_group.py` & `tcex-3.0.8/tcex/api/tc/v3/security/user_groups/user_group.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/user_groups/user_group_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/security/user_groups/user_group_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/user_groups/user_group_model.py` & `tcex-3.0.8/tcex/api/tc/v3/security/user_groups/user_group_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/users/user.py` & `tcex-3.0.8/tcex/api/tc/v3/security/users/user.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/users/user_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/security/users/user_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,26 +106,14 @@
 
         Args:
             operator: The operator enum for the filter.
             locked: A flag indicating whether or not the user's account has been locked.
         """
         self._tql.add_filter('locked', operator, locked, TqlType.BOOLEAN)
 
-    def logout_interval_minutes(self, operator: Enum, logout_interval_minutes: int):
-        """Filter Logout Interval based on **logoutIntervalMinutes** keyword.
-
-        Args:
-            operator: The operator enum for the filter.
-            logout_interval_minutes: The configured period of time to wait for idle activity before
-                being logged out.
-        """
-        self._tql.add_filter(
-            'logoutIntervalMinutes', operator, logout_interval_minutes, TqlType.INTEGER
-        )
-
     def password_reset_required(self, operator: Enum, password_reset_required: bool):
         """Filter Password Reset Required based on **passwordResetRequired** keyword.
 
         Args:
             operator: The operator enum for the filter.
             password_reset_required: A flag indicating whether or not the user's password needs to
                 be reset upoin next login.
@@ -178,23 +166,14 @@
 
         Args:
             operator: The operator enum for the filter.
             tql_timeout: The custom TQL timeout value (if defined).
         """
         self._tql.add_filter('tqlTimeout', operator, tql_timeout, TqlType.INTEGER)
 
-    def ui_theme(self, operator: Enum, ui_theme: str):
-        """Filter UI Theme based on **uiTheme** keyword.
-
-        Args:
-            operator: The operator enum for the filter.
-            ui_theme: The user's configured theme (e.g. light/dark).
-        """
-        self._tql.add_filter('uiTheme', operator, ui_theme, TqlType.STRING)
-
     def user_name(self, operator: Enum, user_name: str):
         """Filter User Name based on **userName** keyword.
 
         Args:
             operator: The operator enum for the filter.
             user_name: The user name of the user.
         """
```

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security/users/user_model.py` & `tcex-3.0.8/tcex/api/tc/v3/security/users/user_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security_labels/security_label.py` & `tcex-3.0.8/tcex/api/tc/v3/security_labels/security_label.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security_labels/security_label_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/security_labels/security_label_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/security_labels/security_label_model.py` & `tcex-3.0.8/tcex/api/tc/v3/security_labels/security_label_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/tags/tag.py` & `tcex-3.0.8/tcex/api/tc/v3/tags/tag.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/tags/tag_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/tags/tag_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/tags/tag_model.py` & `tcex-3.0.8/tcex/api/tc/v3/tags/tag_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/tasks/task.py` & `tcex-3.0.8/tcex/api/tc/v3/tasks/task.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/tasks/task_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/tasks/task_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/tasks/task_model.py` & `tcex-3.0.8/tcex/api/tc/v3/tasks/task_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/threat_intelligence/threat_intelligence.py` & `tcex-3.0.8/tcex/api/tc/v3/threat_intelligence/threat_intelligence.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/tql/tql.py` & `tcex-3.0.8/tcex/api/tc/v3/tql/tql.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/tql/tql_operator.py` & `tcex-3.0.8/tcex/api/tc/v3/tql/tql_operator.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/v3.py` & `tcex-3.0.8/tcex/api/tc/v3/v3.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/v3_model_abc.py` & `tcex-3.0.8/tcex/api/tc/v3/v3_model_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/v3_types.py` & `tcex-3.0.8/tcex/api/tc/v3/v3_types.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/victim_assets/victim_asset.py` & `tcex-3.0.8/tcex/api/tc/v3/victim_assets/victim_asset.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/victim_assets/victim_asset_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/victim_assets/victim_asset_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/victim_assets/victim_asset_model.py` & `tcex-3.0.8/tcex/api/tc/v3/victim_assets/victim_asset_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/victim_attributes/victim_attribute.py` & `tcex-3.0.8/tcex/api/tc/v3/victim_attributes/victim_attribute.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/victim_attributes/victim_attribute_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/victim_attributes/victim_attribute_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/victim_attributes/victim_attribute_model.py` & `tcex-3.0.8/tcex/api/tc/v3/victim_attributes/victim_attribute_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/victims/victim.py` & `tcex-3.0.8/tcex/api/tc/v3/victims/victim.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/victims/victim_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/victims/victim_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/victims/victim_model.py` & `tcex-3.0.8/tcex/api/tc/v3/victims/victim_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/workflow_events/workflow_event.py` & `tcex-3.0.8/tcex/api/tc/v3/workflow_events/workflow_event.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/workflow_events/workflow_event_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/workflow_events/workflow_event_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/workflow_events/workflow_event_model.py` & `tcex-3.0.8/tcex/api/tc/v3/workflow_events/workflow_event_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/workflow_templates/workflow_template.py` & `tcex-3.0.8/tcex/api/tc/v3/workflow_templates/workflow_template.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/workflow_templates/workflow_template_filter.py` & `tcex-3.0.8/tcex/api/tc/v3/workflow_templates/workflow_template_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/api/tc/v3/workflow_templates/workflow_template_model.py` & `tcex-3.0.8/tcex/api/tc/v3/workflow_templates/workflow_template_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/app_config/app_spec_yml.py` & `tcex-3.0.8/tcex/app_config/app_spec_yml.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/app_config/install_json.py` & `tcex-3.0.8/tcex/app_config/install_json.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/app_config/install_json_update.py` & `tcex-3.0.8/tcex/app_config/install_json_update.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/app_config/install_json_validate.py` & `tcex-3.0.8/tcex/app_config/install_json_validate.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/app_config/job_json.py` & `tcex-3.0.8/tcex/app_config/job_json.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/app_config/layout_json.py` & `tcex-3.0.8/tcex/app_config/layout_json.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/app_config/models/app_spec_yml_model.py` & `tcex-3.0.8/tcex/app_config/models/app_spec_yml_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/app_config/models/install_json_model.py` & `tcex-3.0.8/tcex/app_config/models/install_json_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/app_config/models/job_json_model.py` & `tcex-3.0.8/tcex/app_config/models/job_json_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/app_config/models/layout_json_model.py` & `tcex-3.0.8/tcex/app_config/models/layout_json_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/app_config/models/tcex_json_model.py` & `tcex-3.0.8/tcex/app_config/models/tcex_json_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/app_config/models/template_config_model.py` & `tcex-3.0.8/tcex/app_config/models/template_config_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/app_config/permutation.py` & `tcex-3.0.8/tcex/app_config/permutation.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/app_config/tcex_json.py` & `tcex-3.0.8/tcex/app_config/tcex_json.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/app_config/tcex_json_update.py` & `tcex-3.0.8/tcex/app_config/tcex_json_update.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/app_feature/advanced_request.py` & `tcex-3.0.8/tcex/app_feature/advanced_request.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/backports/__init__.py` & `tcex-3.0.8/tcex/backports/__init__.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/bin/bin_abc.py` & `tcex-3.0.8/tcex/bin/bin_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/bin/dep.py` & `tcex-3.0.8/tcex/bin/dep.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import platform
 import shutil
 import subprocess  # nosec
 import sys
 from distutils.version import StrictVersion  # pylint: disable=no-name-in-module
 from pathlib import Path
 from typing import List, Optional
-from urllib.parse import quote
+from urllib.parse import quote, urlsplit
 
 # third-party
 import typer
 
 # first-party
 from tcex.app_config.models.tcex_json_model import LibVersionModel
 from tcex.backports import cached_property
@@ -41,14 +41,21 @@
         self.no_cache_dir = no_cache_dir
         self.pre = pre
         self.proxy_host = proxy_host
         self.proxy_port = proxy_port
         self.proxy_user = proxy_user
         self.proxy_pass = proxy_pass
 
+        if not self.proxy_host and os.environ.get('https_proxy'):
+            parsed_proxy_url = urlsplit(os.environ.get('https_proxy'))
+            self.proxy_host = parsed_proxy_url.hostname
+            self.proxy_port = parsed_proxy_url.port
+            self.proxy_user = parsed_proxy_url.username
+            self.proxy_pass = parsed_proxy_url.password
+
         # properties
         self.env = self._env
         self.latest_version = None
         self.lib_directory = (
             f'lib_{sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro}'
         )
         self.proxy_enabled = False
@@ -196,14 +203,16 @@
     @property
     def has_requirements_lock(self):
         """Return True if requirements.lock exists."""
         return Path('requirements.lock').exists()
 
     def install_deps(self):
         """Install Required Libraries using pip."""
+        error = False  # track if any errors have occurred and if so, don't create lock file.
+
         # check for requirements.txt
         if not self.requirements_fqfn.is_file():
             self.handle_error(
                 f'A {str(self.requirements_fqfn)} file is required to install modules.'
             )
 
         # update requirements_dev.txt file
@@ -214,15 +223,15 @@
             # remove lib directory from previous runs
             self._remove_previous(lib_version.lib_dir)
 
             if (
                 not lib_version.python_executable.is_file()
                 and not lib_version.python_executable.is_symlink()
             ):
-
+                error = True
                 # display error
                 typer.secho(
                     f'The Python executable ({lib_version.python_executable}) could not be found. '
                     'Skipping building lib directory for this Python version.',
                     fg=typer.colors.YELLOW,
                 )
                 continue
@@ -275,15 +284,21 @@
             # remove temp requirements.txt file
             self.requirements_fqfn_branch.unlink()
 
         # create lib_latest directory
         self._create_lib_latest()
 
         if self.has_requirements_lock is False:
-            self.create_requirements_lock()
+            if error:
+                typer.secho(
+                    'Not creating requirements.lock file due to errors.',
+                    fg=typer.colors.YELLOW,
+                )
+            else:
+                self.create_requirements_lock()
 
     @property
     def lib_versions(self) -> List[LibVersionModel]:
         """Return the lib_version data required to build lib directories."""
         if self.tj.model.lib_versions:
             self.print_setting('Python Version', 'using version(s) defined in tcex.json')
```

### Comparing `tcex-3.0.7/tcex/bin/deploy.py` & `tcex-3.0.8/tcex/bin/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,10 +134,10 @@
     @property
     def session(self):
         """Create a TcEx Session."""
         _proxies = proxies(
             proxy_host=self.proxy_host,
             proxy_port=self.proxy_port,
             proxy_user=self.proxy_user,
-            proxy_pass=self.proxy_pass,
+            proxy_pass=Sensitive(self.proxy_pass),
         )
         return TcSession(auth=self.auth, base_url=self.base_url, proxies=_proxies)
```

### Comparing `tcex-3.0.7/tcex/bin/package.py` & `tcex-3.0.8/tcex/bin/package.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/bin/spec_tool.py` & `tcex-3.0.8/tcex/bin/spec_tool.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/bin/spec_tool_app_input.py` & `tcex-3.0.8/tcex/bin/spec_tool_app_input.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/bin/spec_tool_app_input_static.py` & `tcex-3.0.8/tcex/bin/spec_tool_app_input_static.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/bin/spec_tool_app_spec_yml.py` & `tcex-3.0.8/tcex/bin/spec_tool_app_spec_yml.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/bin/spec_tool_install_json.py` & `tcex-3.0.8/tcex/bin/spec_tool_install_json.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/bin/spec_tool_job_json.py` & `tcex-3.0.8/tcex/bin/spec_tool_job_json.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/bin/spec_tool_layout_json.py` & `tcex-3.0.8/tcex/bin/spec_tool_layout_json.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/bin/spec_tool_readme_md.py` & `tcex-3.0.8/tcex/bin/spec_tool_readme_md.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/bin/spec_tool_tcex_json.py` & `tcex-3.0.8/tcex/bin/spec_tool_tcex_json.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/bin/template.py` & `tcex-3.0.8/tcex/bin/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,32 @@
 from requests.auth import HTTPBasicAuth
 from tinydb import Query, TinyDB
 
 # first-party
 from tcex.app_config.models import TemplateConfigModel
 from tcex.backports import cached_property
 from tcex.bin.bin_abc import BinABC
+from tcex.input.field_types import Sensitive
+from tcex.pleb.proxies import proxies
 
 if TYPE_CHECKING:  # pragma: no cover
     # third-party
     from requests import Response
 
 
 class Template(BinABC):
     """Install dependencies for App."""
 
-    def __init__(self):
+    def __init__(
+        self,
+        proxy_host,
+        proxy_port,
+        proxy_user,
+        proxy_pass,
+    ):
         """Initialize class properties."""
         super().__init__()
 
         # properties
         self.base_url = os.getenv(
             'TCEX_TEMPLATE_URL',
             'https://api.github.com/repos/ThreatConnect-Inc/tcex-app-templates',
@@ -39,14 +47,18 @@
         self.base_raw_url = 'https://raw.githubusercontent.com/ThreatConnect-Inc/tcex-app-templates'
         self.errors = False
         self.password = os.getenv('GITHUB_PAT')
         self.template_configs = {}
         self.template_data = {}
         self.template_manifest_fqfn = Path('.template_manifest.json')
         self.username = os.getenv('GITHUB_USER')
+        self.proxy_host = proxy_host
+        self.proxy_port = proxy_port
+        self.proxy_user = proxy_user
+        self.proxy_pass = proxy_pass
 
     @cached_property
     def cache_valid(self) -> bool:
         """Return the current commit sha for the tcex-app-templates project."""
         if self.project_sha is None:
             return False
 
@@ -81,14 +93,15 @@
         if not r.ok:
             self.log.error(
                 f'action=get-contents, url={r.request.url}, '
                 f'status_code={r.status_code}, headers={r.headers}, '
                 f'response={r.text or r.reason}'
             )
             self.errors = True
+            yield from []
         else:
             for content in r.json():
                 # exclusion - this file is only needed for building App Builder templates
                 if content.get('name') == '.appbuilderconfig' and app_builder is False:
                     continue
 
                 # exclusions - files that should not be part of the App
@@ -169,14 +182,18 @@
         )
         if not r.ok:
             self.log.error(
                 f'action=download-template-file, url={r.request.url}, '
                 f'status_code={r.status_code}, headers={r.headers}, '
                 f'response={r.text or r.reason}'
             )
+            raise RuntimeError(
+                f'action=get-template-config, url={r.request.url}, status_code='
+                f'{r.status_code}, reason={r.reason}'
+            )
 
         # get the relative path to the file and create the parent directory if it does not exist
         destination = item.get('relative_path')
         if destination.parent.exists() is False:
             destination.parent.mkdir(parents=True, exist_ok=True)
         destination.open(mode='wb').write(r.content)
         self.log.info(f'action=download-template-file, file={destination}')
@@ -222,15 +239,18 @@
         if not r.ok:
             self.log.error(
                 f'action=get-template-config, url={r.request.url}, '
                 f'status_code={r.status_code}, headers={r.headers}, '
                 f'response={r.text or r.reason}'
             )
             self.errors = True
-            return None
+            raise RuntimeError(
+                f'action=get-template-config, url={r.request.url}, status_code='
+                f'{r.status_code}, reason={r.reason}'
+            )
 
         try:
             template_config_data = yaml.safe_load(r.text)
             template_config_data.update({'name': template, 'type': type_})
             config = TemplateConfigModel(**template_config_data)
 
             # upsert db
@@ -364,29 +384,38 @@
         if not r.ok:
             self.log.error(
                 f'action=get-project-sha, url={r.request.url}, '
                 f'status_code={r.status_code}, headers={r.headers}, '
                 f'response={r.text or r.reason}'
             )
             self.errors = True
-            return None
+            raise RuntimeError(
+                f'action=get-template-config, url={r.request.url}, status_code='
+                f'{r.status_code}, reason={r.reason}'
+            )
 
         try:
             commits_data = r.json()
         except Exception:
             return None
 
         # get current sha
         return commits_data[0].get('sha')
 
     @cached_property
     def session(self) -> 'Session':
         """Return session object"""
         session = Session()
         session.headers.update({'Cache-Control': 'no-cache'})
+        session.proxies = proxies(
+            proxy_host=self.proxy_host,
+            proxy_port=self.proxy_port,
+            proxy_user=self.proxy_user,
+            proxy_pass=Sensitive(self.proxy_pass),
+        )
 
         # add auth if set (typically not require since default site is public)
         if self.username is not None and self.password is not None:
             session.auth = HTTPBasicAuth(self.username, self.password)
 
         return session
```

### Comparing `tcex-3.0.7/tcex/bin/validate.py` & `tcex-3.0.8/tcex/bin/validate.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/decorators/benchmark.py` & `tcex-3.0.8/tcex/decorators/benchmark.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/decorators/debug.py` & `tcex-3.0.8/tcex/decorators/debug.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/decorators/fail_on_output.py` & `tcex-3.0.8/tcex/decorators/fail_on_output.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/decorators/on_exception.py` & `tcex-3.0.8/tcex/decorators/on_exception.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/decorators/on_success.py` & `tcex-3.0.8/tcex/decorators/on_success.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/decorators/output.py` & `tcex-3.0.8/tcex/decorators/output.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/exit/error_codes.py` & `tcex-3.0.8/tcex/exit/error_codes.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/exit/exit.py` & `tcex-3.0.8/tcex/exit/exit.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/field_types/__init__.py` & `tcex-3.0.8/tcex/input/field_types/__init__.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/field_types/binary.py` & `tcex-3.0.8/tcex/input/field_types/binary.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/field_types/case_management_entity.py` & `tcex-3.0.8/tcex/input/field_types/case_management_entity.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/field_types/choice.py` & `tcex-3.0.8/tcex/input/field_types/choice.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/field_types/datetime.py` & `tcex-3.0.8/tcex/input/field_types/datetime.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/field_types/edit_choice.py` & `tcex-3.0.8/tcex/input/field_types/edit_choice.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/field_types/exception.py` & `tcex-3.0.8/tcex/input/field_types/exception.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/field_types/group_entity.py` & `tcex-3.0.8/tcex/input/field_types/group_entity.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/field_types/indicator_entity.py` & `tcex-3.0.8/tcex/input/field_types/indicator_entity.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/field_types/integer.py` & `tcex-3.0.8/tcex/input/field_types/integer.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/field_types/ip_address.py` & `tcex-3.0.8/tcex/input/field_types/ip_address.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/field_types/key_value.py` & `tcex-3.0.8/tcex/input/field_types/key_value.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/field_types/sensitive.py` & `tcex-3.0.8/tcex/input/field_types/sensitive.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/field_types/string.py` & `tcex-3.0.8/tcex/input/field_types/string.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/field_types/tc_entity.py` & `tcex-3.0.8/tcex/input/field_types/tc_entity.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/field_types/validators.py` & `tcex-3.0.8/tcex/input/field_types/validators.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/input.py` & `tcex-3.0.8/tcex/input/input.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/models/__init__.py` & `tcex-3.0.8/tcex/input/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/models/advanced_request_model.py` & `tcex-3.0.8/tcex/input/models/advanced_request_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/models/aot_execution_enabled_model.py` & `tcex-3.0.8/tcex/input/models/aot_execution_enabled_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/models/api_model.py` & `tcex-3.0.8/tcex/input/models/api_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/models/batch_model.py` & `tcex-3.0.8/tcex/input/models/batch_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/models/cal_settings_model.py` & `tcex-3.0.8/tcex/input/models/cal_settings_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/models/create_config_model.py` & `tcex-3.0.8/tcex/input/models/create_config_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/models/logging_model.py` & `tcex-3.0.8/tcex/input/models/logging_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/models/model_map.py` & `tcex-3.0.8/tcex/input/models/model_map.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/models/path_model.py` & `tcex-3.0.8/tcex/input/models/path_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/models/playbook_common_model.py` & `tcex-3.0.8/tcex/input/models/playbook_common_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/models/playbook_model.py` & `tcex-3.0.8/tcex/input/models/playbook_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/models/proxy_model.py` & `tcex-3.0.8/tcex/input/models/proxy_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/models/service_model.py` & `tcex-3.0.8/tcex/input/models/service_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/input/models/smtp_settings_model.py` & `tcex-3.0.8/tcex/input/models/smtp_settings_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/key_value_store/key_value_abc.py` & `tcex-3.0.8/tcex/key_value_store/key_value_abc.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/key_value_store/key_value_api.py` & `tcex-3.0.8/tcex/key_value_store/key_value_api.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/key_value_store/key_value_mock.py` & `tcex-3.0.8/tcex/key_value_store/key_value_mock.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/key_value_store/key_value_redis.py` & `tcex-3.0.8/tcex/key_value_store/key_value_redis.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/key_value_store/redis_client.py` & `tcex-3.0.8/tcex/key_value_store/redis_client.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/logger/api_handler.py` & `tcex-3.0.8/tcex/logger/api_handler.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/logger/cache_handler.py` & `tcex-3.0.8/tcex/logger/cache_handler.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/logger/logger.py` & `tcex-3.0.8/tcex/logger/logger.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/logger/pattern_file_handler.py` & `tcex-3.0.8/tcex/logger/pattern_file_handler.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/logger/rotating_file_handler_custom.py` & `tcex-3.0.8/tcex/logger/rotating_file_handler_custom.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/logger/sensitive_filter.py` & `tcex-3.0.8/tcex/logger/sensitive_filter.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/logger/thread_file_handler.py` & `tcex-3.0.8/tcex/logger/thread_file_handler.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/logger/trace_logger.py` & `tcex-3.0.8/tcex/logger/trace_logger.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/playbook/playbook.py` & `tcex-3.0.8/tcex/playbook/playbook.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/playbook/playbook_create.py` & `tcex-3.0.8/tcex/playbook/playbook_create.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/playbook/playbook_delete.py` & `tcex-3.0.8/tcex/playbook/playbook_delete.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/playbook/playbook_output.py` & `tcex-3.0.8/tcex/playbook/playbook_output.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/playbook/playbook_read.py` & `tcex-3.0.8/tcex/playbook/playbook_read.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/pleb/env_path.py` & `tcex-3.0.8/tcex/pleb/env_path.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/pleb/event.py` & `tcex-3.0.8/tcex/pleb/event.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/pleb/none_model.py` & `tcex-3.0.8/tcex/pleb/none_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/pleb/proxies.py` & `tcex-3.0.8/tcex/pleb/proxies.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/pleb/registry.py` & `tcex-3.0.8/tcex/pleb/registry.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/pleb/scoped_property.py` & `tcex-3.0.8/tcex/pleb/scoped_property.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/pleb/threading.py` & `tcex-3.0.8/tcex/pleb/threading.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/services/api_service.py` & `tcex-3.0.8/tcex/services/api_service.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/services/common_service.py` & `tcex-3.0.8/tcex/services/common_service.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/services/common_service_trigger.py` & `tcex-3.0.8/tcex/services/common_service_trigger.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/services/mqtt_message_broker.py` & `tcex-3.0.8/tcex/services/mqtt_message_broker.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/services/webhook_trigger_service.py` & `tcex-3.0.8/tcex/services/webhook_trigger_service.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/sessions/auth/hmac_auth.py` & `tcex-3.0.8/tcex/sessions/auth/hmac_auth.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/sessions/auth/tc_auth.py` & `tcex-3.0.8/tcex/sessions/auth/tc_auth.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/sessions/auth/token_auth.py` & `tcex-3.0.8/tcex/sessions/auth/token_auth.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/sessions/external_session.py` & `tcex-3.0.8/tcex/sessions/external_session.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/sessions/rate_limit_handler.py` & `tcex-3.0.8/tcex/sessions/rate_limit_handler.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/sessions/tc_session.py` & `tcex-3.0.8/tcex/sessions/tc_session.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/tcex.py` & `tcex-3.0.8/tcex/tcex.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/tokens/tokens.py` & `tcex-3.0.8/tcex/tokens/tokens.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/utils/aes_operations.py` & `tcex-3.0.8/tcex/utils/aes_operations.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/utils/datetime_operations.py` & `tcex-3.0.8/tcex/utils/datetime_operations.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/utils/file_operations.py` & `tcex-3.0.8/tcex/utils/file_operations.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/utils/models/playbook_variable_model.py` & `tcex-3.0.8/tcex/utils/models/playbook_variable_model.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/utils/requests_to_curl.py` & `tcex-3.0.8/tcex/utils/requests_to_curl.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/utils/string_operations.py` & `tcex-3.0.8/tcex/utils/string_operations.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/utils/utils.py` & `tcex-3.0.8/tcex/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex/utils/variables.py` & `tcex-3.0.8/tcex/utils/variables.py`

 * *Files identical despite different names*

### Comparing `tcex-3.0.7/tcex.egg-info/PKG-INFO` & `tcex-3.0.8/tcex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tcex
-Version: 3.0.7
+Version: 3.0.8
 Summary: ThreatConnect Exchange App Framework
 Home-page: https://github.com/ThreatConnect-Inc/tcex
-Download-URL: https://github.com/ThreatConnect-Inc/tcex/tarball/3.0.7
+Download-URL: https://github.com/ThreatConnect-Inc/tcex/tarball/3.0.8
 Author: ThreatConnect (support@threatconnect.com)
 Author-email: support@threatconnect.com
 License: Apache License, Version 2
 Project-URL: Documentation, https://github.com/ThreatConnect-Inc/tcex
 Project-URL: Source, https://github.com/ThreatConnect-Inc/tcex
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `tcex-3.0.7/tcex.egg-info/SOURCES.txt` & `tcex-3.0.8/tcex.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/quickstats-0.6.7.7.tar.gz` & `tmp/quickstats-0.6.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstats-0.6.7.7.tar", last modified: Fri Feb 24 23:10:51 2023, max compression
+gzip compressed data, was "quickstats-0.6.7.8.tar", last modified: Mon Apr 10 20:19:27 2023, max compression
```

## Comparing `quickstats-0.6.7.7.tar` & `quickstats-0.6.7.8.tar`

### file list

```diff
@@ -1,228 +1,237 @@
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:51.000000 quickstats-0.6.7.7/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-02-24 23:10:51.000000 quickstats-0.6.7.7/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2023-01-04 09:02:54.000000 quickstats-0.6.7.7/README.md
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:38.000000 quickstats-0.6.7.7/bin/
--rwxr-xr-x   0 chlcheng (124202) zp        (1307)     1603 2023-01-04 09:02:54.000000 quickstats-0.6.7.7/bin/quickstats
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:38.000000 quickstats-0.6.7.7/quickstats/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      626 2023-01-04 09:02:54.000000 quickstats-0.6.7.7/quickstats/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2023-02-24 23:09:44.000000 quickstats-0.6.7.7/quickstats/_version.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:39.000000 quickstats-0.6.7.7/quickstats/analysis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2023-02-08 03:42:01.000000 quickstats-0.6.7.7/quickstats/analysis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-02-08 08:27:54.000000 quickstats-0.6.7.7/quickstats/analysis/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4191 2023-02-08 05:24:19.000000 quickstats-0.6.7.7/quickstats/analysis/analysis_path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18586 2023-01-04 09:02:54.000000 quickstats-0.6.7.7/quickstats/analysis/config_format_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    41488 2023-02-18 18:09:50.000000 quickstats-0.6.7.7/quickstats/analysis/data_loading.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1303 2023-01-04 09:02:54.000000 quickstats-0.6.7.7/quickstats/analysis/data_preprocessing.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    86085 2023-02-21 19:10:36.000000 quickstats-0.6.7.7/quickstats/analysis/event_categorization.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8060 2023-01-04 09:02:54.000000 quickstats-0.6.7.7/quickstats/analysis/multi_class_boundary_tree.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9176 2023-02-08 11:43:40.000000 quickstats-0.6.7.7/quickstats/analysis/ntuple_conversion_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18667 2023-02-21 02:01:28.000000 quickstats-0.6.7.7/quickstats/analysis/ntuple_process_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8632 2023-02-08 05:31:49.000000 quickstats-0.6.7.7/quickstats/analysis/sample_poly_param_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:40.000000 quickstats-0.6.7.7/quickstats/clis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-05-17 11:53:22.000000 quickstats-0.6.7.7/quickstats/clis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    33609 2023-02-24 23:06:10.000000 quickstats-0.6.7.7/quickstats/clis/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2174 2023-02-14 22:30:46.000000 quickstats-0.6.7.7/quickstats/clis/inspect_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2023-02-14 22:27:47.000000 quickstats-0.6.7.7/quickstats/clis/inspect_ws.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16773 2023-02-14 22:32:02.000000 quickstats-0.6.7.7/quickstats/clis/likelihood_fit.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7818 2023-01-04 09:02:54.000000 quickstats-0.6.7.7/quickstats/clis/likelihood_scan.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8575 2023-01-04 09:02:54.000000 quickstats-0.6.7.7/quickstats/clis/limit_setting.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1327 2023-02-14 22:29:19.000000 quickstats-0.6.7.7/quickstats/clis/processor_cli.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13393 2023-02-14 22:34:00.000000 quickstats-0.6.7.7/quickstats/clis/workspace_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:41.000000 quickstats-0.6.7.7/quickstats/components/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      784 2023-01-04 09:02:54.000000 quickstats-0.6.7.7/quickstats/components/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3084 2022-04-07 12:50:48.000000 quickstats-0.6.7.7/quickstats/components/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13927 2023-01-04 09:02:54.000000 quickstats-0.6.7.7/quickstats/components/analysis_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8521 2023-01-04 09:02:54.000000 quickstats-0.6.7.7/quickstats/components/asimov_generator.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    30317 2023-01-04 09:02:54.000000 quickstats-0.6.7.7/quickstats/components/asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2464 2023-01-04 09:02:54.000000 quickstats-0.6.7.7/quickstats/components/basics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    31828 2023-01-04 09:02:55.000000 quickstats-0.6.7.7/quickstats/components/extended_minimizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    91179 2023-02-24 22:58:34.000000 quickstats-0.6.7.7/quickstats/components/extended_model.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5575 2022-08-09 03:12:09.000000 quickstats-0.6.7.7/quickstats/components/extended_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15678 2023-01-04 09:02:55.000000 quickstats-0.6.7.7/quickstats/components/likelihood.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:42.000000 quickstats-0.6.7.7/quickstats/components/modelling/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.6.7.7/quickstats/components/modelling/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2520 2022-09-18 05:43:28.000000 quickstats-0.6.7.7/quickstats/components/modelling/component_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18985 2023-02-15 11:50:48.000000 quickstats-0.6.7.7/quickstats/components/modelling/data_modelling.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      767 2022-09-18 12:07:18.000000 quickstats-0.6.7.7/quickstats/components/modelling/model_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4562 2022-09-18 16:32:35.000000 quickstats-0.6.7.7/quickstats/components/modelling/parameter_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5391 2022-09-18 19:53:53.000000 quickstats-0.6.7.7/quickstats/components/modelling/pdf_fit_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3541 2022-09-18 12:41:58.000000 quickstats-0.6.7.7/quickstats/components/modelling/tree_data_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10839 2022-04-07 03:18:15.000000 quickstats-0.6.7.7/quickstats/components/nuisance_parameter_harmonizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16929 2023-02-14 22:14:02.000000 quickstats-0.6.7.7/quickstats/components/nuisance_parameter_pull.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:42.000000 quickstats-0.6.7.7/quickstats/components/processors/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      205 2022-07-19 21:07:01.000000 quickstats-0.6.7.7/quickstats/components/processors/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:42.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1985 2022-07-21 18:30:19.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2022-07-21 18:27:25.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/auxiliary.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1010 2022-09-09 03:52:14.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1082 2022-07-19 21:51:30.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_as_numpy.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2580 2022-08-29 07:36:48.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_base_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      710 2022-07-20 13:58:23.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_declare.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      821 2022-07-19 21:53:12.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      937 2023-01-04 09:02:55.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_export.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1164 2022-07-21 15:20:21.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_filter.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1076 2022-08-29 06:56:49.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_global_variables.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_helper_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_hybrid_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      697 2022-07-21 18:29:41.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_if_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      704 2022-07-21 18:48:13.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_if_not_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-19 21:50:41.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_load_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:20.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_max.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      142 2022-07-19 20:41:10.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_mean.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:51.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_min.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_nested_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_rdf_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2022-07-19 20:28:28.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_redefine.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1657 2023-01-04 09:02:55.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_report.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1155 2022-07-19 21:53:35.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_safe_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      454 2022-07-19 20:28:24.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_safe_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2204 2022-11-10 10:03:00.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_save.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      654 2022-07-19 21:53:28.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_save_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1194 2022-07-19 21:50:00.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_stat.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:39:49.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_sum.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      523 2022-07-19 21:54:23.000000 quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_treename.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7708 2022-08-29 03:05:08.000000 quickstats-0.6.7.7/quickstats/components/processors/builtin_methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6361 2022-07-21 19:15:41.000000 quickstats-0.6.7.7/quickstats/components/processors/roo_config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6267 2023-01-17 14:15:49.000000 quickstats-0.6.7.7/quickstats/components/processors/roo_processor.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5397 2021-09-16 21:06:55.000000 quickstats-0.6.7.7/quickstats/components/pvalue_toys.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3517 2022-07-20 11:52:20.000000 quickstats-0.6.7.7/quickstats/components/roo_inspector.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3107 2022-09-17 18:29:41.000000 quickstats-0.6.7.7/quickstats/components/root_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21144 2022-07-28 22:30:24.000000 quickstats-0.6.7.7/quickstats/components/toy_limit_calculator.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:44.000000 quickstats-0.6.7.7/quickstats/components/workspaces/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      551 2023-01-13 12:37:11.000000 quickstats-0.6.7.7/quickstats/components/workspaces/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9929 2023-02-14 22:17:05.000000 quickstats-0.6.7.7/quickstats/components/workspaces/asimov_handler.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1734 2023-01-08 18:44:57.000000 quickstats-0.6.7.7/quickstats/components/workspaces/core_argument_sets.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2023-01-09 17:03:21.000000 quickstats-0.6.7.7/quickstats/components/workspaces/sample.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1956 2023-01-08 17:22:57.000000 quickstats-0.6.7.7/quickstats/components/workspaces/settings.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8291 2023-01-09 17:11:38.000000 quickstats-0.6.7.7/quickstats/components/workspaces/systematic.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2023-01-08 18:43:45.000000 quickstats-0.6.7.7/quickstats/components/workspaces/systematics_domain.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    53246 2023-01-09 16:47:15.000000 quickstats-0.6.7.7/quickstats/components/workspaces/ws_comparer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1756 2022-04-20 13:20:42.000000 quickstats-0.6.7.7/quickstats/components/workspaces/ws_modifier_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10895 2023-02-14 22:19:38.000000 quickstats-0.6.7.7/quickstats/components/workspaces/xml_ws_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    85838 2023-01-08 18:42:21.000000 quickstats-0.6.7.7/quickstats/components/workspaces/xml_ws_builder_v1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    77583 2023-02-08 07:24:05.000000 quickstats-0.6.7.7/quickstats/components/workspaces/xml_ws_builder_v2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    45969 2023-01-04 17:04:30.000000 quickstats-0.6.7.7/quickstats/components/workspaces/xml_ws_combiner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    49107 2023-02-08 09:09:43.000000 quickstats-0.6.7.7/quickstats/components/workspaces/xml_ws_modifier.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:44.000000 quickstats-0.6.7.7/quickstats/concurrent/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      228 2022-03-27 20:47:33.000000 quickstats-0.6.7.7/quickstats/concurrent/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2666 2022-09-21 07:46:09.000000 quickstats-0.6.7.7/quickstats/concurrent/abstract_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.6.7.7/quickstats/concurrent/logging.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5890 2023-01-04 09:02:55.000000 quickstats-0.6.7.7/quickstats/concurrent/parameterised_asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10317 2023-01-04 09:02:55.000000 quickstats-0.6.7.7/quickstats/concurrent/parameterised_likelihood.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3983 2022-09-20 17:52:34.000000 quickstats-0.6.7.7/quickstats/concurrent/parameterised_runner.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:45.000000 quickstats-0.6.7.7/quickstats/core/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2023-01-04 09:02:55.000000 quickstats-0.6.7.7/quickstats/core/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      811 2023-01-04 09:02:55.000000 quickstats-0.6.7.7/quickstats/core/abstract_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20616 2023-01-04 09:02:55.000000 quickstats-0.6.7.7/quickstats/core/configs.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2198 2023-01-04 09:02:55.000000 quickstats-0.6.7.7/quickstats/core/configurable_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      541 2023-01-04 09:02:55.000000 quickstats-0.6.7.7/quickstats/core/dataclass_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      977 2022-05-11 20:30:59.000000 quickstats-0.6.7.7/quickstats/core/decorators.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2150 2023-01-08 11:34:04.000000 quickstats-0.6.7.7/quickstats/core/enums.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6651 2023-02-14 22:36:19.000000 quickstats-0.6.7.7/quickstats/core/methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9057 2023-02-08 05:24:13.000000 quickstats-0.6.7.7/quickstats/core/path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2952 2022-07-21 15:05:33.000000 quickstats-0.6.7.7/quickstats/core/virtual_trees.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:45.000000 quickstats-0.6.7.7/quickstats/interface/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       66 2022-01-31 04:51:23.000000 quickstats-0.6.7.7/quickstats/interface/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:45.000000 quickstats-0.6.7.7/quickstats/interface/cppyy/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-31 03:26:35.000000 quickstats-0.6.7.7/quickstats/interface/cppyy/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2022-01-31 03:37:54.000000 quickstats-0.6.7.7/quickstats/interface/cppyy/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1032 2023-01-04 09:02:55.000000 quickstats-0.6.7.7/quickstats/interface/cppyy/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4433 2023-01-04 09:02:55.000000 quickstats-0.6.7.7/quickstats/interface/cppyy/vectorize.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:45.000000 quickstats-0.6.7.7/quickstats/interface/root/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.6.7.7/quickstats/interface/root/RooAbsData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1564 2022-08-23 02:58:55.000000 quickstats-0.6.7.7/quickstats/interface/root/RooAbsPdf.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      420 2022-08-23 02:59:13.000000 quickstats-0.6.7.7/quickstats/interface/root/RooArgSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14083 2023-01-08 18:47:48.000000 quickstats-0.6.7.7/quickstats/interface/root/RooDataSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.6.7.7/quickstats/interface/root/RooMsgService.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4969 2022-09-20 10:41:26.000000 quickstats-0.6.7.7/quickstats/interface/root/RooRealVar.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.6.7.7/quickstats/interface/root/TArrayData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2023-01-04 09:02:55.000000 quickstats-0.6.7.7/quickstats/interface/root/TF1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1732 2022-08-23 02:54:36.000000 quickstats-0.6.7.7/quickstats/interface/root/TFile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11396 2023-01-08 16:37:29.000000 quickstats-0.6.7.7/quickstats/interface/root/TH1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5489 2022-08-23 03:10:20.000000 quickstats-0.6.7.7/quickstats/interface/root/TH2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      571 2022-08-23 03:14:20.000000 quickstats-0.6.7.7/quickstats/interface/root/TObject.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      794 2023-01-17 14:02:55.000000 quickstats-0.6.7.7/quickstats/interface/root/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.6.7.7/quickstats/interface/root/helper.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-03-24 19:40:20.000000 quickstats-0.6.7.7/quickstats/interface/root/inspection.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.6.7.7/quickstats/interface/root/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11879 2023-01-04 17:04:33.000000 quickstats-0.6.7.7/quickstats/interface/root/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5578 2023-02-24 22:56:11.000000 quickstats-0.6.7.7/quickstats/interface/root/roofit_extension.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:37.000000 quickstats-0.6.7.7/quickstats/macros/
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:46.000000 quickstats-0.6.7.7/quickstats/macros/AsymptoticCLsTool/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7083 2021-08-19 17:39:48.000000 quickstats-0.6.7.7/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1511 2021-06-11 19:36:10.000000 quickstats-0.6.7.7/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:46.000000 quickstats-0.6.7.7/quickstats/macros/FlexibleInterpVarMkII/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.6.7.7/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.6.7.7/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:46.000000 quickstats-0.6.7.7/quickstats/macros/QuickStatsCore/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1231 2022-05-07 02:55:05.000000 quickstats-0.6.7.7/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10322 2022-05-11 00:00:32.000000 quickstats-0.6.7.7/quickstats/macros/QuickStatsCore/RooFitExt.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3429 2022-05-10 23:59:25.000000 quickstats-0.6.7.7/quickstats/macros/QuickStatsCore/RooFitExt.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:46.000000 quickstats-0.6.7.7/quickstats/macros/ResponseFunction/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13946 2022-04-21 19:55:45.000000 quickstats-0.6.7.7/quickstats/macros/ResponseFunction/ResponseFunction.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2022-05-16 03:18:22.000000 quickstats-0.6.7.7/quickstats/macros/ResponseFunction/ResponseFunction.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:46.000000 quickstats-0.6.7.7/quickstats/macros/RooTwoSidedCBShape/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.6.7.7/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.6.7.7/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:46.000000 quickstats-0.6.7.7/quickstats/maths/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.6.7.7/quickstats/maths/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1130 2022-06-30 20:46:46.000000 quickstats-0.6.7.7/quickstats/maths/interpolation.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5339 2023-02-06 11:55:46.000000 quickstats-0.6.7.7/quickstats/maths/numerics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9280 2023-01-04 09:02:55.000000 quickstats-0.6.7.7/quickstats/maths/statistics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.6.7.7/quickstats/maths/symbolics.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:46.000000 quickstats-0.6.7.7/quickstats/parsers/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      113 2022-04-20 10:58:59.000000 quickstats-0.6.7.7/quickstats/parsers/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.6.7.7/quickstats/parsers/config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15568 2023-02-14 22:40:29.000000 quickstats-0.6.7.7/quickstats/parsers/param_parser.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:50.000000 quickstats-0.6.7.7/quickstats/plots/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1382 2023-02-05 13:21:50.000000 quickstats-0.6.7.7/quickstats/plots/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8779 2023-02-15 11:50:34.000000 quickstats-0.6.7.7/quickstats/plots/abstract_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.6.7.7/quickstats/plots/collective_data_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2575 2023-02-05 15:41:51.000000 quickstats-0.6.7.7/quickstats/plots/color_schemes.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4254 2023-02-05 13:08:19.000000 quickstats-0.6.7.7/quickstats/plots/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2353 2022-03-23 09:09:09.000000 quickstats-0.6.7.7/quickstats/plots/correlation_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5901 2022-08-18 15:05:02.000000 quickstats-0.6.7.7/quickstats/plots/general_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22775 2022-09-07 07:18:02.000000 quickstats-0.6.7.7/quickstats/plots/general_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3731 2022-09-09 08:30:51.000000 quickstats-0.6.7.7/quickstats/plots/histo_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6038 2022-02-16 22:08:47.000000 quickstats-0.6.7.7/quickstats/plots/hypotest_inverter_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5748 2022-05-03 14:02:46.000000 quickstats-0.6.7.7/quickstats/plots/likelihood_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9860 2023-01-04 09:02:56.000000 quickstats-0.6.7.7/quickstats/plots/likelihood_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      219 2021-04-19 13:56:55.000000 quickstats-0.6.7.7/quickstats/plots/likelihood_scan_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    26322 2022-04-19 14:42:15.000000 quickstats-0.6.7.7/quickstats/plots/np_ranking_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    24664 2023-01-11 11:29:47.000000 quickstats-0.6.7.7/quickstats/plots/pdf_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5059 2023-02-06 09:15:46.000000 quickstats-0.6.7.7/quickstats/plots/sample_purity_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9933 2022-08-18 13:35:04.000000 quickstats-0.6.7.7/quickstats/plots/score_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4123 2023-01-04 09:02:56.000000 quickstats-0.6.7.7/quickstats/plots/stat_plot_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16942 2023-02-05 12:26:23.000000 quickstats-0.6.7.7/quickstats/plots/template.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13688 2022-07-29 18:50:11.000000 quickstats-0.6.7.7/quickstats/plots/test_statistic_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11061 2023-01-04 09:02:56.000000 quickstats-0.6.7.7/quickstats/plots/upper_limit_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11855 2022-08-18 13:12:19.000000 quickstats-0.6.7.7/quickstats/plots/upper_limit_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13186 2022-08-18 13:35:04.000000 quickstats-0.6.7.7/quickstats/plots/upper_limit_3D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5069 2022-08-24 13:05:29.000000 quickstats-0.6.7.7/quickstats/plots/upper_limit_benchmark_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5617 2023-01-04 09:02:56.000000 quickstats-0.6.7.7/quickstats/plots/variable_distribution_plot.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:50.000000 quickstats-0.6.7.7/quickstats/resources/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      120 2023-01-04 09:02:56.000000 quickstats-0.6.7.7/quickstats/resources/default_workspace_extensions.json
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-04-08 03:20:04.000000 quickstats-0.6.7.7/quickstats/root_checker.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:50.000000 quickstats-0.6.7.7/quickstats/stylesheets/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2021-10-20 08:52:20.000000 quickstats-0.6.7.7/quickstats/stylesheets/quick_default.mplstyle
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:50.000000 quickstats-0.6.7.7/quickstats/utils/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.6.7.7/quickstats/utils/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9693 2023-02-14 22:23:45.000000 quickstats-0.6.7.7/quickstats/utils/common_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.6.7.7/quickstats/utils/condor_tasks.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16130 2023-02-08 10:47:46.000000 quickstats-0.6.7.7/quickstats/utils/data_conversion.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.6.7.7/quickstats/utils/hep_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3862 2023-01-06 12:43:25.000000 quickstats-0.6.7.7/quickstats/utils/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      335 2021-05-17 13:11:29.000000 quickstats-0.6.7.7/quickstats/utils/process_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    24388 2023-02-14 22:24:28.000000 quickstats-0.6.7.7/quickstats/utils/roofit_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9267 2021-11-23 21:10:48.000000 quickstats-0.6.7.7/quickstats/utils/roostats_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12361 2023-01-04 09:02:56.000000 quickstats-0.6.7.7/quickstats/utils/root_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1185 2023-02-14 21:45:46.000000 quickstats-0.6.7.7/quickstats/utils/string_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14436 2023-01-04 17:04:33.000000 quickstats-0.6.7.7/quickstats/utils/xml_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-02-24 23:10:38.000000 quickstats-0.6.7.7/quickstats.egg-info/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-02-24 23:10:35.000000 quickstats-0.6.7.7/quickstats.egg-info/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8450 2023-02-24 23:10:36.000000 quickstats-0.6.7.7/quickstats.egg-info/SOURCES.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2023-02-24 23:10:35.000000 quickstats-0.6.7.7/quickstats.egg-info/dependency_links.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2023-02-24 23:10:35.000000 quickstats-0.6.7.7/quickstats.egg-info/requires.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2023-02-24 23:10:35.000000 quickstats-0.6.7.7/quickstats.egg-info/top_level.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2023-02-24 23:10:51.000000 quickstats-0.6.7.7/setup.cfg
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1687 2023-01-04 09:02:56.000000 quickstats-0.6.7.7/setup.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/README.md
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/bin/
+-rwxr-xr-x   0 chlcheng (124202) zp        (1307)     1603 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/bin/quickstats
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      626 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/quickstats/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2023-04-10 18:07:42.000000 quickstats-0.6.7.8/quickstats/_version.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/analysis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2023-02-08 03:42:01.000000 quickstats-0.6.7.8/quickstats/analysis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-02-08 08:27:54.000000 quickstats-0.6.7.8/quickstats/analysis/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4191 2023-02-08 05:24:19.000000 quickstats-0.6.7.8/quickstats/analysis/analysis_path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22807 2023-03-14 14:12:10.000000 quickstats-0.6.7.8/quickstats/analysis/config_format_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    41488 2023-02-18 18:09:50.000000 quickstats-0.6.7.8/quickstats/analysis/data_loading.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1303 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/quickstats/analysis/data_preprocessing.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    86085 2023-03-23 15:12:41.000000 quickstats-0.6.7.8/quickstats/analysis/event_categorization.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8060 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/quickstats/analysis/multi_class_boundary_tree.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9328 2023-03-05 13:58:00.000000 quickstats-0.6.7.8/quickstats/analysis/ntuple_conversion_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    31710 2023-04-03 17:20:21.000000 quickstats-0.6.7.8/quickstats/analysis/ntuple_process_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8790 2023-04-06 13:30:03.000000 quickstats-0.6.7.8/quickstats/analysis/sample_poly_param_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/analysis/systematics/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2023-03-07 22:17:53.000000 quickstats-0.6.7.8/quickstats/analysis/systematics/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29659 2023-04-10 19:52:47.000000 quickstats-0.6.7.8/quickstats/analysis/systematics/base_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9774 2023-04-03 12:27:59.000000 quickstats-0.6.7.8/quickstats/analysis/systematics/gaussian_shape_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6796 2023-03-14 18:47:57.000000 quickstats-0.6.7.8/quickstats/analysis/systematics/normalization_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11786 2023-03-07 22:18:13.000000 quickstats-0.6.7.8/quickstats/analysis/systematics/systematics_evaluation_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/clis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-05-17 11:53:22.000000 quickstats-0.6.7.8/quickstats/clis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    33609 2023-03-20 15:35:32.000000 quickstats-0.6.7.8/quickstats/clis/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2174 2023-02-14 22:30:46.000000 quickstats-0.6.7.8/quickstats/clis/inspect_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2023-02-14 22:27:47.000000 quickstats-0.6.7.8/quickstats/clis/inspect_ws.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16773 2023-02-14 22:32:02.000000 quickstats-0.6.7.8/quickstats/clis/likelihood_fit.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7818 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/quickstats/clis/likelihood_scan.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8575 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/quickstats/clis/limit_setting.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1327 2023-02-14 22:29:19.000000 quickstats-0.6.7.8/quickstats/clis/processor_cli.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13393 2023-04-06 15:18:32.000000 quickstats-0.6.7.8/quickstats/clis/workspace_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/components/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      784 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/quickstats/components/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3084 2022-04-07 12:50:48.000000 quickstats-0.6.7.8/quickstats/components/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13927 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/quickstats/components/analysis_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8656 2023-04-05 18:11:38.000000 quickstats-0.6.7.8/quickstats/components/asimov_generator.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    30254 2023-04-07 15:54:53.000000 quickstats-0.6.7.8/quickstats/components/asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2464 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/quickstats/components/basics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    31828 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/components/extended_minimizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    95853 2023-04-07 15:44:09.000000 quickstats-0.6.7.8/quickstats/components/extended_model.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5575 2022-08-09 03:12:09.000000 quickstats-0.6.7.8/quickstats/components/extended_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15808 2023-04-05 14:33:57.000000 quickstats-0.6.7.8/quickstats/components/likelihood.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/components/modelling/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.6.7.8/quickstats/components/modelling/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2520 2022-09-18 05:43:28.000000 quickstats-0.6.7.8/quickstats/components/modelling/component_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20163 2023-03-30 14:17:36.000000 quickstats-0.6.7.8/quickstats/components/modelling/data_modelling.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      767 2022-09-18 12:07:18.000000 quickstats-0.6.7.8/quickstats/components/modelling/model_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4562 2022-09-18 16:32:35.000000 quickstats-0.6.7.8/quickstats/components/modelling/parameter_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5552 2023-03-27 16:00:16.000000 quickstats-0.6.7.8/quickstats/components/modelling/pdf_fit_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3541 2022-09-18 12:41:58.000000 quickstats-0.6.7.8/quickstats/components/modelling/tree_data_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10839 2022-04-07 03:18:15.000000 quickstats-0.6.7.8/quickstats/components/nuisance_parameter_harmonizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16921 2023-03-08 10:24:33.000000 quickstats-0.6.7.8/quickstats/components/nuisance_parameter_pull.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/components/processors/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      205 2022-07-19 21:07:01.000000 quickstats-0.6.7.8/quickstats/components/processors/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1985 2022-07-21 18:30:19.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2022-07-21 18:27:25.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/auxiliary.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1072 2023-03-05 12:07:49.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1082 2022-07-19 21:51:30.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_as_numpy.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2580 2022-08-29 07:36:48.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_base_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      710 2022-07-20 13:58:23.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_declare.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      821 2022-07-19 21:53:12.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      937 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_export.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1164 2022-07-21 15:20:21.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_filter.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1076 2022-08-29 06:56:49.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_global_variables.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_helper_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_hybrid_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      697 2022-07-21 18:29:41.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_if_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      704 2022-07-21 18:48:13.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_if_not_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-19 21:50:41.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_load_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:20.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_max.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      142 2022-07-19 20:41:10.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_mean.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:51.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_min.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_nested_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_rdf_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2022-07-19 20:28:28.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_redefine.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1657 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_report.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1382 2023-03-05 12:11:04.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_safe_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      454 2022-07-19 20:28:24.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_safe_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2204 2022-11-10 10:03:00.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_save.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      654 2022-07-19 21:53:28.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_save_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1194 2022-07-19 21:50:00.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_stat.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:39:49.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_sum.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      523 2022-07-19 21:54:23.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_treename.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7708 2022-08-29 03:05:08.000000 quickstats-0.6.7.8/quickstats/components/processors/builtin_methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6361 2022-07-21 19:15:41.000000 quickstats-0.6.7.8/quickstats/components/processors/roo_config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6267 2023-01-17 14:15:49.000000 quickstats-0.6.7.8/quickstats/components/processors/roo_processor.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5397 2021-09-16 21:06:55.000000 quickstats-0.6.7.8/quickstats/components/pvalue_toys.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3517 2022-07-20 11:52:20.000000 quickstats-0.6.7.8/quickstats/components/roo_inspector.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3107 2022-09-17 18:29:41.000000 quickstats-0.6.7.8/quickstats/components/root_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21144 2022-07-28 22:30:24.000000 quickstats-0.6.7.8/quickstats/components/toy_limit_calculator.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/components/workspaces/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      551 2023-01-13 12:37:11.000000 quickstats-0.6.7.8/quickstats/components/workspaces/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9929 2023-04-06 15:37:48.000000 quickstats-0.6.7.8/quickstats/components/workspaces/asimov_handler.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1734 2023-01-08 18:44:57.000000 quickstats-0.6.7.8/quickstats/components/workspaces/core_argument_sets.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2023-01-09 17:03:21.000000 quickstats-0.6.7.8/quickstats/components/workspaces/sample.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2023-03-11 17:09:50.000000 quickstats-0.6.7.8/quickstats/components/workspaces/settings.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8304 2023-04-06 16:51:30.000000 quickstats-0.6.7.8/quickstats/components/workspaces/systematic.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2023-01-08 18:43:45.000000 quickstats-0.6.7.8/quickstats/components/workspaces/systematics_domain.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    53246 2023-01-09 16:47:15.000000 quickstats-0.6.7.8/quickstats/components/workspaces/ws_comparer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1756 2022-04-20 13:20:42.000000 quickstats-0.6.7.8/quickstats/components/workspaces/ws_modifier_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10895 2023-03-20 15:33:53.000000 quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    87128 2023-03-20 15:19:21.000000 quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_builder_v1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    77944 2023-03-14 19:54:53.000000 quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_builder_v2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    45969 2023-01-04 17:04:30.000000 quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_combiner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    49107 2023-02-08 09:09:43.000000 quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_modifier.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/concurrent/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      228 2022-03-27 20:47:33.000000 quickstats-0.6.7.8/quickstats/concurrent/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2666 2022-09-21 07:46:09.000000 quickstats-0.6.7.8/quickstats/concurrent/abstract_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.6.7.8/quickstats/concurrent/logging.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5890 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/concurrent/parameterised_asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10317 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/concurrent/parameterised_likelihood.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3983 2022-09-20 17:52:34.000000 quickstats-0.6.7.8/quickstats/concurrent/parameterised_runner.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/core/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/core/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      811 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/core/abstract_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20616 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/core/configs.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2198 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/core/configurable_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      541 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/core/dataclass_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      977 2022-05-11 20:30:59.000000 quickstats-0.6.7.8/quickstats/core/decorators.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2201 2023-03-30 08:35:19.000000 quickstats-0.6.7.8/quickstats/core/enums.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6651 2023-02-14 22:36:19.000000 quickstats-0.6.7.8/quickstats/core/methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9057 2023-02-08 05:24:13.000000 quickstats-0.6.7.8/quickstats/core/path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2952 2022-07-21 15:05:33.000000 quickstats-0.6.7.8/quickstats/core/virtual_trees.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/interface/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       66 2022-01-31 04:51:23.000000 quickstats-0.6.7.8/quickstats/interface/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/interface/cppyy/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-31 03:26:35.000000 quickstats-0.6.7.8/quickstats/interface/cppyy/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2022-01-31 03:37:54.000000 quickstats-0.6.7.8/quickstats/interface/cppyy/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1032 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/interface/cppyy/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4433 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/interface/cppyy/vectorize.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/interface/root/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.6.7.8/quickstats/interface/root/RooAbsData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3951 2023-04-05 16:18:32.000000 quickstats-0.6.7.8/quickstats/interface/root/RooAbsPdf.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      420 2022-08-23 02:59:13.000000 quickstats-0.6.7.8/quickstats/interface/root/RooArgSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2023-03-12 16:17:52.000000 quickstats-0.6.7.8/quickstats/interface/root/RooCategory.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    32809 2023-04-03 12:29:10.000000 quickstats-0.6.7.8/quickstats/interface/root/RooDataSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.6.7.8/quickstats/interface/root/RooMsgService.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5440 2023-03-13 14:55:24.000000 quickstats-0.6.7.8/quickstats/interface/root/RooRealVar.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.6.7.8/quickstats/interface/root/TArrayData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/interface/root/TF1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1995 2023-02-28 09:57:47.000000 quickstats-0.6.7.8/quickstats/interface/root/TFile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2023-03-28 23:56:03.000000 quickstats-0.6.7.8/quickstats/interface/root/TH1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5489 2022-08-23 03:10:20.000000 quickstats-0.6.7.8/quickstats/interface/root/TH2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      571 2022-08-23 03:14:20.000000 quickstats-0.6.7.8/quickstats/interface/root/TObject.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      856 2023-03-12 13:27:02.000000 quickstats-0.6.7.8/quickstats/interface/root/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.6.7.8/quickstats/interface/root/helper.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-03-24 19:40:20.000000 quickstats-0.6.7.8/quickstats/interface/root/inspection.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.6.7.8/quickstats/interface/root/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13697 2023-03-13 15:22:18.000000 quickstats-0.6.7.8/quickstats/interface/root/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5578 2023-02-24 22:56:11.000000 quickstats-0.6.7.8/quickstats/interface/root/roofit_extension.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/macros/
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/macros/AsymptoticCLsTool/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7083 2021-08-19 17:39:48.000000 quickstats-0.6.7.8/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1511 2021-06-11 19:36:10.000000 quickstats-0.6.7.8/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/macros/FlexibleInterpVarMkII/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.6.7.8/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.6.7.8/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/macros/QuickStatsCore/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1231 2022-05-07 02:55:05.000000 quickstats-0.6.7.8/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10322 2022-05-11 00:00:32.000000 quickstats-0.6.7.8/quickstats/macros/QuickStatsCore/RooFitExt.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3429 2022-05-10 23:59:25.000000 quickstats-0.6.7.8/quickstats/macros/QuickStatsCore/RooFitExt.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/macros/ResponseFunction/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13946 2022-04-21 19:55:45.000000 quickstats-0.6.7.8/quickstats/macros/ResponseFunction/ResponseFunction.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2022-05-16 03:18:22.000000 quickstats-0.6.7.8/quickstats/macros/ResponseFunction/ResponseFunction.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/macros/RooTwoSidedCBShape/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.6.7.8/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.6.7.8/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/maths/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.6.7.8/quickstats/maths/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1130 2023-03-10 17:21:22.000000 quickstats-0.6.7.8/quickstats/maths/interpolation.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5548 2023-03-30 08:30:53.000000 quickstats-0.6.7.8/quickstats/maths/numerics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22465 2023-04-02 17:22:53.000000 quickstats-0.6.7.8/quickstats/maths/statistics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3480 2023-03-14 15:34:34.000000 quickstats-0.6.7.8/quickstats/maths/statistics_jitted.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.6.7.8/quickstats/maths/symbolics.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/parsers/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      113 2022-04-20 10:58:59.000000 quickstats-0.6.7.8/quickstats/parsers/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.6.7.8/quickstats/parsers/config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15568 2023-02-14 22:40:29.000000 quickstats-0.6.7.8/quickstats/parsers/param_parser.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/plots/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1441 2023-03-29 12:38:13.000000 quickstats-0.6.7.8/quickstats/plots/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12881 2023-04-03 01:58:46.000000 quickstats-0.6.7.8/quickstats/plots/abstract_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14145 2023-03-29 14:21:34.000000 quickstats-0.6.7.8/quickstats/plots/bidirectional_bar_chart.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.6.7.8/quickstats/plots/collective_data_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2750 2023-04-01 10:15:48.000000 quickstats-0.6.7.8/quickstats/plots/color_schemes.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5121 2023-04-02 16:46:10.000000 quickstats-0.6.7.8/quickstats/plots/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2687 2023-04-01 08:20:12.000000 quickstats-0.6.7.8/quickstats/plots/correlation_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5968 2023-03-22 14:09:34.000000 quickstats-0.6.7.8/quickstats/plots/general_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22775 2022-09-07 07:18:02.000000 quickstats-0.6.7.8/quickstats/plots/general_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3731 2022-09-09 08:30:51.000000 quickstats-0.6.7.8/quickstats/plots/histo_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6100 2023-03-21 16:34:42.000000 quickstats-0.6.7.8/quickstats/plots/hypotest_inverter_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5749 2023-04-06 23:36:13.000000 quickstats-0.6.7.8/quickstats/plots/likelihood_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9916 2023-04-10 17:13:17.000000 quickstats-0.6.7.8/quickstats/plots/likelihood_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      219 2021-04-19 13:56:55.000000 quickstats-0.6.7.8/quickstats/plots/likelihood_scan_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    26322 2022-04-19 14:42:15.000000 quickstats-0.6.7.8/quickstats/plots/np_ranking_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    25242 2023-03-30 08:39:20.000000 quickstats-0.6.7.8/quickstats/plots/pdf_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5059 2023-02-06 09:15:46.000000 quickstats-0.6.7.8/quickstats/plots/sample_purity_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10293 2023-03-27 13:06:51.000000 quickstats-0.6.7.8/quickstats/plots/score_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4123 2023-01-04 09:02:56.000000 quickstats-0.6.7.8/quickstats/plots/stat_plot_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18642 2023-04-02 13:33:12.000000 quickstats-0.6.7.8/quickstats/plots/template.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13688 2022-07-29 18:50:11.000000 quickstats-0.6.7.8/quickstats/plots/test_statistic_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11061 2023-01-04 09:02:56.000000 quickstats-0.6.7.8/quickstats/plots/upper_limit_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11855 2023-04-07 17:48:01.000000 quickstats-0.6.7.8/quickstats/plots/upper_limit_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13186 2022-08-18 13:35:04.000000 quickstats-0.6.7.8/quickstats/plots/upper_limit_3D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5069 2022-08-24 13:05:29.000000 quickstats-0.6.7.8/quickstats/plots/upper_limit_benchmark_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    23733 2023-04-03 02:04:48.000000 quickstats-0.6.7.8/quickstats/plots/variable_distribution_plot.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/resources/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2023-03-20 15:25:27.000000 quickstats-0.6.7.8/quickstats/resources/default_workspace_extensions.json
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-04-08 03:20:04.000000 quickstats-0.6.7.8/quickstats/root_checker.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/stylesheets/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2021-10-20 08:52:20.000000 quickstats-0.6.7.8/quickstats/stylesheets/quick_default.mplstyle
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/utils/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.6.7.8/quickstats/utils/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10897 2023-03-07 15:00:08.000000 quickstats-0.6.7.8/quickstats/utils/common_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.6.7.8/quickstats/utils/condor_tasks.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16140 2023-03-25 23:04:40.000000 quickstats-0.6.7.8/quickstats/utils/data_conversion.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.6.7.8/quickstats/utils/hep_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3862 2023-01-06 12:43:25.000000 quickstats-0.6.7.8/quickstats/utils/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      335 2021-05-17 13:11:29.000000 quickstats-0.6.7.8/quickstats/utils/process_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    25617 2023-04-06 16:59:06.000000 quickstats-0.6.7.8/quickstats/utils/roofit_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9267 2021-11-23 21:10:48.000000 quickstats-0.6.7.8/quickstats/utils/roostats_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12361 2023-01-04 09:02:56.000000 quickstats-0.6.7.8/quickstats/utils/root_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1225 2023-04-02 03:14:44.000000 quickstats-0.6.7.8/quickstats/utils/string_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15011 2023-03-14 18:38:57.000000 quickstats-0.6.7.8/quickstats/utils/xml_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats.egg-info/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-04-10 20:19:26.000000 quickstats-0.6.7.8/quickstats.egg-info/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8855 2023-04-10 20:19:26.000000 quickstats-0.6.7.8/quickstats.egg-info/SOURCES.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2023-04-10 20:19:26.000000 quickstats-0.6.7.8/quickstats.egg-info/dependency_links.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2023-04-10 20:19:26.000000 quickstats-0.6.7.8/quickstats.egg-info/requires.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2023-04-10 20:19:26.000000 quickstats-0.6.7.8/quickstats.egg-info/top_level.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/setup.cfg
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1687 2023-01-04 09:02:56.000000 quickstats-0.6.7.8/setup.py
```

### Comparing `quickstats-0.6.7.7/PKG-INFO` & `quickstats-0.6.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.6.7.7
+Version: 0.6.7.8
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.6.7.7/README.md` & `quickstats-0.6.7.8/README.md`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/bin/quickstats` & `quickstats-0.6.7.8/bin/quickstats`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/__init__.py` & `quickstats-0.6.7.8/quickstats/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/analysis/analysis_base.py` & `quickstats-0.6.7.8/quickstats/analysis/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/analysis/analysis_path_manager.py` & `quickstats-0.6.7.8/quickstats/analysis/analysis_path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/analysis/config_format_templates.py` & `quickstats-0.6.7.8/quickstats/analysis/config_format_templates.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,20 +4,30 @@
     "sample_dir": ConfigComponent(dtypes="STR", default="./",
                                   description="directory in which the input root samples are located"),
     "sample_subdir": ConfigComponent(dtypes="DICT[STR]", default_factory=dict,
                                      description="(optional) a dictionary mapping the sample type to the sub-directory "
                                                  "of input root samples in which the input root samples are located; "
                                                  "examples of sample type are the mc campaigns and data year for "
                                                  "mc and data samples respectively"),
-    "samples": ConfigComponent(dtypes=["DICT[DICT[STR]]", "DICT[DICT[LIST[STR]]]"], required=True,
+    "samples": ConfigComponent(dtypes=["DICT[DICT[STR]]", "DICT[DICT[LIST[STR]]]"], default_factory=dict,
                                description="A map from the sample name to the sample path in the form "
                                            "{<sample_type>: <sample_path>}; if path is given by an "
                                            "absolute path, the absolute path is used, otherwise the path "
                                            "{sample_dir}/{sample_subdir}/{path} is used",
-                               example='"sample_name": {"ggF": {"mc16a": "ggF_mc16a.root", "mc16d": "ggF_mc16d.root"}}'),
+                               example='"samples": {"ggF": {"mc16a": "ggF_mc16a.root", "mc16d": "ggF_mc16d.root"}}'),
+    "systematic_samples": ConfigComponent(dtypes=["DICT[DICT[DICT[ANY]]]"], default_factory=dict,
+                                          description="A map to the systematic sample path in the form "
+                                                      "<syst_theme>: {<sample_name>: {<sample_type>: <path>}}}; "
+                                                      "if path is given by an absolute path, the absolute path is used, "
+                                                      "otherwise the path {sample_dir}/{sample_subdir}/{path} is used",
+                                          example='"systematic_samples": {"PhotonSys": {"ggF": {"mc16a": "ggF_mc16a.root", '
+                                                  '"mc16d": "ggF_mc16d.root"}}}'),
+    "systematics": ConfigComponent(dtypes=["DICT[LIST[STR]]"], default_factory=dict,
+                                          description="A map to the list systematic names in the form "
+                                                      "<syst_theme>: [<syst_name>]"),
     "merge_samples": ConfigComponent(dtypes="DICT[LIST[STR]]", default_factory=dict,
                                      description="merge the given list of samples into a sample with a given name in "
                                                  "the form {<merged_sample_name>: <list_of_samples_to_be_merged>}",
                                      example='"merge_samples": {"H": ["ggF", "VBF", "VH", "ttH"]}')
 }
 
 DEFAULT_ANALYSIS_CONFIG_FORMAT = {
@@ -228,8 +238,46 @@
                                                               "category index; [0] is the first bin of a 1D (binary "
                                                               "class) boundary scan, [0, 0] is the first bin of a 2D "
                                                               "(multiclass, e.g. [score_signal_1, score_signal_2]) "
                                                               "boundary scan",
                                                   example='"channel": {"LowPtRegion": {"exclude_categories": [[0]]')
         }
     }
+}
+
+DEFAULT_SYSTEMATIC_EVAL_CONFIG = {
+    "observable": ConfigComponent(dtypes="STR", required=True,
+                                  description="Branch name of the observable in the root file"),
+    "weight": ConfigComponent(dtypes="STR", required=True,
+                              description="Branch name of the event weight in the root file"),
+    "index": ConfigComponent(dtypes=["STR", "LIST[STR]"], required=True,
+                             description="Branch name(s) used to index an event in the root file "
+                                         "(e.g. event number, run numver)"),
+    "category_selection": ConfigComponent(dtypes=["DICT[STR]"], required=True,
+                                          description="A map from the category to the corresponding selection"
+                                                      "criteria",
+                                          example='"category_selection": {"cat1": "cat_index == 1", '
+                                                  '"cat2": "cat_index==2"}'),
+    "systematics": ConfigComponent(dtypes=["DICT[LIST[STR]]"], default_factory=dict,
+                                          description="A map to the list systematic names in the form "
+                                                      "<syst_theme>: [<syst_name>]"),
+    "samples": ConfigComponent(dtypes=["LIST[STR]"], default_factory=list,
+                              description="List of samples to evaluate the systematics"),
+    "prune_significative": ConfigComponent(dtypes="BOOL", default=True,
+                                           description="Whether to prune non-significative systematics."),
+    "prune_threshold": ConfigComponent(dtypes="FLOAT", default=0,
+                                       description="Magnitude of systematic below which should be pruned."),
+    "n_toys": ConfigComponent(dtypes="INT", default=100,
+                              description="Number of bootstrap toys to use when evaluating shape systematics."),
+    "norm_syst_eval_method": ConfigComponent(dtypes="STR", default="analytic",
+                                             description="Method by which normalization systematics should be evaluated"),
+    "shape_syst_eval_method": ConfigComponent(dtypes="STR", default="bootstrap",
+                                              description="Method by which shape systematic should be evaluated"),
+    "shape_estimator": ConfigComponent(dtypes="STR", default="mean_IQR",
+                                       description="How the shape parameters (position, spread) should be estimated"),
+    "shape_syst_eval_options": ConfigComponent(dtypes="DICT", default_factory=dict,
+                                               description="Options passed to the shape systematics evaluator"),
+    "norm_syst_eval_options": ConfigComponent(dtypes="DICT", default_factory=dict,
+                                              description="Options passed to the normalization systematics evaluator"),
+    "shape_estimator_options": ConfigComponent(dtypes="DICT", default_factory=dict,
+                                               description="Options passed to the shape estimator"),
 }
```

### Comparing `quickstats-0.6.7.7/quickstats/analysis/data_loading.py` & `quickstats-0.6.7.8/quickstats/analysis/data_loading.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/analysis/data_preprocessing.py` & `quickstats-0.6.7.8/quickstats/analysis/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/analysis/event_categorization.py` & `quickstats-0.6.7.8/quickstats/analysis/event_categorization.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/analysis/multi_class_boundary_tree.py` & `quickstats-0.6.7.8/quickstats/analysis/multi_class_boundary_tree.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/analysis/ntuple_conversion_tool.py` & `quickstats-0.6.7.8/quickstats/analysis/ntuple_conversion_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     REQUIRED_CONFIG_COMPONENTS = ["paths:*"]
     
     DEFAULT_COLUMNS = {}
     
     DEFAULT_NTUPLE_SAMPLE_BASENAME = "{sample_name}.root"
     DEFAULT_ARRAY_SAMPLE_BASENAME  = "{sample_name}.{fmt}"
     
+    DEFAULT_NTUPLE_SYST_SAMPLE_BASENAME = "{sample_name}_{syst_name}.root"
+    DEFAULT_ARRAY_SYST_SAMPLE_BASENAME  = "{sample_name}_{syst_name}.{fmt}"
+    
     DEFAULT_H5_KEY = "analysis_data"
     
     def __init__(self, analysis_config:Optional[Union[Dict, str]]=None,
                  ntuple_dir:Optional[str]=None,
                  array_dir:Optional[str]=None,
                  verbosity:Optional[Union[int, str]]="INFO",
                  **kwargs):
@@ -141,15 +144,15 @@
     def get_ntuple_sample_path(self, sample_name:Dict, dirname:str):
         basename = self.DEFAULT_NTUPLE_SAMPLE_BASENAME.format(sample_name=sample_name)
         return os.path.join(dirname, basename)
     
     @semistaticmethod
     def get_array_sample_path(self, sample_name:Dict, dirname:str, fmt:str):
         basename = self.DEFAULT_ARRAY_SAMPLE_BASENAME.format(sample_name=sample_name, fmt=fmt)
-        return os.path.join(dirname, basename)    
+        return os.path.join(dirname, basename)
                  
     def convert_samples(self, samples:Optional[List[str]]=None,
                         kinematic_regions:Optional[List]=None,
                         columns:Optional[Union[List, Dict]]=None,
                         apply_columns:Optional[Dict]=None,
                         drop_columns:Optional[List]=None,
                         library:str="quickstats",
```

### Comparing `quickstats-0.6.7.7/quickstats/analysis/sample_poly_param_tool.py` & `quickstats-0.6.7.8/quickstats/analysis/sample_poly_param_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,18 @@
         else:
             from IPython import display
             display.display(expr)
             
     def display_sets(self, *objects):
         from sympy import FiniteSet
         self.display_expression(FiniteSet(*objects))
+        
+    def display_equation(self, variable, expression):
+        from sympy import Eq
+        self.display_expression(Eq(variable, expression))
     
     def solve_coefficients(self, formula, parameter_symbols:Dict, coefficient_symbols:Dict,
                     basis_symbols:Dict, basis_value_map:Dict):
         from sympy import simplify, solve
         equations = []
         for basis_name, basis_values in basis_value_map.items():
             subs = [(parameter_symbols[k], simplify(v)) for k, v in basis_values.items()]
@@ -136,25 +140,25 @@
         if len(solutions) == 0:
             raise RuntimeError("unable to solve the system of linear equations")
         elif len(solutions) > 1:
             raise RuntimeError("system of linear equations gives non-unique solutions")
         solution = solutions[0]
         self.stdout.info("Solutions:")
         for coefficient in coefficient_symbols.values():
-            self.display_sets(coefficient, solution[coefficient])
+            self.display_equation(coefficient, solution[coefficient])
         subs = [(k, v) for k, v in solution.items()]
         resolved_formula = formula_expr.subs(subs).expand()
         coefficient_map = {basis:resolved_formula.coeff(basis_symbols[basis]) for basis in bases}
         inverse_latex_map = self._get_inverse_latex_map(latex_map)
         coefficient_map_delatexed = {}
         for basis, coefficient_formula in coefficient_map.items():
             coefficient_map_delatexed[basis] = self.get_delatexed_formula(coefficient_formula, inverse_latex_map)
         self.stdout.info("Contribution from basis sample:")
         for basis, expr in coefficient_map.items():
-            self.display_sets(basis_symbols[basis], expr)
+            self.display_equation(basis_symbols[basis], expr)
         for basis in bases:
             param_data['sample'].append(basis_sample_map[basis])
             for parameter, value in basis_value_map[basis].items():
                 param_data[parameter].append(to_rounded_float(value))
             basis_symbol = basis_symbols[basis]
             param_data['expression'].append(str(coefficient_map_delatexed[basis]))
         return param_data
```

### Comparing `quickstats-0.6.7.7/quickstats/clis/core.py` & `quickstats-0.6.7.8/quickstats/clis/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                                                        'Use "//" as newline delimiter')
 @click.option('--elumi_label/--no_elumi_label', default=True, show_default=True,
               help='Show energy and luminosity labels')
 @click.option('--ranking_label/--no_ranking_label', default=True, show_default=True,
               help='Show ranking label')
 @click.option('--energy', default="13 TeV", show_default=True, 
               help='Beam energy')
-@click.option('--lumi', default="139 fb$^{-1}$", show_default=True, 
+@click.option('--lumi', default="140 fb$^{-1}$", show_default=True, 
               help='Luminosity')
 @click.option('--status', default="int", show_default=True, 
               help='\b\n Analysis status. Choose from'
                    '\b\n            int : Internal'
                    '\b\n            wip : Work in Progress'
                    '\b\n         prelim : Preliminary'
                    '\b\n          final : *no status label*'
```

### Comparing `quickstats-0.6.7.7/quickstats/clis/inspect_rfile.py` & `quickstats-0.6.7.8/quickstats/clis/inspect_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/clis/inspect_ws.py` & `quickstats-0.6.7.8/quickstats/clis/inspect_ws.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/clis/likelihood_fit.py` & `quickstats-0.6.7.8/quickstats/clis/likelihood_fit.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/clis/likelihood_scan.py` & `quickstats-0.6.7.8/quickstats/clis/likelihood_scan.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/clis/limit_setting.py` & `quickstats-0.6.7.8/quickstats/clis/limit_setting.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/clis/processor_cli.py` & `quickstats-0.6.7.8/quickstats/clis/processor_cli.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/clis/workspace_tools.py` & `quickstats-0.6.7.8/quickstats/clis/workspace_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
               help='Minimizer type')
 @click.option('-a', '--minimizer_algo', default="Migrad", show_default=True,
               help='Minimizer algorithm')
 @click.option('-c', '--num_cpu', type=int, default=1, show_default=True,
               help='Number of CPUs to use per parameter')
 @click.option('-e', '--eps', type=float, default=1.0, show_default=True,
               help='Convergence criterium')
-@click.option('--retry', type=int, default=0, show_default=True,
+@click.option('--retry', type=int, default=1, show_default=True,
               help='Maximum number of retries upon a failed fit')
 @click.option('--strategy', type=int, default=1, show_default=True,
               help='Default minimization strategy')
 @click.option('--print_level', type=int, default=-1, show_default=True,
               help='Minimizer print level')
 @click.option('--fix-cache/--no-fix-cache', default=True, show_default=True,
               help='Fix StarMomentMorph cache')
```

### Comparing `quickstats-0.6.7.7/quickstats/components/__init__.py` & `quickstats-0.6.7.8/quickstats/components/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/analysis_base.py` & `quickstats-0.6.7.8/quickstats/components/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/analysis_object.py` & `quickstats-0.6.7.8/quickstats/components/analysis_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/asimov_generator.py` & `quickstats-0.6.7.8/quickstats/components/asimov_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,16 @@
                  config:Optional[Union[Dict, str]]=None,
                  verbosity:Optional[Union[int, str]]="INFO"):
         config = parse_config(config)
         config['filename']  = filename
         config['poi_name']  = poi_name
         config['data_name'] = data_name
         config['verbosity'] = verbosity
+        if 'preset_param' not in config:
+            config['preset_param'] = True
         self._inherit_init(super(AsimovGenerator, self).__init__, **config)
         
     def generate_asimov(self, poi_val:Optional[float]=None, 
                         poi_profile:Optional[float]=None,
                         do_fit:bool=True,
                         modify_globs:bool=True,
                         do_import:bool=True,
@@ -155,14 +157,15 @@
             assert len(asimov_names) == len(asimov_types)
         if asimov_snapshots is not None:
             if isinstance(asimov_snapshots, str):
                 asimov_snapshots = [asimov_snapshots]
             assert len(asimov_snapshots) == len(asimov_types)            
         if poi_scale is None:
             poi_scale = 1.0
+            
         poi_name = self.poi.GetName()
         self.save_snapshot("temp", WSArgument.MUTABLE)
         asimov_datasets = []
         for i, asimov_type in enumerate(asimov_types):
             self.load_snapshot("temp")
             kwargs = copy.deepcopy(self.ASIMOV_SETTINGS[asimov_type])
             if kwargs is None:
@@ -171,15 +174,16 @@
             for key in ['poi_val', 'poi_profile']:
                 if kwargs[key] is not None:
                     kwargs[key] *= poi_scale
             if asimov_names is not None:
                 kwargs['asimov_name'] = asimov_names[i]
             if asimov_snapshots is not None:
                 kwargs['asimov_snapshot'] = asimov_snapshots[i]
-            kwargs['minimizer_options'] = self.minimizer.config
-            kwargs['nll_options'] = list(self.minimizer.nll_commands.values())
+            kwargs['dataset'] = self.model.data
+            kwargs['minimizer_options'] = self.default_minimizer_options
+            kwargs['nll_options'] = self.default_nll_options
             kwargs['do_import'] = do_import
             asimov_dataset = self.model.generate_asimov(**kwargs)
             asimov_datasets.append(asimov_dataset)
         if single_asimov:
             return asimov_datasets[0]
         return asimov_datasets
```

### Comparing `quickstats-0.6.7.7/quickstats/components/asymptotic_cls.py` & `quickstats-0.6.7.8/quickstats/components/asymptotic_cls.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
         return name
 
     def get_nll_val(self, nll:"ROOT.RooNLLVar"):
         snapshot_name = self.nll_maps[nll].get('snapshot', None)
         if snapshot_name:
             self.load_snapshot(snapshot_name)
         else:
-            raise RuntimeError('Failed to load snapshot for nll "{}"'.format(nll.GetName()))
+            raise RuntimeError(f'Failed to load snapshot for nll "{nll.GetName()}"')
         if Verbosity.DEBUG >= self.stdout.verbosity:
             self.stdout.debug("DEBUG: Before Fit ----------------------------------------------")
             self.model.print_summary(items=['poi', 'nuisance_parameter', 'global_observable'])
         self.last_fit_status = self.minimizer.minimize(nll) 
         self.global_status += self.last_fit_status
         self.minimizer_calls += 1
         nll_val = nll.getVal()
@@ -270,18 +270,16 @@
         else:
             mu_hat = self.nll_maps[nll]['mu_hat']
         
         if (mu_hat < 0.1) or (initial_guess != 0):
             self.set_poi_value(initial_guess)
 
         mu = self.poi.getVal()
-        from pdb import set_trace
         
         qmu = self.get_qmu(asimov_0_nll, mu)
-        #set_trace()
         sigma_guess = self.LimitTool.getSigma(mu, self.mu_exp, qmu)
         sigma_b = sigma_guess
         mu_guess = self.LimitTool.findCrossing(sigma_guess, sigma_b, mu_hat)
         pmu = self.LimitTool.calcPmu(qmu, sigma_b, mu_guess)
         pb = self.LimitTool.calcPb(qmu, sigma_b, mu_guess)
         CLs = self.LimitTool.calcCLs(qmu, sigma_b, mu_guess)
         qmu95 = self.LimitTool.getQmu95(sigma_b, mu_guess)
```

### Comparing `quickstats-0.6.7.7/quickstats/components/basics.py` & `quickstats-0.6.7.8/quickstats/components/basics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/extended_minimizer.py` & `quickstats-0.6.7.8/quickstats/components/extended_minimizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/extended_model.py` & `quickstats-0.6.7.8/quickstats/components/extended_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Author: Alkaid Cheng
 # Email: chi.lung.cheng@cern.ch
 ##################################################################################################
 import os
 import sys
 import copy
 import math
+import uuid
 import fnmatch
 from typing import List, Optional, Union, Dict, Set, Tuple
 
 import numpy as np
 
 import ROOT
 from ROOT.RooPrintable import (kName, kClassName, kValue, kArgs, kExtras, kAddress,
@@ -20,15 +21,15 @@
 from quickstats import semistaticmethod, AbstractObject
 from quickstats.maths.numerics import is_integer, pretty_value, get_bins_given_edges, array_issubset
 from quickstats.utils.root_utils import load_macro
 from quickstats.utils.common_utils import str_list_filter
 from quickstats.utils.roofit_utils import (get_variable_attributes, variable_collection_to_dataframe,
                                            get_relevant_components)
 from quickstats.utils.string_utils import split_str
-from quickstats.interface.root import TH1, RooDataSet, RooArgSet, RooMsgService
+from quickstats.interface.root import TH1, RooDataSet, RooArgSet, RooMsgService, RooAbsPdf
 from quickstats.interface.root import roofit_extension as rf_ext
 from quickstats.interface.root.roofit_extension import get_str_data
 from quickstats.components.basics import WSArgument, SetValueMode
 from .extended_minimizer import ExtendedMinimizer
 
 class ExtendedModel(AbstractObject):
     
@@ -1245,27 +1246,27 @@
         if pdf is None:
             pdf = self.pdf
         if not isinstance(pdf, ROOT.RooSimultaneous):
             raise ValueError("input pdf is not a simultaneous pdf")            
         category_map = {}
         index_cat = pdf.indexCat()
         n_cat = index_cat.size()
-        for i in range(n_cat):
-            index_cat.setIndex(i)
-            label = index_cat.getLabel()
-            pdf_cat = pdf.getPdf(label)
+        for cat_data in index_cat:
+            cat_label = cat_data.first
+            cat_index = cat_data.second
+            pdf_cat = pdf.getPdf(cat_label)
             obs = pdf_cat.getObservables(self.observables)
             target_obs = obs.first()
-            category_map[label] = {}
-            category_map[label]['index'] = i
-            category_map[label]['pdf'] = pdf_cat.GetName()
-            category_map[label]['observable'] = target_obs.GetName()
+            category_map[cat_label] = {}
+            category_map[cat_label]['index'] = cat_index
+            category_map[cat_label]['pdf'] = pdf_cat.GetName()
+            category_map[cat_label]['observable'] = target_obs.GetName()
             bin_range = target_obs.getRange()
-            category_map[label]['bin_range'] = (bin_range.first, bin_range.second)
-            category_map[label]['bins'] = target_obs.getBins()
+            category_map[cat_label]['bin_range'] = (bin_range.first, bin_range.second)
+            category_map[cat_label]['bins'] = target_obs.getBins()
         return category_map
     
     @staticmethod
     def get_dataset_values(dataset:ROOT.RooDataSet):
         return RooDataSet.to_numpy(dataset)
     
     def _get_new_binnings(self, bins:Optional[Union[Dict, int]]=None):
@@ -1286,28 +1287,31 @@
                 raise RuntimeError(f"invalid binning format: {bins}")
             bin_width = round((bin_range[1] - bin_range[0]) / _bins, 8)
             binnings[category]['bin_range'] = bin_range
             binnings[category]['bins'] = _bins
             binnings[category]['bin_width'] = bin_width
         return binnings
     
-    def get_dataset_distributions(self, dataset, n_bins:Optional[Union[Dict, int]]=None):
+    def get_dataset_distributions(self, dataset, n_bins:Optional[Union[Dict, int]]=None,
+                                  sum_over_category:bool=False):
         distributions = {}
         dataset_values = self.get_dataset_values(dataset)
-        if 'label' not in dataset_values:
+        if 'category_index' not in dataset_values:
             raise RuntimeError("no categories defined in the dataset")
         category_map = self.get_category_map()
         binnings = self._get_new_binnings(n_bins)
-        for cat in category_map:
+        is_binned = {}
+        for cat, cat_data in category_map.items():
             distributions[cat] = {}
             observable = category_map[cat]['observable']
             if observable not in dataset_values:
                 raise RuntimeError(f"no data associated with the observable \"{observable}\" found in the dataset")
             distributions[cat]['observable'] = observable
-            mask = (dataset_values['label'] == cat)
+            cat_index = cat_data['index']
+            mask = (dataset_values['category_index'] == cat_index)
             x = dataset_values[observable][mask]
             ind = np.argsort(x)
             x = x[ind]
             y = dataset_values['weight'][mask][ind]
             default_bins = category_map[cat]['bins']
             ghost  = False
             if np.all(y == 1.):
@@ -1340,38 +1344,113 @@
                         x = x[idx]
                         y = y[idx]
                     else:
                         raise RuntimeError(f"detected dataset with invalid binning")
             bins = binnings[cat]['bins']
             if binned:
                 if  (bins != default_bins):
-                    raise RuntimeError(f"cannot change binning of binned dataset ({dataset.GetName()}, cat = {cat}): "
-                                       f"original binning = {default_bins}, requested binning = {bins}")
+                    # rebinning
+                    from quickstats.maths.statistics import bin_center_to_bin_edge
+                    bin_edges = bin_center_to_bin_edge(x)
+                    from quickstats.interface.root import TH1
+                    pyh = TH1.from_numpy_histogram(y, bin_edges=bin_edges)
+                    pyh.rebin(bins)
+                    self.stdout.warning(f"WARNING: Rebinned dataset ({dataset.GetName()}, cat = {cat}) from "
+                                        f"nbins = {default_bins} to nbins = {bins}")
+                    x = pyh.bin_center
+                    y = pyh.bin_content
                 distributions[cat]['x'] = x
                 distributions[cat]['y'] = y
+                is_binned[cat] = True
             else:
                 bin_range = binnings[cat]['bin_range']
                 if not ghost:
                     hist, bin_edges = np.histogram(x, bins=bins, range=(bin_range[0], bin_range[1]))
                     bin_centers = (bin_edges[1:] + bin_edges[:-1])/2
                     distributions[cat]['x'] = bin_centers
                     distributions[cat]['y'] = hist
                 else:
                     ghost_idx = y < 1e-8
                     hist, bin_edges = np.histogram(x[~ghost_idx], bins=bins, range=(bin_range[0], bin_range[1]))
                     hist_g, _ = np.histogram(x[ghost_idx], bins=bins, range=(bin_range[0], bin_range[1]), weights=y[ghost_idx])
                     bin_centers = (bin_edges[1:] + bin_edges[:-1])/2
                     distributions[cat]['x'] = bin_centers
                     distributions[cat]['y'] = hist + hist_g
-                bin_errors = TH1.GetPoissonError(distributions[cat]['y'])
-                distributions[cat]['yerrlo'] = bin_errors['lo']
-                distributions[cat]['yerrhi'] = bin_errors['hi']
+                is_binned[cat] = False
+        if sum_over_category:
+            distributions = self._merged_category_distributions(distributions)
+        for cat in distributions:
+            if is_binned[cat]:
+                continue
+            from quickstats.interface.root import TH1
+            bin_errors = TH1.GetPoissonError(distributions[cat]['y'])
+            distributions[cat]['yerrlo'] = bin_errors['lo']
+            distributions[cat]['yerrhi'] = bin_errors['hi']
+        return distributions
+    
+    def _merged_category_distributions(self, distributions):
+        categories = list(distributions)
+        if len(categories) == 1:
+            distributions['all_cat'] = distributions.pop(categories[0])
+        else:
+            binning_first_cat = distributions[categories[0]]['x']
+            if not all(np.allclose(binning_first_cat, distributions[categories[j]]['x']) 
+                       for j in range(1, len(categories))):
+                raise ValueError('can not sum over categories with different binnings')
+            distributions['all_cat'] = distributions.pop(categories[0])
+            for category in categories[1:]:
+                distributions['all_cat']['y'] += distributions[category]['y']
+                distributions.pop(category)
+            distributions['all_cat']['observable'] = ''
         return distributions
 
-    def get_simul_pdf_distributions(self, pdf, observables, n_bins:Optional[Union[Dict, int]]=None):
+    def get_category_pdf_distribution(self, category:str,
+                                      nbins:Optional[int]=None,
+                                      bin_range:Optional[Tuple[float]]=None,
+                                      weight_scale:Optional[float]=None):
+        pdf_cat = self.pdf.getPdf(category)
+        result = RooAbsPdf.get_distribution(pdf_cat, self.observables,
+                                            nbins=nbins, bin_range=bin_range,
+                                            weight_scale=weight_scale)
+        return result
+    
+    def get_merged_pdf_distribution(self, categories:Optional[List[str]]=None,
+                                    nbins:Optional[int]=None,
+                                    bin_range:Optional[Tuple[float]]=None,
+                                    weight_scales:Optional[Union[float, Dict[str, float]]]=None):
+        if categories is None:
+            categories = list(self.get_category_map())
+        if weight_scales is None:
+            weight_scales = {}
+        if not isinstance(weight_scales, dict):
+            weight_scales = {category: weight_scales for category in categories}
+        x = None
+        y = None
+        for category in categories:
+            weight_scale = weight_scales.get(category, None)
+            distribution = self.get_category_pdf_distribution(category=category,
+                                                              nbins=nbins,
+                                                              bin_range=bin_range,
+                                                              weight_scale=weight_scale)
+            if x is None:
+                x = distribution['x']
+                y = distribution['y']
+            elif not np.array_equal(x, distribution['x']):
+                raise RuntimeError('can not merge categories with different binnings')
+            else:
+                y += distribution['y']
+        result = {
+            'x': x,
+            'y': y
+        }
+        return result
+    
+    def get_simul_pdf_distributions(self, pdf, observables,
+                                    n_bins:Optional[Union[Dict, int]]=None,
+                                    sum_over_category:bool=False):
         if not isinstance(pdf, ROOT.RooSimultaneous):
             raise ValueError("input pdf is not a simultaneous pdf")
         distributions = {}
         channel_cat = pdf.indexCat()
         n_cat = channel_cat.size()
         binnings = self._get_new_binnings(n_bins)
         for i in range(n_cat):
@@ -1388,127 +1467,149 @@
             bin_width = binnings[label]['bin_width']
             h = pdf_cat.createHistogram(target_obs.GetName(), bins)
             py_h = TH1(h)
             distributions[label]['x'] = py_h.bin_center
             distributions[label]['y'] = py_h.bin_content * bin_width
             # free memory to avoid memory leak
             h.Delete()
-            """
-            expected_events = pdf_cat.expectedEvents(obs)
-            for i in range(n_bins):
-                target_obs.setBin(i)
-                norm = pdf_cat.getVal(obs)*target_obs.getBinWidth(i)
-                n_events = norm*expected_events
-                bin_value = target_obs.getVal()
-                if n_events <= 0:
-                    self.stdout.warning("WARNING: Detected bin with zero expected events ({})! "
-                                    "Please check your inputs. Obs = {}, bin = {}".format(
-                                    n_events, target_obs.GetName(), i))
-                elif (n_events > 0) and (n_events < 1e18):
-                    distributions[label]['x'].append(bin_value)
-                    distributions[label]['y'].append(n_events)
-                else:
-                    raise RuntimeError(f"detected pdf bin with nan (pdf={pdf.GetName()},obs={target_obs.GetName()},bin={i})")
-            """
+        if sum_over_category:
+            distributions = self._merged_category_distributions(distributions)
         return distributions
     
-    def get_distributions(self, n_bins:Optional[Union[Dict, int]]=None):
-        return self.get_simul_pdf_distributions(self.pdf, self.observables, n_bins=n_bins)
+    def get_distributions(self, n_bins:Optional[Union[Dict, int]]=None,
+                          sum_over_category:bool=False):
+        return self.get_simul_pdf_distributions(self.pdf, self.observables, n_bins=n_bins,
+                                                sum_over_category=sum_over_category)
     
     def get_categories(self):
         return list(self.get_category_map())
     
     def get_collected_distributions(self, current_distributions=True,
                                     datasets:Optional[Union[List[str],List[ROOT.RooDataSet]]]=None,
                                     snapshots:Optional[List[str]]=None,
                                     n_bins:Optional[Union[Dict, int]]=None,
-                                    n_pdf_bins:Optional[Union[Dict, int]]=None):
+                                    n_pdf_bins:Optional[Union[Dict, int]]=None,
+                                    sum_over_category:bool=False):
         collected_distributions = {}
                 
         if datasets is not None:
             for dataset in datasets:
                 if isinstance(dataset, str):
                     dataset_name = dataset
                     dataset = self.workspace.data(dataset)
                     if not dataset:
                         raise ValueError(f"dataset \"{dataset_name}\" does not exist")
                 dataset_name = dataset.GetName()
-                distributions = self.get_dataset_distributions(dataset, n_bins=n_bins)
+                distributions = self.get_dataset_distributions(dataset, n_bins=n_bins,
+                                                               sum_over_category=sum_over_category)
                 for category in distributions:
                     if category not in collected_distributions:
                         collected_distributions[category] = {}
                     collected_distributions[category][dataset_name] = distributions[category]
 
         if current_distributions:
             if n_pdf_bins is not None:
-                distributions = self.get_distributions(n_bins=n_pdf_bins)
-            else:
-                distributions = self.get_distributions(n_bins=n_bins)
+                distributions = self.get_distributions(n_bins=n_pdf_bins,
+                                                       sum_over_category=sum_over_category)
+                distributions_binned = self.get_distributions(n_bins=n_bins,
+                                                              sum_over_category=sum_over_category)
+            else:
+                distributions = self.get_distributions(n_bins=n_bins,
+                                                       sum_over_category=sum_over_category)
+                distributions_binned = None
             for category in distributions:
                 if category not in collected_distributions:
                     collected_distributions[category] = {}
                 collected_distributions[category]['Current'] = distributions[category]
+                if distributions_binned is not None:
+                    collected_distributions[category]['Current_binned'] = distributions_binned[category]
 
         if snapshots is not None:
             self.workspace.saveSnapshot("tmp", self.workspace.allVars())
             try:
                 for snapshot in snapshots:
                     exist = self.workspace.loadSnapshot(snapshot)
                     if not exist:
                         raise RuntimeError("snapshot \"{}\" not found in workspace".format(snapshot))
                     if n_pdf_bins is not None:
-                        distributions = self.get_distributions(n_bins=n_pdf_bins)
+                        distributions = self.get_distributions(n_bins=n_pdf_bins,
+                                                               sum_over_category=sum_over_category)
+                        distributions_binned = self.get_distributions(n_bins=n_bins,
+                                                                      sum_over_category=sum_over_category)
                     else:
-                        distributions = self.get_distributions(n_bins=n_bins)
+                        distributions = self.get_distributions(n_bins=n_bins,
+                                                               sum_over_category=sum_over_category)
+                        distributions_binned = None
                     for category in distributions:
                         if category not in collected_distributions:
                             collected_distributions[category] = {}
                         collected_distributions[category][snapshot] = distributions[category]
+                        if distributions_binned is not None:
+                            collected_distributions[category][f'{snapshot}_binned'] = distributions_binned[category]
             finally:
                 self.workspace.loadSnapshot("tmp")
         return collected_distributions
             
     def plot_distributions(self, categories:Optional[List[str]]=None, current_distributions=True, 
                            datasets:Optional[Union[List[str],List[ROOT.RooDataSet]]]=None,
                            snapshots:Optional[Union[List[str], List[ROOT.RooArgSet]]]=None,
+                           sum_over_category:bool=False,
                            n_bins:Optional[Union[Dict, int]]=None, n_pdf_bins:Optional[Union[Dict, int]]=None,
                            discriminant:Optional[str]=None, unit:Optional[str]=None, blind:bool=False,
                            show_error:bool=True, comparison_options:Optional[Dict]=None,
+                           draw_options:Optional[Dict]=None,
                            logx:bool=False, logy:bool=False,
                            save_as:Optional[str]=None, **kwargs):
         from quickstats.plots import PdfDistributionPlot
         category_map = self.get_category_map()
         if categories is None:
             categories = list(category_map)
         for category in categories:
             if category not in category_map:
                 raise ValueError("category \"{}\" not found in workspace".format(category))
         collected_distributions = self.get_collected_distributions(current_distributions,
                                                                    datasets, snapshots=snapshots,
                                                                    n_bins=n_bins,
-                                                                   n_pdf_bins=n_pdf_bins)
+                                                                   n_pdf_bins=n_pdf_bins,
+                                                                   sum_over_category=sum_over_category)
         if save_as is not None:
             from matplotlib.backends.backend_pdf import PdfPages
             pdf = PdfPages(save_as)
         else:
             pdf = None
             
+        if draw_options is None:
+            draw_options = {}
+            
         if blind:
             all_blind_range = self.get_blind_range()
         else:
             all_blind_range = {}
             
         dataset_names = []    
         if datasets is not None:
             for dataset in datasets:
                 if isinstance(dataset, ROOT.RooDataSet):
                     dataset_names.append(dataset.GetName())
                 else:
                     dataset_names.append(dataset)
-                    
+        target_distributions = []
+        if current_distributions:
+            target_distributions.append('Current')
+        if datasets:
+            target_distributions.extend(datasets)
+        if snapshots:
+            target_distributions.extend(snapshots)
+        
+        
+        if sum_over_category:
+            category_map['all_cat'] = ''
+            binnings['all_cat'] = combine_dict(binnings[categories[0]])
+        
+        categories = list(collected_distributions)
         for i, category in enumerate(categories):
             obs_name = category_map[category]['observable']
             if discriminant is None:
                 xlabel = obs_name
             else:
                 #xlabel = f"{discriminant}_{category}"
                 xlabel = f"{discriminant} (category {category})"
@@ -1527,34 +1628,33 @@
             if _n_pdf_bins is not None:
                 binning_map = {}
                 for key in collected_distributions[category]:
                     data = collected_distributions[category][key]
                     binning_map[key] = data["x"].shape[0]
                 data_binnings = list(set(binning_map.values()) - set([_n_pdf_bins]))
                 if len(data_binnings) == 0:
-                    scale_map = None
+                    pass
                 elif len(data_binnings) == 1:
                     data_binnings = data_binnings[0]
-                    scale_map = {}
                     for key in binning_map:
-                        scale_map[key] = binning_map[key] / data_binnings
+                        data = collected_distributions[category][key]
+                        data['y'] *= binning_map[key] / data_binnings
                 else:
                     raise RuntimeError("found mixed binnings in the target distributions")
-            else:
-                scale_map = None
 
             blind_range = all_blind_range.get(obs_name, None)
             plotter = PdfDistributionPlot(collected_distributions[category],
-                                          scale_map=scale_map,
                                           figure_index=i, **kwargs)
             ax = plotter.draw(xlabel=xlabel, ylabel=ylabel,
                               logx=logx, logy=logy,
                               blind_range=blind_range,
                               show_error=show_error,
-                              comparison_options=comparison_options)
+                              targets=target_distributions,
+                              comparison_options=comparison_options,
+                              **draw_options)
             if pdf is not None:
                 pdf.savefig(bbox_inches="tight")
         if pdf is not None:
             pdf.close()
         return None
     
     def _load_floating_auxiliary_variables(self):
@@ -1763,44 +1863,14 @@
     def get_systematics_variations(self, filter_name:Optional[str]=None,
                                    filter_client:Optional[str]=None, fmt:str="pandas"):
         from quickstats.utils.roofit_utils import get_systematics_variations
         constr_pdfs, constr_nuis, _ = self.pair_constraints()
         return get_systematics_variations(constr_nuis, constr_pdfs, filter_name=filter_name,
                                           filter_client=filter_client, fmt=fmt)
     
-    def compare_datasets(self, ds1:Union[str, ROOT.RooDataSet], ds2:Union[str, ROOT.RooDataSet]):
-        datasets = {}
-        for label, ds in [("left", ds1), ("right", ds2)]:
-            if isinstance(ds, str):
-                if not self.workspace.data(ds):
-                    raise ValueError(f'workspace does not contain a dataset named "{ds}"')
-                ds = self.workspace.data(ds)
-            if not isinstance(ds, ROOT.RooDataSet):
-                raise TypeError('dataset must be an instance of RooDataSet')
-            datasets[label] = ds
-        dataset_values = {}
-        from quickstats.interface.root import RooDataSet
-        for key, ds in datasets.items():
-            dataset_values[key] = RooDataSet.to_category_data(ds, self.pdf)
-        categories = list(dataset_values["left"])
-        difference = {}
-        identical_cats = []
-        modified_cats = []
-        for category in categories:
-            difference[category] = dataset_values["left"][category] - dataset_values["right"][category]
-            if np.allclose(dataset_values["left"][category], dataset_values["right"][category], rtol=1e-8):
-                identical_cats.append(category)
-            else:
-                modified_cats.append(category)
-        for cat_type, cats in [("identical", identical_cats), ("modified", modified_cats)]:
-            self.stdout.info(f"Categories with {cat_type} dataset values:")
-            for cat in cats:
-                self.stdout.info(f"\t{cat}")
-        return difference
-    
     def compare_snapshots(self, ss1:Union[str, ROOT.RooArgSet], ss2:Union[str, ROOT.RooArgSet]):
         snapshots = {}
         for label, ss in [("left", ss1), ("right", ss2)]:
             if isinstance(ss, str):
                 if not self.workspace.getSnapshot(ss):
                     raise ValueError(f'workspace does not contain a snapshot named "{ss}"')
                 ss = self.workspace.getSnapshot(ss)
@@ -1827,8 +1897,25 @@
         constr_pdfs, _, _ = self.pair_constraints()
         from quickstats.utils.roofit_utils import get_gaussian_pdf_attributes
         return get_gaussian_pdf_attributes(constr_pdfs, fmt=fmt)
    
     def get_poisson_constraint_attributes(self, fmt:str="pandas"):
         constr_pdfs, _, _ = self.pair_constraints()
         from quickstats.utils.roofit_utils import get_poisson_pdf_attributes
-        return get_poisson_pdf_attributes(constr_pdfs, fmt=fmt)
+        return get_poisson_pdf_attributes(constr_pdfs, fmt=fmt)
+    
+    
+    def get_category_expected_events_over_range(self, category:str, range:List[float],
+                                                normalized:bool=False):
+        assert len(range) == 2
+        range_name = uuid.uuid4().hex
+        pdf_cat = self.pdf.getPdf(category)
+        if not pdf_cat:
+            raise RuntimeError(f'{category} is not a valid category in the workspace')
+        observables = pdf_cat.getObservables(self.observables)
+        observables.first().setRange(range_name, range[0], range[1])
+        integral = pdf_cat.createIntegral(observables, ROOT.RooFit.NormSet(observables),
+                                          ROOT.RooFit.Range(range_name)).getVal()
+        observables.first().removeRange(range_name)
+        if not normalized:
+            integral *= pdf_cat.expectedEvents(observables)
+        return integral
```

### Comparing `quickstats-0.6.7.7/quickstats/components/extended_rfile.py` & `quickstats-0.6.7.8/quickstats/components/extended_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/likelihood.py` & `quickstats-0.6.7.8/quickstats/components/likelihood.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
                  config:Optional[Dict]=None,
                  verbosity:Optional[Union[int, str]]="INFO"):
         config = parse_config(config)
         config['filename']  = filename
         config['poi_name']  = poi_name
         config['data_name'] = data_name
         config['verbosity'] = verbosity
+        if 'preset_param' not in config:
+            config['preset_param'] = True
         self._inherit_init(super().__init__, **config)
         self.roofit_result = None
     
     @staticmethod
     def _parse_poi_val(pois:"ROOT.RooArgSet", poi_val:Optional[Union[Dict[str, float], float]]=None):
         if poi_val is None:
             poi_val = {}
@@ -292,14 +294,15 @@
             fit_result['total_time'] = fit_time_uncond + fit_time_cond
         else:
             self.stdout.info("prefit NLL = ".rjust(18) + f"{prefit_nll:.5f}")
             self.stdout.info("postfit NLL = ".rjust(18) + f"{postfit_nll:.5f}")
             self.stdout.info("time = ".rjust(18) + f"{fit_time:.3f}")
             fit_result['prefit_nll'] = prefit_nll
             fit_result['postfit_nll'] = postfit_nll
+            fit_result['status'] =  fit_status
             fit_result['total_time'] = fit_time
         
         self.roofit_result = roofit_result
         
         # finallizing
         self.minimizer.config['minos'] = tmp_do_minos
         self.minimizer.minos_set = ROOT.RooArgSet()
```

### Comparing `quickstats-0.6.7.7/quickstats/components/modelling/component_source.py` & `quickstats-0.6.7.8/quickstats/components/modelling/component_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/modelling/data_modelling.py` & `quickstats-0.6.7.8/quickstats/components/modelling/data_modelling.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         'print_level': -1,
         'min_fit': 2,
         'max_fit': 3,
         'binned': False,
         'minos': False,
         'hesse': True,
         'sumw2': True,
+        'asymptotic': False,
         'strategy': 1,
         'range_expand_rate': 1        
     }
     
     _DEFAULT_PLOT_OPTION_ = {
         'bin_range': None,
         'n_bins_data': None,
@@ -193,15 +194,16 @@
                     'error'  : parameters[name].getError()
                 }
         return param_data
 
     @semistaticmethod
     def _run(self, filename:str, tree_name:str, model_class:Callable, param_templates:Callable,
              fit_options:Dict, plot_options:Optional[Dict]=None, save_summary_as:Optional[str]=None, 
-             save_param_as:Optional[str]=None, save_plot_as:Optional[str]=None):
+             save_param_as:Optional[str]=None, save_plot_as:Optional[str]=None,
+             save_data_as:Optional[str]=None):
         
         with Timer() as t:
             canvas = ROOT.TCanvas(uuid.uuid4().hex)
             observable_config = {
                 'name'        : fit_options['observable'],
                 'range'       : fit_options['range'],
                 'n_bins'      : fit_options['n_bins']
@@ -220,14 +222,15 @@
             model_pdf = model_class(model_name, model_name, observable, *model_parameters.values())
 
             fit_kwargs = {
                 'minos'             : fit_options['minos'],
                 'hesse'             : fit_options['hesse'],
                 'strategy'          : fit_options['strategy'],
                 'sumw2'             : fit_options['sumw2'],
+                'asymptotic'        : fit_options['asymptotic'],
                 'min_fit'           : fit_options['min_fit'],
                 'max_fit'           : fit_options['max_fit'],
                 'range_expand_rate' : fit_options['range_expand_rate'],
                 'print_level'       : fit_options['print_level']
             }
 
             fit_tool   = PdfFitTool(model_pdf, dataset, verbosity=self.stdout.verbosity)
@@ -254,32 +257,63 @@
         if not isinstance(summary['fit_options']['functional_form'], str):
             summary['fit_options']['functional_form'] = type(summary['fit_options']['functional_form']).__name__
             
         if save_plot_as is not None:
             self.create_plot(dataset, model_pdf, observable,
                              plot_options=plot_options,
                              model_summary=summary,
-                             save_as=save_plot_as)
+                             save_plot_as=save_plot_as,
+                             save_data_as=save_data_as)
 
         if save_param_as is not None:
             with open(save_param_as, "w") as outfile:
                 json.dump(param_data_value_only, outfile, indent=2)
                 
         if save_summary_as is not None:
             with open(save_summary_as, "w") as outfile:
                 json.dump(summary, outfile, indent=2)
 
         return summary
     
     @semistaticmethod
+    def get_model_summary_text(self, model_summary:Dict,
+                               value_fmt:str="{:.2f}",
+                               show_params:bool=True,
+                               show_stats:bool=True,
+                               show_error:bool=True,
+                               stats_list:Optional[List[str]]=None):
+        text = ""
+        if show_params:
+            param_data = model_summary["parameters"]
+            for param in param_data:
+                value = value_fmt.format(param_data[param]["value"])
+                if show_error:
+                    error = value_fmt.format(param_data[param]["error"])
+                    text += f"{param} = {value} $\\pm$ {error}\n"
+                else:
+                    text += f"{param} = {value}\n"
+            text += "\n"
+        if show_stats:
+            if stats_list is None:
+                stats_list = list(model_summary["stats"])
+            for stat in stats_list:
+                if stat not in model_summary["stats"]:
+                    raise RuntimeError(f"invalid stats item: {stat}")
+                value = value_fmt.format(model_summary["stats"][stat])
+                text += f"{stat} = {value}\n"
+            text += "\n"
+        return text
+    
+    @semistaticmethod
     def create_plot(self, data:ROOT.RooDataSet, pdf:ROOT.RooAbsPdf,
                     observable:Optional[ROOT.RooRealVar]=None,
                     plot_options:Optional[Dict]=None,
                     model_summary:Optional[Dict]=None,
-                    save_as:Optional[str]=None):
+                    save_plot_as:Optional[str]=None,
+                    save_data_as:Optional[str]=None):
         
         if observable is None:
             parameters = data.get()
             if len(parameters) > 1:
                 raise RuntimeError("only single-observable dataset is allowed")
             observable = parameters.first()
         
@@ -297,34 +331,22 @@
             "config"      : plot_options.get("config", None)
         }
         
         from quickstats.plots import PdfDistributionPlot
         plotter = PdfDistributionPlot.from_roofit_data(data, pdf, observable, **init_kwargs)
         
         if model_summary is not None:
-            value_fmt = plot_options["value_fmt"]
-            annotation_text = ""
-            if plot_options['show_params']:
-                param_data = model_summary["parameters"]
-                for param in param_data:
-                    value = value_fmt.format(param_data[param]["value"])
-                    if plot_options["show_error"]:
-                        error = value_fmt.format(param_data[param]["error"])
-                        annotation_text += f"{param} = {value} $\\pm$ {error}\n"
-                    else:
-                        annotation_text += f"{param} = {value}\n"
-                annotation_text += "\n"
-            if plot_options["show_stats"]:
-                stats_list = plot_options["stats_list"]
-                for stat in stats_list:
-                    if stat not in model_summary["stats"]:
-                        raise RuntimeError(f"invalid stats item: {stat}")
-                    value = value_fmt.format(model_summary["stats"][stat])
-                    annotation_text += f"{stat} = {value}\n"
-                annotation_text += "\n"
+            kwargs = {
+                "value_fmt"   : plot_options["value_fmt"],
+                "show_params" : plot_options['show_params'],
+                "show_stats"  : plot_options["show_stats"],
+                "show_error"  : plot_options["show_error"],
+                "stats_list"  : plot_options["stats_list"]
+            }
+            annotation_text = self.get_model_summary_text(model_summary, **kwargs)
             plotter.add_annotation(annotation_text)
         
         annotations = plot_options.get("annotations", None)
         if annotations is not None:
             if isinstance(annotations, dict):
                 plotter.add_annotation(**annotations)
             elif isinstance(annotations, list):
@@ -355,29 +377,35 @@
             
         draw_options = plot_options.get("draw_options", {})
 
         ax = plotter.draw(xlabel=xlabel, ylabel=ylabel, targets=["data", "pdf"],
                           comparison_options=comparison_options, **draw_options)
         
         import matplotlib.pyplot as plt
-        if save_as is not None:
-            plt.savefig(save_as, bbox_inches="tight")
+        if save_plot_as is not None:
+            plt.savefig(save_plot_as, bbox_inches="tight")
+        if save_data_as is not None:
+            from quickstats.utils.common_utils import NpEncoder
+            json.dump(plotter.collective_data, open(save_data_as, 'w'), cls=NpEncoder)
+            
         if in_notebook():
             plt.show()
         return ax
 
     def run(self, filename:str, tree_name:str, save_summary_as:Optional[str]=None, 
-            save_param_as:Optional[str]=None, save_plot_as:Optional[str]=None):
+            save_param_as:Optional[str]=None, save_plot_as:Optional[str]=None,
+            save_data_as:Optional[str]=None):
         summary = self._run(filename, tree_name, model_class=self.model_class, 
                             param_templates=self.param_templates,
                             fit_options=self.fit_options,
                             plot_options=self.plot_options,
                             save_summary_as=save_summary_as,
                             save_param_as=save_param_as,
-                            save_plot_as=save_plot_as)
+                            save_plot_as=save_plot_as,
+                            save_data_as=save_data_as)
         return summary
     
     @staticmethod
     def _get_iter_save_paths(filenames:List[str], save_paths:Optional[Union[List[str], str]]=None):
         # do not save
         if save_paths is None:
             return repeat(None)
```

### Comparing `quickstats-0.6.7.7/quickstats/components/modelling/model_source.py` & `quickstats-0.6.7.8/quickstats/components/modelling/model_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/modelling/parameter_templates.py` & `quickstats-0.6.7.8/quickstats/components/modelling/parameter_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/modelling/pdf_fit_tool.py` & `quickstats-0.6.7.8/quickstats/components/modelling/pdf_fit_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,16 +78,17 @@
     def get_observable(data:"ROOT.RooAbsData"):
         parameters = data.get()
         if len(parameters) > 1:
             raise RuntimeError("only single-observable fit is allowed")
         observable = parameters.first()
         return observable
         
-    def mle_fit(self, minos:bool=False, hesse:bool=True, sumw2:bool=True, strategy:int=1,
-                min_fit:int=2, max_fit:int=3, range_expand_rate:Optional[int]=None, print_level:int=-1):
+    def mle_fit(self, minos:bool=False, hesse:bool=True, sumw2:bool=True, asymptotic:bool=False,
+                strategy:int=1, min_fit:int=2, max_fit:int=3, range_expand_rate:Optional[int]=None,
+                print_level:int=-1):
         
         observable = self.get_observable(self.data)
         vmin = observable.getMin()
         vmax = observable.getMax()
         observable.setRange("fitRange", vmin, vmax)
         
         model_name = self.pdf.GetName()
@@ -97,16 +98,20 @@
         self.stdout.info(f"INFO: Begin model fitting...")
         self.stdout.info(f"      Model : ".rjust(20) + f"{model_name}")
         self.stdout.info(f"    Dataset : ".rjust(20) + f"{data_name}")
         self.stdout.info(f" Observable : ".rjust(20) + f"{obs_name}")
         
         fit_args = [ROOT.RooFit.Range("fitRange"), ROOT.RooFit.PrintLevel(print_level),
                     ROOT.RooFit.Minos(minos), ROOT.RooFit.Hesse(hesse),
-                    ROOT.RooFit.Save(), ROOT.RooFit.SumW2Error(sumw2),
-                    ROOT.RooFit.Strategy(strategy)]
+                    ROOT.RooFit.Save(), ROOT.RooFit.Strategy(strategy)]
+        
+        if asymptotic:
+            fit_args.append(ROOT.RooFit.AsymptoticError(True))
+        elif sumw2:
+            fit_args.append(ROOT.RooFit.SumW2Error(True))
 
         status_label = {
             True  : 'SUCCESS',
             False : 'FAIL'
         }
 
         for i in range(1, max_fit + 1):
```

### Comparing `quickstats-0.6.7.7/quickstats/components/modelling/tree_data_source.py` & `quickstats-0.6.7.8/quickstats/components/modelling/tree_data_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/nuisance_parameter_harmonizer.py` & `quickstats-0.6.7.8/quickstats/components/nuisance_parameter_harmonizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/nuisance_parameter_pull.py` & `quickstats-0.6.7.8/quickstats/components/nuisance_parameter_pull.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
             nll_commands.append(ROOT.RooFit.BatchMode(batch_mode))
         if hasattr(ROOT.RooFit, "IntegrateBins"):
             nll_commands.append(ROOT.RooFit.IntegrateBins(int_bin_precision))            
 
         minimize_options = {
             'minimizer_type'   : minimizer_type,
             'minimizer_algo'   : minimizer_algo,
-            'default_strategy' : strategy,
+            'strategy' : strategy,
             'optimize'         : optimize,
             'precision'        : precision,
             'eps'              : eps,
             'retry'            : retry,
             'max_calls'        : max_calls,
             'max_iters'        : max_iters,
         }
```

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/__init__.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_alias.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_alias.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 class RooProcAlias(RooProcRDFAction):
     
     def __init__(self, alias:str, column_name:str):
         super().__init__(alias=alias, column_name=column_name)
         
     @classmethod
     def parse(cls, main_text:str, block_text:Optional[str]=None):
-        result = re.search(r"^\s*(\w+)\s*=\s*([\w\.]+)\s*$", main_text)
+        result = re.search(r"^\s*(\w+)\s*=\s*([\w\.\${}]+)\s*$", main_text)
         if not result:
-            if re.search(r"^\s*(\w+)\s*=\s*([\w\.]+)", main_text):
-                raise RuntimeError(f"can not alias an expression, please use DEFINE instead")
+            if re.search(r"^\s*(\w+)\s*=\s*([\w\.\${}]+)", main_text):
+                raise RuntimeError(f'can not alias an expression ("{main_text}"), '
+                                   'please use DEFINE instead')
             raise RuntimeError(f"invalid expression {main_text}")
         alias = result.group(1)
         column_name = result.group(2)
         return cls(alias=alias, column_name=column_name)        
         
     def _execute(self, rdf:"ROOT.RDataFrame", **params):
         alias = params['alias']
```

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_as_numpy.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_as_numpy.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_base_action.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_base_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_declare.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_declare.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_define.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_define.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_export.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_export.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_filter.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_filter.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_global_variables.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_global_variables.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_hybrid_action.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_hybrid_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_if_defined.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_if_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_if_not_defined.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_if_not_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_load_frame.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_load_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_nested_action.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_nested_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_report.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_report.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_safe_alias.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_safe_alias.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 class RooProcSafeAlias(RooProcHybridAction):
     
     def __init__(self, alias:str, column_name:str):
         super().__init__(alias=alias, column_name=column_name)
         
     @classmethod
     def parse(cls, main_text:str, block_text:Optional[str]=None):
-        result = re.search(r"^\s*(\w+)\s*=\s*([\w\.]+)", main_text)
+        result = re.search(r"^\s*(\w+)\s*=\s*([\w\.\${}]+)\s*$", main_text)
         if not result:
+            if re.search(r"^\s*(\w+)\s*=\s*([\w\.\${}]+)", main_text):
+                raise RuntimeError(f'can not alias an expression ("{main_text}"), '
+                                   'please use DEFINE instead')
             raise RuntimeError(f"invalid expression {main_text}")
         alias = result.group(1)
         column_name = result.group(2)
         return cls(alias=alias, column_name=column_name)    
     
     def _execute(self, rdf:"ROOT.RDataFrame", processor:"quickstats.RooProcessor", **params):
         alias = params['alias']
```

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_save.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_save.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_save_frame.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_save_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_stat.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_stat.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/actions/rooproc_treename.py` & `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_treename.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/builtin_methods.py` & `quickstats-0.6.7.8/quickstats/components/processors/builtin_methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/roo_config_parser.py` & `quickstats-0.6.7.8/quickstats/components/processors/roo_config_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/processors/roo_processor.py` & `quickstats-0.6.7.8/quickstats/components/processors/roo_processor.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/pvalue_toys.py` & `quickstats-0.6.7.8/quickstats/components/pvalue_toys.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/roo_inspector.py` & `quickstats-0.6.7.8/quickstats/components/roo_inspector.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/root_object.py` & `quickstats-0.6.7.8/quickstats/components/root_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/toy_limit_calculator.py` & `quickstats-0.6.7.8/quickstats/components/toy_limit_calculator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/workspaces/__init__.py` & `quickstats-0.6.7.8/quickstats/components/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/workspaces/asimov_handler.py` & `quickstats-0.6.7.8/quickstats/components/workspaces/asimov_handler.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/workspaces/core_argument_sets.py` & `quickstats-0.6.7.8/quickstats/components/workspaces/core_argument_sets.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/workspaces/sample.py` & `quickstats-0.6.7.8/quickstats/components/workspaces/sample.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/workspaces/settings.py` & `quickstats-0.6.7.8/quickstats/components/workspaces/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,16 @@
 XS_PREFIX = "_xs"
 BR_PREFIX = "_br"
 EFFICIENCY_PREFIX = "_eff"
 ACCEPTANCE_PREFIX = "_A"
 CORRECTION_PREFIX = "_C"
 COMMON_SYST_DOMAIN_NAME = "_allproc_"
 
+COMBINED_PDF_NAME = "CombinedPdf"
+
 #model sources
 USERDEF_MODEL = "userdef"
 EXTERNAL_MODEL = "external"
 HISTOGRAM_MODEL = "histogram"
 
 #blinding
 RANGE_NAME_SB_LO = "SBLo"
```

### Comparing `quickstats-0.6.7.7/quickstats/components/workspaces/systematic.py` & `quickstats-0.6.7.8/quickstats/components/workspaces/systematic.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         obj._value_ = value
         obj.description = description
         obj.keyword = keyword
         return obj    
     
 class ConstraintType(DescriptiveEnum):
     LogN  = (0, "Lognormal constraint", CONSTR_LOGN, 1)
-    Asym  = (1, "Assymetric constraint", CONSTR_ASYM, 4)
+    Asym  = (1, "Asymmetric constraint", CONSTR_ASYM, 4)
     Gaus  = (2, "Gaussian constraint", CONSTR_GAUSSIAN, 0)
     DFD   = (3, "Double Fermi-Dirac", CONSTR_DFD, 0)
     Other = (4, "Unclassified constraint type", OTHER, -1)
     
     def __new__(cls, value:int, description:str, keyword:str, interp_code:int):
         obj = object.__new__(cls)
         obj._value_ = value
@@ -70,29 +70,29 @@
         if result is None:
             return SystematicType.Other
         return result
     
     def get_constr_type(self):
         result = ConstraintType.get_member_by_attribute("keyword", self.constr_term)
         if result is None:
-            return ConstraintType.Other
+            raise ValueError(f'unknown constraint type: {self.constr_term}')
         return result
     
     def is_common_domain(self):
         return self.domain == COMMON_SYST_DOMAIN_NAME
     
     def set_domain(self, domain:str):
         syst_type = self.get_syst_type()
         # systematics defined in the common domain
         if domain == self.common_domain():
             # if a process name is specified, use it as domain name and 
             # remove it from common systematic
             if self.process != "":
                 if syst_type == SystematicType.Shape:
-                    self.domain = f"{self.whereto}_{self.name}_{self.process}"
+                    self.domain = f"{self.whereto}_{self.process}"
                 else:
                     self.domain = self.process
             # otherwise consider it as common systematic
             else:
                 # for shape uncertainty, use NP name as domain
                 if syst_type == SystematicType.Shape:
                     self.domain = f"{self.whereto}_{self.name}"
@@ -112,15 +112,15 @@
             if self.process == "":
                 self.process = domain
                 if syst_type == SystematicType.Shape:
                     self.domain = f"{self.whereto}_{self.name}_{self.process}"
             else:
                 self.process = f"{domain}_{self.process}"
                 if syst_type == SystematicType.Shape:
-                    self.domain = f"{self.whereto}_{self.name}_{self.process}"
+                    self.domain = f"{self.whereto}_{self.process}"
         self.raw_domain = domain
         
     def set_magnitudes(self, values:Union[float, str, List[float], List[str]]):
         # for asymmetric uncertainty, we need to be careful with the relative sign between the two components
         # if both upper and lower uncertainties are numbers, the lower number will always be forced to have opposite sign of upper
         # if either uncertainty is implemented as formula, the neither component can bear sign. Users need to make sure the sign convention is consistent
         if not isinstance(values, list):
```

### Comparing `quickstats-0.6.7.7/quickstats/components/workspaces/systematics_domain.py` & `quickstats-0.6.7.8/quickstats/components/workspaces/systematics_domain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/workspaces/ws_comparer.py` & `quickstats-0.6.7.8/quickstats/components/workspaces/ws_comparer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/workspaces/ws_modifier_config.py` & `quickstats-0.6.7.8/quickstats/components/workspaces/ws_modifier_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/workspaces/xml_ws_base.py` & `quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/workspaces/xml_ws_builder_v1.py` & `quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_builder_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from quickstats.components import ExtendedModel
 from quickstats.utils.io import Verbosity
 from quickstats.utils.xml_tools import TXMLTree
 from quickstats.utils.common_utils import remove_list_duplicates, format_delimiter_enclosed_text
 from quickstats.maths.numerics import is_float, pretty_value
 
 from quickstats.components.workspaces import XMLWSBase, Sample, Systematic, AsimovHandler
+from .settings import *
     
 class XMLWSBuilder(XMLWSBase):
     
     EPSILON = 1e-6
     
     KEYWORDS = {
         # likelihood model
@@ -117,152 +118,157 @@
         elif data_storage_type == "composite":
             ROOT.RooAbsData.setDefaultStorageType(ROOT.RooAbsData.StorageType.Composite)            
         else:
             raise RuntimeError(f"unknown data storage type `{data_storage_type}`")
   
     def initialize(self, source:str):
         self.core_config = self.parse_core_xml(source)
-        self._print_core_xml_summary()
-        self.cat_config = {}
-        self.cat_ws = {}
-        self.datahists = {}
-        self.datasets = {}
+        self.update_paths()
+        self.reset()
+        self.set_data_storage_type(self.data_storage_type)
+        self.print_init_summary()
+        
+    def reset(self) -> None:
+        self.cat_config      = {}
+        self.cat_ws          = {}
+        self.datahists       = {}
+        self.datasets        = {}
         self.datasets_binned = {}
-        self.time_taken = 0.
+        self.time_taken      = 0.
         ws_name = self.core_config['workspace_name']
         mc_name = self.core_config['model_config_name']
-        self.set_data_storage_type(self.data_storage_type)
-        self.comb_ws = ROOT.RooWorkspace(ws_name)
+        self.comb_ws      = ROOT.RooWorkspace(ws_name)
         self.model_config = ROOT.RooStats.ModelConfig(mc_name, self.comb_ws)
+        
+    def update_paths(self) -> None:
+        self.path_manager.set_file("output", self.core_config["output_name"])
+        categories = []
+        for category, file in self.core_config['input_categories'].items():
+            self.path_manager.set_file(f"__Cat_{category}", file)
     
     def parse_core_xml(self, filename:str):
         self.stdout.info(f"INFO: Parsing file `{filename}`")
         # load xml file
         core_xml = TXMLTree.load_as_dict(filename)
-        # parse basic attributes
+        # parse core attributes
         attributes = core_xml['attrib']
-        content = {
+        core_config = {
             'base_dir'           : os.path.dirname(filename),
-            'workspace_name'     : attributes['WorkspaceName'],
-            'model_config_name'  : attributes['ModelConfigName'],
-            'dataset_name'       : attributes['DataName'],
-            'output_name'        : attributes['OutputFile'],
-            'do_blind'           : int(attributes.get('Blind', "0")),
-            'integrator'         : attributes.get('Integrator', ""),
+            'workspace_name'     : self._get_node_attrib(core_xml, 'WorkspaceName'),
+            'model_config_name'  : self._get_node_attrib(core_xml, 'ModelConfigName'),
+            'dataset_name'       : self._get_node_attrib(core_xml, 'DataName'),
+            'output_name'        : self._get_node_attrib(core_xml, 'OutputFile'),
+            'do_blind'           : self._get_node_attrib(core_xml, 'Blind',
+                                                         required=False, default=False, dtype="bool"),
+            'integrator'         : self._get_node_attrib(core_xml, 'Integrator',
+                                                         required=False, default=""),
             'poi_names'          : [],
-            'input_categories'   : [],
+            'input_categories'   : {},
             'asimov_definitions' : []
         }
-        if not content['output_name'].endswith(".root"):
-            content['output_name'] = os.path.splitext(content['output_name'])[0] + ".root"
+        
+        if not core_config['output_name'].endswith(".root"):
+            core_config['output_name'] = os.path.splitext(core_config['output_name'])[0] + ".root"
             self.stdout.warning('WARNING: Output file name does not contain ".root" postfix. '
                                 'Adding it to avoid confusion.')
         # parse child level attributes
         nodes = core_xml['children']
         for node in nodes:
             tag = node['tag']
             if tag == "Input":
-                input_filename = node['text']
-                content['input_categories'].append(input_filename)
+                file = node['text']
+                tree = TXMLTree(file=self.path_manager.get_relpath(file))
+                category = tree.root.get_attribute("Name")
+                if category in core_config['input_categories']:
+                    raise RuntimeError(f'duplicated category name: "{category}"')
+                core_config['input_categories'][category] = file
             elif tag == "POI":
                 poi_expr = node['text']
-                content['poi_names'] += poi_expr.split(",")
+                core_config['poi_names'] += poi_expr.split(",")
             elif tag == "Asimov":
                 definitions = node['attrib']
-                content['asimov_definitions'].append(definitions)
+                core_config['asimov_definitions'].append(definitions)
             else:
                 raise RuntimeError(f"unknown item `{tag}`")
-        return content
-        
-    def _print_core_xml_summary(self):
+        return core_config
+    
+    def print_init_summary(self) -> None:
         if not self.core_config:
             raise RuntimeError("core config not set")
-        self.stdout.info("=========================================================================")
+        self.stdout.info("="*74)
         self.stdout.info("Output file: ".rjust(20) + f"{self.core_config['output_name']}")
         self.stdout.info("Workspace name: ".rjust(20) + f"{self.core_config['workspace_name']}")
         self.stdout.info("ModelConfig name: ".rjust(20) + f"{self.core_config['model_config_name']}")
         self.stdout.info("Dataset name: ".rjust(20) + f"{self.core_config['dataset_name']}")
         self.stdout.info("Blind analysis: ".rjust(20) + ("True" if self.core_config['do_blind'] else "False"))
         self.stdout.info("POIs: ".rjust(20) + ", ".join(self.core_config['poi_names']))
         self.stdout.info("")
         self.stdout.info("Categories to be included:")
         input_categories = self.core_config['input_categories']
-        for i,input_category in enumerate(input_categories):
+        for i, input_category in enumerate(input_categories.values()):
             self.stdout.info(f"XML file {i}: ".rjust(20) + f"{input_category}")
         asimov_definitions = self.core_config['asimov_definitions']
         if asimov_definitions:
             self.stdout.info("")
             self.stdout.info("The following asimov dataset(s) will be generated:")
             for asimov_def in asimov_definitions:
-                is_gen_asimov = self.KEYWORDS['gen_asimov'] in asimov_def['Action']
+                is_gen_asimov = GEN_ASIMOV_ACTION in asimov_def['Action']
                 if is_gen_asimov:
                     asimov_name = asimov_def['Name']
                     self.stdout.info(f"\t{asimov_name}")
-        self.stdout.info("=========================================================================")
+        self.stdout.info("="*74)
+        
+    def get_pdf_name(self, category:str):
+        return f"{FINAL_PDF_NAME}_{category}"
     
     def generate_workspace(self):
         t0 = time.time()
         channel_list = ROOT.RooCategory("channellist", "channellist")
-        combined_pdf = ROOT.RooSimultaneous("CombinedPdf", "", channel_list)
+        combined_pdf = ROOT.RooSimultaneous(COMBINED_PDF_NAME, "", channel_list)
         
-        pois           = ROOT.RooArgSet()
-        nuis           = ROOT.RooArgSet()
-        globobs        = ROOT.RooArgSet()
-        constraints    = ROOT.RooArgSet()
-        observables    = ROOT.RooArgSet()
+        obs          = ROOT.RooArgSet()
+        pois         = ROOT.RooArgSet()
+        nuis         = ROOT.RooArgSet()
+        globs        = ROOT.RooArgSet()
+        constraints  = ROOT.RooArgSet()
         
-        self.cat_config      = {}
-        self.cat_ws          = {}
-        self.datahists       = {}
-        self.datasets        = {}
-        self.datasets_binned = {}
-        self.time_taken      = 0.
+        self.reset()
         
-        inputfiles = self.core_config['input_categories']
+        categories = list(self.core_config['input_categories'])
         
-        for i, inputfile in enumerate(inputfiles):
-            ws_name = f"wchannel_{i}"
-            ws_i = self.generate_single_category(inputfile, ws_name)
-            
-            category = self.current_category
-            self.cat_ws[category] = ws_i
+        for category in categories:
+            ws_cat = self.generate_single_category(category)
+            self.cat_ws[category] = ws_cat
             
+            # import channel pdf
             channel_list.defineType(category)
-            pdf_name = f"{self.KEYWORDS['final_pdf_name']}_{category}"
-            pdf_i = ws_i.pdf(pdf_name)
-            if not pdf_i:
+            pdf_name = self.get_pdf_name(category)
+            pdf_cat = ws_cat.pdf(pdf_name)
+            if not pdf_cat:
                 raise RuntimeError(f"model pdf `{pdf_name}` for the category "
-                                   f"`{category}` not defined")
-            combined_pdf.addPdf(pdf_i, category)
-            
-            nuis.add(ws_i.set("nuisanceParameters"), True)
-            globobs.add(ws_i.set("globalObservables"), True)
-            observables.add(ws_i.set("Observables"), True)
-            pois.add(ws_i.set("POI"), True)
+                                   f"`{category}` is not defined")
+            combined_pdf.addPdf(pdf_cat, category)
             
+            obs.add(ws_cat.set(OBS_SET), True)
+            pois.add(ws_cat.set(POI_SET), True)
+            nuis.add(ws_cat.set(NUIS_SET), True)
+            globs.add(ws_cat.set(GLOB_SET), True)
             if self.debug_mode:
                 ws_i.Print()
+                
         #observables.add(channel_list)
         self.import_object(self.comb_ws, combined_pdf)
         
-        self.comb_ws.defineSet("nuisanceParameters", nuis)
-        self.comb_ws.defineSet("globalObservables", globobs)
-        self.comb_ws.defineSet("Observables", observables)        
-        self.comb_ws.defineSet("POI", pois)
-        
-        self.model_config.SetPdf(self.comb_ws.pdf("CombinedPdf"))
-        self.model_config.SetObservables(self.comb_ws.set("Observables"))
-        self.model_config.SetParametersOfInterest(self.comb_ws.set("POI"))
-        self.model_config.SetNuisanceParameters(self.comb_ws.set("nuisanceParameters"))
-        self.model_config.SetGlobalObservables(self.comb_ws.set("globalObservables"))
-        self.import_object(self.comb_ws, self.model_config, silent=False)
+        # implement model config
+        self.implement_model_config_and_sets(self.comb_ws, self.model_config,
+                                             obs, pois, nuis, globs)
         
         weight_var = ROOT.RooRealVar("wt", "wt", 1)
         args = ROOT.RooArgSet()
-        args.add(observables)
+        args.add(obs)
         args.add(weight_var)
         
         dataset_map = ExtendedModel.get_dataset_map(self.datasets)
         dataset_binned_map = ExtendedModel.get_dataset_map(self.datasets_binned)
         
         dataset_name = self.core_config['dataset_name']
         obs_data = ROOT.RooDataSet(dataset_name, "Combined data", args,
@@ -296,14 +302,30 @@
         if not os.path.exists(output_dir):
             os.makedirs(output_dir)
         self.comb_ws.writeToFile(output_path, True)
         
         t1 = time.time()
         self.time_taken += (t1 - t0)
         self.print_final_summary()
+
+    def implement_model_config_and_sets(self, ws:"ROOT.RooWorkspace",
+                                        mc:"ROOT.RooStats.ModelConfig",
+                                        obs:ROOT.RooArgSet, pois:ROOT.RooArgSet,
+                                        nuis:ROOT.RooArgSet, globs:ROOT.RooArgSet):
+        ws.defineSet(OBS_SET, obs)        
+        ws.defineSet(POI_SET, pois)
+        ws.defineSet(NUIS_SET, nuis)
+        ws.defineSet(GLOB_SET, globs)
+        
+        mc.SetPdf(ws.pdf(COMBINED_PDF_NAME))
+        mc.SetObservables(ws.set(OBS_SET))
+        mc.SetParametersOfInterest(ws.set(POI_SET))
+        mc.SetNuisanceParameters(ws.set(NUIS_SET))
+        mc.SetGlobalObservables(ws.set(GLOB_SET))
+        self.import_object(ws, mc, silent=False)
     
     def print_final_summary(self):
         ws_name = self.comb_ws.GetName()
         model = ExtendedModel(self.comb_ws, data_name=self.core_config['dataset_name'], verbosity="WARNING")
         pdf = model.pdf
         cat = pdf.indexCat()
         n_cat = len(cat)
@@ -377,87 +399,93 @@
         return f"{range_name_SBLo},{range_name_SBHi}"
     
     def get_blind_range_name(self):
         """Get blind range name that are excluded from the fit range
         """
         return self.KEYWORDS['blind']        
         
-    def generate_single_category(self, filename:str, workspace_name:str):
-        ws = ROOT.RooWorkspace(workspace_name)
+    def generate_single_category(self, category:str):
+        """
+        Generate workspace for a single category.
+        
+        Parameters
+        ----------
+        category: str
+            Name of the category.
+        """
+        ws             = ROOT.RooWorkspace(f"__Cat_{category}")
         nuis           = ROOT.RooArgSet()
         globobs        = ROOT.RooArgSet()
         constraints    = ROOT.RooArgSet()
         expected       = ROOT.RooArgSet()
         expected_shape = ROOT.RooArgSet()
         expected_map   = {}
-        # load xml file
-        filepath = self.get_relpath(filename)
+        # load category xml file
+        filepath = self.path_manager.get_file(f"__Cat_{category}", check_exist=True)
         cat_xml = TXMLTree.load_as_dict(filepath)
-        attributes = cat_xml['attrib']
-        nodes = cat_xml['children']
-        category_name = attributes['Name']
-        if category_name in self.cat_config:
-            raise RuntimeError(f'duplicated category name: "{category_name}"')
             
-        title_str = format_delimiter_enclosed_text(f"Category {category_name}", "-")
+        title_str = format_delimiter_enclosed_text(f"Category {category}", "-")
         self.stdout.info(title_str)
         
-        self.current_category = category_name
-        category_type = attributes['Type'].lower()
-        luminosity = float(self._get_node_attrib(cat_xml, "Lumi", False, "-1"))
+        self.active_category = category
+        category_type = self._get_node_attrib(cat_xml, 'Type').lower()
+        luminosity = self._get_node_attrib(cat_xml, "Lumi", required=False,
+                                           default="-1", dtype="float")
         
-        self.cat_config[category_name] = {
-            'input_file': filename,
+        self.cat_config[category] = {
+            'input_file': filepath,
             'category_type': category_type,
             'luminosity': luminosity,
             'observable': {
                 'name': ""
             }
         }
-        ws_factory = ROOT.RooWorkspace(f"factory_{category_name}")
+        ws_factory = ROOT.RooWorkspace(f"factory_{category}")
         
         # define lumi
         if luminosity > 0:
             lumi_expr = f"{self.KEYWORDS['lumi_name']}[{luminosity}]"
             self.import_expression(ws_factory, lumi_expr)
 
+        nodes = cat_xml['children']
+        
         # define dataset
-        data_node = self.fetch_node(nodes, "Data", xml_filename=filename, xml_type="channel",
+        data_node = self.fetch_node(nodes, "Data", xml_filename=filepath, xml_type="channel",
                                     allow_multiple=False, allow_missing=False)
         self.read_data_node(data_node, ws_factory)
         
         # define correlation terms        
-        correlate_node = self.fetch_node(nodes, "Correlate", xml_filename=filename, xml_type="channel",
+        correlate_node = self.fetch_node(nodes, "Correlate", xml_filename=filepath, xml_type="channel",
                                          allow_multiple=False, allow_missing=True)
         self.read_correlate_node(correlate_node)
         
-        self.cat_config[category_name]['items_highpriority'] = []
-        self.cat_config[category_name]['items_lowpriority'] = []
-        self.cat_config[category_name]['systematics'] = {}
-        self.cat_config[category_name]['samples'] = []
+        self.cat_config[category]['items_highpriority'] = []
+        self.cat_config[category]['items_lowpriority'] = []
+        self.cat_config[category]['systematics'] = {}
+        self.cat_config[category]['samples'] = []
 
         remained_nodes = [node for node in nodes if node['tag'] not in ["Data", "Correlate"]]
         self.read_channel_xml_nodes(remained_nodes, ws_factory)
  
         self._fix_item_priority()
-        items_highpriority  = self.cat_config[category_name]['items_highpriority']
-        items_lowpriority   = self.cat_config[category_name]['items_lowpriority']
+        items_highpriority  = self.cat_config[category]['items_highpriority']
+        items_lowpriority   = self.cat_config[category]['items_lowpriority']
         
         self.stdout.debug("REGTEST: High priority items:")
         for item in items_highpriority:
             self.stdout.debug(f"\t{item}")
         self.stdout.debug("REGTEST: Low priority items:")
         for item in items_lowpriority:
             self.stdout.debug(f"\t{item}")
         # first implement high priority items: common variables 
         # and functions not involving systematic uncertainties
         self.import_expressions(ws_factory, items_highpriority)
 
-        systematics = self.cat_config[category_name]['systematics']
-        samples = self.cat_config[category_name]['samples']
+        systematics = self.cat_config[category]['systematics']
+        samples = self.cat_config[category]['samples']
         # secondly implement systematics and import them into the workspace
         for domain in systematics:
             syst_list = systematics[domain]
             if domain == self.KEYWORDS['allproc']:
                 resp_collection_yield = expected
             else:
                 sample = [s for s in samples if s.is_equal(domain)]
@@ -521,15 +549,15 @@
                         else:
                             raise RuntimeError(f"unknwon systematic group `{syst_group}` in "
                                                f"Sample `{sample.process}`")
             norm_comp_str = ",".join(norm_factor_components)
             norm_str = f"prod::{sample.norm_name}({norm_comp_str})"
             self.import_expression(ws_factory, norm_str)
             proc_yield = ws_factory.function(sample.norm_name).getVal()
-            self.stdout.info(f"REGTEST: Yield for category `{category_name}` "
+            self.stdout.info(f"REGTEST: Yield for category `{category}` "
                              f"process `{sample.process}`: {proc_yield}")
             if self.debug_mode:
                 ws_factory.Print()
             
             self.get_model(ws_factory, sample, nuis, constraints, globobs)
         
         if self.debug_mode:
@@ -549,16 +577,16 @@
         # keep track of correlated variables
         correlated_terms = self.get_correlated_terms(ws_factory, nuis)
         correlated_str = ",".join(correlated_terms)
         
         self.stdout.debug(f"REGTEST: The following variables will not be renamed: {','.join(correlated_terms)}")
         # import pdf to new workspace, rename objects as appropriate
         self.import_object(ws, ws_factory.pdf(self.KEYWORDS['sum_pdf_name']),
-                           ROOT.RooFit.RenameAllNodes(category_name),
-                           ROOT.RooFit.RenameAllVariablesExcept(category_name, correlated_str))
+                           ROOT.RooFit.RenameAllNodes(category),
+                           ROOT.RooFit.RenameAllVariablesExcept(category, correlated_str))
         
         # import constraint terms
         self.attach_constraints(ws, constraints)
         
         obs = self.get_observable(ws)
         # define variable sets
         poi_names = self.get_poi_names()
@@ -576,31 +604,31 @@
     
         # prepare binned data
         dataset_binned_name = self.KEYWORDS['obs_ds_name'] + "binned"
         dataset_binned = dataset.Clone(dataset_binned_name)
         
         # consider that blinded analysis the number of bins will reduce
         do_blind = self.core_config['do_blind']
-        blind_range = self.cat_config[category_name]['dataset']['blind_range']
+        blind_range = self.cat_config[category]['dataset']['blind_range']
         blind_sf = 1
         if do_blind and blind_range:
             blind_sf = 1 - (blind_range[1] - blind_range[0]) / (obs.getMax() - obs.getMin())
         if (dataset.numEntries() > (obs.numBins() * blind_sf)):
             dataset_binned = ROOT.RooDataSet(dataset_binned_name, dataset_binned_name,
                                              ROOT.RooArgSet(obs, weight_var),
                                              ROOT.RooFit.WeightVar(weight_var))
             self._fill_dataset_from_hist(dataset_binned, datahist, obs, weight_var)
         num_events = pretty_value(dataset.sumEntries(), 5)
         self.stdout.info(f"REGTEST: Number of data events: {num_events}")
         self.import_object(ws, dataset)
         self.import_object(ws, dataset_binned)
         
-        self.datahists[category_name]       = datahist
-        self.datasets[category_name]        = dataset
-        self.datasets_binned[category_name] = dataset_binned
+        self.datahists[category]       = datahist
+        self.datasets[category]        = dataset
+        self.datasets_binned[category] = dataset_binned
         
         return ws
 
     @staticmethod
     def _define_set(ws:ROOT.RooWorkspace, arg_set:Union[ROOT.RooArgSet, List[str]], name:str):
         proper_set = ROOT.RooArgSet()
         for var in arg_set:
@@ -610,15 +638,15 @@
             else:
                 ws_var = ws.var(var)
             if (ws_var):
                 proper_set.add(ws_var)
         ws.defineSet(name, proper_set)
         
     def generate_dataset(self, obs:ROOT.RooRealVar, weight_var:ROOT.RooRealVar):
-        category_name = self.current_category
+        category_name = self.active_category
         cat_config = self.get_active_category_config()
         data_config = cat_config['dataset']
         obs_min = obs.getMin()
         obs_max = obs.getMax()
         n_bins = obs.getBins()
         data_scale = data_config['scale_data']
         data_name = self.KEYWORDS['obs_ds_name']
@@ -676,14 +704,16 @@
                 raise RuntimeError(f"Binned ({n_event_binned}) and unbinned ({n_event}) "
                                    f"datasets have different number of entries in "
                                    f"category {category_name}")
         else:
             if filetype == self.KEYWORDS['ascii']:
                 filepath = self.get_relpath(filename)
                 dataset_tmp = ROOT.RooDataSet.read(filepath, ROOT.RooArgList(obs))
+                if not dataset_tmp:
+                    raise FileNotFoundError(f"data file {filepath} does not exist")
             else:
                 cut      = data_config['cut']
                 treename = data_config['treename']
                 varname  = data_config['varname']
                 chain, _ = self.get_chain_and_branch(filepath, treename, varname, cut)
                 x_tree = ROOT.RooRealVar(varname, varname, obs.getMin(), obs.getMax())
                 _dataset_name = f"{self.KEYWORDS['obs_ds_name']}_tmp"
@@ -709,15 +739,15 @@
         # inject ghost
         inject_ghost = data_config['inject_ghost']
         if inject_ghost:
             self.release_ghost(dataset, datahist, obs, weight_var, self.EPSILON / 1000.)
         return dataset, datahist
     
     def _rebin_hist_to_obs(self, h:ROOT.TH1, obs:ROOT.RooRealVar):
-        category = self.current_category
+        category = self.active_category
         bin_low, bin_high, n_bins = self._find_bins_wrt_obs(h, obs)
         obs_n_bins = obs.getBins()
         if n_bins != obs_n_bins:
             if n_bins == 0:
                 histname = h.GetName()
                 raise RuntimeError(f"input data histogram `{histname}` in category "
                                    f"{category} has a computed number of bins equal "
@@ -803,15 +833,15 @@
                 obs.setVal(bin_center)
                 weight_var.setVal(ghost_weight)
                 dataset.add(ROOT.RooArgSet(obs, weight_var), ghost_weight)
                 # also put the ghost weight in the histograms
                 datahist.SetBinContent(i, ghost_weight)
                 
     def attach_constraints(self, ws:ROOT.RooWorkspace, constraints:ROOT.RooArgSet):
-        category_name = self.current_category
+        category_name = self.active_category
         self.stdout.debug(f"REGTEST: Attaching contraint pdfs to workspace for the category {category_name}")
         sum_pdf_name = f"{self.KEYWORDS['sum_pdf_name']}_{category_name}"
         final_pdf_name = f"{self.KEYWORDS['final_pdf_name']}_{category_name}"
         remove_set = ROOT.RooArgSet()
         pdf = ws.pdf(sum_pdf_name)
         if not pdf:
             raise RuntimeError(f"sum pdf `{sum_pdf_name}` not defined")
@@ -865,15 +895,15 @@
         return obs
 
     def implement_blind_range(self, ws:ROOT.RooWorkspace):
         # range_name = "" : all blinded
         # range_name = None: no blinding
         # otherwise partially blinded
         cat_config = self.get_active_category_config()
-        category_name = self.current_category
+        category_name = self.active_category
         observable_name = cat_config['observable']['name']
         observable_range = [cat_config['observable']['min'], cat_config['observable']['max']]
         obs = ws.var(observable_name)
         if not obs:
             raise RuntimeError("observable variable not initialized")        
         # now handle blinding if needed
         blind_range = cat_config['dataset']['blind_range']
@@ -961,23 +991,23 @@
         elif (":" in expr) and not ("::" in expr):
             raise RuntimeError(f"syntax error for the expression `{expr}`: missing colon pair")
         else:
             object_type = "defined"
             object_name = expr
         return object_name, object_type
             
-    def import_uncert_expr(self, ws:ROOT.RooWorkspace, expr:str, var_name:str, prefix:str):
+    def import_uncert_expr(self, ws:ROOT.RooWorkspace, expr:str, var_name:Optional[str]=None, prefix:Optional[str]=None):
         if is_float(expr):
             new_expr = f"{prefix}{var_name}[{expr}]"
             return self.import_expression(ws, new_expr)
         else:
             return self.import_expression(ws, expr)
 
     def _translate_keyword(self, expr:str):
-        category_name = self.current_category
+        category_name = self.active_category
         observable_name = self.cat_config[category_name]['observable']['name']
         expr = expr.replace(self.KEYWORDS['response'], 
                             self.KEYWORDS['response_prefix'] + \
                             self.KEYWORDS['shape'] + "_")
         expr = expr.replace(self.KEYWORDS['observable'],
                             observable_name)
         expr = expr.replace(self.KEYWORDS['category'],
@@ -1024,27 +1054,27 @@
         return chain, branch
     
     def get_histogram(self, filename:str, histname:str, check_only:bool=False):
         filepath = self.get_relpath(filename)
         if not os.path.exists(filepath):
             raise FileNotFoundError(f"input data file `{filepath}` not found")
         f = ROOT.TFile(filepath)
-        category_name = self.current_category
+        category_name = self.active_category
         data_config = self.cat_config[category_name]['dataset']
         histname = data_config['histname']
         histogram = f.Get(histname)
         if not isinstance(histogram, ROOT.TH1):
             raise RuntimeError(f"no TH1 named `{histanme}` found in data file `{filepath}`")
         if check_only:
             return None
         histogram.SetDirectory(0)        
         return histogram
     
     def data_file_sanity_check(self):
-        category_name = self.current_category
+        category_name = self.active_category
         category_type = self.cat_config[category_name]['category_type']
         data_config = self.cat_config[category_name]['dataset']
         filename = data_config['filename']    
         if category_type == self.KEYWORDS['counting']:
             if (filename != "") and (self.check_file_exist(filename)):
                 raise FileNotFoundError(f"input data file `{filepath}` not found")
             if (filename == "") and (data_config.get("num_data", -1) < 0):
@@ -1068,15 +1098,15 @@
         elif (len(target_node) == 0) and (not allow_missing):
             raise RuntimError(f"No `{tag}` node found in {xml_type} XML file `{xml_filename}`")
         elif (len(target_node) == 1) and (not allow_multiple):
             target_node = target_node[0]
         return target_node
     
     def get_active_category_config(self):
-        category_name = self.current_category
+        category_name = self.active_category
         if category_name not in self.cat_config:
             raise RuntimeError(f"no config info found for the category `{category_name}`")
         cat_config = self.cat_config[category_name]
         return cat_config
         
     def read_systematics_node(self, node:Dict, domain:str):
         cat_config = self.get_active_category_config()
@@ -1247,15 +1277,16 @@
                 data_config['histname'] = self._translate_node_attrib(node, ["HistName", "HistoName"])
             else:
                 data_config['treename'] = self._translate_node_attrib(node, "TreeName")
                 data_config['varname'] = self._translate_node_attrib(node, "VarName")
                 data_config['cut'] = self._translate_node_attrib(node, "Cut", "",
                                                                  required=False,
                                                                  default="")
-        inject_ghost = self._get_node_attrib(node, "InjectGhost", False, "0", dtype="int")
+        inject_ghost = self._get_node_attrib(node, "InjectGhost", required=False,
+                                             default=False, dtype="bool")
         data_config['inject_ghost'] = inject_ghost
         if (is_counting and data_filename == ""):
             data_config['num_data'] = self._get_node_attrib(node, "NumData")
         else:
             data_config['num_data'] = -1
         data_config['scale_data'] = self._get_node_attrib(node, "ScaleData", False, "1", dtype="float")
         blind_range = self._get_node_attrib(node, "BlindRange", False, None)
@@ -1294,15 +1325,16 @@
         syst_groups = self._translate_node_attrib(node, "ImportSyst", sample.process,
                                                   required=False, default=self.KEYWORDS['self'])
         syst_groups = [s for s in syst_groups.split(",") if s != sample.process]
         syst_groups = remove_list_duplicates(syst_groups)
         sample.syst_groups = syst_groups
         
         if cat_config['luminosity'] > 0:
-            is_multiply_lumi = self._get_node_attrib(node, "MultiplyLumi", False, "1", dtype="int")
+            is_multiply_lumi = self._get_node_attrib(node, "MultiplyLumi", required=False,
+                                                     default=1, dtype="bool")
         else:
             is_multiply_lumi = 0
         
         # assemble the yield central value
         if is_multiply_lumi:
             sample.norm_factors.append(self.KEYWORDS['lumi_name'])        
         
@@ -1334,29 +1366,29 @@
             name = node['tag']
             if name == "Systematic":
                 self.read_systematics_node(node, sample.process)
             elif name == "NormFactor":
                 self.read_sample_factor_node(node, sample, "norm")
             elif name == "ShapeFactor":
                 self.read_sample_factor_node(node, sample, "shape")
-            elif name == "ImportItems":
+            elif name in ["ImportItems", "IncludeSysts"]:
                 self.read_sample_import_node(node, sample)
             else:
                 raise RuntimeError(f"unsupported node `{name}`")        
     
     def read_channel_xml_nodes(self, nodes:List, ws:ROOT.RooWorkspace):
         for node in nodes:
             name = node['tag']
             if name == "Item":
                 self.read_item_node(node)
             elif name == "Systematic":
                 self.read_systematics_node(node, self.KEYWORDS['allproc'])
             elif name == "Sample":
                 self.read_sample_node(node)
-            elif name == "ImportItems":
+            elif name in ["ImportItems", "IncludeSysts"]:
                 self.read_channel_import_node(node, ws)
             else:
                 raise RuntimeError(f"unsupported node `{name}`")
     def make_np(self, ws:ROOT.RooWorkspace, syst:Systematic, nuis:ROOT.RooArgSet,
                 constraint:ROOT.RooArgSet, globobs:ROOT.RooArgSet, expected:ROOT.RooArgSet):
         var_name = f"{syst.whereto}_{syst.name}"
         if syst.domain != self.KEYWORDS['allproc']:
@@ -1441,16 +1473,17 @@
         self.stdout.debug(f"REGTEST: Finished implementing systematic {syst.name}")
     
     def get_model(self, ws:ROOT.RooWorkspace, sample:Sample, nuis:ROOT.RooArgSet,
                   constraints:ROOT.RooArgSet, globobs:ROOT.RooArgSet):
         self.stdout.debug("REGTEST: Getting model")
         tag_name = sample.get_tag_name()
         sample.model_name = self.KEYWORDS['pdf_prefix'] + tag_name
-        
+
         if ws.pdf(sample.model_name):
+            is_shared_pdf = sample.share_pdf_group != ""
             if is_shared_pdf:
                 # use shared pdf
                 self.stdout.debug(f"REGTEST: PDF {sample.model_name} has been created in the workpace.")
                 return None
             else:
                 raise RuntimeError(f"PDF {sample.model_name} already exists but the user asks to create it again")
         self.stdout.debug(sample.model_name)
@@ -1680,15 +1713,15 @@
                 nuis.add(var)
                 var_name = var.GetName()
                 self.stdout.info(f"REGTEST: Adding {var_name} to the nuisance parameter set")
 
         num_float = len(float_set)
         if num_float < num_np:
             self.stdout.warning(f"WARNING: There supposed to be {num_poi + num_np} free parameters, "
-                                f"but only seen {num_float} in the category {self.current_category}. "
+                                f"but only seen {num_float} in the category {self.active_category}. "
                                 f"This is in principle not an issue, but please make sure you "
                                 f"understand what you are doing")
             if self.debug_mode:
                 self.stdout.debug("REGTEST: All free parameters: ")
                 float_set.Print()
                 self.stdout.debug("REGTEST: All nuisance parameters: ")
                 nuis.Print()
```

### Comparing `quickstats-0.6.7.7/quickstats/components/workspaces/xml_ws_builder_v2.py` & `quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_builder_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         self.stdout.info("Blind analysis: ".rjust(20) + ("True" if self.core_config['do_blind'] else "False"))
         self.stdout.info("Generate hist data: ".rjust(20) + ("True" if self.core_config['generate_hist_data'] else "False"))
         self.stdout.info("Scale lumi: ".rjust(20) + f"{self.core_config['scale_lumi']}")
         self.stdout.info("POIs: ".rjust(20) + ", ".join(self.core_config['poi_names']))
         self.stdout.info("")
         self.stdout.info("Categories to be included:")
         input_categories = self.core_config['input_categories']
-        for i,input_category in enumerate(input_categories.values()):
+        for i, input_category in enumerate(input_categories.values()):
             self.stdout.info(f"XML file {i}: ".rjust(20) + f"{input_category}")
         asimov_definitions = self.core_config['asimov_definitions']
         if asimov_definitions:
             self.stdout.info("")
             self.stdout.info("The following asimov dataset(s) will be generated:")
             for asimov_def in asimov_definitions:
                 is_gen_asimov = GEN_ASIMOV_ACTION in asimov_def['Action']
@@ -454,14 +454,17 @@
             # common systematics: only add if exist
             for syst_domain in sample.syst_domains:
                 if syst_domain in resp_func_map:
                     norm_factor_components.append(resp_func_map[syst_domain])
                 # sample without systematics
                 elif sample.process == syst_domain:
                     continue
+                # no common systematics but included :common: in ImportSyst
+                elif syst_domain == COMMON_SYST_DOMAIN_NAME:
+                    continue
                 else:
                     raise RuntimeError(f"unknown systematic domain {syst_domain} in sample {sample.process}")
             norm_factor_components_str = ",".join(norm_factor_components)
             norm_factor_expr = f"prod::{sample.norm_name}({norm_factor_components_str})"
             self.import_expression(ws, norm_factor_expr)
             proc_yield = ws.function(sample.norm_name).getVal()
             self.stdout.info(f'INFO: Yield for category "{category}" '
@@ -484,16 +487,16 @@
                 nuis_expr = f"{syst.name}[0, -5, 5]"
                 nuis_name = self.import_expression(ws, nuis_expr)
                 nuis = ws.var(nuis_name)
                 uncert_hi_expr = syst.get_uncert_hi_expr()
                 uncert_lo_expr = syst.get_uncert_lo_expr()
                 uncert_hi_name = self.import_expression(ws, uncert_hi_expr)
                 uncert_lo_name = self.import_expression(ws, uncert_lo_expr)
-                uncert_hi = ws.var(uncert_hi_name)
-                uncert_lo = ws.var(uncert_lo_name)
+                uncert_hi = ws.obj(uncert_hi_name)
+                uncert_lo = ws.obj(uncert_lo_name)
                 syst_domain.add_item(nuis, syst.nominal, uncert_hi, uncert_lo,
                                      syst.get_interp_code(), syst.constr_term)
             self.build_response_function(ws, syst_domain)
         
     def generate_dataset(self, obs:ROOT.RooRealVar, weight_var:ROOT.RooRealVar):
         category_name = self.active_category
         cat_config = self.get_active_category_config()
@@ -609,14 +612,16 @@
             assert (data.ndim == 2) and (data.shape[1] == 2)
             for data_i in data:
                 obs.setVal(data_i[0])
                 weight.setVal(data_i[1])
                 dataset.add(ROOT.RooArgSet(obs, weight), weight)
         else:
             dataset = ROOT.RooDataSet.read(file, ROOT.RooArgList(obs))
+            if not dataset:
+                raise FileNotFoundError(f"data file {file} does not exist")
         return dataset    
         
     def release_ghost(self, dataset:ROOT.RooDataSet, datahist:ROOT.RooDataHist,
                       obs:ROOT.RooRealVar, weight_var:ROOT.RooRealVar, ghost_weight:float):
         do_blind = self.core_config['do_blind']
         cat_config = self.get_active_category_config()
         blind_range = cat_config['dataset']['blind_range']
@@ -1045,15 +1050,16 @@
         # reading from root ntuples
         else:
             data_config['treename'] = self._translate_node_attrib(node, "TreeName")
             data_config['varname'] = self._translate_node_attrib(node, "VarName")
             data_config['cut'] = self._translate_node_attrib(node, "Cut", "",
                                                              required=False, default="")
 
-        inject_ghost = self._get_node_attrib(node, "InjectGhost", required=False, default=0, dtype="int")
+        inject_ghost = self._get_node_attrib(node, "InjectGhost", required=False,
+                                             default=False, dtype="bool")
         data_config['inject_ghost'] = inject_ghost
         if (is_counting and data_filename == ""):
             data_config['num_data'] = self._get_node_attrib(node, "NumData", dtype="int")
         else:
             data_config['num_data'] = -1
         data_config['scale_data'] = self._get_node_attrib(node, "ScaleData",
                                                           required=False, default=1, dtype="float")
@@ -1099,16 +1105,16 @@
         else:
             syst_domains = syst_domains.split(",")
         sample.set_syst_domains(syst_domains)
         
         # assemble the yield central value
         
         if cat_config['luminosity'] > 0:
-            multiply_lumi = self._get_node_attrib(node, "MultiplyLumi",
-                                                  required=False, default=1, dtype="int")
+            multiply_lumi = self._get_node_attrib(node, "MultiplyLumi", required=False,
+                                                  default=1, dtype="bool")
             if multiply_lumi:
                 sample.norm_factors.append(LUMI_NAME)
 
         norm_factor_names = {
             'norm': ('Norm', NORM_PREFIX),
             'xs': ('XSection', XS_PREFIX),
             'br': ('BR', BR_PREFIX),
@@ -1134,29 +1140,29 @@
     def read_sample_subnode(self, nodes:List, sample:Sample):
         for node in nodes:
             name = node['tag']
             if name == "Systematic":
                 self.read_systematics_node(node, sample.process)
             elif SampleFactorType.has_member(name):
                 self.read_sample_factor_node(node, sample)
-            elif name == "ImportItems":
+            elif name in ["ImportItems", "IncludeSysts"]:
                 self.read_sample_import_node(node, sample)
             else:
                 raise RuntimeError(f"unsupported node `{name}`")        
     
     def read_channel_xml_nodes(self, nodes:List, ws:ROOT.RooWorkspace):
         for node in nodes:
             name = node['tag']
             if name == "Item":
                 self.read_item_node(node)
             elif name == "Systematic":
                 self.read_systematics_node(node, domain=Systematic.default_domain())
             elif name == "Sample":
                 self.read_sample_node(node)
-            elif name == "ImportItems":
+            elif name in ["ImportItems", "IncludeSysts"]:
                 self.read_channel_import_node(node, ws)
             else:
                 raise RuntimeError(f"unsupported node `{name}`")
                 
     def build_response_function(self, ws:ROOT.RooWorkspace, syst_domain:SystematicsDomain):
         cat_config = self.get_active_category_config()
         core_argsets = cat_config['core_argsets']
@@ -1432,32 +1438,34 @@
                 nuis.Print()
         else:
             self.stdout.info("REGTEST: Number of nuisance parameters looks good!")
   
     def get_pdf_name(self, category:str):
         return f"{FINAL_PDF_NAME}_{category}"
     
-    def implement_model_config_and_sets(self, ws:"ROOT.RooWorkspace", mc:"ROOT.RooStats.ModelConfig",
+    def implement_model_config_and_sets(self, ws:"ROOT.RooWorkspace",
+                                        mc:"ROOT.RooStats.ModelConfig",
                                         obs:ROOT.RooArgSet, pois:ROOT.RooArgSet,
                                         nuis:ROOT.RooArgSet, globs:ROOT.RooArgSet):
-        ws.defineSet("nuisanceParameters", nuis)
-        ws.defineSet("globalObservables", globs)
-        ws.defineSet("Observables", obs)        
-        ws.defineSet("POI", pois)
-        mc.SetPdf(ws.pdf("CombinedPdf"))
-        mc.SetObservables(ws.set("Observables"))
-        mc.SetParametersOfInterest(ws.set("POI"))
-        mc.SetNuisanceParameters(ws.set("nuisanceParameters"))
-        mc.SetGlobalObservables(ws.set("globalObservables"))
+        ws.defineSet(OBS_SET, obs)        
+        ws.defineSet(POI_SET, pois)
+        ws.defineSet(NUIS_SET, nuis)
+        ws.defineSet(GLOB_SET, globs)
+        
+        mc.SetPdf(ws.pdf(COMBINED_PDF_NAME))
+        mc.SetObservables(ws.set(OBS_SET))
+        mc.SetParametersOfInterest(ws.set(POI_SET))
+        mc.SetNuisanceParameters(ws.set(NUIS_SET))
+        mc.SetGlobalObservables(ws.set(GLOB_SET))
         self.import_object(ws, mc, silent=False)
                     
     def generate_workspace(self):
         t0 = time.time()
         channel_list = ROOT.RooCategory("channellist", "channellist")
-        combined_pdf = ROOT.RooSimultaneous("CombinedPdf", "", channel_list)
+        combined_pdf = ROOT.RooSimultaneous(COMBINED_PDF_NAME, "", channel_list)
         
         obs          = ROOT.RooArgSet()
         pois         = ROOT.RooArgSet()
         nuis         = ROOT.RooArgSet()
         globs        = ROOT.RooArgSet()
         constraints  = ROOT.RooArgSet()
```

### Comparing `quickstats-0.6.7.7/quickstats/components/workspaces/xml_ws_combiner.py` & `quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_combiner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/components/workspaces/xml_ws_modifier.py` & `quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_modifier.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/concurrent/abstract_runner.py` & `quickstats-0.6.7.8/quickstats/concurrent/abstract_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/concurrent/logging.py` & `quickstats-0.6.7.8/quickstats/concurrent/logging.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/concurrent/parameterised_asymptotic_cls.py` & `quickstats-0.6.7.8/quickstats/concurrent/parameterised_asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/concurrent/parameterised_likelihood.py` & `quickstats-0.6.7.8/quickstats/concurrent/parameterised_likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/concurrent/parameterised_runner.py` & `quickstats-0.6.7.8/quickstats/concurrent/parameterised_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/core/abstract_object.py` & `quickstats-0.6.7.8/quickstats/core/abstract_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/core/configs.py` & `quickstats-0.6.7.8/quickstats/core/configs.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/core/configurable_object.py` & `quickstats-0.6.7.8/quickstats/core/configurable_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/core/dataclass_object.py` & `quickstats-0.6.7.8/quickstats/core/dataclass_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/core/decorators.py` & `quickstats-0.6.7.8/quickstats/core/decorators.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/core/enums.py` & `quickstats-0.6.7.8/quickstats/core/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,17 @@
     def on_parse_exception(cls, expr:str):
         options = cls.get_members()
         raise RuntimeError(f"invalid option \"{expr}\" for the enum class \"{cls.__name__}\" "
                            f"(allowed options: {', '.join(options)})")
     
     @classmethod
     def parse(cls, expr:str):
-        if isinstance(expr, cls):
+        if expr is None:
+            return None
+        elif isinstance(expr, cls):
             return expr
         elif isinstance(expr, int):
             return cls(expr)
         _expr = expr.strip().lower()
         members = cls.get_members_map()
         if _expr in members:
             return cls(members[_expr])
```

### Comparing `quickstats-0.6.7.7/quickstats/core/methods.py` & `quickstats-0.6.7.8/quickstats/core/methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/core/path_manager.py` & `quickstats-0.6.7.8/quickstats/core/path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/core/virtual_trees.py` & `quickstats-0.6.7.8/quickstats/core/virtual_trees.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/interface/cppyy/core.py` & `quickstats-0.6.7.8/quickstats/interface/cppyy/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/interface/cppyy/macros.py` & `quickstats-0.6.7.8/quickstats/interface/cppyy/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/interface/cppyy/vectorize.py` & `quickstats-0.6.7.8/quickstats/interface/cppyy/vectorize.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/interface/root/RooAbsData.py` & `quickstats-0.6.7.8/quickstats/interface/root/RooAbsData.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/interface/root/RooDataSet.py` & `quickstats-0.6.7.8/quickstats/utils/root_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,337 +1,336 @@
-from typing import Dict, Union, List, Optional
+from typing import Optional, Dict, List, Union
+import os
+import glob
+import time
 
 import numpy as np
 
-from quickstats import semistaticmethod
-from quickstats.interface.cppyy.vectorize import as_np_array
+import ROOT
+import quickstats
 
-class RooDataSet:
-    
-    @staticmethod
-    def to_numpy(dataset:"ROOT.RooDataSet"):
-        import ROOT
-        components = dataset.get()
-        observables = ROOT.RooArgSet()
-        category = None
-        for component in components:
-            if component.ClassName() == "RooCategory":
-                if category is not None:
-                    raise RuntimeError("found multiple RooCategory instances")
-                category = component
-            else:
-                observables.add(component)
-        if category is None:
-            result = ROOT.RFUtils.ExtractData(dataset, observables)
-        else:
-            result = ROOT.RFUtils.ExtractCategoryData(dataset, observables, category)
-        obs_values = as_np_array(result.observable_values)
-        n_entries = dataset.numEntries()
-        data = {}
-        for i, obs in enumerate(observables):
-            obs_name = obs.GetName()
-            data[obs_name] = obs_values[i*n_entries: (i + 1)*n_entries]
-        data['weight'] = as_np_array(result.weights)
-        if category is not None:
-            data['label'] = as_np_array(result.category_labels)
-            data['index'] = as_np_array(result.category_index)
-        return data
-    
-    @staticmethod
-    def from_numpy(data:Dict[str, "numpy.ndarray"],
-                   variables:"ROOT.RooArgSet",
-                   name:str=None, title:str=None,
-                   weight_name:str=None, clip_to_limits=True):
-        import ROOT
-        if name is None:
-            name = ""
-        if title is None:
-            title = ""
-            
-        if weight_name is None:
-            dataset = ROOT.RooDataSet(name, title, variables)
-        else:
-            dataset = ROOT.RooDataSet(name, title, variables, weight_name)
-            
-        real_variables = {}
-        cat_variables = {}
-        for v in variables:
-            var_name = v.GetName()
-            class_name = v.ClassName()
-            if var_name == weight_name:
-                continue
-            if var_name not in data:
-                if (class_name == "RooCategory") and ("index" in data):
-                    var_name = "index"
-                else:
-                    raise RuntimeError(f"missing data for the variable `{var_name}`")
-            if class_name == "RooCategory":
-                cat_variables[var_name] = v
-            else:
-                real_variables[var_name] = v
-                if clip_to_limits:
-                    data[var_name] = np.clip(data[var_name], 
-                                             a_min=v.getMin(),
-                                             a_max=v.getMax())
-        if weight_name not in data:
-            if "weight" in data:
-                weight_name = "weight"
-            else:
-                raise RuntimeError(f"missing data for the variable `{weight_name}`")
-        data_sizes = [len(data[k]) for k in data]
-        if len(set(data_sizes)) > 1:
-            raise RuntimeError("data has inconsistent sizes")
-        if weight_name is None:
-            for i in range(data_sizes[0]):
-                for name, variable in real_variables.items():
-                    variable.setVal(data[name][i])
-                for name, variable in cat_variables.items():
-                    variable.setIndex(data[name][i])
-                dataset.add(variables, 1.)
-        else:
-            for i in range(data_sizes[0]):
-                for name, variable in real_variables.items():
-                    variable.setVal(data[name][i])
-                for name, variable in cat_variables.items():
-                    variable.setIndex(int(data[name][i]))
-                weight = data[weight_name][i]
-                dataset.add(variables, weight)
-        return dataset
+root_type_str_maps = {
+    'Char_t'    : 'char',
+    'Bool_t'    : 'bool',
+    'Float_t'   : 'float',
+    'Double_t'  : 'double',
+    'Int_t'     : 'int',
+    'Long_t'    : 'long',
+    'Long64_t'  : 'long long',
+    'UInt_t'    : 'unsigned int',
+    'ULong_t'   : 'unsigned long',
+    'ULong64_t' : 'unsigned long long'
+}
+
+def rtype2ctype(rtypes:List[str]):
+    ctypes = []
+    for rtype in rtypes:
+        #rtype = rtype.replace("ROOT::VecOps::RVec", "vector")
+        ctype = root_type_str_maps.get(rtype, rtype)
+        ctypes.append(ctype)
+    return ctypes
+
+def templated_rdf_snapshot(rdf:ROOT.RDataFrame, columns:List[str]=None):
+    if columns is None:
+        columns = [str(i) for i in rdf.GetColumnNames()]
+    rtypes = [rdf.GetColumnType(c) for c in columns]
+    ctypes = tuple(rtype2ctype(rtypes))
+    snapshot = rdf.Snapshot.__getitem__(ctypes)
+    return snapshot
+
+def is_corrupt(f:Union[ROOT.TFile, str]):
+    if isinstance(f, str):
+        f = ROOT.TFile(f)
+    if f.IsZombie():
+        return True
+    if f.TestBit(ROOT.TFile.kRecovered):
+        return True
+    if f.GetNkeys() == 0:
+        return True
+    return False
+
+def release_tfiles():
+    for f in ROOT.gROOT.GetListOfFiles():
+        f.Close()
+
+def compile_macro(name:str, opt:str="kfOc"):
+    macros_dir = os.path.join(quickstats.macro_path, name)
+    macros_path = os.path.join(macros_dir, name + '.cxx')
+    print('INFO: Compiling macro "{}"...'.format(name))
+    if not os.path.exists(macros_path):
+        print('ERROR: Cannot locate macro files from {}. ROOT macros will not be compiled.'.format(macros_dir))
+        return -1
+    status = ROOT.gSystem.CompileMacro(macros_path, opt)
+    #status = ROOT.gROOT.LoadMacro('{}++'.format(macros_path))
+    return status
+
+def load_macro(name:str):
+    import cppyy
+    if name in dir(cppyy.gbl):
+        return None
+    auto_load = ROOT.gInterpreter.AutoLoad(name)
+    # already loaded by quickstats / third-party
+    if auto_load == 1:
+        return None
+    class_loaded = hasattr(ROOT, name)
+    if class_loaded:
+        return None
+    macros_dir = os.path.join(quickstats.macro_path, name)
+    macros_path = os.path.join(macros_dir, name + '_cxx')
+    if not os.path.exists(macros_path + '.so'):
+        status_compile = compile_macro(name)
+    status_load = ROOT.gSystem.Load(macros_path)
+    if (status_load != 0) and (status_load != 1):
+        raise RuntimeError(f"Shared library for the macro {name} is incompatible with the current pyROOT version. "
+                           "Please recompile by using the command line \"quickstats compile\". "
+                           "(use quickstats.compile_macros() instead inside a jupyter kernel)")
+    return status_load
+
+def get_macro_dir(name:str):
+    return os.path.join(quickstats.macro_path, name)
+
+def get_macro_TClass(name:str):
+    if not getattr(ROOT, name):
+        raise RuntimeError(f"class {name} is not loaded into ROOT yet")    
+    cls = ROOT.TClass.GetClass(name)
+    macro_dir = get_macro_dir(name)
+    macro_decl_file = os.path.join(f"{macro_dir}/{name}.h")
+    macro_impl_file = os.path.join(f"{macro_dir}/{name}.cxx")
+    if not os.path.exists(macro_decl_file):
+        raise FileNotFoundError(f"decl file {macro_decl_file} for the macro \"{name}\" not found")
+    if not os.path.exists(macro_impl_file):
+        raise FileNotFoundError(f"impl file {macro_impl_file} for the macro \"{name}\" not found")        
+    cls.SetDeclFile(macro_decl_file, 0)
+    cls.SetImplFileName(macro_impl_file)
+    return cls
+
+def print_resource_used(start):
+    proc_info = ROOT.ProcInfo_t()
+    flag = ROOT.gSystem.GetProcInfo(proc_info)
+    if flag < 0:
+        return None
+    cpu_time = proc_info.fCpuUser + proc_info.fCpuSys
+    wall_time = time.time()-start
+    print('Resources Used: cpu_time={:.3f}s, mem={}kb, vmem={}kb, wall_time={:.3f}s'.format(
+          cpu_time, proc_info.fMemResident, proc_info.fMemVirtual, wall_time))
+    return None
+
+def process_uproot_array(source):
+    result = np.array(source)
+    if (result.dtype == np.dtype('O')) and (isinstance(result[0], bytes)):
+        result = result.astype(str)
+    return result
+
+def get_data_size(data):
+    if isinstance(data, (tuple, list, np.ndarray)):
+        return len(data)
+    else:
+        return 1
     
-    @semistaticmethod
-    def to_pandas(self, dataset:"ROOT.RooDataSet"):
-        numpy_data = self.to_numpy(dataset)
-        import pandas as pd
-        df = pd.DataFrame(numpy_data)
-        return df
+def root_to_dict(filename:str, simplify:bool=True):
+    f = ROOT.TFile(filename)
+    if is_corrupt(f):
+        raise RuntimeError(f"corrupted ROOT file: {filename}")
+    treenames = [t.GetName() for t in f.GetListOfKeys()]
+    result = {}
+    for treename in treenames:
+        tree = f.Get(treename)
+        rdf = ROOT.RDataFrame(tree)
+        data = rdf.AsNumpy()
+        for branch in data:
+            # convert std::string to python string
+            if rdf.GetColumnType(branch) == "string":
+                data[branch] = np.char.mod('%s', data[branch])
+            # unwrap array if size is 1
+            if simplify and (data[branch].shape[0] == 1):
+                data[branch] = data[branch][0]
+        result[treename] = data
+    return result    
+
+def uproot_to_dict(file):
+    result = {}
+    for tree in file.values():
+        #tree_name = tree.name.decode('utf-8')
+        tree_name = tree.name
+        result[tree_name] = {}
+        for branch in tree.values():
+            #branch_name = branch.name.decode('utf-8')
+            branch_name = branch.name
+            arr = process_uproot_array(branch.array())
+            value = arr[0] if len(arr) == 1 else arr
+            result[tree_name][branch_name] = value    
+    return result
     
-    @staticmethod
-    def get_dataset_map(dataset_dict:Dict):
-        import ROOT
-        dsmap = ROOT.std.map('string, RooDataSet*')()
-        dsmap.keepalive = list()
-        for c, d in dataset_dict.items():
-            dsmap.keepalive.append(d)
-            dsmap.insert(dsmap.begin(), ROOT.std.pair("const string, RooDataSet*")(c, d))
-        return dsmap
+def get_leaf_type_str(data):
+    from six import string_types
     
-    @staticmethod
-    def from_RooDataHist(source:"ROOT.RooDataHist", pdf:"ROOT.RooAbsPdf",
-                         name:Optional[str]=None):
-        import ROOT
-        if name is None:
-            name = source.GetName()
-        parameters = source.get()
-        category = None
-        for parameter in parameters:
-            if parameter.ClassName() == "RooCategory":
-                category = parameter
-                break
-      # case multi-category data
-        if category is not None:
-            dataset_map = {}
-            data_cat = source.split(category, True)
-            n_cat = len(category)
-            observables = ROOT.RooArgSet()
-            for i in range(n_cat):
-                category.setBin(i)
-                cat_name = category.getLabel()
-                pdf_i = pdf.getPdf(cat_name)
-                data_i = data_cat.FindObject(cat_name)                
-                obs_i = pdf_i.getObservables(data_i).first()
-                _obs_i = data_i.get().find(obs_i.GetName())
-                w_i = ROOT.RooRealVar(f"weight_{i}", f"weight_{i}", 1)
-                dataset_i = ROOT.RooDataSet(f"dataset_{i}", f"dataset_{i}",
-                                            ROOT.RooArgSet(obs_i, w_i),
-                                            ROOT.RooFit.WeightVar(w_i))
-                ROOT.RFUtils.CopyData(data_i, dataset_i, _obs_i, obs_i, w_i)
-                dataset_map[cat_name] = dataset_i
-                observables.add(obs_i)
-            w = ROOT.RooRealVar("weight", "weight", 1)
-            observables.add(w)
-            cpp_dataset_map = RooDataSet.get_dataset_map(dataset_map)
-            dataset = ROOT.RooDataSet(name, name, observables,
-                                      ROOT.RooFit.Index(category),
-                                      ROOT.RooFit.Import(cpp_dataset_map),
-                                      ROOT.RooFit.WeightVar(w))
-        # case single-category data
-        else:
-            obs = pdf.getObservables(source).first()
-            _obs = source.get().find(obs.GetName())
-            w = ROOT.RooRealVar("weight", "weight", 1)
-            dataset = ROOT.RooDataSet(name, name, ROOT.RooArgSet(obs, w),
-                                      ROOT.RooFit.WeightVar(w))
-            ROOT.RFUtils.CopyData(source, dataset, _obs, obs, w)
-        return dataset
-
-    @staticmethod
-    def _get_cat_and_obs(variables:"ROOT.RooArgSet"):
-        cat_variable = None
-        observables = {}
-        for v in variables:
-            class_name = v.ClassName()
-            if class_name == "RooCategory":
-                if cat_variable is not None:
-                    raise RuntimeError("found multiple RooCategory instances")
-                cat_variable = v
+    type_str = None
+    data_type = None
+
+    if isinstance(data, (tuple, list, np.ndarray)):
+        data_type = type(data[0])
+        if data_type in string_types:
+            return None
+    elif isinstance(data, string_types):
+        return None
+    else:
+        data_type = type(data)
+        
+    if data_type in [float, np.float64]:
+        type_str = 'D'
+    elif data_type in [int, np.int64]:
+        type_str = 'L'
+    elif data_type in [np.int32]:
+        type_str = 'I'
+    elif data_type in [np.uint32]:
+        type_str = 'i'        
+    elif data_type in [bool, np.bool_]:
+        type_str = 'O'        
+    elif data_type in [np.float32]:
+        type_str = 'F'
+    elif data_type in [np.int8]:
+        type_str = 'B'
+    elif data_type in [np.uint8]:
+        type_str = 'b'
+    else:
+        raise ValueError('cannot infer leaf type for {}'.format(data_type))
+    return type_str
+
+def fill_branch(tree, values_dict):
+    buffer = {}
+    leaf_types = {}
+    data_sizes = list(set([get_data_size(v) for k,v in values_dict.items()]))
+    if len(data_sizes) > 1:
+        raise ValueError('cannot fill tree with values of inconsistent entry sizes')
+    data_size = data_sizes[0]
+    if data_size == 1:
+        for k, v in values_dict.items():
+            leaf_type_str = get_leaf_type_str(v)
+            leaf_types[k] = leaf_type_str
+            if leaf_type_str is not None:
+                buffer[k] = np.array([v], dtype=type(v))
+                tree.Branch(k, buffer[k], '{}/{}'.format(k, leaf_type_str))
             else:
-                var_name = v.GetName()
-                observables[var_name] = v
-        if cat_variable is None:
-            raise RuntimeError("missing RooCategory instance from variables")
-        return cat_variable, observables
-
-    @semistaticmethod
-    def create_binned_category_dataset(self, data:Dict[str, "numpy.ndarray"],
-                                       pdf:"ROOT.RooAbsPdf",
-                                       variables:"ROOT.RooArgSet",
-                                       weight_name:str="weightVar",
-                                       name:str=None, title:str=None):
-        import ROOT
-        if name is None:
-            name = ""
-        if title is None:
-            title = ""        
-        cat_variable, observables = self._get_cat_and_obs(variables)
-        n_cat = cat_variable.size()
-        cat_names = []
-        cat_obs_names = []
-        for i in range(n_cat):
-            cat_variable.setIndex(i)
-            cat_name = cat_variable.getLabel()
-            cat_names.append(cat_name)
-            pdf_cat = pdf.getPdf(cat_name)
-            obs = pdf_cat.getObservables(variables)
-            cat_obs = obs.first()
-            cat_obs_names.append(cat_obs.GetName())
-        if set(cat_obs_names) != set(observables):
-            raise RuntimeError("the given variables are insistent with the category observables")
-        if not set(cat_names).issubset(set(data)):
-            missing = list(set(cat_names) - set(data))
-            raise RuntimeError("missing data for the following categories: {}".format(",".join(missing)))
-        dataset = ROOT.RooDataSet(name, title, variables, weight_name)
-        for i, (cat_name, obs_name) in enumerate(zip(cat_names, cat_obs_names)):
-            observable = observables[obs_name]
-            data_i = data[cat_name]
-            cat_variable.setIndex(i)
-            n_bins = observable.getBins()
-            n_bins_data = len(data_i)
-            if n_bins_data != n_bins:
-                raise RuntimeError(f"the observable has `{n_bins}` bins but data has `{n_bins_data}`")
-            for j in range(n_bins_data):
-                observable.setBin(j)
-                dataset.add(variables, data_i[j])
-        return dataset
-    
-    @semistaticmethod
-    def to_category_data(self, dataset:"ROOT.RooDataSet",
-                         pdf:"ROOT.RooAbsPdf"):
-        variables = dataset.get()
-        cat_variable, observables = self._get_cat_and_obs(variables)
-        n_cat = cat_variable.size()
-        data = self.to_numpy(dataset)
-        result = {}
-        for i in range(n_cat):
-            cat_variable.setIndex(i)
-            cat_name = cat_variable.getLabel()
-            pdf_cat = pdf.getPdf(cat_name)
-            obs = pdf_cat.getObservables(variables)
-            cat_obs = obs.first()
-            obs_name = cat_obs.GetName()
-            mask = (data['index'] == i)
-            bin_value = data[obs_name][mask]
-            ind = np.argsort(bin_value)
-            bin_weight = data['weight'][mask][ind]
-            result[cat_name] = bin_weight
-        return result
-    
-    @staticmethod
-    def fill_from_TH1(dataset:"ROOT.RooDataSet", hist:"ROOT.TH1",
-                      skip_out_of_range:bool=True,
-                      blind_range:Optional[List[float]]=None,
-                      min_bin_value:float=0,
-                      weight_scale:float=1):
-        import ROOT
-        parameters = dataset.get()
-        if parameters.size() > 1:
-            raise RuntimeError("multiple observables are not allowed")
-        x = parameters.first()
-        weight_var = dataset.weightVar()
-        # blinding will be taken care of
-        xmin = x.getMin()
-        xmax = x.getMax()
-        n_bins = hist.GetNbinsX()
-        for i in range(1, n_bins + 1):
-            bin_center = hist.GetBinCenter(i)
-            # skip bins that are out of range
-            if skip_out_of_range and ((bin_center > xmax) or (bin_center < xmin)):
-                continue
-            # skip bins in the blind range
-            if (blind_range and (bin_center > blind_range[0]) and (bin_center < blind_range[1])):
-                continue
-            x.setVal(bin_center)
-            bin_content = hist.GetBinContent(i)
-            weight = bin_content * weight_scale
-            # if the weight is negligible, consider it as zero
-            if (weight < min_bin_value):
-                continue;
-            if weight_var:
-                weight_var.setVal(weight)
-                dataset.add(ROOT.RooArgSet(x, weight_var), weight)
+                buffer[k] = ROOT.std.string(v)
+                tree.Branch(k, buffer[k])
+        tree.Fill()
+    else:
+        for k, v in values_dict.items():
+            leaf_type_str = get_leaf_type_str(v)
+            leaf_types[k] = leaf_type_str
+            if leaf_type_str is not None:
+                buffer[k] = np.array([v[0]], dtype=type(v[0]))
+                tree.Branch(k, buffer[k], '{}/{}'.format(k, leaf_type_str))
             else:
-                dataset.add(ROOT.RooArgSet(x), weight)
-    
-    @staticmethod
-    def get_x_and_weight(dataset:"ROOT.RooDataSet"):
-        parameters = dataset.get()
-        if parameters.size() > 1:
-            raise RuntimeError("multiple observables are not allowed")
-        x = parameters.first()
-        weight_var = dataset.weightVar()
-        return x, weight_var
+                buffer[k] = ROOT.std.string(v[0])
+                tree.Branch(k, buffer[k])
+        for i in range(data_size):
+            for k, v in values_dict.items():
+                if leaf_types[k] is not None:
+                    buffer[k][0] = v[i]
+                else:
+                    buffer[k].replace(0, ROOT.std.string.npos, v[i])
+            tree.Fill()
+            
+def close_all_root_files():
+    opened_files = ROOT.gROOT.GetListOfFiles()
+    for f in opened_files:
+        f.Close()
+        
+def create_declaration(expression:str, name:Optional[str]=None):
+    if name is None:
+        hash_str = str(hash(expression)).replace("-", "n")
+        name_guard = f"__quickstats_declare_{hash_str}__"
+    else:
+        name_guard = f"__quickstats_declare_{name}__"
+    guarded_declaration = f"#ifndef {name_guard}\n"
+    guarded_declaration += f"#define {name_guard}\n"
+    guarded_declaration += f"\n{expression}\n\n#endif\n"
+    return guarded_declaration
+
+def declare_expression(expression:str, name:Optional[str]=None):
+    declaration = create_declaration(expression, name)
+    status = ROOT.gInterpreter.Declare(declaration)
+    return status
+
+def get_tree_names(f:ROOT.TFile):
+    tree_names = []
+    for i in f.GetListOfKeys():
+        obj = f.Get(i.GetName())
+        if isinstance(obj, ROOT.TTree):
+            tree_names.append(obj.GetName())
+    return tree_names
+
+def merge_root_files(source_files:Union[str, List[str]], target_file:str, treename:str=None,
+                     multithread:bool=True, keep_order:bool=False, use_template:bool=True,
+                     ignore_missing_columns:bool=True, verbosity:str="INFO"):
+    from quickstats.utils.io import VerbosePrint
+    stdout = VerbosePrint(verbosity)
     
-    @staticmethod
-    def to_TH1(dataset:"ROOT.RooDataSet", name:str,
-               blind_range:Optional[List[float]]=None,
-               weight_scale:float=1):
-        x, weight_var = RooDataSet.get_x_and_weight(dataset)
-        n_bins = x.getBins()
-        x_min = x.getMin()
-        x_max = x.getMax()
-        import ROOT
-        hist = ROOT.TH1D(name, name, n_bins, x_min, x_max)
-        hist.Sumw2()
-        for i in range(dataset.numEntries()):
-            dataset.get(i)
-            x_val = x.getVal()
-            obs.setVal(x_val)
-            weight = dataset.weight() * weight_scale
-            # ignore data in the blind range
-            if (blind_range and (x_val > blind_range[0]) and (x_val < blind_range[1])):
-                continue
-            hist.Fill(x_val, weight)
-        return hist
+    if isinstance(source_files, str):
+        source_files = [source_files]
+    rfiles = []
+    for source_file in source_files:
+        files = glob.glob(source_file)
+        if not files:
+            raise FileNotFoundError(f"file \"{source_file}\" does not exist")
+        rfiles += files
+    # now all rfiles are guaranteed to exist
+    for i, rfile in enumerate(rfiles):
+        stdout.info(f"Source {i+1}: {rfile}")
+        if is_corrupt(rfile):
+            raise RuntimeError(f"the root file \"{rfile}\" is corrupted")
+    if not rfiles:
+        raise RuntimeError("no source files found")
+    if treename is None:
+        f = ROOT.TFile(rfiles[0])
+        treenames = get_tree_names(f)
+        if len(treenames) > 1:
+            raise RuntimeError("unable to deduce tree name from source files: "
+                               "multiple trees are present")
+        treename = treenames[0]
+        stdout.info("INFO: No tree name specified for merging. Will use "
+                    f"the auto-detected tree name \"{treename}\".")
+        
+    # configure multi-threading setting
+    multithread_orig_state = ROOT.IsImplicitMTEnabled()
+    if multithread and (not multithread_orig_state) and (not keep_order):
+        ROOT.EnableImplicitMT()
+    if keep_order and multithread_orig_state:
+        ROOT.DisableImplicitMT()
     
-    @staticmethod
-    def add_ghost_weights(dataset:"ROOT.RooDataSet",
-                          blind_range:Optional[List[float]]=None,
-                          ghost_weight:float=1e-9):
-        x, weight_var = RooDataSet.get_x_and_weight(dataset)
-        xmin = x.getMin()
-        xmax = x.getMax()
-        n_bins = x.getBins()
-        bin_width = (xmax - xmin) / n_bins
-        data = RooDataSet.to_numpy(dataset)
-        x_data = data[x.GetName()]
-        weight_data = data["weight"]
-        hist, bin_edges = np.histogram(x_data, bins=n_bins, range=(xmin, xmax), weights=weight_data)
-        from quickstats.maths.statistics import bin_edge_to_bin_center
-        bin_centers = bin_edge_to_bin_center(bin_edges)
-        import ROOT
-        for bin_val, bin_center in zip(hist, bin_centers):
-            if (bin_val != 0):
-                continue
-            if (blind_range and (bin_center > blind_range[0]) and (bin_center < blind_range[1])):
-                continue
-            x.setVal(bin_center)
-            weight_var.setVal(ghost_weight)
-            dataset.add(ROOT.RooArgSet(x, weight_var), ghost_weight)
+    if ignore_missing_columns:
+        column_map = {}
+        all_columns = set()
+        for rfile in rfiles:
+            rdf = ROOT.RDataFrame(treename, rfile)
+            columns = set([str(i) for i in rdf.GetColumnNames()])
+            all_columns.update(columns)
+            column_map[rfile] = columns
+        for fname, columns in column_map.items():
+            if columns != all_columns:
+                missing_columns = list(all_columns - columns)
+                stdout.warning(f"WARNING: The root file \"{rfile}\" is missing the following column(s): "
+                               f"{','.join(missing_columns)}. The missing column(s) will not be saved.")
+        columns_to_keep = list(set.intersection(*column_map.values()))
+        rdf = ROOT.RDataFrame(treename, rfiles)
+        stdout.info(f"Target path: {target_file}")
+        if use_template:
+            snapshot = templated_rdf_snapshot(rdf, columns_to_keep)
+        else:
+            snapshot = rdf.Snapshot
+        snapshot(treename, target_file, columns_to_keep)
+    else:
+        rdf = ROOT.RDataFrame(treename, rfiles)
+        stdout.info(f"Target path: {target_file}")
+        if use_template:
+            snapshot = templated_rdf_snapshot(rdf, columns_to_keep)
+        else:
+            snapshot = rdf.Snapshot
+        snapshot(treename, target_file)
+   
+    # restore multi-threading setting
+    if multithread_orig_state != ROOT.IsImplicitMTEnabled():
+        if multithread_orig_state:
+            ROOT.DisableImplicitMT()
+        else:
+            ROOT.EnableImplicitMT()
```

### Comparing `quickstats-0.6.7.7/quickstats/interface/root/RooMsgService.py` & `quickstats-0.6.7.8/quickstats/interface/root/RooMsgService.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/interface/root/RooRealVar.py` & `quickstats-0.6.7.8/quickstats/interface/root/RooRealVar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from typing import Dict, Union, List, Optional
+import copy
 
+from quickstats import semistaticmethod
 from quickstats.maths.numerics import get_proper_ranges
+from quickstats.interface.root import TArrayData
 
 class RooRealVar:
     
     @property
     def range(self):
         return self._range
     
@@ -39,17 +42,19 @@
             self.name = obj["name"]
             self.title = obj.get("title", None)
             self.value = obj.get("value", None)
             self.range = obj.get("range", None)
             self.named_ranges = obj.get("named_ranges", None)
             self.n_bins = obj.get("n_bins", None)
             self.unit = obj.get("unit", None)
+        elif isinstance(obj, RooRealVar):
+            self.__dict__ = copy.deepcopy(obj.__dict__)
         else:
-            import ROOT
-            if not isinstance(obj, ROOT.RooRealVar):
+            isvalid = hasattr(obj, 'ClassName') and (obj.ClassName() == 'RooRealVar')
+            if not isvalid:
                 raise ValueError("object must be an instance of ROOT.RooRealVar")
             self.name   = str(obj.GetName())
             self.title  = str(obj.getTitle())
             self.value  = obj.getVal()
             self.n_bins = obj.getBins()
             self.unit   = obj.getUnit()
             _range = obj.getRange()
@@ -127,9 +132,15 @@
                 variable.setRange(name, _range[0], _range[1])            
         
         if self.n_bins is not None:
             variable.setBins(self.n_bins)
             
         if self.unit is not None:
             variable.setUnit(self.unit)
-            
-        return variable
+        ROOT.SetOwnership(variable, False)
+        return variable
+
+    @semistaticmethod
+    def get_bin_widths(self, obj:"ROOT.RooRealVar"):
+        import ROOT
+        c_vector = ROOT.RFUtils.GetRooRealVarBinWidths(obj)
+        return TArrayData.vec_to_array(c_vector)
```

### Comparing `quickstats-0.6.7.7/quickstats/interface/root/TF1.py` & `quickstats-0.6.7.8/quickstats/interface/root/TF1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/interface/root/TFile.py` & `quickstats-0.6.7.8/quickstats/interface/root/TFile.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,11 +48,19 @@
         for i in range(n_entries):
             for branch in branches:
                 
         tree.SetDirectory(self.obj)
         # save only the new version of the tree
         tree.GetCurrentFile().Write("", ROOT.TObject.kOverwrite)
     """
+    
+    def get_tree(self, name:str, strict:bool=True):
+        tree = self.rfile.Get(name)
+        if not tree:
+            if strict:
+                raise RuntimeError(f'In TFile.Get: Tree "{name}" does not exist')
+            return None
+        return tree
 
     def close(self):
         self.rfile.Close()
         self.rfile = None
```

### Comparing `quickstats-0.6.7.7/quickstats/interface/root/TH1.py` & `quickstats-0.6.7.8/quickstats/interface/root/TH1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from typing import Optional, Tuple, List, Dict
+from typing import Optional, Tuple, List, Dict, Union, Sequence
 import uuid
 import array
 import numpy as np
 
+from quickstats.maths.statistics import (get_hist_mean, get_hist_mean_error,
+                                         get_hist_std, get_cumul_hist, histogram,
+                                         bin_edge_to_bin_center,
+                                         bin_center_to_bin_edge)
 from quickstats.interface.root import TObject, TArrayData
 from quickstats.interface.root import load_macro
 from quickstats.interface.cppyy.vectorize import as_vector, as_np_array, as_c_array, np_type_str_maps
 
 class TH1(TObject):
     
     def __init__(self, h:Optional["ROOT.TH1"]=None, dtype:str='double', 
@@ -37,67 +41,75 @@
             self.bin_content = None
             self.bin_error = None
             self.bin_center = None
             self.bin_width = None
             self.bin_low_edge = None
     
     @classmethod
-    def from_numpy_data(cls, x:np.ndarray, bins:int=10, range:Optional[Tuple[float]]=None,
-                        density:bool=False, weights:Optional[np.ndarray]=None, **kwargs):
-        hist, bin_edges = np.histogram(x, bins=bins, range=range, density=density, weights=weights)
-        return cls.from_numpy_histogram(hist, bin_edges, **kwargs)
+    def from_numpy_data(cls, x:np.ndarray, weights:Optional[np.ndarray]=None,
+                        bins:Union[int, Sequence]=10,
+                        bin_range:Optional[Sequence]=None,
+                        normalize:bool=True,
+                        **kwargs):
+        bin_content, bin_edges, bin_error = histogram(x, weights=weights,
+                                                      bins=bins, bin_range=bin_range,
+                                                      normalize=normalize, clip_weight=True,
+                                                      evaluate_error=True,
+                                                      error_option='sumw2')
+        instance = cls.from_numpy_histogram(bin_content, bin_edges,
+                                            bin_error=bin_error,
+                                            **kwargs)
+        return instance
     
     @classmethod
-    def from_numpy_histogram(cls, hist:np.ndarray, bin_edges:np.ndarray, **kwargs):
-        assert (hist.ndim == 1) and (bin_edges.ndim == 1)
-        th1 = TH1(**kwargs)
-        th1.bin_content = np.array(hist)
-        th1.bin_error = np.zeros(th1.bin_content.shape)
-        th1.bin_low_edge = np.array(bin_edges)
-        from quickstats.maths.statistics import bin_edge_to_bin_center
-        th1.bin_center = bin_edge_to_bin_center(th1.bin_low_edge)
-        th1.bin_width = (th1.bin_low_edge[-1] - th1.bin_low_edge[0]) / (th1.bin_low_edge.shape[0] - 1)
-        return th1
+    def from_numpy_histogram(cls, bin_content:np.ndarray,
+                             bin_edges:np.ndarray,
+                             bin_error:Optional[np.ndarray]=None,
+                             **kwargs):
+        assert (bin_content.ndim == 1) and (bin_edges.ndim == 1)
+        instance = TH1(**kwargs)
+        instance.bin_content = np.array(bin_content)
+        if bin_error is None:
+            instance.bin_error = np.zeros(instance.bin_content.shape)
+        else:
+            bin_error = np.array(bin_error)
+            assert bin_error.shape == instance.bin_content.shape
+            instance.bin_error = bin_error
+        instance.bin_low_edge = np.array(bin_edges)
+        instance.bin_center = bin_edge_to_bin_center(instance.bin_low_edge)
+        instance.bin_width = np.diff(instance.bin_low_edge)
+        return instance
         
     @staticmethod
     def _to_ROOT(name:str, bin_content, bin_width=None, bin_center=None, bin_low_edge=None,
                  bin_error=None, title:str=None):
         import ROOT
         if ((bin_low_edge is None) and (bin_center is None)) or \
            ((bin_low_edge is not None) and (bin_center is not None)):
             raise ValueError("must provide either bin low edge or bin center values")
-        n_bins = len(bin_content)
         if bin_center is not None:
-            if bin_width is None:
-                if n_bins < 2:
-                    raise ValueError("unable to determine bin width with only one bin")
-                bin_width = (bin_center[1] - bin_center[0])
-            bin_low_edge = bin_center - bin_width/2
-        if len(bin_low_edge) == n_bins:
-            bin_width = (bin_low_edge[-1] - bin_low_edge[-2])
-            bin_low_edge = np.insert(bin_low_edge, len(bin_low_edge), bin_low_edge[-1] + bin_width)
+            bin_low_edge = bin_center_to_bin_edge(bin_center)
+        nbins = len(bin_low_edge) - 1
         if title is None:
             title = name
         dtype = bin_content.dtype
         if np_type_str_maps[dtype] == "float":
             h_func = ROOT.TH1F
         else:
             h_func = ROOT.TH1D
-        h = h_func(name, title, n_bins, as_c_array(bin_low_edge))
+        h = h_func(name, title, nbins, as_c_array(bin_low_edge))
         if bin_error is None:
-            bin_error = np.zeros((n_bins,))
-        for i in range(n_bins):
+            bin_error = np.zeros((nbins,))
+        for i in range(nbins):
             h.SetBinContent(i + 1, bin_content[i])
             h.SetBinError(i + 1, bin_error[i])
         return h
     
     def to_ROOT(self, name:str, title:str=None):
         self.sanity_check()
-        if title is None:
-            title = name
         return self._to_ROOT(name, self.bin_content, bin_low_edge=self.bin_low_edge,
                              bin_error=self.bin_error, title=title)
     
     @staticmethod
     def find_bin_by_edge(h:"ROOT.TH1", low_edge:float, tol:float=1e-6):
         import ROOT
         return ROOT.TH1Utils.FindBinIndexByBinEdge(h, low_edge, tol)
@@ -242,8 +254,35 @@
         n_bins = h.GetNbinsX()
         for i in range(1, n_bins + 1):
             if h.GetBinContent(i) != 0:
                 continue
             bin_center = h.GetBinCenter(i)
             if blind_range and (bin_center > blind_range[0]) and (bin_center < blind_range[1]):
                 continue
-            h.SetBinContent(i, ghost_weight)
+            h.SetBinContent(i, ghost_weight)
+            
+    def rebin(self, bins:Union[int, np.ndarray]=None):
+        if isinstance(bins, int):
+            bins = np.linspace(self.bin_low_edge[0], self.bin_low_edge[-1], bins + 1)
+        h = self.to_ROOT('temp', 'temp')
+        h_new = h.Rebin(bins.shape[0] - 1, 'temp_2', bins)
+        self.init(h_new)
+        # free memory
+        h.Delete()
+        h_new.Delete()
+        
+    def GetMean(self):
+        return get_hist_mean(x=self.bin_center, y=self.bin_content)
+    
+    def GetMeanError(self):
+        return get_hist_mean_error(x=self.bin_center,
+                                   y=self.bin_content,
+                                   yerr=self.bin_error)
+    
+    def GetStdDev(self):
+        return get_hist_std(x=self.bin_center, y=self.bin_content)
+    
+    def GetCumulativeHist(self):
+        bin_content, bin_error = get_cumul_hist(self.bin_content, self.bin_error)
+        return self.from_numpy_histogram(bin_content=bin_content,
+                                         bin_edges=self.bin_low_edge,
+                                         bin_error=bin_error)
```

### Comparing `quickstats-0.6.7.7/quickstats/interface/root/TH2.py` & `quickstats-0.6.7.8/quickstats/interface/root/TH2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/interface/root/TObject.py` & `quickstats-0.6.7.8/quickstats/interface/root/TObject.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/interface/root/__init__.py` & `quickstats-0.6.7.8/quickstats/interface/root/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from quickstats.interface.root.TH1 import TH1
 from quickstats.interface.root.TH2 import TH2
 from quickstats.interface.root.TF1 import TF1
 from quickstats.interface.root.TFile import TFile
 from quickstats.interface.root.RooRealVar import RooRealVar
 from quickstats.interface.root.RooAbsData import RooAbsData
 from quickstats.interface.root.RooDataSet import RooDataSet
+from quickstats.interface.root.RooCategory import RooCategory
 from quickstats.interface.root.RooAbsPdf import RooAbsPdf
 from quickstats.interface.root.RooArgSet import RooArgSet
 from quickstats.interface.root.RooMsgService import RooMsgService
 
 load_macros()
 
 import quickstats
```

### Comparing `quickstats-0.6.7.7/quickstats/interface/root/helper.py` & `quickstats-0.6.7.8/quickstats/interface/root/helper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/interface/root/inspection.py` & `quickstats-0.6.7.8/quickstats/interface/root/inspection.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/interface/root/macros.py` & `quickstats-0.6.7.8/quickstats/interface/root/macros.py`

 * *Files 10% similar despite different names*

```diff
@@ -206,14 +206,36 @@
               observable_values = std::vector<double>(n_obs * n_entries);
               weights = std::vector<double>(n_entries);
               category_labels = std::vector<std::string>(n_entries);
               category_index = std::vector<int>(n_entries);
           }
         } ;
         
+        RooCategory* GetDatasetCategory(const RooAbsData* dataset){
+            RooCategory* category = 0;
+            const RooArgSet* argset = dataset->get();
+            for (auto &arg: *argset){
+                if (strcmp(((RooAbsArg*)arg)->ClassName(), "RooCategory") == 0){
+                    category = (RooCategory*) arg;
+                    break;
+                }
+            }
+            return category;
+        }
+        
+        RooArgSet GetDatasetObservables(const RooAbsData* dataset){
+            RooArgSet observables;
+            const RooArgSet* argset = dataset->get();
+            for (auto &arg: *argset){
+                if (strcmp(((RooAbsArg*)arg)->ClassName(), "RooRealVar") == 0)
+                    observables.add(*arg);
+            }
+            return observables;
+        }
+        
         DatasetStruct ExtractCategoryData(const RooAbsData* dataset, const RooArgSet* observables, const RooCategory* cat){
             const size_t n_entries = dataset->numEntries();
             const size_t n_obs = observables->size();
             DatasetStruct result(n_entries, n_obs);
             TIterator* iter(observables->createIterator());
             RooRealVar* obs;
             for (size_t i = 0; i < n_entries; i++){
@@ -249,14 +271,37 @@
                  double weight_val = source->weight();
                  weight->setVal(weight_val);
                  target_var->setVal(source_var->getVal());
                  target->add(RooArgSet(*target_var, *weight), weight_val);
              }
         }
         
+        std::vector<double> GetRooRealVarBinWidths(const RooRealVar* var){
+            const size_t n_bins = var->numBins();
+            std::vector<double> result(n_bins, 0);
+            for (size_t i = 0; i < n_bins; i++)
+                result[i] = var->getBinWidth(i);
+            return result;
+        }
+        
+        template<typename T>
+        std::vector<double> GetPdfValues(const RooAbsPdf* pdf,
+                                         const RooArgSet* vars,
+                                         const std::vector<T> &bin_centers){
+            const auto pdf_obs = pdf->getObservables(*vars);
+            const auto target_obs = pdf_obs->first();
+            const size_t n_bins = bin_centers.size();
+            std::vector<double> result(n_bins, 0);
+            for (size_t i = 0; i < n_bins; i++){
+                ((RooRealVar*)target_obs)->setVal(bin_centers[i]);
+                result[i] = pdf->getVal(pdf_obs);
+            }
+            return result;
+        }
+        
         struct RooArgSetInfo {
           std::vector<std::string> class_names;
           std::vector<std::string> names;
           RooArgSetInfo(const RooArgSet* argset){
             const size_t n_obj = argset->size();
             this->class_names = std::vector<std::string>(n_obj);
             this->names = std::vector<std::string>(n_obj);
```

### Comparing `quickstats-0.6.7.7/quickstats/interface/root/roofit_extension.py` & `quickstats-0.6.7.8/quickstats/interface/root/roofit_extension.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx` & `quickstats-0.6.7.8/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h` & `quickstats-0.6.7.8/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx` & `quickstats-0.6.7.8/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h` & `quickstats-0.6.7.8/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx` & `quickstats-0.6.7.8/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/macros/QuickStatsCore/RooFitExt.cxx` & `quickstats-0.6.7.8/quickstats/macros/QuickStatsCore/RooFitExt.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/macros/QuickStatsCore/RooFitExt.h` & `quickstats-0.6.7.8/quickstats/macros/QuickStatsCore/RooFitExt.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/macros/ResponseFunction/ResponseFunction.cxx` & `quickstats-0.6.7.8/quickstats/macros/ResponseFunction/ResponseFunction.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/macros/ResponseFunction/ResponseFunction.h` & `quickstats-0.6.7.8/quickstats/macros/ResponseFunction/ResponseFunction.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx` & `quickstats-0.6.7.8/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h` & `quickstats-0.6.7.8/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/maths/interpolation.py` & `quickstats-0.6.7.8/quickstats/maths/interpolation.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/maths/numerics.py` & `quickstats-0.6.7.8/quickstats/maths/numerics.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,8 +161,12 @@
         if not np.all(np.diff(ranges.flatten()) >= 0):
             raise ValueError("found overlap ranges")
     return ranges
 
 def get_batch_slice_indices(totalsize:int, batchsize:int):
     assert (totalsize > 0) and (batchsize > 0)
     for i in range(0, totalsize, batchsize):
-        yield (i, min(i + batchsize, totalsize))
+        yield (i, min(i + batchsize, totalsize))
+        
+def safe_div(dividend, divisor, usenan:bool=False):
+    out = np.full(dividend.shape, np.nan) if usenan else np.zeros_like(dividend)
+    return np.divide(dividend, divisor, out=out, where=divisor!=0)
```

### Comparing `quickstats-0.6.7.7/quickstats/maths/symbolics.py` & `quickstats-0.6.7.8/quickstats/maths/symbolics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/parsers/param_parser.py` & `quickstats-0.6.7.8/quickstats/parsers/param_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/plots/__init__.py` & `quickstats-0.6.7.8/quickstats/plots/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .upper_limit_benchmark_plot import UpperLimitBenchmarkPlot
 from .likelihood_1D_plot import Likelihood1DPlot
 from .likelihood_2D_plot import Likelihood2DPlot
 from .pdf_distribution_plot import PdfDistributionPlot
 from .correlation_plot import CorrelationPlot
 from .histo_1D_plot import Histo1DPlot
 from .sample_purity_plot import SamplePurityPlot
+from .bidirectional_bar_chart import BidirectionalBarChart
 
 from matplotlib import style, colors
 
 # Reference from https://github.com/beojan/atlas-mpl
 
 style.core.USER_LIBRARY_PATHS.append(quickstats.stylesheet_path)
 style.core.reload_library()
```

### Comparing `quickstats-0.6.7.7/quickstats/plots/abstract_plot.py` & `quickstats-0.6.7.8/quickstats/plots/likelihood_2D_plot.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,218 +1,227 @@
-from typing import Optional, Union, Dict, List, Tuple, Callable
-from cycler import cycler
+from typing import Dict, Optional, Union, List
+import numpy as np
+import pandas as pd
 
-import matplotlib
+from quickstats.plots import AbstractPlot
+from quickstats.plots.template import create_transform
+from quickstats.utils.common_utils import combine_dict
+from matplotlib.lines import Line2D
+
+
+class Likelihood2DPlot(AbstractPlot):
 
-from quickstats.plots import get_color_cycle, get_cmap
-from quickstats.plots.color_schemes import QUICKSTATS_PALETTES
-from quickstats.plots.template import (single_frame, parse_styles, format_axis_ticks,
-                                       parse_analysis_label_options)
-from quickstats.utils.common_utils import combine_dict, insert_periodic_substr
-
-class AbstractPlot:
-    
-    STYLES = {}
-    
-    COLOR_CYCLE = "default"
-    
-    COLOR_PALLETE = {}
-    COLOR_PALLETE_SEC = {}
-    
     CONFIG = {
-        "xlabellinebreak": 50,
-        "ylabellinebreak": 50
+        'sigma_levels': ('1sigma', '2sigma', '3sigma'),
+        'sigma_pos': 0.93,
+        'sigma_names': ('1 $\sigma$', '2 $\sigma$', '3 $\sigma$'),
+        'sigma_colors': ("hh:darkblue", "#F2385A", "#FDC536"),
+        'highlight_styles': {
+            'linewidth': 0,
+            'marker': '*',
+            'markersize': 20,
+            'color': '#E9F1DF',
+            'markeredgecolor': 'black'
+        },
+        'bestfit_styles':{
+            'marker': 'P',
+            'linewidth': 0,
+            'markersize': 15
+        },
+        'bestfit_label': "Best fit ({x:.2f}, {y:.2f})",
+        'cmap': 'GnBu',
+        'interpolation': 'cubic',
+        'num_grid_points': 500,
     }
-    
-    def __init__(self,
-                 color_pallete:Optional[Dict]=None,
-                 color_pallete_sec:Optional[Dict]=None,
-                 color_cycle:Optional[Union[List, str, "ListedColorMap"]]=None,
-                 styles:Optional[Union[Dict, str]]=None,
-                 analysis_label_options:Optional[Dict]=None,
-                 figure_index:Optional[int]=None,
-                 config:Optional[Dict]=None):
-        
-        self.color_pallete     = combine_dict(self.COLOR_PALLETE, color_pallete)
-        self.color_pallete_sec = combine_dict(self.COLOR_PALLETE_SEC, color_pallete_sec)
-            
-        self.styles = combine_dict(self.STYLES, styles)
-        self.styles = parse_styles(self.styles)
-        
-        if analysis_label_options is None:
-            self.analysis_label_options = None
-        else:
-            self.analysis_label_options = parse_analysis_label_options(analysis_label_options)
-            
-        self.legend_order = self.get_default_legend_order()
-        
-        self.legend_data = {}
-        self.legend_data_sec = {}
-        self.legend_data_ext = {}
-        
-        self.figure_index = figure_index
-        
-        self.config = combine_dict(AbstractPlot.CONFIG, self.CONFIG)
-        if config is not None:
-            self.config = combine_dict(self.config, config)
-
-        if color_cycle is None:
-            color_cycle = self.COLOR_CYCLE
-        self.cmap = get_cmap(color_cycle)
-            
-        self.annotation_list = []
-        
-    def add_annotation(self, text:str, **kwargs):
-        self.annotation_list.append({"text": text, **kwargs})
-        
+    # https://pdg.lbl.gov/2018/reviews/rpp2018-rev-statistics.pdf#page=31
+    likelihood_label_threshold = {
+        '0.68': 2.30,
+        '1sigma': 2.30, # 68.2%
+        '0.90': 4.61,
+        '0.95': 5.99,
+        '2sigma': 6.18, # 95.45%
+        '0.99': 9.21,
+        '3sigma': 11.83, #  99.73%
+    }
+
+    def __init__(self, data_map: Union[pd.DataFrame, Dict[str, pd.DataFrame]],
+                 label_map: Optional[Dict] = None,
+                 styles_map: Optional[Dict] = None,
+                 config_map: Optional[Dict] = None,
+                 color_cycle=None,
+                 styles: Optional[Union[Dict, str]] = None,
+                 analysis_label_options: Optional[Dict] = None,
+                 config: Optional[Dict] = None):
+
+        self.data_map = data_map
+        self.label_map = label_map
+        self.styles_map = styles_map
+        self.config_map = config_map
+        self.highlight_data = []
+        self.legend_order = []
+        self.contours = None
+
+        super().__init__(color_cycle=color_cycle,
+                         styles=styles,
+                         analysis_label_options=analysis_label_options,
+                         config=config)
+
     def get_default_legend_order(self):
-        return []
-    
-    def update_legend_handles(self, handles:Dict, sec:bool=False,
-                              idx:Optional[int]=None):
-        if idx is None:
-            if not sec:
-                legend_data = self.legend_data
-            else:
-                legend_data = self.legend_data_sec
+        if not isinstance(self.data_map, dict):
+            return self.legend_order
         else:
-            if idx not in self.legend_data_ext:
-                self.legend_data_ext[idx] = {}
-            legend_data = self.legend_data_ext[idx]
-            
-        for key in handles:
-            handle = handles[key]
-            if isinstance(handle, matplotlib.container.Container):
-                label = handle.get_label()
-            elif isinstance(handle, (tuple, list)):
-                label = handle[0].get_label()
-            else:
-                label = handle.get_label()               
-            if label and not label.startswith('_'):
-                legend_data[key] = {
-                    'handle': handle,
-                    'label': label
-                }
-            else:
-                raise RuntimeError(f"the handle {handle} does not have an associated label")
-                
-    def add_legend_decoration(self, decorator, targets:List[str]):
-        for key, legend_data in self.legend_data.items():
-            if key not in targets:
-                continue
-            handle = legend_data["handle"]
-            if isinstance(handle, tuple):
-                new_handle = (*handle, decorator)
-            else:
-                new_handle = (handle, decorator)
-            legend_data["handle"] = new_handle
+            return list(self.data_map)
+
+    def draw_single_data(self, ax, data: pd.DataFrame,
+                         xattrib: str, yattrib: str, zattrib: str = 'qmu',
+                         styles: Optional[Dict] = None,
+                         config: Optional[Dict] = None,
+                         clabel_size=None, show_colormesh=False):
+        if config is None:
+            config = self.config
+        colors = list(config['sigma_colors'])
+        if 'sigma_linestyles' not in config:
+            config['sigma_linestyles'] = ['solid'] * \
+                len(list(config['sigma_colors']))
+        linestyles = list(config['sigma_linestyles'])
+        levels = [self.likelihood_label_threshold[key]
+                        for key in config['sigma_levels']]
+        if config['interpolation'] is not None:
+            from scipy import interpolate
+            x = data[xattrib]
+            y = data[yattrib]
+            z = data[zattrib]
+
+            def get_grid(X_range, Y_range, num_grid_points):
+                X_points = np.linspace(*X_range, num_grid_points)
+                Y_points = np.linspace(*Y_range, num_grid_points)
+                X_grid, Y_grid = np.meshgrid(X_points, Y_points)
+                return X_grid, Y_grid
+            X, Y = get_grid(X_range=(x.min(), x.max()), Y_range=(
+                y.min(), y.max()), num_grid_points=config['num_grid_points'])
+            Z = interpolate.griddata(
+                np.stack((x, y), axis=1), z, (X, Y), method=config['interpolation'])
+        else:  # buggy for [dict]
+            X_unique = np.sort(self.data_map[xattrib].unique())
+            Y_unique = np.sort(self.data_map[yattrib].unique())
+            X, Y = np.meshgrid(X_unique, Y_unique)
+            Z = self.data_map.pivot_table(
+                index=xattrib, columns=yattrib, values=zattrib).T.values - self.data_map[zattrib].min()
+
+        if show_colormesh:
+            cmap = config['cmap']
+            im = ax.pcolormesh(X, Y, Z, cmap=cmap, shading='auto')
+            import matplotlib.pyplot as plt
+            self.cbar = plt.colorbar(im, ax=ax, **config['colorbar'])
+            self.cbar.set_label(**config['colorbar_label'])
+        if levels:
+            cp = ax.contour(X, Y, Z, levels=levels, colors=colors,
+                        linestyles=linestyles, linewidths=3)
+            if clabel_size is not None:
+                ax.clabel(cp, inline=True, fontsize=clabel_size)
+        custom_handles = [Line2D([0], [0], color=color, linestyle=linestyle, lw=3, label=label) \
+                          for color, key, label, linestyle in \
+                          zip(config['sigma_colors'], config['sigma_levels'], config['sigma_names'], config['sigma_linestyles'])]
+        self.update_legend_handles(
+            dict(zip(config['sigma_names'], custom_handles)))
+        self.legend_order.extend(config['sigma_names'])
+        return custom_handles
 
-    def get_legend_handles_labels(self, sec:bool=False,
-                                  idx:Optional[Union[int, List[int]]]=None):
-        handles = []
-        labels = []
-        if idx is None:
-            if not sec:
-                legend_data = self.legend_data
+    def draw(self, xattrib: str, yattrib: str, zattrib: str = 'qmu', xlabel: Optional[str] = "",
+             ylabel: Optional[str] = "", zlabel: Optional[str] = "$-2\Delta ln(L)$",
+             ymax: float = 5, ymin: float = -5, xmin: Optional[float] = -10, xmax: Optional[float] = 10,
+             clabel_size=None, draw_sm_line: bool = False, draw_bestfit:bool=True,
+             show_colormesh=False, show_legend=True):
+        ax = self.draw_frame()
+        self.contours = {'keys': [], 'contours': [], 'levels': []}
+        if isinstance(self.data_map, pd.DataFrame):
+            self.draw_single_data(ax, self.data_map, xattrib=xattrib, yattrib=yattrib,
+                                  zattrib=zattrib, styles=self.styles_map, config=self.config,
+                                  clabel_size=clabel_size, show_colormesh=show_colormesh)
+        elif isinstance(self.data_map, dict):
+            if self.styles_map is None:
+                styles_map = {k: None for k in self.data_map}
+            else:
+                styles_map = self.styles_map
+            if self.label_map is None:
+                label_map = {k: k for k in self.data_map}
+            else:
+                label_map = self.label_map
+            if self.config_map is None:
+                config_map = {k: k for k in self.data_map}
             else:
-                legend_data = self.legend_data_sec        
-            for key in self.legend_order:
-                if key in legend_data:
-                    handle = legend_data[key]['handle']
-                    label = legend_data[key]['label']
-                    handles.append(handle)
-                    labels.append(label)
+                config_map = self.config_map
+                
+            for key in self.data_map:
+                self.contours['keys'].append(key)
+                data = self.data_map[key]
+                styles = styles_map.get(key, None)
+                label = label_map.get(key, "")
+                config = config_map.get(key, None)
+                config = combine_dict(self.CONFIG, config)
+                handle = self.draw_single_data(ax, data,
+                                               xattrib=xattrib,
+                                               yattrib=yattrib,
+                                               zattrib=zattrib,
+                                               styles=styles,
+                                               config=config,
+                                               show_colormesh=show_colormesh)
         else:
-            if isinstance(idx, int):
-                indices = [idx]
-            else:
-                indices = idx
-            for index in indices:
-                legend_data = self.legend_data_ext[index]
-                for key in self.legend_order:
-                    if key in legend_data:
-                        handle = legend_data[key]['handle']
-                        label = legend_data[key]['label']
-                        handles.append(handle)
-                        labels.append(label)
-        return handles, labels
-    
-    def draw_frame(self, frame_method:Callable=None, **kwargs):
-        if frame_method is None:
-            frame_method = single_frame
-        ax = frame_method(styles=self.styles,
-                          prop_cycle=get_color_cycle(self.cmap),
-                          analysis_label_options=self.analysis_label_options,
-                          figure_index=self.figure_index,
-                          **kwargs)
-        for annotation_kwargs in self.annotation_list:
-            annotation_kwargs = combine_dict(self.styles['annotation'], annotation_kwargs)
-            if isinstance(ax, tuple):
-                ax[0].annotate(**annotation_kwargs)
-            else:
-                ax.annotate(**annotation_kwargs)
-        self.figure = matplotlib.pyplot.gcf()
-        return ax
-    
-    def draw_axis_labels(self, ax, xlabel:Optional[str]=None, ylabel:Optional[str]=None,
-                         xlabellinebreak:Optional[int]=None, ylabellinebreak:Optional[int]=None):
-        if xlabel is not None:
-            if (xlabellinebreak is not None) and (xlabel.count("$") < 2):
-                xlabel = insert_periodic_substr(xlabel, xlabellinebreak)
-            ax.set_xlabel(xlabel, **self.styles['xlabel'])
-        if ylabel is not None:
-            if (ylabellinebreak is not None) and (ylabel.count("$") < 2):
-                ylabel = insert_periodic_substr(ylabel, ylabellinebreak)            
-            ax.set_ylabel(ylabel, **self.styles['ylabel'])
-            
-    def draw_axis_components(self, ax, xlabel:Optional[str]=None, ylabel:Optional[str]=None,
-                             ylim:Optional[Tuple[float]]=None, xlim:Optional[Tuple[float]]=None,
-                             xticks:Optional[List]=None, yticks:Optional[List]=None,
-                             xticklabels:Optional[List]=None, yticklabels:Optional[List]=None):
+            raise ValueError("invalid data format")
         
-        self.draw_axis_labels(ax, xlabel, ylabel,
-                              xlabellinebreak=self.config["xlabellinebreak"],
-                              ylabellinebreak=self.config["ylabellinebreak"],)
+        highlight_index = 0
         
-        format_axis_ticks(ax, **self.styles['axis'],
-                          xtick_styles=self.styles['xtick'],
-                          ytick_styles=self.styles['ytick'])
-        
-        if ylim is not None:
-            ax.set_ylim(*ylim)
-        if xlim is not None:
-            ax.set_xlim(*xlim)
-        if xticks is not None:
-            ax.set_xticks(xticks)
-        if yticks is not None:
-            ax.set_yticks(yticks)
-        if xticklabels is not None:
-            ax.set_xticklabels(xticklabels)
-        if yticklabels is not None:
-            ax.set_yticklabels(yticklabels)                
-    
-    def set_axis_range(self, ax,
-                       xmin:Optional[float]=None, xmax:Optional[float]=None,
-                       ymin:Optional[float]=None, ymax:Optional[float]=None,
-                       ypad:Optional[float]=None):
-        xlim = list(ax.get_xlim())
-        ylim = list(ax.get_ylim())
-        if xmin is not None:
-            xlim[0] = xmin
-        if xmax is not None:
-            xlim[1] = xmax
-        if ypad is not None:
-            if (ymax is not None):
-                raise ValueError('can not use both "ypad" and "ymax" when setting axis range')
-            if ypad < 0 or ypad > 1:
-                raise ValueError('"ypad" must be between 0 and 1')
-            ylim[1] = ylim[1] / (1 - ypad)
-        if ymin is not None:
-            ylim[0] = ymin
-        if ymax is not None:
-            ylim[1] = ymax                
-        ax.set_xlim(*xlim)
-        ax.set_ylim(*ylim)
-    
-    @staticmethod
-    def close_all_figures():
-        matplotlib.pyplot.close()
+        if draw_bestfit and isinstance(self.data_map, pd.DataFrame):
+            bestfit_idx = np.argmin(self.data_map[zattrib].values)
+            bestfit_x   = self.data_map.iloc[bestfit_idx][xattrib]
+            bestfit_y   = self.data_map.iloc[bestfit_idx][yattrib]
+            highlight_data = {
+                'x': bestfit_x,
+                'y': bestfit_y,
+                'label': self.config["bestfit_label"].format(x=bestfit_x, y=bestfit_y),
+                'styles': self.config["bestfit_styles"]
+            }
+            self.draw_highlight(ax, highlight_data, highlight_index)
+            highlight_index += 1
+        
+        if self.highlight_data is not None:
+            for i, h in enumerate(self.highlight_data):
+                self.draw_highlight(ax, h, highlight_index + i)
+
+        if draw_sm_line:
+            sm_line_styles = self.config['sm_line_styles']
+            sm_values = self.config['sm_values']
+            transform = create_transform(
+                transform_y="axis", transform_x="data")
+            ax.vlines(sm_values[0], ymin=0, ymax=1, zorder=0, transform=transform,
+                      **sm_line_styles)
+            transform = create_transform(
+                transform_x="axis", transform_y="data")
+            ax.hlines(sm_values[1], xmin=0, xmax=1, zorder=0, transform=transform,
+                      **sm_line_styles)
+
+        if show_legend:
+            handles, labels = self.get_legend_handles_labels()
+            ax.legend(handles, labels, **self.styles['legend'])
+
+        self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel)
+        self.set_axis_range(ax, xmin=xmin, xmax=xmax, ymin=ymin, ymax=ymax)
+
+        return ax
+
+    def draw_highlight(self, ax, data, index=0):
+        styles = data['styles']
+        if styles is None:
+            styles = self.config['highlight_styles']
+        handle = ax.plot(data['x'], data['y'], label=data['label'], **styles)
+        self.update_legend_handles({f'highlight_{index}': handle[0]})
+        self.legend_order.append(f'highlight_{index}')
+
+    def add_highlight(self, x: float, y: float, label: str = "SM prediction",
+                      styles: Optional[Dict] = None):
+        highlight_data = {
+            'x': x,
+            'y': y,
+            'label': label,
+            'styles': styles
+        }
+        self.highlight_data.append(highlight_data)
```

### Comparing `quickstats-0.6.7.7/quickstats/plots/collective_data_plot.py` & `quickstats-0.6.7.8/quickstats/plots/collective_data_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/plots/color_schemes.py` & `quickstats-0.6.7.8/quickstats/plots/color_schemes.py`

 * *Files 16% similar despite different names*

```diff
@@ -62,9 +62,11 @@
     shading_medium=["#E0DCC5", "#C5E00C", "#E0C5D4", "#C5C5E0"],
     shading_dark=["#C1B98A", "#8AC199", "#C18AA9", "#8B8AC1"],
     ibm=["#648fff", "#785ef0", "#dc267f", "#fe6100", "#ffb000"],
     butterflycore=["#f4cccc", "#ffe599", "#b6d7a8", "#9fc5e8", "#9C98DB", "#D6BFAB", "#876659"],
     simple_contrast=["#ED553B", "#20639B", "#3CAEA3", "#F6D55C", "#BF51A0", "#735245"],
     checker=["#068EAC", "#DE5B7D", "#4A9451", "#F97623", "#FAE215", "#BF51A0",
              "#84E4D0", "#B32A32", "#ADE85B", "#FFA41A", "#505BB6", "#596D3D",
-             "#2C388E", "#5B3F7B", "#8D89C2", "#6586B3", "#CCA18D", "#735245"]
+             "#2C388E", "#5B3F7B", "#8D89C2", "#6586B3", "#CCA18D", "#735245"],
+    atlas_hdbs=["#047cbc", "#283044", "#ebf5ee", "#fa7e61", "#ca1551", "#b8336a"],
+    atlas_hh=["#f2385a", "#343844", "#36b1bf", "#4ad9d9", "#e9f1df", "#fdc536", "#125125"]
 )
```

### Comparing `quickstats-0.6.7.7/quickstats/plots/core.py` & `quickstats-0.6.7.8/quickstats/plots/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,37 @@
 from typing import List, Dict, Optional, Union
 from cycler import cycler
 
 import numpy as np
 
+from quickstats import DescriptiveEnum
+
+class ErrorDisplayFormat(DescriptiveEnum):
+    ERRORBAR = (0, "Error bar", "errorbar")
+    FILL     = (1, "Fill interpolated error range across bins", "fill_between")
+    SHADE    = (2, "Shade error range in each bin", "bar")
+    
+    def __new__(cls, value:int, description:str="", mpl_method:str=""):
+        obj = object.__new__(cls)
+        obj._value_ = value
+        obj.description = description
+        obj.mpl_method = mpl_method
+        return obj
+    
+class PlotFormat(DescriptiveEnum):
+    ERRORBAR = (0, "Error bar", "errorbar")
+    HIST     = (1, "Histogram", "hist")
+                
+    def __new__(cls, value:int, description:str="", mpl_method:str=""):
+        obj = object.__new__(cls)
+        obj._value_ = value
+        obj.description = description
+        obj.mpl_method = mpl_method
+        return obj
+
 def set_attrib(obj, **kwargs):
     for key, value in kwargs.items():
         target = obj
         if '.' in key:
             tokens = key.split('.')
             if len(tokens) != 2:
                 raise ValueError('maximum of 1 subfield is allowed but {} is given'.format(len(tokens)-1))
```

### Comparing `quickstats-0.6.7.7/quickstats/plots/correlation_plot.py` & `quickstats-0.6.7.8/quickstats/plots/correlation_plot.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,25 +34,32 @@
         _style = STYLES.get(style.lower(), None)
         if not _style:
             raise ValueError(f'unknown style: {style}')
         return _style
         
     def draw(self, cmap:str='seismic', xlabel_rotation:float=90, ylabel_rotation:float=0, label_size:float=25,
               figscale:int=1, show_values:bool=True, value_color:str="black", value_size=16, value_precision:int=2,
-              gridline:Optional[str]="--", gridcolor:str="black"):
+              gridline:Optional[str]="--", gridcolor:str="black", xlabelpad:Optional[float]=None,
+              ylabelpad:Optional[float]=None):
         plt.clf()
         size = len(self.data)
         figsize = size * figscale
         fig, ax = plt.subplots(nrows=1, ncols=1, figsize=(figsize, figsize), facecolor= "#FFFFFF", dpi=72)
         ax.matshow(self.data, cmap=cmap, vmin=-1, vmax=1)
         ticks = np.arange(0, len(self.data), 1)
         ax.set_xticks(ticks)
         ax.set_yticks(ticks)
-        ax.set_xticklabels(self.data.columns, rotation=xlabel_rotation, fontsize=label_size)
-        ax.set_yticklabels(self.data.index, rotation=ylabel_rotation, fontsize=label_size)
+        ax.set_xticklabels(self.data.columns, rotation=xlabel_rotation,
+                           fontsize=label_size)
+        if xlabelpad is not None:
+            ax.tick_params(axis='x', which='major', pad=xlabelpad)
+        ax.set_yticklabels(self.data.index, rotation=ylabel_rotation,
+                           fontsize=label_size)
+        if ylabelpad is not None:
+            ax.tick_params(axis='y', which='major', pad=ylabelpad)
         ax.tick_params(axis="both", which="both", length=0)
         if show_values:
             fmt_str = f'{{:0.{value_precision}f}}'
             for (i, j), z in np.ndenumerate(self.data.values):
                 ax.text(j, i, fmt_str.format(z), ha='center', va='center', color=value_color, fontsize=value_size)
         if gridline:
             for i in range(len(ticks) - 1):
```

### Comparing `quickstats-0.6.7.7/quickstats/plots/general_1D_plot.py` & `quickstats-0.6.7.8/quickstats/plots/general_1D_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,18 @@
             stat_handles = None
         return handle[0], stat_handles
     
     def draw(self, xattrib:str, yattrib:str, targets:Optional[List[str]]=None,
              xlabel:Optional[str]=None, ylabel:Optional[str]=None,
              ymin:Optional[float]=None, ymax:Optional[float]=None,
              xmin:Optional[float]=None, xmax:Optional[float]=None,
+             logx:bool=False, logy:bool=False,
              draw_stats:bool=True):
         
-        ax = self.draw_frame()
+        ax = self.draw_frame(logx=logx, logy=logy)
         
         legend_order = []
         if isinstance(self.data_map, pd.DataFrame):
             if draw_stats and (None in self.stat_configs):
                 stat_configs = self.stat_configs[None]
             else:
                 stat_configs = None
```

### Comparing `quickstats-0.6.7.7/quickstats/plots/general_distribution_plot.py` & `quickstats-0.6.7.8/quickstats/plots/general_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/plots/histo_1D_plot.py` & `quickstats-0.6.7.8/quickstats/plots/histo_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/plots/hypotest_inverter_plot.py` & `quickstats-0.6.7.8/quickstats/plots/hypotest_inverter_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,24 +106,26 @@
         if draw_CLsplusb:
             ax.errorbar(mu_values, CLsplusb, yerr=CLsplusbError, **self.styles['errorbar'], 
                         color=self.color_pallete['CLsplusb'], linestyle='dotted', 
                         label='Observed CLs+b')
 
     def draw(self, nsig:int=2, draw_CLs:bool=True, 
              draw_CLb:bool=True, draw_CLsplusb:bool=True,
-             ymax:float=0.55, draw_CL:bool=True):
+             ymax:float=0.55, draw_CL:bool=True,
+             draw_observed:bool=True):
         if nsig < 0 or nsig > 2:
             raise ValueError("nsig must be between 0 and 2")
             
         ax = self.draw_frame()
         
         self.draw_expected(ax, nsig=nsig)
-        self.draw_observed(ax, draw_CLs=draw_CLs,
-                           draw_CLb=draw_CLb,
-                           draw_CLsplusb=draw_CLsplusb)
+        if draw_observed:
+            self.draw_observed(ax, draw_CLs=draw_CLs,
+                               draw_CLb=draw_CLb,
+                               draw_CLsplusb=draw_CLsplusb)
         ax.set_xlabel("$\mu$", **self.styles['xlabel'])
         ax.set_ylabel("p value", **self.styles['ylabel'])
         
         ax.set_ylim(-0.01, ymax)
         n_entries = self.result.ArraySize()
         mu_list = []
         for i in range(n_entries):
@@ -142,11 +144,11 @@
         elif nsig == 1:
             handles[1].set_linewidth(1.0)
             handles = handles[2:] + [handles[0], (handles[1], border_leg)]
             labels = labels[2:] + [labels[0], labels[1]]
         elif nsig == 2:
             handles[1].set_linewidth(1.0)
             handles[2].set_linewidth(1.0)
-            handles = handles[3:] + [handles[0], (handles[1], border_leg), (handles[2], border_leg)]
+            handles = handles[3:] + [handles[0], handles[1], (handles[2], border_leg)]
             labels = labels[3:] + [labels[0], labels[1], labels[2]]
         ax.legend(handles, labels, loc='upper right', frameon=False, **self.styles['legend'])
         return ax
```

### Comparing `quickstats-0.6.7.7/quickstats/plots/likelihood_1D_plot.py` & `quickstats-0.6.7.8/quickstats/plots/likelihood_1D_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from quickstats.utils.common_utils import combine_dict
 
 class Likelihood1DPlot(General1DPlot):
     
     STYLES = {
         'annotation':{
             'fontsize': 20
-        }    
-    }    
+        }
+    }
     
     CONFIG = {
         'sigma_values': (1, 4),
         'sigma_pos': 0.93,
         'sigma_names': ('1 $\sigma$', '2 $\sigma$'),
         'sigma_line_styles':{
             'color': 'gray',
@@ -96,14 +96,15 @@
             ax.vlines(sm_values, ymin=0, ymax=1, zorder=0, transform=transform,
                       **sm_line_styles)
             if sm_names:
                 sm_pos = self.config['sm_pos']
                 for sm_value, sm_name in zip(sm_values, sm_names):
                     ax.text(sm_value, sm_pos, sm_name, color='gray', ha='right', rotation=90,
                             va='bottom' if (sm_pos > 0 and sm_pos < 1) else 'center', fontsize=20, transform=transform)
+        
         if draw_sigma_intervals:
             if isinstance(self.data_map, pd.DataFrame):
                 x = self.data_map[xattrib]
                 y = self.data_map[yattrib]
             elif isinstance(self.data_map, dict):
                 if not isinstance(draw_sigma_intervals, str):
                     raise RuntimeError("name of the target likelihood curve must be specified "
```

### Comparing `quickstats-0.6.7.7/quickstats/plots/np_ranking_plot.py` & `quickstats-0.6.7.8/quickstats/plots/np_ranking_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/plots/pdf_distribution_plot.py` & `quickstats-0.6.7.8/quickstats/plots/pdf_distribution_plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from quickstats.plots.template import suggest_markersize, ratio_frames, centralize_axis, create_transform
 from quickstats.utils.common_utils import combine_dict
 from quickstats import GeneralEnum
 
 class ErrorDisplayFormat(GeneralEnum):
     ERRORBAR = 0
     FILL     = 1
+    SHADE    = 2
 
 class PdfDistributionPlot(AbstractPlot):
     
     STYLES = {
         'errorbar': {
             "marker": 'o',
             "markersize": None,
@@ -46,17 +47,15 @@
         'ratio_line_styles':{
             'color': 'gray',
             'linestyle': '--'
         }        
     }
     
     def __init__(self, collective_data:Dict,
-                 blind_range:Optional[List[float]]=None,
                  plot_options:Optional[Dict]=None,
-                 scale_map:Optional[Dict]=None,
                  label_map:Optional[Dict]=None,
                  color_cycle:Optional[Dict]=None,
                  styles:Optional[Union[Dict, str]]=None,
                  analysis_label_options:Optional[Union[Dict, str]]=None,
                  figure_index:Optional[int]=None,
                  config:Optional[Dict]=None):
         super().__init__(color_cycle=color_cycle,
@@ -69,18 +68,14 @@
             self.plot_options = {}
         else:
             self.plot_options = plot_options
         if label_map is None:
             self.label_map = {}
         else:
             self.label_map = label_map
-        if scale_map is None:
-            self.scale_map = {}
-        else:
-            self.scale_map = scale_map
         self.colors = {}
         
         self.annotation = None
         
     def set_data(self, collective_data:Dict):
         self.collective_data = collective_data
         self.legend_order = list(collective_data.keys())
@@ -128,85 +123,92 @@
             return err[mask]
         
     def draw_single_data(self, ax, data, label:str, label_blind:Optional[str]=None,
                          blind_range:Optional[List[float]]=None,
                          plot_options:Optional[Dict]=None, show_error:bool=True,
                          error_format:Union[ErrorDisplayFormat, str]="error_bar",
                          error_styles:Optional[Dict]=None,
-                         scale_by:Optional[float]=None):
-        pdata = self.process_data(data, blind_range=blind_range, scale_by=scale_by)
+                         plot_type:str="errorbar"):
+        pdata = self.process_data(data, blind_range=blind_range)
         has_errorbar = not ((pdata['xerr'] is None) and (pdata['yerr'] is None))
         draw_blind = blind_range is not None
         if not has_errorbar:
-            combined_options = combine_dict(self.styles['plot'], plot_options)
-            combined_options['label'] = label
-            if draw_blind:
-                # draw sideband low
-                handle_sblo = ax.plot(pdata['x'][pdata['sideband_lo']], 
-                                      pdata['y'][pdata['sideband_lo']],
-                                      **combined_options)
-                # avoid going through internal color cycle for the three regions
-                combined_options['color'] = handle_sblo[0].get_color()
-                # draw sideband high
-                handle_sbhi = ax.plot(pdata['x'][pdata['sideband_hi']], 
-                                      pdata['y'][pdata['sideband_hi']],
-                                      **combined_options)
-                combined_options['linestyle'] = self.config['blind_linestyle']
-                if label_blind is None:
-                    combined_options['label'] = f"{label} (blind)"
+            if plot_type == "errorbar":
+                combined_options = combine_dict(self.styles['plot'], plot_options)
+                combined_options['label'] = label
+                if draw_blind:
+                    # draw sideband low
+                    handle_sblo = ax.plot(pdata['x'][pdata['sideband_lo']], 
+                                          pdata['y'][pdata['sideband_lo']],
+                                          **combined_options)
+                    # avoid going through internal color cycle for the three regions
+                    combined_options['color'] = handle_sblo[0].get_color()
+                    # draw sideband high
+                    handle_sbhi = ax.plot(pdata['x'][pdata['sideband_hi']], 
+                                          pdata['y'][pdata['sideband_hi']],
+                                          **combined_options)
+                    combined_options['linestyle'] = self.config['blind_linestyle']
+                    if label_blind is None:
+                        combined_options['label'] = f"{label} (blind)"
+                    else:
+                        combined_options['label'] = label_blind
+                    x_blind_plus_sideband_edge = [pdata['x'][pdata['sideband_lo']][-1]] + \
+                                                 list(pdata['x'][pdata['blind']]) + \
+                                                 [pdata['x'][pdata['sideband_hi']][0]]
+                    y_blind_plus_sideband_edge = [pdata['y'][pdata['sideband_lo']][-1]] + \
+                                                 list(pdata['y'][pdata['blind']]) + \
+                                                 [pdata['y'][pdata['sideband_hi']][0]]                
+                    handle_blind = ax.plot(x_blind_plus_sideband_edge, 
+                                           y_blind_plus_sideband_edge,
+                                           **combined_options)
+                    handle = [handle_sblo[0], handle_blind[0]]
                 else:
-                    combined_options['label'] = label_blind
-                x_blind_plus_sideband_edge = [pdata['x'][pdata['sideband_lo']][-1]] + \
-                                             list(pdata['x'][pdata['blind']]) + \
-                                             [pdata['x'][pdata['sideband_hi']][0]]
-                y_blind_plus_sideband_edge = [pdata['y'][pdata['sideband_lo']][-1]] + \
-                                             list(pdata['y'][pdata['blind']]) + \
-                                             [pdata['y'][pdata['sideband_hi']][0]]                
-                handle_blind = ax.plot(x_blind_plus_sideband_edge, 
-                                       y_blind_plus_sideband_edge,
-                                       **combined_options)
-                handle = [handle_sblo[0], handle_blind[0]]
-            else:
-                handle = ax.plot(pdata['x'], pdata['y'], **combined_options)
-                handle = handle[0]
-        else:
-            
-            combined_options = combine_dict(plot_options, {"label": label})
-            if combined_options.get('markersize', None) is None:
-                nbins = len(pdata['x'])
-                combined_options['markersize'] = suggest_markersize(nbins)
-                
-            if draw_blind:
-                x = pdata['x'][pdata['sideband']]
-                y = pdata['y'][pdata['sideband']]
-                xerr = self._get_selected_err(pdata['xerr'], pdata['sideband'])
-                yerr = self._get_selected_err(pdata['yerr'], pdata['sideband'])
-            else:
+                    handle = ax.plot(pdata['x'], pdata['y'], **combined_options)
+                    handle = handle[0]
+            elif plot_tye == "hist":
+                pass
+        else:
+            if plot_type == "errorbar":
+                combined_options = combine_dict(plot_options, {"label": label})
+                if combined_options.get('markersize', None) is None:
+                    nbins = len(pdata['x'])
+                    combined_options['markersize'] = suggest_markersize(nbins)
+
+                if draw_blind:
+                    x = pdata['x'][pdata['sideband']]
+                    y = pdata['y'][pdata['sideband']]
+                    xerr = self._get_selected_err(pdata['xerr'], pdata['sideband'])
+                    yerr = self._get_selected_err(pdata['yerr'], pdata['sideband'])
+                else:
+                    x = pdata['x']
+                    y = pdata['y']
+                    xerr = pdata['xerr']
+                    yerr = pdata['yerr']
+                if not show_error:
+                    error_format = None
+                handle = self._draw_data(ax, x, y, xerr, yerr,
+                                         plot_options=combined_options,
+                                         error_format=error_format,
+                                         error_styles=error_styles)
+            elif plot_type == "hist":
                 x = pdata['x']
                 y = pdata['y']
                 xerr = pdata['xerr']
                 yerr = pdata['yerr']
-            if not show_error:
-                error_format = None
-            handle = self._draw_data(ax, x, y, xerr, yerr,
-                                     plot_options=combined_options,
-                                     error_format=error_format,
-                                     error_styles=error_styles)
+                width = np.diff(x)[0]
+                combined_options = combine_dict(self.styles['bar'], plot_options)
+                combined_options['label'] = label
+                handle = ax.stairs(x, y, align='center', width=width, **combined_options)
         return handle
     
-    def process_data(self, data, blind_range:Optional[List[float]]=None,
-                     scale_by:Optional[float]=None):
+    def process_data(self, data, blind_range:Optional[List[float]]=None):
         processed_data = {}
         processed_data['x'] = data['x']
         processed_data['y'] = data['y']
         error_data = self.get_error_data(data)
-        if (scale_by is not None) and (scale_by != 1.):
-            if error_data['yerr'] is not None:
-                raise RuntimeError("scaling is not allowed for data points with error")
-            processed_data['y'] *= scale_by
         processed_data['xerr'] = error_data['xerr']
         processed_data['yerr'] = error_data['yerr']
         if blind_range is not None:
             x = processed_data['x']
             blind_min = blind_range[0]
             blind_max = blind_range[1]
             sideband_lo = (x <= blind_min)
@@ -220,15 +222,15 @@
     
     def _draw_data(self, ax, x:np.ndarray, y:np.ndarray,
                    xerr:Optional[np.ndarray]=None,
                    yerr:Optional[np.ndarray]=None,
                    plot_options:Optional[Dict]=None,
                    error_format:Optional[Union[ErrorDisplayFormat, str]]="error_bar",
                    error_styles:Optional[Dict]=None):
-        combined_options = combine_dict(plot_options, self.styles['errorbar'])
+        combined_options = combine_dict(self.styles['errorbar'], plot_options)
         if error_format is None:
             combined_options['elinewidth'] = 0
             combined_options['capsize'] = 0
             combined_options['capthick'] = 0
             handle = ax.errorbar(x, y, xerr=xerr, yerr=yerr,
                                  **combined_options)
         elif (error_format == ErrorDisplayFormat.ERRORBAR):
@@ -388,14 +390,15 @@
         }
 
     def draw(self, xlabel:str="", ylabel:str="",
              targets:Optional[List]=None,
              logx:bool=False, logy:bool=False,
              blind_range:Optional[List[float]]=None,
              show_error:bool=True,
+             plot_type:str='errorbar',
              comparison_options:Optional[Union[Dict, List[Dict]]]=None,
              xmin:Optional[float]=None, xmax:Optional[float]=None,
              ymin:Optional[float]=None, ymax:Optional[float]=None,
              ypad:Optional[float]=None):
         
         if comparison_options is not None:
             ax, ax_ratio = self.draw_frame(ratio_frames, logx=logx, logy=logy,
@@ -406,42 +409,43 @@
         for name in self.collective_data:
             if (targets is not None) and(name not in targets):
                 continue
             data = self.collective_data[name]
             label = self.label_map.get(name, name)
             label_blind = self.label_map.get(f"{name}_blind", None)
             plot_options = self.plot_options.get(name, {})
-            scale_by = self.scale_map.get(name, None)
             if (name not in self.error_options) or \
                (self.error_options[name]["display_format"] is None):
                 error_format = None
                 error_styles = None
             else:
                 error_format = self.error_options[name]["display_format"]
                 error_styles = self.error_options[name]["styles"]
             handle = self.draw_single_data(ax, data, label,
                                            label_blind=label_blind,
                                            blind_range=blind_range,
                                            plot_options=plot_options,
                                            show_error=show_error,
                                            error_format=error_format,
                                            error_styles=error_styles,
-                                           scale_by=scale_by)
+                                           plot_type=plot_type)
+            if not handle.get_children():
+                    self.colors[name] = handle.get_color()
+            else:
+                if plot_type == 'errorbar':
+                    self.colors[name] = handle[0].get_color()
+                elif plot_type == 'hist':
+                    self.colors[name] = handle[0].get_edgecolor()
             # case draw blind
             if isinstance(handle, list) and len(handle) == 2:
                 blind_name = f"{name}_blind"
                 self.legend_order.append(blind_name)
                 self.update_legend_handles({name: handle[0], blind_name: handle[1]})
-                self.colors[name] = handle[0].get_color()
             else:
                 self.update_legend_handles({name: handle})
-                if not handle.get_children():
-                    self.colors[name] = handle.get_color()
-                else:
-                    self.colors[name] = handle[0].get_color()
 
         self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel)
         self.set_axis_range(ax, xmin=xmin, xmax=xmax, ymin=ymin, ymax=ymax, ypad=ypad)  
         handles, labels = self.get_legend_handles_labels()
         ax.legend(handles, labels, **self.styles['legend'])
         
         if comparison_options is not None:
@@ -452,31 +456,35 @@
                 target    = options['target']
                 mode      = options.get('mode', "ratio")
                 ylabel    = options.get('label', "")
                 labelsize = options.get('labelsize', None)
                 styles    = options.get('styles', {})
                 draw_ratio_line = options.get('draw_ratio_line', True)
                 plot_options = self.plot_options.get(target, {})
+                plot_options = combine_dict(plot_options, styles)
                 if ('color' not in plot_options) and (target in self.colors):
                     plot_options['color'] = self.colors[target]
                 plot_options.update(styles)
                 if (reference not in self.error_options) or \
                    (self.error_options[reference]["display_format"] is None):
                     error_format = None
                     error_styles = None
                 else:
                     error_format = self.error_options[reference]["display_format"]
                     error_styles = self.error_options[reference]["styles"]
+                comparison_show_error = options.get('show_error', None)
+                if comparison_show_error is None:
+                    comparison_show_error = show_error
                 self.draw_comparison(ax_ratio,
                                      self.collective_data[reference],
                                      self.collective_data[target],
                                      xlabel=ax.get_xlabel(),
                                      ylabel=ylabel, mode=mode,
                                      plot_options=plot_options,
-                                     show_error=show_error,
+                                     show_error=comparison_show_error,
                                      error_format=error_format,
                                      error_styles=error_styles,
                                      blind_range=blind_range,
                                      draw_ratio_line=draw_ratio_line)
                 if labelsize is not None:
                     ax_ratio.yaxis.label.set_size(labelsize)                
             ax.set(xlabel=None)
@@ -510,30 +518,29 @@
                                      n_bins_pdf=n_bins_pdf)
         plotter = cls(hist_data, **kwargs)
         return plotter
     
     @classmethod
     def from_dataframes(cls, collective_df:Dict[str, "pandas.DataFrame"],
                         observable:str, weight:Optional[Union[float, str]]=None,
-                        range:Optional[Union[List, Tuple]]=None,
-                        bins:int=10, normalize:bool=True,
+                        bin_range:Optional[Union[List, Tuple]]=None,
+                        nbins:int=10, normalize:bool=True,
                         x_scale:Optional[float]=None,                        
-                        error_method:str="auto", **kwargs):
+                        error_option:str="auto", **kwargs):
         from quickstats.maths.statistics import get_hist_data
         collective_data = {}
         for key, df in collective_df.items():
             x = df[observable].values 
             if x_scale is not None:
                 x = x * x_scale
             if weight is None:
                 weights = None
             elif isinstance(weight, numbers.Number):
                 weights = np.full(shape=len(df.index), fill_value=weight)
             else:
                 weights = df[weight].values
             hist_data = get_hist_data(x, weights, normalize=normalize,
-                                      range=range, bins=bins, error_method=error_method)
+                                      bin_range=bin_range, bins=nbins,
+                                      error_option=error_option)
             collective_data[key] = hist_data
         plotter = cls(collective_data, **kwargs)
-        return plotter
-        
-                        
+        return plotter
```

### Comparing `quickstats-0.6.7.7/quickstats/plots/sample_purity_plot.py` & `quickstats-0.6.7.8/quickstats/plots/sample_purity_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/plots/score_distribution_plot.py` & `quickstats-0.6.7.8/quickstats/plots/score_distribution_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class ScoreDistributionPlot(AbstractPlot):
     
     CONFIG = {
         "boundary_style": {
             "ymin": 0,
-            "ymax": 0.5,
+            "ymax": 0.4,
             "linestyle": "--",
             "color": "k"
         }
     }
     
     def __init__(self, data_map:Dict[str, pd.DataFrame], plot_options:Dict[str, Dict],
                  styles:Optional[Union[Dict, str]]=None,
@@ -30,28 +30,29 @@
                  config:Optional[Dict]=None):
         """
         Arguments:
             plot_options: dicionary
                 A dictionary containing plot options for various group of samples.
                 Format: { <sample_group>: {
                             "samples": <list of sample names>,
-                            "style": <options in mpl.hist>},
+                            "styles": <options in mpl.hist>},
                             "type": "hist" or "errorbar"
                           ...}
              
         """
         self.data_map = data_map
         self.plot_options = plot_options
         super().__init__(styles=styles,
                          analysis_label_options=analysis_label_options,
                          config=config)
     
     def draw(self, column_name:str="score", weight_name:Optional[str]="weight",
              xlabel:str="Score", ylabel:str="Fraction of Events / {bin_width:.2f}",
-             boundaries:Optional[List]=None, nbins:int=25, xmin:float=0, xmax:float=1):
+             boundaries:Optional[List]=None, nbins:int=25, xmin:float=0, xmax:float=1,
+             ymin:float=0, ymax:float=1, logy:bool=False):
         """
         
         Arguments:
             column_name: string, default = "score"
                 Name of the score variable in the dataframe.
             weight_name: (optional) string, default = "weight"
                 If specified, normalize the histogram by the "weight_name" variable
@@ -64,19 +65,25 @@
                 If specified, draw score boundaries at given values.
             nbins: int, default = 25
                 Number of histogram bins.
             xmin: float, default = 0
                 Minimum value of x-axis.
             xmax: float, default = 1
                 Maximum value of x-axis.
+            ymin: float, default = 0
+                Minimum value of y-axis.
+            ymax: float, default = 1
+                Maximum value of y-axis.
+            logy: bool, default = False
+                Draw y-axis with log scale.
         """
-        ax = self.draw_frame()
+        ax = self.draw_frame(logy=logy)
         for key in self.plot_options:
             samples = self.plot_options[key]["samples"]
-            plot_style  = self.plot_options[key].get("style", {})
+            plot_style  = self.plot_options[key].get("styles", {})
             df = pd.concat([self.data_map[sample] for sample in samples], ignore_index = True)
             if weight_name is not None:
                 norm_weights = df[weight_name] / df[weight_name].sum()
             else:
                 norm_weights = None
             plot_type = self.plot_options[key].get("type", "hist")
             if plot_type == "hist":
@@ -95,18 +102,19 @@
             else:
                 raise RuntimeError(f'unknown plot type: {plot_type}')
                 
         bin_width = (xmax - xmin) / nbins
         ylabel = ylabel.format(bin_width=bin_width)
         
         self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel)
-        self.set_axis_range(ax, xmin=xmin, xmax=xmax)
+        self.set_axis_range(ax, xmin=xmin, xmax=xmax, ymin=ymin, ymax=ymax)
         
-        ax.yaxis.set_major_locator(MaxNLocator(prune='lower', steps=[10]))
-        ax.xaxis.set_major_locator(MaxNLocator(steps=[10]))
+        if not logy:
+            ax.yaxis.set_major_locator(MaxNLocator(prune='lower', steps=[10]))
+            ax.xaxis.set_major_locator(MaxNLocator(steps=[10]))
 
         handles, labels = ax.get_legend_handles_labels()
         new_handles = [Line2D([], [], c=h.get_edgecolor(), linestyle=h.get_linestyle(),
                               **self.styles['legend_Line2D']) if isinstance(h, Polygon) else h for h in handles]
         ax.legend(handles=new_handles, labels=labels, **self.styles['legend'])
         if boundaries is not None:
             for boundary in boundaries:
```

### Comparing `quickstats-0.6.7.7/quickstats/plots/stat_plot_config.py` & `quickstats-0.6.7.8/quickstats/plots/stat_plot_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/plots/template.py` & `quickstats-0.6.7.8/quickstats/plots/template.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,50 @@
 from typing import Optional, Union, Dict, List, Tuple
 from copy import deepcopy
 import re
 from cycler import cycler
+from contextlib import contextmanager
+
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.transforms as transforms
 from matplotlib.patches import Rectangle
 from matplotlib.lines import Line2D
 from matplotlib.ticker import (MultipleLocator, FormatStrFormatter,
                                AutoMinorLocator, ScalarFormatter,
                                Locator, Formatter, AutoLocator,
                                MaxNLocator)
 
 from quickstats.utils.common_utils import update_nested_dict
+from quickstats import DescriptiveEnum
 
+class ResultStatus(DescriptiveEnum):
+    
+    FINAL    = (0, "Finalised results", "")
+    INT      = (1, "Internal results", "Internal")
+    WIP      = (2, "Work in progress results", "Work in Progress")
+    PRELIM   = (3, "Preliminary results", "Preliminary")
+    OPENDATA = (4, "Open data results", "Open Data")
+
+    def __new__(cls, value:int, description:str="", display_text:str=""):
+        obj = object.__new__(cls)
+        obj._value_ = value
+        obj.description = description
+        obj.display_text = display_text
+        return obj
+        
 class NumericFormatter(ScalarFormatter):
     def __call__(self, x, pos=None):
         tmp_format = self.format
         if (x.is_integer() and abs(x) < 1e3):
             self.format = re.sub(r"1\.\d+f", r"1.0f", self.format)
         result = super().__call__(x, pos)
         self.format = tmp_format
         return result
 
-COLOR_PALLETE = ['#000000', '#F2385A', '#4AD9D9', '#FDC536', '#125125', '#E88EED', '#B68D40']
-
 TEMPLATE_STYLES = {
     'default': {
         'figure':{
             'figsize': (11.111, 8.333),
             'dpi': 72,
             'facecolor': "#FFFFFF"
         },
@@ -87,37 +103,43 @@
             "markersize": 0,
             "elinewidth": 1,
             "capsize": 2,
             "capthick": 1,
             "zorder": 1
         },
         'fill_between': {
+            "alpha": 0.5
         },
         'legend':{
             "fontsize": 20
         },
         'ratio_frames':{
             'height_ratios': (3, 1),
             'hspace': 0.07            
         },
         'barh': {
             'height': 0.5
+        },
+        'bar': {
         }
     }
 }
 
 ANALYSIS_OPTIONS = {
     'default': {
+        'status': 'int',
         'loc': (0.05, 0.95),
         'fontsize': 25
     },
-    'Run2': {
+    'ATLAS_Run2': {
+        'colab': 'ATLAS',
         'status': 'int', 
         'energy' : '13 TeV', 
-        'lumi' : 139,
+        'lumi' : "140 fb$^{-1}$",
+        'fontsize': 25
     }
 }
 
 AXIS_LOCATOR_MAPS = {
     'auto': AutoLocator,
     'maxn': MaxNLocator
 }
@@ -146,15 +168,15 @@
 def parse_analysis_label_options(options:Optional[Dict]=None):
     default_options = deepcopy(ANALYSIS_OPTIONS['default'])
     if options is None:
         options = default_styles
     elif isinstance(options, str):
         template_options = ANALYSIS_OPTIONS.get(options, None)
         if template_options is None:
-            raise ValueError(f"template analysis label options `{styles}` not found")
+            raise ValueError(f"template analysis label options `{options}` not found")
         options = update_nested_dict(default_options, deepcopy(template_options))
     else:
         options = update_nested_dict(default_options, deepcopy(options))
     return options
 
 def ratio_frames(height_ratios:Tuple[int]=(3, 1), hspace:float=0.07,
                  logx:bool=False, logy:bool=False, 
@@ -218,15 +240,14 @@
         draw_analysis_label(ax, text_options=styles['text'], **analysis_label_options)
         
     if prop_cycle is not None:
         ax.set_prop_cycle(prop_cycle)
     
     return ax
 
-
 def suggest_markersize(nbins:int):
     bin_max  = 200
     bin_min  = 40
     size_max = 8
     size_min = 2
     if nbins <= bin_min:
         return size_max
@@ -356,119 +377,139 @@
                                                      parse_transform(transform_y))
     return transform
 
 def get_box_dimension(box):
     axis = plt.gca()
     plt.gcf().canvas.draw()
     bb = box.get_window_extent()
-    points  = bb.transformed(axis.transAxes.inverted()).get_points().transpose()
+    points = bb.transformed(axis.transAxes.inverted()).get_points().transpose()
     xmin = np.min(points[0])
     xmax = np.max(points[0])
     ymin = np.min(points[1])
     ymax = np.max(points[1])
     return xmin, xmax, ymin, ymax
 
-def draw_sigma_bands(axis, ymax, height=1.0):
+def draw_sigma_bands(axis, ymax:float, height:float=1.0):
     # +- 2 sigma band
     axis.add_patch(Rectangle((-2, -height/2), 2*2, ymax + height/2, fill=True, color='yellow'))
     # +- 1 sigma band
     axis.add_patch(Rectangle((-1, -height/2), 1*2, ymax + height/2, fill=True, color='lime'))
     
-def draw_sigma_lines(axis, ymax, height=1.0, **styles):
+def draw_sigma_lines(axis, ymax:float, height:float=1.0, **styles):
     y = [-height/2, ymax*height - height/2]
     axis.add_line(Line2D([-1, -1], y, **styles))
     axis.add_line(Line2D([+1, +1], y, **styles))
     axis.add_line(Line2D([0, 0], y, **styles)) 
     
 def draw_hatches(axis, ymax, height=1.0, **styles):
     x_min    = axis.get_xlim()[0]
     x_max    = axis.get_xlim()[1]
     x_range  = x_max - x_min
     y_values = np.arange(0, height*ymax, 2*height) - height/2
     transform = create_transform(transform_x='axis', transform_y='data')
     for y in y_values:
         axis.add_patch(Rectangle((0, y), 1, 1, **styles, zorder=-1, transform=transform))
 
-def draw_text(axis, x, y, s, transform_x:str='axis', 
-              transform_y:str='axis', **styles):
-    current_axis = plt.gca()
-    plt.sca(axis)
-    transform = transforms.blended_transform_factory(parse_transform(transform_x), 
-                                                     parse_transform(transform_y))
-    text = axis.text(x, y, s, transform=transform, **styles)
-    xmin, xmax, ymin, ymax = get_box_dimension(text)
-    plt.sca(current_axis)
+def draw_text(axis, x:float, y:float, s:str,
+              transform_x:str='axis',
+              transform_y:str='axis',
+              **styles):
+    with change_axis(axis):
+        transform = create_transform(transform_x, transform_y)
+        text = axis.text(x, y, s, transform=transform, **styles)
+        xmin, xmax, ymin, ymax = get_box_dimension(text)
     return xmin, xmax, ymin, ymax
 
-
-def _draw_analysis_label(axis, loc=(0.05, 0.95), fontsize=25, extra='Internal',
-                     colab:str='ATLAS', transform_x='axis', transform_y='axis', 
-                     vertical_align='top', horizontal_align='left'):
+@contextmanager
+def change_axis(axis):
     current_axis = plt.gca()
     plt.sca(axis)
-    if vertical_align not in ['top', 'bottom']:
-        raise ValueError('only "top" or "bottom" vertical alignment is allowed')
-    if horizontal_align not in ['left', 'right']:
-        raise ValueError('only "left" or "right" horizontal alignment is allowed') 
-    transform = transforms.blended_transform_factory(parse_transform(transform_x), 
-                                                     parse_transform(transform_y))
-    x, y = loc
-    text_atlas = axis.text(x, y, colab, fontsize=fontsize, transform=transform,
-                           horizontalalignment=horizontal_align,
-                           verticalalignment=vertical_align,
-                           fontproperties={"weight":"bold", "style":"italic"})
-    xmin, xmax, ymin, ymax = get_box_dimension(text_atlas)
-    text_width = xmax - xmin
-    dx = text_width/15
-    text_extra = axis.text(xmax + dx, ymin, extra, fontsize=fontsize, transform=axis.transAxes,
-                           horizontalalignment='left', verticalalignment='bottom')
-    _, xmax, _, ymax = get_box_dimension(text_atlas)
+    yield
     plt.sca(current_axis)
-    return xmin, xmax, ymin, ymax
 
-def draw_analysis_label(axis, loc=(0.05, 0.95), fontsize=25, status:str='int',
+def draw_analysis_label(axis, loc=(0.05, 0.95), fontsize:float=25, status:str='int',
                         energy:Optional[str]=None, lumi:Optional[str]=None,
                         colab:str='ATLAS', extra_text:Optional[str]=None, dy:float=0.05,
                         transform_x:str='axis', transform_y:str='axis',
+                        vertical_align:str='top', horizontal_align:str='left',
                         text_options:Optional[Dict]=None):
+    """
+    Draw analysis label and additional texts on a given axis.
     
-    if status == "final":
-        status_str = ""
-    elif status == "int":
-        status_str = "Internal"
-    elif status == "wip":
-        status_str = "Work in Progress"
-    elif status == "prelim":
-        status_str = "Preliminary"
-    elif status == "opendata":
-        status_str = "Open Data"
-    else:
-        status_str = status
+        Parameters
+        ---------------------------------------------------------------
+        axis: matplotlib.pyplot.axis
+            Axis to be drawn on.
+        loc: (float, float), default = (0.05, 0.95)
+            The location of the analysis label and additional texts.
+        fontsize: float, default = 25
+            Font size of the analysis label and the status label.
+        status: str or ResultStatus, default = 'int'
+            Display text for the analysis status. Certain keywords can be used to convert
+            automatically to the corresponding built-in status texts
+            (see `ResultStatus`).
+        energy: (optional) str
+            Display text for the Center-of-mass energy. A prefix of "\sqrt{s} = " will be
+            automatically appended to the front of the text.
+        lumi: (optional) str
+            Display text for the luminosity. It will be displayed as is.
+        colab: str
+            Display text for the collaboration involved in the analysis. It will be
+            bolded and italised.
+        extra_text: (optional) str
+            Extra text to be displayed after energy and luminosity texts. A new line
+            can be added by adding a double-slash, i.e. "//".
+        dy: float, default = 0.05
+            Vertical separation between each line of text in the axis coordinates.
+        transform_x: str, default = 'axis'
+            Coordinate transform for the x location of the analysis label.
+        transform_y: str, default = 'axis'
+            Coordinate transform for the y location of the analysis label.
+        vertical_align: str, default = 'top'
+            Vertical alignment of the analysis label.
+        horizontal_align: str, default = 'top'
+            Horizontal alignment of the analysis label.
+        text_options: (optional), dict
+            A dictionary specifying the styles for drawing texts.
+    """
+    try:
+        status_text = ResultStatus.parse(status).display_text
+    except:
+        status_text = status
+    
+    with change_axis(axis):
+        transform = create_transform(transform_x, transform_y)
+        x, y = loc
+        # draw collaboration label
+        text_colab = axis.text(x, y, colab, fontsize=fontsize, transform=transform,
+                               horizontalalignment=horizontal_align,
+                               verticalalignment=vertical_align,
+                               fontproperties={"weight":"bold", "style":"italic"})
+        xmin, xmax, ymin, _ = get_box_dimension(text_colab)
+        text_width = xmax - xmin
+        dx = text_width / 15
+        # draw status label
+        text_status = axis.text(xmax + dx, ymin, status_text, fontsize=fontsize,
+                                transform=axis.transAxes,
+                                horizontalalignment='left',
+                                verticalalignment='bottom')
         
-    xmin, xmax, ymin, ymax = _draw_analysis_label(axis, loc, fontsize, 
-                                                  extra=" "+status_str,
-                                                  colab=colab,
-                                                  transform_x=transform_x,
-                                                  transform_y=transform_y)
-
+    # draw energy and luminosity labels as well as additional texts
     elumi_text = []
     if energy is not None:
         elumi_text.append(r"$\sqrt{s} = $" + energy )
     if lumi is not None:
         elumi_text.append(lumi)
-
     elumi_text = ", ".join(elumi_text)
-    
-    texts = []
+
+    all_texts = []
     if elumi_text:
-        texts.append(elumi_text)
-        
+        all_texts.append(elumi_text)
+
     if extra_text is not None:
-        texts += extra_text.split("//")
-    
+        all_texts.extend(extra_text.split("//"))
+
     if text_options is None:
         text_options = {}
-    
-    for text in texts:
-        _, _, ymin, _ = draw_text(axis, xmin, ymin - dy, text, **text_options)
-        
-    return
+
+    for text in all_texts:
+        _, _, ymin, _ = draw_text(axis, xmin, ymin - dy, text, **text_options)
```

### Comparing `quickstats-0.6.7.7/quickstats/plots/test_statistic_distribution_plot.py` & `quickstats-0.6.7.8/quickstats/plots/test_statistic_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/plots/upper_limit_1D_plot.py` & `quickstats-0.6.7.8/quickstats/plots/upper_limit_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/plots/upper_limit_2D_plot.py` & `quickstats-0.6.7.8/quickstats/plots/upper_limit_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/plots/upper_limit_3D_plot.py` & `quickstats-0.6.7.8/quickstats/plots/upper_limit_3D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/plots/upper_limit_benchmark_plot.py` & `quickstats-0.6.7.8/quickstats/plots/upper_limit_benchmark_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/root_checker.py` & `quickstats-0.6.7.8/quickstats/root_checker.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/utils/common_utils.py` & `quickstats-0.6.7.8/quickstats/utils/common_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, Dict, List
+from typing import Optional, Union, Dict, List, Tuple
 import os
 import sys
 import copy
 import fnmatch
 import time
 import json
 import inspect
@@ -266,8 +266,33 @@
             return False  # Other type (?)
     except ImportError:
         return False
     except AttributeError:
         return False
     except NameError:
         return False      # Probably standard Python interpreter    
-    return True
+    return True
+
+def reindex_dataframe(df, index_values:Union[Tuple[List], List],
+                      index_levels:Optional[Union[Tuple[str], Tuple[int], str, int]]=None):
+    if not isinstance(index_values, tuple):
+        index_values = tuple([index_values])
+    if index_levels is None:
+        index_levels = tuple(range(len(index_values)))
+    if isinstance(index_levels, (str, int)):
+        index_levels = (index_levels,)
+    for values, level in zip(index_values, index_levels):
+        mask = np.in1d(values, df.index.get_level_values(level))
+        df = df.reindex(np.array(values)[mask], level=level)
+    return df
+
+def filter_dataframe_by_index_values(df, index_values:Union[Tuple[List], List],
+                                     index_levels:Optional[Union[Tuple[str], Tuple[int], str, int]]=None):
+    if not isinstance(index_values, tuple):
+        index_values = tuple([index_values])
+    if index_levels is None:
+        index_levels = tuple(range(len(index_values)))
+    if isinstance(index_levels, (int, str)):
+        index_levels = (index_levels,)
+    for values, level in zip(index_values, index_levels):
+        df = df.loc[df.index.get_level_values(level).isin(values)]
+    return df
```

### Comparing `quickstats-0.6.7.7/quickstats/utils/data_conversion.py` & `quickstats-0.6.7.8/quickstats/utils/data_conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
                   "long", "long long", "Long_t", "Long64_t",
                   "short", "Short_t", "Size_t", "UChar_t",
                   "UInt_t", "ULong64_t", "ULong_t",
                   "unsigned", "unsigned char", "unsigned int",
                   "unsigned long", "unsigned long long",
                   "unsigned short", "UShort_t"]
 
-uproot_datatypes = ["double", "float", "int", "int64_t", "char*", "int32_t", "uint64_t", "uint32_t"]
+uproot_datatypes = ["double", "float", "int", "int8_t", "int64_t", "char*", "int32_t", "uint64_t", "uint32_t"]
 
 class ConversionMode(DescriptiveEnum):
     ALL = (0, "Convert all variable types")
     REMOVE_NON_STANDARD_TYPE = (1, "Remove variables of non-standard type (i.e. other than bool, int, float, str, etc.)")
     REMOVE_NON_ARRAY_TYPE = (2, "Remove variables of non-standard type or not convertible to array of standard type")
 
 def get_default_library(custom_columns:bool=False):
```

### Comparing `quickstats-0.6.7.7/quickstats/utils/hep_utils.py` & `quickstats-0.6.7.8/quickstats/utils/hep_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/utils/io.py` & `quickstats-0.6.7.8/quickstats/utils/io.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/utils/roofit_utils.py` & `quickstats-0.6.7.8/quickstats/utils/roofit_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -433,15 +433,39 @@
     if len(kappas) == 1:
         return {"nominal": 1, "low":  round(kappas[0] - 1, 8), "high": round(kappas[0] - 1, 8), "type": "logn"}
     elif len(kappas) == 2:
         return {"nominal": 1, "low":  round(kappas[0] - 1, 8), "high": round(kappas[1] - 1, 8), "type": "asym"}
     else:
         raise RuntimeError(f'invalid kappa values for the systematic "{nuis_name}" from '
                            f'the ProcessNormalization client "{client.GetName()}"')
-            
+
+def get_response_function_variations(nuis:ROOT.RooRealVar, client):
+    result = {}
+    param_names = [param.GetName() for param in client.parameters()]
+    nuis_idx = param_names.index(nuis.GetName())
+    low_names = [param.GetName() for param in client.low()]
+    tokens = split_str(low_names[nuis_idx], '_', remove_empty=True)
+    client_name = "_".join(tokens[1:])
+    low_values = [param.getVal() for param in client.low()]
+    high_values = [param.getVal() for param in client.high()]
+    norm_values = [param for param in client.nominal()]
+    interp_codes = [param for param in client.interpolationCodes()]
+    norm_value, interp_code = round(norm_values[nuis_idx], 8), interp_codes[nuis_idx]
+    low_value, high_value = round(low_values[nuis_idx], 8), round(high_values[nuis_idx], 8)
+    result = {"client": client_name, "nominal": norm_value, "low": low_value, "high": high_value}
+    if interp_code == 0:
+        result['type'] = 'gaus'
+    elif interp_code == 1:
+        result['type'] = 'logn'
+    elif interp_code == 4:
+        result['type'] = 'asym'
+    else:
+        result['type'] = 'unknown'
+    return result
+    
 def get_systematic_variations_from_client(nuis:ROOT.RooRealVar, client):
     result = {"client": None, "nominal": None, "low": None, "high": None, "type": None}
     class_name = client.ClassName()
     nuis_name = nuis.GetName()
     # CMS dedicated normalization response function
     if class_name == "ProcessNormalization":
         result["client"] = client.GetName()
@@ -455,14 +479,16 @@
         parent_class_name = parent_client.ClassName()
         if isinstance(parent_client, ROOT.RooFormulaVar):
             result.update(get_logn_response_variations(nuis, parent_client))
         elif isinstance(parent_client, ROOT.RooAddition):
             result.update(get_gaus_response_variations(nuis, parent_client))
         elif isinstance(parent_client, ROOT.RooStats.HistFactory.FlexibleInterpVar):
             result.update(get_asym_response_variations(nuis, parent_client))
+    elif class_name == "ResponseFunction":
+        result = get_response_function_variations(nuis, client)
     return result
 
 def get_systematic_variations_from_clients(nuis:ROOT.RooRealVar, constr_pdf:ROOT.RooAbsPdf):
     constr_pdf_name = constr_pdf.GetName()
     clients = [c for c in nuis.clients() if c.GetName() != constr_pdf_name]
     result = {}
     for client in clients:
```

### Comparing `quickstats-0.6.7.7/quickstats/utils/roostats_utils.py` & `quickstats-0.6.7.8/quickstats/utils/roostats_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.7/quickstats/utils/string_utils.py` & `quickstats-0.6.7.8/quickstats/utils/string_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Optional, Callable
 import re
 
 whitespace_trans = str.maketrans('', '', " \t\r\n\v")
 
 def split_lines(string:str, comment_string:Optional[str]="#", remove_blank:bool=True,
-                with_line_number:bool=False):
-    lines = string.splitlines(True)
+                with_line_number:bool=False, keepends:bool=False):
+    lines = string.splitlines(keepends=keepends)
     # remove comments
     lines = [l.split(comment_string)[0] for l in lines]
     # remove blank lines
     if with_line_number:
         if remove_blank:
             return [(l, i+1) for i, l in enumerate(lines) if not re.match(r'^\s*$', l)]
         return [(l, i+1) for i, l in enumerate(lines)]
     if remove_blank:
-        lines = filter(lambda x: not re.match(r'^\s*$', x), lines)
+        lines = list(filter(lambda x: not re.match(r'^\s*$', x), lines))
     return lines
 
 
 def split_str(string:str, sep:str=None, strip:bool=True,
               remove_empty:bool=False, cast:Optional[Callable]=None):
     if strip:
         tokens = [s.strip() for s in string.strip().split(sep)]
```

### Comparing `quickstats-0.6.7.7/quickstats/utils/xml_tools.py` & `quickstats-0.6.7.8/quickstats/utils/xml_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,16 @@
         if not isinstance(source, dict):
             raise TypeError("source must be dict, not %s" % (
                 source.__class__.__name__,))
         tag = source['tag']
         attrib =source['attrib']
         xml_element = cls(tag, attrib)
         xml_element.text = source['text']
-        for sub_element in source:
+        for sub_element in source['children']:
             xml_element.append(cls.from_dict(sub_element))
-        
         return xml_element
     
     @classmethod
     def from_element(cls, source):
         if not isinstance(source, ET.Element):
             raise TypeError("source must be ElementTree.Element, not %s" % (
                 source.__class__.__name__,))
@@ -68,15 +67,20 @@
                                           level=level+1)
         return string
     
     
     def add_node(self, tag, attrib={}, text=None, tail=None, path=None, **extra):
         element = TXMLElement(tag, attrib, text, tail, **extra)
         self.append(element)
-        return element    
+        return element
+    
+    def add_comment(self, text:str):
+        comment = ET.Comment(text)
+        self.append(comment)
+        return comment
     
     def to_diagram(self, indent=' '*4, show_attrib=False):
         return self._to_diagram(self, indent=indent, show_attrib=show_attrib)
         
     def to_dict(self):
         return self._to_dict(self)
     
@@ -197,15 +201,23 @@
         element = TXMLElement(tag, attrib, text, tail, **extra)
         if path is None:
             root = self._root
         else:
             root = self._root.find(path)
         root.append(element)
         return element
-        
+    
+    def add_comment(self, text:str, path=None, **extra):
+        if self._root is None:
+            raise RuntimeError('root node is not initialized')
+        if path is None:
+            root = self._root
+        else:
+            root = self._root.find(path)
+        return root.add_comment(text)
         
     def set_root(self, element):
         if not isinstance(source, ET.Element):
             raise TypeError('root node must be ElementTree.Element, not %s' % (
                 element.__class__.__name__,))
         if not isinstance(source, TXMLElement):
             self._root = TXMLElement.from_element(source)
@@ -280,15 +292,20 @@
             self.write(f, 'utf-8', **kwargs)
             
     def to_dict(self):
         if self._root is None:
             return {}
         return self._root.to_dict()
     
-    @staticmethod
+    @classmethod
+    def from_dict(cls, dict_element):
+        instance = cls()
+        instance._root = TXMLElement.from_dict(dict_element)
+        return instance
+    
     def load_as_dict(filename:str):
         try:
             xml_dict = TXMLTree(file=filename).to_dict()
         except:
             raise RuntimeError(f'failed to load xml document "{filename}"')
         return xml_dict
```

### Comparing `quickstats-0.6.7.7/quickstats.egg-info/PKG-INFO` & `quickstats-0.6.7.8/quickstats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.6.7.7
+Version: 0.6.7.8
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.6.7.7/quickstats.egg-info/SOURCES.txt` & `quickstats-0.6.7.8/quickstats.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 quickstats/analysis/data_loading.py
 quickstats/analysis/data_preprocessing.py
 quickstats/analysis/event_categorization.py
 quickstats/analysis/multi_class_boundary_tree.py
 quickstats/analysis/ntuple_conversion_tool.py
 quickstats/analysis/ntuple_process_tool.py
 quickstats/analysis/sample_poly_param_tool.py
+quickstats/analysis/systematics/__init__.py
+quickstats/analysis/systematics/base_systematics.py
+quickstats/analysis/systematics/gaussian_shape_systematics.py
+quickstats/analysis/systematics/normalization_systematics.py
+quickstats/analysis/systematics/systematics_evaluation_tool.py
 quickstats/clis/__init__.py
 quickstats/clis/core.py
 quickstats/clis/inspect_rfile.py
 quickstats/clis/inspect_ws.py
 quickstats/clis/likelihood_fit.py
 quickstats/clis/likelihood_scan.py
 quickstats/clis/limit_setting.py
@@ -119,14 +124,15 @@
 quickstats/interface/cppyy/__init__.py
 quickstats/interface/cppyy/core.py
 quickstats/interface/cppyy/macros.py
 quickstats/interface/cppyy/vectorize.py
 quickstats/interface/root/RooAbsData.py
 quickstats/interface/root/RooAbsPdf.py
 quickstats/interface/root/RooArgSet.py
+quickstats/interface/root/RooCategory.py
 quickstats/interface/root/RooDataSet.py
 quickstats/interface/root/RooMsgService.py
 quickstats/interface/root/RooRealVar.py
 quickstats/interface/root/TArrayData.py
 quickstats/interface/root/TF1.py
 quickstats/interface/root/TFile.py
 quickstats/interface/root/TH1.py
@@ -149,20 +155,22 @@
 quickstats/macros/ResponseFunction/ResponseFunction.h
 quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
 quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
 quickstats/maths/__init__.py
 quickstats/maths/interpolation.py
 quickstats/maths/numerics.py
 quickstats/maths/statistics.py
+quickstats/maths/statistics_jitted.py
 quickstats/maths/symbolics.py
 quickstats/parsers/__init__.py
 quickstats/parsers/config_parser.py
 quickstats/parsers/param_parser.py
 quickstats/plots/__init__.py
 quickstats/plots/abstract_plot.py
+quickstats/plots/bidirectional_bar_chart.py
 quickstats/plots/collective_data_plot.py
 quickstats/plots/color_schemes.py
 quickstats/plots/core.py
 quickstats/plots/correlation_plot.py
 quickstats/plots/general_1D_plot.py
 quickstats/plots/general_distribution_plot.py
 quickstats/plots/histo_1D_plot.py
```

### Comparing `quickstats-0.6.7.7/setup.py` & `quickstats-0.6.7.8/setup.py`

 * *Files identical despite different names*


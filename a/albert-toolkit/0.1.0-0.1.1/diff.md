# Comparing `tmp/albert_toolkit-0.1.0.tar.gz` & `tmp/albert_toolkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "albert_toolkit-0.1.0.tar", max compression
+gzip compressed data, was "albert_toolkit-0.1.1.tar", max compression
```

## Comparing `albert_toolkit-0.1.0.tar` & `albert_toolkit-0.1.1.tar`

### file list

```diff
@@ -1,492 +1,492 @@
--rw-r--r--   0        0        0     6145 2023-03-21 20:52:07.491984 albert_toolkit-0.1.0/README.md
--rw-r--r--   0        0        0     2798 2023-04-10 18:31:28.978230 albert_toolkit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-31 20:03:24.700210 albert_toolkit-0.1.0/src/albert/__init__.py
--rw-r--r--   0        0        0     3688 2023-04-06 15:59:29.098549 albert_toolkit-0.1.0/src/albert/albert.py
--rw-r--r--   0        0        0      735 2023-03-14 15:56:43.726528 albert_toolkit-0.1.0/src/albert/api/__init__.py
--rw-r--r--   0        0        0    58500 2023-03-14 15:56:43.726667 albert_toolkit-0.1.0/src/albert/api/api_client.py
--rw-r--r--   0        0        0      214 2023-03-13 19:46:33.000000 albert_toolkit-0.1.0/src/albert/api/apis/__init__.py
--rw-r--r--   0        0        0     9535 2023-03-21 20:46:05.377307 albert_toolkit-0.1.0/src/albert/api/apis/path_to_api.py
--rw-r--r--   0        0        0      237 2023-03-13 19:46:32.000000 albert_toolkit-0.1.0/src/albert/api/apis/paths/__init__.py
--rw-r--r--   0        0        0      195 2023-03-21 20:46:05.376226 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_inventories.py
--rw-r--r--   0        0        0      128 2023-03-21 20:46:05.377222 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_inventories_health.py
--rw-r--r--   0        0        0      295 2023-03-21 20:46:05.376142 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_inventories_id.py
--rw-r--r--   0        0        0      189 2023-03-13 19:46:24.000000 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_locations.py
--rw-r--r--   0        0        0      211 2023-03-14 15:56:43.739587 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_locations_async_id.py
--rw-r--r--   0        0        0      124 2023-03-13 19:46:20.000000 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_locations_health.py
--rw-r--r--   0        0        0      287 2023-03-13 20:14:13.723672 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_locations_id.py
--rw-r--r--   0        0        0      195 2023-03-14 15:56:43.739388 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_predictions.py
--rw-r--r--   0        0        0      128 2023-03-14 15:56:43.739499 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_predictions_health.py
--rw-r--r--   0        0        0      135 2023-03-14 15:56:43.739662 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_predictions_mergedac.py
--rw-r--r--   0        0        0      135 2023-03-14 15:56:43.740248 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_predictions_mergedat.py
--rw-r--r--   0        0        0      215 2023-03-14 15:56:43.740316 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_predictions_models.py
--rw-r--r--   0        0        0      133 2023-03-14 15:56:43.740403 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_predictions_models_id.py
--rw-r--r--   0        0        0      380 2023-03-14 15:56:43.740963 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_predictions_models_parent_id_version.py
--rw-r--r--   0        0        0      166 2023-03-14 15:56:43.741196 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_predictions_models_parent_id_version_id.py
--rw-r--r--   0        0        0      139 2023-03-14 15:56:43.742325 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_predictions_parent_id.py
--rw-r--r--   0        0        0      129 2023-03-14 15:56:43.741941 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_predictions_tasks.py
--rw-r--r--   0        0        0      201 2023-03-14 15:56:43.742702 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_productdesign.py
--rw-r--r--   0        0        0      132 2023-03-14 15:56:43.741793 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_productdesign_health.py
--rw-r--r--   0        0        0      124 2023-03-14 15:56:43.742059 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_productdesign_id.py
--rw-r--r--   0        0        0      427 2023-03-14 15:56:43.742241 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_productdesign_id_designs.py
--rw-r--r--   0        0        0      133 2023-03-14 15:56:43.742137 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_productdesign_id_grid.py
--rw-r--r--   0        0        0      144 2023-03-14 15:56:43.741850 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_productdesign_id_products.py
--rw-r--r--   0        0        0      137 2023-03-14 15:56:43.742546 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_productdesign_id_unpack.py
--rw-r--r--   0        0        0      143 2023-03-14 15:56:43.752434 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_productdesign_id_values.py
--rw-r--r--   0        0        0      241 2023-03-14 15:56:43.752618 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_productdesign_inventories_id.py
--rw-r--r--   0        0        0      151 2023-03-14 15:56:43.752720 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_productdesign_mergeinventory.py
--rw-r--r--   0        0        0      132 2023-03-14 15:56:43.753024 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_productdesign_search.py
--rw-r--r--   0        0        0      134 2023-03-14 15:56:43.752809 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_productdesign_suggest.py
--rw-r--r--   0        0        0      183 2023-03-13 19:46:31.000000 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_reports.py
--rw-r--r--   0        0        0      131 2023-03-13 19:46:19.000000 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_reports_analytics_id.py
--rw-r--r--   0        0        0      119 2023-03-13 19:46:31.000000 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_reports_copy.py
--rw-r--r--   0        0        0      135 2023-03-13 19:46:19.000000 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_reports_datascience_id.py
--rw-r--r--   0        0        0      120 2023-03-13 19:46:20.000000 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_reports_health.py
--rw-r--r--   0        0        0      273 2023-03-13 20:14:13.728098 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_reports_id.py
--rw-r--r--   0        0        0      156 2023-03-13 20:14:13.728814 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_reports_inventory_equipment_usage.py
--rw-r--r--   0        0        0      145 2023-03-13 19:46:28.000000 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_reports_inventory_movements.py
--rw-r--r--   0        0        0      120 2023-03-13 19:46:32.000000 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_reports_search.py
--rw-r--r--   0        0        0      122 2023-03-13 19:46:30.000000 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_reports_suggest.py
--rw-r--r--   0        0        0      281 2023-03-13 20:14:13.729561 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_reports_type.py
--rw-r--r--   0        0        0      121 2023-03-13 19:46:28.000000 albert_toolkit-0.1.0/src/albert/api/apis/paths/api_v3_reports_type_id.py
--rw-r--r--   0        0        0     3003 2023-03-21 20:46:05.378651 albert_toolkit-0.1.0/src/albert/api/apis/tag_to_api.py
--rw-r--r--   0        0        0      838 2023-03-21 20:46:05.379448 albert_toolkit-0.1.0/src/albert/api/apis/tags/__init__.py
--rw-r--r--   0        0        0      658 2023-03-14 15:56:43.760379 albert_toolkit-0.1.0/src/albert/api/apis/tags/analytics_api.py
--rw-r--r--   0        0        0      538 2023-03-14 15:56:43.760471 albert_toolkit-0.1.0/src/albert/api/apis/tags/columns_api.py
--rw-r--r--   0        0        0      514 2023-03-14 15:56:43.760642 albert_toolkit-0.1.0/src/albert/api/apis/tags/default_api.py
--rw-r--r--   0        0        0      510 2023-03-14 15:56:43.760562 albert_toolkit-0.1.0/src/albert/api/apis/tags/grid_api.py
--rw-r--r--   0        0        0      854 2023-03-21 20:46:05.379320 albert_toolkit-0.1.0/src/albert/api/apis/tags/health_check_api.py
--rw-r--r--   0        0        0     1216 2023-03-14 15:56:43.760814 albert_toolkit-0.1.0/src/albert/api/apis/tags/internal_api.py
--rw-r--r--   0        0        0      898 2023-03-21 20:46:05.384851 albert_toolkit-0.1.0/src/albert/api/apis/tags/inventory_api.py
--rw-r--r--   0        0        0      876 2023-03-14 15:56:43.768745 albert_toolkit-0.1.0/src/albert/api/apis/tags/locations_api.py
--rw-r--r--   0        0        0      543 2023-03-14 15:56:43.768664 albert_toolkit-0.1.0/src/albert/api/apis/tags/prediction_flow_api.py
--rw-r--r--   0        0        0     1157 2023-03-14 15:56:43.768894 albert_toolkit-0.1.0/src/albert/api/apis/tags/prediction_models_api.py
--rw-r--r--   0        0        0      710 2023-03-14 15:56:43.769040 albert_toolkit-0.1.0/src/albert/api/apis/tags/predictions_api.py
--rw-r--r--   0        0        0      942 2023-03-14 15:56:43.769149 albert_toolkit-0.1.0/src/albert/api/apis/tags/product_design_api.py
--rw-r--r--   0        0        0      801 2023-03-14 15:56:43.769263 albert_toolkit-0.1.0/src/albert/api/apis/tags/reports_catalogue_api.py
--rw-r--r--   0        0        0      690 2023-03-14 15:56:43.772182 albert_toolkit-0.1.0/src/albert/api/apis/tags/reports_sp_api.py
--rw-r--r--   0        0        0      851 2023-03-14 15:56:43.771708 albert_toolkit-0.1.0/src/albert/api/apis/tags/rows_api.py
--rw-r--r--   0        0        0      516 2023-03-14 15:56:43.773369 albert_toolkit-0.1.0/src/albert/api/apis/tags/search_api.py
--rw-r--r--   0        0        0      522 2023-03-14 15:56:43.773239 albert_toolkit-0.1.0/src/albert/api/apis/tags/unpack_api.py
--rw-r--r--   0        0        0      931 2023-03-14 15:56:43.773977 albert_toolkit-0.1.0/src/albert/api/apis/tags/user_reports_api.py
--rw-r--r--   0        0        0      530 2023-03-14 15:56:43.774342 albert_toolkit-0.1.0/src/albert/api/apis/tags/values_api.py
--rw-r--r--   0        0        0    15750 2023-03-14 15:56:43.774891 albert_toolkit-0.1.0/src/albert/api/configuration.py
--rw-r--r--   0        0        0     4530 2023-03-14 15:56:43.775570 albert_toolkit-0.1.0/src/albert/api/exceptions.py
--rw-r--r--   0        0        0      344 2023-03-13 19:46:33.000000 albert_toolkit-0.1.0/src/albert/api/model/__init__.py
--rw-r--r--   0        0        0     7152 2023-03-14 15:56:43.776709 albert_toolkit-0.1.0/src/albert/api/model/add.py
--rw-r--r--   0        0        0     6682 2023-03-14 15:56:43.776330 albert_toolkit-0.1.0/src/albert/api/model/add.pyi
--rw-r--r--   0        0        0     4592 2023-03-14 15:56:43.776206 albert_toolkit-0.1.0/src/albert/api/model/cas.py
--rw-r--r--   0        0        0     4302 2023-03-14 15:56:43.776425 albert_toolkit-0.1.0/src/albert/api/model/cas.pyi
--rw-r--r--   0        0        0     9457 2023-03-14 15:56:43.776589 albert_toolkit-0.1.0/src/albert/api/model/column_copy_to_existing.py
--rw-r--r--   0        0        0     9266 2023-03-14 15:56:43.776799 albert_toolkit-0.1.0/src/albert/api/model/column_copy_to_existing.pyi
--rw-r--r--   0        0        0     9615 2023-03-14 15:56:43.777053 albert_toolkit-0.1.0/src/albert/api/model/column_copy_to_new.py
--rw-r--r--   0        0        0     9316 2023-03-14 15:56:43.776651 albert_toolkit-0.1.0/src/albert/api/model/column_copy_to_new.pyi
--rw-r--r--   0        0        0     2301 2023-03-14 15:56:43.776514 albert_toolkit-0.1.0/src/albert/api/model/columns.py
--rw-r--r--   0        0        0     2301 2023-03-14 15:56:43.776944 albert_toolkit-0.1.0/src/albert/api/model/columns.pyi
--rw-r--r--   0        0        0     4119 2023-03-14 15:56:43.779720 albert_toolkit-0.1.0/src/albert/api/model/component_input.py
--rw-r--r--   0        0        0     4119 2023-03-14 15:56:43.780161 albert_toolkit-0.1.0/src/albert/api/model/component_input.pyi
--rw-r--r--   0        0        0     2006 2023-03-14 15:56:43.780889 albert_toolkit-0.1.0/src/albert/api/model/copy_report.py
--rw-r--r--   0        0        0     2006 2023-03-14 15:56:43.781926 albert_toolkit-0.1.0/src/albert/api/model/copy_report.pyi
--rw-r--r--   0        0        0    11943 2023-03-14 15:56:43.782602 albert_toolkit-0.1.0/src/albert/api/model/data_model.py
--rw-r--r--   0        0        0    11519 2023-03-14 15:56:43.782066 albert_toolkit-0.1.0/src/albert/api/model/data_model.pyi
--rw-r--r--   0        0        0     8252 2023-03-14 15:56:43.783276 albert_toolkit-0.1.0/src/albert/api/model/default_columns.py
--rw-r--r--   0        0        0     8083 2023-03-14 15:56:43.782863 albert_toolkit-0.1.0/src/albert/api/model/default_columns.pyi
--rw-r--r--   0        0        0     7170 2023-03-14 15:56:43.782682 albert_toolkit-0.1.0/src/albert/api/model/delete.py
--rw-r--r--   0        0        0     6694 2023-03-14 15:56:43.784814 albert_toolkit-0.1.0/src/albert/api/model/delete.pyi
--rw-r--r--   0        0        0     4591 2023-03-14 15:56:43.784532 albert_toolkit-0.1.0/src/albert/api/model/denormalized_inventories.py
--rw-r--r--   0        0        0     4591 2023-03-14 15:56:43.783020 albert_toolkit-0.1.0/src/albert/api/model/denormalized_inventories.pyi
--rw-r--r--   0        0        0     7677 2023-03-14 15:56:43.782496 albert_toolkit-0.1.0/src/albert/api/model/denormalized_inventory.py
--rw-r--r--   0        0        0     7677 2023-03-14 15:56:43.784901 albert_toolkit-0.1.0/src/albert/api/model/denormalized_inventory.pyi
--rw-r--r--   0        0        0     8167 2023-03-14 15:56:43.785545 albert_toolkit-0.1.0/src/albert/api/model/designs.py
--rw-r--r--   0        0        0     7952 2023-03-14 15:56:43.785718 albert_toolkit-0.1.0/src/albert/api/model/designs.pyi
--rw-r--r--   0        0        0     2568 2023-03-14 15:56:43.789016 albert_toolkit-0.1.0/src/albert/api/model/entity_tags.py
--rw-r--r--   0        0        0     2568 2023-03-14 15:56:43.787750 albert_toolkit-0.1.0/src/albert/api/model/entity_tags.pyi
--rw-r--r--   0        0        0    12073 2023-03-14 15:56:43.789817 albert_toolkit-0.1.0/src/albert/api/model/equipment.py
--rw-r--r--   0        0        0    12073 2023-03-14 15:56:43.790448 albert_toolkit-0.1.0/src/albert/api/model/equipment.pyi
--rw-r--r--   0        0        0    12117 2023-03-14 15:56:43.791062 albert_toolkit-0.1.0/src/albert/api/model/error.py
--rw-r--r--   0        0        0    11792 2023-03-14 15:56:43.792119 albert_toolkit-0.1.0/src/albert/api/model/error.pyi
--rw-r--r--   0        0        0     8099 2023-03-14 15:56:43.792027 albert_toolkit-0.1.0/src/albert/api/model/facet_with_value_array.py
--rw-r--r--   0        0        0     8099 2023-03-14 15:56:43.792228 albert_toolkit-0.1.0/src/albert/api/model/facet_with_value_array.pyi
--rw-r--r--   0        0        0    12294 2023-03-14 15:56:43.792564 albert_toolkit-0.1.0/src/albert/api/model/formula_item.py
--rw-r--r--   0        0        0    12294 2023-03-14 15:56:43.792776 albert_toolkit-0.1.0/src/albert/api/model/formula_item.pyi
--rw-r--r--   0        0        0     3760 2023-03-14 15:56:43.792440 albert_toolkit-0.1.0/src/albert/api/model/get_back_update_companies.py
--rw-r--r--   0        0        0     3760 2023-03-14 15:56:43.798617 albert_toolkit-0.1.0/src/albert/api/model/get_back_update_companies.pyi
--rw-r--r--   0        0        0    36595 2023-03-14 15:56:43.798795 albert_toolkit-0.1.0/src/albert/api/model/grid.py
--rw-r--r--   0        0        0    35002 2023-03-14 15:56:43.792917 albert_toolkit-0.1.0/src/albert/api/model/grid.pyi
--rw-r--r--   0        0        0     3004 2023-03-14 15:56:43.807149 albert_toolkit-0.1.0/src/albert/api/model/health.py
--rw-r--r--   0        0        0     3004 2023-03-14 15:56:43.807231 albert_toolkit-0.1.0/src/albert/api/model/health.pyi
--rw-r--r--   0        0        0     4436 2023-03-14 15:56:43.807396 albert_toolkit-0.1.0/src/albert/api/model/inputs.py
--rw-r--r--   0        0        0     4436 2023-03-14 15:56:43.807311 albert_toolkit-0.1.0/src/albert/api/model/inputs.pyi
--rw-r--r--   0        0        0    19222 2023-03-21 20:46:05.384935 albert_toolkit-0.1.0/src/albert/api/model/inventories.py
--rw-r--r--   0        0        0    17436 2023-03-21 20:46:05.384741 albert_toolkit-0.1.0/src/albert/api/model/inventories.pyi
--rw-r--r--   0        0        0    13541 2023-03-21 20:46:05.385022 albert_toolkit-0.1.0/src/albert/api/model/inventory.py
--rw-r--r--   0        0        0    12217 2023-03-21 20:46:05.381651 albert_toolkit-0.1.0/src/albert/api/model/inventory.pyi
--rw-r--r--   0        0        0    15702 2023-03-14 15:56:43.812195 albert_toolkit-0.1.0/src/albert/api/model/location.py
--rw-r--r--   0        0        0    14824 2023-03-14 15:56:43.812727 albert_toolkit-0.1.0/src/albert/api/model/location.pyi
--rw-r--r--   0        0        0     4058 2023-03-14 15:56:43.819729 albert_toolkit-0.1.0/src/albert/api/model/locations.py
--rw-r--r--   0        0        0     4058 2023-03-14 15:56:43.820069 albert_toolkit-0.1.0/src/albert/api/model/locations.pyi
--rw-r--r--   0        0        0     5803 2023-03-14 15:56:43.820001 albert_toolkit-0.1.0/src/albert/api/model/merged_dac.py
--rw-r--r--   0        0        0     5630 2023-03-14 15:56:43.819815 albert_toolkit-0.1.0/src/albert/api/model/merged_dac.pyi
--rw-r--r--   0        0        0     5803 2023-03-14 15:56:43.820183 albert_toolkit-0.1.0/src/albert/api/model/merged_dat.py
--rw-r--r--   0        0        0     5630 2023-03-14 15:56:43.820410 albert_toolkit-0.1.0/src/albert/api/model/merged_dat.pyi
--rw-r--r--   0        0        0     5977 2023-03-14 15:56:43.820315 albert_toolkit-0.1.0/src/albert/api/model/merged_inventory.py
--rw-r--r--   0        0        0     5804 2023-03-14 15:56:43.819871 albert_toolkit-0.1.0/src/albert/api/model/merged_inventory.pyi
--rw-r--r--   0        0        0     3034 2023-03-21 20:46:05.385130 albert_toolkit-0.1.0/src/albert/api/model/minimum.py
--rw-r--r--   0        0        0     2889 2023-03-21 20:46:05.385217 albert_toolkit-0.1.0/src/albert/api/model/minimum.pyi
--rw-r--r--   0        0        0    10846 2023-03-14 15:56:43.824405 albert_toolkit-0.1.0/src/albert/api/model/model_patch.py
--rw-r--r--   0        0        0     9768 2023-03-14 15:56:43.824474 albert_toolkit-0.1.0/src/albert/api/model/model_patch.pyi
--rw-r--r--   0        0        0    36660 2023-03-14 15:56:43.824607 albert_toolkit-0.1.0/src/albert/api/model/model_prediction.py
--rw-r--r--   0        0        0    36408 2023-03-14 15:56:43.825032 albert_toolkit-0.1.0/src/albert/api/model/model_prediction.pyi
--rw-r--r--   0        0        0     6338 2023-03-14 15:56:43.824769 albert_toolkit-0.1.0/src/albert/api/model/model_predictions.py
--rw-r--r--   0        0        0     6338 2023-03-14 15:56:43.825289 albert_toolkit-0.1.0/src/albert/api/model/model_predictions.pyi
--rw-r--r--   0        0        0    31893 2023-03-14 15:56:43.825435 albert_toolkit-0.1.0/src/albert/api/model/model_predictions_values_only.py
--rw-r--r--   0        0        0    31641 2023-03-14 15:56:43.825147 albert_toolkit-0.1.0/src/albert/api/model/model_predictions_values_only.pyi
--rw-r--r--   0        0        0    27904 2023-03-14 15:56:43.825764 albert_toolkit-0.1.0/src/albert/api/model/new_model_version.py
--rw-r--r--   0        0        0    27525 2023-03-14 15:56:43.827113 albert_toolkit-0.1.0/src/albert/api/model/new_model_version.pyi
--rw-r--r--   0        0        0    27362 2023-03-14 15:56:43.827193 albert_toolkit-0.1.0/src/albert/api/model/output.py
--rw-r--r--   0        0        0    27253 2023-03-14 15:56:43.827274 albert_toolkit-0.1.0/src/albert/api/model/output.pyi
--rw-r--r--   0        0        0     7402 2023-03-14 15:56:43.827343 albert_toolkit-0.1.0/src/albert/api/model/parameter.py
--rw-r--r--   0        0        0     7214 2023-03-14 15:56:43.828315 albert_toolkit-0.1.0/src/albert/api/model/parameter.pyi
--rw-r--r--   0        0        0    13128 2023-03-14 15:56:43.828426 albert_toolkit-0.1.0/src/albert/api/model/partial_product_design.py
--rw-r--r--   0        0        0    13128 2023-03-14 15:56:43.828527 albert_toolkit-0.1.0/src/albert/api/model/partial_product_design.pyi
--rw-r--r--   0        0        0    19513 2023-03-14 15:56:43.835360 albert_toolkit-0.1.0/src/albert/api/model/partial_success.py
--rw-r--r--   0        0        0    19513 2023-03-14 15:56:43.836701 albert_toolkit-0.1.0/src/albert/api/model/partial_success.pyi
--rw-r--r--   0        0        0     8043 2023-03-14 15:56:43.836524 albert_toolkit-0.1.0/src/albert/api/model/partial_success1.py
--rw-r--r--   0        0        0     7858 2023-03-14 15:56:43.836770 albert_toolkit-0.1.0/src/albert/api/model/partial_success1.pyi
--rw-r--r--   0        0        0    40104 2023-03-14 15:56:43.836856 albert_toolkit-0.1.0/src/albert/api/model/partial_success_post.py
--rw-r--r--   0        0        0    40104 2023-03-14 15:56:43.855897 albert_toolkit-0.1.0/src/albert/api/model/partial_success_post.pyi
--rw-r--r--   0        0        0    11412 2023-03-14 15:56:43.855758 albert_toolkit-0.1.0/src/albert/api/model/patch.py
--rw-r--r--   0        0        0    10083 2023-03-14 15:56:43.856207 albert_toolkit-0.1.0/src/albert/api/model/patch.pyi
--rw-r--r--   0        0        0    10045 2023-03-14 15:56:43.856129 albert_toolkit-0.1.0/src/albert/api/model/patch1.py
--rw-r--r--   0        0        0     9399 2023-03-14 15:56:43.856027 albert_toolkit-0.1.0/src/albert/api/model/patch1.pyi
--rw-r--r--   0        0        0    13810 2023-03-14 15:56:43.856362 albert_toolkit-0.1.0/src/albert/api/model/patch_blk.py
--rw-r--r--   0        0        0    13144 2023-03-14 15:56:43.856299 albert_toolkit-0.1.0/src/albert/api/model/patch_blk.pyi
--rw-r--r--   0        0        0    13519 2023-03-21 20:46:05.385929 albert_toolkit-0.1.0/src/albert/api/model/patch_inventory.py
--rw-r--r--   0        0        0    11787 2023-03-21 20:46:05.385999 albert_toolkit-0.1.0/src/albert/api/model/patch_inventory.pyi
--rw-r--r--   0        0        0    17163 2023-03-14 15:56:43.865408 albert_toolkit-0.1.0/src/albert/api/model/patch_prediction.py
--rw-r--r--   0        0        0    16148 2023-03-14 15:56:43.865207 albert_toolkit-0.1.0/src/albert/api/model/patch_prediction.pyi
--rw-r--r--   0        0        0    18767 2023-03-14 15:56:43.866047 albert_toolkit-0.1.0/src/albert/api/model/patch_type.py
--rw-r--r--   0        0        0    17847 2023-03-14 15:56:43.867398 albert_toolkit-0.1.0/src/albert/api/model/patch_type.pyi
--rw-r--r--   0        0        0     3430 2023-03-14 15:56:43.866818 albert_toolkit-0.1.0/src/albert/api/model/patch_types.py
--rw-r--r--   0        0        0     3430 2023-03-14 15:56:43.868535 albert_toolkit-0.1.0/src/albert/api/model/patch_types.pyi
--rw-r--r--   0        0        0     4668 2023-03-14 15:56:43.869076 albert_toolkit-0.1.0/src/albert/api/model/pd_row.py
--rw-r--r--   0        0        0     4431 2023-03-14 15:56:43.868613 albert_toolkit-0.1.0/src/albert/api/model/pd_row.pyi
--rw-r--r--   0        0        0     4435 2023-03-14 15:56:43.868957 albert_toolkit-0.1.0/src/albert/api/model/pd_rows.py
--rw-r--r--   0        0        0     4435 2023-03-14 15:56:43.868793 albert_toolkit-0.1.0/src/albert/api/model/pd_rows.pyi
--rw-r--r--   0        0        0     9133 2023-03-14 15:56:43.869009 albert_toolkit-0.1.0/src/albert/api/model/post_partial_success.py
--rw-r--r--   0        0        0     8944 2023-03-14 15:56:43.868721 albert_toolkit-0.1.0/src/albert/api/model/post_partial_success.pyi
--rw-r--r--   0        0        0     1385 2023-03-14 15:56:43.869130 albert_toolkit-0.1.0/src/albert/api/model/post_pd_rows.py
--rw-r--r--   0        0        0     1340 2023-03-14 15:56:43.868876 albert_toolkit-0.1.0/src/albert/api/model/post_pd_rows.pyi
--rw-r--r--   0        0        0     5787 2023-03-14 15:56:43.869212 albert_toolkit-0.1.0/src/albert/api/model/post_prediction_partial_success.py
--rw-r--r--   0        0        0     5787 2023-03-14 15:56:43.871824 albert_toolkit-0.1.0/src/albert/api/model/post_prediction_partial_success.pyi
--rw-r--r--   0        0        0     2921 2023-03-14 15:56:43.870258 albert_toolkit-0.1.0/src/albert/api/model/post_to_scheduler_success.py
--rw-r--r--   0        0        0     2921 2023-03-14 15:56:43.872301 albert_toolkit-0.1.0/src/albert/api/model/post_to_scheduler_success.pyi
--rw-r--r--   0        0        0    14562 2023-03-14 15:56:43.871633 albert_toolkit-0.1.0/src/albert/api/model/prediction_data_model.py
--rw-r--r--   0        0        0    13330 2023-03-14 15:56:43.870541 albert_toolkit-0.1.0/src/albert/api/model/prediction_data_model.pyi
--rw-r--r--   0        0        0    11219 2023-03-14 15:56:43.870632 albert_toolkit-0.1.0/src/albert/api/model/prediction_data_model_success.py
--rw-r--r--   0        0        0    10507 2023-03-14 15:56:43.871923 albert_toolkit-0.1.0/src/albert/api/model/prediction_data_model_success.pyi
--rw-r--r--   0        0        0    34269 2023-03-14 15:56:43.870373 albert_toolkit-0.1.0/src/albert/api/model/prediction_model.py
--rw-r--r--   0        0        0    33466 2023-03-14 15:56:43.870469 albert_toolkit-0.1.0/src/albert/api/model/prediction_model.pyi
--rw-r--r--   0        0        0     4041 2023-03-14 15:56:43.871706 albert_toolkit-0.1.0/src/albert/api/model/prediction_model_versions.py
--rw-r--r--   0        0        0     4007 2023-03-14 15:56:43.872214 albert_toolkit-0.1.0/src/albert/api/model/prediction_model_versions.pyi
--rw-r--r--   0        0        0     3923 2023-03-14 15:56:43.872384 albert_toolkit-0.1.0/src/albert/api/model/prediction_models.py
--rw-r--r--   0        0        0     3889 2023-03-14 15:56:43.872582 albert_toolkit-0.1.0/src/albert/api/model/prediction_models.pyi
--rw-r--r--   0        0        0    23689 2023-03-14 15:56:43.872130 albert_toolkit-0.1.0/src/albert/api/model/product_design.py
--rw-r--r--   0        0        0    22680 2023-03-14 15:56:43.872021 albert_toolkit-0.1.0/src/albert/api/model/product_design.pyi
--rw-r--r--   0        0        0     6925 2023-03-14 15:56:43.872748 albert_toolkit-0.1.0/src/albert/api/model/product_design_search_result.py
--rw-r--r--   0        0        0     6925 2023-03-14 15:56:43.873647 albert_toolkit-0.1.0/src/albert/api/model/product_design_search_result.pyi
--rw-r--r--   0        0        0     3355 2023-03-14 15:56:43.873782 albert_toolkit-0.1.0/src/albert/api/model/product_design_suggest_result.py
--rw-r--r--   0        0        0     3321 2023-03-14 15:56:43.874007 albert_toolkit-0.1.0/src/albert/api/model/product_design_suggest_result.pyi
--rw-r--r--   0        0        0     4061 2023-03-14 15:56:43.874062 albert_toolkit-0.1.0/src/albert/api/model/product_designs.py
--rw-r--r--   0        0        0     4061 2023-03-14 15:56:43.874191 albert_toolkit-0.1.0/src/albert/api/model/product_designs.pyi
--rw-r--r--   0        0        0    20064 2023-03-14 15:56:43.889603 albert_toolkit-0.1.0/src/albert/api/model/property_task_data_model.py
--rw-r--r--   0        0        0    19674 2023-03-14 15:56:43.874256 albert_toolkit-0.1.0/src/albert/api/model/property_task_data_model.pyi
--rw-r--r--   0        0        0     3969 2023-03-14 15:56:43.873944 albert_toolkit-0.1.0/src/albert/api/model/put_back_update_companies.py
--rw-r--r--   0        0        0     3969 2023-03-14 15:56:43.873870 albert_toolkit-0.1.0/src/albert/api/model/put_back_update_companies.pyi
--rw-r--r--   0        0        0     6968 2023-03-21 20:46:05.390703 albert_toolkit-0.1.0/src/albert/api/model/put_report.py
--rw-r--r--   0        0        0     6968 2023-03-21 20:46:05.390801 albert_toolkit-0.1.0/src/albert/api/model/put_report.pyi
--rw-r--r--   0        0        0    12229 2023-03-21 20:46:05.391600 albert_toolkit-0.1.0/src/albert/api/model/report.py
--rw-r--r--   0        0        0    12045 2023-03-21 20:46:05.392646 albert_toolkit-0.1.0/src/albert/api/model/report.pyi
--rw-r--r--   0        0        0     3931 2023-03-14 15:56:43.921553 albert_toolkit-0.1.0/src/albert/api/model/report_list.py
--rw-r--r--   0        0        0     3931 2023-03-14 15:56:43.922029 albert_toolkit-0.1.0/src/albert/api/model/report_list.pyi
--rw-r--r--   0        0        0     6303 2023-03-14 15:56:43.922919 albert_toolkit-0.1.0/src/albert/api/model/report_search_result.py
--rw-r--r--   0        0        0     6303 2023-03-14 15:56:43.924235 albert_toolkit-0.1.0/src/albert/api/model/report_search_result.pyi
--rw-r--r--   0        0        0     3341 2023-03-14 15:56:43.925781 albert_toolkit-0.1.0/src/albert/api/model/report_suggest_result.py
--rw-r--r--   0        0        0     3307 2023-03-14 15:56:43.924984 albert_toolkit-0.1.0/src/albert/api/model/report_suggest_result.pyi
--rw-r--r--   0        0        0     8527 2023-03-14 15:56:43.926506 albert_toolkit-0.1.0/src/albert/api/model/report_type.py
--rw-r--r--   0        0        0     8254 2023-03-14 15:56:43.926779 albert_toolkit-0.1.0/src/albert/api/model/report_type.pyi
--rw-r--r--   0        0        0     3968 2023-03-14 15:56:43.927655 albert_toolkit-0.1.0/src/albert/api/model/report_type_list.py
--rw-r--r--   0        0        0     3968 2023-03-14 15:56:43.928431 albert_toolkit-0.1.0/src/albert/api/model/report_type_list.pyi
--rw-r--r--   0        0        0     3360 2023-03-14 15:56:43.928527 albert_toolkit-0.1.0/src/albert/api/model/task_workflow.py
--rw-r--r--   0        0        0     3338 2023-03-14 15:56:43.928186 albert_toolkit-0.1.0/src/albert/api/model/task_workflow.pyi
--rw-r--r--   0        0        0    58448 2023-03-14 15:56:43.928301 albert_toolkit-0.1.0/src/albert/api/model/unpack.py
--rw-r--r--   0        0        0    58448 2023-03-14 15:56:43.928367 albert_toolkit-0.1.0/src/albert/api/model/unpack.pyi
--rw-r--r--   0        0        0     7179 2023-03-14 15:56:43.928604 albert_toolkit-0.1.0/src/albert/api/model/update.py
--rw-r--r--   0        0        0     6703 2023-03-14 15:56:43.928676 albert_toolkit-0.1.0/src/albert/api/model/update.pyi
--rw-r--r--   0        0        0    12003 2023-03-14 15:56:43.928794 albert_toolkit-0.1.0/src/albert/api/model/values.py
--rw-r--r--   0        0        0    11873 2023-03-14 15:56:43.974127 albert_toolkit-0.1.0/src/albert/api/model/values.pyi
--rw-r--r--   0        0        0     2475 2023-03-14 15:56:43.929067 albert_toolkit-0.1.0/src/albert/api/model/wf_all_accepted.py
--rw-r--r--   0        0        0     2475 2023-03-14 15:56:43.993973 albert_toolkit-0.1.0/src/albert/api/model/wf_all_accepted.pyi
--rw-r--r--   0        0        0    10222 2023-03-14 15:56:43.993892 albert_toolkit-0.1.0/src/albert/api/model/wf_partial_success.py
--rw-r--r--   0        0        0    10222 2023-03-14 15:56:43.993791 albert_toolkit-0.1.0/src/albert/api/model/wf_partial_success.pyi
--rw-r--r--   0        0        0     4905 2023-03-21 20:46:05.392774 albert_toolkit-0.1.0/src/albert/api/models/__init__.py
--rw-r--r--   0        0        0     2907 2023-03-21 20:46:05.394672 albert_toolkit-0.1.0/src/albert/api/paths/__init__.py
--rw-r--r--   0        0        0      315 2023-03-21 20:46:05.394986 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories/__init__.py
--rw-r--r--   0        0        0    16564 2023-03-21 20:46:05.394771 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories/get.py
--rw-r--r--   0        0        0    15744 2023-03-21 20:46:05.394876 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories/get.pyi
--rw-r--r--   0        0        0    15750 2023-03-21 20:46:05.395082 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories/post.py
--rw-r--r--   0        0        0    15496 2023-03-21 20:46:05.395171 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories/post.pyi
--rw-r--r--   0        0        0      329 2023-03-21 20:46:05.395276 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories_health/__init__.py
--rw-r--r--   0        0        0     7585 2023-03-21 20:46:05.395362 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories_health/get.py
--rw-r--r--   0        0        0     7504 2023-03-21 20:46:05.395491 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories_health/get.pyi
--rw-r--r--   0        0        0      321 2023-03-21 20:46:05.400709 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories_id/__init__.py
--rw-r--r--   0        0        0    12176 2023-03-21 20:46:05.400776 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories_id/delete.py
--rw-r--r--   0        0        0    11922 2023-03-21 20:46:05.401496 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories_id/delete.pyi
--rw-r--r--   0        0        0    12316 2023-03-21 20:46:05.401136 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories_id/get.py
--rw-r--r--   0        0        0    12062 2023-03-21 20:46:05.401250 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories_id/get.pyi
--rw-r--r--   0        0        0    16515 2023-03-21 20:46:05.401345 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories_id/patch.py
--rw-r--r--   0        0        0    16261 2023-03-21 20:46:05.401413 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories_id/patch.pyi
--rw-r--r--   0        0        0      311 2023-03-13 19:46:24.000000 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations/__init__.py
--rw-r--r--   0        0        0    15401 2023-03-14 15:56:44.155226 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations/get.py
--rw-r--r--   0        0        0    14858 2023-03-14 15:56:44.155376 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations/get.pyi
--rw-r--r--   0        0        0    13826 2023-03-14 15:56:44.156342 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations/post.py
--rw-r--r--   0        0        0    13602 2023-03-14 15:56:44.156500 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations/post.pyi
--rw-r--r--   0        0        0      329 2023-03-14 15:56:44.156581 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_async_id/__init__.py
--rw-r--r--   0        0        0    15519 2023-03-14 15:56:44.156746 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_async_id/get.py
--rw-r--r--   0        0        0    15087 2023-03-14 15:56:44.156928 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_async_id/get.pyi
--rw-r--r--   0        0        0    16416 2023-03-14 15:56:44.156674 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_async_id/put.py
--rw-r--r--   0        0        0    16162 2023-03-14 15:56:44.156999 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_async_id/put.pyi
--rw-r--r--   0        0        0      325 2023-03-13 19:46:20.000000 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_health/__init__.py
--rw-r--r--   0        0        0     7585 2023-03-14 15:56:44.158928 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_health/get.py
--rw-r--r--   0        0        0     7504 2023-03-14 15:56:44.159721 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_health/get.pyi
--rw-r--r--   0        0        0      317 2023-03-13 19:46:24.000000 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_id/__init__.py
--rw-r--r--   0        0        0    12068 2023-03-14 15:56:44.160454 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_id/delete.py
--rw-r--r--   0        0        0    11814 2023-03-14 15:56:44.161436 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_id/delete.pyi
--rw-r--r--   0        0        0    12301 2023-03-14 15:56:44.161930 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_id/get.py
--rw-r--r--   0        0        0    12047 2023-03-14 15:56:44.162643 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_id/get.pyi
--rw-r--r--   0        0        0    16356 2023-03-14 15:56:44.167103 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_id/patch.py
--rw-r--r--   0        0        0    16102 2023-03-14 15:56:44.167820 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_id/patch.pyi
--rw-r--r--   0        0        0      315 2023-03-14 15:56:44.167246 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions/__init__.py
--rw-r--r--   0        0        0    16527 2023-03-14 15:56:44.167656 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions/get.py
--rw-r--r--   0        0        0    15923 2023-03-14 15:56:44.167389 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions/get.pyi
--rw-r--r--   0        0        0    16821 2023-03-14 15:56:44.167518 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions/post.py
--rw-r--r--   0        0        0    16567 2023-03-14 15:56:44.167742 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions/post.pyi
--rw-r--r--   0        0        0      329 2023-03-14 15:56:44.167947 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_health/__init__.py
--rw-r--r--   0        0        0     7637 2023-03-14 15:56:44.168604 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_health/get.py
--rw-r--r--   0        0        0     7556 2023-03-14 15:56:44.169911 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_health/get.pyi
--rw-r--r--   0        0        0      333 2023-03-14 15:56:44.169497 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_mergedac/__init__.py
--rw-r--r--   0        0        0    15148 2023-03-14 15:56:44.169816 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_mergedac/post.py
--rw-r--r--   0        0        0    14894 2023-03-14 15:56:44.171901 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_mergedac/post.pyi
--rw-r--r--   0        0        0      333 2023-03-14 15:56:44.171192 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_mergedat/__init__.py
--rw-r--r--   0        0        0    15148 2023-03-14 15:56:44.170833 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_mergedat/post.py
--rw-r--r--   0        0        0    14894 2023-03-14 15:56:44.171023 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_mergedat/post.pyi
--rw-r--r--   0        0        0      329 2023-03-14 15:56:44.170671 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models/__init__.py
--rw-r--r--   0        0        0    13762 2023-03-14 15:56:44.170507 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models/get.py
--rw-r--r--   0        0        0    13313 2023-03-14 15:56:44.171427 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models/get.pyi
--rw-r--r--   0        0        0    14980 2023-03-14 15:56:44.171329 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models/post.py
--rw-r--r--   0        0        0    14726 2023-03-14 15:56:44.171693 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models/post.pyi
--rw-r--r--   0        0        0      335 2023-03-14 15:56:44.172067 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_id/__init__.py
--rw-r--r--   0        0        0    16701 2023-03-14 15:56:44.172958 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_id/get.py
--rw-r--r--   0        0        0    16217 2023-03-14 15:56:44.172849 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_id/get.pyi
--rw-r--r--   0        0        0      365 2023-03-14 15:56:44.172578 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_parent_id_version/__init__.py
--rw-r--r--   0        0        0    14450 2023-03-14 15:56:44.172729 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_parent_id_version/delete.py
--rw-r--r--   0        0        0    14196 2023-03-14 15:56:44.173855 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_parent_id_version/delete.pyi
--rw-r--r--   0        0        0    15059 2023-03-14 15:56:44.174601 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_parent_id_version/get.py
--rw-r--r--   0        0        0    14683 2023-03-14 15:56:44.174466 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_parent_id_version/get.pyi
--rw-r--r--   0        0        0    19259 2023-03-14 15:56:44.174139 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_parent_id_version/patch.py
--rw-r--r--   0        0        0    19005 2023-03-14 15:56:44.174337 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_parent_id_version/patch.pyi
--rw-r--r--   0        0        0      371 2023-03-14 15:56:44.174050 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_parent_id_version_id/__init__.py
--rw-r--r--   0        0        0    13151 2023-03-14 15:56:44.174704 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_parent_id_version_id/get.py
--rw-r--r--   0        0        0    12775 2023-03-14 15:56:44.175125 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_parent_id_version_id/get.pyi
--rw-r--r--   0        0        0      335 2023-03-14 15:56:44.175027 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_parent_id/__init__.py
--rw-r--r--   0        0        0    16477 2023-03-14 15:56:44.175194 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_parent_id/patch.py
--rw-r--r--   0        0        0    16192 2023-03-14 15:56:44.176472 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_parent_id/patch.pyi
--rw-r--r--   0        0        0      327 2023-03-14 15:56:44.176575 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_tasks/__init__.py
--rw-r--r--   0        0        0    16206 2023-03-14 15:56:44.177574 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_tasks/post.py
--rw-r--r--   0        0        0    15922 2023-03-14 15:56:44.177288 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_tasks/post.pyi
--rw-r--r--   0        0        0      319 2023-03-14 15:56:44.177145 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign/__init__.py
--rw-r--r--   0        0        0    14687 2023-03-14 15:56:44.178509 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign/get.py
--rw-r--r--   0        0        0    14083 2023-03-14 15:56:44.177427 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign/get.pyi
--rw-r--r--   0        0        0    15051 2023-03-14 15:56:44.177632 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign/post.py
--rw-r--r--   0        0        0    14797 2023-03-14 15:56:44.178279 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign/post.pyi
--rw-r--r--   0        0        0      333 2023-03-14 15:56:44.177838 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_health/__init__.py
--rw-r--r--   0        0        0     7648 2023-03-14 15:56:44.178145 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_health/get.py
--rw-r--r--   0        0        0     7567 2023-03-14 15:56:44.178005 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_health/get.pyi
--rw-r--r--   0        0        0      325 2023-03-14 15:56:44.178691 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id/__init__.py
--rw-r--r--   0        0        0    12691 2023-03-14 15:56:44.178879 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id/get.py
--rw-r--r--   0        0        0    12437 2023-03-14 15:56:44.179044 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id/get.pyi
--rw-r--r--   0        0        0      341 2023-03-14 15:56:44.180454 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_designs/__init__.py
--rw-r--r--   0        0        0    30588 2023-03-14 15:56:44.179372 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_designs/delete.py
--rw-r--r--   0        0        0    30184 2023-03-14 15:56:44.179183 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_designs/delete.pyi
--rw-r--r--   0        0        0    15587 2023-03-14 15:56:44.179270 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_designs/get.py
--rw-r--r--   0        0        0    15197 2023-03-14 15:56:44.180053 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_designs/get.pyi
--rw-r--r--   0        0        0    20625 2023-03-14 15:56:44.179638 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_designs/patch.py
--rw-r--r--   0        0        0    20371 2023-03-14 15:56:44.179458 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_designs/patch.pyi
--rw-r--r--   0        0        0    22220 2023-03-14 15:56:44.180353 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_designs/post.py
--rw-r--r--   0        0        0    21966 2023-03-14 15:56:44.180259 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_designs/post.pyi
--rw-r--r--   0        0        0      335 2023-03-14 15:56:44.180692 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_grid/__init__.py
--rw-r--r--   0        0        0    17566 2023-03-14 15:56:44.180905 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_grid/get.py
--rw-r--r--   0        0        0    17027 2023-03-14 15:56:44.181834 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_grid/get.pyi
--rw-r--r--   0        0        0      343 2023-03-14 15:56:44.181572 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_products/__init__.py
--rw-r--r--   0        0        0    17234 2023-03-14 15:56:44.181676 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_products/post.py
--rw-r--r--   0        0        0    16980 2023-03-14 15:56:44.181988 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_products/post.pyi
--rw-r--r--   0        0        0      339 2023-03-14 15:56:44.182950 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_unpack/__init__.py
--rw-r--r--   0        0        0    15329 2023-03-14 15:56:44.183150 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_unpack/get.py
--rw-r--r--   0        0        0    15052 2023-03-14 15:56:44.183025 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_unpack/get.pyi
--rw-r--r--   0        0        0      339 2023-03-14 15:56:44.183658 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_values/__init__.py
--rw-r--r--   0        0        0    17790 2023-03-14 15:56:44.183903 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_values/patch.py
--rw-r--r--   0        0        0    17506 2023-03-14 15:56:44.184023 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_values/patch.pyi
--rw-r--r--   0        0        0      349 2023-03-14 15:56:44.184881 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_inventories_id/__init__.py
--rw-r--r--   0        0        0    15886 2023-03-14 15:56:44.185162 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_inventories_id/get.py
--rw-r--r--   0        0        0    15454 2023-03-14 15:56:44.185034 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_inventories_id/get.pyi
--rw-r--r--   0        0        0    17918 2023-03-14 15:56:44.184942 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_inventories_id/put.py
--rw-r--r--   0        0        0    17664 2023-03-14 15:56:44.185465 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_inventories_id/put.pyi
--rw-r--r--   0        0        0      349 2023-03-14 15:56:44.185349 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_mergeinventory/__init__.py
--rw-r--r--   0        0        0    15297 2023-03-14 15:56:44.185815 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_mergeinventory/post.py
--rw-r--r--   0        0        0    15043 2023-03-14 15:56:44.185719 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_mergeinventory/post.pyi
--rw-r--r--   0        0        0      333 2023-03-14 15:56:44.186066 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_search/__init__.py
--rw-r--r--   0        0        0    23706 2023-03-14 15:56:44.185963 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_search/get.py
--rw-r--r--   0        0        0    22381 2023-03-14 15:56:44.194482 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_search/get.pyi
--rw-r--r--   0        0        0      335 2023-03-14 15:56:44.194614 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_suggest/__init__.py
--rw-r--r--   0        0        0    13256 2023-03-14 15:56:44.194276 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_suggest/get.py
--rw-r--r--   0        0        0    13002 2023-03-14 15:56:44.194403 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_suggest/get.pyi
--rw-r--r--   0        0        0      307 2023-03-13 19:46:31.000000 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports/__init__.py
--rw-r--r--   0        0        0    14402 2023-03-13 20:14:13.921607 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports/get.py
--rw-r--r--   0        0        0    14073 2023-03-13 20:14:13.922779 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports/get.pyi
--rw-r--r--   0        0        0    14898 2023-03-13 20:14:13.922868 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports/post.py
--rw-r--r--   0        0        0    14644 2023-03-13 20:14:13.925464 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports/post.pyi
--rw-r--r--   0        0        0      333 2023-03-13 19:46:19.000000 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_analytics_id/__init__.py
--rw-r--r--   0        0        0    14926 2023-03-21 16:07:55.093588 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_analytics_id/get.py
--rw-r--r--   0        0        0    14672 2023-03-14 15:56:44.194865 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_analytics_id/get.pyi
--rw-r--r--   0        0        0      317 2023-03-13 19:46:31.000000 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_copy/__init__.py
--rw-r--r--   0        0        0    14964 2023-03-13 20:14:13.925788 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_copy/post.py
--rw-r--r--   0        0        0    14710 2023-03-13 20:14:13.925875 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_copy/post.pyi
--rw-r--r--   0        0        0      337 2023-03-13 19:46:19.000000 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_datascience_id/__init__.py
--rw-r--r--   0        0        0    14951 2023-03-25 21:10:11.094939 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_datascience_id/get.py
--rw-r--r--   0        0        0    14697 2023-03-14 15:56:44.195088 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_datascience_id/get.pyi
--rw-r--r--   0        0        0      321 2023-03-13 19:46:20.000000 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_health/__init__.py
--rw-r--r--   0        0        0     7648 2023-03-21 20:46:05.401611 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_health/get.py
--rw-r--r--   0        0        0     7567 2023-03-21 20:46:05.408631 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_health/get.pyi
--rw-r--r--   0        0        0      313 2023-03-13 19:46:31.000000 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_id/__init__.py
--rw-r--r--   0        0        0    12309 2023-03-13 20:14:13.930104 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_id/delete.py
--rw-r--r--   0        0        0    12055 2023-03-13 20:14:13.930210 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_id/delete.pyi
--rw-r--r--   0        0        0    14786 2023-03-13 20:14:13.930371 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_id/get.py
--rw-r--r--   0        0        0    14532 2023-03-13 20:14:13.930461 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_id/get.pyi
--rw-r--r--   0        0        0    16852 2023-03-13 20:14:13.934345 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_id/put.py
--rw-r--r--   0        0        0    16598 2023-03-13 20:14:13.937587 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_id/put.pyi
--rw-r--r--   0        0        0      359 2023-03-13 19:46:28.000000 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_inventory_equipment_usage/__init__.py
--rw-r--r--   0        0        0    10820 2023-03-13 20:14:13.937676 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_inventory_equipment_usage/get.py
--rw-r--r--   0        0        0    10566 2023-03-13 20:14:13.937826 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_inventory_equipment_usage/get.pyi
--rw-r--r--   0        0        0      347 2023-03-13 19:46:28.000000 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_inventory_movements/__init__.py
--rw-r--r--   0        0        0    12924 2023-03-13 20:14:13.938652 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_inventory_movements/get.py
--rw-r--r--   0        0        0    12670 2023-03-13 20:14:13.938754 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_inventory_movements/get.pyi
--rw-r--r--   0        0        0      321 2023-03-13 19:46:32.000000 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_search/__init__.py
--rw-r--r--   0        0        0    14805 2023-03-13 20:14:13.938886 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_search/get.py
--rw-r--r--   0        0        0    14434 2023-03-13 20:14:13.938979 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_search/get.pyi
--rw-r--r--   0        0        0      323 2023-03-13 19:46:30.000000 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_suggest/__init__.py
--rw-r--r--   0        0        0    13168 2023-03-13 20:14:13.945743 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_suggest/get.py
--rw-r--r--   0        0        0    12914 2023-03-13 20:14:13.951244 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_suggest/get.pyi
--rw-r--r--   0        0        0      317 2023-03-13 19:46:28.000000 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_type/__init__.py
--rw-r--r--   0        0        0    13989 2023-03-13 20:14:13.948583 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_type/get.py
--rw-r--r--   0        0        0    13483 2023-03-13 20:14:13.949679 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_type/get.pyi
--rw-r--r--   0        0        0    15623 2023-03-14 15:56:44.208509 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_type/patch.py
--rw-r--r--   0        0        0    15339 2023-03-14 15:56:44.208618 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_type/patch.pyi
--rw-r--r--   0        0        0    15072 2023-03-13 20:14:13.948029 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_type/post.py
--rw-r--r--   0        0        0    14818 2023-03-13 20:14:13.956046 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_type/post.pyi
--rw-r--r--   0        0        0      323 2023-03-13 19:46:28.000000 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_type_id/__init__.py
--rw-r--r--   0        0        0    12655 2023-03-13 20:14:13.956883 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_type_id/get.py
--rw-r--r--   0        0        0    12401 2023-03-13 20:14:13.957557 albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_type_id/get.pyi
--rw-r--r--   0        0        0    10554 2023-03-14 15:56:44.208723 albert_toolkit-0.1.0/src/albert/api/rest.py
--rw-r--r--   0        0        0    97658 2023-03-14 15:56:44.208827 albert_toolkit-0.1.0/src/albert/api/schemas.py
--rw-r--r--   0        0        0       24 2023-03-21 21:10:12.016256 albert_toolkit-0.1.0/src/albert/binassign/__init__.py
--rw-r--r--   0        0        0     6864 2023-04-07 17:39:15.280277 albert_toolkit-0.1.0/src/albert/binassign/binassign.py
--rw-r--r--   0        0        0    23696 2023-04-07 17:39:15.290368 albert_toolkit-0.1.0/src/albert/binassign/tests/test_binassign.py
--rw-r--r--   0        0        0       24 2023-03-21 21:10:12.017181 albert_toolkit-0.1.0/src/albert/bincreate/__init__.py
--rw-r--r--   0        0        0     9335 2023-04-07 17:39:15.286804 albert_toolkit-0.1.0/src/albert/bincreate/bincreate.py
--rw-r--r--   0        0        0    14049 2023-04-07 17:39:15.286958 albert_toolkit-0.1.0/src/albert/bincreate/tests/test_bincreate.py
--rw-r--r--   0        0        0        0 2023-03-21 20:52:07.490083 albert_toolkit-0.1.0/src/albert/chem/__init__.py
--rw-r--r--   0        0        0     2273 2023-03-25 22:48:15.154593 albert_toolkit-0.1.0/src/albert/chem/descriptors.py
--rw-r--r--   0        0        0     3505 2023-03-21 20:52:07.492466 albert_toolkit-0.1.0/src/albert/chem/structure.py
--rw-r--r--   0        0        0       48 2023-03-13 22:23:01.571954 albert_toolkit-0.1.0/src/albert/data/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 15:43:53.298477 albert_toolkit-0.1.0/src/albert/data/datasets/__init__.py
--rw-r--r--   0        0        0      101 2023-04-10 15:43:53.299300 albert_toolkit-0.1.0/src/albert/data/datasets/molecular/__init__.py
--rw-r--r--   0        0        0     4261 2023-04-10 15:43:53.299798 albert_toolkit-0.1.0/src/albert/data/datasets/molecular/atom.py
--rw-r--r--   0        0        0     1566 2023-04-10 15:43:53.299872 albert_toolkit-0.1.0/src/albert/data/datasets/molecular/bond.py
--rw-r--r--   0        0        0    17402 2023-04-10 15:43:53.300034 albert_toolkit-0.1.0/src/albert/data/datasets/molecular/graph.py
--rw-r--r--   0        0        0     4773 2023-04-10 15:43:53.300168 albert_toolkit-0.1.0/src/albert/data/datasets/molecular/tests/test_atomic_attributes.py
--rw-r--r--   0        0        0      197 2023-04-10 15:43:53.300297 albert_toolkit-0.1.0/src/albert/data/datasets/molecular/utils.py
--rw-r--r--   0        0        0       29 2023-03-21 20:46:05.409720 albert_toolkit-0.1.0/src/albert/data/pipelines/__init__.py
--rw-r--r--   0        0        0     7123 2023-03-21 20:46:05.408976 albert_toolkit-0.1.0/src/albert/data/pipelines/property_data.py
--rw-r--r--   0        0        0       23 2023-03-13 22:15:40.430303 albert_toolkit-0.1.0/src/albert/data/reports/__init__.py
--rw-r--r--   0        0        0     6760 2023-03-21 20:46:05.409093 albert_toolkit-0.1.0/src/albert/data/reports/reports.py
--rw-r--r--   0        0        0     1319 2023-03-21 20:46:05.410994 albert_toolkit-0.1.0/src/albert/data/reports/tests/test_reports.py
--rw-r--r--   0        0        0        0 2023-02-24 19:24:57.946228 albert_toolkit-0.1.0/src/albert/data/warehouse/__init__.py
--rw-r--r--   0        0        0     3099 2023-04-10 15:43:53.301454 albert_toolkit-0.1.0/src/albert/data/warehouse/dbsession.py
--rw-r--r--   0        0        0    57407 2023-03-21 20:52:07.492563 albert_toolkit-0.1.0/src/albert/data/warehouse/dbwarehouse_schema.py
--rw-r--r--   0        0        0    10197 2023-04-10 15:44:55.181618 albert_toolkit-0.1.0/src/albert/data/warehouse/queries.py
--rw-r--r--   0        0        0       29 2023-03-21 21:10:12.016726 albert_toolkit-0.1.0/src/albert/data_cleaning/__init__.py
--rw-r--r--   0        0        0    17510 2023-04-07 17:39:15.287031 albert_toolkit-0.1.0/src/albert/data_cleaning/data_cleaning.py
--rw-r--r--   0        0        0    10268 2023-03-27 15:12:52.337618 albert_toolkit-0.1.0/src/albert/data_cleaning/tests/test_data_cleaning.py
--rw-r--r--   0        0        0       88 2023-03-14 15:56:44.215223 albert_toolkit-0.1.0/src/albert/filters/__init__.py
--rw-r--r--   0        0        0     2039 2023-03-14 15:56:44.215435 albert_toolkit-0.1.0/src/albert/filters/base.py
--rw-r--r--   0        0        0     1395 2023-03-14 15:56:44.216000 albert_toolkit-0.1.0/src/albert/filters/prediction_filters.py
--rw-r--r--   0        0        0     2816 2023-03-14 15:56:44.215546 albert_toolkit-0.1.0/src/albert/filters/report_filters.py
--rw-r--r--   0        0        0     1100 2023-03-14 15:56:44.215641 albert_toolkit-0.1.0/src/albert/filters/tests/test_prediction_filter.py
--rw-r--r--   0        0        0     2731 2023-03-13 20:14:31.499968 albert_toolkit-0.1.0/src/albert/filters/tests/test_report_filter.py
--rw-r--r--   0        0        0       21 2023-03-21 21:10:12.018359 albert_toolkit-0.1.0/src/albert/internal/__init__.py
--rw-r--r--   0        0        0     1678 2023-03-14 15:56:44.215796 albert_toolkit-0.1.0/src/albert/internal/dynamo.py
--rw-r--r--   0        0        0       21 2023-03-14 15:56:44.218878 albert_toolkit-0.1.0/src/albert/internal/utils/__init__.py
--rw-r--r--   0        0        0     3370 2023-03-27 15:12:52.338256 albert_toolkit-0.1.0/src/albert/internal/utils/utils.py
--rw-r--r--   0        0        0       33 2023-04-10 15:43:53.301760 albert_toolkit-0.1.0/src/albert/losses/__init__.py
--rw-r--r--   0        0        0       43 2023-04-10 15:43:53.301282 albert_toolkit-0.1.0/src/albert/losses/molecular/__init__.py
--rw-r--r--   0        0        0     2544 2023-04-10 15:43:53.301655 albert_toolkit-0.1.0/src/albert/losses/molecular/ntxentloss.py
--rw-r--r--   0        0        0        0 2023-03-21 20:52:07.498571 albert_toolkit-0.1.0/src/albert/metrics/__init__.py
--rw-r--r--   0        0        0        0 2023-03-21 21:10:12.018412 albert_toolkit-0.1.0/src/albert/mlops/__init__.py
--rw-r--r--   0        0        0     2066 2023-03-21 21:10:12.018571 albert_toolkit-0.1.0/src/albert/mlops/clearml.py
--rw-r--r--   0        0        0        0 2023-01-24 13:57:52.836583 albert_toolkit-0.1.0/src/albert/models/__init__.py
--rw-r--r--   0        0        0       43 2023-03-13 20:14:44.533959 albert_toolkit-0.1.0/src/albert/models/gp/__init__.py
--rw-r--r--   0        0        0     1671 2023-03-13 20:14:44.538923 albert_toolkit-0.1.0/src/albert/models/gp/exact_gps.py
--rw-r--r--   0        0        0     2953 2023-03-13 20:14:44.543696 albert_toolkit-0.1.0/src/albert/models/gp/tests/test_exact_gps.py
--rw-r--r--   0        0        0        0 2023-01-24 13:57:52.837205 albert_toolkit-0.1.0/src/albert/models/nn/__init__.py
--rw-r--r--   0        0        0       46 2023-04-03 18:50:19.466835 albert_toolkit-0.1.0/src/albert/models/nn/embedding/__init__.py
--rw-r--r--   0        0        0     6230 2023-04-10 15:43:53.302625 albert_toolkit-0.1.0/src/albert/models/nn/embedding/gin.py
--rw-r--r--   0        0        0     2918 2023-01-24 13:57:52.837855 albert_toolkit-0.1.0/src/albert/models/nn/embedding/mlp.py
--rw-r--r--   0        0        0     3557 2023-01-24 13:57:52.838210 albert_toolkit-0.1.0/src/albert/models/nn/embedding/tests/test_mlp.py
--rw-r--r--   0        0        0        0 2023-01-24 13:57:52.838264 albert_toolkit-0.1.0/src/albert/nlp/__init__.py
--rw-r--r--   0        0        0       55 2023-01-24 13:57:52.838484 albert_toolkit-0.1.0/src/albert/nlp/utils/__init__.py
--rw-r--r--   0        0        0      484 2023-03-13 20:14:47.619604 albert_toolkit-0.1.0/src/albert/nlp/utils/edit.py
--rw-r--r--   0        0        0      493 2023-03-13 20:14:47.621546 albert_toolkit-0.1.0/src/albert/nlp/utils/tests/test_ldistance.py
--rw-r--r--   0        0        0       31 2023-02-24 19:24:57.947919 albert_toolkit-0.1.0/src/albert/pipeline/__init__.py
--rw-r--r--   0        0        0     2050 2023-03-14 15:56:44.227623 albert_toolkit-0.1.0/src/albert/pipeline/albert_pipeline.py
--rw-r--r--   0        0        0     6334 2023-03-21 20:46:05.413649 albert_toolkit-0.1.0/src/albert/pipeline/tests/test_pipeline.py
--rw-r--r--   0        0        0        0 2023-01-24 13:57:52.839109 albert_toolkit-0.1.0/src/albert/predictors/__init__.py
--rw-r--r--   0        0        0        0 2023-03-21 21:10:12.018729 albert_toolkit-0.1.0/src/albert/resources/__init__.py
--rw-r--r--   0        0        0     4423 2023-03-21 21:10:12.019637 albert_toolkit-0.1.0/src/albert/resources/constants_en.txt
--rw-r--r--   0        0        0     9437 2023-03-21 21:10:12.019703 albert_toolkit-0.1.0/src/albert/resources/replace_rules.xlsx
--rw-r--r--   0        0        0    30373 2023-04-07 17:39:15.287090 albert_toolkit-0.1.0/src/albert/resources/unit_registry_custom.txt
--rw-r--r--   0        0        0       34 2023-01-26 22:14:09.774088 albert_toolkit-0.1.0/src/albert/session/__init__.py
--rw-r--r--   0        0        0     6620 2023-04-10 15:43:53.303824 albert_toolkit-0.1.0/src/albert/session/session.py
--rw-r--r--   0        0        0     1944 2023-02-24 19:24:57.948551 albert_toolkit-0.1.0/src/albert/session/token_manager.py
--rw-r--r--   0        0        0      169 2023-03-21 20:46:05.415645 albert_toolkit-0.1.0/src/albert/transforms/__init__.py
--rw-r--r--   0        0        0      415 2023-04-10 15:44:55.181803 albert_toolkit-0.1.0/src/albert/transforms/clustering_transforms.py
--rw-r--r--   0        0        0    17758 2023-03-21 20:46:05.416202 albert_toolkit-0.1.0/src/albert/transforms/dataframe_transforms.py
--rw-r--r--   0        0        0    11208 2023-03-23 15:19:49.329501 albert_toolkit-0.1.0/src/albert/transforms/formulation_transforms.py
--rw-r--r--   0        0        0      536 2023-04-10 15:44:55.181714 albert_toolkit-0.1.0/src/albert/transforms/molecular_transforms.py
--rw-r--r--   0        0        0     5921 2023-03-21 20:46:05.417113 albert_toolkit-0.1.0/src/albert/transforms/operating_condition_transforms.py
--rw-r--r--   0        0        0     2112 2023-03-21 20:46:05.417028 albert_toolkit-0.1.0/src/albert/transforms/property_transforms.py
--rw-r--r--   0        0        0     2385 2023-03-21 20:46:05.417809 albert_toolkit-0.1.0/src/albert/transforms/report_gather.py
--rw-r--r--   0        0        0     2039 2023-03-21 20:46:05.419237 albert_toolkit-0.1.0/src/albert/transforms/tests/test_dataframe_transforms.py
--rw-r--r--   0        0        0      270 2023-03-21 20:46:05.419868 albert_toolkit-0.1.0/src/albert/transforms/tests/test_formulation_pivot.py
--rw-r--r--   0        0        0     4016 2023-03-21 20:46:05.421066 albert_toolkit-0.1.0/src/albert/transforms/tests/test_report_gather.py
--rw-r--r--   0        0        0     1529 2023-03-21 20:46:05.420678 albert_toolkit-0.1.0/src/albert/transforms/tests/test_util_transforms.py
--rw-r--r--   0        0        0     7051 2023-03-21 20:46:05.420555 albert_toolkit-0.1.0/src/albert/transforms/util_transforms.py
--rw-r--r--   0        0        0       27 2023-03-21 21:10:12.019755 albert_toolkit-0.1.0/src/albert/unitconversion/__init__.py
--rw-r--r--   0        0        0    23589 2023-04-07 17:39:15.289569 albert_toolkit-0.1.0/src/albert/unitconversion/tests/test_unit_convert.py
--rw-r--r--   0        0        0    10123 2023-04-07 17:39:15.286892 albert_toolkit-0.1.0/src/albert/unitconversion/unit_convert.py
--rw-r--r--   0        0        0       20 2023-03-21 21:10:12.020663 albert_toolkit-0.1.0/src/albert/utils/__init__.py
--rw-r--r--   0        0        0     1280 2023-03-27 15:13:02.180149 albert_toolkit-0.1.0/src/albert/utils/utils.py
--rw-r--r--   0        0        0       21 2023-02-24 19:24:57.949823 albert_toolkit-0.1.0/src/albert/version.py
--rw-r--r--   0        0        0        0 2023-01-24 13:57:52.839885 albert_toolkit-0.1.0/src/albert/viz/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 13:57:52.839968 albert_toolkit-0.1.0/src/albert/viz/plots.py
--rw-r--r--   0        0        0     4663 2023-03-21 20:46:05.422241 albert_toolkit-0.1.0/src/albert/viz/umap_visualization.py
--rw-r--r--   0        0        0     1074 2023-03-21 20:46:05.422938 albert_toolkit-0.1.0/src/albert/viz/utils/dimension_reduction.py
--rw-r--r--   0        0        0     8494 1970-01-01 00:00:00.000000 albert_toolkit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5685 2023-04-10 18:43:41.820012 albert_toolkit-0.1.1/README.md
+-rw-r--r--   0        0        0     2798 2023-04-10 18:44:14.342638 albert_toolkit-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-31 20:03:24.700210 albert_toolkit-0.1.1/src/albert/__init__.py
+-rw-r--r--   0        0        0     3688 2023-04-06 15:59:29.098549 albert_toolkit-0.1.1/src/albert/albert.py
+-rw-r--r--   0        0        0      735 2023-03-14 15:56:43.726528 albert_toolkit-0.1.1/src/albert/api/__init__.py
+-rw-r--r--   0        0        0    58500 2023-03-14 15:56:43.726667 albert_toolkit-0.1.1/src/albert/api/api_client.py
+-rw-r--r--   0        0        0      214 2023-03-13 19:46:33.000000 albert_toolkit-0.1.1/src/albert/api/apis/__init__.py
+-rw-r--r--   0        0        0     9535 2023-03-21 20:46:05.377307 albert_toolkit-0.1.1/src/albert/api/apis/path_to_api.py
+-rw-r--r--   0        0        0      237 2023-03-13 19:46:32.000000 albert_toolkit-0.1.1/src/albert/api/apis/paths/__init__.py
+-rw-r--r--   0        0        0      195 2023-03-21 20:46:05.376226 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_inventories.py
+-rw-r--r--   0        0        0      128 2023-03-21 20:46:05.377222 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_inventories_health.py
+-rw-r--r--   0        0        0      295 2023-03-21 20:46:05.376142 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_inventories_id.py
+-rw-r--r--   0        0        0      189 2023-03-13 19:46:24.000000 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_locations.py
+-rw-r--r--   0        0        0      211 2023-03-14 15:56:43.739587 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_locations_async_id.py
+-rw-r--r--   0        0        0      124 2023-03-13 19:46:20.000000 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_locations_health.py
+-rw-r--r--   0        0        0      287 2023-03-13 20:14:13.723672 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_locations_id.py
+-rw-r--r--   0        0        0      195 2023-03-14 15:56:43.739388 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_predictions.py
+-rw-r--r--   0        0        0      128 2023-03-14 15:56:43.739499 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_predictions_health.py
+-rw-r--r--   0        0        0      135 2023-03-14 15:56:43.739662 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_predictions_mergedac.py
+-rw-r--r--   0        0        0      135 2023-03-14 15:56:43.740248 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_predictions_mergedat.py
+-rw-r--r--   0        0        0      215 2023-03-14 15:56:43.740316 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_predictions_models.py
+-rw-r--r--   0        0        0      133 2023-03-14 15:56:43.740403 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_predictions_models_id.py
+-rw-r--r--   0        0        0      380 2023-03-14 15:56:43.740963 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_predictions_models_parent_id_version.py
+-rw-r--r--   0        0        0      166 2023-03-14 15:56:43.741196 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_predictions_models_parent_id_version_id.py
+-rw-r--r--   0        0        0      139 2023-03-14 15:56:43.742325 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_predictions_parent_id.py
+-rw-r--r--   0        0        0      129 2023-03-14 15:56:43.741941 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_predictions_tasks.py
+-rw-r--r--   0        0        0      201 2023-03-14 15:56:43.742702 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_productdesign.py
+-rw-r--r--   0        0        0      132 2023-03-14 15:56:43.741793 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_productdesign_health.py
+-rw-r--r--   0        0        0      124 2023-03-14 15:56:43.742059 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_productdesign_id.py
+-rw-r--r--   0        0        0      427 2023-03-14 15:56:43.742241 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_productdesign_id_designs.py
+-rw-r--r--   0        0        0      133 2023-03-14 15:56:43.742137 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_productdesign_id_grid.py
+-rw-r--r--   0        0        0      144 2023-03-14 15:56:43.741850 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_productdesign_id_products.py
+-rw-r--r--   0        0        0      137 2023-03-14 15:56:43.742546 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_productdesign_id_unpack.py
+-rw-r--r--   0        0        0      143 2023-03-14 15:56:43.752434 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_productdesign_id_values.py
+-rw-r--r--   0        0        0      241 2023-03-14 15:56:43.752618 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_productdesign_inventories_id.py
+-rw-r--r--   0        0        0      151 2023-03-14 15:56:43.752720 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_productdesign_mergeinventory.py
+-rw-r--r--   0        0        0      132 2023-03-14 15:56:43.753024 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_productdesign_search.py
+-rw-r--r--   0        0        0      134 2023-03-14 15:56:43.752809 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_productdesign_suggest.py
+-rw-r--r--   0        0        0      183 2023-03-13 19:46:31.000000 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_reports.py
+-rw-r--r--   0        0        0      131 2023-03-13 19:46:19.000000 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_reports_analytics_id.py
+-rw-r--r--   0        0        0      119 2023-03-13 19:46:31.000000 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_reports_copy.py
+-rw-r--r--   0        0        0      135 2023-03-13 19:46:19.000000 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_reports_datascience_id.py
+-rw-r--r--   0        0        0      120 2023-03-13 19:46:20.000000 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_reports_health.py
+-rw-r--r--   0        0        0      273 2023-03-13 20:14:13.728098 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_reports_id.py
+-rw-r--r--   0        0        0      156 2023-03-13 20:14:13.728814 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_reports_inventory_equipment_usage.py
+-rw-r--r--   0        0        0      145 2023-03-13 19:46:28.000000 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_reports_inventory_movements.py
+-rw-r--r--   0        0        0      120 2023-03-13 19:46:32.000000 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_reports_search.py
+-rw-r--r--   0        0        0      122 2023-03-13 19:46:30.000000 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_reports_suggest.py
+-rw-r--r--   0        0        0      281 2023-03-13 20:14:13.729561 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_reports_type.py
+-rw-r--r--   0        0        0      121 2023-03-13 19:46:28.000000 albert_toolkit-0.1.1/src/albert/api/apis/paths/api_v3_reports_type_id.py
+-rw-r--r--   0        0        0     3003 2023-03-21 20:46:05.378651 albert_toolkit-0.1.1/src/albert/api/apis/tag_to_api.py
+-rw-r--r--   0        0        0      838 2023-03-21 20:46:05.379448 albert_toolkit-0.1.1/src/albert/api/apis/tags/__init__.py
+-rw-r--r--   0        0        0      658 2023-03-14 15:56:43.760379 albert_toolkit-0.1.1/src/albert/api/apis/tags/analytics_api.py
+-rw-r--r--   0        0        0      538 2023-03-14 15:56:43.760471 albert_toolkit-0.1.1/src/albert/api/apis/tags/columns_api.py
+-rw-r--r--   0        0        0      514 2023-03-14 15:56:43.760642 albert_toolkit-0.1.1/src/albert/api/apis/tags/default_api.py
+-rw-r--r--   0        0        0      510 2023-03-14 15:56:43.760562 albert_toolkit-0.1.1/src/albert/api/apis/tags/grid_api.py
+-rw-r--r--   0        0        0      854 2023-03-21 20:46:05.379320 albert_toolkit-0.1.1/src/albert/api/apis/tags/health_check_api.py
+-rw-r--r--   0        0        0     1216 2023-03-14 15:56:43.760814 albert_toolkit-0.1.1/src/albert/api/apis/tags/internal_api.py
+-rw-r--r--   0        0        0      898 2023-03-21 20:46:05.384851 albert_toolkit-0.1.1/src/albert/api/apis/tags/inventory_api.py
+-rw-r--r--   0        0        0      876 2023-03-14 15:56:43.768745 albert_toolkit-0.1.1/src/albert/api/apis/tags/locations_api.py
+-rw-r--r--   0        0        0      543 2023-03-14 15:56:43.768664 albert_toolkit-0.1.1/src/albert/api/apis/tags/prediction_flow_api.py
+-rw-r--r--   0        0        0     1157 2023-03-14 15:56:43.768894 albert_toolkit-0.1.1/src/albert/api/apis/tags/prediction_models_api.py
+-rw-r--r--   0        0        0      710 2023-03-14 15:56:43.769040 albert_toolkit-0.1.1/src/albert/api/apis/tags/predictions_api.py
+-rw-r--r--   0        0        0      942 2023-03-14 15:56:43.769149 albert_toolkit-0.1.1/src/albert/api/apis/tags/product_design_api.py
+-rw-r--r--   0        0        0      801 2023-03-14 15:56:43.769263 albert_toolkit-0.1.1/src/albert/api/apis/tags/reports_catalogue_api.py
+-rw-r--r--   0        0        0      690 2023-03-14 15:56:43.772182 albert_toolkit-0.1.1/src/albert/api/apis/tags/reports_sp_api.py
+-rw-r--r--   0        0        0      851 2023-03-14 15:56:43.771708 albert_toolkit-0.1.1/src/albert/api/apis/tags/rows_api.py
+-rw-r--r--   0        0        0      516 2023-03-14 15:56:43.773369 albert_toolkit-0.1.1/src/albert/api/apis/tags/search_api.py
+-rw-r--r--   0        0        0      522 2023-03-14 15:56:43.773239 albert_toolkit-0.1.1/src/albert/api/apis/tags/unpack_api.py
+-rw-r--r--   0        0        0      931 2023-03-14 15:56:43.773977 albert_toolkit-0.1.1/src/albert/api/apis/tags/user_reports_api.py
+-rw-r--r--   0        0        0      530 2023-03-14 15:56:43.774342 albert_toolkit-0.1.1/src/albert/api/apis/tags/values_api.py
+-rw-r--r--   0        0        0    15750 2023-03-14 15:56:43.774891 albert_toolkit-0.1.1/src/albert/api/configuration.py
+-rw-r--r--   0        0        0     4530 2023-03-14 15:56:43.775570 albert_toolkit-0.1.1/src/albert/api/exceptions.py
+-rw-r--r--   0        0        0      344 2023-03-13 19:46:33.000000 albert_toolkit-0.1.1/src/albert/api/model/__init__.py
+-rw-r--r--   0        0        0     7152 2023-03-14 15:56:43.776709 albert_toolkit-0.1.1/src/albert/api/model/add.py
+-rw-r--r--   0        0        0     6682 2023-03-14 15:56:43.776330 albert_toolkit-0.1.1/src/albert/api/model/add.pyi
+-rw-r--r--   0        0        0     4592 2023-03-14 15:56:43.776206 albert_toolkit-0.1.1/src/albert/api/model/cas.py
+-rw-r--r--   0        0        0     4302 2023-03-14 15:56:43.776425 albert_toolkit-0.1.1/src/albert/api/model/cas.pyi
+-rw-r--r--   0        0        0     9457 2023-03-14 15:56:43.776589 albert_toolkit-0.1.1/src/albert/api/model/column_copy_to_existing.py
+-rw-r--r--   0        0        0     9266 2023-03-14 15:56:43.776799 albert_toolkit-0.1.1/src/albert/api/model/column_copy_to_existing.pyi
+-rw-r--r--   0        0        0     9615 2023-03-14 15:56:43.777053 albert_toolkit-0.1.1/src/albert/api/model/column_copy_to_new.py
+-rw-r--r--   0        0        0     9316 2023-03-14 15:56:43.776651 albert_toolkit-0.1.1/src/albert/api/model/column_copy_to_new.pyi
+-rw-r--r--   0        0        0     2301 2023-03-14 15:56:43.776514 albert_toolkit-0.1.1/src/albert/api/model/columns.py
+-rw-r--r--   0        0        0     2301 2023-03-14 15:56:43.776944 albert_toolkit-0.1.1/src/albert/api/model/columns.pyi
+-rw-r--r--   0        0        0     4119 2023-03-14 15:56:43.779720 albert_toolkit-0.1.1/src/albert/api/model/component_input.py
+-rw-r--r--   0        0        0     4119 2023-03-14 15:56:43.780161 albert_toolkit-0.1.1/src/albert/api/model/component_input.pyi
+-rw-r--r--   0        0        0     2006 2023-03-14 15:56:43.780889 albert_toolkit-0.1.1/src/albert/api/model/copy_report.py
+-rw-r--r--   0        0        0     2006 2023-03-14 15:56:43.781926 albert_toolkit-0.1.1/src/albert/api/model/copy_report.pyi
+-rw-r--r--   0        0        0    11943 2023-03-14 15:56:43.782602 albert_toolkit-0.1.1/src/albert/api/model/data_model.py
+-rw-r--r--   0        0        0    11519 2023-03-14 15:56:43.782066 albert_toolkit-0.1.1/src/albert/api/model/data_model.pyi
+-rw-r--r--   0        0        0     8252 2023-03-14 15:56:43.783276 albert_toolkit-0.1.1/src/albert/api/model/default_columns.py
+-rw-r--r--   0        0        0     8083 2023-03-14 15:56:43.782863 albert_toolkit-0.1.1/src/albert/api/model/default_columns.pyi
+-rw-r--r--   0        0        0     7170 2023-03-14 15:56:43.782682 albert_toolkit-0.1.1/src/albert/api/model/delete.py
+-rw-r--r--   0        0        0     6694 2023-03-14 15:56:43.784814 albert_toolkit-0.1.1/src/albert/api/model/delete.pyi
+-rw-r--r--   0        0        0     4591 2023-03-14 15:56:43.784532 albert_toolkit-0.1.1/src/albert/api/model/denormalized_inventories.py
+-rw-r--r--   0        0        0     4591 2023-03-14 15:56:43.783020 albert_toolkit-0.1.1/src/albert/api/model/denormalized_inventories.pyi
+-rw-r--r--   0        0        0     7677 2023-03-14 15:56:43.782496 albert_toolkit-0.1.1/src/albert/api/model/denormalized_inventory.py
+-rw-r--r--   0        0        0     7677 2023-03-14 15:56:43.784901 albert_toolkit-0.1.1/src/albert/api/model/denormalized_inventory.pyi
+-rw-r--r--   0        0        0     8167 2023-03-14 15:56:43.785545 albert_toolkit-0.1.1/src/albert/api/model/designs.py
+-rw-r--r--   0        0        0     7952 2023-03-14 15:56:43.785718 albert_toolkit-0.1.1/src/albert/api/model/designs.pyi
+-rw-r--r--   0        0        0     2568 2023-03-14 15:56:43.789016 albert_toolkit-0.1.1/src/albert/api/model/entity_tags.py
+-rw-r--r--   0        0        0     2568 2023-03-14 15:56:43.787750 albert_toolkit-0.1.1/src/albert/api/model/entity_tags.pyi
+-rw-r--r--   0        0        0    12073 2023-03-14 15:56:43.789817 albert_toolkit-0.1.1/src/albert/api/model/equipment.py
+-rw-r--r--   0        0        0    12073 2023-03-14 15:56:43.790448 albert_toolkit-0.1.1/src/albert/api/model/equipment.pyi
+-rw-r--r--   0        0        0    12117 2023-03-14 15:56:43.791062 albert_toolkit-0.1.1/src/albert/api/model/error.py
+-rw-r--r--   0        0        0    11792 2023-03-14 15:56:43.792119 albert_toolkit-0.1.1/src/albert/api/model/error.pyi
+-rw-r--r--   0        0        0     8099 2023-03-14 15:56:43.792027 albert_toolkit-0.1.1/src/albert/api/model/facet_with_value_array.py
+-rw-r--r--   0        0        0     8099 2023-03-14 15:56:43.792228 albert_toolkit-0.1.1/src/albert/api/model/facet_with_value_array.pyi
+-rw-r--r--   0        0        0    12294 2023-03-14 15:56:43.792564 albert_toolkit-0.1.1/src/albert/api/model/formula_item.py
+-rw-r--r--   0        0        0    12294 2023-03-14 15:56:43.792776 albert_toolkit-0.1.1/src/albert/api/model/formula_item.pyi
+-rw-r--r--   0        0        0     3760 2023-03-14 15:56:43.792440 albert_toolkit-0.1.1/src/albert/api/model/get_back_update_companies.py
+-rw-r--r--   0        0        0     3760 2023-03-14 15:56:43.798617 albert_toolkit-0.1.1/src/albert/api/model/get_back_update_companies.pyi
+-rw-r--r--   0        0        0    36595 2023-03-14 15:56:43.798795 albert_toolkit-0.1.1/src/albert/api/model/grid.py
+-rw-r--r--   0        0        0    35002 2023-03-14 15:56:43.792917 albert_toolkit-0.1.1/src/albert/api/model/grid.pyi
+-rw-r--r--   0        0        0     3004 2023-03-14 15:56:43.807149 albert_toolkit-0.1.1/src/albert/api/model/health.py
+-rw-r--r--   0        0        0     3004 2023-03-14 15:56:43.807231 albert_toolkit-0.1.1/src/albert/api/model/health.pyi
+-rw-r--r--   0        0        0     4436 2023-03-14 15:56:43.807396 albert_toolkit-0.1.1/src/albert/api/model/inputs.py
+-rw-r--r--   0        0        0     4436 2023-03-14 15:56:43.807311 albert_toolkit-0.1.1/src/albert/api/model/inputs.pyi
+-rw-r--r--   0        0        0    19222 2023-03-21 20:46:05.384935 albert_toolkit-0.1.1/src/albert/api/model/inventories.py
+-rw-r--r--   0        0        0    17436 2023-03-21 20:46:05.384741 albert_toolkit-0.1.1/src/albert/api/model/inventories.pyi
+-rw-r--r--   0        0        0    13541 2023-03-21 20:46:05.385022 albert_toolkit-0.1.1/src/albert/api/model/inventory.py
+-rw-r--r--   0        0        0    12217 2023-03-21 20:46:05.381651 albert_toolkit-0.1.1/src/albert/api/model/inventory.pyi
+-rw-r--r--   0        0        0    15702 2023-03-14 15:56:43.812195 albert_toolkit-0.1.1/src/albert/api/model/location.py
+-rw-r--r--   0        0        0    14824 2023-03-14 15:56:43.812727 albert_toolkit-0.1.1/src/albert/api/model/location.pyi
+-rw-r--r--   0        0        0     4058 2023-03-14 15:56:43.819729 albert_toolkit-0.1.1/src/albert/api/model/locations.py
+-rw-r--r--   0        0        0     4058 2023-03-14 15:56:43.820069 albert_toolkit-0.1.1/src/albert/api/model/locations.pyi
+-rw-r--r--   0        0        0     5803 2023-03-14 15:56:43.820001 albert_toolkit-0.1.1/src/albert/api/model/merged_dac.py
+-rw-r--r--   0        0        0     5630 2023-03-14 15:56:43.819815 albert_toolkit-0.1.1/src/albert/api/model/merged_dac.pyi
+-rw-r--r--   0        0        0     5803 2023-03-14 15:56:43.820183 albert_toolkit-0.1.1/src/albert/api/model/merged_dat.py
+-rw-r--r--   0        0        0     5630 2023-03-14 15:56:43.820410 albert_toolkit-0.1.1/src/albert/api/model/merged_dat.pyi
+-rw-r--r--   0        0        0     5977 2023-03-14 15:56:43.820315 albert_toolkit-0.1.1/src/albert/api/model/merged_inventory.py
+-rw-r--r--   0        0        0     5804 2023-03-14 15:56:43.819871 albert_toolkit-0.1.1/src/albert/api/model/merged_inventory.pyi
+-rw-r--r--   0        0        0     3034 2023-03-21 20:46:05.385130 albert_toolkit-0.1.1/src/albert/api/model/minimum.py
+-rw-r--r--   0        0        0     2889 2023-03-21 20:46:05.385217 albert_toolkit-0.1.1/src/albert/api/model/minimum.pyi
+-rw-r--r--   0        0        0    10846 2023-03-14 15:56:43.824405 albert_toolkit-0.1.1/src/albert/api/model/model_patch.py
+-rw-r--r--   0        0        0     9768 2023-03-14 15:56:43.824474 albert_toolkit-0.1.1/src/albert/api/model/model_patch.pyi
+-rw-r--r--   0        0        0    36660 2023-03-14 15:56:43.824607 albert_toolkit-0.1.1/src/albert/api/model/model_prediction.py
+-rw-r--r--   0        0        0    36408 2023-03-14 15:56:43.825032 albert_toolkit-0.1.1/src/albert/api/model/model_prediction.pyi
+-rw-r--r--   0        0        0     6338 2023-03-14 15:56:43.824769 albert_toolkit-0.1.1/src/albert/api/model/model_predictions.py
+-rw-r--r--   0        0        0     6338 2023-03-14 15:56:43.825289 albert_toolkit-0.1.1/src/albert/api/model/model_predictions.pyi
+-rw-r--r--   0        0        0    31893 2023-03-14 15:56:43.825435 albert_toolkit-0.1.1/src/albert/api/model/model_predictions_values_only.py
+-rw-r--r--   0        0        0    31641 2023-03-14 15:56:43.825147 albert_toolkit-0.1.1/src/albert/api/model/model_predictions_values_only.pyi
+-rw-r--r--   0        0        0    27904 2023-03-14 15:56:43.825764 albert_toolkit-0.1.1/src/albert/api/model/new_model_version.py
+-rw-r--r--   0        0        0    27525 2023-03-14 15:56:43.827113 albert_toolkit-0.1.1/src/albert/api/model/new_model_version.pyi
+-rw-r--r--   0        0        0    27362 2023-03-14 15:56:43.827193 albert_toolkit-0.1.1/src/albert/api/model/output.py
+-rw-r--r--   0        0        0    27253 2023-03-14 15:56:43.827274 albert_toolkit-0.1.1/src/albert/api/model/output.pyi
+-rw-r--r--   0        0        0     7402 2023-03-14 15:56:43.827343 albert_toolkit-0.1.1/src/albert/api/model/parameter.py
+-rw-r--r--   0        0        0     7214 2023-03-14 15:56:43.828315 albert_toolkit-0.1.1/src/albert/api/model/parameter.pyi
+-rw-r--r--   0        0        0    13128 2023-03-14 15:56:43.828426 albert_toolkit-0.1.1/src/albert/api/model/partial_product_design.py
+-rw-r--r--   0        0        0    13128 2023-03-14 15:56:43.828527 albert_toolkit-0.1.1/src/albert/api/model/partial_product_design.pyi
+-rw-r--r--   0        0        0    19513 2023-03-14 15:56:43.835360 albert_toolkit-0.1.1/src/albert/api/model/partial_success.py
+-rw-r--r--   0        0        0    19513 2023-03-14 15:56:43.836701 albert_toolkit-0.1.1/src/albert/api/model/partial_success.pyi
+-rw-r--r--   0        0        0     8043 2023-03-14 15:56:43.836524 albert_toolkit-0.1.1/src/albert/api/model/partial_success1.py
+-rw-r--r--   0        0        0     7858 2023-03-14 15:56:43.836770 albert_toolkit-0.1.1/src/albert/api/model/partial_success1.pyi
+-rw-r--r--   0        0        0    40104 2023-03-14 15:56:43.836856 albert_toolkit-0.1.1/src/albert/api/model/partial_success_post.py
+-rw-r--r--   0        0        0    40104 2023-03-14 15:56:43.855897 albert_toolkit-0.1.1/src/albert/api/model/partial_success_post.pyi
+-rw-r--r--   0        0        0    11412 2023-03-14 15:56:43.855758 albert_toolkit-0.1.1/src/albert/api/model/patch.py
+-rw-r--r--   0        0        0    10083 2023-03-14 15:56:43.856207 albert_toolkit-0.1.1/src/albert/api/model/patch.pyi
+-rw-r--r--   0        0        0    10045 2023-03-14 15:56:43.856129 albert_toolkit-0.1.1/src/albert/api/model/patch1.py
+-rw-r--r--   0        0        0     9399 2023-03-14 15:56:43.856027 albert_toolkit-0.1.1/src/albert/api/model/patch1.pyi
+-rw-r--r--   0        0        0    13810 2023-03-14 15:56:43.856362 albert_toolkit-0.1.1/src/albert/api/model/patch_blk.py
+-rw-r--r--   0        0        0    13144 2023-03-14 15:56:43.856299 albert_toolkit-0.1.1/src/albert/api/model/patch_blk.pyi
+-rw-r--r--   0        0        0    13519 2023-03-21 20:46:05.385929 albert_toolkit-0.1.1/src/albert/api/model/patch_inventory.py
+-rw-r--r--   0        0        0    11787 2023-03-21 20:46:05.385999 albert_toolkit-0.1.1/src/albert/api/model/patch_inventory.pyi
+-rw-r--r--   0        0        0    17163 2023-03-14 15:56:43.865408 albert_toolkit-0.1.1/src/albert/api/model/patch_prediction.py
+-rw-r--r--   0        0        0    16148 2023-03-14 15:56:43.865207 albert_toolkit-0.1.1/src/albert/api/model/patch_prediction.pyi
+-rw-r--r--   0        0        0    18767 2023-03-14 15:56:43.866047 albert_toolkit-0.1.1/src/albert/api/model/patch_type.py
+-rw-r--r--   0        0        0    17847 2023-03-14 15:56:43.867398 albert_toolkit-0.1.1/src/albert/api/model/patch_type.pyi
+-rw-r--r--   0        0        0     3430 2023-03-14 15:56:43.866818 albert_toolkit-0.1.1/src/albert/api/model/patch_types.py
+-rw-r--r--   0        0        0     3430 2023-03-14 15:56:43.868535 albert_toolkit-0.1.1/src/albert/api/model/patch_types.pyi
+-rw-r--r--   0        0        0     4668 2023-03-14 15:56:43.869076 albert_toolkit-0.1.1/src/albert/api/model/pd_row.py
+-rw-r--r--   0        0        0     4431 2023-03-14 15:56:43.868613 albert_toolkit-0.1.1/src/albert/api/model/pd_row.pyi
+-rw-r--r--   0        0        0     4435 2023-03-14 15:56:43.868957 albert_toolkit-0.1.1/src/albert/api/model/pd_rows.py
+-rw-r--r--   0        0        0     4435 2023-03-14 15:56:43.868793 albert_toolkit-0.1.1/src/albert/api/model/pd_rows.pyi
+-rw-r--r--   0        0        0     9133 2023-03-14 15:56:43.869009 albert_toolkit-0.1.1/src/albert/api/model/post_partial_success.py
+-rw-r--r--   0        0        0     8944 2023-03-14 15:56:43.868721 albert_toolkit-0.1.1/src/albert/api/model/post_partial_success.pyi
+-rw-r--r--   0        0        0     1385 2023-03-14 15:56:43.869130 albert_toolkit-0.1.1/src/albert/api/model/post_pd_rows.py
+-rw-r--r--   0        0        0     1340 2023-03-14 15:56:43.868876 albert_toolkit-0.1.1/src/albert/api/model/post_pd_rows.pyi
+-rw-r--r--   0        0        0     5787 2023-03-14 15:56:43.869212 albert_toolkit-0.1.1/src/albert/api/model/post_prediction_partial_success.py
+-rw-r--r--   0        0        0     5787 2023-03-14 15:56:43.871824 albert_toolkit-0.1.1/src/albert/api/model/post_prediction_partial_success.pyi
+-rw-r--r--   0        0        0     2921 2023-03-14 15:56:43.870258 albert_toolkit-0.1.1/src/albert/api/model/post_to_scheduler_success.py
+-rw-r--r--   0        0        0     2921 2023-03-14 15:56:43.872301 albert_toolkit-0.1.1/src/albert/api/model/post_to_scheduler_success.pyi
+-rw-r--r--   0        0        0    14562 2023-03-14 15:56:43.871633 albert_toolkit-0.1.1/src/albert/api/model/prediction_data_model.py
+-rw-r--r--   0        0        0    13330 2023-03-14 15:56:43.870541 albert_toolkit-0.1.1/src/albert/api/model/prediction_data_model.pyi
+-rw-r--r--   0        0        0    11219 2023-03-14 15:56:43.870632 albert_toolkit-0.1.1/src/albert/api/model/prediction_data_model_success.py
+-rw-r--r--   0        0        0    10507 2023-03-14 15:56:43.871923 albert_toolkit-0.1.1/src/albert/api/model/prediction_data_model_success.pyi
+-rw-r--r--   0        0        0    34269 2023-03-14 15:56:43.870373 albert_toolkit-0.1.1/src/albert/api/model/prediction_model.py
+-rw-r--r--   0        0        0    33466 2023-03-14 15:56:43.870469 albert_toolkit-0.1.1/src/albert/api/model/prediction_model.pyi
+-rw-r--r--   0        0        0     4041 2023-03-14 15:56:43.871706 albert_toolkit-0.1.1/src/albert/api/model/prediction_model_versions.py
+-rw-r--r--   0        0        0     4007 2023-03-14 15:56:43.872214 albert_toolkit-0.1.1/src/albert/api/model/prediction_model_versions.pyi
+-rw-r--r--   0        0        0     3923 2023-03-14 15:56:43.872384 albert_toolkit-0.1.1/src/albert/api/model/prediction_models.py
+-rw-r--r--   0        0        0     3889 2023-03-14 15:56:43.872582 albert_toolkit-0.1.1/src/albert/api/model/prediction_models.pyi
+-rw-r--r--   0        0        0    23689 2023-03-14 15:56:43.872130 albert_toolkit-0.1.1/src/albert/api/model/product_design.py
+-rw-r--r--   0        0        0    22680 2023-03-14 15:56:43.872021 albert_toolkit-0.1.1/src/albert/api/model/product_design.pyi
+-rw-r--r--   0        0        0     6925 2023-03-14 15:56:43.872748 albert_toolkit-0.1.1/src/albert/api/model/product_design_search_result.py
+-rw-r--r--   0        0        0     6925 2023-03-14 15:56:43.873647 albert_toolkit-0.1.1/src/albert/api/model/product_design_search_result.pyi
+-rw-r--r--   0        0        0     3355 2023-03-14 15:56:43.873782 albert_toolkit-0.1.1/src/albert/api/model/product_design_suggest_result.py
+-rw-r--r--   0        0        0     3321 2023-03-14 15:56:43.874007 albert_toolkit-0.1.1/src/albert/api/model/product_design_suggest_result.pyi
+-rw-r--r--   0        0        0     4061 2023-03-14 15:56:43.874062 albert_toolkit-0.1.1/src/albert/api/model/product_designs.py
+-rw-r--r--   0        0        0     4061 2023-03-14 15:56:43.874191 albert_toolkit-0.1.1/src/albert/api/model/product_designs.pyi
+-rw-r--r--   0        0        0    20064 2023-03-14 15:56:43.889603 albert_toolkit-0.1.1/src/albert/api/model/property_task_data_model.py
+-rw-r--r--   0        0        0    19674 2023-03-14 15:56:43.874256 albert_toolkit-0.1.1/src/albert/api/model/property_task_data_model.pyi
+-rw-r--r--   0        0        0     3969 2023-03-14 15:56:43.873944 albert_toolkit-0.1.1/src/albert/api/model/put_back_update_companies.py
+-rw-r--r--   0        0        0     3969 2023-03-14 15:56:43.873870 albert_toolkit-0.1.1/src/albert/api/model/put_back_update_companies.pyi
+-rw-r--r--   0        0        0     6968 2023-03-21 20:46:05.390703 albert_toolkit-0.1.1/src/albert/api/model/put_report.py
+-rw-r--r--   0        0        0     6968 2023-03-21 20:46:05.390801 albert_toolkit-0.1.1/src/albert/api/model/put_report.pyi
+-rw-r--r--   0        0        0    12229 2023-03-21 20:46:05.391600 albert_toolkit-0.1.1/src/albert/api/model/report.py
+-rw-r--r--   0        0        0    12045 2023-03-21 20:46:05.392646 albert_toolkit-0.1.1/src/albert/api/model/report.pyi
+-rw-r--r--   0        0        0     3931 2023-03-14 15:56:43.921553 albert_toolkit-0.1.1/src/albert/api/model/report_list.py
+-rw-r--r--   0        0        0     3931 2023-03-14 15:56:43.922029 albert_toolkit-0.1.1/src/albert/api/model/report_list.pyi
+-rw-r--r--   0        0        0     6303 2023-03-14 15:56:43.922919 albert_toolkit-0.1.1/src/albert/api/model/report_search_result.py
+-rw-r--r--   0        0        0     6303 2023-03-14 15:56:43.924235 albert_toolkit-0.1.1/src/albert/api/model/report_search_result.pyi
+-rw-r--r--   0        0        0     3341 2023-03-14 15:56:43.925781 albert_toolkit-0.1.1/src/albert/api/model/report_suggest_result.py
+-rw-r--r--   0        0        0     3307 2023-03-14 15:56:43.924984 albert_toolkit-0.1.1/src/albert/api/model/report_suggest_result.pyi
+-rw-r--r--   0        0        0     8527 2023-03-14 15:56:43.926506 albert_toolkit-0.1.1/src/albert/api/model/report_type.py
+-rw-r--r--   0        0        0     8254 2023-03-14 15:56:43.926779 albert_toolkit-0.1.1/src/albert/api/model/report_type.pyi
+-rw-r--r--   0        0        0     3968 2023-03-14 15:56:43.927655 albert_toolkit-0.1.1/src/albert/api/model/report_type_list.py
+-rw-r--r--   0        0        0     3968 2023-03-14 15:56:43.928431 albert_toolkit-0.1.1/src/albert/api/model/report_type_list.pyi
+-rw-r--r--   0        0        0     3360 2023-03-14 15:56:43.928527 albert_toolkit-0.1.1/src/albert/api/model/task_workflow.py
+-rw-r--r--   0        0        0     3338 2023-03-14 15:56:43.928186 albert_toolkit-0.1.1/src/albert/api/model/task_workflow.pyi
+-rw-r--r--   0        0        0    58448 2023-03-14 15:56:43.928301 albert_toolkit-0.1.1/src/albert/api/model/unpack.py
+-rw-r--r--   0        0        0    58448 2023-03-14 15:56:43.928367 albert_toolkit-0.1.1/src/albert/api/model/unpack.pyi
+-rw-r--r--   0        0        0     7179 2023-03-14 15:56:43.928604 albert_toolkit-0.1.1/src/albert/api/model/update.py
+-rw-r--r--   0        0        0     6703 2023-03-14 15:56:43.928676 albert_toolkit-0.1.1/src/albert/api/model/update.pyi
+-rw-r--r--   0        0        0    12003 2023-03-14 15:56:43.928794 albert_toolkit-0.1.1/src/albert/api/model/values.py
+-rw-r--r--   0        0        0    11873 2023-03-14 15:56:43.974127 albert_toolkit-0.1.1/src/albert/api/model/values.pyi
+-rw-r--r--   0        0        0     2475 2023-03-14 15:56:43.929067 albert_toolkit-0.1.1/src/albert/api/model/wf_all_accepted.py
+-rw-r--r--   0        0        0     2475 2023-03-14 15:56:43.993973 albert_toolkit-0.1.1/src/albert/api/model/wf_all_accepted.pyi
+-rw-r--r--   0        0        0    10222 2023-03-14 15:56:43.993892 albert_toolkit-0.1.1/src/albert/api/model/wf_partial_success.py
+-rw-r--r--   0        0        0    10222 2023-03-14 15:56:43.993791 albert_toolkit-0.1.1/src/albert/api/model/wf_partial_success.pyi
+-rw-r--r--   0        0        0     4905 2023-03-21 20:46:05.392774 albert_toolkit-0.1.1/src/albert/api/models/__init__.py
+-rw-r--r--   0        0        0     2907 2023-03-21 20:46:05.394672 albert_toolkit-0.1.1/src/albert/api/paths/__init__.py
+-rw-r--r--   0        0        0      315 2023-03-21 20:46:05.394986 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories/__init__.py
+-rw-r--r--   0        0        0    16564 2023-03-21 20:46:05.394771 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories/get.py
+-rw-r--r--   0        0        0    15744 2023-03-21 20:46:05.394876 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories/get.pyi
+-rw-r--r--   0        0        0    15750 2023-03-21 20:46:05.395082 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories/post.py
+-rw-r--r--   0        0        0    15496 2023-03-21 20:46:05.395171 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories/post.pyi
+-rw-r--r--   0        0        0      329 2023-03-21 20:46:05.395276 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories_health/__init__.py
+-rw-r--r--   0        0        0     7585 2023-03-21 20:46:05.395362 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories_health/get.py
+-rw-r--r--   0        0        0     7504 2023-03-21 20:46:05.395491 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories_health/get.pyi
+-rw-r--r--   0        0        0      321 2023-03-21 20:46:05.400709 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories_id/__init__.py
+-rw-r--r--   0        0        0    12176 2023-03-21 20:46:05.400776 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories_id/delete.py
+-rw-r--r--   0        0        0    11922 2023-03-21 20:46:05.401496 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories_id/delete.pyi
+-rw-r--r--   0        0        0    12316 2023-03-21 20:46:05.401136 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories_id/get.py
+-rw-r--r--   0        0        0    12062 2023-03-21 20:46:05.401250 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories_id/get.pyi
+-rw-r--r--   0        0        0    16515 2023-03-21 20:46:05.401345 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories_id/patch.py
+-rw-r--r--   0        0        0    16261 2023-03-21 20:46:05.401413 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories_id/patch.pyi
+-rw-r--r--   0        0        0      311 2023-03-13 19:46:24.000000 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations/__init__.py
+-rw-r--r--   0        0        0    15401 2023-03-14 15:56:44.155226 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations/get.py
+-rw-r--r--   0        0        0    14858 2023-03-14 15:56:44.155376 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations/get.pyi
+-rw-r--r--   0        0        0    13826 2023-03-14 15:56:44.156342 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations/post.py
+-rw-r--r--   0        0        0    13602 2023-03-14 15:56:44.156500 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations/post.pyi
+-rw-r--r--   0        0        0      329 2023-03-14 15:56:44.156581 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_async_id/__init__.py
+-rw-r--r--   0        0        0    15519 2023-03-14 15:56:44.156746 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_async_id/get.py
+-rw-r--r--   0        0        0    15087 2023-03-14 15:56:44.156928 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_async_id/get.pyi
+-rw-r--r--   0        0        0    16416 2023-03-14 15:56:44.156674 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_async_id/put.py
+-rw-r--r--   0        0        0    16162 2023-03-14 15:56:44.156999 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_async_id/put.pyi
+-rw-r--r--   0        0        0      325 2023-03-13 19:46:20.000000 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_health/__init__.py
+-rw-r--r--   0        0        0     7585 2023-03-14 15:56:44.158928 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_health/get.py
+-rw-r--r--   0        0        0     7504 2023-03-14 15:56:44.159721 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_health/get.pyi
+-rw-r--r--   0        0        0      317 2023-03-13 19:46:24.000000 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_id/__init__.py
+-rw-r--r--   0        0        0    12068 2023-03-14 15:56:44.160454 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_id/delete.py
+-rw-r--r--   0        0        0    11814 2023-03-14 15:56:44.161436 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_id/delete.pyi
+-rw-r--r--   0        0        0    12301 2023-03-14 15:56:44.161930 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_id/get.py
+-rw-r--r--   0        0        0    12047 2023-03-14 15:56:44.162643 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_id/get.pyi
+-rw-r--r--   0        0        0    16356 2023-03-14 15:56:44.167103 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_id/patch.py
+-rw-r--r--   0        0        0    16102 2023-03-14 15:56:44.167820 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_id/patch.pyi
+-rw-r--r--   0        0        0      315 2023-03-14 15:56:44.167246 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions/__init__.py
+-rw-r--r--   0        0        0    16527 2023-03-14 15:56:44.167656 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions/get.py
+-rw-r--r--   0        0        0    15923 2023-03-14 15:56:44.167389 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions/get.pyi
+-rw-r--r--   0        0        0    16821 2023-03-14 15:56:44.167518 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions/post.py
+-rw-r--r--   0        0        0    16567 2023-03-14 15:56:44.167742 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions/post.pyi
+-rw-r--r--   0        0        0      329 2023-03-14 15:56:44.167947 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_health/__init__.py
+-rw-r--r--   0        0        0     7637 2023-03-14 15:56:44.168604 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_health/get.py
+-rw-r--r--   0        0        0     7556 2023-03-14 15:56:44.169911 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_health/get.pyi
+-rw-r--r--   0        0        0      333 2023-03-14 15:56:44.169497 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_mergedac/__init__.py
+-rw-r--r--   0        0        0    15148 2023-03-14 15:56:44.169816 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_mergedac/post.py
+-rw-r--r--   0        0        0    14894 2023-03-14 15:56:44.171901 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_mergedac/post.pyi
+-rw-r--r--   0        0        0      333 2023-03-14 15:56:44.171192 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_mergedat/__init__.py
+-rw-r--r--   0        0        0    15148 2023-03-14 15:56:44.170833 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_mergedat/post.py
+-rw-r--r--   0        0        0    14894 2023-03-14 15:56:44.171023 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_mergedat/post.pyi
+-rw-r--r--   0        0        0      329 2023-03-14 15:56:44.170671 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models/__init__.py
+-rw-r--r--   0        0        0    13762 2023-03-14 15:56:44.170507 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models/get.py
+-rw-r--r--   0        0        0    13313 2023-03-14 15:56:44.171427 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models/get.pyi
+-rw-r--r--   0        0        0    14980 2023-03-14 15:56:44.171329 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models/post.py
+-rw-r--r--   0        0        0    14726 2023-03-14 15:56:44.171693 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models/post.pyi
+-rw-r--r--   0        0        0      335 2023-03-14 15:56:44.172067 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_id/__init__.py
+-rw-r--r--   0        0        0    16701 2023-03-14 15:56:44.172958 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_id/get.py
+-rw-r--r--   0        0        0    16217 2023-03-14 15:56:44.172849 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_id/get.pyi
+-rw-r--r--   0        0        0      365 2023-03-14 15:56:44.172578 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_parent_id_version/__init__.py
+-rw-r--r--   0        0        0    14450 2023-03-14 15:56:44.172729 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_parent_id_version/delete.py
+-rw-r--r--   0        0        0    14196 2023-03-14 15:56:44.173855 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_parent_id_version/delete.pyi
+-rw-r--r--   0        0        0    15059 2023-03-14 15:56:44.174601 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_parent_id_version/get.py
+-rw-r--r--   0        0        0    14683 2023-03-14 15:56:44.174466 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_parent_id_version/get.pyi
+-rw-r--r--   0        0        0    19259 2023-03-14 15:56:44.174139 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_parent_id_version/patch.py
+-rw-r--r--   0        0        0    19005 2023-03-14 15:56:44.174337 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_parent_id_version/patch.pyi
+-rw-r--r--   0        0        0      371 2023-03-14 15:56:44.174050 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_parent_id_version_id/__init__.py
+-rw-r--r--   0        0        0    13151 2023-03-14 15:56:44.174704 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_parent_id_version_id/get.py
+-rw-r--r--   0        0        0    12775 2023-03-14 15:56:44.175125 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_parent_id_version_id/get.pyi
+-rw-r--r--   0        0        0      335 2023-03-14 15:56:44.175027 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_parent_id/__init__.py
+-rw-r--r--   0        0        0    16477 2023-03-14 15:56:44.175194 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_parent_id/patch.py
+-rw-r--r--   0        0        0    16192 2023-03-14 15:56:44.176472 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_parent_id/patch.pyi
+-rw-r--r--   0        0        0      327 2023-03-14 15:56:44.176575 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_tasks/__init__.py
+-rw-r--r--   0        0        0    16206 2023-03-14 15:56:44.177574 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_tasks/post.py
+-rw-r--r--   0        0        0    15922 2023-03-14 15:56:44.177288 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_tasks/post.pyi
+-rw-r--r--   0        0        0      319 2023-03-14 15:56:44.177145 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign/__init__.py
+-rw-r--r--   0        0        0    14687 2023-03-14 15:56:44.178509 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign/get.py
+-rw-r--r--   0        0        0    14083 2023-03-14 15:56:44.177427 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign/get.pyi
+-rw-r--r--   0        0        0    15051 2023-03-14 15:56:44.177632 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign/post.py
+-rw-r--r--   0        0        0    14797 2023-03-14 15:56:44.178279 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign/post.pyi
+-rw-r--r--   0        0        0      333 2023-03-14 15:56:44.177838 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_health/__init__.py
+-rw-r--r--   0        0        0     7648 2023-03-14 15:56:44.178145 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_health/get.py
+-rw-r--r--   0        0        0     7567 2023-03-14 15:56:44.178005 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_health/get.pyi
+-rw-r--r--   0        0        0      325 2023-03-14 15:56:44.178691 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id/__init__.py
+-rw-r--r--   0        0        0    12691 2023-03-14 15:56:44.178879 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id/get.py
+-rw-r--r--   0        0        0    12437 2023-03-14 15:56:44.179044 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id/get.pyi
+-rw-r--r--   0        0        0      341 2023-03-14 15:56:44.180454 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_designs/__init__.py
+-rw-r--r--   0        0        0    30588 2023-03-14 15:56:44.179372 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_designs/delete.py
+-rw-r--r--   0        0        0    30184 2023-03-14 15:56:44.179183 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_designs/delete.pyi
+-rw-r--r--   0        0        0    15587 2023-03-14 15:56:44.179270 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_designs/get.py
+-rw-r--r--   0        0        0    15197 2023-03-14 15:56:44.180053 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_designs/get.pyi
+-rw-r--r--   0        0        0    20625 2023-03-14 15:56:44.179638 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_designs/patch.py
+-rw-r--r--   0        0        0    20371 2023-03-14 15:56:44.179458 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_designs/patch.pyi
+-rw-r--r--   0        0        0    22220 2023-03-14 15:56:44.180353 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_designs/post.py
+-rw-r--r--   0        0        0    21966 2023-03-14 15:56:44.180259 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_designs/post.pyi
+-rw-r--r--   0        0        0      335 2023-03-14 15:56:44.180692 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_grid/__init__.py
+-rw-r--r--   0        0        0    17566 2023-03-14 15:56:44.180905 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_grid/get.py
+-rw-r--r--   0        0        0    17027 2023-03-14 15:56:44.181834 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_grid/get.pyi
+-rw-r--r--   0        0        0      343 2023-03-14 15:56:44.181572 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_products/__init__.py
+-rw-r--r--   0        0        0    17234 2023-03-14 15:56:44.181676 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_products/post.py
+-rw-r--r--   0        0        0    16980 2023-03-14 15:56:44.181988 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_products/post.pyi
+-rw-r--r--   0        0        0      339 2023-03-14 15:56:44.182950 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_unpack/__init__.py
+-rw-r--r--   0        0        0    15329 2023-03-14 15:56:44.183150 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_unpack/get.py
+-rw-r--r--   0        0        0    15052 2023-03-14 15:56:44.183025 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_unpack/get.pyi
+-rw-r--r--   0        0        0      339 2023-03-14 15:56:44.183658 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_values/__init__.py
+-rw-r--r--   0        0        0    17790 2023-03-14 15:56:44.183903 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_values/patch.py
+-rw-r--r--   0        0        0    17506 2023-03-14 15:56:44.184023 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_values/patch.pyi
+-rw-r--r--   0        0        0      349 2023-03-14 15:56:44.184881 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_inventories_id/__init__.py
+-rw-r--r--   0        0        0    15886 2023-03-14 15:56:44.185162 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_inventories_id/get.py
+-rw-r--r--   0        0        0    15454 2023-03-14 15:56:44.185034 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_inventories_id/get.pyi
+-rw-r--r--   0        0        0    17918 2023-03-14 15:56:44.184942 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_inventories_id/put.py
+-rw-r--r--   0        0        0    17664 2023-03-14 15:56:44.185465 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_inventories_id/put.pyi
+-rw-r--r--   0        0        0      349 2023-03-14 15:56:44.185349 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_mergeinventory/__init__.py
+-rw-r--r--   0        0        0    15297 2023-03-14 15:56:44.185815 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_mergeinventory/post.py
+-rw-r--r--   0        0        0    15043 2023-03-14 15:56:44.185719 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_mergeinventory/post.pyi
+-rw-r--r--   0        0        0      333 2023-03-14 15:56:44.186066 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_search/__init__.py
+-rw-r--r--   0        0        0    23706 2023-03-14 15:56:44.185963 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_search/get.py
+-rw-r--r--   0        0        0    22381 2023-03-14 15:56:44.194482 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_search/get.pyi
+-rw-r--r--   0        0        0      335 2023-03-14 15:56:44.194614 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_suggest/__init__.py
+-rw-r--r--   0        0        0    13256 2023-03-14 15:56:44.194276 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_suggest/get.py
+-rw-r--r--   0        0        0    13002 2023-03-14 15:56:44.194403 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_suggest/get.pyi
+-rw-r--r--   0        0        0      307 2023-03-13 19:46:31.000000 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports/__init__.py
+-rw-r--r--   0        0        0    14402 2023-03-13 20:14:13.921607 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports/get.py
+-rw-r--r--   0        0        0    14073 2023-03-13 20:14:13.922779 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports/get.pyi
+-rw-r--r--   0        0        0    14898 2023-03-13 20:14:13.922868 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports/post.py
+-rw-r--r--   0        0        0    14644 2023-03-13 20:14:13.925464 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports/post.pyi
+-rw-r--r--   0        0        0      333 2023-03-13 19:46:19.000000 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_analytics_id/__init__.py
+-rw-r--r--   0        0        0    14926 2023-03-21 16:07:55.093588 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_analytics_id/get.py
+-rw-r--r--   0        0        0    14672 2023-03-14 15:56:44.194865 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_analytics_id/get.pyi
+-rw-r--r--   0        0        0      317 2023-03-13 19:46:31.000000 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_copy/__init__.py
+-rw-r--r--   0        0        0    14964 2023-03-13 20:14:13.925788 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_copy/post.py
+-rw-r--r--   0        0        0    14710 2023-03-13 20:14:13.925875 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_copy/post.pyi
+-rw-r--r--   0        0        0      337 2023-03-13 19:46:19.000000 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_datascience_id/__init__.py
+-rw-r--r--   0        0        0    14951 2023-03-25 21:10:11.094939 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_datascience_id/get.py
+-rw-r--r--   0        0        0    14697 2023-03-14 15:56:44.195088 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_datascience_id/get.pyi
+-rw-r--r--   0        0        0      321 2023-03-13 19:46:20.000000 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_health/__init__.py
+-rw-r--r--   0        0        0     7648 2023-03-21 20:46:05.401611 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_health/get.py
+-rw-r--r--   0        0        0     7567 2023-03-21 20:46:05.408631 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_health/get.pyi
+-rw-r--r--   0        0        0      313 2023-03-13 19:46:31.000000 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_id/__init__.py
+-rw-r--r--   0        0        0    12309 2023-03-13 20:14:13.930104 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_id/delete.py
+-rw-r--r--   0        0        0    12055 2023-03-13 20:14:13.930210 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_id/delete.pyi
+-rw-r--r--   0        0        0    14786 2023-03-13 20:14:13.930371 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_id/get.py
+-rw-r--r--   0        0        0    14532 2023-03-13 20:14:13.930461 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_id/get.pyi
+-rw-r--r--   0        0        0    16852 2023-03-13 20:14:13.934345 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_id/put.py
+-rw-r--r--   0        0        0    16598 2023-03-13 20:14:13.937587 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_id/put.pyi
+-rw-r--r--   0        0        0      359 2023-03-13 19:46:28.000000 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_inventory_equipment_usage/__init__.py
+-rw-r--r--   0        0        0    10820 2023-03-13 20:14:13.937676 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_inventory_equipment_usage/get.py
+-rw-r--r--   0        0        0    10566 2023-03-13 20:14:13.937826 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_inventory_equipment_usage/get.pyi
+-rw-r--r--   0        0        0      347 2023-03-13 19:46:28.000000 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_inventory_movements/__init__.py
+-rw-r--r--   0        0        0    12924 2023-03-13 20:14:13.938652 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_inventory_movements/get.py
+-rw-r--r--   0        0        0    12670 2023-03-13 20:14:13.938754 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_inventory_movements/get.pyi
+-rw-r--r--   0        0        0      321 2023-03-13 19:46:32.000000 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_search/__init__.py
+-rw-r--r--   0        0        0    14805 2023-03-13 20:14:13.938886 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_search/get.py
+-rw-r--r--   0        0        0    14434 2023-03-13 20:14:13.938979 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_search/get.pyi
+-rw-r--r--   0        0        0      323 2023-03-13 19:46:30.000000 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_suggest/__init__.py
+-rw-r--r--   0        0        0    13168 2023-03-13 20:14:13.945743 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_suggest/get.py
+-rw-r--r--   0        0        0    12914 2023-03-13 20:14:13.951244 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_suggest/get.pyi
+-rw-r--r--   0        0        0      317 2023-03-13 19:46:28.000000 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_type/__init__.py
+-rw-r--r--   0        0        0    13989 2023-03-13 20:14:13.948583 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_type/get.py
+-rw-r--r--   0        0        0    13483 2023-03-13 20:14:13.949679 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_type/get.pyi
+-rw-r--r--   0        0        0    15623 2023-03-14 15:56:44.208509 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_type/patch.py
+-rw-r--r--   0        0        0    15339 2023-03-14 15:56:44.208618 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_type/patch.pyi
+-rw-r--r--   0        0        0    15072 2023-03-13 20:14:13.948029 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_type/post.py
+-rw-r--r--   0        0        0    14818 2023-03-13 20:14:13.956046 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_type/post.pyi
+-rw-r--r--   0        0        0      323 2023-03-13 19:46:28.000000 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_type_id/__init__.py
+-rw-r--r--   0        0        0    12655 2023-03-13 20:14:13.956883 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_type_id/get.py
+-rw-r--r--   0        0        0    12401 2023-03-13 20:14:13.957557 albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_type_id/get.pyi
+-rw-r--r--   0        0        0    10554 2023-03-14 15:56:44.208723 albert_toolkit-0.1.1/src/albert/api/rest.py
+-rw-r--r--   0        0        0    97658 2023-03-14 15:56:44.208827 albert_toolkit-0.1.1/src/albert/api/schemas.py
+-rw-r--r--   0        0        0       24 2023-03-21 21:10:12.016256 albert_toolkit-0.1.1/src/albert/binassign/__init__.py
+-rw-r--r--   0        0        0     6864 2023-04-07 17:39:15.280277 albert_toolkit-0.1.1/src/albert/binassign/binassign.py
+-rw-r--r--   0        0        0    23696 2023-04-07 17:39:15.290368 albert_toolkit-0.1.1/src/albert/binassign/tests/test_binassign.py
+-rw-r--r--   0        0        0       24 2023-03-21 21:10:12.017181 albert_toolkit-0.1.1/src/albert/bincreate/__init__.py
+-rw-r--r--   0        0        0     9335 2023-04-07 17:39:15.286804 albert_toolkit-0.1.1/src/albert/bincreate/bincreate.py
+-rw-r--r--   0        0        0    14049 2023-04-07 17:39:15.286958 albert_toolkit-0.1.1/src/albert/bincreate/tests/test_bincreate.py
+-rw-r--r--   0        0        0        0 2023-03-21 20:52:07.490083 albert_toolkit-0.1.1/src/albert/chem/__init__.py
+-rw-r--r--   0        0        0     2273 2023-03-25 22:48:15.154593 albert_toolkit-0.1.1/src/albert/chem/descriptors.py
+-rw-r--r--   0        0        0     3505 2023-03-21 20:52:07.492466 albert_toolkit-0.1.1/src/albert/chem/structure.py
+-rw-r--r--   0        0        0       48 2023-03-13 22:23:01.571954 albert_toolkit-0.1.1/src/albert/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:43:53.298477 albert_toolkit-0.1.1/src/albert/data/datasets/__init__.py
+-rw-r--r--   0        0        0      101 2023-04-10 15:43:53.299300 albert_toolkit-0.1.1/src/albert/data/datasets/molecular/__init__.py
+-rw-r--r--   0        0        0     4261 2023-04-10 15:43:53.299798 albert_toolkit-0.1.1/src/albert/data/datasets/molecular/atom.py
+-rw-r--r--   0        0        0     1566 2023-04-10 15:43:53.299872 albert_toolkit-0.1.1/src/albert/data/datasets/molecular/bond.py
+-rw-r--r--   0        0        0    17402 2023-04-10 15:43:53.300034 albert_toolkit-0.1.1/src/albert/data/datasets/molecular/graph.py
+-rw-r--r--   0        0        0     4773 2023-04-10 15:43:53.300168 albert_toolkit-0.1.1/src/albert/data/datasets/molecular/tests/test_atomic_attributes.py
+-rw-r--r--   0        0        0      197 2023-04-10 15:43:53.300297 albert_toolkit-0.1.1/src/albert/data/datasets/molecular/utils.py
+-rw-r--r--   0        0        0       29 2023-03-21 20:46:05.409720 albert_toolkit-0.1.1/src/albert/data/pipelines/__init__.py
+-rw-r--r--   0        0        0     7123 2023-03-21 20:46:05.408976 albert_toolkit-0.1.1/src/albert/data/pipelines/property_data.py
+-rw-r--r--   0        0        0       23 2023-03-13 22:15:40.430303 albert_toolkit-0.1.1/src/albert/data/reports/__init__.py
+-rw-r--r--   0        0        0     6760 2023-03-21 20:46:05.409093 albert_toolkit-0.1.1/src/albert/data/reports/reports.py
+-rw-r--r--   0        0        0     1319 2023-03-21 20:46:05.410994 albert_toolkit-0.1.1/src/albert/data/reports/tests/test_reports.py
+-rw-r--r--   0        0        0        0 2023-02-24 19:24:57.946228 albert_toolkit-0.1.1/src/albert/data/warehouse/__init__.py
+-rw-r--r--   0        0        0     3099 2023-04-10 15:43:53.301454 albert_toolkit-0.1.1/src/albert/data/warehouse/dbsession.py
+-rw-r--r--   0        0        0    57407 2023-03-21 20:52:07.492563 albert_toolkit-0.1.1/src/albert/data/warehouse/dbwarehouse_schema.py
+-rw-r--r--   0        0        0    10197 2023-04-10 15:44:55.181618 albert_toolkit-0.1.1/src/albert/data/warehouse/queries.py
+-rw-r--r--   0        0        0       29 2023-03-21 21:10:12.016726 albert_toolkit-0.1.1/src/albert/data_cleaning/__init__.py
+-rw-r--r--   0        0        0    17510 2023-04-07 17:39:15.287031 albert_toolkit-0.1.1/src/albert/data_cleaning/data_cleaning.py
+-rw-r--r--   0        0        0    10268 2023-03-27 15:12:52.337618 albert_toolkit-0.1.1/src/albert/data_cleaning/tests/test_data_cleaning.py
+-rw-r--r--   0        0        0       88 2023-03-14 15:56:44.215223 albert_toolkit-0.1.1/src/albert/filters/__init__.py
+-rw-r--r--   0        0        0     2039 2023-03-14 15:56:44.215435 albert_toolkit-0.1.1/src/albert/filters/base.py
+-rw-r--r--   0        0        0     1395 2023-03-14 15:56:44.216000 albert_toolkit-0.1.1/src/albert/filters/prediction_filters.py
+-rw-r--r--   0        0        0     2816 2023-03-14 15:56:44.215546 albert_toolkit-0.1.1/src/albert/filters/report_filters.py
+-rw-r--r--   0        0        0     1100 2023-03-14 15:56:44.215641 albert_toolkit-0.1.1/src/albert/filters/tests/test_prediction_filter.py
+-rw-r--r--   0        0        0     2731 2023-03-13 20:14:31.499968 albert_toolkit-0.1.1/src/albert/filters/tests/test_report_filter.py
+-rw-r--r--   0        0        0       21 2023-03-21 21:10:12.018359 albert_toolkit-0.1.1/src/albert/internal/__init__.py
+-rw-r--r--   0        0        0     1678 2023-03-14 15:56:44.215796 albert_toolkit-0.1.1/src/albert/internal/dynamo.py
+-rw-r--r--   0        0        0       21 2023-03-14 15:56:44.218878 albert_toolkit-0.1.1/src/albert/internal/utils/__init__.py
+-rw-r--r--   0        0        0     3370 2023-03-27 15:12:52.338256 albert_toolkit-0.1.1/src/albert/internal/utils/utils.py
+-rw-r--r--   0        0        0       33 2023-04-10 15:43:53.301760 albert_toolkit-0.1.1/src/albert/losses/__init__.py
+-rw-r--r--   0        0        0       43 2023-04-10 15:43:53.301282 albert_toolkit-0.1.1/src/albert/losses/molecular/__init__.py
+-rw-r--r--   0        0        0     2544 2023-04-10 15:43:53.301655 albert_toolkit-0.1.1/src/albert/losses/molecular/ntxentloss.py
+-rw-r--r--   0        0        0        0 2023-03-21 20:52:07.498571 albert_toolkit-0.1.1/src/albert/metrics/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-21 21:10:12.018412 albert_toolkit-0.1.1/src/albert/mlops/__init__.py
+-rw-r--r--   0        0        0     2066 2023-03-21 21:10:12.018571 albert_toolkit-0.1.1/src/albert/mlops/clearml.py
+-rw-r--r--   0        0        0        0 2023-01-24 13:57:52.836583 albert_toolkit-0.1.1/src/albert/models/__init__.py
+-rw-r--r--   0        0        0       43 2023-03-13 20:14:44.533959 albert_toolkit-0.1.1/src/albert/models/gp/__init__.py
+-rw-r--r--   0        0        0     1671 2023-03-13 20:14:44.538923 albert_toolkit-0.1.1/src/albert/models/gp/exact_gps.py
+-rw-r--r--   0        0        0     2953 2023-03-13 20:14:44.543696 albert_toolkit-0.1.1/src/albert/models/gp/tests/test_exact_gps.py
+-rw-r--r--   0        0        0        0 2023-01-24 13:57:52.837205 albert_toolkit-0.1.1/src/albert/models/nn/__init__.py
+-rw-r--r--   0        0        0       46 2023-04-03 18:50:19.466835 albert_toolkit-0.1.1/src/albert/models/nn/embedding/__init__.py
+-rw-r--r--   0        0        0     6230 2023-04-10 15:43:53.302625 albert_toolkit-0.1.1/src/albert/models/nn/embedding/gin.py
+-rw-r--r--   0        0        0     2918 2023-01-24 13:57:52.837855 albert_toolkit-0.1.1/src/albert/models/nn/embedding/mlp.py
+-rw-r--r--   0        0        0     3557 2023-01-24 13:57:52.838210 albert_toolkit-0.1.1/src/albert/models/nn/embedding/tests/test_mlp.py
+-rw-r--r--   0        0        0        0 2023-01-24 13:57:52.838264 albert_toolkit-0.1.1/src/albert/nlp/__init__.py
+-rw-r--r--   0        0        0       55 2023-01-24 13:57:52.838484 albert_toolkit-0.1.1/src/albert/nlp/utils/__init__.py
+-rw-r--r--   0        0        0      484 2023-03-13 20:14:47.619604 albert_toolkit-0.1.1/src/albert/nlp/utils/edit.py
+-rw-r--r--   0        0        0      493 2023-03-13 20:14:47.621546 albert_toolkit-0.1.1/src/albert/nlp/utils/tests/test_ldistance.py
+-rw-r--r--   0        0        0       31 2023-02-24 19:24:57.947919 albert_toolkit-0.1.1/src/albert/pipeline/__init__.py
+-rw-r--r--   0        0        0     2050 2023-03-14 15:56:44.227623 albert_toolkit-0.1.1/src/albert/pipeline/albert_pipeline.py
+-rw-r--r--   0        0        0     6334 2023-03-21 20:46:05.413649 albert_toolkit-0.1.1/src/albert/pipeline/tests/test_pipeline.py
+-rw-r--r--   0        0        0        0 2023-01-24 13:57:52.839109 albert_toolkit-0.1.1/src/albert/predictors/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-21 21:10:12.018729 albert_toolkit-0.1.1/src/albert/resources/__init__.py
+-rw-r--r--   0        0        0     4423 2023-03-21 21:10:12.019637 albert_toolkit-0.1.1/src/albert/resources/constants_en.txt
+-rw-r--r--   0        0        0     9437 2023-03-21 21:10:12.019703 albert_toolkit-0.1.1/src/albert/resources/replace_rules.xlsx
+-rw-r--r--   0        0        0    30373 2023-04-07 17:39:15.287090 albert_toolkit-0.1.1/src/albert/resources/unit_registry_custom.txt
+-rw-r--r--   0        0        0       34 2023-01-26 22:14:09.774088 albert_toolkit-0.1.1/src/albert/session/__init__.py
+-rw-r--r--   0        0        0     6620 2023-04-10 15:43:53.303824 albert_toolkit-0.1.1/src/albert/session/session.py
+-rw-r--r--   0        0        0     1944 2023-02-24 19:24:57.948551 albert_toolkit-0.1.1/src/albert/session/token_manager.py
+-rw-r--r--   0        0        0      169 2023-03-21 20:46:05.415645 albert_toolkit-0.1.1/src/albert/transforms/__init__.py
+-rw-r--r--   0        0        0      415 2023-04-10 15:44:55.181803 albert_toolkit-0.1.1/src/albert/transforms/clustering_transforms.py
+-rw-r--r--   0        0        0    17758 2023-03-21 20:46:05.416202 albert_toolkit-0.1.1/src/albert/transforms/dataframe_transforms.py
+-rw-r--r--   0        0        0    11208 2023-03-23 15:19:49.329501 albert_toolkit-0.1.1/src/albert/transforms/formulation_transforms.py
+-rw-r--r--   0        0        0      536 2023-04-10 15:44:55.181714 albert_toolkit-0.1.1/src/albert/transforms/molecular_transforms.py
+-rw-r--r--   0        0        0     5921 2023-03-21 20:46:05.417113 albert_toolkit-0.1.1/src/albert/transforms/operating_condition_transforms.py
+-rw-r--r--   0        0        0     2112 2023-03-21 20:46:05.417028 albert_toolkit-0.1.1/src/albert/transforms/property_transforms.py
+-rw-r--r--   0        0        0     2385 2023-03-21 20:46:05.417809 albert_toolkit-0.1.1/src/albert/transforms/report_gather.py
+-rw-r--r--   0        0        0     2039 2023-03-21 20:46:05.419237 albert_toolkit-0.1.1/src/albert/transforms/tests/test_dataframe_transforms.py
+-rw-r--r--   0        0        0      270 2023-03-21 20:46:05.419868 albert_toolkit-0.1.1/src/albert/transforms/tests/test_formulation_pivot.py
+-rw-r--r--   0        0        0     4016 2023-03-21 20:46:05.421066 albert_toolkit-0.1.1/src/albert/transforms/tests/test_report_gather.py
+-rw-r--r--   0        0        0     1529 2023-03-21 20:46:05.420678 albert_toolkit-0.1.1/src/albert/transforms/tests/test_util_transforms.py
+-rw-r--r--   0        0        0     7051 2023-03-21 20:46:05.420555 albert_toolkit-0.1.1/src/albert/transforms/util_transforms.py
+-rw-r--r--   0        0        0       27 2023-03-21 21:10:12.019755 albert_toolkit-0.1.1/src/albert/unitconversion/__init__.py
+-rw-r--r--   0        0        0    23589 2023-04-07 17:39:15.289569 albert_toolkit-0.1.1/src/albert/unitconversion/tests/test_unit_convert.py
+-rw-r--r--   0        0        0    10123 2023-04-07 17:39:15.286892 albert_toolkit-0.1.1/src/albert/unitconversion/unit_convert.py
+-rw-r--r--   0        0        0       20 2023-03-21 21:10:12.020663 albert_toolkit-0.1.1/src/albert/utils/__init__.py
+-rw-r--r--   0        0        0     1280 2023-03-27 15:13:02.180149 albert_toolkit-0.1.1/src/albert/utils/utils.py
+-rw-r--r--   0        0        0       21 2023-02-24 19:24:57.949823 albert_toolkit-0.1.1/src/albert/version.py
+-rw-r--r--   0        0        0        0 2023-01-24 13:57:52.839885 albert_toolkit-0.1.1/src/albert/viz/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-24 13:57:52.839968 albert_toolkit-0.1.1/src/albert/viz/plots.py
+-rw-r--r--   0        0        0     4663 2023-03-21 20:46:05.422241 albert_toolkit-0.1.1/src/albert/viz/umap_visualization.py
+-rw-r--r--   0        0        0     1074 2023-03-21 20:46:05.422938 albert_toolkit-0.1.1/src/albert/viz/utils/dimension_reduction.py
+-rw-r--r--   0        0        0     8034 1970-01-01 00:00:00.000000 albert_toolkit-0.1.1/PKG-INFO
```

### Comparing `albert_toolkit-0.1.0/README.md` & `albert_toolkit-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 
 # Non-Python Dependencies
 
 ## Docker
 If you want to use the docker image for doing development you will need to install the docker runtime (or docker desktop for windows/macos). If you are going to be running the docker image on an ubuntu system with a GPU you will need to additionally install the nvidia docker runtime -- instructions for which can be found at https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html
 
 # Getting Started
-After installing the albert-ds package, you can setup your environment configuration by running the command `albert init` and following the prompts. Any credentials that you do not have (e.g. if you do not have data warehouse credentials) you can simply leave them blank. 
+After installing the albert-toolkit package, you can setup your environment configuration by running the command `albert init` and following the prompts. Any credentials that you do not have (e.g. if you do not have data warehouse credentials) you can simply leave them blank. 
 
-If you will be using clearML integrations then be sure to have your clearml pip install command ready as you will be prompted for it as part of the init process. If you have already setup clearml in your virtual environment prior to installing albert-ds then you can simply answer no to the prompt and it will leave your current configuration untouched.
+If you will be using clearML integrations then be sure to have your clearml pip install command ready as you will be prompted for it as part of the init process. If you have already setup clearml in your virtual environment prior to installing albert-toolkit then you can simply answer no to the prompt and it will leave your current configuration untouched.
 
 # Running Unit Tests
-NOTE: All the following commands should be run from within a virtual environment.
+NOTE: All the following commands should be run from within a virtual environment. And they will all require that your albert API token is setup correctly
 
-albert-ds utilizes pytest as its testing framework -- to run the full suite of unit tests use the helper script and the `ta` command:
+albert-toolkit utilizes pytest as its testing framework -- to run the full suite of unit tests use the helper script and the `ta` command:
 ```bash
 $ ./al.sh ta
 ```
 
 Alternatively if you want to run the tests in a fresh venv (i.e. test the build/install/unit test workflow) run the command `tb` -- This is useful for checking that you have correctly supplied all dependencies in the package setup.cfg. 
 
 ```bash
@@ -30,60 +30,51 @@
 ```
 Note that running the above command will look for lib-jwt-python at the relative path `../lib-jwt-python` if it is not located there it will attempt to clone the repo using ssh and will fail if you don't have your github ssh keys setup correct. 
 
 # Package Installation 
 Until we get a pypi package setup you will need to clone this repository and perform a pip install locally.
 
 ## Choosing an Install Environment
-Depending on the application you may not need or want the full development stack associated with this library. You can therefore install different dependencies using the square bracket syntax e.g. `albert-ds[viz]` if you only want to install a certain set of dependencies. This is particularly useful if you are building out an application or microservice which only depends upon a subset of the full albert-ds library, and you do not want to install unused dependencies. 
+Depending on the application you may not need or want the full development stack associated with this library. You can therefore install different dependencies using the square bracket syntax e.g. `albert-toolkit[viz]` if you only want to install a certain set of dependencies. This is particularly useful if you are building out an application or microservice which only depends upon a subset of the full albert-toolkit library, and you do not want to install unused dependencies. 
 
-If you specify no environment tag then you will just the get base code for albert-ds installed into your environment and most of it will not function without the required dependencies -- so be sure to choose one of the following stacks when installing the library. 
+If you specify no environment tag then you will just the get base code for albert-toolkit installed into your environment and most of it will not function without the required dependencies -- so be sure to choose one of the following stacks when installing the library. 
 
-Note the use of quotes in the package install commands below e.g. `"albert-ds[dev]"` -- the quotes are required and you will get an error if you forget to include them.
+Note the use of quotes in the package install commands below e.g. `"albert-toolkit[dev]"` -- the quotes are required and you will get an error if you forget to include them.
 
 ## Full Development Stack
 The full development stack can be installed using the `[dev]` or `[all]` tags. The development environment contains support for juptyerlab and all the associated ipython dependencies. It should not be installed in a deployed application
 ```bash
-$ git clone git@github.com:MoleculeEngineering/albert-ds.git
-$ pip install "albert-ds[torch]" # This needs to be run first for the [chem] dependency to work properly
-$ pip install "albert-ds[dev]" #This should be run from within your python virtual environment
+$ pip install "albert-toolkit[dev]"  #This should be run from within your python virtual environment
 ```
 
 
 ## Visualization Stack
-The visualization stack includes only those dependencies which are needed to utilize the visualization components of the albert-ds library. It can be installed with the `[viz]` tag
+The visualization stack includes only those dependencies which are needed to utilize the visualization components of the albert-toolkit library. It can be installed with the `[viz]` tag
 ```bash
-$ git clone git@github.com:MoleculeEngineering/albert-ds.git
-$ pip install "albert-ds[viz]" #This should be run from within your python virtual environment
+$ pip install "albert-toolkit[viz]" #This should be run from within your python virtual environment
 ```
 
 ## Metrics Stack
 The metrics stack includes only those depenencies which are necessary to compute metrics (for example: if you have a microservice architecture and you are running lots of predictions and storing those in a database, you may want to have a microservice which is dedicated to computing performance/accuracy/etc... metrics and hence that service should not require any of the other stacks)
 ```bash
-$ git clone git@github.com:MoleculeEngineering/albert-ds.git
-$ pip install "albert-ds[metrics]" #This should be run from within your python virtual environment
+$ pip install "albert-toolkit[metrics]" #This should be run from within your python virtual environment
 ```
 
 ## NLP Stack
 The NLP Stack includes only those dependencies which are necessary to compute NLP transforms or embeddings, including helper functions for transforming or analyzing text data
 ```bash
-$ git clone git@github.com:MoleculeEngineering/albert-ds.git
-$ pip install "albert-ds[nlp]" #This should be run from within your python virtual environment
+$ pip install "albert-toolkit[nlp]" #This should be run from within your python virtual environment
 ```
 
 ## Models Stack
 The models stack includes all the dependencies necessary to build or run models. Installing the Models stack will also install the metrics stack
 ```bash
-$ git clone git@github.com:MoleculeEngineering/albert-ds.git
-$ pip install "albert-ds[models]" #This should be run from within your python virtual environment
+$ pip install "albert-toolkit[models]" #This should be run from within your python virtual environment
 ```
 
 ## Chemistry Stack
-The chemistry stacks includes all the dependencies needed to run the chemistry modeuls. 
+The chemistry stacks includes all the dependencies needed to run the chemistry modules -- the proper way to install the chemistry stack is throught he use of the `albert` cli tool. Simply run the following to install the chemistry dependencies after installing the main albert toolkit
 ```bash
-$ git clone git@github.com:MoleculeEngineering/albert-ds.git
-$ pip install "albert-ds[torch]" #This needs to happen first for the [chem] install to work correctly
-$ pip install "albert-ds[chem]" 
-
-# Using the Helper Script
-Included in the repository is a helper script `al.sh` which contains a few simple helper scripts for building, publishing, etc... 
-TODO: Include documentation here on the use of the helper script to build and publish the package to pypi.
+$ albert init-chem
+```
+This will require `cmake` and CUDA to be installed. 
+
```

### Comparing `albert_toolkit-0.1.0/pyproject.toml` & `albert_toolkit-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "albert-toolkit"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python toolkit for Albert Invent"
 authors = ["Jonathan Welch <Jonathan@albertinvent.com>"]
 license = "MIT"
 readme = "README.md"
 include = ["pyproject.toml"]
 packages = [{ include = "albert", from = "src" }]
```

### Comparing `albert_toolkit-0.1.0/src/albert/albert.py` & `albert_toolkit-0.1.1/src/albert/albert.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/__init__.py` & `albert_toolkit-0.1.1/src/albert/api/__init__.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/api_client.py` & `albert_toolkit-0.1.1/src/albert/api/api_client.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/path_to_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tag_to_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tags/__init__.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tags/analytics_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tags/analytics_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tags/columns_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tags/columns_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tags/default_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tags/default_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tags/health_check_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tags/health_check_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tags/internal_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tags/internal_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tags/inventory_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tags/inventory_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tags/locations_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tags/locations_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tags/prediction_flow_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tags/prediction_flow_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tags/prediction_models_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tags/prediction_models_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tags/predictions_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tags/predictions_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tags/product_design_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tags/product_design_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tags/reports_catalogue_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tags/reports_catalogue_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tags/reports_sp_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tags/reports_sp_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tags/rows_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tags/rows_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tags/search_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tags/search_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tags/unpack_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tags/unpack_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tags/user_reports_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tags/user_reports_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/apis/tags/values_api.py` & `albert_toolkit-0.1.1/src/albert/api/apis/tags/values_api.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/configuration.py` & `albert_toolkit-0.1.1/src/albert/api/configuration.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/exceptions.py` & `albert_toolkit-0.1.1/src/albert/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/add.py` & `albert_toolkit-0.1.1/src/albert/api/model/add.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/add.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/add.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/cas.py` & `albert_toolkit-0.1.1/src/albert/api/model/cas.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/cas.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/cas.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/column_copy_to_existing.py` & `albert_toolkit-0.1.1/src/albert/api/model/column_copy_to_existing.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/column_copy_to_existing.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/column_copy_to_existing.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/column_copy_to_new.py` & `albert_toolkit-0.1.1/src/albert/api/model/column_copy_to_new.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/column_copy_to_new.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/column_copy_to_new.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/columns.py` & `albert_toolkit-0.1.1/src/albert/api/model/columns.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/columns.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/columns.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/component_input.py` & `albert_toolkit-0.1.1/src/albert/api/model/component_input.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/component_input.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/component_input.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/copy_report.py` & `albert_toolkit-0.1.1/src/albert/api/model/copy_report.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/copy_report.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/copy_report.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/data_model.py` & `albert_toolkit-0.1.1/src/albert/api/model/data_model.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/data_model.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/data_model.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/default_columns.py` & `albert_toolkit-0.1.1/src/albert/api/model/default_columns.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/default_columns.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/default_columns.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/delete.py` & `albert_toolkit-0.1.1/src/albert/api/model/delete.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/delete.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/delete.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/denormalized_inventories.py` & `albert_toolkit-0.1.1/src/albert/api/model/denormalized_inventories.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/denormalized_inventories.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/denormalized_inventories.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/denormalized_inventory.py` & `albert_toolkit-0.1.1/src/albert/api/model/denormalized_inventory.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/denormalized_inventory.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/denormalized_inventory.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/designs.py` & `albert_toolkit-0.1.1/src/albert/api/model/designs.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/designs.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/designs.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/entity_tags.py` & `albert_toolkit-0.1.1/src/albert/api/model/entity_tags.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/entity_tags.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/entity_tags.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/equipment.py` & `albert_toolkit-0.1.1/src/albert/api/model/equipment.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/equipment.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/equipment.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/error.py` & `albert_toolkit-0.1.1/src/albert/api/model/error.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/error.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/error.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/facet_with_value_array.py` & `albert_toolkit-0.1.1/src/albert/api/model/facet_with_value_array.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/facet_with_value_array.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/facet_with_value_array.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/formula_item.py` & `albert_toolkit-0.1.1/src/albert/api/model/formula_item.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/formula_item.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/formula_item.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/get_back_update_companies.py` & `albert_toolkit-0.1.1/src/albert/api/model/get_back_update_companies.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/get_back_update_companies.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/get_back_update_companies.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/grid.py` & `albert_toolkit-0.1.1/src/albert/api/model/grid.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/grid.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/grid.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/health.py` & `albert_toolkit-0.1.1/src/albert/api/model/health.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/health.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/health.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/inputs.py` & `albert_toolkit-0.1.1/src/albert/api/model/inputs.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/inputs.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/inputs.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/inventories.py` & `albert_toolkit-0.1.1/src/albert/api/model/inventories.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/inventories.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/inventories.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/inventory.py` & `albert_toolkit-0.1.1/src/albert/api/model/inventory.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/inventory.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/inventory.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/location.py` & `albert_toolkit-0.1.1/src/albert/api/model/location.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/location.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/location.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/locations.py` & `albert_toolkit-0.1.1/src/albert/api/model/locations.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/locations.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/locations.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/merged_dac.py` & `albert_toolkit-0.1.1/src/albert/api/model/merged_dac.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/merged_dac.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/merged_dac.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/merged_dat.py` & `albert_toolkit-0.1.1/src/albert/api/model/merged_dat.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/merged_dat.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/merged_dat.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/merged_inventory.py` & `albert_toolkit-0.1.1/src/albert/api/model/merged_inventory.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/merged_inventory.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/merged_inventory.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/minimum.py` & `albert_toolkit-0.1.1/src/albert/api/model/minimum.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/minimum.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/minimum.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/model_patch.py` & `albert_toolkit-0.1.1/src/albert/api/model/model_patch.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/model_patch.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/model_patch.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/model_prediction.py` & `albert_toolkit-0.1.1/src/albert/api/model/model_prediction.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/model_prediction.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/model_prediction.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/model_predictions.py` & `albert_toolkit-0.1.1/src/albert/api/model/model_predictions.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/model_predictions.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/model_predictions.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/model_predictions_values_only.py` & `albert_toolkit-0.1.1/src/albert/api/model/model_predictions_values_only.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/model_predictions_values_only.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/model_predictions_values_only.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/new_model_version.py` & `albert_toolkit-0.1.1/src/albert/api/model/new_model_version.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/new_model_version.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/new_model_version.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/output.py` & `albert_toolkit-0.1.1/src/albert/api/model/output.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/output.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/output.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/parameter.py` & `albert_toolkit-0.1.1/src/albert/api/model/parameter.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/parameter.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/parameter.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/partial_product_design.py` & `albert_toolkit-0.1.1/src/albert/api/model/partial_product_design.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/partial_product_design.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/partial_product_design.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/partial_success.py` & `albert_toolkit-0.1.1/src/albert/api/model/partial_success.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/partial_success.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/partial_success.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/partial_success1.py` & `albert_toolkit-0.1.1/src/albert/api/model/partial_success1.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/partial_success1.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/partial_success1.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/partial_success_post.py` & `albert_toolkit-0.1.1/src/albert/api/model/partial_success_post.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/partial_success_post.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/partial_success_post.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/patch.py` & `albert_toolkit-0.1.1/src/albert/api/model/patch.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/patch.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/patch.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/patch1.py` & `albert_toolkit-0.1.1/src/albert/api/model/patch1.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/patch1.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/patch1.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/patch_blk.py` & `albert_toolkit-0.1.1/src/albert/api/model/patch_blk.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/patch_blk.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/patch_blk.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/patch_inventory.py` & `albert_toolkit-0.1.1/src/albert/api/model/patch_inventory.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/patch_inventory.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/patch_inventory.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/patch_prediction.py` & `albert_toolkit-0.1.1/src/albert/api/model/patch_prediction.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/patch_prediction.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/patch_prediction.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/patch_type.py` & `albert_toolkit-0.1.1/src/albert/api/model/patch_type.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/patch_type.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/patch_type.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/patch_types.py` & `albert_toolkit-0.1.1/src/albert/api/model/patch_types.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/patch_types.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/patch_types.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/pd_row.py` & `albert_toolkit-0.1.1/src/albert/api/model/pd_row.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/pd_row.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/pd_row.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/pd_rows.py` & `albert_toolkit-0.1.1/src/albert/api/model/pd_rows.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/pd_rows.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/pd_rows.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/post_partial_success.py` & `albert_toolkit-0.1.1/src/albert/api/model/post_partial_success.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/post_partial_success.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/post_partial_success.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/post_pd_rows.py` & `albert_toolkit-0.1.1/src/albert/api/model/post_pd_rows.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/post_pd_rows.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/post_pd_rows.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/post_prediction_partial_success.py` & `albert_toolkit-0.1.1/src/albert/api/model/post_prediction_partial_success.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/post_prediction_partial_success.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/post_prediction_partial_success.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/post_to_scheduler_success.py` & `albert_toolkit-0.1.1/src/albert/api/model/post_to_scheduler_success.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/post_to_scheduler_success.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/post_to_scheduler_success.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/prediction_data_model.py` & `albert_toolkit-0.1.1/src/albert/api/model/prediction_data_model.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/prediction_data_model.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/prediction_data_model.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/prediction_data_model_success.py` & `albert_toolkit-0.1.1/src/albert/api/model/prediction_data_model_success.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/prediction_data_model_success.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/prediction_data_model_success.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/prediction_model.py` & `albert_toolkit-0.1.1/src/albert/api/model/prediction_model.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/prediction_model.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/prediction_model.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/prediction_model_versions.py` & `albert_toolkit-0.1.1/src/albert/api/model/prediction_model_versions.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/prediction_model_versions.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/prediction_model_versions.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/prediction_models.py` & `albert_toolkit-0.1.1/src/albert/api/model/prediction_models.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/prediction_models.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/prediction_models.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/product_design.py` & `albert_toolkit-0.1.1/src/albert/api/model/product_design.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/product_design.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/product_design.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/product_design_search_result.py` & `albert_toolkit-0.1.1/src/albert/api/model/product_design_search_result.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/product_design_search_result.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/product_design_search_result.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/product_design_suggest_result.py` & `albert_toolkit-0.1.1/src/albert/api/model/product_design_suggest_result.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/product_design_suggest_result.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/product_design_suggest_result.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/product_designs.py` & `albert_toolkit-0.1.1/src/albert/api/model/product_designs.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/product_designs.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/product_designs.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/property_task_data_model.py` & `albert_toolkit-0.1.1/src/albert/api/model/property_task_data_model.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/property_task_data_model.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/property_task_data_model.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/put_back_update_companies.py` & `albert_toolkit-0.1.1/src/albert/api/model/put_back_update_companies.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/put_back_update_companies.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/put_back_update_companies.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/put_report.py` & `albert_toolkit-0.1.1/src/albert/api/model/put_report.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/put_report.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/put_report.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/report.py` & `albert_toolkit-0.1.1/src/albert/api/model/report.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/report.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/report.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/report_list.py` & `albert_toolkit-0.1.1/src/albert/api/model/report_list.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/report_list.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/report_list.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/report_search_result.py` & `albert_toolkit-0.1.1/src/albert/api/model/report_search_result.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/report_search_result.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/report_search_result.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/report_suggest_result.py` & `albert_toolkit-0.1.1/src/albert/api/model/report_suggest_result.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/report_suggest_result.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/report_suggest_result.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/report_type.py` & `albert_toolkit-0.1.1/src/albert/api/model/report_type.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/report_type.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/report_type.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/report_type_list.py` & `albert_toolkit-0.1.1/src/albert/api/model/report_type_list.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/report_type_list.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/report_type_list.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/task_workflow.py` & `albert_toolkit-0.1.1/src/albert/api/model/task_workflow.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/task_workflow.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/task_workflow.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/unpack.py` & `albert_toolkit-0.1.1/src/albert/api/model/unpack.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/unpack.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/unpack.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/update.py` & `albert_toolkit-0.1.1/src/albert/api/model/update.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/update.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/update.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/values.py` & `albert_toolkit-0.1.1/src/albert/api/model/values.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/values.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/values.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/wf_all_accepted.py` & `albert_toolkit-0.1.1/src/albert/api/model/wf_all_accepted.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/wf_all_accepted.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/wf_all_accepted.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/wf_partial_success.py` & `albert_toolkit-0.1.1/src/albert/api/model/wf_partial_success.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/model/wf_partial_success.pyi` & `albert_toolkit-0.1.1/src/albert/api/model/wf_partial_success.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/models/__init__.py` & `albert_toolkit-0.1.1/src/albert/api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/__init__.py` & `albert_toolkit-0.1.1/src/albert/api/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories/post.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories/post.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories/post.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories/post.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories_health/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories_health/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories_health/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories_health/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories_id/delete.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories_id/delete.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories_id/delete.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories_id/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories_id/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories_id/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories_id/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories_id/patch.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories_id/patch.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_inventories_id/patch.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_inventories_id/patch.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations/post.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations/post.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations/post.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations/post.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_async_id/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_async_id/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_async_id/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_async_id/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_async_id/put.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_async_id/put.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_async_id/put.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_async_id/put.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_health/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_health/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_health/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_health/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_id/delete.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_id/delete.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_id/delete.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_id/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_id/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_id/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_id/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_id/patch.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_id/patch.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_locations_id/patch.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_locations_id/patch.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions/post.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions/post.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions/post.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions/post.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_health/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_health/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_health/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_health/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_mergedac/post.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_mergedac/post.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_mergedac/post.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_mergedac/post.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_mergedat/post.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_mergedat/post.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_mergedat/post.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_mergedat/post.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models/post.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models/post.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models/post.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models/post.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_id/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_id/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_id/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_id/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_parent_id_version/delete.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_parent_id_version/delete.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_parent_id_version/delete.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_parent_id_version/delete.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_parent_id_version/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_parent_id_version/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_parent_id_version/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_parent_id_version/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_parent_id_version/patch.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_parent_id_version/patch.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_parent_id_version/patch.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_parent_id_version/patch.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_parent_id_version_id/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_parent_id_version_id/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_models_parent_id_version_id/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_models_parent_id_version_id/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_parent_id/patch.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_parent_id/patch.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_parent_id/patch.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_parent_id/patch.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_tasks/post.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_tasks/post.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_predictions_tasks/post.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_predictions_tasks/post.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign/post.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign/post.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign/post.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign/post.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_health/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_health/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_health/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_health/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_designs/delete.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_designs/delete.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_designs/delete.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_designs/delete.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_designs/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_designs/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_designs/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_designs/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_designs/patch.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_designs/patch.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_designs/patch.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_designs/patch.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_designs/post.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_designs/post.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_designs/post.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_designs/post.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_grid/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_grid/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_grid/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_grid/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_products/post.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_products/post.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_products/post.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_products/post.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_unpack/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_unpack/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_unpack/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_unpack/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_values/patch.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_values/patch.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_id_values/patch.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_id_values/patch.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_inventories_id/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_inventories_id/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_inventories_id/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_inventories_id/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_inventories_id/put.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_inventories_id/put.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_inventories_id/put.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_inventories_id/put.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_mergeinventory/post.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_mergeinventory/post.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_mergeinventory/post.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_mergeinventory/post.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_search/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_search/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_search/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_search/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_suggest/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_suggest/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_productdesign_suggest/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_productdesign_suggest/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports/post.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports/post.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports/post.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports/post.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_analytics_id/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_analytics_id/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_analytics_id/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_analytics_id/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_copy/post.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_copy/post.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_copy/post.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_copy/post.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_datascience_id/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_datascience_id/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_datascience_id/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_datascience_id/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_health/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_health/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_health/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_health/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_id/delete.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_id/delete.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_id/delete.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_id/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_id/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_id/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_id/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_id/put.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_id/put.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_id/put.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_id/put.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_inventory_equipment_usage/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_inventory_equipment_usage/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_inventory_equipment_usage/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_inventory_equipment_usage/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_inventory_movements/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_inventory_movements/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_inventory_movements/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_inventory_movements/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_search/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_search/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_search/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_search/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_suggest/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_suggest/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_suggest/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_suggest/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_type/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_type/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_type/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_type/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_type/patch.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_type/patch.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_type/patch.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_type/patch.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_type/post.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_type/post.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_type/post.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_type/post.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_type_id/get.py` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_type_id/get.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/paths/api_v3_reports_type_id/get.pyi` & `albert_toolkit-0.1.1/src/albert/api/paths/api_v3_reports_type_id/get.pyi`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/rest.py` & `albert_toolkit-0.1.1/src/albert/api/rest.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/api/schemas.py` & `albert_toolkit-0.1.1/src/albert/api/schemas.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/binassign/binassign.py` & `albert_toolkit-0.1.1/src/albert/binassign/binassign.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/binassign/tests/test_binassign.py` & `albert_toolkit-0.1.1/src/albert/binassign/tests/test_binassign.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/bincreate/bincreate.py` & `albert_toolkit-0.1.1/src/albert/bincreate/bincreate.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/bincreate/tests/test_bincreate.py` & `albert_toolkit-0.1.1/src/albert/bincreate/tests/test_bincreate.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/chem/descriptors.py` & `albert_toolkit-0.1.1/src/albert/chem/descriptors.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/chem/structure.py` & `albert_toolkit-0.1.1/src/albert/chem/structure.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/data/datasets/molecular/atom.py` & `albert_toolkit-0.1.1/src/albert/data/datasets/molecular/atom.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/data/datasets/molecular/bond.py` & `albert_toolkit-0.1.1/src/albert/data/datasets/molecular/bond.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/data/datasets/molecular/graph.py` & `albert_toolkit-0.1.1/src/albert/data/datasets/molecular/graph.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/data/datasets/molecular/tests/test_atomic_attributes.py` & `albert_toolkit-0.1.1/src/albert/data/datasets/molecular/tests/test_atomic_attributes.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/data/pipelines/property_data.py` & `albert_toolkit-0.1.1/src/albert/data/pipelines/property_data.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/data/reports/reports.py` & `albert_toolkit-0.1.1/src/albert/data/reports/reports.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/data/reports/tests/test_reports.py` & `albert_toolkit-0.1.1/src/albert/data/reports/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/data/warehouse/dbsession.py` & `albert_toolkit-0.1.1/src/albert/data/warehouse/dbsession.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/data/warehouse/dbwarehouse_schema.py` & `albert_toolkit-0.1.1/src/albert/data/warehouse/dbwarehouse_schema.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/data/warehouse/queries.py` & `albert_toolkit-0.1.1/src/albert/data/warehouse/queries.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/data_cleaning/data_cleaning.py` & `albert_toolkit-0.1.1/src/albert/data_cleaning/data_cleaning.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/data_cleaning/tests/test_data_cleaning.py` & `albert_toolkit-0.1.1/src/albert/data_cleaning/tests/test_data_cleaning.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/filters/base.py` & `albert_toolkit-0.1.1/src/albert/filters/base.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/filters/prediction_filters.py` & `albert_toolkit-0.1.1/src/albert/filters/prediction_filters.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/filters/report_filters.py` & `albert_toolkit-0.1.1/src/albert/filters/report_filters.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/filters/tests/test_prediction_filter.py` & `albert_toolkit-0.1.1/src/albert/filters/tests/test_prediction_filter.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/filters/tests/test_report_filter.py` & `albert_toolkit-0.1.1/src/albert/filters/tests/test_report_filter.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/internal/dynamo.py` & `albert_toolkit-0.1.1/src/albert/internal/dynamo.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/internal/utils/utils.py` & `albert_toolkit-0.1.1/src/albert/internal/utils/utils.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/losses/molecular/ntxentloss.py` & `albert_toolkit-0.1.1/src/albert/losses/molecular/ntxentloss.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/mlops/clearml.py` & `albert_toolkit-0.1.1/src/albert/mlops/clearml.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/models/gp/exact_gps.py` & `albert_toolkit-0.1.1/src/albert/models/gp/exact_gps.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/models/gp/tests/test_exact_gps.py` & `albert_toolkit-0.1.1/src/albert/models/gp/tests/test_exact_gps.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/models/nn/embedding/gin.py` & `albert_toolkit-0.1.1/src/albert/models/nn/embedding/gin.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/models/nn/embedding/mlp.py` & `albert_toolkit-0.1.1/src/albert/models/nn/embedding/mlp.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/models/nn/embedding/tests/test_mlp.py` & `albert_toolkit-0.1.1/src/albert/models/nn/embedding/tests/test_mlp.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/pipeline/albert_pipeline.py` & `albert_toolkit-0.1.1/src/albert/pipeline/albert_pipeline.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/pipeline/tests/test_pipeline.py` & `albert_toolkit-0.1.1/src/albert/pipeline/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/resources/constants_en.txt` & `albert_toolkit-0.1.1/src/albert/resources/constants_en.txt`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/resources/replace_rules.xlsx` & `albert_toolkit-0.1.1/src/albert/resources/replace_rules.xlsx`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/resources/unit_registry_custom.txt` & `albert_toolkit-0.1.1/src/albert/resources/unit_registry_custom.txt`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/session/session.py` & `albert_toolkit-0.1.1/src/albert/session/session.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/session/token_manager.py` & `albert_toolkit-0.1.1/src/albert/session/token_manager.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/transforms/dataframe_transforms.py` & `albert_toolkit-0.1.1/src/albert/transforms/dataframe_transforms.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/transforms/formulation_transforms.py` & `albert_toolkit-0.1.1/src/albert/transforms/formulation_transforms.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/transforms/molecular_transforms.py` & `albert_toolkit-0.1.1/src/albert/transforms/molecular_transforms.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/transforms/operating_condition_transforms.py` & `albert_toolkit-0.1.1/src/albert/transforms/operating_condition_transforms.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/transforms/property_transforms.py` & `albert_toolkit-0.1.1/src/albert/transforms/property_transforms.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/transforms/report_gather.py` & `albert_toolkit-0.1.1/src/albert/transforms/report_gather.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/transforms/tests/test_dataframe_transforms.py` & `albert_toolkit-0.1.1/src/albert/transforms/tests/test_dataframe_transforms.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/transforms/tests/test_report_gather.py` & `albert_toolkit-0.1.1/src/albert/transforms/tests/test_report_gather.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/transforms/tests/test_util_transforms.py` & `albert_toolkit-0.1.1/src/albert/transforms/tests/test_util_transforms.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/transforms/util_transforms.py` & `albert_toolkit-0.1.1/src/albert/transforms/util_transforms.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/unitconversion/tests/test_unit_convert.py` & `albert_toolkit-0.1.1/src/albert/unitconversion/tests/test_unit_convert.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/unitconversion/unit_convert.py` & `albert_toolkit-0.1.1/src/albert/unitconversion/unit_convert.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/utils/utils.py` & `albert_toolkit-0.1.1/src/albert/utils/utils.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/viz/umap_visualization.py` & `albert_toolkit-0.1.1/src/albert/viz/umap_visualization.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/src/albert/viz/utils/dimension_reduction.py` & `albert_toolkit-0.1.1/src/albert/viz/utils/dimension_reduction.py`

 * *Files identical despite different names*

### Comparing `albert_toolkit-0.1.0/PKG-INFO` & `albert_toolkit-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albert-toolkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python toolkit for Albert Invent
 License: MIT
 Author: Jonathan Welch
 Author-email: Jonathan@albertinvent.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -61,22 +61,22 @@
 
 # Non-Python Dependencies
 
 ## Docker
 If you want to use the docker image for doing development you will need to install the docker runtime (or docker desktop for windows/macos). If you are going to be running the docker image on an ubuntu system with a GPU you will need to additionally install the nvidia docker runtime -- instructions for which can be found at https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html
 
 # Getting Started
-After installing the albert-ds package, you can setup your environment configuration by running the command `albert init` and following the prompts. Any credentials that you do not have (e.g. if you do not have data warehouse credentials) you can simply leave them blank. 
+After installing the albert-toolkit package, you can setup your environment configuration by running the command `albert init` and following the prompts. Any credentials that you do not have (e.g. if you do not have data warehouse credentials) you can simply leave them blank. 
 
-If you will be using clearML integrations then be sure to have your clearml pip install command ready as you will be prompted for it as part of the init process. If you have already setup clearml in your virtual environment prior to installing albert-ds then you can simply answer no to the prompt and it will leave your current configuration untouched.
+If you will be using clearML integrations then be sure to have your clearml pip install command ready as you will be prompted for it as part of the init process. If you have already setup clearml in your virtual environment prior to installing albert-toolkit then you can simply answer no to the prompt and it will leave your current configuration untouched.
 
 # Running Unit Tests
-NOTE: All the following commands should be run from within a virtual environment.
+NOTE: All the following commands should be run from within a virtual environment. And they will all require that your albert API token is setup correctly
 
-albert-ds utilizes pytest as its testing framework -- to run the full suite of unit tests use the helper script and the `ta` command:
+albert-toolkit utilizes pytest as its testing framework -- to run the full suite of unit tests use the helper script and the `ta` command:
 ```bash
 $ ./al.sh ta
 ```
 
 Alternatively if you want to run the tests in a fresh venv (i.e. test the build/install/unit test workflow) run the command `tb` -- This is useful for checking that you have correctly supplied all dependencies in the package setup.cfg. 
 
 ```bash
@@ -84,61 +84,52 @@
 ```
 Note that running the above command will look for lib-jwt-python at the relative path `../lib-jwt-python` if it is not located there it will attempt to clone the repo using ssh and will fail if you don't have your github ssh keys setup correct. 
 
 # Package Installation 
 Until we get a pypi package setup you will need to clone this repository and perform a pip install locally.
 
 ## Choosing an Install Environment
-Depending on the application you may not need or want the full development stack associated with this library. You can therefore install different dependencies using the square bracket syntax e.g. `albert-ds[viz]` if you only want to install a certain set of dependencies. This is particularly useful if you are building out an application or microservice which only depends upon a subset of the full albert-ds library, and you do not want to install unused dependencies. 
+Depending on the application you may not need or want the full development stack associated with this library. You can therefore install different dependencies using the square bracket syntax e.g. `albert-toolkit[viz]` if you only want to install a certain set of dependencies. This is particularly useful if you are building out an application or microservice which only depends upon a subset of the full albert-toolkit library, and you do not want to install unused dependencies. 
 
-If you specify no environment tag then you will just the get base code for albert-ds installed into your environment and most of it will not function without the required dependencies -- so be sure to choose one of the following stacks when installing the library. 
+If you specify no environment tag then you will just the get base code for albert-toolkit installed into your environment and most of it will not function without the required dependencies -- so be sure to choose one of the following stacks when installing the library. 
 
-Note the use of quotes in the package install commands below e.g. `"albert-ds[dev]"` -- the quotes are required and you will get an error if you forget to include them.
+Note the use of quotes in the package install commands below e.g. `"albert-toolkit[dev]"` -- the quotes are required and you will get an error if you forget to include them.
 
 ## Full Development Stack
 The full development stack can be installed using the `[dev]` or `[all]` tags. The development environment contains support for juptyerlab and all the associated ipython dependencies. It should not be installed in a deployed application
 ```bash
-$ git clone git@github.com:MoleculeEngineering/albert-ds.git
-$ pip install "albert-ds[torch]" # This needs to be run first for the [chem] dependency to work properly
-$ pip install "albert-ds[dev]" #This should be run from within your python virtual environment
+$ pip install "albert-toolkit[dev]"  #This should be run from within your python virtual environment
 ```
 
 
 ## Visualization Stack
-The visualization stack includes only those dependencies which are needed to utilize the visualization components of the albert-ds library. It can be installed with the `[viz]` tag
+The visualization stack includes only those dependencies which are needed to utilize the visualization components of the albert-toolkit library. It can be installed with the `[viz]` tag
 ```bash
-$ git clone git@github.com:MoleculeEngineering/albert-ds.git
-$ pip install "albert-ds[viz]" #This should be run from within your python virtual environment
+$ pip install "albert-toolkit[viz]" #This should be run from within your python virtual environment
 ```
 
 ## Metrics Stack
 The metrics stack includes only those depenencies which are necessary to compute metrics (for example: if you have a microservice architecture and you are running lots of predictions and storing those in a database, you may want to have a microservice which is dedicated to computing performance/accuracy/etc... metrics and hence that service should not require any of the other stacks)
 ```bash
-$ git clone git@github.com:MoleculeEngineering/albert-ds.git
-$ pip install "albert-ds[metrics]" #This should be run from within your python virtual environment
+$ pip install "albert-toolkit[metrics]" #This should be run from within your python virtual environment
 ```
 
 ## NLP Stack
 The NLP Stack includes only those dependencies which are necessary to compute NLP transforms or embeddings, including helper functions for transforming or analyzing text data
 ```bash
-$ git clone git@github.com:MoleculeEngineering/albert-ds.git
-$ pip install "albert-ds[nlp]" #This should be run from within your python virtual environment
+$ pip install "albert-toolkit[nlp]" #This should be run from within your python virtual environment
 ```
 
 ## Models Stack
 The models stack includes all the dependencies necessary to build or run models. Installing the Models stack will also install the metrics stack
 ```bash
-$ git clone git@github.com:MoleculeEngineering/albert-ds.git
-$ pip install "albert-ds[models]" #This should be run from within your python virtual environment
+$ pip install "albert-toolkit[models]" #This should be run from within your python virtual environment
 ```
 
 ## Chemistry Stack
-The chemistry stacks includes all the dependencies needed to run the chemistry modeuls. 
+The chemistry stacks includes all the dependencies needed to run the chemistry modules -- the proper way to install the chemistry stack is throught he use of the `albert` cli tool. Simply run the following to install the chemistry dependencies after installing the main albert toolkit
 ```bash
-$ git clone git@github.com:MoleculeEngineering/albert-ds.git
-$ pip install "albert-ds[torch]" #This needs to happen first for the [chem] install to work correctly
-$ pip install "albert-ds[chem]" 
-
-# Using the Helper Script
-Included in the repository is a helper script `al.sh` which contains a few simple helper scripts for building, publishing, etc... 
-TODO: Include documentation here on the use of the helper script to build and publish the package to pypi.
+$ albert init-chem
+```
+This will require `cmake` and CUDA to be installed. 
+
```


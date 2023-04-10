# Comparing `tmp/Simba-UW-tf-dev-1.55.6.tar.gz` & `tmp/Simba-UW-tf-dev-1.55.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.55.6.tar", last modified: Fri Apr  7 12:49:03 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.55.7.tar", last modified: Mon Apr 10 12:23:11 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.55.6.tar` & `Simba-UW-tf-dev-1.55.7.tar`

### file list

```diff
@@ -1,381 +1,385 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/
--rw-r--r--   0 simon      (501) staff       (20)    32569 2023-03-19 16:35:16.000000 Simba-UW-tf-dev-1.55.6/simba/video_processing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.55.6/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    10851 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.55.6/simba/unsupervised/unsupervised_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6566 2023-03-21 14:26:03.000000 Simba-UW-tf-dev-1.55.6/simba/unsupervised/misc.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7227 2023-03-21 11:41:26.000000 Simba-UW-tf-dev-1.55.6/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     4061 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/unsupervised/data_extractors.py
--rw-r--r--   0 simon      (501) staff       (20)    11192 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.55.6/simba/unsupervised/dbcv.py
--rw-r--r--   0 simon      (501) staff       (20)    11456 2023-03-21 18:17:26.000000 Simba-UW-tf-dev-1.55.6/simba/unsupervised/visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7526 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/unsupervised/umap_embedder.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/unsupervised/visualization_tools/
--rw-r--r--   0 simon      (501) staff       (20)     2019 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/unsupervised/visualization_tools/vtk_embeddings.py
--rw-r--r--   0 simon      (501) staff       (20)      150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/unsupervised/ui_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    49992 2023-03-22 15:08:56.000000 Simba-UW-tf-dev-1.55.6/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)    16189 2023-03-21 15:42:27.000000 Simba-UW-tf-dev-1.55.6/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6642 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3789 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     5630 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/unsupervised/cluster_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    19024 2023-04-06 19:25:58.000000 Simba-UW-tf-dev-1.55.6/simba/enums.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7463 2023-03-15 19:17:12.000000 Simba-UW-tf-dev-1.55.6/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)     8562 2023-03-15 19:17:04.000000 Simba-UW-tf-dev-1.55.6/simba/bounding_box_tools/find_bounderies.py
--rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.55.6/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     9530 2023-03-15 16:54:41.000000 Simba-UW-tf-dev-1.55.6/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12627 2023-03-15 16:54:41.000000 Simba-UW-tf-dev-1.55.6/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-07 11:26:42.000000 Simba-UW-tf-dev-1.55.6/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42807 2023-04-04 12:57:34.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21541 2023-03-15 19:11:32.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)    19620 2023-04-03 12:08:14.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/fish_feature_extractor_2023.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    28028 2023-04-04 13:11:31.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-06 18:38:15.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     2347 2023-04-04 12:57:34.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    10734 2023-04-06 14:57:55.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    36798 2023-03-15 17:04:48.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/extract_features_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)     8428 2023-03-15 19:11:54.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)     5323 2023-03-19 18:30:53.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    46473 2023-04-04 13:07:58.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    24093 2023-04-04 13:11:31.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16763 2023-03-15 19:11:50.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/plotly_create_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.55.6/simba/requirements.txt
--rw-r--r--   0 simon      (501) staff       (20)     5832 2023-03-15 19:16:48.000000 Simba-UW-tf-dev-1.55.6/simba/severity_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     5941 2023-03-19 16:35:16.000000 Simba-UW-tf-dev-1.55.6/simba/user_pose_config_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.55.6/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    41856 2023-04-05 17:24:50.000000 Simba-UW-tf-dev-1.55.6/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     8182 2023-04-05 13:03:24.000000 Simba-UW-tf-dev-1.55.6/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-06 14:21:49.000000 Simba-UW-tf-dev-1.55.6/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    34512 2023-04-06 19:49:53.000000 Simba-UW-tf-dev-1.55.6/simba/machine_model_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5266 2023-03-15 15:43:20.000000 Simba-UW-tf-dev-1.55.6/simba/remove_keypoints_in_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6326 2023-03-17 16:27:19.000000 Simba-UW-tf-dev-1.55.6/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9947 2023-03-18 15:35:38.000000 Simba-UW-tf-dev-1.55.6/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9170 2023-03-22 19:35:38.000000 Simba-UW-tf-dev-1.55.6/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.55.6/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.55.6/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18283 2023-04-01 14:14:21.000000 Simba-UW-tf-dev-1.55.6/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8336 2023-03-15 19:12:46.000000 Simba-UW-tf-dev-1.55.6/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6919 2023-03-19 15:03:14.000000 Simba-UW-tf-dev-1.55.6/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5426 2023-03-19 16:33:18.000000 Simba-UW-tf-dev-1.55.6/simba/third_party_label_appenders/solomon_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7261 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.55.6/simba/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)    13056 2023-03-19 16:33:18.000000 Simba-UW-tf-dev-1.55.6/simba/FSTTC_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12620 2023-04-06 11:43:07.000000 Simba-UW-tf-dev-1.55.6/simba/create_project_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    13421 2023-04-06 11:40:29.000000 Simba-UW-tf-dev-1.55.6/simba/video_info_table.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.55.6/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8507 2023-03-15 19:09:16.000000 Simba-UW-tf-dev-1.55.6/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    13530 2023-03-15 19:08:52.000000 Simba-UW-tf-dev-1.55.6/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.55.6/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    16374 2023-03-15 19:09:04.000000 Simba-UW-tf-dev-1.55.6/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    13160 2023-03-20 13:43:59.000000 Simba-UW-tf-dev-1.55.6/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/extract_frames_fast.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.55.6/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     5626 2023-03-28 20:35:14.000000 Simba-UW-tf-dev-1.55.6/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     3825 2023-04-06 19:25:38.000000 Simba-UW-tf-dev-1.55.6/simba/utils/lookups.py
--rw-r--r--   0 simon      (501) staff       (20)    11967 2023-04-06 19:37:44.000000 Simba-UW-tf-dev-1.55.6/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    21581 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.55.6/simba/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     9937 2023-03-19 16:35:16.000000 Simba-UW-tf-dev-1.55.6/simba/timebins_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    45524 2023-04-04 20:09:14.000000 Simba-UW-tf-dev-1.55.6/simba/train_model_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     7520 2023-03-19 16:35:16.000000 Simba-UW-tf-dev-1.55.6/simba/timebins_clf_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.55.6/simba/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     6548 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.55.6/simba/movement_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/pybursts.py
--rw-r--r--   0 simon      (501) staff       (20)     5265 2023-03-29 18:04:02.000000 Simba-UW-tf-dev-1.55.6/simba/run_model_new.py
--rw-r--r--   0 simon      (501) staff       (20)     3104 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/rw_dfs.py
--rw-r--r--   0 simon      (501) staff       (20)     6684 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/reverse_2_animal_tracking.py
--rw-r--r--   0 simon      (501) staff       (20)     9743 2023-03-17 16:34:02.000000 Simba-UW-tf-dev-1.55.6/simba/Directing_animals_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     4357 2023-03-30 16:19:09.000000 Simba-UW-tf-dev-1.55.6/simba/Validate_model_one_video_run_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9548 2023-04-06 00:40:25.000000 Simba-UW-tf-dev-1.55.6/simba/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.55.6/simba/setting_menu.py
--rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.55.6/simba/interpolate_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     8571 2023-03-30 10:06:59.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    17962 2023-03-24 13:40:30.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14592 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12928 2023-03-30 10:08:46.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15777 2023-03-20 13:34:43.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8884 2023-03-20 13:34:43.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    16058 2023-03-22 14:43:52.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/misc_visualizations.py
--rw-r--r--   0 simon      (501) staff       (20)    13501 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    17696 2023-03-29 16:22:09.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16328 2023-03-24 13:47:50.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12588 2023-03-20 13:34:43.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    12585 2023-03-20 13:34:43.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5832 2023-03-29 17:02:51.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12184 2023-03-31 13:53:09.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    11202 2023-03-19 16:21:53.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)    12442 2023-03-17 16:34:02.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9856 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    17290 2023-04-06 00:33:50.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    19958 2023-03-24 13:47:50.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10157 2023-03-17 16:27:19.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    12444 2023-03-20 13:34:43.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8609 2023-03-15 13:37:59.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    12970 2023-03-20 13:34:43.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15626 2023-03-29 17:05:49.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13165 2023-03-20 13:34:43.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     8891 2023-03-20 13:34:43.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13554 2023-04-01 13:12:31.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9839 2023-03-17 16:34:02.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16155 2023-03-20 13:34:43.000000 Simba-UW-tf-dev-1.55.6/simba/plotting/heat_mapper_location_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)     7454 2023-03-13 22:11:36.000000 Simba-UW-tf-dev-1.55.6/simba/interpolate_smooth_post_hoc.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/reverse_tracking_order.py
--rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.55.6/simba/concatenator_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2824 2023-03-24 16:12:51.000000 Simba-UW-tf-dev-1.55.6/simba/extract_annotation_frames.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7385 2023-03-24 13:34:06.000000 Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     2248 2023-03-24 13:34:06.000000 Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.55.6/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43831 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    21382 2023-03-31 10:40:20.000000 Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11920 2023-03-31 10:48:40.000000 Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    15175 2023-03-20 12:28:41.000000 Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_image.py
--rw-r--r--   0 simon      (501) staff       (20)    57395 2023-04-06 00:28:01.000000 Simba-UW-tf-dev-1.55.6/simba/misc_tools.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)    25782 2023-03-20 12:51:35.000000 Simba-UW-tf-dev-1.55.6/simba/pose_importers/sleap_importer_slp.py
--rw-r--r--   0 simon      (501) staff       (20)    24720 2023-03-13 15:26:36.000000 Simba-UW-tf-dev-1.55.6/simba/pose_importers/sleap_importer_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    26507 2023-03-21 12:58:39.000000 Simba-UW-tf-dev-1.55.6/simba/pose_importers/dlc_multi_animal_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    23731 2023-03-20 12:55:04.000000 Simba-UW-tf-dev-1.55.6/simba/pose_importers/sleap_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)    16536 2023-03-20 13:30:18.000000 Simba-UW-tf-dev-1.55.6/simba/pose_importers/import_trk.py
--rw-r--r--   0 simon      (501) staff       (20)     7837 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.55.6/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     8905 2023-03-20 13:49:13.000000 Simba-UW-tf-dev-1.55.6/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8173 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/pose_importers/trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)   232876 2023-04-06 14:21:49.000000 Simba-UW-tf-dev-1.55.6/simba/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/extract_seqframes.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/1.png
--rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/get_coordinates_tools_v2.py
--rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.55.6/simba/pup_retrieval_protocol.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7712 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.55.6/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8264 2023-03-15 17:05:35.000000 Simba-UW-tf-dev-1.55.6/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     4362 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     2569 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.55.6/simba/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)    17642 2023-04-04 23:10:52.000000 Simba-UW-tf-dev-1.55.6/simba/train_mutiple_models.py
--rw-r--r--   0 simon      (501) staff       (20)    60456 2023-04-07 12:46:45.000000 Simba-UW-tf-dev-1.55.6/simba/SimBA.py
--rw-r--r--   0 simon      (501) staff       (20)    27431 2023-04-04 14:39:01.000000 Simba-UW-tf-dev-1.55.6/simba/labelling_advanced_interface.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-07 11:26:42.000000 Simba-UW-tf-dev-1.55.6/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.55.6/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)   454535 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/img/splash.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.55.6/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.55.6/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/assets/TheGoldenLab.PNG
--rw-r--r--   0 simon      (501) staff       (20)    21392 2023-03-22 19:01:48.000000 Simba-UW-tf-dev-1.55.6/simba/drop_bp_cords.py
--rw-r--r--   0 simon      (501) staff       (20)     8116 2023-03-19 18:27:51.000000 Simba-UW-tf-dev-1.55.6/simba/read_config_unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    11564 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.55.6/simba/project_config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.55.6/simba/set_hyperparameters.py
--rw-r--r--   0 simon      (501) staff       (20)    20780 2023-04-04 23:58:36.000000 Simba-UW-tf-dev-1.55.6/simba/train_single_model.py
--rw-r--r--   0 simon      (501) staff       (20)     6426 2023-03-17 16:57:53.000000 Simba-UW-tf-dev-1.55.6/simba/create_clf_log.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/simba/batch_process_videos/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.55.6/simba/batch_process_videos/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    24896 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.55.6/simba/batch_process_videos/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/batch_process_videos/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    10936 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
--rw-r--r--   0 simon      (501) staff       (20)     9563 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.55.6/simba/Kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8392 2023-04-03 14:06:05.000000 Simba-UW-tf-dev-1.55.6/simba/reorganize_keypoint_in_pose.py
--rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.55.6/simba/~$features.pptx
--rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.6/simba/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    12878 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      640 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.55.6/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.55.6/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.55.6/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-07 12:49:01.000000 Simba-UW-tf-dev-1.55.6/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-07 12:49:03.000000 Simba-UW-tf-dev-1.55.6/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/
+-rw-r--r--   0 simon      (501) staff       (20)    32514 2023-04-09 17:57:09.000000 Simba-UW-tf-dev-1.55.7/simba/video_processing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.55.7/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    10851 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.55.7/simba/unsupervised/unsupervised_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6566 2023-03-21 14:26:03.000000 Simba-UW-tf-dev-1.55.7/simba/unsupervised/misc.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7227 2023-03-21 11:41:26.000000 Simba-UW-tf-dev-1.55.7/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4061 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/unsupervised/data_extractors.py
+-rw-r--r--   0 simon      (501) staff       (20)    11192 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.55.7/simba/unsupervised/dbcv.py
+-rw-r--r--   0 simon      (501) staff       (20)    11456 2023-03-21 18:17:26.000000 Simba-UW-tf-dev-1.55.7/simba/unsupervised/visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7526 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/unsupervised/umap_embedder.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/unsupervised/visualization_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     2019 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/unsupervised/visualization_tools/vtk_embeddings.py
+-rw-r--r--   0 simon      (501) staff       (20)      150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/unsupervised/ui_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    49992 2023-03-22 15:08:56.000000 Simba-UW-tf-dev-1.55.7/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)    16189 2023-03-21 15:42:27.000000 Simba-UW-tf-dev-1.55.7/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6642 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3789 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     5630 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/unsupervised/cluster_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    19253 2023-04-10 11:55:27.000000 Simba-UW-tf-dev-1.55.7/simba/enums.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7518 2023-04-09 17:57:09.000000 Simba-UW-tf-dev-1.55.7/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)     8594 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.7/simba/bounding_box_tools/find_bounderies.py
+-rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.55.7/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     9504 2023-04-09 17:57:09.000000 Simba-UW-tf-dev-1.55.7/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12662 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.7/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-09 00:53:36.000000 Simba-UW-tf-dev-1.55.7/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42806 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21558 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)    19620 2023-04-03 12:08:14.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/fish_feature_extractor_2023.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27987 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-09 15:55:31.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     2347 2023-04-04 12:57:34.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    10742 2023-04-09 18:45:48.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    36798 2023-03-15 17:04:48.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/extract_features_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8462 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)     5323 2023-03-19 18:30:53.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    46472 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24059 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16776 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/plotly_create_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.55.7/simba/requirements.txt
+-rw-r--r--   0 simon      (501) staff       (20)     5870 2023-04-09 17:32:42.000000 Simba-UW-tf-dev-1.55.7/simba/severity_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5941 2023-03-19 16:35:16.000000 Simba-UW-tf-dev-1.55.7/simba/user_pose_config_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.55.7/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    41856 2023-04-05 17:24:50.000000 Simba-UW-tf-dev-1.55.7/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-04-07 13:58:40.000000 Simba-UW-tf-dev-1.55.7/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-06 14:21:49.000000 Simba-UW-tf-dev-1.55.7/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    34553 2023-04-10 12:16:44.000000 Simba-UW-tf-dev-1.55.7/simba/machine_model_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5261 2023-04-09 17:32:42.000000 Simba-UW-tf-dev-1.55.7/simba/remove_keypoints_in_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6366 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.7/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9955 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.7/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9208 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.7/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.55.7/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.55.7/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18290 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.7/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8339 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.7/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6932 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.7/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5467 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.7/simba/third_party_label_appenders/solomon_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7284 2023-04-09 17:01:02.000000 Simba-UW-tf-dev-1.55.7/simba/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)    12829 2023-04-09 17:01:02.000000 Simba-UW-tf-dev-1.55.7/simba/FSTTC_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.7/simba/create_project_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    13421 2023-04-06 11:40:29.000000 Simba-UW-tf-dev-1.55.7/simba/video_info_table.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.55.7/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8598 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.7/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    13530 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.7/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.55.7/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    16395 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.7/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    13231 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.7/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/extract_frames_fast.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.55.7/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     5999 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.7/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     4038 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.7/simba/utils/lookups.py
+-rw-r--r--   0 simon      (501) staff       (20)    12855 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.7/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    21609 2023-04-10 12:16:44.000000 Simba-UW-tf-dev-1.55.7/simba/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)    10038 2023-04-09 17:40:33.000000 Simba-UW-tf-dev-1.55.7/simba/timebins_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    45516 2023-04-10 11:45:13.000000 Simba-UW-tf-dev-1.55.7/simba/train_model_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     7598 2023-04-09 17:40:33.000000 Simba-UW-tf-dev-1.55.7/simba/timebins_clf_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.55.7/simba/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     6653 2023-04-09 17:01:02.000000 Simba-UW-tf-dev-1.55.7/simba/movement_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/pybursts.py
+-rw-r--r--   0 simon      (501) staff       (20)     5421 2023-04-09 17:32:42.000000 Simba-UW-tf-dev-1.55.7/simba/run_model_new.py
+-rw-r--r--   0 simon      (501) staff       (20)     3104 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/rw_dfs.py
+-rw-r--r--   0 simon      (501) staff       (20)     6684 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/reverse_2_animal_tracking.py
+-rw-r--r--   0 simon      (501) staff       (20)     9739 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.7/simba/Directing_animals_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     4308 2023-04-09 17:57:09.000000 Simba-UW-tf-dev-1.55.7/simba/Validate_model_one_video_run_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9548 2023-04-06 00:40:25.000000 Simba-UW-tf-dev-1.55.7/simba/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.55.7/simba/setting_menu.py
+-rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.55.7/simba/interpolate_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     8599 2023-04-09 19:29:40.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    17990 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14590 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12951 2023-04-09 19:32:53.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15777 2023-04-09 19:32:53.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8884 2023-04-09 19:45:13.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16002 2023-04-09 19:41:31.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/misc_visualizations.py
+-rw-r--r--   0 simon      (501) staff       (20)    13500 2023-04-09 19:41:31.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    17700 2023-04-09 19:45:13.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16307 2023-04-09 19:48:05.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12657 2023-04-09 19:32:53.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    12612 2023-04-09 19:48:05.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5861 2023-04-09 19:45:13.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12222 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    11230 2023-04-09 19:29:40.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)    12467 2023-04-09 18:45:48.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9884 2023-04-09 18:45:48.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    17318 2023-04-09 19:41:31.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    20003 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10185 2023-04-09 18:45:48.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    12473 2023-04-09 19:41:31.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8638 2023-04-09 19:29:40.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    12994 2023-04-09 19:29:40.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15652 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13196 2023-04-09 19:32:53.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-09 19:29:40.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13591 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9884 2023-04-09 18:45:48.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16155 2023-04-09 19:41:31.000000 Simba-UW-tf-dev-1.55.7/simba/plotting/heat_mapper_location_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)     7607 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.7/simba/interpolate_smooth_post_hoc.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/reverse_tracking_order.py
+-rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.55.7/simba/concatenator_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2861 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.7/simba/extract_annotation_frames.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7403 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2133 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.55.7/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43831 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    21400 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11952 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    15204 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_image.py
+-rw-r--r--   0 simon      (501) staff       (20)    58097 2023-04-10 11:55:27.000000 Simba-UW-tf-dev-1.55.7/simba/misc_tools.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)    25829 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.7/simba/pose_importers/sleap_importer_slp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24655 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.7/simba/pose_importers/sleap_importer_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    26542 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.7/simba/pose_importers/dlc_multi_animal_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    23766 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.7/simba/pose_importers/sleap_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)    16536 2023-03-20 13:30:18.000000 Simba-UW-tf-dev-1.55.7/simba/pose_importers/import_trk.py
+-rw-r--r--   0 simon      (501) staff       (20)     7871 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.7/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     8967 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.7/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8173 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/pose_importers/trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)   232870 2023-04-09 17:26:39.000000 Simba-UW-tf-dev-1.55.7/simba/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/extract_seqframes.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/1.png
+-rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/get_coordinates_tools_v2.py
+-rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.55.7/simba/pup_retrieval_protocol.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7719 2023-04-09 18:45:48.000000 Simba-UW-tf-dev-1.55.7/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.55.7/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8272 2023-04-09 18:45:48.000000 Simba-UW-tf-dev-1.55.7/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     4311 2023-04-09 18:45:48.000000 Simba-UW-tf-dev-1.55.7/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     2582 2023-04-09 17:26:39.000000 Simba-UW-tf-dev-1.55.7/simba/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)    17772 2023-04-09 17:40:33.000000 Simba-UW-tf-dev-1.55.7/simba/train_mutiple_models.py
+-rw-r--r--   0 simon      (501) staff       (20)    62529 2023-04-09 17:32:42.000000 Simba-UW-tf-dev-1.55.7/simba/SimBA.py
+-rw-r--r--   0 simon      (501) staff       (20)    27470 2023-04-10 12:16:44.000000 Simba-UW-tf-dev-1.55.7/simba/labelling_advanced_interface.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-09 15:55:31.000000 Simba-UW-tf-dev-1.55.7/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-09 00:58:33.000000 Simba-UW-tf-dev-1.55.7/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)    48127 2023-04-09 01:08:10.000000 Simba-UW-tf-dev-1.55.7/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.55.7/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)   454535 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/img/splash.png
+-rw-r--r--   0 simon      (501) staff       (20)    59795 2023-04-09 00:58:12.000000 Simba-UW-tf-dev-1.55.7/simba/assets/img/splash_1500ms.mp4
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.55.7/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.55.7/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/assets/TheGoldenLab.PNG
+-rw-r--r--   0 simon      (501) staff       (20)    21471 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.7/simba/drop_bp_cords.py
+-rw-r--r--   0 simon      (501) staff       (20)     8116 2023-03-19 18:27:51.000000 Simba-UW-tf-dev-1.55.7/simba/read_config_unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    11710 2023-04-09 17:26:39.000000 Simba-UW-tf-dev-1.55.7/simba/project_config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.55.7/simba/set_hyperparameters.py
+-rw-r--r--   0 simon      (501) staff       (20)    20898 2023-04-09 17:40:33.000000 Simba-UW-tf-dev-1.55.7/simba/train_single_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     6434 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.7/simba/create_clf_log.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/simba/batch_process_videos/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.55.7/simba/batch_process_videos/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    24896 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.55.7/simba/batch_process_videos/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/batch_process_videos/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    10882 2023-04-09 17:57:09.000000 Simba-UW-tf-dev-1.55.7/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
+-rw-r--r--   0 simon      (501) staff       (20)     9581 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.7/simba/Kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8394 2023-04-09 17:32:42.000000 Simba-UW-tf-dev-1.55.7/simba/reorganize_keypoint_in_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.55.7/simba/~$features.pptx
+-rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.7/simba/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    13013 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      640 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.55.7/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.55.7/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.55.7/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-10 12:23:00.000000 Simba-UW-tf-dev-1.55.7/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-10 12:23:10.000000 Simba-UW-tf-dev-1.55.7/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.55.6/PKG-INFO` & `Simba-UW-tf-dev-1.55.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.55.6
+Version: 1.55.7
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/video_processing.py` & `Simba-UW-tf-dev-1.55.7/simba/video_processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __author__ = "Simon Nilsson"
 
 import glob, os
 from simba.read_config_unit_tests import (check_file_exist_and_readable,
                                           check_int)
-from simba.misc_tools import get_fn_ext, get_video_meta_data
+from simba.misc_tools import (get_fn_ext, get_video_meta_data, stdout_success)
 import cv2
 from pathlib import Path
 from PIL import Image
 from simba.extract_frames_fast import video_to_frames
 from simba.enums import Formats
 import re
 import subprocess
@@ -50,15 +50,15 @@
         raise NoFilesFoundError('SIMBA ERROR: No {} files (with .{} file ending) found in the {} directory'.format(file_type_in, file_type_in, directory))
     print('{} image files found in {}...'.format(str(len(files_found)), directory))
     for file_path in files_found:
         im = Image.open(file_path)
         save_name = file_path.replace('.' + str(file_type_in), '.' + str(file_type_out))
         im.save(save_name)
         os.remove(file_path)
-    print('SIMBA COMPLETE: Files in {} directory converted to {}'.format(directory, file_type_out))
+    stdout_success(msg=f'SIMBA COMPLETE: Files in {directory} directory converted to {file_type_out}')
 
 
 def clahe_enhance_video(file_path: str):
     """
     Helper to convert a single video file to clahe-enhanced greyscale .avi file. The result is saved with prefix
     ``CLAHE_`` in the same directory as in the input file.
 
@@ -137,17 +137,15 @@
     if not os.path.exists(save_dir): os.makedirs(save_dir)
     for frm_cnt, frm_number in enumerate(frame_range):
         cap.set(1, frm_number)
         ret, frame = cap.read()
         frm_save_path = os.path.join(save_dir, '{}.{}'.format(str(frm_number), 'png'))
         cv2.imwrite(frm_save_path,frame)
         print('Frame {} saved (Frame {}/{})'.format(str(frm_number), str(frm_cnt), str(len(frame_range))))
-    print('SIMBA COMPLETE: {} frames extracted for video {}'.format(str(len(frame_range)), file_name))
-
-
+    stdout_success(msg=f'{str(len(frame_range))} frames extracted for video {file_name}')
 
 
 def change_single_video_fps(file_path: str,
                             fps: int):
     """
     Helper to change the fps of a single video file. Results are stored in the same directory as in the input file with
     the suffix ``_fps_new_fps``.
@@ -167,16 +165,15 @@
     if int(fps) == int(video_meta_data['fps']):
         print('SIMBA WARNING: The new fps is the same as the input fps for video {}'.format(file_name))
     save_path = os.path.join(dir_name, file_name + '_fps_{}{}'.format(str(fps), str(ext)))
     if os.path.isfile(save_path):
         print('SIMBA WARNING: Overwriting existing file at {}'.format(save_path))
     command = str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -filter:v fps=fps=' + str(fps) + ' ' + '"' + save_path + '"'
     subprocess.call(command, shell=True)
-    print('SIMBA COMPLETE: FPS of video {} changed from {} to {} and saved in directory {}'.format(file_name, str(video_meta_data['fps']), str(fps), save_path))
-
+    stdout_success(msg=f'SIMBA COMPLETE: FPS of video {file_name} changed from {str(video_meta_data["fps"])} to {str(fps)} and saved in directory {save_path}')
 
 def change_fps_of_multiple_videos(directory: str,
                                   fps: int):
     """
     Helper to change the fps of video files in a folder. Results are stored in the same directory as in the input files with
     the suffix ``_fps_new_fps``.
 
@@ -202,15 +199,15 @@
     for file_cnt, file_path in enumerate(video_paths):
         dir_name, file_name, ext = get_fn_ext(filepath=file_path)
         print('Converting FPS for {}...'.format(file_name))
         save_path = os.path.join(dir_name, file_name + '_fps_{}{}'.format(str(fps), str(ext)))
         command = str('ffmpeg -i ') + str(file_path) + ' -filter:v fps=fps=' + str(fps) + ' ' + '"' + save_path + '"'
         subprocess.call(command, shell=True)
         print('Video {} complete...'.format(file_name))
-    print('SIMBA COMPLETE: FPS of {} videos changed to {}'.format(str(len(video_paths)), str(fps)))
+    stdout_success(msg=f'SIMBA COMPLETE: FPS of {str(len(video_paths))} videos changed to { str(fps)}')
 
 def convert_video_powerpoint_compatible_format(file_path: str):
     """
     Helper to make a powerpoint compatible copy of a video file. The results is stored in the same directory as the
     input file with the ``_powerpointready`` suffix.
 
     Parameters
@@ -225,15 +222,15 @@
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_powerpointready.mp4')
     if os.path.isfile(save_name):
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
     command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -c:v libx264 -preset slow  -profile:v high -level:v 4.0 -pix_fmt yuv420p -crf 22 -codec:a aac ' + '"' + save_name + '"')
     print('Creating video in powerpoint compatible format... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-    print('SIMBA COMPLETE: Video converted! {} generated!'.format(save_name))
+    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 def convert_to_mp4(file_path: str):
     """
     Helper to convert a video file to mp4 format. The results is stored in the same directory as the
     input file with the ``_converted.mp4`` suffix.
 
     Parameters
@@ -247,15 +244,15 @@
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_converted.mp4')
     if os.path.isfile(save_name):
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
     command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' ' + '"' + save_name + '"')
     print('Converting to mp4... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-    print('SIMBA COMPLETE: Video converted! {} generated!'.format(save_name))
+    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 
 def video_to_greyscale(file_path: str):
     """
     Helper to convert a video file to greyscale mp4 format. The results is stored in the same directory as the
     input file with the ``_grayscale.mp4`` suffix.
 
@@ -270,15 +267,15 @@
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_grayscale.mp4')
     if os.path.isfile(save_name):
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
     command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -vf format=gray ' + '"' + save_name + '"')
     print('Converting to greyscale... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-    print('SIMBA COMPLETE: Video converted! {} generated!'.format(save_name))
+    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 
 def superimpose_frame_count(file_path: str):
     """
     Helper to superimpose frame count on a video file. The results is stored in the same directory as the
     input file with the ``_frame_no.mp4`` suffix.
 
@@ -299,17 +296,15 @@
         subprocess.check_output(command, shell=True)
         subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     except subprocess.CalledProcessError as e:
         simba_cw = os.path.dirname(simba.__file__)
         simba_font_path = Path(simba_cw, 'assets', 'UbuntuMono-Regular.ttf')
         command = 'ffmpeg -y -i ' + file_path + ' -vf "drawtext=fontfile={}:'.format(simba_font_path) + "text='%{frame_num}': start_number=1: x=(w-tw)/2: y=h-(2*lh): fontcolor=black: fontsize=20: box=1: boxcolor=white: boxborderw=5" + '" ' + "-c:a copy " + save_name
         subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-    print('SIMBA COMPLETE: Video converted! {} generated!'.format(save_name))
-
-
+    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 def remove_beginning_of_video(file_path: str,
                               time: int):
     """
     Helper to remove N seconds from the beginning of a video file. The results is stored in the same directory as the
     input file with the ``_shorten.mp4`` suffix.
 
@@ -324,16 +319,15 @@
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_shorten.mp4')
     if os.path.isfile(save_name):
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
     command = (str('ffmpeg -ss ') + str(int(time)) + ' -i ' + '"' + str(file_path) + '"' + ' -c:v libx264 -c:a aac ' + '"' + save_name + '"')
     print('Shortening video... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-    print('SIMBA COMPLETE: Video converted! {} generated!'.format(save_name))
-
+    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 
 def clip_video_in_range(file_path: str,
                         start_time: str,
                         end_time: str):
     """
     Helper to clip video in a specific range. The results is stored in the same directory as the
@@ -353,15 +347,15 @@
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_clipped.mp4')
     if os.path.isfile(save_name):
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
     command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -ss ' + str(start_time) + ' -to ' + str(end_time) + ' -async 1 ' + '"' + save_name + '"')
     print('Clipping video... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-    print('SIMBA COMPLETE: Video converted! {} generated!'.format(save_name))
+    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 def downsample_video(file_path: str,
                      video_height: int,
                      video_width: int):
     """
     Helper to down-sample a video file. The results is stored in the same directory as the
     input file with the ``_downsampled.mp4`` suffix.
@@ -382,16 +376,15 @@
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_downsampled.mp4')
     if os.path.isfile(save_name):
         raise FileExistError('SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
     command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -vf scale=' + str(video_width) + ':' + str(video_height) + ' ' + '"' + save_name + '"' + ' -hide_banner')
     print('Down-sampling video... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-    print('SIMBA COMPLETE: Video converted! {} generated!'.format(save_name))
-
+    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 def gif_creator(file_path: str,
                 start_time: int,
                 duration: int,
                 width: int):
     """
     Helper to create a sample gif from a video file. The results is stored in the same directory as the
@@ -418,16 +411,15 @@
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '.gif')
     if os.path.isfile(save_name):
         raise FileExistError('SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
     command = 'ffmpeg -ss ' + str(start_time) + ' -t ' + str(duration) + ' -i ' + '"' + str(file_path) + '"' + ' -filter_complex "[0:v] fps=15,scale=w=' + str(width) + ':h=-1,split [a][b];[a] palettegen=stats_mode=single [p];[b][p] paletteuse=new=1" ' + '"' + str(save_name) + '"'
     print('Creating gif sample... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-    print('SIMBA COMPLETE: Video converted! {} generated!'.format(save_name))
-
+    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 
 def batch_convert_video_format(directory: str,
                                input_format: str,
                                output_format: str):
     """
     Helper to batch convert all videos in a folder of specific format into a different video format. The results are
@@ -458,16 +450,16 @@
         print('Processing video {}...'.format(file_name))
         save_path = os.path.join(dir_name, file_name + '.{}'.format(output_format.lower()))
         if os.path.isfile(save_path):
             raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_path))
         command = 'ffmpeg -y -i ' + '"' + file_path + '"' + ' -c:v libx264 -crf 5 -preset medium -c:a libmp3lame -b:a 320k '+'"' + save_path + '"'
         subprocess.call(command, shell=True, stdout=subprocess.PIPE)
         print('Video {} complete, (Video {}/{})...'.format(file_name, str(file_cnt+1), str(len(video_paths))))
-    print('SIMBA COMPLETE: {} videos converted in {} directory!'.format(str(len(video_paths)), directory))
 
+    stdout_success(msg=f'SIMBA COMPLETE: {str(len(video_paths))} videos converted in {directory} directory!')
 
 def batch_create_frames(directory: str):
     """
     Helper to extract all frames for all videos in a directory. Results are stored within sub-directories in the input
     directory named according to the video files.
 
     Parameters
@@ -489,16 +481,15 @@
     for file_cnt, file_path in enumerate(video_paths):
         dir_name, file_name, ext = get_fn_ext(filepath=file_path)
         print('Processing video {}...'.format(file_name))
         save_dir = os.path.join(dir_name, file_name)
         if not os.path.exists(save_dir): os.makedirs(save_dir)
         video_to_frames(file_path, save_dir, overwrite=True, every=1, chunk_size=1000)
         print('Video {} complete, (Video {}/{})...'.format(file_name, str(file_cnt + 1), str(len(video_paths))))
-    print('SIMBA COMPLETE: {} videos converted into frames in {} directory!'.format(str(len(video_paths)), directory))
-
+    stdout_success(msg=f'{str(len(video_paths))} videos converted into frames in {directory} directory!')
 
 def extract_frames_single_video(file_path: str):
     """
     Helper to extract all frames for a single. Results are stored within a sub-directory in the same
     directory as the input file.
 
     Parameters
@@ -510,16 +501,15 @@
     check_file_exist_and_readable(file_path=file_path)
     _ = get_video_meta_data(file_path)
     dir_name, file_name, ext = get_fn_ext(filepath=file_path)
     save_dir = os.path.join(dir_name, file_name)
     if not os.path.exists(save_dir): os.makedirs(save_dir)
     print('Processing video {}...'.format(file_name))
     video_to_frames(file_path, save_dir, overwrite=True, every=1, chunk_size=1000)
-    print('SIMBA COMPLETE: Video {} converted to images in {} directory!'.format(file_name, dir_name))
-
+    stdout_success(msg=f'Video {file_name} converted to images in {dir_name} directory!')
 
 def multi_split_video(file_path: str,
                       start_times: list,
                       end_times: list):
     """
     Helper divide a video file into multiple video files from specified start and stop times.
 
@@ -563,16 +553,15 @@
         save_path = os.path.join(dir_name, file_name + '_{}'.format(str(clip_cnt+1)) + '.mp4')
         if os.path.isfile(save_path):
             print('SIMBA ERROR: The outfile file already exist: {}.'.format(save_path))
             raise FileExistsError()
         command = (str('ffmpeg -i ') + '"' + file_path + '"' + ' -ss ' + start_time + ' -to ' + end_time + ' -async 1 ' + '"' + save_path + '"')
         print('Processing video clip {}...'.format(str(clip_cnt+1)))
         subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-    print('SIMBA COMPLETE: Video {} converted into {} clips in directory {}!'.format(file_name, str(len(start_times)), dir_name))
-
+    stdout_success(msg=f'Video {file_name} converted into {str(len(start_times))} clips in directory {dir_name}!')
 
 def crop_single_video(file_path: str):
     """
     Helper to crop a single video,
 
     Parameters
     ----------
@@ -596,16 +585,15 @@
     if (width == 0 and height == 0) or (width + height + top_lext_x + top_left_y == 0):
         raise CountError(msg='CROP FAILED: Cropping height and width are both 0. Please try again.')
     save_path = os.path.join(dir_name, file_name + '_cropped.mp4')
     if os.path.isfile(save_path):
         raise FileExistError(msg='SIMBA ERROR: The out file file already exist: {}.'.format(save_path))
     command = str('ffmpeg -y -i ') + '"' + str(file_path) + '"' + str(' -vf ') + str('"crop=') + str(width) + ':' + str(height) + ':' + str(top_lext_x) + ':' + str(top_left_y) + '" ' + str('-c:v libx264 -crf 21 -c:a copy ') + '"' + str(save_path) + '"'
     subprocess.call(command, shell=True)
-    print('SIMBA COMPLETE: Video {} cropped and saved at {}'.format(file_name, save_path))
-
+    stdout_success(f'Video {file_name} cropped and saved at {save_path}')
 
 def crop_multiple_videos(directory_path: str,
                          output_path: str):
     """
     Helper to crop multiple videos in a folder according to coordinates defines in one video.
 
     Parameters
@@ -642,17 +630,15 @@
         dir_name, file_name, ext = get_fn_ext(filepath=file_path)
         print('Cropping video {}...'.format(file_name))
         _ = get_video_meta_data(file_path)
         save_path = os.path.join(output_path, file_name + '_cropped.mp4')
         command = str('ffmpeg -i ') + '"' + file_path + '"' + str(' -vf ') + str('"crop=') + str(width) + ':' + str(height) + ':' + str(top_lext_x) + ':' + str(top_left_y) + '" ' + str('-c:v libx264 -crf 21 -c:a copy ') + '"' + str(save_path) + '"'
         subprocess.call(command, shell=True)
         print('Video {} cropped (Video {}/{})'.format(file_name, str(file_cnt+1), str(len(video_paths))))
-    print('SIMBA COMPLETE: {} videos cropped and saved in {} directory '.format(str(len(video_paths)), directory_path))
-
-
+    stdout_success(msg=f'{str(len(video_paths))} videos cropped and saved in {directory_path} directory')
 
 def frames_to_movie(directory: str,
                     fps: int,
                     bitrate: int,
                     img_format: str):
 
     """
@@ -683,15 +669,15 @@
     img = cv2.imread(img_paths_in_folder[0])
     img_h, img_w = int(img.shape[0]), int(img.shape[1])
     ffmpeg_fn = os.path.join(directory, '%d.{}'.format(img_format))
     save_path = os.path.join(os.path.dirname(directory), os.path.basename(directory) + '.mp4')
     command = str('ffmpeg -y -r ' + str(fps) + ' -f image2 -s ' + str(img_h) + 'x' + str(img_w) + ' -i ' + '"' + ffmpeg_fn + '"' + ' -vcodec libx264 -b ' + str(bitrate) + 'k ' + '"' + str(save_path) + '"')
     print('Creating {} from {} images...'.format(os.path.basename(save_path), str(len(img_paths_in_folder))))
     subprocess.call(command, shell=True)
-    print('SIMBA COMPLETE: Video created at {}'.format(save_path))
+    stdout_success(msg=f'Video created at {save_path}')
 
 
 def video_concatenator(video_one_path: str,
                        video_two_path: str,
                        resolution: int or str,
                        horizontal: bool):
     for file_path in [video_one_path, video_two_path]:
@@ -712,15 +698,15 @@
     print('Concatenating videos...')
     save_path = os.path.join(dir, file_name_1 + file_name_2 + '_concat.mp4')
     if horizontal:
         command = 'ffmpeg -y -i "{}" -i "{}" -filter_complex "[0:v]scale=-1:{}[v0];[v0][1:v]hstack=inputs=2" "{}"'.format(video_one_path, video_two_path, video_meta_data['height'], save_path)
     else:
         command = 'ffmpeg -y -i "{}" -i "{}" -filter_complex "[0:v]scale={}:-1[v0];[v0][1:v]vstack=inputs=2" "{}"'.format(video_one_path, video_two_path, video_meta_data['width'], save_path)
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-    print('SIMBA COMPLETE! Videos concatenated and saved at {}.'.format(save_path))
+    stdout_success(msg=f'Videos concatenated and saved at {save_path}')
 
 # video_concatenator(video_one_path='/Users/simon/Desktop/troubleshooting/Open_field_5/project_folder/frames/output/gantt_plots/SI_DAY3_308_CD1_PRESENT_2.mp4',
 #                    video_two_path= '/Users/simon/Desktop/troubleshooting/Open_field_5/project_folder/frames/output/gantt_plots/SI_DAY3_308_CD1_PRESENT.mp4',
 #                    resolution='Video 1',
 #                    horizontal=False)
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/unsupervised/unsupervised_ui.py` & `Simba-UW-tf-dev-1.55.7/simba/unsupervised/unsupervised_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/unsupervised/misc.py` & `Simba-UW-tf-dev-1.55.7/simba/unsupervised/misc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.55.7/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/unsupervised/data_extractors.py` & `Simba-UW-tf-dev-1.55.7/simba/unsupervised/data_extractors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/unsupervised/dbcv.py` & `Simba-UW-tf-dev-1.55.7/simba/unsupervised/dbcv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/unsupervised/visualizers.py` & `Simba-UW-tf-dev-1.55.7/simba/unsupervised/visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.55.7/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/unsupervised/visualization_tools/vtk_embeddings.py` & `Simba-UW-tf-dev-1.55.7/simba/unsupervised/visualization_tools/vtk_embeddings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.55.7/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.55.7/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.55.7/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.55.7/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.55.7/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/enums.py` & `Simba-UW-tf-dev-1.55.7/simba/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
     ABOUT_ME = Path('assets/img/about_me.png')
     PROBABILITY_PLOTS_DIR = Path('frames/output/probability_plots/')
     ROI_DEFINITIONS = Path('measures/ROI_definitions.h5')
     DETAILED_ROI_DATA_DIR = Path('logs/Detailed_ROI_data/')
     SHAP_LOGS = Path('logs/shap/')
     SPLASH_PATH_WINDOWS = Path('assets/img/splash.png')
     SPLASH_PATH_LINUX = Path('assets/img/splash.PNG')
+    SPLASH_PATH_MOVIE = Path('assets/img/splash.mp4')
     BG_IMG_PATH = Path('assets/img/bg_2.png')
     LOGO_ICON_WINDOWS_PATH = Path('assets/icons/SimBA_logo.ico')
     LOGO_ICON_DARWIN_PATH = Path('assets/icons/SimBA_logo.png')
     UNSUPERVISED_MODEL_NAMES = Path('assets/lookups/model_names.parquet')
 
 class Formats(Enum):
     MP4_CODEC = 'mp4v'
@@ -183,20 +184,26 @@
                                             'Annotations EVENT COUNT conflict',
                                             'Annotations data file NOT FOUND']
 
 class Defaults(Enum):
     MAX_TASK_PER_CHILD = 10
     CHUNK_SIZE = 1
     SPLASH_TIME = 2500
-    WELCOME_MSG = 'Welcome fellow scientists \n'
+    WELCOME_MSG = 'Welcome fellow scientists! \n'
     BROWSE_FOLDER_BTN_TEXT = 'Browse Folder'
     BROWSE_FILE_BTN_TEXT = 'Browse File'
     NO_FILE_SELECTED_TEXT = 'No file selected'
+    STR_SPLIT_DELIMITER = '\t'
 
-
+class TagNames(Enum):
+    GREETING = 'greeting'
+    COMPLETE = 'complete'
+    WARNING = 'warning'
+    ERROR = 'error'
+    STANDARD = 'standard'
 
 class DirNames(Enum):
     PROJECT = 'project_folder'
     MODEL = 'models'
     CONFIGS = 'configs'
     CSV = 'csv'
     FRAMES = 'frames'
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.55.7/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import pandas as pd
 from simba.rw_dfs import read_df
 from simba.read_config_unit_tests import (read_config_entry,
                                           read_config_file)
-from simba.misc_tools import detect_bouts, plug_holes_shortest_bout
+from simba.misc_tools import (detect_bouts,
+                              plug_holes_shortest_bout,
+                              stdout_success)
 from simba.feature_extractors.unit_tests import read_video_info_csv, read_video_info
 from simba.misc_tools import get_fn_ext
 from datetime import datetime
 import os, glob
 from simba.utils.errors import NotDirectoryError
 
 class AggBoundaryStatisticsCalculator(object):
@@ -90,22 +92,21 @@
                         animal_names = animal_interaction.split(':')
                         if len(animal_names) == 2:
                             animal_names.append('None')
                         out_df.loc[len(out_df)] = [video, animal_names[0], animal_names[1], animal_names[2], measurement, animal_interaction_value]
             out_df['VALUE'] = out_df['VALUE'].round(4)
             out_df = out_df.sort_values(by=['VIDEO', 'MEASUREMENT']).set_index('VIDEO')
             out_df.to_csv(save_path)
-            print('SIMBA COMPLETE: Aggregate animal-anchored ROI statistics saved at {}'.format(save_path))
-
+            stdout_success(msg=f'Aggregate animal-anchored ROI statistics saved at {save_path}')
         if len(self.detailed_interactions_results.keys()) > 0:
             save_path = os.path.join(self.project_path, 'logs', 'detailed_aggregate_statistics_anchored_rois_{}.csv'.format(self.datetime))
             out_df = pd.concat(self.detailed_interactions_results.values(), ignore_index=True)
             out_df = out_df.sort_values(by=['VIDEO']).set_index('VIDEO')
             out_df.to_csv(save_path)
-            print('SIMBA COMPLETE: Detailed Aggregate animal-anchored ROI statistics saved at {}'.format(save_path))
+            stdout_success(msg=f'Detailed Aggregate animal-anchored ROI statistics saved at {save_path}')
 
     def create_detailed_interactions_table(self,
                                            df: pd.DataFrame):
 
         df = df.rename(columns={'Start_time': 'START TIME (s)', 'End Time': 'END TIME (s)', 'Start_frame': 'START FRAME', 'End_frame': 'END FRAME', 'Bout_time': 'BOUT TIME (s)'})
         df['ROI 1'], df['ROI 2'], df['KEY-POINT'] = df['Event'].str.split(':', 2).str
         df = df.drop(['Event'], axis=1)
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/bounding_box_tools/find_bounderies.py` & `Simba-UW-tf-dev-1.55.7/simba/bounding_box_tools/find_bounderies.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 import shapely.wkt
 from joblib import Parallel, delayed
 import pickle
 import platform
 from simba.enums import ReadConfig, Dtypes, Paths
 from scipy.spatial import ConvexHull
 from simba.misc_tools import (check_multi_animal_status,
-                              find_core_cnt)
+                              find_core_cnt,
+                              stdout_success)
 
 
 class AnimalBoundaryFinder(object):
     """
     Class finding boundaries (animal-anchored) ROIs for animals in each frame. Result is saved as a pickle in the
     `project_folder/logs` directory of the SimBA project.
 
@@ -81,15 +82,15 @@
             self.center_bp_names = {}
             for animal, body_part in self.body_parts.items():
                 self.center_bp_names[animal] = [body_part + '_x', body_part + '_y']
 
     def _save_results(self):
         with open(self.save_path, 'wb') as path:
             pickle.dump(self.polygons, path, pickle.HIGHEST_PROTOCOL)
-        print('SIMBA COMPLETE: Animal shapes for {} videos saved at {}'.format(str(len(self.files_found)), self.save_path))
+        stdout_success(msg='Animal shapes for {str(len(self.files_found))} videos saved at {self.save_path}')
 
     def minimum_bounding_rectangle(self, points):
         pi2 = np.pi / 2.
         hull_points = points[ConvexHull(points).vertices]
         edges = hull_points[1:] - hull_points[:-1]
         angles = np.arctan2(edges[:, 1], edges[:, 0])
         angles = np.abs(np.mod(angles, pi2))
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.55.7/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.55.7/simba/bounding_box_tools/boundary_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 from simba.read_config_unit_tests import (read_config_file,
                                           read_config_entry,
                                           read_project_path_and_file_type)
 from simba.drop_bp_cords import (create_body_part_dictionary,
                                  getBpNames)
 from simba.enums import ReadConfig, Paths, Dtypes
-from simba.misc_tools import check_multi_animal_status
+from simba.misc_tools import check_multi_animal_status, stdout_success
 from simba.rw_dfs import read_df, save_df
 from joblib import Parallel, delayed
 from shapely.geometry import Point
 from copy import deepcopy
 from collections import defaultdict
 from simba.utils.errors import NoFilesFoundError
 import os
@@ -136,23 +136,23 @@
 
     def save_results(self):
         if not os.path.exists(self.save_folder): os.makedirs(self.save_folder)
         for video_cnt, (video_name, video_data) in enumerate(self.polygons.items()):
             save_path = os.path.join(self.save_folder, video_name + '.' + self.file_type)
             if (self.roi_intersections) and (self.roi_keypoint_intersections):
                 out_df = pd.concat([self.intersection_dfs[video_name], self.keypoint_dfs[video_name]], axis=1)
-                print(out_df)
             elif self.roi_intersections:
                 out_df = self.intersection_dfs[video_name]
             elif self.roi_keypoint_intersections:
                 out_df = self.keypoint_dfs[video_name]
             if self.save_format == 'CSV':
                 save_df(df=out_df,file_type='csv', save_path=save_path)
             elif self.save_format == 'PARQUET':
                 save_df(df=out_df, file_type='parquet', save_path=save_path)
             elif self.save_format == 'PICKLE':
                 out_df.to_pickle(save_path)
             print('Data for video {} saved...'.format(video_name))
-        print('SIMBA COMPLETE: Data for {} videos saved in {}'.format(str(len(self.polygons.keys())), self.save_folder))
+
+        stdout_success(msg=f'Data for {str(len(self.polygons.keys()))} videos saved in {self.save_folder}')
 
 # boundary_stats_calculator = BoundaryStatisticsCalculator(config_path='/Users/simon/Desktop/troubleshooting/termites/project_folder/project_config.ini',roi_intersections=True, roi_keypoint_intersections=True, save_format='CSV')
 # boundary_stats_calculator.save_results()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.55.7/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 from simba.read_config_unit_tests import (read_config_file,
                                           read_config_entry,
                                           read_project_path_and_file_type)
 from simba.read_config_unit_tests import check_file_exist_and_readable
 from simba.misc_tools import (check_multi_animal_status,
                               find_video_of_file,
                               get_video_meta_data,
-                              find_core_cnt, remove_a_folder)
+                              find_core_cnt,
+                              remove_a_folder,
+                              stdout_success)
 from simba.drop_bp_cords import (create_body_part_dictionary,
                                  getBpNames,
                                  createColorListofList)
 from simba.enums import Paths, ReadConfig, Dtypes
 from simba.rw_dfs import read_df
 import numpy as np
 import pickle
@@ -101,15 +103,14 @@
         if platform.system() == "Darwin":
             multiprocessing.set_start_method('spawn', force=True)
 
         self.config, self.config_path = read_config_file(ini_path=config_path), config_path
         self.project_path, self.file_type = read_project_path_and_file_type(config=self.config)
         self.polygon_path = os.path.join(self.project_path, 'logs', 'anchored_rois.pickle')
         self.video_name, self.include_key_points, self.greyscale, self.roi_attributes = video_name, include_key_points, greyscale, roi_attributes
-        print(roi_attributes)
         self.show_intersections, self.intersection_data_folder = show_intersections, os.path.join(self.project_path, 'csv', 'anchored_roi_data')
         check_file_exist_and_readable(file_path=self.polygon_path)
         self.intersections_df = None
         if self.show_intersections: self._find_intersection_data()
         with open(self.polygon_path, 'rb') as fp: self.polygons = pickle.load(fp)
         self.input_dir = os.path.join(self.project_path, Paths.OUTLIER_CORRECTED.value)
         self.video_dir = os.path.join(self.project_path, 'videos')
@@ -202,15 +203,15 @@
         returned = os.system('ffmpeg -f concat -safe 0 -i "{}" "{}" -hide_banner -loglevel error'.format(temp_txt_path, self.save_video_path))
         while True:
             if returned != 0:
                 pass
             else:
                 remove_a_folder(folder_dir=self.temp_folder)
                 break
-        print('SIMBA COMPLETE: Anchored ROI video created at {}'.format(self.save_video_path))
+        stdout_success(msg=f'Anchored ROI video created at {self.save_video_path}')
 
 # boundary_visualizer = BoundaryVisualizer(config_path='/Users/simon/Desktop/troubleshooting/termites/project_folder/project_config.ini',
 #                                          video_name='termites_test',
 #                                          include_key_points=True,
 #                                          greyscale=True,
 #                                          show_intersections=True)
 # boundary_visualizer.run_visualization()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -358,15 +358,15 @@
 00001650: 3230 7d2c 207b 3737 302c 2034 3336 7d7d  20}, {770, 436}}
 00001660: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e99  ...%1=I`myz{|}~.
 00001670: 0000 0000 0000 0101 0000 0000 0000 000f  ................
 00001680: 0000 0000 0000 0000 0000 0000 0000 009a  ................
 00001690: 0000 0005 0075 0074 0069 006c 0073 6473  .....u.t.i.l.sds
 000016a0: 636c 626f 6f6c 0000 0000 0500 7500 7400  clbool......u.t.
 000016b0: 6900 6c00 736c 6731 5363 6f6d 7000 0000  i.l.slg1Scomp...
-000016c0: 0000 00dd 1900 0000 0500 7500 7400 6900  ..........u.t.i.
+000016c0: 0000 00e3 b300 0000 0500 7500 7400 6900  ..........u.t.i.
 000016d0: 6c00 736c 7376 4362 6c6f 6200 0002 9762  l.slsvCblob....b
 000016e0: 706c 6973 7430 30d8 0102 0304 0506 0708  plist00.........
 000016f0: 090a 0b19 494a 0a4c 5f10 1276 6965 774f  ....IJ.L_..viewO
 00001700: 7074 696f 6e73 5665 7273 696f 6e5f 100f  ptionsVersion_..
 00001710: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
 00001720: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
 00001730: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
@@ -442,19 +442,19 @@
 00001b90: 0147 0148 014a 014b 0154 0156 0157 0159  .G.H.J.K.T.V.W.Y
 00001ba0: 015a 0163 0165 0166 0168 0169 0172 0174  .Z.c.e.f.h.i.r.t
 00001bb0: 0175 0177 0178 0181 0183 0184 0187 0188  .u.w.x..........
 00001bc0: 0191 0192 0193 0194 019d 01a2 01a3 0000  ................
 00001bd0: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
 00001be0: 0000 0000 0000 0000 0000 0000 01ac 0000  ................
 00001bf0: 0005 0075 0074 0069 006c 0073 6d6f 4444  ...u.t.i.l.smoDD
-00001c00: 626c 6f62 0000 0008 3da3 0784 abef c441  blob....=......A
+00001c00: 626c 6f62 0000 0008 99a4 30ee 36f0 c441  blob......0.6..A
 00001c10: 0000 0005 0075 0074 0069 006c 0073 6d6f  .....u.t.i.l.smo
-00001c20: 6444 626c 6f62 0000 0008 3da3 0784 abef  dDblob....=.....
+00001c20: 6444 626c 6f62 0000 0008 99a4 30ee 36f0  dDblob......0.6.
 00001c30: c441 0000 0005 0075 0074 0069 006c 0073  .A.....u.t.i.l.s
-00001c40: 7068 3153 636f 6d70 0000 0000 0001 1000  ph1Scomp........
+00001c40: 7068 3153 636f 6d70 0000 0000 0001 2000  ph1Scomp...... .
 00001c50: 0000 0005 0075 0074 0069 006c 0073 7653  .....u.t.i.l.svS
 00001c60: 726e 6c6f 6e67 0000 0001 0000 0000 0000  rnlong..........
 00001c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -509,53 +509,53 @@
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000 0000 0000 0000 0013 0000 000b  ................
 00002010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00002020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00002030: 0000 0041 2043 0000 000b 005f 005f 0070  ...A C....._._.p
+00002030: 0000 0041 2846 0000 000b 005f 005f 0070  ...A(F....._._.p
 00002040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00002050: 6d6f 4444 626c 6f62 0000 0008 2451 082e  moDDblob....$Q..
-00002060: 1af0 c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00002050: 6d6f 4444 626c 6f62 0000 0008 4eb5 f512  moDDblob....N...
+00002060: 6af0 c441 0000 000b 005f 005f 0070 0079  j..A....._._.p.y
 00002070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00002080: 6444 626c 6f62 0000 0008 2451 082e 1af0  dDblob....$Q....
+00002080: 6444 626c 6f62 0000 0008 4eb5 f512 6af0  dDblob....N...j.
 00002090: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000020a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000020b0: 636f 6d70 0000 0000 004f 0000 0000 0006  comp.....O......
+000020b0: 636f 6d70 0000 0000 004e f000 0000 0006  comp.....N......
 000020c0: 0061 0073 0073 0065 0074 0073 6277 7370  .a.s.s.e.t.sbwsp
 000020d0: 626c 6f62 0000 00c9 6270 6c69 7374 3030  blob....bplist00
 000020e0: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
 000020f0: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
 00002100: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
 00002110: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 00002120: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 00002130: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
 00002140: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00002150: 7208 0809 0809 5f10 187b 7b34 3134 2c20  r....._..{{414, 
-00002160: 3136 317d 2c20 7b37 3730 2c20 3433 367d  161}, {770, 436}
+00002150: 7208 0809 0809 5f10 187b 7b34 3334 2c20  r....._..{{434, 
+00002160: 3134 317d 2c20 7b37 3730 2c20 3433 367d  141}, {770, 436}
 00002170: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
 00002180: 9900 0000 0000 0001 0100 0000 0000 0000  ................
 00002190: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
 000021a0: 9a00 0000 0600 6100 7300 7300 6500 7400  ......a.s.s.e.t.
-000021b0: 736c 6731 5363 6f6d 7000 0000 0000 82d2  slg1Scomp.......
-000021c0: 0100 0000 0600 6100 7300 7300 6500 7400  ......a.s.s.e.t.
+000021b0: 736c 6731 5363 6f6d 7000 0000 0000 82d6  slg1Scomp.......
+000021c0: e500 0000 0600 6100 7300 7300 6500 7400  ......a.s.s.e.t.
 000021d0: 736c 7376 4362 6c6f 6200 0002 b062 706c  slsvCblob....bpl
 000021e0: 6973 7430 30da 0102 0304 0506 0708 090a  ist00...........
-000021f0: 0b0c 0d18 4849 484a 0c4c 5f10 1276 6965  ....HIHJ.L_..vie
+000021f0: 0b0c 0d18 4849 484a 4b0c 5f10 1276 6965  ....HIHJK._..vie
 00002200: 774f 7074 696f 6e73 5665 7273 696f 6e5f  wOptionsVersion_
 00002210: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
 00002220: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
 00002230: 756c 6174 6541 6c6c 5369 7a65 735f 100f  ulateAllSizes_..
 00002240: 7363 726f 6c6c 506f 7369 7469 6f6e 5958  scrollPositionYX
 00002250: 7465 7874 5369 7a65 5f10 0f73 6372 6f6c  textSize_..scrol
 00002260: 6c50 6f73 6974 696f 6e58 5a73 6f72 7443  lPositionXZsortC
-00002270: 6f6c 756d 6e5f 1010 7573 6552 656c 6174  olumn_..useRelat
-00002280: 6976 6544 6174 6573 5869 636f 6e53 697a  iveDatesXiconSiz
-00002290: 6510 0109 ab0e 171c 2125 2a2f 3439 3e43  e.......!%*/49>C
+00002270: 6f6c 756d 6e58 6963 6f6e 5369 7a65 5f10  olumnXiconSize_.
+00002280: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
+00002290: 7310 0109 ab0e 171c 2125 2a2f 3439 3e43  s.......!%*/49>C
 000022a0: d40f 1011 120c 140c 1657 7669 7369 626c  .........Wvisibl
 000022b0: 6555 7769 6474 6859 6173 6365 6e64 696e  eUwidthYascendin
 000022c0: 675a 6964 656e 7469 6669 6572 0911 0127  gZidentifier...'
 000022d0: 0954 6e61 6d65 d40f 1011 1218 1918 1b08  .Tname..........
 000022e0: 1023 0858 7562 6971 7569 7479 d40f 1011  .#.Xubiquity....
 000022f0: 120c 1e18 2009 10b5 085c 6461 7465 4d6f  .... ....\dateMo
 00002300: 6469 6669 6564 d40f 1011 1218 1e18 2408  dified........$.
@@ -566,40 +566,40 @@
 00002350: 6162 656c d40f 1011 1218 360c 3808 104b  abel......6.8..K
 00002360: 0957 7665 7273 696f 6ed4 0f10 1112 183b  .Wversion......;
 00002370: 0c3d 0811 012c 0958 636f 6d6d 656e 7473  .=...,.Xcomments
 00002380: d40f 1011 1218 4018 4208 10c8 085e 6461  ......@.B....^da
 00002390: 7465 4c61 7374 4f70 656e 6564 d40f 1011  teLastOpened....
 000023a0: 1218 1e18 4608 0859 6461 7465 4164 6465  ....F..YdateAdde
 000023b0: 6408 2300 0000 0000 0000 0023 4028 0000  d.#........#@(..
-000023c0: 0000 0000 546e 616d 6509 2340 3000 0000  ....Tname.#@0...
-000023d0: 0000 0000 0800 1d00 3200 4400 4c00 6000  ........2.D.L.`.
-000023e0: 7200 7b00 8d00 9800 ab00 b400 b600 b700  r.{.............
+000023c0: 0000 0000 546e 616d 6523 4030 0000 0000  ....Tname#@0....
+000023d0: 0000 0900 0800 1d00 3200 4400 4c00 6000  ........2.D.L.`.
+000023e0: 7200 7b00 8d00 9800 a100 b400 b600 b700  r.{.............
 000023f0: c300 cc00 d400 da00 e400 ef00 f000 f300  ................
 00002400: f400 f901 0201 0301 0501 0601 0f01 1801  ................
 00002410: 1901 1b01 1c01 2901 3201 3301 3401 4001  ......).2.3.4.@.
 00002420: 4901 4a01 4c01 4d01 5201 5b01 5c01 5e01  I.J.L.M.R.[.\.^.
 00002430: 5f01 6401 6d01 6e01 7001 7101 7701 8001  _.d.m.n.p.q.w...
 00002440: 8101 8301 8401 8c01 9501 9601 9901 9a01  ................
 00002450: a301 ac01 ad01 af01 b001 bf01 c801 c901  ................
-00002460: ca01 d401 d501 de01 e701 ec01 ed00 0000  ................
+00002460: ca01 d401 d501 de01 e701 ec01 f500 0000  ................
 00002470: 0000 0002 0100 0000 0000 0000 4d00 0000  ............M...
 00002480: 0000 0000 0000 0000 0000 0001 f600 0000  ................
 00002490: 0600 6100 7300 7300 6500 7400 736c 7376  ..a.s.s.e.t.slsv
 000024a0: 7062 6c6f 6200 0002 9562 706c 6973 7430  pblob....bplist0
 000024b0: 30da 0102 0304 0506 0708 090a 0b0c 0d1f  0...............
-000024c0: 4748 4749 0c4b 5f10 1276 6965 774f 7074  GHGI.K_..viewOpt
+000024c0: 4748 4749 4a0c 5f10 1276 6965 774f 7074  GHGIJ._..viewOpt
 000024d0: 696f 6e73 5665 7273 696f 6e5f 100f 7368  ionsVersion_..sh
 000024e0: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
 000024f0: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
 00002500: 6541 6c6c 5369 7a65 735f 100f 7363 726f  eAllSizes_..scro
 00002510: 6c6c 506f 7369 7469 6f6e 5958 7465 7874  llPositionYXtext
 00002520: 5369 7a65 5f10 0f73 6372 6f6c 6c50 6f73  Size_..scrollPos
 00002530: 6974 696f 6e58 5a73 6f72 7443 6f6c 756d  itionXZsortColum
-00002540: 6e5f 1010 7573 6552 656c 6174 6976 6544  n_..useRelativeD
-00002550: 6174 6573 5869 636f 6e53 697a 6510 0109  atesXiconSize...
+00002540: 6e58 6963 6f6e 5369 7a65 5f10 1075 7365  nXiconSize_..use
+00002550: 5265 6c61 7469 7665 4461 7465 7310 0109  RelativeDates...
 00002560: d90e 0f10 1112 1314 1516 1720 2529 2d32  ........... %)-2
 00002570: 373c 4158 636f 6d6d 656e 7473 5e64 6174  7<AXcomments^dat
 00002580: 654c 6173 744f 7065 6e65 645c 6461 7465  eLastOpened\date
 00002590: 4d6f 6469 6669 6564 5b64 6174 6543 7265  Modified[dateCre
 000025a0: 6174 6564 5473 697a 6555 6c61 6265 6c54  atedTsizeUlabelT
 000025b0: 6b69 6e64 5776 6572 7369 6f6e 546e 616d  kindWversionTnam
 000025c0: 65d4 1819 1a1b 1c1d 0c1f 5569 6e64 6578  e.........Uindex
@@ -609,34 +609,34 @@
 00002600: 191a 1b0b 261f 0c10 b508 09d4 1819 1a1b  ....&...........
 00002610: 2a26 1f1f 1002 0808 d418 191a 1b2e 2f1f  *&............/.
 00002620: 0c10 0310 6108 09d4 1819 1a1b 3334 0c1f  ....a.......34..
 00002630: 1005 1064 0908 d418 191a 1b38 390c 0c10  ...d.......89...
 00002640: 0410 7309 09d4 1819 1a1b 3d3e 0c1f 1006  ..s.......=>....
 00002650: 104b 0908 d418 191a 1b42 430c 0c10 0011  .K.......BC.....
 00002660: 0127 0909 0823 0000 0000 0000 0000 2340  .'...#........#@
-00002670: 2800 0000 0000 0054 6e61 6d65 0923 4030  (......Tname.#@0
-00002680: 0000 0000 0000 0008 001d 0032 0044 004c  ...........2.D.L
-00002690: 0060 0072 007b 008d 0098 00ab 00b4 00b6  .`.r.{..........
+00002670: 2800 0000 0000 0054 6e61 6d65 2340 3000  (......Tname#@0.
+00002680: 0000 0000 0009 0008 001d 0032 0044 004c  ...........2.D.L
+00002690: 0060 0072 007b 008d 0098 00a1 00b4 00b6  .`.r.{..........
 000026a0: 00b7 00ca 00d3 00e2 00ef 00fb 0100 0106  ................
 000026b0: 010b 0113 0118 0121 0127 012d 0137 013f  .......!.'.-.7.?
 000026c0: 0141 0144 0145 0146 014f 0151 0153 0154  .A.D.E.F.O.Q.S.T
 000026d0: 0155 015e 0160 0161 0162 016b 016d 016e  .U.^.`.a.b.k.m.n
 000026e0: 016f 0178 017a 017c 017d 017e 0187 0189  .o.x.z.|.}.~....
 000026f0: 018b 018c 018d 0196 0198 019a 019b 019c  ................
 00002700: 01a5 01a7 01a9 01aa 01ab 01b4 01b6 01b9  ................
-00002710: 01ba 01bb 01bc 01c5 01ce 01d3 01d4 0000  ................
+00002710: 01ba 01bb 01bc 01c5 01ce 01d3 01dc 0000  ................
 00002720: 0000 0000 0201 0000 0000 0000 004c 0000  .............L..
 00002730: 0000 0000 0000 0000 0000 0000 01dd 0000  ................
 00002740: 0006 0061 0073 0073 0065 0074 0073 6d6f  ...a.s.s.e.t.smo
 00002750: 4444 626c 6f62 0000 0008 cf95 8ce8 d0e1  DDblob..........
 00002760: c441 0000 0006 0061 0073 0073 0065 0074  .A.....a.s.s.e.t
 00002770: 0073 6d6f 6444 626c 6f62 0000 0008 cf95  .smodDblob......
 00002780: 8ce8 d0e1 c441 0000 0006 0061 0073 0073  .....A.....a.s.s
 00002790: 0065 0074 0073 7068 3153 636f 6d70 0000  .e.t.sph1Scomp..
-000027a0: 0000 0086 7000 0000 0006 0061 0073 0073  ....p......a.s.s
+000027a0: 0000 0086 8000 0000 0006 0061 0073 0073  ...........a.s.s
 000027b0: 0065 0074 0073 7653 726e 6c6f 6e67 0000  .e.t.svSrnlong..
 000027c0: 0001 0000 0014 0062 0061 0074 0063 0068  .......b.a.t.c.h
 000027d0: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
 000027e0: 005f 0076 0069 0064 0065 006f 0073 6277  ._.v.i.d.e.o.sbw
 000027f0: 7370 626c 6f62 0000 00ca 6270 6c69 7374  spblob....bplist
 00002800: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 00002810: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
@@ -965,15 +965,15 @@
 00003c40: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
 00003c50: 9b00 0000 1200 6600 6500 6100 7400 7500  ......f.e.a.t.u.
 00003c60: 7200 6500 5f00 6500 7800 7400 7200 6100  r.e._.e.x.t.r.a.
 00003c70: 6300 7400 6f00 7200 7364 7363 6c62 6f6f  c.t.o.r.sdsclboo
 00003c80: 6c00 0000 0012 0066 0065 0061 0074 0075  l......f.e.a.t.u
 00003c90: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
 00003ca0: 0063 0074 006f 0072 0073 6c67 3153 636f  .c.t.o.r.slg1Sco
-00003cb0: 6d70 0000 0000 0011 b6b2 0000 0012 0066  mp.............f
+00003cb0: 6d70 0000 0000 0011 bd05 0000 0012 0066  mp.............f
 00003cc0: 0065 0061 0074 0075 0072 0065 005f 0065  .e.a.t.u.r.e._.e
 00003cd0: 0078 0074 0072 0061 0063 0074 006f 0072  .x.t.r.a.c.t.o.r
 00003ce0: 0073 6c73 7643 626c 6f62 0000 02b8 6270  .slsvCblob....bp
 00003cf0: 6c69 7374 3030 da01 0203 0405 0607 0809  list00..........
 00003d00: 0a0b 0c0d 1a48 4948 4a4b 0c5f 1012 7669  .....HIHJK._..vi
 00003d10: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
 00003d20: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
@@ -1025,19 +1025,19 @@
 00004000: 0000 0000 0000 0000 0000 0015 0000 0012  ................
 00004010: 0066 0065 0061 0074 0075 0072 0065 005f  .f.e.a.t.u.r.e._
 00004020: 0065 0078 0074 0072 0061 0063 0074 006f  .e.x.t.r.a.c.t.o
 00004030: 0072 0073 6d6f 4444 626c 6f62 0000 0008  .r.smoDDblob....
 00004040: ef06 84b9 8aef c441 0000 0012 0066 0065  .......A.....f.e
 00004050: 0061 0074 0075 0072 0065 005f 0065 0078  .a.t.u.r.e._.e.x
 00004060: 0074 0072 0061 0063 0074 006f 0072 0073  .t.r.a.c.t.o.r.s
-00004070: 6d6f 6444 626c 6f62 0000 0008 8d23 5871  modDblob.....#Xq
-00004080: d5ee c441 0000 0012 0066 0065 0061 0074  ...A.....f.e.a.t
+00004070: 6d6f 6444 626c 6f62 0000 0008 ef06 84b9  modDblob........
+00004080: 8aef c441 0000 0012 0066 0065 0061 0074  ...A.....f.e.a.t
 00004090: 0075 0072 0065 005f 0065 0078 0074 0072  .u.r.e._.e.x.t.r
 000040a0: 0061 0063 0074 006f 0072 0073 7068 3153  .a.c.t.o.r.sph1S
-000040b0: 636f 6d70 0000 0000 0013 d000 0000 0012  comp............
+000040b0: 636f 6d70 0000 0000 0013 e000 0000 0012  comp............
 000040c0: 0066 0065 0061 0074 0075 0072 0065 005f  .f.e.a.t.u.r.e._
 000040d0: 0065 0078 0074 0072 0061 0063 0074 006f  .e.x.t.r.a.c.t.o
 000040e0: 0072 0073 7653 726e 6c6f 6e67 0000 0001  .r.svSrnlong....
 000040f0: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
 00004100: 6277 7370 626c 6f62 0000 00c9 6270 6c69  bwspblob....bpli
 00004110: 7374 3030 d701 0203 0405 0607 0808 0a08  st00............
 00004120: 0a0d 0a5d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
@@ -1049,21 +1049,21 @@
 00004180: 6465 6261 7208 0809 0809 5f10 187b 7b33  debar....._..{{3
 00004190: 3934 2c20 3138 317d 2c20 7b37 3730 2c20  94, 181}, {770, 
 000041a0: 3433 367d 7d09 0817 2531 3d49 606d 797a  436}}...%1=I`myz
 000041b0: 7b7c 7d7e 9900 0000 0000 0001 0100 0000  {|}~............
 000041c0: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
 000041d0: 0000 0000 9a00 0000 0600 6d00 6900 7800  ..........m.i.x.
 000041e0: 6900 6e00 736c 6731 5363 6f6d 7000 0000  i.n.slg1Scomp...
-000041f0: 0000 017f 5200 0000 0600 6d00 6900 7800  ....R.....m.i.x.
+000041f0: 0000 017f c400 0000 0600 6d00 6900 7800  ..........m.i.x.
 00004200: 6900 6e00 736d 6f44 4462 6c6f 6200 0000  i.n.smoDDblob...
-00004210: 082f 8ef9 7e86 efc4 4100 0000 0600 6d00  ./..~...A.....m.
+00004210: 08a1 1c42 882c f0c4 4100 0000 0600 6d00  ...B.,..A.....m.
 00004220: 6900 7800 6900 6e00 736d 6f64 4462 6c6f  i.x.i.n.smodDblo
-00004230: 6200 0000 08e6 8907 31f3 eec4 4100 0000  b.......1...A...
+00004230: 6200 0000 08ec 3b8b 3426 f0c4 4100 0000  b.....;.4&..A...
 00004240: 0600 6d00 6900 7800 6900 6e00 7370 6831  ..m.i.x.i.n.sph1
-00004250: 5363 6f6d 7000 0000 0000 01b0 0000 0000  Scomp...........
+00004250: 5363 6f6d 7000 0000 0000 01c0 0000 0000  Scomp...........
 00004260: 0600 6d00 6900 7800 6900 6e00 7376 5372  ..m.i.x.i.n.svSr
 00004270: 6e6c 6f6e 6700 0000 0100 0000 0d00 6f00  nlong.........o.
 00004280: 7500 7400 6c00 6900 6500 7200 5f00 7400  u.t.l.i.e.r._.t.
 00004290: 6f00 6f00 6c00 7362 7773 7062 6c6f 6200  o.o.l.sbwspblob.
 000042a0: 0000 c962 706c 6973 7430 30d7 0102 0304  ...bplist00.....
 000042b0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
 000042c0: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from simba.read_config_unit_tests import (insert_default_headers_for_feature_extraction)
 import os
 from simba.feature_extractors.unit_tests import (read_video_info)
-from simba.misc_tools import get_feature_extraction_headers
+from simba.misc_tools import get_feature_extraction_headers, stdout_success
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df, save_df
 import pandas as pd
 from copy import deepcopy
 from scipy.spatial import ConvexHull
 import scipy
 import numpy as np
@@ -443,15 +443,15 @@
             save_df(self.out_data, self.file_type, save_path)
             session_time, file_time = session_time + (time.time() - file_start_time), int(time.time() - file_start_time)
             print('Feature extraction complete for {} ({}/{} (elapsed time: {}s)...'.format(self.video_name,
                                                                                              str(file_cnt + 1),
                                                                                              str(len(self.files_found)),
                                                                                              str(file_time)))
 
-        print('SIMBA COMPLETE: All features extracted (elapsed time: {}s). Results stored in project_folder/csv/features_extracted directory'.format(str(int(session_time))))
+        stdout_success(msg='All features extracted. Results stored in project_folder/csv/features_extracted directory', elapsed_time=str(int(session_time)))
 
 # test = ExtractFeaturesFrom14bps(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
 # test.extract_features()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os, glob
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.read_config_unit_tests import insert_default_headers_for_feature_extraction
-from simba.misc_tools import get_feature_extraction_headers
+from simba.misc_tools import get_feature_extraction_headers, stdout_success
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df, save_df
 import pandas as pd
 import numpy as np
 from copy import deepcopy
 import math
 from scipy.spatial import ConvexHull
@@ -248,15 +248,17 @@
             self.out_data = pd.concat([self.out_data, results], axis=1)
 
             self.out_data = self.out_data.reset_index(drop=True).fillna(0)
             save_path = os.path.join(self.save_dir, self.video_name + '.' + self.file_type)
             save_df(self.out_data, self.file_type, save_path)
 
             print('Feature extraction complete for {} ({}/{})...'.format(self.video_name, str(file_cnt + 1),str(len(self.files_found))))
-        print('SIMBA COMPLETE: All features extracted. Results are stored in the project_folder/csv/features_extracted directory')
+        stdout_success(msg='All features extracted. Results are stored in the project_folder/csv/features_extracted directory')
+
+
 
 # test = ExtractFeaturesFrom7bps(config_path='/Users/simon/Desktop/train_model_project/project_folder/project_config.ini')
 # test.extract_features()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/fish_feature_extractor_2023.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/fish_feature_extractor_2023.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from simba.read_config_unit_tests import (insert_default_headers_for_feature_extraction)
-from simba.misc_tools import get_feature_extraction_headers
+from simba.misc_tools import get_feature_extraction_headers, stdout_success
 import os
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df, save_df
 import pandas as pd
 import numpy as np
 from copy import deepcopy
@@ -70,15 +70,14 @@
             self.out_data = deepcopy(self.in_data)
             mouse_1_ar = np.reshape(self.out_data[self.mouse_1_headers].values, (len(self.out_data / 2), -1, 2))
             self.out_data['Mouse_1_poly_area'] = jitted_hull(points=mouse_1_ar, target=Formats.PERIMETER.value) / self.px_per_mm
             mouse_2_ar = np.reshape(self.out_data[self.mouse_2_headers].values, (len(self.out_data / 2), -1, 2))
             self.out_data['Mouse_2_poly_area'] = jitted_hull(points=mouse_2_ar, target=Formats.PERIMETER.value) / self.px_per_mm
             self.in_data_shifted = self.out_data.shift(periods=1).add_suffix('_shifted').fillna(0)
             self.in_data = pd.concat([self.in_data, self.in_data_shifted], axis=1, join='inner').fillna(0).reset_index(drop=True)
-            print(self.out_data.columns)
             self.out_data['Mouse_1_nose_to_tail'] = self.euclidean_distance(self.out_data['Nose_1_x'].values, self.out_data['Tail_base_1_x'].values, self.out_data['Nose_1_y'].values, self.out_data['Tail_base_1_y'].values, self.px_per_mm)
             self.out_data['Mouse_2_nose_to_tail'] = self.euclidean_distance(self.out_data['Nose_2_x'].values, self.out_data['Tail_base_2_x'].values, self.out_data['Nose_2_y'].values, self.out_data['Tail_base_2_y'].values, self.px_per_mm)
             self.out_data['Mouse_1_Ear_distance'] = self.euclidean_distance(self.out_data['Ear_left_1_x'].values, self.out_data['Ear_right_1_x'].values, self.out_data['Ear_left_1_y'].values, self.out_data['Ear_right_1_y'].values, self.px_per_mm)
             self.out_data['Mouse_2_Ear_distance'] = self.euclidean_distance(self.out_data['Ear_left_2_x'].values, self.out_data['Ear_right_2_x'].values, self.out_data['Ear_left_2_y'].values, self.out_data['Ear_right_2_y'].values, self.px_per_mm)
             self.out_data['Nose_to_nose_distance'] = self.euclidean_distance(self.out_data['Nose_2_x'].values, self.out_data['Nose_1_x'].values, self.out_data['Nose_2_y'].values, self.out_data['Nose_1_y'].values, self.px_per_mm)
             self.out_data['Movement_mouse_1_nose'] = self.euclidean_distance(self.in_data['Nose_1_x_shifted'].values, self.in_data['Nose_1_x'].values, self.in_data['Nose_1_y_shifted'].values, self.in_data['Nose_1_y'].values, self.px_per_mm)
             self.out_data['Movement_mouse_2_nose'] = self.euclidean_distance(self.in_data['Nose_2_x_shifted'].values, self.in_data['Nose_2_x'].values, self.in_data['Nose_2_y_shifted'].values, self.in_data['Nose_2_y'].values, self.px_per_mm)
@@ -325,11 +324,11 @@
             self.out_data = pd.concat([self.out_data, results], axis=1)
             self.out_data = self.out_data.reset_index(drop=True).fillna(0)
             save_path = os.path.join(self.save_dir, self.video_name + '.' + self.file_type)
             save_df(self.out_data, self.file_type, save_path)
             session_time, file_time = session_time + (time.time()-file_start_time), int(time.time() - file_start_time)
             print('Feature extraction complete for {} ({}/{} (elapsed time: {}s))...'.format(self.video_name, str(file_cnt + 1), str(len(self.files_found)), str(file_time)))
 
-        print('SIMBA COMPLETE: All features extracted (elapsed time: {}s). Results stored in project_folder/csv/features_extracted directory'.format(str(int(session_time))))
+        stdout_success(msg='All features extracted. Results stored in project_folder/csv/features_extracted directory.', elapsed_time=str(int(session_time)))
 
 # test = ExtractFeaturesFrom8bps2Animals(config_path='/Users/simon/Desktop/envs/troubleshooting/8Bp_2_animals/project_folder/project_config.ini')
 # test.extract_features()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -276,18 +276,18 @@
 00001130: 5f10 197b 7b34 3732 2c20 3134 327d 2c20  _..{{472, 142}, 
 00001140: 7b31 3037 362c 2036 3231 7d7d 0908 1725  {1076, 621}}...%
 00001150: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
 00001160: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 00001170: 0000 0000 0000 0000 0000 009b 0000 000b  ................
 00001180: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001190: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-000011a0: 0000 000b dd5c 0000 000b 005f 005f 0070  .....\....._._.p
+000011a0: 0000 000b e0fe 0000 000b 005f 005f 0070  ..........._._.p
 000011b0: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-000011c0: 6d6f 4444 626c 6f62 0000 0008 41e2 0579  moDDblob....A..y
-000011d0: d5ee c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+000011c0: 6d6f 4444 626c 6f62 0000 0008 ab3a 61c1  moDDblob.....:a.
+000011d0: 8aef c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 000011e0: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
 000011f0: 6444 626c 6f62 0000 0008 41e2 0579 d5ee  dDblob....A..y..
 00001200: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 00001210: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 00001220: 636f 6d70 0000 0000 000c 9000 0000 000b  comp............
 00001230: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001240: 0065 005f 005f 7653 726e 6c6f 6e67 0000  .e._._vSrnlong..
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/feature_subsets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
-from simba.misc_tools import check_if_filepath_list_is_empty
+from simba.misc_tools import check_if_filepath_list_is_empty, stdout_success
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.misc_tools import get_fn_ext, SimbaTimer
 from simba.rw_dfs import read_df
 import os
 import numpy as np
 from itertools import combinations
 from simba.feature_extractors.perimeter_jit import jitted_hull
@@ -62,16 +62,15 @@
             elif self.feature_family == 'Frame-by-frame body-parts inside ROIs (Boolean)':
                 self.calc_inside_roi()
 
             self.__save()
             self.video_timer.stop_timer()
             print(f'Video {self.video_name} complete (elapsed time {self.video_timer.elapsed_time_str}s)...')
         self.timer.stop_timer()
-        print(f'SIMBA COMPLETE: {self.feature_family} for {str(len(self.outlier_corrected_paths))} videos saved in {self.save_dir} (elapsed time: {self.timer.elapsed_time_str}s')
-
+        stdout_success(msg=f'{self.feature_family} for {str(len(self.outlier_corrected_paths))} videos saved in {self.save_dir}', elapsed_time=self.timer.elapsed_time_str)
 
     def calc_distances(self):
         for c in self.two_point_combs:
             col_names = list(sum([(x + '_x', y + '_y') for (x, y) in zip(c, c)], ()))
 
             self.results[f'Distance (mm) {c[0]}-{c[1]}'] = self.euclidean_distance(self.df[col_names[0]].values,
                                                                               self.df[col_names[2]].values,
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/extract_features_9bp.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/extract_features_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from simba.misc_tools import get_fn_ext
-from simba.misc_tools import SimbaTimer
+from simba.misc_tools import (get_fn_ext,
+                              SimbaTimer,
+                              stdout_success)
 from simba.read_config_unit_tests import check_str
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.rw_dfs import (read_df,
                           save_df)
 import os
 import pandas as pd
 import numpy as np
@@ -128,11 +129,11 @@
             self.data_df = self.data_df.reset_index(drop=True).fillna(0)
             save_df(self.data_df, self.file_type, save_path)
             video_timer.stop_timer()
             print('Saving features for video {}...'.format(file_name))
             print('Feature extraction complete for video {} (elapsed time: {}s)'.format(file_name, video_timer.elapsed_time_str))
 
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: Feature extraction complete for {} video(s). Results are saved inside the project_folder/csv/features_extracted director (elapsed time: {}s).'.format(len(self.files_found), self.timer.elapsed_time_str))
+        stdout_success(f'Feature extraction complete for {str(len(self.files_found))} video(s). Results are saved inside the project_folder/csv/features_extracted directory', elapsed_time=self.timer.elapsed_time_str)
 
 # test = UserDefinedFeatureExtractor(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
 # test.extract_features()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/unit_tests.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from simba.read_config_unit_tests import insert_default_headers_for_feature_extraction
 import os
 from simba.feature_extractors.unit_tests import read_video_info
-from simba.misc_tools import get_feature_extraction_headers
+from simba.misc_tools import get_feature_extraction_headers, stdout_success
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df, save_df
 import pandas as pd
 import numpy as np
 from copy import deepcopy
 import math
 from scipy.spatial import ConvexHull
@@ -475,11 +475,11 @@
             self.out_data = pd.concat([self.out_data, results], axis=1)
             self.out_data = self.out_data.reset_index(drop=True).fillna(0)
             save_path = os.path.join(self.save_dir, self.video_name + '.' + self.file_type)
             save_df(self.out_data, self.file_type, save_path)
             session_time, file_time = session_time + (time.time()-file_start_time), int(time.time() - file_start_time)
             print('Feature extraction complete for {} ({}/{} (elapsed time: {}s)...'.format(self.video_name, str(file_cnt + 1), str(len(self.files_found)), str(file_time)))
 
-        print('SIMBA COMPLETE: All features extracted (elapsed time: {}s). Results stored in project_folder/csv/features_extracted directory'.format(str(int(session_time))))
+        stdout_success(msg='All features extracted. Results stored in project_folder/csv/features_extracted directory', elapsed_time=str(int(session_time)))
 
 # test = ExtractFeaturesFrom16bps(config_path='/Users/simon/Desktop/envs/troubleshooting/two_animals_16bp_032023/project_folder/project_config.ini')
 # test.extract_features()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import os, glob
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.read_config_unit_tests import insert_default_headers_for_feature_extraction
-from simba.misc_tools import get_feature_extraction_headers
+from simba.misc_tools import get_feature_extraction_headers, stdout_success
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df, save_df
 import numpy as np
 import pandas as pd
 from copy import deepcopy
 import math
 from scipy.spatial import ConvexHull
 import scipy
 from collections import defaultdict
-from simba.enums import Formats
 import time
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.feature_extractors.perimeter_jit import jitted_hull
 
 
 class ExtractFeaturesFrom8bps(FeatureExtractionMixin):
     """
@@ -277,11 +276,11 @@
 
             self.out_data = self.out_data.reset_index(drop=True).fillna(0)
             save_path = os.path.join(self.save_dir, self.video_name + '.' + self.file_type)
             save_df(self.out_data, self.file_type, save_path)
             session_time, file_time = session_time + (time.time() - file_start_time), int(time.time() - file_start_time)
             print('Feature extraction complete for {} ({}/{} (elapsed time: {}s)...'.format(self.video_name, str(file_cnt + 1), str(len(self.files_found)), str(file_time)))
 
-        print('SIMBA COMPLETE: All features extracted (elapsed time: {}s). Results stored in project_folder/csv/features_extracted directory'.format(str(int(session_time))))
+        stdout_success(msg='All features extracted. Results stored in project_folder/csv/features_extracted directory', elapsed_time=str(int(session_time)))
 #
 # test = ExtractFeaturesFrom8bps(config_path='/Users/simon/Desktop/envs/troubleshooting/one_black_animal/project_folder/project_config.ini')
 # test.extract_features()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.read_config_unit_tests import insert_default_headers_for_feature_extraction
-from simba.misc_tools import get_feature_extraction_headers
+from simba.misc_tools import get_feature_extraction_headers, stdout_success
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df, save_df
 import pandas as pd
 import numpy as np
 from copy import deepcopy
 import math
 from collections import defaultdict
@@ -212,15 +212,15 @@
 
             self.out_data = self.out_data.reset_index(drop=True).fillna(0)
             save_path = os.path.join(self.save_dir, self.video_name + '.' + self.file_type)
             save_df(self.out_data, self.file_type, save_path)
 
             print('Feature extraction complete for {} ({}/{})...'.format(self.video_name, str(file_cnt + 1), str(len(self.files_found))))
 
-        print('SIMBA COMPLETE: All features extracted. Results are stored in the project_folder/csv/features_extracted directory')
+        stdout_success(msg='All features extracted. Results are stored in the project_folder/csv/features_extracted directory')
 
 # test = ExtractFeaturesFrom4bps(config_path='/Users/simon/Desktop/train_model_project/project_folder/project_config.ini')
 # test.extract_features()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.55.7/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotly_create_h5.py` & `Simba-UW-tf-dev-1.55.7/simba/plotly_create_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/requirements.txt` & `Simba-UW-tf-dev-1.55.7/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/severity_processor.py` & `Simba-UW-tf-dev-1.55.7/simba/severity_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,16 @@
                                           check_if_filepath_list_is_empty)
 from datetime import datetime
 from numba import jit
 from simba.drop_bp_cords import getBpNames, create_body_part_dictionary
 from simba.enums import ReadConfig, Dtypes, Paths
 from simba.misc_tools import (check_multi_animal_status,
                               get_fn_ext,
-                              SimbaTimer)
+                              SimbaTimer,
+                              stdout_success)
 
 
 class SeverityProcessor(object):
     """
     Class for analyzing the `severity` of classification frame events based on how much
     the animals are moving. Frames are scored as less or more severe at lower and higher movements.
 
@@ -102,8 +103,8 @@
     def save(self):
         out_df = pd.DataFrame(columns=['VIDEO', 'MEASUREMENT', 'VALUE'])
         for video_name, video_data in self.results.items():
             for grade, grade_data in video_data.items():
                 out_df.loc[len(out_df)] = [video_name, grade, grade_data]
         out_df.to_csv(self.save_path)
         self.timer.stop_timer()
-        print(f'SIMBA COMPLETE: Severity data saved at {self.save_path} (elapsed time {self.timer.elapsed_time_str}s)')
+        stdout_success(msg=f'Severity data saved at {self.save_path}', elapsed_time=self.timer.elapsed_time_str)
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/user_pose_config_creator.py` & `Simba-UW-tf-dev-1.55.7/simba/user_pose_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.55.7/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.55.7/simba/mixins/config_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
                                           read_config_entry)
 from simba.feature_extractors.unit_tests import read_video_info_csv
 from simba.drop_bp_cords import createColorListofList
 from simba.misc_tools import SimbaTimer, find_core_cnt, check_multi_animal_status
 from simba.train_model_functions import get_all_clf_names
 from simba.drop_bp_cords import getBpNames, create_body_part_dictionary, getBpHeaders
 from simba.utils.errors import NoROIDataError
+from simba.utils.lookups import get_emojis
 import os, glob
 import pandas as pd
 import itertools
 import cv2
-import numpy as np
 from simba.enums import Paths, ReadConfig, Dtypes, Defaults, Keys
 from datetime import datetime
 
 class ConfigReader(object):
     def __init__(self,
                  config_path: str,
                  read_video_info: bool=True):
@@ -66,18 +66,18 @@
         self.x_cols, self.y_cols, self.p_cols = getBpNames(config_path)
         self.column_headers = getBpHeaders(config_path)
         self.multiprocess_chunksize = Defaults.CHUNK_SIZE.value
         self.maxtasksperchild = Defaults.MAX_TASK_PER_CHILD.value
         self.clr_lst = createColorListofList(self.animal_cnt, int(len(self.x_cols)/self.animal_cnt) + 1)
         self.animal_bp_dict = create_body_part_dictionary(self.multi_animal_status, self.multi_animal_id_list, self.animal_cnt, self.x_cols, self.y_cols, self.p_cols, [])
         self.project_bps = list(set([x[:-2] for x in self.column_headers]))
+        self.emojis = get_emojis()
         if read_video_info:
             self.video_info_df = read_video_info_csv(os.path.join(self.project_path, Paths.VIDEO_INFO.value))
 
-
     def read_roi_data(self):
         """
         Method to read in ROI definitions from SimBA project
 
         Returns
         -------
         roi_df: dict
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.55.7/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/machine_model_settings_pop_up.py` & `Simba-UW-tf-dev-1.55.7/simba/machine_model_settings_pop_up.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,16 @@
                                      FileSelect,
                                      Entry_Box)
 import pandas as pd
 import os, ast
 from simba.enums import ReadConfig, Options, Formats, Keys, Links
 from simba.train_model_functions import get_all_clf_names
 from simba.misc_tools import (find_files_of_filetypes_in_directory,
-                              get_fn_ext)
+                              get_fn_ext,
+                              stdout_success)
 from simba.tkinter_functions import CreateLabelFrameWithIcon
 from simba.utils.errors import InvalidHyperparametersFileError
 from simba.mixins.pop_up_mixin import PopUpMixin
 import webbrowser
 from tkinter import *
 from tkinter import ttk
 
@@ -301,15 +302,16 @@
         self.config.set('create ensemble settings', 'shap_save_iteration', str(self.shap_save_it))
         self.config.set('create ensemble settings', 'partial_dependency', str(self.partial_dependency))
         self.config.set('create ensemble settings', 'class_weights', str(self.class_weight_method))
         self.config.set('create ensemble settings', 'custom_weights', str(self.class_custom_weights))
 
         with open(self.config_path, 'w') as f:
             self.config.write(f)
-        print('SIMBA COMPLETE: Global model settings saved in the project_folder/project_config.ini')
+
+        stdout_success(msg='Global model settings saved in the project_folder/project_config.ini')
 
     def save_config(self):
         self.__checks()
         self.__get_variables()
 
         meta = {'RF_n_estimators': self.n_estimators,
                 'RF_max_features': self.max_features,
@@ -342,15 +344,15 @@
 
         meta_df = pd.DataFrame(meta, index=[0])
         meta_df.insert(0, 'Classifier_name', self.behavior_name)
         self.find_meta_file_cnt()
         file_name = '{}_meta_{}.csv'.format(self.behavior_name, str(self.meta_file_cnt))
         save_path = os.path.join(self.configs_path, file_name)
         meta_df.to_csv(save_path, index=FALSE)
-        print(f'SIMBA COMPLETE: Hyper-parameter config ({str(len(self.total_meta_files)+1)} saved in project_folder/configs folder.')
+        stdout_success(msg=f'Hyper-parameter config ({str(len(self.total_meta_files)+1)} saved in project_folder/configs folder.')
 
     def clear_cache(self):
         self.behavior_name = self.behavior_name_dropdown.getChoices()
         self.find_meta_file_cnt()
         for file_path in self.total_meta_files:
             os.remove(os.path.join(file_path))
             print('Deleted hyperparameters config {} ...'.format(file_path))
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/remove_keypoints_in_pose.py` & `Simba-UW-tf-dev-1.55.7/simba/remove_keypoints_in_pose.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import glob, os
 import pandas as pd
 from datetime import datetime
 import warnings
 from tables import NaturalNameWarning
-from simba.misc_tools import SimbaTimer
+from simba.misc_tools import SimbaTimer, stdout_success
 from simba.read_config_unit_tests import check_if_filepath_list_is_empty
 from simba.utils.errors import NotDirectoryError
 warnings.filterwarnings('ignore', category=NaturalNameWarning)
 
 class KeypointRemover(object):
     """
     Class for removing pose-estimated keypoints from data in CSV or H5 format.
@@ -94,8 +94,8 @@
                                 self.df = self.df.drop((first_header_value, animal_name, body_part, cord), axis=1)
                             except:
                                 print('SIMBA ERROR: Could not find body part {} in {}'.format(body_part, file_path))
                                 raise ValueError
                     self.df.to_hdf(save_path, key='re-organized', format='table', mode='w')
                 print('Saved {}, Video {}/{}.'.format(os.path.basename(file_path), str(file_cnt + 1), str(len(self.files_found))))
             self.timer.stop_timer()
-            print('SIMBA COMPLETE: {} new data with {} body-parts removed saved in {} directory (elapsed time {}s)'.format(str(len(self.files_found)), str(len(bp_to_remove_list)), save_directory, self.timer.elapsed_time_str))
+            stdout_success(msg=f'{str(len(self.files_found))} new data with {str(len(bp_to_remove_list))} body-parts removed saved in {save_directory} directory', elapsed_time=self.timer.elapsed_time_str)
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.55.7/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 __author__ = "Simon Nilsson"
 
 from simba.rw_dfs import read_df, save_df
 import os, glob
 from copy import deepcopy
 import pandas as pd
-from simba.misc_tools import get_fn_ext
+from simba.misc_tools import (get_fn_ext,
+                              stdout_success)
 from simba.read_config_unit_tests import (check_if_filepath_list_is_empty,
                                           check_if_dir_exists)
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.mixins.config_reader import ConfigReader
 
 class DeepEthogramImporter(ConfigReader):
 
@@ -95,12 +96,12 @@
             for clf_name in self.clf_names:
                 self.out_data[clf_name] = self.annotations_df[clf_name]
 
             save_path = os.path.join(self.targets_folder, video_name + '.' + self.file_type)
             save_df(df=self.out_data, file_type=self.file_type, save_path=save_path)
             print('DeepEthogram annotation for video {} saved...'.format(video_name))
 
-        print('SIMBA COMPLETE: Annotations for {} behaviors added to {} videos and saved in the project_folder/csv/targets_inserted directory.'.format(len(list(self.clf_names)), len(self.matches_dict.keys())))
+        stdout_success(msg=f'Annotations for {str(len(list(self.clf_names)))} behaviors added to {len(self.matches_dict.keys())} videos and saved in the project_folder/csv/targets_inserted directory.')
 
 # test = DeepEthogramImporter(deep_ethogram_dir='/Users/simon/Desktop/troubleshooting/deepethnogram/deepethnogram',
 #                             config_path='/Users/simon/Desktop/troubleshooting/deepethnogram/project_folder/project_config.ini')
 # test.import_deepethogram()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.55.7/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __author__ = "Simon Nilsson"
 
 from simba.read_config_unit_tests import (check_if_dir_exists,
                                           check_if_filepath_list_is_empty)
 from simba.mixins.config_reader import ConfigReader
 import os, glob
 from simba.rw_dfs import read_df, save_df
-from simba.misc_tools import get_fn_ext
+from simba.misc_tools import (get_fn_ext, stdout_success)
 from simba.utils.errors import (ThirdPartyAnnotationOverlapError,
                                 ThirdPartyAnnotationEventCountError)
 from simba.utils.warnings import ThirdPartyAnnotationsOutsidePoseEstimationDataWarning
 import pandas as pd
 from copy import deepcopy
 
 class BorisAppender(ConfigReader):
@@ -137,15 +137,15 @@
                                                                           first_error_frm=idx_difference[0],
                                                                           ambiguous_cnt=len(idx_difference))
                     annotations_idx = [x for x in annotations_idx if x not in idx_difference]
                 self.out_df[clf] = 0
                 self.out_df.loc[annotations_idx, clf] = 1
             self.__save_boris_annotations()
         self.timer.stop_timer()
-        print(f'SIMBA COMPLETE: BORIS annotations appended to dataset and saved in project_folder/csv/targets_inserted directory (elapsed time: {self.timer.elapsed_time_str}s).')
+        stdout_success(msg='BORIS annotations appended to dataset and saved in project_folder/csv/targets_inserted directory', elapsed_time=self.timer.elapsed_time_str)
 
     def __save_boris_annotations(self):
         save_path = os.path.join(self.targets_folder, self.video_name + '.' + self.file_type)
         save_df(self.out_df, self.file_type, save_path)
         print('Saved BORIS annotations for video {}...'.format(self.video_name))
 
 # test = BorisAppender(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.55.7/simba/third_party_label_appenders/observer_importer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from simba.mixins.config_reader import ConfigReader
 from simba.read_config_unit_tests import check_if_filepath_list_is_empty
 import os, glob
 import numpy as np
 from simba.misc_tools import (get_fn_ext,
-                              SimbaTimer)
+                              SimbaTimer,
+                              stdout_success)
 from simba.rw_dfs import read_df, save_df
 from simba.utils.errors import (ColumnNotFoundError,
                                 AnnotationFileNotFoundError,
                                 ThirdPartyAnnotationEventCountError,
                                 ThirdPartyAnnotationOverlapError)
 from simba.utils.warnings import (ThirdPartyAnnotationsClfMissingWarning,
                                   ThirdPartyAnnotationsOutsidePoseEstimationDataWarning)
@@ -142,15 +143,15 @@
                     annot_idx = [x for x in annot_idx if x not in idx_diff]
                 output_df[clf_name] = 0
                 output_df.loc[annot_idx, clf_name] = 1
             self.__save(df=output_df, path= os.path.join(self.targets_folder, file_name + '.' + self.file_type))
             video_timer.stop_timer()
             print(f'Imported Noldus Observer annotations for video {file_name} (elapsed time {video_timer.elapsed_time_str}s)...')
         self.timer.stop_timer()
-        print(f'SIMBA COMPLETE: Imported annotations saved in project/folder/csv/targets_inserted directory (elapsed time {self.timer.elapsed_time_str}s).')
+        stdout_success(msg=f'Imported annotations saved in project/folder/csv/targets_inserted directory', elapsed_time=self.timer.elapsed_time_str)
 
     def __save(self, df: pd.DataFrame, path: str):
         save_df(df=df, file_type=self.file_type, save_path=path)
 
 # test = NoldusObserverImporter(config_path='/Users/simon/Desktop/envs/troubleshooting/Gosia/project_folder/project_config.ini',
 #                               data_dir='/Users/simon/Desktop/envs/troubleshooting/Gosia/source/behaviours/Exp_38')
 # test.run()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.55.7/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.55.7/simba/third_party_label_appenders/third_party_appender.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 
 from simba.mixins.config_reader import ConfigReader
 from simba.read_config_unit_tests import (check_if_dir_exists,
                                           check_if_filepath_list_is_empty)
 from simba.rw_dfs import read_df, save_df
-from simba.misc_tools import (get_fn_ext, create_logger)
+from simba.misc_tools import (get_fn_ext, create_logger, stdout_success)
 from simba.third_party_label_appenders.tools import (read_boris_annotation_files,
                                                      read_deepethogram_files,
                                                      read_ethovision_files,
                                                      read_observer_files,
                                                      read_solomon_files,
                                                      read_bento_files,
                                                      fix_uneven_start_stop_count,
@@ -228,15 +228,15 @@
                 annot_idx = [x for x in annot_idx if x not in idx_diff]
                 out_df[clf] = 0
                 out_df.loc[annot_idx, clf] = 1
             save_path = os.path.join(self.targets_folder, self.video_name + '.' + self.file_type)
             save_df(out_df, self.file_type, save_path)
             print(f'Saved {self.app} annotations for video {self.video_name}...')
         self.timer.stop_timer()
-        print(f'SIMBA COMPLETE: {self.app} annotations appended to dataset and saved in project_folder/csv/targets_inserted directory (elapsed time: {self.timer.elapsed_time_str}s).')
+        stdout_success(msg=f'{self.app} annotations appended to dataset and saved in project_folder/csv/targets_inserted directory', elapsed_time=self.timer.elapsed_time_str)
 
 # settings = {'log': True,  'file_format': 'xlsx', 'errors': {'INVALID annotations file data format': 'WARNING',
 #                                                            'ADDITIONAL third-party behavior detected': 'NONE',
 #                                                            'Annotations EVENT COUNT conflict': 'WARNING',
 #                                                            'Annotations OVERLAP inaccuracy': 'WARNING',
 #                                                            'ZERO third-party video behavior annotations found': 'WARNING',
 #                                                            'Annotations and pose FRAME COUNT conflict': 'WARNING',
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.55.7/simba/third_party_label_appenders/ethovision_import.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import pandas as pd
 from simba.rw_dfs import read_df, save_df
 from simba.read_config_unit_tests import (read_config_file,
                                           check_if_filepath_list_is_empty,
                                           check_that_column_exist)
 from simba.feature_extractors.unit_tests import read_video_info
-from simba.misc_tools import SimbaTimer, get_fn_ext
+from simba.misc_tools import get_fn_ext, stdout_success
 from simba.mixins.config_reader import ConfigReader
 
 
 class ImportEthovision(ConfigReader):
     """
     Class for appending ETHOVISION human annotations onto featurized pose-estimation data.
     Results are saved within the project_folder/csv/targets_inserted directory of
@@ -46,15 +46,15 @@
         self.files_found = glob.glob(folder_path + '/*.xlsx') + glob.glob(folder_path + '/*.xls')
         self.files_found = [x for x in self.files_found if '~$' not in x]
         check_if_filepath_list_is_empty(filepaths=self.files_found,
                                         error_msg='SIMBA ERROR: No ETHOVISION xlsx or xls files found in {}'.format(str(folder_path)))
         self.processed_videos = []
         self.__read_files()
         self.timer.stop_timer()
-        print('All Ethovision annotations added. Files with annotation are located in the project_folder/csv/targets_inserted directory (elapsed time: {}s)'.format(self.timer.elapsed_time_str))
+        stdout_success(msg='All Ethovision annotations added. Files with annotation are located in the project_folder/csv/targets_inserted directory', elapsed_time=self.timer.elapsed_time_str)
 
     def __read_files(self):
         for file_path in self.files_found:
             ethovision_df = pd.read_excel(file_path, sheet_name=None)
             manual_scoring_sheet_name = list(ethovision_df.keys())[-1]
             ethovision_df = pd.read_excel(file_path, sheet_name=manual_scoring_sheet_name, index_col=0, header=None)
             try:
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.55.7/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __author__ = "Simon Nilsson"
 
 
 import os, glob
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.read_config_unit_tests import check_if_filepath_list_is_empty
 from simba.mixins.config_reader import ConfigReader
-from simba.misc_tools import get_fn_ext
+from simba.misc_tools import get_fn_ext, stdout_success
 from simba.rw_dfs import read_df, save_df
 from simba.utils.warnings import (ThirdPartyAnnotationsOutsidePoseEstimationDataWarning,
                                   ThirdPartyAnnotationsClfMissingWarning,
                                   ThirdPartyAnnotationsAdditionalClfWarning)
 from simba.utils.errors import AnnotationFileNotFoundError
 import pandas as pd
 from copy import deepcopy
@@ -100,15 +100,15 @@
                                                                           frm_cnt=len(feature_df),
                                                                           first_error_frm=annotations_idx_outside_video[0],
                                                                           ambiguous_cnt=len(annotations_idx_outside_video))
                 if len(valid_annotation_ids) > 0:
                     print(f'Appending {str(len(valid_annotation_ids))} {clf_name} frame annotations to video {self.video_name}...')
                     self.results_df.loc[valid_annotation_ids, clf_name] = 1
             self.__save()
-        print(f'SIMBA COMPLETE: Annotations for {str(len(self.saved_files))} video(s) and saved in project_folder/csv/targets_inserted directory.')
+        stdout_success(msg=f'Annotations for {str(len(self.saved_files))} video(s) and saved in project_folder/csv/targets_inserted directory.')
 
     def __save(self):
         save_df(df=self.results_df, file_type=self.file_type, save_path=self.save_path)
         self.saved_files.append(self.save_path)
         print(f'BENTO annotations appended to video {self.video_name} and saved in {self.save_path}')
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.55.7/simba/third_party_label_appenders/solomon_importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 __author__ = "Simon Nilsson"
 
 import os, glob
 from simba.drop_bp_cords import get_fn_ext
 from simba.feature_extractors.unit_tests import read_video_info
+from simba.misc_tools import stdout_success
 from simba.read_config_unit_tests import (check_if_filepath_list_is_empty,
                                           check_that_column_exist)
 from simba.rw_dfs import read_df, save_df
 from copy import deepcopy
 from simba.mixins.config_reader import ConfigReader
 
 class SolomonImporter(ConfigReader):
@@ -79,15 +80,15 @@
                               f'Please make sure you imported the same video as you annotated in SOLOMON into SimBA and the video is registered with the correct frame rate.')
                     target_frm_list = [x for x in target_frm_list if x not in idx_difference]
                 out_df[clf_name] = 0
                 out_df.loc[target_frm_list, clf_name] = 1
 
             save_df(out_df, self.file_type, save_path)
             print('Solomon annotations appended for video {}...'.format(file_name))
-        print('SIMBA COMPLETE: All SOLOMON annotations imported. Data saved in the project_folder/csv/targets_inserted directory of the SimBA project')
+        stdout_success(msg='All SOLOMON annotations imported. Data saved in the project_folder/csv/targets_inserted directory of the SimBA project')
 
 # test = SolomonImporter(config_path='/Users/simon/Desktop/envs/simba_dev/tests/test_data/import_tests/project_folder/project_config.ini',
 #                        solomon_dir='/Users/simon/Desktop/envs/simba_dev/tests/test_data/import_tests/solomon_data')
 #
 # test.import_solomon()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/multi_cropper.py` & `Simba-UW-tf-dev-1.55.7/simba/multi_cropper.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from simba.read_config_unit_tests import (check_int,
                                           check_str,
                                           check_if_filepath_list_is_empty)
 import os, glob
 import cv2
 from copy import deepcopy
 from simba.misc_tools import (get_fn_ext,
-                              SimbaTimer)
+                              SimbaTimer,
+                              stdout_success)
 import subprocess
 from simba.enums import Formats
 from simba.utils.errors import CountError, InvalidVideoFileError
 
 class MultiCropper(object):
     """
     Class for cropping single video into multiple videos
@@ -127,16 +128,15 @@
                 command = str('ffmpeg -y -i ') + str(in_video_path) + str(' -vf ') + str('"crop=') + str(width) + ':' + str(
                     height) + ':' + str(topLeftX) + ':' + str(topLeftY) + '" ' + str('-c:v libx264 -c:a copy ') + str(
                     out_file_fn + ' -hide_banner -loglevel error')
                 subprocess.call(command, shell=True)
                 print('Video {} crop {} complete...'.format(name, str(cnt+1)))
 
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: {} new cropped videos created from {} input videos. Cropped videos are saved in the {} directory (elapsed time: {}s)'.format(str(len(self.crop_df)), str(len(self.files_found)), self.output_folder, self.timer.elapsed_time_str))
-
+        stdout_success(msg=f'{str(len(self.crop_df))} new cropped videos created from {str(len(self.files_found))} input videos. Cropped videos are saved in the {self.output_folder} directory', elapsed_time=self.timer.elapsed_time_str)
 
 # test = MultiCropper(file_type='avi', input_folder='/Users/simon/Desktop/troubleshooting/train_model_project/project_folder/test',
 #                     output_folder='/Users/simon/Desktop/troubleshooting/train_model_project/project_folder/test_2', crop_cnt=2)
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/FSTTC_calculator.py` & `Simba-UW-tf-dev-1.55.7/simba/FSTTC_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 __author__ = "Simon Nilsson"
 
-from simba.read_config_unit_tests import (read_config_entry,
-                                          read_config_file,
-                                          check_if_filepath_list_is_empty)
-import os, glob
+from simba.read_config_unit_tests import check_if_filepath_list_is_empty
+import os
 import pandas as pd
-from datetime import datetime
-from simba.feature_extractors.unit_tests import read_video_info_csv, read_video_info
+from simba.feature_extractors.unit_tests import read_video_info
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df
-from simba.misc_tools import (detect_bouts,
-                              SimbaTimer)
-from simba.enums import Paths, ReadConfig
+from simba.misc_tools import (detect_bouts, stdout_success)
+from simba.enums import Defaults, TagNames
 from simba.mixins.config_reader import ConfigReader
 import itertools
 import seaborn as sns
 
 class FSTTCPerformer(ConfigReader):
     """
     Class for calculating forward spike-time tiling coefficients between pairs of
@@ -188,15 +184,15 @@
         for video, data in self.results_dict.items():
             video_df = pd.DataFrame.from_dict(data, orient='index').reset_index().rename(columns={'index': 'FSTTC', 0: 'Value'})
             video_df.insert(loc=0, column='Video', value=video)
             self.out_df = pd.concat([self.out_df,video_df], axis=0)
         file_save_path = os.path.join(self.logs_path, 'FSTTC_{}.csv'.format(str(self.datetime)))
         self.out_df.to_csv(file_save_path)
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: FSTTC data saved at {} (elapsed time: {}s)'.format(file_save_path, self.timer.elapsed_time_str))
+        stdout_success(msg=f'FSTTC data saved at {file_save_path}', elapsed_time=self.timer.elapsed_time_str)
 
     def plot_FSTTC(self):
         """
         Method to visualize forward spike-time tiling coefficients (FSTTC) as png violin plots. Results are stored on
         disk within the `project_folder/logs` directory.
 
         Returns
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/create_project_pop_up.py` & `Simba-UW-tf-dev-1.55.7/simba/create_project_pop_up.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
                                      Entry_Box,
                                      DropDownMenu)
 from PIL import ImageTk
 import PIL.Image
 from simba.mixins.pop_up_mixin import PopUpMixin
 from simba.enums import Formats, Options, Methods, Paths, Keys, Links
 from simba.tkinter_functions import CreateLabelFrameWithIcon
-from simba.utils.errors import DuplicationError
+from simba.utils.errors import DuplicationError, MissingProjectConfigEntryError
 from simba.utils.lookups import (get_body_part_configurations,
                                  get_bp_config_codes,
                                  get_icons_paths)
 from simba.pop_up_classes import (PoseResetterPopUp,
                                   CreateUserDefinedPoseConfigurationPopUp)
 from simba.read_config_unit_tests import (check_if_dir_exists, check_str)
 from simba.project_config_creator import ProjectConfigCreator
@@ -144,16 +144,15 @@
         if selected_value != Methods.CREATE_POSE_CONFIG.value:
             self.img_lbl.config(image=self.bp_lu[selected_value]['img'])
         else:
             _ = CreateUserDefinedPoseConfigurationPopUp(master=self.main_frm, project_config_class=ProjectCreatorPopUp)
 
     def extract_frames(self):
         if not hasattr(self, 'config_path'):
-            print('SIMBA ERROR: Create PROJECT CONFIG before extracting frames')
-            raise FileNotFoundError('SIMBA ERROR: Create PROJECT CONFIG before extracting frames')
+            raise MissingProjectConfigEntryError(msg='Create PROJECT CONFIG before extracting frames')
         video_dir = os.path.join(os.path.dirname(self.config_path), 'videos')
         extract_frames_from_all_videos_in_directory(config_path=self.config_path, directory=video_dir)
 
     def run(self):
         project_dir = self.project_dir_select.folder_path
         check_if_dir_exists(in_dir=project_dir)
         project_name = self.project_name_eb.entry_get
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/video_info_table.py` & `Simba-UW-tf-dev-1.55.7/simba/video_info_table.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.55.7/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import pandas as pd
 from simba.read_config_unit_tests import (read_config_entry, read_config_file, check_file_exist_and_readable)
 from simba.feature_extractors.unit_tests import read_video_info_csv, read_video_info
 import os, glob
 from simba.drop_bp_cords import getBpNames, create_body_part_dictionary
-from simba.misc_tools import check_multi_animal_status, get_fn_ext
+from simba.misc_tools import (check_multi_animal_status,
+                              get_fn_ext,
+                              stdout_success)
 from simba.rw_dfs import read_df
 from simba.read_config_unit_tests import check_that_column_exist
 from datetime import datetime
 from simba.cue_light_tools.cue_light_tools import find_frames_when_cue_light_on
 from simba.utils.errors import NoFilesFoundError
 
 class CueLightClfAnalyzer(object):
@@ -142,15 +144,15 @@
         Returns
         -------
         None
         """
 
         save_results_path = os.path.join(self.logs_path, 'Cue_lights_clf_statistics_{}.csv'.format(self.datetime))
         self.results_df.to_csv(save_results_path)
-        print('SIMBA COMPLETE: Cue light classifier statistics saved in project_folder/logs directory.')
+        stdout_success(msg='SIMBA COMPLETE: Cue light classifier statistics saved in project_folder/logs directory.')
 
 
 # test = CueLightClfAnalyzer(config_path='/Users/simon/Desktop/troubleshooting/light_analyzer/project_folder/project_config.ini',
 #                            pre_window=1000,
 #                            post_window=1000,
 #                            cue_light_names=['Cue_light'],
 #                            clf_list=['Attack'])
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.55.7/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import time
 from simba.read_config_unit_tests import (read_config_entry,
                                           read_config_file)
 from sklearn.cluster import KMeans
 import os, glob
 import itertools
 import pandas as pd
 from simba.rw_dfs import read_df, save_df
 from simba.drop_bp_cords import (get_fn_ext,
                                  create_body_part_dictionary)
 from simba.misc_tools import (find_video_of_file,
                               get_video_meta_data,
                               detect_bouts,
                               find_core_cnt,
-                              check_multi_animal_status)
+                              check_multi_animal_status,
+                              stdout_success)
 from simba.drop_bp_cords import getBpNames
 import cv2
 import numpy as np
 import multiprocessing
 from simba.feature_extractors.unit_tests import read_video_info_csv, read_video_info
 import functools
 import time
@@ -201,15 +201,15 @@
             pool.terminate()
             pool.join()
             self.calculate_descriptive_statistics()
             self.insert_light_data()
             self.remove_outlier_events()
             save_df(self.data_df, self.file_type, self.save_path)
         elapsed_time = str(round(time.time() - start_time, 2)) + 's'
-        print('SIMBA CUE LIGHT ANALYSIS COMPLETE: Analysed {} files. Data stored in project_folder/csv/cue_lights. Elapsed time {}'.format(str(len(self.files_found)), elapsed_time))
+        stdout_success(msg=f'Analysed {str(len(self.files_found))} files. Data stored in project_folder/csv/cue_lights', elapsed_time=elapsed_time)
 
 # test = CueLightAnalyzer(config_path='/Users/simon/Desktop/troubleshooting/light_analyzer/project_folder/project_config.ini',
 #                         in_dir='/Users/simon/Desktop/troubleshooting/light_analyzer/project_folder/csv/outlier_corrected_movement_location',
 #                         cue_light_names=['Cue_light'])
 # test.analyze_files()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.55.7/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.55.7/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.55.7/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from simba.read_config_unit_tests import (read_config_entry, read_config_file, check_file_exist_and_readable)
 from simba.feature_extractors.unit_tests import read_video_info_csv, read_video_info
-from simba.misc_tools import get_video_meta_data
+from simba.misc_tools import get_video_meta_data, stdout_success
 import itertools, os
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df
 import pandas as pd
 import cv2
 from simba.drop_bp_cords import getBpNames, create_body_part_dictionary, createColorListofList
 from simba.misc_tools import check_multi_animal_status
@@ -225,15 +225,15 @@
                     self.writer.release()
                 print(e.args)
                 print('NOTE: index error / keyerror. Some frames of the video may be missing. Make sure you are running latest version of SimBA with pip install simba-uw-tf-dev')
                 break
 
         if self.video_setting:
             self.writer.release()
-        print('Cue light visualization for video {} saved...'.format(self.video_name))
+        stdout_success(msg=f'Cue light visualization for video {self.video_name} saved...')
 
 # test = CueLightVisualizer(config_path='/Users/simon/Desktop/troubleshooting/light_analyzer/project_folder/project_config.ini',
 #                           cue_light_names=['Cue_light'],
 #                           video_path='/Users/simon/Desktop/troubleshooting/light_analyzer/project_folder/videos/20220422_ALMEAG02_B0.avi',
 #                           video_setting=True,
 #                           frame_setting=False)
 # test.visualize_cue_light_data()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.55.7/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os, glob
 from simba.read_config_unit_tests import (read_config_entry, read_config_file, check_file_exist_and_readable)
 from simba.feature_extractors.unit_tests import read_video_info_csv, read_video_info
 from simba.rw_dfs import read_df
-from simba.misc_tools import get_fn_ext, check_multi_animal_status
+from simba.misc_tools import (get_fn_ext,
+                              check_multi_animal_status,
+                              stdout_success)
 from simba.drop_bp_cords import getBpNames, create_body_part_dictionary
 from collections import defaultdict
 import pandas as pd
 import numpy as np
 from statistics import mean
 from simba.roi_tools.ROI_analyzer import ROIAnalyzer
 from datetime import datetime
@@ -204,13 +206,13 @@
         -------
         None
         """
 
         save_results_path = os.path.join(self.logs_path, 'Cue_lights_movement_statistics_{}.csv'.format(self.datetime))
         self.results_df = self.results_df.sort_values('Video').reset_index(drop=True)
         self.results_df.to_csv(save_results_path)
-        print('SIMBA COMPLETE: Cue light movement statistics saved in project_folder/logs directory.')
+        stdout_success(msg='Cue light movement statistics saved in project_folder/logs directory.')
         if self.roi_setting:
             save_roi_results_path = os.path.join(self.logs_path, 'Cue_lights_roi_statistics_{}.csv'.format(self.datetime))
             self.results_roi_df = self.results_roi_df.sort_values('Video').reset_index(drop=True)
-            self.results_roi_df.to_csv(save_roi_results_path )
-            print('SIMBA COMPLETE: Cue light ROI statistics saved in project_folder/logs directory.')
+            self.results_roi_df.to_csv(save_roi_results_path)
+            stdout_success(msg='Cue light ROI statistics saved in project_folder/logs directory.')
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/extract_frames_fast.py` & `Simba-UW-tf-dev-1.55.7/simba/extract_frames_fast.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.55.7/simba/utils/warnings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from simba.misc_tools import stdout_warning
 
 def ThirdPartyAnnotationsOutsidePoseEstimationDataWarning(video_name: str,
                                                           frm_cnt: int,
                                                           log_status: bool = False,
                                                           clf_name: str or None = None,
                                                           annotation_frms: int or None = None,
                                                           first_error_frm: int or None=None,
@@ -15,60 +16,66 @@
                f'However, in BORIS, you have annotated {clf_name} to happen at frame number {str(first_error_frm)}. '
                f'These ambiguous annotations occur in {str(ambiguous_cnt)} different frames for video {video_name} that SimBA will **remove** by default. '
                f'Please make sure you imported the same video as you annotated in BORIS into SimBA and the video is registered with the correct frame rate. '
                f'SimBA will only append annotations made to the frames present in the pose estimation data.')
     else:
         msg = f'SIMBA THIRD-PARTY ANNOTATION WARNING: The annotations for video {video_name} contain data for {str(annotation_frms)} frames. The pose-estimation features for the same video contain data for {str(frm_cnt)} frames. SimBA will use the annotations for the frames present in the pose-estimation data and discard the rest. If the annotation data is shorter than the pose-estimation data, SimBA will assume the missing annotation frames are all behavior absent.'
     if log_status: logging.warning(msg=msg)
-    print(msg)
+    stdout_warning(msg=msg)
 
 def ThirdPartyAnnotationsClfMissingWarning(video_name: str,
                                               clf_name: str):
     msg = f'SIMBA THIRD-PARTY ANNOTATION WARNING: No annotations detected for video {video_name} and behavior {clf_name}. ' \
           f'SimBA will set all frame annotations as absent.'
-    print(msg)
+    stdout_warning(msg=msg)
 
 def ThirdPartyAnnotationsAdditionalClfWarning(video_name: str,
                                               clf_names: list,
                                               log_status: bool=False):
     msg = f'SIMBA THIRD-PARTY ANNOTATION WARNING: Annotations file for video {video_name} has annotations for the following behaviors {clf_names} that are NOT classifiers named in the SimBA project. SimBA will OMIT appending the data for these {str(len(clf_names))} classifiers.'
     if log_status: logging.warning(msg=msg)
-    print(msg)
+    stdout_warning(msg=msg)
 
 
 def ThirdPartyAnnotationsInvalidFileFormatWarning(annotation_app: str,
                                                   file_path: str,
                                                   log_status: bool=False):
     msg = f'SIMBA WARNING: {file_path} is not a valid {annotation_app} file and is skipped. See the SimBA GitHub repository for expected file format'
     if log_status: logging.warning(msg=msg)
-    print(msg)
+    stdout_warning(msg=msg)
 
 def ThirdPartyAnnotationsMissingAnnotationsWarning(video_name: str,
                                                    clf_names: list,
                                                    log_status: bool=False):
     msg = f'SIMBA THIRD-PARTY ANNOTATION WARNING: No annotations detected for SimBA classifier(s) named {clf_names} for video {video_name}. All frame annotations will be set to behavior absent (0).'
     if log_status: logging.warning(msg=msg)
-    print(msg)
+    stdout_warning(msg=msg)
 
 def ThirdPartyAnnotationsFpsConflictWarning(video_name: str,
                                             annotation_fps: int,
                                             video_fps: int):
     msg = f'SIMBA THIRD-PARTY ANNOTATION WARNING: The FPS for video {video_name} is set to {str(video_fps)} in SimBA and {str(annotation_fps)} in the annotation file'
-    print(msg)
+    stdout_warning(msg=msg)
 
 
 def ThirdPartyAnnotationEventCountWarning(video_name: str, clf_name: str, start_event_cnt: int, stop_event_cnt: int, log_status: bool=False):
     msg = f'SIMBA THIRD-PARTY ANNOTATION WARNING: The annotations for behavior {clf_name} in video {video_name} contains {str(start_event_cnt)} start events and {str(stop_event_cnt)} stop events. SimBA requires the number of stop and start event counts to be equal. SimBA will try to find and delete the odd event stamps.'
     if log_status: logging.warning(msg=msg)
-    print(msg)
+    stdout_warning(msg=msg)
 
 def ThirdPartyAnnotationOverlapWarning(video_name: str,
                                        clf_name: str,
                                        log_status: bool=False):
     msg = f'SIMBA THIRD-PARTY ANNOTATION WARNING: The annotations for behavior {clf_name} in video {video_name} contains behavior start events that are initiated PRIOR to the PRECEDING behavior event ending. SimBA requires a specific behavior event to end before another behavior event can start. SimBA will try and delete these events.'
     if log_status: logging.warning(msg=msg)
-    print(msg)
+    stdout_warning(msg=msg)
 
 def ThirdPartyAnnotationFileNotFoundWarning(video_name: str, log_status: bool=False):
     msg = f'SIMBA THIRD-PARTY ANNOTATION WARNING: Could not find annotations for video features file {video_name} in the annotations directory.'
     if log_status: logging.warning(msg=msg)
-    print(msg)
+    stdout_warning(msg=msg)
+
+def BodypartColumnNotFoundWarning(msg: str):
+    stdout_warning(msg=f'SIMBA BODY-PART COLUMN NOT FOUND WARNING: {msg}')
+
+def KleinbergWarning(msg: str):
+    stdout_warning(msg=f'SIMBA KLEINBERG WARNING: {msg}')
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.55.7/simba/utils/lookups.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,23 @@
             'DEEPETHOGRAM': 'csv',
             'BENTO': 'annot'}
 
 
 def get_emojis() -> dict:
     return {'thank_you': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001f64f'.encode('utf-16be'))),
             'relaxed': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001F600'.encode('utf-16be'))),
-            'angry': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001F92C'.encode('utf-16be')))}
+            'error': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001F6A8'.encode('utf-16be'))),
+            'complete': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001F680'.encode('utf-16be'))),
+            'warning': ''.join(chr(x) for x in struct.unpack('>2H', '\U000FEB23'.encode('utf-16be')))}
+
+
+
+
+
+
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/utils/errors.py` & `Simba-UW-tf-dev-1.55.7/simba/utils/errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,237 +1,244 @@
 from tkinter import messagebox as mb
-
+from simba.enums import TagNames, Defaults
 
 WINDOW_TITLE = 'SIMBA ERROR'
 
 class SimbaError(Exception):
     def __init__(self, msg: str, show_window: bool):
         from simba.utils.lookups import get_emojis
         self.msg = msg
         self.emojis = get_emojis()
         if show_window:
             mb.showerror(title=WINDOW_TITLE, message=msg)
 
     def __str__(self):
         return self.msg
 
+    def print_msg(self, msg):
+        print(f'SIMBA ERROR: {msg}{Defaults.STR_SPLIT_DELIMITER.value}{TagNames.ERROR.value}')
+
 
 class NoSpecifiedOutputError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA ERROR: {msg}' + self.emojis['angry'])
+        self.print_msg(msg=f'SIMBA NO SPECIFIED OUTPUT ERROR: {msg}')
 
 class ROICoordinatesNotFoundError(SimbaError):
     def __init__(self, expected_file_path: str, show_window: bool = False):
         msg = f'No ROI coordinates found. Please use the [ROI] tab to define ROIs. Expected at location {expected_file_path}'
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA ERROR: {msg}')
 
 class NoChoosenClassifierError(SimbaError):
     def __init__(self, show_window: bool = False):
         msg = f'Select at least one classifiers'
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA ERROR: {msg}')
 
 class NoChoosenROIError(SimbaError):
     def __init__(self, show_window: bool = False):
         msg = f'Please select at least one ROI.'
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA ERROR: {msg}')
 
 class NoChoosenMeasurementError(SimbaError):
     def __init__(self, show_window: bool = False):
         msg = 'Please select at least one measurement to calculate descriptive statistics for.'
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA ERROR: {msg}')
 
 
 class NoROIDataError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(msg)
+        self.print_msg(msg=f'SIMBA ERROR: {msg}')
+
 
 class MixedMosaicError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(msg)
+        self.print_msg(msg=f'SIMBA ERROR: {msg}')
+
 
 class AnimalNumberError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA ERROR: {msg}')
 
 class InvalidFilepathError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA ERROR: {msg}')
 
 
 class NoFilesFoundError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA ERROR: {msg}')
 
 class NotDirectoryError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA ERROR: {msg}')
 
 class DirectoryExistError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA ERROR: {msg}')
 
 class FileExistError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA ERROR: {msg}')
 
 
 class FrameRangeError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA ERROR: {msg}')
 
 class AdvancedLabellingError(SimbaError):
     def __init__(self, frame: str, lbl_lst: list, unlabel_lst: list, show_window: bool = False):
         msg = 'SIMBA ERROR: In advanced labelling of multiple behaviors, any annotated frame cannot have some ' \
                    'behaviors annotated as present/absent, while other behaviors are un-labelled. All behaviors need ' \
                    'labels for a frame with one or more labels. In frame {}, behaviors {} are labelled, while behaviors ' \
                    '{} are un-labelled.'.format(str(frame), lbl_lst, unlabel_lst)
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA ERROR: {msg}')
 
 class InvalidHyperparametersFileError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA HYPERPAREMETER FILE ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA HYPERPARAMETER FILE ERROR: {msg}')
 
 class InvalidVideoFileError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA VIDEO FILE ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA VIDEO FILE ERROR: {msg}')
 
 class InvalidFileTypeError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA INVALID FILE TYPE ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA INVALID FILE TYPE ERROR: {msg}')
 
 class FaultyTrainingSetError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA INVALID ML TRAINING SET ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA INVALID ML TRAINING SET ERROR: {msg}')
 
 class CountError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA COUNT ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA COUNT ERROR: {msg}')
 
 class DuplicationError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA DUPLICATION ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA DUPLICATION ERROR: {msg}')
 
 class InvalidInputError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA VALUE ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA VALUE ERROR: {msg}')
 
 class IntegerError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA INTEGER ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA INTEGER ERROR: {msg}')
 
 class StringError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA STRING ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA STRING ERROR: {msg}')
 
 class FloatError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA FLOAT ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA FLOAT ERROR: {msg}')
 
 class MissingProjectConfigEntryError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA MISSING PROJECT CONFIG ENTRY ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA MISSING PROJECT CONFIG ENTRY ERROR: {msg}')
 
 class CorruptedFileError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA CORRUPTED FILE ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA CORRUPTED FILE ERROR: {msg}')
 
 class ParametersFileError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        print(f'SIMBA VIDEO PARAMETERS FILE ERROR: {msg}')
-
+        self.print_msg(msg=f'SIMBA VIDEO PARAMETERS FILE ERROR: {msg}')
 
-
-#####
 class ColumnNotFoundError(SimbaError):
     def __init__(self, column_name: str, file_name: str, show_window: bool = False):
         msg = f'SIMBA ERROR: Field name {column_name} could not be found in file {file_name}'
         super().__init__(msg=msg, show_window=show_window)
-        print(msg)
+        self.print_msg(msg=msg)
+
+class BodypartColumnNotFoundError(SimbaError):
+    def __init__(self, msg: str, show_window: bool = False):
+        super().__init__(msg=msg, show_window=show_window)
+        self.print_msg(msg=msg)
 
 class AnnotationFileNotFoundError(SimbaError):
     def __init__(self, video_name: str, show_window: bool = False):
         msg = f'SIMBA THIRD-PARTY ANNOTATION ERROR: NO ANNOTATION DATA FOR VIDEO {video_name} FOUND'
         super().__init__(msg=msg, show_window=show_window)
-        print(msg)
+        self.print_msg(msg=msg)
 
 
 
 #####
 
 
 class ThirdPartyAnnotationFileNotFoundError(SimbaError):
     def __init__(self, video_name: str, show_window: bool = False):
         msg = f'SIMBA ERROR: Could not find file in project_folder/csv/features_extracted directory representing annotations for video {video_name}'
         super().__init__(msg=msg, show_window=show_window)
-        print(msg)
+        self.print_msg(msg=msg)
 
 class ThirdPartyAnnotationsFpsConflictError(SimbaError):
     def __init__(self, video_name: str, annotation_fps: int, video_fps: int, show_window: bool = False):
         msg = f'SIMBA THIRD-PARTY ANNOTATION ERROR: The FPS for video {video_name} is set to {str(video_fps)} in SimBA and {str(annotation_fps)} in the annotation file'
         super().__init__(msg=msg, show_window=show_window)
-        print(msg)
+        self.print_msg(msg=msg)
 
 
 class ThirdPartyAnnotationsMissingAnnotationsError(SimbaError):
     def __init__(self, video_name: str, clf_names: list, show_window: bool = False):
         msg = f'SIMBA THIRD-PARTY ANNOTATION ERROR: No annotations detected for SimBA classifier(s) named {clf_names} for video {video_name}'
         super().__init__(msg=msg, show_window=show_window)
-        print(msg)
+        self.print_msg(msg=msg)
 
 class ThirdPartyAnnotationOverlapError(SimbaError):
     def __init__(self, video_name: str, clf_name: str, show_window: bool = False):
         msg = f'SIMBA THIRD-PARTY ANNOTATION ERROR: The annotations for behavior {clf_name} in video {video_name} contains behavior start events that are initiated PRIOR to the PRECEDING behavior event ending. SimBA requires a specific behavior event to end before another behavior event can start.'
         super().__init__(msg=msg, show_window=show_window)
-        print(msg)
+        self.print_msg(msg=msg)
 
 class ThirdPartyAnnotationsAdditionalClfError(SimbaError):
     def __init__(self, video_name: str, clf_names: list, show_window: bool = False):
         msg = f'SIMBA THIRD-PARTY ANNOTATION ERROR: Annotations file for video {video_name} has annotations for the following behaviors {clf_names} that are NOT classifiers named in the SimBA project.'
         super().__init__(msg=msg, show_window=show_window)
-        print(msg)
+        self.print_msg(msg=msg)
 
 class ThirdPartyAnnotationEventCountError(SimbaError):
     def __init__(self, video_name: str, clf_name: str, start_event_cnt: int, stop_event_cnt: int, show_window: bool = False):
         msg = f'SIMBA THIRD-PARTY ANNOTATION ERROR: The annotations for behavior {clf_name} in video {video_name} contains {str(start_event_cnt)} start events and {str(stop_event_cnt)} stop events. SimBA requires the number of stop and start event counts to be equal.'
         super().__init__(msg=msg, show_window=show_window)
-        print(msg)
+        self.print_msg(msg=msg)
 
 class ThirdPartyAnnotationsClfMissingError(SimbaError):
     def __init__(self, video_name: str, clf_name: str, show_window: bool = False):
         msg = f'SIMBA THIRD-PARTY ANNOTATION WARNING: No annotations detected for video {video_name} and behavior {clf_name}.'
         super().__init__(msg=msg, show_window=show_window)
-        print(msg)
+        self.print_msg(msg=msg)
 
 class ThirdPartyAnnotationsOutsidePoseEstimationDataError(SimbaError):
     def __init__(self,
                  video_name: str,
                  frm_cnt: int,
                  clf_name: str or None = None,
                  annotation_frms: int or None = None,
@@ -247,8 +254,8 @@
                 f'However, in BORIS, you have annotated {clf_name} to happen at frame number {str(first_error_frm)}. '
                 f'These ambiguous annotations occur in {str(ambiguous_cnt)} different frames for video {video_name} that SimBA will **remove** by default. '
                 f'Please make sure you imported the same video as you annotated in BORIS into SimBA and the video is registered with the correct frame rate.')
         else:
             msg = f'SIMBA THIRD-PARTY ANNOTATION WARNING: The annotations for video {video_name} contain data for {str(annotation_frms)} frames. The pose-estimation features for the same video contain data for {str(frm_cnt)} frames.'
 
         super().__init__(msg=msg, show_window=show_window)
-        print(msg)
+        self.print_msg(msg=msg)
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/labelling_interface.py` & `Simba-UW-tf-dev-1.55.7/simba/labelling_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from simba.rw_dfs import read_df, save_df
 from simba.read_config_unit_tests import (read_config_entry,
                                           read_config_file,
                                           check_file_exist_and_readable,
                                           check_int,
                                           check_float,
                                           read_project_path_and_file_type)
-from simba.misc_tools import get_video_meta_data, get_fn_ext
+from simba.misc_tools import get_video_meta_data, get_fn_ext, stdout_success
 from simba.enums import ReadConfig, Paths, Dtypes
 import simba
 from tkinter import *
 from tkinter import filedialog
 from PIL import Image, ImageTk
 from subprocess import Popen, PIPE
 import os
@@ -296,15 +296,15 @@
         self.save_df = read_df(self.features_extracted_file_path, self.file_type)
         self.save_df = pd.concat([self.save_df, self.data_df_targets], axis=1)
         try:
             save_df(self.save_df, self.file_type, self.targets_inserted_file_path)
         except Exception as e:
             print(e, 'SIMBA ERROR: File for video {} could not be saved.')
             raise FileExistsError
-        print('Annotation file for video {} saved within the project_folder/csv/targets_inserted directory.'.format(self.video_name))
+        stdout_success(msg=f'SAVED: Annotation file for video {self.video_name} saved within the project_folder/csv/targets_inserted directory.')
         if not self.config.has_section('Last saved frames'):
             self.config.add_section('Last saved frames')
         self.config.set('Last saved frames', str(self.video_name), str(self.current_frm_n.get()))
         with open(self.config_path, 'w') as configfile:
             self.config.write(configfile)
 
     def __create_print_statements(self, frame_range: bool=None, start_frame: int=None, end_frame: int=None):
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/timebins_movement_analyzer.py` & `Simba-UW-tf-dev-1.55.7/simba/timebins_movement_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 
 import pandas as pd
 from simba.read_config_unit_tests import (read_config_entry,
                                           check_that_column_exist,
                                           check_if_filepath_list_is_empty)
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.misc_tools import (SimbaTimer,
-                              framewise_euclidean_distance)
+                              framewise_euclidean_distance,
+                              stdout_success)
 from simba.enums import (ReadConfig,
-                         Dtypes)
+                         Dtypes,
+                         Defaults,
+                         TagNames)
 from simba.drop_bp_cords import create_body_part_dictionary, getBpNames
 import os, glob
 from simba.rw_dfs import read_df
 from simba.drop_bp_cords import get_fn_ext
 import seaborn as sns
 import matplotlib.pyplot as plt
 import itertools
@@ -149,15 +152,15 @@
         self.video_df = pd.concat(self.out_df_lst, axis= 0).sort_values(by=['Video', 'Time bin #']).set_index('Video')
         if self.plots:
             self.__create_plots()
 
         save_path = os.path.join(self.project_path, 'logs', 'Time_bins_movement_results_' + self.datetime + '.csv')
         self.video_df.to_csv(save_path)
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: Movement time-bins results saved at {} (elapsed time: {}s)'.format(save_path, self.timer.elapsed_time_str))
+        stdout_success(msg=f'Movement time-bins results saved at {save_path}', elapsed_time=self.timer.elapsed_time_str)
 
 # test = TimeBinsMovementAnalyzer(config_path='/Users/simon/Desktop/envs/troubleshooting/Vince_time_bins/project_folder/project_config.ini',
 #                                 bin_length=60, plots=True)
 # test.analyze_movement()
 
 # test = TimeBinsMovementAnalyzer(config_path='/Users/simon/Desktop/envs/troubleshooting/Two_animals_16bps/project_folder/project_config.ini',
 #                                 bin_length=1, plots=True)
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/train_model_functions.py` & `Simba-UW-tf-dev-1.55.7/simba/train_model_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     Helper to delete fields that contain annotations which are not the target.
 
     Parameters
     ----------
     df: pd.DataFrame
         pandas Dataframe holding features and annotations.
     annotations_lst: list
-        List of column fields to be removed from df
+        Column fields to be removed from df
 
     Returns
     -------
     df: pd.DataFrame
     """
 
     for a_col in annotations_lst:
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.55.7/simba/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/timebins_clf_analyzer.py` & `Simba-UW-tf-dev-1.55.7/simba/timebins_clf_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 from simba.read_config_unit_tests import (check_int,
                                           check_if_filepath_list_is_empty)
-from simba.misc_tools import detect_bouts
+from simba.misc_tools import (detect_bouts,
+                              stdout_success)
 from simba.feature_extractors.unit_tests import read_video_info
 import os, glob
+from simba.enums import Defaults, TagNames
 from simba.rw_dfs import read_df
 from simba.drop_bp_cords import get_fn_ext
 from collections import defaultdict
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import NoChoosenMeasurementError
 
 class TimeBinsClf(ConfigReader):
@@ -111,18 +113,17 @@
                 self.out_df_lst.append(data_df)
         out_df = pd.concat(self.out_df_lst, axis=0).sort_values(by=['Video', 'Time bin #']).set_index('Video')
         out_df = out_df[out_df['Measurement'].isin(self.measurements)]
         out_df = out_df[out_df['Classifier'].isin(self.classifiers)]
         save_path = os.path.join(self.project_path, 'logs', 'Time_bins_ML_results_' + self.datetime + '.csv')
         out_df.to_csv(save_path)
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: Classification time-bins results saved at project_folder/logs/output/{} (elapsed time: {}s)'.format(str('Time_bins_ML_results_' + self.datetime + '.csv'), self.timer.elapsed_time_str))
+        stdout_success(msg=f'Classification time-bins results saved at project_folder/logs/output/{str("Time_bins_ML_results_" + self.datetime + ".csv")}', elapsed_time=self.timer.elapsed_time_str)
 
-
-# test = TimeBinsClf(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals/project_folder/project_config.ini',
+# test = TimeBinsClf(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                    bin_length=2,
 #                    measurements=['First occurance (s)', 'Event count', 'Total event duration (s)', 'Mean event duration (s)'],
 #                    classifiers=['Attack', 'Sniffing'])
 # test.analyze_timebins_clf()
 
 
 # test = TimeBinsClf(config_path='/Users/simon/Desktop/troubleshooting/light_analyzer/project_folder/project_config.ini',
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/calculate_px_dist.py` & `Simba-UW-tf-dev-1.55.7/simba/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/movement_processor.py` & `Simba-UW-tf-dev-1.55.7/simba/movement_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 from simba.misc_tools import (get_fn_ext,
-                              framewise_euclidean_distance)
+                              framewise_euclidean_distance,
+                              stdout_success)
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.read_config_unit_tests import (read_config_entry,
                                           check_if_filepath_list_is_empty)
-from simba.enums import ReadConfig
+from simba.enums import (ReadConfig,
+                         Defaults,
+                         TagNames)
 import os
 from simba.mixins.config_reader import ConfigReader
 from collections import defaultdict
 from simba.rw_dfs import read_df
 import numpy as np
 from statistics import mean
 
@@ -126,12 +129,12 @@
         self.out_df = pd.DataFrame(columns=['Video', 'Animal', 'Measurement', 'Value'])
         for video, video_data in self.results.items():
             for animal, animal_data in video_data.items():
                 for measure, mesure_val in animal_data.items():
                     self.out_df.loc[len(self.out_df)] = [video, animal, measure, mesure_val]
         self.out_df.set_index('Video').to_csv(self.save_path)
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: Movement log saved in {} (elapsed time: {}s)'.format(self.save_path, self.timer.elapsed_time_str))
+        stdout_success(msg= f'Movement log saved in {self.save_path}', elapsed_time=self.timer.elapsed_time_str)
 
-# test = MovementProcessor(config_path='/Users/simon/Desktop/envs/troubleshooting/Two_animals_16bps/project_folder/project_config.ini')
+#test = MovementProcessor(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
 # test.process_movement()
 # test.save_results()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pybursts.py` & `Simba-UW-tf-dev-1.55.7/simba/pybursts.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/run_model_new.py` & `Simba-UW-tf-dev-1.55.7/simba/run_model_new.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,21 @@
                                                read_video_info)
 from simba.read_config_unit_tests import (read_config_entry,
                                           read_config_file,
                                           read_project_path_and_file_type)
 from simba.train_model_functions import get_model_info
 from simba.misc_tools import (get_fn_ext,
                               plug_holes_shortest_bout,
-                              SimbaTimer)
-from simba.enums import ReadConfig, Paths, Dtypes
+                              SimbaTimer,
+                              stdout_success)
+from simba.enums import (ReadConfig,
+                         Paths,
+                         Dtypes,
+                         Defaults,
+                         TagNames)
 from simba.drop_bp_cords import drop_bp_cords
 from simba.rw_dfs import read_df, save_df
 import os, glob
 from copy import deepcopy
 import pickle
 import numpy as np
 from simba.utils.errors import NoFilesFoundError
@@ -87,12 +92,12 @@
                     print(e.args)
                     raise IndexError('SIMBA INDEX ERROR: Your classifier has not been created properly. See The SimBA GitHub FAQ page for more information and suggested fixes.')
                 out_df[m_hyp['model_name']] = np.where(out_df[probability_column] > m_hyp['threshold'], 1, 0)
                 out_df = plug_holes_shortest_bout(data_df=out_df, clf_name=m_hyp['model_name'], fps=fps, shortest_bout=m_hyp['minimum_bout_length'])
             save_df(out_df, self.file_type, file_save_path)
             print('Predictions created for {} ...'.format(file_name))
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: Machine predictions complete. Files saved in project_folder/csv/machine_results directory (elapsed time: {}s)'.format(self.timer.elapsed_time_str))
+        stdout_success(msg='Machine predictions complete. Files saved in project_folder/csv/machine_results directory', elapsed_time=self.timer.elapsed_time_str)
 
 # test = RunModel(config_path='/Users/simon/Downloads/Automated PRT_test/project_folder/project_config.ini')
 # test.run_models()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/rw_dfs.py` & `Simba-UW-tf-dev-1.55.7/simba/rw_dfs.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/reverse_2_animal_tracking.py` & `Simba-UW-tf-dev-1.55.7/simba/reverse_2_animal_tracking.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/Directing_animals_analyzer.py` & `Simba-UW-tf-dev-1.55.7/simba/Directing_animals_analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Simon Nilsson"
 
 from simba.read_config_unit_tests import check_if_filepath_list_is_empty
 from simba.feature_extractors.unit_tests import read_video_info
-from simba.misc_tools import line_length_numba, SimbaTimer
+from simba.misc_tools import line_length_numba, SimbaTimer, stdout_success
 from simba.drop_bp_cords import (get_fn_ext,
                                  checkDirectionalityCords)
 from simba.rw_dfs import read_df
 import pandas as pd
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import AnimalNumberError
 import itertools
@@ -128,15 +128,14 @@
         into CSV files on disk. Results are stored in `project_folder/logs` directory of the SimBA project.
 
         Returns
         -------
         None
         """
 
-
         for video_name, video_data in self.directionality_df_dict.items():
             save_name = os.path.join(self.directionality_df_dir, video_name + '.csv')
             video_data.to_csv(save_name)
             print(f'Detailed directional data saved for video {video_name}...')
         print(f'All detailed directional data saved in the {self.directionality_df_dir} directory')
 
     def summary_statistics(self):
@@ -161,15 +160,15 @@
                 value = round(len(idx_directing) / fps, 3)
                 out_df_lst.append(pd.DataFrame([[video_name, animal_permutation, value]], columns=['Video', 'Animal permutation', 'Value (s)']))
         self.summary_df = pd.concat(out_df_lst, axis=0).sort_values(by=['Video', 'Animal permutation']).set_index('Video')
         self.save_path = os.path.join(self.logs_path, 'Direction_data_{}{}'.format(str(self.datetime), '.csv'))
         self.summary_df.to_csv(self.save_path)
         self.timer.stop_timer()
         print('Summary directional statistics saved at ' + os.path.join(self.logs_path, 'Direction_data_{}{}'.format(str(self.datetime), '.csv')))
-        print('SIMBA COMPLETE: All directional data saved in SimBA project (elapsed time: {}s).'.format(self.timer.elapsed_time_str))
+        stdout_success(msg='All directional data saved in SimBA project', elapsed_time=self.timer.elapsed_time_str)
 
 # test = DirectingOtherAnimalsAnalyzer(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
 # test.process_directionality()
 # test.create_directionality_dfs()
 # test.save_directionality_dfs()
 # test.summary_statistics()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/Validate_model_one_video_run_clf.py` & `Simba-UW-tf-dev-1.55.7/simba/Validate_model_one_video_run_clf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 __author__ = "Simon Nilsson"
 
-from simba.read_config_unit_tests import (read_config_entry,
-                                          read_config_file,
+from simba.read_config_unit_tests import (read_config_file,
                                           check_file_exist_and_readable,
                                           read_project_path_and_file_type)
 
 from simba.rw_dfs import (read_df,
                           save_df)
 from simba.train_model_functions import read_pickle
 from simba.drop_bp_cords import (get_fn_ext,
                                  drop_bp_cords)
 from copy import deepcopy
-import pickle
+from simba.misc_tools import stdout_success
 import warnings
 import time
 import os
 warnings.filterwarnings('ignore',category=FutureWarning)
 warnings.filterwarnings('ignore',category=DeprecationWarning)
 
 class ValidateModelRunClf(object):
@@ -80,13 +79,13 @@
             print('SIMBA INDEXERROR: Your classifier has not been created properly. See The SimBA GitHub FAQ page for more information and suggested fixes.')
             raise IndexError
 
         save_filename = os.path.join(self.save_path, file_name + '.' + self.file_type)
         save_df(output_df, self.file_type, save_filename)
         elapsed_time = str(round(time.time() - self.start_time, 2))
 
-        print('SIMBA COMPLETE: Validation predictions generated for "{}" within the project_folder/csv/validation directory (elapsed time: {})'.format(file_name, elapsed_time))
+        stdout_success(msg=f'Validation predictions generated for "{file_name}" within the project_folder/csv/validation directory', elapsed_time=elapsed_time)
         print('Click on "Interactive probability plot" to inspect classifier probability thresholds. If satisfactory proceed to specify threshold and minimum bout length and click on "Validate" to create video.')
 #
 # ValidateModelRunClf(config_path=r"Z:\DeepLabCut\DLC_extract\Troubleshooting\DLC_two_mice\project_folder\project_config.ini",
 #                                input_file_path=r"Z:\DeepLabCut\DLC_extract\Troubleshooting\DLC_2_black_060320\project_folder\csv\features_extracted\Together_1.csv",
 #                                clf_path=r"Z:\DeepLabCut\DLC_extract\Troubleshooting\DLC_2_black_060320\models\Approach.sav")
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/tkinter_functions.py` & `Simba-UW-tf-dev-1.55.7/simba/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/setting_menu.py` & `Simba-UW-tf-dev-1.55.7/simba/setting_menu.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/interpolate_pose.py` & `Simba-UW-tf-dev-1.55.7/simba/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/gantt_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 __author__ = "Simon Nilsson"
 
 from simba.misc_tools import (detect_bouts,
-                              get_named_colors)
+                              get_named_colors,
+                              stdout_success)
 from simba.read_config_unit_tests import check_if_filepath_list_is_empty
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.enums import Formats
 from simba.plotting.misc_visualizations import make_gantt_plot
 from simba.train_model_functions import get_all_clf_names
 from simba.drop_bp_cords import get_fn_ext
 from simba.mixins.config_reader import ConfigReader
@@ -133,16 +134,15 @@
                         self.writer.write(frame)
                     print('Gantt frame: {} / {}. Video: {} ({}/{})'.format(str(image_cnt+1), str(len(self.data_df)),
                                                                      self.video_name, str(file_cnt + 1), len(self.files_found)))
                 if self.video_setting:
                     self.writer.release()
                 print('Gantt for video {} saved...'.format(self.video_name))
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: All gantt visualizations created in project_folder/frames/output/gantt_plots directory (elapsed time: {}s)'.format(self.timer.elapsed_time_str))
-
+        stdout_success(msg='All gantt visualizations created in project_folder/frames/output/gantt_plots directory', elapsed_time=self.timer.elapsed_time_str)
 
 # style_attr = {'width': 640, 'height': 480, 'font size': 12, 'font rotation': 45}
 # test = GanttCreatorSingleProcess(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals/project_folder/project_config.ini',
 #                                  frame_setting=False,
 #                                  video_setting=True,
 #                                  last_frm_setting=True,
 #                                  style_attr=style_attr,
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/ROI_plotter_mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 import multiprocessing
 import functools
 from simba.enums import Formats, Paths
 from simba.misc_tools import (get_video_meta_data,
                               add_missing_ROI_cols,
                               SimbaTimer,
                               detect_bouts,
-                              concatenate_videos_in_folder)
+                              concatenate_videos_in_folder,
+                              stdout_success)
 import numpy as np
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import NoFilesFoundError
 
 pd.options.mode.chained_assignment = None
 def _img_creator(data: pd.DataFrame,
                  loc_dict: dict,
@@ -290,15 +291,16 @@
                 print('Image {}/{}, Video {}...'.format(str(int(frm_per_core * (result + 1))), str(len(self.data_df)), self.video_name))
             print('Joining {} multi-processed video...'.format(self.video_name))
             concatenate_videos_in_folder(in_folder=self.temp_folder, save_path=self.video_save_path, video_format='mp4')
 
             video_timer.stop_timer()
             pool.terminate()
             pool.join()
-            print('SIMBA COMPLETE: Video {} created. Video saved in project_folder/frames/output/ROI_analysis (elapsed time: {}s).'.format(self.video_name, video_timer.elapsed_time_str))
+
+            stdout_success(msg=f'Video {self.video_name} created. Video saved in project_folder/frames/output/ROI_analysis', elapsed_time=video_timer.elapsed_time_str)
 
 # test = ROIPlotMultiprocess(ini_path=r'/Users/simon/Desktop/envs/troubleshooting/Termites_5/project_folder/project_config.ini',
 #                video_path="termite_test.mp4",
 #                core_cnt=5,
 #                style_attr={'Show_body_part': True, 'Show_animal_name': True})
 # test.insert_data()
 # test.visualize_ROI_data()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import cv2
 import simba
 from simba.read_config_unit_tests import (read_config_entry,
                                           read_config_file,
                                           check_file_exist_and_readable,
                                           read_project_path_and_file_type)
 from simba.enums import ReadConfig, Dtypes, Paths
-from simba.misc_tools import SimbaTimer
+from simba.misc_tools import SimbaTimer, stdout_success
 
 class ShapAggregateStatisticsVisualizer(object):
 
     """
     Class for calculating aggregate, binned, SHAP value statistics where individual bins represent reaulated features.
     Also creates line chart visualizations reprsenting aggregations of behavior-present SHAP values.
 
@@ -194,8 +194,8 @@
         color_bar_top_left[0] + self.color_bar_img.shape[0], color_bar_top_left[1] + self.color_bar_img.shape[1])
         self.img[color_bar_top_left[0]:color_bar_bottom_right[0],color_bar_top_left[1]:color_bar_bottom_right[1]] = self.color_bar_img
 
         color_bar_middle = ((int(580 + self.baseline_scale_img.shape[1] / 2)), color_bar_bottom_right[0] + 50)
         cv2.putText(self.img, 'CLASSIFICATION PROBABILITY', color_bar_middle, cv2.FONT_HERSHEY_COMPLEX, 1, (0, 0, 0), 2)
         cv2.imwrite(self.img_save_path, self.img)
         self.visualization_timer.stop_timer()
-        print('SIMBA COMPLETE: SHAP summary graph saved at {} (elapsed time: {}s)'.format(self.img_save_path, self.visualization_timer.elapsed_time_str))
+        stdout_success(msg=f'SHAP summary graph saved at {self.img_save_path}', elapsed_time=self.visualization_timer.elapsed_time_str)
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/gantt_creator_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 import pandas as pd
 from simba.misc_tools import (detect_bouts,
                               concatenate_videos_in_folder,
                               SimbaTimer,
-                              get_named_colors)
+                              get_named_colors,
+                              stdout_success)
 from simba.read_config_unit_tests import (check_if_filepath_list_is_empty)
 from simba.feature_extractors.unit_tests import (read_video_info)
 from simba.enums import Formats
 from simba.plotting.misc_visualizations import make_gantt_plot
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df
 from simba.mixins.config_reader import ConfigReader
@@ -220,15 +221,15 @@
                 if self.video_setting:
                     print('Joining {} multiprocessed video...'.format(self.video_name))
                     concatenate_videos_in_folder(in_folder=self.temp_folder, save_path=self.save_video_path)
                 video_timer.stop_timer()
                 print('Gantt video {} complete (elapsed time: {}s) ...'.format(self.video_name, video_timer.elapsed_time_str))
 
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: Gantt visualizations for {} videos created in project_folder/frames/output/gantt_plots directory (elapsed time: {}s)'.format(str(len(self.files_found)), self.timer.elapsed_time_str))
+        stdout_success(msg=f'Gantt visualizations for {len(self.files_found)} videos created in project_folder/frames/output/gantt_plots directory', elapsed_time=self.timer.elapsed_time_str)
 
 # test = GanttCreatorMultiprocess(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                                 frame_setting=False,
 #                                 video_setting=True,
 #                                 files_found=['/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/machine_results/Together_1.csv'],
 #                                 cores=5,
 #                                 last_frm_setting=False,
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/heat_mapper_clf_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.misc_tools import (get_fn_ext,
                               SimbaTimer,
                               remove_a_folder,
-                              concatenate_videos_in_folder)
+                              concatenate_videos_in_folder,
+                              stdout_success)
 from simba.plotting.misc_visualizations import make_clf_heatmap_plot
 from simba.rw_dfs import read_df
 import numpy as np
 import os
 import cv2
 from numba import jit, prange
 from simba.enums import Formats
@@ -296,16 +297,15 @@
                     print('Joining {} multiprocessed video...'.format(self.video_name))
                     concatenate_videos_in_folder(in_folder=self.temp_folder, save_path=self.save_video_path)
 
                 video_timer.stop_timer()
                 print('Heatmap video {} complete (elapsed time: {}s) ...'.format(self.video_name, video_timer.elapsed_time_str))
 
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: heatmap visualizations for {} videos created in project_folder/frames/output/heatmap_classifier locations directory (elapsed time: {}s)'.format(str(len(self.files_found)), self.timer.elapsed_time_str))
-
+        stdout_success(msg='heatmap visualizations for {} videos created in project_folder/frames/output/heatmap_classifier locations directory', elapsed_time=self.timer.elapsed_time_str)
 
 
 # test = HeatMapperClfMultiprocess(config_path='/Users/simon/Desktop/envs/troubleshooting/Two_animals_16bps/project_folder/project_config.ini',
 #                      style_attr = {'palette': 'jet', 'shading': 'gouraud', 'bin_size': 100, 'max_scale': 'auto'},
 #                      final_img_setting=False,
 #                      video_setting=True,
 #                      frame_setting=False,
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/probability_plot_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Simon Nilsson"
 
 from simba.read_config_unit_tests import check_that_column_exist
 from simba.feature_extractors.unit_tests import read_video_info
-from simba.misc_tools import SimbaTimer
+from simba.misc_tools import SimbaTimer, stdout_success
 from simba.plotting.misc_visualizations import make_probability_plot
 import os
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df
 from simba.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 import matplotlib.pyplot as plt
@@ -133,15 +133,15 @@
                         self.writer.write(frame)
                     print('Probability frame: {} / {}. Video: {} ({}/{})'.format(str(i+1), str(len(data_df)), self.video_name, str(file_cnt + 1), len(self.files_found)))
                 if self.video_setting:
                     self.writer.release()
                 video_timer.stop_timer()
                 print('Probability plot for video {} saved (elapsed time: {}s)...'.format(self.video_name, video_timer.elapsed_time_str))
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: All probability visualizations created in project_folder/frames/output/probability_plots directory (elapsed time: {}s)'.format(self.timer.elapsed_time_str))
+        stdout_success(msg=f'All probability visualizations created in project_folder/frames/output/probability_plots directory', elapsed_time=self.timer.elapsed_time_str)
 
 
 #
 # test = TresholdPlotCreatorSingleProcess(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals/project_folder/project_config.ini',
 #                                         frame_setting=False,
 #                                         video_setting=True,
 #                                         last_image=True,
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/misc_visualizations.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/misc_visualizations.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import PIL
 import cv2
 import pandas as pd
 from matplotlib.backends.backend_agg import FigureCanvasAgg as FigureCanvas
 
 from simba.misc_tools import (get_color_dict,
                               get_named_colors,
-                              SimbaTimer)
+                              SimbaTimer,
+                              stdout_success)
 
 
 
 def make_distance_plot(data: np.array,
                        line_attr: dict,
                        style_attr: dict,
                        fps: int,
@@ -80,15 +81,15 @@
     img = np.uint8(cv2.cvtColor(np.asarray(img), cv2.COLOR_RGB2BGR))
     buffer_.close()
     plt.close()
     img = cv2.resize(img, (style_attr['width'], style_attr['height']))
     timer.stop_timer()
     if save_img:
         cv2.imwrite(save_path, img)
-        print('SIMBA COMPLETE: Final distance plot saved at {} (elapsed time: {}s)'.format(save_path, timer.elapsed_time_str))
+        stdout_success(f'Final distance plot saved at {save_path}', elapsed_time=timer.elapsed_time_str)
     else:
         return img
 
 def make_probability_plot(data: pd.Series,
                           style_attr: dict,
                           clf_name: str,
                           fps,
@@ -153,15 +154,15 @@
     img = cv2.cvtColor(ar, cv2.COLOR_RGB2BGR)
     img = np.uint8(cv2.resize(img, (style_attr['width'], style_attr['height'])))
     buffer_.close()
     plt.close()
 
     timer.stop_timer()
     cv2.imwrite(save_path, img)
-    print('SIMBA COMPLETE: Final distance plot saved at {} (elapsed time: {}s)'.format(save_path, timer.elapsed_time_str))
+    stdout_success(msg=f'Final distance plot saved at {save_path}', elapsed_time=timer.elapsed_time_str)
 
 
 def make_path_plot(data_df: pd.DataFrame,
                    video_info: pd.DataFrame,
                    style_attr: dict,
                    deque_dict: dict,
                    clf_attr: dict,
@@ -203,15 +204,15 @@
             locations = data_df.loc[sliced_df_idx, [animal_bp_x, animal_bp_y]].astype(int).values
             for i in range(locations.shape[0]):
                 cv2.circle(img, (locations[i][0], locations[i][1]), 0, clf_clr, clf_size)
 
     video_timer.stop_timer()
     img = cv2.resize(img, (style_attr['width'], style_attr['height']))
     cv2.imwrite(save_path, img)
-    print('SIMBA COMPLETE: Final path plot saved at {} (elapsed time: {}s)'.format(save_path, video_timer.elapsed_time_str))
+    stdout_success(msg=f'Final path plot saved at {save_path}', elapsed_time=video_timer.elapsed_time_str)
 
 def make_gantt_plot(data_df: pd.DataFrame,
                     bouts_df: pd.DataFrame,
                     clf_names: list,
                     fps: int,
                     style_attr: dict,
                     video_name: str,
@@ -246,16 +247,15 @@
         open_cv_image = cv2.cvtColor(ar, cv2.COLOR_RGB2BGR)
         open_cv_image = cv2.resize(open_cv_image, (style_attr['width'], style_attr['height']))
         frame = np.uint8(open_cv_image)
         buffer_.close()
         plt.close(fig)
         cv2.imwrite(save_path, frame)
         video_timer.stop_timer()
-        print('SIMBA COMPLETE: Final gantt frame for video {} saved at {} (elapsed time: {}s) ...'.format(video_name, save_path, video_timer.elapsed_time_str))
-
+        stdout_success(msg=f'Final gantt frame for video {video_name} saved at {save_path}', elapsed_time= video_timer.elapsed_time_str)
 
 def make_clf_heatmap_plot(frm_data: np.array,
                       max_scale: float,
                       palette: str,
                       aspect_ratio: float,
                       shading: str,
                       clf_name: str,
@@ -292,15 +292,15 @@
     mat = np.array(canvas.renderer._renderer)
     image = cv2.cvtColor(mat, cv2.COLOR_RGB2BGR)
     image = cv2.resize(image, img_size)
     image = np.uint8(image)
     plt.close()
     if final_img:
         cv2.imwrite(file_name, image)
-        print('SIMBA COMPLETE: Final classifier heatmap image saved at at {}...'.format(file_name))
+        stdout_success(msg=f'Final classifier heatmap image saved at at {file_name}')
     else:
         return image
 
 def make_location_heatmap_plot(frm_data: np.array,
                                max_scale: float,
                                palette: str,
                                aspect_ratio: float,
@@ -338,15 +338,15 @@
     mat = np.array(canvas.renderer._renderer)
     image = cv2.cvtColor(mat, cv2.COLOR_RGB2BGR)
     image = cv2.resize(image, img_size)
     image = np.uint8(image)
     plt.close()
     if final_img:
         cv2.imwrite(file_name, image)
-        print(f'SIMBA COMPLETE: Final location heatmap image saved at at {file_name}...')
+        stdout_success(msg=f'Final location heatmap image saved at at {file_name}')
     else:
         return image
 
 
 
 
 # style_attr = {'width': 'As input',
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/plot_clf_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from simba.read_config_unit_tests import (read_config_entry,
                                           check_file_exist_and_readable,
                                           check_float,
                                           check_int)
 from simba.misc_tools import (find_video_of_file,
                               get_video_meta_data)
 from simba.rw_dfs import read_df
-from simba.misc_tools import create_single_color_lst
+from simba.misc_tools import create_single_color_lst, stdout_success
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.drop_bp_cords import (createColorListofList,
                                  create_body_part_dictionary,
                                  get_fn_ext)
 from simba.enums import ReadConfig, Formats, Dtypes
 import os, glob
 from copy import deepcopy
@@ -196,15 +196,15 @@
             _, file_name, _ = get_fn_ext(file_path)
             self.file_path = os.path.join(self.machine_results_dir, file_name + '.' + self.file_type)
             self.files_found = [self.file_path]
             check_file_exist_and_readable(self.file_path)
             self.create_visualizations()
 
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: All visualizations created in project_folder/frames/output/sklearn_results directory (elapsed time: {}s)'.format(self.timer.elapsed_time_str))
+        stdout_success(msg='All visualizations created in project_folder/frames/output/sklearn_results directory', elapsed_time=self.timer.elapsed_time_str)
 
 # test = PlotSklearnResults(config_path='/Users/simon/Desktop/troubleshooting/train_model_project/project_folder/project_config.ini',
 #                           video_setting=True,
 #                           frame_setting=False,
 #                           video_file_path='/Users/simon/Desktop/troubleshooting/train_model_project/project_folder/videos/Together_1.avi',
 #                           print_timers=False)
 # test.initialize_visualizations()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/plot_clf_results_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
                                           check_float,
                                           check_int)
 from simba.misc_tools import (find_video_of_file,
                               get_video_meta_data,
                               concatenate_videos_in_folder)
 from simba.rw_dfs import read_df
 from simba.misc_tools import (create_single_color_lst,
-                              SimbaTimer)
+                              SimbaTimer,
+                              stdout_success)
 from simba.feature_extractors.unit_tests import (read_video_info_csv,
                                                read_video_info)
 from simba.drop_bp_cords import (getBpNames,
                                  createColorListofList,
                                  create_body_part_dictionary,
                                  get_fn_ext)
 
@@ -257,18 +258,17 @@
             self.file_path = os.path.join(self.machine_results_dir, file_name + '.' + self.file_type)
             self.files_found = [self.file_path]
             check_file_exist_and_readable(self.file_path)
             self.create_visualizations()
 
         self.timer.stop_timer()
         if self.video_setting:
-            print('SIMBA COMPLETE: {} videos saved in project_folder/frames/output/sklearn_results directory (elapsed time: {}s)'.format(len(self.files_found), self.timer.elapsed_time_str))
+            stdout_success(msg=f'{len(self.files_found)} videos saved in project_folder/frames/output/sklearn_results directory', elapsed_time=self.timer.elapsed_time_str)
         if self.frame_setting:
-            print('SIMBA COMPLETE: Frames for {} videos saved in sub-folders within project_folder/frames/output/sklearn_results directory. (elapsed time: {}s)'.format(len(self.files_found), self.timer.elapsed_time_str))
-
+            stdout_success(f'Frames for {len(self.files_found)} videos saved in sub-folders within project_folder/frames/output/sklearn_results directory', elapsed_time=self.timer.elapsed_time_str)
 
 # test = PlotSklearnResultsMultiProcess(config_path='/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/project_config.ini',
 #                                       video_setting=True,
 #                                       frame_setting=False,
 #                                       video_file_path='/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/videos/SF2.mp4',
 #                                       print_timers=True,
 #                                       text_settings=False,
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/ROI_feature_visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Simon Nilsson"
 
 from simba.read_config_unit_tests import check_file_exist_and_readable
 import os
-from simba.misc_tools import get_video_meta_data
+from simba.misc_tools import get_video_meta_data, stdout_success
 from simba.drop_bp_cords import (createColorListofList,
                                  create_body_part_dictionary,
                                  get_fn_ext)
 from simba.enums import Formats
 from simba.roi_tools.ROI_feature_analyzer import ROIFeatureCreator
 import cv2
 from simba.rw_dfs import read_df
@@ -215,15 +215,15 @@
 
             except:
                 break
 
         self.timer.stop_timer()
         self.cap.release()
         self.writer.release()
-        print('Feature video {} saved in {} directory ...(elapsed time: {}s)'.format(self.video_name, self.save_path, self.timer.elapsed_time_str))
+        stdout_success('Feature video {} saved in {} directory ...', elapsed_time=self.timer.elapsed_time_str)
 
 # style_attr = {'ROI_centers': True, 'ROI_ear_tags': True, 'Directionality': True, 'Border_color': (0, 128, 0), 'Pose_estimation': True}
 # test = ROIfeatureVisualizer(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', video_name='Together_1.avi', style_attr=style_attr)
 # test.create_visualization()
 
 
 # style_attr = {'ROI_centers': True, 'ROI_ear_tags': True, 'Directionality': True, 'Directionality_style': 'Line', 'Border_color': (0, 128, 0), 'Pose_estimation': True}
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/heat_mapper_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 __author__ = "Simon Nilsson", "JJ Choong"
 
 from simba.feature_extractors.unit_tests import read_video_info
-from simba.misc_tools import get_fn_ext, SimbaTimer
+from simba.misc_tools import (get_fn_ext,
+                              SimbaTimer,
+                              stdout_success)
 import os
 import cv2
 from simba.rw_dfs import read_df
 import numpy as np
 from numba import jit, prange
 import pandas as pd
 from simba.enums import Formats
@@ -197,17 +199,16 @@
                     print('Heatmap frame: {} / {}. Video: {} ({}/{})'.format(str(frm_cnt + 1), str(len(self.data_df)), self.video_name, str(file_cnt + 1), len(self.files_found)))
 
             if self.video_setting:
                 self.writer.release()
             video_timer.stop_timer()
             print(f'Heatmap plot for video {self.video_name} saved (elapsed time: {video_timer.elapsed_time_str}s')
         self.timer.stop_timer()
-        print(f'SIMBA COMPLETE: Created heatmaps for {str(len(self.files_found))} videos (elapsed time {self.timer.elapsed_time_str}s)')
 
-#
+        stdout_success(msg=f'Created heatmaps for {str(len(self.files_found))} videos', elapsed_time=self.timer.elapsed_time_str)
 #
 # test = HeatmapperLocationSingleCore(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                                       style_attr = {'palette': 'jet', 'shading': 'gouraud', 'bin_size': 100, 'max_scale': 'auto'},
 #                                       final_img_setting=False,
 #                                       video_setting=True,
 #                                       frame_setting=False,
 #                                       bodypart='Nose_1',
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/probability_plot_creator_mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 
 from simba.read_config_unit_tests import check_that_column_exist
 from simba.feature_extractors.unit_tests import read_video_info
 import functools
 import pandas as pd
 from simba.misc_tools import (SimbaTimer,
-                              concatenate_videos_in_folder)
+                              concatenate_videos_in_folder,
+                              stdout_success)
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.plotting.misc_visualizations import make_probability_plot
 from simba.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 import os
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df
@@ -195,16 +196,15 @@
                     print('Joining {} multiprocessed video...'.format(self.video_name))
                     concatenate_videos_in_folder(in_folder=self.temp_folder, save_path=self.save_video_path)
 
                 video_timer.stop_timer()
                 print('Probability video {} complete (elapsed time: {}s) ...'.format(self.video_name, video_timer.elapsed_time_str))
 
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: Probability visualizations for {} videos created in project_folder/frames/output/gantt_plots directory (elapsed time: {}s)'.format(str(len(self.files_found)), self.timer.elapsed_time_str))
-
+        stdout_success(msg=f'Probability visualizations for {str(len(self.files_found))} videos created in project_folder/frames/output/gantt_plots directory', elapsed_time=self.timer.elapsed_time_str)
 
 
 # test = TresholdPlotCreatorMultiprocess(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals/project_folder/project_config.ini',
 #                                         frame_setting=False,
 #                                         video_setting=True,
 #                                         last_frame=False,
 #                                         clf_name='Attack',
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/plot_pose_in_dir.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import os, glob
 from simba.drop_bp_cords import get_fn_ext
 from pathlib import Path
 from simba.misc_tools import (find_video_of_file,
                               get_video_meta_data,
                               create_single_color_lst,
                               get_color_dict,
-                              SimbaTimer)
+                              SimbaTimer,
+                              stdout_success)
 from simba.enums import Formats
 from simba.read_config_unit_tests import check_if_filepath_list_is_empty
 from simba.rw_dfs import read_df
 from simba.utils.errors import InvalidInputError
 
 
 ACCEPTED_DIRECTORIES = ['input_csv', 'outlier_corrected_movement', 'outlier_corrected_movement_location']
@@ -106,14 +107,14 @@
                 print('Video: {} / {} Frame: {} / {}'.format(str(video_cnt + 1), str(len(files_found)), str(frm_cnt), str(len(pose_df))))
             else:
                 break
         print('{} complete...'.format(file_name))
         cap.release()
         writer.release()
     timer.stop_timer()
-    print('SIMBA COMPLETE: All pose videos complete. Results located in {} directory (elapsed time: {}s)'.format(str(out_directory), timer.elapsed_time_str))
+    stdout_success(msg=f'All pose videos complete. Results located in {str(out_directory)} directory', elapsed_time=timer.elapsed_time_str)
 
 # create_video_from_dir(in_directory=r'/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/csv/features_extracted',
 #                       out_directory=r'/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/csv/features_extracted/test',
 #                       circle_size=5,
 #                       clr_attr=None)
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/single_run_model_validation_video.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 from simba.rw_dfs import *
 from simba.misc_tools import (find_video_of_file,
                               get_fn_ext,
                               get_video_meta_data,
                               plug_holes_shortest_bout,
                               get_bouts_for_gantt,
                               create_gantt_img,
-                              resize_gantt)
+                              resize_gantt,
+                              stdout_success)
 from simba.feature_extractors.unit_tests import read_video_info
 plt.interactive(True)
 plt.ioff()
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
 class ValidateModelOneVideo(ConfigReader):
     """
@@ -150,15 +151,15 @@
             print('SIMBA WARNING: Some frames appear to be missing in the video vs the data file.')
             cap.release()
             writer.release()
 
         cap.release()
         writer.release()
         self.timer.stop_timer()
-        print(f'SIMBA COMPLETE: Validation video saved at {self.vid_output_path} (elapsed time: {self.timer.elapsed_time_str}s)')
+        stdout_success(msg=f'Validation video saved at {self.vid_output_path}', elapsed_time=self.timer.elapsed_time_str)
 
     def run(self):
         self.__run_clf()
         if self.shortest_bout > 1:
             self.__plug_bouts()
         self.__save()
         self.__create_video()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from simba.read_config_unit_tests import (read_config_file,
                                           read_config_entry)
 import os
 import subprocess, shutil
 from simba.misc_tools import (get_video_meta_data,
                               remove_a_folder,
                               get_fn_ext,
-                              SimbaTimer)
+                              SimbaTimer,
+                              stdout_success)
 from datetime import datetime
 from simba.enums import Paths, ReadConfig
 
 
 class FrameMergererFFmpeg(object):
     """
     Class for merging separate visualizations of classifications, descriptive statistics etc., into  single
@@ -133,15 +134,15 @@
         for video_type in frames_dict.keys():
             video_path_str += ' -i "{}"'.format(os.path.join(self.temp_dir, video_type + '.mp4'))
         cmd = 'ffmpeg -y{} -filter_complex hstack=inputs={} -vsync 2 "{}"'.format(video_path_str, str(len(frames_dict.keys())), out_path)
         print('Concatenating (horizontal) {} videos...'.format(str(len(frames_dict.keys()))))
         subprocess.call(cmd, shell=True, stdout=subprocess.PIPE)
         if final_img:
             self.timer.stop_timer()
-            print('SIMBA COMPLETE: Merged video saved at {} (elapsed time: {}s)'.format(out_path, self.timer.elapsed_time_str))
+            stdout_success(msg=f'Merged video saved at {out_path}', elapsed_time=self.timer.elapsed_time_str)
 
     def __vertical_concatenator(self,
                                 frames_dict: dict,
                                 out_path: str,
                                 include_resize=True,
                                 final_img=True):
         """ Helper to vertically concatenate N videos """
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
                                  create_body_part_dictionary)
 from simba.misc_tools import (find_video_of_file,
                               get_video_meta_data,
                               SimbaTimer,
                               get_color_dict,
                               split_and_group_df,
                               remove_a_folder,
-                              concatenate_videos_in_folder)
+                              concatenate_videos_in_folder,
+                              stdout_success)
 import cv2
 import numpy as np
 import random
 from simba.rw_dfs import read_df
 import platform
 import multiprocessing
 import functools
@@ -213,16 +214,15 @@
             for cnt, result in enumerate(pool.imap(constants, data_arr, chunksize=self.multiprocess_chunksize)):
                 print('Image {}/{}, Video {}...'.format(str(int(frm_per_core * (result + 1))), str(len(self.data_df)), self.video_name))
 
             concatenate_videos_in_folder(in_folder=self.save_temp_path, save_path=self.save_path, video_format='mp4')
             video_timer.stop_timer()
             pool.terminate()
             pool.join()
-            print('SIMBA COMPLETE: Video {} created. Video saved in project_folder/frames/output/ROI_directionality_visualize (elapsed time: {}s).'.format(self.video_name, video_timer.elapsed_time_str))
-
+            stdout_success(msg=f'Video {self.video_name} created. Video saved in project_folder/frames/output/ROI_directionality_visualize', elapsed_time=self.timer.elapsed_time_str)
 
 # style_attr = {'Show_pose': True, 'Pose_circle_size': 3, "Direction_color": 'Random', 'Direction_thickness': 4, 'Highlight_endpoints': True, 'Polyfill': True}
 # test = DirectingOtherAnimalsVisualizerMultiprocess(config_path='/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/project_config.ini',
 #                                        data_path='/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/csv/outlier_corrected_movement_location/Testing_Video_3.csv',
 #                                        style_attr=style_attr,
 #                                                    core_cnt=5)
 #
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/clf_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 __author__ = "Simon Nilsson"
 
-
 from simba.read_config_unit_tests import (check_int,
                                           check_that_column_exist,
                                           check_if_filepath_list_is_empty)
 from simba.misc_tools import (find_video_of_file,
                               get_file_path_parts,
                               detect_bouts,
-                              get_video_meta_data)
+                              get_video_meta_data,
+                              stdout_success)
 from simba.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.rw_dfs import read_df
 import numpy as np
 import os
 import cv2
@@ -146,15 +146,15 @@
                 if self.clips:
                     bout_writer.release()
                 if self.concat_video:
                     self.__insert_inter_frms()
             if self.concat_video:
                 self.concat_writer.release()
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: All validation clips complete. Files are saved in the project_folder/frames/output/classifier_validation directory of the SimBA project (elapsed time: {}s)'.format(self.timer.elapsed_time_str))
+        stdout_success(msg='All validation clips complete. Files are saved in the project_folder/frames/output/classifier_validation directory of the SimBA project', elapsed_time=self.timer.elapsed_time_str)
 
 # test = ClassifierValidationClips(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                                  window=1,
 #                                  clf_name='Attack',
 #                                  clips=False,
 #                                  concat_video=True,
 #                                  text_clr=(0, 0, 255))
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/path_plotter_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from copy import deepcopy
 from collections import deque
 from simba.misc_tools import (get_fn_ext,
                               SimbaTimer,
                               get_color_dict,
                               remove_a_folder,
                               concatenate_videos_in_folder,
-                              find_animal_name_from_body_part_name)
+                              find_animal_name_from_body_part_name,
+                              stdout_success)
 from simba.enums import Formats
 from numba import jit, prange
 from simba.plotting.misc_visualizations import make_path_plot
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.rw_dfs import read_df
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import NoSpecifiedOutputError
@@ -220,15 +221,15 @@
                     print('Joining {} multiprocessed video...'.format(self.video_name))
                     concatenate_videos_in_folder(in_folder=self.temp_folder, save_path=self.save_video_path)
 
                 video_timer.stop_timer()
                 print('Path plot video {} complete (elapsed time: {}s) ...'.format(self.video_name,video_timer.elapsed_time_str))
 
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: Path plot visualizations for {} videos created in project_folder/frames/output/path_plots directory (elapsed time: {}s)'.format(str(len(self.files_found)), self.timer.elapsed_time_str))
+        stdout_success(msg=f'Path plot visualizations for {str(len(self.files_found))} videos created in project_folder/frames/output/path_plots directory', elapsed_time=self.timer.elapsed_time_str)
 
     @staticmethod
     @jit(nopython=True)
     def __split_array_into_max_lines(data: np.array,
                                      max_lines: int):
 
         results = np.full((data.shape[0], max_lines, data.shape[1]), np.nan, data.dtype)
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import os
 from simba.feature_extractors.unit_tests import read_video_info_csv
 from simba.misc_tools import (check_multi_animal_status,
                               get_video_meta_data,
                               SimbaTimer,
                               split_and_group_df,
                               remove_a_folder,
-                              concatenate_videos_in_folder)
+                              concatenate_videos_in_folder,
+                              stdout_success)
 from simba.drop_bp_cords import (getBpNames,
                                  createColorListofList,
                                  create_body_part_dictionary,
                                  get_fn_ext)
 from simba.enums import Formats, Paths
 from simba.roi_tools.ROI_feature_analyzer import ROIFeatureCreator
 import cv2
@@ -300,17 +301,17 @@
 
             print('Joining {} multiprocessed video...'.format(self.video_name))
             concatenate_videos_in_folder(in_folder=self.save_temp_dir, save_path=self.save_path, video_format='mp4')
 
             self.timer.stop_timer()
             pool.terminate()
             pool.join()
-            print('Video {} complete (elapsed time: {}s). Video saved in project_folder/frames/output/ROI_features.'.format(self.video_name, self.timer.elapsed_time_str))
+            stdout_success(msg=f'Video {self.video_name} complete. Video saved in project_folder/frames/output/ROI_features.', elapsed_time=self.timer.elapsed_time_str)
 
 
 # style_attr = {'ROI_centers': True, 'ROI_ear_tags': True, 'Directionality': True, 'Directionality_style': 'Funnel', 'Border_color': (0, 128, 0), 'Pose_estimation': True}
 # roi_feature_visualizer = ROIfeatureVisualizerMultiprocess(config_path='/Users/simon/Desktop/envs/simba_dev/tests/test_data/mouse_open_field/project_folder/project_config.ini', video_name='Video1.mp4', style_attr=style_attr, core_cnt=3)
 # roi_feature_visualizer.create_visualization()
-
+#
 # style_attr = {'ROI_centers': True, 'ROI_ear_tags': True, 'Directionality': True, 'Directionality_style': 'Funnel', 'Border_color': (0, 128, 0), 'Pose_estimation': True}
 # test = ROIfeatureVisualizerMultiprocess(config_path='/Users/simon/Desktop/envs/simba_dev/tests/test_data/mouse_open_field/project_folder/project_config.ini', video_name='Video1.mp4', style_attr=style_attr, core_cnt=5)
 # test.create_visualization()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/data_plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from joblib import Parallel, delayed
 import os
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.movement_processor import MovementProcessor
 from simba.misc_tools import (check_multi_animal_status,
                               get_fn_ext,
                               SimbaTimer,
-                              get_color_dict)
+                              get_color_dict,
+                              stdout_success)
 import numpy as np
 import cv2
 from simba.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import NoSpecifiedOutputError
 
 
@@ -157,15 +158,15 @@
             print('Data tables created for video {}...'.format(video_name))
             if self.video_setting:
                 self.writer.release()
                 video_timer.stop_timer()
                 print('Video {} complete (elapsed time {}s)...'.format(video_name, video_timer.elapsed_time_str))
 
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: All data table videos created inside {} (elapsed time: {}s)'.format(self.data_table_path, self.timer.elapsed_time_str))
+        stdout_success(msg=f'All data table videos created inside {self.data_table_path}', elapsed_time=self.timer.elapsed_time_str)
 
 # style_attr = {'bg_color': 'White', 'header_color': 'Black', 'font_thickness': 1, 'size': (640, 480), 'data_accuracy': 2}
 # body_part_attr = [['Ear_left_1', 'Grey'], ['Ear_right_2', 'Red']]
 # data_paths = ['/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/machine_results/Together_1.csv']
 #
 #
 # test = DataPlotter(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/path_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import cv2
 
 from simba.read_config_unit_tests import check_if_filepath_list_is_empty
 from collections import deque
 from simba.misc_tools import (get_fn_ext,
                               SimbaTimer,
-                              get_color_dict)
+                              get_color_dict,
+                              stdout_success)
 from simba.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 from simba.plotting.misc_visualizations import make_path_plot
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.misc_tools import find_animal_name_from_body_part_name
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.rw_dfs import read_df
@@ -153,15 +154,15 @@
 
                 if self.video_setting:
                     self.writer.release()
                 video_timer.stop_timer()
                 print('Path visualization for video {} saved (elapsed time {}s)...'.format(self.video_name, video_timer.elapsed_time_str))
 
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: Path visualizations for {} videos saved in project_folder/frames/output/path_plots directory (elapsed time {}s)'.format(str(len(self.files_found)), self.timer.elapsed_time_str))
+        stdout_success(msg=f'Path visualizations for {str(len(self.files_found))} videos saved in project_folder/frames/output/path_plots directory', elapsed_time=self.timer.elapsed_time_str)
 
     def __get_styles(self):
         self.color_dict = get_color_dict()
         if self.style_attr is not None:
             self.style_attr['bg color'] = self.color_dict[self.style_attr['bg color']]
             self.style_attr['max lines'] = int(self.style_attr['max lines'] * (int(self.video_info['fps'].values[0]) / 1000))
             if self.style_attr['width'] == 'As input':
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/ez_lineplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import os
 import cv2
 import numpy as np
 from simba.drop_bp_cords import get_fn_ext
 import pandas as pd
 from simba.misc_tools import (get_video_meta_data,
                               get_color_dict,
-                              SimbaTimer)
+                              SimbaTimer,
+                              stdout_success)
 from simba.read_config_unit_tests import read_config_file
 from simba.rw_dfs import read_df
 from copy import deepcopy
 
 class DrawPathPlot(object):
     def __init__(self,
                  data_path: str,
@@ -82,15 +83,15 @@
                 print('Frame {}/{}'.format(str(frm_counter), str(self.video_meta_data['frame_count'])))
 
             else:
                 break
 
         self.cap.release()
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: Path plot saved at {} (elapsed time: {}s)'.format(self.save_name, self.timer.elapsed_time_str))
+        stdout_success(msg=f'Path plot saved at {self.save_name}', elapsed_time=self.timer.elapsed_time_str)
 
 def draw_line_plot(configini, video, bodypart):
     configFile = str(configini)
     config = read_config_file(configini)
     configdir = os.path.dirname(configini)
     wfileType = 'csv'
     dir_path, vid_name, ext = get_fn_ext(video)
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/distance_plotter_mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from simba.read_config_unit_tests import check_if_filepath_list_is_empty
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.misc_tools import (get_fn_ext,
                               SimbaTimer,
                               get_color_dict,
                               remove_a_folder,
-                              concatenate_videos_in_folder)
+                              concatenate_videos_in_folder,
+                              stdout_success)
 
 from simba.plotting.misc_visualizations import make_distance_plot
 from simba.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 from simba.rw_dfs import read_df
 import numpy as np
 import matplotlib.pyplot as plt
@@ -216,15 +217,15 @@
                     print('Joining {} multiprocessed video...'.format(self.video_name))
                     concatenate_videos_in_folder(in_folder=self.temp_folder, save_path=self.save_video_path)
 
                 video_timer.stop_timer()
                 print('Distance line chart video {} complete (elapsed time: {}s) ...'.format(self.video_name,video_timer.elapsed_time_str))
 
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: Distance plot visualizations for {} videos created in project_folder/frames/output/line_plot directory (elapsed time: {}s)'.format(str(len(self.files_found)), self.timer.elapsed_time_str))
+        stdout_success(f'Distance plot visualizations for {str(len(self.files_found))} videos created in project_folder/frames/output/line_plot directory', elapsed_time=self.timer.elapsed_time_str)
 
     @staticmethod
     @jit(nopython=True)
     def __insert_group_idx_column(data: np.array,
                                   group: int):
         group_col = np.full((data.shape[0], 1), group)
         return np.hstack((group_col, data))
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/ROI_plotter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 __author__ = "Simon Nilsson"
 
 from simba.roi_tools.ROI_analyzer import ROIAnalyzer
 from simba.drop_bp_cords import get_fn_ext, createColorListofList
 from simba.feature_extractors.unit_tests import read_video_info
-import pandas as pd
 import os
 import itertools
 import cv2
 from simba.enums import Paths, Formats
 from simba.misc_tools import (get_video_meta_data,
                               add_missing_ROI_cols,
-                              SimbaTimer)
+                              SimbaTimer,
+                              stdout_success)
 import numpy as np
 from simba.utils.errors import NoFilesFoundError
 
 
 class ROIPlot(object):
     """
     Class for visualizing the ROI data (number of entries/exits, time-spent-in etc)
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/heat_mapper_clf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.misc_tools import (get_fn_ext,
-                              SimbaTimer)
+                              SimbaTimer,
+                              stdout_success)
 from simba.plotting.misc_visualizations import make_clf_heatmap_plot
 from simba.rw_dfs import read_df
 import numpy as np
 import os
 import cv2
 from numba import jit, prange
 import matplotlib.pyplot as plt
@@ -238,15 +239,15 @@
                 if self.video_setting:
                     self.writer.release()
 
                 video_timer.stop_timer()
                 print('Heatmap plot for video {} saved (elapsed time: {}s) ... '.format(self.video_name, video_timer.elapsed_time_str))
 
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: All heatmap visualizations created in project_folder/frames/output/heatmaps_classifier_locations directory (elapsed time: {}s)'.format(self.timer.elapsed_time_str))
+        stdout_success(msg='All heatmap visualizations created in project_folder/frames/output/heatmaps_classifier_locations directory', elapsed_time='self.timer.elapsed_time_str')
 
 # test = HeatMapperClfSingleCore(config_path='/Users/simon/Desktop/envs/troubleshooting/Two_animals_16bps/project_folder/project_config.ini',
 #                      style_attr = {'palette': 'jet', 'shading': 'gouraud', 'bin_size': 75, 'max_scale': 'auto'},
 #                      final_img_setting=False,
 #                      video_setting=True,
 #                      frame_setting=False,
 #                      bodypart='Nose_1',
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/distance_plotter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 __author__ = "Simon Nilsson"
 
 from simba.read_config_unit_tests import check_if_filepath_list_is_empty
 from simba.feature_extractors.unit_tests import (read_video_info)
 from simba.misc_tools import (get_fn_ext,
                               SimbaTimer,
-                              get_color_dict)
+                              get_color_dict,
+                              stdout_success)
 
 from simba.plotting.misc_visualizations import make_distance_plot
 
 from simba.enums import Formats
 from simba.rw_dfs import read_df
 import numpy as np
 import matplotlib.pyplot as plt
@@ -140,16 +141,15 @@
                     print('Distance frame: {} / {}. Video: {} ({}/{})'.format(str(i+1), str(len(self.data_df)), self.video_name, str(file_cnt + 1), len(self.files_found)))
 
                 if self.video_setting:
                     writer.release()
                 video_timer.stop_timer()
                 print('Distance plot for video {} saved (elapsed time: {}s)...'.format(self.video_name, video_timer.elapsed_time_str))
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: All distance visualizations created in project_folder/frames/output/line_plot directory (elapsed time: {}s)'.format(self.timer.elapsed_time_str))
-
+        stdout_success(msg='All distance visualizations created in project_folder/frames/output/line_plot directory', elapsed_time=self.timer.elapsed_time_str)
 
 # style_attr = {'width': 640, 'height': 480, 'line width': 6, 'font size': 8, 'y_max': 'auto', 'opacity': 0.9}
 # line_attr = {0: ['Center_1', 'Center_2', 'Green'], 1: ['Ear_left_2', 'Ear_left_1', 'Red']}
 #
 # test = DistancePlotterSingleCore(config_path=r'/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                        frame_setting=False,
 #                        video_setting=True,
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 from simba.rw_dfs import *
 from simba.misc_tools import (find_video_of_file,
                               get_fn_ext,
                               get_video_meta_data,
                               plug_holes_shortest_bout,
                               get_bouts_for_gantt,
                               create_gantt_img,
-                              resize_gantt)
+                              resize_gantt,
+                              stdout_success)
 from matplotlib.backends.backend_agg import FigureCanvasAgg as FigureCanvas
 from simba.misc_tools import concatenate_videos_in_folder
 from simba.feature_extractors.unit_tests import read_video_info
 import platform
 import functools
 import multiprocessing
 import matplotlib
@@ -232,15 +233,15 @@
             for cnt, result in enumerate(pool.imap(constants, data, chunksize=self.multiprocess_chunksize)):
                 print('Image {}/{}, Video {}...'.format(str(int(frm_per_core * (result+1))), str(len(self.data_df)), self.feature_filename))
             print('Joining {} multiprocessed video...'.format(self.feature_filename))
         concatenate_videos_in_folder(in_folder=self.temp_dir, save_path=self.video_save_path)
         self.timer.stop_timer()
         pool.terminate()
         pool.join()
-        print(f'SIMBA COMPLETE: Video {self.feature_filename} complete (elapsed time: {self.timer.elapsed_time_str}s).')
+        stdout_success(msg=f'Video {self.feature_filename} complete', elapsed_time=self.timer.elapsed_time_str)
 
     def run(self):
         self.__run_clf()
         if self.shortest_bout > 1:
             self.__plug_bouts()
         self.__save()
         self.__create_video()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/Directing_animals_visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 from simba.Directing_animals_analyzer import DirectingOtherAnimalsAnalyzer
 import os
 from simba.drop_bp_cords import (get_fn_ext, createColorListofList, create_body_part_dictionary)
 from simba.misc_tools import (find_video_of_file,
                               get_video_meta_data,
                               SimbaTimer,
-                              get_color_dict)
+                              get_color_dict,
+                              stdout_success)
 import cv2
 import numpy as np
 import random
 from simba.rw_dfs import read_df
 from simba.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 
@@ -157,19 +158,16 @@
                     self.writer.release()
                     break
 
             except IndexError:
                 self.cap.release()
                 self.writer.release()
 
-
-
         video_timer.stop_timer()
-        print(f'Directionality video {self.video_name} saved in {self.directing_animals_video_output_path} directory (elapsed time: {self.timer.elapsed_time_str}s) ...')
-
+        stdout_success(msg=f'Directionality video {self.video_name} saved in {self.directing_animals_video_output_path} directory', elapsed_time=self.timer.elapsed_time_str)
 
 # style_attr = {'Show_pose': True, 'Pose_circle_size': 3, "Direction_color": 'Random', 'Direction_thickness': 4, 'Highlight_endpoints': True, 'Polyfill': True}
 # test = DirectingOtherAnimalsVisualizer(config_path='/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/project_config.ini',
 #                                        data_path='/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/csv/outlier_corrected_movement_location/Testing_Video_3.csv',
 #                                        style_attr=style_attr)
 #
 # test.run()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.55.7/simba/plotting/heat_mapper_location_mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 __author__ = "Simon Nilsson", "JJ Choong"
 
 import pandas as pd
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.misc_tools import (get_fn_ext,
                               SimbaTimer,
                               remove_a_folder,
-                              concatenate_videos_in_folder)
+                              concatenate_videos_in_folder,
+                              stdout_success)
 from simba.plotting.misc_visualizations import make_location_heatmap_plot
 from simba.rw_dfs import read_df
 import numpy as np
 import os
 import cv2
 from numba import jit, prange
 from simba.enums import Formats
@@ -292,16 +293,15 @@
                     print('Joining {} multiprocessed heatmap location video...'.format(self.video_name))
                     concatenate_videos_in_folder(in_folder=self.temp_folder, save_path=self.save_video_path)
 
                 video_timer.stop_timer()
                 print('Heatmap video {} complete (elapsed time: {}s) ...'.format(self.video_name, video_timer.elapsed_time_str))
 
             self.timer.stop_timer()
-            print('SIMBA COMPLETE: Heatmap location videos visualizations for {} videos created in project_folder/frames/output/heatmaps_locations directory (elapsed time: {}s)'.format(str(len(self.files_found)), self.timer.elapsed_time_str))
-
+            stdout_success(msg='Heatmap location videos visualizations for {} videos created in project_folder/frames/output/heatmaps_locations directory', elapsed_time=self.timer.elapsed_time_str)
 
 # test = HeatMapperLocationMultiprocess(config_path='/Users/simon/Desktop/envs/troubleshooting/locomotion/project_folder/project_config.ini',
 #                                       style_attr = {'palette': 'jet', 'shading': 'gouraud', 'bin_size': 50, 'max_scale': 'auto'},
 #                                       final_img_setting=False,
 #                                       video_setting=True,
 #                                       frame_setting=False,
 #                                       bodypart='Nose',
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.55.7/simba/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/interpolate_smooth_post_hoc.py` & `Simba-UW-tf-dev-1.55.7/simba/interpolate_smooth_post_hoc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from scipy.signal import savgol_filter
 from simba.mixins.config_reader import ConfigReader
-from simba.misc_tools import check_if_filepath_list_is_empty, SimbaTimer, get_fn_ext, get_video_meta_data, find_video_of_file
+from simba.misc_tools import (check_if_filepath_list_is_empty,
+                              SimbaTimer,
+                              get_fn_ext,
+                              get_video_meta_data,
+                              find_video_of_file,
+                              stdout_success)
 import glob, os
 from simba.rw_dfs import read_df, save_df
 import numpy as np
 import shutil
 
 class PostHocInterpolate(ConfigReader):
     def __init__(self,
@@ -20,15 +25,15 @@
         self.files_found = glob.glob(input_dir + '/*.' + self.file_type)
         check_if_filepath_list_is_empty(filepaths=self.files_found, error_msg=f"SIMBA ERROR: {input_dir} does not contain any {self.file_type} files.")
         if self.interpolation_type == 'Animal(s)':
             self.animal_interpolator()
         if self.interpolation_type == 'Body-parts':
             self.body_part_interpolator()
         self.timer.stop_timer()
-        print(f'SIMBA COMPLETE: {str(len(self.files_found))} data file(s) interpolated (elapsed time {self.timer.elapsed_time_str}s).')
+        stdout_success(msg=f'{str(len(self.files_found))} data file(s) interpolated)', elapsed_time=self.timer.elapsed_time_str)
 
     def animal_interpolator(self):
         for file_path in self.files_found:
             video_timer = SimbaTimer()
             video_timer.start_timer()
             _, video_name, _ = get_fn_ext(filepath=file_path)
             df = read_df(file_path=file_path, file_type=self.file_type)
@@ -74,15 +79,15 @@
         self.files_found = glob.glob(input_dir + '/*.' + self.file_type)
         check_if_filepath_list_is_empty(filepaths=self.files_found, error_msg=f"SIMBA ERROR: {input_dir} does not contain any {self.file_type} files.")
         if smoothing_method == 'Savitzky Golay':
             self.savgol_smoother()
         if smoothing_method == 'Gaussian':
             self.gaussian_smoother()
         self.timer.stop_timer()
-        print(f'SIMBA COMPLETE: {str(len(self.files_found))} data file(s) smoothened (elapsed time {self.timer.elapsed_time_str}s).')
+        stdout_success(msg=f'{str(len(self.files_found))} data file(s) smoothened', elapsed_time=self.timer.elapsed_time_str)
 
     def savgol_smoother(self):
         for file_path in self.files_found:
             video_timer = SimbaTimer()
             video_timer.start_timer()
             _, video_name, _ = get_fn_ext(filepath=file_path)
             df = read_df(file_path=file_path, file_type=self.file_type)
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/dash_app.py` & `Simba-UW-tf-dev-1.55.7/simba/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/reverse_tracking_order.py` & `Simba-UW-tf-dev-1.55.7/simba/reverse_tracking_order.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/concatenator_pop_up.py` & `Simba-UW-tf-dev-1.55.7/simba/concatenator_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/extract_annotation_frames.py` & `Simba-UW-tf-dev-1.55.7/simba/extract_annotation_frames.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os.path
-
 from simba.mixins.config_reader import ConfigReader
 from simba.misc_tools import (find_video_of_file,
                               get_fn_ext,
-                              get_video_meta_data)
+                              get_video_meta_data,
+                              stdout_success)
 from simba.read_config_unit_tests import check_that_column_exist
 from simba.rw_dfs import read_df
 from simba.enums import Dtypes
 from simba.utils.errors import FrameRangeError
 import cv2
 
 
@@ -40,13 +40,12 @@
                     if not ret:
                         raise FrameRangeError(msg=f'Frame {str(frm+1)} is annotated as {clf} present. But frame {str(frm+1)} does not exist in video file {video_path}. The video file contains {video_meta_data["frame_count"]} frames.')
                     if self.settings['downsample'] != Dtypes.NONE.value:
                         img = cv2.resize(img, (int(img.shape[1] / self.settings['downsample']), int((img.shape[0] / self.settings['downsample']))), cv2.INTER_NEAREST)
                     cv2.imwrite(os.path.join(save_dir, f'{str(frm)}.png'), img)
                     print(f'Saved {clf} annotated img ({str(frm_cnt)}/{str(len(annot_idx))}), Video: {video_name}')
         self.timer.stop_timer()
-        print(f'SIMBA COMPLETE: Annotated frames saved in {self.annotated_frm_dir} directory (elapsed time {self.timer.elapsed_time_str}s)')
-
+        stdout_success(msg=f'Annotated frames saved in {self.annotated_frm_dir} directory', elapsed_time=self.timer.elapsed_time_str)
 # test = AnnotationFrameExtractor(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                                 clfs=['Sniffing', 'Attack'],
 #                                 settings={'downsample': 2})
 # test.run()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,16 @@
                                           read_project_path_and_file_type)
 from simba.feature_extractors.unit_tests import (read_video_info_csv,
                                                read_video_info)
 import os
 import pandas as pd
 from simba.roi_tools.ROI_analyzer import ROIAnalyzer
 from simba.misc_tools import (get_fn_ext,
-                              SimbaTimer)
+                              SimbaTimer,
+                              stdout_success)
 from simba.enums import ReadConfig, Paths, DirNames, Dtypes
 from simba.rw_dfs import read_df
 import itertools
 
 class ROITimebinCalculator(object):
     """
     Class for calulating how much time and how many entries animals are making into user-defined ROIs
@@ -92,23 +93,23 @@
         for video_name, video_data in self.out_dict_time.items():
             for shape_name, shape_data in video_data.items():
                 for animal_name, animal_data in shape_data.items():
                     for bin_name, bin_data in animal_data.items():
                         results_time_df.loc[len(results_time_df)] = [video_name, shape_name, animal_name, bin_name, bin_data]
         results_time_df['TIME INSIDE SHAPE (S)'] = results_time_df['TIME INSIDE SHAPE (S)'].round(6)
         results_time_df.to_csv(self.save_path_time)
-        print('SIMBA COMPLETE: ROI time bin time data saved at {}'.format(self.save_path_time))
+        stdout_success(msg=f'ROI time bin time data saved at {self.save_path_time}')
         for video_name, video_data in self.out_dict_entries.items():
             for shape_name, shape_data in video_data.items():
                 for animal_name, animal_data in shape_data.items():
                     for bin_name, bin_data in animal_data.items():
                         results_entries_df.loc[len(results_entries_df)] = [video_name, shape_name, animal_name, bin_name, bin_data]
         results_entries_df.to_csv(self.save_path_entries)
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: ROI time bin entry data saved at {} (elapsed time {}s)'.format(self.save_path_entries, self.timer.elapsed_time_str))
+        stdout_success(msg=f'ROI time bin entry data saved at {self.save_path_entries}', elapsed_time=self.timer.elapsed_time_str)
 
 
 # test = ROITimebinCalculator(config_path='/Users/simon/Desktop/troubleshooting/train_model_project/project_folder/project_config.ini',bin_length=5)
 # test.analyze_time_bins()
 # test.save_results()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 __author__ = "Simon Nilsson", "JJ Choong"
 
 
 from datetime import datetime
-from simba.read_config_unit_tests import (read_config_entry,
-                                          read_config_file,
+from simba.read_config_unit_tests import (read_config_file,
                                           read_project_path_and_file_type)
-from simba.misc_tools import SimbaTimer
-import pandas as pd
+from simba.misc_tools import SimbaTimer, stdout_success
 import os
-from simba.enums import ReadConfig
-from simba.ROI_analyzer import ROIAnalyzer
+from simba.roi_tools.ROI_analyzer import ROIAnalyzer
 
 class ROIMovementAnalyzer(object):
     """
 
     Class for computing movements of individual animals within individual user-defined ROIs.
 
     Parameters
@@ -48,13 +45,13 @@
         Save ROI movement analysis. Results are stored in the ``project_folder/logs`` directory
         of the SimBA project.
 
         Returns
         ----------
         None
         """
-        save_path = os.path.join(self.roi_analyzer.logs_path, 'ROI_movement_data_' + self.roi_analyzer.timestamp + '.csv')
+        save_path = os.path.join(self.roi_analyzer.logs_path, 'ROI_movement_data_' + self.roi_analyzer.datetime + '.csv')
         self.roi_analyzer.movements_df.to_csv(save_path)
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: ROI movement data saved in the "project_folder/logs/" directory (elapsed time: {}s)'.format(self.timer.elapsed_time_str))
+        stdout_success('ROI movement data saved in the "project_folder/logs/" directory', elapsed_time=self.timer.elapsed_time_str)
 
 #test = ROIMovementAnalyzer(config_path='/Users/simon/Desktop/train_model_project/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 __author__ = "Simon Nilsson", "JJ Choong"
 
 import os, glob, itertools
 import numpy as np
 from shapely.geometry import Point, Polygon
 from simba.drop_bp_cords import getBpHeaders, get_fn_ext
-from simba.rw_dfs import read_df, save_df
+from simba.rw_dfs import read_df
 import pandas as pd
-from simba.misc_tools import find_animal_name_from_body_part_name
+from simba.misc_tools import (find_animal_name_from_body_part_name,
+                              stdout_success)
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.enums import Paths, Keys, ReadConfig, Dtypes
 from simba.mixins.config_reader import ConfigReader
 from simba.read_config_unit_tests import read_config_entry
 from simba.utils.errors import NoFilesFoundError, NoROIDataError
 
 class ROIAnalyzer(ConfigReader):
@@ -296,22 +297,21 @@
         -------
         None
         """
 
         self.entries_df.to_csv(os.path.join(self.logs_path, f'{"ROI_entry_data"}_{self.datetime}.csv'))
         self.time_df.to_csv(os.path.join(self.logs_path, f'{"ROI_time_data"}_{self.datetime}.csv'))
         self.detailed_df.to_csv(os.path.join(self.logs_path, f'{"Detailed_ROI_data"}_{self.datetime}.csv'))
-        print('SIMBA COMPLETE: ROI time, ROI entry, and Detailed ROI data, have been saved in the "project_folder/logs/" directory in CSV format.')
-
+        stdout_success(msg='ROI time, ROI entry, and Detailed ROI data, have been saved in the "project_folder/logs/" directory in CSV format.')
         if self.calculate_distances:
             self.movements_df.to_csv(os.path.join(self.logs_path, f'{"ROI_movement_data"}_{self.datetime}.csv'))
             print('ROI movement data saved in the "project_folder/logs/" directory')
 
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: ROI analysis complete (elapsed time: {}s)'.format(self.timer.elapsed_time_str))
+        stdout_success(msg='ROI analysis complete', elapsed_time=self.timer.elapsed_time_str)
 
 
 # settings = {'body_parts': {'animal_1_bp': 'Ear_left_1', 'animal_2_bp': 'Ear_left_2', 'animal_3_bp': 'Ear_right_1',}, 'threshold': 0.4}
 # test = ROIAnalyzer(ini_path = r"/Users/simon/Desktop/envs/troubleshooting/two_animals_16bp_032023/project_folder/project_config.ini",
 #                    data_path = "outlier_corrected_movement_location",
 #                    settings=settings,
 #                    calculate_distances=True)
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from simba.roi_tools.ROI_directing_analyzer import DirectingROIAnalyzer
 import numpy as np
 import os, glob
 from simba.rw_dfs import read_df, save_df
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.misc_tools import (check_directionality_viable,
-                              find_animal_name_from_body_part_name)
+                              find_animal_name_from_body_part_name,
+                              stdout_success)
 from simba.drop_bp_cords import createColorListofList, create_body_part_dictionary, get_fn_ext
 from simba.roi_tools.ROI_analyzer import ROIAnalyzer
 import itertools
 from copy import deepcopy
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import NoFilesFoundError, NoROIDataError
 
@@ -198,15 +199,16 @@
         """
 
         for video_name, video_data in self.data.items():
             save_path = os.path.join(self.features_dir, video_name + '.' + self.file_type)
             save_df(video_data.fillna(0), self.file_type, save_path)
             print('Created additional ROI features for {}...'.format(video_name))
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: Created additional ROI features for files within the project_folder/csv/features_extracted directory (elapsed time: {}s)'.format(self.timer.elapsed_time_str))
+        stdout_success(msg='Created additional ROI features for files within the project_folder/csv/features_extracted directory', elapsed_time=self.timer.elapsed_time_str)
+
 
 # roi_featurizer = ROIFeatureCreator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_animals_16bp_032023/project_folder/project_config.ini')
 # roi_featurizer.analyze_ROI_data()
 #roi_featurizer.save_new_features_files()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_clf_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import pandas as pd
 from simba.rw_dfs import read_df
 import numpy as np
 from shapely import geometry
 from shapely.geometry import Point, Polygon
 from datetime import datetime
 from simba.misc_tools import (get_fn_ext,
-                              detect_bouts)
+                              detect_bouts,
+                              stdout_success)
 import os
 from simba.read_config_unit_tests import (read_config_entry,
                                           check_that_column_exist,
                                           check_if_filepath_list_is_empty)
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.enums import Keys
 from simba.mixins.config_reader import ConfigReader
@@ -225,15 +226,15 @@
             for clf, clf_data in video_data.items():
                 for roi_name, roi_data in clf_data.items():
                     for measurement_name, mesurement_value in roi_data.items():
                         out_df.loc[len(out_df)] = [video_name, clf, roi_name, measurement_name, mesurement_value]
         out_path = os.path.join(self.logs_path, 'Classification_time_by_ROI_{}.csv'.format(self.date_time))
         out_df.to_csv(out_path)
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: Classification data by ROIs saved in {} (selapsed time: {}s)'.format(out_path, self.timer.elapsed_time_str))
+        stdout_success(msg=f'Classification data by ROIs saved in {out_path}.', elapsed_time=self.timer.elapsed_time_str)
 #
 # clf_ROI_analyzer = clf_within_ROI(config_ini="/Users/simon/Desktop/troubleshooting/train_model_project/project_folder/project_config.ini")
 # clf_ROI_analyzer.run(behavior_list=['Attack', 'Sniffing'], ROI_dict_lists={'Rectangle': ['rec'], 'Circle': ['Stimulus 1', 'Stimulus 2', 'Stimulus 3']}, body_part_list=['Nose_1'], measurements=['Total time by ROI (s)', 'Started bouts by ROI (count)', 'Ended bouts by ROI (count)'])
 #
 
 # clf_ROI_analyzer = clf_within_ROI(config_ini="/Users/simon/Desktop/envs/troubleshooting/Two_animals_16bps/project_folder/project_config.ini")
 # clf_ROI_analyzer.perform_ROI_clf_analysis(behavior_list=['Attack', 'Sniffing'], ROI_dict_lists={'Rectangle': ['DAMN'], 'Circle': [], 'Polygon': ['YOU_SUCK_SIMON']}, body_part_list=['Nose_1'], measurements=['Total time by ROI (s)', 'Started bouts by ROI (count)', 'Ended bouts by ROI (count)'])
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.55.7/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/misc_tools.py` & `Simba-UW-tf-dev-1.55.7/simba/misc_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from configparser import (ConfigParser,
                           MissingSectionHeaderError)
 import multiprocessing
 from simba.read_config_unit_tests import (check_file_exist_and_readable,
                                           read_config_entry,
                                           read_config_file,
                                           check_if_filepath_list_is_empty)
-from simba.enums import ReadConfig, Dtypes, Paths
+from simba.enums import ReadConfig, Dtypes, Paths, Defaults, TagNames
 from simba.extract_frames_fast import video_to_frames
 from simba.utils.errors import (InvalidVideoFileError,
                                 NotDirectoryError,
                                 NoFilesFoundError,
                                 DirectoryExistError,
                                 InvalidFileTypeError,
                                 CountError)
@@ -41,15 +41,14 @@
 import pathlib
 from datetime import datetime
 import sys
 import importlib
 import ast
 import simba
 
-
 def get_video_meta_data(video_path: str):
     """
     Helper to read video metadata (fps, resolution, frame cnt etc.) from video file.
 
     Parameters
     ----------
     video_path: str
@@ -1459,14 +1458,27 @@
     user_class(config_path=config_path)
 
 def find_animal_name_from_body_part_name(bp_name: str, bp_dict: dict) -> str:
     for animal_name, animal_bps in bp_dict.items():
         if bp_name in [x[:-2] for x in animal_bps['X_bps']]:
             return animal_name
 
+def stdout_success(msg: str, elapsed_time: str or None=None) -> None:
+    if elapsed_time:
+        print(f'SIMBA COMPLETE: {msg} (elapsed time: {elapsed_time}) {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.COMPLETE.value}')
+    else:
+        print(f'SIMBA COMPLETE: {msg} {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.COMPLETE.value}')
+
+def stdout_warning(msg: str, elapsed_time: str or None=None) -> None:
+    if elapsed_time:
+        print(f'SIMBA WARNING: {msg} (elapsed time: {elapsed_time}) {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.WARNING.value}')
+    else:
+        print(f'SIMBA WARNING: {msg} {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.WARNING.value}')
+
+
 def create_logger(path: str):
     logger = logging.getLogger()
     logger.setLevel(logging.INFO)
     handler = logging.FileHandler(filename=path, encoding='utf-8')  # or whatever
     handler.setFormatter(logging.Formatter('%(asctime)s %(levelname)s %(message)s'))
     logger.addHandler(handler)
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.55.7/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_importers/sleap_importer_slp.py` & `Simba-UW-tf-dev-1.55.7/simba/pose_importers/sleap_importer_slp.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,16 @@
                                  create_body_part_dictionary,
                                  getBpNames,
                                  getBpHeaders)
 from simba.misc_tools import (find_video_of_file,
                               check_multi_animal_status,
                               smooth_data_gaussian,
                               smooth_data_savitzky_golay,
-                              get_video_meta_data)
+                              get_video_meta_data,
+                              stdout_success)
 from simba.read_config_unit_tests import (check_if_filepath_list_is_empty,
                                           read_project_path_and_file_type,
                                           read_config_file)
 from simba.enums import Paths, ReadConfig, Methods
 from simba.rw_dfs import read_df
 import json
 from collections import defaultdict
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_importers/sleap_importer_h5.py` & `Simba-UW-tf-dev-1.55.7/simba/pose_importers/sleap_importer_h5.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
                                           read_project_path_and_file_type)
 from simba.misc_tools import (find_video_of_file,
                               check_multi_animal_status,
                               smooth_data_gaussian,
                               smooth_data_savitzky_golay,
                               get_video_meta_data,
                               get_fn_ext,
-                              SimbaTimer)
+                              SimbaTimer,
+                              stdout_success)
 from simba.drop_bp_cords import (createColorListofList,
                                  create_body_part_dictionary,
                                  getBpNames,
                                  getBpHeaders)
 from datetime import datetime
 from simba.enums import ReadConfig, Paths
 import itertools
@@ -355,17 +356,15 @@
                 self.data_df = self.data_df.reindex(range(self.data_df.index[0], self.data_df.index[-1] + 1), fill_value=0)
                 p_df = pd.DataFrame(1.0, index=self.data_df.index, columns=self.data_df.columns[1::2] + .5)
                 self.data_df = pd.concat([self.data_df, p_df], axis=1).sort_index(axis=1)
                 self.data_df.columns = self.df_headers
                 self.out_df = deepcopy(self.data_df)
 
             if self.animals_cnt > 1:
-                print(self.video_name, self.video_dir)
                 self.video_path = find_video_of_file(video_dir=self.video_dir, filename=self.video_name)
-                print(self.video_path)
                 self.video_info = get_video_meta_data(self.video_path)
                 self.max_video_dimension = max(self.video_info['width'], self.video_info['height'])
                 self.vid_circle_scale = int(self.radius_scaler / (self.res_scaler / self.max_video_dimension))
                 self.vid_font_scale = float(self.font_scaler / (self.res_scaler / self.max_video_dimension))
                 self.vid_space_scale = int(self.space_scaler / (self.res_scaler / self.max_video_dimension))
                 self.cap = cv2.VideoCapture(self.video_path)
                 self.__initiate_choose_frame()
@@ -384,16 +383,15 @@
                                                'SLEAP H5',
                                                str(self.interpolation_settings),
                                                str(self.smoothing_settings)]
             print('Video "{}" imported (elapsed time {}s)...'.format(self.video_name, video_timer.elapsed_time_str))
 
         import_log.to_csv(self.import_log_path)
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: {} file(s) imported to the SimBA project (project_folder/csv/input_csv directory, elapsed time {}s'.format(str(len(self.files_found)), self.timer.elapsed_time_str))
-
+        stdout_success(msg=f'{str(len(self.files_found))} file(s) imported to the SimBA project (project_folder/csv/input_csv directory', elapsed_time=self.timer.elapsed_time_str)
 
 # test = SLEAPImporterH5(config_path="/Users/simon/Desktop/envs/troubleshooting/Termites_5/project_folder/project_config.ini",
 #                    data_folder=r'/Users/simon/Desktop/envs/troubleshooting/Termites_5/test',
 #                    actor_IDs=['Simon', 'Nastacia'],
 #                    interpolation_settings="Body-parts: Nearest",
 #                    smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
 # test.import_sleap()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_importers/dlc_multi_animal_importer.py` & `Simba-UW-tf-dev-1.55.7/simba/pose_importers/dlc_multi_animal_importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,16 @@
                                           read_config_file,
                                           check_if_filepath_list_is_empty,
                                           read_project_path_and_file_type)
 import os, glob
 from simba.misc_tools import (check_multi_animal_status,
                               get_video_meta_data,
                               smooth_data_gaussian,
-                              smooth_data_savitzky_golay)
+                              smooth_data_savitzky_golay,
+                              stdout_success)
 from simba.drop_bp_cords import (getBpNames,
                                  get_fn_ext,
                                  createColorListofList,
                                  create_body_part_dictionary)
 from simba.enums import Paths, ReadConfig, Dtypes
 from datetime import datetime
 import itertools
@@ -401,15 +402,15 @@
                                                datetime.now().strftime('%Y%m%d%H%M%S'),
                                                'MADLC',
                                                str(self.interpolation_settings),
                                                str(self.smoothing_settings)]
             print('SimBA import of file {} complete!'.format(self.file_name))
 
         import_log.to_csv(self.import_log_path)
-        print('SIMBA COMPLETE: {} files imported to your SimBA project. Imported files are located in the project_folder/csv/input_csv directory.'.format(str(len(self.files_found))))
+        stdout_success(msg=f'{str(len(self.files_found))} files imported to your SimBA project. Imported files are located in the project_folder/csv/input_csv directory.')
 
 # test = MADLC_Importer(config_path=r'/Users/simon/Desktop/envs/troubleshooting/two_black_animals/project_folder/project_config.ini',
 #                    data_folder=r'/Users/simon/Desktop/envs/troubleshooting/two_black_animals/h5',
 #                    file_type='ellipse',
 #                    id_lst=['Simon', 'JJ'],
 #                    interpolation_settings='Body-parts: Nearest',
 #                    smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_importers/sleap_importer_csv.py` & `Simba-UW-tf-dev-1.55.7/simba/pose_importers/sleap_importer_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from numba import jit, prange
 import numpy as np
 from copy import deepcopy
 from simba.misc_tools import (find_video_of_file,
                               check_multi_animal_status,
                               smooth_data_gaussian,
                               smooth_data_savitzky_golay,
-                              get_video_meta_data)
+                              get_video_meta_data,
+                              stdout_success)
 from simba.drop_bp_cords import (get_fn_ext,
                                  createColorListofList,
                                  create_body_part_dictionary,
                                  getBpNames,
                                  getBpHeaders)
 from datetime import datetime
 import itertools
@@ -366,15 +367,15 @@
                                                datetime.now().strftime('%Y%m%d%H%M%S'),
                                                'SLEAP_CSV',
                                                str(self.interpolation_settings),
                                                str(self.smoothing_settings)]
             print('Video "{}" imported...'.format(self.video_basename))
 
         import_log.to_csv(self.import_log_path)
-        print('SIMBA COMPLETE: {} file(s) imported to the SimBA project (project_folder/csv/input_csv directory)'.format(str(len(self.files_found))))
+        stdout_success(msg=f'{str(len(self.files_found))} file(s) imported to the SimBA project (project_folder/csv/input_csv directory)')
 
 
 # test = SleapCsvImporter(config_path=r'/Users/simon/Desktop/envs/troubleshooting/Hornet/project_folder/project_config.ini',
 #                  data_folder=r'/Users/simon/Desktop/envs/troubleshooting/Hornet_single_slp/import',
 #                  actor_IDs=['Hornet'],
 #                  interpolation_settings="Body-parts: Nearest",
 #                  smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_importers/import_trk.py` & `Simba-UW-tf-dev-1.55.7/simba/pose_importers/import_trk.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.55.7/simba/pose_importers/import_mars.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import json
 import numpy as np
 import pandas as pd
 from copy import deepcopy
 from simba.rw_dfs import save_df
 from simba.misc_tools import (get_fn_ext,
                               smooth_data_gaussian,
-                              smooth_data_savitzky_golay)
+                              smooth_data_savitzky_golay,
+                              stdout_success)
 from simba.enums import Paths, Methods, Dtypes
 from simba.interpolate_pose import Interpolate
 import pyarrow.parquet as pq
 import pyarrow as pa
 
 
 class MarsImporter(object):
@@ -155,9 +156,9 @@
 
             if self.interpolation_method != Dtypes.NONE.value:
                 print('Performing interpolation...')
                 self.__perform_interpolation(self.save_path, self.file_type, self._config_path, self.interpolation_method)
             if self.smoothing_method['Method'] != Dtypes.NONE.value:
                 self.__run_smoothing()
             print('Video imported {}.'.format(self.file_name))
-        print('SIMBA COMPLETE: {} data files imported to SimBA project.'.format(str(len(self.files_found))))
+        stdout_success(msg=f'{str(len(self.files_found))} data files imported to SimBA project')
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.55.7/simba/pose_importers/dlc_importer_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 import pandas as pd
 from simba.drop_bp_cords import get_fn_ext
 from simba.read_config_unit_tests import (read_config_file,
                                           read_project_path_and_file_type,
                                           check_file_exist_and_readable,
                                           check_if_filepath_list_is_empty,
                                           check_int)
-from simba.misc_tools import SimbaTimer, get_number_of_header_columns_in_df
+from simba.misc_tools import (SimbaTimer,
+                              get_number_of_header_columns_in_df,
+                              stdout_success)
 from simba.enums import Methods
 from simba.interpolate_pose import Interpolate
 from simba.misc_tools import smooth_data_savitzky_golay, smooth_data_gaussian
 from simba.utils.errors import NoFilesFoundError, FileExistError
 
 
 def import_dlc_csv(config_path: str, source: str) -> list:
@@ -115,16 +117,15 @@
     if smoothing_setting == Methods.GAUSSIAN.value:
         print(f'Smoothing data using Gaussian method and {str(smoothing_time)} ms time window ...')
         smooth_data_gaussian(config=config, file_path=imported_file_paths[0], time_window_parameter=int(smoothing_time))
     if smoothing_setting == Methods.SAVITZKY_GOLAY.value:
         print(f'Smoothing data using Savitzky Golay method and {str(smoothing_time)} ms time window ...')
         smooth_data_savitzky_golay(config=config, file_path=imported_file_paths[0], time_window_parameter=int(smoothing_time))
     timer.stop_timer()
-    print(f'SIMBA COMPLETE: Imported {str(len(imported_file_paths))} pose estimation file(s) (elapsed time {timer.elapsed_time_str}s)')
-
+    stdout_success(msg=f'Imported {str(len(imported_file_paths))} pose estimation file(s)', elapsed_time=timer.elapsed_time_str)
 
 def import_multiple_dlc_tracking_csv_file(config_path: str,
                                           interpolation_setting: str,
                                           smoothing_setting: str,
                                           smoothing_time: int,
                                           folder_path: str):
     timer = SimbaTimer()
@@ -152,8 +153,8 @@
             smooth_data_gaussian(config=config, file_path=file_path, time_window_parameter=int(smoothing_time))
 
     if smoothing_setting == Methods.SAVITZKY_GOLAY.value:
         print(f'Smoothing data using Savitzky Golay method and {str(smoothing_time)} ms time window ...')
         for file_path in imported_file_paths:
             smooth_data_savitzky_golay(config=config, file_path=file_path, time_window_parameter=int(smoothing_time))
     timer.stop_timer()
-    print(f'SIMBA COMPLETE: Imported {str(len(imported_file_paths))} pose estimation file(s) (elapsed time {timer.elapsed_time_str}s)')
+    stdout_success(msg=f'Imported {str(len(imported_file_paths))} pose estimation file(s)', elapsed_time=timer.elapsed_time_str)
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.55.7/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pop_up_classes.py` & `Simba-UW-tf-dev-1.55.7/simba/pop_up_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,16 @@
                               get_color_dict,
                               find_all_videos_in_directory,
                               get_file_name_info_in_directory,
                               SimbaTimer,
                               find_files_of_filetypes_in_directory,
                               archive_processed_files,
                               copy_img_folder,
-                              str_2_bool)
+                              str_2_bool,
+                              stdout_success)
 from simba.drop_bp_cords import get_fn_ext
 from simba.utils.lookups import get_third_party_appender_file_formats
 from simba.third_party_label_appenders.third_party_appender import ThirdPartyLabelAppender
 from simba.plotting.ROI_feature_visualizer import ROIfeatureVisualizer
 from simba.get_coordinates_tools_v2 import get_coordinates_nilsson
 from simba.roi_tools.ROI_clf_calculator import ROIClfCalculator
 from simba.tkinter_functions import hxtScrollbar, DropDownMenu, CreateToolTip, CreateLabelFrameWithIcon
@@ -464,15 +465,15 @@
 
         targets = []
         for behaviour, behavior_val in behaviors_dict.items():
             if behavior_val.get():
                 targets.append(behaviour)
 
         if len(targets) == 0:
-            print('SIMBA ERROR: Select at least one classifier to apply Kleinberg smoothing')
+            raise NoChoosenClassifierError()
 
         check_int(name='Hierarchy', value=self.k_hierarchy.entry_get)
         check_float(name='Sigma', value=self.k_sigma.entry_get)
         check_float(name='Gamma', value=self.k_gamma.entry_get)
 
         try:
             print('Applying kleinberg hyperparameter Setting: Sigma: {}, Gamma: {}, Hierarchy: {}'.format(str(self.k_sigma.entry_get), str(self.k_gamma.entry_get), str(self.k_hierarchy.entry_get)))
@@ -1404,15 +1405,15 @@
             self.config.set('SML settings', 'model_path_{}'.format(str(cnt+1)), model_settings['path'].file_path)
             self.config.set('threshold_settings', 'threshold_{}'.format(str(cnt+1)), model_settings['threshold'].entry_get)
             self.config.set('Minimum_bout_lengths', 'min_bout_{}'.format(str(cnt+1)), model_settings['min_bout'].entry_get)
 
         with open(self.config_path, 'w') as f:
             self.config.write(f)
 
-        print('SIMBA COMPLETE: Model paths/settings saved in project_config.ini')
+        stdout_success(msg='Model paths/settings saved in project_config.ini')
 
 #_ = SetMachineModelParameters(config_path='/Users/simon/Desktop/envs/troubleshooting/Two_animals_16bps/project_folder/project_config.ini')
 
 class OutlierSettingsPopUp(PopUpMixin):
     def __init__(self,
                  config_path: str):
         super().__init__(config_path=config_path, title='OUTLIER SETTINGS')
@@ -1704,15 +1705,16 @@
             with open(self.config_path, 'w') as f:
                 self.config.write(f)
             core_cnt = self.multiprocess_dropdown.getChoices()
             for video in videos:
                 roi_plotter = ROIPlotMultiprocess(ini_path=self.config_path, video_path=video, core_cnt=int(core_cnt), style_attr=style_attr)
                 roi_plotter.insert_data()
                 roi_plotter.visualize_ROI_data()
-        print('All ROI videos created and saved in project_folder/frames/output/ROI_analysis directory')
+
+        stdout_success(msg='All ROI videos created and saved in project_folder/frames/output/ROI_analysis directory')
 
 #_ = VisualizeROITrackingPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/Two_animals_16bps/project_folder/project_config.ini')
 
 class CreateUserDefinedPoseConfigurationPopUp(object):
     def __init__(self,
                  master=None,
                  project_config_class=None):
@@ -1801,15 +1803,15 @@
 
         pose_config_creator = PoseConfigCreator(pose_name=config_name,
                                                 no_animals=int(self.selected_animal_cnt),
                                                 img_path=image_path,
                                                 bp_list=bp_lst,
                                                 animal_id_int_list=animal_id_lst)
         pose_config_creator.launch()
-        print('SIMBA COMPLETE: User-defined pose-configuration "{}" created.'.format(config_name))
+        stdout_success(msg=f'User-defined pose-configuration "{config_name}" created.')
         self.main_frm.winfo_toplevel().destroy()
         self.master.winfo_toplevel().destroy()
         self.project_config_class()
 
 class PoseResetterPopUp(object):
     def __init__(self):
         popup = Tk()
@@ -3304,15 +3306,15 @@
         self.config.set(ReadConfig.SML_SETTINGS.value, ReadConfig.TARGET_CNT.value, str(self.target_cnt+1))
         self.config.set(ReadConfig.SML_SETTINGS.value, f'model_path_{str(self.target_cnt + 1)}', '')
         self.config.set(ReadConfig.SML_SETTINGS.value, f'target_name_{str(self.target_cnt + 1)}', clf_name)
         self.config.set(ReadConfig.THRESHOLD_SETTINGS.value, f'threshold_{str(self.target_cnt + 1)}', 'None')
         self.config.set(ReadConfig.MIN_BOUT_LENGTH.value, f'min_bout_{str(self.target_cnt + 1)}', 'None')
         with open(self.config_path, 'w') as f:
             self.config.write(f)
-        print(f'SIMBA COMPLETE: {clf_name} classifier added to SimBA project')
+        stdout_success(msg=f'{clf_name} classifier added to SimBA project')
 
 class ArchiveProcessedFilesPopUp(PopUpMixin):
     def __init__(self,
                  config_path: str):
         PopUpMixin.__init__(self, config_path=config_path, title='ADD CLASSIFIER')
         self.archive_eb = Entry_Box(self.main_frm,'ARCHIVE DIRECTORY NAME', '25')
         archive_btn = Button(self.main_frm, text='RUN ARCHIVE', fg='blue', command=lambda: self.run())
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/extract_seqframes.py` & `Simba-UW-tf-dev-1.55.7/simba/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.55.7/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Ear_left,Ear_right,Nose,Tail_base,,,,,,,,,,,,
 Ear_left,Ear_right,Nose,Center,Lat_left,Lat_right,Tail_base,,,,,,,,,
 Ear_left,Ear_right,Nose,Center,Lat_left,Lat_right,Tail_base,Tail_end,,,,,,,,
 Mouse1_left_ear,Mouse1_right_ear,Mouse1_left_hand,Mouse1_right_hand,Mouse1_left_foot,Mouse1_right_foot,Mouse1_nose,Mouse1_tail,Mouse1_back,,,,,,,
-Ear_left_1,Ear_right_1,Nose_1,Tail_base_1,Ear_left_2,Right_ear_2,Nose_2,Tail_base_2,,,,,,,,
+Ear_left_1,Ear_right_1,Nose_1,Tail_base_1,Ear_left_2,Ear_right_2,Nose_2,Tail_base_2,,,,,,,,
 Ear_left_1,Ear_right_1,Nose_1,Center_1,Lat_left_1,Lat_right_1,Tail_base_1,Ear_left_2,Ear_right_2,Nose_2,Center_2,Lat_left_2,Lat_right_2,Tail_base_2,,
 Ear_left_1,Ear_right_1,Nose_1,Center_1,Lat_left_1,Lat_right_1,Tail_base_1,Tail_end_1,Ear_left_2,Ear_right_2,Nose_2,Center_2,Lat_left_2,Lat_right_2,Tail_base_2,Tail_end_2
 Nose_1,Ear_left_1,Ear_right_1,Neck_1,Hip_left_1,Hip_right_1,Tail_1,Nose_2,Ear_left_2,Ear_right_2,Neck_2,Hip_left_2,Hip_right_2,Tail_2,,
 Ear_left_1,Ear_right_1,Nose_1,Tail_base_1,Ear_left_2,Right_ear_2,Nose_2,Tail_base_2,,,,,,,,
 Ear_left_1,Ear_right_1,Nose_1,Center_1,Lat_left_1,Lat_right_1,Tail_base_1,Ear_left_2,Ear_right_2,Nose_2,Center_2,Lat_left_2,Lat_right_2,Tail_base_2,,
 Ear_left_1,Ear_right_1,Nose_1,Center_1,Lat_left_1,Lat_right_1,Tail_base_1,Tail_end_1,Ear_left_2,Ear_right_2,Nose_2,Center_2,Lat_left_2,Lat_right_2,Tail_base_2,Tail_end_2
 3D,,,,,,,,,,,,,,,
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.55.7/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/get_coordinates_tools_v2.py` & `Simba-UW-tf-dev-1.55.7/simba/get_coordinates_tools_v2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pup_retrieval_protocol.py` & `Simba-UW-tf-dev-1.55.7/simba/pup_retrieval_protocol.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.55.7/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from simba.misc_tools import get_fn_ext
+from simba.misc_tools import get_fn_ext, stdout_success
 from simba.read_config_unit_tests import read_config_entry
 from simba.train_model_functions import insert_column_headers_for_outlier_correction
 from simba.enums import ReadConfig, Dtypes
 import os, glob
 from simba.rw_dfs import read_df, save_df
 import pandas as pd
 import numpy as np
@@ -107,15 +107,15 @@
                 for bp_name, vid_idx_lst in animal_data.items():
                     correction_ratio = round(len(vid_idx_lst) / len(self.data_df), 6)
                     out_df_lst.append(pd.DataFrame([[video_name, animal_name, bp_name, len(vid_idx_lst), correction_ratio]], columns=['Video', 'Animal', 'Body-part', 'Corrections', 'Correction ratio (%)']))
         out_df = pd.concat(out_df_lst, axis=0).reset_index(drop=True)
         log_fn = os.path.join(self.logs_path, 'Outliers_movement_{}.csv'.format(self.datetime))
         out_df.to_csv(log_fn)
         self.timer.stop_timer()
-        print(f'SIMBA COMPLETE: Log for corrected "movement outliers" saved in project_folder/logs (elapsed time {self.timer.elapsed_time_str}s).')
+        stdout_success(msg='Log for corrected "movement outliers" saved in project_folder/logs', elapsed_time=self.timer.elapsed_time_str)
 
 # test = OutlierCorrecterMovement(config_path='/Users/simon/Desktop/troubleshooting/User_def_2/project_folder/project_config.ini')
 # test.correct_movement_outliers()
 
 # test = OutlierCorrecterMovement(config_path='/Users/simon/Desktop/envs/troubleshooting/two_animals_16bp_032023/project_folder/project_config.ini')
 # test.correct_movement_outliers()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.55.7/simba/outlier_tools/outlier_corrector_location.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from simba.read_config_unit_tests import read_config_entry
 import os, glob
-from simba.misc_tools import get_fn_ext
+from simba.misc_tools import get_fn_ext, stdout_success
 from simba.rw_dfs import (read_df,
                           save_df)
 from simba.enums import ReadConfig, Dtypes
 import numpy as np
 import pandas as pd
 from simba.mixins.config_reader import ConfigReader
 
@@ -124,14 +124,14 @@
                 for bp_name, vid_idx_lst in animal_data.items():
                     correction_ratio = round(len(vid_idx_lst) / len(self.data_df), 6)
                     out_df_lst.append(pd.DataFrame([[video_name, animal_name, bp_name, len(vid_idx_lst), correction_ratio]], columns=['Video', 'Animal', 'Body-part', 'Corrections', 'Correction ratio (%)']))
         out_df = pd.concat(out_df_lst, axis=0).reset_index(drop=True)
         log_fn = os.path.join(self.logs_path, 'Outliers_location_{}.csv'.format(self.datetime))
         out_df.to_csv(log_fn)
         self.timer.stop_timer()
-        print(f'SIMBA COMPLETE: Log for corrected "location outliers" saved in project_folder/logs (elapsed time {self.timer.elapsed_time_str}s)')
+        stdout_success(msg='Log for corrected "location outliers" saved in project_folder/logs', elapsed_time=self.timer.elapsed_time_str)
 
 # test = OutlierCorrecterLocation(config_path='/Users/simon/Desktop/troubleshooting/Zebrafish/project_folder/project_config.ini')
 # test.correct_location_outliers()
 #
 # test = OutlierCorrecterLocation(config_path='/Users/simon/Desktop/envs/troubleshooting/two_animals_16bp_032023/project_folder/project_config.ini')
 # test.correct_location_outliers()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.55.7/simba/outlier_tools/skip_outlier_correction.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from simba.read_config_unit_tests import (read_config_entry,
-                                          check_file_exist_and_readable,
+from simba.read_config_unit_tests import (check_file_exist_and_readable,
                                           read_config_file,
                                           read_project_path_and_file_type)
 import os, glob
 import pandas as pd
 from simba.drop_bp_cords import getBpNames, get_fn_ext
 from simba.rw_dfs import read_df, save_df
-from simba.enums import ReadConfig, Paths, Dtypes
+from simba.enums import Paths
 from simba.train_model_functions import insert_column_headers_for_outlier_correction
+from simba.misc_tools import stdout_success
 
 class OutlierCorrectionSkipper(object):
     """
     Class for skipping outlier correction in SimBA projects.
 
     Parameters
     ----------
@@ -65,16 +65,15 @@
                 data_df = data_df.set_index('scorer')
             data_df = insert_column_headers_for_outlier_correction(data_df=data_df, new_headers=self.header_line, filepath=file_path)
             data_df.index.name = None
             save_path = os.path.join(self.out_dir, video_name + '.' + self.file_type)
             save_df(data_df, self.file_type, save_path)
             self.file_cnt += 1
             print('Skipped outlier correction for video {} ...'.format(video_name))
-
-        print('SIMBA COMPLETE: Skipped outlier correction for {} files.'.format(str(self.file_cnt)))
+        stdout_success(msg=f'Skipped outlier correction for {str(self.file_cnt)} files')
 
 # test = OutlierCorrectionSkipper(config_path='/Users/simon/Desktop/troubleshooting/Zebrafish/project_folder/project_config.ini')
 # test.skip_outlier_correction()
 
 # test = OutlierCorrectionSkipper(config_path=r"Z:\DeepLabCut\DLC_extract\Troubleshooting\Parquet_test2\project_folder\project_config.ini")
 # test.skip_outlier_correction()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.55.7/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.55.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.55.7/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/pose_reset.py` & `Simba-UW-tf-dev-1.55.7/simba/pose_reset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __author__ = "Simon Nilsson"
 
 import os
 import simba
 import shutil
-from simba.misc_tools import check_file_exist_and_readable
+from simba.misc_tools import check_file_exist_and_readable, stdout_success
 from simba.utils.lookups import get_bp_config_codes
 import pandas as pd
 
 class PoseResetter(object):
     """
     Class for deleting all user-defined pose-estimation schematics, diagrams and other settings from the
     SimBA installation
@@ -51,15 +51,15 @@
         default_pic_list = []
         user_pic_lst = os.listdir(self.schematics_path)
         for idx in range(self.default_pose_configs_cnt):
             default_pic_list.append('{}.png'.format(str(idx+1)))
         for i in list(set(user_pic_lst) - set(default_pic_list)):
             os.remove(os.path.join(self.schematics_path, i))
 
-        print('SIMBA COMPLETE: User-defined pose-estimation configuration reset. User-defined poses removed.')
+        stdout_success(msg='User-defined pose-estimation configuration reset. User-defined poses removed.')
         master.destroy()
 
 # test = PoseResetter()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/train_mutiple_models.py` & `Simba-UW-tf-dev-1.55.7/simba/train_mutiple_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,24 +31,27 @@
                                           read_config_entry,
                                           read_simba_meta_files,
                                           read_meta_file,
                                           read_config_file,
                                           check_if_filepath_list_is_empty,
                                           check_if_valid_input,
                                           read_project_path_and_file_type)
+from simba.misc_tools import stdout_success
 from simba.drop_bp_cords import drop_bp_cords
 from sklearn.model_selection import train_test_split
 from sklearn.ensemble import RandomForestClassifier
 from simba.utils.errors import InvalidInputError
 from simba.enums import (Options,
                          ReadConfig,
                          Paths,
                          Dtypes,
                          Methods,
-                         MetaKeys)
+                         MetaKeys,
+                         Defaults,
+                         TagNames)
 
 
 class TrainMultipleModelsFromMeta(object):
     """
     Class for grid-searching random forest models from hyperparameter setting and sampling methods
     stored within the `project_folder/configs` directory of a SimBA project.
 
@@ -206,15 +209,15 @@
                     create_shap_log(self.ini_path, self.rf_clf, self.x_train, self.y_train, self.feature_names, self.clf_name, self.meta_dict[MetaKeys.SHAP_PRESENT.value], self.meta_dict[MetaKeys.SHAP_ABSENT.value], self.model_dir_out, save_it=save_n, save_file_no=config_cnt)
             if MetaKeys.PARTIAL_DEPENDENCY.value in self.meta_dict.keys():
                 if self.meta_dict[MetaKeys.PARTIAL_DEPENDENCY.value] in Options.PERFORM_FLAGS.value:
                     partial_dependence_calculator(clf=self.rf_clf, x_df=self.x_train, clf_name=self.clf_name, save_dir=self.model_dir_out)
             create_meta_data_csv_training_multiple_models(self.meta_dict, self.clf_name, self.model_dir_out, save_file_no=config_cnt)
             save_rf_model(self.rf_clf, self.clf_name, self.model_dir_out, save_file_no=config_cnt)
             print('Classifier {} saved in models/validations/model_files directory ...'.format(str(self.clf_name + '_' + str(config_cnt))))
-        print('All models and evaluations complete. The models/evaluation files are in models/validations folders')
+        stdout_success(msg='All models and evaluations complete. The models/evaluation files are in models/validations folders')
 
 # test = TrainMultipleModelsFromMeta(config_path='/Users/simon/Desktop/envs/troubleshooting/locomotion/project_folder/project_config.ini')
 # test.train_models_from_meta()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/SimBA.py` & `Simba-UW-tf-dev-1.55.7/simba/SimBA.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,17 @@
 import atexit
 from simba.video_info_table import VideoInfoTable
 from simba.read_config_unit_tests import check_int
 from simba.roi_tools.ROI_define import *
 from simba.roi_tools.ROI_menus import *
 from simba.roi_tools.ROI_reset import *
 from simba.misc_tools import (run_user_defined_feature_extraction_class,
-                              extract_frames_from_all_videos_in_directory)
+                              extract_frames_from_all_videos_in_directory,
+                              get_video_meta_data,
+                              stdout_success)
 from simba.video_processing import (video_to_greyscale,
                                     superimpose_frame_count)
 from simba.setting_menu import SettingsMenu
 from simba.pop_up_classes import (HeatmapLocationPopup,
                                   QuickLineplotPopup,
                                   ClfByROIPopUp,
                                   FSTTCPopUp,
@@ -105,15 +107,16 @@
                                   ThirdPartyAnnotatorAppenderPopUp,
                                   ValidationVideoPopUp)
 from simba.bounding_box_tools.boundary_menus import BoundaryMenus
 from simba.labelling_interface import select_labelling_video
 from simba.labelling_advanced_interface import select_labelling_video_advanced
 from simba.enums import (Formats,
                          OS,
-                         Defaults)
+                         Defaults,
+                         TagNames)
 from simba.utils.lookups import get_bp_config_code_class_pairs, get_icons_paths
 from simba.mixins.pop_up_mixin import PopUpMixin
 from simba.create_project_pop_up import ProjectCreatorPopUp
 from simba.plotly_create_h5 import create_plotly_container
 from simba.utils.lookups import get_emojis
 #from simba.unsupervised.unsupervised_ui import UnsupervisedGUI
 import sys
@@ -127,19 +130,19 @@
         main_frm = Toplevel()
         main_frm.minsize(300, 200)
         main_frm.wm_title("Load SimBA project (project_config.ini file)")
 
 
         load_project_frm = CreateLabelFrameWithIcon(parent=main_frm, header='LOAD SIMBA PROJECT_CONFIG.INI', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.LOAD_PROJECT.value)
         self.selected_file = FileSelect(load_project_frm,'Select file: ', title='Select project_config.ini file')
-        load_project_btn = Button(load_project_frm, text='LOAD PROJECT', font=("Helvetica", 12, 'bold'), command=lambda: self.launch_project())
+        load_project_btn = Button(load_project_frm, text='LOAD PROJECT', fg='blue', command=lambda: self.launch_project())
 
-        load_project_frm.grid(row=0)
-        self.selected_file.grid(row=0,sticky=NW)
-        load_project_btn.grid(row=1,pady=10, sticky=NW)
+        load_project_frm.grid(row=0, sticky=NW)
+        self.selected_file.grid(row=0, sticky=NW)
+        load_project_btn.grid(row=1, pady=10, sticky=NW)
 
     def launch_project(self):
         print('Loading {}...'.format(self.selected_file.file_path))
         check_file_exist_and_readable(file_path=self.selected_file.file_path)
         _ = SimbaProjectPopUp(config_path=self.selected_file.file_path)
 
 def wait_for_internet_connection(url):
@@ -709,15 +712,16 @@
             self.config.write(f)
 
     def correct_outlier(self):
         outlier_correcter_movement = OutlierCorrecterMovement(config_path=self.config_path)
         outlier_correcter_movement.correct_movement_outliers()
         outlier_correcter_location = OutlierCorrecterLocation(config_path=self.config_path)
         outlier_correcter_location.correct_location_outliers()
-        print('SIMBA COMPLETE: Outlier correction complete. Outlier corrected files located in "project_folder/csv/outlier_corrected_movement_location" directory')
+        stdout_success(msg='Outlier corrected files located in "project_folder/csv/outlier_corrected_movement_location" directory')
+
 
     def callback(self,url):
         webbrowser.open_new(url)
 
 
 
 class App(object):
@@ -816,17 +820,20 @@
         help_menu.add_cascade(label="Links",menu=links_menu, compound='left', image=self.menu_icons['link']['img'])
         help_menu.add_command(label='About', compound='left', image=self.menu_icons['about']['img'], command=AboutSimBAPopUp)
 
         self.frame = Frame(background, bd=2, relief=SUNKEN, width=750, height=300)
         y_sb = Scrollbar(self.frame, orient=VERTICAL)
         self.frame.pack(expand=True)
         self.txt = Text(self.frame, bg='white', insertborderwidth=2, height=30, width=100, yscrollcommand=y_sb)
-        self.txt.tag_configure("center", justify='center', foreground='blue', font=("Rockwell", 16, 'bold'))
+        self.txt.tag_configure(TagNames.GREETING.value, justify='center', foreground='blue', font=("Rockwell", 16, 'bold'))
+        self.txt.tag_configure(TagNames.ERROR.value, justify='left', foreground='red', font=Formats.TKINTER_FONT.value)
+        self.txt.tag_configure(TagNames.STANDARD.value, justify='left', foreground='black', font=Formats.TKINTER_FONT.value)
+        self.txt.tag_configure(TagNames.COMPLETE.value, justify='left', foreground='blue', font=Formats.TKINTER_FONT.value)
         self.txt.insert(INSERT, Defaults.WELCOME_MSG.value + emojis['relaxed'] + '\n' * 2)
-        self.txt.tag_add("center", "1.0", "2.25")
+        self.txt.tag_add(TagNames.GREETING.value, "1.0", "2.25")
         y_sb.pack(side=RIGHT, fill=Y)
         self.txt.pack(expand=True, fill='both')
         y_sb.config(command=self.txt.yview)
         self.txt.config(state=DISABLED, font=Formats.TKINTER_FONT.value)
 
         clear_txt_btn = Button(self.frame, text=' CLEAR', compound=LEFT, image=self.menu_icons['clean']['img'], font=Formats.LABELFRAME_HEADER_FORMAT.value, command=lambda: self.clean_txt())
         clear_txt_btn.pack(side=BOTTOM, fill=X)
@@ -843,61 +850,97 @@
     def clean_txt(self):
         self.txt.config(state=NORMAL)
         self.txt.delete('1.0', END)
 
 class StdRedirector(object):
     def __init__(self, text_widget):
         self.text_space = text_widget
+        self.emojis = get_emojis()
 
-    def write(self, string):
+    def write(self, s: str):
+        tag_name = TagNames.STANDARD.value
+        try:
+            s, tag_name = s.split(Defaults.STR_SPLIT_DELIMITER.value, 2)
+        except ValueError:
+            pass
+        if tag_name != TagNames.STANDARD.value:
+            s = s + ' ' + self.emojis[tag_name]
         self.text_space.config(state=NORMAL)
-        self.text_space.insert("end", string)
+        self.text_space.insert("end", s, (tag_name))
         self.text_space.update()
         self.text_space.see("end")
         self.text_space.config(state=DISABLED)
 
     def flush(self):
         pass
 
-class SplashScreen:
+class SplashStatic:
     def __init__(self, parent):
         self.parent = parent
-        self.Splash()
-        self.Window()
+        self.load_splash_img()
+        self.display_splash()
 
-    def Splash(self):
+    def load_splash_img(self):
         splash_path_win = os.path.join(os.path.dirname(__file__), Paths.SPLASH_PATH_WINDOWS.value)
         splash_path_linux = os.path.join(os.path.dirname(__file__), Paths.SPLASH_PATH_LINUX.value)
         if currentPlatform == OS.WINDOWS.value:
             self.splash_img = PIL.Image.open(splash_path_win)
         else:
             if os.path.isfile(splash_path_linux):
                 self.splash_img = PIL.Image.open(splash_path_linux)
             else:
                 self.splash_img = PIL.Image.open(splash_path_win)
         self.splash_img_tk = ImageTk.PhotoImage(self.splash_img)
 
 
-    def Window(self):
+    def display_splash(self):
         width, height = self.splash_img.size
         half_width = int((self.parent.winfo_screenwidth()-width)//2)
         half_height = int((self.parent.winfo_screenheight()-height)//2)
         self.parent.geometry("%ix%i+%i+%i" %(width, height, half_width, half_height))
         Label(self.parent, image=self.splash_img_tk).pack()
 
+
+class SplashMovie():
+    def __init__(self):
+        #self.parent = Tk()
+        self.parent, self.img_cnt = Tk(), 0
+        self.parent.overrideredirect(True)
+        self.parent.configure(bg='white')
+        splash_path = os.path.join(os.path.dirname(__file__), Paths.SPLASH_PATH_MOVIE.value)
+        self.meta_ = get_video_meta_data(splash_path)
+        self.cap = cv2.VideoCapture(splash_path)
+        width, height = self.meta_['width'], self.meta_['height']
+        half_width = int((self.parent.winfo_screenwidth() - width) // 2)
+        half_height = int((self.parent.winfo_screenheight() - height) // 2)
+        self.parent.geometry("%ix%i+%i+%i" % (width, height, half_width, half_height))
+        self.img_lbl = Label(self.parent, bg='white', image='')
+        self.img_lbl.pack()
+        self.show_animation()
+
+    def show_animation(self):
+        for frm_cnt in range(self.meta_['frame_count']-1):
+            self.cap.set(1, frm_cnt)
+            ret, frame = self.cap.read()
+            if not ret: break
+            frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGBA)
+            frame = ImageTk.PhotoImage(image=PIL.Image.fromarray(frame))
+            self.img_lbl.configure(image=frame)
+            self.img_lbl.imgtk = frame
+            self.parent.update()
+            cv2.waitKey(int(self.meta_['fps'] / 1000))
+        self.parent.destroy()
+
 def terminate_children(children):
     for process in children:
         process.terminate()
 
 def main():
     if currentPlatform == OS.WINDOWS.value:
         import ctypes
         myappid = 'SimBA development wheel'
         ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(myappid)
-    root = Tk()
-    root.overrideredirect(True)
-    _ = SplashScreen(root)
-    root.after(Defaults.SPLASH_TIME.value, root.destroy)
-    root.mainloop()
+    splash = SplashMovie()
+
     app = App()
     #print(Defaults.WELCOME_MSG.value)
     app.root.mainloop()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.55.7/simba/labelling_advanced_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 import pandas as pd
 from simba.rw_dfs import read_df, save_df
 from simba.read_config_unit_tests import (read_config_entry,
                                           read_config_file,
                                           check_file_exist_and_readable,
                                           check_int,
                                           read_project_path_and_file_type)
-from simba.misc_tools import get_video_meta_data, get_fn_ext
+from simba.misc_tools import (get_video_meta_data,
+                              get_fn_ext,
+                              stdout_success)
 import simba
 from tkinter import *
 from tkinter import filedialog
 from PIL import Image, ImageTk
 from subprocess import Popen, PIPE
 import os
 from simba.train_model_functions import get_all_clf_names
@@ -292,15 +294,14 @@
             self.change_frm_box.insert(0, self.current_frm_n.get())
         elif (new_frm_number != self.current_frm_n.get()) and (not keep_prior_img_cb_status):
             self.save_behavior_in_frm()
             self.create_print_statements()
             self.current_frm_n = IntVar(value=new_frm_number)
             for target in self.target_lst:
                 new_frame_annotation = self.data_df_targets[target].loc[int(self.current_frm_n.get())]
-                print(new_frame_annotation)
                 if new_frame_annotation == 0:
                     self.check_absent_vars[target].set(value=1)
                     self.check_present_vars[target].set(value=0)
                 elif new_frame_annotation == 1:
                     self.check_present_vars[target].set(value=1)
                     self.check_absent_vars[target].set(value=0)
                 else:
@@ -374,15 +375,15 @@
         self.save_df = pd.concat([self.save_df, self.data_df_targets], axis=1)
         self.save_df = self.save_df.dropna(subset=self.target_lst)
         try:
             save_df(self.save_df, self.file_type, self.targets_inserted_file_path)
         except Exception as e:
             print(e, 'SIMBA ERROR: File for video {} could not be saved.')
             raise FileExistsError
-        print('SAVED: Annotation file for video {} saved within the project_folder/csv/targets_inserted directory.'.format(self.video_name))
+        stdout_success(msg=f'SAVED: Annotation file for video {self.video_name} saved within the project_folder/csv/targets_inserted directory.')
         if not self.config.has_section('Last annotated frames'):
             self.config.add_section('Last annotated frames')
         self.config.set('Last annotated frames', str(self.video_name), str(self.current_frm_n.get()))
         with open(self.config_path, 'w') as configfile: self.config.write(configfile)
 
     def check_integrity_of_multiple_classifiers(self):
         none_target_lst, labelled_target_lst = [], []
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.55.7/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.55.7/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.55.7/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.55.7/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.55.7/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.55.7/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.55.7/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.55.7/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.55.7/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.55.7/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.55.7/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.55.7/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.55.7/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.55.7/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.55.7/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.55.7/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.55.7/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/assets/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -484,37 +484,37 @@
 00001e30: 010a 010b 010c 0118 0121 0122 0124 0125  .........!.".$.%
 00001e40: 012a 0133 0134 0136 0137 013c 0145 0146  .*.3.4.6.7.<.E.F
 00001e50: 0148 0149 014f 0158 0159 015b 015c 0164  .H.I.O.X.Y.[.\.d
 00001e60: 016d 016e 0171 0172 017b 0184 0185 0187  .m.n.q.r.{......
 00001e70: 0188 0197 01a0 01a1 01a2 01ac 01ad 01b6  ................
 00001e80: 01bb 01c4 0000 0000 0000 0201 0000 0000  ................
 00001e90: 0000 004a 0000 0000 0000 0000 0000 0000  ...J............
-00001ea0: 0000 01c5 eeee c441 0000 0005 0069 0063  .......A.....i.c
-00001eb0: 006f 006e 0073 6d6f 6444 626c 6f62 0000  .o.n.smodDblob..
-00001ec0: 0008 7ef0 e459 eeee c441 0000 0005 0069  ..~..Y...A.....i
-00001ed0: 0063 006f 006e 0073 7068 3153 636f 6d70  .c.o.n.sph1Scomp
-00001ee0: 0000 0000 0007 e000 0000 0005 0069 0063  .............i.c
-00001ef0: 006f 006e 0073 7653 726e 6c6f 6e67 0000  .o.n.svSrnlong..
-00001f00: 0001 0000 0003 0069 006d 0067 6277 7370  .......i.m.gbwsp
-00001f10: 626c 6f62 0000 00c9 6270 6c69 7374 3030  blob....bplist00
-00001f20: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
-00001f30: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
-00001f40: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
-00001f50: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-00001f60: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-00001f70: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-00001f80: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00001f90: 7208 0809 0809 5f10 187b 7b32 302c 2031  r....._..{{20, 1
-00001fa0: 3232 7d2c 207b 3130 3736 2c20 3632 317d  22}, {1076, 621}
-00001fb0: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
-00001fc0: 9900 0000 0000 0001 0100 0000 0000 0000  ................
-00001fd0: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
-00001fe0: 9a00 0000 0300 6900 6d00 676c 6731 5363  ......i.m.glg1Sc
-00001ff0: 6f6d 7000 0000 0000 161e ce00 0000 0300  omp.............
-00002000: 6900 6d00 0000 0000 0000 0012 0000 0005  i.m.............
+00001ea0: 0000 01c5 c441 0000 0005 0069 0063 006f  .....A.....i.c.o
+00001eb0: 006e 0073 6d6f 6444 626c 6f62 0000 0008  .n.smodDblob....
+00001ec0: da62 afb9 1af0 c441 0000 0005 0069 0063  .b.....A.....i.c
+00001ed0: 006f 006e 0073 7068 3153 636f 6d70 0000  .o.n.sph1Scomp..
+00001ee0: 0000 0007 f000 0000 0005 0069 0063 006f  ...........i.c.o
+00001ef0: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
+00001f00: 0000 0003 0069 006d 0067 6277 7370 626c  .....i.m.gbwspbl
+00001f10: 6f62 0000 00c9 6270 6c69 7374 3030 d701  ob....bplist00..
+00001f20: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
+00001f30: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00001f40: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
+00001f50: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
+00001f60: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
+00001f70: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
+00001f80: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
+00001f90: 0809 0809 5f10 187b 7b32 302c 2031 3232  ...._..{{20, 122
+00001fa0: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
+00001fb0: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
+00001fc0: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
+00001fd0: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
+00001fe0: 0000 0300 6900 6d00 676c 6731 5363 6f6d  ....i.m.glg1Scom
+00001ff0: 7000 0000 0000 161e ce00 0000 0300 6900  p.............i.
+00002000: 6d00 676c 0000 0000 0000 0012 0000 0005  m.gl............
 00002010: 0069 0063 006f 006e 0073 6277 7370 626c  .i.c.o.n.sbwspbl
 00002020: 6f62 0000 00c9 6270 6c69 7374 3030 d701  ob....bplist00..
 00002030: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
 00002040: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00002050: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
 00002060: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00002070: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
@@ -522,230 +522,230 @@
 00002090: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
 000020a0: 0809 0809 5f10 187b 7b34 3134 2c20 3136  ...._..{{414, 16
 000020b0: 317d 2c20 7b37 3730 2c20 3433 367d 7d09  1}, {770, 436}}.
 000020c0: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
 000020d0: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
 000020e0: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
 000020f0: 0000 0500 6900 6300 6f00 6e00 736c 6731  ....i.c.o.n.slg1
-00002100: 5363 6f6d 7000 0000 0000 058b 9300 0000  Scomp...........
+00002100: 5363 6f6d 7000 0000 0000 0590 7700 0000  Scomp.......w...
 00002110: 0500 6900 6300 6f00 6e00 736c 7376 4362  ..i.c.o.n.slsvCb
-00002120: 6c6f 6200 0002 b062 706c 6973 7430 30da  lob....bplist00.
+00002120: 6c6f 6200 0002 af62 706c 6973 7430 30da  lob....bplist00.
 00002130: 0102 0304 0506 0708 090a 0b0c 0d18 4849  ..............HI
-00002140: 484a 4b0c 5f10 1276 6965 774f 7074 696f  HJK._..viewOptio
-00002150: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
-00002160: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
-00002170: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
-00002180: 6c6c 5369 7a65 735f 100f 7363 726f 6c6c  llSizes_..scroll
-00002190: 506f 7369 7469 6f6e 5958 7465 7874 5369  PositionYXtextSi
-000021a0: 7a65 5f10 0f73 6372 6f6c 6c50 6f73 6974  ze_..scrollPosit
-000021b0: 696f 6e58 5a73 6f72 7443 6f6c 756d 6e58  ionXZsortColumnX
-000021c0: 6963 6f6e 5369 7a65 5f10 1075 7365 5265  iconSize_..useRe
-000021d0: 6c61 7469 7665 4461 7465 7310 0109 ab0e  lativeDates.....
-000021e0: 171c 2125 2a2f 3439 3e43 d40f 1011 120c  ..!%*/49>C......
-000021f0: 140c 1657 7669 7369 626c 6555 7769 6474  ...WvisibleUwidt
-00002200: 6859 6173 6365 6e64 696e 675a 6964 656e  hYascendingZiden
-00002210: 7469 6669 6572 0911 0127 0954 6e61 6d65  tifier...'.Tname
-00002220: d40f 1011 1218 1918 1b08 1023 0858 7562  ...........#.Xub
-00002230: 6971 7569 7479 d40f 1011 120c 1e18 2009  iquity........ .
-00002240: 10b5 085c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
-00002250: d40f 1011 1218 1e18 2408 085b 6461 7465  ........$..[date
-00002260: 4372 6561 7465 64d4 0f10 1112 0c27 1829  Created......'.)
-00002270: 0910 6108 5473 697a 65d4 0f10 1112 0c2c  ..a.Tsize......,
-00002280: 0c2e 0910 7309 546b 696e 64d4 0f10 1112  ....s.Tkind.....
-00002290: 1831 0c33 0810 6409 556c 6162 656c d40f  .1.3..d.Ulabel..
-000022a0: 1011 1218 360c 3808 104b 0957 7665 7273  ....6.8..K.Wvers
-000022b0: 696f 6ed4 0f10 1112 183b 0c3d 0811 012c  ion......;.=...,
-000022c0: 0958 636f 6d6d 656e 7473 d40f 1011 1218  .Xcomments......
-000022d0: 4018 4208 10c8 085e 6461 7465 4c61 7374  @.B....^dateLast
-000022e0: 4f70 656e 6564 d40f 1011 1218 1e18 4608  Opened........F.
-000022f0: 0859 6461 7465 4164 6465 6408 2300 0000  .YdateAdded.#...
-00002300: 0000 0000 0023 4028 0000 0000 0000 546e  .....#@(......Tn
-00002310: 616d 6523 4030 0000 0000 0000 0900 0800  ame#@0..........
-00002320: 1d00 3200 4400 4c00 6000 7200 7b00 8d00  ..2.D.L.`.r.{...
-00002330: 9800 a100 b400 b600 b700 c300 cc00 d400  ................
-00002340: da00 e400 ef00 f000 f300 f400 f901 0201  ................
-00002350: 0301 0501 0601 0f01 1801 1901 1b01 1c01  ................
-00002360: 2901 3201 3301 3401 4001 4901 4a01 4c01  ).2.3.4.@.I.J.L.
-00002370: 4d01 5201 5b01 5c01 5e01 5f01 6401 6d01  M.R.[.\.^._.d.m.
-00002380: 6e01 7001 7101 7701 8001 8101 8301 8401  n.p.q.w.........
-00002390: 8c01 9501 9601 9901 9a01 a301 ac01 ad01  ................
-000023a0: af01 b001 bf01 c801 c901 ca01 d401 d501  ................
-000023b0: de01 e701 ec01 f500 0000 0000 0002 0100  ................
-000023c0: 0000 0000 0000 4d00 0000 0000 0000 0000  ......M.........
-000023d0: 0000 0000 0001 f600 0000 0500 6900 6300  ............i.c.
-000023e0: 6f00 6e00 736c 7376 7062 6c6f 6200 0002  o.n.slsvpblob...
-000023f0: 9562 706c 6973 7430 30da 0102 0304 0506  .bplist00.......
-00002400: 0708 090a 0b0c 0d1f 4748 4749 4a0c 5f10  ........GHGIJ._.
-00002410: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
-00002420: 696f 6e5f 100f 7368 6f77 4963 6f6e 5072  ion_..showIconPr
-00002430: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
-00002440: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
-00002450: 735f 100f 7363 726f 6c6c 506f 7369 7469  s_..scrollPositi
-00002460: 6f6e 5958 7465 7874 5369 7a65 5f10 0f73  onYXtextSize_..s
-00002470: 6372 6f6c 6c50 6f73 6974 696f 6e58 5a73  crollPositionXZs
-00002480: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
-00002490: 7a65 5f10 1075 7365 5265 6c61 7469 7665  ze_..useRelative
-000024a0: 4461 7465 7310 0109 d90e 0f10 1112 1314  Dates...........
-000024b0: 1516 1720 2529 2d32 373c 4158 636f 6d6d  ... %)-27<AXcomm
-000024c0: 656e 7473 5e64 6174 654c 6173 744f 7065  ents^dateLastOpe
-000024d0: 6e65 645c 6461 7465 4d6f 6469 6669 6564  ned\dateModified
-000024e0: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
-000024f0: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
-00002500: 7369 6f6e 546e 616d 65d4 1819 1a1b 1c1d  sionTname.......
-00002510: 0c1f 5569 6e64 6578 5577 6964 7468 5961  ..UindexUwidthYa
-00002520: 7363 656e 6469 6e67 5776 6973 6962 6c65  scendingWvisible
-00002530: 1007 1101 2c09 08d4 1819 1a1b 2122 1f1f  ....,.......!"..
-00002540: 1008 10c8 0808 d418 191a 1b0b 261f 0c10  ............&...
-00002550: b508 09d4 1819 1a1b 2a26 1f1f 1002 0808  ........*&......
-00002560: d418 191a 1b2e 2f1f 0c10 0310 6108 09d4  ....../.....a...
-00002570: 1819 1a1b 3334 0c1f 1005 1064 0908 d418  ....34.....d....
-00002580: 191a 1b38 390c 0c10 0410 7309 09d4 1819  ...89.....s.....
-00002590: 1a1b 3d3e 0c1f 1006 104b 0908 d418 191a  ..=>.....K......
-000025a0: 1b42 430c 0c10 0011 0127 0909 0823 0000  .BC......'...#..
-000025b0: 0000 0000 0000 2340 2800 0000 0000 0054  ......#@(......T
-000025c0: 6e61 6d65 2340 3000 0000 0000 0009 0008  name#@0.........
-000025d0: 001d 0032 0044 004c 0060 0072 007b 008d  ...2.D.L.`.r.{..
-000025e0: 0098 00a1 00b4 00b6 00b7 00ca 00d3 00e2  ................
-000025f0: 00ef 00fb 0100 0106 010b 0113 0118 0121  ...............!
-00002600: 0127 012d 0137 013f 0141 0144 0145 0146  .'.-.7.?.A.D.E.F
-00002610: 014f 0151 0153 0154 0155 015e 0160 0161  .O.Q.S.T.U.^.`.a
-00002620: 0162 016b 016d 016e 016f 0178 017a 017c  .b.k.m.n.o.x.z.|
-00002630: 017d 017e 0187 0189 018b 018c 018d 0196  .}.~............
-00002640: 0198 019a 019b 019c 01a5 01a7 01a9 01aa  ................
-00002650: 01ab 01b4 01b6 01b9 01ba 01bb 01bc 01c5  ................
-00002660: 01ce 01d3 01dc 0000 0000 0000 0201 0000  ................
-00002670: 0000 0000 004c 0000 0000 0000 0000 0000  .....L..........
-00002680: 0000 0000 01dd 0000 0005 0069 0063 006f  ...........i.c.o
-00002690: 006e 0073 6d6f 4444 626c 6f62 0000 0008  .n.smoDDblob....
-000026a0: 7ef0 e459 eeee c441 0000 0005 0069 0063  ~..Y...A.....i.c
-000026b0: 006f 006e 0073 6d6f 6444 626c 6f62 0000  .o.n.smodDblob..
-000026c0: 0008 7ef0 e459 eeee c441 0000 0005 0069  ..~..Y...A.....i
-000026d0: 0063 006f 006e 0073 7068 3153 636f 6d70  .c.o.n.sph1Scomp
-000026e0: 0000 0000 0007 e000 0000 0005 0069 0063  .............i.c
-000026f0: 006f 006e 0073 7653 726e 6c6f 6e67 0000  .o.n.svSrnlong..
-00002700: 0001 0000 0003 0069 006d 0067 6277 7370  .......i.m.gbwsp
-00002710: 626c 6f62 0000 00c9 6270 6c69 7374 3030  blob....bplist00
-00002720: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
-00002730: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
-00002740: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
-00002750: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-00002760: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-00002770: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-00002780: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00002790: 7208 0809 0809 5f10 187b 7b32 302c 2031  r....._..{{20, 1
-000027a0: 3232 7d2c 207b 3130 3736 2c20 3632 317d  22}, {1076, 621}
-000027b0: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
-000027c0: 9900 0000 0000 0001 0100 0000 0000 0000  ................
-000027d0: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
-000027e0: 9a00 0000 0300 6900 6d00 676c 6731 5363  ......i.m.glg1Sc
-000027f0: 6f6d 7000 0000 0000 161e ce00 0000 0300  omp.............
-00002800: 6900 6d00 676c 7376 4362 6c6f 6200 0002  i.m.glsvCblob...
-00002810: 7962 706c 6973 7430 30d8 0102 0304 0506  ybplist00.......
-00002820: 0708 0909 0b16 4647 4849 5f10 1075 7365  ......FGHI_..use
-00002830: 5265 6c61 7469 7665 4461 7465 735f 100f  RelativeDates_..
-00002840: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
-00002850: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
-00002860: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
-00002870: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e58  SizeZsortColumnX
-00002880: 6963 6f6e 5369 7a65 5f10 1276 6965 774f  iconSize_..viewO
-00002890: 7074 696f 6e73 5665 7273 696f 6e09 09ab  ptionsVersion...
-000028a0: 0c15 1a1f 2328 2d32 373c 41d4 0d0e 0f10  ....#(-27<A.....
-000028b0: 0912 0914 5776 6973 6962 6c65 5577 6964  ....WvisibleUwid
-000028c0: 7468 5961 7363 656e 6469 6e67 5a69 6465  thYascendingZide
-000028d0: 6e74 6966 6965 7209 1101 2709 546e 616d  ntifier...'.Tnam
-000028e0: 65d4 0d0e 0f10 1617 1619 0810 2308 5875  e...........#.Xu
-000028f0: 6269 7175 6974 79d4 0d0e 0f10 091c 161e  biquity.........
-00002900: 0910 b508 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
-00002910: 64d4 0d0e 0f10 161c 1622 0808 5b64 6174  d........"..[dat
-00002920: 6543 7265 6174 6564 d40d 0e0f 1009 2516  eCreated......%.
-00002930: 2709 1061 0854 7369 7a65 d40d 0e0f 1009  '..a.Tsize......
-00002940: 2a09 2c09 1073 0954 6b69 6e64 d40d 0e0f  *.,..s.Tkind....
-00002950: 1016 2f09 3108 1064 0955 6c61 6265 6cd4  ../.1..d.Ulabel.
-00002960: 0d0e 0f10 1634 0936 0810 4b09 5776 6572  .....4.6..K.Wver
-00002970: 7369 6f6e d40d 0e0f 1016 3909 3b08 1101  sion......9.;...
-00002980: 2c09 5863 6f6d 6d65 6e74 73d4 0d0e 0f10  ,.Xcomments.....
-00002990: 163e 1640 0810 c808 5e64 6174 654c 6173  .>.@....^dateLas
-000029a0: 744f 7065 6e65 64d4 0d0e 0f10 161c 1644  tOpened........D
-000029b0: 0808 5964 6174 6541 6464 6564 0823 4028  ..YdateAdded.#@(
-000029c0: 0000 0000 0000 546e 616d 6523 4030 0000  ......Tname#@0..
-000029d0: 0000 0000 1001 0008 0019 002c 003e 0046  ...........,.>.F
-000029e0: 005a 0063 006e 0077 008c 008d 008e 009a  .Z.c.n.w........
-000029f0: 00a3 00ab 00b1 00bb 00c6 00c7 00ca 00cb  ................
-00002a00: 00d0 00d9 00da 00dc 00dd 00e6 00ef 00f0  ................
-00002a10: 00f2 00f3 0100 0109 010a 010b 0117 0120  ............... 
-00002a20: 0121 0123 0124 0129 0132 0133 0135 0136  .!.#.$.).2.3.5.6
-00002a30: 013b 0144 0145 0147 0148 014e 0157 0158  .;.D.E.G.H.N.W.X
-00002a40: 015a 015b 0163 016c 016d 0170 0171 017a  .Z.[.c.l.m.p.q.z
-00002a50: 0183 0184 0186 0187 0196 019f 01a0 01a1  ................
-00002a60: 01ab 01ac 01b5 01ba 01c3 0000 0000 0000  ................
-00002a70: 0201 0000 0000 0000 004a 0000 0000 0000  .........J......
-00002a80: 0000 0000 0000 0000 01c5 0000 0003 0069  ...............i
-00002a90: 006d 0067 6c73 7670 626c 6f62 0000 025e  .m.glsvpblob...^
-00002aa0: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
-00002ab0: 0809 090b 1d46 4748 245f 1010 7573 6552  .....FGH$_..useR
-00002ac0: 656c 6174 6976 6544 6174 6573 5f10 0f73  elativeDates_..s
-00002ad0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
-00002ae0: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
-00002af0: 7465 416c 6c53 697a 6573 5874 6578 7453  teAllSizesXtextS
-00002b00: 697a 655a 736f 7274 436f 6c75 6d6e 5869  izeZsortColumnXi
-00002b10: 636f 6e53 697a 655f 1012 7669 6577 4f70  conSize_..viewOp
-00002b20: 7469 6f6e 7356 6572 7369 6f6e 0909 d90c  tionsVersion....
-00002b30: 0d0e 0f10 1112 1314 151e 2328 2c31 363b  ..........#(,16;
-00002b40: 4058 636f 6d6d 656e 7473 5e64 6174 654c  @Xcomments^dateL
-00002b50: 6173 744f 7065 6e65 645c 6461 7465 4d6f  astOpened\dateMo
-00002b60: 6469 6669 6564 5b64 6174 6543 7265 6174  dified[dateCreat
-00002b70: 6564 5473 697a 6555 6c61 6265 6c54 6b69  edTsizeUlabelTki
-00002b80: 6e64 5776 6572 7369 6f6e 546e 616d 65d4  ndWversionTname.
-00002b90: 1617 1819 1a1b 091d 5569 6e64 6578 5577  ........UindexUw
-00002ba0: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
-00002bb0: 6973 6962 6c65 1007 1101 2c09 08d4 1617  isible....,.....
-00002bc0: 1819 1f20 1d1d 1008 10c8 0808 d416 1718  ... ............
-00002bd0: 1924 251d 0910 0110 b508 09d4 1617 1819  .$%.............
-00002be0: 2925 1d1d 1002 0808 d416 1718 192d 2e1d  )%...........-..
-00002bf0: 0910 0310 6108 09d4 1617 1819 3233 091d  ....a.......23..
-00002c00: 1005 1064 0908 d416 1718 1937 3809 0910  ...d.......78...
-00002c10: 0410 7309 09d4 1617 1819 3c3d 091d 1006  ..s.......<=....
-00002c20: 104b 0908 d416 1718 1941 4209 0910 0011  .K.......AB.....
-00002c30: 0127 0909 0823 4028 0000 0000 0000 546e  .'...#@(......Tn
-00002c40: 616d 6523 4030 0000 0000 0000 0008 0019  ame#@0..........
-00002c50: 002c 003e 0046 005a 0063 006e 0077 008c  .,.>.F.Z.c.n.w..
-00002c60: 008d 008e 00a1 00aa 00b9 00c6 00d2 00d7  ................
-00002c70: 00dd 00e2 00ea 00ef 00f8 00fe 0104 010e  ................
-00002c80: 0116 0118 011b 011c 011d 0126 0128 012a  ...........&.(.*
-00002c90: 012b 012c 0135 0137 0139 013a 013b 0144  .+.,.5.7.9.:.;.D
-00002ca0: 0146 0147 0148 0151 0153 0155 0156 0157  .F.G.H.Q.S.U.V.W
-00002cb0: 0160 0162 0164 0165 0166 016f 0171 0173  .`.b.d.e.f.o.q.s
-00002cc0: 0174 0175 017e 0180 0182 0183 0184 018d  .t.u.~..........
-00002cd0: 018f 0192 0193 0194 0195 019e 01a3 0000  ................
-00002ce0: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
-00002cf0: 0000 0000 0000 0000 0000 0000 01ac 0000  ................
-00002d00: 0003 0069 006d 0067 6d6f 4444 626c 6f62  ...i.m.gmoDDblob
-00002d10: 0000 0008 aa6d bd8d 96ef c441 0000 0003  .....m.....A....
-00002d20: 0069 006d 0067 6d6f 6444 626c 6f62 0000  .i.m.gmodDblob..
-00002d30: 0008 aa6d bd8d 96ef c441 0000 0003 0069  ...m.....A.....i
-00002d40: 006d 0067 7068 3153 636f 6d70 0000 0000  .m.gph1Scomp....
-00002d50: 0016 3000 0000 0003 0069 006d 0067 7653  ..0......i.m.gvS
-00002d60: 726e 6c6f 6e67 0000 0001 0000 0007 006c  rnlong.........l
-00002d70: 006f 006f 006b 0075 0070 0073 6277 7370  .o.o.k.u.p.sbwsp
-00002d80: 626c 6f62 0000 00c8 6270 6c69 7374 3030  blob....bplist00
-00002d90: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
-00002da0: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
-00002db0: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
-00002dc0: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-00002dd0: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-00002de0: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-00002df0: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00002e00: 7208 0809 0809 5f10 177b 7b30 2c20 3131  r....._..{{0, 11
-00002e10: 367d 2c20 7b31 3235 302c 2037 3631 7d7d  6}, {1250, 761}}
-00002e20: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e98  ...%1=I`myz{|}~.
-00002e30: 0000 0000 0000 0101 0000 0000 0000 000f  ................
-00002e40: 0000 0000 0000 0000 0000 0000 0000 0099  ................
-00002e50: 0000 0007 006c 006f 006f 006b 0075 0070  .....l.o.o.k.u.p
-00002e60: 0073 6c67 3153 636f 6d70 0000 0000 0004  .slg1Scomp......
-00002e70: b1fb 0000 0000 0000 0000 0000 0000 0000  ................
+00002140: 484a 0c4c 5869 636f 6e53 697a 655f 100f  HJ.LXiconSize_..
+00002150: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
+00002160: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
+00002170: 6174 6541 6c6c 5369 7a65 735f 100f 7363  ateAllSizes_..sc
+00002180: 726f 6c6c 506f 7369 7469 6f6e 5958 7465  rollPositionYXte
+00002190: 7874 5369 7a65 5f10 0f73 6372 6f6c 6c50  xtSize_..scrollP
+000021a0: 6f73 6974 696f 6e58 5a73 6f72 7443 6f6c  ositionXZsortCol
+000021b0: 756d 6e5f 1010 7573 6552 656c 6174 6976  umn_..useRelativ
+000021c0: 6544 6174 6573 5f10 1276 6965 774f 7074  eDates_..viewOpt
+000021d0: 696f 6e73 5665 7273 696f 6e23 4030 0000  ionsVersion#@0..
+000021e0: 0000 0000 09ab 0e17 1c21 252a 2f34 393e  .........!%*/49>
+000021f0: 43d4 0f10 1112 0c14 0c16 5776 6973 6962  C.........Wvisib
+00002200: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
+00002210: 6e67 5a69 6465 6e74 6966 6965 7209 10b3  ngZidentifier...
+00002220: 0954 6e61 6d65 d40f 1011 1218 1918 1b08  .Tname..........
+00002230: 1023 0858 7562 6971 7569 7479 d40f 1011  .#.Xubiquity....
+00002240: 120c 1e18 2009 10b5 085c 6461 7465 4d6f  .... ....\dateMo
+00002250: 6469 6669 6564 d40f 1011 1218 1e18 2408  dified........$.
+00002260: 085b 6461 7465 4372 6561 7465 64d4 0f10  .[dateCreated...
+00002270: 1112 0c27 1829 0910 6108 5473 697a 65d4  ...'.)..a.Tsize.
+00002280: 0f10 1112 0c2c 0c2e 0910 7309 546b 696e  .....,....s.Tkin
+00002290: 64d4 0f10 1112 1831 0c33 0810 6409 556c  d......1.3..d.Ul
+000022a0: 6162 656c d40f 1011 1218 360c 3808 104b  abel......6.8..K
+000022b0: 0957 7665 7273 696f 6ed4 0f10 1112 183b  .Wversion......;
+000022c0: 0c3d 0811 012c 0958 636f 6d6d 656e 7473  .=...,.Xcomments
+000022d0: d40f 1011 1218 4018 4208 10c8 085e 6461  ......@.B....^da
+000022e0: 7465 4c61 7374 4f70 656e 6564 d40f 1011  teLastOpened....
+000022f0: 1218 1e18 4608 0859 6461 7465 4164 6465  ....F..YdateAdde
+00002300: 6408 2300 0000 0000 0000 0023 4028 0000  d.#........#@(..
+00002310: 0000 0000 546e 616d 6509 1001 0008 001d  ....Tname.......
+00002320: 0026 0038 0040 0054 0066 006f 0081 008c  .&.8.@.T.f.o....
+00002330: 009f 00b4 00bd 00be 00ca 00d3 00db 00e1  ................
+00002340: 00eb 00f6 00f7 00f9 00fa 00ff 0108 0109  ................
+00002350: 010b 010c 0115 011e 011f 0121 0122 012f  ...........!."./
+00002360: 0138 0139 013a 0146 014f 0150 0152 0153  .8.9.:.F.O.P.R.S
+00002370: 0158 0161 0162 0164 0165 016a 0173 0174  .X.a.b.d.e.j.s.t
+00002380: 0176 0177 017d 0186 0187 0189 018a 0192  .v.w.}..........
+00002390: 019b 019c 019f 01a0 01a9 01b2 01b3 01b5  ................
+000023a0: 01b6 01c5 01ce 01cf 01d0 01da 01db 01e4  ................
+000023b0: 01ed 01f2 01f3 0000 0000 0000 0201 0000  ................
+000023c0: 0000 0000 004d 0000 0000 0000 0000 0000  .....M..........
+000023d0: 0000 0000 01f5 0000 0005 0069 0063 006f  ...........i.c.o
+000023e0: 006e 0073 6c73 7670 626c 6f62 0000 0294  .n.slsvpblob....
+000023f0: 6270 6c69 7374 3030 da01 0203 0405 0607  bplist00........
+00002400: 0809 0a0b 0c0d 1f48 4948 4a0c 2658 6963  .......HIHJ.&Xic
+00002410: 6f6e 5369 7a65 5f10 0f73 686f 7749 636f  onSize_..showIco
+00002420: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+00002430: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+00002440: 697a 6573 5f10 0f73 6372 6f6c 6c50 6f73  izes_..scrollPos
+00002450: 6974 696f 6e59 5874 6578 7453 697a 655f  itionYXtextSize_
+00002460: 100f 7363 726f 6c6c 506f 7369 7469 6f6e  ..scrollPosition
+00002470: 585a 736f 7274 436f 6c75 6d6e 5f10 1075  XZsortColumn_..u
+00002480: 7365 5265 6c61 7469 7665 4461 7465 735f  seRelativeDates_
+00002490: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
+000024a0: 7369 6f6e 2340 3000 0000 0000 0009 d90e  sion#@0.........
+000024b0: 0f10 1112 1314 1516 1720 252a 2e33 383d  ......... %*.38=
+000024c0: 4258 636f 6d6d 656e 7473 5e64 6174 654c  BXcomments^dateL
+000024d0: 6173 744f 7065 6e65 645c 6461 7465 4d6f  astOpened\dateMo
+000024e0: 6469 6669 6564 5b64 6174 6543 7265 6174  dified[dateCreat
+000024f0: 6564 5473 697a 6555 6c61 6265 6c54 6b69  edTsizeUlabelTki
+00002500: 6e64 5776 6572 7369 6f6e 546e 616d 65d4  ndWversionTname.
+00002510: 1819 1a1b 1c1d 0c1f 5569 6e64 6578 5577  ........UindexUw
+00002520: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
+00002530: 6973 6962 6c65 1007 1101 2c09 08d4 1819  isible....,.....
+00002540: 1a1b 2122 1f1f 1008 10c8 0808 d418 191a  ..!"............
+00002550: 1b26 271f 0c10 0110 b508 09d4 1819 1a1b  .&'.............
+00002560: 2b27 1f1f 1002 0808 d418 191a 1b2f 301f  +'.........../0.
+00002570: 0c10 0310 6108 09d4 1819 1a1b 3435 0c1f  ....a.......45..
+00002580: 1005 1064 0908 d418 191a 1b39 3a0c 0c10  ...d.......9:...
+00002590: 0410 7309 09d4 1819 1a1b 3e3f 0c1f 1006  ..s.......>?....
+000025a0: 104b 0908 d418 191a 1b43 440c 0c10 0010  .K.......CD.....
+000025b0: b309 0908 2300 0000 0000 0000 0023 4028  ....#........#@(
+000025c0: 0000 0000 0000 546e 616d 6509 0008 001d  ......Tname.....
+000025d0: 0026 0038 0040 0054 0066 006f 0081 008c  .&.8.@.T.f.o....
+000025e0: 009f 00b4 00bd 00be 00d1 00da 00e9 00f6  ................
+000025f0: 0102 0107 010d 0112 011a 011f 0128 012e  .............(..
+00002600: 0134 013e 0146 0148 014b 014c 014d 0156  .4.>.F.H.K.L.M.V
+00002610: 0158 015a 015b 015c 0165 0167 0169 016a  .X.Z.[.\.e.g.i.j
+00002620: 016b 0174 0176 0177 0178 0181 0183 0185  .k.t.v.w.x......
+00002630: 0186 0187 0190 0192 0194 0195 0196 019f  ................
+00002640: 01a1 01a3 01a4 01a5 01ae 01b0 01b2 01b3  ................
+00002650: 01b4 01bd 01bf 01c1 01c2 01c3 01c4 01cd  ................
+00002660: 01d6 01db 0000 0000 0000 0201 0000 0000  ................
+00002670: 0000 004c 0000 0000 0000 0000 0000 0000  ...L............
+00002680: 0000 01dc 0000 0005 0069 0063 006f 006e  .........i.c.o.n
+00002690: 0073 6d6f 4444 626c 6f62 0000 0008 da62  .smoDDblob.....b
+000026a0: afb9 1af0 c441 0000 0005 0069 0063 006f  .....A.....i.c.o
+000026b0: 006e 0073 6d6f 6444 626c 6f62 0000 0008  .n.smodDblob....
+000026c0: da62 afb9 1af0 c441 0000 0005 0069 0063  .b.....A.....i.c
+000026d0: 006f 006e 0073 7068 3153 636f 6d70 0000  .o.n.sph1Scomp..
+000026e0: 0000 0007 f000 0000 0005 0069 0063 006f  ...........i.c.o
+000026f0: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
+00002700: 0000 0003 0069 006d 0067 6277 7370 626c  .....i.m.gbwspbl
+00002710: 6f62 0000 00c9 6270 6c69 7374 3030 d701  ob....bplist00..
+00002720: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
+00002730: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00002740: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
+00002750: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
+00002760: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
+00002770: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
+00002780: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
+00002790: 0809 0809 5f10 187b 7b32 302c 2031 3232  ...._..{{20, 122
+000027a0: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
+000027b0: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
+000027c0: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
+000027d0: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
+000027e0: 0000 0300 6900 6d00 676c 6731 5363 6f6d  ....i.m.glg1Scom
+000027f0: 7000 0000 0000 161e ce00 0000 0300 6900  p.............i.
+00002800: 6d00 676c 7376 4362 6c6f 6200 0002 7962  m.glsvCblob...yb
+00002810: 706c 6973 7430 30d8 0102 0304 0506 0708  plist00.........
+00002820: 090a 0b16 4647 0a49 5869 636f 6e53 697a  ....FG.IXiconSiz
+00002830: 655f 100f 7368 6f77 4963 6f6e 5072 6576  e_..showIconPrev
+00002840: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
+00002850: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
+00002860: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
+00002870: 756d 6e5f 1010 7573 6552 656c 6174 6976  umn_..useRelativ
+00002880: 6544 6174 6573 5f10 1276 6965 774f 7074  eDates_..viewOpt
+00002890: 696f 6e73 5665 7273 696f 6e23 4030 0000  ionsVersion#@0..
+000028a0: 0000 0000 09ab 0c15 1a1f 2328 2d32 373c  ..........#(-27<
+000028b0: 41d4 0d0e 0f10 0a12 0a14 5776 6973 6962  A.........Wvisib
+000028c0: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
+000028d0: 6e67 5a69 6465 6e74 6966 6965 7209 1101  ngZidentifier...
+000028e0: 2709 546e 616d 65d4 0d0e 0f10 1617 1619  '.Tname.........
+000028f0: 0810 2308 5875 6269 7175 6974 79d4 0d0e  ..#.Xubiquity...
+00002900: 0f10 0a1c 161e 0910 b508 5c64 6174 654d  ..........\dateM
+00002910: 6f64 6966 6965 64d4 0d0e 0f10 161c 1622  odified........"
+00002920: 0808 5b64 6174 6543 7265 6174 6564 d40d  ..[dateCreated..
+00002930: 0e0f 100a 2516 2709 1061 0854 7369 7a65  ....%.'..a.Tsize
+00002940: d40d 0e0f 100a 2a0a 2c09 1073 0954 6b69  ......*.,..s.Tki
+00002950: 6e64 d40d 0e0f 1016 2f0a 3108 1064 0955  nd....../.1..d.U
+00002960: 6c61 6265 6cd4 0d0e 0f10 1634 0a36 0810  label......4.6..
+00002970: 4b09 5776 6572 7369 6f6e d40d 0e0f 1016  K.Wversion......
+00002980: 390a 3b08 1101 2c09 5863 6f6d 6d65 6e74  9.;...,.Xcomment
+00002990: 73d4 0d0e 0f10 163e 1640 0810 c808 5e64  s......>.@....^d
+000029a0: 6174 654c 6173 744f 7065 6e65 64d4 0d0e  ateLastOpened...
+000029b0: 0f10 161c 1644 0808 5964 6174 6541 6464  .....D..YdateAdd
+000029c0: 6564 0823 4028 0000 0000 0000 546e 616d  ed.#@(......Tnam
+000029d0: 6509 1001 0008 0019 0022 0034 003c 0050  e........".4.<.P
+000029e0: 0059 0064 0077 008c 0095 0096 00a2 00ab  .Y.d.w..........
+000029f0: 00b3 00b9 00c3 00ce 00cf 00d2 00d3 00d8  ................
+00002a00: 00e1 00e2 00e4 00e5 00ee 00f7 00f8 00fa  ................
+00002a10: 00fb 0108 0111 0112 0113 011f 0128 0129  .............(.)
+00002a20: 012b 012c 0131 013a 013b 013d 013e 0143  .+.,.1.:.;.=.>.C
+00002a30: 014c 014d 014f 0150 0156 015f 0160 0162  .L.M.O.P.V._.`.b
+00002a40: 0163 016b 0174 0175 0178 0179 0182 018b  .c.k.t.u.x.y....
+00002a50: 018c 018e 018f 019e 01a7 01a8 01a9 01b3  ................
+00002a60: 01b4 01bd 01c2 01c3 0000 0000 0000 0201  ................
+00002a70: 0000 0000 0000 004a 0000 0000 0000 0000  .......J........
+00002a80: 0000 0000 0000 01c5 0000 0003 0069 006d  .............i.m
+00002a90: 0067 6c73 7670 626c 6f62 0000 025e 6270  .glsvpblob...^bp
+00002aa0: 6c69 7374 3030 d801 0203 0405 0607 0809  list00..........
+00002ab0: 0a0b 1d46 470a 2458 6963 6f6e 5369 7a65  ...FG.$XiconSize
+00002ac0: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
+00002ad0: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
+00002ae0: 6375 6c61 7465 416c 6c53 697a 6573 5874  culateAllSizesXt
+00002af0: 6578 7453 697a 655a 736f 7274 436f 6c75  extSizeZsortColu
+00002b00: 6d6e 5f10 1075 7365 5265 6c61 7469 7665  mn_..useRelative
+00002b10: 4461 7465 735f 1012 7669 6577 4f70 7469  Dates_..viewOpti
+00002b20: 6f6e 7356 6572 7369 6f6e 2340 3000 0000  onsVersion#@0...
+00002b30: 0000 0009 d90c 0d0e 0f10 1112 1314 151e  ................
+00002b40: 2328 2c31 363b 4058 636f 6d6d 656e 7473  #(,16;@Xcomments
+00002b50: 5e64 6174 654c 6173 744f 7065 6e65 645c  ^dateLastOpened\
+00002b60: 6461 7465 4d6f 6469 6669 6564 5b64 6174  dateModified[dat
+00002b70: 6543 7265 6174 6564 5473 697a 6555 6c61  eCreatedTsizeUla
+00002b80: 6265 6c54 6b69 6e64 5776 6572 7369 6f6e  belTkindWversion
+00002b90: 546e 616d 65d4 1617 1819 1a1b 0a1d 5569  Tname.........Ui
+00002ba0: 6e64 6578 5577 6964 7468 5961 7363 656e  ndexUwidthYascen
+00002bb0: 6469 6e67 5776 6973 6962 6c65 1007 1101  dingWvisible....
+00002bc0: 2c09 08d4 1617 1819 1f20 1d1d 1008 10c8  ,........ ......
+00002bd0: 0808 d416 1718 1924 251d 0a10 0110 b508  .......$%.......
+00002be0: 09d4 1617 1819 2925 1d1d 1002 0808 d416  ......)%........
+00002bf0: 1718 192d 2e1d 0a10 0310 6108 09d4 1617  ...-......a.....
+00002c00: 1819 3233 0a1d 1005 1064 0908 d416 1718  ..23.....d......
+00002c10: 1937 380a 0a10 0410 7309 09d4 1617 1819  .78.....s.......
+00002c20: 3c3d 0a1d 1006 104b 0908 d416 1718 1941  <=.....K.......A
+00002c30: 420a 0a10 0011 0127 0909 0823 4028 0000  B......'...#@(..
+00002c40: 0000 0000 546e 616d 6509 0008 0019 0022  ....Tname......"
+00002c50: 0034 003c 0050 0059 0064 0077 008c 0095  .4.<.P.Y.d.w....
+00002c60: 0096 00a9 00b2 00c1 00ce 00da 00df 00e5  ................
+00002c70: 00ea 00f2 00f7 0100 0106 010c 0116 011e  ................
+00002c80: 0120 0123 0124 0125 012e 0130 0132 0133  . .#.$.%...0.2.3
+00002c90: 0134 013d 013f 0141 0142 0143 014c 014e  .4.=.?.A.B.C.L.N
+00002ca0: 014f 0150 0159 015b 015d 015e 015f 0168  .O.P.Y.[.].^._.h
+00002cb0: 016a 016c 016d 016e 0177 0179 017b 017c  .j.l.m.n.w.y.{.|
+00002cc0: 017d 0186 0188 018a 018b 018c 0195 0197  .}..............
+00002cd0: 019a 019b 019c 019d 01a6 01ab 0000 0000  ................
+00002ce0: 0000 0201 0000 0000 0000 0049 0000 0000  ...........I....
+00002cf0: 0000 0000 0000 0000 0000 01ac 0000 0003  ................
+00002d00: 0069 006d 0067 6d6f 4444 626c 6f62 0000  .i.m.gmoDDblob..
+00002d10: 0008 aa6d bd8d 96ef c441 0000 0003 0069  ...m.....A.....i
+00002d20: 006d 0067 6d6f 6444 626c 6f62 0000 0008  .m.gmodDblob....
+00002d30: aa6d bd8d 96ef c441 0000 0003 0069 006d  .m.....A.....i.m
+00002d40: 0067 7068 3153 636f 6d70 0000 0000 0016  .gph1Scomp......
+00002d50: 3000 0000 0003 0069 006d 0067 7653 726e  0......i.m.gvSrn
+00002d60: 6c6f 6e67 0000 0001 0000 0007 006c 006f  long.........l.o
+00002d70: 006f 006b 0075 0070 0073 6277 7370 626c  .o.k.u.p.sbwspbl
+00002d80: 6f62 0000 00c8 6270 6c69 7374 3030 d701  ob....bplist00..
+00002d90: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
+00002da0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00002db0: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
+00002dc0: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
+00002dd0: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
+00002de0: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
+00002df0: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
+00002e00: 0809 0809 5f10 177b 7b30 2c20 3131 367d  ...._..{{0, 116}
+00002e10: 2c20 7b31 3235 302c 2037 3631 7d7d 0908  , {1250, 761}}..
+00002e20: 1725 313d 4960 6d79 7a7b 7c7d 7e98 0000  .%1=I`myz{|}~...
+00002e30: 0000 0000 0101 0000 0000 0000 000f 0000  ................
+00002e40: 0000 0000 0000 0000 0000 0000 0099 0000  ................
+00002e50: 0007 006c 006f 006f 006b 0075 0070 0073  ...l.o.o.k.u.p.s
+00002e60: 6c67 3153 636f 6d70 0000 0000 0004 b1fb  lg1Scomp........
+00002e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -868,37 +868,37 @@
 00003630: 010a 010b 010c 0118 0121 0122 0124 0125  .........!.".$.%
 00003640: 012a 0133 0134 0136 0137 013c 0145 0146  .*.3.4.6.7.<.E.F
 00003650: 0148 0149 014f 0158 0159 015b 015c 0164  .H.I.O.X.Y.[.\.d
 00003660: 016d 016e 0171 0172 017b 0184 0185 0187  .m.n.q.r.{......
 00003670: 0188 0197 01a0 01a1 01a2 01ac 01ad 01b6  ................
 00003680: 01bb 01c4 0000 0000 0000 0201 0000 0000  ................
 00003690: 0000 004a 0000 0000 0000 0000 0000 0000  ...J............
-000036a0: 0000 01c5 eeee c441 0000 0005 0069 0063  .......A.....i.c
-000036b0: 006f 006e 0073 6d6f 6444 626c 6f62 0000  .o.n.smodDblob..
-000036c0: 0008 7ef0 e459 eeee c441 0000 0005 0069  ..~..Y...A.....i
-000036d0: 0063 006f 006e 0073 7068 3153 636f 6d70  .c.o.n.sph1Scomp
-000036e0: 0000 0000 0007 e000 0000 0005 0069 0063  .............i.c
-000036f0: 006f 006e 0073 7653 726e 6c6f 6e67 0000  .o.n.svSrnlong..
-00003700: 0001 0000 0003 0069 006d 0067 6277 7370  .......i.m.gbwsp
-00003710: 626c 6f62 0000 00c9 6270 6c69 7374 3030  blob....bplist00
-00003720: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
-00003730: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
-00003740: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
-00003750: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-00003760: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-00003770: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-00003780: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00003790: 7208 0809 0809 5f10 187b 7b32 302c 2031  r....._..{{20, 1
-000037a0: 3232 7d2c 207b 3130 3736 2c20 3632 317d  22}, {1076, 621}
-000037b0: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
-000037c0: 9900 0000 0000 0001 0100 0000 0000 0000  ................
-000037d0: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
-000037e0: 9a00 0000 0300 6900 6d00 676c 6731 5363  ......i.m.glg1Sc
-000037f0: 6f6d 7000 0000 0000 161e ce00 0000 0300  omp.............
-00003800: 6900 6d00 0000 0006 0000 0000 0000 380b  i.m...........8.
+000036a0: 0000 01c5 c441 0000 0005 0069 0063 006f  .....A.....i.c.o
+000036b0: 006e 0073 6d6f 6444 626c 6f62 0000 0008  .n.smodDblob....
+000036c0: da62 afb9 1af0 c441 0000 0005 0069 0063  .b.....A.....i.c
+000036d0: 006f 006e 0073 7068 3153 636f 6d70 0000  .o.n.sph1Scomp..
+000036e0: 0000 0007 f000 0000 0005 0069 0063 006f  ...........i.c.o
+000036f0: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
+00003700: 0000 0003 0069 006d 0067 6277 7370 626c  .....i.m.gbwspbl
+00003710: 6f62 0000 00c9 6270 6c69 7374 3030 d701  ob....bplist00..
+00003720: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
+00003730: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00003740: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
+00003750: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
+00003760: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
+00003770: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
+00003780: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
+00003790: 0809 0809 5f10 187b 7b32 302c 2031 3232  ...._..{{20, 122
+000037a0: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
+000037b0: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
+000037c0: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
+000037d0: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
+000037e0: 0000 0300 6900 6d00 676c 6731 5363 6f6d  ....i.m.glg1Scom
+000037f0: 7000 0000 0000 161e ce00 0000 0300 6900  p.............i.
+00003800: 6d00 676c 0000 0006 0000 0000 0000 380b  m.gl..........8.
 00003810: 0000 0045 0000 100b 0000 300b 0000 200c  ...E......0... .
 00003820: 0000 180b 0000 0000 0000 0000 0000 0000  ................
 00003830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -996,30 +996,30 @@
 00003e30: 010a 010b 010c 0118 0121 0122 0124 0125  .........!.".$.%
 00003e40: 012a 0133 0134 0136 0137 013c 0145 0146  .*.3.4.6.7.<.E.F
 00003e50: 0148 0149 014f 0158 0159 015b 015c 0164  .H.I.O.X.Y.[.\.d
 00003e60: 016d 016e 0171 0172 017b 0184 0185 0187  .m.n.q.r.{......
 00003e70: 0188 0197 01a0 01a1 01a2 01ac 01ad 01b6  ................
 00003e80: 01bb 01c4 0000 0000 0000 0201 0000 0000  ................
 00003e90: 0000 004a 0000 0000 0000 0000 0000 0000  ...J............
-00003ea0: 0000 01c5 eeee c441 0000 0005 0069 0063  .......A.....i.c
-00003eb0: 006f 006e 0073 6d6f 6444 626c 6f62 0000  .o.n.smodDblob..
-00003ec0: 0008 7ef0 e459 eeee c441 0000 0005 0069  ..~..Y...A.....i
-00003ed0: 0063 006f 006e 0073 7068 3153 636f 6d70  .c.o.n.sph1Scomp
-00003ee0: 0000 0000 0007 e000 0000 0005 0069 0063  .............i.c
-00003ef0: 006f 006e 0073 7653 726e 6c6f 6e67 0000  .o.n.svSrnlong..
-00003f00: 0001 0000 0003 0069 006d 0067 6277 7370  .......i.m.gbwsp
-00003f10: 626c 6f62 0000 00c9 6270 6c69 7374 3030  blob....bplist00
-00003f20: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
-00003f30: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
-00003f40: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
-00003f50: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-00003f60: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-00003f70: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-00003f80: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00003f90: 7208 0809 0809 5f10 187b 7b32 302c 2031  r....._..{{20, 1
-00003fa0: 3232 7d2c 207b 3130 3736 2c20 3632 317d  22}, {1076, 621}
-00003fb0: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
-00003fc0: 9900 0000 0000 0001 0100 0000 0000 0000  ................
-00003fd0: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
-00003fe0: 9a00 0000 0300 6900 6d00 676c 6731 5363  ......i.m.glg1Sc
-00003ff0: 6f6d 7000 0000 0000 161e ce00 0000 0300  omp.............
-00004000: 6900 6d00                                i.m.
+00003ea0: 0000 01c5 c441 0000 0005 0069 0063 006f  .....A.....i.c.o
+00003eb0: 006e 0073 6d6f 6444 626c 6f62 0000 0008  .n.smodDblob....
+00003ec0: da62 afb9 1af0 c441 0000 0005 0069 0063  .b.....A.....i.c
+00003ed0: 006f 006e 0073 7068 3153 636f 6d70 0000  .o.n.sph1Scomp..
+00003ee0: 0000 0007 f000 0000 0005 0069 0063 006f  ...........i.c.o
+00003ef0: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
+00003f00: 0000 0003 0069 006d 0067 6277 7370 626c  .....i.m.gbwspbl
+00003f10: 6f62 0000 00c9 6270 6c69 7374 3030 d701  ob....bplist00..
+00003f20: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
+00003f30: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00003f40: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
+00003f50: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
+00003f60: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
+00003f70: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
+00003f80: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
+00003f90: 0809 0809 5f10 187b 7b32 302c 2031 3232  ...._..{{20, 122
+00003fa0: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
+00003fb0: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
+00003fc0: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
+00003fd0: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
+00003fe0: 0000 0300 6900 6d00 676c 6731 5363 6f6d  ....i.m.glg1Scom
+00003ff0: 7000 0000 0000 161e ce00 0000 0300 6900  p.............i.
+00004000: 6d00 676c                                m.gl
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.55.7/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.55.7/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.55.7/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.55.7/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.55.7/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.55.7/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.55.7/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.55.7/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/img/splash.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/img/splash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.55.7/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.55.7/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.55.7/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.55.7/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.55.7/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/drop_bp_cords.py` & `Simba-UW-tf-dev-1.55.7/simba/drop_bp_cords.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from datetime import datetime
 from simba.rw_dfs import read_df, save_df
 from simba.read_config_unit_tests import (read_config_entry,
                                           read_config_file,
                                           check_file_exist_and_readable)
 from simba.enums import ReadConfig, Paths
 from simba.utils.errors import InvalidFilepathError
+from simba.utils.warnings import BodypartColumnNotFoundWarning
 
 
 def create_body_part_dictionary(multiAnimalStatus: bool,
                                 multiAnimalIDList: list,
                                 animalsNo: int,
                                 Xcols: list,
                                 Ycols: list,
@@ -237,16 +238,15 @@
     for bodypart in pose_lst:
         colHead1, colHead2, colHead3 = (bodypart + '_x', bodypart + '_y', bodypart + '_p')
         bp_headers.extend((colHead1, colHead2, colHead3))
     try:
         out_df = df.drop(bp_headers, axis=1)
         return out_df
     except KeyError as e:
-        print('SIMBA WARNING: SimBA could not drop bodypart coordinates, some bodypart names are missing in dataframe. SimBA expected the following body-parts, that could not be found inside the file:')
-        print(e.args[0])
+        BodypartColumnNotFoundWarning(msg=f'SIMBA WARNING: SimBA could not drop bodypart coordinates, some bodypart names are missing in dataframe. SimBA expected the following body-parts, that could not be found inside the file: {e.args[0]}')
 
 def define_movement_cols(multi_animal_id_list: list):
     """
     Helper to create column names representing aggregate movement and velocity for each animal in the video.
 
     Parameters
     ----------
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/read_config_unit_tests.py` & `Simba-UW-tf-dev-1.55.7/simba/read_config_unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/project_config_creator.py` & `Simba-UW-tf-dev-1.55.7/simba/project_config_creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 __author__ = "Simon Nilsson"
 
 import os
 import platform
 from configparser import ConfigParser
 import simba
-from simba.misc_tools import SimbaTimer
+from simba.misc_tools import SimbaTimer, stdout_success
 from simba.utils.errors import DirectoryExistError
 import csv
-from simba.enums import DirNames, ReadConfig, Dtypes, Paths
+from simba.enums import (DirNames,
+                         ReadConfig,
+                         Dtypes,
+                         Paths,
+                         Defaults,
+                         TagNames)
 
 class ProjectConfigCreator(object):
 
     """
     Class for creating SimBA project directory tree and project_config.ini
 
     Parameters
@@ -177,8 +182,9 @@
 
         project_bp_file_path = os.path.join(self.bp_names_folder, 'project_bp_names.csv')
         f = open(project_bp_file_path, 'w+')
         for i in chosen_bps:
             f.write(i + '\n')
         f.close()
         self.timer.stop_timer()
-        print('SIMBA COMPLETE: Project directory tree and project_config.ini created in {} (elapsed time: {}s)'.format(self.project_folder, self.timer.elapsed_time_str))
+
+        stdout_success(msg=f'Project directory tree and project_config.ini created in {self.project_folder}', elapsed_time=self.timer.elapsed_time_str)
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/set_hyperparameters.py` & `Simba-UW-tf-dev-1.55.7/simba/set_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/train_single_model.py` & `Simba-UW-tf-dev-1.55.7/simba/train_single_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,20 +29,23 @@
                                           read_config_entry,
                                           read_config_file,
                                           check_if_filepath_list_is_empty,
                                           read_project_path_and_file_type)
 from simba.drop_bp_cords import drop_bp_cords
 from sklearn.model_selection import train_test_split
 from sklearn.ensemble import RandomForestClassifier
-from simba.misc_tools import SimbaTimer
+from simba.misc_tools import (SimbaTimer,
+                              stdout_success)
 from simba.enums import (Options,
                          ReadConfig,
                          Dtypes,
                          Paths,
-                         Methods)
+                         Methods,
+                         Defaults,
+                         TagNames)
 
 class TrainSingleModel(object):
     """
     Class for training a single random forest model from hyper-parameter setting and sampling methods
     stored within the SimBA project config .ini file (`global environment`).
 
     Parameters
@@ -271,16 +274,16 @@
         Returns
         ----------
         None
         """
 
         self.timer.stop_timer()
         save_rf_model(self.rf_clf, self.clf_name, self.model_dir_out)
-        print('Classifier {} saved in models/generated_models directory (elapsed time: {}s).'.format(self.clf_name, self.timer.elapsed_time_str))
-        print('Evaluation files are in models/generated_models/model_evaluations folders')
+        stdout_success(msg='Classifier {} saved in models/generated_models directory', elapsed_time=self.timer.elapsed_time_str)
+        stdout_success(msg=f'Evaluation files are in models/generated_models/model_evaluations folders')
 
 # test = TrainSingleModel(config_path='/Users/simon/Desktop/envs/troubleshooting/locomotion/project_folder/project_config.ini')
 # test.perform_sampling()
 # test.train_model()
 # test.save_model()
 
 # test = TrainSingleModel(config_path='/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/create_clf_log.py` & `Simba-UW-tf-dev-1.55.7/simba/create_clf_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pandas as pd
 from simba.read_config_unit_tests import (check_file_exist_and_readable,
                                           check_if_filepath_list_is_empty)
 from simba.feature_extractors.unit_tests import read_video_info
 import os
 from simba.mixins.config_reader import ConfigReader
 from simba.drop_bp_cords import get_fn_ext
-from simba.misc_tools import detect_bouts
+from simba.misc_tools import detect_bouts, stdout_success
 from simba.rw_dfs import read_df
 
 class ClfLogCreator(ConfigReader):
     """
     Class for creating aggregate statistics from classification data.
 
     Parameters
@@ -106,16 +106,16 @@
         None
         """
 
         self.results_df = self.results_df[self.results_df['Measure'].isin(self.chosen_measures)].sort_values(by=['Video', 'Classifier', 'Measure']).reset_index(drop=True)
         self.results_df = self.results_df[self.results_df['Classifier'].isin(self.classifiers)].set_index('Video')
         self.results_df.to_csv(self.file_save_name)
         self.timer.stop_timer()
-        print(f'SIMBA COMPLETE: Data log saved at {self.file_save_name} (elapsed time: {self.timer.elapsed_time_str}s)')
 
+        stdout_success(msg=f'Data log saved at {self.file_save_name}', elapsed_time=self.timer.elapsed_time_str)
 
 # test = ClfLogCreator(config_path=r"/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini",
 #                      data_measures=['Bout count',
 #                                     'Total event duration (s)'],
 #                      classifiers=['Attack', 'Sniffing'])
 # test.run()
 # test.save()
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/batch_process_videos/.DS_Store` & `Simba-UW-tf-dev-1.55.7/simba/batch_process_videos/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/batch_process_videos/batch_process_menus.py` & `Simba-UW-tf-dev-1.55.7/simba/batch_process_videos/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.55.7/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,21 +127,19 @@
         for video, video_data in self.videos_to_frm_cnt.items():
             print('Applying frame count print {}...'.format(video))
             in_path, out_path = video_data['path'], os.path.join(self.process_dir, os.path.basename(video_data['path']))
             try:
                 command = 'ffmpeg -i ' + '"' + in_path + '"' + ' -vf "drawtext=fontfile=Arial.ttf: text=\'%{frame_num}\': start_number=0: x=(w-tw)/2: y=h-(2*lh): fontcolor=black: fontsize=20: box=1: boxcolor=white: boxborderw=5" -c:a copy -y ' + '"' + out_path + '" -hide_banner -loglevel error'
                 subprocess.check_output(command, shell=True)
                 subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-                print('s')
             except:
                 simba_cw = os.path.dirname(simba.__file__)
                 simba_font_path = pathlib.Path(simba_cw, 'assets', 'UbuntuMono-Regular.ttf')
                 command = 'ffmpeg -i "' + in_path + '" -vf "drawtext=fontfile={}:'.format(simba_font_path) + "text='%{frame_num}': start_number=1: x=(w-tw)/2: y=h-(2*lh): fontcolor=black: fontsize=20: box=1: boxcolor=white: boxborderw=5" + '" ' + '-c:a copy -y "' + out_path + '" -hide_banner -loglevel error'
                 subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-                print('p')
         self.replace_files_in_temp()
         print('Applying frame count complete...')
 
     def apply_clahe(self):
         self.videos_to_frm_cnt = self.find_relevant_videos(variable='clahe')
         self.create_process_dir()
         for video, video_data in self.videos_to_frm_cnt.items():
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/Kleinberg_calculator.py` & `Simba-UW-tf-dev-1.55.7/simba/Kleinberg_calculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,18 @@
                                           check_float,
                                           check_if_filepath_list_is_empty)
 import os
 from simba.rw_dfs import read_df, save_df
 from simba.drop_bp_cords import get_fn_ext
 import pandas as pd
 from simba.pybursts import kleinberg_burst_detection
+from simba.misc_tools import stdout_success
 from simba.enums import Paths
 from simba.mixins.config_reader import ConfigReader
+from simba.utils.warnings import KleinbergWarning
 import numpy as np
 import shutil
 from copy import deepcopy
 
 class KleinbergCalculator(ConfigReader):
     '''
     Class for smoothing classification results using the Kleinberg burst
@@ -146,18 +148,17 @@
             save_df(video_out_df, self.file_type, file_path)
 
         self.timer.stop_timer()
         if len(detailed_df_lst) > 0:
             detailed_df = pd.concat(detailed_df_lst, axis=0)
             detailed_save_path = os.path.join(self.logs_path, 'Kleinberg_detailed_log_{}.csv'.format(str(self.datetime)))
             detailed_df.to_csv(detailed_save_path)
-            print('SIMBA COMPLETE: Kleinberg analysis complete. See {} for details of detected bouts of all classifiers in all hierarchies (elapsed time: {}s)'.format(detailed_save_path, self.timer.elapsed_time_str))
+            stdout_success(msg='Kleinberg analysis complete. See {detailed_save_path} for details of detected bouts of all classifiers in all hierarchies', elapsed_time=self.timer.elapsed_time_str)
         else:
-            print('SIMBA WARNING: All behavior bouts removed following kleinberg smoothing (elapsed time: {}s).'.format(self.timer.elapsed_time_str))
-
+            KleinbergWarning(msg='All behavior bouts removed following kleinberg smoothing')
 
 # test = KleinbergCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals/project_folder/project_config.ini',
 #                            classifier_names=['Attack'],
 #                            sigma=1.1,
 #                            gamma=0.3,
 #                            hierarchy=5,
 #                            hierarchical_search=False)
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/reorganize_keypoint_in_pose.py` & `Simba-UW-tf-dev-1.55.7/simba/reorganize_keypoint_in_pose.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import glob, os
 import pandas as pd
 from collections import OrderedDict
 from datetime import datetime
 from simba.read_config_unit_tests import (check_if_filepath_list_is_empty,
                                           check_if_dir_exists)
-from simba.misc_tools import check_if_filepath_list_is_empty
+from simba.misc_tools import check_if_filepath_list_is_empty, stdout_success
 from simba.enums import Formats
 
 
 class KeypointReorganizer(object):
     """
     Class for re-organizing the order of pose-estimated keypoints in directory containing
     CSV or H5 format files.
@@ -122,16 +122,15 @@
                 df_reorganized = pd.DataFrame(df, columns=new_df_ordered_cols)
                 df_reorganized.to_hdf(df_save_path, key='re-organized', format='table', mode='w')
             if self.file_format == 'csv':
                 df = pd.read_csv(file_path, header=[0, 1, 2])
                 df_reorganized = pd.DataFrame(df, columns=new_df_ordered_cols)
                 df_reorganized.to_csv(df_save_path)
             print('Saved {}, Video {}/{}.'.format(os.path.basename(file_path), str(file_cnt + 1), str(len(self.files_found))))
-        print('SIMBA COMPLETE: {} new data files with reorganized body-parts saved in {} directory'.format(str(len(self.files_found)), save_directory))
-
+        stdout_success(msg=f'{str(len(self.files_found))} new data files with reorganized body-parts saved in {save_directory} directory')
 
 #keypoint_reorganizer = KeypointReorganizer(data_folder="/Users/simon/Desktop/envs/troubleshooting/Termites_5/import_h5", pose_tool='SLEAP', file_format='csv')
```

### Comparing `Simba-UW-tf-dev-1.55.6/simba/play_annotation_video.py` & `Simba-UW-tf-dev-1.55.7/simba/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.55.7/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.55.6
+Version: 1.55.7
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.55.6/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.55.7/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -118,19 +118,22 @@
 simba/assets/icons/trash.png
 simba/assets/icons/video.png
 simba/assets/icons/visualize.png
 simba/assets/icons/concat_icons/horizontal.png
 simba/assets/icons/concat_icons/mixed_mosaic.png
 simba/assets/icons/concat_icons/mosaic.png
 simba/assets/icons/concat_icons/vertical.png
+simba/assets/img/.DS_Store
 simba/assets/img/about_me.png
 simba/assets/img/bg.png
 simba/assets/img/bg_2.png
+simba/assets/img/splash.mp4
 simba/assets/img/splash.png
 simba/assets/img/splash.pptx
+simba/assets/img/splash_1500ms.mp4
 simba/assets/lookups/.DS_Store
 simba/assets/lookups/feature_extraction_headers.csv
 simba/assets/lookups/features.csv
 simba/assets/lookups/model_names.parquet
 simba/assets/lookups/unsupervised_example_x.csv
 simba/assets/shap/.DS_Store
 simba/assets/shap/UbuntuMono-Regular.ttf
@@ -210,14 +213,15 @@
 simba/feature_extractors/misc/convex_hull_scratch_1.py
 simba/feature_extractors/misc/convex_hull_scratch_2.py
 simba/feature_extractors/misc/egocentrical_aligner.py
 simba/feature_extractors/misc/fish_feature_extractor_2022.py
 simba/feature_extractors/misc/fish_feature_extractor_2023.py
 simba/feature_extractors/misc/graph_3d_plotter.py
 simba/feature_extractors/misc/graph_creator.py
+simba/feature_extractors/misc/make_splash.py
 simba/feature_extractors/misc/mutual_exclusive.py
 simba/feature_extractors/misc/read_in_mp.py
 simba/feature_extractors/misc/termite_rois.csv
 simba/mixins/.DS_Store
 simba/mixins/config_reader.py
 simba/mixins/feature_extraction_mixin.py
 simba/mixins/pop_up_mixin.py
```

### Comparing `Simba-UW-tf-dev-1.55.6/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.55.7/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/LICENSE.md` & `Simba-UW-tf-dev-1.55.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/README.md` & `Simba-UW-tf-dev-1.55.7/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.6/setup.py` & `Simba-UW-tf-dev-1.55.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.55.6",
+    version="1.55.7",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```


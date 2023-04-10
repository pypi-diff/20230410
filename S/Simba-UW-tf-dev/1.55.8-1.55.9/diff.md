# Comparing `tmp/Simba-UW-tf-dev-1.55.8.tar.gz` & `tmp/Simba-UW-tf-dev-1.55.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.55.8.tar", last modified: Mon Apr 10 12:28:55 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.55.9.tar", last modified: Mon Apr 10 14:26:33 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.55.8.tar` & `Simba-UW-tf-dev-1.55.9.tar`

### file list

```diff
@@ -1,385 +1,386 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/
--rw-r--r--   0 simon      (501) staff       (20)    32514 2023-04-09 17:57:09.000000 Simba-UW-tf-dev-1.55.8/simba/video_processing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.55.8/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    10851 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.55.8/simba/unsupervised/unsupervised_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6566 2023-03-21 14:26:03.000000 Simba-UW-tf-dev-1.55.8/simba/unsupervised/misc.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7227 2023-03-21 11:41:26.000000 Simba-UW-tf-dev-1.55.8/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     4061 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/unsupervised/data_extractors.py
--rw-r--r--   0 simon      (501) staff       (20)    11192 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.55.8/simba/unsupervised/dbcv.py
--rw-r--r--   0 simon      (501) staff       (20)    11456 2023-03-21 18:17:26.000000 Simba-UW-tf-dev-1.55.8/simba/unsupervised/visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7526 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/unsupervised/umap_embedder.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/unsupervised/visualization_tools/
--rw-r--r--   0 simon      (501) staff       (20)     2019 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/unsupervised/visualization_tools/vtk_embeddings.py
--rw-r--r--   0 simon      (501) staff       (20)      150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/unsupervised/ui_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    49992 2023-03-22 15:08:56.000000 Simba-UW-tf-dev-1.55.8/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)    16189 2023-03-21 15:42:27.000000 Simba-UW-tf-dev-1.55.8/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6642 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3789 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     5630 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/unsupervised/cluster_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    19253 2023-04-10 11:55:27.000000 Simba-UW-tf-dev-1.55.8/simba/enums.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7518 2023-04-09 17:57:09.000000 Simba-UW-tf-dev-1.55.8/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)     8594 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.8/simba/bounding_box_tools/find_bounderies.py
--rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.55.8/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     9504 2023-04-09 17:57:09.000000 Simba-UW-tf-dev-1.55.8/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12662 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.8/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-09 00:53:36.000000 Simba-UW-tf-dev-1.55.8/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42806 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21558 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)    19620 2023-04-03 12:08:14.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/fish_feature_extractor_2023.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27987 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-09 15:55:31.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     2347 2023-04-04 12:57:34.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    10742 2023-04-09 18:45:48.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    36798 2023-03-15 17:04:48.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/extract_features_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)     8462 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)     5323 2023-03-19 18:30:53.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    46472 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    24059 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16776 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/plotly_create_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.55.8/simba/requirements.txt
--rw-r--r--   0 simon      (501) staff       (20)     5870 2023-04-09 17:32:42.000000 Simba-UW-tf-dev-1.55.8/simba/severity_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     5941 2023-03-19 16:35:16.000000 Simba-UW-tf-dev-1.55.8/simba/user_pose_config_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.55.8/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    41856 2023-04-05 17:24:50.000000 Simba-UW-tf-dev-1.55.8/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-04-07 13:58:40.000000 Simba-UW-tf-dev-1.55.8/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-06 14:21:49.000000 Simba-UW-tf-dev-1.55.8/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    34553 2023-04-10 12:16:44.000000 Simba-UW-tf-dev-1.55.8/simba/machine_model_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5261 2023-04-09 17:32:42.000000 Simba-UW-tf-dev-1.55.8/simba/remove_keypoints_in_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6366 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.8/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9955 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.8/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9208 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.8/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.55.8/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.55.8/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18290 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.8/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8339 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.8/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6932 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.8/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5467 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.8/simba/third_party_label_appenders/solomon_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7284 2023-04-09 17:01:02.000000 Simba-UW-tf-dev-1.55.8/simba/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)    12829 2023-04-09 17:01:02.000000 Simba-UW-tf-dev-1.55.8/simba/FSTTC_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.8/simba/create_project_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    13421 2023-04-06 11:40:29.000000 Simba-UW-tf-dev-1.55.8/simba/video_info_table.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.55.8/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8598 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.8/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    13530 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.8/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.55.8/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    16395 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.8/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    13231 2023-04-09 18:39:27.000000 Simba-UW-tf-dev-1.55.8/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/extract_frames_fast.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.55.8/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     5986 2023-04-10 12:27:18.000000 Simba-UW-tf-dev-1.55.8/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     4038 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.8/simba/utils/lookups.py
--rw-r--r--   0 simon      (501) staff       (20)    12855 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.8/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    21609 2023-04-10 12:16:44.000000 Simba-UW-tf-dev-1.55.8/simba/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)    10038 2023-04-09 17:40:33.000000 Simba-UW-tf-dev-1.55.8/simba/timebins_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    45516 2023-04-10 11:45:13.000000 Simba-UW-tf-dev-1.55.8/simba/train_model_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     7598 2023-04-09 17:40:33.000000 Simba-UW-tf-dev-1.55.8/simba/timebins_clf_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.55.8/simba/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     6653 2023-04-09 17:01:02.000000 Simba-UW-tf-dev-1.55.8/simba/movement_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/pybursts.py
--rw-r--r--   0 simon      (501) staff       (20)     5421 2023-04-09 17:32:42.000000 Simba-UW-tf-dev-1.55.8/simba/run_model_new.py
--rw-r--r--   0 simon      (501) staff       (20)     3104 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/rw_dfs.py
--rw-r--r--   0 simon      (501) staff       (20)     6684 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/reverse_2_animal_tracking.py
--rw-r--r--   0 simon      (501) staff       (20)     9739 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.8/simba/Directing_animals_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     4308 2023-04-09 17:57:09.000000 Simba-UW-tf-dev-1.55.8/simba/Validate_model_one_video_run_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9548 2023-04-06 00:40:25.000000 Simba-UW-tf-dev-1.55.8/simba/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.55.8/simba/setting_menu.py
--rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.55.8/simba/interpolate_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     8599 2023-04-09 19:29:40.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    17990 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14590 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12951 2023-04-09 19:32:53.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15777 2023-04-09 19:32:53.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8884 2023-04-09 19:45:13.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    16002 2023-04-09 19:41:31.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/misc_visualizations.py
--rw-r--r--   0 simon      (501) staff       (20)    13500 2023-04-09 19:41:31.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    17700 2023-04-09 19:45:13.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16307 2023-04-09 19:48:05.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12657 2023-04-09 19:32:53.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    12612 2023-04-09 19:48:05.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5861 2023-04-09 19:45:13.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12222 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    11230 2023-04-09 19:29:40.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)    12467 2023-04-09 18:45:48.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9884 2023-04-09 18:45:48.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    17318 2023-04-09 19:41:31.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    20003 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10185 2023-04-09 18:45:48.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    12473 2023-04-09 19:41:31.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8638 2023-04-09 19:29:40.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    12994 2023-04-09 19:29:40.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15652 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13196 2023-04-09 19:32:53.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-09 19:29:40.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13591 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9884 2023-04-09 18:45:48.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16155 2023-04-09 19:41:31.000000 Simba-UW-tf-dev-1.55.8/simba/plotting/heat_mapper_location_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)     7607 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.8/simba/interpolate_smooth_post_hoc.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/reverse_tracking_order.py
--rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.55.8/simba/concatenator_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2861 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.8/simba/extract_annotation_frames.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7403 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     2133 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.55.8/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43831 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    21400 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11952 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    15204 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_image.py
--rw-r--r--   0 simon      (501) staff       (20)    58097 2023-04-10 11:55:27.000000 Simba-UW-tf-dev-1.55.8/simba/misc_tools.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)    25829 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.8/simba/pose_importers/sleap_importer_slp.py
--rw-r--r--   0 simon      (501) staff       (20)    24655 2023-04-09 20:37:48.000000 Simba-UW-tf-dev-1.55.8/simba/pose_importers/sleap_importer_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    26542 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.8/simba/pose_importers/dlc_multi_animal_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    23766 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.8/simba/pose_importers/sleap_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)    16536 2023-03-20 13:30:18.000000 Simba-UW-tf-dev-1.55.8/simba/pose_importers/import_trk.py
--rw-r--r--   0 simon      (501) staff       (20)     7871 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.8/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     8967 2023-04-09 19:59:08.000000 Simba-UW-tf-dev-1.55.8/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8173 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/pose_importers/trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)   232870 2023-04-09 17:26:39.000000 Simba-UW-tf-dev-1.55.8/simba/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/extract_seqframes.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/1.png
--rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/get_coordinates_tools_v2.py
--rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.55.8/simba/pup_retrieval_protocol.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7719 2023-04-09 18:45:48.000000 Simba-UW-tf-dev-1.55.8/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.55.8/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8272 2023-04-09 18:45:48.000000 Simba-UW-tf-dev-1.55.8/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     4311 2023-04-09 18:45:48.000000 Simba-UW-tf-dev-1.55.8/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     2582 2023-04-09 17:26:39.000000 Simba-UW-tf-dev-1.55.8/simba/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)    17772 2023-04-09 17:40:33.000000 Simba-UW-tf-dev-1.55.8/simba/train_mutiple_models.py
--rw-r--r--   0 simon      (501) staff       (20)    62529 2023-04-09 17:32:42.000000 Simba-UW-tf-dev-1.55.8/simba/SimBA.py
--rw-r--r--   0 simon      (501) staff       (20)    27470 2023-04-10 12:16:44.000000 Simba-UW-tf-dev-1.55.8/simba/labelling_advanced_interface.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-09 15:55:31.000000 Simba-UW-tf-dev-1.55.8/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-09 00:58:33.000000 Simba-UW-tf-dev-1.55.8/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)    48127 2023-04-09 01:08:10.000000 Simba-UW-tf-dev-1.55.8/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.55.8/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)   454535 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/img/splash.png
--rw-r--r--   0 simon      (501) staff       (20)    59795 2023-04-09 00:58:12.000000 Simba-UW-tf-dev-1.55.8/simba/assets/img/splash_1500ms.mp4
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.55.8/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.55.8/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/assets/TheGoldenLab.PNG
--rw-r--r--   0 simon      (501) staff       (20)    21471 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.8/simba/drop_bp_cords.py
--rw-r--r--   0 simon      (501) staff       (20)     8116 2023-03-19 18:27:51.000000 Simba-UW-tf-dev-1.55.8/simba/read_config_unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    11710 2023-04-09 17:26:39.000000 Simba-UW-tf-dev-1.55.8/simba/project_config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.55.8/simba/set_hyperparameters.py
--rw-r--r--   0 simon      (501) staff       (20)    20898 2023-04-09 17:40:33.000000 Simba-UW-tf-dev-1.55.8/simba/train_single_model.py
--rw-r--r--   0 simon      (501) staff       (20)     6434 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.8/simba/create_clf_log.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/simba/batch_process_videos/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.55.8/simba/batch_process_videos/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    24896 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.55.8/simba/batch_process_videos/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/batch_process_videos/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    10882 2023-04-09 17:57:09.000000 Simba-UW-tf-dev-1.55.8/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
--rw-r--r--   0 simon      (501) staff       (20)     9581 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.8/simba/Kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8394 2023-04-09 17:32:42.000000 Simba-UW-tf-dev-1.55.8/simba/reorganize_keypoint_in_pose.py
--rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.55.8/simba/~$features.pptx
--rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.8/simba/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    13013 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      640 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.55.8/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.55.8/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.55.8/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-10 12:28:51.000000 Simba-UW-tf-dev-1.55.8/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-10 12:28:55.000000 Simba-UW-tf-dev-1.55.8/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/
+-rw-r--r--   0 simon      (501) staff       (20)    32546 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/video_processing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.55.9/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    10851 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.55.9/simba/unsupervised/unsupervised_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6566 2023-03-21 14:26:03.000000 Simba-UW-tf-dev-1.55.9/simba/unsupervised/misc.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7227 2023-03-21 11:41:26.000000 Simba-UW-tf-dev-1.55.9/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4061 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/unsupervised/data_extractors.py
+-rw-r--r--   0 simon      (501) staff       (20)    11192 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.55.9/simba/unsupervised/dbcv.py
+-rw-r--r--   0 simon      (501) staff       (20)    11456 2023-03-21 18:17:26.000000 Simba-UW-tf-dev-1.55.9/simba/unsupervised/visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7526 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/unsupervised/umap_embedder.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/unsupervised/visualization_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     2019 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/unsupervised/visualization_tools/vtk_embeddings.py
+-rw-r--r--   0 simon      (501) staff       (20)      150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/unsupervised/ui_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    49992 2023-03-22 15:08:56.000000 Simba-UW-tf-dev-1.55.9/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)    16189 2023-03-21 15:42:27.000000 Simba-UW-tf-dev-1.55.9/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6642 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3789 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     5630 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/unsupervised/cluster_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    19253 2023-04-10 11:55:27.000000 Simba-UW-tf-dev-1.55.9/simba/enums.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7520 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)     8596 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/bounding_box_tools/find_bounderies.py
+-rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.55.9/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     9536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12664 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-09 00:53:36.000000 Simba-UW-tf-dev-1.55.9/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42839 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21591 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)    19620 2023-04-03 12:08:14.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/fish_feature_extractor_2023.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    28019 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-09 15:55:31.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     2347 2023-04-04 12:57:34.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    10774 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    36798 2023-03-15 17:04:48.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/extract_features_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)     5323 2023-03-19 18:30:53.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    46505 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24092 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16809 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/plotly_create_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.55.9/simba/requirements.txt
+-rw-r--r--   0 simon      (501) staff       (20)     5872 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/severity_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5941 2023-03-19 16:35:16.000000 Simba-UW-tf-dev-1.55.9/simba/user_pose_config_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.55.9/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    41856 2023-04-05 17:24:50.000000 Simba-UW-tf-dev-1.55.9/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-04-07 13:58:40.000000 Simba-UW-tf-dev-1.55.9/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-06 14:21:49.000000 Simba-UW-tf-dev-1.55.9/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    34555 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/machine_model_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5293 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/remove_keypoints_in_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9988 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9242 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.55.9/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.55.9/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18322 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8372 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6964 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5471 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/third_party_label_appenders/solomon_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7286 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)    12862 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/FSTTC_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.9/simba/create_project_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    13421 2023-04-06 11:40:29.000000 Simba-UW-tf-dev-1.55.9/simba/video_info_table.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.55.9/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8632 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    13564 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.55.9/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    16427 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    13265 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/extract_frames_fast.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.55.9/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     6003 2023-04-10 13:29:40.000000 Simba-UW-tf-dev-1.55.9/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     4040 2023-04-10 13:56:11.000000 Simba-UW-tf-dev-1.55.9/simba/utils/lookups.py
+-rw-r--r--   0 simon      (501) staff       (20)    12855 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.55.9/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)      713 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)    21641 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     9968 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/timebins_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    45516 2023-04-10 11:45:13.000000 Simba-UW-tf-dev-1.55.9/simba/train_model_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     7600 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/timebins_clf_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.55.9/simba/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     6615 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/movement_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/pybursts.py
+-rw-r--r--   0 simon      (501) staff       (20)     5351 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/run_model_new.py
+-rw-r--r--   0 simon      (501) staff       (20)     3104 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/rw_dfs.py
+-rw-r--r--   0 simon      (501) staff       (20)     6536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/reverse_2_animal_tracking.py
+-rw-r--r--   0 simon      (501) staff       (20)     9772 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/Directing_animals_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     4312 2023-04-10 13:30:05.000000 Simba-UW-tf-dev-1.55.9/simba/Validate_model_one_video_run_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9548 2023-04-06 00:40:25.000000 Simba-UW-tf-dev-1.55.9/simba/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.55.9/simba/setting_menu.py
+-rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.55.9/simba/interpolate_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     8634 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    18024 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14622 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12985 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15811 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8917 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16036 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/misc_visualizations.py
+-rw-r--r--   0 simon      (501) staff       (20)    13533 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    17734 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16340 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12691 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    12646 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5896 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12256 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    11264 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)    12501 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9918 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    17352 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    20037 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10219 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    12507 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    13027 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15687 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13230 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     8951 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13625 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9919 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16189 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/plotting/heat_mapper_location_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)     7609 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/interpolate_smooth_post_hoc.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/reverse_tracking_order.py
+-rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.55.9/simba/concatenator_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2863 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/extract_annotation_frames.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7437 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2166 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.55.9/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43831 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    21435 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11987 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    15239 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_image.py
+-rw-r--r--   0 simon      (501) staff       (20)    57413 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/misc_tools.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)    25864 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/pose_importers/sleap_importer_slp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24689 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/pose_importers/sleap_importer_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    26576 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/pose_importers/dlc_multi_animal_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    23800 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/pose_importers/sleap_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)    16536 2023-03-20 13:30:18.000000 Simba-UW-tf-dev-1.55.9/simba/pose_importers/import_trk.py
+-rw-r--r--   0 simon      (501) staff       (20)     7905 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     9002 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8173 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/pose_importers/trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)   232872 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/extract_seqframes.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/1.png
+-rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/get_coordinates_tools_v2.py
+-rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.55.9/simba/pup_retrieval_protocol.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7751 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.55.9/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8304 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     4315 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     2614 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)    17776 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/train_mutiple_models.py
+-rw-r--r--   0 simon      (501) staff       (20)    62620 2023-04-10 13:42:47.000000 Simba-UW-tf-dev-1.55.9/simba/SimBA.py
+-rw-r--r--   0 simon      (501) staff       (20)    27472 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/labelling_advanced_interface.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-09 15:55:31.000000 Simba-UW-tf-dev-1.55.9/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-09 00:58:33.000000 Simba-UW-tf-dev-1.55.9/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)    48127 2023-04-09 01:08:10.000000 Simba-UW-tf-dev-1.55.9/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.55.9/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)   454535 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/img/splash.png
+-rw-r--r--   0 simon      (501) staff       (20)    59795 2023-04-09 00:58:12.000000 Simba-UW-tf-dev-1.55.9/simba/assets/img/splash_1500ms.mp4
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.55.9/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.55.9/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/assets/TheGoldenLab.PNG
+-rw-r--r--   0 simon      (501) staff       (20)    21459 2023-04-10 14:07:19.000000 Simba-UW-tf-dev-1.55.9/simba/drop_bp_cords.py
+-rw-r--r--   0 simon      (501) staff       (20)     8116 2023-03-19 18:27:51.000000 Simba-UW-tf-dev-1.55.9/simba/read_config_unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    11742 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/project_config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.55.9/simba/set_hyperparameters.py
+-rw-r--r--   0 simon      (501) staff       (20)    21130 2023-04-10 14:14:09.000000 Simba-UW-tf-dev-1.55.9/simba/train_single_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     6467 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/create_clf_log.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/simba/batch_process_videos/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.55.9/simba/batch_process_videos/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    24896 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.55.9/simba/batch_process_videos/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/batch_process_videos/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    10882 2023-04-09 17:57:09.000000 Simba-UW-tf-dev-1.55.9/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
+-rw-r--r--   0 simon      (501) staff       (20)     9585 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.55.9/simba/Kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8349 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.55.9/simba/reorganize_keypoint_in_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.55.9/simba/~$features.pptx
+-rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.55.9/simba/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    13037 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      640 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.55.9/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.55.9/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.55.9/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-10 14:26:27.000000 Simba-UW-tf-dev-1.55.9/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-10 14:26:33.000000 Simba-UW-tf-dev-1.55.9/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.55.8/PKG-INFO` & `Simba-UW-tf-dev-1.55.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.55.8
+Version: 1.55.9
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/video_processing.py` & `Simba-UW-tf-dev-1.55.9/simba/video_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 __author__ = "Simon Nilsson"
 
 import glob, os
 from simba.read_config_unit_tests import (check_file_exist_and_readable,
                                           check_int)
-from simba.misc_tools import (get_fn_ext, get_video_meta_data, stdout_success)
+from simba.misc_tools import (get_fn_ext, get_video_meta_data)
+from simba.utils.printing import stdout_success
 import cv2
 from pathlib import Path
 from PIL import Image
 from simba.extract_frames_fast import video_to_frames
 from simba.enums import Formats
 import re
 import subprocess
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/unsupervised/unsupervised_ui.py` & `Simba-UW-tf-dev-1.55.9/simba/unsupervised/unsupervised_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/unsupervised/misc.py` & `Simba-UW-tf-dev-1.55.9/simba/unsupervised/misc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.55.9/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/unsupervised/data_extractors.py` & `Simba-UW-tf-dev-1.55.9/simba/unsupervised/data_extractors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/unsupervised/dbcv.py` & `Simba-UW-tf-dev-1.55.9/simba/unsupervised/dbcv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/unsupervised/visualizers.py` & `Simba-UW-tf-dev-1.55.9/simba/unsupervised/visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.55.9/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/unsupervised/visualization_tools/vtk_embeddings.py` & `Simba-UW-tf-dev-1.55.9/simba/unsupervised/visualization_tools/vtk_embeddings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.55.9/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.55.9/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.55.9/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.55.9/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.55.9/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/enums.py` & `Simba-UW-tf-dev-1.55.9/simba/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.55.9/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 from simba.rw_dfs import read_df
 from simba.read_config_unit_tests import (read_config_entry,
                                           read_config_file)
 from simba.misc_tools import (detect_bouts,
-                              plug_holes_shortest_bout,
-                              stdout_success)
+                              plug_holes_shortest_bout)
+from simba.utils.printing import stdout_success
 from simba.feature_extractors.unit_tests import read_video_info_csv, read_video_info
 from simba.misc_tools import get_fn_ext
 from datetime import datetime
 import os, glob
 from simba.utils.errors import NotDirectoryError
 
 class AggBoundaryStatisticsCalculator(object):
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/bounding_box_tools/find_bounderies.py` & `Simba-UW-tf-dev-1.55.9/simba/bounding_box_tools/find_bounderies.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
                               LineString)
 import shapely.wkt
 from joblib import Parallel, delayed
 import pickle
 import platform
 from simba.enums import ReadConfig, Dtypes, Paths
 from scipy.spatial import ConvexHull
+from simba.utils.printing import stdout_success
 from simba.misc_tools import (check_multi_animal_status,
-                              find_core_cnt,
-                              stdout_success)
+                              find_core_cnt)
 
 
 class AnimalBoundaryFinder(object):
     """
     Class finding boundaries (animal-anchored) ROIs for animals in each frame. Result is saved as a pickle in the
     `project_folder/logs` directory of the SimBA project.
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.55.9/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.55.9/simba/bounding_box_tools/boundary_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import pandas as pd
 from simba.read_config_unit_tests import (read_config_file,
                                           read_config_entry,
                                           read_project_path_and_file_type)
 from simba.drop_bp_cords import (create_body_part_dictionary,
                                  getBpNames)
 from simba.enums import ReadConfig, Paths, Dtypes
-from simba.misc_tools import check_multi_animal_status, stdout_success
+from simba.misc_tools import check_multi_animal_status
+from simba.utils.printing import stdout_success
 from simba.rw_dfs import read_df, save_df
 from joblib import Parallel, delayed
 from shapely.geometry import Point
 from copy import deepcopy
 from collections import defaultdict
 from simba.utils.errors import NoFilesFoundError
 import os
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.55.9/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
                                           read_config_entry,
                                           read_project_path_and_file_type)
 from simba.read_config_unit_tests import check_file_exist_and_readable
 from simba.misc_tools import (check_multi_animal_status,
                               find_video_of_file,
                               get_video_meta_data,
                               find_core_cnt,
-                              remove_a_folder,
-                              stdout_success)
+                              remove_a_folder)
+from simba.utils.printing import stdout_success
 from simba.drop_bp_cords import (create_body_part_dictionary,
                                  getBpNames,
                                  createColorListofList)
 from simba.enums import Paths, ReadConfig, Dtypes
 from simba.rw_dfs import read_df
 import numpy as np
 import pickle
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from simba.read_config_unit_tests import (insert_default_headers_for_feature_extraction)
 import os
 from simba.feature_extractors.unit_tests import (read_video_info)
-from simba.misc_tools import get_feature_extraction_headers, stdout_success
+from simba.misc_tools import get_feature_extraction_headers
+from simba.utils.printing import stdout_success
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df, save_df
 import pandas as pd
 from copy import deepcopy
 from scipy.spatial import ConvexHull
 import scipy
 import numpy as np
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os, glob
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.read_config_unit_tests import insert_default_headers_for_feature_extraction
-from simba.misc_tools import get_feature_extraction_headers, stdout_success
+from simba.misc_tools import get_feature_extraction_headers
+from simba.utils.printing import stdout_success
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df, save_df
 import pandas as pd
 import numpy as np
 from copy import deepcopy
 import math
 from scipy.spatial import ConvexHull
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/fish_feature_extractor_2023.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/fish_feature_extractor_2023.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from simba.read_config_unit_tests import (insert_default_headers_for_feature_extraction)
-from simba.misc_tools import get_feature_extraction_headers, stdout_success
+from simba.misc_tools import get_feature_extraction_headers
+from simba.utils.printing import stdout_success
 import os
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df, save_df
 import pandas as pd
 import numpy as np
 from copy import deepcopy
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/feature_subsets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as pd
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
-from simba.misc_tools import check_if_filepath_list_is_empty, stdout_success
+from simba.misc_tools import check_if_filepath_list_is_empty
+from simba.utils.printing import stdout_success
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.misc_tools import get_fn_ext, SimbaTimer
 from simba.rw_dfs import read_df
 import os
 import numpy as np
 from itertools import combinations
 from simba.feature_extractors.perimeter_jit import jitted_hull
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/extract_features_9bp.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/extract_features_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from simba.misc_tools import (get_fn_ext,
                               SimbaTimer,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.read_config_unit_tests import check_str
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.rw_dfs import (read_df,
                           save_df)
 import os
 import pandas as pd
 import numpy as np
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/unit_tests.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from simba.read_config_unit_tests import insert_default_headers_for_feature_extraction
 import os
 from simba.feature_extractors.unit_tests import read_video_info
-from simba.misc_tools import get_feature_extraction_headers, stdout_success
+from simba.misc_tools import get_feature_extraction_headers
+from simba.utils.printing import stdout_success
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df, save_df
 import pandas as pd
 import numpy as np
 from copy import deepcopy
 import math
 from scipy.spatial import ConvexHull
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os, glob
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.read_config_unit_tests import insert_default_headers_for_feature_extraction
-from simba.misc_tools import get_feature_extraction_headers, stdout_success
+from simba.misc_tools import get_feature_extraction_headers
+from simba.utils.printing import stdout_success
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df, save_df
 import numpy as np
 import pandas as pd
 from copy import deepcopy
 import math
 from scipy.spatial import ConvexHull
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.read_config_unit_tests import insert_default_headers_for_feature_extraction
-from simba.misc_tools import get_feature_extraction_headers, stdout_success
+from simba.misc_tools import get_feature_extraction_headers
+from simba.utils.printing import stdout_success
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df, save_df
 import pandas as pd
 import numpy as np
 from copy import deepcopy
 import math
 from collections import defaultdict
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.55.9/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotly_create_h5.py` & `Simba-UW-tf-dev-1.55.9/simba/plotly_create_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/requirements.txt` & `Simba-UW-tf-dev-1.55.9/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/severity_processor.py` & `Simba-UW-tf-dev-1.55.9/simba/severity_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
                                           check_if_filepath_list_is_empty)
 from datetime import datetime
 from numba import jit
 from simba.drop_bp_cords import getBpNames, create_body_part_dictionary
 from simba.enums import ReadConfig, Dtypes, Paths
 from simba.misc_tools import (check_multi_animal_status,
                               get_fn_ext,
-                              SimbaTimer,
-                              stdout_success)
+                              SimbaTimer)
+from simba.utils.printing import stdout_success
 
 
 class SeverityProcessor(object):
     """
     Class for analyzing the `severity` of classification frame events based on how much
     the animals are moving. Frames are scored as less or more severe at lower and higher movements.
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/user_pose_config_creator.py` & `Simba-UW-tf-dev-1.55.9/simba/user_pose_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.55.9/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.55.9/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.55.9/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/machine_model_settings_pop_up.py` & `Simba-UW-tf-dev-1.55.9/simba/machine_model_settings_pop_up.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
                                      FileSelect,
                                      Entry_Box)
 import pandas as pd
 import os, ast
 from simba.enums import ReadConfig, Options, Formats, Keys, Links
 from simba.train_model_functions import get_all_clf_names
 from simba.misc_tools import (find_files_of_filetypes_in_directory,
-                              get_fn_ext,
-                              stdout_success)
+                              get_fn_ext)
+from simba.utils.printing import stdout_success
 from simba.tkinter_functions import CreateLabelFrameWithIcon
 from simba.utils.errors import InvalidHyperparametersFileError
 from simba.mixins.pop_up_mixin import PopUpMixin
 import webbrowser
 from tkinter import *
 from tkinter import ttk
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/remove_keypoints_in_pose.py` & `Simba-UW-tf-dev-1.55.9/simba/remove_keypoints_in_pose.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import glob, os
 import pandas as pd
 from datetime import datetime
 import warnings
 from tables import NaturalNameWarning
-from simba.misc_tools import SimbaTimer, stdout_success
+from simba.misc_tools import SimbaTimer
+from simba.utils.printing import stdout_success
 from simba.read_config_unit_tests import check_if_filepath_list_is_empty
 from simba.utils.errors import NotDirectoryError
 warnings.filterwarnings('ignore', category=NaturalNameWarning)
 
 class KeypointRemover(object):
     """
     Class for removing pose-estimated keypoints from data in CSV or H5 format.
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.55.9/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 __author__ = "Simon Nilsson"
 
 from simba.rw_dfs import read_df, save_df
 import os, glob
 from copy import deepcopy
 import pandas as pd
 from simba.misc_tools import (get_fn_ext,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.read_config_unit_tests import (check_if_filepath_list_is_empty,
                                           check_if_dir_exists)
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.mixins.config_reader import ConfigReader
 
 class DeepEthogramImporter(ConfigReader):
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.55.9/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 __author__ = "Simon Nilsson"
 
 from simba.read_config_unit_tests import (check_if_dir_exists,
                                           check_if_filepath_list_is_empty)
 from simba.mixins.config_reader import ConfigReader
 import os, glob
 from simba.rw_dfs import read_df, save_df
-from simba.misc_tools import (get_fn_ext, stdout_success)
+from simba.misc_tools import (get_fn_ext)
+from simba.utils.printing import stdout_success
 from simba.utils.errors import (ThirdPartyAnnotationOverlapError,
                                 ThirdPartyAnnotationEventCountError)
 from simba.utils.warnings import ThirdPartyAnnotationsOutsidePoseEstimationDataWarning
 import pandas as pd
 from copy import deepcopy
 
 class BorisAppender(ConfigReader):
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.55.9/simba/third_party_label_appenders/observer_importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from simba.mixins.config_reader import ConfigReader
 from simba.read_config_unit_tests import check_if_filepath_list_is_empty
 import os, glob
 import numpy as np
 from simba.misc_tools import (get_fn_ext,
                               SimbaTimer,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.rw_dfs import read_df, save_df
 from simba.utils.errors import (ColumnNotFoundError,
                                 AnnotationFileNotFoundError,
                                 ThirdPartyAnnotationEventCountError,
                                 ThirdPartyAnnotationOverlapError)
 from simba.utils.warnings import (ThirdPartyAnnotationsClfMissingWarning,
                                   ThirdPartyAnnotationsOutsidePoseEstimationDataWarning)
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.55.9/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.55.9/simba/third_party_label_appenders/third_party_appender.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pandas as pd
 
 from simba.mixins.config_reader import ConfigReader
 from simba.read_config_unit_tests import (check_if_dir_exists,
                                           check_if_filepath_list_is_empty)
 from simba.rw_dfs import read_df, save_df
-from simba.misc_tools import (get_fn_ext, create_logger, stdout_success)
+from simba.misc_tools import (get_fn_ext, create_logger)
+from simba.utils.printing import stdout_success
 from simba.third_party_label_appenders.tools import (read_boris_annotation_files,
                                                      read_deepethogram_files,
                                                      read_ethovision_files,
                                                      read_observer_files,
                                                      read_solomon_files,
                                                      read_bento_files,
                                                      fix_uneven_start_stop_count,
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.55.9/simba/third_party_label_appenders/ethovision_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import numpy as np
 import pandas as pd
 from simba.rw_dfs import read_df, save_df
 from simba.read_config_unit_tests import (read_config_file,
                                           check_if_filepath_list_is_empty,
                                           check_that_column_exist)
 from simba.feature_extractors.unit_tests import read_video_info
-from simba.misc_tools import get_fn_ext, stdout_success
+from simba.misc_tools import get_fn_ext
+from simba.utils.printing import stdout_success
 from simba.mixins.config_reader import ConfigReader
 
 
 class ImportEthovision(ConfigReader):
     """
     Class for appending ETHOVISION human annotations onto featurized pose-estimation data.
     Results are saved within the project_folder/csv/targets_inserted directory of
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.55.9/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 __author__ = "Simon Nilsson"
 
 
 import os, glob
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.read_config_unit_tests import check_if_filepath_list_is_empty
 from simba.mixins.config_reader import ConfigReader
-from simba.misc_tools import get_fn_ext, stdout_success
+from simba.misc_tools import get_fn_ext
+from simba.utils.printing import stdout_success
 from simba.rw_dfs import read_df, save_df
 from simba.utils.warnings import (ThirdPartyAnnotationsOutsidePoseEstimationDataWarning,
                                   ThirdPartyAnnotationsClfMissingWarning,
                                   ThirdPartyAnnotationsAdditionalClfWarning)
 from simba.utils.errors import AnnotationFileNotFoundError
 import pandas as pd
 from copy import deepcopy
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.55.9/simba/third_party_label_appenders/solomon_importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __author__ = "Simon Nilsson"
 
 import os, glob
 from simba.drop_bp_cords import get_fn_ext
 from simba.feature_extractors.unit_tests import read_video_info
-from simba.misc_tools import stdout_success
+from simba.utils.printing import stdout_success
 from simba.read_config_unit_tests import (check_if_filepath_list_is_empty,
                                           check_that_column_exist)
 from simba.rw_dfs import read_df, save_df
 from copy import deepcopy
 from simba.mixins.config_reader import ConfigReader
 
 class SolomonImporter(ConfigReader):
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/multi_cropper.py` & `Simba-UW-tf-dev-1.55.9/simba/multi_cropper.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from simba.read_config_unit_tests import (check_int,
                                           check_str,
                                           check_if_filepath_list_is_empty)
 import os, glob
 import cv2
 from copy import deepcopy
 from simba.misc_tools import (get_fn_ext,
-                              SimbaTimer,
-                              stdout_success)
+                              SimbaTimer)
+from simba.utils.printing import stdout_success
 import subprocess
 from simba.enums import Formats
 from simba.utils.errors import CountError, InvalidVideoFileError
 
 class MultiCropper(object):
     """
     Class for cropping single video into multiple videos
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/FSTTC_calculator.py` & `Simba-UW-tf-dev-1.55.9/simba/FSTTC_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from simba.read_config_unit_tests import check_if_filepath_list_is_empty
 import os
 import pandas as pd
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df
-from simba.misc_tools import (detect_bouts, stdout_success)
+from simba.misc_tools import (detect_bouts)
+from simba.utils.printing import stdout_success
 from simba.enums import Defaults, TagNames
 from simba.mixins.config_reader import ConfigReader
 import itertools
 import seaborn as sns
 
 class FSTTCPerformer(ConfigReader):
     """
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/create_project_pop_up.py` & `Simba-UW-tf-dev-1.55.9/simba/create_project_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/video_info_table.py` & `Simba-UW-tf-dev-1.55.9/simba/video_info_table.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.55.9/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import pandas as pd
 from simba.read_config_unit_tests import (read_config_entry, read_config_file, check_file_exist_and_readable)
 from simba.feature_extractors.unit_tests import read_video_info_csv, read_video_info
 import os, glob
 from simba.drop_bp_cords import getBpNames, create_body_part_dictionary
 from simba.misc_tools import (check_multi_animal_status,
                               get_fn_ext,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.rw_dfs import read_df
 from simba.read_config_unit_tests import check_that_column_exist
 from datetime import datetime
 from simba.cue_light_tools.cue_light_tools import find_frames_when_cue_light_on
 from simba.utils.errors import NoFilesFoundError
 
 class CueLightClfAnalyzer(object):
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.55.9/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from simba.drop_bp_cords import (get_fn_ext,
                                  create_body_part_dictionary)
 from simba.misc_tools import (find_video_of_file,
                               get_video_meta_data,
                               detect_bouts,
                               find_core_cnt,
                               check_multi_animal_status,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.drop_bp_cords import getBpNames
 import cv2
 import numpy as np
 import multiprocessing
 from simba.feature_extractors.unit_tests import read_video_info_csv, read_video_info
 import functools
 import time
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.55.9/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.55.9/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.55.9/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from simba.read_config_unit_tests import (read_config_entry, read_config_file, check_file_exist_and_readable)
 from simba.feature_extractors.unit_tests import read_video_info_csv, read_video_info
-from simba.misc_tools import get_video_meta_data, stdout_success
+from simba.misc_tools import get_video_meta_data
+from simba.utils.printing import stdout_success
 import itertools, os
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df
 import pandas as pd
 import cv2
 from simba.drop_bp_cords import getBpNames, create_body_part_dictionary, createColorListofList
 from simba.misc_tools import check_multi_animal_status
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.55.9/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os, glob
 from simba.read_config_unit_tests import (read_config_entry, read_config_file, check_file_exist_and_readable)
 from simba.feature_extractors.unit_tests import read_video_info_csv, read_video_info
 from simba.rw_dfs import read_df
 from simba.misc_tools import (get_fn_ext,
                               check_multi_animal_status,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.drop_bp_cords import getBpNames, create_body_part_dictionary
 from collections import defaultdict
 import pandas as pd
 import numpy as np
 from statistics import mean
 from simba.roi_tools.ROI_analyzer import ROIAnalyzer
 from datetime import datetime
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/extract_frames_fast.py` & `Simba-UW-tf-dev-1.55.9/simba/extract_frames_fast.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.55.9/simba/utils/warnings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from simba.misc_tools import *
+from simba.utils.printing import stdout_warning
 
 def ThirdPartyAnnotationsOutsidePoseEstimationDataWarning(video_name: str,
                                                           frm_cnt: int,
                                                           log_status: bool = False,
                                                           clf_name: str or None = None,
                                                           annotation_frms: int or None = None,
                                                           first_error_frm: int or None=None,
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.55.9/simba/utils/lookups.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
 
 def get_emojis() -> dict:
     return {'thank_you': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001f64f'.encode('utf-16be'))),
             'relaxed': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001F600'.encode('utf-16be'))),
             'error': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001F6A8'.encode('utf-16be'))),
             'complete': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001F680'.encode('utf-16be'))),
-            'warning': ''.join(chr(x) for x in struct.unpack('>2H', '\U000FEB23'.encode('utf-16be')))}
+            'warning': ''.join(chr(x) for x in struct.unpack('>2H', '\u2757\uFE0F'.encode('utf-16be')))}
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/utils/errors.py` & `Simba-UW-tf-dev-1.55.9/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/labelling_interface.py` & `Simba-UW-tf-dev-1.55.9/simba/labelling_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from simba.rw_dfs import read_df, save_df
 from simba.read_config_unit_tests import (read_config_entry,
                                           read_config_file,
                                           check_file_exist_and_readable,
                                           check_int,
                                           check_float,
                                           read_project_path_and_file_type)
-from simba.misc_tools import get_video_meta_data, get_fn_ext, stdout_success
+from simba.misc_tools import get_video_meta_data, get_fn_ext
+from simba.utils.printing import stdout_success
 from simba.enums import ReadConfig, Paths, Dtypes
 import simba
 from tkinter import *
 from tkinter import filedialog
 from PIL import Image, ImageTk
 from subprocess import Popen, PIPE
 import os
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/timebins_movement_analyzer.py` & `Simba-UW-tf-dev-1.55.9/simba/timebins_movement_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 
 import pandas as pd
 from simba.read_config_unit_tests import (read_config_entry,
                                           check_that_column_exist,
                                           check_if_filepath_list_is_empty)
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.misc_tools import (SimbaTimer,
-                              framewise_euclidean_distance,
-                              stdout_success)
+                              framewise_euclidean_distance)
+from simba.utils.printing import stdout_success
 from simba.enums import (ReadConfig,
-                         Dtypes,
-                         Defaults,
-                         TagNames)
+                         Dtypes)
 from simba.drop_bp_cords import create_body_part_dictionary, getBpNames
 import os, glob
 from simba.rw_dfs import read_df
 from simba.drop_bp_cords import get_fn_ext
 import seaborn as sns
 import matplotlib.pyplot as plt
 import itertools
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/train_model_functions.py` & `Simba-UW-tf-dev-1.55.9/simba/train_model_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.55.9/simba/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/timebins_clf_analyzer.py` & `Simba-UW-tf-dev-1.55.9/simba/timebins_clf_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 from simba.read_config_unit_tests import (check_int,
                                           check_if_filepath_list_is_empty)
-from simba.misc_tools import (detect_bouts,
-                              stdout_success)
+from simba.misc_tools import (detect_bouts)
+from simba.utils.printing import stdout_success
 from simba.feature_extractors.unit_tests import read_video_info
 import os, glob
 from simba.enums import Defaults, TagNames
 from simba.rw_dfs import read_df
 from simba.drop_bp_cords import get_fn_ext
 from collections import defaultdict
 from simba.mixins.config_reader import ConfigReader
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/calculate_px_dist.py` & `Simba-UW-tf-dev-1.55.9/simba/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/movement_processor.py` & `Simba-UW-tf-dev-1.55.9/simba/movement_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 from simba.misc_tools import (get_fn_ext,
                               framewise_euclidean_distance,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.read_config_unit_tests import (read_config_entry,
                                           check_if_filepath_list_is_empty)
-from simba.enums import (ReadConfig,
-                         Defaults,
-                         TagNames)
+from simba.enums import ReadConfig
 import os
 from simba.mixins.config_reader import ConfigReader
 from collections import defaultdict
 from simba.rw_dfs import read_df
 import numpy as np
 from statistics import mean
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pybursts.py` & `Simba-UW-tf-dev-1.55.9/simba/pybursts.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/run_model_new.py` & `Simba-UW-tf-dev-1.55.9/simba/run_model_new.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,19 @@
                                                read_video_info)
 from simba.read_config_unit_tests import (read_config_entry,
                                           read_config_file,
                                           read_project_path_and_file_type)
 from simba.train_model_functions import get_model_info
 from simba.misc_tools import (get_fn_ext,
                               plug_holes_shortest_bout,
-                              SimbaTimer,
-                              stdout_success)
+                              SimbaTimer)
+from simba.utils.printing import stdout_success
 from simba.enums import (ReadConfig,
                          Paths,
-                         Dtypes,
-                         Defaults,
-                         TagNames)
+                         Dtypes)
 from simba.drop_bp_cords import drop_bp_cords
 from simba.rw_dfs import read_df, save_df
 import os, glob
 from copy import deepcopy
 import pickle
 import numpy as np
 from simba.utils.errors import NoFilesFoundError
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/rw_dfs.py` & `Simba-UW-tf-dev-1.55.9/simba/rw_dfs.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/reverse_2_animal_tracking.py` & `Simba-UW-tf-dev-1.55.9/simba/reverse_2_animal_tracking.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,24 +4,22 @@
 import shutil
 from simba.read_config_unit_tests import read_config_entry, check_that_column_exist, read_config_file, check_file_exist_and_readable
 from datetime import datetime
 from simba.misc_tools import check_multi_animal_status, get_fn_ext
 import os, glob
 from simba.rw_dfs import read_df, save_df
 from simba.drop_bp_cords import getBpNames, create_body_part_dictionary
-from simba.features_scripts.feature_extractor_16bp import ExtractFeaturesFrom16bps
-from simba.features_scripts.feature_extractor_14bp import ExtractFeaturesFrom14bps
-from simba.features_scripts.extract_features_14bp_from_16bp import extract_features_wotarget_14_from_16
-from simba.features_scripts.extract_features_9bp import extract_features_wotarget_9
-from simba.features_scripts.feature_extractor_8bp import ExtractFeaturesFrom8bps
-from simba.features_scripts.feature_extractor_7bp import ExtractFeaturesFrom7bps
-from simba.features_scripts.feature_extractor_4bp import ExtractFeaturesFrom4bps
-from simba.features_scripts.feature_extractor_user_defined import UserDefinedFeatureExtractor
+from simba.feature_extractors.feature_extractor_16bp import ExtractFeaturesFrom16bps
+from simba.feature_extractors.feature_extractor_14bp import ExtractFeaturesFrom14bps
+from simba.feature_extractors.extract_features_9bp import extract_features_wotarget_9
+from simba.feature_extractors.feature_extractor_8bp import ExtractFeaturesFrom8bps
+from simba.feature_extractors.feature_extractor_7bp import ExtractFeaturesFrom7bps
+from simba.feature_extractors.feature_extractor_4bp import ExtractFeaturesFrom4bps
+from simba.feature_extractors.feature_extractor_user_defined import UserDefinedFeatureExtractor
 from simba.train_model_functions import get_all_clf_names
-from _legacy.test import check_that_two_dfs_are_equal_len
 
 class Reverse2AnimalTracking(object):
     def __init__(self,
                  config_path: str):
 
         self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
         self.config, self.config_path = read_config_file(config_path), config_path
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/Directing_animals_analyzer.py` & `Simba-UW-tf-dev-1.55.9/simba/Directing_animals_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 __author__ = "Simon Nilsson"
 
 from simba.read_config_unit_tests import check_if_filepath_list_is_empty
 from simba.feature_extractors.unit_tests import read_video_info
-from simba.misc_tools import line_length_numba, SimbaTimer, stdout_success
+from simba.misc_tools import line_length_numba, SimbaTimer
+from simba.utils.printing import stdout_success
 from simba.drop_bp_cords import (get_fn_ext,
                                  checkDirectionalityCords)
 from simba.rw_dfs import read_df
 import pandas as pd
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import AnimalNumberError
 import itertools
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/Validate_model_one_video_run_clf.py` & `Simba-UW-tf-dev-1.55.9/simba/Validate_model_one_video_run_clf.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from simba.rw_dfs import (read_df,
                           save_df)
 from simba.train_model_functions import read_pickle
 from simba.drop_bp_cords import (get_fn_ext,
                                  drop_bp_cords)
 from copy import deepcopy
-from simba.misc_tools import stdout_success
+from simba.utils.printing import stdout_success
 import warnings
 import time
 import os
 warnings.filterwarnings('ignore',category=FutureWarning)
 warnings.filterwarnings('ignore',category=DeprecationWarning)
 
 class ValidateModelRunClf(object):
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/tkinter_functions.py` & `Simba-UW-tf-dev-1.55.9/simba/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/setting_menu.py` & `Simba-UW-tf-dev-1.55.9/simba/setting_menu.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/interpolate_pose.py` & `Simba-UW-tf-dev-1.55.9/simba/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/gantt_creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 __author__ = "Simon Nilsson"
 
 from simba.misc_tools import (detect_bouts,
                               get_named_colors,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.read_config_unit_tests import check_if_filepath_list_is_empty
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.enums import Formats
 from simba.plotting.misc_visualizations import make_gantt_plot
 from simba.train_model_functions import get_all_clf_names
 from simba.drop_bp_cords import get_fn_ext
 from simba.mixins.config_reader import ConfigReader
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/ROI_plotter_mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 import functools
 from simba.enums import Formats, Paths
 from simba.misc_tools import (get_video_meta_data,
                               add_missing_ROI_cols,
                               SimbaTimer,
                               detect_bouts,
                               concatenate_videos_in_folder,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 import numpy as np
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import NoFilesFoundError
 
 pd.options.mode.chained_assignment = None
 def _img_creator(data: pd.DataFrame,
                  loc_dict: dict,
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import cv2
 import simba
 from simba.read_config_unit_tests import (read_config_entry,
                                           read_config_file,
                                           check_file_exist_and_readable,
                                           read_project_path_and_file_type)
 from simba.enums import ReadConfig, Dtypes, Paths
-from simba.misc_tools import SimbaTimer, stdout_success
+from simba.misc_tools import SimbaTimer
+from simba.utils.printing import stdout_success
 
 class ShapAggregateStatisticsVisualizer(object):
 
     """
     Class for calculating aggregate, binned, SHAP value statistics where individual bins represent reaulated features.
     Also creates line chart visualizations reprsenting aggregations of behavior-present SHAP values.
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/gantt_creator_mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import warnings
 warnings.simplefilter(action='ignore', category=FutureWarning)
 import pandas as pd
 from simba.misc_tools import (detect_bouts,
                               concatenate_videos_in_folder,
                               SimbaTimer,
                               get_named_colors,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.read_config_unit_tests import (check_if_filepath_list_is_empty)
 from simba.feature_extractors.unit_tests import (read_video_info)
 from simba.enums import Formats
 from simba.plotting.misc_visualizations import make_gantt_plot
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df
 from simba.mixins.config_reader import ConfigReader
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/heat_mapper_clf_mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import pandas as pd
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.misc_tools import (get_fn_ext,
                               SimbaTimer,
                               remove_a_folder,
                               concatenate_videos_in_folder,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.plotting.misc_visualizations import make_clf_heatmap_plot
 from simba.rw_dfs import read_df
 import numpy as np
 import os
 import cv2
 from numba import jit, prange
 from simba.enums import Formats
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/probability_plot_creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 __author__ = "Simon Nilsson"
 
 from simba.read_config_unit_tests import check_that_column_exist
 from simba.feature_extractors.unit_tests import read_video_info
-from simba.misc_tools import SimbaTimer, stdout_success
+from simba.misc_tools import SimbaTimer
+from simba.utils.printing import stdout_success
 from simba.plotting.misc_visualizations import make_probability_plot
 import os
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df
 from simba.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 import matplotlib.pyplot as plt
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/misc_visualizations.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/misc_visualizations.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 import cv2
 import pandas as pd
 from matplotlib.backends.backend_agg import FigureCanvasAgg as FigureCanvas
 
 from simba.misc_tools import (get_color_dict,
                               get_named_colors,
                               SimbaTimer,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 
 
 
 def make_distance_plot(data: np.array,
                        line_attr: dict,
                        style_attr: dict,
                        fps: int,
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/plot_clf_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from simba.read_config_unit_tests import (read_config_entry,
                                           check_file_exist_and_readable,
                                           check_float,
                                           check_int)
 from simba.misc_tools import (find_video_of_file,
                               get_video_meta_data)
 from simba.rw_dfs import read_df
-from simba.misc_tools import create_single_color_lst, stdout_success
+from simba.misc_tools import create_single_color_lst
+from simba.utils.printing import stdout_success
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.drop_bp_cords import (createColorListofList,
                                  create_body_part_dictionary,
                                  get_fn_ext)
 from simba.enums import ReadConfig, Formats, Dtypes
 import os, glob
 from copy import deepcopy
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/plot_clf_results_mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
                                           check_int)
 from simba.misc_tools import (find_video_of_file,
                               get_video_meta_data,
                               concatenate_videos_in_folder)
 from simba.rw_dfs import read_df
 from simba.misc_tools import (create_single_color_lst,
                               SimbaTimer,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.feature_extractors.unit_tests import (read_video_info_csv,
                                                read_video_info)
 from simba.drop_bp_cords import (getBpNames,
                                  createColorListofList,
                                  create_body_part_dictionary,
                                  get_fn_ext)
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/ROI_feature_visualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 __author__ = "Simon Nilsson"
 
 from simba.read_config_unit_tests import check_file_exist_and_readable
 import os
-from simba.misc_tools import get_video_meta_data, stdout_success
+from simba.misc_tools import get_video_meta_data
+from simba.utils.printing import stdout_success
 from simba.drop_bp_cords import (createColorListofList,
                                  create_body_part_dictionary,
                                  get_fn_ext)
 from simba.enums import Formats
 from simba.roi_tools.ROI_feature_analyzer import ROIFeatureCreator
 import cv2
 from simba.rw_dfs import read_df
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/heat_mapper_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 __author__ = "Simon Nilsson", "JJ Choong"
 
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.misc_tools import (get_fn_ext,
                               SimbaTimer,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 import os
 import cv2
 from simba.rw_dfs import read_df
 import numpy as np
 from numba import jit, prange
 import pandas as pd
 from simba.enums import Formats
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/probability_plot_creator_mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 from simba.read_config_unit_tests import check_that_column_exist
 from simba.feature_extractors.unit_tests import read_video_info
 import functools
 import pandas as pd
 from simba.misc_tools import (SimbaTimer,
                               concatenate_videos_in_folder,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.plotting.misc_visualizations import make_probability_plot
 from simba.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 import os
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/plot_pose_in_dir.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from simba.drop_bp_cords import get_fn_ext
 from pathlib import Path
 from simba.misc_tools import (find_video_of_file,
                               get_video_meta_data,
                               create_single_color_lst,
                               get_color_dict,
                               SimbaTimer,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.enums import Formats
 from simba.read_config_unit_tests import check_if_filepath_list_is_empty
 from simba.rw_dfs import read_df
 from simba.utils.errors import InvalidInputError
 
 
 ACCEPTED_DIRECTORIES = ['input_csv', 'outlier_corrected_movement', 'outlier_corrected_movement_location']
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/single_run_model_validation_video.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 from simba.misc_tools import (find_video_of_file,
                               get_fn_ext,
                               get_video_meta_data,
                               plug_holes_shortest_bout,
                               get_bouts_for_gantt,
                               create_gantt_img,
                               resize_gantt,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.feature_extractors.unit_tests import read_video_info
 plt.interactive(True)
 plt.ioff()
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
 class ValidateModelOneVideo(ConfigReader):
     """
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
                                           read_config_entry)
 import os
 import subprocess, shutil
 from simba.misc_tools import (get_video_meta_data,
                               remove_a_folder,
                               get_fn_ext,
                               SimbaTimer,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from datetime import datetime
 from simba.enums import Paths, ReadConfig
 
 
 class FrameMergererFFmpeg(object):
     """
     Class for merging separate visualizations of classifications, descriptive statistics etc., into  single
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from simba.misc_tools import (find_video_of_file,
                               get_video_meta_data,
                               SimbaTimer,
                               get_color_dict,
                               split_and_group_df,
                               remove_a_folder,
                               concatenate_videos_in_folder,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 import cv2
 import numpy as np
 import random
 from simba.rw_dfs import read_df
 import platform
 import multiprocessing
 import functools
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/clf_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from simba.read_config_unit_tests import (check_int,
                                           check_that_column_exist,
                                           check_if_filepath_list_is_empty)
 from simba.misc_tools import (find_video_of_file,
                               get_file_path_parts,
                               detect_bouts,
                               get_video_meta_data,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.rw_dfs import read_df
 import numpy as np
 import os
 import cv2
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/path_plotter_mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from collections import deque
 from simba.misc_tools import (get_fn_ext,
                               SimbaTimer,
                               get_color_dict,
                               remove_a_folder,
                               concatenate_videos_in_folder,
                               find_animal_name_from_body_part_name,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.enums import Formats
 from numba import jit, prange
 from simba.plotting.misc_visualizations import make_path_plot
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.rw_dfs import read_df
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import NoSpecifiedOutputError
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from simba.feature_extractors.unit_tests import read_video_info_csv
 from simba.misc_tools import (check_multi_animal_status,
                               get_video_meta_data,
                               SimbaTimer,
                               split_and_group_df,
                               remove_a_folder,
                               concatenate_videos_in_folder,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.drop_bp_cords import (getBpNames,
                                  createColorListofList,
                                  create_body_part_dictionary,
                                  get_fn_ext)
 from simba.enums import Formats, Paths
 from simba.roi_tools.ROI_feature_analyzer import ROIFeatureCreator
 import cv2
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/data_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import os
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.movement_processor import MovementProcessor
 from simba.misc_tools import (check_multi_animal_status,
                               get_fn_ext,
                               SimbaTimer,
                               get_color_dict,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 import numpy as np
 import cv2
 from simba.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import NoSpecifiedOutputError
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/path_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import cv2
 
 from simba.read_config_unit_tests import check_if_filepath_list_is_empty
 from collections import deque
 from simba.misc_tools import (get_fn_ext,
                               SimbaTimer,
                               get_color_dict,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 from simba.plotting.misc_visualizations import make_path_plot
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.misc_tools import find_animal_name_from_body_part_name
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.rw_dfs import read_df
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/ez_lineplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import cv2
 import numpy as np
 from simba.drop_bp_cords import get_fn_ext
 import pandas as pd
 from simba.misc_tools import (get_video_meta_data,
                               get_color_dict,
                               SimbaTimer,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.read_config_unit_tests import read_config_file
 from simba.rw_dfs import read_df
 from copy import deepcopy
 
 class DrawPathPlot(object):
     def __init__(self,
                  data_path: str,
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/distance_plotter_mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from simba.read_config_unit_tests import check_if_filepath_list_is_empty
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.misc_tools import (get_fn_ext,
                               SimbaTimer,
                               get_color_dict,
                               remove_a_folder,
                               concatenate_videos_in_folder,
-                              stdout_success)
-
+                              )
+from simba.utils.printing import stdout_success
 from simba.plotting.misc_visualizations import make_distance_plot
 from simba.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 from simba.rw_dfs import read_df
 import numpy as np
 import matplotlib.pyplot as plt
 import PIL
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/ROI_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import os
 import itertools
 import cv2
 from simba.enums import Paths, Formats
 from simba.misc_tools import (get_video_meta_data,
                               add_missing_ROI_cols,
                               SimbaTimer,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 import numpy as np
 from simba.utils.errors import NoFilesFoundError
 
 
 class ROIPlot(object):
     """
     Class for visualizing the ROI data (number of entries/exits, time-spent-in etc)
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/heat_mapper_clf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.misc_tools import (get_fn_ext,
                               SimbaTimer,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.plotting.misc_visualizations import make_clf_heatmap_plot
 from simba.rw_dfs import read_df
 import numpy as np
 import os
 import cv2
 from numba import jit, prange
 import matplotlib.pyplot as plt
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/distance_plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 __author__ = "Simon Nilsson"
 
 from simba.read_config_unit_tests import check_if_filepath_list_is_empty
 from simba.feature_extractors.unit_tests import (read_video_info)
 from simba.misc_tools import (get_fn_ext,
                               SimbaTimer,
                               get_color_dict,
-                              stdout_success)
-
+                              )
+from simba.utils.printing import stdout_success
 from simba.plotting.misc_visualizations import make_distance_plot
-
 from simba.enums import Formats
 from simba.rw_dfs import read_df
 import numpy as np
 import matplotlib.pyplot as plt
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import NoSpecifiedOutputError
 import PIL
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 from simba.misc_tools import (find_video_of_file,
                               get_fn_ext,
                               get_video_meta_data,
                               plug_holes_shortest_bout,
                               get_bouts_for_gantt,
                               create_gantt_img,
                               resize_gantt,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from matplotlib.backends.backend_agg import FigureCanvasAgg as FigureCanvas
 from simba.misc_tools import concatenate_videos_in_folder
 from simba.feature_extractors.unit_tests import read_video_info
 import platform
 import functools
 import multiprocessing
 import matplotlib
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/Directing_animals_visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from simba.Directing_animals_analyzer import DirectingOtherAnimalsAnalyzer
 import os
 from simba.drop_bp_cords import (get_fn_ext, createColorListofList, create_body_part_dictionary)
 from simba.misc_tools import (find_video_of_file,
                               get_video_meta_data,
                               SimbaTimer,
                               get_color_dict,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 import cv2
 import numpy as np
 import random
 from simba.rw_dfs import read_df
 from simba.enums import Formats
 from simba.mixins.config_reader import ConfigReader
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.55.9/simba/plotting/heat_mapper_location_mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import pandas as pd
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.misc_tools import (get_fn_ext,
                               SimbaTimer,
                               remove_a_folder,
                               concatenate_videos_in_folder,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.plotting.misc_visualizations import make_location_heatmap_plot
 from simba.rw_dfs import read_df
 import numpy as np
 import os
 import cv2
 from numba import jit, prange
 from simba.enums import Formats
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.55.9/simba/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/interpolate_smooth_post_hoc.py` & `Simba-UW-tf-dev-1.55.9/simba/interpolate_smooth_post_hoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from scipy.signal import savgol_filter
 from simba.mixins.config_reader import ConfigReader
 from simba.misc_tools import (check_if_filepath_list_is_empty,
                               SimbaTimer,
                               get_fn_ext,
                               get_video_meta_data,
-                              find_video_of_file,
-                              stdout_success)
+                              find_video_of_file)
+from simba.utils.printing import stdout_success
 import glob, os
 from simba.rw_dfs import read_df, save_df
 import numpy as np
 import shutil
 
 class PostHocInterpolate(ConfigReader):
     def __init__(self,
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/dash_app.py` & `Simba-UW-tf-dev-1.55.9/simba/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/reverse_tracking_order.py` & `Simba-UW-tf-dev-1.55.9/simba/reverse_tracking_order.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/concatenator_pop_up.py` & `Simba-UW-tf-dev-1.55.9/simba/concatenator_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/extract_annotation_frames.py` & `Simba-UW-tf-dev-1.55.9/simba/extract_annotation_frames.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os.path
 from simba.mixins.config_reader import ConfigReader
 from simba.misc_tools import (find_video_of_file,
                               get_fn_ext,
-                              get_video_meta_data,
-                              stdout_success)
+                              get_video_meta_data)
+from simba.utils.printing import stdout_success
 from simba.read_config_unit_tests import check_that_column_exist
 from simba.rw_dfs import read_df
 from simba.enums import Dtypes
 from simba.utils.errors import FrameRangeError
 import cv2
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from simba.feature_extractors.unit_tests import (read_video_info_csv,
                                                read_video_info)
 import os
 import pandas as pd
 from simba.roi_tools.ROI_analyzer import ROIAnalyzer
 from simba.misc_tools import (get_fn_ext,
                               SimbaTimer,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.enums import ReadConfig, Paths, DirNames, Dtypes
 from simba.rw_dfs import read_df
 import itertools
 
 class ROITimebinCalculator(object):
     """
     Class for calulating how much time and how many entries animals are making into user-defined ROIs
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 __author__ = "Simon Nilsson", "JJ Choong"
 
 
 from datetime import datetime
 from simba.read_config_unit_tests import (read_config_file,
                                           read_project_path_and_file_type)
-from simba.misc_tools import SimbaTimer, stdout_success
+from simba.misc_tools import SimbaTimer
+from simba.utils.printing import stdout_success
 import os
 from simba.roi_tools.ROI_analyzer import ROIAnalyzer
 
 class ROIMovementAnalyzer(object):
     """
 
     Class for computing movements of individual animals within individual user-defined ROIs.
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import os, glob, itertools
 import numpy as np
 from shapely.geometry import Point, Polygon
 from simba.drop_bp_cords import getBpHeaders, get_fn_ext
 from simba.rw_dfs import read_df
 import pandas as pd
 from simba.misc_tools import (find_animal_name_from_body_part_name,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.enums import Paths, Keys, ReadConfig, Dtypes
 from simba.mixins.config_reader import ConfigReader
 from simba.read_config_unit_tests import read_config_entry
 from simba.utils.errors import NoFilesFoundError, NoROIDataError
 
 class ROIAnalyzer(ConfigReader):
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from simba.roi_tools.ROI_directing_analyzer import DirectingROIAnalyzer
 import numpy as np
 import os, glob
 from simba.rw_dfs import read_df, save_df
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.misc_tools import (check_directionality_viable,
                               find_animal_name_from_body_part_name,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.drop_bp_cords import createColorListofList, create_body_part_dictionary, get_fn_ext
 from simba.roi_tools.ROI_analyzer import ROIAnalyzer
 import itertools
 from copy import deepcopy
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.errors import NoFilesFoundError, NoROIDataError
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_clf_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from simba.rw_dfs import read_df
 import numpy as np
 from shapely import geometry
 from shapely.geometry import Point, Polygon
 from datetime import datetime
 from simba.misc_tools import (get_fn_ext,
                               detect_bouts,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 import os
 from simba.read_config_unit_tests import (read_config_entry,
                                           check_that_column_exist,
                                           check_if_filepath_list_is_empty)
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.enums import Keys
 from simba.mixins.config_reader import ConfigReader
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.55.9/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/misc_tools.py` & `Simba-UW-tf-dev-1.55.9/simba/misc_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1458,27 +1458,14 @@
     user_class(config_path=config_path)
 
 def find_animal_name_from_body_part_name(bp_name: str, bp_dict: dict) -> str:
     for animal_name, animal_bps in bp_dict.items():
         if bp_name in [x[:-2] for x in animal_bps['X_bps']]:
             return animal_name
 
-def stdout_success(msg: str, elapsed_time: str or None=None) -> None:
-    if elapsed_time:
-        print(f'SIMBA COMPLETE: {msg} (elapsed time: {elapsed_time}) {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.COMPLETE.value}')
-    else:
-        print(f'SIMBA COMPLETE: {msg} {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.COMPLETE.value}')
-
-def stdout_warning(msg: str, elapsed_time: str or None=None) -> None:
-    if elapsed_time:
-        print(f'SIMBA WARNING: {msg} (elapsed time: {elapsed_time}) {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.WARNING.value}')
-    else:
-        print(f'SIMBA WARNING: {msg} {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.WARNING.value}')
-
-
 def create_logger(path: str):
     logger = logging.getLogger()
     logger.setLevel(logging.INFO)
     handler = logging.FileHandler(filename=path, encoding='utf-8')  # or whatever
     handler.setFormatter(logging.Formatter('%(asctime)s %(levelname)s %(message)s'))
     logger.addHandler(handler)
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.55.9/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_importers/sleap_importer_slp.py` & `Simba-UW-tf-dev-1.55.9/simba/pose_importers/sleap_importer_slp.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,16 @@
                                  getBpNames,
                                  getBpHeaders)
 from simba.misc_tools import (find_video_of_file,
                               check_multi_animal_status,
                               smooth_data_gaussian,
                               smooth_data_savitzky_golay,
                               get_video_meta_data,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.read_config_unit_tests import (check_if_filepath_list_is_empty,
                                           read_project_path_and_file_type,
                                           read_config_file)
 from simba.enums import Paths, ReadConfig, Methods
 from simba.rw_dfs import read_df
 import json
 from collections import defaultdict
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_importers/sleap_importer_h5.py` & `Simba-UW-tf-dev-1.55.9/simba/pose_importers/sleap_importer_h5.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from simba.misc_tools import (find_video_of_file,
                               check_multi_animal_status,
                               smooth_data_gaussian,
                               smooth_data_savitzky_golay,
                               get_video_meta_data,
                               get_fn_ext,
                               SimbaTimer,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.drop_bp_cords import (createColorListofList,
                                  create_body_part_dictionary,
                                  getBpNames,
                                  getBpHeaders)
 from datetime import datetime
 from simba.enums import ReadConfig, Paths
 import itertools
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_importers/dlc_multi_animal_importer.py` & `Simba-UW-tf-dev-1.55.9/simba/pose_importers/dlc_multi_animal_importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,16 @@
                                           check_if_filepath_list_is_empty,
                                           read_project_path_and_file_type)
 import os, glob
 from simba.misc_tools import (check_multi_animal_status,
                               get_video_meta_data,
                               smooth_data_gaussian,
                               smooth_data_savitzky_golay,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.drop_bp_cords import (getBpNames,
                                  get_fn_ext,
                                  createColorListofList,
                                  create_body_part_dictionary)
 from simba.enums import Paths, ReadConfig, Dtypes
 from datetime import datetime
 import itertools
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_importers/sleap_importer_csv.py` & `Simba-UW-tf-dev-1.55.9/simba/pose_importers/sleap_importer_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import numpy as np
 from copy import deepcopy
 from simba.misc_tools import (find_video_of_file,
                               check_multi_animal_status,
                               smooth_data_gaussian,
                               smooth_data_savitzky_golay,
                               get_video_meta_data,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.drop_bp_cords import (get_fn_ext,
                                  createColorListofList,
                                  create_body_part_dictionary,
                                  getBpNames,
                                  getBpHeaders)
 from datetime import datetime
 import itertools
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_importers/import_trk.py` & `Simba-UW-tf-dev-1.55.9/simba/pose_importers/import_trk.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.55.9/simba/pose_importers/import_mars.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 import numpy as np
 import pandas as pd
 from copy import deepcopy
 from simba.rw_dfs import save_df
 from simba.misc_tools import (get_fn_ext,
                               smooth_data_gaussian,
                               smooth_data_savitzky_golay,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.enums import Paths, Methods, Dtypes
 from simba.interpolate_pose import Interpolate
 import pyarrow.parquet as pq
 import pyarrow as pa
 
 
 class MarsImporter(object):
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.55.9/simba/pose_importers/dlc_importer_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from simba.read_config_unit_tests import (read_config_file,
                                           read_project_path_and_file_type,
                                           check_file_exist_and_readable,
                                           check_if_filepath_list_is_empty,
                                           check_int)
 from simba.misc_tools import (SimbaTimer,
                               get_number_of_header_columns_in_df,
-                              stdout_success)
+                              )
+from simba.utils.printing import stdout_success
 from simba.enums import Methods
 from simba.interpolate_pose import Interpolate
 from simba.misc_tools import smooth_data_savitzky_golay, smooth_data_gaussian
 from simba.utils.errors import NoFilesFoundError, FileExistError
 
 
 def import_dlc_csv(config_path: str, source: str) -> list:
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.55.9/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pop_up_classes.py` & `Simba-UW-tf-dev-1.55.9/simba/pop_up_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,16 @@
                               get_color_dict,
                               find_all_videos_in_directory,
                               get_file_name_info_in_directory,
                               SimbaTimer,
                               find_files_of_filetypes_in_directory,
                               archive_processed_files,
                               copy_img_folder,
-                              str_2_bool,
-                              stdout_success)
+                              str_2_bool)
+from simba.utils.printing import stdout_success
 from simba.drop_bp_cords import get_fn_ext
 from simba.utils.lookups import get_third_party_appender_file_formats
 from simba.third_party_label_appenders.third_party_appender import ThirdPartyLabelAppender
 from simba.plotting.ROI_feature_visualizer import ROIfeatureVisualizer
 from simba.get_coordinates_tools_v2 import get_coordinates_nilsson
 from simba.roi_tools.ROI_clf_calculator import ROIClfCalculator
 from simba.tkinter_functions import hxtScrollbar, DropDownMenu, CreateToolTip, CreateLabelFrameWithIcon
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/extract_seqframes.py` & `Simba-UW-tf-dev-1.55.9/simba/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.55.9/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.55.9/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/get_coordinates_tools_v2.py` & `Simba-UW-tf-dev-1.55.9/simba/get_coordinates_tools_v2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pup_retrieval_protocol.py` & `Simba-UW-tf-dev-1.55.9/simba/pup_retrieval_protocol.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.55.9/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from simba.misc_tools import get_fn_ext, stdout_success
+from simba.misc_tools import get_fn_ext
+from simba.utils.printing import stdout_success
 from simba.read_config_unit_tests import read_config_entry
 from simba.train_model_functions import insert_column_headers_for_outlier_correction
 from simba.enums import ReadConfig, Dtypes
 import os, glob
 from simba.rw_dfs import read_df, save_df
 import pandas as pd
 import numpy as np
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.55.9/simba/outlier_tools/outlier_corrector_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from simba.read_config_unit_tests import read_config_entry
 import os, glob
-from simba.misc_tools import get_fn_ext, stdout_success
+from simba.misc_tools import get_fn_ext
+from simba.utils.printing import stdout_success
 from simba.rw_dfs import (read_df,
                           save_df)
 from simba.enums import ReadConfig, Dtypes
 import numpy as np
 import pandas as pd
 from simba.mixins.config_reader import ConfigReader
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.55.9/simba/outlier_tools/skip_outlier_correction.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
                                           read_project_path_and_file_type)
 import os, glob
 import pandas as pd
 from simba.drop_bp_cords import getBpNames, get_fn_ext
 from simba.rw_dfs import read_df, save_df
 from simba.enums import Paths
 from simba.train_model_functions import insert_column_headers_for_outlier_correction
-from simba.misc_tools import stdout_success
+from simba.utils.printing import stdout_success
 
 class OutlierCorrectionSkipper(object):
     """
     Class for skipping outlier correction in SimBA projects.
 
     Parameters
     ----------
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.55.9/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.55.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.55.9/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/pose_reset.py` & `Simba-UW-tf-dev-1.55.9/simba/pose_reset.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 __author__ = "Simon Nilsson"
 
 import os
 import simba
 import shutil
-from simba.misc_tools import check_file_exist_and_readable, stdout_success
+from simba.misc_tools import check_file_exist_and_readable
+from simba.utils.printing import stdout_success
 from simba.utils.lookups import get_bp_config_codes
 import pandas as pd
 
 class PoseResetter(object):
     """
     Class for deleting all user-defined pose-estimation schematics, diagrams and other settings from the
     SimBA installation
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/train_mutiple_models.py` & `Simba-UW-tf-dev-1.55.9/simba/train_mutiple_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                                           read_config_entry,
                                           read_simba_meta_files,
                                           read_meta_file,
                                           read_config_file,
                                           check_if_filepath_list_is_empty,
                                           check_if_valid_input,
                                           read_project_path_and_file_type)
-from simba.misc_tools import stdout_success
+from simba.utils.printing import stdout_success
 from simba.drop_bp_cords import drop_bp_cords
 from sklearn.model_selection import train_test_split
 from sklearn.ensemble import RandomForestClassifier
 from simba.utils.errors import InvalidInputError
 from simba.enums import (Options,
                          ReadConfig,
                          Paths,
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/SimBA.py` & `Simba-UW-tf-dev-1.55.9/simba/SimBA.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 from simba.video_info_table import VideoInfoTable
 from simba.read_config_unit_tests import check_int
 from simba.roi_tools.ROI_define import *
 from simba.roi_tools.ROI_menus import *
 from simba.roi_tools.ROI_reset import *
 from simba.misc_tools import (run_user_defined_feature_extraction_class,
                               extract_frames_from_all_videos_in_directory,
-                              get_video_meta_data,
-                              stdout_success)
+                              get_video_meta_data)
+from simba.utils.printing import stdout_success
 from simba.video_processing import (video_to_greyscale,
                                     superimpose_frame_count)
 from simba.setting_menu import SettingsMenu
 from simba.pop_up_classes import (HeatmapLocationPopup,
                                   QuickLineplotPopup,
                                   ClfByROIPopUp,
                                   FSTTCPopUp,
@@ -824,14 +824,15 @@
         y_sb = Scrollbar(self.frame, orient=VERTICAL)
         self.frame.pack(expand=True)
         self.txt = Text(self.frame, bg='white', insertborderwidth=2, height=30, width=100, yscrollcommand=y_sb)
         self.txt.tag_configure(TagNames.GREETING.value, justify='center', foreground='blue', font=("Rockwell", 16, 'bold'))
         self.txt.tag_configure(TagNames.ERROR.value, justify='left', foreground='red', font=Formats.TKINTER_FONT.value)
         self.txt.tag_configure(TagNames.STANDARD.value, justify='left', foreground='black', font=Formats.TKINTER_FONT.value)
         self.txt.tag_configure(TagNames.COMPLETE.value, justify='left', foreground='blue', font=Formats.TKINTER_FONT.value)
+        self.txt.tag_configure(TagNames.WARNING.value, justify='left', foreground='darkorange', font=Formats.TKINTER_FONT.value)
         self.txt.insert(INSERT, Defaults.WELCOME_MSG.value + emojis['relaxed'] + '\n' * 2)
         self.txt.tag_add(TagNames.GREETING.value, "1.0", "2.25")
         y_sb.pack(side=RIGHT, fill=Y)
         self.txt.pack(expand=True, fill='both')
         y_sb.config(command=self.txt.yview)
         self.txt.config(state=DISABLED, font=Formats.TKINTER_FONT.value)
 
@@ -936,11 +937,9 @@
 
 def main():
     if currentPlatform == OS.WINDOWS.value:
         import ctypes
         myappid = 'SimBA development wheel'
         ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(myappid)
     splash = SplashMovie()
-
     app = App()
-    #print(Defaults.WELCOME_MSG.value)
     app.root.mainloop()
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.55.9/simba/labelling_advanced_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from simba.rw_dfs import read_df, save_df
 from simba.read_config_unit_tests import (read_config_entry,
                                           read_config_file,
                                           check_file_exist_and_readable,
                                           check_int,
                                           read_project_path_and_file_type)
 from simba.misc_tools import (get_video_meta_data,
-                              get_fn_ext,
-                              stdout_success)
+                              get_fn_ext)
+from simba.utils.printing import stdout_success
 import simba
 from tkinter import *
 from tkinter import filedialog
 from PIL import Image, ImageTk
 from subprocess import Popen, PIPE
 import os
 from simba.train_model_functions import get_all_clf_names
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.55.9/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.55.9/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.55.9/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.55.9/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.55.9/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.55.9/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.55.9/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.55.9/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.55.9/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.55.9/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.55.9/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.55.9/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.55.9/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.55.9/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.55.9/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.55.9/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.55.9/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.55.9/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.55.9/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.55.9/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.55.9/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.55.9/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.55.9/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.55.9/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.55.9/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.55.9/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/img/splash.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/img/splash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/img/splash_1500ms.mp4` & `Simba-UW-tf-dev-1.55.9/simba/assets/img/splash_1500ms.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.55.9/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.55.9/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.55.9/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.55.9/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.55.9/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/drop_bp_cords.py` & `Simba-UW-tf-dev-1.55.9/simba/drop_bp_cords.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 __author__ = "Simon Nilsson", "JJ Choong"
 
+from simba.utils.warnings import BodypartColumnNotFoundWarning
 import configparser
 import pandas as pd
 import os
 from pathlib import Path
 from configparser import (ConfigParser,
                           NoOptionError)
 import glob
@@ -13,15 +14,15 @@
 from datetime import datetime
 from simba.rw_dfs import read_df, save_df
 from simba.read_config_unit_tests import (read_config_entry,
                                           read_config_file,
                                           check_file_exist_and_readable)
 from simba.enums import ReadConfig, Paths
 from simba.utils.errors import InvalidFilepathError
-from simba.utils.warnings import BodypartColumnNotFoundWarning
+
 
 
 def create_body_part_dictionary(multiAnimalStatus: bool,
                                 multiAnimalIDList: list,
                                 animalsNo: int,
                                 Xcols: list,
                                 Ycols: list,
@@ -238,15 +239,15 @@
     for bodypart in pose_lst:
         colHead1, colHead2, colHead3 = (bodypart + '_x', bodypart + '_y', bodypart + '_p')
         bp_headers.extend((colHead1, colHead2, colHead3))
     try:
         out_df = df.drop(bp_headers, axis=1)
         return out_df
     except KeyError as e:
-        BodypartColumnNotFoundWarning(msg=f'SIMBA WARNING: SimBA could not drop bodypart coordinates, some bodypart names are missing in dataframe. SimBA expected the following body-parts, that could not be found inside the file: {e.args[0]}')
+        BodypartColumnNotFoundWarning(msg=f'SimBA could not drop body-part coordinates, some bodypart names are missing in dataframe. SimBA expected the following body-parts, that could not be found inside the file: {e.args[0]}')
 
 def define_movement_cols(multi_animal_id_list: list):
     """
     Helper to create column names representing aggregate movement and velocity for each animal in the video.
 
     Parameters
     ----------
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/read_config_unit_tests.py` & `Simba-UW-tf-dev-1.55.9/simba/read_config_unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/project_config_creator.py` & `Simba-UW-tf-dev-1.55.9/simba/project_config_creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 __author__ = "Simon Nilsson"
 
 import os
 import platform
 from configparser import ConfigParser
 import simba
-from simba.misc_tools import SimbaTimer, stdout_success
+from simba.misc_tools import SimbaTimer
+from simba.utils.printing import stdout_success
 from simba.utils.errors import DirectoryExistError
 import csv
 from simba.enums import (DirNames,
                          ReadConfig,
                          Dtypes,
                          Paths,
                          Defaults,
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/set_hyperparameters.py` & `Simba-UW-tf-dev-1.55.9/simba/set_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/train_single_model.py` & `Simba-UW-tf-dev-1.55.9/simba/train_single_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
                                           read_config_entry,
                                           read_config_file,
                                           check_if_filepath_list_is_empty,
                                           read_project_path_and_file_type)
 from simba.drop_bp_cords import drop_bp_cords
 from sklearn.model_selection import train_test_split
 from sklearn.ensemble import RandomForestClassifier
-from simba.misc_tools import (SimbaTimer,
-                              stdout_success)
+from simba.misc_tools import (SimbaTimer)
+from simba.utils.printing import stdout_success
 from simba.enums import (Options,
                          ReadConfig,
                          Dtypes,
                          Paths,
                          Methods,
                          Defaults,
                          TagNames)
@@ -248,15 +248,15 @@
                                 x_names=self.feature_names,
                                 clf_name=self.clf_name,
                                 cnt_present=shap_target_present_cnt,
                                 cnt_absent=shap_target_absent_cnt,
                                 save_it=shap_save_n,
                                 save_path=self.eval_out_path)
 
-            if compute_partial_dependency:
+            if compute_partial_dependency in Options.PERFORM_FLAGS.value:
                 partial_dependence_calculator(clf=self.rf_clf, x_df=self.x_train, clf_name=self.clf_name, save_dir=self.eval_out_path)
 
             if save_meta_data in Options.PERFORM_FLAGS.value:
                 meta_data_lst = [self.clf_name, criterion, max_features, min_sample_leaf,
                                  n_estimators, compute_permutation_importance, generate_classification_report,
                                  generate_example_decision_tree, generate_features_importance_bar_graph,
                                  generate_features_importance_log, generate_precision_recall_curve, save_meta_data,
@@ -282,11 +282,17 @@
         stdout_success(msg=f'Evaluation files are in models/generated_models/model_evaluations folders')
 
 # test = TrainSingleModel(config_path='/Users/simon/Desktop/envs/troubleshooting/locomotion/project_folder/project_config.ini')
 # test.perform_sampling()
 # test.train_model()
 # test.save_model()
 
+
+# test = TrainSingleModel(config_path='/Users/simon/Desktop/envs/troubleshooting/prueba/project_folder/project_config.ini')
+# test.perform_sampling()
+# test.train_model()
+# test.save_model()
+
 # test = TrainSingleModel(config_path='/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/project_config.ini')
 # test.perform_sampling()
 # test.train_model()
 # test.save_model()
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/create_clf_log.py` & `Simba-UW-tf-dev-1.55.9/simba/create_clf_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import pandas as pd
 from simba.read_config_unit_tests import (check_file_exist_and_readable,
                                           check_if_filepath_list_is_empty)
 from simba.feature_extractors.unit_tests import read_video_info
 import os
 from simba.mixins.config_reader import ConfigReader
 from simba.drop_bp_cords import get_fn_ext
-from simba.misc_tools import detect_bouts, stdout_success
+from simba.misc_tools import detect_bouts
+from simba.utils.printing import stdout_success
 from simba.rw_dfs import read_df
 
 class ClfLogCreator(ConfigReader):
     """
     Class for creating aggregate statistics from classification data.
 
     Parameters
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/batch_process_videos/.DS_Store` & `Simba-UW-tf-dev-1.55.9/simba/batch_process_videos/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/batch_process_videos/batch_process_menus.py` & `Simba-UW-tf-dev-1.55.9/simba/batch_process_videos/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.55.9/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/simba/Kleinberg_calculator.py` & `Simba-UW-tf-dev-1.55.9/simba/Kleinberg_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
                                           check_float,
                                           check_if_filepath_list_is_empty)
 import os
 from simba.rw_dfs import read_df, save_df
 from simba.drop_bp_cords import get_fn_ext
 import pandas as pd
 from simba.pybursts import kleinberg_burst_detection
-from simba.misc_tools import stdout_success
+from simba.utils.printing import stdout_success
 from simba.enums import Paths
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.warnings import KleinbergWarning
 import numpy as np
 import shutil
 from copy import deepcopy
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/reorganize_keypoint_in_pose.py` & `Simba-UW-tf-dev-1.55.9/simba/reorganize_keypoint_in_pose.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import glob, os
 import pandas as pd
 from collections import OrderedDict
 from datetime import datetime
-from simba.read_config_unit_tests import (check_if_filepath_list_is_empty,
-                                          check_if_dir_exists)
-from simba.misc_tools import check_if_filepath_list_is_empty, stdout_success
+from simba.read_config_unit_tests import check_if_dir_exists
+from simba.misc_tools import check_if_filepath_list_is_empty
+from simba.utils.printing import stdout_success
 from simba.enums import Formats
 
 
 class KeypointReorganizer(object):
     """
     Class for re-organizing the order of pose-estimated keypoints in directory containing
     CSV or H5 format files.
```

### Comparing `Simba-UW-tf-dev-1.55.8/simba/play_annotation_video.py` & `Simba-UW-tf-dev-1.55.9/simba/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.55.9/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.55.8
+Version: 1.55.9
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.55.8/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.55.9/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -336,8 +336,9 @@
 simba/unsupervised/umap_embedder.py
 simba/unsupervised/unsupervised_ui.py
 simba/unsupervised/visualizers.py
 simba/unsupervised/visualization_tools/vtk_embeddings.py
 simba/utils/.DS_Store
 simba/utils/errors.py
 simba/utils/lookups.py
+simba/utils/printing.py
 simba/utils/warnings.py
```

### Comparing `Simba-UW-tf-dev-1.55.8/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.55.9/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/LICENSE.md` & `Simba-UW-tf-dev-1.55.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/README.md` & `Simba-UW-tf-dev-1.55.9/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.55.8/setup.py` & `Simba-UW-tf-dev-1.55.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.55.8",
+    version="1.55.9",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```


# Comparing `tmp/ml4h-0.0.4.dev4.tar.gz` & `tmp/ml4h-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml4h-0.0.4.dev4.tar", last modified: Mon Feb  6 18:00:48 2023, max compression
+gzip compressed data, was "ml4h-0.0.5.tar", last modified: Mon Apr 10 17:29:18 2023, max compression
```

## Comparing `ml4h-0.0.4.dev4.tar` & `ml4h-0.0.5.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-02-06 18:00:48.639245 ml4h-0.0.4.dev4/
--rw-r--r--   0 sam        (503) staff       (20)     1633 2023-01-26 10:40:07.000000 ml4h-0.0.4.dev4/LICENSE.txt
--rw-r--r--   0 sam        (503) staff       (20)     4491 2023-01-26 10:40:07.000000 ml4h-0.0.4.dev4/NOTICE.txt
--rw-r--r--   0 sam        (503) staff       (20)      229 2023-02-06 18:00:48.638641 ml4h-0.0.4.dev4/PKG-INFO
--rw-r--r--   0 sam        (503) staff       (20)     6592 2023-01-26 10:40:07.000000 ml4h-0.0.4.dev4/README.md
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-02-06 18:00:48.497634 ml4h-0.0.4.dev4/ml4h/
--rw-r--r--   0 sam        (503) staff       (20)     2361 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/DatabaseClient.py
--rwxr-xr-x   0 sam        (503) staff       (20)    23803 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/TensorMap.py
--rw-r--r--   0 sam        (503) staff       (20)       22 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/__init__.py
--rw-r--r--   0 sam        (503) staff       (20)    35435 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/arguments.py
--rwxr-xr-x   0 sam        (503) staff       (20)     9705 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/defines.py
--rw-r--r--   0 sam        (503) staff       (20)    55652 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/explorations.py
--rw-r--r--   0 sam        (503) staff       (20)     7604 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/hypertuning.py
--rw-r--r--   0 sam        (503) staff       (20)     1846 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/logger.py
--rw-r--r--   0 sam        (503) staff       (20)     6325 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/make_tensor_maps_for_partners_ecg_labels.py
--rwxr-xr-x   0 sam        (503) staff       (20)    27628 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/metrics.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-02-06 18:00:48.502383 ml4h-0.0.4.dev4/ml4h/ml4ht_integration/
--rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/ml4ht_integration/__init__.py
--rw-r--r--   0 sam        (503) staff       (20)     4264 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/ml4ht_integration/tensor_generator.py
--rw-r--r--   0 sam        (503) staff       (20)     5358 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/ml4ht_integration/tensor_map.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-02-06 18:00:48.516147 ml4h-0.0.4.dev4/ml4h/models/
--rw-r--r--   0 sam        (503) staff       (20)      422 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/models/Block.py
--rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/models/__init__.py
--rw-r--r--   0 sam        (503) staff       (20)     7921 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/models/basic_blocks.py
--rw-r--r--   0 sam        (503) staff       (20)    23869 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/models/conv_blocks.py
--rw-r--r--   0 sam        (503) staff       (20)     6020 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/models/inspect.py
--rw-r--r--   0 sam        (503) staff       (20)     6368 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/models/layer_wrappers.py
--rwxr-xr-x   0 sam        (503) staff       (20)    67636 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/models/legacy_models.py
--rw-r--r--   0 sam        (503) staff       (20)    13249 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/models/merge_blocks.py
--rw-r--r--   0 sam        (503) staff       (20)    18364 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/models/model_factory.py
--rw-r--r--   0 sam        (503) staff       (20)     3642 2023-02-01 18:47:24.000000 ml4h-0.0.4.dev4/ml4h/models/pretrained_blocks.py
--rw-r--r--   0 sam        (503) staff       (20)     4144 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/models/train.py
--rw-r--r--   0 sam        (503) staff       (20)    14384 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/models/transformer_blocks.py
--rw-r--r--   0 sam        (503) staff       (20)     2848 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/normalizer.py
--rw-r--r--   0 sam        (503) staff       (20)     4238 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/optimizers.py
--rw-r--r--   0 sam        (503) staff       (20)   128480 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/plots.py
--rwxr-xr-x   0 sam        (503) staff       (20)    49510 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/recipes.py
--rw-r--r--   0 sam        (503) staff       (20)     5424 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/runtime_data_defines.py
--rwxr-xr-x   0 sam        (503) staff       (20)    40052 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensor_generators.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-02-06 18:00:48.566961 ml4h-0.0.4.dev4/ml4h/tensorize/
--rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensorize/__init__.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-02-06 18:00:48.572931 ml4h-0.0.4.dev4/ml4h/tensorize/dataflow/
--rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensorize/dataflow/__init__.py
--rw-r--r--   0 sam        (503) staff       (20)     7724 2023-01-26 10:45:27.000000 ml4h-0.0.4.dev4/ml4h/tensorize/dataflow/bigquery_ukb_queries.py
--rw-r--r--   0 sam        (503) staff       (20)     4257 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensorize/merge_hd5s.py
--rw-r--r--   0 sam        (503) staff       (20)    18759 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensorize/tensor_writer_mgb.py
--rw-r--r--   0 sam        (503) staff       (20)    61573 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensorize/tensor_writer_ukbb.py
--rw-r--r--   0 sam        (503) staff       (20)     3243 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensorize/tensorize_dataflow.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-02-06 18:00:48.584746 ml4h-0.0.4.dev4/ml4h/tensormap/
--rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/__init__.py
--rw-r--r--   0 sam        (503) staff       (20)     8657 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/celeba.py
--rw-r--r--   0 sam        (503) staff       (20)     2152 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/gatk.py
--rw-r--r--   0 sam        (503) staff       (20)     6283 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/general.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-02-06 18:00:48.588215 ml4h-0.0.4.dev4/ml4h/tensormap/mgb/
--rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/mgb/__init__.py
--rw-r--r--   0 sam        (503) staff       (20)    47783 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/mgb/dynamic.py
--rw-r--r--   0 sam        (503) staff       (20)    73630 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/mgb/ecg.py
--rw-r--r--   0 sam        (503) staff       (20)     4035 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/mnist.py
--rw-r--r--   0 sam        (503) staff       (20)    14184 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/tensor_map_maker.py
--rw-r--r--   0 sam        (503) staff       (20)     4154 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/text.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-02-06 18:00:48.627302 ml4h-0.0.4.dev4/ml4h/tensormap/ukb/
--rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/ukb/__init__.py
--rw-r--r--   0 sam        (503) staff       (20)  2199726 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/ukb/by_script.py
--rw-r--r--   0 sam        (503) staff       (20)   127529 2023-02-06 15:34:51.000000 ml4h-0.0.4.dev4/ml4h/tensormap/ukb/categorical.py
--rw-r--r--   0 sam        (503) staff       (20)   497367 2023-02-06 16:25:53.000000 ml4h-0.0.4.dev4/ml4h/tensormap/ukb/continuous.py
--rw-r--r--   0 sam        (503) staff       (20)    41549 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/ukb/demographics.py
--rw-r--r--   0 sam        (503) staff       (20)     4465 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/ukb/dxa.py
--rw-r--r--   0 sam        (503) staff       (20)    62296 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/ukb/ecg.py
--rw-r--r--   0 sam        (503) staff       (20)    30381 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/ukb/genetics.py
--rw-r--r--   0 sam        (503) staff       (20)   118948 2023-02-01 19:12:06.000000 ml4h-0.0.4.dev4/ml4h/tensormap/ukb/mri.py
--rw-r--r--   0 sam        (503) staff       (20)    12774 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/ukb/mri_brain.py
--rw-r--r--   0 sam        (503) staff       (20)     6557 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/ukb/mri_ecg.py
--rw-r--r--   0 sam        (503) staff       (20)    11925 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/ukb/mri_vtk.py
--rw-r--r--   0 sam        (503) staff       (20)    12708 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/tensormap/ukb/survival.py
--rw-r--r--   0 sam        (503) staff       (20)     3316 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/test_utils.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-02-06 18:00:48.637607 ml4h-0.0.4.dev4/ml4h/visualization_tools/
--rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/visualization_tools/__init__.py
--rw-r--r--   0 sam        (503) staff       (20)     7219 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/visualization_tools/annotation_storage.py
--rw-r--r--   0 sam        (503) staff       (20)     5764 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/visualization_tools/annotations.py
--rw-r--r--   0 sam        (503) staff       (20)    10397 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/visualization_tools/batch_image_annotations.py
--rw-r--r--   0 sam        (503) staff       (20)    10420 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/visualization_tools/dicom_interactive_plots.py
--rw-r--r--   0 sam        (503) staff       (20)    15258 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/visualization_tools/dicom_plots.py
--rw-r--r--   0 sam        (503) staff       (20)     6203 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/visualization_tools/ecg_interactive_plots.py
--rw-r--r--   0 sam        (503) staff       (20)     9855 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/visualization_tools/ecg_reshape.py
--rw-r--r--   0 sam        (503) staff       (20)     3106 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/visualization_tools/ecg_static_plots.py
--rw-r--r--   0 sam        (503) staff       (20)     3329 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/visualization_tools/facets.py
--rw-r--r--   0 sam        (503) staff       (20)    14368 2023-01-26 10:40:08.000000 ml4h-0.0.4.dev4/ml4h/visualization_tools/hd5_mri_plots.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-02-06 18:00:48.500459 ml4h-0.0.4.dev4/ml4h.egg-info/
--rw-r--r--   0 sam        (503) staff       (20)      229 2023-02-06 18:00:48.000000 ml4h-0.0.4.dev4/ml4h.egg-info/PKG-INFO
--rw-r--r--   0 sam        (503) staff       (20)     2347 2023-02-06 18:00:48.000000 ml4h-0.0.4.dev4/ml4h.egg-info/SOURCES.txt
--rw-r--r--   0 sam        (503) staff       (20)        1 2023-02-06 18:00:48.000000 ml4h-0.0.4.dev4/ml4h.egg-info/dependency_links.txt
--rw-r--r--   0 sam        (503) staff       (20)        5 2023-02-06 18:00:48.000000 ml4h-0.0.4.dev4/ml4h.egg-info/top_level.txt
--rw-r--r--   0 sam        (503) staff       (20)       38 2023-02-06 18:00:48.639436 ml4h-0.0.4.dev4/setup.cfg
--rw-r--r--   0 sam        (503) staff       (20)      749 2023-02-06 17:59:34.000000 ml4h-0.0.4.dev4/setup.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.450923 ml4h-0.0.5/
+-rw-r--r--   0 sam        (503) staff       (20)     1633 2023-01-26 10:40:07.000000 ml4h-0.0.5/LICENSE.txt
+-rw-r--r--   0 sam        (503) staff       (20)     4491 2023-01-26 10:40:07.000000 ml4h-0.0.5/NOTICE.txt
+-rw-r--r--   0 sam        (503) staff       (20)     6857 2023-04-10 17:29:18.450007 ml4h-0.0.5/PKG-INFO
+-rw-r--r--   0 sam        (503) staff       (20)     6592 2023-03-08 12:42:24.000000 ml4h-0.0.5/README.md
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.360829 ml4h-0.0.5/ml4h/
+-rw-r--r--   0 sam        (503) staff       (20)     2361 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/DatabaseClient.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    23803 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/TensorMap.py
+-rw-r--r--   0 sam        (503) staff       (20)       22 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/__init__.py
+-rw-r--r--   0 sam        (503) staff       (20)    35435 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/arguments.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     9464 2023-03-08 12:42:24.000000 ml4h-0.0.5/ml4h/defines.py
+-rw-r--r--   0 sam        (503) staff       (20)    55869 2023-03-08 12:42:24.000000 ml4h-0.0.5/ml4h/explorations.py
+-rw-r--r--   0 sam        (503) staff       (20)     7604 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/hypertuning.py
+-rw-r--r--   0 sam        (503) staff       (20)     1846 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/logger.py
+-rw-r--r--   0 sam        (503) staff       (20)     6325 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/make_tensor_maps_for_partners_ecg_labels.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    27628 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/metrics.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.370658 ml4h-0.0.5/ml4h/ml4ht_integration/
+-rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/ml4ht_integration/__init__.py
+-rw-r--r--   0 sam        (503) staff       (20)     4264 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/ml4ht_integration/tensor_generator.py
+-rw-r--r--   0 sam        (503) staff       (20)     5358 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/ml4ht_integration/tensor_map.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.388059 ml4h-0.0.5/ml4h/models/
+-rw-r--r--   0 sam        (503) staff       (20)      422 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/Block.py
+-rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/__init__.py
+-rw-r--r--   0 sam        (503) staff       (20)     7921 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/basic_blocks.py
+-rw-r--r--   0 sam        (503) staff       (20)    23869 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/conv_blocks.py
+-rw-r--r--   0 sam        (503) staff       (20)     6020 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/inspect.py
+-rw-r--r--   0 sam        (503) staff       (20)     6368 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/layer_wrappers.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    67636 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/legacy_models.py
+-rw-r--r--   0 sam        (503) staff       (20)    13249 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/merge_blocks.py
+-rw-r--r--   0 sam        (503) staff       (20)    18364 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/model_factory.py
+-rw-r--r--   0 sam        (503) staff       (20)     3642 2023-03-08 12:42:24.000000 ml4h-0.0.5/ml4h/models/pretrained_blocks.py
+-rw-r--r--   0 sam        (503) staff       (20)     4144 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/train.py
+-rw-r--r--   0 sam        (503) staff       (20)    14384 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/transformer_blocks.py
+-rw-r--r--   0 sam        (503) staff       (20)     2848 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/normalizer.py
+-rw-r--r--   0 sam        (503) staff       (20)     4238 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/optimizers.py
+-rw-r--r--   0 sam        (503) staff       (20)   128766 2023-03-26 13:50:21.000000 ml4h-0.0.5/ml4h/plots.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    49510 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/recipes.py
+-rw-r--r--   0 sam        (503) staff       (20)     5424 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/runtime_data_defines.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    40052 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensor_generators.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.393913 ml4h-0.0.5/ml4h/tensorize/
+-rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensorize/__init__.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.395345 ml4h-0.0.5/ml4h/tensorize/dataflow/
+-rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensorize/dataflow/__init__.py
+-rw-r--r--   0 sam        (503) staff       (20)     7724 2023-03-08 12:42:24.000000 ml4h-0.0.5/ml4h/tensorize/dataflow/bigquery_ukb_queries.py
+-rw-r--r--   0 sam        (503) staff       (20)     4257 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensorize/merge_hd5s.py
+-rw-r--r--   0 sam        (503) staff       (20)    18759 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensorize/tensor_writer_mgb.py
+-rw-r--r--   0 sam        (503) staff       (20)    61752 2023-03-25 15:36:49.000000 ml4h-0.0.5/ml4h/tensorize/tensor_writer_ukbb.py
+-rw-r--r--   0 sam        (503) staff       (20)     3243 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensorize/tensorize_dataflow.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.402847 ml4h-0.0.5/ml4h/tensormap/
+-rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/__init__.py
+-rw-r--r--   0 sam        (503) staff       (20)     8657 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/celeba.py
+-rw-r--r--   0 sam        (503) staff       (20)     2152 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/gatk.py
+-rw-r--r--   0 sam        (503) staff       (20)     6283 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/general.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.406297 ml4h-0.0.5/ml4h/tensormap/mgb/
+-rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/mgb/__init__.py
+-rw-r--r--   0 sam        (503) staff       (20)    47783 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/mgb/dynamic.py
+-rw-r--r--   0 sam        (503) staff       (20)    73630 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/mgb/ecg.py
+-rw-r--r--   0 sam        (503) staff       (20)     4035 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/mnist.py
+-rw-r--r--   0 sam        (503) staff       (20)    14184 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/tensor_map_maker.py
+-rw-r--r--   0 sam        (503) staff       (20)     4154 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/text.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.437716 ml4h-0.0.5/ml4h/tensormap/ukb/
+-rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/ukb/__init__.py
+-rw-r--r--   0 sam        (503) staff       (20)   250867 2023-03-08 12:42:24.000000 ml4h-0.0.5/ml4h/tensormap/ukb/categorical.py
+-rw-r--r--   0 sam        (503) staff       (20)   542886 2023-03-08 12:42:24.000000 ml4h-0.0.5/ml4h/tensormap/ukb/continuous.py
+-rw-r--r--   0 sam        (503) staff       (20)    42508 2023-04-04 16:37:17.000000 ml4h-0.0.5/ml4h/tensormap/ukb/demographics.py
+-rw-r--r--   0 sam        (503) staff       (20)   101606 2023-04-10 14:42:05.000000 ml4h-0.0.5/ml4h/tensormap/ukb/disease.py
+-rw-r--r--   0 sam        (503) staff       (20)     4465 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/ukb/dxa.py
+-rw-r--r--   0 sam        (503) staff       (20)    61466 2023-03-26 15:24:00.000000 ml4h-0.0.5/ml4h/tensormap/ukb/ecg.py
+-rw-r--r--   0 sam        (503) staff       (20)    34805 2023-03-08 12:42:24.000000 ml4h-0.0.5/ml4h/tensormap/ukb/genetics.py
+-rw-r--r--   0 sam        (503) staff       (20)   126679 2023-04-06 19:41:39.000000 ml4h-0.0.5/ml4h/tensormap/ukb/mri.py
+-rw-r--r--   0 sam        (503) staff       (20)    12774 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/ukb/mri_brain.py
+-rw-r--r--   0 sam        (503) staff       (20)     6557 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/ukb/mri_ecg.py
+-rw-r--r--   0 sam        (503) staff       (20)    11925 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/ukb/mri_vtk.py
+-rw-r--r--   0 sam        (503) staff       (20)    14549 2023-03-20 19:08:05.000000 ml4h-0.0.5/ml4h/tensormap/ukb/survival.py
+-rw-r--r--   0 sam        (503) staff       (20)     3316 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/test_utils.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.448454 ml4h-0.0.5/ml4h/visualization_tools/
+-rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/__init__.py
+-rw-r--r--   0 sam        (503) staff       (20)     7219 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/annotation_storage.py
+-rw-r--r--   0 sam        (503) staff       (20)     5764 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/annotations.py
+-rw-r--r--   0 sam        (503) staff       (20)    10397 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/batch_image_annotations.py
+-rw-r--r--   0 sam        (503) staff       (20)    10420 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/dicom_interactive_plots.py
+-rw-r--r--   0 sam        (503) staff       (20)    15258 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/dicom_plots.py
+-rw-r--r--   0 sam        (503) staff       (20)     6203 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/ecg_interactive_plots.py
+-rw-r--r--   0 sam        (503) staff       (20)     9855 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/ecg_reshape.py
+-rw-r--r--   0 sam        (503) staff       (20)     3106 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/ecg_static_plots.py
+-rw-r--r--   0 sam        (503) staff       (20)     3329 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/facets.py
+-rw-r--r--   0 sam        (503) staff       (20)    14368 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/hd5_mri_plots.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.366153 ml4h-0.0.5/ml4h.egg-info/
+-rw-r--r--   0 sam        (503) staff       (20)     6857 2023-04-10 17:29:18.000000 ml4h-0.0.5/ml4h.egg-info/PKG-INFO
+-rw-r--r--   0 sam        (503) staff       (20)     2372 2023-04-10 17:29:18.000000 ml4h-0.0.5/ml4h.egg-info/SOURCES.txt
+-rw-r--r--   0 sam        (503) staff       (20)        1 2023-04-10 17:29:18.000000 ml4h-0.0.5/ml4h.egg-info/dependency_links.txt
+-rw-r--r--   0 sam        (503) staff       (20)      556 2023-04-10 17:29:18.000000 ml4h-0.0.5/ml4h.egg-info/requires.txt
+-rw-r--r--   0 sam        (503) staff       (20)        5 2023-04-10 17:29:18.000000 ml4h-0.0.5/ml4h.egg-info/top_level.txt
+-rw-r--r--   0 sam        (503) staff       (20)       38 2023-04-10 17:29:18.451157 ml4h-0.0.5/setup.cfg
+-rw-r--r--   0 sam        (503) staff       (20)      735 2023-04-10 16:51:22.000000 ml4h-0.0.5/setup.py
```

### Comparing `ml4h-0.0.4.dev4/LICENSE.txt` & `ml4h-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/NOTICE.txt` & `ml4h-0.0.5/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/README.md` & `ml4h-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/DatabaseClient.py` & `ml4h-0.0.5/ml4h/DatabaseClient.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/TensorMap.py` & `ml4h-0.0.5/ml4h/TensorMap.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/arguments.py` & `ml4h-0.0.5/ml4h/arguments.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/defines.py` & `ml4h-0.0.5/ml4h/defines.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 MRI_ANNOTATION_CHANNEL_MAP = {'good': 0, 'included-lvot': 1, 'mistrace': 2, 'phantom-apex': 3, 'hardclip': 4}
 MRI_LAX_2CH_SEGMENTED_CHANNEL_MAP = {
     'background': 0, 'aortic_arch': 1, 'left_pulmonary_artery_wall': 2, 'left_pulmonary_artery': 3,
     'LA_appendage': 4, 'LA_free_wall': 5, 'LV_posterior_wall': 6, 'LV_anterior_wall': 7, 'posterior_papillary': 8,
     'anterior_papillary': 9, 'LV_cavity': 10, 'LA_cavity': 11, 'body': 12,
 }
 LAX_2CH_HEART_LABELS = {
-    'aortic_arch': 1, 'left_pulmonary_artery_wall': 2, 'left_pulmonary_artery': 3,
     'LA_appendage': 4, 'LA_free_wall': 5, 'LV_posterior_wall': 6, 'LV_anterior_wall': 7, 'posterior_papillary': 8,
     'anterior_papillary': 9, 'LV_cavity': 10, 'LA_cavity': 11,
 }
 MRI_LAX_3CH_SEGMENTED_CHANNEL_MAP = {'background': 0, 'LV_anteroseptum': 1, 'left_atrium': 2, 'LV_inferior_wall': 3, 'LV_Papillary': 4, 'LV_Cavity': 5}
 LAX_3CH_HEART_LABELS = {'LV_anteroseptum': 1, 'left_atrium': 2, 'LV_inferior_wall': 3, 'LV_Papillary': 4, 'LV_Cavity': 5}
 MRI_LAX_4CH_SEGMENTED_CHANNEL_MAP = {
     'background': 0, 'RV_free_wall': 1, 'RA_free_wall': 2, 'LA_free_wall': 3, 'LV_anterolateral_wall': 4,
@@ -84,18 +83,17 @@
     'left_atrium': 13, 'right_atrium': 14, 'aorta': 15, 'pulmonary_artery': 16,
 }
 MRI_SAX_SEGMENTED_CHANNEL_MAP = {
     'background': 0, 'RV_free_wall': 1, 'interventricular_septum': 2, 'LV_free_wall': 3, 'LV_cavity': 4,
     'RV_cavity': 5, 'thoracic_cavity': 6, 'liver': 7, 'stomach': 8, 'spleen': 9, 'kidney': 11, 'body': 10,
     'left_atrium': 12, 'right_atrium': 13, 'aorta': 14, 'pulmonary_artery': 15,
 }
-MRI_SAX_SEGMENTED_CHANNEL_MAP = {
-    'background': 0, 'RV_free_wall': 1, 'interventricular_septum': 2, 'LV_free_wall': 3, 'LV_cavity': 4,
-    'RV_cavity': 5, 'thoracic_cavity': 6, 'liver': 7, 'stomach': 8, 'spleen': 9, 'kidney': 11, 'body': 10,
-    'left_atrium': 12, 'right_atrium': 13, 'aorta': 14, 'pulmonary_artery': 15,
+SAX_HEART_LABELS = {
+    'RV_free_wall': 1, 'interventricular_septum': 2, 'LV_free_wall': 3, 'LV_cavity': 4,
+    'RV_cavity': 5, 'left_atrium': 12, 'right_atrium': 13,
 }
 MRI_AO_SEGMENTED_CHANNEL_MAP = {
     'ao_background': 0, 'ao_superior_vena_cava': 1, 'ao_pulmonary_artery': 2, 'ao_ascending_aortic_wall': 3, 'ao_ascending_aorta': 4,
     'ao_descending_aortic_wall': 5, 'ao_descending_aorta': 6, 'ao_thorax': 7, 'ao_body': 8, 'ao_breast_implant': 9,
 }
 MRI_LVOT_SEGMENTED_CHANNEL_MAP = {
     'background': 0, 'body': 1, 'lungs': 2, 'RV_wall': 3, 'RV_cavity': 4, 'LV_wall': 5, 'LV_cavity': 6,
```

### Comparing `ml4h-0.0.4.dev4/ml4h/explorations.py` & `ml4h-0.0.5/ml4h/explorations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1041,15 +1041,21 @@
                 figure_path = os.path.join(args.output_folder, args.id, f"{name}_histogram{IMAGE_EXT}")
                 plt.savefig(figure_path)
                 logging.info(f"Saved {name} histogram plot at: {figure_path}")
 
 
 def latent_space_dataframe(infer_hidden_tsv, explore_csv):
     df = pd.read_csv(explore_csv)
-    df['sample_id'] = pd.to_numeric(df['sample_id'], errors='coerce')
+    if 'sample_id' in df.columns:
+        id_col = 'sample_id'
+    elif 'fpath' in df.columns:
+        id_col = 'fpath'
+    else:
+        raise ValueError(f'Could not find a sample ID column in explore CSV:{explore_csv}')
+    df['sample_id'] = pd.to_numeric(df[id_col], errors='coerce')
     df2 = pd.read_csv(infer_hidden_tsv, sep='\t', engine='python')
     df2['sample_id'] = pd.to_numeric(df2['sample_id'], errors='coerce')
     latent_df = pd.merge(df, df2, on='sample_id', how='inner')
     return latent_df
 
 
 def plot_scree(pca_components, percent_explained, figure_path):
```

### Comparing `ml4h-0.0.4.dev4/ml4h/hypertuning.py` & `ml4h-0.0.5/ml4h/hypertuning.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/logger.py` & `ml4h-0.0.5/ml4h/logger.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/make_tensor_maps_for_partners_ecg_labels.py` & `ml4h-0.0.5/ml4h/make_tensor_maps_for_partners_ecg_labels.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/metrics.py` & `ml4h-0.0.5/ml4h/metrics.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/ml4ht_integration/tensor_generator.py` & `ml4h-0.0.5/ml4h/ml4ht_integration/tensor_generator.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/ml4ht_integration/tensor_map.py` & `ml4h-0.0.5/ml4h/ml4ht_integration/tensor_map.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/models/basic_blocks.py` & `ml4h-0.0.5/ml4h/models/basic_blocks.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/models/conv_blocks.py` & `ml4h-0.0.5/ml4h/models/conv_blocks.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/models/inspect.py` & `ml4h-0.0.5/ml4h/models/inspect.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/models/layer_wrappers.py` & `ml4h-0.0.5/ml4h/models/layer_wrappers.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/models/legacy_models.py` & `ml4h-0.0.5/ml4h/models/legacy_models.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/models/merge_blocks.py` & `ml4h-0.0.5/ml4h/models/merge_blocks.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/models/model_factory.py` & `ml4h-0.0.5/ml4h/models/model_factory.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/models/pretrained_blocks.py` & `ml4h-0.0.5/ml4h/models/pretrained_blocks.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/models/train.py` & `ml4h-0.0.5/ml4h/models/train.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/models/transformer_blocks.py` & `ml4h-0.0.5/ml4h/models/transformer_blocks.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/normalizer.py` & `ml4h-0.0.5/ml4h/normalizer.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/optimizers.py` & `ml4h-0.0.5/ml4h/optimizers.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/plots.py` & `ml4h-0.0.5/ml4h/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -1028,14 +1028,17 @@
 
     :param events: Array indicating if each sample had an event (1) or not (0) by the end of follow up
     :param days_follow_up: Array with the total days of follow up for each sample
     :param predictions: Array with model predictions of an event before the end of follow up.
     :param title: Title for the plot
     :param prefix: Path prefix where plot will be saved
     :param days_window: Maximum days of follow up
+    :param dpi: Dots per inch of the figure
+    :param width: Width in inches of the figure
+    :param height: Height in inches of the figure
     """
     plt.figure(figsize=(width, height), dpi=dpi)
     days_sorted_index = np.argsort(days_follow_up)
     days_sorted = days_follow_up[days_sorted_index]
     alive_per_step = len(events)
 
     sick_per_step = 0
@@ -1096,24 +1099,27 @@
     """Plot Kaplan-Meier survivorship and predicted proportion surviving, calculate and return C-Index
 
     :param prediction: Array with model predictions of an event at each time step, with shape (num_samples, intervals*2).
     :param truth: Array with survival at each time step followed by events, shape is (num_samples, intervals*2)
     :param title: Title for the plot
     :param days_window: Maximum days of follow up
     :param prefix: Path prefix where plot will be saved
+    :param dpi: Dots per inch of the figure
+    :param width: Width in inches of the figure
+    :param height: Height in inches of the figure
 
     :return: Dictionary mapping metric names to their floating point values
     """
     c_index, concordant, discordant, tied_risk, tied_time = concordance_index(prediction, truth)
 
     intervals = truth.shape[-1] // 2
     plt.figure(figsize=(width, height), dpi=dpi)
 
     cumulative_sick = np.cumsum(np.sum(truth[:, intervals:], axis=0))
-    cumulative_censored = (truth.shape[0]-np.sum(truth[:, :intervals], axis=0))-cumulative_sick
+    cumulative_censored = (truth.shape[0]-np.sum(truth[:, :intervals], axis=0)) - cumulative_sick
     alive_per_step = np.sum(truth[:, :intervals], axis=0)
     sick_per_step = np.sum(truth[:, intervals:], axis=0)
     survivorship = np.cumprod(1 - (sick_per_step / alive_per_step))
     predicted_proportion = np.sum(np.cumprod(prediction[:, :intervals], axis=1), axis=0) / truth.shape[0]
 
     plt.plot(range(0, days_window, 1 + days_window // intervals), predicted_proportion, marker='o', label=f'Predicted Proportion C-Index:{c_index:0.3f}')
     plt.plot(range(0, days_window, 1 + days_window // intervals), survivorship, marker='o', label='Survivorship')
```

### Comparing `ml4h-0.0.4.dev4/ml4h/recipes.py` & `ml4h-0.0.5/ml4h/recipes.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/runtime_data_defines.py` & `ml4h-0.0.5/ml4h/runtime_data_defines.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/tensor_generators.py` & `ml4h-0.0.5/ml4h/tensor_generators.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/tensorize/dataflow/bigquery_ukb_queries.py` & `ml4h-0.0.5/ml4h/tensorize/dataflow/bigquery_ukb_queries.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/tensorize/merge_hd5s.py` & `ml4h-0.0.5/ml4h/tensorize/merge_hd5s.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/tensorize/tensor_writer_mgb.py` & `ml4h-0.0.5/ml4h/tensorize/tensor_writer_mgb.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/tensorize/tensor_writer_ukbb.py` & `ml4h-0.0.5/ml4h/tensorize/tensor_writer_ukbb.py`

 * *Files 2% similar despite different names*

```diff
@@ -782,19 +782,17 @@
     return datetime.datetime.strptime(date, DATE_FORMAT)
 
 
 def _write_ecg_bike_tensors(ecgs, xml_field, hd5, sample_id, stats):
     for ecg in ecgs:
         root = et.parse(ecg).getroot()
         date = datetime.datetime.strptime(_date_str_from_ecg(root), '%Y-%m-%d')
-        write_to_hd5 = partial(create_tensor_in_hd5, hd5=hd5, path_prefix='ukb_ecg_bike', stats=stats, date=date)
-        logging.info('Got ECG for sample:{} XML field:{}'.format(sample_id, xml_field))
-
         instance = ecg.split(JOIN_CHAR)[-2]
-        write_to_hd5(storage_type=StorageType.STRING, name='instance', value=instance)
+        write_to_hd5 = partial(create_tensor_in_hd5, hd5=hd5, path_prefix='ukb_ecg_bike', instance=instance, stats=stats, date=date)
+        logging.info(f'Got ECG for sample:{sample_id} XML field:{xml_field}')
 
         protocol = root.findall('./Protocol/Phase')[0].find('ProtocolName').text
         write_to_hd5(storage_type=StorageType.STRING, name='protocol', value=protocol)
 
         median_ecgs = defaultdict(list)
         for median_waves in root.findall('./MedianData/Median/WaveformData'):
             median_ecgs[median_waves.attrib['lead']].extend(list(map(float, median_waves.text.strip().split(','))))
@@ -877,18 +875,21 @@
                 field_val = lead.find(lead_field)
                 if field_val is None:
                     continue
                 field_val = _to_float_or_false(field_val.text.strip('?'))
                 if field_val is False:
                     continue
                 trends[lead_field][i, lead_to_int[lead_num]] = field_val
-            trends['time'][i] = SECONDS_PER_MINUTE * int(trend_entry.find("EntryTime/Minute").text) + int(trend_entry.find("EntryTime/Second").text)
-            trends['PhaseTime'][i] = SECONDS_PER_MINUTE * int(trend_entry.find("PhaseTime/Minute").text) + int(trend_entry.find("PhaseTime/Second").text)
-            trends['PhaseName'][i] = phase_to_int[trend_entry.find('PhaseName').text]
-            trends['Artifact'][i] = float(trend_entry.find('Artifact').text.strip('%')) / 100  # Artifact is reported as a percentage
+            try:
+                trends['time'][i] = SECONDS_PER_MINUTE * int(trend_entry.find("EntryTime/Minute").text) + int(trend_entry.find("EntryTime/Second").text)
+                trends['PhaseTime'][i] = SECONDS_PER_MINUTE * int(trend_entry.find("PhaseTime/Minute").text) + int(trend_entry.find("PhaseTime/Second").text)
+                trends['PhaseName'][i] = phase_to_int[trend_entry.find('PhaseName').text]
+                trends['Artifact'][i] = float(trend_entry.find('Artifact').text.strip('%')) / 100  # Artifact is reported as a percentage
+            except AttributeError as e:
+                stats['AttributeError on Trend Data'] += 1
 
         for field, trend_list in trends.items():
             write_to_hd5(name=f'trend_{str.lower(field)}', value=trend_list)
 
         # Last 60 seconds of raw given that the rest phase is 60s
         phase_durations = {}
         for protocol in root.findall("./Protocol/Phase"):
@@ -896,20 +897,23 @@
             phase_duration = SECONDS_PER_MINUTE * int(protocol.find("PhaseDuration/Minute").text) + int(
                 protocol.find("PhaseDuration/Second").text,
             )
             phase_durations[phase_name] = phase_duration
             write_to_hd5(name=f'{str.lower(phase_name)}_duration', value=[phase_duration])
 
         # HR stats
-        max_hr = _xml_path_to_float(root, './ExerciseMeasurements/MaxHeartRate')
-        resting_hr = _xml_path_to_float(root, './ExerciseMeasurements/RestingStats/RestHR')
-        max_pred_hr = _xml_path_to_float(root, './ExerciseMeasurements/MaxPredictedHR')
-        write_to_hd5(name='max_hr', value=[max_hr])
-        write_to_hd5(name='resting_hr', value=[resting_hr])
-        write_to_hd5(name='max_pred_hr', value=[max_pred_hr])
+        try:
+            max_hr = _xml_path_to_float(root, './ExerciseMeasurements/MaxHeartRate')
+            write_to_hd5(name='max_hr', value=[max_hr])
+            resting_hr = _xml_path_to_float(root, './ExerciseMeasurements/RestingStats/RestHR')
+            write_to_hd5(name='resting_hr', value=[resting_hr])
+            max_pred_hr = _xml_path_to_float(root, './ExerciseMeasurements/MaxPredictedHR')
+            write_to_hd5(name='max_pred_hr', value=[max_pred_hr])
+        except AttributeError as e:
+            stats['AttributeError on HR Stats'] += 1
 
 
 def _write_tensors_from_niftis(folder: str, hd5: h5py.File, field_id: str, stats: Counter):
     niftis = glob.glob(os.path.join(folder, MRI_NIFTI_FIELD_ID_TO_ROOT[field_id], '**/*nii.gz'), recursive=True)
     logging.info(f'Found {len(niftis)} NIFTI files at {os.path.join(folder, MRI_NIFTI_FIELD_ID_TO_ROOT[field_id])} ')
     for nifti in niftis:  # iterate through all nii.gz files and add them to the hd5
         nifti_mri = nib.load(nifti)
```

### Comparing `ml4h-0.0.4.dev4/ml4h/tensorize/tensorize_dataflow.py` & `ml4h-0.0.5/ml4h/tensorize/tensorize_dataflow.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/tensormap/celeba.py` & `ml4h-0.0.5/ml4h/tensormap/celeba.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/tensormap/gatk.py` & `ml4h-0.0.5/ml4h/tensormap/gatk.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/tensormap/general.py` & `ml4h-0.0.5/ml4h/tensormap/general.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/tensormap/mgb/dynamic.py` & `ml4h-0.0.5/ml4h/tensormap/mgb/dynamic.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/tensormap/mgb/ecg.py` & `ml4h-0.0.5/ml4h/tensormap/mgb/ecg.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/tensormap/mnist.py` & `ml4h-0.0.5/ml4h/tensormap/mnist.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/tensormap/tensor_map_maker.py` & `ml4h-0.0.5/ml4h/tensormap/tensor_map_maker.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/tensormap/text.py` & `ml4h-0.0.5/ml4h/tensormap/text.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/tensormap/ukb/demographics.py` & `ml4h-0.0.5/ml4h/tensormap/ukb/demographics.py`

 * *Files 2% similar despite different names*

```diff
@@ -500,14 +500,35 @@
 )
 diastolic_blood_pressure_2 = TensorMap(
     '4079_Diastolic-blood-pressure-automated-reading_2_0', Interpretation.CONTINUOUS, path_prefix='continuous', loss='logcosh',
     channel_map={'4079_Diastolic-blood-pressure-automated-reading_2_0': 0}, validator=make_range_validator(20, 300),
     normalization={'mean': 82.20657551284782, 'std': 10.496040770224475},
 )
 
+hypertension = TensorMap(
+    'hypertension_diagnosis', Interpretation.CATEGORICAL,
+    storage_type=StorageType.CATEGORICAL_FLAG, path_prefix='categorical',
+    loss='categorical_crossentropy',
+    channel_map={'no_hypertension': 0, 'hypertension': 1},
+)
+hypertension_med = TensorMap(
+    'start_fu_hypertension_med', Interpretation.CATEGORICAL, loss='categorical_crossentropy',
+    storage_type=StorageType.CATEGORICAL_FLAG, path_prefix='categorical',
+    channel_map={'no_start_fu_hypertension_med':0, 'start_fu_hypertension_med': 1},
+)
+peak_vo2 = TensorMap(
+    'peak_vo2', Interpretation.CONTINUOUS,
+    storage_type=StorageType.CATEGORICAL_INDEX, path_prefix='continuous',
+    channel_map={'peak_vo2':0},
+)
+cad = TensorMap(
+    'cad', Interpretation.CATEGORICAL, loss='categorical_crossentropy',
+    storage_type=StorageType.CATEGORICAL_INDEX, path_prefix='categorical',
+    channel_map={'no_coronary_artery_disease':0, 'coronary_artery_disease': 1},
+)
 
 categorical_phenotypes_25 = TensorMap(
     'categorical-phenotypes-25', Interpretation.CATEGORICAL, path_prefix='categorical',
     channel_map={
         'Adopted-as-a-child_No_0_0': 0,
         'Beef-intake_Less-than-once-a-week_0_0': 1,
         'Breastfed-as-a-baby_Yes_0_0': 2,
```

### Comparing `ml4h-0.0.4.dev4/ml4h/tensormap/ukb/dxa.py` & `ml4h-0.0.5/ml4h/tensormap/ukb/dxa.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/tensormap/ukb/ecg.py` & `ml4h-0.0.5/ml4h/tensormap/ukb/ecg.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 import numpy as np
 import scipy
 import logging
 
 import biosppy
 from typing import List, Tuple, Dict
 from tensorflow.keras.utils import to_categorical
-# from ml4h.tensor_writer_ukbb import tensor_path
+
+from ml4h.tensormap.ukb.demographics import age_in_years_tensor
 from ml4h.normalizer import ZeroMeanStd1, Standardize, RandomStandardize
-from ml4h.tensormap.general import tensor_path, pad_or_crop_array_to_shape, tensor_from_hd5, named_tensor_from_hd5
+from ml4h.metrics import weighted_crossentropy, ignore_zeros_logcosh, mse_10x
 from ml4h.TensorMap import TensorMap, Interpretation, no_nans, make_range_validator
-from ml4h.defines import ECG_REST_LEADS, ECG_REST_MEDIAN_LEADS, ECG_REST_AMP_LEADS, ECG_SEGMENTED_CHANNEL_MAP, ECG_CHAR_2_IDX, ECG_REST_MGB_LEADS, ECG_REST_AMP_LEADS_UKB
+from ml4h.defines import ECG_CHAR_2_IDX, ECG_REST_MGB_LEADS, ECG_REST_AMP_LEADS_UKB, ECG_BIKE_LEADS
+from ml4h.defines import ECG_REST_LEADS, ECG_REST_MEDIAN_LEADS, ECG_REST_AMP_LEADS, ECG_SEGMENTED_CHANNEL_MAP
+from ml4h.tensormap.general import tensor_path, pad_or_crop_array_to_shape, tensor_from_hd5, named_tensor_from_hd5
 from ml4h.tensormap.general import get_tensor_at_first_date, normalized_first_date, pass_nan, build_tensor_from_file
-from ml4h.metrics import weighted_crossentropy, ignore_zeros_logcosh, mse_10x
-from ml4h.tensormap.ukb.demographics import age_in_years_tensor
 
 _HRR_SENTINEL = -1000
 
 
 # BIKE ECG
 def _check_phase_full_len(hd5: h5py.File, phase: str):
     phase_len = get_tensor_at_first_date(hd5, 'ecg_bike', f'{phase}_duration')
@@ -197,15 +198,15 @@
     categorical_data = np.zeros(tm.shape, dtype=np.float32)
     ecg_interpretation = str(
         tm.hd5_first_dataset_in_group(
         hd5, 'ukb_ecg_rest/ecg_rest_text/',
         )[()],
     )
     for channel in tm.channel_map:
-        if channel in ecg_interpretation:
+        if channel.lower() in ecg_interpretation.lower():
             categorical_data[tm.channel_map[channel]] = 1.0
             return categorical_data
     if 'no_' + tm.name in tm.channel_map:
         categorical_data[tm.channel_map['no_' + tm.name]] = 1.0
         return categorical_data
     else:
         raise ValueError(
@@ -953,28 +954,32 @@
 
 
 ecg_semi_coarse_with_poor = TensorMap(
     'ecg_semi_coarse_with_poor', Interpretation.CATEGORICAL, loss=weighted_crossentropy([1.0, 2.0, 3.0, 3.0, 20.0, 20.0], 'ecg_semi_coarse_with_poor'),
     channel_map={'Normal_sinus_rhythm': 0, 'Sinus_bradycardia': 1, 'Marked_sinus_bradycardia': 2, 'Other_sinus_rhythm': 3, 'Atrial_fibrillation': 4, 'Other_rhythm': 5},
 )
 
-ecg_normal = TensorMap(
-    'ecg_normal', Interpretation.CATEGORICAL, loss=weighted_crossentropy([2.0, 3.0, 3.0, 3.0], 'ecg_normal'),
-    channel_map={'Normal_ECG': 0, 'Abnormal_ECG': 1, 'Borderline_ECG': 2, 'Otherwise_normal_ECG': 3},
-)
-ecg_infarct = TensorMap(
-    'ecg_infarct', Interpretation.CATEGORICAL, channel_map={'no_infarct': 0, 'infarct': 1},
+normal = TensorMap(
+    'normal', Interpretation.CATEGORICAL, loss=weighted_crossentropy([2.0, 3.0, 3.0, 3.0], 'ecg_normal'),
+    tensor_from_file=label_from_ecg_interpretation_text,
+    channel_map={'Normal ECG': 0, 'Abnormal ECG': 1, 'Borderline ECG': 2, 'Otherwise normal ECG': 3},
+)
+infarct = TensorMap(
+    'infarct', Interpretation.CATEGORICAL, channel_map={'no_infarct': 0, 'infarct': 1},
+    tensor_from_file=label_from_ecg_interpretation_text,
     loss=weighted_crossentropy([1.0, 8.0], 'ecg_infarct'),
 )
 ecg_poor_data = TensorMap(
     'ecg_poor_data', Interpretation.CATEGORICAL, channel_map={'no_poor_data_quality': 0, 'poor_data_quality': 1},
+    tensor_from_file=label_from_ecg_interpretation_text,
     loss=weighted_crossentropy([1.0, 8.0], 'ecg_poor_data'),
 )
-ecg_block = TensorMap(
-    'ecg_block', Interpretation.CATEGORICAL, channel_map={'no_block': 0, 'block': 1},
+block = TensorMap(
+    'block', Interpretation.CATEGORICAL, channel_map={'no_block': 0, 'block': 1},
+    tensor_from_file=label_from_ecg_interpretation_text,
     loss=weighted_crossentropy([1.0, 8.0], 'ecg_block'),
 )
 
 ecg_rest_next_char = TensorMap('ecg_rest_next_char', Interpretation.LANGUAGE, shape=(len(ECG_CHAR_2_IDX),), channel_map=ECG_CHAR_2_IDX, activation='softmax', loss='categorical_crossentropy', loss_weight=2.0)
 ecg_rest_text = TensorMap('ecg_rest_text', Interpretation.LANGUAGE, shape=(100, len(ECG_CHAR_2_IDX)), path_prefix='ukb_ecg_rest', channel_map={'context': 0, 'alphabet': 1}, dependent_map=ecg_rest_next_char)
 
 p_axis = TensorMap(
@@ -1187,47 +1192,14 @@
     'bike_resting_hr', Interpretation.CONTINUOUS, channel_map={'bike_resting_hr': 0},
     loss=ignore_zeros_logcosh, metrics=['logcosh'], normalization={'mean': 71.2, 'std': 12.57},
 )
 ecg_bike_max_pred_hr_no0 = TensorMap(
     'bike_max_pred_hr', Interpretation.CONTINUOUS, channel_map={'bike_max_pred_hr': 0},
     loss=ignore_zeros_logcosh, metrics=['logcosh'], normalization={'mean': 167.5, 'std': 5.78},
 )
-
-ecg_bike_max_hr = TensorMap(
-    'max_hr', path_prefix='ecg_bike', loss='logcosh', metrics=['mape'],
-    normalization={'mean': 110.03, 'std': 20.04}, shape=(1,),
-    tensor_from_file=normalized_first_date,
-)
-ecg_bike_resting_hr = TensorMap(
-    'resting_hr', Interpretation.CONTINUOUS, path_prefix='ecg_bike', loss='logcosh', shape=(1,),
-    metrics=['mape'], normalization={'mean': 71.2, 'std': 12.57},
-    tensor_from_file=normalized_first_date,
-)
-ecg_bike_age = TensorMap(
-    'age', Interpretation.CONTINUOUS, path_prefix='ecg_bike', loss='logcosh', metrics=['mape'], shape=(1,),
-    normalization={'mean': 60, 'std': 7.65},
-    tensor_from_file=normalized_first_date,
-)
-ecg_bike_max_pred_hr = TensorMap(
-    'max_pred_hr', Interpretation.CONTINUOUS, path_prefix='ecg_bike', loss='logcosh', metrics=['mape'], shape=(1,),
-    normalization={'mean': 167.5, 'std': 5.81},
-    tensor_from_file=normalized_first_date,
-)
-ecg_bike_trend_hr = TensorMap(
-    'trend_heartrate', Interpretation.CONTINUOUS, shape=(106, 1), path_prefix='ecg_bike',
-    tensor_from_file=normalized_first_date,
-)
-ecg_bike_trend_load = TensorMap(
-    'trend_load', Interpretation.CONTINUOUS, shape=(106, 1), path_prefix='ecg_bike',
-    tensor_from_file=normalized_first_date,
-)
-ecg_bike_trend_grade = TensorMap(
-    'trend_grade', Interpretation.CONTINUOUS, shape=(106, 1), path_prefix='ecg_bike',
-    tensor_from_file=normalized_first_date,
-)
 ecg_bike_raw_trend_hr = TensorMap(
     'trend_heartrate', Interpretation.CONTINUOUS, shape=(87,), path_prefix='ukb_ecg_bike',
     tensor_from_file=normalized_first_date,
 )
 ecg_bike_raw_trend_load = TensorMap(
     'trend_load', Interpretation.CONTINUOUS, shape=(87,), path_prefix='ukb_ecg_bike',
     tensor_from_file=normalized_first_date,
@@ -1264,15 +1236,22 @@
     'trend_vecount', Interpretation.CONTINUOUS, shape=(87,), path_prefix='ukb_ecg_bike',
     tensor_from_file=normalized_first_date,
 )
 ecg_bike_raw_full = TensorMap(
     'full', Interpretation.CONTINUOUS, shape=(216500, 3), path_prefix='ukb_ecg_bike',
     tensor_from_file=normalized_first_date,
 )
-
+ecg_bike_median = TensorMap(
+    'median', Interpretation.CONTINUOUS, shape=(5500, 3), path_prefix='ukb_ecg_bike',
+    tensor_from_file=normalized_first_date, normalization=ZeroMeanStd1(), channel_map=ECG_BIKE_LEADS,
+)
+ecg_bike_strip = TensorMap(
+    'strip', Interpretation.CONTINUOUS, shape=(5000, 3), path_prefix='ukb_ecg_bike',
+    tensor_from_file=normalized_first_date,
+)
 
 def ppg_from_hd5(tm: TensorMap, hd5: h5py.File, dependents: Dict = {}) -> np.ndarray:
     ppg = np.zeros(tm.shape,  dtype=np.float32)
     ppg[:, 0] = hd5[tm.name]
     return ppg
 
 ppg_0 = TensorMap(
```

### Comparing `ml4h-0.0.4.dev4/ml4h/tensormap/ukb/genetics.py` & `ml4h-0.0.5/ml4h/tensormap/ukb/genetics.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,171 @@
 from tensorflow.keras.losses import mean_squared_error
 
 from ml4h.TensorMap import TensorMap, Interpretation
 from ml4h.defines import StorageType
 from ml4h.metrics import weighted_crossentropy, abs_pearson, pearson
 
-
 diploid_cm = {'homozygous_reference': 0, 'heterozygous': 1, 'homozygous_variant': 2}
 rs3829740 = TensorMap('rs3829740', Interpretation.CATEGORICAL, channel_map=diploid_cm)
 rs2234962 = TensorMap('rs2234962', Interpretation.CATEGORICAL, channel_map=diploid_cm)
 rs2042995 = TensorMap('rs2042995', Interpretation.CATEGORICAL, channel_map=diploid_cm)
 
-rs3829740_weighted = TensorMap('rs3829740', Interpretation.CATEGORICAL, channel_map=diploid_cm, loss=weighted_crossentropy([1, 1, 1.5], 'rs3829740'))
-rs2234962_weighted = TensorMap('rs2234962', Interpretation.CATEGORICAL, channel_map=diploid_cm, loss=weighted_crossentropy([.8, 1, 1.5], 'rs2234962'))
-rs2042995_weighted = TensorMap('rs2042995', Interpretation.CATEGORICAL, channel_map=diploid_cm, loss=weighted_crossentropy([.6, 1.5, 2], 'rs2042995'))
+rs3829740_weighted = TensorMap(
+    'rs3829740', Interpretation.CATEGORICAL, channel_map=diploid_cm,
+    loss=weighted_crossentropy([1, 1, 1.5], 'rs3829740'),
+)
+rs2234962_weighted = TensorMap(
+    'rs2234962', Interpretation.CATEGORICAL, channel_map=diploid_cm,
+    loss=weighted_crossentropy([.8, 1, 1.5], 'rs2234962'),
+)
+rs2042995_weighted = TensorMap(
+    'rs2042995', Interpretation.CATEGORICAL, channel_map=diploid_cm,
+    loss=weighted_crossentropy([.6, 1.5, 2], 'rs2042995'),
+)
 
 # KCNJ5 = TensorMap('KCNJ5', Interpretation.CONTIG, channel_map={'position': 0, 'genotype': 1})
 # KCNH2 = TensorMap('KCNH2', Interpretation.CONTIG, channel_map={'position': 0, 'genotype': 1})
 # SCN5A = TensorMap('SCN5A', Interpretation.CONTIG, channel_map={'position': 0, 'genotype': 1})
 # TTN = TensorMap('TTN', Interpretation.CONTIG, channel_map={'position': 0, 'genotype': 1})
 
 akap9_lof = TensorMap('AKAP9', Interpretation.CATEGORICAL, channel_map={'no_akap9_lof': 0, 'akap9_lof': 1})
 dsc2_lof = TensorMap('DSC2', Interpretation.CATEGORICAL, channel_map={'no_dsc2_lof': 0, 'dsc2_lof': 1})
 ryr2_lof = TensorMap('RYR2', Interpretation.CATEGORICAL, channel_map={'no_ryr2_lof': 0, 'ryr2_lof': 1})
 ttn_lof = TensorMap('ttn_lof', Interpretation.CATEGORICAL, channel_map={'no_ttn_lof': 0, 'ttn_lof': 1})
 
-TTN_LOF = TensorMap('TTN', Interpretation.CATEGORICAL, path_prefix='categorical', storage_type=StorageType.CATEGORICAL_INDEX, channel_map={'no_TTN_LOF': 0, 'TTN_LOF': 1})
-LMNA_LOF = TensorMap('LMNA', Interpretation.CATEGORICAL, path_prefix='categorical', storage_type=StorageType.CATEGORICAL_INDEX, channel_map={'no_LMNA_LOF': 0, 'LMNA_LOF': 1})
-PKP2_LOF = TensorMap('PKP2', Interpretation.CATEGORICAL, path_prefix='categorical', storage_type=StorageType.CATEGORICAL_INDEX, channel_map={'no_PKP2_LOF': 0, 'PKP2_LOF': 1})
-SCN5A_LOF = TensorMap('SCN5A', Interpretation.CATEGORICAL, path_prefix='categorical', storage_type=StorageType.CATEGORICAL_INDEX, channel_map={'no_SCN5A_LOF': 0, 'SCN5A_LOF': 1})
-KCNQ1_LOF = TensorMap('KCNQ1', Interpretation.CATEGORICAL, path_prefix='categorical', storage_type=StorageType.CATEGORICAL_INDEX, channel_map={'no_KCNQ1_LOF': 0, 'KCNQ1_LOF': 1})
-KCNH2_LOF = TensorMap('KCNH2', Interpretation.CATEGORICAL, path_prefix='categorical', storage_type=StorageType.CATEGORICAL_INDEX, channel_map={'no_KCNH2_LOF': 0, 'KCNH2_LOF': 1})
-KCNJ5_LOF = TensorMap('KCNJ5', Interpretation.CATEGORICAL, path_prefix='categorical', storage_type=StorageType.CATEGORICAL_INDEX, channel_map={'no_KCNJ5_LOF': 0, 'KCNJ5_LOF': 1})
-MYBPC3_LOF = TensorMap('MYBPC3', Interpretation.CATEGORICAL, path_prefix='categorical', storage_type=StorageType.CATEGORICAL_INDEX, channel_map={'no_MYBPC3_LOF': 0, 'MYBPC3_LOF': 1})
+TTN_LOF = TensorMap(
+    'TTN', Interpretation.CATEGORICAL, path_prefix='categorical',
+    storage_type=StorageType.CATEGORICAL_INDEX, channel_map={'no_TTN_LOF': 0, 'TTN_LOF': 1},
+)
+LMNA_LOF = TensorMap(
+    'LMNA', Interpretation.CATEGORICAL, path_prefix='categorical',
+    storage_type=StorageType.CATEGORICAL_INDEX, channel_map={'no_LMNA_LOF': 0, 'LMNA_LOF': 1},
+)
+PKP2_LOF = TensorMap(
+    'PKP2', Interpretation.CATEGORICAL, path_prefix='categorical',
+    storage_type=StorageType.CATEGORICAL_INDEX, channel_map={'no_PKP2_LOF': 0, 'PKP2_LOF': 1},
+)
+SCN5A_LOF = TensorMap(
+    'SCN5A', Interpretation.CATEGORICAL, path_prefix='categorical',
+    storage_type=StorageType.CATEGORICAL_INDEX, channel_map={'no_SCN5A_LOF': 0, 'SCN5A_LOF': 1},
+)
+KCNQ1_LOF = TensorMap(
+    'KCNQ1', Interpretation.CATEGORICAL, path_prefix='categorical',
+    storage_type=StorageType.CATEGORICAL_INDEX, channel_map={'no_KCNQ1_LOF': 0, 'KCNQ1_LOF': 1},
+)
+KCNH2_LOF = TensorMap(
+    'KCNH2', Interpretation.CATEGORICAL, path_prefix='categorical',
+    storage_type=StorageType.CATEGORICAL_INDEX, channel_map={'no_KCNH2_LOF': 0, 'KCNH2_LOF': 1},
+)
+KCNJ5_LOF = TensorMap(
+    'KCNJ5', Interpretation.CATEGORICAL, path_prefix='categorical',
+    storage_type=StorageType.CATEGORICAL_INDEX, channel_map={'no_KCNJ5_LOF': 0, 'KCNJ5_LOF': 1},
+)
+MYBPC3_LOF = TensorMap(
+    'MYBPC3', Interpretation.CATEGORICAL, path_prefix='categorical',
+    storage_type=StorageType.CATEGORICAL_INDEX, channel_map={'no_MYBPC3_LOF': 0, 'MYBPC3_LOF': 1},
+)
 
 TTN_LOF_weighted = TensorMap(
     'TTN', Interpretation.CATEGORICAL, path_prefix='categorical', loss=weighted_crossentropy([0.2, 15.0]),
     storage_type=StorageType.CATEGORICAL_INDEX, channel_map={'no_TTN_LOF': 0, 'TTN_LOF': 1},
 )
 
 ttntv = TensorMap(
-    'has_ttntv',  Interpretation.CATEGORICAL, path_prefix='categorical', storage_type=StorageType.CATEGORICAL_INDEX,
+    'has_ttntv', Interpretation.CATEGORICAL, path_prefix='categorical', storage_type=StorageType.CATEGORICAL_INDEX,
     channel_map={'no_ttntv': 0, 'has_ttntv': 1},
 )
 
-bsa_mosteller = TensorMap('bsa_mosteller',  Interpretation.CONTINUOUS, normalization={'mean': 1.8894831981880114, 'std': 0.22169301057810176}, loss='logcosh', channel_map={'bsa_mosteller': 0})
-bsa_dubois = TensorMap('bsa_dubois',  Interpretation.CONTINUOUS, normalization={'mean': 1.8671809970639703, 'std': 0.20913930961120797}, loss='logcosh', channel_map={'bsa_dubois': 0})
+bsa_mosteller = TensorMap(
+    'bsa_mosteller', Interpretation.CONTINUOUS,
+    normalization={'mean': 1.8894831981880114, 'std': 0.22169301057810176}, loss='logcosh',
+    channel_map={'bsa_mosteller': 0},
+)
+bsa_dubois = TensorMap(
+    'bsa_dubois', Interpretation.CONTINUOUS,
+    normalization={'mean': 1.8671809970639703, 'std': 0.20913930961120797}, loss='logcosh',
+    channel_map={'bsa_dubois': 0},
+)
 
+ancestry_pca_40 = TensorMap(
+    'ancestry_pca_40', Interpretation.CONTINUOUS, shape=(40,), loss='logcosh', path_prefix='continuous',
+    channel_map={
+        '22009_Genetic-principal-components_0_1': 0, '22009_Genetic-principal-components_0_2': 1,
+        '22009_Genetic-principal-components_0_3': 2, '22009_Genetic-principal-components_0_4': 3,
+        '22009_Genetic-principal-components_0_5': 4, '22009_Genetic-principal-components_0_6': 5,
+        '22009_Genetic-principal-components_0_7': 6, '22009_Genetic-principal-components_0_8': 7,
+        '22009_Genetic-principal-components_0_9': 8, '22009_Genetic-principal-components_0_10': 9,
+        '22009_Genetic-principal-components_0_11': 10, '22009_Genetic-principal-components_0_12': 11,
+        '22009_Genetic-principal-components_0_13': 12, '22009_Genetic-principal-components_0_14': 13,
+        '22009_Genetic-principal-components_0_15': 14, '22009_Genetic-principal-components_0_16': 15,
+        '22009_Genetic-principal-components_0_17': 16, '22009_Genetic-principal-components_0_18': 17,
+        '22009_Genetic-principal-components_0_19': 18, '22009_Genetic-principal-components_0_20': 19,
+        '22009_Genetic-principal-components_0_21': 20, '22009_Genetic-principal-components_0_22': 21,
+        '22009_Genetic-principal-components_0_23': 22, '22009_Genetic-principal-components_0_24': 23,
+        '22009_Genetic-principal-components_0_25': 24, '22009_Genetic-principal-components_0_26': 25,
+        '22009_Genetic-principal-components_0_27': 26, '22009_Genetic-principal-components_0_28': 27,
+        '22009_Genetic-principal-components_0_29': 28, '22009_Genetic-principal-components_0_30': 29,
+        '22009_Genetic-principal-components_0_31': 30, '22009_Genetic-principal-components_0_32': 31,
+        '22009_Genetic-principal-components_0_33': 32, '22009_Genetic-principal-components_0_34': 33,
+        '22009_Genetic-principal-components_0_35': 34, '22009_Genetic-principal-components_0_36': 35,
+        '22009_Genetic-principal-components_0_37': 36, '22009_Genetic-principal-components_0_38': 37,
+        '22009_Genetic-principal-components_0_39': 38, '22009_Genetic-principal-components_0_40': 39,
+    },
+)
+
+ancestry_pca_43 = TensorMap(
+    'ancestry_pca_43', Interpretation.CONTINUOUS, shape=(43,), loss='logcosh', path_prefix='continuous',
+    channel_map={
+        '22005_Missingness_0_0': 0, '22004_Heterozygosity-PCA-corrected_0_0': 1, '22003_Heterozygosity_0_0': 2,
+        '22009_Genetic-principal-components_0_1': 3, '22009_Genetic-principal-components_0_2': 4,
+        '22009_Genetic-principal-components_0_3': 5, '22009_Genetic-principal-components_0_4': 6,
+        '22009_Genetic-principal-components_0_5': 7, '22009_Genetic-principal-components_0_6': 8,
+        '22009_Genetic-principal-components_0_7': 9, '22009_Genetic-principal-components_0_8': 10,
+        '22009_Genetic-principal-components_0_9': 11, '22009_Genetic-principal-components_0_10': 12,
+        '22009_Genetic-principal-components_0_11': 13, '22009_Genetic-principal-components_0_12': 14,
+        '22009_Genetic-principal-components_0_13': 15, '22009_Genetic-principal-components_0_14': 16,
+        '22009_Genetic-principal-components_0_15': 17, '22009_Genetic-principal-components_0_16': 18,
+        '22009_Genetic-principal-components_0_17': 19, '22009_Genetic-principal-components_0_18': 20,
+        '22009_Genetic-principal-components_0_19': 21, '22009_Genetic-principal-components_0_20': 22,
+        '22009_Genetic-principal-components_0_21': 23, '22009_Genetic-principal-components_0_22': 24,
+        '22009_Genetic-principal-components_0_23': 25, '22009_Genetic-principal-components_0_24': 26,
+        '22009_Genetic-principal-components_0_25': 27, '22009_Genetic-principal-components_0_26': 28,
+        '22009_Genetic-principal-components_0_27': 29, '22009_Genetic-principal-components_0_28': 30,
+        '22009_Genetic-principal-components_0_29': 31, '22009_Genetic-principal-components_0_30': 32,
+        '22009_Genetic-principal-components_0_31': 33, '22009_Genetic-principal-components_0_32': 34,
+        '22009_Genetic-principal-components_0_33': 35, '22009_Genetic-principal-components_0_34': 36,
+        '22009_Genetic-principal-components_0_35': 37, '22009_Genetic-principal-components_0_36': 38,
+        '22009_Genetic-principal-components_0_37': 39, '22009_Genetic-principal-components_0_38': 40,
+        '22009_Genetic-principal-components_0_39': 41, '22009_Genetic-principal-components_0_40': 42,
+    },
+)
 
 genetic_pca_1 = TensorMap(
-    '22009_Genetic-principal-components_0_1', Interpretation.CONTINUOUS, path_prefix='continuous', normalization={'mean': -0.014422761536727896, 'std': 10.57799283718005},
+    '22009_Genetic-principal-components_0_1', Interpretation.CONTINUOUS, path_prefix='continuous',
+    normalization={'mean': -0.014422761536727896, 'std': 10.57799283718005},
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_1': 0},
 )
 genetic_pca_2 = TensorMap(
-    '22009_Genetic-principal-components_0_2', Interpretation.CONTINUOUS, path_prefix='continuous', #normalization={'mean': -0.014422761536727896, 'std': 10.57799283718005},
+    '22009_Genetic-principal-components_0_2', Interpretation.CONTINUOUS, path_prefix='continuous',
+    # normalization={'mean': -0.014422761536727896, 'std': 10.57799283718005},
     loss='logcosh', activation='linear', channel_map={'22009_Genetic-principal-components_0_2': 0},
 )
 genetic_pca_3 = TensorMap(
-    '22009_Genetic-principal-components_0_3', Interpretation.CONTINUOUS, path_prefix='continuous', #normalization={'mean': -0.014422761536727896, 'std': 10.57799283718005},
+    '22009_Genetic-principal-components_0_3', Interpretation.CONTINUOUS, path_prefix='continuous',
+    # normalization={'mean': -0.014422761536727896, 'std': 10.57799283718005},
     loss='logcosh', activation='linear', channel_map={'22009_Genetic-principal-components_0_3': 0},
 )
 genetic_pca_4 = TensorMap(
-    '22009_Genetic-principal-components_0_4', Interpretation.CONTINUOUS, path_prefix='continuous', #normalization={'mean': -0.014422761536727896, 'std': 10.57799283718005},
+    '22009_Genetic-principal-components_0_4', Interpretation.CONTINUOUS, path_prefix='continuous',
+    # normalization={'mean': -0.014422761536727896, 'std': 10.57799283718005},
     loss='logcosh', activation='linear', channel_map={'22009_Genetic-principal-components_0_4': 0},
 )
 genetic_pca_5 = TensorMap(
-    '22009_Genetic-principal-components_0_5', Interpretation.CONTINUOUS, path_prefix='continuous', #normalization={'mean': -0.014422761536727896, 'std': 10.57799283718005},
+    '22009_Genetic-principal-components_0_5', Interpretation.CONTINUOUS, path_prefix='continuous',
+    # normalization={'mean': -0.014422761536727896, 'std': 10.57799283718005},
     loss='logcosh', activation='linear', channel_map={'22009_Genetic-principal-components_0_5': 0},
 )
 genetic_pca_6 = TensorMap(
     '22009_Genetic-principal-components_0_6', Interpretation.CONTINUOUS, path_prefix='continuous',
     loss='logcosh', activation='linear', channel_map={'22009_Genetic-principal-components_0_6': 0},
 )
 
@@ -238,319 +335,321 @@
 )
 
 genetic_pca_40 = TensorMap(
     '22009_Genetic-principal-components_0_40', Interpretation.CONTINUOUS, path_prefix='continuous',
     loss='logcosh', activation='linear', channel_map={'22009_Genetic-principal-components_0_40': 0},
 )
 
-
 offset = 192
 genetic_pca_1_partition = TensorMap(
     '22009_Genetic-principal-components_0_1', Interpretation.CONTINUOUS, path_prefix='continuous',
     normalization={'mean': -0.014422761536727896, 'std': 10.57799283718005},
-    days_window = offset, annotation_units = 64,
+    days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_1': 0},
 )
 genetic_pca_2_partition = TensorMap(
     '22009_Genetic-principal-components_0_2', Interpretation.CONTINUOUS, path_prefix='continuous',
     normalization={'mean': -0.014422761536727896, 'std': 10.57799283718005},
-    days_window = offset, annotation_units = 64,
+    days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_2': 0},
 )
 genetic_pca_3_partition = TensorMap(
     '22009_Genetic-principal-components_0_3', Interpretation.CONTINUOUS, path_prefix='continuous',
     normalization={'mean': -0.014422761536727896, 'std': 10.57799283718005},
-    days_window = offset, annotation_units = 64,
+    days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_3': 0},
 )
 genetic_pca_4_partition = TensorMap(
     '22009_Genetic-principal-components_0_4', Interpretation.CONTINUOUS, path_prefix='continuous',
     normalization={'mean': -0.014422761536727896, 'std': 10.57799283718005},
-    days_window = offset, annotation_units = 64,
+    days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_4': 0},
 )
 genetic_pca_5_partition = TensorMap(
     '22009_Genetic-principal-components_0_5', Interpretation.CONTINUOUS, path_prefix='continuous',
     normalization={'mean': -0.014422761536727896, 'std': 10.57799283718005},
-    days_window = offset, annotation_units = 64,
+    days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_5': 0},
 )
 genetic_pca_6_partition = TensorMap(
     '22009_Genetic-principal-components_0_6', Interpretation.CONTINUOUS, path_prefix='continuous',
-    normalization={'mean': -0.0144, 'std': 10.578}, days_window = offset, annotation_units = 64,
+    normalization={'mean': -0.0144, 'std': 10.578}, days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_6': 0},
 )
 
 genetic_pca_7_partition = TensorMap(
     '22009_Genetic-principal-components_0_7', Interpretation.CONTINUOUS, path_prefix='continuous',
-    normalization={'mean': -0.0144, 'std': 10.578}, days_window = offset, annotation_units = 64,
+    normalization={'mean': -0.0144, 'std': 10.578}, days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_7': 0},
 )
 
 genetic_pca_8_partition = TensorMap(
     '22009_Genetic-principal-components_0_8', Interpretation.CONTINUOUS, path_prefix='continuous',
-    normalization={'mean': -0.0144, 'std': 10.578}, days_window = offset, annotation_units = 64,
+    normalization={'mean': -0.0144, 'std': 10.578}, days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_8': 0},
 )
 
 genetic_pca_9_partition = TensorMap(
     '22009_Genetic-principal-components_0_9', Interpretation.CONTINUOUS, path_prefix='continuous',
-    normalization={'mean': -0.0144, 'std': 10.578}, days_window = offset, annotation_units = 64,
+    normalization={'mean': -0.0144, 'std': 10.578}, days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_9': 0},
 )
 
 genetic_pca_10_partition = TensorMap(
     '22009_Genetic-principal-components_0_10', Interpretation.CONTINUOUS, path_prefix='continuous',
-    normalization={'mean': -0.0144, 'std': 10.578}, days_window = offset, annotation_units = 64,
+    normalization={'mean': -0.0144, 'std': 10.578}, days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_10': 0},
 )
 
 genetic_pca_11_partition = TensorMap(
     '22009_Genetic-principal-components_0_11', Interpretation.CONTINUOUS, path_prefix='continuous',
-    normalization={'mean': -0.0144, 'std': 10.578}, days_window = offset, annotation_units = 64,
+    normalization={'mean': -0.0144, 'std': 10.578}, days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_11': 0},
 )
 
 genetic_pca_12_partition = TensorMap(
     '22009_Genetic-principal-components_0_12', Interpretation.CONTINUOUS, path_prefix='continuous',
-    normalization={'mean': -0.0144, 'std': 10.578}, days_window = offset, annotation_units = 64,
+    normalization={'mean': -0.0144, 'std': 10.578}, days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_12': 0},
 )
 
 genetic_pca_13_partition = TensorMap(
     '22009_Genetic-principal-components_0_13', Interpretation.CONTINUOUS, path_prefix='continuous',
-    normalization={'mean': -0.0144, 'std': 10.578}, days_window = offset, annotation_units = 64,
+    normalization={'mean': -0.0144, 'std': 10.578}, days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_13': 0},
 )
 
 genetic_pca_14_partition = TensorMap(
     '22009_Genetic-principal-components_0_14', Interpretation.CONTINUOUS, path_prefix='continuous',
-    normalization={'mean': -0.0144, 'std': 10.578}, days_window = offset, annotation_units = 64,
+    normalization={'mean': -0.0144, 'std': 10.578}, days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_14': 0},
 )
 
 genetic_pca_15_partition = TensorMap(
     '22009_Genetic-principal-components_0_15', Interpretation.CONTINUOUS, path_prefix='continuous',
-    normalization={'mean': -0.0144, 'std': 10.578}, days_window = offset, annotation_units = 64,
+    normalization={'mean': -0.0144, 'std': 10.578}, days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_15': 0},
 )
 
 genetic_pca_16_partition = TensorMap(
     '22009_Genetic-principal-components_0_16', Interpretation.CONTINUOUS, path_prefix='continuous',
-    normalization={'mean': -0.0144, 'std': 10.578}, days_window = offset, annotation_units = 64,
+    normalization={'mean': -0.0144, 'std': 10.578}, days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_16': 0},
 )
 
 genetic_pca_17_partition = TensorMap(
     '22009_Genetic-principal-components_0_17', Interpretation.CONTINUOUS, path_prefix='continuous',
-    normalization={'mean': -0.0144, 'std': 10.578}, days_window = offset, annotation_units = 64,
+    normalization={'mean': -0.0144, 'std': 10.578}, days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_17': 0},
 )
 
 genetic_pca_18_partition = TensorMap(
     '22009_Genetic-principal-components_0_18', Interpretation.CONTINUOUS, path_prefix='continuous',
-    normalization={'mean': -0.0144, 'std': 10.578}, days_window = offset, annotation_units = 64,
+    normalization={'mean': -0.0144, 'std': 10.578}, days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_18': 0},
 )
 
 genetic_pca_19_partition = TensorMap(
     '22009_Genetic-principal-components_0_19', Interpretation.CONTINUOUS, path_prefix='continuous',
-    normalization={'mean': -0.0144, 'std': 10.578}, days_window = offset, annotation_units = 64,
+    normalization={'mean': -0.0144, 'std': 10.578}, days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_19': 0},
 )
 
 genetic_pca_20_partition = TensorMap(
     '22009_Genetic-principal-components_0_20', Interpretation.CONTINUOUS, path_prefix='continuous',
-    normalization={'mean': -0.0144, 'std': 10.578}, days_window = offset, annotation_units = 64,
+    normalization={'mean': -0.0144, 'std': 10.578}, days_window=offset, annotation_units=64,
     loss='logcosh', channel_map={'22009_Genetic-principal-components_0_20': 0},
 )
 
 genetic_pca_all5 = TensorMap(
     'genetic_pca_all5', Interpretation.CONTINUOUS, path_prefix='continuous',
     normalization={'mean': -0.014, 'std': 10.578}, loss='logcosh', annotation_units=5, shape=(5,), activation='linear',
     channel_map={
         '22009_Genetic-principal-components_0_0': 0, '22009_Genetic-principal-components_0_1': 1,
         '22009_Genetic-principal-components_0_2': 2, '22009_Genetic-principal-components_0_3': 3,
         '22009_Genetic-principal-components_0_4': 4,
     },
 )
 
 genetic_caucasian = TensorMap(
-    'Genetic-ethnic-grouping_Caucasian_0_0', Interpretation.CATEGORICAL, path_prefix='categorical', storage_type=StorageType.CATEGORICAL_FLAG,
+    'Genetic-ethnic-grouping_Caucasian_0_0', Interpretation.CATEGORICAL, path_prefix='categorical',
+    storage_type=StorageType.CATEGORICAL_FLAG,
     channel_map={'no_caucasian': 0, 'Genetic-ethnic-grouping_Caucasian_0_0': 1},
 )
 
 genetic_caucasian_weighted = TensorMap(
-    'Genetic-ethnic-grouping_Caucasian_0_0', Interpretation.CATEGORICAL, path_prefix='categorical', storage_type=StorageType.CATEGORICAL_FLAG,
-    channel_map={'no_caucasian': 0, 'Genetic-ethnic-grouping_Caucasian_0_0': 1}, loss=weighted_crossentropy([10.0, 1.0], 'caucasian_loss'),
+    'Genetic-ethnic-grouping_Caucasian_0_0', Interpretation.CATEGORICAL, path_prefix='categorical',
+    storage_type=StorageType.CATEGORICAL_FLAG,
+    channel_map={'no_caucasian': 0, 'Genetic-ethnic-grouping_Caucasian_0_0': 1},
+    loss=weighted_crossentropy([10.0, 1.0], 'caucasian_loss'),
 )
 
 
 def negative_mean_squared_error(y_true, y_pred):
-    return -1*mean_squared_error(y_true, y_pred)
+    return -1 * mean_squared_error(y_true, y_pred)
 
 
 negative_genetic_pca_1 = TensorMap(
     '22009_Genetic-principal-components_0_1', Interpretation.CONTINUOUS, path_prefix='continuous',
     loss=negative_mean_squared_error, activation='linear', channel_map={'22009_Genetic-principal-components_0_1': 0},
 )
 
 pearson_loss_genetic_pca_1 = TensorMap(
     'ploss_pca_1', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_1': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_1': 0},
 )
 pearson_loss_genetic_pca_2 = TensorMap(
     'ploss_pca_2', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_2': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_2': 0},
 )
 pearson_loss_genetic_pca_3 = TensorMap(
     'ploss_pca_3', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_3': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_3': 0},
 )
 pearson_loss_genetic_pca_4 = TensorMap(
     'ploss_pca_4', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_4': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_4': 0},
 )
 pearson_loss_genetic_pca_5 = TensorMap(
     'ploss_pca_5', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_5': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_5': 0},
 )
 pearson_loss_genetic_pca_6 = TensorMap(
     'ploss_pca_6', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_6': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_6': 0},
 )
 pearson_loss_genetic_pca_7 = TensorMap(
     'ploss_pca_7', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_7': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_7': 0},
 )
 pearson_loss_genetic_pca_8 = TensorMap(
     'ploss_pca_8', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_8': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_8': 0},
 )
 pearson_loss_genetic_pca_9 = TensorMap(
     'ploss_pca_9', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_9': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_9': 0},
 )
 pearson_loss_genetic_pca_10 = TensorMap(
     'ploss_pca_10', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_10': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_10': 0},
 )
 pearson_loss_genetic_pca_11 = TensorMap(
     'ploss_pca_11', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_11': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_11': 0},
 )
 pearson_loss_genetic_pca_12 = TensorMap(
     'ploss_pca_12', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_12': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_12': 0},
 )
 pearson_loss_genetic_pca_13 = TensorMap(
     'ploss_pca_13', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_13': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_13': 0},
 )
 pearson_loss_genetic_pca_14 = TensorMap(
     'ploss_pca_14', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_14': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_14': 0},
 )
 pearson_loss_genetic_pca_15 = TensorMap(
     'ploss_pca_15', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_15': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_15': 0},
 )
 pearson_loss_genetic_pca_16 = TensorMap(
     'ploss_pca_16', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_16': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_16': 0},
 )
 pearson_loss_genetic_pca_17 = TensorMap(
     'ploss_pca_17', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_17': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_17': 0},
 )
 pearson_loss_genetic_pca_18 = TensorMap(
     'ploss_pca_18', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_18': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_18': 0},
 )
 pearson_loss_genetic_pca_19 = TensorMap(
     'ploss_pca_19', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_19': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_19': 0},
 )
 pearson_loss_genetic_pca_20 = TensorMap(
     'ploss_pca_20', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_20': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_20': 0},
 )
 pearson_loss_genetic_pca_21 = TensorMap(
     'ploss_pca_21', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_21': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_21': 0},
 )
 pearson_loss_genetic_pca_22 = TensorMap(
     'ploss_pca_22', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_22': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_22': 0},
 )
 pearson_loss_genetic_pca_23 = TensorMap(
     'ploss_pca_23', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_23': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_23': 0},
 )
 pearson_loss_genetic_pca_24 = TensorMap(
     'ploss_pca_24', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_24': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_24': 0},
 )
 pearson_loss_genetic_pca_25 = TensorMap(
     'ploss_pca_25', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_25': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_25': 0},
 )
 pearson_loss_genetic_pca_26 = TensorMap(
     'ploss_pca_26', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_26': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_26': 0},
 )
 pearson_loss_genetic_pca_27 = TensorMap(
     'ploss_pca_27', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_27': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_27': 0},
 )
 pearson_loss_genetic_pca_28 = TensorMap(
     'ploss_pca_28', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_28': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_28': 0},
 )
 pearson_loss_genetic_pca_29 = TensorMap(
     'ploss_pca_29', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_29': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_29': 0},
 )
 pearson_loss_genetic_pca_30 = TensorMap(
     'ploss_pca_30', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_30': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_30': 0},
 )
 pearson_loss_genetic_pca_31 = TensorMap(
     'ploss_pca_31', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_31': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_31': 0},
 )
 pearson_loss_genetic_pca_32 = TensorMap(
     'ploss_pca_32', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_32': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_32': 0},
 )
 pearson_loss_genetic_pca_33 = TensorMap(
     'ploss_pca_33', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_33': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_33': 0},
 )
 pearson_loss_genetic_pca_34 = TensorMap(
     'ploss_pca_34', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_34': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_34': 0},
 )
 pearson_loss_genetic_pca_35 = TensorMap(
     'ploss_pca_35', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_35': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_35': 0},
 )
 pearson_loss_genetic_pca_36 = TensorMap(
     'ploss_pca_36', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_36': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_36': 0},
 )
 pearson_loss_genetic_pca_37 = TensorMap(
     'ploss_pca_37', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_37': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_37': 0},
 )
 pearson_loss_genetic_pca_38 = TensorMap(
     'ploss_pca_38', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_38': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_38': 0},
 )
 pearson_loss_genetic_pca_39 = TensorMap(
     'ploss_pca_39', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_39': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_39': 0},
 )
 pearson_loss_genetic_pca_40 = TensorMap(
     'ploss_pca_40', Interpretation.CONTINUOUS, path_prefix='continuous',
-        loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_40': 0},
+    loss=abs_pearson, metrics=[pearson], channel_map={'22009_Genetic-principal-components_0_40': 0},
 )
```

### Comparing `ml4h-0.0.4.dev4/ml4h/tensormap/ukb/mri.py` & `ml4h-0.0.5/ml4h/tensormap/ukb/mri.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from ml4h.normalizer import ZeroMeanStd1, Standardize
 from ml4h.TensorMap import TensorMap, Interpretation, make_range_validator
 from ml4h.tensormap.ukb.demographics import is_genetic_man, is_genetic_woman
 from ml4h.defines import MRI_TO_SEGMENT, MRI_SEGMENTED, MRI_SEGMENTED_CHANNEL_MAP, MRI_FRAMES, MRI_LVOT_SEGMENTED_CHANNEL_MAP, \
     MRI_LAX_2CH_SEGMENTED_CHANNEL_MAP, MRI_SAX_SEGMENTED_CHANNEL_MAP, LAX_4CH_HEART_LABELS, LAX_4CH_MYOCARDIUM_LABELS, StorageType, LAX_3CH_HEART_LABELS, \
     LAX_2CH_HEART_LABELS
 from ml4h.tensormap.general import get_tensor_at_first_date, normalized_first_date, pad_or_crop_array_to_shape, tensor_from_hd5
-from ml4h.defines import MRI_LAX_3CH_SEGMENTED_CHANNEL_MAP, MRI_LAX_4CH_SEGMENTED_CHANNEL_MAP, MRI_SAX_PAP_SEGMENTED_CHANNEL_MAP, MRI_AO_SEGMENTED_CHANNEL_MAP, MRI_LIVER_SEGMENTED_CHANNEL_MAP
+from ml4h.defines import MRI_LAX_3CH_SEGMENTED_CHANNEL_MAP, MRI_LAX_4CH_SEGMENTED_CHANNEL_MAP, MRI_SAX_PAP_SEGMENTED_CHANNEL_MAP, MRI_AO_SEGMENTED_CHANNEL_MAP, MRI_LIVER_SEGMENTED_CHANNEL_MAP, SAX_HEART_LABELS
 
 
 def _slice_subset_tensor(
     tensor_key,
     start,
     stop,
     step=1,
@@ -105,14 +105,18 @@
 def _mask_from_file(tm: TensorMap, hd5: h5py.File, dependents=None):
     original = get_tensor_at_first_date(hd5, tm.path_prefix, tm.name)
     reshaped = pad_or_crop_array_to_shape(tm.shape, original)
     tensor = to_categorical(reshaped[..., 0], tm.shape[-1])
     return tensor
 
 
+def image_from_hd5(tm: TensorMap, hd5: h5py.File, dependents: Dict = {}) -> np.ndarray:
+    return np.array(hd5[tm.name][:tm.shape[0], :tm.shape[1], :tm.shape[2]], dtype=np.float32)
+
+
 def _mask_subset_tensor(tensor_key, start, stop, step=1, pad_shape=None):
     slice_subset_tensor_from_file = _slice_subset_tensor(
         tensor_key,
         start,
         stop,
         step=step,
         pad_shape=pad_shape,
@@ -732,42 +736,50 @@
     tensor_from_file=_segmented_dicom_slices(
         'liver_shmolli_segmented_annotated_', path_prefix='ukb_liver_mri',
     ),
     channel_map=MRI_LIVER_SEGMENTED_CHANNEL_MAP,
 )
 
 
-def sax_tensor(b_series_prefix, b_series_offset=1):
+def sax_tensor(b_series_prefix, b_series_start=0, b_series_offset=1):
     def sax_tensor_from_file(tm, hd5, dependents={}):
         missing = 0
         tensor = np.zeros(tm.shape, dtype=np.float32)
         if tm.axes() == 3:
             for b in range(tm.shape[-1]):
                 try:
                     tm_shape = (tm.shape[0], tm.shape[1])
-                    tensor[:, :, b] = pad_or_crop_array_to_shape(tm_shape, np.array(hd5[f'{tm.path_prefix}/{b_series_prefix}/instance_{(50*b)+b_series_offset}'], dtype=np.float32))
+                    b_instance = (50*(b_series_start+b))+b_series_offset
+                    tensor[:, :, b] = pad_or_crop_array_to_shape(
+                        tm_shape, np.array(
+                            hd5[f'{tm.path_prefix}/{b_series_prefix}/instance_{b_instance}'], dtype=np.float32,
+                        ),
+                    )
                 except KeyError:
                     missing += 1
                     tensor[:, :, b] = 0
         else:
             for b in range(tm.shape[-2]):
                 try:
                     tm_shape = (tm.shape[0], tm.shape[1])
-                    hd5_array = np.array(hd5[f'{tm.path_prefix}/{b_series_prefix}/instance_{(50*b)+b_series_offset}'], dtype=np.float32)
+                    b_instance = (50 * (b_series_start + b)) + b_series_offset
+                    hd5_array = np.array(
+                        hd5[f'{tm.path_prefix}/{b_series_prefix}/instance_{b_instance}'], dtype=np.float32,
+                    )
                     if tm.is_categorical():
                         categorical_index_slice = pad_or_crop_array_to_shape(tm_shape, hd5_array)
                         tensor[:, :, b] = to_categorical(categorical_index_slice, len(tm.channel_map))
                     else:
                         tensor[:, :, b, 0] = pad_or_crop_array_to_shape(tm_shape, hd5_array)
                 except KeyError:
                     missing += 1
                     if tm.is_categorical():
                         tensor[:, :, b, MRI_SEGMENTED_CHANNEL_MAP['background']] = 1
             if missing == tm.shape[-2]:
-                raise ValueError(f'Could not find any slices in {tm.name} was hoping for {tm.shape[-2]} looked at: {tm.path_prefix}/{b_series_prefix}')
+                raise ValueError(f'No {tm.name} instances {tm.shape[-2]} tried:{tm.path_prefix}/{b_series_prefix}')
         return tensor
     return sax_tensor_from_file
 
 
 sax_all_diastole_segmented = TensorMap(
     'sax_all_diastole_segmented', Interpretation.CATEGORICAL, shape=(256, 256, 13, len(MRI_SEGMENTED_CHANNEL_MAP)),
     tensor_from_file=sax_tensor('cine_segmented_sax_inlinevf_segmented/2'),
@@ -802,25 +814,29 @@
     'sax_all_systole_3d', shape=(224, 224, 13), tensor_from_file=sax_tensor('cine_segmented_sax_inlinevf/2', 18),
     path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
 )
 sax_all_diastole_3d_3slice = TensorMap(
     'sax_all_diastole', shape=(224, 224, 3), tensor_from_file=sax_tensor('cine_segmented_sax_inlinevf/2'),
     path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
 )
-sax_all_diastole_3d_3slice = TensorMap(
-    'sax_all_diastole', shape=(224, 224, 3), path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
+sax_b0_b2_diastole = TensorMap(
+    'sax_b0_b2_diastole', shape=(224, 224, 3), path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
     tensor_from_file=sax_tensor('cine_segmented_sax_inlinevf/2'),
 )
-sax_all_diastole_3d_3slice_b3 = TensorMap(
-    'sax_all_diastole', shape=(224, 224, 3), path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
-    tensor_from_file=sax_tensor('cine_segmented_sax_inlinevf/2', b_series_offset=3),
-)
-sax_all_diastole_3d_3slice_b6 = TensorMap(
-    'sax_all_diastole', shape=(224, 224, 3), path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
-    tensor_from_file=sax_tensor('cine_segmented_sax_inlinevf/2', b_series_offset=6),
+sax_b3_b5_diastole = TensorMap(
+    'sax_b3_b5_diastole', shape=(224, 224, 3), path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
+    tensor_from_file=sax_tensor('cine_segmented_sax_inlinevf/2', b_series_start=3),
+)
+sax_b6_b8_diastole = TensorMap(
+    'sax_b6_b8_diastole', shape=(224, 224, 3), path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
+    tensor_from_file=sax_tensor('cine_segmented_sax_inlinevf/2', b_series_start=6),
+)
+sax_b9_b11_diastole = TensorMap(
+    'sax_b9_b11_diastole', shape=(224, 224, 3), path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
+    tensor_from_file=sax_tensor('cine_segmented_sax_inlinevf/2', b_series_start=9),
 )
 
 def sax_random_slice_tensor_maker(b_series_prefix, b_segmented_prefix, lv_tsv=None):
     error = None
     if lv_tsv:
         try:
             with open(lv_tsv, 'r') as f:
@@ -1174,14 +1190,33 @@
         'cine_segmented_lax_4ch/2/',
         'cine_segmented_lax_4ch_annotated_',
         LAX_4CH_HEART_LABELS,
         random_instance=True,
     ),
     normalization=ZeroMeanStd1(), cacheable=False,
 )
+heart_mask_lax_4ch_diastole = TensorMap(
+    'heart_mask_lax_4ch_diastole', Interpretation.CONTINUOUS, shape=(160, 224, 1), path_prefix='ukb_cardiac_mri',
+    tensor_from_file=_heart_mask_instance(
+        'cine_segmented_lax_4ch/2/',
+        'cine_segmented_lax_4ch_annotated_',
+        LAX_4CH_HEART_LABELS,
+        instance_num=1,
+    ),
+    normalization=ZeroMeanStd1(),
+)
+
+heart_mask_lax_4ch_diastole_registered = TensorMap(
+    'heart_mask_lax_4ch_diastole_registered', Interpretation.CONTINUOUS, shape=(160, 224, 1),
+    tensor_from_file=image_from_hd5, normalization=ZeroMeanStd1(),
+)
+heart_mask_lax_4ch_diastole_flow = TensorMap(
+    'heart_mask_lax_4ch_diastole_flow', Interpretation.CONTINUOUS, shape=(160, 224, 2),
+    tensor_from_file=image_from_hd5, normalization=ZeroMeanStd1(),
+)
 myocardium_mask_lax_4ch_random_time = TensorMap(
     'myocardium_mask_lax_4ch_random_time', Interpretation.CONTINUOUS, shape=(120, 180, 1), path_prefix='ukb_cardiac_mri',
     tensor_from_file=_heart_mask_instance(
         'cine_segmented_lax_4ch/2/',
         'cine_segmented_lax_4ch_annotated_',
         LAX_4CH_MYOCARDIUM_LABELS,
         random_instance=True,
@@ -1232,50 +1267,174 @@
         LAX_4CH_MYOCARDIUM_LABELS,
         8,
     ),
     normalization=ZeroMeanStd1(), cacheable=False,
 )
 
 
-def _heart_mask_instances(mri_key, segmentation_key, labels, mask=False, max_frame=False):
+def _heart_mask_instances(mri_key, segmentation_key, labels, mask=False, max_frame=False, max_instance=50, is_sax=False, sax_b=3):
     def _heart_mask_tensor_from_file(tm, hd5, dependents={}):
-        diastole_categorical = get_tensor_at_first_date(hd5, tm.path_prefix, f'{segmentation_key}{1}')
-        mri = get_tensor_at_first_date(hd5, tm.path_prefix, f'{mri_key}')
+        if is_sax:
+            b_instance = (50 * sax_b) + 1
+            diastole_categorical = get_tensor_at_first_date(hd5, tm.path_prefix, f'{segmentation_key}')
+            b_frames = []
+            for b in range(b_instance, b_instance+tm.shape[-2]):
+                b_frames.append(np.array(hd5[f'{tm.path_prefix}/{mri_key}{b}'], dtype=np.float32))
+            mri = np.swapaxes(np.swapaxes(np.array(b_frames), 0, 2), 0, 1)
+        else:
+            diastole_categorical = get_tensor_at_first_date(hd5, tm.path_prefix, f'{segmentation_key}{1}')
+            mri = get_tensor_at_first_date(hd5, tm.path_prefix, f'{mri_key}')
         heart_mask = np.isin(diastole_categorical, list(labels.values()))
         i, j = np.where(heart_mask)
         if max_frame:
             max_i = np.argmax(np.sum(heart_mask, axis=(0, 1)))
             indices = np.meshgrid(np.arange(min(i), max(i) + 1), np.arange(min(j), max(j) + 1), max_i, indexing='ij')
             if mask:
                 mri[..., max_i] = heart_mask[:mri.shape[0], :mri.shape[1]] * mri[..., max_i]
             return pad_or_crop_array_to_shape(tm.shape, mri[tuple(indices)])
-        indices = np.meshgrid(np.arange(min(i), max(i) + 1), np.arange(min(j), max(j) + 1), np.arange(50), indexing='ij')
+        indices = np.meshgrid(np.arange(min(i), max(i) + 1), np.arange(min(j), max(j) + 1), np.arange(max_instance), indexing='ij')
         if mask:
-            for frame in range(1, 51):
+            for frame in range(1, max_instance+1):
                 frame_categorical = get_tensor_at_first_date(hd5, tm.path_prefix, f'{segmentation_key}{frame}')
                 heart_mask = np.isin(frame_categorical, list(labels.values()))
                 mri[..., frame-1] = heart_mask[:mri.shape[0], :mri.shape[1]] * mri[..., frame-1]
         tensor = pad_or_crop_array_to_shape(tm.shape, mri[tuple(indices)])
         return tensor
     return _heart_mask_tensor_from_file
 
 
 lax_4ch_heart_center = TensorMap(
     'lax_4ch_heart_center', Interpretation.CONTINUOUS, shape=(96, 96, 50), path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
     tensor_from_file=_heart_mask_instances('cine_segmented_lax_4ch/2/', 'cine_segmented_lax_4ch_annotated_', LAX_4CH_HEART_LABELS),
 )
+lax_4ch_heart_center_48 = TensorMap(
+    'lax_4ch_heart_center', Interpretation.CONTINUOUS, shape=(96, 96, 48), path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
+    tensor_from_file=_heart_mask_instances('cine_segmented_lax_4ch/2/', 'cine_segmented_lax_4ch_annotated_', LAX_4CH_HEART_LABELS, max_instance=48),
+)
 lax_3ch_heart_center = TensorMap(
     'lax_3ch_heart_center', Interpretation.CONTINUOUS, shape=(96, 96, 50), path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
     tensor_from_file=_heart_mask_instances('cine_segmented_lax_3ch/2/', 'cine_segmented_lax_3ch_annotated_', LAX_3CH_HEART_LABELS),
 )
 lax_2ch_heart_center = TensorMap(
     'lax_2ch_heart_center', Interpretation.CONTINUOUS, shape=(96, 96, 50), path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
     tensor_from_file=_heart_mask_instances('cine_segmented_lax_2ch/2/', 'cine_segmented_lax_2ch_annotated_', LAX_2CH_HEART_LABELS),
 )
+sax_b0_heart_center = TensorMap(
+    'sax_b0_heart_center', Interpretation.CONTINUOUS, shape=(64, 64, 50),
+    path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
+    tensor_from_file=_heart_mask_instances(
+        'cine_segmented_sax_inlinevf/2/instance_',  'cine_segmented_sax_inlinevf_segmented/2',
+        {'myocardium': 1, 'pool': 2}, is_sax = True, sax_b=0,
+    ),
+)
+sax_b1_heart_center = TensorMap(
+    'sax_b1_heart_center', Interpretation.CONTINUOUS, shape=(64, 64, 50),
+    path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
+    tensor_from_file=_heart_mask_instances(
+        'cine_segmented_sax_inlinevf/2/instance_',  'cine_segmented_sax_inlinevf_segmented/2',
+        {'myocardium': 1, 'pool': 2}, is_sax = True, sax_b=1,
+    ),
+)
+sax_b2_heart_center = TensorMap(
+    'sax_b2_heart_center', Interpretation.CONTINUOUS, shape=(64, 64, 50),
+    path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
+    tensor_from_file=_heart_mask_instances(
+        'cine_segmented_sax_inlinevf/2/instance_',  'cine_segmented_sax_inlinevf_segmented/2',
+        {'myocardium': 1, 'pool': 2}, is_sax = True, sax_b=2,
+    ),
+)
+sax_b3_heart_center = TensorMap(
+    'sax_b3_heart_center', Interpretation.CONTINUOUS, shape=(64, 64, 50),
+    path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
+    tensor_from_file=_heart_mask_instances(
+        'cine_segmented_sax_inlinevf/2/instance_',  'cine_segmented_sax_inlinevf_segmented/2',
+        {'myocardium': 1, 'pool': 2}, is_sax = True, sax_b=3,
+    ),
+)
+sax_b4_heart_center = TensorMap(
+    'sax_b4_heart_center', Interpretation.CONTINUOUS, shape=(64, 64, 50),
+    path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
+    tensor_from_file=_heart_mask_instances(
+        'cine_segmented_sax_inlinevf/2/instance_',  'cine_segmented_sax_inlinevf_segmented/2',
+        {'myocardium': 1, 'pool': 2}, is_sax = True, sax_b=4,
+    ),
+)
+sax_b5_heart_center = TensorMap(
+    'sax_b5_heart_center', Interpretation.CONTINUOUS, shape=(64, 64, 50),
+    path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
+    tensor_from_file=_heart_mask_instances(
+        'cine_segmented_sax_inlinevf/2/instance_',  'cine_segmented_sax_inlinevf_segmented/2',
+        {'myocardium': 1, 'pool': 2}, is_sax = True, sax_b=5,
+    ),
+)
+sax_b6_heart_center = TensorMap(
+    'sax_b6_heart_center', Interpretation.CONTINUOUS, shape=(64, 64, 50),
+    path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
+    tensor_from_file=_heart_mask_instances(
+        'cine_segmented_sax_inlinevf/2/instance_',  'cine_segmented_sax_inlinevf_segmented/2',
+        {'myocardium': 1, 'pool': 2}, is_sax = True, sax_b=6,
+    ),
+)
+sax_b7_heart_center = TensorMap(
+    'sax_b7_heart_center', Interpretation.CONTINUOUS, shape=(64, 64, 50),
+    path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
+    tensor_from_file=_heart_mask_instances(
+        'cine_segmented_sax_inlinevf/2/instance_',  'cine_segmented_sax_inlinevf_segmented/2',
+        {'myocardium': 1, 'pool': 2}, is_sax = True, sax_b=7,
+    ),
+)
+sax_b8_heart_center = TensorMap(
+    'sax_b8_heart_center', Interpretation.CONTINUOUS, shape=(64, 64, 50),
+    path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
+    tensor_from_file=_heart_mask_instances(
+        'cine_segmented_sax_inlinevf/2/instance_',  'cine_segmented_sax_inlinevf_segmented/2',
+        {'myocardium': 1, 'pool': 2}, is_sax = True, sax_b=8,
+    ),
+)
+sax_b9_heart_center = TensorMap(
+    'sax_b9_heart_center', Interpretation.CONTINUOUS, shape=(64, 64, 50),
+    path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
+    tensor_from_file=_heart_mask_instances(
+        'cine_segmented_sax_inlinevf/2/instance_',  'cine_segmented_sax_inlinevf_segmented/2',
+        {'myocardium': 1, 'pool': 2}, is_sax = True, sax_b=9,
+    ),
+)
+sax_b10_heart_center = TensorMap(
+    'sax_b10_heart_center', Interpretation.CONTINUOUS, shape=(64, 64, 50),
+    path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
+    tensor_from_file=_heart_mask_instances(
+        'cine_segmented_sax_inlinevf/2/instance_',  'cine_segmented_sax_inlinevf_segmented/2',
+        {'myocardium': 1, 'pool': 2}, is_sax = True, sax_b=10,
+    ),
+)
+sax_b11_heart_center = TensorMap(
+    'sax_b11_heart_center', Interpretation.CONTINUOUS, shape=(64, 64, 50),
+    path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
+    tensor_from_file=_heart_mask_instances(
+        'cine_segmented_sax_inlinevf/2/instance_',  'cine_segmented_sax_inlinevf_segmented/2',
+        {'myocardium': 1, 'pool': 2}, is_sax = True, sax_b=11,
+    ),
+)
+sax_b12_heart_center = TensorMap(
+    'sax_b12_heart_center', Interpretation.CONTINUOUS, shape=(64, 64, 50),
+    path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
+    tensor_from_file=_heart_mask_instances(
+        'cine_segmented_sax_inlinevf/2/instance_',  'cine_segmented_sax_inlinevf_segmented/2',
+        {'myocardium': 1, 'pool': 2}, is_sax = True, sax_b=12,
+    ),
+)
 
+lax_4ch_heart_center_48_registered = TensorMap(
+    'lax_4ch_heart_center_registered', Interpretation.CONTINUOUS, shape=(96, 96, 48), path_prefix='ukb_cardiac_mri',
+    normalization=ZeroMeanStd1(), tensor_from_file=image_from_hd5,
+)
+lax_4ch_heart_center_48_flow = TensorMap(
+    'lax_4ch_heart_center_flow', Interpretation.CONTINUOUS, shape=(96, 96, 48, 3), path_prefix='ukb_cardiac_mri',
+    normalization=ZeroMeanStd1(), tensor_from_file=image_from_hd5,
+)
 lax_2ch_laa = TensorMap(
     'lax_2ch_laa', Interpretation.CONTINUOUS, shape=(16, 16, 50), path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
     tensor_from_file=_heart_mask_instances('cine_segmented_lax_2ch/2/', 'cine_segmented_lax_2ch_annotated_', {'LA_appendage': 4}),
 )
 lax_2ch_la_plus = TensorMap(
     'lax_2ch_la_plus', Interpretation.CONTINUOUS, shape=(48, 48, 50), path_prefix='ukb_cardiac_mri', normalization=ZeroMeanStd1(),
     tensor_from_file=_heart_mask_instances(
```

### Comparing `ml4h-0.0.4.dev4/ml4h/tensormap/ukb/mri_brain.py` & `ml4h-0.0.5/ml4h/tensormap/ukb/mri_brain.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/tensormap/ukb/mri_ecg.py` & `ml4h-0.0.5/ml4h/tensormap/ukb/mri_ecg.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/tensormap/ukb/mri_vtk.py` & `ml4h-0.0.5/ml4h/tensormap/ukb/mri_vtk.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/tensormap/ukb/survival.py` & `ml4h-0.0.5/ml4h/tensormap/ukb/survival.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import datetime
 from ml4h.TensorMap import TensorMap, Interpretation, str2date
 from ml4h.defines import StorageType
 from ml4h.metrics import weighted_crossentropy
 from ml4h.tensormap.ukb.demographics import prevalent_tensor
 
 DAYS_IN_5_YEARS = 365 * 5
+DAYS_IN_10_YEARS = 365 * 10
 
 
 def _survival_tensor(
     start_date_key: str,
     day_window: int,
     disease_name_override: str = None,
     incidence_only: bool = False,
@@ -313,15 +314,70 @@
     days_window=DAYS_IN_5_YEARS,
     tensor_from_file=_survival_tensor(
         'ukb_ecg_rest/ecg_rest_text/instance_2', DAYS_IN_5_YEARS,
         disease_name_override='myocardial_infarction',
         start_date_is_attribute=True, incidence_only=True,
     ),
 )
+mgb_hf_wrt_instance2 = TensorMap(
+    'hf_event',
+    Interpretation.SURVIVAL_CURVE,
+    shape=(50,),
+    days_window=DAYS_IN_10_YEARS,
+    tensor_from_file=_survival_tensor(
+        'ukb_ecg_rest/ecg_rest_text/instance_2', DAYS_IN_10_YEARS,
+        disease_name_override='heart_failure',
+        start_date_is_attribute=True, incidence_only=True,
+    ),
+)
+mgb_hf_wrt_instance2 = TensorMap(
+    'hf_event',
+    Interpretation.SURVIVAL_CURVE,
+    shape=(50,),
+    days_window=DAYS_IN_10_YEARS,
+    tensor_from_file=_survival_tensor(
+        'ukb_ecg_rest/ecg_rest_text/instance_2', DAYS_IN_10_YEARS,
+        disease_name_override='heart_failure',
+        start_date_is_attribute=True, incidence_only=True,
+    ),
+)
+mgb_hf_nlp_wrt_instance2 = TensorMap(
+    'hf_nlp_event',
+    Interpretation.SURVIVAL_CURVE,
+    shape=(50,),
+    days_window=DAYS_IN_10_YEARS,
+    tensor_from_file=_survival_tensor(
+        'ukb_ecg_rest/ecg_rest_text/instance_2', DAYS_IN_10_YEARS,
+        disease_name_override='heart_failure',
+        start_date_is_attribute=True, incidence_only=True,
+    ),
+)
+mgb_hf_primary_wrt_instance2 = TensorMap(
+    'hf_primary_event',
+    Interpretation.SURVIVAL_CURVE,
+    shape=(50,),
+    days_window=DAYS_IN_10_YEARS,
+    tensor_from_file=_survival_tensor(
+        'ukb_ecg_rest/ecg_rest_text/instance_2', DAYS_IN_10_YEARS,
+        disease_name_override='heart_failure',
+        start_date_is_attribute=True, incidence_only=True,
+    ),
+)
 
+mgb_hf_death_wrt_instance2 = TensorMap(
+    'hf_death_event',
+    Interpretation.SURVIVAL_CURVE,
+    shape=(50,),
+    days_window=DAYS_IN_10_YEARS,
+    tensor_from_file=_survival_tensor(
+        'ukb_ecg_rest/ecg_rest_text/instance_2', DAYS_IN_10_YEARS,
+        disease_name_override='death',
+        start_date_is_attribute=True, incidence_only=True,
+    ),
+)
 mgb_afib_as_hf_wrt_instance2 = TensorMap(
     'survival_curve_af',
     Interpretation.SURVIVAL_CURVE,
     shape=(50,),
     days_window=DAYS_IN_5_YEARS,
     tensor_from_file=_survival_tensor(
         'ukb_ecg_rest/ecg_rest_text/instance_2', DAYS_IN_5_YEARS,
```

### Comparing `ml4h-0.0.4.dev4/ml4h/test_utils.py` & `ml4h-0.0.5/ml4h/test_utils.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/visualization_tools/annotation_storage.py` & `ml4h-0.0.5/ml4h/visualization_tools/annotation_storage.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/visualization_tools/annotations.py` & `ml4h-0.0.5/ml4h/visualization_tools/annotations.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/visualization_tools/batch_image_annotations.py` & `ml4h-0.0.5/ml4h/visualization_tools/batch_image_annotations.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/visualization_tools/dicom_interactive_plots.py` & `ml4h-0.0.5/ml4h/visualization_tools/dicom_interactive_plots.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/visualization_tools/dicom_plots.py` & `ml4h-0.0.5/ml4h/visualization_tools/dicom_plots.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/visualization_tools/ecg_interactive_plots.py` & `ml4h-0.0.5/ml4h/visualization_tools/ecg_interactive_plots.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/visualization_tools/ecg_reshape.py` & `ml4h-0.0.5/ml4h/visualization_tools/ecg_reshape.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/visualization_tools/ecg_static_plots.py` & `ml4h-0.0.5/ml4h/visualization_tools/ecg_static_plots.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/visualization_tools/facets.py` & `ml4h-0.0.5/ml4h/visualization_tools/facets.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h/visualization_tools/hd5_mri_plots.py` & `ml4h-0.0.5/ml4h/visualization_tools/hd5_mri_plots.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.4.dev4/ml4h.egg-info/SOURCES.txt` & `ml4h-0.0.5/ml4h.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 ml4h/recipes.py
 ml4h/runtime_data_defines.py
 ml4h/tensor_generators.py
 ml4h/test_utils.py
 ml4h.egg-info/PKG-INFO
 ml4h.egg-info/SOURCES.txt
 ml4h.egg-info/dependency_links.txt
+ml4h.egg-info/requires.txt
 ml4h.egg-info/top_level.txt
 ml4h/ml4ht_integration/__init__.py
 ml4h/ml4ht_integration/tensor_generator.py
 ml4h/ml4ht_integration/tensor_map.py
 ml4h/models/Block.py
 ml4h/models/__init__.py
 ml4h/models/basic_blocks.py
@@ -52,18 +53,18 @@
 ml4h/tensormap/mnist.py
 ml4h/tensormap/tensor_map_maker.py
 ml4h/tensormap/text.py
 ml4h/tensormap/mgb/__init__.py
 ml4h/tensormap/mgb/dynamic.py
 ml4h/tensormap/mgb/ecg.py
 ml4h/tensormap/ukb/__init__.py
-ml4h/tensormap/ukb/by_script.py
 ml4h/tensormap/ukb/categorical.py
 ml4h/tensormap/ukb/continuous.py
 ml4h/tensormap/ukb/demographics.py
+ml4h/tensormap/ukb/disease.py
 ml4h/tensormap/ukb/dxa.py
 ml4h/tensormap/ukb/ecg.py
 ml4h/tensormap/ukb/genetics.py
 ml4h/tensormap/ukb/mri.py
 ml4h/tensormap/ukb/mri_brain.py
 ml4h/tensormap/ukb/mri_ecg.py
 ml4h/tensormap/ukb/mri_vtk.py
```


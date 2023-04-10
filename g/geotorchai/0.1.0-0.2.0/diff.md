# Comparing `tmp/geotorchai-0.1.0.tar.gz` & `tmp/geotorchai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/media/kchowdh1/fcf87b53-9c62-4c1d-9df2-cb2b83598bea/kanchan/programs/DataSysLab/Insall-Test/GeoTorchAI/dist/.tmp-ny4v3tx9/geot", last modified: Sun Jan  8 01:34:31 2023, max compression
+gzip compressed data, was "geotorchai-0.2.0.tar", last modified: Mon Apr 10 00:16:03 2023, max compression
```

## Comparing `geotorchai-0.1.0.tar` & `geotorchai-0.2.0.tar`

### file list

```diff
@@ -1,95 +1,101 @@
-drwxr-xr-x   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:31.000000 geotorchai-0.1.0/
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)    34524 2023-01-08 01:34:13.000000 geotorchai-0.1.0/LICENSE.md
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)    11135 2023-01-08 01:34:31.000000 geotorchai-0.1.0/PKG-INFO
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     9998 2023-01-08 01:34:13.000000 geotorchai-0.1.0/README.md
-drwxr-xr-x   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai/
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)       57 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/__init__.py
-drwxr-xr-x   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai/datasets/
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/datasets/__init__.py
-drwxr-xr-x   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai/datasets/grid/
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)      274 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/datasets/grid/__init__.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     8599 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/datasets/grid/nyc_bike_deepstn.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)    13747 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/datasets/grid/nyc_bike_stdn.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)    13711 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/datasets/grid/nyc_taxi_stdn.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     7333 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/datasets/grid/processed.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     7704 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/datasets/grid/taxi_bj_21.py
-drwxr-xr-x   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai/datasets/raster/
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)      356 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/datasets/raster/__init__.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     4188 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/datasets/raster/cloud_38.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     9216 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/datasets/raster/euro_sat.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     2008 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/datasets/raster/processed.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     3097 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/datasets/raster/processed_extra_features.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     8240 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/datasets/raster/sat4.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     8297 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/datasets/raster/sat6.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     8132 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/datasets/raster/slum_detection.py
-drwxr-xr-x   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai/datasets/raster/utility/
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/datasets/raster/utility/__init__.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     1106 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/datasets/raster/utility/spectral_indices.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     2034 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/datasets/raster/utility/textural_features.py
-drwxr-xr-x   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai/models/
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/models/__init__.py
-drwxr-xr-x   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai/models/grid/
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)      145 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/models/grid/__init__.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     4859 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/models/grid/conv_lstm.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)    10432 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/models/grid/deep_stn_net.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     6378 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/models/grid/st_resnet.py
-drwxr-xr-x   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai/models/raster/
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)      198 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/models/raster/__init__.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     1698 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/models/raster/deepsat2.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     1632 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/models/raster/fcn.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     1797 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/models/raster/sat_cnn.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     3488 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/models/raster/unet.py
-drwxr-xr-x   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai/preprocessing/
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)      284 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/preprocessing/__init__.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     7510 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/preprocessing/adapter.py
-drwxr-xr-x   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai/preprocessing/enums/
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)      256 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/preprocessing/enums/__init__.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)      556 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/preprocessing/enums/adjacency_type.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)      515 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/preprocessing/enums/aggregation_type.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)      450 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/preprocessing/enums/geo_file_type.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)      548 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/preprocessing/enums/geo_relationship.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     7614 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/preprocessing/geo_io.py
-drwxr-xr-x   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai/preprocessing/grid/
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)      167 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/preprocessing/grid/__init__.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     5943 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/preprocessing/grid/adjacency.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     6980 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/preprocessing/grid/space_partition.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)    21087 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/preprocessing/grid/st_manager.py
-drwxr-xr-x   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai/preprocessing/raster/
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)       80 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/preprocessing/raster/__init__.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)    39162 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/preprocessing/raster/raster_processing.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     1400 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/preprocessing/spark_registration.py
-drwxr-xr-x   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai/transforms/
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/transforms/__init__.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     2891 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/transforms/raster.py
-drwxr-xr-x   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai/utility/
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/utility/__init__.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     2506 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/utility/_download_utils.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)      801 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/utility/exceptions.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     5473 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/utility/method_overload.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)      207 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/utility/properties.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)       65 2023-01-08 01:34:13.000000 geotorchai-0.1.0/geotorchai/utility/types.py
-drwxr-xr-x   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai.egg-info/
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)    11135 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai.egg-info/PKG-INFO
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     2806 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai.egg-info/SOURCES.txt
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)        1 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai.egg-info/dependency_links.txt
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)       87 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai.egg-info/requires.txt
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)       17 2023-01-08 01:34:31.000000 geotorchai-0.1.0/geotorchai.egg-info/top_level.txt
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)       38 2023-01-08 01:34:31.000000 geotorchai-0.1.0/setup.cfg
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     1867 2023-01-08 01:34:13.000000 geotorchai-0.1.0/setup.py
-drwxr-xr-x   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:31.000000 geotorchai-0.1.0/tests/
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:13.000000 geotorchai-0.1.0/tests/__init__.py
-drwxr-xr-x   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:31.000000 geotorchai-0.1.0/tests/deep-learning/
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:13.000000 geotorchai-0.1.0/tests/deep-learning/__init__.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     2377 2023-01-08 01:34:13.000000 geotorchai-0.1.0/tests/deep-learning/test_grid_datasets.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     3541 2023-01-08 01:34:13.000000 geotorchai-0.1.0/tests/deep-learning/test_models.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     1928 2023-01-08 01:34:13.000000 geotorchai-0.1.0/tests/deep-learning/test_raster_datasets.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)      890 2023-01-08 01:34:13.000000 geotorchai-0.1.0/tests/deep-learning/test_transforms.py
-drwxr-xr-x   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:31.000000 geotorchai-0.1.0/tests/preprocessing/
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)        0 2023-01-08 01:34:13.000000 geotorchai-0.1.0/tests/preprocessing/__init__.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     2692 2023-01-08 01:34:13.000000 geotorchai-0.1.0/tests/preprocessing/test_adjacency.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     3081 2023-01-08 01:34:13.000000 geotorchai-0.1.0/tests/preprocessing/test_data_loader.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     2025 2023-01-08 01:34:13.000000 geotorchai-0.1.0/tests/preprocessing/test_feature_aggregation.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     2530 2023-01-08 01:34:13.000000 geotorchai-0.1.0/tests/preprocessing/test_raster_transform.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     3523 2023-01-08 01:34:13.000000 geotorchai-0.1.0/tests/preprocessing/test_space_partition.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)     2191 2023-01-08 01:34:13.000000 geotorchai-0.1.0/tests/preprocessing/test_spark_registration.py
--rw-r--r--   0 kchowdh1 (1941242839) domain^users (1940914689)      166 2023-01-08 01:34:13.000000 geotorchai-0.1.0/tests/preprocessing/utility.py
+drwxr-xr-x   0 kanchan    (501) staff       (20)        0 2023-04-10 00:16:03.176509 geotorchai-0.2.0/
+-rw-r--r--   0 kanchan    (501) staff       (20)    34524 2023-04-07 18:27:33.000000 geotorchai-0.2.0/LICENSE.md
+-rw-r--r--   0 kanchan    (501) staff       (20)    11097 2023-04-10 00:16:03.176332 geotorchai-0.2.0/PKG-INFO
+-rw-r--r--   0 kanchan    (501) staff       (20)     9960 2023-04-07 18:27:33.000000 geotorchai-0.2.0/README.md
+drwxr-xr-x   0 kanchan    (501) staff       (20)        0 2023-04-10 00:16:03.164397 geotorchai-0.2.0/geotorchai/
+-rw-r--r--   0 kanchan    (501) staff       (20)       57 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/__init__.py
+drwxr-xr-x   0 kanchan    (501) staff       (20)        0 2023-04-10 00:16:03.165259 geotorchai-0.2.0/geotorchai/datasets/
+-rw-r--r--   0 kanchan    (501) staff       (20)        0 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/datasets/__init__.py
+drwxr-xr-x   0 kanchan    (501) staff       (20)        0 2023-04-10 00:16:03.166910 geotorchai-0.2.0/geotorchai/datasets/grid/
+-rw-r--r--   0 kanchan    (501) staff       (20)      618 2023-02-07 21:36:55.000000 geotorchai-0.2.0/geotorchai/datasets/grid/__init__.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     8385 2023-04-09 05:40:33.000000 geotorchai-0.2.0/geotorchai/datasets/grid/geopotential.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     8659 2023-04-09 05:40:53.000000 geotorchai-0.2.0/geotorchai/datasets/grid/nyc_bike_deepstn.py
+-rw-r--r--   0 kanchan    (501) staff       (20)    13722 2023-04-09 05:41:10.000000 geotorchai-0.2.0/geotorchai/datasets/grid/nyc_bike_stdn.py
+-rw-r--r--   0 kanchan    (501) staff       (20)    13686 2023-04-09 05:41:26.000000 geotorchai-0.2.0/geotorchai/datasets/grid/nyc_taxi_stdn.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     6982 2023-04-09 05:41:50.000000 geotorchai-0.2.0/geotorchai/datasets/grid/processed.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     7273 2023-04-09 05:42:13.000000 geotorchai-0.2.0/geotorchai/datasets/grid/taxi_bj_21.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     8287 2023-04-09 05:47:46.000000 geotorchai-0.2.0/geotorchai/datasets/grid/temperature.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     8304 2023-04-09 05:43:11.000000 geotorchai-0.2.0/geotorchai/datasets/grid/toa_incident_solar_radiation.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     8282 2023-04-09 05:43:30.000000 geotorchai-0.2.0/geotorchai/datasets/grid/total_cloud_cover.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     8286 2023-04-09 05:43:50.000000 geotorchai-0.2.0/geotorchai/datasets/grid/total_precipitation.py
+drwxr-xr-x   0 kanchan    (501) staff       (20)        0 2023-04-10 00:16:03.168089 geotorchai-0.2.0/geotorchai/datasets/raster/
+-rw-r--r--   0 kanchan    (501) staff       (20)      356 2023-02-07 21:36:55.000000 geotorchai-0.2.0/geotorchai/datasets/raster/__init__.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     3736 2023-04-09 05:33:36.000000 geotorchai-0.2.0/geotorchai/datasets/raster/cloud_38.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     9171 2023-04-09 05:39:10.000000 geotorchai-0.2.0/geotorchai/datasets/raster/euro_sat.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     1963 2023-04-09 05:39:39.000000 geotorchai-0.2.0/geotorchai/datasets/raster/processed.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     3062 2023-04-09 05:40:01.000000 geotorchai-0.2.0/geotorchai/datasets/raster/processed_extra_features.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     7872 2023-04-09 05:34:35.000000 geotorchai-0.2.0/geotorchai/datasets/raster/sat4.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     7929 2023-04-09 05:35:44.000000 geotorchai-0.2.0/geotorchai/datasets/raster/sat6.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     7750 2023-04-09 05:33:22.000000 geotorchai-0.2.0/geotorchai/datasets/raster/slum_detection.py
+drwxr-xr-x   0 kanchan    (501) staff       (20)        0 2023-04-10 00:16:03.168495 geotorchai-0.2.0/geotorchai/datasets/raster/utility/
+-rw-r--r--   0 kanchan    (501) staff       (20)        0 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/datasets/raster/utility/__init__.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     1106 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/datasets/raster/utility/spectral_indices.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     2034 2023-04-07 23:34:49.000000 geotorchai-0.2.0/geotorchai/datasets/raster/utility/textural_features.py
+drwxr-xr-x   0 kanchan    (501) staff       (20)        0 2023-04-10 00:16:03.168637 geotorchai-0.2.0/geotorchai/models/
+-rw-r--r--   0 kanchan    (501) staff       (20)        0 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/models/__init__.py
+drwxr-xr-x   0 kanchan    (501) staff       (20)        0 2023-04-10 00:16:03.169345 geotorchai-0.2.0/geotorchai/models/grid/
+-rw-r--r--   0 kanchan    (501) staff       (20)      204 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/models/grid/__init__.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     4859 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/models/grid/conv_lstm.py
+-rw-r--r--   0 kanchan    (501) staff       (20)    10506 2023-04-08 18:09:37.000000 geotorchai-0.2.0/geotorchai/models/grid/deep_stn_net.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     2421 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/models/grid/periodical_cnn.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     6378 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/models/grid/st_resnet.py
+drwxr-xr-x   0 kanchan    (501) staff       (20)        0 2023-04-10 00:16:03.170053 geotorchai-0.2.0/geotorchai/models/raster/
+-rw-r--r--   0 kanchan    (501) staff       (20)      198 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/models/raster/__init__.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     1698 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/models/raster/deepsat2.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     1632 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/models/raster/fcn.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     1797 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/models/raster/sat_cnn.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     3488 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/models/raster/unet.py
+drwxr-xr-x   0 kanchan    (501) staff       (20)        0 2023-04-10 00:16:03.170646 geotorchai-0.2.0/geotorchai/preprocessing/
+-rw-r--r--   0 kanchan    (501) staff       (20)      284 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/preprocessing/__init__.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     7510 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/preprocessing/adapter.py
+drwxr-xr-x   0 kanchan    (501) staff       (20)        0 2023-04-10 00:16:03.171480 geotorchai-0.2.0/geotorchai/preprocessing/enums/
+-rw-r--r--   0 kanchan    (501) staff       (20)      256 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/preprocessing/enums/__init__.py
+-rw-r--r--   0 kanchan    (501) staff       (20)      556 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/preprocessing/enums/adjacency_type.py
+-rw-r--r--   0 kanchan    (501) staff       (20)      515 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/preprocessing/enums/aggregation_type.py
+-rw-r--r--   0 kanchan    (501) staff       (20)      450 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/preprocessing/enums/geo_file_type.py
+-rw-r--r--   0 kanchan    (501) staff       (20)      548 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/preprocessing/enums/geo_relationship.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     7614 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/preprocessing/geo_io.py
+drwxr-xr-x   0 kanchan    (501) staff       (20)        0 2023-04-10 00:16:03.172117 geotorchai-0.2.0/geotorchai/preprocessing/grid/
+-rw-r--r--   0 kanchan    (501) staff       (20)      167 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/preprocessing/grid/__init__.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     5943 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/preprocessing/grid/adjacency.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     7016 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/preprocessing/grid/space_partition.py
+-rw-r--r--   0 kanchan    (501) staff       (20)    27765 2023-04-09 22:15:24.000000 geotorchai-0.2.0/geotorchai/preprocessing/grid/st_manager.py
+drwxr-xr-x   0 kanchan    (501) staff       (20)        0 2023-04-10 00:16:03.172467 geotorchai-0.2.0/geotorchai/preprocessing/raster/
+-rw-r--r--   0 kanchan    (501) staff       (20)       80 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/preprocessing/raster/__init__.py
+-rw-r--r--   0 kanchan    (501) staff       (20)    39162 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/preprocessing/raster/raster_processing.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     1400 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/preprocessing/spark_registration.py
+drwxr-xr-x   0 kanchan    (501) staff       (20)        0 2023-04-10 00:16:03.172745 geotorchai-0.2.0/geotorchai/transforms/
+-rw-r--r--   0 kanchan    (501) staff       (20)        0 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/transforms/__init__.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     2891 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/transforms/raster.py
+drwxr-xr-x   0 kanchan    (501) staff       (20)        0 2023-04-10 00:16:03.173810 geotorchai-0.2.0/geotorchai/utility/
+-rw-r--r--   0 kanchan    (501) staff       (20)        0 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/utility/__init__.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     3792 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/utility/_download_utils.py
+-rw-r--r--   0 kanchan    (501) staff       (20)      801 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/utility/exceptions.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     5473 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/utility/method_overload.py
+-rw-r--r--   0 kanchan    (501) staff       (20)      207 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/utility/properties.py
+-rw-r--r--   0 kanchan    (501) staff       (20)       65 2023-04-07 18:27:33.000000 geotorchai-0.2.0/geotorchai/utility/types.py
+drwxr-xr-x   0 kanchan    (501) staff       (20)        0 2023-04-10 00:16:03.165124 geotorchai-0.2.0/geotorchai.egg-info/
+-rw-r--r--   0 kanchan    (501) staff       (20)    11097 2023-04-10 00:16:03.000000 geotorchai-0.2.0/geotorchai.egg-info/PKG-INFO
+-rw-r--r--   0 kanchan    (501) staff       (20)     3079 2023-04-10 00:16:03.000000 geotorchai-0.2.0/geotorchai.egg-info/SOURCES.txt
+-rw-r--r--   0 kanchan    (501) staff       (20)        1 2023-04-10 00:16:03.000000 geotorchai-0.2.0/geotorchai.egg-info/dependency_links.txt
+-rw-r--r--   0 kanchan    (501) staff       (20)      109 2023-04-10 00:16:03.000000 geotorchai-0.2.0/geotorchai.egg-info/requires.txt
+-rw-r--r--   0 kanchan    (501) staff       (20)       17 2023-04-10 00:16:03.000000 geotorchai-0.2.0/geotorchai.egg-info/top_level.txt
+-rw-r--r--   0 kanchan    (501) staff       (20)       38 2023-04-10 00:16:03.176545 geotorchai-0.2.0/setup.cfg
+-rw-r--r--   0 kanchan    (501) staff       (20)     1904 2023-04-10 00:15:47.000000 geotorchai-0.2.0/setup.py
+drwxr-xr-x   0 kanchan    (501) staff       (20)        0 2023-04-10 00:16:03.173998 geotorchai-0.2.0/tests/
+-rw-r--r--   0 kanchan    (501) staff       (20)        0 2023-04-07 18:27:33.000000 geotorchai-0.2.0/tests/__init__.py
+drwxr-xr-x   0 kanchan    (501) staff       (20)        0 2023-04-10 00:16:03.174816 geotorchai-0.2.0/tests/deep-learning/
+-rw-r--r--   0 kanchan    (501) staff       (20)        0 2023-04-07 18:27:33.000000 geotorchai-0.2.0/tests/deep-learning/__init__.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     2377 2023-04-07 18:27:33.000000 geotorchai-0.2.0/tests/deep-learning/test_grid_datasets.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     3541 2023-04-07 18:27:33.000000 geotorchai-0.2.0/tests/deep-learning/test_models.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     1928 2023-04-07 18:27:33.000000 geotorchai-0.2.0/tests/deep-learning/test_raster_datasets.py
+-rw-r--r--   0 kanchan    (501) staff       (20)      890 2023-04-07 18:27:33.000000 geotorchai-0.2.0/tests/deep-learning/test_transforms.py
+drwxr-xr-x   0 kanchan    (501) staff       (20)        0 2023-04-10 00:16:03.176115 geotorchai-0.2.0/tests/preprocessing/
+-rw-r--r--   0 kanchan    (501) staff       (20)        0 2023-04-07 18:27:33.000000 geotorchai-0.2.0/tests/preprocessing/__init__.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     2692 2023-04-07 18:27:33.000000 geotorchai-0.2.0/tests/preprocessing/test_adjacency.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     3081 2023-04-07 18:27:33.000000 geotorchai-0.2.0/tests/preprocessing/test_data_loader.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     2025 2023-04-07 18:27:33.000000 geotorchai-0.2.0/tests/preprocessing/test_feature_aggregation.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     2530 2023-04-07 18:27:33.000000 geotorchai-0.2.0/tests/preprocessing/test_raster_transform.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     3523 2023-04-07 18:27:33.000000 geotorchai-0.2.0/tests/preprocessing/test_space_partition.py
+-rw-r--r--   0 kanchan    (501) staff       (20)     2191 2023-04-07 18:27:33.000000 geotorchai-0.2.0/tests/preprocessing/test_spark_registration.py
+-rw-r--r--   0 kanchan    (501) staff       (20)      166 2023-04-07 18:27:33.000000 geotorchai-0.2.0/tests/preprocessing/utility.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `geotorchai-0.1.0/LICENSE.md` & `geotorchai-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/PKG-INFO` & `geotorchai-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geotorchai
-Version: 0.1.0
+Version: 0.2.0
 Summary: GeoTorchAI, formarly GeoTorch, A Spatiotemporal Deep Learning Framework
 Home-page: https://github.com/DataSystemsLab/GeoTorch
 Author: Kanchan Chowdhury
 Author-email: kchowdh1@asu.edu
 License: AGPL-3.0
 Keywords: spatial-machine-learning,spatiotemporal-deep-learning,spatial forecasting,deep learning,machine learning,spatiotemporal forecasting,temporal signal,raster classification,satellite classification,raster segmentation,satellite segmentation,convlstm,st-resnet,deepstn+,deepsatv2,lstm,temporal network,eurosat,representation learning
 Classifier: Development Status :: 3 - Alpha
@@ -48,27 +48,20 @@
 
 Our preprocessing module is designed such that it minimizes the number of methods and classes in the API. Users can perform end-to-end spatiotemporal data preprocessing, which starts by loading raw datasets and ends by generating a trainable Tensor-shaped array, with a minimum number of method calls. It helps the users understand the API fast and reduces their confusion.
 
 
 ## Documentation
 Details documentation on installation, API, and programming guide is available on [GeoTorchAI Website](https://kanchanchy.github.io/geotorchai/).
 
-## Dependency Set up
-Following libraries need to be set up before using GeoTorchAI.
-
-##### Dependencies for Deep Learning Module:
-1. PyTorch >=1.10
-2. Rasterio
-3. Scikit-image
-
-##### Dependencies for Preprocessing Module:
-1. PySpark >=3.0.0
-2. Apache Sedona >=1.2.0-incubating
-
-For installation, visit the [instructions](https://kanchanchy.github.io/geotorchai/installation.html).
+## Installation
+GeoTorchAI can be installed by running the following command:
+```
+pip install geotorchai
+```
+GeoTorchAI is available on [PyPI](https://pypi.org/project/geotorchai/). For more instructions regrading the required and optional dependencies, please visit the [website](https://kanchanchy.github.io/geotorchai/installation.html).
 
 ## Example
 End-to-end coding examples for various applications including model training and data preprocessing are available in our [binders](https://github.com/DataSystemsLab/GeoTorchAI/tree/main/binders) and [examples](https://github.com/DataSystemsLab/GeoTorchAI/tree/main/examples) sections.
 
 We show a very short example of satellite imagery classification using GeoTorchAI in a step-by-step manner below. Training a satellite imagery classification model consists of three steps: loading the dataset, initializing the model and parameters, and train the model. We pick the [DeepSatV2](https://arxiv.org/abs/1911.07747) model to classify [EuroSAT](https://github.com/phelber/EuroSAT) satellite images.
 #### EuroSAT Image Classes
 * Annual Crop
@@ -84,15 +77,15 @@
 #### Spectral Bands of a Highway Image
 ![Highway Image](https://github.com/DataSystemsLab/GeoTorchAI/blob/main/data/euro-highway.png)
 #### Spectral Bands of an Industry Image
 ![Industry Image](https://github.com/DataSystemsLab/GeoTorchAI/blob/main/data/euro-industry.png)
 #### Loading Training Dataset
 Load the EuroSAT Dataset. Setting download=True will download the full data in the given directory. If data is already available, set download=False.
 ```
-full_data = geotorch.datasets.raser.EuroSAT(root="data/eurosat", download=True, include_additional_features=True)
+full_data = geotorchai.datasets.raser.EuroSAT(root="data/eurosat", download=True, include_additional_features=True)
 ```
 #### Split data into 80% train and 20% validation parts
 ```
 dataset_size = len(full_data)
 indices = list(range(dataset_size))
 split = int(np.floor(0.2 * dataset_size))
 np.random.seed(random_seed)
```

### Comparing `geotorchai-0.1.0/README.md` & `geotorchai-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -26,27 +26,20 @@
 
 Our preprocessing module is designed such that it minimizes the number of methods and classes in the API. Users can perform end-to-end spatiotemporal data preprocessing, which starts by loading raw datasets and ends by generating a trainable Tensor-shaped array, with a minimum number of method calls. It helps the users understand the API fast and reduces their confusion.
 
 
 ## Documentation
 Details documentation on installation, API, and programming guide is available on [GeoTorchAI Website](https://kanchanchy.github.io/geotorchai/).
 
-## Dependency Set up
-Following libraries need to be set up before using GeoTorchAI.
-
-##### Dependencies for Deep Learning Module:
-1. PyTorch >=1.10
-2. Rasterio
-3. Scikit-image
-
-##### Dependencies for Preprocessing Module:
-1. PySpark >=3.0.0
-2. Apache Sedona >=1.2.0-incubating
-
-For installation, visit the [instructions](https://kanchanchy.github.io/geotorchai/installation.html).
+## Installation
+GeoTorchAI can be installed by running the following command:
+```
+pip install geotorchai
+```
+GeoTorchAI is available on [PyPI](https://pypi.org/project/geotorchai/). For more instructions regrading the required and optional dependencies, please visit the [website](https://kanchanchy.github.io/geotorchai/installation.html).
 
 ## Example
 End-to-end coding examples for various applications including model training and data preprocessing are available in our [binders](https://github.com/DataSystemsLab/GeoTorchAI/tree/main/binders) and [examples](https://github.com/DataSystemsLab/GeoTorchAI/tree/main/examples) sections.
 
 We show a very short example of satellite imagery classification using GeoTorchAI in a step-by-step manner below. Training a satellite imagery classification model consists of three steps: loading the dataset, initializing the model and parameters, and train the model. We pick the [DeepSatV2](https://arxiv.org/abs/1911.07747) model to classify [EuroSAT](https://github.com/phelber/EuroSAT) satellite images.
 #### EuroSAT Image Classes
 * Annual Crop
@@ -62,15 +55,15 @@
 #### Spectral Bands of a Highway Image
 ![Highway Image](https://github.com/DataSystemsLab/GeoTorchAI/blob/main/data/euro-highway.png)
 #### Spectral Bands of an Industry Image
 ![Industry Image](https://github.com/DataSystemsLab/GeoTorchAI/blob/main/data/euro-industry.png)
 #### Loading Training Dataset
 Load the EuroSAT Dataset. Setting download=True will download the full data in the given directory. If data is already available, set download=False.
 ```
-full_data = geotorch.datasets.raser.EuroSAT(root="data/eurosat", download=True, include_additional_features=True)
+full_data = geotorchai.datasets.raser.EuroSAT(root="data/eurosat", download=True, include_additional_features=True)
 ```
 #### Split data into 80% train and 20% validation parts
 ```
 dataset_size = len(full_data)
 indices = list(range(dataset_size))
 split = int(np.floor(0.2 * dataset_size))
 np.random.seed(random_seed)
```

### Comparing `geotorchai-0.1.0/geotorchai/datasets/grid/nyc_bike_deepstn.py` & `geotorchai-0.2.0/geotorchai/datasets/grid/nyc_bike_deepstn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import os
-import numpy as np
 import torch
 from torch.utils.data import Dataset
 from geotorchai.utility.exceptions import InvalidParametersException
 from geotorchai.utility._download_utils import _download_remote_file
+import numpy as np
 
 
 class BikeNYCDeepSTN(Dataset):
     '''
     This dataset is based on https://github.com/FIBLAB/DeepSTN/tree/master/BikeNYC/DATA
     Grid map_height and map_width = 21 and 12
 
@@ -25,95 +25,117 @@
     T_period (Int, Optional) - Period length of T_data. Default: 24
     T_trend (Int, Optional) - Trend length of T_data. Default: 24*7
     '''
 
     DATA_URL = "https://raw.githubusercontent.com/FIBLAB/DeepSTN/master/BikeNYC/DATA/dataBikeNYC/flow_data.npy"
     POI_URL = "https://raw.githubusercontent.com/FIBLAB/DeepSTN/master/BikeNYC/DATA/dataBikeNYC/poi_data.npy"
 
-    def __init__(self, root, download = False, is_training_data=True, test_ratio = 0.1, len_closeness = 3, len_period = 4, len_trend = 4, T_closeness=1, T_period=24, T_trend=24*7):
+    def __init__(self, root, download = False, len_closeness = 3, len_period = 4, len_trend = 4, T_closeness=1, T_period=24, T_trend=24*7, normalize=True):
         super().__init__()
-        self.is_training_data = is_training_data
 
         if download:
             _download_remote_file(self.DATA_URL, root)
             _download_remote_file(self.POI_URL, root)
 
         data_dir = self._get_path(root)
 
         flow_data = np.load(open(data_dir + "/flow_data.npy", "rb"))
         poi_data = np.load(open(data_dir + "/poi_data.npy", "rb"))
 
-        self.len_test  = int(np.floor(test_ratio * len(flow_data)))
-        self.merged_data = np.copy(flow_data)
-        self.is_merged = False
+        self.full_data = np.copy(flow_data)
 
-        self._create_feature_vector(flow_data, poi_data, len_closeness, len_period, len_trend, T_closeness, T_period, T_trend)
+        max_data = np.max(self.full_data)
+        min_data = np.min(self.full_data)
+        self.min_max_diff = max_data - min_data
+        if normalize:
+            self.full_data = (2.0 * self.full_data - (max_data + min_data)) / (max_data - min_data)
+
+        self._create_feature_vector(self.full_data, poi_data, len_closeness, len_period, len_trend, T_closeness, T_period, T_trend)
+
+        self.use_lead_time = False
+        self.sequential = False
+        self.periodical = True
 
 
 
     ## This method returns the difference between maximum and minimum values of this dataset
     def get_min_max_difference(self):
         return self.min_max_diff
 
 
-    def merge_closeness_period_trend(self, history_length, predict_length):
+    def set_sequential_representation(self, history_length, prediction_length):
         '''
         Call this method if you want to iterate the dataset as a sequence of histories and predictions instead of closeness, period, and trend.
 
         Parameters
         ..........
         history_length (Int) - Length of history data in sequence of each sample
         predict_length (Int) - Length of prediction data in sequence of each sample
         '''
 
-        max_data = np.max(self.merged_data)
-        min_data = np.min(self.merged_data)
-        self.min_max_diff = max_data-min_data
-        self.merged_data=(2.0*self.merged_data-(max_data+min_data))/(max_data-min_data)
-
         history_data = []
         predict_data = []
-        total_length = self.merged_data.shape[0]
-        for end_idx in range(history_length + predict_length, total_length):
-            predict_frames = self.merged_data[end_idx-predict_length:end_idx]
-            history_frames = self.merged_data[end_idx-predict_length-history_length:end_idx-predict_length]
+        total_length = self.full_data.shape[0]
+        for end_idx in range(history_length + prediction_length, total_length):
+            predict_frames = self.full_data[end_idx-prediction_length:end_idx]
+            history_frames = self.full_data[end_idx-prediction_length-history_length:end_idx-prediction_length]
             history_data.append(history_frames)
             predict_data.append(predict_frames)
         history_data = np.stack(history_data)
         predict_data = np.stack(predict_data)
 
-        if self.is_training_data:
-            self.X_data = history_data[:-self.len_test]
-            self.Y_data = predict_data[:-self.len_test]
-        else:
-            self.X_data = history_data[-self.len_test:]
-            self.Y_data = predict_data[-self.len_test:]
+        self.X_data = torch.tensor(history_data)
+        self.Y_data = torch.tensor(predict_data)
 
-        self.X_data = torch.tensor(self.X_data)
-        self.Y_data = torch.tensor(self.Y_data)
+        self.use_lead_time = False
+        self.sequential = True
+        self.periodical = False
 
-        self.is_merged = True
+
+    def merge_closeness_period_trend(self, lead_time = 2*24):
+        '''
+        Call this method if you want to iterate the dataset as a sequence of histories and predictions instead of closeness, period, and trend.
+
+        Parameters
+        ..........
+        history_length (Int) - Length of history data in sequence of each sample
+        predict_length (Int) - Length of prediction data in sequence of each sample
+        '''
+
+        self.lead_time_data = torch.tensor(self.full_data)
+        self.lead_time = lead_time
+        self.use_lead_time = True
+        self.sequential = False
+        self.periodical = False
 
 
     def __len__(self) -> int:
-        return len(self.Y_data)
+        if self.use_lead_time:
+            return len(self.lead_time_data) - self.lead_time
+        else:
+            return len(self.Y_data)
 
 
     def __getitem__(self, index: int):
 
-        if self.is_merged:
-            sample = {"x_data": self.X_data[index], \
-            "y_data": self.Y_data[index]}
-        else:
+        if self.periodical:
             sample = {"x_closeness": self.X_closeness[index], \
-            "x_period": self.X_period[index], \
-            "x_trend": self.X_trend[index], \
-            "t_data": self.T_data[index], \
-            "p_data": self.P_data[index], \
-            "y_data": self.Y_data[index]}
+                      "x_period": self.X_period[index], \
+                      "x_trend": self.X_trend[index], \
+                      "t_data": self.T_data[index], \
+                      "p_data": self.P_data[index], \
+                      "y_data": self.Y_data[index]}
+        else:
+            if self.use_lead_time:
+                x_data = self.lead_time_data[index]
+                y_data = self.lead_time_data[index + self.lead_time]
+            else:
+                x_data = self.X_data[index]
+                y_data = self.Y_data[index]
+            sample = {"x_data": x_data, "y_data": y_data}
 
         return sample
 
 
     def _get_path(self, root_dir):
         queue = [root_dir]
         while queue:
@@ -127,33 +149,28 @@
                     queue.append(data_dir + "/" + folder)
 
         return None
 
 
     # This is replication of lzq_load_data method proposed by authors here: https://github.com/FIBLAB/DeepSTN/blob/master/BikeNYC/DATA/lzq_read_data_time_poi.py
     def _create_feature_vector(self, all_data, poi, len_closeness, len_period, len_trend, T_closeness, T_period, T_trend):
-        max_data = np.max(all_data)
-        min_data = np.min(all_data)
-        self.min_max_diff = max_data-min_data
-
         len_total,feature,map_height,map_width = all_data.shape
 
         time=np.arange(len_total,dtype=int)
         time_hour=time%T_period
         matrix_hour=np.zeros([len_total,24,map_height,map_width])
         for i in range(len_total):
             matrix_hour[i,time_hour[i],:,:]=1
 
         time_day=(time//T_period)%7
         matrix_day=np.zeros([len_total,7,map_height,map_width])
         for i in range(len_total):
             matrix_day[i,time_day[i],:,:]=1
 
         matrix_T=np.concatenate((matrix_hour,matrix_day),axis=1)
-        all_data=(2.0*all_data-(max_data+min_data))/(max_data-min_data)
 
         if len_trend>0:
             number_of_skip_hours=T_trend*len_trend
         elif len_period>0:
             number_of_skip_hours=T_period*len_period
         elif len_closeness>0:
             number_of_skip_hours=T_closeness*len_closeness
@@ -173,28 +190,16 @@
         if len_trend>0:
             self.X_trend=all_data[number_of_skip_hours-T_trend:len_total-T_trend]
             for i in range(len_trend-1):
                 self.X_trend=np.concatenate((self.X_trend,all_data[number_of_skip_hours-T_trend*(2+i):len_total-T_trend*(2+i)]),axis=1)
 
         matrix_T=matrix_T[number_of_skip_hours:]
 
-        if self.is_training_data:
-            self.X_closeness=self.X_closeness[:-self.len_test]
-            self.X_period=self.X_period[:-self.len_test]
-            self.X_trend=self.X_trend[:-self.len_test]
-            self.T_data=matrix_T[:-self.len_test]
-
-            self.Y_data=Y[:-self.len_test]
-        else:
-            self.X_closeness=self.X_closeness[-self.len_test:]
-            self.X_period=self.X_period[-self.len_test:]
-            self.X_trend=self.X_trend[-self.len_test:]
-            self.T_data=matrix_T[-self.len_test:]
-
-            self.Y_data=Y[-self.len_test:]
+        self.T_data = matrix_T
+        self.Y_data = Y
 
         len_data=self.X_closeness.shape[0]
 
         for i in range(poi.shape[0]):
             poi[i]=poi[i]/np.max(poi[i])
         self.P_data=np.repeat(poi.reshape(1,poi.shape[0],map_height,map_width),len_data,axis=0)
```

### Comparing `geotorchai-0.1.0/geotorchai/datasets/grid/nyc_bike_stdn.py` & `geotorchai-0.2.0/geotorchai/datasets/grid/nyc_bike_stdn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 
 import os
-import numpy as np
 import torch
-from torch import Tensor
 from torch.utils.data import Dataset
 from geotorchai.utility._download_utils import _download_remote_file, _extract_archive
+import numpy as np
 
 
 class BikeNYCSTDN(Dataset):
     '''
     This dataset is based on https://github.com/tangxianfeng/STDN/blob/master/file_loader.py
     Grid map_height and map_width = 10 and 20
```

### Comparing `geotorchai-0.1.0/geotorchai/datasets/grid/nyc_taxi_stdn.py` & `geotorchai-0.2.0/geotorchai/datasets/grid/nyc_taxi_stdn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 
 import os
-import numpy as np
 import torch
-from torch import Tensor
 from torch.utils.data import Dataset
 from geotorchai.utility._download_utils import _download_remote_file, _extract_archive
+import numpy as np
 
 
 class TaxiNYCSTDN(Dataset):
     '''
     This dataset is based on https://github.com/tangxianfeng/STDN/blob/master/file_loader.py
     Grid map_height and map_width = 10 and 20
```

### Comparing `geotorchai-0.1.0/geotorchai/datasets/grid/processed.py` & `geotorchai-0.2.0/geotorchai/datasets/grid/processed.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 
-import os
-import numpy as np
 import torch
 from torch.utils.data import Dataset
 from geotorchai.utility.exceptions import InvalidParametersException
+import numpy as np
 
 
 class Processed(Dataset):
     '''
     This dataset is used load a grid-based spatiotemporal tensor/dataset that is created through GeoTorch Preprocessing module or any other means.
     The tensor created through the preprocessing steps should available as an npy file of shape: TxCxHxW
     T => total number of timesteps, C => number of channels/features, H => Grid Height, W => Grid Width.
@@ -21,113 +20,122 @@
     len_period (Int, Optional) - Length of period. Default: 4
     len_trend (Int, Optional) - Length of trend. Default: 4
     T_closeness (Int, Optional) - Closeness length of T_data. Default: 1
     T_period (Int, Optional) - Period length of T_data. Default: 24
     T_trend (Int, Optional) - Trend length of T_data. Default: 24*7
     '''
 
-    def __init__(self, root, is_training_data=True, test_ratio = 0.1, len_closeness = 3, len_period = 4, len_trend = 4, T_closeness=1, T_period=24, T_trend=24*7):
+    def __init__(self, root, lead_time = 2*24, normalize=True):
         super().__init__()
-        self.is_training_data = is_training_data
 
-        st_data = np.load(open(root, "rb"))
+        self.full_data = np.load(open(root, "rb"))
+        self.normalize = normalize
 
-        self.len_test  = int(np.floor(test_ratio * len(st_data)))
-        self.merged_data = np.copy(st_data)
-        self.is_merged = False
-
-        self._create_feature_vector(st_data, len_closeness, len_period, len_trend, T_closeness, T_period, T_trend)
+        max_data = np.max(self.full_data)
+        min_data = np.min(self.full_data)
+        self.min_max_diff = max_data - min_data
+        if normalize:
+            self.full_data = (2.0 * self.full_data - (max_data + min_data)) / (max_data - min_data)
+
+        self.lead_time_data = torch.tensor(self.full_data)
+
+        self.lead_time = lead_time
+        self.use_lead_time = True
+        self.sequential = False
+        self.periodical = False
         
 
 
     ## This method returns the difference between maximum and minimum values of this dataset
     def get_min_max_difference(self):
         return self.min_max_diff
 
 
-    def merge_closeness_period_trend(self, history_length, predict_length):
+    def set_sequential_representation(self, history_length, predict_length):
         '''
         Call this method if you want to iterate the dataset as a sequence of histories and predictions instead of closeness, period, and trend.
 
         Parameters
         ..........
         history_length (Int) - Length of history data in sequence of each sample
         predict_length (Int) - Length of prediction data in sequence of each sample
         '''
 
-        max_data = np.max(self.merged_data)
-        min_data = np.min(self.merged_data)
-        self.min_max_diff = max_data-min_data
-        self.merged_data=(2.0*self.merged_data-(max_data+min_data))/(max_data-min_data)
-
         history_data = []
         predict_data = []
-        total_length = self.merged_data.shape[0]
+        total_length = self.full_data.shape[0]
         for end_idx in range(history_length + predict_length, total_length):
-            predict_frames = self.merged_data[end_idx-predict_length:end_idx]
-            history_frames = self.merged_data[end_idx-predict_length-history_length:end_idx-predict_length]
+            predict_frames = self.full_data[end_idx-predict_length:end_idx]
+            history_frames = self.full_data[end_idx-predict_length-history_length:end_idx-predict_length]
             history_data.append(history_frames)
             predict_data.append(predict_frames)
         history_data = np.stack(history_data)
         predict_data = np.stack(predict_data)
 
-        if self.is_training_data:
-            self.X_data = history_data[:-self.len_test]
-            self.Y_data = predict_data[:-self.len_test]
-        else:
-            self.X_data = history_data[-self.len_test:]
-            self.Y_data = predict_data[-self.len_test:]
+        self.X_data = torch.tensor(history_data)
+        self.Y_data = torch.tensor(predict_data)
+
+        self.use_lead_time = False
+        self.sequential = True
+        self.periodical = False
+
 
-        self.X_data = torch.tensor(self.X_data)
-        self.Y_data = torch.tensor(self.Y_data)
 
-        self.is_merged = True
+    def set_periodical_representation(self, len_closeness = 3, len_period = 4, len_trend = 4, T_closeness=1, T_period=24, T_trend=24*7):
+        self._create_feature_vector(self.full_data, len_closeness, len_period, len_trend, T_closeness, T_period,
+                                    T_trend)
+        self.use_lead_time = False
+        self.sequential = False
+        self.periodical = True
 
 
     def __len__(self) -> int:
-        return len(self.Y_data)
+        if self.use_lead_time:
+            return len(self.lead_time_data) - self.lead_time
+        else:
+            return len(self.Y_data)
 
 
     def __getitem__(self, index: int):
 
-        if self.is_merged:
-            sample = {"x_data": self.X_data[index], \
-            "y_data": self.Y_data[index]}
-        else:
+        if self.periodical:
             sample = {"x_closeness": self.X_closeness[index], \
-            "x_period": self.X_period[index], \
-            "x_trend": self.X_trend[index], \
-            "t_data": self.T_data[index], \
-            "y_data": self.Y_data[index]}
+                      "x_period": self.X_period[index], \
+                      "x_trend": self.X_trend[index], \
+                      "t_data": self.T_data[index], \
+                      "y_data": self.Y_data[index]}
+        else:
+            if self.use_lead_time:
+                x_data = self.lead_time_data[index]
+                y_data = self.lead_time_data[index + self.lead_time]
+            else:
+                x_data = self.X_data[index]
+                y_data = self.Y_data[index]
+            sample = {"x_data": x_data, "y_data": y_data}
 
         return sample
 
 
 
     # This is replication of lzq_load_data method proposed by authors here: https://github.com/FIBLAB/DeepSTN/blob/master/BikeNYC/DATA/lzq_read_data_time_poi.py
     def _create_feature_vector(self, all_data, len_closeness, len_period, len_trend, T_closeness, T_period, T_trend):
-        max_data = np.max(all_data)
-        min_data = np.min(all_data)
-        self.min_max_diff = max_data-min_data
-
         len_total,feature,map_height,map_width = all_data.shape
 
         time=np.arange(len_total,dtype=int)
         time_hour=time%T_period
         matrix_hour=np.zeros([len_total,24,map_height,map_width])
         for i in range(len_total):
             matrix_hour[i,time_hour[i],:,:]=1
 
         time_day=(time//T_period)%7
         matrix_day=np.zeros([len_total,7,map_height,map_width])
         for i in range(len_total):
             matrix_day[i,time_day[i],:,:]=1
 
         matrix_T=np.concatenate((matrix_hour,matrix_day),axis=1)
-        all_data=(2.0*all_data-(max_data+min_data))/(max_data-min_data)
 
         if len_trend>0:
             number_of_skip_hours=T_trend*len_trend
         elif len_period>0:
             number_of_skip_hours=T_period*len_period
         elif len_closeness>0:
             number_of_skip_hours=T_closeness*len_closeness
@@ -147,30 +155,16 @@
         if len_trend>0:
             self.X_trend=all_data[number_of_skip_hours-T_trend:len_total-T_trend]
             for i in range(len_trend-1):
                 self.X_trend=np.concatenate((self.X_trend,all_data[number_of_skip_hours-T_trend*(2+i):len_total-T_trend*(2+i)]),axis=1)
 
         matrix_T=matrix_T[number_of_skip_hours:]
 
-        if self.is_training_data:
-            self.X_closeness=self.X_closeness[:-self.len_test]
-            self.X_period=self.X_period[:-self.len_test]
-            self.X_trend=self.X_trend[:-self.len_test]
-            self.T_data=matrix_T[:-self.len_test]
-
-            self.Y_data=Y[:-self.len_test]
-        else:
-            self.X_closeness=self.X_closeness[-self.len_test:]
-            self.X_period=self.X_period[-self.len_test:]
-            self.X_trend=self.X_trend[-self.len_test:]
-            self.T_data=matrix_T[-self.len_test:]
-
-            self.Y_data=Y[-self.len_test:]
-
-        len_data=self.X_closeness.shape[0]
+        self.T_data = matrix_T
+        self.Y_data = Y
 
         self.X_closeness = torch.tensor(self.X_closeness)
         self.X_period = torch.tensor(self.X_period)
         self.X_trend = torch.tensor(self.X_trend)
         self.T_data = torch.tensor(self.T_data)
         self.Y_data = torch.tensor(self.Y_data)
```

### Comparing `geotorchai-0.1.0/geotorchai/datasets/grid/taxi_bj_21.py` & `geotorchai-0.2.0/geotorchai/datasets/grid/taxi_bj_21.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 
 import os
-import numpy as np
 import torch
-from torch import Tensor
 from torch.utils.data import Dataset
 from geotorchai.utility.exceptions import InvalidParametersException
 from geotorchai.utility._download_utils import _download_remote_file
+import numpy as np
 
 
 class TaxiBJ21(Dataset):
     '''
     This dataset is based on https://github.com/jwwthu/DL4Traffic/tree/main/TaxiBJ21
     Grid map_height and map_width = 32 and 32
 
@@ -25,88 +24,97 @@
     T_closeness (Int, Optional) - Closeness length of T_data. Default: 1
     T_period (Int, Optional) - Period length of T_data. Default: 24
     T_trend (Int, Optional) - Trend length of T_data. Default: 24*7
     '''
 
     DATA_URL = "https://raw.githubusercontent.com/jwwthu/DL4Traffic/main/TaxiBJ21/TaxiBJ21.npy"
 
-    def __init__(self, root, download=False, is_training_data=True, test_ratio = 0.1, len_closeness = 3, len_period = 4, len_trend = 4, T_closeness=1, T_period=24, T_trend=24*7):
+    def __init__(self, root, download=False, lead_time = 2*24):
         super().__init__()
-        self.is_training_data = is_training_data
 
         if download:
             _download_remote_file(self.DATA_URL, root)
 
         data_dir = self._get_path(root)
 
         flow_data = np.load(open(data_dir + "/TaxiBJ21.npy", "rb"))
 
-        self.len_test = int(np.floor(test_ratio * len(flow_data)))
-        self.merged_data = np.copy(flow_data)
-        self.is_merged = False
+        self.full_data = np.copy(flow_data)
 
-        self._create_feature_vector(flow_data, len_closeness, len_period, len_trend, T_closeness, T_period, T_trend)
+        self.lead_time = lead_time
+        self.use_lead_time = True
+        self.sequential = False
+        self.periodical = False
 
+        self.lead_time_data = torch.tensor(self.full_data)
 
 
-    def merge_closeness_period_trend(self, history_length, predict_length):
+
+    def set_sequential_representation(self, history_length, prediction_length):
         '''
         Call this method if you want to iterate the dataset as a sequence of histories and predictions instead of closeness, period, and trend.
 
         Parameters
         ..........
         history_length (Int) - Length of history data in sequence of each sample
-        predict_length (Int) - Length of prediction data in sequence of each sample
+        prediction_length (Int) - Length of prediction data in sequence of each sample
         '''
 
-        max_data = np.max(self.merged_data)
-        min_data = np.min(self.merged_data)
-        self.min_max_diff = max_data-min_data
-        self.merged_data=(2.0*self.merged_data-(max_data+min_data))/(max_data-min_data)
-
         history_data = []
         predict_data = []
-        total_length = self.merged_data.shape[0]
-        for end_idx in range(history_length + predict_length, total_length):
-            predict_frames = self.merged_data[end_idx-predict_length:end_idx]
-            history_frames = self.merged_data[end_idx-predict_length-history_length:end_idx-predict_length]
+        total_length = self.full_data.shape[0]
+        for end_idx in range(history_length + prediction_length, total_length):
+            predict_frames = self.full_data[end_idx-prediction_length:end_idx]
+            history_frames = self.full_data[end_idx-prediction_length-history_length:end_idx-prediction_length]
             history_data.append(history_frames)
             predict_data.append(predict_frames)
         history_data = np.stack(history_data)
         predict_data = np.stack(predict_data)
 
-        if self.is_training_data:
-            self.X_data = history_data[:-self.len_test]
-            self.Y_data = predict_data[:-self.len_test]
-        else:
-            self.X_data = history_data[-self.len_test:]
-            self.Y_data = predict_data[-self.len_test:]
+        self.X_data = torch.tensor(history_data)
+        self.Y_data = torch.tensor(predict_data)
+
+        self.use_lead_time = False
+        self.sequential = True
+        self.periodical = False
+
 
-        self.X_data = torch.tensor(self.X_data)
-        self.Y_data = torch.tensor(self.Y_data)
 
-        self.is_merged = True
+    def set_periodical_representation(self, len_closeness = 3, len_period = 4, len_trend = 4, T_closeness=1, T_period=24, T_trend=24*7):
+        self._create_feature_vector(self.full_data, len_closeness, len_period, len_trend, T_closeness, T_period,
+                                    T_trend)
+        self.use_lead_time = False
+        self.sequential = False
+        self.periodical = True
         
 
 
     def __len__(self) -> int:
-        return len(self.Y_data)
+        if self.use_lead_time:
+            return len(self.lead_time_data) - self.lead_time
+        else:
+            return len(self.Y_data)
 
 
     def __getitem__(self, index: int):
 
-        if self.is_merged:
-            sample = {"x_data": self.X_data[index], \
-            "y_data": self.Y_data[index]}
-        else:
+        if self.periodical:
             sample = {"x_closeness": self.X_closeness[index], \
-            "x_period": self.X_period[index], \
-            "x_trend": self.X_trend[index], \
-            "t_data": self.T_data[index], \
-            "y_data": self.Y_data[index]}
+                      "x_period": self.X_period[index], \
+                      "x_trend": self.X_trend[index], \
+                      "t_data": self.T_data[index], \
+                      "y_data": self.Y_data[index]}
+        else:
+            if self.use_lead_time:
+                x_data = self.lead_time_data[index]
+                y_data = self.lead_time_data[index + self.lead_time]
+            else:
+                x_data = self.X_data[index]
+                y_data = self.Y_data[index]
+            sample = {"x_data": x_data, "y_data": y_data}
 
         return sample
 
 
     def _get_path(self, root_dir):
         queue = [root_dir]
         while queue:
@@ -161,31 +169,16 @@
         if len_trend>0:
             self.X_trend=all_data[number_of_skip_hours-T_trend:len_total-T_trend]
             for i in range(len_trend-1):
                 self.X_trend=np.concatenate((self.X_trend,all_data[number_of_skip_hours-T_trend*(2+i):len_total-T_trend*(2+i)]),axis=1)
 
         matrix_T=matrix_T[number_of_skip_hours:]
 
-        if self.is_training_data:
-            self.X_closeness=self.X_closeness[:-self.len_test]
-            self.X_period=self.X_period[:-self.len_test]
-            self.X_trend=self.X_trend[:-self.len_test]
-            self.T_data=matrix_T[:-self.len_test]
-
-            self.Y_data=Y[:-self.len_test]
-        else:
-            self.X_closeness=self.X_closeness[-self.len_test:]
-            self.X_period=self.X_period[-self.len_test:]
-            self.X_trend=self.X_trend[-self.len_test:]
-            self.T_data=matrix_T[-self.len_test:]
-
-            self.Y_data=Y[-self.len_test:]
-
-
-        len_data=self.X_closeness.shape[0]
+        self.T_data = matrix_T
+        self.Y_data = Y
 
         self.X_closeness = torch.tensor(self.X_closeness)
         self.X_period = torch.tensor(self.X_period)
         self.X_trend = torch.tensor(self.X_trend)
         self.T_data = torch.tensor(self.T_data)
         self.Y_data = torch.tensor(self.Y_data)
```

### Comparing `geotorchai-0.1.0/geotorchai/datasets/raster/cloud_38.py` & `geotorchai-0.2.0/geotorchai/datasets/raster/cloud_38.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 
 import os
 from typing import Optional, Callable
-import numpy as np
 import torch
-from torch import Tensor
 from torch.utils.data import Dataset
-from kaggle.api.kaggle_api_extended import KaggleApi
-import rasterio
 from geotorchai.utility.exceptions import InvalidParametersException
-from geotorchai.utility._download_utils import _extract_archive
+import numpy as np
+import rasterio
 
 
 class Cloud38(Dataset):
 	'''
     This is a segmentation dtaaset. Link: https://www.kaggle.com/datasets/sorour/38cloud-cloud-segmentation-in-satellite-images
     Image Height and Width: 384 x 384, No of bands: 4
 
@@ -25,31 +22,25 @@
     target_transform (Callable, Optional) - Tranforms to apply to each label. Default: None
     '''
 
 
 	SPECTRAL_BANDS = ["red", "green", "blue", "nir"]
 	RGB_BANDS = ["red", "green", "blue"]
 
-	def __init__(self, root, download = False, bands = SPECTRAL_BANDS, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None):
+	def __init__(self, root, bands = SPECTRAL_BANDS, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None):
 		super().__init__()
 		# first check if selected bands are valid. Trow exception otherwise
 		if not self._is_valid_bands(bands):
 			raise InvalidParametersException("Invalid band names")
 
 		self.selected_band_indices = torch.tensor([self.SPECTRAL_BANDS.index(band) for band in bands])
 		self.transform = transform
 		self.target_transform = target_transform
 		self.image_paths = []
 
-		if download:
-			api = KaggleApi()
-			api.authenticate()
-			api.dataset_download_files('sorour/38cloud-cloud-segmentation-in-satellite-images', root)
-			_extract_archive(root + "/38cloud-cloud-segmentation-in-satellite-images.zip", root + "/38cloud-cloud-segmentation-in-satellite-images")
-
 		image_folders = ["train_red", "train_green", "train_blue", "train_nir"]
 		label_folder = "train_gt"
 		data_dir = self._get_path(root)
 		band_indices = self.selected_band_indices.numpy()
 		folder_band_1 = data_dir + "/" + image_folders[band_indices[0]]
 		files = os.listdir(folder_band_1)
 		for i in range(len(files)):
```

### Comparing `geotorchai-0.1.0/geotorchai/datasets/raster/euro_sat.py` & `geotorchai-0.2.0/geotorchai/datasets/raster/euro_sat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 
 import os
 from typing import Optional, Callable, Dict
-import numpy as np
-import rasterio
 import torch
-from torch import Tensor
 from torch.utils.data import Dataset
-import pandas as pd
 from geotorchai.datasets.raster.utility import textural_features as ttf
 from geotorchai.datasets.raster.utility import spectral_indices as si
 from geotorchai.utility.exceptions import InvalidParametersException
 from geotorchai.utility._download_utils import _download_remote_file, _extract_archive
+import numpy as np
+import rasterio
 
 
 class EuroSAT(Dataset):
 	'''
     This is a multi-class classification dtaaset. Link: https://github.com/phelber/EuroSAT
     Image Height and Width: 64 x 64, No of bands: 13, No of classes: 10
```

### Comparing `geotorchai-0.1.0/geotorchai/datasets/raster/processed.py` & `geotorchai-0.2.0/geotorchai/datasets/raster/processed.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 
 import os
 from typing import Optional, Callable
-import numpy as np
-import rasterio
 import torch
-from torch import Tensor
 from torch.utils.data import Dataset
-import pandas as pd
+import numpy as np
+import rasterio
 
 
 class Processed(Dataset):
 	'''
     This dataset is a custom dataset which can be used for any preprocessed raster image data. Datasets that are not preprocessed
     can also be used to create a custom PyTorch dataset with this class. All raster images should be put inside multiple folders
     where each folder represents a class. All folders representing classes should be located inside a root folder.
```

### Comparing `geotorchai-0.1.0/geotorchai/datasets/raster/processed_extra_features.py` & `geotorchai-0.2.0/geotorchai/datasets/raster/processed_extra_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 
-import os
 from typing import Optional, Callable
+import torch
+from torch.utils.data import Dataset
 import numpy as np
 import pandas as pd
 import rasterio
-import torch
-from torch import Tensor
-from torch.utils.data import Dataset
 
 
 class ProcessedWithExtraFeatures(Dataset):
 	'''
     This dataset is a custom dataset which is exactly similar to Processed dataset with the only exception that users can include
     pre-extracted additional features similar to the EuroSAT. The difference with EuroSAT is that, here, users need to extract
     the features beforehand and save to a CSV file. The CSV file should include more than two column: one column contains the path
```

### Comparing `geotorchai-0.1.0/geotorchai/datasets/raster/sat4.py` & `geotorchai-0.2.0/geotorchai/datasets/raster/sat6.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 
 import os
 from typing import Optional, Callable, Dict
-import pandas as pd
-import numpy as np
-import rasterio
 import torch
-from torch import Tensor
 from torch.utils.data import Dataset
-from kaggle.api.kaggle_api_extended import KaggleApi
 from geotorchai.datasets.raster.utility import textural_features as ttf
 from geotorchai.datasets.raster.utility import spectral_indices as si
 from geotorchai.utility.exceptions import InvalidParametersException
-from geotorchai.utility._download_utils import _extract_archive
+import pandas as pd
+import numpy as np
 
 
-class SAT4(Dataset):
+class SAT6(Dataset):
 	'''
-    This is a multi-class classification dtaaset. Link: https://www.kaggle.com/datasets/crawford/deepsat-sat4
-    Image Height and Width: 28 x 28, No of bands: 4, No of classes: 4
+    This is a multi-class classification dtaaset. Link: https://www.kaggle.com/datasets/crawford/deepsat-sat6
+    Image Height and Width: 28 x 28, No of bands: 4, No of classes: 6
 
     Parameters
     ..........
     root (String) - Path to the dataset if it is already downloaded. If not downloaded, it will be downloaded in the given path.
     download (Boolean, Optional) - Set to True if dataset is not available in the given directory. Default: False
     is_train_data (Boolean, Optional) - True denotes training data, while False indicates testing data. Default: True
     bands (List, Optional) - List of all bands that need to be included in the dataset. Default: list of all bands in the EuroSAT images.
@@ -37,60 +33,54 @@
 
 
 	SPECTRAL_BANDS = ["red", "green", "blue", "nir"]
 	RGB_BANDS = ["red", "green", "blue"]
 	ADDITIONAL_FEATURES = ["contrast", "dissimilarity", "homogeneity", "energy", "correlation", "ASM", "mean_NDWI", "mean_NDVI", "mean_RVI"]
 	TEXTURAL_FEATURES = ["contrast", "dissimilarity", "homogeneity", "energy", "correlation", "ASM"]
 	SPECTRAL_INDICES = ["mean_NDWI", "mean_NDVI", "mean_RVI"]
-	SAT4_CLASSES = ["barren_land", "trees", "grassland", "none"]
+	SAT6_CLASSES = ["building", "barren_land", "trees", "grassland", "road", "water"]
 	
 	IMAGE_HEIGHT = 28
 	IMAGE_WIDTH = 28
 	BAND_GREEN_INDEX = 1
 	BAND_RED_INDEX = 0
 	BAND_NIR_INDEX = 3
 
 
-	def __init__(self, root, download = False, is_train_data = True, bands = SPECTRAL_BANDS, include_additional_features = False, additional_features_list = ADDITIONAL_FEATURES, user_features_callback: Optional[Dict[str, Callable]] = None, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None):
+	def __init__(self, root, is_train_data = True, bands = SPECTRAL_BANDS, include_additional_features = False, additional_features_list = ADDITIONAL_FEATURES, user_features_callback: Optional[Dict[str, Callable]] = None, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None):
 		super().__init__()
 		# first check if selected bands are valid. Trow exception otherwise
 		if not self._is_valid_bands(bands):
 			raise InvalidParametersException("Invalid band names")
 
 		self._feature_callbacks = [ttf._get_GLCM_Contrast, ttf._get_GLCM_Dissimilarity, ttf._get_GLCM_Homogeneity, ttf._get_GLCM_Energy, ttf._get_GLCM_Correlation, ttf._get_GLCM_ASM]
 
 		self.selected_band_indices = torch.tensor([self.SPECTRAL_BANDS.index(band) for band in bands])
 		self.user_features_callback = user_features_callback
 		self.transform = transform
 		self.target_transform = target_transform
 
-		self._idx_to_class = {i:j for i, j in enumerate(self.SAT4_CLASSES)}
+		self._idx_to_class = {i:j for i, j in enumerate(self.SAT6_CLASSES)}
 		self._class_to_idx = {value:key for key, value in self._idx_to_class.items()}
 		self._rgb_band_indices = torch.tensor([self.SPECTRAL_BANDS.index(band) for band in self.RGB_BANDS])
 
-		if download:
-			api = KaggleApi()
-			api.authenticate()
-			api.dataset_download_files('crawford/deepsat-sat4', root)
-			_extract_archive(root + "/deepsat-sat4.zip", root + "/deepsat-sat4")
-
 		data_dir = self._get_path(root)
 		if is_train_data:
-			df = pd.read_csv(data_dir + '/X_train_sat4.csv', header=None)
-			self.x_data = torch.tensor(df.values.reshape((400000, 28, 28, 4)))
+			df = pd.read_csv(data_dir + '/X_train_sat6.csv', header=None)
+			self.x_data = torch.tensor(df.values.reshape((324000, 28, 28, 4)), dtype=torch.float)
 			self.x_data = torch.moveaxis(self.x_data, -1, 1)
 
-			df = pd.read_csv(data_dir + '/y_train_sat4.csv', header=None)
+			df = pd.read_csv(data_dir + '/y_train_sat6.csv', header=None)
 			self.y_data = torch.argmax(torch.tensor(df.values), axis=1)
 		else:
-			df = pd.read_csv(data_dir + '/X_test_sat4.csv', header=None)
-			self.x_data = torch.tensor(df.values.reshape((100000, 28, 28, 4)))
+			df = pd.read_csv(data_dir + '/X_test_sat6.csv', header=None)
+			self.x_data = torch.tensor(df.values.reshape((81000, 28, 28, 4)), dtype=torch.float)
 			self.x_data = torch.moveaxis(self.x_data, -1, 1)
 
-			df = pd.read_csv(data_dir + '/y_test_sat4.csv', header=None)
+			df = pd.read_csv(data_dir + '/y_test_sat6.csv', header=None)
 			self.y_data = torch.argmax(torch.tensor(df.values), axis=1)
 
 		if include_additional_features == True and additional_features_list != None:
 			self.external_features = []
 
 			len_textural_features = len(self.TEXTURAL_FEATURES)
 			all_features = np.array(self.ADDITIONAL_FEATURES)
@@ -118,15 +108,14 @@
 
 				self.external_features.append(features_row)
 			self.external_features = torch.tensor(self.external_features)
 
 		else:
 			self.external_features = None
 
-
 	## This method returns the class labels as a dictionary of key-value pairs. Key-> class name, value-> class index
 	def get_class_labels(self):
 		return self._class_to_idx
 
 
 	def __len__(self) -> int:
 		return len(self.x_data)
@@ -149,15 +138,15 @@
 
 
 	def _get_path(self, root_dir):
 		queue = [root_dir]
 		while queue:
 			data_dir = queue.pop(0)
 			folders = os.listdir(data_dir)
-			if "X_train_sat4.csv" in folders and "y_train_sat4.csv" in folders and "X_test_sat4.csv" in folders  and "y_test_sat4.csv" in folders and "sat4annotations.csv" in folders:
+			if "X_train_sat6.csv" in folders and "y_train_sat6.csv" in folders and "X_test_sat6.csv" in folders  and "y_test_sat6.csv" in folders and "sat6annotations.csv" in folders:
 				return data_dir
 
 			for folder in folders:
 				if os.path.isdir(data_dir + "/" + folder):
 					queue.append(data_dir + "/" + folder)
 
 		return None
```

### Comparing `geotorchai-0.1.0/geotorchai/datasets/raster/sat6.py` & `geotorchai-0.2.0/geotorchai/datasets/raster/sat4.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 
 import os
 from typing import Optional, Callable, Dict
-import pandas as pd
-import numpy as np
-import rasterio
 import torch
-from torch import Tensor
 from torch.utils.data import Dataset
-from kaggle.api.kaggle_api_extended import KaggleApi
 from geotorchai.datasets.raster.utility import textural_features as ttf
 from geotorchai.datasets.raster.utility import spectral_indices as si
 from geotorchai.utility.exceptions import InvalidParametersException
-from geotorchai.utility._download_utils import _extract_archive
+import pandas as pd
+import numpy as np
 
 
-class SAT6(Dataset):
+class SAT4(Dataset):
 	'''
-    This is a multi-class classification dtaaset. Link: https://www.kaggle.com/datasets/crawford/deepsat-sat6
-    Image Height and Width: 28 x 28, No of bands: 4, No of classes: 6
+    This is a multi-class classification dtaaset. Link: https://www.kaggle.com/datasets/crawford/deepsat-sat4
+    Image Height and Width: 28 x 28, No of bands: 4, No of classes: 4
 
     Parameters
     ..........
     root (String) - Path to the dataset if it is already downloaded. If not downloaded, it will be downloaded in the given path.
     download (Boolean, Optional) - Set to True if dataset is not available in the given directory. Default: False
     is_train_data (Boolean, Optional) - True denotes training data, while False indicates testing data. Default: True
     bands (List, Optional) - List of all bands that need to be included in the dataset. Default: list of all bands in the EuroSAT images.
@@ -37,60 +33,54 @@
 
 
 	SPECTRAL_BANDS = ["red", "green", "blue", "nir"]
 	RGB_BANDS = ["red", "green", "blue"]
 	ADDITIONAL_FEATURES = ["contrast", "dissimilarity", "homogeneity", "energy", "correlation", "ASM", "mean_NDWI", "mean_NDVI", "mean_RVI"]
 	TEXTURAL_FEATURES = ["contrast", "dissimilarity", "homogeneity", "energy", "correlation", "ASM"]
 	SPECTRAL_INDICES = ["mean_NDWI", "mean_NDVI", "mean_RVI"]
-	SAT6_CLASSES = ["building", "barren_land", "trees", "grassland", "road", "water"]
+	SAT4_CLASSES = ["barren_land", "trees", "grassland", "none"]
 	
 	IMAGE_HEIGHT = 28
 	IMAGE_WIDTH = 28
 	BAND_GREEN_INDEX = 1
 	BAND_RED_INDEX = 0
 	BAND_NIR_INDEX = 3
 
 
-	def __init__(self, root, download = False, is_train_data = True, bands = SPECTRAL_BANDS, include_additional_features = False, additional_features_list = ADDITIONAL_FEATURES, user_features_callback: Optional[Dict[str, Callable]] = None, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None):
+	def __init__(self, root, is_train_data = True, bands = SPECTRAL_BANDS, include_additional_features = False, additional_features_list = ADDITIONAL_FEATURES, user_features_callback: Optional[Dict[str, Callable]] = None, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None):
 		super().__init__()
 		# first check if selected bands are valid. Trow exception otherwise
 		if not self._is_valid_bands(bands):
 			raise InvalidParametersException("Invalid band names")
 
 		self._feature_callbacks = [ttf._get_GLCM_Contrast, ttf._get_GLCM_Dissimilarity, ttf._get_GLCM_Homogeneity, ttf._get_GLCM_Energy, ttf._get_GLCM_Correlation, ttf._get_GLCM_ASM]
 
 		self.selected_band_indices = torch.tensor([self.SPECTRAL_BANDS.index(band) for band in bands])
 		self.user_features_callback = user_features_callback
 		self.transform = transform
 		self.target_transform = target_transform
 
-		self._idx_to_class = {i:j for i, j in enumerate(self.SAT6_CLASSES)}
+		self._idx_to_class = {i:j for i, j in enumerate(self.SAT4_CLASSES)}
 		self._class_to_idx = {value:key for key, value in self._idx_to_class.items()}
 		self._rgb_band_indices = torch.tensor([self.SPECTRAL_BANDS.index(band) for band in self.RGB_BANDS])
 
-		if download:
-			api = KaggleApi()
-			api.authenticate()
-			api.dataset_download_files('crawford/deepsat-sat6', root)
-			_extract_archive(root + "/deepsat-sat6.zip", root + "/deepsat-sat6")
-
 		data_dir = self._get_path(root)
 		if is_train_data:
-			df = pd.read_csv(data_dir + '/X_train_sat6.csv', header=None)
-			self.x_data = torch.tensor(df.values.reshape((324000, 28, 28, 4)), dtype=torch.float)
+			df = pd.read_csv(data_dir + '/X_train_sat4.csv', header=None)
+			self.x_data = torch.tensor(df.values.reshape((400000, 28, 28, 4)))
 			self.x_data = torch.moveaxis(self.x_data, -1, 1)
 
-			df = pd.read_csv(data_dir + '/y_train_sat6.csv', header=None)
+			df = pd.read_csv(data_dir + '/y_train_sat4.csv', header=None)
 			self.y_data = torch.argmax(torch.tensor(df.values), axis=1)
 		else:
-			df = pd.read_csv(data_dir + '/X_test_sat6.csv', header=None)
-			self.x_data = torch.tensor(df.values.reshape((81000, 28, 28, 4)), dtype=torch.float)
+			df = pd.read_csv(data_dir + '/X_test_sat4.csv', header=None)
+			self.x_data = torch.tensor(df.values.reshape((100000, 28, 28, 4)))
 			self.x_data = torch.moveaxis(self.x_data, -1, 1)
 
-			df = pd.read_csv(data_dir + '/y_test_sat6.csv', header=None)
+			df = pd.read_csv(data_dir + '/y_test_sat4.csv', header=None)
 			self.y_data = torch.argmax(torch.tensor(df.values), axis=1)
 
 		if include_additional_features == True and additional_features_list != None:
 			self.external_features = []
 
 			len_textural_features = len(self.TEXTURAL_FEATURES)
 			all_features = np.array(self.ADDITIONAL_FEATURES)
@@ -118,14 +108,15 @@
 
 				self.external_features.append(features_row)
 			self.external_features = torch.tensor(self.external_features)
 
 		else:
 			self.external_features = None
 
+
 	## This method returns the class labels as a dictionary of key-value pairs. Key-> class name, value-> class index
 	def get_class_labels(self):
 		return self._class_to_idx
 
 
 	def __len__(self) -> int:
 		return len(self.x_data)
@@ -148,15 +139,15 @@
 
 
 	def _get_path(self, root_dir):
 		queue = [root_dir]
 		while queue:
 			data_dir = queue.pop(0)
 			folders = os.listdir(data_dir)
-			if "X_train_sat6.csv" in folders and "y_train_sat6.csv" in folders and "X_test_sat6.csv" in folders  and "y_test_sat6.csv" in folders and "sat6annotations.csv" in folders:
+			if "X_train_sat4.csv" in folders and "y_train_sat4.csv" in folders and "X_test_sat4.csv" in folders  and "y_test_sat4.csv" in folders and "sat4annotations.csv" in folders:
 				return data_dir
 
 			for folder in folders:
 				if os.path.isdir(data_dir + "/" + folder):
 					queue.append(data_dir + "/" + folder)
 
 		return None
```

### Comparing `geotorchai-0.1.0/geotorchai/datasets/raster/slum_detection.py` & `geotorchai-0.2.0/geotorchai/datasets/raster/slum_detection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 
 import os
 from typing import Optional, Callable, Dict
-import pandas as pd
-import numpy as np
-import rasterio
 import torch
-from torch import Tensor
 from torch.utils.data import Dataset
-from kaggle.api.kaggle_api_extended import KaggleApi
 from geotorchai.datasets.raster.utility import textural_features as ttf
 from geotorchai.datasets.raster.utility import spectral_indices as si
 from geotorchai.utility.exceptions import InvalidParametersException
-from geotorchai.utility._download_utils import _extract_archive
+import numpy as np
+import rasterio
 
 
 class SlumDetection(Dataset):
 	'''
     This is a binary classification dtaaset. Link: https://www.kaggle.com/datasets/fedebayle/slums-argentina
     Image Height and Width: 32 x 32, No of bands: 4, No of classes: 2
 
@@ -45,15 +41,15 @@
 	IMAGE_HEIGHT = 32
 	IMAGE_WIDTH = 32
 	BAND_GREEN_INDEX = 1
 	BAND_RED_INDEX = 2
 	BAND_NIR_INDEX = 3
 
 
-	def __init__(self, root, download = False, bands = SPECTRAL_BANDS, include_additional_features = False, additional_features_list = ADDITIONAL_FEATURES, user_features_callback: Optional[Dict[str, Callable]] = None, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None):
+	def __init__(self, root, bands = SPECTRAL_BANDS, include_additional_features = False, additional_features_list = ADDITIONAL_FEATURES, user_features_callback: Optional[Dict[str, Callable]] = None, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None):
 		super().__init__()
 		# first check if selected bands are valid. Trow exception otherwise
 		if not self._is_valid_bands(bands):
 			raise InvalidParametersException("Invalid band names")
 
 		self._feature_callbacks = [ttf._get_GLCM_Contrast, ttf._get_GLCM_Dissimilarity, ttf._get_GLCM_Homogeneity, ttf._get_GLCM_Energy, ttf._get_GLCM_Correlation, ttf._get_GLCM_ASM]
 
@@ -62,20 +58,14 @@
 		self.transform = transform
 		self.target_transform = target_transform
 
 		self._idx_to_class = {i:j for i, j in enumerate(self.SLUM_CLASSES)}
 		self._class_to_idx = {value:key for key, value in self._idx_to_class.items()}
 		self._rgb_band_indices = torch.tensor([self.SPECTRAL_BANDS.index(band) for band in self.RGB_BANDS])
 
-		if download:
-			api = KaggleApi()
-			api.authenticate()
-			api.dataset_download_files('fedebayle/slums-argentina', root)
-			_extract_archive(root + "/slums-argentina.zip", root + "/slums-argentina")
-
 		data_dir = self._get_path(root)
 
 		self.image_paths = []
 		self._get_image_paths(data_dir)
 
 		if include_additional_features == True and additional_features_list != None:
 			self.external_features = []
```

### Comparing `geotorchai-0.1.0/geotorchai/datasets/raster/utility/spectral_indices.py` & `geotorchai-0.2.0/geotorchai/datasets/raster/utility/spectral_indices.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/geotorchai/datasets/raster/utility/textural_features.py` & `geotorchai-0.2.0/geotorchai/datasets/raster/utility/textural_features.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 import numpy as np
 from skimage.feature import *
-from skimage.feature import greycoprops as gc
+from skimage.feature import graycoprops as gc
 import torch
 
 def _normalize(img):
     divider = np.amax(img.numpy())/255.0
     return torch.div(img, divider, rounding_mode='floor')
 
 def _rgb_to_grayscale(rgb_image):
@@ -17,37 +17,37 @@
     #ks = 5
     nbit = 8
     bins = np.linspace(mi, ma + 1, nbit + 1)
     bin_image = np.digitize(pixels, bins) - 1
     return bin_image
 
 def _get_GLCM_Contrast(digitized_image):
-    glcm = greycomatrix(digitized_image, [1], [0, np.pi/4, np.pi/2], levels=8 , normed=True, symmetric=True)
+    glcm = graycomatrix(digitized_image, [1], [0, np.pi/4, np.pi/2], levels=8 , normed=True, symmetric=True)
     feature = gc(glcm, "contrast")
     return sum(feature[0].tolist())/len(feature[0].tolist())
 
 def _get_GLCM_Dissimilarity(digitized_image):
-    glcm = greycomatrix(digitized_image, [1], [0, np.pi/4, np.pi/2], levels=8 , normed=True, symmetric=True)
+    glcm = graycomatrix(digitized_image, [1], [0, np.pi/4, np.pi/2], levels=8 , normed=True, symmetric=True)
     feature = gc(glcm, "dissimilarity")
     return sum(feature[0].tolist())/len(feature[0].tolist())
 
 
 def _get_GLCM_Homogeneity(digitized_image):
-    glcm = greycomatrix(digitized_image, [1], [0, np.pi/4, np.pi/2], levels=8 , normed=True, symmetric=True)
+    glcm = graycomatrix(digitized_image, [1], [0, np.pi/4, np.pi/2], levels=8 , normed=True, symmetric=True)
     feature = gc(glcm, "homogeneity")
     return sum(feature[0].tolist())/len(feature[0].tolist())
 
 def _get_GLCM_Energy(digitized_image):
-    glcm = greycomatrix(digitized_image, [1], [0, np.pi/4, np.pi/2], levels=8 , normed=True, symmetric=True)
+    glcm = graycomatrix(digitized_image, [1], [0, np.pi/4, np.pi/2], levels=8 , normed=True, symmetric=True)
     feature = gc(glcm, "energy")
     return sum(feature[0].tolist())/len(feature[0].tolist())
 
 
 def _get_GLCM_Correlation(digitized_image):
-    glcm = greycomatrix(digitized_image, [1], [0, np.pi/4, np.pi/2], levels=8 , normed=True, symmetric=True)
+    glcm = graycomatrix(digitized_image, [1], [0, np.pi/4, np.pi/2], levels=8 , normed=True, symmetric=True)
     feature = gc(glcm, "correlation")
     return sum(feature[0].tolist())/len(feature[0].tolist())
 
 def _get_GLCM_ASM(digitized_image):
-    glcm = greycomatrix(digitized_image, [1], [np.pi/4,np.pi/2], levels=8 , normed=True, symmetric=True)
+    glcm = graycomatrix(digitized_image, [1], [np.pi/4,np.pi/2], levels=8 , normed=True, symmetric=True)
     feature = gc(glcm, "ASM")
     return sum(feature[0].tolist())/len(feature[0].tolist())
```

### Comparing `geotorchai-0.1.0/geotorchai/models/grid/conv_lstm.py` & `geotorchai-0.2.0/geotorchai/models/grid/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/geotorchai/models/grid/deep_stn_net.py` & `geotorchai-0.2.0/geotorchai/models/grid/deep_stn_net.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,18 @@
         input_p (Tensor) - Period sequence part of the input sample
         input_t (Tensor) - Trend sequence part of the input sample
         input_time (Tensor, Optional) - Temporal part of input sample when is_pt is True. Default: None
         input_poi (Tensor, Optional) - POI part of input sample when is_pt is True. Default: None
         '''
 
         if self._device == None:
-            if input_c.get_device() == 0:
+            if input_c.is_cuda:
                 self._device = torch.device("cuda")
+            elif input_c.is_mps:
+                self._device = torch.device("mps")
             else:
                 self._device = torch.device("cpu")
             self.ptTrans._set_device(self._device)
 
         input_c = input_c.view(-1, self.channel_c, self.H, self.W)
         input_p = input_p.view(-1, self.channel_p, self.H, self.W)
         input_t = input_t.view(-1, self.channel_t, self.H, self.W)
```

### Comparing `geotorchai-0.1.0/geotorchai/models/grid/st_resnet.py` & `geotorchai-0.2.0/geotorchai/models/grid/st_resnet.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/geotorchai/models/raster/deepsat2.py` & `geotorchai-0.2.0/geotorchai/models/raster/deepsat2.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/geotorchai/models/raster/fcn.py` & `geotorchai-0.2.0/geotorchai/models/raster/fcn.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/geotorchai/models/raster/sat_cnn.py` & `geotorchai-0.2.0/geotorchai/models/raster/sat_cnn.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/geotorchai/models/raster/unet.py` & `geotorchai-0.2.0/geotorchai/models/raster/unet.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/geotorchai/preprocessing/adapter.py` & `geotorchai-0.2.0/geotorchai/preprocessing/adapter.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/geotorchai/preprocessing/enums/adjacency_type.py` & `geotorchai-0.2.0/geotorchai/preprocessing/enums/adjacency_type.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/geotorchai/preprocessing/enums/aggregation_type.py` & `geotorchai-0.2.0/geotorchai/preprocessing/enums/aggregation_type.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/geotorchai/preprocessing/enums/geo_relationship.py` & `geotorchai-0.2.0/geotorchai/preprocessing/enums/geo_relationship.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/geotorchai/preprocessing/geo_io.py` & `geotorchai-0.2.0/geotorchai/preprocessing/geo_io.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/geotorchai/preprocessing/grid/adjacency.py` & `geotorchai-0.2.0/geotorchai/preprocessing/grid/adjacency.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/geotorchai/preprocessing/grid/space_partition.py` & `geotorchai-0.2.0/geotorchai/preprocessing/grid/space_partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from shapely.geometry import Polygon
-from sedona.utils.adapter import Adapter
-from pyspark.sql import SparkSession
 from pyspark.sql import DataFrame
 from pyspark.sql.types import StructType
 from pyspark.sql.types import StructField
 from pyspark.sql.types import IntegerType
 from sedona.sql.types import GeometryType
 from geotorchai.utility.method_overload import MultipleMeta
 from geotorchai.preprocessing.spark_registration import SparkRegistration
@@ -29,17 +27,17 @@
 		........
 		a pyspark dataframe constsiting of two columns: id of each cell and polygon object representing each cell
 		'''
 
 		# retrieve the SparkSession instance
 		spark = SparkRegistration._get_spark_session()
 
-		geo_rdd = Adapter.toSpatialRdd(geo_df, geometry)
-		geo_rdd.analyze()
-		boundary = geo_rdd.boundaryEnvelope
+		geo_df.createOrReplaceTempView("geo_df")
+		boundary = \
+		spark.sql("SELECT ST_Envelope_Aggr(geo_df.{0}) as boundary FROM geo_df".format(geometry)).collect()[0][0]
 		x_arr, y_arr = boundary.exterior.coords.xy
 		x = list(x_arr)
 		y = list(y_arr)
 
 		min_x, min_y, max_x, max_y = min(x), min(y), max(x), max(y)
 		interval_x = (max_x - min_x)/partitions_x
 		interval_y = (max_y - min_y)/partitions_y
@@ -77,17 +75,17 @@
 		........
 		a pyspark dataframe constsiting of two columns: id of each cell and polygon object representing each cell
 		'''
 
 		# retrieve the SparkSession instance
 		spark = SparkRegistration._get_spark_session()
 
-		geo_rdd = Adapter.toSpatialRdd(geo_df, geometry)
-		geo_rdd.analyze()
-		boundary = geo_rdd.boundaryEnvelope
+		geo_df.createOrReplaceTempView("geo_df")
+		boundary = \
+		spark.sql("SELECT ST_Envelope_Aggr(geo_df.{0}) as boundary FROM geo_df".format(geometry)).collect()[0][0]
 		x_arr, y_arr = boundary.exterior.coords.xy
 		x = list(x_arr)
 		y = list(y_arr)
 
 		min_x, min_y, max_x, max_y = min(x), min(y), max(x), max(y)
 		interval_x = (max_x - min_x)/partitions
 		interval_y = (max_y - min_y)/partitions
```

### Comparing `geotorchai-0.1.0/geotorchai/preprocessing/grid/st_manager.py` & `geotorchai-0.2.0/geotorchai/preprocessing/grid/st_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,86 @@
-from pyspark.sql import SparkSession
-from pyspark.sql.functions import unix_timestamp, date_format, to_date, expr, col
+
+from shapely.geometry import Polygon
+from pyspark.sql import DataFrame
+from pyspark.sql.types import StructType
+from pyspark.sql.types import StructField
+from pyspark.sql.types import IntegerType
+from sedona.sql.types import GeometryType
+from pyspark.sql.functions import unix_timestamp, date_format, to_date, expr, udf, col, count, when, lit
 from pyspark.sql.types import LongType
-from pyspark.sql.functions import udf
 from geotorchai.utility.exceptions import InvalidParametersException
 from geotorchai.preprocessing.spark_registration import SparkRegistration
 import numpy as np
+from decimal import Decimal
 
 class STManager:
 
 
 	@classmethod
 	def convert_date_format(cls, df, date_column, new_format, new_column_alias = None):
 		'''
-	    This function converts dates of a column from one format to another format.
+		This function converts dates of a column from one format to another format.
+
+		Parameters
+		...........
+		df (pyspark.sql.DataFrame) - PySpark DataFrame containing the date column
+		date_column (String) - Column name in df dataframe that contains the dates
+		new_format (String) - New format to which date will be converted
+		new_column_alias (String, Optional) - New column name which will contain the reformatted date. Default: "reformatted_" + date_column
 
-	    Parameters
-	    ........... 
-        df (pyspark.sql.DataFrame) - PySpark DataFrame containing the date column
-        date_column (String) - Column name in df dataframe that contains the dates
-        new_format (String) - New format to which date will be converted
-        new_column_alias (String, Optional) - New column name which will contain the reformatted date. Default: "reformatted_" + date_column
-
-	    Returns
-	    .........
-	    A PySpark DataFrame.
-	    '''
+		Returns
+		.........
+		A PySpark DataFrame.
+		'''
 		if new_column_alias == None:
 			new_column_alias = "reformatted_" + date_column
 		return df.withColumn(new_column_alias, date_format(date_column, new_format))
 
 
 
 	@classmethod
 	def get_unix_timestamp(cls, df, date_column, date_format = "yyyy-MM-dd HH:mm:ss", new_column_alias = None):
 		'''
-	    This function converts the dates in a column into unix timestamps and appends to the dataframe as a new column.
+		This function converts the dates in a column into unix timestamps and appends to the dataframe as a new column.
 
-	    Parameters
-	    ........... 
-        df (pyspark.sql.DataFrame) - PySpark DataFrame containing the date column
-        date_column (String) - Column name in df dataframe that contains the dates
-        date_format (String, Optional) - Current format of the dates. If not provided, it assumes the default format to be: "yyyy-MM-dd HH:mm:ss"
-        new_column_alias (String, Optional) - New column name which will contain the reformatted date. Default: "unix_" + date_column
-
-	    Returns
-	    .........
-	    A PySpark DataFrame.
-	    '''
+		Parameters
+		...........
+		df (pyspark.sql.DataFrame) - PySpark DataFrame containing the date column
+		date_column (String) - Column name in df dataframe that contains the dates
+		date_format (String, Optional) - Current format of the dates. If not provided, it assumes the default format to be: "yyyy-MM-dd HH:mm:ss"
+		new_column_alias (String, Optional) - New column name which will contain the reformatted date. Default: "unix_" + date_column
+
+		Returns
+		.........
+		A PySpark DataFrame.
+		'''
 		if new_column_alias == None:
 			new_column_alias = "unix_" + date_column
 
 		return df.withColumn(new_column_alias, unix_timestamp(date_column, date_format))
 
 
 
 	@classmethod
 	def trim_on_timestamp(cls, df, target_column, upper_threshold = None, lower_threshold = None):
 		'''
-	    This function filters a dataframe deleting rows having timestamp values either above an upper threshold or below a lower threshold.
-	    Among upper and lower thresholds, one of the parameters can be optionally None, but both of these parameters cannot be None simultaneously.
+		This function filters a dataframe deleting rows having timestamp values either above an upper threshold or below a lower threshold.
+		Among upper and lower thresholds, one of the parameters can be optionally None, but both of these parameters cannot be None simultaneously.
 
-	    Parameters
-	    ........... 
-        df (pyspark.sql.DataFrame) - PySpark DataFrame containing the timestamp column
-        target_column (String) - Column name in df dataframe that contains the timestamps
-        upper_threshold (Long, Optional) - Upper threshold, default: None
-        lower_threshold (Long, Optional) - Lower threshold, default: None
-
-	    Returns
-	    .........
-	    A PySpark DataFrame.
-	    '''
+		Parameters
+		...........
+		df (pyspark.sql.DataFrame) - PySpark DataFrame containing the timestamp column
+		target_column (String) - Column name in df dataframe that contains the timestamps
+		upper_threshold (Long, Optional) - Upper threshold, default: None
+		lower_threshold (Long, Optional) - Lower threshold, default: None
+
+		Returns
+		.........
+		A PySpark DataFrame.
+		'''
 		if upper_threshold == None and lower_threshold == None:
 			raise InvalidParametersException("Both upper_threshold and lower_threshold cannot be None")
 		else:
 			spark = SparkRegistration._get_spark_session()
 			df.createOrReplaceTempView("dataset_timestamp")
 			if upper_threshold != None and lower_threshold != None:
 				return df.filter("{0} <= {1} and {0} >= {2}".format(target_column, upper_threshold, lower_threshold))
@@ -84,29 +90,29 @@
 				return df.filter("{0} >= {1}".format(target_column, lower_threshold))
 
 
 
 	@classmethod
 	def trim_on_datetime(cls, df, target_column, upper_date = None, lower_date = None, date_format = "yyyy-MM-dd HH:mm:ss"):
 		'''
-	    This function filters a dataframe deleting rows having datetime values either above an upper threshold or below a lower threshold.
-	    Among upper and lower thresholds, one of the parameters can be optionally None, but both of these parameters cannot be None simultaneously.
+		This function filters a dataframe deleting rows having datetime values either above an upper threshold or below a lower threshold.
+		Among upper and lower thresholds, one of the parameters can be optionally None, but both of these parameters cannot be None simultaneously.
+
+		Parameters
+		...........
+		df (pyspark.sql.DataFrame) - PySpark DataFrame containing the timestamp column
+		target_column (String) - Column name in df dataframe that contains the timestamps
+		upper_date (Long, Optional) - Date denoting the upper threshold, default: None
+		lower_date (Long, Optional) - Date denoting the lower threshold, default: None
+		date_format (String, Optional) - Current format of the date column. If not provided, it assumes the default format to be: "yyyy-MM-dd HH:mm:ss"
 
-	    Parameters
-	    ........... 
-        df (pyspark.sql.DataFrame) - PySpark DataFrame containing the timestamp column
-        target_column (String) - Column name in df dataframe that contains the timestamps
-        upper_date (Long, Optional) - Date denoting the upper threshold, default: None
-        lower_date (Long, Optional) - Date denoting the lower threshold, default: None
-        date_format (String, Optional) - Current format of the date column. If not provided, it assumes the default format to be: "yyyy-MM-dd HH:mm:ss"
-
-	    Returns
-	    .........
-	    A PySpark DataFrame.
-	    '''
+		Returns
+		.........
+		A PySpark DataFrame.
+		'''
 		if upper_date == None and lower_date == None:
 			raise InvalidParametersException("Both upper_date and lower_date cannot be None")
 		else:
 			target_column_converted = target_column + "_converted"
 			spark = SparkRegistration._get_spark_session()
 			df = df.withColumn(target_column_converted, unix_timestamp(target_column, date_format))
 			df.createOrReplaceTempView("dataset_timestamp")
@@ -129,27 +135,27 @@
 				return df.filter("{0} >= {1}".format(target_column_converted, lower_val)).drop(target_column_converted)
 
 
 
 	@classmethod
 	def add_temporal_steps(cls, df, timestamp_column, step_duration, temporal_steps_alias = None):
 		'''
-	    This function adds timestep intervals as a new column to a dataframe which contains a column with unix timestamps.
+		This function adds timestep intervals as a new column to a dataframe which contains a column with unix timestamps.
+
+		Parameters
+		...........
+		df (pyspark.sql.DataFrame) - PySpark DataFrame containing the timestamp column
+		timestamp_column (String) - Column name in df dataframe that contains the timestamps
+		step_duration (Int, Optional) - Duration of a timestep interval or distance between two consecutive timesteps
+		temporal_steps_alias (String, Optional) - New column name which will contain the timesteps. Default: "temporal_steps"
 
-	    Parameters
-	    ........... 
-        df (pyspark.sql.DataFrame) - PySpark DataFrame containing the timestamp column
-        timestamp_column (String) - Column name in df dataframe that contains the timestamps
-        step_duration (Int, Optional) - Duration of a timestep interval or distance between two consecutive timesteps
-        temporal_steps_alias (String, Optional) - New column name which will contain the timesteps. Default: "temporal_steps"
-
-	    Returns
-	    .........
-	    A PySpark DataFrame.
-	    '''
+		Returns
+		.........
+		A PySpark DataFrame.
+		'''
 		if temporal_steps_alias == None:
 			temporal_steps_alias = "temporal_steps"
 
 		min_time = int(df.agg({timestamp_column: "min"}).collect()[0][0])
 
 		def get_step_value(time_value):
 			return (time_value - min_time)//step_duration
@@ -158,49 +164,49 @@
 		return df.withColumn(temporal_steps_alias, get_step(df[timestamp_column].cast(LongType())))
 
 
 
 	@classmethod
 	def get_temporal_steps_count(cls, df, temporal_steps_column):
 		'''
-	    This function returns the total number of timesteps or timestep intervals in a dataframe.
+		This function returns the total number of timesteps or timestep intervals in a dataframe.
+
+		Parameters
+		...........
+		df (pyspark.sql.DataFrame) - PySpark DataFrame containing the timestamp column
+		temporal_steps_column (String) - Column name in df dataframe that contains the timesteps
 
-	    Parameters
-	    ........... 
-        df (pyspark.sql.DataFrame) - PySpark DataFrame containing the timestamp column
-        temporal_steps_column (String) - Column name in df dataframe that contains the timesteps
-
-	    Returns
-	    .........
-	    An Integer: number of timesteps
-	    '''
+		Returns
+		.........
+		An Integer: number of timesteps
+		'''
 		return int(df.agg({temporal_steps_column: "max"}).collect()[0][0]) + 1
 
 
 
 	@classmethod
 	def add_spatial_points(cls, df, lat_column, lon_column, new_column_alias = None):
 		'''
-	    This function creates a column of spatial Point objects from latitude and longitude columns.
+		This function creates a column of spatial Point objects from latitude and longitude columns.
+
+		Parameters
+		...........
+		df (pyspark.sql.DataFrame) - PySpark DataFrame containing latitude and longitude columns
+		lat_column (String) - Name of the latitude column
+		lon_column (String, Optional) - Name of the longitude column
+		new_column_alias (String, Optional) - New column name which will contain the spatial point objects. Default: "st_points"
 
-	    Parameters
-	    ........... 
-        df (pyspark.sql.DataFrame) - PySpark DataFrame containing latitude and longitude columns
-        lat_column (String) - Name of the latitude column
-        lon_column (String, Optional) - Name of the longitude column
-        new_column_alias (String, Optional) - New column name which will contain the spatial point objects. Default: "st_points"
-
-	    Returns
-	    .........
-	    A PySpark DataFrame.
-	    '''
+		Returns
+		.........
+		A PySpark DataFrame.
+		'''
 		if new_column_alias == None:
 			new_column_alias = "st_points"
 
-		return df.withColumn(new_column_alias, expr("ST_Point(double({0}), double({1}))".format(lat_column, lon_column)))
+		return df.withColumn(new_column_alias, expr("ST_Point(double({0}), double({1}))".format(lon_column, lat_column)))
 
 
 
 	@classmethod
 	def aggregate_st_dfs(cls, dataset1, dataset2, geometry1, geometry2, id1, id2, geo_relationship, columns_to_aggregate, column_aggregatioin_types, column_alias_list = None):
 		'''
 		Joins two geo-datasets based on spatial relationships such as contains, intersects, touches, etc.
@@ -213,47 +219,51 @@
 		dataset1: pyspark dataframe containing polygon objects
 		dataset2: pyspark dataframe which contains the features that need to be aggregated
 		geometry1: column name in dataset1 dataframe that contains geometry coordinates
 		geometry2: column name in dataset2 dataframe that contains geometry coordinates
 		id1: column name in dataset1 dataframe that contains ids of polygons
 		id2: column name in dataset2 dataframe that contains ids of temporal steps
 		geo_relationship: stands for the type of spatial relationship. It takes 4 different values:
-		                      SpatialRelationshipType.CONTAINS: geometry in dataset1 completely contains geometry in dataset2
-		                      SpatialRelationshipType.INTERSECTS: geometry in dataset1 intersects geometry in dataset2
-		                      SpatialRelationshipType.TOUCHES: geometry in dataset1 touches geometry in dataset2
-		                      SpatialRelationshipType.WITHIN: geometry in dataset1 in completely within the geometry in dataset2
+							  SpatialRelationshipType.CONTAINS: geometry in dataset1 completely contains geometry in dataset2
+							  SpatialRelationshipType.INTERSECTS: geometry in dataset1 intersects geometry in dataset2
+							  SpatialRelationshipType.TOUCHES: geometry in dataset1 touches geometry in dataset2
+							  SpatialRelationshipType.WITHIN: geometry in dataset1 in completely within the geometry in dataset2
 		columns_to_aggregate: a python list containing the names of columns from dataset2 which need to be aggregated
 		column_aggregatioin_types: stands for the type of column aggregations such as sum, count, avg. It takes 5 different values:
-		                           AggregationType.COUNT: similar to count aggregation type in SQL
-		                           AggregationType.SUM: similar to sum aggregation type in SQL
-		                           AggregationType.AVG: similar to avg aggregation type in SQL
-		                           AggregationType.MIN: similar to min aggregation type in SQL
-		                           AggregationType.MAX: similar to max aggregation type in SQL
+								   AggregationType.COUNT: similar to count aggregation type in SQL
+								   AggregationType.SUM: similar to sum aggregation type in SQL
+								   AggregationType.AVG: similar to avg aggregation type in SQL
+								   AggregationType.MIN: similar to min aggregation type in SQL
+								   AggregationType.MAX: similar to max aggregation type in SQL
 		column_alias_list: Optional, if you want to rename the aggregated columns from the list columns_to_aggregate, provide a list of new names
 
 		Returns
 		.......
 		a pyspark dataframe consisting of polygon ids from dataset1 and aggregated features from dataset2
 		'''
 
-		def __get_columns_selection__(columns_to_aggregate, column_aggregatioin_types, column_alias_list):
+		def __get_columns_selection__():
 			expr = ""
 			for i in range(len(columns_to_aggregate)):
+				if column_aggregatioin_types is not None:
+					aggregation = column_aggregatioin_types[i].value
+				else:
+					aggregation = "COUNT"
 				if i != 0:
 					expr += ", "
-				expr += column_aggregatioin_types[i].value + "(" + columns_to_aggregate[i] + ")"
+				expr += aggregation + "(" + columns_to_aggregate[i] + ")"
 				if column_alias_list is not None:
 					expr += " AS " + column_alias_list[i]
 			return expr
 
 
 		# retrieve the SparkSession instance
 		spark = SparkRegistration._get_spark_session()
 
-		select_expr = __get_columns_selection__(columns_to_aggregate, column_aggregatioin_types, column_alias_list)
+		select_expr = __get_columns_selection__()
 
 		dataset1.createOrReplaceTempView("dataset1")
 		dataset2.createOrReplaceTempView("dataset2")
 		dfJoined = spark.sql("SELECT * FROM dataset1 AS d1 INNER JOIN dataset2 AS d2 ON {0}(d1.{1}, d2.{2})".format(geo_relationship.value, geometry1, geometry2))
 		dfJoined.createOrReplaceTempView("dfJoined")
 		dfJoined = spark.sql("SELECT dfJoined.{0}, dfJoined.{1}, {2} FROM dfJoined GROUP BY dfJoined.{0}, dfJoined.{1} ORDER BY dfJoined.{0}, dfJoined.{1}".format(id2, id1, select_expr))
 		return dfJoined
@@ -272,76 +282,80 @@
 		...........
 		dataset1: pyspark dataframe containing polygon objects
 		dataset2: pyspark dataframe which contains the features that need to be aggregated
 		geometry1: column name in dataset1 dataframe that contains geometry coordinates
 		geometry2: column name in dataset2 dataframe that contains geometry coordinates
 		id1: column name in dataset1 dataframe that contains ids of polygons
 		geo_relationship: stands for the type of spatial relationship. It takes 4 different values:
-		                      SpatialRelationshipType.CONTAINS: geometry in dataset1 completely contains geometry in dataset2
-		                      SpatialRelationshipType.INTERSECTS: geometry in dataset1 intersects geometry in dataset2
-		                      SpatialRelationshipType.TOUCHES: geometry in dataset1 touches geometry in dataset2
-		                      SpatialRelationshipType.WITHIN: geometry in dataset1 in completely within the geometry in dataset2
+							  SpatialRelationshipType.CONTAINS: geometry in dataset1 completely contains geometry in dataset2
+							  SpatialRelationshipType.INTERSECTS: geometry in dataset1 intersects geometry in dataset2
+							  SpatialRelationshipType.TOUCHES: geometry in dataset1 touches geometry in dataset2
+							  SpatialRelationshipType.WITHIN: geometry in dataset1 in completely within the geometry in dataset2
 		columns_to_aggregate: a python list containing the names of columns from dataset2 which need to be aggregated
 		column_aggregatioin_types: stands for the type of column aggregations such as sum, count, avg. It takes 5 different values:
-		                           AggregationType.COUNT: similar to count aggregation type in SQL
-		                           AggregationType.SUM: similar to sum aggregation type in SQL
-		                           AggregationType.AVG: similar to avg aggregation type in SQL
-		                           AggregationType.MIN: similar to min aggregation type in SQL
-		                           AggregationType.MAX: similar to max aggregation type in SQL
+								   AggregationType.COUNT: similar to count aggregation type in SQL
+								   AggregationType.SUM: similar to sum aggregation type in SQL
+								   AggregationType.AVG: similar to avg aggregation type in SQL
+								   AggregationType.MIN: similar to min aggregation type in SQL
+								   AggregationType.MAX: similar to max aggregation type in SQL
 		column_alias_list: Optional, if you want to rename the aggregated columns from the list columns_to_aggregate, provide a list of new names
 
 		Returns
 		.......
 		a pyspark dataframe consisting of polygon ids from dataset1 and aggregated features from dataset2
 		'''
 
-		def __get_columns_selection__(columns_to_aggregate, column_aggregatioin_types, column_alias_list):
+		def __get_columns_selection__():
 			expr = ""
 			for i in range(len(columns_to_aggregate)):
+				if column_aggregatioin_types is not None:
+					aggregation = column_aggregatioin_types[i].value
+				else:
+					aggregation = "COUNT"
 				if i != 0:
 					expr += ", "
-				expr += column_aggregatioin_types[i].value + "(" + columns_to_aggregate[i] + ")"
+				expr += aggregation + "(" + columns_to_aggregate[i] + ")"
 				if column_alias_list is not None:
 					expr += " AS " + column_alias_list[i]
 			return expr
 
 
 		# retrieve the SparkSession instance
 		spark = SparkRegistration._get_spark_session()
 
-		select_expr = __get_columns_selection__(columns_to_aggregate, column_aggregatioin_types, column_alias_list)
+		select_expr = __get_columns_selection__()
 
 		dataset1.createOrReplaceTempView("dataset1")
 		dataset2.createOrReplaceTempView("dataset2")
-		dfJoined = spark.sql("SELECT * FROM dataset1 AS d1 JOIN dataset2 AS d2 ON {0}(d1.{1}, d2.{2})".format(geo_relationship.value, geometry1, geometry2))
+		dfJoined = spark.sql("SELECT * FROM dataset1 AS d1 INNER JOIN dataset2 AS d2 ON {0}(d1.{1}, d2.{2})".format(geo_relationship.value, geometry1, geometry2))
 		dfJoined.createOrReplaceTempView("dfJoined")
 		dfJoined = spark.sql("SELECT dfJoined.{0}, {1} FROM dfJoined GROUP BY dfJoined.{0} ORDER BY dfJoined.{0}".format(id1, select_expr))
 		return dfJoined
 
 
 
 	@classmethod
 	def get_st_array(cls, df, temporal_id, spatial_id, columns_list, temporal_length, spatial_length, missing_data = None):
 		'''
-	    This function creates a spatiotemporal tensor shaped array from a spatiotemporal dataframe.
+		This function creates a spatiotemporal tensor shaped array from a spatiotemporal dataframe.
 
-	    Parameters
-	    ........... 
-        df (pyspark.sql.DataFrame) - PySpark DataFrame from which spatiotemporal array will be created
-        temporal_id (String) - Name of the column that contains timestep ids
-        spatial_id (String) - Name of the column that contains spatial polygon/point ids
-        columns_list (String) - Columns representing the features to be included to the array or spatiotemporal tensor.
-        temporal_length (String) - Total number of timesteps
-        spatial_length (String) - Total number of spatial point or polygon objects
-        missing_data (String, Optional) - Feature value which will replace the empty cells
-
-	    Returns
-	    .........
-	    A numpy array with a shape of spatiotemporal tensor
-	    '''
+		Parameters
+		...........
+		df (pyspark.sql.DataFrame) - PySpark DataFrame from which spatiotemporal array will be created
+		temporal_id (String) - Name of the column that contains timestep ids
+		spatial_id (String) - Name of the column that contains spatial polygon/point ids
+		columns_list (String) - Columns representing the features to be included to the array or spatiotemporal tensor.
+		temporal_length (String) - Total number of timesteps
+		spatial_length (String) - Total number of spatial point or polygon objects
+		missing_data (String, Optional) - Feature value which will replace the empty cells
+
+		Returns
+		.........
+		A numpy array with a shape of spatiotemporal tensor
+		'''
 		st_array = np.empty((temporal_length, spatial_length, len(columns_list)))
 		if missing_data == None:
 			st_array[:] = np.NaN
 		else:
 			st_array[:] = missing_data
 
 		for row in df.collect():
@@ -353,31 +367,31 @@
 		return st_array
 
 
 
 	@classmethod
 	def get_st_grid_array(cls, df, temporal_id, spatial_id, columns_list, temporal_length, height, width, missing_data = None):
 		'''
-	    This function creates a grid-based spatiotemporal tensor shaped array from a grid-based spatiotemporal dataframe.
+		This function creates a grid-based spatiotemporal tensor shaped array from a grid-based spatiotemporal dataframe.
 
-	    Parameters
-	    ........... 
-        df (pyspark.sql.DataFrame) - PySpark DataFrame from which spatiotemporal array will be created
-        temporal_id (String) - Name of the column that contains timestep ids
-        spatial_id (String) - Name of the column that contains spatial polygon/point ids
-        columns_list (String) - Columns representing the features to be included to the array or spatiotemporal tensor.
-        temporal_length (String) - Total number of timesteps
-        height (String) - Height of grid or number of rows
-        width (String) - Width of grid or number of columns
-        missing_data (String, Optional) - Feature value which will replace the empty cells
-
-	    Returns
-	    .........
-	    A numpy array with a shape of spatiotemporal tensor
-	    '''
+		Parameters
+		...........
+		df (pyspark.sql.DataFrame) - PySpark DataFrame from which spatiotemporal array will be created
+		temporal_id (String) - Name of the column that contains timestep ids
+		spatial_id (String) - Name of the column that contains spatial polygon/point ids
+		columns_list (String) - Columns representing the features to be included to the array or spatiotemporal tensor.
+		temporal_length (String) - Total number of timesteps
+		height (String) - Height of grid or number of rows or number of partitions along latitude
+		width (String) - Width of grid or number of columns or number of partitions along longitude
+		missing_data (String, Optional) - Feature value which will replace the empty cells
+
+		Returns
+		.........
+		A numpy array with a shape of spatiotemporal tensor
+		'''
 		st_array = np.empty((temporal_length, height, width, len(columns_list)))
 		if missing_data == None:
 			st_array[:] = np.NaN
 		else:
 			st_array[:] = missing_data
 
 		for row in df.collect():
@@ -391,28 +405,28 @@
 		return st_array
 
 
 
 	@classmethod
 	def get_spatial_array(cls, df, spatial_id, columns_list, spatial_length, missing_data = None):
 		'''
-	    This function creates a spatial tensor shaped array from a spatial dataframe. It does not contain any temporal dimension.
+		This function creates a spatial tensor shaped array from a spatial dataframe. It does not contain any temporal dimension.
 
-	    Parameters
-	    ........... 
-        df (pyspark.sql.DataFrame) - PySpark DataFrame from which spatial array will be created
-        spatial_id (String) - Name of the column that contains spatial polygon/point ids
-        columns_list (String) - Columns representing the features to be included to the array or spatial tensor.
-        spatial_length (String) - Total number of spatial point or polygon objects
-        missing_data (String, Optional) - Feature value which will replace the empty cells
-
-	    Returns
-	    .........
-	    A numpy array with a shape of spatial tensor
-	    '''
+		Parameters
+		...........
+		df (pyspark.sql.DataFrame) - PySpark DataFrame from which spatial array will be created
+		spatial_id (String) - Name of the column that contains spatial polygon/point ids
+		columns_list (String) - Columns representing the features to be included to the array or spatial tensor.
+		spatial_length (String) - Total number of spatial point or polygon objects
+		missing_data (String, Optional) - Feature value which will replace the empty cells
+
+		Returns
+		.........
+		A numpy array with a shape of spatial tensor
+		'''
 		st_array = np.empty((spatial_length, len(columns_list)))
 		if missing_data == None:
 			st_array[:] = np.NaN
 		else:
 			st_array[:] = missing_data
 
 		for row in df.collect():
@@ -422,29 +436,29 @@
 
 		return st_array
 
 
 	@classmethod
 	def get_spatial_grid_array(cls, df, spatial_id, columns_list, height, width, missing_data = None):
 		'''
-	    This function creates a grid-based spatial tensor shaped array from a grid-based spatial dataframe. It does not contain any temporal dimension.
+		This function creates a grid-based spatial tensor shaped array from a grid-based spatial dataframe. It does not contain any temporal dimension.
+
+		Parameters
+		...........
+		df (pyspark.sql.DataFrame) - PySpark DataFrame from which spatial array will be created
+		spatial_id (String) - Name of the column that contains spatial polygon/point ids
+		columns_list (String) - Columns representing the features to be included to the array or spatial tensor.
+		height (String) - Height of grid or number of rows
+		width (String) - Width of grid or number of columns
+		missing_data (String, Optional) - Feature value which will replace the empty cells
 
-	    Parameters
-	    ........... 
-        df (pyspark.sql.DataFrame) - PySpark DataFrame from which spatial array will be created
-        spatial_id (String) - Name of the column that contains spatial polygon/point ids
-        columns_list (String) - Columns representing the features to be included to the array or spatial tensor.
-        height (String) - Height of grid or number of rows
-        width (String) - Width of grid or number of columns
-        missing_data (String, Optional) - Feature value which will replace the empty cells
-
-	    Returns
-	    .........
-	    A numpy array with a shape of spatial tensor
-	    '''
+		Returns
+		.........
+		A numpy array with a shape of spatial tensor
+		'''
 		st_array = np.empty((height, width, len(columns_list)))
 		if missing_data == None:
 			st_array[:] = np.NaN
 		else:
 			st_array[:] = missing_data
 
 		for row in df.collect():
@@ -452,9 +466,175 @@
 			h = spatial_pos//width
 			w = spatial_pos%width
 			for i in range(len(columns_list)):
 				st_array[h][w][i] = row[columns_list[i]]
 
 		return st_array
 
+	@classmethod
+	def get_st_grid_dataframe(cls, geo_df: DataFrame, geometry: str, partitions_x: int, partitions_y: int,
+							  col_date: str,
+							  step_duration_sec: int = 3600, date_format: str = "yyyy-MM-dd HH:mm:ss",
+							  columns_to_aggregate: list = None, column_aggregatioin_types: list = None,
+							  column_alias_list: list = None):
+		'''
+		Function aggregates features into a spatiotemporal grid format
+
+		Parameters
+		...........
+		geo_df: pyspark dataframe containing a column of geometry type
+		geometry: name of the geometry typed column in geo_df dataframe
+		partitions_x: number of partitions along longitude or width
+		partitions_y: number of partitions along latitude or height
+		col_date (String) - Column name in geo_df dataframe that contains the dates
+		step_duration_sec (Int, Optional) - Duration of a timestep interval or distance between two consecutive timesteps
+		date_format (String, Optional) - Current format of the dates. If not provided, it assumes the default format to be: "yyyy-MM-dd HH:mm:ss"
+		columns_to_aggregate: a python list containing the names of columns from dataset2 which need to be aggregated
+		column_aggregatioin_types: stands for the type of column aggregations such as sum, count, avg. It takes 5 different values:
+								   AggregationType.COUNT: similar to count aggregation type in SQL
+								   AggregationType.SUM: similar to sum aggregation type in SQL
+								   AggregationType.AVG: similar to avg aggregation type in SQL
+								   AggregationType.MIN: similar to min aggregation type in SQL
+								   AggregationType.MAX: similar to max aggregation type in SQL
+		column_alias_list: Optional, if you want to rename the aggregated columns from the list columns_to_aggregate, provide a list of new names
+
+		Returns
+		........
+		a pyspark dataframe consisting of aggregated features in spatiotemporal grid format
+		'''
+
+		def __get_columns_selection__():
+			expr = ""
+			for i in range(len(columns_to_aggregate)):
+				if column_aggregatioin_types is not None:
+					aggregation = column_aggregatioin_types[i].value
+				else:
+					aggregation = "COUNT"
+				if i != 0:
+					expr += ", "
+				expr += aggregation + "(" + columns_to_aggregate[i] + ")"
+				if column_alias_list is not None:
+					expr += " AS " + column_alias_list[i]
+			return expr
+
+		# retrieve the SparkSession instance
+		spark = SparkRegistration._get_spark_session()
+
+		geo_df.createOrReplaceTempView("geo_df")
+		boundary = \
+			spark.sql("SELECT ST_Envelope_Aggr(geo_df.{0}) as boundary FROM geo_df".format(geometry)).collect()[0][0]
+		x_arr, y_arr = boundary.exterior.coords.xy
+
+		x = list(x_arr)
+		y = list(y_arr)
+		min_x, min_y, max_x, max_y = min(x), min(y), max(x), max(y)
+		frac_x = 1 / (10 ** (len(str(min_x).split(".")[1])))
+		frac_y = 1 / (10 ** (len(str(min_y).split(".")[1])))
+		interval_x = (max_x - min_x + frac_x) / partitions_x
+		interval_y = (max_y - min_y + frac_y) / partitions_y
+
+		def get_cell_id(longitude, latitude):
+			i = int((latitude - min_y) / interval_y)
+			j = int((longitude - min_x) / interval_x)
+			return i * partitions_x + j
+
+		get_cell = udf(lambda x, y: get_cell_id(x, y), IntegerType())
+		geo_df = geo_df.withColumn("cell_id", get_cell(expr("ST_X({0})".format(geometry)),
+													   expr("ST_Y({0})".format(geometry))))
+
+		geo_df = geo_df.withColumn("_unix_time_", unix_timestamp(col_date, date_format))
+		min_time = int(geo_df.agg({"_unix_time_": "min"}).collect()[0][0])
+
+		def get_step_value(time_value):
+			return (time_value - min_time) // step_duration_sec
+
+		get_step = udf(lambda x: get_step_value(x), LongType())
+		geo_df = geo_df.withColumn("_id_timestep", get_step(geo_df["_unix_time_"])).drop("_unix_time_")
+
+		if columns_to_aggregate != None:
+			geo_df.createOrReplaceTempView("geo_df")
+			select_expr = __get_columns_selection__()
+			geo_df = spark.sql(
+				"SELECT cell_id, _id_timestep, {0} FROM geo_df GROUP BY cell_id, _id_timestep".format(
+					select_expr))
+		else:
+			geo_df = geo_df.groupBy(["cell_id", "_id_timestep"]).agg(count(col(geometry)).alias("aggregated_feature"))
+		return geo_df
+
+
+	@classmethod
+	def get_spatial_grid_dataframe(cls, geo_df: DataFrame, geometry: str, partitions_x: int, partitions_y: int, columns_to_aggregate: list=None, column_aggregatioin_types: list=None, column_alias_list: list = None):
+		'''
+		Function aggregates features into a spatial grid format
+
+		Parameters
+		...........
+		geo_df: pyspark dataframe containing a column of geometry type
+		geometry: name of the geometry typed column in geo_df dataframe
+		partitions_x: number of partitions along latitude
+		partitions_y: number of partitions along longitude
+		columns_to_aggregate: a python list containing the names of columns from dataset2 which need to be aggregated
+		column_aggregatioin_types: stands for the type of column aggregations such as sum, count, avg. It takes 5 different values:
+								   AggregationType.COUNT: similar to count aggregation type in SQL
+								   AggregationType.SUM: similar to sum aggregation type in SQL
+								   AggregationType.AVG: similar to avg aggregation type in SQL
+								   AggregationType.MIN: similar to min aggregation type in SQL
+								   AggregationType.MAX: similar to max aggregation type in SQL
+		column_alias_list: Optional, if you want to rename the aggregated columns from the list columns_to_aggregate, provide a list of new names
+
+		Returns
+		........
+		a pyspark dataframe consisting of aggregated features in spatial grid format
+		'''
+
+		def __get_columns_selection__():
+			expr = ""
+			for i in range(len(columns_to_aggregate)):
+				if column_aggregatioin_types is not None:
+					aggregation = column_aggregatioin_types[i].value
+				else:
+					aggregation = "COUNT"
+				if i != 0:
+					expr += ", "
+				expr += aggregation + "(" + columns_to_aggregate[i] + ")"
+				if column_alias_list is not None:
+					expr += " AS " + column_alias_list[i]
+			return expr
+
+		# retrieve the SparkSession instance
+		spark = SparkRegistration._get_spark_session()
+
+		geo_df.createOrReplaceTempView("geo_df")
+		boundary = \
+		spark.sql("SELECT ST_Envelope_Aggr(geo_df.{0}) as boundary FROM geo_df".format(geometry)).collect()[0][0]
+		x_arr, y_arr = boundary.exterior.coords.xy
+
+		x = list(x_arr)
+		y = list(y_arr)
+		min_x, min_y, max_x, max_y = min(x), min(y), max(x), max(y)
+		frac_x = 1 / (10 ** (len(str(min_x).split(".")[1])))
+		frac_y = 1 / (10 ** (len(str(min_y).split(".")[1])))
+		interval_x = (max_x - min_x + frac_x) / partitions_x
+		interval_y = (max_y - min_y + frac_y) / partitions_y
+
+		def get_cell_id(longitude, latitude):
+			i = int((latitude - min_y) / interval_y)
+			j = int((longitude - min_x) / interval_x)
+			return i * partitions_x + j
+
+		get_cell = udf(lambda x, y: get_cell_id(x, y), IntegerType())
+		geo_df = geo_df.withColumn("cell_id", get_cell(expr("ST_X({0})".format(geometry)),
+													   expr("ST_Y({0})".format(geometry))))
+
+		if columns_to_aggregate != None:
+			geo_df.createOrReplaceTempView("geo_df")
+			select_expr = __get_columns_selection__()
+			geo_df = spark.sql(
+				"SELECT cell_id, {0} FROM geo_df GROUP BY cell_id ORDER BY cell_id".format(select_expr))
+		else:
+			geo_df = geo_df.groupBy("cell_id").agg(
+				count(col(geometry)).alias("aggregated_feature")).orderBy("cell_id")
+		return geo_df
+
+
```

### Comparing `geotorchai-0.1.0/geotorchai/preprocessing/raster/raster_processing.py` & `geotorchai-0.2.0/geotorchai/preprocessing/raster/raster_processing.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/geotorchai/preprocessing/spark_registration.py` & `geotorchai-0.2.0/geotorchai/preprocessing/spark_registration.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/geotorchai/transforms/raster.py` & `geotorchai-0.2.0/geotorchai/transforms/raster.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/geotorchai/utility/exceptions.py` & `geotorchai-0.2.0/geotorchai/utility/exceptions.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/geotorchai/utility/method_overload.py` & `geotorchai-0.2.0/geotorchai/utility/method_overload.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/geotorchai.egg-info/PKG-INFO` & `geotorchai-0.2.0/geotorchai.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geotorchai
-Version: 0.1.0
+Version: 0.2.0
 Summary: GeoTorchAI, formarly GeoTorch, A Spatiotemporal Deep Learning Framework
 Home-page: https://github.com/DataSystemsLab/GeoTorch
 Author: Kanchan Chowdhury
 Author-email: kchowdh1@asu.edu
 License: AGPL-3.0
 Keywords: spatial-machine-learning,spatiotemporal-deep-learning,spatial forecasting,deep learning,machine learning,spatiotemporal forecasting,temporal signal,raster classification,satellite classification,raster segmentation,satellite segmentation,convlstm,st-resnet,deepstn+,deepsatv2,lstm,temporal network,eurosat,representation learning
 Classifier: Development Status :: 3 - Alpha
@@ -48,27 +48,20 @@
 
 Our preprocessing module is designed such that it minimizes the number of methods and classes in the API. Users can perform end-to-end spatiotemporal data preprocessing, which starts by loading raw datasets and ends by generating a trainable Tensor-shaped array, with a minimum number of method calls. It helps the users understand the API fast and reduces their confusion.
 
 
 ## Documentation
 Details documentation on installation, API, and programming guide is available on [GeoTorchAI Website](https://kanchanchy.github.io/geotorchai/).
 
-## Dependency Set up
-Following libraries need to be set up before using GeoTorchAI.
-
-##### Dependencies for Deep Learning Module:
-1. PyTorch >=1.10
-2. Rasterio
-3. Scikit-image
-
-##### Dependencies for Preprocessing Module:
-1. PySpark >=3.0.0
-2. Apache Sedona >=1.2.0-incubating
-
-For installation, visit the [instructions](https://kanchanchy.github.io/geotorchai/installation.html).
+## Installation
+GeoTorchAI can be installed by running the following command:
+```
+pip install geotorchai
+```
+GeoTorchAI is available on [PyPI](https://pypi.org/project/geotorchai/). For more instructions regrading the required and optional dependencies, please visit the [website](https://kanchanchy.github.io/geotorchai/installation.html).
 
 ## Example
 End-to-end coding examples for various applications including model training and data preprocessing are available in our [binders](https://github.com/DataSystemsLab/GeoTorchAI/tree/main/binders) and [examples](https://github.com/DataSystemsLab/GeoTorchAI/tree/main/examples) sections.
 
 We show a very short example of satellite imagery classification using GeoTorchAI in a step-by-step manner below. Training a satellite imagery classification model consists of three steps: loading the dataset, initializing the model and parameters, and train the model. We pick the [DeepSatV2](https://arxiv.org/abs/1911.07747) model to classify [EuroSAT](https://github.com/phelber/EuroSAT) satellite images.
 #### EuroSAT Image Classes
 * Annual Crop
@@ -84,15 +77,15 @@
 #### Spectral Bands of a Highway Image
 ![Highway Image](https://github.com/DataSystemsLab/GeoTorchAI/blob/main/data/euro-highway.png)
 #### Spectral Bands of an Industry Image
 ![Industry Image](https://github.com/DataSystemsLab/GeoTorchAI/blob/main/data/euro-industry.png)
 #### Loading Training Dataset
 Load the EuroSAT Dataset. Setting download=True will download the full data in the given directory. If data is already available, set download=False.
 ```
-full_data = geotorch.datasets.raser.EuroSAT(root="data/eurosat", download=True, include_additional_features=True)
+full_data = geotorchai.datasets.raser.EuroSAT(root="data/eurosat", download=True, include_additional_features=True)
 ```
 #### Split data into 80% train and 20% validation parts
 ```
 dataset_size = len(full_data)
 indices = list(range(dataset_size))
 split = int(np.floor(0.2 * dataset_size))
 np.random.seed(random_seed)
```

### Comparing `geotorchai-0.1.0/geotorchai.egg-info/SOURCES.txt` & `geotorchai-0.2.0/geotorchai.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,24 @@
 geotorchai.egg-info/PKG-INFO
 geotorchai.egg-info/SOURCES.txt
 geotorchai.egg-info/dependency_links.txt
 geotorchai.egg-info/requires.txt
 geotorchai.egg-info/top_level.txt
 geotorchai/datasets/__init__.py
 geotorchai/datasets/grid/__init__.py
+geotorchai/datasets/grid/geopotential.py
 geotorchai/datasets/grid/nyc_bike_deepstn.py
 geotorchai/datasets/grid/nyc_bike_stdn.py
 geotorchai/datasets/grid/nyc_taxi_stdn.py
 geotorchai/datasets/grid/processed.py
 geotorchai/datasets/grid/taxi_bj_21.py
+geotorchai/datasets/grid/temperature.py
+geotorchai/datasets/grid/toa_incident_solar_radiation.py
+geotorchai/datasets/grid/total_cloud_cover.py
+geotorchai/datasets/grid/total_precipitation.py
 geotorchai/datasets/raster/__init__.py
 geotorchai/datasets/raster/cloud_38.py
 geotorchai/datasets/raster/euro_sat.py
 geotorchai/datasets/raster/processed.py
 geotorchai/datasets/raster/processed_extra_features.py
 geotorchai/datasets/raster/sat4.py
 geotorchai/datasets/raster/sat6.py
@@ -25,14 +30,15 @@
 geotorchai/datasets/raster/utility/__init__.py
 geotorchai/datasets/raster/utility/spectral_indices.py
 geotorchai/datasets/raster/utility/textural_features.py
 geotorchai/models/__init__.py
 geotorchai/models/grid/__init__.py
 geotorchai/models/grid/conv_lstm.py
 geotorchai/models/grid/deep_stn_net.py
+geotorchai/models/grid/periodical_cnn.py
 geotorchai/models/grid/st_resnet.py
 geotorchai/models/raster/__init__.py
 geotorchai/models/raster/deepsat2.py
 geotorchai/models/raster/fcn.py
 geotorchai/models/raster/sat_cnn.py
 geotorchai/models/raster/unet.py
 geotorchai/preprocessing/__init__.py
```

### Comparing `geotorchai-0.1.0/setup.py` & `geotorchai-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,29 +25,30 @@
     "eurosat",
     "representation learning",
 ]
 
 setup(
     name='geotorchai',
     packages=find_packages(),
-    version='0.1.0',
+    version='0.2.0',
     description='GeoTorchAI, formarly GeoTorch, A Spatiotemporal Deep Learning Framework',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     author='Kanchan Chowdhury',
     author_email='kchowdh1@asu.edu',
     url='https://github.com/DataSystemsLab/GeoTorch',
     license='AGPL-3.0',
     install_requires=[
         'torch',
-        'rasterio',
-        'scikit-image',
+        'rasterio <= 1.1.8',
+        'scikit-image >= 0.19.0',
         'numpy',
         'pandas',
-        'kaggle',
+        'xarray',
+        'cdsapi',
     ],
     extras_require={
         'Preprocessing':  ['pyspark', 'apache-sedona'],
     },
     setup_requires=['pytest-runner'],
     tests_require=['pytest'],
     test_suite='tests',
```

### Comparing `geotorchai-0.1.0/tests/deep-learning/test_grid_datasets.py` & `geotorchai-0.2.0/tests/deep-learning/test_grid_datasets.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/tests/deep-learning/test_models.py` & `geotorchai-0.2.0/tests/deep-learning/test_models.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/tests/deep-learning/test_raster_datasets.py` & `geotorchai-0.2.0/tests/deep-learning/test_raster_datasets.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/tests/deep-learning/test_transforms.py` & `geotorchai-0.2.0/tests/deep-learning/test_transforms.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/tests/preprocessing/test_adjacency.py` & `geotorchai-0.2.0/tests/preprocessing/test_adjacency.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/tests/preprocessing/test_data_loader.py` & `geotorchai-0.2.0/tests/preprocessing/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/tests/preprocessing/test_feature_aggregation.py` & `geotorchai-0.2.0/tests/preprocessing/test_feature_aggregation.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/tests/preprocessing/test_raster_transform.py` & `geotorchai-0.2.0/tests/preprocessing/test_raster_transform.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/tests/preprocessing/test_space_partition.py` & `geotorchai-0.2.0/tests/preprocessing/test_space_partition.py`

 * *Files identical despite different names*

### Comparing `geotorchai-0.1.0/tests/preprocessing/test_spark_registration.py` & `geotorchai-0.2.0/tests/preprocessing/test_spark_registration.py`

 * *Files identical despite different names*


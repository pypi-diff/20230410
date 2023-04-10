# Comparing `tmp/traceml-1.1.0rc2.tar.gz` & `tmp/traceml-1.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traceml-1.1.0rc2.tar", last modified: Sun Apr  9 15:48:03 2023, max compression
+gzip compressed data, was "traceml-1.1.0rc3.tar", last modified: Mon Apr 10 12:17:47 2023, max compression
```

## Comparing `traceml-1.1.0rc2.tar` & `traceml-1.1.0rc3.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:48:03.332481 traceml-1.1.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-09 15:48:03.332481 traceml-1.1.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-09 15:48:03.336480 traceml-1.1.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:48:03.320480 traceml-1.1.0rc2/traceml/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:48:03.324480 traceml-1.1.0rc2/traceml/artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/artifacts/kinds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/artifacts/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:48:03.324480 traceml-1.1.0rc2/traceml/events/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/events/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    15500 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/events/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:48:03.324480 traceml-1.1.0rc2/traceml/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/integrations/fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/integrations/fastai_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/integrations/hugging_face.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/integrations/ignite.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/integrations/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/integrations/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/integrations/pytorch_lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/integrations/scikit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/integrations/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/integrations/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/integrations/xgboost.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:48:03.328480 traceml-1.1.0rc2/traceml/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/logging/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/logging/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/logging/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/logging/streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/pkg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:48:03.328480 traceml-1.1.0rc2/traceml/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/processors/df_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/processors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:48:03.328480 traceml-1.1.0rc2/traceml/processors/events_processors/
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/processors/events_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/processors/events_processors/events_artifacts_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/processors/events_processors/events_audio_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/processors/events_processors/events_charts_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/processors/events_processors/events_image_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/processors/events_processors/events_metrics_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/processors/events_processors/events_models_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/processors/events_processors/events_tables_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/processors/events_processors/events_video_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/processors/gpu_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/processors/importance_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/processors/logs_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/processors/psutil_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/processors/units_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:48:03.328480 traceml-1.1.0rc2/traceml/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/serialization/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/serialization/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:48:03.328480 traceml-1.1.0rc2/traceml/summary/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/summary/df.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:48:03.332481 traceml-1.1.0rc2/traceml/tracking/
--rw-r--r--   0 runner    (1001) docker     (123)    28282 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61766 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/tracking/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:48:03.332481 traceml-1.1.0rc2/traceml/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:48:03.332481 traceml-1.1.0rc2/traceml/vendor/matplotlylib/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/vendor/matplotlylib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:48:03.332481 traceml-1.1.0rc2/traceml/vendor/matplotlylib/mplexporter/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/vendor/matplotlylib/mplexporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/vendor/matplotlylib/mplexporter/_py3k_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/vendor/matplotlylib/mplexporter/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:48:03.332481 traceml-1.1.0rc2/traceml/vendor/matplotlylib/mplexporter/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/vendor/matplotlylib/mplexporter/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/vendor/matplotlylib/mplexporter/renderers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/vendor/matplotlylib/mplexporter/renderers/fake_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/vendor/matplotlylib/mplexporter/renderers/vega_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/vendor/matplotlylib/mplexporter/renderers/vincent_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/vendor/matplotlylib/mplexporter/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/vendor/matplotlylib/mplexporter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/vendor/matplotlylib/mpltools.py
--rw-r--r--   0 runner    (1001) docker     (123)    35762 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/vendor/matplotlylib/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/vendor/matplotlylib/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)   166500 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/vendor/pynvml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:48:03.332481 traceml-1.1.0rc2/traceml/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-04-09 15:47:53.000000 traceml-1.1.0rc2/traceml/visualization/run_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:48:03.324480 traceml-1.1.0rc2/traceml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-09 15:48:03.000000 traceml-1.1.0rc2/traceml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-09 15:48:03.000000 traceml-1.1.0rc2/traceml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 15:48:03.000000 traceml-1.1.0rc2/traceml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-09 15:48:03.000000 traceml-1.1.0rc2/traceml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 15:48:03.000000 traceml-1.1.0rc2/traceml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:47.463384 traceml-1.1.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-10 12:17:47.463384 traceml-1.1.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-10 12:17:47.463384 traceml-1.1.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:47.451384 traceml-1.1.0rc3/traceml/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:47.451384 traceml-1.1.0rc3/traceml/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/artifacts/kinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/artifacts/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:47.451384 traceml-1.1.0rc3/traceml/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/events/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15500 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/events/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:47.455384 traceml-1.1.0rc3/traceml/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/integrations/fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/integrations/fastai_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/integrations/hugging_face.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/integrations/ignite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/integrations/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/integrations/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/integrations/pytorch_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/integrations/scikit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/integrations/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/integrations/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/integrations/xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:47.455384 traceml-1.1.0rc3/traceml/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/logging/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/logging/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/logging/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/logging/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/pkg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:47.455384 traceml-1.1.0rc3/traceml/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/processors/df_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/processors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:47.459384 traceml-1.1.0rc3/traceml/processors/events_processors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/processors/events_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/processors/events_processors/events_artifacts_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/processors/events_processors/events_audio_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/processors/events_processors/events_charts_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/processors/events_processors/events_image_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/processors/events_processors/events_metrics_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/processors/events_processors/events_models_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/processors/events_processors/events_tables_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/processors/events_processors/events_video_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/processors/gpu_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/processors/importance_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/processors/logs_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/processors/psutil_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/processors/units_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:47.459384 traceml-1.1.0rc3/traceml/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/serialization/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/serialization/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:47.459384 traceml-1.1.0rc3/traceml/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/summary/df.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:47.459384 traceml-1.1.0rc3/traceml/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)    28282 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61786 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/tracking/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:47.459384 traceml-1.1.0rc3/traceml/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:47.459384 traceml-1.1.0rc3/traceml/vendor/matplotlylib/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/vendor/matplotlylib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:47.459384 traceml-1.1.0rc3/traceml/vendor/matplotlylib/mplexporter/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/vendor/matplotlylib/mplexporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/vendor/matplotlylib/mplexporter/_py3k_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/vendor/matplotlylib/mplexporter/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:47.463384 traceml-1.1.0rc3/traceml/vendor/matplotlylib/mplexporter/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/vendor/matplotlylib/mplexporter/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/vendor/matplotlylib/mplexporter/renderers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/vendor/matplotlylib/mplexporter/renderers/fake_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/vendor/matplotlylib/mplexporter/renderers/vega_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/vendor/matplotlylib/mplexporter/renderers/vincent_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/vendor/matplotlylib/mplexporter/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/vendor/matplotlylib/mplexporter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/vendor/matplotlylib/mpltools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35762 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/vendor/matplotlylib/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/vendor/matplotlylib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)   166500 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/vendor/pynvml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:47.463384 traceml-1.1.0rc3/traceml/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-04-10 12:17:37.000000 traceml-1.1.0rc3/traceml/visualization/run_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:17:47.451384 traceml-1.1.0rc3/traceml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-10 12:17:47.000000 traceml-1.1.0rc3/traceml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-10 12:17:47.000000 traceml-1.1.0rc3/traceml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:17:47.000000 traceml-1.1.0rc3/traceml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-10 12:17:47.000000 traceml-1.1.0rc3/traceml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 12:17:47.000000 traceml-1.1.0rc3/traceml.egg-info/top_level.txt
```

### Comparing `traceml-1.1.0rc2/PKG-INFO` & `traceml-1.1.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceml
-Version: 1.1.0rc2
+Version: 1.1.0rc3
 Summary: Engine for ML/Data tracking, visualization, dashboards, and model UI for Polyaxon.
 Home-page: https://github.com/polyaxon/traceml
 Author: Polyaxon, Inc.
 Author-email: contact@polyaxon.com
 Maintainer: Polyaxon, Inc.
 Maintainer-email: contact@polyaxon.com
 License: Apache 2.0
```

### Comparing `traceml-1.1.0rc2/setup.cfg` & `traceml-1.1.0rc3/setup.cfg`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/setup.py` & `traceml-1.1.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/__init__.py` & `traceml-1.1.0rc3/traceml/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/artifacts/__init__.py` & `traceml-1.1.0rc3/traceml/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/artifacts/kinds.py` & `traceml-1.1.0rc3/traceml/artifacts/kinds.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/artifacts/schemas.py` & `traceml-1.1.0rc3/traceml/artifacts/schemas.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/events/__init__.py` & `traceml-1.1.0rc3/traceml/events/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/events/paths.py` & `traceml-1.1.0rc3/traceml/events/paths.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/events/schemas.py` & `traceml-1.1.0rc3/traceml/events/schemas.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/exceptions.py` & `traceml-1.1.0rc3/traceml/exceptions.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/integrations/__init__.py` & `traceml-1.1.0rc3/traceml/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/integrations/fastai.py` & `traceml-1.1.0rc3/traceml/integrations/fastai.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/integrations/fastai_v1.py` & `traceml-1.1.0rc3/traceml/integrations/fastai_v1.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/integrations/hugging_face.py` & `traceml-1.1.0rc3/traceml/integrations/hugging_face.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/integrations/ignite.py` & `traceml-1.1.0rc3/traceml/integrations/ignite.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/integrations/keras.py` & `traceml-1.1.0rc3/traceml/integrations/keras.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/integrations/lightgbm.py` & `traceml-1.1.0rc3/traceml/integrations/lightgbm.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/integrations/pytorch_lightning.py` & `traceml-1.1.0rc3/traceml/integrations/pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/integrations/scikit.py` & `traceml-1.1.0rc3/traceml/integrations/scikit.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/integrations/tensorboard.py` & `traceml-1.1.0rc3/traceml/integrations/tensorboard.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/integrations/tensorflow.py` & `traceml-1.1.0rc3/traceml/integrations/tensorflow.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/integrations/xgboost.py` & `traceml-1.1.0rc3/traceml/integrations/xgboost.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/logger.py` & `traceml-1.1.0rc3/traceml/logger.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/logging/__init__.py` & `traceml-1.1.0rc3/traceml/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/logging/handler.py` & `traceml-1.1.0rc3/traceml/logging/handler.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/logging/parser.py` & `traceml-1.1.0rc3/traceml/logging/parser.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/logging/schemas.py` & `traceml-1.1.0rc3/traceml/logging/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                 value, timestamp = timestamp_search_regex(DATETIME_REGEX, value)
         if isinstance(timestamp, str):
             try:
                 timestamp = parse_datetime(timestamp)
             except Exception as e:
                 raise ValueError("Received an invalid timestamp") from e
 
-        return cls(
+        return cls.construct(
             timestamp=timestamp if timestamp else now(tzinfo=True),
             node=node,
             pod=pod,
             container=container,
             value=value,
         )
 
@@ -104,21 +104,21 @@
 
     def to_csv(self):
         _logs = ["\n{}".format(e.to_csv()) for e in self.logs if e.value]
         return "".join(_logs)
 
     @classmethod
     def should_chunk(cls, logs: List[V1Log]):
-        return len(logs) >= cls.CHUNK_SIZE
+        return len(logs) >= cls._CHUNK_SIZE
 
     @classmethod
     def chunk_logs(cls, logs: List[V1Log]):
         total_size = len(logs)
-        for i in range(0, total_size, cls.CHUNK_SIZE):
-            yield cls(logs=logs[i : i + cls.CHUNK_SIZE])
+        for i in range(0, total_size, cls._CHUNK_SIZE):
+            yield cls(logs=logs[i : i + cls._CHUNK_SIZE])
 
     @classmethod
     def read_csv(cls, data: str, parse_dates: bool = True) -> "V1Logs":
         import numpy as np
         import pandas as pd
 
         csv = validate_csv(data)
@@ -131,17 +131,17 @@
             )
         else:
             df = pd.read_csv(
                 csv,
                 sep=V1Log._SEPARATOR,
             )
 
-        return cls(
+        return cls.construct(
             logs=[
-                V1Log(
+                V1Log.construct(
                     timestamp=i.get("timestamp"),
                     node=i.get("node"),
                     pod=i.get("pod"),
                     container=i.get("container"),
                     value=ujson.loads(i.get("value")).get("_"),
                 )
                 for i in df.replace({np.nan: None}).to_dict(orient="records")
```

### Comparing `traceml-1.1.0rc2/traceml/logging/streamer.py` & `traceml-1.1.0rc3/traceml/logging/streamer.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/pkg.py` & `traceml-1.1.0rc3/traceml/pkg.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 NAME = "traceml"
-VERSION = "1.1.0-rc2"
+VERSION = "1.1.0-rc3"
 DESC = (
     "Engine for ML/Data tracking, visualization, dashboards, and model UI for Polyaxon."
 )
 URL = "https://github.com/polyaxon/traceml"
 AUTHOR = "Polyaxon, Inc."
 EMAIL = "contact@polyaxon.com"
 LICENSE = "Apache 2.0"
```

### Comparing `traceml-1.1.0rc2/traceml/processors/__init__.py` & `traceml-1.1.0rc3/traceml/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/processors/df_processors.py` & `traceml-1.1.0rc3/traceml/processors/df_processors.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/processors/errors.py` & `traceml-1.1.0rc3/traceml/processors/errors.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/processors/events_processors/__init__.py` & `traceml-1.1.0rc3/traceml/processors/events_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/processors/events_processors/events_artifacts_processors.py` & `traceml-1.1.0rc3/traceml/processors/events_processors/events_artifacts_processors.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/processors/events_processors/events_audio_processors.py` & `traceml-1.1.0rc3/traceml/processors/events_processors/events_audio_processors.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/processors/events_processors/events_charts_processors.py` & `traceml-1.1.0rc3/traceml/processors/events_processors/events_charts_processors.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/processors/events_processors/events_image_processors.py` & `traceml-1.1.0rc3/traceml/processors/events_processors/events_image_processors.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/processors/events_processors/events_metrics_processors.py` & `traceml-1.1.0rc3/traceml/processors/events_processors/events_metrics_processors.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/processors/events_processors/events_models_processors.py` & `traceml-1.1.0rc3/traceml/processors/events_processors/events_models_processors.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/processors/events_processors/events_tables_processors.py` & `traceml-1.1.0rc3/traceml/processors/events_processors/events_tables_processors.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/processors/events_processors/events_video_processors.py` & `traceml-1.1.0rc3/traceml/processors/events_processors/events_video_processors.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/processors/gpu_processor.py` & `traceml-1.1.0rc3/traceml/processors/gpu_processor.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/processors/importance_processors.py` & `traceml-1.1.0rc3/traceml/processors/importance_processors.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/processors/logs_processor.py` & `traceml-1.1.0rc3/traceml/processors/logs_processor.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/processors/psutil_processor.py` & `traceml-1.1.0rc3/traceml/processors/psutil_processor.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/processors/units_processors.py` & `traceml-1.1.0rc3/traceml/processors/units_processors.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/serialization/__init__.py` & `traceml-1.1.0rc3/traceml/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/serialization/base.py` & `traceml-1.1.0rc3/traceml/serialization/base.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/serialization/writer.py` & `traceml-1.1.0rc3/traceml/serialization/writer.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/summary/__init__.py` & `traceml-1.1.0rc3/traceml/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/summary/df.py` & `traceml-1.1.0rc3/traceml/summary/df.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/tracking/__init__.py` & `traceml-1.1.0rc3/traceml/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/tracking/run.py` & `traceml-1.1.0rc3/traceml/tracking/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             project=project,
             run_uuid=run_uuid,
             client=client,
             is_offline=is_offline,
             no_op=no_op,
         )
         track_logs = track_logs if track_logs is not None else self._is_offline
-        self._logs_history = V1Logs(logs=[])
+        self._logs_history = V1Logs.construct(logs=[])
         self._artifacts_path = None
         self._outputs_path = None
         self._event_logger = None
         self._resource_logger = None
         self._sidecar = None
         self._exit_handler = None
         self._store_path = None
@@ -257,15 +257,15 @@
     def _add_logs(self, log: V1Log):
         if not log:
             return
         self._logs_history.logs.append(log)
         if V1Logs.should_chunk(self._logs_history.logs):
             self._persist_logs_history()
             # Reset
-            self._logs_history = V1Logs(logs=[])
+            self._logs_history = V1Logs.construct(logs=[])
 
     def create(self, **kwargs):
         raise NotImplementedError(
             "The tracking `Run` subclass does not allow to call "
             "`create` method manually, please create a new instance of `Run` with `is_new=True`"
         )
```

### Comparing `traceml-1.1.0rc2/traceml/vendor/__init__.py` & `traceml-1.1.0rc3/traceml/vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/vendor/matplotlylib/mplexporter/exporter.py` & `traceml-1.1.0rc3/traceml/vendor/matplotlylib/mplexporter/exporter.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/vendor/matplotlylib/mplexporter/renderers/base.py` & `traceml-1.1.0rc3/traceml/vendor/matplotlylib/mplexporter/renderers/base.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/vendor/matplotlylib/mplexporter/renderers/fake_renderer.py` & `traceml-1.1.0rc3/traceml/vendor/matplotlylib/mplexporter/renderers/fake_renderer.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/vendor/matplotlylib/mplexporter/renderers/vega_renderer.py` & `traceml-1.1.0rc3/traceml/vendor/matplotlylib/mplexporter/renderers/vega_renderer.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/vendor/matplotlylib/mplexporter/renderers/vincent_renderer.py` & `traceml-1.1.0rc3/traceml/vendor/matplotlylib/mplexporter/renderers/vincent_renderer.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/vendor/matplotlylib/mplexporter/tools.py` & `traceml-1.1.0rc3/traceml/vendor/matplotlylib/mplexporter/tools.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/vendor/matplotlylib/mplexporter/utils.py` & `traceml-1.1.0rc3/traceml/vendor/matplotlylib/mplexporter/utils.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/vendor/matplotlylib/mpltools.py` & `traceml-1.1.0rc3/traceml/vendor/matplotlylib/mpltools.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/vendor/matplotlylib/renderer.py` & `traceml-1.1.0rc3/traceml/vendor/matplotlylib/renderer.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/vendor/matplotlylib/tools.py` & `traceml-1.1.0rc3/traceml/vendor/matplotlylib/tools.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/vendor/pynvml.py` & `traceml-1.1.0rc3/traceml/vendor/pynvml.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/visualization/__init__.py` & `traceml-1.1.0rc3/traceml/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml/visualization/run_plot.py` & `traceml-1.1.0rc3/traceml/visualization/run_plot.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc2/traceml.egg-info/PKG-INFO` & `traceml-1.1.0rc3/traceml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceml
-Version: 1.1.0rc2
+Version: 1.1.0rc3
 Summary: Engine for ML/Data tracking, visualization, dashboards, and model UI for Polyaxon.
 Home-page: https://github.com/polyaxon/traceml
 Author: Polyaxon, Inc.
 Author-email: contact@polyaxon.com
 Maintainer: Polyaxon, Inc.
 Maintainer-email: contact@polyaxon.com
 License: Apache 2.0
```

### Comparing `traceml-1.1.0rc2/traceml.egg-info/SOURCES.txt` & `traceml-1.1.0rc3/traceml.egg-info/SOURCES.txt`

 * *Files identical despite different names*


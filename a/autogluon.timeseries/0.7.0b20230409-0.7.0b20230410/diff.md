# Comparing `tmp/autogluon.timeseries-0.7.0b20230409.tar.gz` & `tmp/autogluon.timeseries-0.7.0b20230410.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-0.7.0b20230409.tar", last modified: Sun Apr  9 09:03:57 2023, max compression
+gzip compressed data, was "autogluon.timeseries-0.7.0b20230410.tar", last modified: Mon Apr 10 09:04:29 2023, max compression
```

## Comparing `autogluon.timeseries-0.7.0b20230409.tar` & `autogluon.timeseries-0.7.0b20230410.tar`

### file list

```diff
@@ -1,69 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:03:57.199082 autogluon.timeseries-0.7.0b20230409/
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-04-09 09:03:57.199082 autogluon.timeseries-0.7.0b20230409/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 09:03:57.199082 autogluon.timeseries-0.7.0b20230409/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:03:57.191082 autogluon.timeseries-0.7.0b20230409/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:03:57.191082 autogluon.timeseries-0.7.0b20230409/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:03:57.191082 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:03:57.191082 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:03:57.191082 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:03:57.195082 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:03:57.195082 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19622 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:03:57.195082 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17352 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:03:57.195082 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:03:57.195082 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18951 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:03:57.195082 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/gluonts/mx/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/gluonts/mx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/gluonts/mx/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/gluonts/mx/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:03:57.195082 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:03:57.195082 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12125 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/local/statsforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/local/statsmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    41780 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:03:57.195082 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38831 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:03:57.199082 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/utils/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-09 09:03:21.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-09 09:03:57.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:03:57.191082 autogluon.timeseries-0.7.0b20230409/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-04-09 09:03:57.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-09 09:03:57.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 09:03:57.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 09:03:57.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-09 09:03:57.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 09:03:57.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 09:03:57.000000 autogluon.timeseries-0.7.0b20230409/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:04:29.151851 autogluon.timeseries-0.7.0b20230410/
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-04-10 09:04:29.151851 autogluon.timeseries-0.7.0b20230410/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 09:04:29.151851 autogluon.timeseries-0.7.0b20230410/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:04:29.143850 autogluon.timeseries-0.7.0b20230410/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:04:29.147851 autogluon.timeseries-0.7.0b20230410/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:04:29.147851 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:04:29.147851 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:04:29.147851 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37101 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:04:29.147851 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:04:29.147851 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19803 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:04:29.147851 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17322 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:04:29.147851 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:04:29.147851 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18951 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:04:29.151851 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/gluonts/mx/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/gluonts/mx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/gluonts/mx/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/gluonts/mx/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:04:29.151851 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:04:29.151851 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/local/statsforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/local/statsmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:04:29.151851 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42503 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:04:29.151851 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40270 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:04:29.151851 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/utils/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-10 09:03:47.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-10 09:04:28.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:04:29.147851 autogluon.timeseries-0.7.0b20230410/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-04-10 09:04:29.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-10 09:04:29.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 09:04:29.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-10 09:04:29.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-10 09:04:29.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-10 09:04:29.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 09:04:29.000000 autogluon.timeseries-0.7.0b20230410/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-0.7.0b20230409/PKG-INFO` & `autogluon.timeseries-0.7.0b20230410/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.0b20230409
+Version: 0.7.0b20230410
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.0b20230409/setup.py` & `autogluon.timeseries-0.7.0b20230410/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/__init__.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,18 +8,11 @@
         "hyperparameters": "best_quality",
         "hyperparameter_tune_kwargs": {
             "scheduler": "local",
             "searcher": "auto",
             "num_trials": 10,
         },
     },
-    high_quality={
-        "hyperparameters": "high_quality",
-        "hyperparameter_tune_kwargs": {
-            "scheduler": "local",
-            "searcher": "auto",
-            "num_trials": 5,
-        },
-    },
+    high_quality={"hyperparameters": "high_quality"},
     medium_quality={"hyperparameters": "medium_quality"},
     fast_training={"hyperparameters": "local_only"},
 )
```

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import copy
 import itertools
-import warnings
 from collections.abc import Iterable
 from typing import Any, List, Optional, Tuple, Type
 
 import numpy as np
 import pandas as pd
 from joblib.parallel import Parallel, delayed
 from pandas.core.internals import ArrayManager, BlockManager
@@ -813,7 +812,46 @@
         past_data = self.slice_by_timestep(None, -prediction_length)
         if known_covariates_names is not None and len(known_covariates_names) > 0:
             future_data = self.slice_by_timestep(-prediction_length, None)
             known_covariates = future_data[known_covariates_names]
         else:
             known_covariates = None
         return past_data, known_covariates
+
+    def train_test_split(
+        self,
+        prediction_length: int,
+        end_index: Optional[int] = None,
+        suffix: Optional[str] = None,
+    ) -> Tuple[TimeSeriesDataFrame, TimeSeriesDataFrame]:
+        """Generate a train/test split from the given dataset.
+        This method can be used to generate splits for multi-window backtesting.
+
+        Parameters
+        ----------
+        prediction_length : int
+            Number of time steps in a single evaluation window.
+        end_index : int, optional
+            If given, all time series will be shortened up to ``end_idx`` before the train/test splitting. In other
+            words, test data will include the slice ``[:end_index]`` of each time series, and train data will include
+            the slice ``[:end_index - prediction_length]``.
+        suffix : str, optional
+            Suffix appended to all entries in the ``item_id`` index level.
+
+        Returns
+        -------
+        train_data : TimeSeriesDataFrame
+            Train portion of the data. Contains the slice ``[:-prediction_length]`` of each time series in ``test_data``.
+        test_data : TimeSeriesDataFrame
+            Test portion of the data. Contains the slice ``[:end_idx]`` of each time series in the original dataset.
+        """
+        test_data = self.slice_by_timestep(None, end_index)
+        train_data = test_data.slice_by_timestep(None, -prediction_length)
+
+        if suffix is not None:
+            for data in [train_data, test_data]:
+                new_item_id = data.index.levels[0].astype(str) + suffix
+                data.index = data.index.set_levels(levels=new_item_id, level=0)
+                if data.static_features is not None:
+                    data.static_features.index = data.static_features.index.astype(str)
+                    data.static_features.index += suffix
+        return train_data, test_data
```

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/evaluator.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/evaluator.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/learner.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,30 +27,28 @@
         path_context: str,
         target: str = "target",
         known_covariates_names: Optional[List[str]] = None,
         trainer_type: Type[AbstractTimeSeriesTrainer] = AutoTimeSeriesTrainer,
         eval_metric: Optional[str] = None,
         eval_metric_seasonal_period: Optional[int] = None,
         prediction_length: int = 1,
-        validation_splitter: AbstractTimeSeriesSplitter = LastWindowSplitter(),
         ignore_time_index: bool = False,
         **kwargs,
     ):
         super().__init__(path_context=path_context)
         self.eval_metric: str = TimeSeriesEvaluator.check_get_evaluation_metric(eval_metric)
         self.eval_metric_seasonal_period = eval_metric_seasonal_period
         self.trainer_type = trainer_type
         self.target = target
         self.known_covariates_names = [] if known_covariates_names is None else known_covariates_names
         self.prediction_length = prediction_length
         self.quantile_levels = kwargs.get(
             "quantile_levels",
             kwargs.get("quantiles", [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9]),
         )
-        self.validation_splitter = validation_splitter
         self.ignore_time_index = ignore_time_index
 
         self.feature_generator = TimeSeriesFeatureGenerator(
             target=self.target, known_covariates_names=self.known_covariates_names
         )
 
     def load_trainer(self) -> AbstractTimeSeriesTrainer:
@@ -76,14 +74,15 @@
     def _fit(
         self,
         train_data: TimeSeriesDataFrame,
         val_data: Optional[TimeSeriesDataFrame] = None,
         hyperparameters: Union[str, Dict] = None,
         hyperparameter_tune_kwargs: Optional[Union[str, dict]] = None,
         time_limit: Optional[int] = None,
+        num_val_windows: int = 1,
         **kwargs,
     ) -> None:
         self._time_limit = time_limit
         time_start = time.time()
 
         logger.debug(
             "Beginning AutoGluon training with TimeSeriesLearner "
@@ -97,36 +96,27 @@
                 "\tThis metric's sign has been flipped to adhere to being 'higher is better'. "
                 "The reported score can be multiplied by -1 to get the metric value.",
             )
         train_data = self.feature_generator.fit_transform(train_data, data_frame_name="train_data")
         if val_data is not None:
             val_data = self.feature_generator.transform(val_data, data_frame_name="tuning_data")
 
-        # Train / validation split
-        if val_data is None:
-            logger.warning(
-                "tuning_data is None. "
-                + self.validation_splitter.describe_validation_strategy(prediction_length=self.prediction_length)
-            )
-            train_data, val_data = self.validation_splitter.split(
-                ts_dataframe=train_data, prediction_length=self.prediction_length
-            )
-
         trainer_init_kwargs = kwargs.copy()
         trainer_init_kwargs.update(
             dict(
                 path=self.model_context,
                 prediction_length=self.prediction_length,
                 eval_metric=self.eval_metric,
                 eval_metric_seasonal_period=self.eval_metric_seasonal_period,
                 target=self.target,
                 quantile_levels=self.quantile_levels,
                 verbosity=kwargs.get("verbosity", 2),
                 enable_ensemble=kwargs.get("enable_ensemble", True),
                 metadata=self.feature_generator.covariate_metadata,
+                num_val_windows=num_val_windows,
             )
         )
         self.trainer = self.trainer_type(**trainer_init_kwargs)
         self.trainer_path = self.trainer.path
         self.save()
 
         self.trainer.fit(
```

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -362,27 +362,31 @@
     def score_and_cache_oof(
         self,
         val_data: TimeSeriesDataFrame,
         store_val_score: bool = False,
         store_predict_time: bool = False,
     ) -> None:
         """Compute val_score, predict_time and cache out-of-fold (OOF) predictions."""
-        if self.val_score is not None or self.predict_time is not None or self._oof_predictions is not None:
-            raise ValueError(f"Model {self.name} has already been scored on OOF data!")
-
         past_data, known_covariates = val_data.get_model_inputs_for_scoring(
             prediction_length=self.prediction_length, known_covariates_names=self.metadata.known_covariates_real
         )
         predict_start_time = time.time()
         self._oof_predictions = self.predict(past_data, known_covariates=known_covariates)
         if store_predict_time:
             self.predict_time = time.time() - predict_start_time
         if store_val_score:
             self.val_score = self._score_with_predictions(val_data, self._oof_predictions)
 
+    def _get_hpo_train_fn_kwargs(self, **train_fn_kwargs) -> dict:
+        """Update kwargs passed to model_trial depending on the model configuration.
+
+        These kwargs need to be updated, for example, by MultiWindowBacktestingModel.
+        """
+        return train_fn_kwargs
+
     def _hyperparameter_tune(
         self,
         train_data: TimeSeriesDataFrame,
         val_data: TimeSeriesDataFrame,
         hpo_executor: HpoExecutor,
         **kwargs,
     ):
@@ -402,16 +406,18 @@
         train_path = os.path.join(self.path, dataset_train_filename)
         save_pkl.save(path=train_path, object=train_data)
 
         dataset_val_filename = "dataset_val.pkl"
         val_path = os.path.join(self.path, dataset_val_filename)
         save_pkl.save(path=val_path, object=val_data)
 
-        fit_kwargs = dict()
-        train_fn_kwargs = dict(
+        fit_kwargs = dict(
+            num_val_windows=kwargs.get("num_val_windows", 1),
+        )
+        train_fn_kwargs = self._get_hpo_train_fn_kwargs(
             model_cls=self.__class__,
             init_params=self.get_params(),
             time_start=time_start,
             time_limit=hpo_executor.time_limit,
             fit_kwargs=fit_kwargs,
             train_path=train_path,
             val_path=val_path,
```

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,23 +14,26 @@
     args,
     model_cls,
     init_params,
     train_path,
     val_path,
     time_start,
     hpo_executor,
+    is_bagged_model=False,
     reporter=None,  # reporter only used by custom strategy, hence optional
     time_limit=None,
     fit_kwargs=None,
 ):
     """Runs a single trial of a hyperparameter tuning. Replaces
     `core.models.abstract.model_trial.model_trial` for timeseries models.
     """
     try:
-        model = init_model(args, model_cls, init_params, backend=hpo_executor.executor_type)
+        model = init_model(
+            args, model_cls, init_params, backend=hpo_executor.executor_type, is_bagged_model=is_bagged_model
+        )
         model.set_contexts(path_context=model.path_root + model.name + os.path.sep)
 
         train_data = load_pkl.load(train_path)
         val_data = load_pkl.load(val_path)
 
         eval_metric = model.eval_metric
```

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,19 +36,18 @@
     Other Parameters
     ----------------
     max_train_size : int, default = 1_000_000
         Maximum number of rows in the training and validation sets. If the number of rows in train or validation data
         exceeds ``max_train_size``, then ``max_train_size`` many rows are subsampled from the dataframe.
     tabular_hyperparameters : Dict[Dict[str, Any]], optional
         Hyperparameters dictionary passed to `TabularPredictor.fit`. Contains the names of models that should be fit.
-        Defaults to ``{"XGB": {}, "CAT": {}, "GBM" :{}}``.
+        Defaults to ``{"CAT": {}, "GBM" :{}}``.
     """
 
     default_tabular_hyperparameters = {
-        "XGB": {},
         "CAT": {},
         "GBM": {},
     }
 
     PREDICTION_BATCH_SIZE = 100_000
 
     TIMESERIES_METRIC_TO_TABULAR_METRIC = {
```

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/gluonts/mx/__init__.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/gluonts/mx/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/gluonts/mx/callback.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/gluonts/mx/callback.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/gluonts/mx/models.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/gluonts/mx/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     return hash_per_timestep.groupby(level=ITEMID, sort=False).apply(lambda x: hashlib.md5(x.values).hexdigest())
 
 
 class AbstractLocalModel(AbstractTimeSeriesModel):
     allowed_local_model_args: List[str] = []
     # Use 50% of the cores since some models rely on parallel ops and are actually slower if n_jobs=-1
     DEFAULT_N_JOBS: Union[float, int] = 0.5
+    MAX_TS_LENGTH: Optional[int] = None
 
     def __init__(
         self,
         freq: Optional[str] = None,
         prediction_length: int = 1,
         path: Optional[str] = None,
         name: Optional[str] = None,
@@ -106,14 +107,17 @@
             quantile_levels = self.quantile_levels
 
         if self.freq != data.freq:
             raise RuntimeError(
                 f"{self.name} has frequency '{self.freq}', which doesn't match the frequency "
                 f"of the dataset '{data.freq}'."
             )
+        if self.MAX_TS_LENGTH is not None:
+            logger.debug(f"Shortening all time series to at most {self.MAX_TS_LENGTH}")
+            data = data.groupby(level=ITEMID, sort=False).tail(self.MAX_TS_LENGTH)
 
         self._fit_and_cache_predictions(data, quantile_levels=quantile_levels)
         item_id_to_prediction = {}
         for item_id, ts_hash in hash_ts_dataframe_items(data).items():
             item_id_to_prediction[item_id] = self._cached_predictions[ts_hash]
         predictions_df = pd.concat(item_id_to_prediction)
         predictions_df.index.rename([ITEMID, TIMESTAMP], inplace=True)
```

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List, Type, Union
 
 import pandas as pd
 
 from autogluon.core.utils.exceptions import TimeLimitExceeded
 from autogluon.timeseries.dataset.ts_dataframe import ITEMID, TIMESTAMP, TimeSeriesDataFrame
 from autogluon.timeseries.models.local.abstract_local_model import AbstractLocalModel, hash_ts_dataframe_items
-from autogluon.timeseries.utils.warning_filters import statsmodels_warning_filter
+from autogluon.timeseries.utils.warning_filters import statsmodels_joblib_warning_filter, statsmodels_warning_filter
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractStatsForecastModel(AbstractLocalModel):
     """Wrapper for StatsForecast models.
 
@@ -85,15 +85,15 @@
                 level = round(abs(q - 0.5) * 200, 1)
                 suffix = "lo" if q < 0.5 else "hi"
                 levels.append(level)
                 new_column_names[f"{model_name}-{suffix}-{level}"] = str(q)
             levels = sorted(list(set(levels)))
             chosen_columns = list(new_column_names.values())
 
-            with statsmodels_warning_filter():
+            with statsmodels_warning_filter(), statsmodels_joblib_warning_filter():
                 raw_predictions = sf.forecast(
                     df=self._to_statsforecast_dataframe(data_to_fit),
                     h=self.prediction_length,
                     level=levels,
                 ).reset_index()
             predictions = raw_predictions.rename(new_column_names, axis=1)[chosen_columns].set_index(TIMESTAMP)
             item_ids = predictions.pop(ITEMID)
@@ -181,14 +181,15 @@
         "stationary",
         "seasonal",
         "approximatio",
         "allowdrift",
         "allowmean",
         "seasonal_period",
     ]
+    MAX_TS_LENGTH = 3000
 
     def _update_local_model_args(self, local_model_args: dict, data: TimeSeriesDataFrame) -> dict:
         local_model_args.setdefault("approximation", True)
         local_model_args.setdefault("allowmean", True)
         return local_model_args
 
     def get_model_type(self):
```

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/local/statsmodels.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/local/statsmodels.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,14 +196,15 @@
         "seasonal_order",
         "seasonal_period",
         "trend",
         "enforce_stationarity",
         "enforce_invertibility",
         "maxiter",
     ]
+    MAX_TS_LENGTH = 3000
 
     def _update_local_model_args(
         self, local_model_args: Dict[str, Any], data: TimeSeriesDataFrame, **kwargs
     ) -> Dict[str, Any]:
         local_model_args.setdefault("trend", "c")
         local_model_args.setdefault("order", (1, 1, 1))
         local_model_args.setdefault("maxiter", 50)
```

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/models/presets.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,23 +16,23 @@
     NaiveModel,
     SeasonalNaiveModel,
     SimpleFeedForwardModel,
     TemporalFusionTransformerModel,
     ThetaModel,
 )
 from .abstract import AbstractTimeSeriesModel, AbstractTimeSeriesModelFactory
+from .multi_window.multi_window_model import MultiWindowBacktestingModel
 
 logger = logging.getLogger(__name__)
 
 # define the model zoo with their aliases
 MODEL_TYPES = dict(
     SimpleFeedForward=SimpleFeedForwardModel,
     DeepAR=DeepARModel,
     TemporalFusionTransformer=TemporalFusionTransformerModel,
-    # Prophet=ProphetModel,
     ETS=ETSModel,
     ARIMA=ARIMAModel,
     Theta=ThetaModel,
     AutoGluonTabular=AutoGluonTabularModel,
     Naive=NaiveModel,
     SeasonalNaive=SeasonalNaiveModel,
     AutoETS=AutoETSModel,
@@ -111,17 +111,15 @@
         "high_quality": {
             "Naive": {},
             "SeasonalNaive": {},
             "ARIMA": {},
             "ETS": {},
             "AutoETS": {},
             "AutoARIMA": {},
-            "Theta": {
-                "deseasonalize": ag.Categorical(True, False),
-            },
+            "Theta": {},
             "AutoGluonTabular": {},
             "DeepAR": {
                 "context_length": context_length,
             },
             "SimpleFeedForward": {
                 "context_length": context_length,
             },
@@ -131,17 +129,15 @@
             "Naive": {},
             "SeasonalNaive": {},
             "ARIMA": {},
             "ETS": {},
             "AutoETS": {},
             "AutoARIMA": {},
             "DynamicOptimizedTheta": {},
-            "Theta": {
-                "deseasonalize": ag.Categorical(True, False),
-            },
+            "Theta": {},
             "AutoGluonTabular": {},
             "DeepAR": {
                 "context_length": context_length,
                 "num_layers": ag.Int(1, 3, default=2),
                 "hidden_size": ag.Int(40, 80, default=40),
             },
             "SimpleFeedForward": {
@@ -174,14 +170,15 @@
     prediction_length: int,
     path: str,
     eval_metric: str,
     eval_metric_seasonal_period: Optional[int],
     hyperparameters: Union[str, Dict],
     hyperparameter_tune: bool,
     invalid_model_names: List[str],
+    multi_window: bool = False,
     **kwargs,
 ):
     """
     Create a list of models according to hyperparameters. If hyperparamaters=None,
     will create models according to presets.
     """
     models = []
@@ -245,14 +242,17 @@
 
         model_type_kwargs.pop("name", None)
         increment = 1
         while model.name in all_assigned_names:
             increment += 1
             model = model_type(name=f"{name_stem}_{increment}", **model_type_kwargs)
 
+        if multi_window:
+            model = MultiWindowBacktestingModel(model_base=model, name=model.name, **model_type_kwargs)
+
         all_assigned_names.add(model.name)
         models.append(model)
 
     return models
 
 
 def contains_searchspace(model_hyperparameters: Dict[str, Any]) -> bool:
```

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/predictor.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from autogluon.common.utils.utils import setup_outputdir
 from autogluon.core.utils.decorators import apply_presets
 from autogluon.core.utils.loaders import load_pkl
 from autogluon.core.utils.savers import save_pkl
 from autogluon.timeseries.configs import TIMESERIES_PRESETS_CONFIGS
 from autogluon.timeseries.dataset.ts_dataframe import ITEMID, TIMESTAMP, TimeSeriesDataFrame
 from autogluon.timeseries.learner import AbstractLearner, TimeSeriesLearner
-from autogluon.timeseries.splitter import AbstractTimeSeriesSplitter, LastWindowSplitter, MultiWindowSplitter
 from autogluon.timeseries.trainer import AbstractTimeSeriesTrainer
 from autogluon.timeseries.utils.random import set_random_seed
 
 logger = logging.getLogger(__name__)
 
 SUPPORTED_FREQUENCIES = {"D", "W", "M", "Q", "A", "Y", "H", "T", "min", "S"}
 
@@ -90,22 +89,14 @@
         If using ``logging``, you can alternatively control amount of information printed via ``logger.setLevel(L)``,
         where ``L`` ranges from 0 to 50 (Note: higher values of ``L`` correspond to fewer print statements, opposite
         of verbosity levels).
     ignore_time_index : bool, default = False
         If True, the predictor will ignore the datetime indexes during both training and testing, and will replace
         the data indexes with dummy timestamps in second frequency. In this case, the forecast output time indexes will
         be arbitrary values, and seasonality will be turned off for local models.
-    validation_splitter : Union[str, AbstractTimeSeriesSplitter], default = "last_window"
-        Strategy for splitting ``train_data`` into training and validation parts during
-        :meth:`~autogluon.timeseries.TimeSeriesPredictor.fit`. If ``tuning_data`` is passed to
-        :meth:`~autogluon.timeseries.TimeSeriesPredictor.fit`, validation_splitter is ignored. Possible choices:
-
-        - ``"last_window"``: use last ``prediction_length`` time steps of each time series for validation.
-        - ``"multi_window"``: use last 3 non-overlapping windows of length ``prediction_length`` of each time series for validation.
-        - object of type :class:`~autogluon.timeseries.splitter.AbstractTimeSeriesSplitter` implementing a custom splitting strategy (for advanced users only).
     learner_type : AbstractLearner, default = TimeSeriesLearner
         A class which inherits from ``AbstractLearner``. The learner specifies the inner logic of the
         ``TimeSeriesPredictor``.
     learner_kwargs : dict, optional
         Keyword arguments to send to the learner (for advanced users only). Options include ``trainer_type``, a
         class inheriting from ``AbstractTrainer`` which controls training of multiple models.
         If ``path`` and ``eval_metric`` are re-specified within ``learner_kwargs``, these are ignored.
@@ -124,19 +115,19 @@
         prediction_length: int = 1,
         eval_metric: Optional[str] = None,
         eval_metric_seasonal_period: Optional[int] = None,
         path: Optional[str] = None,
         verbosity: int = 2,
         quantile_levels: Optional[List[float]] = None,
         ignore_time_index: bool = False,
-        validation_splitter: Union[str, AbstractTimeSeriesSplitter] = "last_window",
         learner_type: Type[AbstractLearner] = TimeSeriesLearner,
         learner_kwargs: Optional[dict] = None,
         label: Optional[str] = None,
         quantiles: Optional[List[float]] = None,
+        validation_splitter: Optional[Any] = None,
     ):
         self.verbosity = verbosity
         set_logger_verbosity(self.verbosity, logger=logger)
         self.path = setup_outputdir(path)
 
         self.ignore_time_index = ignore_time_index
         if target is not None and label is not None:
@@ -160,54 +151,42 @@
         self.eval_metric_seasonal_period = eval_metric_seasonal_period
         if quantile_levels is not None and quantiles is not None:
             raise ValueError(
                 "Both `quantile_levels` and `quantiles` are specified. Please specify at most one of these arguments."
             )
         self.quantile_levels = quantile_levels or quantiles or [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9]
 
-        if validation_splitter == "last_window":
-            splitter = LastWindowSplitter()
-        elif validation_splitter == "multi_window":
-            splitter = MultiWindowSplitter()
-        elif isinstance(validation_splitter, AbstractTimeSeriesSplitter):
-            splitter = validation_splitter
-        else:
-            raise ValueError(
-                f"`validation_splitter` must be one of 'last_window', 'multi_window', or an object of type "
-                f"`autogluon.timeseries.splitter.AbstractTimeSeriesSplitter` "
-                f"(received {validation_splitter} of type {type(validation_splitter)})."
+        if validation_splitter is not None:
+            warnings.warn(
+                "validation_splitter argument has been deprecated as of v0.8.0. "
+                "Please user the `num_val_windows` argument of `TimeSeriesPredictor.fit` instead."
             )
 
         if learner_kwargs is None:
             learner_kwargs = {}
         learner_kwargs = learner_kwargs.copy()
         learner_kwargs.update(
             dict(
                 path_context=self.path,
                 eval_metric=eval_metric,
                 eval_metric_seasonal_period=eval_metric_seasonal_period,
                 target=self.target,
                 known_covariates_names=self.known_covariates_names,
                 prediction_length=self.prediction_length,
                 quantile_levels=self.quantile_levels,
-                validation_splitter=splitter,
                 ignore_time_index=ignore_time_index,
             )
         )
         self._learner: AbstractLearner = learner_type(**learner_kwargs)
         self._learner_type = type(self._learner)
 
     @property
     def _trainer(self) -> AbstractTimeSeriesTrainer:
         return self._learner.load_trainer()  # noqa
 
-    @property
-    def validation_splitter(self) -> AbstractTimeSeriesSplitter:
-        return self._learner.validation_splitter
-
     def _check_and_prepare_data_frame(self, df: Union[TimeSeriesDataFrame, pd.DataFrame]) -> TimeSeriesDataFrame:
         """Ensure that TimeSeriesDataFrame has a frequency, or replace its time index with a dummy if
         ``self.ignore_time_index`` is True.
         """
         if df is None:
             return df
         if not isinstance(df, TimeSeriesDataFrame):
@@ -228,14 +207,15 @@
         is_sorted = timestamps.groupby(level=ITEMID, sort=False).apply(lambda x: x.is_monotonic_increasing).all()
         if not is_sorted:
             warnings.warn(
                 "Provided data contains timestamps that are not sorted chronologically. "
                 "This will lead to TimeSeriesPredictor not working as intended. "
                 "Please make sure that the timestamps are sorted in increasing order for all time series."
             )
+        # TODO: Make sure that entries for each item_id are contiguous -> https://github.com/autogluon/autogluon/issues/3036
         if df.freq is None:
             raise ValueError(
                 "Frequency not provided and cannot be inferred. This is often due to the "
                 "time index of the data being irregularly sampled. Please ensure that the "
                 "data set used has a uniform time index, or create the `TimeSeriesPredictor` "
                 "setting `ignore_time_index=True`."
             )
@@ -251,29 +231,70 @@
             )
         if df.isna().values.any():
             raise ValueError(
                 "TimeSeriesPredictor does not yet support missing values. "
                 "Please make sure that the provided data contains no NaNs."
             )
         if (df.num_timesteps_per_item() <= 2).any():
-            warnings.warn(
-                "Detected time series with length <= 2 in data. "
-                "Please remove them from the dataset or TimeSeriesPredictor likely won't work as intended."
-            )
+            # Time series with length <= 2 make frequency inference impossible
+            raise ValueError("Detected time series with length <= 2 in data. Please remove them from the dataset.")
         return df
 
+    def _validate_num_val_windows(
+        self,
+        train_data: TimeSeriesDataFrame,
+        tuning_data: Optional[TimeSeriesDataFrame],
+        num_val_windows: int,
+    ) -> int:
+        """Check if given num_val_windows is suitable for given data and validate length of training time series.
+
+        Returns
+        -------
+        num_val_windows : int
+            Number of cross validation windows adjusted based on the length of training time series.
+        """
+        shortest_ts_length = train_data.num_timesteps_per_item().min()
+        if tuning_data is None:
+            recommended_ts_length = 2 * self.prediction_length + 1
+            recommended_ts_length_str = "2 * prediction_length + 1"
+        else:
+            recommended_ts_length = self.prediction_length + 1
+            recommended_ts_length_str = "prediction_length + 1"
+
+        if shortest_ts_length < recommended_ts_length:
+            logger.warning(
+                f"\nIt is recommended that all time series in train_data have length >= {recommended_ts_length_str} "
+                f"(at least {recommended_ts_length}). "
+                "Otherwise the predictor may not work as expected. "
+                "\nPlease reduce prediction_length or provide longer time series as train_data. "
+            )
+
+        # Ensure that after splitting off the last prediction_length timesteps all time series have length >= 1
+        max_possible_num_val_windows = int((shortest_ts_length - 1) / self.prediction_length)
+        if num_val_windows > max_possible_num_val_windows:
+            logger.warning(
+                f"\nTime series in train_data are too short for the given num_val_windows = {num_val_windows}. "
+                f"Setting num_val_windows = {max_possible_num_val_windows}"
+            )
+            num_val_windows = max_possible_num_val_windows
+        if num_val_windows == 0 and tuning_data is None:
+            raise ValueError("Training is impossible because num_val_windows = 0 and no tuning_data is provided")
+
+        return num_val_windows
+
     @apply_presets(TIMESERIES_PRESETS_CONFIGS)
     def fit(
         self,
         train_data: Union[TimeSeriesDataFrame, pd.DataFrame],
         tuning_data: Optional[Union[TimeSeriesDataFrame, pd.DataFrame]] = None,
         time_limit: Optional[int] = None,
         presets: Optional[str] = None,
         hyperparameters: Dict[Union[str, Type], Any] = None,
         hyperparameter_tune_kwargs: Optional[Union[str, Dict]] = None,
+        num_val_windows: int = 1,
         enable_ensemble: bool = True,
         random_seed: Optional[int] = None,
         verbosity: Optional[int] = None,
     ) -> "TimeSeriesPredictor":
         """Fit probabilistic forecasting models to the given time series dataset.
 
         Parameters
@@ -302,22 +323,20 @@
             to a ``TimeSeriesDataFrame``.
 
         tuning_data : Union[TimeSeriesDataFrame, pd.DataFrame], optional
             Data reserved for model selection and hyperparameter tuning, rather than training individual models. Also
             used to compute the validation scores. Note that only the last ``prediction_length`` time steps of each
             time series are used for computing the validation score.
 
+            If ``tuning_data`` is provided, multi-window backtesting on training data will be disabled and the
+            ``num_val_windows`` argument will be ignored.
+
             Leaving this argument empty and letting AutoGluon automatically generate the validation set from
             ``train_data`` is a good default.
 
-            If not provided, AutoGluon will split :attr:`train_data` into training and tuning subsets using
-            ``validation_splitter``. If ``tuning_data`` is provided, ``validation_splitter`` will be ignored.
-            See the description of ``validation_splitter`` in the docstring for
-            :class:`~autogluon.timeseries.TimeSeriesPredictor` for more details.
-
             If ``known_covariates_names`` were specified when creating the predictor, ``tuning_data`` must also include
             the columns listed in ``known_covariates_names`` with the covariates values aligned with the target time
             series.
 
             If ``train_data`` has past covariates or static features, ``tuning_data`` must have also include them (with
             same columns names and dtypes).
 
@@ -419,15 +438,17 @@
                     ...
                     hyperparameter_tune_kwargs={
                         "scheduler": "local",
                         "searcher": "auto",
                         "num_trials": 5,
                     }
                 )
-
+        num_val_windows : int, default = 1
+            Number of backtests done on ``train_data`` for each trained model to estimate the validation performance.
+            When ``num_val_windows = k``, training time is increased roughly by a factor of ``k``.
         enable_ensemble : bool, default = True
             If True, the ``TimeSeriesPredictor`` will fit a simple weighted ensemble on top of the models specified via
             ``hyperparameters``.
         random_seed : int, optional
             If provided, fixes the seed of the random number generator for all models. This guarantees reproducible
             results for most models (except those trained on GPU because of the non-determinism of GPU operations).
         verbosity : int, optional
@@ -441,65 +462,65 @@
 
         if hyperparameters is None:
             hyperparameters = "default"
 
         train_data = self._check_and_prepare_data_frame(train_data)
         tuning_data = self._check_and_prepare_data_frame(tuning_data)
 
-        if (train_data.num_timesteps_per_item() <= 2 * self.prediction_length).any():
-            warnings.warn(
-                "Detected short time series in train_data. "
-                "For best performance, all training time series should have length >= 2 * prediction_length + 1"
-                f"(at least {2 * self.prediction_length + 1})."
-            )
-
         if verbosity is None:
             verbosity = self.verbosity
         set_logger_verbosity(verbosity)
 
         fit_args = dict(
             prediction_length=self.prediction_length,
             target=self.target,
             time_limit=time_limit,
             evaluation_metric=self.eval_metric,
             hyperparameters=hyperparameters,
             hyperparameter_tune_kwargs=hyperparameter_tune_kwargs,
+            num_val_windows=num_val_windows,
             enable_ensemble=enable_ensemble,
             random_seed=random_seed,
             verbosity=verbosity,
         )
         logger.info("================ TimeSeriesPredictor ================")
         logger.info("TimeSeriesPredictor.fit() called")
         if presets is not None:
             logger.info(f"Setting presets to: {presets}")
         logger.info("Fitting with arguments:")
         logger.info(f"{pprint.pformat(fit_args)}")
         logger.info(
             f"Provided training data set with {len(train_data)} rows, {train_data.num_items} items (item = single time series). "
-            f"Average time series length is {len(train_data) / train_data.num_items:.1f}."
+            f"Average time series length is {len(train_data) / train_data.num_items:.1f}. "
+            f"Data frequency is '{train_data.freq}'."
         )
         if tuning_data is not None:
             logger.info(
                 f"Provided tuning data set with {len(tuning_data)} rows, {tuning_data.num_items} items. "
                 f"Average time series length is {len(tuning_data) / tuning_data.num_items:.1f}."
             )
-        logger.info(f"Training artifacts will be saved to: {Path(self.path).resolve()}")
+            if num_val_windows > 0:
+                logger.warning("Multi-window backtesting is disabled (setting num_val_windows = 0)")
+                num_val_windows = 0
+        num_val_windows = self._validate_num_val_windows(train_data, tuning_data, num_val_windows)
+
         logger.info("=====================================================")
 
         if random_seed is not None:
             set_random_seed(random_seed)
 
         time_left = None if time_limit is None else time_limit - (time.time() - time_start)
         self._learner.fit(
             train_data=train_data,
             val_data=tuning_data,
             hyperparameters=hyperparameters,
             hyperparameter_tune_kwargs=hyperparameter_tune_kwargs,
             time_limit=time_left,
             verbosity=verbosity,
+            num_val_windows=num_val_windows,
             enable_ensemble=enable_ensemble,
         )
 
         self.save()
         return self
 
     def get_model_names(self) -> List[str]:
```

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from autogluon.common.utils.log_utils import set_logger_verbosity
 from autogluon.core.models import AbstractModel
 from autogluon.core.utils.loaders import load_pkl
 from autogluon.core.utils.savers import save_json, save_pkl
 from autogluon.timeseries import TimeSeriesDataFrame, TimeSeriesEvaluator
 from autogluon.timeseries.models.abstract import AbstractTimeSeriesModel
 from autogluon.timeseries.models.ensemble import AbstractTimeSeriesEnsembleModel, TimeSeriesGreedyEnsemble
+from autogluon.timeseries.models.multi_window.multi_window_model import MultiWindowBacktestingModel
 from autogluon.timeseries.models.presets import contains_searchspace
 from autogluon.timeseries.utils.features import CovariateMetadata
 from autogluon.timeseries.utils.warning_filters import disable_tqdm
 
 logger = logging.getLogger("autogluon.timeseries.trainer")
 
 
@@ -272,14 +273,15 @@
         path: str,
         prediction_length: Optional[int] = 1,
         eval_metric: Optional[str] = None,
         eval_metric_seasonal_period: Optional[int] = None,
         save_data: bool = True,
         enable_ensemble: bool = True,
         verbosity: int = 2,
+        num_val_windows: int = 1,
         **kwargs,
     ):
         super().__init__(path=path, save_data=save_data, low_memory=True, **kwargs)
 
         self.prediction_length = prediction_length
         self.quantile_levels = kwargs.get(
             "quantile_levels",
@@ -298,14 +300,15 @@
         # self.refit_single_full() and self.refit_ensemble_full().
         self.model_full_dict = {}
 
         # Dict of FULL model -> normal model validation score in case the normal model had been deleted.
         self._model_full_dict_val_score = {}
         self.eval_metric = TimeSeriesEvaluator.check_get_evaluation_metric(eval_metric)
         self.eval_metric_seasonal_period = eval_metric_seasonal_period
+        self.num_val_windows = num_val_windows
         self.hpo_results = {}
 
     def save_train_data(self, data: TimeSeriesDataFrame, verbose: bool = True) -> None:
         path = self.path_data + "train.pkl"
         save_pkl.save(path=path, object=data, verbose=verbose)
 
     def save_val_data(self, data: TimeSeriesDataFrame, verbose: bool = True) -> None:
@@ -412,14 +415,15 @@
         """Train the single model and return the model object that was fitted. This method
         does not save the resulting model."""
         model.fit(
             train_data=train_data,
             val_data=val_data,
             time_limit=time_limit,
             verbosity=self.verbosity,
+            num_val_windows=self.num_val_windows,
         )
         return model
 
     def tune_model_hyperparameters(
         self,
         model: AbstractTimeSeriesModel,
         train_data: TimeSeriesDataFrame,
@@ -437,14 +441,15 @@
         with disable_tqdm():
             hpo_models, _ = model.hyperparameter_tune(
                 train_data=train_data,
                 val_data=val_data,
                 hyperparameter_tune_kwargs=hyperparameter_tune_kwargs,
                 time_limit=time_limit,
                 default_num_trials=default_num_trials,
+                num_val_windows=self.num_val_windows,
             )
         total_tuning_time = time.time() - tuning_start_time
 
         self.hpo_results[model.name] = hpo_models
         model_names_trained = []
         # add each of the trained HPO configurations to the trained models
         for model_hpo_name, model_info in hpo_models.items():
@@ -478,15 +483,15 @@
     def _train_and_save(
         self,
         train_data: TimeSeriesDataFrame,
         model: AbstractTimeSeriesModel,
         val_data: Optional[TimeSeriesDataFrame] = None,
         time_limit: Optional[float] = None,
     ) -> List[str]:
-        """Fit and save the given model on given training and validation data.
+        """Fit and save the given model on given training and validation data and save the trained model.
 
         Returns
         -------
         model_names_trained: the list of model names that were successfully trained
         """
         fit_start_time = time.time()
         model_names_trained = []
@@ -556,19 +561,25 @@
 
         if self.save_data and not self.is_data_saved:
             self.save_train_data(train_data)
             if val_data is not None:
                 self.save_val_data(val_data)
             self.is_data_saved = True
 
+        if self.num_val_windows > 0:
+            assert val_data is None, "val_data shouldn't be provided if num_val_windows > 0"
+        else:
+            assert val_data is not None, "val_data should be provided if num_val_windows > 0"
+
         if models is None:
             models = self.construct_model_templates(
                 hyperparameters=hyperparameters,
                 hyperparameter_tune=hyperparameter_tune_kwargs is not None,  # TODO: remove hyperparameter_tune
                 freq=train_data.freq,
+                multi_window=self.num_val_windows > 0,
             )
 
         logger.info(f"Models that will be trained: {list(m.name for m in models)}")
 
         time_limit_model_split = time_limit
         if time_limit is not None and len(models) > 0:
             time_limit_model_split /= len(models)
@@ -638,14 +649,16 @@
                         "no models were successfully trained."
                         if not models_available_for_ensemble
                         else "only 1 model was trained."
                     )
                 )
             else:
                 try:
+                    if val_data is None:
+                        val_data = self._get_ensemble_oof_data(train_data)
                     model_names_trained.append(
                         self.fit_ensemble(
                             val_data=val_data,
                             model_names=models_available_for_ensemble,
                             time_limit=time_left_for_ensemble,
                         )
                     )
@@ -663,14 +676,30 @@
             logger.info(f"Best model: {best_model}")
             logger.info(f"Best model score: {self.get_model_attribute(best_model, 'val_score'):.4f}")
         except ValueError as e:
             logger.error(str(e))
 
         return model_names_trained
 
+    def _get_ensemble_oof_data(self, train_data: TimeSeriesDataFrame) -> TimeSeriesDataFrame:
+        """Stack validation data for all windows into a single dataframe"""
+        split_per_window = []
+        for window_index in range(self.num_val_windows):
+            if window_index == 0:
+                end_index = None
+            else:
+                end_index = -self.prediction_length * window_index
+            _, val_fold = train_data.train_test_split(
+                self.prediction_length,
+                end_index=end_index,
+                suffix=f"_W{window_index}",
+            )
+            split_per_window.append(val_fold)
+        return pd.concat(split_per_window)
+
     def _get_ensemble_model_name(self) -> str:
         """Ensure we don't have name collisions in the ensemble model name"""
         ensemble_name = "WeightedEnsemble"
         increment = 1
         while ensemble_name in self._get_banned_model_names():
             increment += 1
             ensemble_name = f"WeightedEnsemble_{increment}"
@@ -919,15 +948,15 @@
         if valid_model_set:
             self.refit_single_full(models=valid_model_set)
 
         self.save()
         return copy.deepcopy(self.model_full_dict)
 
     def construct_model_templates(
-        self, hyperparameters: Union[str, Dict[str, Any]], **kwargs
+        self, hyperparameters: Union[str, Dict[str, Any]], multi_window: bool = False, **kwargs
     ) -> List[AbstractTimeSeriesModel]:
         """Constructs a list of unfit models based on the hyperparameters dict."""
         raise NotImplementedError
 
     def fit(
         self,
         train_data: TimeSeriesDataFrame,
```

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ..models.presets import get_preset_models
 from .abstract_trainer import AbstractTimeSeriesTrainer, TimeSeriesDataFrame
 
 logger = logging.getLogger(__name__)
 
 
 class AutoTimeSeriesTrainer(AbstractTimeSeriesTrainer):
-    def construct_model_templates(self, hyperparameters, **kwargs):
+    def construct_model_templates(self, hyperparameters, multi_window: bool = False, **kwargs):
         path = kwargs.pop("path", self.path)
         eval_metric = kwargs.pop("eval_metric", self.eval_metric)
         eval_metric_seasonal_period = kwargs.pop("eval_metric", self.eval_metric_seasonal_period)
         quantile_levels = kwargs.pop("quantile_levels", self.quantile_levels)
         hyperparameter_tune = kwargs.get("hyperparameter_tune", False)
         return get_preset_models(
             path=path,
@@ -22,14 +22,15 @@
             freq=kwargs.get("freq"),
             hyperparameters=hyperparameters,
             hyperparameter_tune=hyperparameter_tune,
             quantiles=quantile_levels,
             invalid_model_names=self._get_banned_model_names(),
             target=self.target,
             metadata=self.metadata,
+            multi_window=multi_window,
         )
 
     def fit(
         self,
         train_data: TimeSeriesDataFrame,
         hyperparameters: Union[str, Dict[Any, Dict]],
         val_data: Optional[TimeSeriesDataFrame] = None,
```

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/utils/seasonality.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/utils/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-0.7.0b20230410/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-0.7.0b20230410/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.0b20230409
+Version: 0.7.0b20230410
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.0b20230409/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-0.7.0b20230410/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 src/autogluon/timeseries/models/gluonts/torch/__init__.py
 src/autogluon/timeseries/models/gluonts/torch/models.py
 src/autogluon/timeseries/models/local/__init__.py
 src/autogluon/timeseries/models/local/abstract_local_model.py
 src/autogluon/timeseries/models/local/naive.py
 src/autogluon/timeseries/models/local/statsforecast.py
 src/autogluon/timeseries/models/local/statsmodels.py
+src/autogluon/timeseries/models/multi_window/__init__.py
+src/autogluon/timeseries/models/multi_window/multi_window_model.py
 src/autogluon/timeseries/trainer/__init__.py
 src/autogluon/timeseries/trainer/abstract_trainer.py
 src/autogluon/timeseries/trainer/auto_trainer.py
 src/autogluon/timeseries/utils/__init__.py
 src/autogluon/timeseries/utils/features.py
 src/autogluon/timeseries/utils/forecast.py
 src/autogluon/timeseries/utils/random.py
```


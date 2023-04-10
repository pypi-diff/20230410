# Comparing `tmp/falcon-ml-0.5.0.tar.gz` & `tmp/falcon-ml-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon-ml-0.5.0.tar", last modified: Sat Dec 31 18:08:05 2022, max compression
+gzip compressed data, was "falcon-ml-0.6.0.tar", last modified: Mon Apr 10 19:12:17 2023, max compression
```

## Comparing `falcon-ml-0.5.0.tar` & `falcon-ml-0.6.0.tar`

### file list

```diff
@@ -1,59 +1,81 @@
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2022-12-31 18:08:05.035343 falcon-ml-0.5.0/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1062 2022-10-25 08:32:28.000000 falcon-ml-0.5.0/LICENSE
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     3211 2022-12-31 18:08:05.034860 falcon-ml-0.5.0/PKG-INFO
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     2721 2022-11-18 19:08:58.000000 falcon-ml-0.5.0/README.md
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2022-12-31 18:08:05.009448 falcon-ml-0.5.0/falcon/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      204 2022-12-31 17:35:57.000000 falcon-ml-0.5.0/falcon/__init__.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2022-12-31 18:08:05.016822 falcon-ml-0.5.0/falcon/abstract/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      361 2022-12-31 17:37:55.000000 falcon-ml-0.5.0/falcon/abstract/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      574 2022-10-25 08:32:28.000000 falcon-ml-0.5.0/falcon/abstract/learner.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1109 2022-10-25 08:32:28.000000 falcon-ml-0.5.0/falcon/abstract/model.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      412 2022-12-24 21:00:18.000000 falcon-ml-0.5.0/falcon/abstract/onnx_convertible.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      807 2022-12-31 16:22:48.000000 falcon-ml-0.5.0/falcon/abstract/optuna.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      283 2022-11-18 19:08:58.000000 falcon-ml-0.5.0/falcon/abstract/processor.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     5710 2022-11-18 19:08:58.000000 falcon-ml-0.5.0/falcon/abstract/task_manager.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     3771 2022-11-18 19:08:58.000000 falcon-ml-0.5.0/falcon/abstract/task_pipeline.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2022-12-31 18:08:04.976403 falcon-ml-0.5.0/falcon/addons/
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2022-12-31 18:08:05.017712 falcon-ml-0.5.0/falcon/addons/sklearn/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)       88 2022-10-25 08:32:28.000000 falcon-ml-0.5.0/falcon/addons/sklearn/__init__.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2022-12-31 18:08:05.018196 falcon-ml-0.5.0/falcon/addons/sklearn/ensemble/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     5515 2022-10-25 08:32:28.000000 falcon-ml-0.5.0/falcon/addons/sklearn/ensemble/balanced_stacking.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2022-12-31 18:08:05.018792 falcon-ml-0.5.0/falcon/addons/sklearn/model_selection/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      525 2022-10-25 08:32:28.000000 falcon-ml-0.5.0/falcon/addons/sklearn/model_selection/balanced_strat_kfold.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)       49 2022-11-21 19:07:31.000000 falcon-ml-0.5.0/falcon/config.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1441 2022-11-18 19:08:58.000000 falcon-ml-0.5.0/falcon/datasets.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     5144 2022-12-31 16:32:35.000000 falcon-ml-0.5.0/falcon/main.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     6053 2022-11-18 19:08:58.000000 falcon-ml-0.5.0/falcon/runtime.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     4106 2022-11-21 19:15:27.000000 falcon-ml-0.5.0/falcon/serialization.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2022-12-31 18:08:05.023069 falcon-ml-0.5.0/falcon/tabular/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      173 2022-10-25 08:32:28.000000 falcon-ml-0.5.0/falcon/tabular/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     4076 2022-12-19 17:33:39.000000 falcon-ml-0.5.0/falcon/tabular/configurations.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2022-12-31 18:08:05.025648 falcon-ml-0.5.0/falcon/tabular/learners/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      127 2022-12-19 17:30:32.000000 falcon-ml-0.5.0/falcon/tabular/learners/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     7272 2022-12-31 17:36:29.000000 falcon-ml-0.5.0/falcon/tabular/learners/optuna_learner.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)    42188 2022-12-18 16:10:22.000000 falcon-ml-0.5.0/falcon/tabular/learners/super_learner.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2022-12-31 18:08:05.028941 falcon-ml-0.5.0/falcon/tabular/models/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      186 2022-12-31 16:36:56.000000 falcon-ml-0.5.0/falcon/tabular/models/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     5219 2022-12-31 17:03:25.000000 falcon-ml-0.5.0/falcon/tabular/models/hist_gbt.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     7171 2022-12-31 17:01:09.000000 falcon-ml-0.5.0/falcon/tabular/models/stacking.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2022-12-31 18:08:05.030882 falcon-ml-0.5.0/falcon/tabular/pipelines/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)       83 2022-10-25 08:32:28.000000 falcon-ml-0.5.0/falcon/tabular/pipelines/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     3277 2022-11-18 19:08:58.000000 falcon-ml-0.5.0/falcon/tabular/pipelines/simple_tabular_pipeline.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2022-12-31 18:08:05.032594 falcon-ml-0.5.0/falcon/tabular/processors/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      139 2022-10-25 08:32:28.000000 falcon-ml-0.5.0/falcon/tabular/processors/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     4477 2022-11-18 19:08:58.000000 falcon-ml-0.5.0/falcon/tabular/processors/label_decoder.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     4651 2022-11-18 19:08:58.000000 falcon-ml-0.5.0/falcon/tabular/processors/scaler_and_encoder.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     5637 2022-11-18 19:08:58.000000 falcon-ml-0.5.0/falcon/tabular/reporting.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)    11950 2022-11-18 19:08:58.000000 falcon-ml-0.5.0/falcon/tabular/tabular_manager.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     5574 2022-11-18 19:08:58.000000 falcon-ml-0.5.0/falcon/tabular/utils.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      682 2022-11-18 19:08:58.000000 falcon-ml-0.5.0/falcon/task_configurations.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      217 2022-11-18 19:08:58.000000 falcon-ml-0.5.0/falcon/types.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1648 2022-11-18 19:08:58.000000 falcon-ml-0.5.0/falcon/utils.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2022-12-31 18:08:05.034439 falcon-ml-0.5.0/falcon_ml.egg-info/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     3211 2022-12-31 18:08:04.000000 falcon-ml-0.5.0/falcon_ml.egg-info/PKG-INFO
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1339 2022-12-31 18:08:04.000000 falcon-ml-0.5.0/falcon_ml.egg-info/SOURCES.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)        1 2022-12-31 18:08:04.000000 falcon-ml-0.5.0/falcon_ml.egg-info/dependency_links.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      166 2022-12-31 18:08:04.000000 falcon-ml-0.5.0/falcon_ml.egg-info/requires.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)        7 2022-12-31 18:08:04.000000 falcon-ml-0.5.0/falcon_ml.egg-info/top_level.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      882 2022-12-31 17:35:47.000000 falcon-ml-0.5.0/pyproject.toml
--rw-r--r--   0 kostrominoleg   (501) staff       (20)       38 2022-12-31 18:08:05.035457 falcon-ml-0.5.0/setup.cfg
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 19:12:17.475823 falcon-ml-0.6.0/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1062 2023-02-06 13:05:16.000000 falcon-ml-0.6.0/LICENSE
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2839 2023-04-10 19:12:17.475823 falcon-ml-0.6.0/PKG-INFO
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2349 2023-03-04 11:21:20.000000 falcon-ml-0.6.0/README.md
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 19:12:17.471824 falcon-ml-0.6.0/falcon/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      204 2023-03-04 11:19:41.000000 falcon-ml-0.6.0/falcon/__init__.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 19:12:17.471824 falcon-ml-0.6.0/falcon/abstract/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      361 2023-02-06 13:05:16.000000 falcon-ml-0.6.0/falcon/abstract/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      574 2023-02-06 13:05:16.000000 falcon-ml-0.6.0/falcon/abstract/learner.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1229 2023-02-26 12:49:06.000000 falcon-ml-0.6.0/falcon/abstract/model.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      412 2023-02-06 13:05:16.000000 falcon-ml-0.6.0/falcon/abstract/onnx_convertible.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      878 2023-02-26 12:49:06.000000 falcon-ml-0.6.0/falcon/abstract/optuna.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      283 2023-02-08 20:18:52.000000 falcon-ml-0.6.0/falcon/abstract/processor.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5860 2023-04-06 19:41:27.000000 falcon-ml-0.6.0/falcon/abstract/task_manager.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     3508 2023-04-06 19:41:27.000000 falcon-ml-0.6.0/falcon/abstract/task_pipeline.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 19:12:17.471824 falcon-ml-0.6.0/falcon/addons/
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 19:12:17.471824 falcon-ml-0.6.0/falcon/addons/sklearn/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      183 2023-02-26 12:49:06.000000 falcon-ml-0.6.0/falcon/addons/sklearn/__init__.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 19:12:17.471824 falcon-ml-0.6.0/falcon/addons/sklearn/decomposition/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2154 2023-02-26 12:49:06.000000 falcon-ml-0.6.0/falcon/addons/sklearn/decomposition/svd.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 19:12:17.471824 falcon-ml-0.6.0/falcon/addons/sklearn/ensemble/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     6043 2023-04-06 20:09:48.000000 falcon-ml-0.6.0/falcon/addons/sklearn/ensemble/balanced_stacking.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 19:12:17.471824 falcon-ml-0.6.0/falcon/addons/sklearn/model_selection/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      525 2023-02-06 13:05:16.000000 falcon-ml-0.6.0/falcon/addons/sklearn/model_selection/balanced_strat_kfold.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 19:12:17.471824 falcon-ml-0.6.0/falcon/addons/sklearn/preprocessing/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2406 2023-02-26 12:49:06.000000 falcon-ml-0.6.0/falcon/addons/sklearn/preprocessing/date_tokenizer.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       49 2023-02-06 13:05:16.000000 falcon-ml-0.6.0/falcon/config.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      101 2023-02-26 12:49:14.000000 falcon-ml-0.6.0/falcon/constants.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1441 2023-02-06 13:05:16.000000 falcon-ml-0.6.0/falcon/datasets.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5910 2023-04-06 19:41:27.000000 falcon-ml-0.6.0/falcon/main.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     3293 2023-04-06 19:41:27.000000 falcon-ml-0.6.0/falcon/runtime.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5421 2023-04-06 19:41:27.000000 falcon-ml-0.6.0/falcon/serialization.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5080 2023-04-06 19:41:27.000000 falcon-ml-0.6.0/falcon/sklapi.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 19:12:17.475823 falcon-ml-0.6.0/falcon/tabular/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      229 2023-04-06 19:41:27.000000 falcon-ml-0.6.0/falcon/tabular/__init__.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 19:12:17.471824 falcon-ml-0.6.0/falcon/tabular/adapters/
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 19:12:17.475823 falcon-ml-0.6.0/falcon/tabular/adapters/ts/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5342 2023-04-09 12:27:53.000000 falcon-ml-0.6.0/falcon/tabular/adapters/ts/adapter.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     3668 2023-04-06 19:41:27.000000 falcon-ml-0.6.0/falcon/tabular/adapters/ts/auxiliary.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2562 2023-04-07 08:46:31.000000 falcon-ml-0.6.0/falcon/tabular/adapters/ts/learner.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1250 2023-04-06 19:41:27.000000 falcon-ml-0.6.0/falcon/tabular/adapters/ts/pipeline.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      721 2023-04-06 19:41:27.000000 falcon-ml-0.6.0/falcon/tabular/adapters/ts/plot_errors.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4902 2023-04-10 18:38:52.000000 falcon-ml-0.6.0/falcon/tabular/configurations.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 19:12:17.475823 falcon-ml-0.6.0/falcon/tabular/learners/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      190 2023-02-26 12:49:14.000000 falcon-ml-0.6.0/falcon/tabular/learners/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     8447 2023-04-10 18:43:14.000000 falcon-ml-0.6.0/falcon/tabular/learners/optuna_learner.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     3734 2023-03-24 21:18:49.000000 falcon-ml-0.6.0/falcon/tabular/learners/plain_learner.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)    42694 2023-04-06 19:41:27.000000 falcon-ml-0.6.0/falcon/tabular/learners/super_learner.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 19:12:17.475823 falcon-ml-0.6.0/falcon/tabular/models/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      186 2023-02-06 13:05:16.000000 falcon-ml-0.6.0/falcon/tabular/models/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5327 2023-02-26 12:49:06.000000 falcon-ml-0.6.0/falcon/tabular/models/hist_gbt.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     7202 2023-03-02 12:54:47.000000 falcon-ml-0.6.0/falcon/tabular/models/stacking.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 19:12:17.475823 falcon-ml-0.6.0/falcon/tabular/pipelines/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       83 2023-02-06 13:05:16.000000 falcon-ml-0.6.0/falcon/tabular/pipelines/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4260 2023-04-06 19:41:27.000000 falcon-ml-0.6.0/falcon/tabular/pipelines/simple_tabular_pipeline.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 19:12:17.475823 falcon-ml-0.6.0/falcon/tabular/processors/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      214 2023-03-04 10:16:34.000000 falcon-ml-0.6.0/falcon/tabular/processors/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4586 2023-03-04 10:13:17.000000 falcon-ml-0.6.0/falcon/tabular/processors/label_decoder.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     3299 2023-03-24 17:09:02.000000 falcon-ml-0.6.0/falcon/tabular/processors/multi_modal_encoder.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5900 2023-03-24 17:08:42.000000 falcon-ml-0.6.0/falcon/tabular/processors/scaler_and_encoder.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5582 2023-03-26 09:27:58.000000 falcon-ml-0.6.0/falcon/tabular/reporting.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)    13874 2023-04-06 19:41:27.000000 falcon-ml-0.6.0/falcon/tabular/tabular_manager.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5363 2023-04-06 19:41:27.000000 falcon-ml-0.6.0/falcon/tabular/utils.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1983 2023-04-09 12:41:45.000000 falcon-ml-0.6.0/falcon/tabular/wrappers.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     6782 2023-03-04 10:04:38.000000 falcon-ml-0.6.0/falcon/task_configurations.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2459 2023-04-06 19:41:27.000000 falcon-ml-0.6.0/falcon/type_guessing.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      543 2023-02-26 12:49:06.000000 falcon-ml-0.6.0/falcon/types.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1879 2023-04-09 12:09:36.000000 falcon-ml-0.6.0/falcon/utils.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 19:12:17.475823 falcon-ml-0.6.0/falcon_ml.egg-info/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2839 2023-04-10 19:12:17.000000 falcon-ml-0.6.0/falcon_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1902 2023-04-10 19:12:17.000000 falcon-ml-0.6.0/falcon_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        1 2023-04-10 19:12:17.000000 falcon-ml-0.6.0/falcon_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      169 2023-04-10 19:12:17.000000 falcon-ml-0.6.0/falcon_ml.egg-info/requires.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        7 2023-04-10 19:12:17.000000 falcon-ml-0.6.0/falcon_ml.egg-info/top_level.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      884 2023-04-06 14:12:08.000000 falcon-ml-0.6.0/pyproject.toml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       38 2023-04-10 19:12:17.475823 falcon-ml-0.6.0/setup.cfg
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 19:12:17.475823 falcon-ml-0.6.0/tests/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      315 2023-02-06 13:05:16.000000 falcon-ml-0.6.0/tests/test_datasets.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      589 2023-04-04 19:17:56.000000 falcon-ml-0.6.0/tests/test_main.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4058 2023-04-06 19:41:27.000000 falcon-ml-0.6.0/tests/test_sklapi.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2574 2023-04-04 19:17:58.000000 falcon-ml-0.6.0/tests/test_type_guessing.py
```

### Comparing `falcon-ml-0.5.0/LICENSE` & `falcon-ml-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `falcon-ml-0.5.0/PKG-INFO` & `falcon-ml-0.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon-ml
-Version: 0.5.0
+Version: 0.6.0
 Summary: AutoML library for fast experementations.
 Author-email: Oleg Kostromin <kostromin97@gmail.com>, Iryna Kondrashchenko <iryna230520@gmail.com>, Marco Pasini <marco.pasini.98@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -66,13 +66,13 @@
 ## Documentation 📚
 You can find a more detailed guide as well as an API reference in our [official docs](https://okua1.github.io/falcon/intro.html#).
 
 ## Authors & Contributors ✨
 <table>
   <tbody>
     <tr>
-      <td align="center"><a href="https://www.linkedin.com/in/oleh-kostromin-b671a4157/"><img src="https://media-exp1.licdn.com/dms/image/C4E03AQFydN-5z3UMtg/profile-displayphoto-shrink_800_800/0/1608633662231?e=1669852800&v=beta&t=X_0kzVZJmVOGO7hZWB3ljjf17_nFBmwji5-7npknUNQ" width="100px;" alt=""/><br /><sub><b>Oleg Kostromin</b></sub></a><br /></td>
-      <td align="center"><a href="https://www.linkedin.com/in/iryna-kondrashchenko-673800155/"><img src="https://media-exp1.licdn.com/dms/image/C4E03AQFDt5RccbPXcA/profile-displayphoto-shrink_800_800/0/1623761751542?e=1669852800&v=beta&t=l3mNCKbk8Vngi7rO5eADXCkiuH5rRGs33q54n1E8ye0" width="100px;" alt=""/><br /><sub><b>Iryna Kondrashchenko</b></sub></a><br /></td>
-      <td align="center"><a href="https://www.linkedin.com/in/pasinimarco/"><img src="https://media-exp1.licdn.com/dms/image/C5603AQF8fCDUN4wTGQ/profile-displayphoto-shrink_800_800/0/1563967808742?e=1669852800&v=beta&t=dhIuM_6SVGLGHl1gsVygFrcJcP_h2sZwzidsxZOsVQU" width="100px;" alt=""/><br /><sub><b>Marco Pasini</b></sub></a><br /></td>
+      <td align="center"><a href="https://www.linkedin.com/in/oleh-kostromin-b671a4157/"><img src="https://avatars.githubusercontent.com/u/48349467?v=4" width="100px;" alt=""/><br /><sub><b>Oleg Kostromin</b></sub></a><br /></td>
+      <td align="center"><a href="https://www.linkedin.com/in/iryna-kondrashchenko-673800155/"><img src="https://avatars.githubusercontent.com/u/72279145?v=4" width="100px;" alt=""/><br /><sub><b>Iryna Kondrashchenko</b></sub></a><br /></td>
+      <td align="center"><a href="https://www.linkedin.com/in/pasinimarco/"><img src="https://avatars.githubusercontent.com/u/50598094?v=4" width="100px;" alt=""/><br /><sub><b>Marco Pasini</b></sub></a><br /></td>
     </tr>
   </tbody>
 </table>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: falcon-ml Version: 0.5.0 Summary: AutoML library
+Metadata-Version: 2.1 Name: falcon-ml Version: 0.6.0 Summary: AutoML library
 for fast experementations. Author-email: Oleg Kostromin
 gmail.com>, Iryna Kondrashchenko
 gmail.com>, Marco Pasini
 pasini.98@gmail.com> License: MIT Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE
```

### Comparing `falcon-ml-0.5.0/README.md` & `falcon-ml-0.6.0/falcon_ml.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: falcon-ml
+Version: 0.6.0
+Summary: AutoML library for fast experementations.
+Author-email: Oleg Kostromin <kostromin97@gmail.com>, Iryna Kondrashchenko <iryna230520@gmail.com>, Marco Pasini <marco.pasini.98@gmail.com>
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
   <img src="https://raw.githubusercontent.com/OKUA1/falcon/main/docs/source/logo_cropped.png" width="256" height="217"/>
 </p>
 
 
 # FALCON: A Lightweight AutoML Library
 Falcon is a lightweight python library that allows to train production-ready machine learning models in a single line of code. 
@@ -53,13 +66,13 @@
 ## Documentation 📚
 You can find a more detailed guide as well as an API reference in our [official docs](https://okua1.github.io/falcon/intro.html#).
 
 ## Authors & Contributors ✨
 <table>
   <tbody>
     <tr>
-      <td align="center"><a href="https://www.linkedin.com/in/oleh-kostromin-b671a4157/"><img src="https://media-exp1.licdn.com/dms/image/C4E03AQFydN-5z3UMtg/profile-displayphoto-shrink_800_800/0/1608633662231?e=1669852800&v=beta&t=X_0kzVZJmVOGO7hZWB3ljjf17_nFBmwji5-7npknUNQ" width="100px;" alt=""/><br /><sub><b>Oleg Kostromin</b></sub></a><br /></td>
-      <td align="center"><a href="https://www.linkedin.com/in/iryna-kondrashchenko-673800155/"><img src="https://media-exp1.licdn.com/dms/image/C4E03AQFDt5RccbPXcA/profile-displayphoto-shrink_800_800/0/1623761751542?e=1669852800&v=beta&t=l3mNCKbk8Vngi7rO5eADXCkiuH5rRGs33q54n1E8ye0" width="100px;" alt=""/><br /><sub><b>Iryna Kondrashchenko</b></sub></a><br /></td>
-      <td align="center"><a href="https://www.linkedin.com/in/pasinimarco/"><img src="https://media-exp1.licdn.com/dms/image/C5603AQF8fCDUN4wTGQ/profile-displayphoto-shrink_800_800/0/1563967808742?e=1669852800&v=beta&t=dhIuM_6SVGLGHl1gsVygFrcJcP_h2sZwzidsxZOsVQU" width="100px;" alt=""/><br /><sub><b>Marco Pasini</b></sub></a><br /></td>
+      <td align="center"><a href="https://www.linkedin.com/in/oleh-kostromin-b671a4157/"><img src="https://avatars.githubusercontent.com/u/48349467?v=4" width="100px;" alt=""/><br /><sub><b>Oleg Kostromin</b></sub></a><br /></td>
+      <td align="center"><a href="https://www.linkedin.com/in/iryna-kondrashchenko-673800155/"><img src="https://avatars.githubusercontent.com/u/72279145?v=4" width="100px;" alt=""/><br /><sub><b>Iryna Kondrashchenko</b></sub></a><br /></td>
+      <td align="center"><a href="https://www.linkedin.com/in/pasinimarco/"><img src="https://avatars.githubusercontent.com/u/50598094?v=4" width="100px;" alt=""/><br /><sub><b>Marco Pasini</b></sub></a><br /></td>
     </tr>
   </tbody>
 </table>
```

#### html2text {}

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1 Name: falcon-ml Version: 0.6.0 Summary: AutoML library
+for fast experementations. Author-email: Oleg Kostromin
+gmail.com>, Iryna Kondrashchenko
+gmail.com>, Marco Pasini
+pasini.98@gmail.com> License: MIT Classifier: Programming Language :: Python ::
+3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
+System :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
+markdown License-File: LICENSE
        [https://raw.githubusercontent.com/OKUA1/falcon/main/docs/source/
                                logo_cropped.png]
 # FALCON: A Lightweight AutoML Library Falcon is a lightweight python library
 that allows to train production-ready machine learning models in a single line
 of code. ## Quick Start ð You can try falcon out simply by pointing it to
 the location of your dataset. ```python from falcon import AutoML AutoML(task =
 'tabular_classification', train_data = '/path/to/titanic.csv') ```
```

### Comparing `falcon-ml-0.5.0/falcon/abstract/learner.py` & `falcon-ml-0.6.0/falcon/abstract/learner.py`

 * *Files identical despite different names*

### Comparing `falcon-ml-0.5.0/falcon/abstract/model.py` & `falcon-ml-0.6.0/falcon/abstract/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from abc import ABC, abstractmethod
 from numpy import typing as npt
 from typing import Any
+from typing_extensions import Protocol
 
 
 class Model(ABC):
     """
     Base class for all models.
     """
 
     @abstractmethod
-    def fit(self, X: npt.NDArray, y: npt.NDArray) -> Any:
+    def fit(self, X: npt.NDArray, y: npt.NDArray, *args: Any, **kwargs: Any) -> Any:
         """
 
         Parameters
         ----------
         X : npt.NDArray
             features
         y : npt.NDArray
@@ -23,15 +24,15 @@
         -------
         Any
             usually `None`
         """
         pass
 
     @abstractmethod
-    def predict(self, X: npt.NDArray) -> npt.NDArray:
+    def predict(self, X: npt.NDArray, *args: Any, **kwargs: Any) -> npt.NDArray:
         """
         Parameters
         ----------
         X : npt.NDArray
             features
 
         Returns
@@ -39,15 +40,15 @@
         npt.NDArray
             predictions
         """
         pass
 
 
 class TransformerMixin:
-    def transform(self, X: npt.NDArray) -> npt.NDArray:
+    def transform(self, X: npt.NDArray, *args: Any, **kwargs: Any) -> npt.NDArray:
         """
         Equivalent of `self.predict(X)`
 
         Parameters
         ----------
         X : npt.NDArray
             features
```

### Comparing `falcon-ml-0.5.0/falcon/abstract/optuna.py` & `falcon-ml-0.6.0/falcon/abstract/optuna.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from abc import abstractmethod, ABC
 from typing import Any, Union, Callable, Dict
+from typing_extensions import Protocol
+from numpy import typing as npt
 
 class OptunaMixin(ABC):
 
     """
     Abstract mixin that should be used in order to indicate the compatibility of the model with OptunaLearner. 
     """
     @classmethod
```

### Comparing `falcon-ml-0.5.0/falcon/abstract/task_manager.py` & `falcon-ml-0.6.0/falcon/abstract/task_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from numpy import typing as npt
 from .task_pipeline import Pipeline
-from typing import Dict, Optional, Any, Callable, Type
+from typing import Dict, Optional, Any, Callable, Type, List
 from falcon.serialization import SerializedModelRepr
+from onnx import ModelProto
+from onnx import save_model as onnx_save_model
+
 
 class TaskManager(ABC):
     """
     Base class for all Task Managers.
     """
     def __init__(
         self,
@@ -37,16 +40,20 @@
             featrues to be used for training, by default None
         target : Any, optional
             targets to be used for training, by default None
         """
         self.task: str = task
         self.features = features
         self.target = target
+        self.dataset_size = ()
+        self.feature_names_to_save: List[Any] = []
         self._data = self._prepare_data(data)
-        self._extra_pipeline_options = extra_pipeline_options
+        if self.dataset_size is None: 
+            raise RuntimeError('It seems like prepare_data() method did not set dataset_size attribute.')
+        self._extra_pipeline_options: Optional[Dict] = extra_pipeline_options
         self._create_pipeline(pipeline=pipeline, options=pipeline_options)
 
     @abstractmethod
     def train(self, **kwargs: Any) -> TaskManager:
         """
         Trains the underlying pipeline.
 
@@ -80,14 +87,15 @@
     def default_pipeline(self) -> Type[Pipeline]:
         """
         Default pipeline class. Can be chosen dynamically.
         """
         pass
 
     @property
+    @abstractmethod
     def default_pipeline_options(self) -> Dict:
         """
         Default pipeline options. Can be chosen dynamically.
         """
         pass
 
     def predict(self, X: Any) -> Any:
@@ -118,49 +126,43 @@
             pipeline class
         options : Optional[Dict]
             pipeline options
         """
 
         # if pipeline is not None and options is None:
         #     self._pipeline = pipeline(task=self.task)
+
         if pipeline is None:
             pipeline = self.default_pipeline
         if options is None:
             options = self.default_pipeline_options
             if self._extra_pipeline_options is not None:
                 for k, v in self._extra_pipeline_options.items():
                     options[k] = v
-        self._pipeline = pipeline(task=self.task, **options)
+        self._pipeline: Pipeline = pipeline(task=self.task, dataset_size = self.dataset_size, **options)
 
-    def save_model(self, format: str = "auto", filename: Optional[str] = None) -> bytes:
+    def save_model(self, filename: Optional[str] = None, **kwargs: Any) -> ModelProto:
         """
         Serializes and saves the model.
 
         Parameters
         ----------
-        format : str, optional
-            "auto", "onnx" or "falcon"; "falcon" format should only be used in rare cases when converting to onnx is not possible, by default "auto"
         filename : Optional[str], optional
             filename for the model file, by default None. If filename is not specified, the model is not saved on disk and only returned as bytes object
-
         Returns
         -------
-        bytes
-            serialized model as bytes
+        ModelProto
+            ONNX ModelProto of the model
         """
-        if format not in {"falcon", "onnx", "auto"}:
-            raise ValueError(
-                f"expected one of [onnx, falcon] as output format, got {format}"
-            )
-        serialized_model, format = self._pipeline.save(format=format)
+
+        serialized_model = self._pipeline.save(feature_names=self.feature_names_to_save)
         if filename is not None:
-            if not filename.endswith(f".{format}"):
-                filename += f".{format}"
-            with open(filename, "wb+") as f:
-                f.write(serialized_model)
+            if not filename.endswith(f".onnx"):
+                filename += f".onnx"
+            onnx_save_model(serialized_model, filename, save_as_external_data=True, all_tensors_to_one_file=True, location=f"{filename}.tensors", size_threshold=0, convert_attribute=True)
         return serialized_model
 
     @abstractmethod
     def evaluate(self, test_data: Any) -> Any:
         """
         Evaluates the performance of a trained pipeline.
```

### Comparing `falcon-ml-0.5.0/falcon/abstract/task_pipeline.py` & `falcon-ml-0.6.0/falcon/abstract/task_pipeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from abc import abstractmethod
 from typing import Any, Type, Union, Optional, List, Tuple
+from onnx import ModelProto
 from falcon.abstract.model import Model
 from falcon.abstract.onnx_convertible import ONNXConvertible
-from falcon.serialization import SerializedModelRepr, serialize_to_falcon, serialize_to_onnx
+from falcon.serialization import SerializedModelRepr, serialize_to_onnx
 
 
 class PipelineElement(Model):
     """
     Base class for all pipeline elements.
     """
 
@@ -26,31 +27,31 @@
         Returns
         -------
         Type
             Output types
         """
         pass
 
-    def forward(self, X: Any) -> Any:
+    def forward(self, X: Any, *args: Any, **kwargs: Any) -> Any:
         """
         Equivalent of `predict` method that is used for elements chaining inside pipeline during inference.
 
         Parameters
         ----------
         X : Any
             featrues
 
         Returns
         -------
         Any
             predictions
         """
-        self.predict(X)
+        return self.predict(X)
 
-    def fit_pipe(self, X: Any, y: Any) -> Any:
+    def fit_pipe(self, X: Any, y: Any, *args: Any, **kwargs: Any) -> Any:
         """
         Equivalent of `fit` method that is used for elements chaining inisde pipeline during training.
 
         Parameters
         ----------
         X : Any
             features
@@ -66,17 +67,21 @@
 
 
 class Pipeline(Model):
     """
     Base class for all pipelines.
     """
 
-    def __init__(self, task: str, **kwargs: Any) -> None:
+    def __init__(
+        self, task: str, dataset_size: Tuple[int, ...], mask: List[Any], **kwargs: Any
+    ) -> None:
         self.task = task
         self._pipeline: List[PipelineElement] = []
+        self.dataset_size = dataset_size
+        self.mask = mask
 
     def add_element(self, element: PipelineElement) -> None:
         """
         Adds element to pipeline. The input type of added element should match the output type of the last element in the pipeline.
 
         Parameters
         ----------
@@ -90,44 +95,34 @@
             raise RuntimeError(
                 "The element cannot be added to pipeline due to input type missmatch."
             )
         if element is self:
             raise ValueError("Cannot add self to the pipeline")
         self._pipeline.append(element)
 
-    def save(self, format: str = "auto") -> Tuple[bytes, str]:
+    def save(self, feature_names: Optional[List] = None) -> ModelProto:
         """
-        Serializes the model to string. For more details please refer to the documentation of `TaskManager.save_model(...)` method.
+        Exports the pipeline to ONNX ModelProto
 
         Parameters
         ----------
-        format : str, optional
-           `auto`, `falcon` or `onnx`, by default `auto`
-
+        feature_names : Optional[List], optional
+            feature names, by default None
         Returns
         -------
-        Tuple[SerializedModelRepr, str]
-            Serialized model, format
-
-
+        ModelProto
+            Pipeline as ONNX ModelProto
         """
-        if format not in {"falcon", "onnx"}:
-            raise ValueError(
-                f"expected one of [onnx, falcon] as output format, got {format}"
-            )
         serialized_pipeline_elements: List[SerializedModelRepr] = []
         for p in self._pipeline:
             if isinstance(p, ONNXConvertible):
                 serialized_pipeline_elements.append(p.to_onnx())
             else:
-                if format == "onnx":
-                    raise RuntimeError("This model cannot be serialized to onnx")
-                elif format == "auto":
-                    format = "falcon"
-        if format == "falcon":
-            serialized_model = serialize_to_falcon(serialized_pipeline_elements)
-        else:
-            format = "onnx"
-            serialized_model = serialize_to_onnx(
-                serialized_pipeline_elements
-            ).SerializeToString()
-        return serialized_model, format
+                raise RuntimeError("Encountered non convertible pipeline element")
+
+        serialized_model = serialize_to_onnx(
+            serialized_pipeline_elements,
+            task=self.task,
+            init_types=self.mask,
+            init_feature_names=feature_names,
+        )
+        return serialized_model
```

### Comparing `falcon-ml-0.5.0/falcon/addons/sklearn/ensemble/balanced_stacking.py` & `falcon-ml-0.6.0/falcon/addons/sklearn/ensemble/balanced_stacking.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 from sklearn.utils.validation import check_scalar
 from sklearn.utils.fixes import delayed
 from sklearn.ensemble import StackingClassifier
 from types import MethodType
 from falcon.addons.sklearn.model_selection.balanced_strat_kfold import (
     BalancedStratifiedKFold,
 )
+from sklearn.preprocessing import LabelEncoder
+from sklearn import __version__ as sklearn_version
+from packaging import version
 
 # Slightly modified version of StackingClassifier from sklearn that upsamples the minority class during training
 # The .fit() method was adopted from https://github.com/scikit-learn/scikit-learn/blob/36958fb24/sklearn/ensemble/_stacking.py
 
 
 def _fit(self, X, y, sample_weight=None):
     check_classification_targets(y)
@@ -134,14 +137,31 @@
         X_meta_resampled,
         y_meta_resampled,
         sample_weight=sample_weight,
     )
 
     return self
 
+class _EncoderPlaceholder(LabelEncoder):
+    
+    def fit(self, y, **args):
+        return self
+    
+    def transform(self, y, **args):
+        return y
+    
+    def fit_transform(self, y, **args):
+        return y
+    
+    def inverse_transform(self, y, **args):
+        return y
+
+
 
 # the object is being patched with a new method instead of subclassing
 # so the estimator can be converted to ONNX using the default converter
 def BalancedStackingClassifier(estimators, final_estimator, **kwargs):
     clf = StackingClassifier(estimators, final_estimator, **kwargs)
     clf.fit = MethodType(_fit, clf)
+    if version.parse(sklearn_version) >= version.parse("1.2.0"):
+        clf._label_encoder = _EncoderPlaceholder()
     return clf
```

### Comparing `falcon-ml-0.5.0/falcon/addons/sklearn/model_selection/balanced_strat_kfold.py` & `falcon-ml-0.6.0/falcon/addons/sklearn/model_selection/balanced_strat_kfold.py`

 * *Files identical despite different names*

### Comparing `falcon-ml-0.5.0/falcon/datasets.py` & `falcon-ml-0.6.0/falcon/datasets.py`

 * *Files identical despite different names*

### Comparing `falcon-ml-0.5.0/falcon/main.py` & `falcon-ml-0.6.0/falcon/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from falcon.abstract import TaskManager
 from falcon.tabular import TabularTaskManager
-from typing import Any, Optional, Dict, Type, Union
+from typing import Any, Optional, Dict, Type, Union, Callable
+from sklearn.model_selection import BaseCrossValidator
 from falcon.abstract import Pipeline, TaskManager
 import warnings
 import datetime
-from falcon.task_configurations import get_task_configuration
+from falcon.task_configurations import get_task_configuration, TaskConfigurationRegistry
+from falcon.utils import set_eval_strategy
+
 
 def warn(*args: Any, **kwargs: Any) -> None:
     pass
 
 
 def initialize(
     task: str,
     data: Any,
     pipeline: Optional[Type[Pipeline]] = None,
     pipeline_options: Optional[Dict] = None,
     extra_pipeline_options: Optional[Dict] = None,
     features: Any = None,
     target: Any = None,
-    **options: Any
+    **options: Any,
 ) -> TaskManager:
     """
     Initializes and returns a task manager object for a given task.
 
     Parameters
     ----------
     task : str
@@ -45,44 +48,44 @@
 
     Returns
     -------
     TaskManager
         Initialized task manager object
     """
     warnings.warn = warn
-    if task == "tabular_classification" or task == "tabular_regression":
-        manager: TabularTaskManager = TabularTaskManager(
-            task=task,
-            data=data,
-            pipeline=pipeline,
-            pipeline_options=pipeline_options,
-            extra_pipeline_options=extra_pipeline_options,
-            features=features,
-            target=target,
-            **options
-        )
-    else:
-        raise ValueError("Invalid task")
+
+    Manager = TaskConfigurationRegistry.get_task_manager(task)
+
+    manager = Manager(
+        task=task,
+        data=data,
+        pipeline=pipeline,
+        pipeline_options=pipeline_options,
+        extra_pipeline_options=extra_pipeline_options,
+        features=features,
+        target=target,
+        **options,
+    )
 
     return manager
 
 
-# TODO Allow NONE for the task
 def AutoML(
     task: str,
     train_data: Any,
-    test_data: Any =  None,
+    test_data: Any = None,
     features: Any = None,
     target: Any = None,
     manager_configuration: Optional[Union[Dict, str]] = None,
-    config: Optional[Union[Dict, str]] = None
+    config: Optional[Union[Dict, str]] = None,
+    eval_strategy: Optional[Union[str, Callable, BaseCrossValidator]] = "dynamic",
 ) -> TaskManager:
     """
     High level API for one line model training and evaluation.
-    
+
     When calling the following steps will be executed:
         1) task manager object will be initialized;
         2) the model will be trained;
         3) performance summary table is printed (if test set is not provided, random split is done);
         4) the model is saved as an onnx file.
 
     Parameters
@@ -97,32 +100,56 @@
         features to be used for training, for tabular classification and regression this can be: list of column names or indexes, by default None
     target : Any, optional
         target to be used for training, for tabular classification and regression this can be: column name or index, by default None
     manager_configuration : Union[Dict, str], optional
         task manager configuration to be used (can be used to replace pipeline/learner and/or their arguments), by default None
     config : Union[Dict, str], optional
         alias for `manager_configuration` argument
+    eval_strategy : Optional[Union[str, Callable, BaseCrossValidator]], optional
+        evaluation strategy, by default "dynamic"
+        - "dynamic" - if test_data is provided, evaluation will be done on test_data, otherwise "auto" will be used
+        - "auto" - random split / cv will be done
+        - "cv" - cross validation will be done
+        - "holdout" - random split will be done
+        - None - no evaluation will be done
+        - Callable - custom function for performing train/eval split
+        - BaseCrossValidator - custom cross validator
 
     Returns
     -------
     TaskManager
         Task Manager object for the corresponding task.
     """
     task = task.lower()
     if config is not None and manager_configuration is not None:
-        print("Both `config` and `manager_configuration` were set; `manager_configuration` will be ignored in this case.")
+        print(
+            "Both `config` and `manager_configuration` were set; `manager_configuration` will be ignored in this case."
+        )
     if config is not None:
         manager_configuration = config
     if manager_configuration is None:
         manager_configuration_ = {}
-    elif isinstance(manager_configuration, str): 
-        manager_configuration_ = get_task_configuration(task=task, configuration_name=manager_configuration)
-    manager = initialize(task=task, data=train_data, features=features, target=target, **manager_configuration_)
-    make_eval_subset = True if test_data is None else False
-    manager.train(pre_eval = False, make_eval_subset = make_eval_subset)
-    manager.performance_summary(test_data = test_data)
-    print('Saving the model ...')
-    ts = datetime.datetime.now().strftime('%Y%m%d.%H%M%S')
+    elif isinstance(manager_configuration, dict):
+        manager_configuration_ = manager_configuration
+    elif isinstance(manager_configuration, str):
+        manager_configuration_ = get_task_configuration(
+            task=task, configuration_name=manager_configuration
+        )
+
+    set_eval_strategy(eval_strategy, manager_configuration_, test_data)
+
+    manager = initialize(
+        task=task,
+        data=train_data,
+        features=features,
+        target=target,
+        **manager_configuration_,
+    )
+
+    manager.train()
+    manager.performance_summary(test_data=test_data)
+    print("Saving the model ...")
+    ts = datetime.datetime.now().strftime("%Y%m%d.%H%M%S")
     filename = f"falcon_{ts}.onnx"
-    manager.save_model(format = 'onnx', filename = filename)
+    manager.save_model(format="onnx", filename=filename)
     print(f"The model was saved as `{filename}`")
     return manager
```

### Comparing `falcon-ml-0.5.0/falcon/runtime.py` & `falcon-ml-0.6.0/falcon/serialization.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,180 +1,150 @@
-from typing import Any, Union, Dict, List, Type, Optional
-import onnxruntime as ort
+from typing import List, Optional, Dict
+from falcon.utils import print_
+from typing import List, Tuple, Optional
+from numpy import typing as npt
+from onnx import ModelProto, load_from_string
+from onnx.compose import add_prefix, merge_models
+from onnx.helper import make_model
+from falcon.config import ONNX_OPSET_VERSION, ML_ONNX_OPSET_VERSION
+from falcon import __version__ as falcon_version
 import numpy as np
-from abc import ABC, abstractmethod
-import bson
-from bson import BSON
-
-
-class BaseRuntime(ABC):
-    @abstractmethod
-    def run(self, X: np.ndarray, **kwargs: Any) -> Any:
-        pass
-
-
-class ONNXRuntime(BaseRuntime):
-    """
-    Runtime for ONNX models. This runtime can only run onnx models produced by falcon.
-    """
-    def __init__(self, model: Union[bytes, str]):
-        self.ort_session = ort.InferenceSession(model)
-
-    def run(self, X: np.ndarray, outputs: str = "final", **kwargs: Any) -> List[np.ndarray]:
-        """
-        Runs the model.
-
-        Parameters
-        ----------
-        X : np.ndarray
-            model 
-        outputs : str, optional
-            when set to "all", all onnx output nodes will be returned; when "final" only the last layer outputs are returned, by default "final"
-
-        Returns
-        -------
-        List[np.ndarray]
-            model predictions
-        """
-        if outputs not in ["all", "final"]:
-            raise ValueError(
-                f"Expected `outputs` to be one of [all, final], got `{outputs}`."
+from typing import Any, Dict, Union
+import onnx
+from onnx import TensorProto, helper as h, OperatorSetIdProto
+
+
+class SerializedModelRepr:
+    def __init__(
+        self,
+        model: onnx.ModelProto,
+        n_inputs: int,
+        n_outputs: int,
+        initial_types: List[str],
+        initial_shapes: List[List[Optional[int]]],
+        type_: str = "onnx",
+    ):
+        self._model = model
+        self._n_inputs = n_inputs
+        self._n_outputs = n_outputs
+        self._initial_types = initial_types
+        self._initial_shapes = initial_shapes
+        self._type = type_
+
+    def get_model(self) -> onnx.ModelProto:
+        return self._model
+
+    def get_n_inputs(self) -> int:
+        return self._n_inputs
+
+    def get_n_outputs(self) -> int:
+        return self._n_outputs
+
+    def get_initial_types(self) -> List[str]:
+        return self._initial_types
+
+    def get_initial_shapes(self) -> List[List[Optional[int]]]:
+        return self._initial_shapes
+
+    def get_type(self) -> str:
+        return self._type
+
+    def to_dict(self) -> Dict:
+        return {
+            "n_inputs": self._n_inputs,
+            "n_outputs": self._n_outputs,
+            "initial_types": self._initial_types,
+            "initial_shapes": self._initial_shapes,
+            "model": self._model,
+            "type": self._type,
+        }
+
+
+def _make_self_name(name: Any) -> str:
+    name = str(name)
+    name = "".join([c for c in name if c.isalpha() or c.isdigit() or c == " "]).rstrip()
+    name = name.replace(" ", "_")
+    return name
+
+
+def _rename_inputs(
+    model: onnx.ModelProto, feature_names: List[Any], feature_types: List
+) -> None:
+    # print(feature_types, len(model.graph.input))
+    if len(feature_types) != len(model.graph.input):
+        feature_types = ["9999" for _ in range(len(model.graph.input))]
+    else:
+        feature_types = [str(i.value) for i in feature_types]
+    if len(feature_names) != len(feature_types):
+        feature_names = [str(i) for i in range(len(feature_types))]
+    mapping = {}
+    for i, inp in enumerate(model.graph.input):
+        new_name = f"falcon-input-{str(i)}_{_make_self_name(feature_names[i])}_{feature_types[i]}"
+        mapping[inp.name] = new_name
+        inp.name = new_name
+    for node in model.graph.node:
+        for key in mapping.keys():
+            for ii, input in enumerate(node.input):
+                if input == key:
+                    node.input[ii] = mapping[key]
+
+
+def serialize_to_onnx(
+    models_: List[SerializedModelRepr],
+    init_types: Optional[List] = None,
+    init_feature_names: Optional[List] = None,
+    task: Optional[str] = None,
+) -> onnx.ModelProto:
+    if init_types is None:
+        init_types = []
+    if init_feature_names is None:
+        init_feature_names = []
+    print_("Serializing to onnx...")
+    if len(models_) == 0:
+        raise ValueError("List of models cannot be empty")
+
+    # Updating the models by resetting the opset and adding prefix to node names
+    updated_models: List[ModelProto] = []
+    models = [m.get_model() for m in models_]
+    for i, model in enumerate(models):
+        op1 = h.make_operatorsetid("", ONNX_OPSET_VERSION)
+        op2 = h.make_operatorsetid("ai.onnx.ml", ML_ONNX_OPSET_VERSION)
+        op3 = h.make_operatorsetid("com.microsoft", 1)
+        updated_model = make_model(model.graph, opset_imports=[op1, op2, op3])
+        updated_model = add_prefix(updated_model, prefix=f"falcon-pl-{i}/")
+        updated_models.append(updated_model)
+
+    # Merging the models sequentially
+    prev: ModelProto = updated_models[0]
+    for i in range(1, len(updated_models)):
+        current: ModelProto = updated_models[i]
+        prev_outputs: List = prev.graph.output
+        current_inputs: List = current.graph.input
+        if len(prev_outputs) > len(current_inputs):
+            prev_outputs = prev_outputs[: len(current_inputs)]
+        if len(prev_outputs) < len(current_inputs):
+            raise RuntimeError(
+                "When merging, previous model should have at least as many outputs as inputs in the next model."
             )
-
-        inputs = self._get_inputs(X)
-        output_names = self._get_output_names(outputs)
-
-        return self.ort_session.run(output_names, inputs)
-
-    def _get_inputs(self, X: np.ndarray) -> Dict:
-        ort_inputs = self.ort_session.get_inputs()
-        inputs = {}
-
-        for i, inp in enumerate(ort_inputs):
-            dtype: Any
-            if str(inp.type) == "tensor(float)":
-                dtype = np.float32
-            elif str(inp.type) == "tensor(string)":
-                dtype = np.str_
-            elif "int" in str(inp.type).lower():
-                dtype = np.int64
-            else:
-                RuntimeError(
-                    f"The model input type should be one of [str, int, float], got f{inp.type}"
-                )
-            if len(ort_inputs) > 1:
-                inputs[str(inp.name)] = np.expand_dims(X[:, i], 1).astype(dtype)
-            else:
-                inputs[str(inp.name)] = X.astype(dtype)
-        return inputs
-
-    def _get_output_names(self, outputs: str = "final") -> List[str]:
-        ort_outputs = self.ort_session.get_outputs()
-        output_names = [o.name for o in ort_outputs]
-        if outputs == "final" and len(ort_outputs) > 1:
-            idx_ = []
-            for name in output_names:
-                if not name[0:10] == "falcon_pl_":
-                    raise RuntimeError("One of the output nodes has an invalid name.")
-                idx = int(name.split("/")[0][10:])
-                idx_.append(idx)
-            max_idx = max(idx_)
-            output_names = [
-                n for n in output_names if n.startswith(f"falcon_pl_{max_idx}")
-            ]
-        return output_names
-
-
-class FalconRuntime(BaseRuntime):
-    """
-    Runtime for falcon models.
-    This runtime is added for future compatibility in case some models will not be onnx convertible. 
-    Ideally, it will not have to be used.
-    """
-    def __init__(self, model: Union[bson.BSON, str, bytes]):
-        """
-        Parameters
-        ----------
-        model : Union[bson.BSON, str, bytes]
-            Serialized model or filepath
-        """
-
-        if isinstance(model, str) and model.endswith(".falcon"):
-            with (open(model, "rb")) as f:
-                model = f.read()
-
-        self.decoded_model: Dict = bson.BSON.decode(model) # type: ignore
-
-    def run(self, X: np.ndarray, **kwargs: Any) -> Union[List, np.ndarray]:
-        """
-        Runs the model.
-
-        Parameters
-        ----------
-        X : np.ndarray
-            model inputs
-            
-
-        Returns
-        -------
-        Union[List, np.ndarray]
-            model prediction
-        """
-        for i, node in enumerate(self.decoded_model["nodes"]):
-            if node["type"] == "onnx":
-                X = self._run_onnx_node(node, X, self._get_n_inputs_node(i + 1))
-            else:
-                raise RuntimeError(f"Unknown node type {node['type']}")
-        if len(X) == 1:
-            X = X[0]
-        if len(X.shape) > 1:
-            X = np.squeeze(X)
-        return X
-
-    def _get_n_inputs_node(self, i: int) -> Optional[int]:
-        if len(self.decoded_model["nodes"]) > i:
-            return self.decoded_model["nodes"][i]["n_inputs"]
-        else:
-            return None
-
-    def _run_onnx_node(
-        self, node: Dict, X: np.ndarray, n_inputs_next: Optional[int] = None
-    ) -> np.ndarray:
-        ort_sess = ort.InferenceSession(node["model"])
-        ort_inputs = ort_sess.get_inputs()
-        inputs = {}
-        for oi, inp in enumerate(ort_inputs):
-            dtype = self._get_np_type(node["initial_types"][oi])
-            if len(ort_sess.get_inputs()) > 1:
-                inputs[str(inp.name)] = np.expand_dims(X[:, oi], 1).astype(dtype)
-            else:
-                if len(X.shape) > len(node["initial_shapes"][oi]):
-                    X = X.squeeze()
-                elif len(X.shape) < len(node["initial_shapes"][oi]):
-                    X = np.expand_dims(X, 1)
-                inputs[str(inp.name)] = X.astype(dtype)
-        outputs = [o.name for o in ort_sess.get_outputs()]
-        print("next >> ", n_inputs_next)
-        if n_inputs_next is not None:
-            outputs = outputs[:n_inputs_next]
-        pred = ort_sess.run(outputs, inputs)
-        if len(pred) == 1:
-            pred = pred[0]
-        else:
-            print(len(pred))
-            print(pred)
-            raise NotImplementedError(  # TODO
-                "Multiple outputs from node is not yet supported."
-            )
-        return pred
-
-    def _get_np_type(self, type_: str) -> Type:
-        dtype: Type
-        if type_ == "FLOAT32":
-            dtype = np.float32
-        elif type_ == "STRING":
-            dtype = np.str_
-        elif type_ == "INT64":
-            dtype = np.int64
-        else:
-            RuntimeError("The model has an unsupported input type")
-        return dtype
+        io_map: List[Tuple[str, str]] = []
+        outputs: List[str] = [o.name for o in current.graph.output]
+        for p, c in zip(prev_outputs, current_inputs):
+            mapping: Tuple[str, str] = (p.name, c.name)
+            io_map.append(mapping)
+
+        print_(f"\t -> Merging step {i} ::: io_map {io_map} ::: outputs: {outputs}")
+        combined_model: ModelProto = merge_models(
+            prev, current, io_map=io_map  # , outputs=outputs
+        )
+
+        prev = combined_model
+    combined_model = prev
+    # TODO: Rename the inputs here
+    description = {}
+    if task is not None:
+        description["task"] = task
+    _rename_inputs(combined_model, init_feature_names, init_types)
+    combined_model.graph.doc_string = str(description)
+    combined_model.producer_name = "Falcon ML"
+    combined_model.producer_version = falcon_version
+    print_("Serialization completed.")
+    return combined_model
```

### Comparing `falcon-ml-0.5.0/falcon/tabular/learners/optuna_learner.py` & `falcon-ml-0.6.0/falcon/tabular/learners/optuna_learner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,151 +1,189 @@
 from falcon.abstract import Learner
-from typing import Type, Optional, Any, Union, Dict, Callable
+from typing import Type, Optional, Any, Union, Dict, Callable, Tuple
 from falcon.types import Float32Array, Int64Array
 from numpy import typing as npt
 from falcon.serialization import SerializedModelRepr
 from falcon.abstract import Model, ONNXConvertible
 from falcon.abstract.optuna import OptunaMixin
-from falcon.tabular.models.hist_gbt import HistGradientBoostingClassifier, HistGradientBoostingRegressor
+from falcon.tabular.models.hist_gbt import (
+    HistGradientBoostingClassifier,
+    HistGradientBoostingRegressor,
+)
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import mean_squared_error, balanced_accuracy_score
 import optuna
 from imblearn.over_sampling import RandomOverSampler
 from tqdm import tqdm
 
+
 class OptunaLearner(Learner, ONNXConvertible):
     """
     OptunaLerner select the best hyperparameters for the given model using the Optuna Framework.
     """
 
     def __init__(
-        self, task: str, model_class: Optional[Type] = None, n_trials: Optional[int] = None, **kwargs: Any
+        self,
+        task: str,
+        model_class: Optional[Type] = None,
+        n_trials: Optional[int] = None,
+        dataset_size: Optional[Tuple[int, ...]] = None,
+        **kwargs: Any,
     ) -> None:
         """
 
         Parameters
         ----------
         task : str
             'tabular_classification' or 'tabular_regression'
         model_class : Optional[Type], optional
             the class of the model to train, by default None;
             if None, HistGradientBoosting
         n_trials : Optional[int], optional
             number of optimization trials, minimum 20, by default None;
             if None, the number of trials is chosen dynamically based on the dataset size
+        dataset_size : Optional[Tuple[int]], optional
+            the size of the dataset, by default None;
 
         """
         self.task = task
-        if model_class is None: 
-            if task == "tabular_classification": 
-                model_class = HistGradientBoostingClassifier
+        self.dataset_size = dataset_size
+        self.model_class: Type[Any]
+        if model_class is None:
+            if task == "tabular_classification":
+                self.model_class = HistGradientBoostingClassifier
             elif task == "tabular_regression":
-                model_class = HistGradientBoostingRegressor
+                self.model_class = HistGradientBoostingRegressor
             else:
                 ValueError("Not supported task")
-        if not issubclass(model_class, Model) or not issubclass(model_class, OptunaMixin):
-            raise ValueError('Model class should be a subclass of falcon.abstract.Model')
-        if not issubclass(model_class, ONNXConvertible):
-            raise ValueError('OptunaLearner only supports ONNXConvertible models')
-        
+        else:
+            self.model_class = model_class
+
+        if not issubclass(self.model_class, Model) or not issubclass(self.model_class, OptunaMixin):  # type: ignore
+            raise ValueError(
+                "Model class should be a subclass of falcon.abstract.Model"
+            )
+        if not issubclass(self.model_class, ONNXConvertible):  # type: ignore
+            raise ValueError("OptunaLearner only supports ONNXConvertible models")
+
         if n_trials is not None and n_trials < 5:
-            print('n_trials should be >= 20, setting n_trials = 20')
+            print("n_trials should be >= 20, setting n_trials = 20")
             n_trials = 20
 
         self.n_trials = n_trials
-        
-        self.model_class = model_class
 
-    def _make_objective_func(self, search_space: Dict, X: npt.NDArray, y: npt.NDArray) -> Callable:
+    def _make_objective_func(
+        self, search_space: Union[Dict, Callable], X: npt.NDArray, y: npt.NDArray
+    ) -> Callable:
         stratify = y if self.task == "tabular_classification" else None
-        X_train, X_val, y_train, y_val = train_test_split(X, y, random_state=42, stratify=stratify)
-        
-        if self.task == 'tabular_regression':
+        X_train, X_val, y_train, y_val = train_test_split(
+            X, y, random_state=42, stratify=stratify
+        )
+
+        if self.task == "tabular_regression":
             loss = mean_squared_error
-        elif self.task == 'tabular_classification':
-            loss = lambda y, y_h : - balanced_accuracy_score(y,y_h)
-            X_train, y_train = RandomOverSampler().fit_resample(
-                X_train, y_train
-            )
-        progress_bar = tqdm(total = self.n_trials)
-        def objective(trial) -> float:
-            params = {}
-            for hp_n, hp_v in search_space.items():
-                if hp_v["type"] == "int":
-                    params[hp_n] = trial.suggest_int(name = hp_n, **hp_v["kwargs"])
-                if hp_v["type"] == "float":
-                    params[hp_n] = trial.suggest_float(name = hp_n, **hp_v["kwargs"]) 
-                if hp_v["type"] == "categorical":
-                    params[hp_n] = trial.suggest_categorical(name = hp_n, **hp_v["kwargs"]) 
-            
-            model = self.model_class(**params)
-            model.fit(X_train, y_train)
-            y_pred = model.predict(X_val)
-            loss_ = loss(y_val, y_pred)
-            progress_bar.update(1)
-            return loss_
+        elif self.task == "tabular_classification":
+            loss = lambda y, y_h: -balanced_accuracy_score(y, y_h)
+            X_train, y_train = RandomOverSampler().fit_resample(X_train, y_train)
+        progress_bar = tqdm(total=self.n_trials)
+        if isinstance(search_space, Dict):
+            search_space_dict: Dict = search_space
+
+            def objective(trial) -> float:  # type: ignore
+                params = {}
+                for hp_n, hp_v in search_space_dict.items():
+                    if hp_v["type"] == "int":
+                        params[hp_n] = trial.suggest_int(name=hp_n, **hp_v["kwargs"])
+                    if hp_v["type"] == "float":
+                        params[hp_n] = trial.suggest_float(name=hp_n, **hp_v["kwargs"])
+                    if hp_v["type"] == "categorical":
+                        params[hp_n] = trial.suggest_categorical(
+                            name=hp_n, **hp_v["kwargs"]
+                        )
+
+                model = self.model_class(**params)
+                model.fit(X_train, y_train)
+                y_pred = model.predict(X_val)
+                loss_ = loss(y_val, y_pred)
+                progress_bar.update(1)
+                return loss_
+
+        else:
+            search_space_fn: Callable = search_space
+
+            def objective(trial) -> float:  # type: ignore
+                res = search_space_fn(trial, X_train, X_val, y_train, y_val)
+                if res["loss"] is None:
+                    pred = res["predictions"]
+                    loss_ = loss(y_val, pred)
+                else:
+                    loss_ = res["loss"]
+                progress_bar.update(1)
+                return loss_
+
         self.progress_bar = progress_bar
         return objective
 
-    
     def _set_n_trials(self, X: npt.NDArray, y: npt.NDArray) -> None:
-        if self.n_trials is not None: 
-            return 
-        
-        volume = X.shape[0] * X.shape[1]
+        if self.n_trials is not None:
+            return
+
+        if self.dataset_size is None:
+            self.dataset_size = X.shape
+        volume = self.dataset_size[0] * self.dataset_size[1]
 
         min_threshold = 80_000  # 5_000 samples with 16 features
         mid_threshold = 4_000_000  # 125_000 samples with 32 featrues / 250_000 samples with 16 features
-        large_threshold = 16_000_000 # 1_000_000 samples with 16 features
+        large_threshold = 16_000_000  # 1_000_000 samples with 16 features
 
         if volume < min_threshold:
-            self.n_trials = 500
+            self.n_trials = 1000
         elif volume < mid_threshold:
-            self.n_trials = 200
+            self.n_trials = 500
         elif volume < large_threshold:
+            self.n_trials = 200
+        else:
             self.n_trials = 100
-        else: 
-            self.n_trials = 30
 
-    def fit(self, X: Float32Array, y: Float32Array) -> None:
+    def fit(self, X: Float32Array, y: Float32Array, *args: Any, **kwargs: Any) -> None:
         """
         Fits the model by choosing the best hyperparameters and training the final model using them.
         For classification tasks, the dataset will be balanced by upsampling the minority class(es).
 
         Parameters
         ----------
         X : Float32Array
             features
         y : Float32Array
             targets
         """
         self._set_n_trials(X, y)
         search_space = self.model_class.get_search_space(X, y)
         self.progress_bar = None
-        if isinstance(search_space, dict):
-            objective = self._make_objective_func(search_space, X, y)
-        else: 
-            NotImplementedError('Non-dict search space is not yet supported.')
-        
+        objective = self._make_objective_func(search_space, X, y)
+
         optuna.logging.set_verbosity(optuna.logging.ERROR)
-        study = optuna.create_study(direction="minimize", sampler=optuna.samplers.TPESampler(seed=42))
+        study = optuna.create_study(
+            direction="minimize", sampler=optuna.samplers.TPESampler(seed=42)
+        )
         study.optimize(objective, n_trials=self.n_trials)
         if self.progress_bar:
             self.progress_bar.close()
         best_params = study.best_params
+        self.best_params_ = best_params
 
-        if self.task == 'tabular_classification':
-            X, y = RandomOverSampler().fit_resample(
-                X, y
-            )
+        if self.task == "tabular_classification":
+            X, y = RandomOverSampler().fit_resample(X, y)
         model = self.model_class(**best_params)
-        model.fit(X,y)
+        model.fit(X, y)
         self.model = model
-    
-    def predict(self, X: Float32Array) -> Union[Float32Array, Int64Array]:
+
+    def predict(
+        self, X: Float32Array, *args: Any, **kwargs: Any
+    ) -> Union[Float32Array, Int64Array]:
         return self.model.predict(X)
 
     def get_input_type(self) -> Type:
         """
         Returns
         -------
         Type
@@ -157,16 +195,18 @@
         """
         Returns
         -------
         Type
             Float32Array for regression, Int64Array for classification
         """
         return Float32Array if self.task == "tabular_regression" else Int64Array
-    
-    def forward(self, X: Float32Array) -> Union[Float32Array, Int64Array]:
+
+    def forward(
+        self, X: Float32Array, *args: Any, **kwargs: Any
+    ) -> Union[Float32Array, Int64Array]:
         """
         Equivalent to `.predict(X)`
 
         Parameters
         ----------
         X : Float32Array
             features
@@ -174,15 +214,17 @@
         Returns
         -------
         Union[Float32Array, Int64Array]
             predictions
         """
         return self.model.predict(X)
 
-    def fit_pipe(self, X: Float32Array, y: Float32Array) -> None:
+    def fit_pipe(
+        self, X: Float32Array, y: Float32Array, *args: Any, **kwargs: Any
+    ) -> None:
         """
         Equivalent to `.fit(X, y)`
 
         Parameters
         ----------
         X : Float32Array
             features
@@ -196,8 +238,7 @@
         Serializes the underlying model to onnx by calling its `.to_onnx()` method.
 
         Returns
         -------
         SerializedModelRepr
         """
         return self.model.to_onnx()
-
```

### Comparing `falcon-ml-0.5.0/falcon/tabular/learners/super_learner.py` & `falcon-ml-0.6.0/falcon/tabular/learners/super_learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -488,15 +488,14 @@
             ),
             (
                 "RandomForestRegressor_100",
                 RandomForestRegressor,
                 {"min_samples_split": 0.003, "n_jobs": 1, "verbose": _SKLEARN_VERBOSE},
             ),
         ],
-
     },
     "tabular_classification": {
         "mini": [
             ("LogisticRegression", LogisticRegression, {}),
             ("DecisionTreeClassifier", DecisionTreeClassifier, {}),
             ("SVC", SVC, {}),
             ("NuSVC", NuSVC, {}),
@@ -919,15 +918,14 @@
                     "n_estimators": 50,
                     "min_samples_split": 0.003,
                     "n_jobs": 1,
                     "verbose": _SKLEARN_VERBOSE,
                 },
             ),
         ],
-
         "x-large": [
             ("HistGradientBoostingClassifier_100", HistGradientBoostingClassifier, {}),
             (
                 "HistGradientBoostingClassifier_200",
                 HistGradientBoostingClassifier,
                 {"max_iter": 200},
             ),
@@ -937,15 +935,14 @@
                 {"max_iter": 50},
             ),
             (
                 "RandomForestClassifier_100",
                 RandomForestClassifier,
                 {"min_samples_split": 0.003, "n_jobs": 1, "verbose": _SKLEARN_VERBOSE},
             ),
-            
         ],
     },
 }
 
 
 class SuperLearner(Learner, ONNXConvertible):
     """
@@ -955,14 +952,16 @@
     def __init__(
         self,
         task: str,
         base_estimators: Optional[List[Tuple[str, Callable, Dict]]] = None,
         base_score_threshold: Optional[float] = None,
         cv: Any = None,
         filter_estimators: Optional[bool] = None,
+        dataset_size: Optional[Tuple[int, ...]] = None,
+        **kwargs: Any,
     ) -> None:
         """
         Constructs a meta model which is trained on cross-validated predictions of base estimators.
 
         Parameters
         ----------
         task : str
@@ -971,22 +970,25 @@
             list of base estimators, by default None
         base_score_threshold : Optional[float], optional
             threshold for filtering of the estimators, by default None
         cv : Any, optional
             number of CV folds or CV custom object, by default None
         filter_estimators : Optional[bool], optional
             when True, the perfomance of the estimators pre-estimated on the subset of training, estimators with the performance below the threshold will not be used for meta model construction, by default None
+        dataset_size : Optional[Tuple[int]], optional
+            size of the dataset, by default None
         """
 
         if task not in ["tabular_classification", "tabular_regression"]:
             raise ValueError(
                 f"Invalid task type. Expected `tabular_classification` or `tabular_regression`, found `{task}`."
             )
 
         self.base_estimators = base_estimators
+        self.dataset_size: Optional[Tuple[int, ...]] = dataset_size
         self.task = task
         self.base_score_threshold = base_score_threshold
         self.cv = cv
         self.filter_estimators = filter_estimators
 
     def _split(
         self, X: npt.NDArray, y: npt.NDArray
@@ -1010,32 +1012,33 @@
     def _calculate_base_score(self, y_hat: Float32Array, y: Float32Array) -> float:
         if self.task == "tabular_classification":
             return balanced_accuracy_score(y, y_hat)
         else:
             return (r2_score(y, y_hat) + 1) / 2
 
     def _set_size_optimized_config(self, X: Float32Array) -> None:
-
-        volume = X.shape[0] * X.shape[1]
+        if self.dataset_size is None:
+            self.dataset_size = X.shape
+        volume = self.dataset_size[0] * self.dataset_size[1]
 
         min_threshold = 80_000  # 5_000 samples with 16 features
         mid_threshold = 4_000_000  # 125_000 samples with 32 featrues / 250_000 samples with 16 features
-        large_threshold = 16_000_000 # 1_000_000 samples with 16 features
+        large_threshold = 16_000_000  # 1_000_000 samples with 16 features
 
         if volume < min_threshold:
             print_("Setting up learner config [small dataset]")
             cv = 10
             base_estimators = _default_estimators[self.task]["mini"]
             filter_estimators = True
         elif volume < mid_threshold:
             print_("Setting up learner config [mid dataset]")
             cv = 5
             base_estimators = _default_estimators[self.task]["mid"]
             filter_estimators = True
-        elif volume < large_threshold: 
+        elif volume < large_threshold:
             print_("Setting up learner config [large dataset]")
             base_estimators = _default_estimators[self.task]["large"]
             cv = 3
             filter_estimators = False
         else:
             print_("Setting up learner config [x-large dataset]")
             base_estimators = _default_estimators[self.task]["x-large"]
@@ -1093,44 +1096,46 @@
                 selected_estimators.append((estimator[0], estimator[1](**estimator[2])))
         if len(selected_estimators) < 3:  # using all estimators
             for estimator in self.base_estimators:
                 selected_estimators = []
                 selected_estimators.append((estimator[0], estimator[1](**estimator[2])))
         return selected_estimators
 
-    def fit(self, X: Float32Array, y: Float32Array) -> None:
+    def fit(self, X: Float32Array, y: Float32Array, *args: Any, **kwargs: Any) -> None:
         """
         Fits the model. The hyperparameters that were not passed to the `__init__` will be automatically determined based on the size of the training set.
         For classification tasks, the dataset will be balanced by upsampling the minority class(es).
 
         Parameters
         ----------
         X : Float32Array
             features
         y : Float32Array
             targets
         """
         print_("Fitting stacked model... ")
         self._set_size_optimized_config(X)
         estimators: List[Tuple[str, Callable]] = self._preselect(X, y)
-        stacked_estimator: SklearnBaseEstimator
         print_(f"\t -> Fitting the final estimator")
+        stacked_estimator: Union[StackingClassifier, StackingRegressor]
         if self.task == "tabular_classification":
             stacked_estimator = StackingClassifier(
                 estimators=estimators, final_estimator=LogisticRegression(), cv=self.cv
             )
         else:
             stacked_estimator = StackingRegressor(
                 estimators=estimators, final_estimator=LinearRegression(), cv=self.cv
             )
 
         stacked_estimator.fit(X, y)
         self.model = stacked_estimator
 
-    def predict(self, X: Float32Array) -> Union[Float32Array, Int64Array]:
+    def predict(
+        self, X: Float32Array, *args: Any, **kwargs: Any
+    ) -> Union[Float32Array, Int64Array]:
         """
         Makes a prediction for given X.
 
         Parameters
         ----------
         X : Float32Array
             features
@@ -1156,15 +1161,17 @@
         Returns
         -------
         Type
             Float32Array for regression, Int64Array for classification
         """
         return Float32Array if self.task == "tabular_regression" else Int64Array
 
-    def forward(self, X: Float32Array) -> Union[Float32Array, Int64Array]:
+    def forward(
+        self, X: Float32Array, *args: Any, **kwargs: Any
+    ) -> Union[Float32Array, Int64Array]:
         """
         Equivalen to `.predict(X)`
 
         Parameters
         ----------
         X : Float32Array
             features
@@ -1172,15 +1179,17 @@
         Returns
         -------
         Union[Float32Array, Int64Array]
             predictions
         """
         return self.model.predict(X)
 
-    def fit_pipe(self, X: Float32Array, y: Float32Array) -> None:
+    def fit_pipe(
+        self, X: Float32Array, y: Float32Array, *args: Any, **kwargs: Any
+    ) -> None:
         """
         Equivalent to `.fit(X, y)`
 
         Parameters
         ----------
         X : Float32Array
             features
```

### Comparing `falcon-ml-0.5.0/falcon/tabular/models/hist_gbt.py` & `falcon-ml-0.6.0/falcon/tabular/models/hist_gbt.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from falcon.types import Float32Array, Int64Array
 from falcon.serialization import SerializedModelRepr
 from falcon.config import ONNX_OPSET_VERSION, ML_ONNX_OPSET_VERSION
 from falcon.abstract.optuna import OptunaMixin
 from numpy import typing as npt
 
 class _BaseHistGradientBoosting(Model, ONNXConvertible, OptunaMixin):
-    def __init__(self, estimator: Callable, **kwargs: Any):
+    def __init__(self, estimator: Union[SklearnHistGradientBoostingClassifier, SklearnHistGradientBoostingRegressor], **kwargs: Any):
         self.estimator = estimator
     
-    def fit(self, X: Float32Array, y: Float32Array) -> None:
+    def fit(self, X: Float32Array, y: Float32Array, *args: Any, **kwargs: Any) -> None:
         """
         Fits the model
 
         Parameters
         ----------
         X : Float32Array
             Features
@@ -46,25 +46,25 @@
             target_opset={'': ONNX_OPSET_VERSION, 'ai.onnx.ml': ML_ONNX_OPSET_VERSION},
             options=options,
         )
         n_inputs = len(onnx_model.graph.input)
         n_outputs = len(onnx_model.graph.output)
 
         return SerializedModelRepr(
-            onnx_model.SerializeToString(),
+            onnx_model,
             n_inputs,
             n_outputs,
             ["FLOAT32"],
             [self._shape]
         )
 
     def _get_onnx_options(self) -> Dict:
         return {}
     
-    def predict(self, X: npt.NDArray) -> npt.NDArray:
+    def predict(self, X: npt.NDArray, *args: Any, **kwargs: Any) -> npt.NDArray:
         return self.estimator.predict(X)
     
     @classmethod
     def get_search_space(cls, X: npt.NDArray, y: npt.NDArray) -> Union[Callable, Dict]:
         return { 
             "max_iter" : {
                 "type": "int",
```

### Comparing `falcon-ml-0.5.0/falcon/tabular/models/stacking.py` & `falcon-ml-0.6.0/falcon/tabular/models/stacking.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 class _StackingBase(Model, ONNXConvertible):
     def __init__(
         self,
         cls: Callable,
         estimators: List[Tuple[str, BaseEstimator]],
         final_estimator: BaseEstimator,
         cv: Any = None,
-        n_jobs: int = -1,
+        n_jobs: int = 1,
         passthrough: bool = False,
         verbose: int = 0,
         **kwargs: Any,
     ) -> None:
         self.estimator: BaseEstimator = cls(
             estimators=estimators,
             final_estimator=final_estimator,
@@ -41,29 +41,29 @@
 
         self._ret_type: Type = (
             np.float32
             if isinstance(self.estimator, SklearnStackingRegressor)
             else np.int64
         )
 
-    def fit(self, X: Float32Array, y: Float32Array) -> None:
+    def fit(self, X: Float32Array, y: Float32Array, *args: Any, **kwargs: Any) -> None:
         """
         Fits the model
 
         Parameters
         ----------
         X : Float32Array
             Features
         y : Float32Array
             targets
         """
         self._shape = [None, *X.shape[1:]]
         self.estimator.fit(X, y)
 
-    def predict(self, X: Float32Array) -> Float32Array:
+    def predict(self, X: Float32Array, *args: Any, **kwargs: Any) -> Float32Array:
         """
         Predicts the target for the given input
 
         Parameters
         ----------
         X : Float32Array
             featrues
@@ -94,15 +94,15 @@
             # final_types=self._get_onnx_final_types(),
             options=options,
         )
         n_inputs = len(onnx_model.graph.input)
         n_outputs = len(onnx_model.graph.output)
 
         return SerializedModelRepr(
-            onnx_model.SerializeToString(),
+            onnx_model,
             n_inputs,
             n_outputs,
             ["FLOAT32"],
             [self._shape],
         )
 
     # def _get_onnx_final_types(self) -> List[Tuple[str, TensorType]]:
@@ -119,15 +119,15 @@
 
     def __init__(
         self,
         estimators: List[Tuple[str, BaseEstimator]],
         final_estimator: BaseEstimator,
         balanced: bool = True,
         cv: Any = 5,
-        n_jobs: int = -1,
+        n_jobs: int = 1,
         passthrough: bool = False,
         verbose: int = 0,
         stack_method: Any = "auto",
         **kwargs: Any,
     ) -> None:
         """
         Small wrapper around `sklearn.ensemble.StackingClassifier`. 
@@ -187,15 +187,15 @@
     Small wrapper around `sklearn.ensemble.StackingRegressor`. 
     """
     def __init__(
         self,
         estimators: List[Tuple[str, BaseEstimator]],
         final_estimator: BaseEstimator,
         cv: Any = 5,
-        n_jobs: int = -1,
+        n_jobs: int = 1,
         passthrough: bool = False,
         verbose: int = 0,
         **kwargs: Any,
     ) -> None:
         """
         Small wrapper around `sklearn.ensemble.StackingRegressor`. 
         For more detailed description please refer to sklarn documentation.
```

### Comparing `falcon-ml-0.5.0/falcon/tabular/pipelines/simple_tabular_pipeline.py` & `falcon-ml-0.6.0/falcon/tabular/pipelines/simple_tabular_pipeline.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,106 @@
 from numpy import typing as npt
 import numpy.typing as npt
-from typing import List, Any, Optional, Dict, Type
+from typing import List, Any, Optional, Dict, Type, Tuple
 from falcon.abstract import Pipeline, PipelineElement
 from falcon.abstract.learner import Learner
 from falcon.abstract.onnx_convertible import ONNXConvertible
 from falcon.tabular.processors.label_decoder import LabelDecoder
 from falcon.tabular.processors.scaler_and_encoder import ScalerAndEncoder
+from falcon.tabular.processors.multi_modal_encoder import MultiModalEncoder
 from falcon.tabular.learners.super_learner import SuperLearner
+from falcon.types import ColumnTypes
 from falcon.utils import print_
 
+
 class SimpleTabularPipeline(Pipeline):
     """
     Default tabular pipeline.
     """
-    def __init__(self, task: str, mask: List[int], learner: Type[Learner] = SuperLearner, learner_kwargs: Optional[Dict] = None):
+
+    def __init__(
+        self,
+        task: str,
+        dataset_size: Tuple[int],
+        mask: List[ColumnTypes],
+        learner: Type[Learner] = SuperLearner,
+        learner_kwargs: Optional[Dict] = None,
+        preprocessor: str = "MultiModalEncoder",
+        **kwargs: Any,
+    ):
         """
-        Default tabular pipeline. On a high level it simply chains a preprocessor and model learner (by default `SuperLearner`). 
+        Default tabular pipeline. On a high level it simply chains a preprocessor and model learner (by default `SuperLearner`).
         For classification tasks, the labels are also encoded as integers (while predictions are decoded back to strings).
-        Internally, all numerical features are scaled to 0 mean and 1 std. All categorical features are one-hot encoded (this approach might not be suitable for features with very high cardinality). 
+        Internally, all numerical features are scaled to 0 mean and 1 std. All categorical features are one-hot encoded (this approach might not be suitable for features with very high cardinality).
 
         Parameters
         ----------
         task : str
             `tabular_classification` or `tabular_regression`
         mask : List[int]
             list of ints where 1/2 indicates a low/high cardinality categorical feature and 0 indicates a numerical feature
         learner : Learner, optional
             learner class to be used, by default `SuperLearner`
         learner_kwargs : Optional[Dict], optional
             arguments to be passed to the learner, by default None
+        preprocessor: str
+            defines which preprocessor to use, can be one of {'MultiModalEncoder','ScalerAndEncoder'}, by default 'MultiModalEncoder'
         """
-        super().__init__(task=task)
-        
-        encoder: PipelineElement = ScalerAndEncoder(mask)
+
+        super().__init__(task=task, dataset_size=dataset_size, mask = mask)
+
+        self.preprocessor = preprocessor
+        self.learner = learner
+        self.learner_kwargs = learner_kwargs
+
+    def _reset(self) -> None:
+        self._pipeline = []
+        encoder: PipelineElement
+        if self.preprocessor == "MultiModalEncoder":
+            encoder = MultiModalEncoder(self.mask)
+        else:
+            encoder = ScalerAndEncoder(self.mask)
+
         self.add_element(encoder)
-        
-        if not learner_kwargs:
+
+        if not self.learner_kwargs:
             learner_kwargs = {}
-        learner_: PipelineElement = learner(task=task, **learner_kwargs)
+        else:
+            learner_kwargs = self.learner_kwargs
+        learner_: PipelineElement = self.learner(
+            task=self.task, dataset_size=self.dataset_size, **learner_kwargs
+        )
         self.add_element(learner_)
 
         if self.task == "tabular_classification":
             self.labels_transformer: LabelDecoder = LabelDecoder()
             self.add_element(self.labels_transformer)
 
-    def fit(self, X: npt.NDArray, y: npt.NDArray) -> None:
+    def fit(self, X: npt.NDArray, y: npt.NDArray, *args: Any, **kwargs: Any) -> None:
         """
         Fits the pipeline by consecutively calling `.fit_pipe()` method of each element in pipeline.
         For tabular classification, `LabelDecoder` is applied to targets before actual training occurs.
 
         Parameters
         ----------
         X : npt.NDArray
             train featrues
         y : npt.NDArray
             train targets
         """
-        print_('Fitting the pipeline...')
+        print_("Fitting the pipeline...")
+        self._reset()
         if self.task == "tabular_classification":
             self.labels_transformer.fit(y)
             y = self.labels_transformer.transform(y, inverse=False)
         for p in self._pipeline:
             p.fit_pipe(X, y)
             X = p.forward(X)
 
-    def predict(self, X: npt.NDArray) -> npt.NDArray:
+    def predict(self, X: npt.NDArray, *args: Any, **kwargs: Any) -> npt.NDArray:
         """
         Predicts the label of passed data points.
 
         Parameters
         ----------
         X : npt.NDArray
             features
@@ -77,11 +109,7 @@
         -------
         npt.NDArray
             predicted label
         """
         for p in self._pipeline:
             X = p.forward(X)
         return X
-
-    
-
-
```

### Comparing `falcon-ml-0.5.0/falcon/tabular/processors/label_decoder.py` & `falcon-ml-0.6.0/falcon/tabular/processors/label_decoder.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,41 +20,41 @@
     """
     def __init__(self) -> None:
         """
         does not take any arguments
         """
         self.le = LabelEncoder()
 
-    def fit_pipe(self, _: Any, __: Any) -> None:  # Do nothing
+    def fit_pipe(self, X: Any, y: Any, *args: Any, **kwargs: Any) -> None:  # Do nothing
         """
         Since label decoder should initially be fitted and applied before the main training phase of pipeline, this method does nothing. 
 
         Parameters
         ----------
-        _ : Any
+        X : Any
             dummy argument
-        __ : Any
+        y : Any
             dummy argument
         """
         return
 
-    def fit(self, X: npt.NDArray, _: Any = None) -> None:
+    def fit(self, X: npt.NDArray, y: Any = None, *args: Any, **kwargs: Any) -> None:
         """
         Fits the decoder.
 
         Parameters
         ----------
         X : npt.NDArray
             labels to be encoded as integers
-        _ : Any, optional
+        y : Any, optional
             dummy argument, by default None
         """
         self.le.fit(X)
 
-    def predict(self, X: npt.NDArray, inverse: bool = True) -> npt.NDArray:
+    def predict(self, X: npt.NDArray, inverse: bool = True, *args: Any, **kwargs: Any) -> npt.NDArray:
         """
         Equivalent of `.transform()`.
 
         Parameters
         ----------
         X : npt.NDArray
             labels
@@ -64,15 +64,15 @@
         Returns
         -------
         npt.NDArray
             encoded/decoded labels
         """
         return self.transform(X, inverse=inverse)
 
-    def transform(self, X: npt.NDArray, inverse: bool = True) -> npt.NDArray:
+    def transform(self, X: npt.NDArray, inverse: bool = True, *args: Any, **kwargs: Any) -> npt.NDArray:
         """
         Encodes/decodes the labels.
 
         Parameters
         ----------
         X : npt.NDArray
             labels
@@ -99,15 +99,15 @@
         return Int64Array
 
     def get_output_type(self) -> Type:
         """
         Returns
         -------
         Type
-            NDArray[np.str_]
+            NDArray[str]
         """
         return NDArray[np.str_]
 
     def to_onnx(self) -> SerializedModelRepr:
         """
         Serializes the encoder to onnx. 
 
@@ -127,18 +127,18 @@
             keys_int64s=[int(i) for i in range(len(self.le.classes_))],
             name=f"labels_decoder",
             domain="ai.onnx.ml",
         )
         graph = h.make_graph([node], f"decoder", inputs, outputs)
         op = h.make_operatorsetid("ai.onnx.ml", ML_ONNX_OPSET_VERSION)
         model = h.make_model(graph, producer_name="falcon", opset_imports = [op])
-        return SerializedModelRepr(model.SerializeToString(), 1, 1, ["INT64"], [[None]])
+        return SerializedModelRepr(model, 1, 1, ["INT64"], [[None]])
 
     def forward(
-        self, X: npt.NDArray
+        self, X: npt.NDArray, *args: Any, **kwargs: Any
     ) -> npt.NDArray:  # Inside pipeline used as post-processor to decode labels back to strings
         """
         Equivalent to `.transform(X, inverse=True)`.
 
         Parameters
         ----------
         X : npt.NDArray
```

### Comparing `falcon-ml-0.5.0/falcon/tabular/processors/scaler_and_encoder.py` & `falcon-ml-0.6.0/falcon/tabular/processors/scaler_and_encoder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,112 @@
 import numpy as np
 from numpy import typing as npt
-from falcon.types import Float32Array
+from falcon.types import Float32Array, ColumnTypes
+from sklearn.base import BaseEstimator
+from sklearn import __version__ as sklearn_version
+from packaging import version
 from sklearn.compose import ColumnTransformer
 from sklearn.preprocessing import StandardScaler
 from sklearn.preprocessing import OneHotEncoder
 from falcon.abstract import Processor, ONNXConvertible
 from skl2onnx import convert_sklearn
 from skl2onnx.common.data_types import FloatTensorType, StringTensorType
 from falcon.config import ONNX_OPSET_VERSION, ML_ONNX_OPSET_VERSION
 from typing import List, Optional, Type, Any
 from sklearn.pipeline import Pipeline as SKLPipeline
 from sklearn.preprocessing import MaxAbsScaler, OrdinalEncoder
 from skl2onnx.sklapi import CastTransformer
 from falcon.serialization import SerializedModelRepr
 
+
 class ScalerAndEncoder(Processor, ONNXConvertible):
     """
     Applies OneHotEncoder/OrdinalEncoder on low/high cardinality categorical features and StandardScaler on numerical features.
     """
-    
-    def __init__(
-        self, mask: List[int]
-    ) -> None:  # [1/2 -> low/high cardinality categorical, 0 -> numerical]
+
+    def __init__(self, mask: List[ColumnTypes]) -> None:
         """
         Parameters
         ----------
-        mask : List[int]
-            boolean mask with True/False for categorical/numerical features
+        mask : List[ColumnTypes]
+            provides a type for each column at a given index
         """
         self.mask = mask
 
-    def fit(self, X: npt.NDArray, _: Any = None) -> None:
+    def _get_ohe(self) -> BaseEstimator:
+        if version.parse(sklearn_version) < version.parse("1.2.0"):
+            not_sparse = {"sparse": False}
+        else:
+            not_sparse = {"sparse_output": False}
+
+        method = SKLPipeline(
+            steps=[
+                ("cast_str", CastTransformer(dtype=np.str_)),
+                (
+                    "ohe",
+                    OneHotEncoder(
+                        categories="auto", handle_unknown="ignore", **not_sparse
+                    ),
+                ),
+            ]
+        )
+        return method
+
+    def _get_numeric_scaler(self) -> BaseEstimator:
+        return SKLPipeline(
+            steps=[
+                ("cast64", CastTransformer(dtype=np.float64)),
+                ("scaler", StandardScaler(with_mean=True, with_std=True)),
+                ("cast32", CastTransformer()),
+            ]
+        )
+
+    def _get_ordinal_encoder(self) -> BaseEstimator:
+        return SKLPipeline(
+            steps=[
+                ("cast_str", CastTransformer(dtype=np.str_)),
+                (
+                    "ord_enc",
+                    OrdinalEncoder(
+                        categories="auto",
+                        handle_unknown="use_encoded_value",
+                        unknown_value=-1,
+                    ),
+                ),
+                ("sc", MaxAbsScaler()),
+            ]
+        )
+
+    def fit(self, X: npt.NDArray, y: Any = None, *args: Any, **kwargs: Any) -> None:
         """
         Fits the encoder.
 
         Parameters
         ----------
         X : npt.NDArray
             data to encode
         _ : Any, optional
-            dummy argument to keep compatibility with pipeline training, by default None
+            dummy argument to keep compatibility with pipeline training
         """
         transformers = []
+
         for i, v in enumerate(self.mask):
-            if v == 1:
-                method = OneHotEncoder(
-                    categories="auto", sparse=False, handle_unknown="ignore"
-                )
-            elif v == 0:
-                method = SKLPipeline(steps = [('cast64', CastTransformer(dtype=np.float64)),('scaler', StandardScaler(with_mean=True, with_std=True)),('cast32', CastTransformer())])
+            if v == ColumnTypes.CAT_LOW_CARD:
+                method = self._get_ohe()
+            elif v == ColumnTypes.NUMERIC_REGULAR:
+                method = self._get_numeric_scaler()
             else:
-                method = SKLPipeline(steps=[('ord_enc', OrdinalEncoder(categories="auto", handle_unknown = "use_encoded_value", unknown_value = -1)), ('sc', MaxAbsScaler())])
-            
+                method = self._get_ordinal_encoder()
             t = (f"input {i}", method, [i])
             transformers.append(t)
 
         self.ct = ColumnTransformer(transformers)
         self.ct.fit(X)
 
-    def predict(self, X: npt.NDArray) -> npt.NDArray:
+    def predict(self, X: npt.NDArray, *args: Any, **kwargs: Any) -> npt.NDArray:
         """
         Applies the encoder.
 
         Parameters
         ----------
         X : npt.NDArray
             input data
@@ -75,70 +119,75 @@
         return self.ct.transform(X).astype(dtype=np.float32)
 
     def get_input_type(self) -> Type:
         """
         Returns
         -------
         Type
-            npt.NDArray[np.object_]
+            object
         """
         return npt.NDArray[np.object_]
 
     def get_output_type(self) -> Type:
         """
         Returns
         -------
         Type
             Float32Array
         """
         return Float32Array
 
-    def forward(self, X: npt.NDArray[np.object_]) -> npt.NDArray:
+    def forward(
+        self, X: npt.NDArray[np.object_], *args: Any, **kwargs: Any
+    ) -> npt.NDArray:
         """
         Equivalent of `.predict()` or `.transform()`.
 
 
         Parameters
         ----------
-        X : npt.NDArray[np.object_]
+        X : npt.NDArray[object]
             data to process
 
         Returns
         -------
         npt.NDArray
             processed data
         """
         return self.transform(X)
 
     def to_onnx(self) -> SerializedModelRepr:
         """
-        Serializes the encoder to onnx. 
+        Serializes the encoder to onnx.
         Each feature in the original dataset is mapped to its own input node (`float32` for numerical or `string` for categorical).
 
         Returns
         -------
         SerializedModelRepr
         """
         initial_types = []
         initial_types_str: List[str] = []
         initial_shapes: List[List[Optional[int]]] = []
         for i, t in enumerate(self.mask):
-            if t == 1 or t == 2:
-                tensor = StringTensorType([None, 1])
-                initial_types_str.append("STRING")
-            else:
+            if t in [ColumnTypes.NUMERIC_REGULAR]:
                 tensor = FloatTensorType([None, 1])
                 initial_types_str.append("FLOAT32")
+            else:
+                tensor = StringTensorType([None, 1])
+                initial_types_str.append("STRING")
             initial_types.append((f"input{i}", tensor))
             initial_shapes.append([None, 1])
         return SerializedModelRepr(
             convert_sklearn(
                 self.ct,
                 initial_types=initial_types,
-                target_opset={'': ONNX_OPSET_VERSION, 'ai.onnx.ml': ML_ONNX_OPSET_VERSION},
+                target_opset={
+                    "": ONNX_OPSET_VERSION,
+                    "ai.onnx.ml": ML_ONNX_OPSET_VERSION,
+                },
                 options={StandardScaler: {"div": "div_cast"}},
-            ).SerializeToString(),
+            ),
             len(self.mask),
             1,
             initial_types_str,
             initial_shapes,
         )
```

### Comparing `falcon-ml-0.5.0/falcon/tabular/reporting.py` & `falcon-ml-0.6.0/falcon/tabular/reporting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from numpy import typing as npt
 from typing import Dict
 import numpy as np
 from sklearn import metrics
-from falcon.tabular.utils import calculate_model_score
 
 def scale_acc(acc: float, n_classes: int) -> float: 
     if acc < 0. or acc > 1.:
         raise ValueError('Accuracy score should be in range [0,1]')
     elif acc == 0. or acc == 1. or n_classes < 3: 
         return acc
```

### Comparing `falcon-ml-0.5.0/falcon/tabular/tabular_manager.py` & `falcon-ml-0.6.0/falcon/tabular/tabular_manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 from __future__ import annotations
 from falcon.abstract import TaskManager, Pipeline
 from falcon.tabular.pipelines.simple_tabular_pipeline import SimpleTabularPipeline
 from falcon.tabular.utils import convert_to_np_obj
 from .reporting import print_classification_report, print_regression_report
 from falcon.tabular.utils import *
+from falcon.type_guessing import determine_column_types
 from falcon import types as ft
+from falcon.types import ColumnTypes
 from typing import Union, Optional, List, Tuple, Type, Dict, Any
 from numpy import typing as npt
 import pandas as pd
 from falcon.utils import print_, set_verbosity_level
 from sklearn.model_selection import train_test_split
 import os
 import pandas as pd
 
+
 class TabularTaskManager(TaskManager):
     """
     Default task manager for tabular data.
     """
 
     def __init__(
         self,
         task: str,
-        data: Union[str, npt.NDArray, pd.DataFrame, Tuple], 
+        data: Union[str, npt.NDArray, pd.DataFrame, Tuple],
         pipeline: Optional[Type[Pipeline]] = None,
         pipeline_options: Optional[Dict] = None,
         extra_pipeline_options: Optional[Dict] = None,
         features: Optional[ft.ColumnsList] = None,
         target: Optional[Union[str, int]] = None,
+        eval_strategy: Optional[Union[str, BaseCrossValidator, Callable]] = "auto",
         **options: Any,
     ) -> None:
         """
 
         Parameters
         ----------
         task : str
             `tabular_classification` or `tabular_regression`
         data : Union[str, npt.NDArray, pd.DataFrame, Tuple]
             path to data file or pandas dataframe or numpy array or tuple (X,y)
-        pipeline: Optional[Type[Pipeline]] 
+        pipeline: Optional[Type[Pipeline]]
             class to be used as pipeline, by default None.
             If None, `SimpleTabularPipeline` will be used
         pipeline_options : Optional[Dict], optional
             arguments to be passed to the pipeline, by default None.
             These options will overwrite the ones from `default_pipeline_options` attribute.
         extra_pipeline_options : Optional[Dict], optional
             arguments to be passed to the pipeline, by default None.
@@ -51,69 +55,118 @@
             names or indices of columns to be used as features, by default None.
             If None, all columns except the last one will be used.
             If `target` argument is not None, features should be passed explicitly as well
         target : Optional[Union[str, int]], optional
             name or index of column to be used as target, by default None.
             If None, the last column will be used as target.
             If `features` argument is not None, target should be specified explicitly as well
+        eval_strategy : Optional[Union[str, BaseCrossValidator, Callable]], optional
+            evaluation strategy, can be one of {'auto', 'holdout' 'cv', BaseCrossValidator, Callable} by default 'auto'.
+            If 'auto', uses 5 fold CV for small datasets and holdout for large ones.
+            If 'holdout', uses holdout strategy with 25% of data for validation.
+            If 'cv', uses 5 fold CV.
+            If BaseCrossValidator, uses the specified cross-validator.
+            If Callable, uses the specified function to split data into train and validation sets.
+            If None, no evaluation will be performed.
         """
         print_(f"\nInitializing a new TabularTaskManager for task `{task}`")
-
+        self._data: Tuple[npt.NDArray, npt.NDArray, List[ColumnTypes]]
+        # self._pipeline: Pipeline
         super().__init__(
             task=task,
             data=data,
             pipeline=pipeline,
             pipeline_options=pipeline_options,
             extra_pipeline_options=extra_pipeline_options,
             features=features,
             target=target,
         )
 
         self._eval_set: Optional[Tuple] = None
+        self._stored_cv_score: Optional[Dict] = None
+        self.eval_strategy = eval_strategy
+        if not self._validate_eval_strategy():
+            raise ValueError(
+                f"Invalid value for `eval_strategy` argument: {self.eval_strategy}"
+            )
+
+    def _validate_eval_strategy(self) -> bool:
+        if self.eval_strategy is None:
+            return True
+        if self.eval_strategy in ("auto", "cv", "holdout"):
+            return True
+        if isinstance(self.eval_strategy, BaseCrossValidator):
+            return True
+        if callable(self.eval_strategy):
+            return True
+        return False
+
+    def _infer_feature_names(self, data: Any) -> None:
+        print(type(data))
+        if (
+            isinstance(data, pd.DataFrame)
+            and self.features is None
+            and self.target is not None
+        ):
+            self.features: Optional[Union[List[str], List[int]]] = [c for c in data.columns if c != self.target]
+
 
     def _prepare_data(
         self, data: Union[str, npt.NDArray, pd.DataFrame, Tuple], training: bool = True
-    ) -> Tuple[npt.NDArray, npt.NDArray, List[int]]:
+    ) -> Tuple[npt.NDArray, npt.NDArray, List[ColumnTypes]]:
         """
-        Initial data preparation: 
+        Initial data preparation:
         1) optional: read data from the specified location;
         2) split into features and targets. By default it is assumed that the last column is the target;
         3) clean data;
         4) determine numerical and categorical features (create categorical mask).
 
         Parameters
         ----------
         data : Union[str, npt.NDArray, pd.DataFrame, Tuple]
             path to data file or pandas dataframe or numpy array or Tuple(X,y)
 
         Returns
         -------
-        Tuple[npt.NDArray, npt.NDArray, List[int]]
-            tuple of features, target and categorical mask for features
+        Tuple[npt.NDArray, npt.NDArray, List[ColumnTypes]]
+            tuple of features, target and type mask for features
         """
         if isinstance(data, str):
             data = read_data(data)
+            self._infer_feature_names(data)
         if isinstance(data, tuple):
-            if self.features is not None or self.target is not None: 
-                print('When data is passed as tuple of (X, y) all columns are used regardless the values of `features` or `target` arguments.')
-            if len(data) != 2: 
-                raise ValueError('When passing data as tuple, it should contain exactly 2 elements: `X` and `y`.')
+            if self.features is not None or self.target is not None:
+                print(
+                    "When data is passed as tuple of (X, y) all columns are used regardless the values of `features` or `target` arguments."
+                )
+            if len(data) != 2:
+                raise ValueError(
+                    "When passing data as tuple, it should contain exactly 2 elements: `X` and `y`."
+                )
             X, y = data
-            if len(y.shape) > 3 or len(X.shape) > 3: 
-                raise ValueError('Invalid data shape.')
-            if len(y.shape) > 1 and y.shape[-1] != 1: 
-                raise ValueError('The target should contain only one column.')
+            if isinstance(X, pd.DataFrame):
+                self.feature_names_to_save = list(X.columns)
+            if len(y.shape) > 3 or len(X.shape) > 3:
+                raise ValueError("Invalid data shape.")
+            if len(y.shape) > 1 and y.shape[-1] != 1:
+                raise ValueError("The target should contain only one column.")
             X, y = convert_to_np_obj(X), convert_to_np_obj(y)
         else:
+            self._infer_feature_names(data)
             X, y = split_features(data, features=self.features, target=self.target)
+            if self.features is None and isinstance(data, pd.DataFrame):
+                self.feature_names_to_save = list(data.columns[:-1])
+            elif self.features is not None:
+                self.feature_names_to_save = self.features
         X, y = clean_data_split(X, y)
-        mask: List[int]
+        self.dataset_size = X.shape
+        mask: List[ColumnTypes]
         if training:
-            mask = get_cat_mask(X)
-        else: 
+            mask = determine_column_types(X)
+        else:
             mask = []
         if len(y.shape) == 2:
             y = y.ravel()
         return X, y, mask
 
     @property
     def default_pipeline(self) -> Type[Pipeline]:
@@ -124,73 +177,74 @@
         return SimpleTabularPipeline
 
     @property
     def default_pipeline_options(self) -> Dict:
         """
         Default options for pipeline.
         """
-        options = {"mask": self._data[2]}
+        options: Dict[str, Any] = {"mask": self._data[2]}
         return options
-    
-    def _pre_eval_pipeline(self) -> float: 
-        print_("Pre-evaluation of model performance")
-        # TODO make `no_print` context manager
-        old_verbosity_level = int(os.getenv("FALCON_VERBOSITYLEVEL", "1"))
-        set_verbosity_level(0)
-        if (
-            self._data[0].shape[0] * self._data[0].shape[1] < 50000
-            or self._data[0].shape[0] < 500
-        ):
-            score = tab_cv_score(
-                self._pipeline, self._data[0], self._data[1], self.task
-            )
-            avg_score = float(np.mean(score))
-        else:
-            X_train, X_test, y_train, y_test = train_test_split(
-                self._data[0], self._data[1], test_size=0.25, stratify = self._data[1] if self.task == 'tabular_classification' else None
-            )
-            copied_pipeline = deepcopy(self._pipeline)
-            copied_pipeline.fit(X_train, y_train)
-            pred = copied_pipeline.predict(X_test)
-            avg_score = calculate_model_score(y_test, pred, self.task)
-        set_verbosity_level(old_verbosity_level)
-        return avg_score
 
+    def _cross_validate(self) -> None:
+        cv = (
+            self.eval_strategy
+            if isinstance(self.eval_strategy, BaseCrossValidator)
+            else None
+        )
+        scores = tab_cv_score(
+            self._pipeline, self._data[0], self._data[1], self.task, cv=cv
+        )
+        scores["N_SAMPLES"] = self.dataset_size[0]
+        self._stored_cv_score = scores
 
-    def train(self, make_eval_subset: bool = True, pre_eval: bool = False, **kwargs: Any) -> TabularTaskManager:
+    def train(self, **kwargs: Any) -> TabularTaskManager:
         """
-        Invokes the training procedure of an underlying pipeline. Print an expected model performance if available.
+        Invokes the training procedure of an underlying pipeline.
 
-        Parameters
-        ----------
-        pre_eval : bool
-            if True, first estimate model perfromance via 10 folds CV for small datasets or 25% test split for large datasets, by default False.
-            Setting pre_eval = True is not reccomended as it pre-evaluates the pipeline as a whole which has lots of random elements therefore the results might be non reproducable
-        make_eval_subset: bool
-            controls whether a dedicated eval set should be allocated for performance report, by default True. 
-            If True, overwrites the value of `pre_eval` to False
         Returns
         -------
         TabularTaskManager
             `self`
         """
         print_("Beginning training")
-        if make_eval_subset:
-            if self._eval_set is None:
-                X_train, X_eval, y_train, y_eval = train_test_split(
-                    self._data[0], self._data[1], test_size=0.25, stratify = self._data[1] if self.task == 'tabular_classification' else None
+        if self.eval_strategy is not None:
+            eval_strategy = self.eval_strategy
+            split_fn = None
+            if eval_strategy == "auto":
+                if self.dataset_size[0] < 2500:
+                    eval_strategy = "cv"
+                else:
+                    eval_strategy = "holdout"
+
+            if eval_strategy == "holdout":
+                split_fn = lambda X, y: train_test_split(
+                    X,
+                    y,
+                    test_size=0.25,
+                    stratify=y if self.task == "tabular_classification" else None,
                 )
-                self._data = (X_train, y_train, self._data[2])
-                self._eval_set = (X_eval, y_eval)
-            else: 
-                print('Evaluation set is already available.')
-        elif pre_eval:
-            print("Setting `pre_eval = True` is not reccomended as it pre evaluates the whole pipeline, can be lenghty and innacurate")
-            preeval_score = self._pre_eval_pipeline()
-            print(f"Pre evaluation score: {preeval_score}")
+            elif callable(eval_strategy) and not isinstance(
+                eval_strategy, BaseCrossValidator
+            ):
+                split_fn = eval_strategy
+
+            if callable(split_fn):
+                if self._eval_set is None:
+                    X_train, X_eval, y_train, y_eval = split_fn(
+                        self._data[0], self._data[1]
+                    )
+                    self._data = (X_train, y_train, self._data[2])
+                    self._eval_set = (X_eval, y_eval)
+                else:
+                    print_("Evaluation set is already available.")
+            elif eval_strategy == "cv" or isinstance(eval_strategy, BaseCrossValidator):
+                print_("Starting cross validation")
+                self._cross_validate()
+                print_("Finished cross-validation")
+
         print_("Beginning the main training phase")
         self._pipeline.fit(self._data[0], self._data[1])
         print_("Finished training")
         return self
 
     def predict(self, data: Union[str, npt.NDArray, pd.DataFrame]) -> npt.NDArray:
         """
@@ -208,78 +262,90 @@
         """
         if isinstance(data, str):
             data = read_data(data)
         if not isinstance(data, np.ndarray):
             data = np.asarray(data, dtype=np.object_)
         return self._pipeline.predict(data)
 
-    def predict_stored_subset(self, subset: str = 'train') -> npt.NDArray:
+    def predict_stored_subset(self, subset: str = "train") -> npt.NDArray:
         """
         Makes a prediction on a stored subset (`train` or `eval`).
 
         Parameters
         ----------
         subset : str, optional
             subset to predict on (train or eval), by default 'train'
 
         Returns
         -------
         npt.NDArray
             predicted values
         """
-        if subset == 'train': 
+        if subset == "train":
             return self.predict(self._data[0])
-        elif subset == 'eval':
-            if self._eval_set is None: 
-                raise RuntimeError('validation set is not available') 
+        elif subset == "eval":
+            if self._eval_set is None:
+                raise RuntimeError("validation set is not available")
             return self.predict(self._eval_set[0])
         else:
-            raise ValueError('subset should be either `train` or `eval`')
+            raise ValueError("subset should be either `train` or `eval`")
 
-    def performance_summary(self, test_data: Optional[Union[str, npt.NDArray, pd.DataFrame, Tuple]]) -> dict:
-        """
-        Prints a performance summary of the model. 
-        The summary always includes metrics calculated for the train set. 
-        If the train/eval split was done during training, the summary includes metrics calculated on eval set. 
+    def performance_summary(
+        self, test_data: Optional[Union[str, npt.NDArray, pd.DataFrame, Tuple]] = None
+    ) -> dict:
+        """
+        Prints a performance summary of the model.
+        The summary always includes metrics calculated for the train set.
+        If the train/eval split was done during training, the summary includes metrics calculated on eval set.
         If test set is provided as an argument, the performance includes metrics calculated on test set.
 
         Parameters
         ----------
         test_data : Optional[Union[str, npt.NDArray, pd.DataFrame, Tuple]]
             data to be used as test set, by default None
 
         Returns
         -------
         dict
             metrics for each subset
         """
         metrics_ = {}
-        report_fn = print_classification_report if self.task == 'tabular_classification' else print_regression_report
-        y_hat_train = self.predict_stored_subset('train')
-        metrics_['train'] = report_fn(self._data[1], y_hat_train, silent = True)
-        if self._eval_set is not None: 
-            y_hat_eval = self.predict_stored_subset('eval')
-            metrics_['eval'] = report_fn(self._eval_set[1], y_hat_eval, silent = True)
-        if test_data is not None: 
-            metrics_['test'] = self.evaluate(test_data, silent = True)
-        df = pd.DataFrame.from_dict(metrics_, orient = 'index')
+        report_fn = (
+            print_classification_report
+            if self.task == "tabular_classification"
+            else print_regression_report
+        )
+        y_hat_train = self.predict_stored_subset("train")
+        metrics_["train"] = report_fn(self._data[1], y_hat_train, silent=True)
+        if self._eval_set is not None:
+            y_hat_eval = self.predict_stored_subset("eval")
+            metrics_["eval"] = report_fn(self._eval_set[1], y_hat_eval, silent=True)
+        if self._stored_cv_score is not None:
+            metrics_["eval_cv"] = self._stored_cv_score
+        if test_data is not None:
+            metrics_["test"] = self.evaluate(test_data, silent=True)
+        df = pd.DataFrame.from_dict(metrics_, orient="index")
         print("\n", df, "\n")
         return metrics_
 
-    def evaluate(self, test_data: Union[str, npt.NDArray, pd.DataFrame, Tuple], silent: bool = False) -> Dict:
+    def evaluate(
+        self,
+        test_data: Union[str, npt.NDArray, pd.DataFrame, Tuple],
+        silent: bool = False,
+    ) -> Dict:
         """
         Perfoms and prints the evaluation report on the given dataset.
 
         Parameters
         ----------
         test_data : Union[str, npt.NDArray, pd.DataFrame, Tuple]
             dataset to be used for evaluation
         silent: bool
             controls whether the metrics are printed on screen, by default False
         """
         print("The evaluation report will be provided here")
-        X, y, _ = self._prepare_data(test_data, training = False)
+        X, y, _ = self._prepare_data(test_data, training=False)
         y_hat = self.predict(X)
         if self.task == "tabular_classification":
-            return print_classification_report(y, y_hat, silent = silent)
+            return print_classification_report(y, y_hat, silent=silent)
         else:
-            return print_regression_report(y, y_hat, silent = silent)
+            return print_regression_report(y, y_hat, silent=silent)
```

### Comparing `falcon-ml-0.5.0/falcon/tabular/utils.py` & `falcon-ml-0.6.0/falcon/tabular/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from copy import deepcopy
 import pandas as pd
-from typing import Union, Tuple, Optional, List
+from typing import Union, Tuple, Optional, List, Callable, Dict
 import numpy as np
 from numpy import isin, typing as npt
 from falcon import types as ft
-from ..abstract.task_pipeline import Pipeline
+from falcon.abstract.task_pipeline import Pipeline
+from falcon.types import ColumnTypes
 from sklearn.model_selection import RepeatedStratifiedKFold, RepeatedKFold
 from sklearn.metrics import balanced_accuracy_score, r2_score
-
+from sklearn.model_selection._split import BaseCrossValidator
+from falcon.tabular.reporting import print_classification_report, print_regression_report
 
 def read_data(path: str) -> pd.DataFrame:
     if path.endswith(".csv"):
         data = pd.read_csv(path)
     elif path.endswith(".parquet"):
         data = pd.read_parquet(path)
     else:
@@ -120,57 +122,43 @@
             y = data[:, -1]
         else:
             y = data[:, np.asarray(target, dtype=np.int64)]
 
     return convert_to_np_obj(X), convert_to_np_obj(y)
 
 
-def get_cat_mask(data: npt.NDArray) -> List[int]:
-    num_cat_threshold: int = 10
-    high_cardinality_threshold: int = 100
-    mask: List[int] = []  # True -> cat ; False -> num
-    tmp_df: pd.DataFrame = pd.DataFrame(data).infer_objects()
-    for col in range(tmp_df.shape[-1]):
-        if isinstance(
-            tmp_df.iloc[-1, col],
-            (int, float, np.int32, np.int64, np.float32, np.float64),
-        ):
-            if len(tmp_df.iloc[:, col].unique().tolist()) > num_cat_threshold:
-                mask.append(0)
-            else:
-                mask.append(1)
-        else:
-            if len(tmp_df.iloc[:, col].unique().tolist()) > high_cardinality_threshold:
-                mask.append(2)
-            else: 
-                mask.append(1)
-    return mask # 0 - numerical, 1 - cat low cardinality, 2 - cat high cardinality
-
-
 def calculate_model_score(y: npt.NDArray, y_hat: npt.NDArray, task: str) -> float:
     if task == "tabular_classification":
         return balanced_accuracy_score(y.astype(np.str_), y_hat)
     else:
         score = r2_score(y, y_hat)
         if score < 0:
             score = 0
         score = (score + 1) / 2
         return score
 
 
 def tab_cv_score(
-    pipeline: Pipeline, X: npt.NDArray, y: npt.NDArray, task: str, n_folds: int = 5
-) -> List[float]:
-    if task == "tabular_classification":
-        kf = RepeatedStratifiedKFold(n_splits=n_folds, n_repeats=1)
+    pipeline: Pipeline, X: npt.NDArray, y: npt.NDArray, task: str, cv: Optional[BaseCrossValidator] = None,
+) -> Dict[str, float]:
+    if cv is not None:
+        if not isinstance(cv, BaseCrossValidator):
+            raise ValueError("cv should be an instance of BaseCrossValidator")
+        kf = cv
+    elif task == "tabular_classification":
+        kf = RepeatedStratifiedKFold(n_splits=5, n_repeats=1)
         y = y.astype(np.str_)
     else:
-        kf = RepeatedKFold(n_splits=n_folds, n_repeats=1)
+        kf = RepeatedKFold(n_splits=5, n_repeats=1)
     scores = []
     for train_index, test_index in kf.split(X, y):
         copied_pipeline = deepcopy(pipeline)
         X_train, X_test = X[train_index], X[test_index]
         y_train, y_test = y[train_index], y[test_index]
         copied_pipeline.fit(X_train, y_train)
         pred = copied_pipeline.predict(X_test)
-        scores.append(calculate_model_score(y_test, pred, task))
-    return scores
+        report_fn = print_classification_report if task == 'tabular_classification' else print_regression_report
+        scores.append(report_fn(y_test, pred, silent = True))
+    mean_scores = {}
+    for key in scores[0].keys():
+        mean_scores[key] = np.mean([score[key] for score in scores])
+    return mean_scores
```

### Comparing `falcon-ml-0.5.0/falcon_ml.egg-info/SOURCES.txt` & `falcon-ml-0.6.0/falcon_ml.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,61 @@
 LICENSE
 README.md
 pyproject.toml
 falcon/__init__.py
 falcon/config.py
+falcon/constants.py
 falcon/datasets.py
 falcon/main.py
 falcon/runtime.py
 falcon/serialization.py
+falcon/sklapi.py
 falcon/task_configurations.py
+falcon/type_guessing.py
 falcon/types.py
 falcon/utils.py
 falcon/abstract/__init__.py
 falcon/abstract/learner.py
 falcon/abstract/model.py
 falcon/abstract/onnx_convertible.py
 falcon/abstract/optuna.py
 falcon/abstract/processor.py
 falcon/abstract/task_manager.py
 falcon/abstract/task_pipeline.py
 falcon/addons/sklearn/__init__.py
+falcon/addons/sklearn/decomposition/svd.py
 falcon/addons/sklearn/ensemble/balanced_stacking.py
 falcon/addons/sklearn/model_selection/balanced_strat_kfold.py
+falcon/addons/sklearn/preprocessing/date_tokenizer.py
 falcon/tabular/__init__.py
 falcon/tabular/configurations.py
 falcon/tabular/reporting.py
 falcon/tabular/tabular_manager.py
 falcon/tabular/utils.py
+falcon/tabular/wrappers.py
+falcon/tabular/adapters/ts/adapter.py
+falcon/tabular/adapters/ts/auxiliary.py
+falcon/tabular/adapters/ts/learner.py
+falcon/tabular/adapters/ts/pipeline.py
+falcon/tabular/adapters/ts/plot_errors.py
 falcon/tabular/learners/__init__.py
 falcon/tabular/learners/optuna_learner.py
+falcon/tabular/learners/plain_learner.py
 falcon/tabular/learners/super_learner.py
 falcon/tabular/models/__init__.py
 falcon/tabular/models/hist_gbt.py
 falcon/tabular/models/stacking.py
 falcon/tabular/pipelines/__init__.py
 falcon/tabular/pipelines/simple_tabular_pipeline.py
 falcon/tabular/processors/__init__.py
 falcon/tabular/processors/label_decoder.py
+falcon/tabular/processors/multi_modal_encoder.py
 falcon/tabular/processors/scaler_and_encoder.py
 falcon_ml.egg-info/PKG-INFO
 falcon_ml.egg-info/SOURCES.txt
 falcon_ml.egg-info/dependency_links.txt
 falcon_ml.egg-info/requires.txt
-falcon_ml.egg-info/top_level.txt
+falcon_ml.egg-info/top_level.txt
+tests/test_datasets.py
+tests/test_main.py
+tests/test_sklapi.py
+tests/test_type_guessing.py
```

### Comparing `falcon-ml-0.5.0/pyproject.toml` & `falcon-ml-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 dependencies = [
 "skl2onnx>=1.12.0",
 "scikit-learn>=1.1.0",
 "numpy>=1.18.0",
 "onnx>=1.12.0",
 "onnxruntime>=1.12.1",
 "pandas>=1.0.0", 
-"imbalanced-learn>=0.8.1", 
-"pymongo>=3.9.0", 
+"imbalanced-learn>=0.8.1",
 "pyarrow>=8.0.0",
-"optuna>=3.0.0"
+"optuna>=3.0.0", 
+"packaging>=20.0.0"
 ]
 name = "falcon-ml"
-version = "0.5.0"
+version = "0.6.0"
 authors = [
   { name="Oleg Kostromin", email="kostromin97@gmail.com" },
   { name="Iryna Kondrashchenko", email="iryna230520@gmail.com" },
   { name="Marco Pasini", email="marco.pasini.98@gmail.com" },
 ]
 description = "AutoML library for fast experementations."
 readme = "README.md"
```


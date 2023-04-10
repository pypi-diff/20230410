# Comparing `tmp/TSInterpret-0.1.2.tar.gz` & `tmp/TSInterpret-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSInterpret-0.1.2.tar", last modified: Fri Mar 10 17:55:33 2023, max compression
+gzip compressed data, was "TSInterpret-0.1.3.tar", last modified: Mon Apr 10 08:45:45 2023, max compression
```

## Comparing `TSInterpret-0.1.2.tar` & `TSInterpret-0.1.3.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 17:55:33.168248 TSInterpret-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 17:55:33.156248 TSInterpret-0.1.2/ClassificationModels/
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/ClassificationModels/CNN.py
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/ClassificationModels/CNN_T.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/ClassificationModels/DecisionTree.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/ClassificationModels/LSTM.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/ClassificationModels/LSTM_T.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/ClassificationModels/ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/ClassificationModels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/ClassificationModels/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-03-10 17:55:33.168248 TSInterpret-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 17:55:33.156248 TSInterpret-0.1.2/TSInterpret/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 17:55:33.160248 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/FeatureAttribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 17:55:33.160248 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/GradCam/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/GradCam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/InstanceBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 17:55:33.160248 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/Saliency/
--rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/Saliency/TSR.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/Saliency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 17:55:33.164248 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/counterfactual/Ates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10517 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/counterfactual/CF.py
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 17:55:33.164248 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 17:55:33.164248 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 17:55:33.164248 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/learning_process/
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 17:55:33.164248 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/leftist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/neighbors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 17:55:33.168248 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 17:55:33.168248 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 17:55:33.168248 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 17:55:33.168248 TSInterpret-0.1.2/TSInterpret/Models/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/Models/PyTorchModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/Models/SklearnModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/Models/TensorflowModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/Models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/TSInterpret/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 17:55:33.160248 TSInterpret-0.1.2/TSInterpret.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-03-10 17:55:33.000000 TSInterpret-0.1.2/TSInterpret.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-03-10 17:55:33.000000 TSInterpret-0.1.2/TSInterpret.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 17:55:33.000000 TSInterpret-0.1.2/TSInterpret.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-03-10 17:55:33.000000 TSInterpret-0.1.2/TSInterpret.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-10 17:55:33.000000 TSInterpret-0.1.2/TSInterpret.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 17:55:33.168248 TSInterpret-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-03-10 17:55:20.000000 TSInterpret-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:45:45.711140 TSInterpret-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:45:45.703140 TSInterpret-0.1.3/ClassificationModels/
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/ClassificationModels/CNN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/ClassificationModels/CNN_T.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/ClassificationModels/DecisionTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/ClassificationModels/LSTM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/ClassificationModels/LSTM_T.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/ClassificationModels/ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/ClassificationModels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/ClassificationModels/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-10 08:45:45.711140 TSInterpret-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:45:45.703140 TSInterpret-0.1.3/TSInterpret/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:45:45.707140 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/FeatureAttribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:45:45.707140 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/GradCam/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/GradCam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/InstanceBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:45:45.707140 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/Saliency/
+-rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/Saliency/TSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/Saliency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:45:45.707140 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/counterfactual/Ates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10517 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/counterfactual/CF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:45:45.707140 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:45:45.707140 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:45:45.707140 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/learning_process/
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:45:45.707140 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/leftist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/neighbors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:45:45.711140 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:45:45.711140 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:45:45.711140 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:45:45.711140 TSInterpret-0.1.3/TSInterpret/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/Models/PyTorchModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/Models/SklearnModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/Models/TensorflowModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/Models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/TSInterpret/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:45:45.703140 TSInterpret-0.1.3/TSInterpret.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-10 08:45:45.000000 TSInterpret-0.1.3/TSInterpret.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-10 08:45:45.000000 TSInterpret-0.1.3/TSInterpret.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:45:45.000000 TSInterpret-0.1.3/TSInterpret.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-10 08:45:45.000000 TSInterpret-0.1.3/TSInterpret.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 08:45:45.000000 TSInterpret-0.1.3/TSInterpret.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 08:45:45.711140 TSInterpret-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-10 08:45:36.000000 TSInterpret-0.1.3/setup.py
```

### Comparing `TSInterpret-0.1.2/ClassificationModels/CNN.py` & `TSInterpret-0.1.3/ClassificationModels/CNN.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/ClassificationModels/CNN_T.py` & `TSInterpret-0.1.3/ClassificationModels/CNN_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/ClassificationModels/DecisionTree.py` & `TSInterpret-0.1.3/ClassificationModels/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/ClassificationModels/LSTM.py` & `TSInterpret-0.1.3/ClassificationModels/LSTM.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/ClassificationModels/LSTM_T.py` & `TSInterpret-0.1.3/ClassificationModels/LSTM_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/ClassificationModels/ResNet.py` & `TSInterpret-0.1.3/ClassificationModels/ResNet.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/ClassificationModels/utils.py` & `TSInterpret-0.1.3/ClassificationModels/utils.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/LICENSE` & `TSInterpret-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/PKG-INFO` & `TSInterpret-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.1.2
+Version: 0.1.3
 Summary: todo
 Home-page: https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries
 Author: Jacqueline Hoellig
 Author-email: hoellig@fzi.de
 License: BSD-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
@@ -109,14 +109,23 @@
 ## :monocle_face: Why a special package for the interpretability of time series predictors? 
 
 Compared to other data types like tabular, image, or natural language data, time series data is unintuitive to understand. Approaches to the explainability of tabular regression and classification often assume independent features.  Compared to images or textual data, humans cannot intuitively and instinctively understand the underlying information contained in time series data. Further, research has shown that applying explainability algorithms for tabular, image, or natural language data often yields non-understandable  and inaccurate explanations, as they do not consider the time component (e.g., highlighting many unconnected time-steps, instead of features or time slices [1]). 
 Increasing research has focused on developing and adapting approaches to time series (survey: [2]). However, with no unified interface, accessibility to those methods is still an issue. TSInterpret tries to facilitate this by providing a PyPI package with a unified interface for multiple algorithms, documentation, and learning resources (notebooks) on the application.
 
 [2] Rojat, Thomas, et al. "Explainable artificial intelligence (xai) on timeseries data: A survey." arXiv preprint arXiv:2104.00950 (2021).
 
+## 👐 Contributing
+
+Feel free to contribute in any way you like, we're always open to new ideas and approaches.
+
+- If you have questions, spotted a bug or ideas, feel free to open an [issue](https://github.com/fzi-forschungszentrum-informatik/TSInterpret/issues/new/choose).
+- Before opening a pull request, we also encourage users to open an issue for discussion. 
+
+Details on how to Contribute can be found  [here](https://github.com/fzi-forschungszentrum-informatik/TSInterpret/blob/main/CONTRIBUTING.md).
+
 ## 🏫 Affiliations
 <p align="center">
     <img src="https://upload.wikimedia.org/wikipedia/de/thumb/4/44/Fzi_logo.svg/1200px-Fzi_logo.svg.png?raw=true" alt="FZI Logo" height="200"/>
 </p>
 
 ## Citation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TSInterpret Version: 0.1.2 Summary: todo Home-page:
+Metadata-Version: 2.1 Name: TSInterpret Version: 0.1.3 Summary: todo Home-page:
 https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries Author:
 Jacqueline Hoellig Author-email: hoellig@fzi.de License: BSD-3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
@@ -65,15 +65,21 @@
 or_time_slices_[1])._Increasing_research_has_focused_on_developing_and_adapting
 approaches_to_time_series_(survey:_[2])._However,_with_no_unified_interface,
 accessibility_to_those_methods_is_still_an_issue._TSInterpret_tries_to
 facilitate_this_by_providing_a_PyPI_package_with_a_unified_interface_for
 multiple_algorithms,_documentation,_and_learning_resources_(notebooks)_on_the
 application._[2]_Rojat,_Thomas,_et_al._"Explainable_artificial_intelligence
 (xai)_on_timeseries_data:_A_survey."_arXiv_preprint_arXiv:2104.00950_(2021)._##
-ð«_Affiliations
+ð_Contributing_Feel_free_to_contribute_in_any_way_you_like,_we're_always
+open_to_new_ideas_and_approaches._-_If_you_have_questions,_spotted_a_bug_or
+ideas,_feel_free_to_open_an_[issue](https://github.com/fzi-forschungszentrum-
+informatik/TSInterpret/issues/new/choose)._-_Before_opening_a_pull_request,_we
+also_encourage_users_to_open_an_issue_for_discussion._Details_on_how_to
+Contribute_can_be_found_[here](https://github.com/fzi-forschungszentrum-
+informatik/TSInterpret/blob/main/CONTRIBUTING.md)._##_ð«_Affiliations
                                   [FZI_Logo]
 ##_Citation_If_you_use_TSInterpret_in_your_research,_please_consider_citing_it
 and_the_authors'_original_papers._The_authors'_original_papers_are_cited_in_the
 documentation_and_the_paper_below._```_@misc{https://doi.org/10.48550/
 arxiv.2208.05280,_doi_=_{10.48550/ARXIV.2208.05280},_url_=_{https://arxiv.org/
 abs/2208.05280},_author_=_{HÃ¶llig,_Jacqueline_and_Kulbach,_Cedric_and_Thoma,
 Steffen},_keywords_=_{Machine_Learning_(cs.LG),_FOS:_Computer_and_information
```

### Comparing `TSInterpret-0.1.2/README.md` & `TSInterpret-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -83,14 +83,23 @@
 ## :monocle_face: Why a special package for the interpretability of time series predictors? 
 
 Compared to other data types like tabular, image, or natural language data, time series data is unintuitive to understand. Approaches to the explainability of tabular regression and classification often assume independent features.  Compared to images or textual data, humans cannot intuitively and instinctively understand the underlying information contained in time series data. Further, research has shown that applying explainability algorithms for tabular, image, or natural language data often yields non-understandable  and inaccurate explanations, as they do not consider the time component (e.g., highlighting many unconnected time-steps, instead of features or time slices [1]). 
 Increasing research has focused on developing and adapting approaches to time series (survey: [2]). However, with no unified interface, accessibility to those methods is still an issue. TSInterpret tries to facilitate this by providing a PyPI package with a unified interface for multiple algorithms, documentation, and learning resources (notebooks) on the application.
 
 [2] Rojat, Thomas, et al. "Explainable artificial intelligence (xai) on timeseries data: A survey." arXiv preprint arXiv:2104.00950 (2021).
 
+## 👐 Contributing
+
+Feel free to contribute in any way you like, we're always open to new ideas and approaches.
+
+- If you have questions, spotted a bug or ideas, feel free to open an [issue](https://github.com/fzi-forschungszentrum-informatik/TSInterpret/issues/new/choose).
+- Before opening a pull request, we also encourage users to open an issue for discussion. 
+
+Details on how to Contribute can be found  [here](https://github.com/fzi-forschungszentrum-informatik/TSInterpret/blob/main/CONTRIBUTING.md).
+
 ## 🏫 Affiliations
 <p align="center">
     <img src="https://upload.wikimedia.org/wikipedia/de/thumb/4/44/Fzi_logo.svg/1200px-Fzi_logo.svg.png?raw=true" alt="FZI Logo" height="200"/>
 </p>
 
 ## Citation
```

#### html2text {}

```diff
@@ -53,15 +53,21 @@
 or_time_slices_[1])._Increasing_research_has_focused_on_developing_and_adapting
 approaches_to_time_series_(survey:_[2])._However,_with_no_unified_interface,
 accessibility_to_those_methods_is_still_an_issue._TSInterpret_tries_to
 facilitate_this_by_providing_a_PyPI_package_with_a_unified_interface_for
 multiple_algorithms,_documentation,_and_learning_resources_(notebooks)_on_the
 application._[2]_Rojat,_Thomas,_et_al._"Explainable_artificial_intelligence
 (xai)_on_timeseries_data:_A_survey."_arXiv_preprint_arXiv:2104.00950_(2021)._##
-ð«_Affiliations
+ð_Contributing_Feel_free_to_contribute_in_any_way_you_like,_we're_always
+open_to_new_ideas_and_approaches._-_If_you_have_questions,_spotted_a_bug_or
+ideas,_feel_free_to_open_an_[issue](https://github.com/fzi-forschungszentrum-
+informatik/TSInterpret/issues/new/choose)._-_Before_opening_a_pull_request,_we
+also_encourage_users_to_open_an_issue_for_discussion._Details_on_how_to
+Contribute_can_be_found_[here](https://github.com/fzi-forschungszentrum-
+informatik/TSInterpret/blob/main/CONTRIBUTING.md)._##_ð«_Affiliations
                                   [FZI_Logo]
 ##_Citation_If_you_use_TSInterpret_in_your_research,_please_consider_citing_it
 and_the_authors'_original_papers._The_authors'_original_papers_are_cited_in_the
 documentation_and_the_paper_below._```_@misc{https://doi.org/10.48550/
 arxiv.2208.05280,_doi_=_{10.48550/ARXIV.2208.05280},_url_=_{https://arxiv.org/
 abs/2208.05280},_author_=_{HÃ¶llig,_Jacqueline_and_Kulbach,_Cedric_and_Thoma,
 Steffen},_keywords_=_{Machine_Learning_(cs.LG),_FOS:_Computer_and_information
```

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/FeatureAttribution.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/FeatureAttribution.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/InterpretabilityBase.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/InterpretabilityBase.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/Saliency/TSR.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/Saliency/TSR.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/counterfactual/Ates.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/counterfactual/Ates.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/counterfactual/CF.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/counterfactual/CF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,17 +91,18 @@
 
         if num_channels == 1:
             ind1[0], ind2[0] = tools.cxUniform(
                 np.array(ind1[0]).tolist(), np.array(ind2[0]).tolist(), indpb=0.1
             )
 
         else:
+
             items = np.where(channel1 == 1)
             if len(items[0]) != 0:
-                for item in items:
+                for item in items[0]:
                     ind1[item], ind2[item] = tools.cxUniform(
                         np.array(ind1[item]).tolist(),
                         np.array(ind2[item]).tolist(),
                         indpb=0.1,
                     )
 
     shape_new = np.array(ind1).reshape(1, -1).shape[1]
```

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/leftist.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/leftist.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/neighbors.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/neighbors.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/InterpretabilityModels/leftist/transform.py` & `TSInterpret-0.1.3/TSInterpret/InterpretabilityModels/leftist/transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/Models/PyTorchModel.py` & `TSInterpret-0.1.3/TSInterpret/Models/PyTorchModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/Models/SklearnModel.py` & `TSInterpret-0.1.3/TSInterpret/Models/SklearnModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/Models/TensorflowModel.py` & `TSInterpret-0.1.3/TSInterpret/Models/TensorflowModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret/Models/base_model.py` & `TSInterpret-0.1.3/TSInterpret/Models/base_model.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret.egg-info/PKG-INFO` & `TSInterpret-0.1.3/TSInterpret.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.1.2
+Version: 0.1.3
 Summary: todo
 Home-page: https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries
 Author: Jacqueline Hoellig
 Author-email: hoellig@fzi.de
 License: BSD-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
@@ -109,14 +109,23 @@
 ## :monocle_face: Why a special package for the interpretability of time series predictors? 
 
 Compared to other data types like tabular, image, or natural language data, time series data is unintuitive to understand. Approaches to the explainability of tabular regression and classification often assume independent features.  Compared to images or textual data, humans cannot intuitively and instinctively understand the underlying information contained in time series data. Further, research has shown that applying explainability algorithms for tabular, image, or natural language data often yields non-understandable  and inaccurate explanations, as they do not consider the time component (e.g., highlighting many unconnected time-steps, instead of features or time slices [1]). 
 Increasing research has focused on developing and adapting approaches to time series (survey: [2]). However, with no unified interface, accessibility to those methods is still an issue. TSInterpret tries to facilitate this by providing a PyPI package with a unified interface for multiple algorithms, documentation, and learning resources (notebooks) on the application.
 
 [2] Rojat, Thomas, et al. "Explainable artificial intelligence (xai) on timeseries data: A survey." arXiv preprint arXiv:2104.00950 (2021).
 
+## 👐 Contributing
+
+Feel free to contribute in any way you like, we're always open to new ideas and approaches.
+
+- If you have questions, spotted a bug or ideas, feel free to open an [issue](https://github.com/fzi-forschungszentrum-informatik/TSInterpret/issues/new/choose).
+- Before opening a pull request, we also encourage users to open an issue for discussion. 
+
+Details on how to Contribute can be found  [here](https://github.com/fzi-forschungszentrum-informatik/TSInterpret/blob/main/CONTRIBUTING.md).
+
 ## 🏫 Affiliations
 <p align="center">
     <img src="https://upload.wikimedia.org/wikipedia/de/thumb/4/44/Fzi_logo.svg/1200px-Fzi_logo.svg.png?raw=true" alt="FZI Logo" height="200"/>
 </p>
 
 ## Citation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TSInterpret Version: 0.1.2 Summary: todo Home-page:
+Metadata-Version: 2.1 Name: TSInterpret Version: 0.1.3 Summary: todo Home-page:
 https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries Author:
 Jacqueline Hoellig Author-email: hoellig@fzi.de License: BSD-3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
@@ -65,15 +65,21 @@
 or_time_slices_[1])._Increasing_research_has_focused_on_developing_and_adapting
 approaches_to_time_series_(survey:_[2])._However,_with_no_unified_interface,
 accessibility_to_those_methods_is_still_an_issue._TSInterpret_tries_to
 facilitate_this_by_providing_a_PyPI_package_with_a_unified_interface_for
 multiple_algorithms,_documentation,_and_learning_resources_(notebooks)_on_the
 application._[2]_Rojat,_Thomas,_et_al._"Explainable_artificial_intelligence
 (xai)_on_timeseries_data:_A_survey."_arXiv_preprint_arXiv:2104.00950_(2021)._##
-ð«_Affiliations
+ð_Contributing_Feel_free_to_contribute_in_any_way_you_like,_we're_always
+open_to_new_ideas_and_approaches._-_If_you_have_questions,_spotted_a_bug_or
+ideas,_feel_free_to_open_an_[issue](https://github.com/fzi-forschungszentrum-
+informatik/TSInterpret/issues/new/choose)._-_Before_opening_a_pull_request,_we
+also_encourage_users_to_open_an_issue_for_discussion._Details_on_how_to
+Contribute_can_be_found_[here](https://github.com/fzi-forschungszentrum-
+informatik/TSInterpret/blob/main/CONTRIBUTING.md)._##_ð«_Affiliations
                                   [FZI_Logo]
 ##_Citation_If_you_use_TSInterpret_in_your_research,_please_consider_citing_it
 and_the_authors'_original_papers._The_authors'_original_papers_are_cited_in_the
 documentation_and_the_paper_below._```_@misc{https://doi.org/10.48550/
 arxiv.2208.05280,_doi_=_{10.48550/ARXIV.2208.05280},_url_=_{https://arxiv.org/
 abs/2208.05280},_author_=_{HÃ¶llig,_Jacqueline_and_Kulbach,_Cedric_and_Thoma,
 Steffen},_keywords_=_{Machine_Learning_(cs.LG),_FOS:_Computer_and_information
```

### Comparing `TSInterpret-0.1.2/TSInterpret.egg-info/SOURCES.txt` & `TSInterpret-0.1.3/TSInterpret.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.1.2/TSInterpret.egg-info/requires.txt` & `TSInterpret-0.1.3/TSInterpret.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 scikit-learn==1.0.2
-torch
+torch<2.0,>=1.13.0
 pandas~=1.3.2
 numpy<2.0,>=1.21.6
 tqdm~=4.61.2
 h5py==3.7.0
 joblib<2.0,>=1.0.1
 Markdown<4.0,==3.3.4
 matplotlib<4.0,>=3.3.4
@@ -28,15 +28,15 @@
 wheel
 
 [:python_version == '3.8']
 dataclasses
 
 [all]
 scikit-learn==1.0.2
-torch
+torch<2.0,>=1.13.0
 pandas~=1.3.2
 numpy<2.0,>=1.21.6
 tqdm~=4.61.2
 h5py==3.7.0
 joblib<2.0,>=1.0.1
 Markdown<4.0,==3.3.4
 matplotlib<4.0,>=3.3.4
@@ -82,15 +82,15 @@
 nbconvert==6.4.2
 numpydoc==1.2
 spacy==3.2.2
 jinja2==3.0.3
 
 [dev]
 scikit-learn==1.0.2
-torch
+torch<2.0,>=1.13.0
 pandas~=1.3.2
 numpy<2.0,>=1.21.6
 tqdm~=4.61.2
 h5py==3.7.0
 joblib<2.0,>=1.0.1
 Markdown<4.0,==3.3.4
 matplotlib<4.0,>=3.3.4
@@ -138,15 +138,15 @@
 nbconvert==6.4.2
 numpydoc==1.2
 spacy==3.2.2
 jinja2==3.0.3
 
 [test]
 scikit-learn==1.0.2
-torch
+torch<2.0,>=1.13.0
 pandas~=1.3.2
 numpy<2.0,>=1.21.6
 tqdm~=4.61.2
 h5py==3.7.0
 joblib<2.0,>=1.0.1
 Markdown<4.0,==3.3.4
 matplotlib<4.0,>=3.3.4
```

### Comparing `TSInterpret-0.1.2/setup.py` & `TSInterpret-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 AUTHOR = "Jacqueline Hoellig"
 REQUIRES_PYTHON = ">=3.6.0"
 
 # Package requirements.
 base_packages = [
     "scikit-learn==1.0.2",
     # "scikit-surprise==1.1.1",
-    "torch",
+    "torch>=1.13.0,<2.0",
     "pandas~=1.3.2",
     "numpy>=1.21.6,< 2.0",
     "tqdm~=4.61.2",
     "h5py==3.7.0", # todo add version
     "joblib>=1.0.1,< 2.0",
     #"lime==0.2.0.1",
     "Markdown==3.3.4,< 4.0",
```


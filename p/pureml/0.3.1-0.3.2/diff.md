# Comparing `tmp/pureml-0.3.1.tar.gz` & `tmp/pureml-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pureml-0.3.1.tar", max compression
+gzip compressed data, was "pureml-0.3.2.tar", max compression
```

## Comparing `pureml-0.3.1.tar` & `pureml-0.3.2.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0    11370 2023-04-05 12:44:15.330474 pureml-0.3.1/README.md
--rw-r--r--   0        0        0      734 2023-04-08 14:57:03.440354 pureml-0.3.1/pureml/__init__.py
--rw-r--r--   0        0        0     2534 2023-02-10 14:59:50.822240 pureml-0.3.1/pureml/cli/__init__.py
--rw-r--r--   0        0        0    11620 2023-04-08 14:57:03.440354 pureml-0.3.1/pureml/cli/auth.py
--rw-r--r--   0        0        0        0 2023-04-06 11:08:34.084115 pureml-0.3.1/pureml/cli/config.py
--rw-r--r--   0        0        0      737 2023-04-08 14:57:03.440354 pureml-0.3.1/pureml/cli/main.py
--rw-r--r--   0        0        0     1924 2023-04-08 14:57:03.440354 pureml-0.3.1/pureml/cli/orgs.py
--rw-r--r--   0        0        0      451 2023-01-10 08:50:07.936557 pureml-0.3.1/pureml/cli/public.pem
--rw-r--r--   0        0        0     6501 2023-04-05 12:44:15.330474 pureml-0.3.1/pureml/cli/secrets.py
--rw-r--r--   0        0        0     1552 2023-04-05 12:44:15.330474 pureml-0.3.1/pureml/components/__init__.py
--rw-r--r--   0        0        0     1748 2023-03-15 11:32:06.993246 pureml-0.3.1/pureml/components/auth.py
--rw-r--r--   0        0        0    15690 2023-04-08 14:57:03.440354 pureml-0.3.1/pureml/components/dataset.py
--rw-r--r--   0        0        0       99 2023-04-05 12:44:15.342474 pureml-0.3.1/pureml/components/log/__init__.py
--rw-r--r--   0        0        0     7073 2023-04-05 12:44:15.702483 pureml-0.3.1/pureml/components/log/arrays.py
--rw-r--r--   0        0        0     6852 2023-04-05 12:44:15.702483 pureml-0.3.1/pureml/components/log/artifacts.py
--rw-r--r--   0        0        0     6830 2023-04-05 12:44:15.702483 pureml-0.3.1/pureml/components/log/audio.py
--rw-r--r--   0        0        0     9667 2023-04-05 12:44:15.702483 pureml-0.3.1/pureml/components/log/figure.py
--rw-r--r--   0        0        0     6801 2023-04-05 12:44:15.702483 pureml-0.3.1/pureml/components/log/image.py
--rw-r--r--   0        0        0     2052 2023-04-05 12:44:15.358475 pureml-0.3.1/pureml/components/log/log.py
--rw-r--r--   0        0        0     6045 2023-04-05 12:44:15.702483 pureml-0.3.1/pureml/components/log/metrics.py
--rw-r--r--   0        0        0     6016 2023-04-05 12:44:15.702483 pureml-0.3.1/pureml/components/log/params.py
--rw-r--r--   0        0        0     6196 2023-04-05 12:44:15.358475 pureml-0.3.1/pureml/components/log/pip_requirement.py
--rw-r--r--   0        0        0     6213 2023-04-05 12:44:15.358475 pureml-0.3.1/pureml/components/log/predict.py
--rw-r--r--   0        0        0     6029 2023-04-05 12:44:15.358475 pureml-0.3.1/pureml/components/log/resources.py
--rw-r--r--   0        0        0     6909 2023-04-05 12:44:15.698483 pureml-0.3.1/pureml/components/log/tabular.py
--rw-r--r--   0        0        0     6308 2023-04-05 12:44:15.698483 pureml-0.3.1/pureml/components/log/video.py
--rw-r--r--   0        0        0    13620 2023-04-08 14:57:03.440354 pureml-0.3.1/pureml/components/model.py
--rw-r--r--   0        0        0        0 2023-01-10 08:50:07.988555 pureml-0.3.1/pureml/config/__init__.py
--rw-r--r--   0        0        0     3753 2023-01-10 08:50:07.988555 pureml-0.3.1/pureml/config/parser.py
--rw-r--r--   0        0        0      123 2023-04-06 11:08:21.812260 pureml-0.3.1/pureml/decorators/__init__.py
--rw-r--r--   0        0        0     2219 2023-04-06 11:08:21.812260 pureml-0.3.1/pureml/decorators/dataset.py
--rw-r--r--   0        0        0      856 2023-04-05 12:44:15.358475 pureml-0.3.1/pureml/decorators/load_data.py
--rw-r--r--   0        0        0     2720 2023-04-05 12:44:15.358475 pureml-0.3.1/pureml/decorators/model.py
--rw-r--r--   0        0        0      607 2023-01-10 08:50:07.992555 pureml-0.3.1/pureml/decorators/pip_requirements.py
--rw-r--r--   0        0        0      838 2023-01-10 08:50:08.012554 pureml-0.3.1/pureml/decorators/predict.py
--rw-r--r--   0        0        0      895 2023-04-05 12:44:15.362475 pureml-0.3.1/pureml/decorators/transformer.py
--rw-r--r--   0        0        0       49 2023-04-05 12:44:15.362475 pureml-0.3.1/pureml/evaluate/__init__.py
--rw-r--r--   0        0        0     1489 2023-04-05 12:44:15.362475 pureml-0.3.1/pureml/evaluate/classification.py
--rw-r--r--   0        0        0     1766 2023-04-05 12:44:15.362475 pureml-0.3.1/pureml/evaluate/eval.py
--rw-r--r--   0        0        0     1665 2023-04-05 12:44:15.370475 pureml-0.3.1/pureml/evaluate/grade.py
--rw-r--r--   0        0        0      227 2023-04-05 12:44:15.382475 pureml-0.3.1/pureml/evaluate/metrics/__init__.py
--rw-r--r--   0        0        0      633 2023-04-05 12:44:15.398476 pureml-0.3.1/pureml/evaluate/metrics/accuracy.py
--rw-r--r--   0        0        0        0 2023-04-05 12:44:15.398476 pureml-0.3.1/pureml/evaluate/metrics/base.py
--rw-r--r--   0        0        0      673 2023-04-05 12:44:15.402476 pureml-0.3.1/pureml/evaluate/metrics/confusion_matrix.py
--rw-r--r--   0        0        0      699 2023-04-05 12:44:15.406476 pureml-0.3.1/pureml/evaluate/metrics/f1.py
--rw-r--r--   0        0        0      629 2023-04-05 12:44:15.406476 pureml-0.3.1/pureml/evaluate/metrics/mae.py
--rw-r--r--   0        0        0      686 2023-04-05 12:44:15.410476 pureml-0.3.1/pureml/evaluate/metrics/mse.py
--rw-r--r--   0        0        0      802 2023-04-05 12:44:15.418476 pureml-0.3.1/pureml/evaluate/metrics/precision.py
--rw-r--r--   0        0        0      787 2023-04-05 12:44:15.434476 pureml-0.3.1/pureml/evaluate/metrics/recall.py
--rw-r--r--   0        0        0     1225 2023-04-05 12:44:15.434476 pureml-0.3.1/pureml/evaluate/metrics/roc_auc.py
--rw-r--r--   0        0        0      654 2023-04-05 12:44:15.434476 pureml-0.3.1/pureml/evaluate/regression.py
--rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.1/pureml/lineage/__init__.py
--rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.1/pureml/lineage/data/__init__.py
--rw-r--r--   0        0        0     2852 2023-04-05 12:44:15.434476 pureml-0.3.1/pureml/lineage/data/create_lineage.py
--rw-r--r--   0        0        0        0 2023-03-15 11:32:07.345247 pureml-0.3.1/pureml/package/__init__.py
--rw-r--r--   0        0        0     4251 2023-04-05 12:44:15.466477 pureml-0.3.1/pureml/package/docker.py
--rw-r--r--   0        0        0     5913 2023-04-05 12:44:15.486478 pureml-0.3.1/pureml/package/fastapi.py
--rw-r--r--   0        0        0      876 2023-03-15 11:32:07.429247 pureml-0.3.1/pureml/packaging/__init__.py
--rw-r--r--   0        0        0      496 2023-01-10 08:50:08.016554 pureml-0.3.1/pureml/packaging/errors.py
--rw-r--r--   0        0        0     2245 2023-01-10 08:50:08.016554 pureml-0.3.1/pureml/packaging/model_framework.py
--rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.1/pureml/packaging/model_packaging/__init__.py
--rw-r--r--   0        0        0      973 2023-01-10 08:50:08.016554 pureml-0.3.1/pureml/packaging/model_packaging/catboost.py
--rw-r--r--   0        0        0     1103 2023-01-10 08:50:08.016554 pureml-0.3.1/pureml/packaging/model_packaging/custom.py
--rw-r--r--   0        0        0      965 2023-01-10 08:50:08.016554 pureml-0.3.1/pureml/packaging/model_packaging/keras.py
--rw-r--r--   0        0        0      976 2023-01-10 08:50:08.016554 pureml-0.3.1/pureml/packaging/model_packaging/lightgbm.py
--rw-r--r--   0        0        0     1075 2023-01-10 08:50:08.016554 pureml-0.3.1/pureml/packaging/model_packaging/pytorch.py
--rw-r--r--   0        0        0     1146 2023-01-10 08:50:08.016554 pureml-0.3.1/pureml/packaging/model_packaging/pytorch_tabnet.py
--rw-r--r--   0        0        0     2163 2023-01-10 08:50:08.016554 pureml-0.3.1/pureml/packaging/model_packaging/sklearn.py
--rw-r--r--   0        0        0     1028 2023-01-10 08:50:08.016554 pureml-0.3.1/pureml/packaging/model_packaging/tensorflow.py
--rw-r--r--   0        0        0     1021 2023-01-10 08:50:08.016554 pureml-0.3.1/pureml/packaging/model_packaging/xgboost.py
--rw-r--r--   0        0        0     4006 2023-03-15 11:32:07.457247 pureml-0.3.1/pureml/packaging/packaging.py
--rw-r--r--   0        0        0     1381 2023-01-10 08:50:08.016554 pureml-0.3.1/pureml/packaging/packaging_utils.py
--rw-r--r--   0        0        0        0 2023-03-15 11:32:07.457247 pureml-0.3.1/pureml/predictor/__init__.py
--rw-r--r--   0        0        0      778 2023-03-15 11:32:07.545248 pureml-0.3.1/pureml/predictor/predictor.py
--rw-r--r--   0        0        0      365 2023-04-05 12:44:15.486478 pureml-0.3.1/pureml/schema/__init__.py
--rw-r--r--   0        0        0      897 2023-04-06 11:08:34.088115 pureml-0.3.1/pureml/schema/backend.py
--rw-r--r--   0        0        0      350 2023-04-05 12:44:15.486478 pureml-0.3.1/pureml/schema/config.py
--rw-r--r--   0        0        0      330 2023-03-15 11:32:07.669248 pureml-0.3.1/pureml/schema/dataset.py
--rw-r--r--   0        0        0      474 2023-04-05 12:44:15.510478 pureml-0.3.1/pureml/schema/log.py
--rw-r--r--   0        0        0      396 2023-03-15 11:32:07.681248 pureml-0.3.1/pureml/schema/model.py
--rw-r--r--   0        0        0     1042 2023-04-05 12:44:15.510478 pureml-0.3.1/pureml/schema/packaging.py
--rw-r--r--   0        0        0     2528 2023-03-15 11:32:07.685248 pureml-0.3.1/pureml/schema/paths.py
--rw-r--r--   0        0        0     1048 2023-04-05 12:44:15.650482 pureml-0.3.1/pureml/schema/predict.py
--rw-r--r--   0        0        0      385 2023-03-15 11:32:07.733248 pureml-0.3.1/pureml/schema/singleton.py
--rw-r--r--   0        0        0      243 2023-04-05 12:44:15.510478 pureml-0.3.1/pureml/schema/storage.py
--rw-r--r--   0        0        0      177 2023-03-15 11:32:07.789248 pureml-0.3.1/pureml/schema/types.py
--rw-r--r--   0        0        0       66 2023-04-05 12:44:15.510478 pureml-0.3.1/pureml/settings/__init__.py
--rw-r--r--   0        0        0      278 2023-04-05 12:44:15.510478 pureml-0.3.1/pureml/settings/backend.py
--rw-r--r--   0        0        0      376 2023-04-05 12:44:15.510478 pureml-0.3.1/pureml/settings/storage.py
--rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.1/pureml/utils/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-05 12:44:15.510478 pureml-0.3.1/pureml/utils/config.py
--rw-r--r--   0        0        0     2234 2023-03-15 11:32:07.789248 pureml-0.3.1/pureml/utils/constants.py
--rw-r--r--   0        0        0     2998 2023-03-15 11:32:07.825248 pureml-0.3.1/pureml/utils/hash.py
--rw-r--r--   0        0        0      522 2023-02-10 14:59:51.046215 pureml-0.3.1/pureml/utils/log_utils.py
--rw-r--r--   0        0        0     1985 2023-03-15 11:32:07.865248 pureml-0.3.1/pureml/utils/package.py
--rw-r--r--   0        0        0    12921 2023-04-05 12:48:59.157035 pureml-0.3.1/pureml/utils/pipeline.py
--rw-r--r--   0        0        0     2868 2023-04-05 12:44:15.642481 pureml-0.3.1/pureml/utils/predict.py
--rw-r--r--   0        0        0      815 2023-02-10 14:59:51.066213 pureml-0.3.1/pureml/utils/readme.py
--rw-r--r--   0        0        0     1393 2023-04-05 12:44:15.542479 pureml-0.3.1/pureml/utils/resources.py
--rw-r--r--   0        0        0      137 2023-01-10 08:50:08.036553 pureml-0.3.1/pureml/utils/source_code.py
--rw-r--r--   0        0        0        0 2023-03-15 11:32:08.013249 pureml-0.3.1/pureml/utils/types.py
--rw-r--r--   0        0        0      698 2023-03-15 11:32:08.013249 pureml-0.3.1/pureml/utils/version_utils.py
--rw-r--r--   0        0        0     1903 2023-04-08 14:57:03.440354 pureml-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    13246 1970-01-01 00:00:00.000000 pureml-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11370 2023-04-05 12:44:15.330474 pureml-0.3.2/README.md
+-rw-r--r--   0        0        0      734 2023-04-10 21:14:43.159086 pureml-0.3.2/pureml/__init__.py
+-rw-r--r--   0        0        0     2534 2023-02-10 14:59:50.822240 pureml-0.3.2/pureml/cli/__init__.py
+-rw-r--r--   0        0        0    11620 2023-04-08 14:57:03.440354 pureml-0.3.2/pureml/cli/auth.py
+-rw-r--r--   0        0        0        0 2023-04-06 11:08:34.084115 pureml-0.3.2/pureml/cli/config.py
+-rw-r--r--   0        0        0      737 2023-04-08 14:57:03.440354 pureml-0.3.2/pureml/cli/main.py
+-rw-r--r--   0        0        0     1924 2023-04-08 14:57:03.440354 pureml-0.3.2/pureml/cli/orgs.py
+-rw-r--r--   0        0        0      451 2023-01-10 08:50:07.936557 pureml-0.3.2/pureml/cli/public.pem
+-rw-r--r--   0        0        0     6501 2023-04-05 12:44:15.330474 pureml-0.3.2/pureml/cli/secrets.py
+-rw-r--r--   0        0        0     1552 2023-04-05 12:44:15.330474 pureml-0.3.2/pureml/components/__init__.py
+-rw-r--r--   0        0        0     1748 2023-03-15 11:32:06.993246 pureml-0.3.2/pureml/components/auth.py
+-rw-r--r--   0        0        0    15690 2023-04-08 14:57:03.440354 pureml-0.3.2/pureml/components/dataset.py
+-rw-r--r--   0        0        0       99 2023-04-05 12:44:15.342474 pureml-0.3.2/pureml/components/log/__init__.py
+-rw-r--r--   0        0        0     7073 2023-04-05 12:44:15.702483 pureml-0.3.2/pureml/components/log/arrays.py
+-rw-r--r--   0        0        0     6852 2023-04-05 12:44:15.702483 pureml-0.3.2/pureml/components/log/artifacts.py
+-rw-r--r--   0        0        0     6830 2023-04-05 12:44:15.702483 pureml-0.3.2/pureml/components/log/audio.py
+-rw-r--r--   0        0        0     9667 2023-04-05 12:44:15.702483 pureml-0.3.2/pureml/components/log/figure.py
+-rw-r--r--   0        0        0     6801 2023-04-05 12:44:15.702483 pureml-0.3.2/pureml/components/log/image.py
+-rw-r--r--   0        0        0     2052 2023-04-05 12:44:15.358475 pureml-0.3.2/pureml/components/log/log.py
+-rw-r--r--   0        0        0     6045 2023-04-05 12:44:15.702483 pureml-0.3.2/pureml/components/log/metrics.py
+-rw-r--r--   0        0        0     6016 2023-04-05 12:44:15.702483 pureml-0.3.2/pureml/components/log/params.py
+-rw-r--r--   0        0        0     6198 2023-04-10 21:10:47.279602 pureml-0.3.2/pureml/components/log/pip_requirement.py
+-rw-r--r--   0        0        0     6214 2023-04-10 21:10:47.311604 pureml-0.3.2/pureml/components/log/predict.py
+-rw-r--r--   0        0        0     6084 2023-04-10 21:10:47.323604 pureml-0.3.2/pureml/components/log/resources.py
+-rw-r--r--   0        0        0     6909 2023-04-05 12:44:15.698483 pureml-0.3.2/pureml/components/log/tabular.py
+-rw-r--r--   0        0        0     6308 2023-04-05 12:44:15.698483 pureml-0.3.2/pureml/components/log/video.py
+-rw-r--r--   0        0        0    13620 2023-04-08 23:11:11.562439 pureml-0.3.2/pureml/components/model.py
+-rw-r--r--   0        0        0        0 2023-01-10 08:50:07.988555 pureml-0.3.2/pureml/config/__init__.py
+-rw-r--r--   0        0        0     3753 2023-01-10 08:50:07.988555 pureml-0.3.2/pureml/config/parser.py
+-rw-r--r--   0        0        0      123 2023-04-06 11:08:21.812260 pureml-0.3.2/pureml/decorators/__init__.py
+-rw-r--r--   0        0        0     2219 2023-04-06 11:08:21.812260 pureml-0.3.2/pureml/decorators/dataset.py
+-rw-r--r--   0        0        0      856 2023-04-05 12:44:15.358475 pureml-0.3.2/pureml/decorators/load_data.py
+-rw-r--r--   0        0        0     2720 2023-04-05 12:44:15.358475 pureml-0.3.2/pureml/decorators/model.py
+-rw-r--r--   0        0        0      607 2023-01-10 08:50:07.992555 pureml-0.3.2/pureml/decorators/pip_requirements.py
+-rw-r--r--   0        0        0      838 2023-01-10 08:50:08.012554 pureml-0.3.2/pureml/decorators/predict.py
+-rw-r--r--   0        0        0      895 2023-04-05 12:44:15.362475 pureml-0.3.2/pureml/decorators/transformer.py
+-rw-r--r--   0        0        0       49 2023-04-05 12:44:15.362475 pureml-0.3.2/pureml/evaluate/__init__.py
+-rw-r--r--   0        0        0     1489 2023-04-05 12:44:15.362475 pureml-0.3.2/pureml/evaluate/classification.py
+-rw-r--r--   0        0        0     1766 2023-04-05 12:44:15.362475 pureml-0.3.2/pureml/evaluate/eval.py
+-rw-r--r--   0        0        0     1665 2023-04-05 12:44:15.370475 pureml-0.3.2/pureml/evaluate/grade.py
+-rw-r--r--   0        0        0      227 2023-04-05 12:44:15.382475 pureml-0.3.2/pureml/evaluate/metrics/__init__.py
+-rw-r--r--   0        0        0      633 2023-04-05 12:44:15.398476 pureml-0.3.2/pureml/evaluate/metrics/accuracy.py
+-rw-r--r--   0        0        0        0 2023-04-05 12:44:15.398476 pureml-0.3.2/pureml/evaluate/metrics/base.py
+-rw-r--r--   0        0        0      673 2023-04-05 12:44:15.402476 pureml-0.3.2/pureml/evaluate/metrics/confusion_matrix.py
+-rw-r--r--   0        0        0      699 2023-04-05 12:44:15.406476 pureml-0.3.2/pureml/evaluate/metrics/f1.py
+-rw-r--r--   0        0        0      629 2023-04-05 12:44:15.406476 pureml-0.3.2/pureml/evaluate/metrics/mae.py
+-rw-r--r--   0        0        0      686 2023-04-05 12:44:15.410476 pureml-0.3.2/pureml/evaluate/metrics/mse.py
+-rw-r--r--   0        0        0      802 2023-04-05 12:44:15.418476 pureml-0.3.2/pureml/evaluate/metrics/precision.py
+-rw-r--r--   0        0        0      787 2023-04-05 12:44:15.434476 pureml-0.3.2/pureml/evaluate/metrics/recall.py
+-rw-r--r--   0        0        0     1225 2023-04-05 12:44:15.434476 pureml-0.3.2/pureml/evaluate/metrics/roc_auc.py
+-rw-r--r--   0        0        0      654 2023-04-05 12:44:15.434476 pureml-0.3.2/pureml/evaluate/regression.py
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.2/pureml/lineage/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:50.954225 pureml-0.3.2/pureml/lineage/data/__init__.py
+-rw-r--r--   0        0        0     2852 2023-04-05 12:44:15.434476 pureml-0.3.2/pureml/lineage/data/create_lineage.py
+-rw-r--r--   0        0        0        0 2023-03-15 11:32:07.345247 pureml-0.3.2/pureml/package/__init__.py
+-rw-r--r--   0        0        0     5795 2023-04-10 21:10:47.331605 pureml-0.3.2/pureml/package/docker.py
+-rw-r--r--   0        0        0     5913 2023-04-05 12:44:15.486478 pureml-0.3.2/pureml/package/fastapi.py
+-rw-r--r--   0        0        0      876 2023-03-15 11:32:07.429247 pureml-0.3.2/pureml/packaging/__init__.py
+-rw-r--r--   0        0        0      496 2023-01-10 08:50:08.016554 pureml-0.3.2/pureml/packaging/errors.py
+-rw-r--r--   0        0        0     2245 2023-01-10 08:50:08.016554 pureml-0.3.2/pureml/packaging/model_framework.py
+-rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.2/pureml/packaging/model_packaging/__init__.py
+-rw-r--r--   0        0        0      973 2023-01-10 08:50:08.016554 pureml-0.3.2/pureml/packaging/model_packaging/catboost.py
+-rw-r--r--   0        0        0     1103 2023-01-10 08:50:08.016554 pureml-0.3.2/pureml/packaging/model_packaging/custom.py
+-rw-r--r--   0        0        0      965 2023-01-10 08:50:08.016554 pureml-0.3.2/pureml/packaging/model_packaging/keras.py
+-rw-r--r--   0        0        0      976 2023-01-10 08:50:08.016554 pureml-0.3.2/pureml/packaging/model_packaging/lightgbm.py
+-rw-r--r--   0        0        0     1075 2023-01-10 08:50:08.016554 pureml-0.3.2/pureml/packaging/model_packaging/pytorch.py
+-rw-r--r--   0        0        0     1146 2023-01-10 08:50:08.016554 pureml-0.3.2/pureml/packaging/model_packaging/pytorch_tabnet.py
+-rw-r--r--   0        0        0     2163 2023-01-10 08:50:08.016554 pureml-0.3.2/pureml/packaging/model_packaging/sklearn.py
+-rw-r--r--   0        0        0     1028 2023-01-10 08:50:08.016554 pureml-0.3.2/pureml/packaging/model_packaging/tensorflow.py
+-rw-r--r--   0        0        0     1021 2023-01-10 08:50:08.016554 pureml-0.3.2/pureml/packaging/model_packaging/xgboost.py
+-rw-r--r--   0        0        0     4006 2023-03-15 11:32:07.457247 pureml-0.3.2/pureml/packaging/packaging.py
+-rw-r--r--   0        0        0     1381 2023-01-10 08:50:08.016554 pureml-0.3.2/pureml/packaging/packaging_utils.py
+-rw-r--r--   0        0        0        0 2023-03-15 11:32:07.457247 pureml-0.3.2/pureml/predictor/__init__.py
+-rw-r--r--   0        0        0      778 2023-03-15 11:32:07.545248 pureml-0.3.2/pureml/predictor/predictor.py
+-rw-r--r--   0        0        0      365 2023-04-05 12:44:15.486478 pureml-0.3.2/pureml/schema/__init__.py
+-rw-r--r--   0        0        0      897 2023-04-06 11:08:34.088115 pureml-0.3.2/pureml/schema/backend.py
+-rw-r--r--   0        0        0      350 2023-04-05 12:44:15.486478 pureml-0.3.2/pureml/schema/config.py
+-rw-r--r--   0        0        0      330 2023-03-15 11:32:07.669248 pureml-0.3.2/pureml/schema/dataset.py
+-rw-r--r--   0        0        0      474 2023-04-05 12:44:15.510478 pureml-0.3.2/pureml/schema/log.py
+-rw-r--r--   0        0        0      396 2023-03-15 11:32:07.681248 pureml-0.3.2/pureml/schema/model.py
+-rw-r--r--   0        0        0     1042 2023-04-05 12:44:15.510478 pureml-0.3.2/pureml/schema/packaging.py
+-rw-r--r--   0        0        0     2528 2023-03-15 11:32:07.685248 pureml-0.3.2/pureml/schema/paths.py
+-rw-r--r--   0        0        0     1048 2023-04-05 12:44:15.650482 pureml-0.3.2/pureml/schema/predict.py
+-rw-r--r--   0        0        0      385 2023-03-15 11:32:07.733248 pureml-0.3.2/pureml/schema/singleton.py
+-rw-r--r--   0        0        0      243 2023-04-05 12:44:15.510478 pureml-0.3.2/pureml/schema/storage.py
+-rw-r--r--   0        0        0      177 2023-03-15 11:32:07.789248 pureml-0.3.2/pureml/schema/types.py
+-rw-r--r--   0        0        0       66 2023-04-05 12:44:15.510478 pureml-0.3.2/pureml/settings/__init__.py
+-rw-r--r--   0        0        0      278 2023-04-05 12:44:15.510478 pureml-0.3.2/pureml/settings/backend.py
+-rw-r--r--   0        0        0      376 2023-04-05 12:44:15.510478 pureml-0.3.2/pureml/settings/storage.py
+-rw-r--r--   0        0        0        0 2023-01-10 08:50:08.016554 pureml-0.3.2/pureml/utils/__init__.py
+-rw-r--r--   0        0        0     1751 2023-04-05 12:44:15.510478 pureml-0.3.2/pureml/utils/config.py
+-rw-r--r--   0        0        0     2234 2023-03-15 11:32:07.789248 pureml-0.3.2/pureml/utils/constants.py
+-rw-r--r--   0        0        0     2998 2023-03-15 11:32:07.825248 pureml-0.3.2/pureml/utils/hash.py
+-rw-r--r--   0        0        0      522 2023-02-10 14:59:51.046215 pureml-0.3.2/pureml/utils/log_utils.py
+-rw-r--r--   0        0        0     1985 2023-03-15 11:32:07.865248 pureml-0.3.2/pureml/utils/package.py
+-rw-r--r--   0        0        0    14445 2023-04-10 21:10:47.359606 pureml-0.3.2/pureml/utils/pipeline.py
+-rw-r--r--   0        0        0     2868 2023-04-05 12:44:15.642481 pureml-0.3.2/pureml/utils/predict.py
+-rw-r--r--   0        0        0      815 2023-02-10 14:59:51.066213 pureml-0.3.2/pureml/utils/readme.py
+-rw-r--r--   0        0        0     1393 2023-04-05 12:44:15.542479 pureml-0.3.2/pureml/utils/resources.py
+-rw-r--r--   0        0        0      137 2023-01-10 08:50:08.036553 pureml-0.3.2/pureml/utils/source_code.py
+-rw-r--r--   0        0        0        0 2023-03-15 11:32:08.013249 pureml-0.3.2/pureml/utils/types.py
+-rw-r--r--   0        0        0      698 2023-03-15 11:32:08.013249 pureml-0.3.2/pureml/utils/version_utils.py
+-rw-r--r--   0        0        0     1927 2023-04-10 21:14:43.159086 pureml-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    13291 1970-01-01 00:00:00.000000 pureml-0.3.2/PKG-INFO
```

### Comparing `pureml-0.3.1/README.md` & `pureml-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/__init__.py` & `pureml-0.3.2/pureml/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 from .evaluate import grader, eval
 
 from .package import docker, fastapi
 
 from .schema import Input, Output
 from .predictor.predictor import BasePredictor
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
```

### Comparing `pureml-0.3.1/pureml/cli/__init__.py` & `pureml-0.3.2/pureml/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/cli/auth.py` & `pureml-0.3.2/pureml/cli/auth.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/cli/main.py` & `pureml-0.3.2/pureml/cli/main.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/cli/orgs.py` & `pureml-0.3.2/pureml/cli/orgs.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/cli/secrets.py` & `pureml-0.3.2/pureml/cli/secrets.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/components/__init__.py` & `pureml-0.3.2/pureml/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/components/auth.py` & `pureml-0.3.2/pureml/components/auth.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/components/dataset.py` & `pureml-0.3.2/pureml/components/dataset.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/components/log/arrays.py` & `pureml-0.3.2/pureml/components/log/arrays.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/components/log/artifacts.py` & `pureml-0.3.2/pureml/components/log/artifacts.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/components/log/audio.py` & `pureml-0.3.2/pureml/components/log/audio.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/components/log/figure.py` & `pureml-0.3.2/pureml/components/log/figure.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/components/log/image.py` & `pureml-0.3.2/pureml/components/log/image.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/components/log/log.py` & `pureml-0.3.2/pureml/components/log/log.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/components/log/metrics.py` & `pureml-0.3.2/pureml/components/log/metrics.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/components/log/params.py` & `pureml-0.3.2/pureml/components/log/params.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/components/log/pip_requirement.py` & `pureml-0.3.2/pureml/components/log/pip_requirement.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         }
 
         # print("figure url", url)
 
         # response = requests.get(url, headers=headers)
         response = requests.get(url)
 
-        print(response.status_code)
+        # print(response.status_code)
 
         if response.ok:
             print(
                 "[bold green] pip_requirement file {} has been fetched".format(
                     file_name
                 )
             )
```

### Comparing `pureml-0.3.1/pureml/components/log/predict.py` & `pureml-0.3.2/pureml/components/log/predict.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         # print("save path", save_path)
 
         headers = {
             "Content-Type": "application/x-www-form-urlencoded",
             "Authorization": "Bearer {}".format(user_token),
         }
 
-        # print("figure url", url)
+        # print("predict url", url)
 
         response = requests.get(url)
 
         # print(response.status_code)
 
         if response.ok:
             print("[bold green] predict file {} has been fetched".format(file_name))
```

### Comparing `pureml-0.3.1/pureml/components/log/resources.py` & `pureml-0.3.2/pureml/components/log/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,27 +143,27 @@
     org_id = get_org_id()
 
     def fetch_resource(file_details):
 
         file_name, url = file_details
 
         save_path = os.path.join(path_schema.PATH_PREDICT_DIR, file_name)
-        print("save path", save_path)
+        # print("save path", save_path)
 
         headers = {
             "Content-Type": "application/x-www-form-urlencoded",
             "Authorization": "Bearer {}".format(user_token),
         }
 
-        # print("figure url", url)
+        # print("resorce url", url)
 
         # response = requests.get(url, headers=headers)
         response = requests.get(url)
 
-        print(response.status_code)
+        # print(response.status_code)
 
         if response.ok:
             print("[bold green] resource {} has been fetched".format(file_name))
 
             save_dir = os.path.dirname(save_path)
 
             os.makedirs(save_dir, exist_ok=True)
@@ -182,14 +182,15 @@
             return response.text
         else:
             print("[bold red] Unable to fetch the resource")
 
             return response.text
 
     resource_details = details(label=label)
+    # print("resource_details", resource_details)
 
     if resource_details is None:
         return
 
     # pred_urls = give_resource_urls(details=resource_details)
     pred_urls = give_resource_url(details=resource_details, key=post_key_resources)
```

### Comparing `pureml-0.3.1/pureml/components/log/tabular.py` & `pureml-0.3.2/pureml/components/log/tabular.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/components/log/video.py` & `pureml-0.3.2/pureml/components/log/video.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/components/model.py` & `pureml-0.3.2/pureml/components/model.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/config/parser.py` & `pureml-0.3.2/pureml/config/parser.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/decorators/dataset.py` & `pureml-0.3.2/pureml/decorators/dataset.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/decorators/load_data.py` & `pureml-0.3.2/pureml/decorators/load_data.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/decorators/model.py` & `pureml-0.3.2/pureml/decorators/model.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/decorators/pip_requirements.py` & `pureml-0.3.2/pureml/decorators/pip_requirements.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/decorators/predict.py` & `pureml-0.3.2/pureml/decorators/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/decorators/transformer.py` & `pureml-0.3.2/pureml/decorators/transformer.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/evaluate/classification.py` & `pureml-0.3.2/pureml/evaluate/classification.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/evaluate/eval.py` & `pureml-0.3.2/pureml/evaluate/eval.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/evaluate/grade.py` & `pureml-0.3.2/pureml/evaluate/grade.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/evaluate/metrics/accuracy.py` & `pureml-0.3.2/pureml/evaluate/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/evaluate/metrics/confusion_matrix.py` & `pureml-0.3.2/pureml/evaluate/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/evaluate/metrics/f1.py` & `pureml-0.3.2/pureml/evaluate/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/evaluate/metrics/mae.py` & `pureml-0.3.2/pureml/evaluate/metrics/mae.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/evaluate/metrics/mse.py` & `pureml-0.3.2/pureml/evaluate/metrics/mse.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/evaluate/metrics/precision.py` & `pureml-0.3.2/pureml/evaluate/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/evaluate/metrics/recall.py` & `pureml-0.3.2/pureml/evaluate/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/evaluate/metrics/roc_auc.py` & `pureml-0.3.2/pureml/evaluate/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/evaluate/regression.py` & `pureml-0.3.2/pureml/evaluate/regression.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/lineage/data/create_lineage.py` & `pureml-0.3.2/pureml/lineage/data/create_lineage.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/package/docker.py` & `pureml-0.3.2/pureml/package/docker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import docker
 from .fastapi import create_fastapi_file
 from pureml.schema import FastAPISchema, PredictSchema, DockerSchema
+import string, random
 
 prediction_schema = PredictSchema()
 fastapi_schema = FastAPISchema()
 docker_schema = DockerSchema()
 
 
 def create_docker_file(org_id, access_token):
@@ -76,91 +77,138 @@
         CONTAINER_NAME="pureml_prediction",
     )
 
     with open(docker_schema.PATH_DOCKER_CONFIG, "w") as docker_yaml_file:
         docker_yaml_file.write(docker_yaml)
 
 
-def create_docker_image(image_tag=None):
-    if image_tag is None:
-        image_tag = "pureml_docker_image"
-    else:
-        image_tag = image_tag.replace(" ", "")
+def create_docker_image(label):
+    # if image_tag is None:
+    # image_tag = "pureml_docker_image"
+    label = label.replace(" ", "")
 
-        client = docker.from_env()
+    image_repository = label.split(":", 1)[0]
+    image_tag = label.split(":", 1)[1].replace(":", "-")
 
-        docker_file_path_relative = docker_schema.PATH_DOCKER_IMAGE.split(os.path.sep)[
-            -1
-        ]
+    # random_value = "".join(random.choices(string.ascii_lowercase + string.digits, k=8))
+    # image_tag = "-".join([image_tag, random_value])
 
-        try:
-            image, build_log = client.images.build(
-                path=docker_schema.paths.PATH_PREDICT_DIR,
-                dockerfile=docker_file_path_relative,
-                tag=image_tag,
-                nocache=True,
-                rm=True,
-            )
+    image_tag = ":".join([image_repository, image_tag])
+
+    client = docker.from_env()
+
+    docker_file_path_relative = docker_schema.PATH_DOCKER_IMAGE.split(os.path.sep)[-1]
+    # print(docker_schema.paths.PATH_PREDICT_DIR)
+    # print(docker_file_path_relative)
+    # print(image_tag)
+
+    try:
+        image, build_log = client.images.build(
+            path=docker_schema.paths.PATH_PREDICT_DIR,
+            dockerfile=docker_file_path_relative,
+            tag=image_tag,
+            nocache=True,
+            rm=True,
+        )
 
-            print("Docker image is created")
-            print(image)
+        print("Docker image is created.")
+        print("Tag: ", image_tag)
+        print("Image Long Id:", image.id)
+        print("Image Short Id: ", image.short_id)
 
-        except Exception as e:
-            print(e)
-            image = None
+    except Exception as e:
+        print(e)
+        image = None
+        build_log = None
 
-        return image
+    return image, build_log, image_tag
 
 
-def run_docker_container(image, name):
+def run_docker_container(image, runtime, gpu_ids, host_port):
     client = docker.from_env()
+    name = image.tags[0].replace(":", "-")
+
+    random_value = "".join(random.choices(string.ascii_lowercase + string.digits, k=8))
+    name = "-".join([name, random_value])
+
+    docker_port = "{p}/tcp".format(p=docker_schema.PORT_DOCKER)
 
-    docker_port = "{port}/tcp".format(port=docker_schema.PORT_DOCKER)
     # print(docker_port)
+    container_args = {
+        "image": image,
+        "ports": {docker_port: host_port},
+        "detach": True,
+        "auto_remove": True,
+        "name": name,
+        "runtime": runtime,
+    }
+
+    if len(gpu_ids) != 0:
+        gpu_ids = [str(id) for id in gpu_ids]
+        container_args["device_requests"] = [
+            docker.types.DeviceRequest(device_ids=gpu_ids, capabilities=[["gpu"]])
+        ]
 
-    container = client.containers.run(
-        image=image,
-        ports={docker_port: docker_schema.PORT_HOST},
-        detach=True,
-        name=name,
-    )
+    container = client.containers.run(**container_args)
+
+    # container = client.containers.run(
+    #     image=image,
+    #     ports={docker_port: docker_schema.PORT_HOST},
+    #     detach=True,
+    #     name=name,
+    #     runtime=runtime,
+    # )
 
     return container
 
 
 def create(
     label,
     org_id,
     access_token,
-    image_tag=None,
+    runtime=None,
+    gpu_ids=[],
+    port=None,
     predict_path=None,
     requirements_path=None,
-    container_name=None,
 ):
 
     create_fastapi_file(
         label=label, predict_path=predict_path, requirements_path=requirements_path
     )
 
     create_docker_file(org_id=org_id, access_token=access_token)
 
-    image = create_docker_image(image_tag)
+    image, build_log, image_tag = create_docker_image(label=label)
 
     if image is not None:
-        container = run_docker_container(image=image, name=container_name)
+
+        if port is None:
+            host_port = docker_schema.PORT_HOST
+        else:
+            host_port = port
+
+        container = run_docker_container(
+            image=image, runtime=runtime, gpu_ids=gpu_ids, host_port=host_port
+        )
 
         print("Created Docker container")
-        print(container)
+        print("Container Name: ", container.name)
+        print("Container Long Id: ", container.id)
+        print("Container id: ", container.short_id)
+
         print(
             "Prediction requests can be forwarded to {ip}:{port}/predict".format(
-                ip=docker_schema.API_IP_HOST, port=docker_schema.PORT_HOST
+                ip=docker_schema.API_IP_HOST, port=host_port
             )
         )
     else:
         print("Failed to create the container")
+        print("Build Log")
+        print(build_log)
 
 
 def get(container_id):
 
     client = docker.from_env()
 
     container = client.containers.get(container_id)
```

### Comparing `pureml-0.3.1/pureml/package/fastapi.py` & `pureml-0.3.2/pureml/package/fastapi.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/packaging/__init__.py` & `pureml-0.3.2/pureml/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/packaging/model_framework.py` & `pureml-0.3.2/pureml/packaging/model_framework.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/packaging/model_packaging/catboost.py` & `pureml-0.3.2/pureml/packaging/model_packaging/catboost.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/packaging/model_packaging/custom.py` & `pureml-0.3.2/pureml/packaging/model_packaging/custom.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/packaging/model_packaging/keras.py` & `pureml-0.3.2/pureml/packaging/model_packaging/keras.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/packaging/model_packaging/lightgbm.py` & `pureml-0.3.2/pureml/packaging/model_packaging/lightgbm.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/packaging/model_packaging/pytorch.py` & `pureml-0.3.2/pureml/packaging/model_packaging/pytorch.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/packaging/model_packaging/pytorch_tabnet.py` & `pureml-0.3.2/pureml/packaging/model_packaging/pytorch_tabnet.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/packaging/model_packaging/sklearn.py` & `pureml-0.3.2/pureml/packaging/model_packaging/sklearn.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/packaging/model_packaging/tensorflow.py` & `pureml-0.3.2/pureml/packaging/model_packaging/tensorflow.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/packaging/model_packaging/xgboost.py` & `pureml-0.3.2/pureml/packaging/model_packaging/xgboost.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/packaging/packaging.py` & `pureml-0.3.2/pureml/packaging/packaging.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/packaging/packaging_utils.py` & `pureml-0.3.2/pureml/packaging/packaging_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/predictor/predictor.py` & `pureml-0.3.2/pureml/predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/schema/backend.py` & `pureml-0.3.2/pureml/schema/backend.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/schema/packaging.py` & `pureml-0.3.2/pureml/schema/packaging.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/schema/paths.py` & `pureml-0.3.2/pureml/schema/paths.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/schema/predict.py` & `pureml-0.3.2/pureml/schema/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/utils/config.py` & `pureml-0.3.2/pureml/utils/config.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/utils/constants.py` & `pureml-0.3.2/pureml/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/utils/hash.py` & `pureml-0.3.2/pureml/utils/hash.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/utils/log_utils.py` & `pureml-0.3.2/pureml/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/utils/package.py` & `pureml-0.3.2/pureml/utils/package.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/utils/pipeline.py` & `pureml-0.3.2/pureml/utils/pipeline.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .hash import generate_hash_for_dict, generate_hash_for_function
 from .source_code import get_source_code
 import os
 import shutil
 from .log_utils import update_step_dict
 import time
 from pureml.schema import ConfigKeys
+from datetime import datetime
 
 config_keys = ConfigKeys
 
 
 def add_load_data_to_config(name, description=None, func=None, hash=""):
 
     config = load_config()
@@ -18,18 +19,21 @@
         try:
             code = get_source_code(func)
             hash = generate_hash_for_function(func)
         except Exception as e:
             print("Unable to get load_data source code")
             print(e)
 
+    current_datetime = datetime.now()
+    current_datetime = str(current_datetime.strftime("%d %b %Y, %H:%M"))
+
     config[config_keys.load_data.value] = {
         "name": name,
         "desc": str(description),
-        "time": str(time.time()),
+        "time": current_datetime,
         "hash": hash,
         "type": config_keys.load_data.value,
         "code": code,
     }
 
     save_config(config=config)
 
@@ -55,18 +59,21 @@
         try:
             code = get_source_code(func)
             hash = generate_hash_for_function(func)
         except Exception as e:
             print("Unable to get transformer source code")
             print(e)
 
+    current_datetime = datetime.now()
+    current_datetime = str(current_datetime.strftime("%d %b %Y, %H:%M"))
+
     config[config_keys.transformer.value][position] = {
         "name": name,
         "desc": str(description),
-        "time": str(time.time()),
+        "time": current_datetime,
         "hash": hash,
         "type": config_keys.transformer.value,
         "parent": parent,
         "code": code,
     }
     # print('saveing configuration for ', name)
     save_config(config=config)
@@ -90,18 +97,21 @@
         try:
             code = get_source_code(func)
             hash = generate_hash_for_function(func)
         except Exception as e:
             print("Unable to get dataset source code")
             print(e)
 
+    current_datetime = datetime.now()
+    current_datetime = str(current_datetime.strftime("%d %b %Y, %H:%M"))
+
     config[config_keys.dataset.value] = {
         "name": name,
         "desc": str(description),
-        "time": str(time.time()),
+        "time": current_datetime,
         "branch": branch,
         "hash": hash,
         "type": config_keys.dataset.value,
         "version": version,
         "parent": parent,
         "code": code,
     }
@@ -121,23 +131,26 @@
         try:
             code = get_source_code(func)
             hash = generate_hash_for_function(func)
         except Exception as e:
             print("Unable to get model source code")
             print(e)
 
+    current_datetime = datetime.now()
+    current_datetime = str(current_datetime.strftime("%d %b %Y, %H:%M"))
+
     # Empty hash is passed to create the empty model with just model name the first time
     # Complete hash is passed to create the model with all the details in the second time
     if hash == "":
         position = len(config[config_keys.model.value]) + 1
 
         config[config_keys.model.value][position] = {
             "name": name,
             "desc": str(description),
-            "time": str(time.time()),
+            "time": current_datetime,
             "branch": branch,
             "hash": hash,
             "version": version,
             "code": code,
         }
     else:
         position = len(config[config_keys.model.value])
@@ -169,21 +182,25 @@
     else:
         metric_values = values
 
         # print('not default',metric_values)
 
     hash = generate_hash_for_dict(values=metric_values)
 
+    current_datetime = datetime.now()
+    current_datetime = str(current_datetime.strftime("%d %b %Y, %H:%M"))
+
     config[config_keys.metrics.value].update(
         {
             "values": metric_values,
             "hash": hash,
             "model_name": model_name,
             "model_branch": model_branch,
             "model_version": model_version,
+            "time": current_datetime,
         }
     )
 
     save_config(config=config)
 
 
 def load_metrics_from_config():
@@ -215,21 +232,25 @@
         param_values.update(values)
     else:
         param_values = values
 
     hash = generate_hash_for_dict(values=param_values)
     # print("params", model_version)
 
+    current_datetime = datetime.now()
+    current_datetime = str(current_datetime.strftime("%d %b %Y, %H:%M"))
+
     config[config_keys.params.value].update(
         {
             "values": param_values,
             "hash": hash,
             "model_name": model_name,
             "model_branch": model_branch,
             "model_version": model_version,
+            "time": current_datetime,
         }
     )
 
     save_config(config=config)
 
 
 def load_params_from_config():
@@ -260,21 +281,25 @@
         figure_values.update(values)
     else:
         figure_values = values
 
     hash = generate_hash_for_dict(values=figure_values)
     # print("figures", model_version)
 
+    current_datetime = datetime.now()
+    current_datetime = str(current_datetime.strftime("%d %b %Y, %H:%M"))
+
     config[config_keys.figure.value].update(
         {
             "values": figure_values,
             "hash": hash,
             "model_name": model_name,
             "model_branch": model_branch,
             "model_version": model_version,
+            "time": current_datetime,
         }
     )
 
     save_config(config=config)
 
 
 def load_figures_from_config():
@@ -306,21 +331,25 @@
         pred_function_values = values
     else:
         pred_function_values = values
 
     hash = generate_hash_for_dict(values=pred_function_values)
     # print("pred_function", model_version)
 
+    current_datetime = datetime.now()
+    current_datetime = str(current_datetime.strftime("%d %b %Y, %H:%M"))
+
     config[config_keys.pred_function.value].update(
         {
             "values": pred_function_values,
             "hash": hash,
             "model_name": model_name,
             "model_branch": model_branch,
             "model_version": model_version,
+            "time": current_datetime,
         }
     )
 
     save_config(config=config)
 
 
 def load_pred_from_config():
@@ -352,21 +381,25 @@
         pip_requirement_values = values
     else:
         pip_requirement_values = values
 
     hash = generate_hash_for_dict(values=pip_requirement_values)
     # print("pred_function", model_version)
 
+    current_datetime = datetime.now()
+    current_datetime = str(current_datetime.strftime("%d %b %Y, %H:%M"))
+
     config[config_keys.pip_requirement.value].update(
         {
             "values": pip_requirement_values,
             "hash": hash,
             "model_name": model_name,
             "model_branch": model_branch,
             "model_version": model_version,
+            "time": current_datetime,
         }
     )
 
     save_config(config=config)
 
 
 def load_pip_req_from_config():
@@ -398,21 +431,25 @@
         pip_requirement_values = values
     else:
         pip_requirement_values = values
 
     hash = generate_hash_for_dict(values=pip_requirement_values)
     # print("pred_function", model_version)
 
+    current_datetime = datetime.now()
+    current_datetime = str(current_datetime.strftime("%d %b %Y, %H:%M"))
+
     config[config_keys.resource.value].update(
         {
             "values": pip_requirement_values,
             "hash": hash,
             "model_name": model_name,
             "model_branch": model_branch,
             "model_version": model_version,
+            "time": current_datetime,
         }
     )
 
     save_config(config=config)
 
 
 def load_resource_from_config():
@@ -433,21 +470,25 @@
     version = ""
     config = load_config()
 
     model_name, model_branch, model_version, model_hash = get_model_latest(
         config=config
     )
 
+    current_datetime = datetime.now()
+    current_datetime = str(current_datetime.strftime("%d %b %Y, %H:%M"))
+
     position = len(config[config_keys.artifacts.value]) + 1
     config[config_keys.artifacts.value][position] = {
         "name": name,
         "hash": hash,
         "version": version,
         "model_name": model_name,
         "model_version": model_version,
+        "time": current_datetime,
     }
 
 
 def get_model_latest(config, version="latest"):
     config_model = config[config_keys.model.value]
     model_name = None
     model_version = None
```

### Comparing `pureml-0.3.1/pureml/utils/predict.py` & `pureml-0.3.2/pureml/utils/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/utils/readme.py` & `pureml-0.3.2/pureml/utils/readme.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/utils/resources.py` & `pureml-0.3.2/pureml/utils/resources.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pureml/utils/version_utils.py` & `pureml-0.3.2/pureml/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.3.1/pyproject.toml` & `pureml-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pureml"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 license = "Apache-2.0"
 authors = ["vamsidhar muthireddy <vamsi.muthireddy@gmail.com>"]
 readme = "README.md"
 homepage = "https://pureml.com/"
 repository = "https://github.com/engageml-github/Pure"
 documentation = "https://docs.pureml.com"
@@ -37,14 +37,15 @@
 fastapi = "^0.88.0"
 uvicorn = "^0.20.0"
 docker = "^6.0.1"
 python-multipart = "^0.0.5"
 nest-asyncio = "^1.5.6"
 pyngrok = "^5.2.1"
 ipapi = "^1.0.4"
+scikit-learn = "^1.2.2"
 
 [tool.poetry.dev-dependencies]
 ipykernel = "^6.19.2"
 lightgbm = "^3.3.2"
 xgboost = "^1.6.1"
 catboost = "^1.0.6"
 scikit-learn = "^1.1.1"
```

### Comparing `pureml-0.3.1/PKG-INFO` & `pureml-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pureml
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Home-page: https://pureml.com/
 License: Apache-2.0
 Keywords: pureml,model-store,machine-learning,python,model-registry,collabortion
 Author: vamsidhar muthireddy
 Author-email: vamsi.muthireddy@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -33,14 +33,15 @@
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: pyarrow (>=8.0.0,<9.0.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: pyngrok (>=5.2.1,<6.0.0)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: typer[all] (>=0.6.1,<0.7.0)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
 Project-URL: Documentation, https://docs.pureml.com
 Project-URL: Repository, https://github.com/engageml-github/Pure
 Description-Content-Type: text/markdown
 
 [![PureML](/assets/SDKCoverImg.png)](https://pureml.com)
```


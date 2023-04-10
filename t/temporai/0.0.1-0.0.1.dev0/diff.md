# Comparing `tmp/temporai-0.0.1-py3-none-any.whl.zip` & `tmp/temporai-0.0.1.dev0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,116 +1,48 @@
-Zip file size: 163693 bytes, number of entries: 114
--rw-rw-rw-  2.0 fat      353 b- defN 23-Apr-10 17:20 hydra_plugins/tempor_searchpath_plugin.py
--rw-rw-rw-  2.0 fat      725 b- defN 23-Apr-10 17:20 tempor/__init__.py
--rw-rw-rw-  2.0 fat      391 b- defN 23-Apr-10 17:20 tempor/benchmarks/__init__.py
--rw-rw-rw-  2.0 fat     3901 b- defN 23-Apr-10 17:20 tempor/benchmarks/benchmark.py
--rw-rw-rw-  2.0 fat    25736 b- defN 23-Apr-10 17:20 tempor/benchmarks/evaluation.py
--rw-rw-rw-  2.0 fat    30051 b- defN 23-Apr-10 17:20 tempor/benchmarks/metrics.py
--rw-rw-rw-  2.0 fat     2476 b- defN 23-Apr-10 17:20 tempor/benchmarks/utils.py
--rw-rw-rw-  2.0 fat     4134 b- defN 23-Apr-10 17:20 tempor/config/__init__.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-10 17:20 tempor/config/conf/__init__.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-10 17:20 tempor/config/conf/tempor/__init__.py
--rw-rw-rw-  2.0 fat      175 b- defN 23-Apr-10 17:20 tempor/config/conf/tempor/config.yaml
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-10 17:20 tempor/core/__init__.py
--rw-rw-rw-  2.0 fat     2126 b- defN 23-Apr-10 17:20 tempor/core/pydantic_utils.py
--rw-rw-rw-  2.0 fat     2353 b- defN 23-Apr-10 17:20 tempor/core/utils.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-10 17:20 tempor/data/__init__.py
--rw-rw-rw-  2.0 fat     7816 b- defN 23-Apr-10 17:20 tempor/data/clv2conv.py
--rw-rw-rw-  2.0 fat     1930 b- defN 23-Apr-10 17:20 tempor/data/data_typing.py
--rw-rw-rw-  2.0 fat     5196 b- defN 23-Apr-10 17:20 tempor/data/dataloader.py
--rw-rw-rw-  2.0 fat    22737 b- defN 23-Apr-10 17:20 tempor/data/dataset.py
--rw-rw-rw-  2.0 fat    14378 b- defN 23-Apr-10 17:20 tempor/data/pandera_utils.py
--rw-rw-rw-  2.0 fat     6235 b- defN 23-Apr-10 17:20 tempor/data/predictive.py
--rw-rw-rw-  2.0 fat    31955 b- defN 23-Apr-10 17:20 tempor/data/samples.py
--rw-rw-rw-  2.0 fat     1407 b- defN 23-Apr-10 17:20 tempor/data/settings.py
--rw-rw-rw-  2.0 fat    19885 b- defN 23-Apr-10 17:20 tempor/data/utils.py
--rw-rw-rw-  2.0 fat      300 b- defN 23-Apr-10 17:20 tempor/exc/__init__.py
--rw-rw-rw-  2.0 fat       60 b- defN 23-Apr-10 17:20 tempor/log/__init__.py
--rw-rw-rw-  2.0 fat     3262 b- defN 23-Apr-10 17:20 tempor/log/_custom_logger.py
--rw-rw-rw-  2.0 fat      235 b- defN 23-Apr-10 17:20 tempor/log/_custom_logger.pyi
--rw-rw-rw-  2.0 fat      644 b- defN 23-Apr-10 17:20 tempor/log/log_helpers.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-10 17:20 tempor/models/__init__.py
--rw-rw-rw-  2.0 fat      703 b- defN 23-Apr-10 17:20 tempor/models/constants.py
--rw-rw-rw-  2.0 fat    21824 b- defN 23-Apr-10 17:20 tempor/models/ddh.py
--rw-rw-rw-  2.0 fat    15688 b- defN 23-Apr-10 17:20 tempor/models/mlp.py
--rw-rw-rw-  2.0 fat     2786 b- defN 23-Apr-10 17:20 tempor/models/samplers.py
--rw-rw-rw-  2.0 fat     3192 b- defN 23-Apr-10 17:20 tempor/models/transformer.py
--rw-rw-rw-  2.0 fat    28705 b- defN 23-Apr-10 17:20 tempor/models/ts_model.py
--rw-rw-rw-  2.0 fat    31391 b- defN 23-Apr-10 17:20 tempor/models/ts_ode.py
--rw-rw-rw-  2.0 fat     5969 b- defN 23-Apr-10 17:20 tempor/models/utils.py
--rw-rw-rw-  2.0 fat       83 b- defN 23-Apr-10 17:20 tempor/plugins/__init__.py
--rw-rw-rw-  2.0 fat      253 b- defN 23-Apr-10 17:20 tempor/plugins/_plugin_loader.py
--rw-rw-rw-  2.0 fat      461 b- defN 23-Apr-10 17:20 tempor/plugins/core/__init__.py
--rw-rw-rw-  2.0 fat     4146 b- defN 23-Apr-10 17:20 tempor/plugins/core/_base_estimator.py
--rw-rw-rw-  2.0 fat     2884 b- defN 23-Apr-10 17:20 tempor/plugins/core/_base_predictor.py
--rw-rw-rw-  2.0 fat     1128 b- defN 23-Apr-10 17:20 tempor/plugins/core/_base_transformer.py
--rw-rw-rw-  2.0 fat     2048 b- defN 23-Apr-10 17:20 tempor/plugins/core/_params.py
--rw-rw-rw-  2.0 fat     7722 b- defN 23-Apr-10 17:20 tempor/plugins/core/_plugin.py
--rw-rw-rw-  2.0 fat      174 b- defN 23-Apr-10 17:20 tempor/plugins/core/_types.py
--rw-rw-rw-  2.0 fat     2057 b- defN 23-Apr-10 17:20 tempor/plugins/core/utils.py
--rw-rw-rw-  2.0 fat     2977 b- defN 23-Apr-10 17:20 tempor/plugins/pipeline/__init__.py
--rw-rw-rw-  2.0 fat     3991 b- defN 23-Apr-10 17:20 tempor/plugins/pipeline/generators.py
--rw-rw-rw-  2.0 fat       84 b- defN 23-Apr-10 17:20 tempor/plugins/prediction/__init__.py
--rw-rw-rw-  2.0 fat      102 b- defN 23-Apr-10 17:20 tempor/plugins/prediction/one_off/__init__.py
--rw-rw-rw-  2.0 fat     2709 b- defN 23-Apr-10 17:20 tempor/plugins/prediction/one_off/classification/__init__.py
--rw-rw-rw-  2.0 fat     6907 b- defN 23-Apr-10 17:20 tempor/plugins/prediction/one_off/classification/plugin_cde_classifier.py
--rw-rw-rw-  2.0 fat     7436 b- defN 23-Apr-10 17:20 tempor/plugins/prediction/one_off/classification/plugin_laplace_classifier.py
--rw-rw-rw-  2.0 fat     7080 b- defN 23-Apr-10 17:20 tempor/plugins/prediction/one_off/classification/plugin_nn_classifier.py
--rw-rw-rw-  2.0 fat     6905 b- defN 23-Apr-10 17:20 tempor/plugins/prediction/one_off/classification/plugin_ode_classifier.py
--rw-rw-rw-  2.0 fat     2136 b- defN 23-Apr-10 17:20 tempor/plugins/prediction/one_off/regression/__init__.py
--rw-rw-rw-  2.0 fat     6805 b- defN 23-Apr-10 17:20 tempor/plugins/prediction/one_off/regression/plugin_cde_regressor.py
--rw-rw-rw-  2.0 fat     7334 b- defN 23-Apr-10 17:20 tempor/plugins/prediction/one_off/regression/plugin_laplace_regressor.py
--rw-rw-rw-  2.0 fat     6449 b- defN 23-Apr-10 17:20 tempor/plugins/prediction/one_off/regression/plugin_nn_regressor.py
--rw-rw-rw-  2.0 fat     6802 b- defN 23-Apr-10 17:20 tempor/plugins/prediction/one_off/regression/plugin_ode_regressor.py
--rw-rw-rw-  2.0 fat      102 b- defN 23-Apr-10 17:20 tempor/plugins/prediction/temporal/__init__.py
--rw-rw-rw-  2.0 fat     2606 b- defN 23-Apr-10 17:20 tempor/plugins/prediction/temporal/classification/__init__.py
--rw-rw-rw-  2.0 fat     5794 b- defN 23-Apr-10 17:20 tempor/plugins/prediction/temporal/classification/plugin_seq2seq_classifier.py
--rw-rw-rw-  2.0 fat     1839 b- defN 23-Apr-10 17:20 tempor/plugins/prediction/temporal/regression/__init__.py
--rw-rw-rw-  2.0 fat     5563 b- defN 23-Apr-10 17:20 tempor/plugins/prediction/temporal/regression/plugin_seq2seq_regressor.py
--rw-rw-rw-  2.0 fat      105 b- defN 23-Apr-10 17:20 tempor/plugins/preprocessing/__init__.py
--rw-rw-rw-  2.0 fat      134 b- defN 23-Apr-10 17:20 tempor/plugins/preprocessing/imputation/__init__.py
--rw-rw-rw-  2.0 fat      211 b- defN 23-Apr-10 17:20 tempor/plugins/preprocessing/imputation/_base.py
--rw-rw-rw-  2.0 fat      297 b- defN 23-Apr-10 17:20 tempor/plugins/preprocessing/imputation/static/__init__.py
--rw-rw-rw-  2.0 fat     3702 b- defN 23-Apr-10 17:20 tempor/plugins/preprocessing/imputation/static/plugin_static_imputation.py
--rw-rw-rw-  2.0 fat      299 b- defN 23-Apr-10 17:20 tempor/plugins/preprocessing/imputation/temporal/__init__.py
--rw-rw-rw-  2.0 fat     3544 b- defN 23-Apr-10 17:20 tempor/plugins/preprocessing/imputation/temporal/plugin_bfill.py
--rw-rw-rw-  2.0 fat     3501 b- defN 23-Apr-10 17:20 tempor/plugins/preprocessing/imputation/temporal/plugin_ffill.py
--rw-rw-rw-  2.0 fat      835 b- defN 23-Apr-10 17:20 tempor/plugins/preprocessing/nop/__init__.py
--rw-rw-rw-  2.0 fat      132 b- defN 23-Apr-10 17:20 tempor/plugins/preprocessing/scaling/__init__.py
--rw-rw-rw-  2.0 fat      210 b- defN 23-Apr-10 17:20 tempor/plugins/preprocessing/scaling/_base.py
--rw-rw-rw-  2.0 fat      292 b- defN 23-Apr-10 17:20 tempor/plugins/preprocessing/scaling/static/__init__.py
--rw-rw-rw-  2.0 fat     2254 b- defN 23-Apr-10 17:20 tempor/plugins/preprocessing/scaling/static/plugin_static_minmax_scaler.py
--rw-rw-rw-  2.0 fat     2115 b- defN 23-Apr-10 17:20 tempor/plugins/preprocessing/scaling/static/plugin_static_standard_scaler.py
--rw-rw-rw-  2.0 fat      294 b- defN 23-Apr-10 17:20 tempor/plugins/preprocessing/scaling/temporal/__init__.py
--rw-rw-rw-  2.0 fat     2176 b- defN 23-Apr-10 17:20 tempor/plugins/preprocessing/scaling/temporal/plugin_ts_minmax_scaler.py
--rw-rw-rw-  2.0 fat     2037 b- defN 23-Apr-10 17:20 tempor/plugins/preprocessing/scaling/temporal/plugin_ts_standard_scaler.py
--rw-rw-rw-  2.0 fat     2114 b- defN 23-Apr-10 17:20 tempor/plugins/time_to_event/__init__.py
--rw-rw-rw-  2.0 fat     9375 b- defN 23-Apr-10 17:20 tempor/plugins/time_to_event/helper_embedding.py
--rw-rw-rw-  2.0 fat     7872 b- defN 23-Apr-10 17:20 tempor/plugins/time_to_event/plugin_ddh.py
--rw-rw-rw-  2.0 fat     7417 b- defN 23-Apr-10 17:20 tempor/plugins/time_to_event/plugin_ts_coxph.py
--rw-rw-rw-  2.0 fat     9831 b- defN 23-Apr-10 17:20 tempor/plugins/time_to_event/plugin_ts_xgb.py
--rw-rw-rw-  2.0 fat       84 b- defN 23-Apr-10 17:20 tempor/plugins/treatments/__init__.py
--rw-rw-rw-  2.0 fat      184 b- defN 23-Apr-10 17:20 tempor/plugins/treatments/one_off/__init__.py
--rw-rw-rw-  2.0 fat     1756 b- defN 23-Apr-10 17:20 tempor/plugins/treatments/one_off/_base.py
--rw-rw-rw-  2.0 fat      453 b- defN 23-Apr-10 17:20 tempor/plugins/treatments/one_off/classification/__init__.py
--rw-rw-rw-  2.0 fat      355 b- defN 23-Apr-10 17:20 tempor/plugins/treatments/one_off/regression/__init__.py
--rw-rw-rw-  2.0 fat     5311 b- defN 23-Apr-10 17:20 tempor/plugins/treatments/one_off/regression/plugin_synctwin_regressor.py
--rw-rw-rw-  2.0 fat      188 b- defN 23-Apr-10 17:20 tempor/plugins/treatments/temporal/__init__.py
--rw-rw-rw-  2.0 fat     1763 b- defN 23-Apr-10 17:20 tempor/plugins/treatments/temporal/_base.py
--rw-rw-rw-  2.0 fat      365 b- defN 23-Apr-10 17:20 tempor/plugins/treatments/temporal/classification/__init__.py
--rw-rw-rw-  2.0 fat     7029 b- defN 23-Apr-10 17:20 tempor/plugins/treatments/temporal/classification/plugin_crn_classifier.py
--rw-rw-rw-  2.0 fat      361 b- defN 23-Apr-10 17:20 tempor/plugins/treatments/temporal/regression/__init__.py
--rw-rw-rw-  2.0 fat     7228 b- defN 23-Apr-10 17:20 tempor/plugins/treatments/temporal/regression/plugin_crn_regressor.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-10 17:20 tempor/utils/__init__.py
--rw-rw-rw-  2.0 fat      631 b- defN 23-Apr-10 17:20 tempor/utils/serialization.py
--rw-rw-rw-  2.0 fat      535 b- defN 23-Apr-10 17:20 tempor/utils/dataloaders/__init__.py
--rw-rw-rw-  2.0 fat     5342 b- defN 23-Apr-10 17:20 tempor/utils/dataloaders/dummy.py
--rw-rw-rw-  2.0 fat     2796 b- defN 23-Apr-10 17:20 tempor/utils/dataloaders/google_stocks.py
--rw-rw-rw-  2.0 fat     4832 b- defN 23-Apr-10 17:20 tempor/utils/dataloaders/pbc.py
--rw-rw-rw-  2.0 fat     1557 b- defN 23-Apr-10 17:20 tempor/utils/dataloaders/pkpd.py
--rw-rw-rw-  2.0 fat     5187 b- defN 23-Apr-10 17:20 tempor/utils/dataloaders/sine.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Apr-10 17:21 temporai-0.0.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    18024 b- defN 23-Apr-10 17:21 temporai-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 17:21 temporai-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-10 17:21 temporai-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat    11168 b- defN 23-Apr-10 17:21 temporai-0.0.1.dist-info/RECORD
-114 files, 548863 bytes uncompressed, 145461 bytes compressed:  73.5%
+Zip file size: 42991 bytes, number of entries: 46
+-rw-rw-rw-  2.0 fat      353 b- defN 23-Mar-10 19:44 hydra_plugins/tempor_searchpath_plugin.py
+-rw-rw-rw-  2.0 fat      578 b- defN 23-Mar-10 19:44 tempor/__init__.py
+-rw-rw-rw-  2.0 fat     4006 b- defN 23-Mar-10 19:44 tempor/config/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-10 19:44 tempor/config/conf/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-10 19:44 tempor/config/conf/tempor/__init__.py
+-rw-rw-rw-  2.0 fat      175 b- defN 23-Mar-10 19:44 tempor/config/conf/tempor/config.yaml
+-rw-rw-rw-  2.0 fat      166 b- defN 23-Mar-10 19:44 tempor/core/__init__.py
+-rw-rw-rw-  2.0 fat     4627 b- defN 23-Mar-10 19:44 tempor/core/_register_method_decorator.py
+-rw-rw-rw-  2.0 fat     1646 b- defN 23-Mar-10 19:44 tempor/core/_supports_impl.py
+-rw-rw-rw-  2.0 fat      598 b- defN 23-Mar-10 19:44 tempor/core/pydantic_utils.py
+-rw-rw-rw-  2.0 fat     1927 b- defN 23-Mar-10 19:44 tempor/core/requirements.py
+-rw-rw-rw-  2.0 fat       60 b- defN 23-Mar-10 19:44 tempor/core/supports_impl.py
+-rw-rw-rw-  2.0 fat      563 b- defN 23-Mar-10 19:44 tempor/core/utils.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-10 19:44 tempor/data/__init__.py
+-rw-rw-rw-  2.0 fat     1685 b- defN 23-Mar-10 19:44 tempor/data/data_typing.py
+-rw-rw-rw-  2.0 fat    13144 b- defN 23-Mar-10 19:44 tempor/data/dataset.py
+-rw-rw-rw-  2.0 fat    10620 b- defN 23-Mar-10 19:44 tempor/data/pandera_utils.py
+-rw-rw-rw-  2.0 fat     4316 b- defN 23-Mar-10 19:44 tempor/data/predictive.py
+-rw-rw-rw-  2.0 fat    26740 b- defN 23-Mar-10 19:44 tempor/data/samples.py
+-rw-rw-rw-  2.0 fat     1409 b- defN 23-Mar-10 19:44 tempor/data/settings.py
+-rw-rw-rw-  2.0 fat    12992 b- defN 23-Mar-10 19:44 tempor/data/utils.py
+-rw-rw-rw-  2.0 fat       54 b- defN 23-Mar-10 19:44 tempor/exc/__init__.py
+-rw-rw-rw-  2.0 fat       60 b- defN 23-Mar-10 19:44 tempor/log/__init__.py
+-rw-rw-rw-  2.0 fat     3232 b- defN 23-Mar-10 19:44 tempor/log/_custom_logger.py
+-rw-rw-rw-  2.0 fat      235 b- defN 23-Mar-10 19:44 tempor/log/_custom_logger.pyi
+-rw-rw-rw-  2.0 fat      644 b- defN 23-Mar-10 19:44 tempor/log/log_helpers.py
+-rw-rw-rw-  2.0 fat       83 b- defN 23-Mar-10 19:44 tempor/plugins/__init__.py
+-rw-rw-rw-  2.0 fat      154 b- defN 23-Mar-10 19:44 tempor/plugins/_plugin_loader.py
+-rw-rw-rw-  2.0 fat      461 b- defN 23-Mar-10 19:44 tempor/plugins/core/__init__.py
+-rw-rw-rw-  2.0 fat     3735 b- defN 23-Mar-10 19:44 tempor/plugins/core/_base_estimator.py
+-rw-rw-rw-  2.0 fat     1005 b- defN 23-Mar-10 19:44 tempor/plugins/core/_base_predictor.py
+-rw-rw-rw-  2.0 fat      988 b- defN 23-Mar-10 19:44 tempor/plugins/core/_base_transformer.py
+-rw-rw-rw-  2.0 fat      444 b- defN 23-Mar-10 19:44 tempor/plugins/core/_params.py
+-rw-rw-rw-  2.0 fat     6529 b- defN 23-Mar-10 19:44 tempor/plugins/core/_plugin.py
+-rw-rw-rw-  2.0 fat      174 b- defN 23-Mar-10 19:44 tempor/plugins/core/_types.py
+-rw-rw-rw-  2.0 fat     2059 b- defN 23-Mar-10 19:44 tempor/plugins/core/utils.py
+-rw-rw-rw-  2.0 fat       88 b- defN 23-Mar-10 19:44 tempor/plugins/preprocessing/__init__.py
+-rw-rw-rw-  2.0 fat      449 b- defN 23-Mar-10 19:44 tempor/plugins/preprocessing/imputation/__init__.py
+-rw-rw-rw-  2.0 fat      602 b- defN 23-Mar-10 19:44 tempor/plugins/preprocessing/imputation/plugin_nop.py
+-rw-rw-rw-  2.0 fat      443 b- defN 23-Mar-10 19:44 tempor/plugins/preprocessing/scaling/__init__.py
+-rw-rw-rw-  2.0 fat      591 b- defN 23-Mar-10 19:44 tempor/plugins/preprocessing/scaling/plugin_nop.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Mar-10 19:44 temporai-0.0.1.dev0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     9364 b- defN 23-Mar-10 19:44 temporai-0.0.1.dev0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-10 19:44 temporai-0.0.1.dev0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       21 b- defN 23-Mar-10 19:44 temporai-0.0.1.dev0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     3990 b- defN 23-Mar-10 19:44 temporai-0.0.1.dev0.dist-info/RECORD
+46 files, 132660 bytes uncompressed, 36559 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -1,61 +1,52 @@
 Filename: hydra_plugins/tempor_searchpath_plugin.py
 Comment: 
 
 Filename: tempor/__init__.py
 Comment: 
 
-Filename: tempor/benchmarks/__init__.py
-Comment: 
-
-Filename: tempor/benchmarks/benchmark.py
+Filename: tempor/config/__init__.py
 Comment: 
 
-Filename: tempor/benchmarks/evaluation.py
+Filename: tempor/config/conf/__init__.py
 Comment: 
 
-Filename: tempor/benchmarks/metrics.py
+Filename: tempor/config/conf/tempor/__init__.py
 Comment: 
 
-Filename: tempor/benchmarks/utils.py
+Filename: tempor/config/conf/tempor/config.yaml
 Comment: 
 
-Filename: tempor/config/__init__.py
+Filename: tempor/core/__init__.py
 Comment: 
 
-Filename: tempor/config/conf/__init__.py
+Filename: tempor/core/_register_method_decorator.py
 Comment: 
 
-Filename: tempor/config/conf/tempor/__init__.py
+Filename: tempor/core/_supports_impl.py
 Comment: 
 
-Filename: tempor/config/conf/tempor/config.yaml
+Filename: tempor/core/pydantic_utils.py
 Comment: 
 
-Filename: tempor/core/__init__.py
+Filename: tempor/core/requirements.py
 Comment: 
 
-Filename: tempor/core/pydantic_utils.py
+Filename: tempor/core/supports_impl.py
 Comment: 
 
 Filename: tempor/core/utils.py
 Comment: 
 
 Filename: tempor/data/__init__.py
 Comment: 
 
-Filename: tempor/data/clv2conv.py
-Comment: 
-
 Filename: tempor/data/data_typing.py
 Comment: 
 
-Filename: tempor/data/dataloader.py
-Comment: 
-
 Filename: tempor/data/dataset.py
 Comment: 
 
 Filename: tempor/data/pandera_utils.py
 Comment: 
 
 Filename: tempor/data/predictive.py
@@ -81,41 +72,14 @@
 
 Filename: tempor/log/_custom_logger.pyi
 Comment: 
 
 Filename: tempor/log/log_helpers.py
 Comment: 
 
-Filename: tempor/models/__init__.py
-Comment: 
-
-Filename: tempor/models/constants.py
-Comment: 
-
-Filename: tempor/models/ddh.py
-Comment: 
-
-Filename: tempor/models/mlp.py
-Comment: 
-
-Filename: tempor/models/samplers.py
-Comment: 
-
-Filename: tempor/models/transformer.py
-Comment: 
-
-Filename: tempor/models/ts_model.py
-Comment: 
-
-Filename: tempor/models/ts_ode.py
-Comment: 
-
-Filename: tempor/models/utils.py
-Comment: 
-
 Filename: tempor/plugins/__init__.py
 Comment: 
 
 Filename: tempor/plugins/_plugin_loader.py
 Comment: 
 
 Filename: tempor/plugins/core/__init__.py
@@ -138,206 +102,38 @@
 
 Filename: tempor/plugins/core/_types.py
 Comment: 
 
 Filename: tempor/plugins/core/utils.py
 Comment: 
 
-Filename: tempor/plugins/pipeline/__init__.py
-Comment: 
-
-Filename: tempor/plugins/pipeline/generators.py
-Comment: 
-
-Filename: tempor/plugins/prediction/__init__.py
-Comment: 
-
-Filename: tempor/plugins/prediction/one_off/__init__.py
-Comment: 
-
-Filename: tempor/plugins/prediction/one_off/classification/__init__.py
-Comment: 
-
-Filename: tempor/plugins/prediction/one_off/classification/plugin_cde_classifier.py
-Comment: 
-
-Filename: tempor/plugins/prediction/one_off/classification/plugin_laplace_classifier.py
-Comment: 
-
-Filename: tempor/plugins/prediction/one_off/classification/plugin_nn_classifier.py
-Comment: 
-
-Filename: tempor/plugins/prediction/one_off/classification/plugin_ode_classifier.py
-Comment: 
-
-Filename: tempor/plugins/prediction/one_off/regression/__init__.py
-Comment: 
-
-Filename: tempor/plugins/prediction/one_off/regression/plugin_cde_regressor.py
-Comment: 
-
-Filename: tempor/plugins/prediction/one_off/regression/plugin_laplace_regressor.py
-Comment: 
-
-Filename: tempor/plugins/prediction/one_off/regression/plugin_nn_regressor.py
-Comment: 
-
-Filename: tempor/plugins/prediction/one_off/regression/plugin_ode_regressor.py
-Comment: 
-
-Filename: tempor/plugins/prediction/temporal/__init__.py
-Comment: 
-
-Filename: tempor/plugins/prediction/temporal/classification/__init__.py
-Comment: 
-
-Filename: tempor/plugins/prediction/temporal/classification/plugin_seq2seq_classifier.py
-Comment: 
-
-Filename: tempor/plugins/prediction/temporal/regression/__init__.py
-Comment: 
-
-Filename: tempor/plugins/prediction/temporal/regression/plugin_seq2seq_regressor.py
-Comment: 
-
 Filename: tempor/plugins/preprocessing/__init__.py
 Comment: 
 
 Filename: tempor/plugins/preprocessing/imputation/__init__.py
 Comment: 
 
-Filename: tempor/plugins/preprocessing/imputation/_base.py
-Comment: 
-
-Filename: tempor/plugins/preprocessing/imputation/static/__init__.py
-Comment: 
-
-Filename: tempor/plugins/preprocessing/imputation/static/plugin_static_imputation.py
-Comment: 
-
-Filename: tempor/plugins/preprocessing/imputation/temporal/__init__.py
-Comment: 
-
-Filename: tempor/plugins/preprocessing/imputation/temporal/plugin_bfill.py
-Comment: 
-
-Filename: tempor/plugins/preprocessing/imputation/temporal/plugin_ffill.py
-Comment: 
-
-Filename: tempor/plugins/preprocessing/nop/__init__.py
+Filename: tempor/plugins/preprocessing/imputation/plugin_nop.py
 Comment: 
 
 Filename: tempor/plugins/preprocessing/scaling/__init__.py
 Comment: 
 
-Filename: tempor/plugins/preprocessing/scaling/_base.py
-Comment: 
-
-Filename: tempor/plugins/preprocessing/scaling/static/__init__.py
-Comment: 
-
-Filename: tempor/plugins/preprocessing/scaling/static/plugin_static_minmax_scaler.py
-Comment: 
-
-Filename: tempor/plugins/preprocessing/scaling/static/plugin_static_standard_scaler.py
-Comment: 
-
-Filename: tempor/plugins/preprocessing/scaling/temporal/__init__.py
-Comment: 
-
-Filename: tempor/plugins/preprocessing/scaling/temporal/plugin_ts_minmax_scaler.py
-Comment: 
-
-Filename: tempor/plugins/preprocessing/scaling/temporal/plugin_ts_standard_scaler.py
-Comment: 
-
-Filename: tempor/plugins/time_to_event/__init__.py
-Comment: 
-
-Filename: tempor/plugins/time_to_event/helper_embedding.py
-Comment: 
-
-Filename: tempor/plugins/time_to_event/plugin_ddh.py
-Comment: 
-
-Filename: tempor/plugins/time_to_event/plugin_ts_coxph.py
-Comment: 
-
-Filename: tempor/plugins/time_to_event/plugin_ts_xgb.py
-Comment: 
-
-Filename: tempor/plugins/treatments/__init__.py
-Comment: 
-
-Filename: tempor/plugins/treatments/one_off/__init__.py
-Comment: 
-
-Filename: tempor/plugins/treatments/one_off/_base.py
-Comment: 
-
-Filename: tempor/plugins/treatments/one_off/classification/__init__.py
-Comment: 
-
-Filename: tempor/plugins/treatments/one_off/regression/__init__.py
-Comment: 
-
-Filename: tempor/plugins/treatments/one_off/regression/plugin_synctwin_regressor.py
-Comment: 
-
-Filename: tempor/plugins/treatments/temporal/__init__.py
-Comment: 
-
-Filename: tempor/plugins/treatments/temporal/_base.py
-Comment: 
-
-Filename: tempor/plugins/treatments/temporal/classification/__init__.py
-Comment: 
-
-Filename: tempor/plugins/treatments/temporal/classification/plugin_crn_classifier.py
-Comment: 
-
-Filename: tempor/plugins/treatments/temporal/regression/__init__.py
-Comment: 
-
-Filename: tempor/plugins/treatments/temporal/regression/plugin_crn_regressor.py
-Comment: 
-
-Filename: tempor/utils/__init__.py
-Comment: 
-
-Filename: tempor/utils/serialization.py
-Comment: 
-
-Filename: tempor/utils/dataloaders/__init__.py
-Comment: 
-
-Filename: tempor/utils/dataloaders/dummy.py
-Comment: 
-
-Filename: tempor/utils/dataloaders/google_stocks.py
-Comment: 
-
-Filename: tempor/utils/dataloaders/pbc.py
-Comment: 
-
-Filename: tempor/utils/dataloaders/pkpd.py
-Comment: 
-
-Filename: tempor/utils/dataloaders/sine.py
+Filename: tempor/plugins/preprocessing/scaling/plugin_nop.py
 Comment: 
 
-Filename: temporai-0.0.1.dist-info/LICENSE.txt
+Filename: temporai-0.0.1.dev0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: temporai-0.0.1.dist-info/METADATA
+Filename: temporai-0.0.1.dev0.dist-info/METADATA
 Comment: 
 
-Filename: temporai-0.0.1.dist-info/WHEEL
+Filename: temporai-0.0.1.dev0.dist-info/WHEEL
 Comment: 
 
-Filename: temporai-0.0.1.dist-info/top_level.txt
+Filename: temporai-0.0.1.dev0.dist-info/top_level.txt
 Comment: 
 
-Filename: temporai-0.0.1.dist-info/RECORD
+Filename: temporai-0.0.1.dev0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tempor/__init__.py

```diff
@@ -1,13 +1,8 @@
-import sys
-
-if sys.version_info[:2] >= (3, 8):  # pragma: no cover
-    from importlib.metadata import PackageNotFoundError, version
-else:  # pragma: no cover
-    from importlib_metadata import PackageNotFoundError, version
+from importlib.metadata import PackageNotFoundError, version  # pragma: no cover
 
 try:
     # Change here if project is renamed and does not equal the package name
     import_name = "tempor"
     dist_name = "temporai"
     __version__ = version(dist_name)
 except PackageNotFoundError:  # pragma: no cover
```

## tempor/config/__init__.py

```diff
@@ -5,16 +5,14 @@
 import sys
 from typing import TYPE_CHECKING, Callable, Set, Union
 
 import hydra.core.config_store
 import omegaconf
 from omegaconf import OmegaConf
 
-import tempor
-
 # NOTE: This config module is loaded before everything else, as other modules may use the config.
 
 DEFAULT_CONFIG_DIR = "conf/tempor"
 DEFAULT_CONFIG_FILE_NAME = "config"
 DEFAULT_CONFIG_FILE_PATH = os.path.join(
     os.path.dirname(__file__),
     f"{DEFAULT_CONFIG_DIR}/{DEFAULT_CONFIG_FILE_NAME}.yaml",
@@ -42,33 +40,33 @@
 
 @dataclasses.dataclass
 class TemporConfig:
     logging: LoggingConfig
     working_directory: str = omegaconf.MISSING
 
     def get_working_dir(self):
-        if self.working_directory.startswith("$PWD"):
-            return self.working_directory.replace("$PWD", os.getcwd(), 1)
-        elif self.working_directory.startswith("~"):
-            return self.working_directory.replace("~", os.path.expanduser("~"), 1)
+        if self.working_directory == "$PWD":
+            return os.getcwd()
+        elif self.working_directory == "~":
+            return os.path.expanduser("~")
         else:
             return self.working_directory
 
 
 # --- Config structure: end. ---
 
 # Minimal observer-pattern like setup to trigger relevant changes when configure() is called.
 # To "subscribe":
 # from tempor.configuration import updated_on_configure
 # updated_on_configure.add(my_method)
 updated_on_configure: Set[Callable[[TemporConfig], None]] = set()
 
 # Register dataclass with Hydra config store for Hydra type checking.
 _cs = hydra.core.config_store.ConfigStore.instance()
-_cs.store(name=tempor.import_name, node=TemporConfig)
+_cs.store(name="tempor", node=TemporConfig)
 
 # Initialize OmegaConf schema.
 _tempor_config_schema = OmegaConf.structured(TemporConfig)
 
 
 _this_module = sys.modules[__name__]  # Needed to directly set `config` on this module in the configure() function.
```

## tempor/core/__init__.py

```diff
@@ -0,0 +1,11 @@
+00000000: 6672 6f6d 202e 2069 6d70 6f72 7420 7375  from . import su
+00000010: 7070 6f72 7473 5f69 6d70 6c0d 0a66 726f  pports_impl..fro
+00000020: 6d20 2e5f 7265 6769 7374 6572 5f6d 6574  m ._register_met
+00000030: 686f 645f 6465 636f 7261 746f 7220 696d  hod_decorator im
+00000040: 706f 7274 2052 6567 6973 7465 724d 6574  port RegisterMet
+00000050: 686f 6444 6563 6f72 6174 6f72 0d0a 0d0a  hodDecorator....
+00000060: 5f5f 616c 6c5f 5f20 3d20 5b0d 0a20 2020  __all__ = [..   
+00000070: 2022 5265 6769 7374 6572 4d65 7468 6f64   "RegisterMethod
+00000080: 4465 636f 7261 746f 7222 2c0d 0a20 2020  Decorator",..   
+00000090: 2022 7375 7070 6f72 7473 5f69 6d70 6c22   "supports_impl"
+000000a0: 2c0d 0a5d 0d0a                           ,..]..
```

## tempor/core/pydantic_utils.py

```diff
@@ -1,10 +1,8 @@
-from typing import Any, Dict, Optional, Type
-
-import pydantic
+from typing import Dict, Optional
 
 
 def exclusive_args(
     values: Dict,
     arg1: str,
     arg2: str,
     arg1_friendly_name: Optional[str] = None,
@@ -12,51 +10,7 @@
 ) -> None:
     arg1_value = values.get(arg1, None)
     arg2_value = values.get(arg2, None)
     arg1_name = arg1_friendly_name if arg1_friendly_name else f"`{arg1}`"
     arg2_name = arg2_friendly_name if arg2_friendly_name else f"`{arg2}`"
     if arg1_value is not None and arg2_value is not None:
         raise ValueError(f"Must provide either {arg1_name} or {arg2_name} but not both")
-
-
-def is_pydantic_dataclass(cls: Type) -> bool:
-    return hasattr(cls, "__dataclass__")
-
-
-PYDANTIC_DATACLASS_WORKAROUND_DICT = dict()
-
-
-def make_pydantic_dataclass(builtin_dataclass: Type) -> Type:
-    """Workaround for a `pydantic` edge case issue when calling ``pydantic.dataclass(<builtin_dataclass>)``
-    more than once where ``builtin_dataclass`` has a default factory filed after a keyword parameter.
-
-    E.g. the following would normally fail, this works around the issue.
-
-    .. code-block:: python
-
-        from typing import List
-        import dataclasses
-        import pydantic
-
-
-        @dataclasses.dataclass
-        class MyDataclass:
-            a: str = "string"
-            b: List[int] = dataclasses.field(default_factory=lambda: [1, 2, 3])
-
-
-        pydantic.dataclasses.dataclass(MyDataclass)  # OK.
-        pydantic.dataclasses.dataclass(MyDataclass)  # TypeError.
-
-    Args:
-        builtin_dataclass (Type): Python builtin dataclass.
-
-    Returns:
-        Type: ``builtin_dataclass`` safely converted to pydantic dataclass.
-    """
-    name = f"{builtin_dataclass.__module__}.{builtin_dataclass.__name__}"
-    if name not in PYDANTIC_DATACLASS_WORKAROUND_DICT:
-        pydantic_dataclass: Any = pydantic.dataclasses.dataclass(builtin_dataclass)
-        PYDANTIC_DATACLASS_WORKAROUND_DICT[name] = pydantic_dataclass
-    else:
-        pydantic_dataclass = PYDANTIC_DATACLASS_WORKAROUND_DICT[name]
-    return pydantic_dataclass
```

## tempor/core/utils.py

```diff
@@ -1,11 +1,8 @@
 import enum
-from typing import Any, Dict, Tuple
-
-from typing_extensions import get_args
 
 
 def get_class_full_name(o: object):
     # See: https://stackoverflow.com/a/2020083
     class_ = o.__class__
     module = class_.__module__
     if module == "builtins":
@@ -19,56 +16,7 @@
 
 class RichReprStrPassthrough:
     def __init__(self, string: str) -> None:
         self.string = string
 
     def __repr__(self) -> str:
         return self.string
-
-
-def is_iterable(o: object) -> bool:
-    is_iterable_ = True
-    try:
-        iter(o)  # type: ignore[call-overload]
-    except TypeError:
-        is_iterable_ = False
-    return is_iterable_
-
-
-def get_version(version: str) -> Tuple[int, ...]:
-    """Get the semantic ``version`` as a tuple of ``int`` s.
-
-    Note:
-        Assumes that the ``version`` string is specified as ``.``-separated ``ints``; will throw exceptions in
-        case of more complex version semantics.
-
-    Args:
-        module (ModuleType): The module to get the version of.
-
-    Returns:
-        Tuple[int, ...]: Tuple of integers representing ``(major, minor, patch[, ...])``.
-    """
-    return tuple(int(v) for v in version.split("."))
-
-
-def version_above_incl(version: Tuple[int, int], above_incl: Tuple[int, int]) -> bool:
-    v_major, v_minor = version
-    compare_major, compare_minor = above_incl
-    return (v_major == compare_major and v_minor >= compare_minor) or v_major > compare_major
-
-
-def version_below_excl(version: Tuple[int, int], below_excl: Tuple[int, int]) -> bool:
-    v_major, v_minor = version
-    compare_major, compare_minor = below_excl
-    return (v_major == compare_major and v_minor < compare_minor) or v_major < compare_major
-
-
-def ensure_literal_matches_dict_keys(
-    literal: Any, d: Dict[str, Any], literal_name: str = "literal", dict_name: str = "dictionary"
-):
-    lits = set(get_args(literal))
-    keys = set(d.keys())
-    if lits != keys:
-        raise TypeError(
-            f"There was a mismatch between the literal '{literal_name}' and the the dictionary "
-            f"'{dict_name}' keys: {list(lits.symmetric_difference(keys))}"
-        )
```

## tempor/data/data_typing.py

```diff
@@ -1,21 +1,21 @@
-"""Types (and related code) for TemporAI data handling."""
+"""Types (and related code) for TemporAI data handling.
+"""
 
 import enum
-from typing import Dict, Iterable, List, Tuple, Type, Union
+from typing import Dict, List, Literal, Tuple, Type, Union
 
 import numpy as np
 import pandas as pd
-from typing_extensions import Literal
 
 DataContainer = Union[pd.DataFrame, np.ndarray]
 
 Dtype = Union[Type, Literal["category", "datetime"]]
 """Type annotation to indicate dtypes. May be `Type`, e.g. `str`, `bool`, or one of the literals:
-``"category"``, ``"datetime"``.
+`"category"`, `"datetime"`
 """
 
 
 class DataModality(enum.Enum):
     STATIC = enum.auto()
     TIME_SERIES = enum.auto()
     EVENT = enum.auto()
@@ -37,36 +37,25 @@
     List[int],
     List[pd.Timestamp],
 ]
 SampleToTimeIndexDict = Union[
     Dict[int, TimeIndex],
     Dict[str, TimeIndex],
 ]
-SampleToNumTimestepsDict = Union[
-    Dict[int, int],
-    Dict[str, int],
-]
 SampleTimeIndexTuples = List[
     Union[
         Tuple[int, float],
         Tuple[int, int],
         Tuple[int, pd.Timestamp],
         Tuple[str, float],
         Tuple[str, int],
         Tuple[str, pd.Timestamp],
     ]
 ]
-TimeIndexList = Union[
-    List[List[float]],
-    List[List[int]],
-    List[List[pd.Timestamp]],
-]
-
-
-GetItemKey = Union[int, Iterable[int], slice]
+TimeIndexList = List[TimeIndex]
 
 
 class PredictiveTask(enum.Enum):
     ONE_OFF_PREDICTION = enum.auto()
     TEMPORAL_PREDICTION = enum.auto()
     TIME_TO_EVENT_ANALYSIS = enum.auto()
     ONE_OFF_TREATMENT_EFFECTS = enum.auto()
```

## tempor/data/dataset.py

```diff
@@ -1,124 +1,100 @@
 # pylint: disable=unnecessary-ellipsis
 
 import abc
 import dataclasses
-from typing import Any, ClassVar, Generator, Optional, Tuple, Union
+from typing import ClassVar, Optional, Union
 
 import rich.pretty
-import sklearn.model_selection
-from typing_extensions import Self
 
 from tempor.core.utils import RichReprStrPassthrough
-from tempor.log import log_helpers, logger
+from tempor.log import log_helpers
 
 from . import data_typing
 from . import predictive as pred
-from . import samples, utils
-
-# NOTE: Can probably add other splitters:
-Splitter = Union[
-    sklearn.model_selection.KFold,
-    sklearn.model_selection.StratifiedKFold,
-]
+from . import samples
 
 
 @dataclasses.dataclass(frozen=True)
 class _SampleIndexMismatchMsg:
-    static: ClassVar[str] = (
-        "`sample_index` of static samples did not match `sample_index` of time series samples. "
-        "Note that the samples need to be in the same order."
-    )
-    targets: ClassVar[str] = (
-        "`sample_index` of targets did not match `sample_index` of time series samples. "
-        "Note that the samples need to be in the same order."
-    )
-    treatments: ClassVar[str] = (
-        "`sample_index` of treatments did not match `sample_index` of time series samples. "
-        "Note that the samples need to be in the same order."
-    )
-
-
-@dataclasses.dataclass(frozen=True)
-class _TimeIndexesMismatchMsg:
-    targets: ClassVar[str] = "`time_indexes` of targets did not match `time_indexes` of time series covariates."
-    treatments: ClassVar[str] = "`time_indexes` of treatments did not match `time_indexes` of time series covariates."
+    static: ClassVar[str] = "`sample_index` of static samples did not match `sample_index` of time series samples"
+    targets: ClassVar[str] = "`sample_index` of targets did not match `sample_index` of time series samples"
+    treatments: ClassVar[str] = "`sample_index` of treatments did not match `sample_index` of time series samples"
 
 
 @dataclasses.dataclass(frozen=True)
 class _ExceptionMessages:
     sample_index_mismatch: ClassVar[_SampleIndexMismatchMsg] = _SampleIndexMismatchMsg()
-    time_indexes_mismatch: ClassVar[_TimeIndexesMismatchMsg] = _TimeIndexesMismatchMsg()
 
 
 EXCEPTION_MESSAGES = _ExceptionMessages()
 """Reusable error messages for the module."""
 
 
-class BaseDataset(abc.ABC):
-    _time_series: samples.TimeSeriesSamples
-    _static: Optional[samples.StaticSamples]
+class Dataset(abc.ABC):
+    time_series: samples.TimeSeriesSamples
+    static: Optional[samples.StaticSamples]
     predictive: Optional[pred.PredictiveTaskData]
 
     def __init__(
         self,
         time_series: data_typing.DataContainer,
         *,
         static: Optional[data_typing.DataContainer] = None,
         targets: Optional[data_typing.DataContainer] = None,
         treatments: Optional[data_typing.DataContainer] = None,
         **kwargs,  # pylint: disable=unused-argument
     ) -> None:
-        """Abstract base class representing a dataset used by TemporAI.
+        """Base class representing a dataset used by TemporAI.
 
-        Initialize one of its derived classes (e.g. :class:`OneOffPredictionDataset`,
-        :class:`TimeToEventAnalysisDataset` etc.) depending on the type of task.
+        Initialize one of its derived classes (e.g. `OneOffPredictionDataset`, `TimeToEventAnalysisDataset` etc.)
+        depending on the type of task.
 
-        See also tutorial ``tutorials/tutorial01_data_format.ipynb`` for examples of use.
+        See also tutorial `tutorials/tutorial01_data_format.ipynb` for examples of use.
 
         Args:
-            time_series (numpy.ndarray | pandas.DataFrame):
-                Data representing time series covariates of the samples. Will be initialized as `TimeSeriesSamples`.
-            static (numpy.ndarray | pandas.DataFrame, optional):
-                Data representing static covariates of the samples. Will be initialized as `StaticSamples`.
-                Defaults to `None`.
-            targets (numpy.ndarray | pandas.DataFrame, optional):
-                Data representing target (outcome) feature(s) of the samples. Will be initialized as
-                ``{TimeSeries,Static,Event}Samples`` depending on problem setting in the derived class.
-                Defaults to `None`.
-            treatments (numpy.ndarray | pandas.DataFrame, optional):
-                Data representing treatment (intervention) feature(s) of the samples. Will be initialized as
-                ``{TimeSeries,Static,Event}Samples`` depending on problem setting in the derived class.
-                Defaults to `None`.
+            time_series (numpy.ndarray | pandas.DataFrame): Data representing time series covariates of the samples.
+            Will be initialized as `TimeSeriesSamples`.
+            static (numpy.ndarray | pandas.DataFrame, optional): Data representing static covariates of the samples.
+            Will be initialized as `StaticSamples`. Defaults to None.
+            targets (numpy.ndarray | pandas.DataFrame, optional): Data representing target (outcome) feature(s) of the
+            samples. Will be initialized as `{TimeSeries,Static,Event}Samples` depending on problem setting in the
+            derived class. Defaults to None.
+            treatments (numpy.ndarray | pandas.DataFrame, optional): Data representing treatment (intervention)
+            feature(s) of the samples. Will be initialized as `{TimeSeries,Static,Event}Samples` depending on problem
+            setting in the derived class. Defaults to None.
         """
-        self._time_series = samples.TimeSeriesSamples(time_series)
-        self._static = samples.StaticSamples(static) if static is not None else None
+        self.time_series = samples.TimeSeriesSamples(time_series)
+        self.static = samples.StaticSamples(static) if static is not None else None
 
-        self._init_predictive(targets=targets, treatments=treatments, **kwargs)
+        if targets is not None:
+            self._init_predictive(targets=targets, treatments=treatments, **kwargs)
+        else:
+            self.predictive = None
 
         self.validate()
 
     def __rich_repr__(self):
         yield "time_series", RichReprStrPassthrough(self.time_series.short_repr())
         if self.static is not None:
             yield "static", RichReprStrPassthrough(self.static.short_repr())
         if self.predictive is not None:
-            yield "predictive", self.predictive
+            yield "static", self.predictive
 
     def __repr__(self) -> str:
         return rich.pretty.pretty_repr(self)
 
     @abc.abstractmethod
     def _init_predictive(
         self,
-        targets: Optional[data_typing.DataContainer],
-        treatments: Optional[data_typing.DataContainer],
+        targets: data_typing.DataContainer,
+        treatments: Optional[data_typing.DataContainer] = None,
         **kwargs,
     ) -> None:  # pragma: no cover
-        """A method to initialize ``self.predictive`` in derived classes."""
+        """A method to initialize `self.predictive` in derived classes."""
         ...
 
     @property
     def has_static(self) -> bool:
         return self.static is not None
 
     @property
@@ -140,426 +116,192 @@
                     raise ValueError(EXCEPTION_MESSAGES.sample_index_mismatch.static)
             self._validate()
 
     @abc.abstractmethod
     def _validate(self) -> None:  # pragma: no cover
         ...
 
-    @property
-    def time_series(self) -> samples.TimeSeriesSamples:
-        return self._time_series
-
-    @time_series.setter
-    def time_series(self, value: samples.TimeSeriesSamples) -> None:
-        self._time_series = value
-        self.validate()
-
-    @property
-    def static(self) -> Optional[samples.StaticSamples]:
-        return self._static
-
-    @static.setter
-    def static(self, value: Optional[samples.StaticSamples]) -> None:
-        self._static = value
-        self.validate()
-
-    @property
-    @abc.abstractmethod
-    def fit_ready(self) -> bool:  # pragma: no cover
-        """Returns whether the :class:`BaseDataset` is in a state ready to be ``fit`` on."""
-        ...
-
-    def __len__(self) -> int:
-        return self.time_series.num_samples
-
-    def __getitem__(self, key: data_typing.GetItemKey) -> Self:
-        key_ = utils.ensure_pd_iloc_key_returns_df(key)
-        new_dataset = self.__class__(
-            time_series=self.time_series[key_].dataframe(),  # pyright: ignore
-            static=self.static[key_].dataframe() if self.has_static else None,  # type: ignore[union-attr,index]
-            targets=(
-                self.predictive.targets[key_].dataframe()  # type: ignore[union-attr]
-                if (self.has_predictive_data and self.predictive.targets is not None)  # type: ignore[union-attr]
-                else None
-            ),
-            treatments=(
-                self.predictive.treatments[key_].dataframe()  # type: ignore[union-attr]
-                if (self.has_predictive_data and self.predictive.treatments is not None)  # type: ignore[union-attr]
-                else None
-            ),
-        )
-        return new_dataset
-
-    def train_test_split(
-        self,
-        *,
-        test_size=None,
-        train_size=None,
-        random_state=None,
-        shuffle=True,
-        stratify=None,
-    ) -> Tuple[Self, Self]:
-        """Split `Dataset` into train and test sets.
-
-        The arguments ``test_size`` ... ``stratify`` are passed to `sklearn.model_selection.train_test_split` to
-        generate the split.
-
-        Returns:
-            Tuple[Self, Self]: The split tuple ``(dataset_train, dataset_test)``.
-        """
-        sample_ilocs = list(range(len(self)))
-        sample_ilocs_train, sample_ilocs_test = sklearn.model_selection.train_test_split(
-            sample_ilocs,
-            test_size=test_size,
-            train_size=train_size,
-            random_state=random_state,
-            shuffle=shuffle,
-            stratify=stratify,
-        )
-        return self[sample_ilocs_train], self[sample_ilocs_test]
-
-    def split(
-        self,
-        splitter: Splitter,
-        **kwargs,
-    ) -> Generator[Tuple[Self, Self], None, None]:
-        """Generate dataset splits according to the scikit-learn ``splitter`` (`~tempor.data.dataset.Splitter`).
-        The ``kwargs`` are passed to the underlying splitter's ``split`` method.
-
-        Example:
-            >>> from sklearn.model_selection import KFold
-            >>> from tempor.utils.dataloaders import SineDataLoader
-            >>> data = SineDataLoader().load()
-            >>> kfold = KFold(n_splits=5)
-            >>> len([(data_train, data_test) for (data_train, data_test) in data.split(splitter=kfold)])
-            5
-
-        Args:
-            splitter (Splitter): A `sklearn` splitter.
-
-        Yields:
-            Generator[Tuple[Self, Self], None, None]: ``(dataset_train, dataset_test)`` for each split.
-        """
-        sample_ilocs: Any = list(range(len(self)))
-        for sample_ilocs_train, sample_ilocs_test in splitter.split(X=sample_ilocs, **kwargs):
-            yield self[sample_ilocs_train], self[sample_ilocs_test]
-
 
 # `Dataset`s corresponding to different tasks follow. More can be added to handle new Tasks.
 
-# TODO: unit test CovariatesDataset.
-class CovariatesDataset(BaseDataset):
-    def __init__(
-        self,
-        time_series: data_typing.DataContainer,
-        *,
-        static: Optional[data_typing.DataContainer] = None,
-        targets: Optional[data_typing.DataContainer] = None,
-        treatments: Optional[data_typing.DataContainer] = None,
-        **kwargs,
-    ) -> None:
-        """A :class:`BaseDataset` subclass for a dataset that does not contain any predictive data
-        (``targets`` or ``treatments``).
-        """
-        super().__init__(time_series=time_series, static=static, targets=targets, treatments=treatments, **kwargs)
-
-    def _init_predictive(
-        self,
-        targets: Optional[data_typing.DataContainer],
-        treatments: Optional[data_typing.DataContainer],
-        **kwargs,
-    ) -> None:
-        if targets is not None:
-            raise ValueError(f"`targets` must not be set for a {self.__class__.__name__}.")
-        if treatments is not None:
-            raise ValueError(f"`treatments` must not be set for a {self.__class__.__name__}.")
-        self.predictive = None
-
-    def _validate(self) -> None:
-        # No additional checks needed.
-        pass
-
-    @property
-    def fit_ready(self) -> bool:
-        return True
-
-
-class PredictiveDataset(BaseDataset):
-    predictive: pred.PredictiveTaskData
-
-    def __init__(
-        self,
-        time_series: data_typing.DataContainer,
-        *,
-        targets: Optional[data_typing.DataContainer],
-        static: Optional[data_typing.DataContainer] = None,
-        treatments: Optional[data_typing.DataContainer] = None,
-        **kwargs,
-    ) -> None:
-        """A :class:`BaseDataset` subclass for a dataset that can contain predictive data
-        (``targets`` or ``treatments``).
-
-        This is an abstract class, to be derived from for different predictive task -specific ``Dataset`` s.
-        """
-        super().__init__(time_series=time_series, static=static, targets=targets, treatments=treatments, **kwargs)
-
-    @property
-    @abc.abstractmethod
-    def predict_ready(self) -> bool:  # pragma: no cover
-        """Returns whether the :class:`PredictiveDataset` is in a state ready to be ``predict`` ed on."""
-        ...
-
 
-class OneOffPredictionDataset(PredictiveDataset):
+class OneOffPredictionDataset(Dataset):
     predictive: pred.OneOffPredictionTaskData
 
-    def __init__(
+    def __init__(  # pylint: disable=useless-super-delegation
         self,
         time_series: data_typing.DataContainer,
         *,
-        targets: Optional[data_typing.DataContainer],
+        targets: data_typing.DataContainer,
         static: Optional[data_typing.DataContainer] = None,
         treatments: Optional[data_typing.DataContainer] = None,
         **kwargs,
     ) -> None:
-        """A :class:`PredictiveDataset` subclass for the one-off prediction problem setting,
-        see :class:`BaseDataset` docs.
+        """A `Dataset` subclass for the one-off prediction problem setting, see `Dataset` docs.
 
-        In this setting: ``targets`` are required for fitting, will be initialized as `StaticSamples`.
+        In this setting: `targets` are required, will be initialized as `StaticSamples`.
         """
         super().__init__(time_series=time_series, static=static, targets=targets, treatments=treatments, **kwargs)
 
     def _init_predictive(
         self,
-        targets: Optional[data_typing.DataContainer],
-        treatments: Optional[data_typing.DataContainer],
+        targets: data_typing.DataContainer,
+        treatments: Optional[data_typing.DataContainer] = None,
         **kwargs,
     ) -> None:
         if targets is None:
-            logger.debug(
-                f"`targets` provided was None for {self.__class__.__name__}, "
-                "this Dataset can only be used for prediction not fitting"
-            )
-        self.predictive = pred.OneOffPredictionTaskData(parent_dataset=self, targets=targets, **kwargs)
+            raise ValueError("One-off prediction task requires `targets`")
+        self.predictive = pred.OneOffPredictionTaskData(targets=targets, **kwargs)
 
     def _validate(self) -> None:
-        if self.predictive.targets is not None:
-            if self.predictive.targets.sample_index() != self.time_series.sample_index():
-                raise ValueError(EXCEPTION_MESSAGES.sample_index_mismatch.targets)
-
-    @property
-    def fit_ready(self) -> bool:
-        return self.predictive.targets is not None
-
-    @property
-    def predict_ready(self) -> bool:
-        return True
+        if self.predictive.targets.sample_index() != self.time_series.sample_index():
+            raise ValueError(EXCEPTION_MESSAGES.sample_index_mismatch.targets)
 
 
-class TemporalPredictionDataset(PredictiveDataset):
+class TemporalPredictionDataset(Dataset):
     predictive: pred.TemporalPredictionTaskData
 
-    def __init__(
+    def __init__(  # pylint: disable=useless-super-delegation
         self,
         time_series: data_typing.DataContainer,
         *,
-        targets: Optional[data_typing.DataContainer],
+        targets: data_typing.DataContainer,
         static: Optional[data_typing.DataContainer] = None,
         treatments: Optional[data_typing.DataContainer] = None,
         **kwargs,
     ) -> None:
-        """A :class:`PredictiveDataset` subclass for the temporal prediction problem setting,
-        see :class:`BaseDataset` docs.
+        """A `Dataset` subclass for the temporal prediction problem setting, see `Dataset` docs.
 
-        In this setting: ``targets`` are required for fitting, will be initialized as `TimeSeriesSamples`.
+        In this setting: `targets` are required, will be initialized as `TimeSeriesSamples`.
         """
         super().__init__(time_series=time_series, static=static, targets=targets, treatments=treatments, **kwargs)
 
     def _init_predictive(
         self,
-        targets: Optional[data_typing.DataContainer],
-        treatments: Optional[data_typing.DataContainer],
+        targets: data_typing.DataContainer,
+        treatments: Optional[data_typing.DataContainer] = None,
         **kwargs,
     ) -> None:
         if targets is None:
-            logger.debug(
-                f"`targets` provided was None for {self.__class__.__name__}, "
-                "this Dataset can only be used for prediction not fitting"
-            )
-        self.predictive = pred.TemporalPredictionTaskData(parent_dataset=self, targets=targets, **kwargs)
+            raise ValueError("Temporal prediction task requires `targets`")
+        self.predictive = pred.TemporalPredictionTaskData(targets=targets, **kwargs)
 
     def _validate(self) -> None:
-        if self.predictive.targets is not None:
-            if self.predictive.targets.sample_index() != self.time_series.sample_index():
-                raise ValueError(EXCEPTION_MESSAGES.sample_index_mismatch.targets)
-            if self.predictive.targets.time_indexes() != self.time_series.time_indexes():
-                raise ValueError(EXCEPTION_MESSAGES.time_indexes_mismatch.targets)
+        print(self.predictive.targets.sample_index())
+        if self.predictive.targets.sample_index() != self.time_series.sample_index():
+            raise ValueError(EXCEPTION_MESSAGES.sample_index_mismatch.targets)
+        # TODO: Possible check - check that .time_series and .predictive.targets have the same time_indexes.
 
-    @property
-    def fit_ready(self) -> bool:
-        return self.predictive.targets is not None
 
-    @property
-    def predict_ready(self) -> bool:
-        return True
-
-
-class TimeToEventAnalysisDataset(PredictiveDataset):
+class TimeToEventAnalysisDataset(Dataset):
     predictive: pred.TimeToEventAnalysisTaskData
 
-    def __init__(
+    def __init__(  # pylint: disable=useless-super-delegation
         self,
         time_series: data_typing.DataContainer,
         *,
-        targets: Optional[data_typing.DataContainer],
+        targets: data_typing.DataContainer,
         static: Optional[data_typing.DataContainer] = None,
         treatments: Optional[data_typing.DataContainer] = None,
         **kwargs,
     ) -> None:
-        """A :class:`PredictiveDataset` subclass for the time-to-event analysis problem setting,
-        see :class:`BaseDataset` docs.
+        """A `Dataset` subclass for the time-to-event analysis problem setting, see `Dataset` docs.
 
-        In this setting: ``targets`` are required for fitting, will be initialized as `EventSamples`.
+        In this setting: `targets` are required, will be initialized as `EventSamples`.
         """
         super().__init__(time_series=time_series, static=static, targets=targets, treatments=treatments, **kwargs)
 
-    def _init_predictive(
+    def _init_predictive(  # pylint: disable=useless-super-delegation
         self,
-        targets: Optional[data_typing.DataContainer],
-        treatments: Optional[data_typing.DataContainer],
+        targets: data_typing.DataContainer,
+        treatments: Optional[data_typing.DataContainer] = None,
         **kwargs,
     ) -> None:
         if targets is None:
-            logger.debug(
-                f"`targets` provided was None for {self.__class__.__name__}, "
-                "this Dataset can only be used for prediction not fitting"
-            )
-        self.predictive = pred.TimeToEventAnalysisTaskData(parent_dataset=self, targets=targets, **kwargs)
+            raise ValueError("Time-to-event analysis task requires `targets`")
+        self.predictive = pred.TimeToEventAnalysisTaskData(targets=targets, **kwargs)
 
     def _validate(self) -> None:
-        if self.predictive.targets is not None:
-            if self.predictive.targets.sample_index() != self.time_series.sample_index():
-                raise ValueError(EXCEPTION_MESSAGES.sample_index_mismatch.targets)
+        if self.predictive.targets.sample_index() != self.time_series.sample_index():
+            raise ValueError(EXCEPTION_MESSAGES.sample_index_mismatch.targets)
         # TODO: Possible checks - some checks on .time_series and .predictive.targets in terms of
         # their relative position in time?
 
-    @property
-    def fit_ready(self) -> bool:
-        return self.predictive.targets is not None
-
-    @property
-    def predict_ready(self) -> bool:
-        return True
-
 
-class OneOffTreatmentEffectsDataset(PredictiveDataset):
+class OneOffTreatmentEffectsDataset(Dataset):
     predictive: pred.OneOffTreatmentEffectsTaskData
 
-    def __init__(
+    def __init__(  # pylint: disable=useless-super-delegation
         self,
         time_series: data_typing.DataContainer,
         *,
-        targets: Optional[data_typing.DataContainer],
+        targets: data_typing.DataContainer,
         treatments: data_typing.DataContainer,
         static: Optional[data_typing.DataContainer] = None,
         **kwargs,
     ) -> None:
-        """A :class:`PredictiveDataset` subclass for the one-off treatment effects problem setting,
-        see :class:`BaseDataset` docs.
+        """A `Dataset` subclass for the one-off treatment effects problem setting, see `Dataset` docs.
 
-        In this setting: ``targets`` are required for fitting, will be initialized as `TimeSeriesSamples`;
-        ``treatments`` are required for both fitting and prediction, will be initialized as `EventSamples`.
+        In this setting: `targets` are required, will be initialized as `TimeSeriesSamples`; `treatments` are required,
+        will be initialized as `EventSamples`.
         """
         super().__init__(time_series=time_series, static=static, targets=targets, treatments=treatments, **kwargs)
 
     def _init_predictive(
         self,
-        targets: Optional[data_typing.DataContainer],
-        treatments: Optional[data_typing.DataContainer],
+        targets: data_typing.DataContainer,
+        treatments: Optional[data_typing.DataContainer] = None,
         **kwargs,
     ) -> None:
         if targets is None:
-            logger.debug(
-                f"`targets` provided was None for {self.__class__.__name__}, "
-                "this Dataset can only be used for prediction not fitting"
-            )
+            raise ValueError("On-off treatment effects task requires `targets`")
         if treatments is None:
-            raise ValueError("One-off treatment effects task requires `treatments`")
-        self.predictive = pred.OneOffTreatmentEffectsTaskData(
-            parent_dataset=self, targets=targets, treatments=treatments, **kwargs
-        )
+            raise ValueError("On-off treatment effects task requires `treatments`")
+        self.predictive = pred.OneOffTreatmentEffectsTaskData(targets=targets, treatments=treatments, **kwargs)
 
     def _validate(self) -> None:
-        if self.predictive.targets is not None:
-            if self.predictive.targets.sample_index() != self.time_series.sample_index():
-                raise ValueError(EXCEPTION_MESSAGES.sample_index_mismatch.targets)
-            if self.predictive.targets.time_indexes() != self.time_series.time_indexes():
-                raise ValueError(EXCEPTION_MESSAGES.time_indexes_mismatch.targets)
+        if self.predictive.targets.sample_index() != self.time_series.sample_index():
+            raise ValueError(EXCEPTION_MESSAGES.sample_index_mismatch.targets)
         if self.predictive.treatments.sample_index() != self.time_series.sample_index():
             raise ValueError(EXCEPTION_MESSAGES.sample_index_mismatch.treatments)
+        # TODO: Possible check - check that .time_series and .predictive.targets have the same time_indexes.
         # TODO: Possible checks - some checks on .time_series and .predictive.treatments in terms of
         # their relative position in time?
 
-    @property
-    def fit_ready(self) -> bool:
-        return self.predictive.targets is not None and self.predictive.treatments is not None
-
-    @property
-    def predict_ready(self) -> bool:
-        return self.predictive.treatments is not None
-
 
-class TemporalTreatmentEffectsDataset(PredictiveDataset):
+class TemporalTreatmentEffectsDataset(Dataset):
     predictive: pred.TemporalTreatmentEffectsTaskData
 
-    def __init__(
+    def __init__(  # pylint: disable=useless-super-delegation
         self,
         time_series: data_typing.DataContainer,
         *,
-        targets: Optional[data_typing.DataContainer],
+        targets: data_typing.DataContainer,
         treatments: data_typing.DataContainer,
         static: Optional[data_typing.DataContainer] = None,
         **kwargs,
     ) -> None:
-        """A :class:`PredictiveDataset` subclass for the temporal treatment effects problem setting,
-        see :class:`BaseDataset` docs.
+        """A `Dataset` subclass for the temporal treatment effects problem setting, see `Dataset` docs.
 
-        In this setting: ``targets`` are required for fitting, will be initialized as `TimeSeriesSamples`;
-        ``treatments`` are required for both fitting and prediction, will be initialized as `TimeSeriesSamples`.
+        In this setting: `targets` are required, will be initialized as `TimeSeriesSamples`; `treatments` are required,
+        will be initialized as `TimeSeriesSamples`.
         """
         super().__init__(time_series=time_series, static=static, targets=targets, treatments=treatments, **kwargs)
 
     def _init_predictive(
         self,
-        targets: Optional[data_typing.DataContainer],
-        treatments: Optional[data_typing.DataContainer],
+        targets: data_typing.DataContainer,
+        treatments: Optional[data_typing.DataContainer] = None,
         **kwargs,
     ) -> None:
         if targets is None:
-            logger.debug(
-                f"`targets` provided was None for {self.__class__.__name__}, "
-                "this Dataset can only be used for prediction not fitting"
-            )
+            raise ValueError("Temporal treatment effects task requires `targets`")
         if treatments is None:
             raise ValueError("Temporal treatment effects task requires `treatments`")
-        self.predictive = pred.TemporalTreatmentEffectsTaskData(
-            parent_dataset=self, targets=targets, treatments=treatments, **kwargs
-        )
+        self.predictive = pred.TemporalTreatmentEffectsTaskData(targets=targets, treatments=treatments, **kwargs)
 
     def _validate(self) -> None:
-        if self.predictive.targets is not None:
-            if self.predictive.targets.sample_index() != self.time_series.sample_index():
-                raise ValueError(EXCEPTION_MESSAGES.sample_index_mismatch.targets)
-            if self.predictive.targets.time_indexes() != self.time_series.time_indexes():
-                raise ValueError(EXCEPTION_MESSAGES.time_indexes_mismatch.targets)
+        if self.predictive.targets.sample_index() != self.time_series.sample_index():
+            raise ValueError(EXCEPTION_MESSAGES.sample_index_mismatch.targets)
         if self.predictive.treatments.sample_index() != self.time_series.sample_index():
             raise ValueError(EXCEPTION_MESSAGES.sample_index_mismatch.treatments)
-        if self.predictive.treatments.time_indexes() != self.time_series.time_indexes():
-            raise ValueError(EXCEPTION_MESSAGES.time_indexes_mismatch.treatments)
-
-    @property
-    def fit_ready(self) -> bool:
-        return self.predictive.targets is not None and self.predictive.treatments is not None
-
-    @property
-    def predict_ready(self) -> bool:
-        return self.predictive.treatments is not None
+        # TODO: Possible check - check that .time_series and .predictive.treatments/targets have the same time_indexes.
```

## tempor/data/pandera_utils.py

```diff
@@ -1,18 +1,13 @@
-import sys
-from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Tuple
 
-import numpy as np
 import pandas as pd
 import pandera as pa
-import pandera.dtypes as pa_dtypes
-import pandera.engines.pandas_engine as pd_engine
-from packaging.version import Version
 
-import tempor.core.utils
+from tempor.log import logger
 
 from . import data_typing
 
 _PA_DF_SCHEMA_INIT_PARAMETERS = [
     "columns",
     "checks",
     "index",
@@ -45,217 +40,120 @@
 _PA_MULTI_INDEX_INIT_PARAMETERS = [
     "indexes",
     "coerce",
     "strict",
     "name",
     "ordered",
     "unique",
+    "report_duplicates",
 ]
 
-if Version(pa.__version__) < Version("0.14"):
-    # Before v0.14, pandera API had an extra parameter `report_duplicates`.
-    _PA_MULTI_INDEX_INIT_PARAMETERS.append("report_duplicates")
-
 
 def _get_pa_init_args(pa_object: Any, param_names: List[str]) -> Dict[str, Any]:
     """A helper method for updating `pandera` objects dynamically.
 
-    Get values of items in ``pa_object``'s ``__dict__``, specified by ``param_names`` .
-    ``param_names`` should contain names (`str`) of the ``__init__`` parameters of the ``pa_object``.
+    Get values of items in `pa_object`'s `__dict__`, specified by `param_names`.
+    `param_names` should contain names (`str`) of the `__init__` parameters of the `pa_object`.
 
     Algorithm:
-    - Will attempt to get by ``param_names`` item.
-    - If not found, will attempt to get by ``param_names`` item prepended with ``_``.
-    - If an ``arg_name`` item isn't found, it is ignored.
+    - Will attempt to get by `param_names` item.
+    - If not found, will attempt to get by `param_names` item prepended with `_`.
+    - If an `arg_name` item isn't found, it is ignored.
 
     Args:
         pa_object (Any): `pandera` object.
-        param_names (List[str]): list of `pandera` object's ``__init__`` parameters.
+        param_names (List[str]): list of `pandera` object's `__init__` parameters.
 
     Returns:
-        Dict[str, Any]: dictionary mapping ``pa_object`` 's ``__init__`` parameter names to their current values.
+        Dict[str, Any]: dictionary mapping `pa_object`'s `__init__` parameter names to their current values.
     """
     # Try attributes with matching name:
     args = set(param_names)
     items = {k: v for k, v in pa_object.__dict__.items() if k in args}
     # If any left, try attributes prepended with `_`.
     args_left = args - set(items.keys())
     _args_left = set([f"_{i}" for i in args_left])
     additional_items = {k[1:]: v for k, v in pa_object.__dict__.items() if k in _args_left}
     items.update(additional_items)
     return items
 
 
-def update_schema(schema: pa.DataFrameSchema, **kwargs) -> pa.DataFrameSchema:
+def update_schema(schema: pa.DataFrameSchema, /, **kwargs) -> pa.DataFrameSchema:
     items = _get_pa_init_args(schema, param_names=_PA_DF_SCHEMA_INIT_PARAMETERS)
     items.update(kwargs)
     return pa.DataFrameSchema(**items)
 
 
-def update_index(index: pa.Index, **kwargs) -> pa.Index:
+def update_index(index: pa.Index, /, **kwargs) -> pa.Index:
     items = _get_pa_init_args(index, param_names=_PA_INDEX_INIT_PARAMETERS)
     items.update(kwargs)
     return pa.Index(**items)
 
 
-def update_multiindex(multi_index: pa.MultiIndex, **kwargs) -> pa.MultiIndex:
+def update_multiindex(multi_index: pa.MultiIndex, /, **kwargs) -> pa.MultiIndex:
     items = _get_pa_init_args(multi_index, param_names=_PA_MULTI_INDEX_INIT_PARAMETERS)
     items.update(kwargs)
     return pa.MultiIndex(**items)
 
 
 PA_DTYPE_MAP: Dict[data_typing.Dtype, pa.DataType] = {
     bool: pa.Bool(),
     int: pa.Int(),
     float: pa.Float(),
     str: pa.String(),
     "category": pa.Category(),
     "datetime": pa.DateTime(),
 }
-"""A mapping from dtype specified as :obj:`~tempor.data.data_typing.Dtype` to a `pandera.DataType`.
+"""A mapping from dtype specified as `Dtype` to a `pandera.DataType`.
 """
 
 
 def get_pa_dtypes(dtypes: Iterable[data_typing.Dtype]) -> List[pa.DataType]:
-    """Return a list of `pandera.DataType` corresponding to ``dtypes``. Raises `KeyError` If not found."""
-    pa_dtypes_ = []
+    """Return a `set` of `pandera.DataType` corresponding to `dtypes`. Raises `KeyError` If not found."""
+    pa_dtypes = []
     for dt in dtypes:
         if isinstance(dt, pa.DataType):
-            # If item in `dtypes` already an instance of `pandera.DataType`, pass it through.
-            dt_add = dt
-        elif hasattr(dt, "__mro__") and issubclass(dt, pa.DataType):  # type: ignore
-            # If item in `dtypes` a `pandera.DataType` class, pass it through as an instance.
-            dt_add = dt()  # type: ignore
+            # If item in `dtypes` already a `pandera.Dtype`, pass it through.
+            pa_dtypes.append(dt)
         else:
             try:
-                dt_add = PA_DTYPE_MAP[dt]
+                pa_dtypes.append(PA_DTYPE_MAP[dt])
             except KeyError as ex:
                 raise KeyError(f"Mapping from `{dt}` to a pandera DataType not found") from ex
-        pa_dtypes_.append(dt_add)
-        if sys.platform == "win32":
-            # Pandera .Int()/.Float() do not appear to correctly validate on Windows, unless one specifically
-            # provides the bytes.
-            if dt_add == pa.Int():
-                pa_dtypes_.extend([pa.Int8(), pa.Int16(), pa.Int32(), pa.Int64()])
-            if dt_add == pa.Float():
-                pa_dtypes_.extend([pa.Float16(), pa.Float32(), pa.Float64()])
-    return list(set(pa_dtypes_))
-
-
-class UnionDtype(pd_engine.DataType):
-    """Extend `pandera` ``DataType`` s with a custom ``UnionDtype``, which will function similarly to ``Union``.
-
-    See `pandera` ``DataType`` [guide](https://pandera.readthedocs.io/en/stable/dtypes.html) for details.
-
-    In this case, rather than wrapping the extension ``DataType`` with ``register_dtype`` and ``immutable`` decorators,
-    we apply these directly to the class returned by ``__class_getitem__``, which dynamically creates the union
-    specified with its dtypes. In this way, `pandera`'s ``pandas`` engine correctly registers each new kind of union
-    as a different dtype.
-    """
-
-    union_dtypes: List
-    """The list of types in the union."""
-    type: Any
-    """The string representation of the data type, which will be, e.g., shown in exceptions."""
-
-    name: str
-    """The string representation of the data type used for `repr`."""
-
-    @classmethod
-    def __class_getitem__(cls, item):
-        """Allows for setting union types like ``UnionDtype[dtype, ...]``.
-
-        Acceptable ``dtype`` s are: `pandera.DataType` (as a class or instance) or the keys of
-        `~tempor.data.pandera_utils.PA_DTYPE_MAP`.
-        """
-        if not tempor.core.utils.is_iterable(item):
-            item = [item]
-        union_dtypes = get_pa_dtypes(item)
-        union_dtypes = sorted(union_dtypes, key=str)  # For consistency: `item` can get captured in random order.
-        repr_union_dtypes = str([str(t) for t in union_dtypes]).replace("'", "")
-        name = f"{cls.__name__}{repr_union_dtypes}"
-
-        cls_ = type(name, (UnionDtype,), dict())
-        cls_.union_dtypes = union_dtypes  # type: ignore
-        cls_.type = name  # type: ignore
-        cls_.name = name  # type: ignore
-
-        return pd_engine.Engine.register_dtype(pa_dtypes.immutable(cls_))  # type: ignore
-
-    def __repr__(self) -> str:
-        return self.name
-
-    def check(
-        self,
-        pandera_dtype: pa_dtypes.DataType,
-        data_container=None,
-    ) -> Union[bool, Iterable[bool]]:
-        """Checks whether the ``pandera_dtype`` and optionally ``data_container`` satisfy at least one the union's
-        ``union_dtypes``.
-
-        Args:
-            pandera_dtype (pa_dtypes.DataType):
-                The data type received as part of the check/validation.
-            data_container (PandasObject, optional):
-                The data container received as part of the check/validation. Defaults to `None`.
-
-        Returns:
-            Union[bool, Iterable[bool]]:
-                A `bool` stating whether the data type is satisfied, or an iterable thereof\
-                (for each item in the ``data_container``).
-        """
-        for union_dtype in self.union_dtypes:
-            validated = pd_engine.Engine.dtype(union_dtype).check(pandera_dtype, data_container)
-            if data_container is None:
-                # Only in case of direct type comparison, we also need to check via the union_dtype.check(pandera_dtype)
-                # method, making sure that pandera_dtype is an DataType instance not class.
-                if hasattr(pandera_dtype, "__mro__"):
-                    pandera_dtype = pandera_dtype()  # type: ignore
-                validated = validated or union_dtype.check(pandera_dtype)
-            if tempor.core.utils.is_iterable(validated):
-                validated = all(validated)  # type: ignore
-            if validated:
-                if data_container is None:
-                    return True
-                else:
-                    return np.full_like(data_container, True, dtype=bool)
-
-        if data_container is None:
-            return False
-        else:
-            return np.full_like(data_container, False, dtype=bool)
+    return list(set(pa_dtypes))
 
-    def coerce(self, data_container):
-        """The ``coerce`` method is not supported and will throw a `NotImplementedError`."""
-        raise NotImplementedError(f"`coerce` not supported by {self.__class__.__name__}")
 
-
-def init_schema(data: pd.DataFrame, **kwargs) -> pa.DataFrameSchema:
-    schema = pa.infer_schema(data)
-    if TYPE_CHECKING:  # pragma: no cover
-        assert isinstance(schema, pa.DataFrameSchema)  # nosec B101
-    schema = update_schema(schema, **kwargs)
-    return schema
+def check_by_series_schema(series: pd.Series, series_name: str, dtypes: List[pa.DataType], **kwargs) -> bool:
+    """Will check that `series` satisfies a `SeriesSchema` with at least one dtype from `dtypes`.
+    May pass additional `SeriesSchema` kwargs via `kwargs`.
+    """
+    logger.trace(f"Doing {series_name} dtype validation.")
+    validated: List[bool] = []
+    for type_ in set(dtypes):
+        try:
+            pa.SeriesSchema(type_, **kwargs).validate(series)
+            logger.trace(f"{series_name} validated? Yes: {type_}")
+            validated.append(True)
+            break
+        except (pa.errors.SchemaError, pa.errors.SchemaErrors):
+            logger.trace(f"{series_name} validated?  No: {type_}")
+            validated.append(False)
+    return any(validated)
 
 
-def add_df_checks(schema: pa.DataFrameSchema, *, checks_list: List[pa.Check]) -> pa.DataFrameSchema:
+def add_df_checks(schema: pa.DataFrameSchema, /, *, checks_list: List[pa.Check]) -> pa.DataFrameSchema:
     schema = update_schema(schema, checks=checks_list)
     return schema
 
 
 def add_regex_column_checks(
-    schema: pa.DataFrameSchema,
-    *,
-    regex: str = ".*",
-    dtype: Any,
-    nullable: bool,
-    checks_list: Optional[List[pa.Check]] = None,
+    schema: pa.DataFrameSchema, /, *, regex: str = ".*", dtype: Any, nullable: bool, checks_list: List[pa.Check]
 ) -> pa.DataFrameSchema:
-    """Update ``schema`` with checks specified in ``checks_list``, applied to all columns specified by ``regex``.
-    ``dtype`` and ``nullable`` can also be specified and will apply to all columns.
+    """Update `schema` with checks specified in `checks_list`, applied to all columns specified by `regex`.
+    `dtype` and `nullable` can also be specified and will apply to all columns.
     """
     schema_out = schema.add_columns(
         {
             regex: pa.Column(
                 dtype=dtype,
                 nullable=nullable,
                 regex=True,
@@ -268,93 +166,83 @@
     return schema_out
 
 
 def set_up_index(
     schema: pa.DataFrameSchema,
     data: pd.DataFrame,
     *,
-    dtype: Any,
     name: str,
     nullable: bool,
     unique: bool,
-    coerce: bool,
-    checks_list: Optional[List[pa.Check]] = None,
+    checks_list: List[pa.Check],
 ) -> Tuple[pa.DataFrameSchema, pd.DataFrame]:
-    """Update ``schema.index`` (`pandera.Index`) with ``dtype``, ``name``, ``nullable``, ... schema settings.
+    """Update `schema.index` (`pandera.Index`) with `name`, `nullable`, ... schema settings.
 
-    In addition, set the index name of ``data`` (`pandas.DataFrame`) to ``name``.
+    In addition, set the index name of `data` (`pandas.DataFrame`) to `name`.
 
     Returns the schema and the dataframe.
     """
     if schema.index is None:
         raise ValueError("Expected DataFrameSchema Index to not be None")
     index = update_index(
         schema.index,
-        dtype=dtype,
         nullable=nullable,
         unique=unique,
         name=name,
         checks=checks_list,
-        coerce=coerce,
     )
     schema = update_schema(schema, index=index)
     data.index.set_names(name, inplace=True)  # Name the index.
     return schema, data
 
 
 def set_up_2level_multiindex(
     schema: pa.DataFrameSchema,
     data: pd.DataFrame,
     *,
-    dtypes: Tuple[Any, Any],
     names: Tuple[str, str],
     nullable: Tuple[bool, bool],
-    coerce: bool,
     unique: Tuple[str, ...],
-    checks_list: Optional[Tuple[List[pa.Check], List[pa.Check]]] = None,
+    checks_list: Tuple[List[pa.Check], List[pa.Check]],
 ) -> Tuple[pa.DataFrameSchema, pd.DataFrame]:
-    """Update ``schema.index`` (`pandera.MultiIndex`), which is expected to have 2 levels, with `dtypes```, ``names``,
-    ``nullable``, ... schema settings.
+    """Update `schema.index` (`pandera.MultiIndex`), which is expected to have 2 levels, with `name`, `nullable`, ...
+    schema settings.
 
-    In addition, set the index name of ``data`` (`pandas.DataFrame`) to ``name``.
+    In addition, set the index name of `data` (`pandas.DataFrame`) to `name`.
 
     Returns the schema and the dataframe.
     """
     if schema.index is None:
         raise ValueError("Expected DataFrameSchema Index to not be None")
     if not isinstance(schema.index, pa.MultiIndex):
         raise ValueError("Expected DataFrameSchema Index to not be MultiIndex")
     if len(schema.index.indexes) != 2:
         raise ValueError("Expected DataFrameSchema Index to have 2 levels")
 
     index_0 = update_index(
         schema.index.indexes[0],
-        dtype=dtypes[0],
         name=names[0],
         nullable=nullable[0],
-        coerce=coerce,
-        checks=checks_list[0] if checks_list is not None else None,
+        checks=checks_list[0],
     )
     index_1 = update_index(
         schema.index.indexes[1],
-        dtype=dtypes[1],
         name=names[1],
-        coerce=coerce,
-        checks=checks_list[1] if checks_list is not None else None,
+        checks=checks_list[1],
     )
 
     index = update_multiindex(schema.index, indexes=[index_0, index_1], unique=unique)
     schema = update_schema(schema, index=index)
     data.index.set_names(names, inplace=True)  # Name the index.
 
     return schema, data
 
 
 class checks:
-    """Namespace containing reusable `pandera.Check` s."""
+    """Namespace containing reusable `pandera.Check`s."""
 
     forbid_multiindex_index = pa.Check(
         lambda df: df.index.nlevels == 1,
         error="MultiIndex Index not allowed",
     )
     forbid_multiindex_columns = pa.Check(
         lambda df: df.columns.nlevels == 1,
@@ -371,24 +259,53 @@
     require_element_len_2 = pa.Check(
         lambda x: len(x) == 2,
         element_wise=True,
         error="Each item must contain a sequence of length 2",
     )
 
     class configurable:
-        """Namespace containing functions to get configurable `pandera.Check` s."""
+        """Namespace containing functions to get configurable `pandera.Check`s."""
 
         @staticmethod
-        def column_index_satisfies_dtype(dtype: Any, *, nullable: bool) -> pa.Check:
-            series_name = "Column Index"
-            error = str(f"DataFrame {series_name} dtype validation failed, must be of type: {dtype}")
+        def values_satisfy_dtypes(dtypes: List[data_typing.Dtype]) -> pa.Check:
+            series_name = "Values"
+            error = str(f"DataFrame {series_name} dtype validation failed, must be one of: {dtypes}")
+            return pa.Check(
+                lambda col: check_by_series_schema(
+                    pd.Series(col),
+                    series_name=series_name,
+                    dtypes=get_pa_dtypes(dtypes),
+                    nullable=True,
+                    coerce=False,  # NOTE: For simplicity "coerce-able" values are not accepted.
+                ),
+                error=error,
+            )
 
-            def _check(df: pd.DataFrame) -> bool:
-                pa.SeriesSchema(
-                    dtype,
-                    name=series_name,
-                    nullable=nullable,
+        @staticmethod
+        def index_satisfies_dtypes(dtypes: List[data_typing.Dtype]) -> pa.Check:
+            series_name = "Index"
+            error = str(f"DataFrame {series_name} dtype validation failed, must be one of: {dtypes}")
+            return pa.Check(
+                lambda idx: check_by_series_schema(
+                    pd.Series(idx),
+                    series_name=series_name,
+                    dtypes=get_pa_dtypes(dtypes),
+                    nullable=False,
                     coerce=False,
-                ).validate(pd.Series(df.columns, name=series_name))
-                return True
+                ),
+                error=error,
+            )
 
-            return pa.Check(_check, error=error)
+        @staticmethod
+        def column_index_satisfies_dtypes(dtypes: List[data_typing.Dtype], *, nullable: bool) -> pa.Check:
+            series_name = "Column Index"
+            error = str(f"DataFrame {series_name} dtype validation failed, must be one of: {dtypes}")
+            return pa.Check(
+                lambda df: check_by_series_schema(
+                    pd.Series(df.columns),
+                    series_name=series_name,
+                    dtypes=get_pa_dtypes(dtypes),
+                    nullable=nullable,
+                    coerce=False,
+                ),
+                error=error,
+            )
```

## tempor/data/predictive.py

```diff
@@ -1,175 +1,128 @@
 import abc
-from typing import TYPE_CHECKING, Any, Optional
+from typing import Any, Optional
 
 import rich.pretty
 
 from tempor.core.utils import RichReprStrPassthrough
 
 from . import data_typing, samples
 
-if TYPE_CHECKING:  # pragma: no cover
-    from .dataset import PredictiveDataset  # For typing only, no circular import.
-
-
 # TODO: Unit test.
 
 
 class PredictiveTaskData(abc.ABC):
-    _targets: Optional[samples.DataSamples]
-    _treatments: Optional[samples.DataSamples]
+    targets: samples.DataSamples
+    treatments: Optional[samples.DataSamples]
 
     @property
     @abc.abstractmethod
     def predictive_task(self) -> data_typing.PredictiveTask:  # pragma: no cover
         ...
 
+    @abc.abstractmethod
     def __init__(
         self,
-        parent_dataset: "PredictiveDataset",
-        targets: Any,  # pylint: disable=unused-argument
-        treatments: Optional[Any],  # pylint: disable=unused-argument
-        **kwargs,  # pylint: disable=unused-argument
+        targets: Any,
+        treatments: Optional[Any],
+        **kwargs,
     ) -> None:  # pragma: no cover
-        self.parent_dataset = parent_dataset
-        # ^ In order to be able to call parent dataset's `validate` method in the targets/treatments property setters.
-
-        self._targets = targets
-        self._treatments = treatments
+        ...
 
     def __rich_repr__(self):
-        if self.targets is not None:
-            yield "targets", RichReprStrPassthrough(self.targets.short_repr())
-        else:
-            yield "targets", None
+        yield "targets", RichReprStrPassthrough(self.targets.short_repr())
         if self.treatments is not None:
             yield "treatments", RichReprStrPassthrough(self.treatments.short_repr())
 
     def __repr__(self) -> str:
         return rich.pretty.pretty_repr(self)
 
-    @property
-    def targets(self) -> Optional[samples.DataSamples]:
-        return self._targets
-
-    @targets.setter
-    def targets(self, value: Optional[samples.DataSamples]) -> None:
-        self._targets = value
-        self.parent_dataset.validate()
-
-    @property
-    def treatments(self) -> Optional[samples.DataSamples]:
-        return self._treatments
-
-    @treatments.setter
-    def treatments(self, value: Optional[samples.DataSamples]) -> None:
-        self._treatments = value
-        self.parent_dataset.validate()
-
 
 # Predictive task data classes corresponding to different tasks follow. More can be added to handle new tasks.
 
 # --- Prediction tasks: ---
 
 
 class OneOffPredictionTaskData(PredictiveTaskData):
     # One-off prediction (e.g., one-off classification with a target like patient death).
 
-    targets: Optional[samples.StaticSamples]
+    targets: samples.StaticSamples
     treatments: None
 
     @property
     def predictive_task(self) -> data_typing.PredictiveTask:
         return data_typing.PredictiveTask.ONE_OFF_PREDICTION
 
-    def __init__(
-        self, parent_dataset: "PredictiveDataset", targets: Optional[data_typing.DataContainer], **kwargs
-    ) -> None:
-        super().__init__(parent_dataset=parent_dataset, targets=targets, treatments=None)
-        self._targets = samples.StaticSamples(targets) if targets is not None else None
-        self._treatments = None
+    def __init__(self, targets: data_typing.DataContainer, **kwargs) -> None:
+        self.targets = samples.StaticSamples(targets)
+        self.treatments = None
+        super().__init__(targets=targets, treatments=None)
 
 
 class TemporalPredictionTaskData(PredictiveTaskData):
     # Temporal prediction (e.g., predicting a patient's temperature real valued time series).
 
-    targets: Optional[samples.TimeSeriesSamples]
+    targets: samples.TimeSeriesSamples
     treatments: None
 
     @property
     def predictive_task(self) -> data_typing.PredictiveTask:
         return data_typing.PredictiveTask.TEMPORAL_PREDICTION
 
-    def __init__(
-        self, parent_dataset: "PredictiveDataset", targets: Optional[data_typing.DataContainer], **kwargs
-    ) -> None:
-        super().__init__(parent_dataset=parent_dataset, targets=targets, treatments=None)
-        self._targets = samples.TimeSeriesSamples(targets) if targets is not None else None
-        self._treatments = None
+    def __init__(self, targets: data_typing.DataContainer, **kwargs) -> None:
+        self.targets = samples.TimeSeriesSamples(targets)
+        self.treatments = None
+        super().__init__(targets=targets, treatments=None)
 
 
 # --- Time-to-event tasks: ---
 
 
 class TimeToEventAnalysisTaskData(PredictiveTaskData):
     # Time-to-event (survival) analysis (e.g. Dynamic DeepHit).
 
-    targets: Optional[samples.EventSamples]
+    targets: samples.EventSamples
     treatments: None
 
     @property
     def predictive_task(self) -> data_typing.PredictiveTask:
         return data_typing.PredictiveTask.TIME_TO_EVENT_ANALYSIS
 
-    def __init__(
-        self, parent_dataset: "PredictiveDataset", targets: Optional[data_typing.DataContainer], **kwargs
-    ) -> None:
-        super().__init__(parent_dataset=parent_dataset, targets=targets, treatments=None)
-        self._targets = samples.EventSamples(targets) if targets is not None else None
-        self._treatments = None
+    def __init__(self, targets: data_typing.DataContainer, **kwargs) -> None:
+        self.targets = samples.EventSamples(targets)
+        self.treatments = None
+        super().__init__(targets=targets, treatments=None)
 
 
 # --- Treatment Effects tasks: ---
 
 
 class OneOffTreatmentEffectsTaskData(PredictiveTaskData):
     # Treatment effects with time series outcomes but one-off treatment event(s) (e.g. SyncTwin)
 
-    targets: Optional[samples.TimeSeriesSamples]
+    targets: samples.TimeSeriesSamples
     treatments: samples.EventSamples
 
     @property
     def predictive_task(self) -> data_typing.PredictiveTask:
         return data_typing.PredictiveTask.TEMPORAL_TREATMENT_EFFECTS
 
-    def __init__(
-        self,
-        parent_dataset: "PredictiveDataset",
-        targets: Optional[data_typing.DataContainer],
-        treatments: data_typing.DataContainer,
-        **kwargs,
-    ) -> None:
-        super().__init__(parent_dataset=parent_dataset, targets=targets, treatments=treatments)
-        self._targets = samples.TimeSeriesSamples(targets) if targets is not None else None
-        self._treatments = samples.EventSamples(treatments)
+    def __init__(self, targets: data_typing.DataContainer, treatments: data_typing.DataContainer, **kwargs) -> None:
+        self.targets = samples.TimeSeriesSamples(targets)
+        self.treatments = samples.EventSamples(treatments)
+        super().__init__(targets=targets, treatments=treatments)
 
 
 class TemporalTreatmentEffectsTaskData(PredictiveTaskData):
     # Temporal treatment effects (i.e. outcomes are time series and treatments are also time series, e.g. RMSN, CRN).
 
-    targets: Optional[samples.TimeSeriesSamples]
+    targets: samples.TimeSeriesSamples
     treatments: samples.TimeSeriesSamples
 
     @property
     def predictive_task(self) -> data_typing.PredictiveTask:
         return data_typing.PredictiveTask.TEMPORAL_TREATMENT_EFFECTS
 
-    def __init__(
-        self,
-        parent_dataset: "PredictiveDataset",
-        targets: Optional[data_typing.DataContainer],
-        treatments: data_typing.DataContainer,
-        **kwargs,
-    ) -> None:
-        super().__init__(parent_dataset=parent_dataset, targets=targets, treatments=treatments)
-        self._targets = samples.TimeSeriesSamples(targets) if targets is not None else None
-        self._treatments = samples.TimeSeriesSamples(treatments)
+    def __init__(self, targets: data_typing.DataContainer, treatments: data_typing.DataContainer, **kwargs) -> None:
+        self.targets = samples.TimeSeriesSamples(targets)
+        self.treatments = samples.TimeSeriesSamples(treatments)
+        super().__init__(targets=targets, treatments=treatments)
```

## tempor/data/samples.py

```diff
@@ -1,19 +1,19 @@
-"""Data handling for different data samples modalities supported by TemporAI."""
+"""Data handling for different data samples modalities supported by TemporAI.
+"""
 
 # pylint: disable=useless-super-delegation, unnecessary-ellipsis
 
 import abc
-from typing import TYPE_CHECKING, Any, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any, List, Optional
 
 import numpy as np
 import pandas as pd
 import pandera as pa
 import pydantic
-from typing_extensions import Self
 
 import tempor.exc
 from tempor.log import log_helpers, logger
 
 from . import data_typing, pandera_utils, utils
 from .settings import DATA_SETTINGS
 
@@ -27,82 +27,69 @@
         ...
 
     def __init__(
         self,
         data: data_typing.DataContainer,  # pylint: disable=unused-argument
         **kwargs,  # pylint: disable=unused-argument
     ) -> None:  # pragma: no cover
-        if "_skip_validate" not in kwargs:
-            # For efficiency, pass `_skip_validate` internally (e.g. in `__getitem__`)
-            # when there is no need to validate.
-            self.validate()
+        self.validate()
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__} with data:\n{self.dataframe()}"
 
-    def _repr_html_(self) -> str:
-        repr_ = (
-            # pylint: disable-next=protected-access
-            f'<p><span style="font-family: monospace;">{self.__class__.__name__}</span> with data:</p>'
-            f"{self.dataframe()._repr_html_()}"  # pyright: ignore
-        )
-        return repr_
-
     def validate(self) -> None:
         with log_helpers.exc_to_log():
             try:
                 self._validate()
             except (
-                pa.errors.SchemaError,  # pyright: ignore
-                pa.errors.SchemaErrors,  # pyright: ignore
+                pa.errors.SchemaError,
+                pa.errors.SchemaErrors,
                 ValueError,
                 TypeError,
             ) as ex:
                 raise tempor.exc.DataValidationException(
                     "Data validation failed, see traceback for more details"
                 ) from ex
 
     @abc.abstractmethod
     def _validate(self) -> None:  # pragma: no cover
         """Validate integrity of the data samples. Raise any of `ValueError`, `TypeError`,
-        `pandera.errors.SchemaError`, `pandera.errors.SchemaErrors` (or exceptions derived from these) to indicate
-        validation failure.
+        `pandera.errors.SchemaError[s]` (or exceptions derived from these) to indicate validation failure.
         """
         ...
 
     @staticmethod
     @abc.abstractmethod
     def from_numpy(
         array: np.ndarray,
         *,
         sample_index: Optional[data_typing.SampleIndex] = None,
         feature_index: Optional[data_typing.FeatureIndex] = None,
         **kwargs,
     ) -> "DataSamples":  # pragma: no cover
-        """Create :class:`DataSamples` from `numpy.ndarray`.
+        """Create `DataSamples` from `numpy.ndarray`.
 
         Args:
-            array (np.ndarray):
-                The array that represents the data.
-            sample_index (List[<sample element>], optional):
-                List with sample (row) index for each sample. Optional, if `None`, will be of form ``[0, 1, ...]``.
-                Defaults to `None`.
-            feature_index (List[<feature element>], optional):
-                List with feature (column) index for each feature. Optional, if `None`, will be of form
-                ``["feat_0", "feat_1", ...]``. Defaults to `None`.
+            array (np.ndarray): The array that represents the data.
+            sample_index (List[<sample element>], optional): List with sample (row) index for each sample.
+            Optional, if `None`, will be of form `[0, 1, ...]`. Defaults to `None`.
+            feature_index (List[<feature element>], optional): List with feature (column) index for each feature.
+            Optional, if `None`, will be of form `["feat_0", "feat_1", ...]`. Defaults to `None`.
 
         Returns:
-            DataSamples: :class:`DataSamples` object from ``array``.
+            DataSamples: `DataSamples` object from `array`.
         """
         ...
 
     @staticmethod
     @abc.abstractmethod
     def from_dataframe(dataframe: pd.DataFrame, **kwargs) -> "DataSamples":  # pragma: no cover
-        """Create :class:`DataSamples` from `pandas.DataFrame`."""
+        """
+        Create `DataSamples` from `pandas.DataFrame`.
+        """
         ...
 
     @abc.abstractmethod
     def numpy(self, **kwargs) -> np.ndarray:  # pragma: no cover
         """Return `numpy.ndarray` representation of the data."""
         ...
 
@@ -131,18 +118,14 @@
         """Return number of features."""
         ...
 
     @abc.abstractmethod
     def short_repr(self) -> str:  # pragma: no cover
         ...
 
-    @abc.abstractmethod
-    def __getitem__(self, key: data_typing.GetItemKey) -> Self:
-        ...
-
 
 def _array_default_sample_index(array: np.ndarray) -> List[int]:
     n_samples, *_ = array.shape
     return list(range(0, n_samples))
 
 
 def _array_default_feature_index(array: np.ndarray) -> List[str]:
@@ -164,76 +147,73 @@
         self,
         data: data_typing.DataContainer,
         *,
         sample_index: Optional[data_typing.SampleIndex] = None,
         feature_index: Optional[data_typing.FeatureIndex] = None,
         **kwargs,
     ) -> None:
-        """Create a :class:`StaticSamples` object from the ``data``.
+        """Create a `StaticSamples` object from the `data`.
 
         Args:
-            data (numpy.ndarray | pandas.DataFrame):
-                A container with the data.
-            sample_index (List[<sample element>], optional):
-                Used only if ``data`` is a `numpy.ndarray`. List with sample (row) index for each sample. Optional,
-                if `None`, will be of form ``[0, 1, ...]``. Defaults to `None`.
-            feature_index (List[<feature element>], optional):
-                Used only if ``data`` is a `numpy.ndarray`.  List with feature (column) index for each feature.
-                Optional, if `None`, will be of form ``["feat_0", "feat_1", ...]``. Defaults to `None`.
+            data (numpy.ndarray | pandas.DataFrame): A container with the data.
+            sample_index (List[<sample element>], optional): Used only if `data` is a `numpy.ndarray`. List with sample
+            (row) index for each sample. Optional, if `None`, will be of form `[0, 1, ...]`. Defaults to `None`.
+            feature_index (List[<feature element>], optional): Used only if `data` is a `numpy.ndarray`.  List with
+            feature (column) index for each feature. Optional, if `None`, will be of form `["feat_0", "feat_1", ...]`.
+            Defaults to `None`.
         """
         if isinstance(data, pd.DataFrame):
             self._data = data
         elif isinstance(data, np.ndarray):
             self._data = self._array_to_df(data, sample_index=sample_index, feature_index=feature_index, **kwargs)
         else:  # pragma: no cover  # Prevented by pydantic check.
             raise ValueError(f"Data object {type(data)} not supported")
         super().__init__(data, **kwargs)
 
     @property
     def modality(self) -> data_typing.DataModality:
         return data_typing.DataModality.STATIC
 
     def _validate(self) -> None:
-        schema = pandera_utils.init_schema(self._data, coerce=False)
+        schema = pa.infer_schema(self._data)
         if TYPE_CHECKING:  # pragma: no cover
             assert isinstance(schema, pa.DataFrameSchema)  # nosec B101
         logger.debug(f"Inferred schema:\n{schema}")
 
         # DataFrame-level validation:
         schema = pandera_utils.add_df_checks(
             schema,
             checks_list=[
                 pandera_utils.checks.forbid_multiindex_index,
                 pandera_utils.checks.forbid_multiindex_columns,
-                pandera_utils.checks.configurable.column_index_satisfies_dtype(
-                    pandera_utils.UnionDtype[DATA_SETTINGS.feature_index_dtypes],  # type: ignore
-                    nullable=DATA_SETTINGS.feature_index_nullable,
+                pandera_utils.checks.configurable.column_index_satisfies_dtypes(
+                    DATA_SETTINGS.feature_index_dtypes, nullable=DATA_SETTINGS.feature_index_nullable
                 ),
             ],
         )
         self._data = schema.validate(self._data)
 
         # Values validation:
         schema = pandera_utils.add_regex_column_checks(
             schema,
             regex=".*",
-            dtype=pandera_utils.UnionDtype[DATA_SETTINGS.static_value_dtypes],  # type: ignore
+            dtype=None,
             nullable=DATA_SETTINGS.static_values_nullable,
+            checks_list=[pandera_utils.checks.configurable.values_satisfy_dtypes(DATA_SETTINGS.static_value_dtypes)],
         )
         self._data = schema.validate(self._data)
 
         # Index validation:
         schema, data = pandera_utils.set_up_index(
             schema,
             self._data,
-            dtype=pandera_utils.UnionDtype[DATA_SETTINGS.sample_index_dtypes],  # type: ignore
             name=DATA_SETTINGS.sample_index_name,
             nullable=DATA_SETTINGS.sample_index_nullable,
-            coerce=False,
             unique=DATA_SETTINGS.sample_index_unique,
+            checks_list=[pandera_utils.checks.configurable.index_satisfies_dtypes(DATA_SETTINGS.sample_index_dtypes)],
         )
         self._data = schema.validate(data)
 
         logger.debug(f"Final schema:\n{schema}")
         self._schema = schema
 
     @staticmethod
@@ -280,21 +260,14 @@
     @property
     def num_features(self) -> int:
         return self._data.shape[1]
 
     def short_repr(self) -> str:
         return f"{self.__class__.__name__}([{self.num_samples}, {self.num_features}])"
 
-    def __getitem__(self, key: data_typing.GetItemKey) -> Self:
-        key_ = utils.ensure_pd_iloc_key_returns_df(key)
-        return StaticSamples(  # type: ignore[return-value]
-            self._data.iloc[key_, :],  # pyright: ignore
-            _skip_validate=True,
-        )
-
 
 class TimeSeriesSamples(DataSamples):
     _data: pd.DataFrame
     _schema: pa.DataFrameSchema
 
     @property
     def modality(self) -> data_typing.DataModality:
@@ -307,39 +280,34 @@
         *,
         padding_indicator: Any = None,
         sample_index: Optional[data_typing.SampleIndex] = None,
         time_indexes: Optional[data_typing.TimeIndexList] = None,
         feature_index: Optional[data_typing.FeatureIndex] = None,
         **kwargs,
     ) -> None:
-        """Create a :class:`TimeSeriesSamples` object from the ``data``.
+        """Create a `TimeSeriesSamples` object from the `data`.
 
-        If ``data`` is a `pandas.DataFrame`, this should be a 2-level multiindex (sample, timestep) dataframe.
+        If `data` is a `pandas.DataFrame`, this should be a 2-level multiindex (sample, timestep) dataframe.
 
-        If ``data`` is a `numpy.ndarray`, this should be a 3D array, with dimensions ``(sample, timestep, feature)``.
-        Optionally, padding values of ``padding_indicator`` can be set inside the array to pad out the length of arrays
+        If `data` is a `numpy.ndarray`, this should be a 3D array, with dimensions `(sample, timestep, feature)`.
+        Optionally, padding values of `padding_indicator` can be set inside the array to pad out the length of arrays
         of different samples in case they differ. Padding needs to go at the end of the timesteps (dim 1). Padding must
         be the same across the feature dimension (dim 2) for each sample.
 
         Args:
-            data (numpy.ndarray | pandas.DataFrame):
-                A container with the data.
-            padding_indicator (Any, optional):
-                Padding indicator used in ``data`` to indicate padding. Defaults to `None`.
-            sample_index (List[<sample element>], optional):
-                Used only if ``data`` is a `numpy.ndarray`. List with sample (row) index for each sample.
-                Optional, if `None`, will be of form ``[0, 1, ...]``. Defaults to `None`.
-            time_indexes (List[List[<timestep element>]], optional):
-                Used only if ``data`` is a `numpy.ndarray`. List of lists containing timesteps for each sample (outer
-                list should be the same length as dim 0 of `data`, inner list should contain as many elements as each
-                sample has timesteps). Optional, if `None`, will be of form ``[[0, 1, ...], [0, 1, ...], ...]``
-                Defaults to `None`.
-            feature_index (List[<feature element>], optional):
-                Used only if ``data`` is a `numpy.ndarray`.  List with feature (column) index for each feature.
-                Optional, if `None`, will be of form ``["feat_0", "feat_1", ...]``.
+            data (numpy.ndarray | pandas.DataFrame): A container with the data.
+            padding_indicator (Any, optional): Padding indicator used in `data` to indicate padding. Defaults to None.
+            sample_index (List[<sample element>], optional): Used only if `data` is a `numpy.ndarray`. List with sample
+            (row) index for each sample. Optional, if `None`, will be of form `[0, 1, ...]`. Defaults to `None`.
+            time_indexes (List[List[<timestep element>]], optional): Used only if `data` is a `numpy.ndarray`. List of
+            lists containing timesteps for each sample (outer list should be the same length as dim 0 of `data`,
+            inner list should contain as many elements as each sample has timesteps). Optional, if `None`, will be of
+            form `[[0, 1, ...], [0, 1, ...], ...]` Defaults to None.
+            feature_index (List[<feature element>], optional): Used only if `data` is a `numpy.ndarray`.  List with
+            feature (column) index for each feature. Optional, if `None`, will be of form `["feat_0", "feat_1", ...]`.
         """
         if isinstance(data, pd.DataFrame):
             self._data = data
         elif isinstance(data, np.ndarray):
             self._data = self._array_to_df(
                 data,
                 padding_indicator=padding_indicator,
@@ -349,57 +317,58 @@
                 **kwargs,
             )
         else:  # pragma: no cover  # Prevented by pydantic check.
             raise ValueError(f"Data object {type(data)} not supported")
         super().__init__(data, **kwargs)
 
     def _validate(self) -> None:
-        schema = pandera_utils.init_schema(self._data, coerce=False)
+        schema = pa.infer_schema(self._data)
         if TYPE_CHECKING:  # pragma: no cover
             assert isinstance(schema, pa.DataFrameSchema)  # nosec B101
         logger.debug(f"Inferred schema:\n{schema}")
 
         # DataFrame-level validation:
         schema = pandera_utils.add_df_checks(
             schema,
             checks_list=[
                 pandera_utils.checks.forbid_multiindex_columns,
                 pandera_utils.checks.require_2level_multiindex_index,
-                pandera_utils.checks.configurable.column_index_satisfies_dtype(
-                    pandera_utils.UnionDtype[DATA_SETTINGS.feature_index_dtypes],  # type: ignore
-                    nullable=DATA_SETTINGS.feature_index_nullable,
+                pandera_utils.checks.configurable.column_index_satisfies_dtypes(
+                    DATA_SETTINGS.feature_index_dtypes, nullable=DATA_SETTINGS.feature_index_nullable
                 ),
             ],
         )
         self._data = schema.validate(self._data)
 
         # Values validation:
         schema = pandera_utils.add_regex_column_checks(
             schema,
             regex=".*",
-            dtype=pandera_utils.UnionDtype[DATA_SETTINGS.time_series_value_dtypes],  # type: ignore
+            dtype=None,
             nullable=DATA_SETTINGS.time_series_values_nullable,
+            checks_list=[
+                pandera_utils.checks.configurable.values_satisfy_dtypes(DATA_SETTINGS.time_series_value_dtypes)
+            ],
         )
         self._data = schema.validate(self._data)
 
         # Index validation:
         if not (DATA_SETTINGS.sample_index_unique and DATA_SETTINGS.sample_timestep_index_unique):
             raise NotImplementedError("Only supported case: unique sample and unique timestep indexes")
         multiindex_unique_def = (DATA_SETTINGS.sample_index_name, DATA_SETTINGS.time_index_name)
         schema, data = pandera_utils.set_up_2level_multiindex(
             schema,
             self._data,
-            dtypes=(
-                pandera_utils.UnionDtype[DATA_SETTINGS.sample_index_dtypes],  # type: ignore
-                pandera_utils.UnionDtype[DATA_SETTINGS.time_index_dtypes],  # type: ignore
-            ),
             names=(DATA_SETTINGS.sample_index_name, DATA_SETTINGS.time_index_name),
             nullable=(DATA_SETTINGS.sample_index_nullable, DATA_SETTINGS.time_index_nullable),
-            coerce=False,
             unique=multiindex_unique_def,
+            checks_list=(
+                [pandera_utils.checks.configurable.index_satisfies_dtypes(DATA_SETTINGS.sample_index_dtypes)],
+                [pandera_utils.checks.configurable.index_satisfies_dtypes(DATA_SETTINGS.time_index_dtypes)],
+            ),
         )
         self._data = schema.validate(data)
 
         logger.debug(f"Final schema:\n{schema}")
         self._schema = schema
 
         # TODO:
@@ -461,109 +430,56 @@
             df=self._data, padding_indicator=padding_indicator, max_timesteps=None
         )
 
     def dataframe(self, **kwargs) -> pd.DataFrame:
         return self._data
 
     def sample_index(self) -> data_typing.SampleIndex:
-        return list(utils.get_df_index_level0_unique(self._data))  # pyright: ignore
+        return list(self._data.index.levels[0])  # pyright: ignore
 
     def time_indexes(self) -> data_typing.TimeIndexList:
         """Get a list containing time indexes for each sample. Each time index is represented as a list of time step
         elements.
 
         Returns:
             List[List[<timestep element>]]: A list containing time indexes for each sample.
         """
-        return list(self.time_indexes_as_dict().values())  # pyright: ignore
+        return list(self.time_indexes_as_dict().values())
 
     def time_indexes_as_dict(self) -> data_typing.SampleToTimeIndexDict:
         """Get a dictionary mapping each sample index to its time index. Time index is represented as a list of time
         step elements.
 
         Returns:
             Dict[<sample element>, List[<timestep element>]]: A list containing time indexes for each sample.
         """
         multiindex = self._data.index
         if TYPE_CHECKING:  # pragma: no cover
             assert isinstance(multiindex, pd.MultiIndex)  # nosec B101
-        sample_index = self.sample_index()
+        sample_index = list(self._data.index.levels[0])  # pyright: ignore
         d = dict()
         for s in sample_index:
-            time_index_locs = multiindex.get_locs([s, slice(None)])
+            time_index_locs = multiindex.get_locs(s)
             d[s] = list(multiindex.get_level_values(1)[time_index_locs])
-        return d  # type: ignore[return-value]
-
-    def time_indexes_float(self) -> List[np.ndarray]:
-        """Return time indexes but converting their elements to `float` values.
-
-        Date-time time index will be converted using :obj:`~tempor.data.utils.datetime_time_index_to_float`.
-
-        Returns:
-            List[np.ndarray]: List of 1D `numpy.ndarray` s of `float` values, corresponding to the time index.
-        """
-        return [utils.datetime_time_index_to_float(ti) for ti in self.time_indexes()]
-
-    def num_timesteps(self) -> List[int]:
-        """Get the number of timesteps for each sample.
-
-        Returns:
-            List[int]: List containing the number of timesteps for each sample.
-        """
-        return [len(x) for x in self.time_indexes()]
+        return d
 
-    def num_timesteps_as_dict(self) -> data_typing.SampleToNumTimestepsDict:
-        """Get a dictionary mapping each sample index to its the number of timesteps.
-
-        Returns:
-            List[int]: List containing the number of timesteps for each sample.
-        """
-        return {key: len(x) for key, x in self.time_indexes_as_dict().items()}  # type: ignore
-
-    def num_timesteps_equal(self) -> bool:
-        """Returns `True` if all samples share the same number of timesteps, `False` otherwise.
-
-        Returns:
-            bool: whether all samples share the same number of timesteps.
-        """
-        timesteps = self.num_timesteps()
-        return True if len(timesteps) == 0 else all([x == timesteps[0] for x in timesteps])
-
-    def list_of_dataframes(self) -> List[pd.DataFrame]:
-        """Returns a list of dataframes where each dataframe has the data for each sample.
-
-        Returns:
-            List[pd.DataFrame]: List of dataframes for each sample.
-        """
-        return utils.multiindex_timeseries_dataframe_to_list_of_dataframes(self._data)
+    # TODO: time indexes sensibly converted to floats would be useful.
 
     @property
     def num_samples(self) -> int:
-        sample_ids = utils.get_df_index_level0_unique(self._data)
+        sample_ids = self._data.index.levels[0]  # pyright: ignore
         return len(sample_ids)
 
     @property
     def num_features(self) -> int:
         return self._data.shape[1]
 
     def short_repr(self) -> str:
         return f"{self.__class__.__name__}([{self.num_samples}, *, {self.num_features}])"
 
-    def __getitem__(self, key: data_typing.GetItemKey) -> Self:
-        key_ = utils.ensure_pd_iloc_key_returns_df(key)
-        sample_index = utils.get_df_index_level0_unique(self._data)
-        selected = list(sample_index[key_])  # pyright: ignore
-        return TimeSeriesSamples(  # type: ignore[return-value]
-            self._data.loc[(selected, slice(None)), :],  # pyright: ignore
-            _skip_validate=True,
-        )
-
-
-_DEFAULT_EVENTS_TIME_FEATURE_SUFFIX = "_time"
-
 
 class EventSamples(DataSamples):
     _data: pd.DataFrame
     _schema: pa.DataFrameSchema
     _schema_split: pa.DataFrameSchema
 
     @property
@@ -575,49 +491,46 @@
         self,
         data: data_typing.DataContainer,
         *,
         sample_index: Optional[data_typing.SampleIndex] = None,
         feature_index: Optional[data_typing.FeatureIndex] = None,
         **kwargs,
     ) -> None:
-        """Create an :class:`EventSamples` object from the ``data``.
+        """Create an `EventSamples` object from the `data`.
 
         Args:
-            data (numpy.ndarray | pandas.DataFrame):
-                A container with the data.
-            sample_index (List[<sample element>], optional):
-                Used only if ``data`` is a `numpy.ndarray`. List with sample (row) index for each sample. Optional,
-                if `None`, will be of form ``[0, 1, ...]``. Defaults to `None`.
-            feature_index (List[<feature element>], optional):
-                Used only if ``data`` is a `numpy.ndarray`.  List with feature (column) index for each feature.
-                Optional, if `None`, will be of form ``["feat_0", "feat_1", ...]``. Defaults to `None`.
+            data (numpy.ndarray | pandas.DataFrame): A container with the data.
+            sample_index (List[<sample element>], optional): Used only if `data` is a `numpy.ndarray`. List with sample
+            (row) index for each sample. Optional, if `None`, will be of form `[0, 1, ...]`. Defaults to `None`.
+            feature_index (List[<feature element>], optional): Used only if `data` is a `numpy.ndarray`.  List with
+            feature (column) index for each feature. Optional, if `None`, will be of form `["feat_0", "feat_1", ...]`.
+            Defaults to `None`.
         """
         if isinstance(data, pd.DataFrame):
             self._data = data
         elif isinstance(data, np.ndarray):
             self._data = self._array_to_df(data, sample_index=sample_index, feature_index=feature_index, **kwargs)
         else:  # pragma: no cover  # Prevented by pydantic check.
             raise ValueError(f"Data object {type(data)} not supported")
         super().__init__(data, **kwargs)
 
     def _validate(self) -> None:
-        schema = pandera_utils.init_schema(self._data, coerce=False)
+        schema = pa.infer_schema(self._data)
         if TYPE_CHECKING:  # pragma: no cover
             assert isinstance(schema, pa.DataFrameSchema)  # nosec B101
         logger.debug(f"Inferred schema:\n{schema}")
 
         # DataFrame-level validation:
         schema = pandera_utils.add_df_checks(
             schema,
             checks_list=[
                 pandera_utils.checks.forbid_multiindex_index,
                 pandera_utils.checks.forbid_multiindex_columns,
-                pandera_utils.checks.configurable.column_index_satisfies_dtype(
-                    pandera_utils.UnionDtype[DATA_SETTINGS.feature_index_dtypes],  # type: ignore
-                    nullable=DATA_SETTINGS.feature_index_nullable,
+                pandera_utils.checks.configurable.column_index_satisfies_dtypes(
+                    DATA_SETTINGS.feature_index_dtypes, nullable=DATA_SETTINGS.feature_index_nullable
                 ),
             ],
         )
         self._data = schema.validate(self._data)
 
         # Values validation:
         schema = pandera_utils.add_regex_column_checks(
@@ -625,42 +538,43 @@
             regex=".*",
             dtype=None,
             nullable=DATA_SETTINGS.event_values_nullable,
             checks_list=[pandera_utils.checks.require_element_len_2],
         )
         self._data = schema.validate(self._data)
         # Validate event time and value components:
-        suffix = _DEFAULT_EVENTS_TIME_FEATURE_SUFFIX
+        suffix = "_time"
         data_split = self.split(time_feature_suffix=suffix)
-        schema_split = pandera_utils.init_schema(data_split, coerce=False)
+        schema_split = pa.infer_schema(data_split)
         schema_split = pandera_utils.add_regex_column_checks(
             schema_split,
             regex=f".*{suffix}$",  # Event time columns, end in "_time".
-            dtype=pandera_utils.UnionDtype[DATA_SETTINGS.time_index_dtypes],  # type: ignore
+            dtype=None,
             nullable=DATA_SETTINGS.time_index_nullable,
+            checks_list=[pandera_utils.checks.configurable.values_satisfy_dtypes(DATA_SETTINGS.time_index_dtypes)],
         )
         schema_split = pandera_utils.add_regex_column_checks(
             schema_split,
             regex=f"^((?!{suffix}$).)*$",  # Event value columns, do not end in "_time".
-            dtype=pandera_utils.UnionDtype[DATA_SETTINGS.event_value_dtypes],  # type: ignore
+            dtype=None,
             nullable=DATA_SETTINGS.event_values_nullable,
+            checks_list=[pandera_utils.checks.configurable.values_satisfy_dtypes(DATA_SETTINGS.event_value_dtypes)],
         )
         logger.debug(f"Time split-off schema (checks event time and values separately):\n{schema_split}")
         schema_split.validate(data_split)
         self._schema_split = schema_split
 
         # Index validation:
         schema, data = pandera_utils.set_up_index(
             schema,
             self._data,
-            dtype=pandera_utils.UnionDtype[DATA_SETTINGS.sample_index_dtypes],  # type: ignore
             name=DATA_SETTINGS.sample_index_name,
             nullable=DATA_SETTINGS.sample_index_nullable,
-            coerce=False,
             unique=DATA_SETTINGS.sample_index_unique,
+            checks_list=[pandera_utils.checks.configurable.index_satisfies_dtypes(DATA_SETTINGS.sample_index_dtypes)],
         )
         self._data = schema.validate(data)
 
         logger.debug(f"Final schema:\n{schema}")
         self._schema = schema
 
     @staticmethod
@@ -706,60 +620,32 @@
         return self._data.shape[0]
 
     @property
     def num_features(self) -> int:
         return self._data.shape[1]
 
     @pydantic.validate_arguments(config={"arbitrary_types_allowed": True})
-    def split(self, time_feature_suffix: str = _DEFAULT_EVENTS_TIME_FEATURE_SUFFIX) -> pd.DataFrame:
+    def split(self, time_feature_suffix: str = "_time") -> pd.DataFrame:
         """Return a `pandas.DataFrame` where the time component of each event feature has been split off to its own
-        column. The new columns that contain the times will be named ``"<original column name><time_feature_suffix>"``
-        and will be inserted before each corresponding ``<original column name>`` column. The ``<original column name>``
+        column. The new columns that contain the times will be named `"<original column name><time_feature_suffix>"`
+        and will be inserted before each corresponding `<original column name>` column. The `<original column name>`
         columns will contain only the event value.
 
         Args:
-            time_feature_suffix (str, optional):
-                A column name suffix string to identify the time columns that will be split off. Defaults to
-                ``"_time"``.
+            time_feature_suffix (str, optional): A column name suffix string to identify the time columns that will be
+            split off. Defaults to `"_time"`.
 
         Returns:
             pd.DataFrame: The output dataframe.
         """
         df = self._data.copy()
         features = list(df.columns)
         if any(time_feature_suffix in str(c) for c in features):
             raise ValueError(f"Column names must not contain '{time_feature_suffix}'")
         for f_idx, f in enumerate(features):
             df.insert(f_idx * 2, f"{f}{time_feature_suffix}", df[f].apply(lambda x: x[0]))
         for f in features:
             df[f] = df[f].apply(lambda x: x[1])
         return df
 
-    def split_as_two_dataframes(
-        self, time_feature_suffix: str = _DEFAULT_EVENTS_TIME_FEATURE_SUFFIX
-    ) -> Tuple[pd.DataFrame, pd.DataFrame]:
-        """Analogous to :func:`~tempor.data.samples.EventSamples.split` but returns two `pandas.DataFrame` s:
-            - first dataframe contains the event times of each feature.
-            - second dataframe contains the event values (`True`/`False`) of each feature.
-
-        Args:
-            time_feature_suffix (str, optional):
-                A column name suffix string to identify the time columns that will be split off. Defaults to
-                ``"_time"``.
-
-        Returns:
-            Tuple[pd.DataFrame, pd.DataFrame]: Two `pandas.DataFrame` s containing event times and values respectively.
-        """
-        df_split = self.split(time_feature_suffix=time_feature_suffix)
-        df_event_times = df_split.loc[:, [c for c in df_split.columns if time_feature_suffix in c]]
-        df_event_values = df_split.loc[:, [c for c in df_split.columns if time_feature_suffix not in c]]
-        return df_event_times, df_event_values
-
     def short_repr(self) -> str:
         return f"{self.__class__.__name__}([{self.num_samples}, {self.num_features}])"
-
-    def __getitem__(self, key: data_typing.GetItemKey) -> Self:
-        key_ = utils.ensure_pd_iloc_key_returns_df(key)
-        return EventSamples(  # type: ignore[return-value]
-            self._data.iloc[key_, :],  # pyright: ignore
-            _skip_validate=True,
-        )
```

## tempor/data/settings.py

```diff
@@ -1,8 +1,9 @@
-"""Settings for TemporAI data handling."""
+"""Settings for TemporAI data handling.
+"""
 
 from typing import ClassVar, List
 
 import pydantic
 
 from . import data_typing
```

## tempor/data/utils.py

```diff
@@ -1,19 +1,16 @@
 import dataclasses
 import itertools
-from typing import Any, ClassVar, List, Optional, Sequence, Tuple, Union
+from typing import Any, ClassVar, List, Optional
 
 import numpy as np
 import pandas as pd
 import pydantic
-from packaging.version import Version
 
-import tempor.core.utils
-
-from . import data_typing, settings
+from . import data_typing
 
 
 @dataclasses.dataclass(frozen=True)
 class _ExceptionMessages:
     expected_array1d: ClassVar[str] = "Expected 1d array"
     expected_array2d: ClassVar[str] = "Expected 2d array"
     expected_array3d: ClassVar[str] = "Expected 3d array"
@@ -21,92 +18,74 @@
     padding_indicator_nan_not_supported: ClassVar[str] = "Padding indicator of `numpy.nan` is not supported"
 
 
 EXCEPTION_MESSAGES = _ExceptionMessages()
 """Reusable error messages for the module."""
 
 
-def value_in_df(df: pd.DataFrame, *, value: Any) -> bool:
-    """Check if ``value`` exists in dataframe ``df``, accounting for the case where ``value`` is `numpy.nan`."""
-    return (pd.isnull(value) and df.isna().any().any()) or (df == value).any().any()
-
-
-def set_df_column_names_inplace(df: pd.DataFrame, names: Sequence) -> pd.DataFrame:
-    if Version(pd.__version__) < Version("1.5"):
-        df.set_axis(names, axis="columns", inplace=True)  # pyright: ignore
-        return df
-    else:
-        return df.set_axis(names, axis="columns", copy=False)
-
-
-def get_df_index_level0_unique(df: pd.DataFrame) -> pd.Index:
-    return df.index.get_level_values(level=0).unique()
+# --- Multiindex timeseries dataframe --> 3D numpy array. ---
 
 
-# --- Multiindex timeseries dataframe --> 3D numpy array. ---
+def value_in_df(df: pd.DataFrame, *, value: Any) -> bool:
+    """Check if `value` exists in dataframe `df`, accounting for the case where `value` is `nan`."""
+    return (pd.isnull(value) and df.isna().any().any()) or (df == value).any().any()
 
 
 @pydantic.validate_arguments(config={"arbitrary_types_allowed": True, "smart_union": True})
 def multiindex_timeseries_dataframe_to_array3d(
     df: pd.DataFrame, *, padding_indicator: Any, max_timesteps: Optional[int] = None
 ) -> np.ndarray:
-    """Convert timeseries dataframe ``df`` with a 2-level multiindex (sample, timestep) to a 3D numpy array with
-    dimensions ``(sample, timestep, feature)``.
+    """Convert timeseries dataframe `df` with a 2-level multiindex (sample, timestep) to a 3D numpy array with
+    dimensions `(sample, timestep, feature)`.
 
     Args:
-        df (pd.DataFrame):
-            Input dataframe.
-        padding_indicator (Any):
-            padding indicator value to use to pad the output array in case of unequal number of timesteps for
-            different samples.
-        max_timesteps (int, optional):
-            Maximum number of timesteps to use. This will become the size of the dim 1 of the output array. If set to
-            `None`, this dimension will be set as the highest number of timesteps among the samples. Defaults to `None`.
+        df (pd.DataFrame): Input dataframe
+        padding_indicator (Any): padding indicator value to use to pad the output array in case of unequal number of
+        timesteps for different samples.
+        max_timesteps (int, optional): Maximum number of timesteps to use. This will become the size of the dim 1 of the
+        output array. If set to `None`, this dimension will be set as the highest number of timesteps among the samples.
+        Defaults to None.
 
     Raises:
-        ValueError: raised if the ``padding_indicator`` found as one of the data values in ``df``.
+        ValueError: raised if the `padding_indicator` found as one of the data values in `df`.
 
     Returns:
         np.ndarray: Output 3D numpy array.
     """
     if value_in_df(df, value=padding_indicator):
         raise ValueError(f"Value `{padding_indicator}` found in data frame, choose a different padding indicator")
-    samples = get_df_index_level0_unique(df)
+    samples = df.index.get_level_values(level=0).unique()
     num_samples = len(samples)
     num_features = len(df.columns)
     num_timesteps_per_sample = df.groupby(level=0).size()
     max_actual_timesteps = num_timesteps_per_sample.max()
     max_timesteps = max_actual_timesteps if max_timesteps is None else max_timesteps
     array = np.full(shape=(num_samples, max_timesteps, num_features), fill_value=padding_indicator)
     for i_sample, idx_sample in enumerate(samples):
         set_vals = df.loc[idx_sample, :, :].to_numpy()[:max_timesteps, :]  # pyright: ignore
-        if i_sample == 0:
-            array = array.astype(set_vals.dtype)  # Need to cast to the type matching source data.
         array[i_sample, : num_timesteps_per_sample[idx_sample], :] = set_vals  # pyright: ignore
     return array
 
 
 # --- 3D numpy array --> Multiindex timeseries dataframe. ---
 
 
 def check_bool_array1d_trues_consecutive(array: np.ndarray, at_beginning: bool = False, at_end: bool = False) -> bool:
-    """Check if 1D ``array`` (containing `bool` values) has all `True` elements consecutively. If ``at_{beginning,end}``
-    is set, will also check that a `True` element is present as the first or last element of the ``array``,
-    respectively. Raises `ValueError` if input `array` format is unexpected.
+    """Check if 1D `array` (containing `bool` values) has all `True` elements consecutively. If `at_{beginning,end}` is
+    set, will also check that a `True` element is present as the first or last element of the `array`, respectively.
+    Raises `ValueError` if input `array` format is unexpected.
 
     Examples:
-        >>> import numpy as np
-        >>> from tempor.data.utils import *
-        >>>
-        >>> check_bool_array1d_trues_consecutive(np.asarray([False, True, True, True, False]))
-        True
-        >>> check_bool_array1d_trues_consecutive(np.asarray([False, True, False, True, False]))
-        False
-        >>> check_bool_array1d_trues_consecutive(np.asarray([False, True, True, True]), at_end=True)
-        True
+    >>> import numpy as np
+    >>> check_bool_array1d_trues_consecutive(np.asarray([False, True, True, True, False]))
+    True
+    >>> check_bool_array1d_trues_consecutive(np.asarray([False, True, False, True, False]))
+    False
+    >>> check_bool_array1d_trues_consecutive(np.asarray([False, True, True, True]), at_end=True)
+    True
     """
     if array.ndim != 1:
         raise ValueError(EXCEPTION_MESSAGES.expected_array1d)
     if array.dtype != bool:
         raise ValueError(EXCEPTION_MESSAGES.expected_array_dtype_bool)
     if len(array) == 0:
         return True
@@ -121,98 +100,92 @@
             check_passed = check_passed and 0 in true_idxs
         if at_end:
             check_passed = check_passed and (len(array) - 1) in true_idxs
         return check_passed
 
 
 def check_bool_array2d_identical_along_dim1(array: np.ndarray) -> bool:
-    """Check if 2D ``array`` (containing `bool` values) has the same values along dimension 1.
+    """Check if 2D `array` (containing `bool` values) has the same values along dimension 1.
 
     Examples:
-        >>> import numpy as np
-        >>> from tempor.data.utils import *
-        >>>
-        >>> check_bool_array2d_identical_along_dim1(np.asarray([[True, True, False], [True, True, False]]).T)
-        True
-        >>> check_bool_array2d_identical_along_dim1(np.asarray([[True, True, False], [False, True, False]]).T)
-        False
+    >>> import numpy as np
+    >>> check_bool_array2d_identical_along_dim1(np.asarray([[True, True, False], [True, True, False]]).T)
+    True
+    >>> check_bool_array2d_identical_along_dim1(np.asarray([[True, True, False], [False, True, False]]).T)
+    False
     """
     if array.ndim != 2:
         raise ValueError(EXCEPTION_MESSAGES.expected_array2d)
     if array.dtype != bool:
         raise ValueError(EXCEPTION_MESSAGES.expected_array_dtype_bool)
     return (np.diff(array.astype(int), axis=1) == 0).all()
 
 
 def get_array1d_length_until_padding(array: np.ndarray, padding_indicator: Any = None) -> int:
-    """Get the length of 1D ``array`` up to first padding indicated by ``padding_indicator``. Raises `ValueError` if
-    input ``array`` format is unexpected.
+    """Get the length of 1D `array` up to first padding indicated by `padding_indicator`. Raises `ValueError` if input
+    `array` format is unexpected.
 
     Examples:
-        >>> import numpy as np
-        >>> from tempor.data.utils import *
-        >>>
-        >>> pad = 999.0
-        >>> get_array1d_length_until_padding(np.asarray([1, 8, -3, 9, pad]), padding_indicator=pad)
-        4
-        >>> get_array1d_length_until_padding(np.asarray([1, 8, -3, 9, 5]), padding_indicator=pad)
-        5
+    >>> import numpy as np
+    >>> pad = 999.0
+    >>> get_array1d_length_until_padding(np.asarray([1, 8, -3, 9, pad]), padding_indicator=pad)
+    4
+    >>> get_array1d_length_until_padding(np.asarray([1, 8, -3, 9, 5]), padding_indicator=pad)
+    5
     """
     if array.ndim != 1:
         raise ValueError(EXCEPTION_MESSAGES.expected_array1d)
     if np.isnan(padding_indicator):
         raise ValueError(EXCEPTION_MESSAGES.padding_indicator_nan_not_supported)
     array_padding = array == padding_indicator
     positions = np.where(array_padding)[0]
     if len(positions) != 0:
         return positions[0]
     else:
         return len(array)
 
 
 def validate_timeseries_array3d(array: np.ndarray, padding_indicator: Any = None):
-    """Check if 3D ``array`` representing timeseries satisfies the blow criteria, otherwise raise `ValueError`:
+    """Check if 3D `array` representing timeseries satisfies the blow criteria, otherwise raise ValueError:
     - 3 dimensions,
     - Dimension 2 not of size 0,
-    - If ``padding_indicator`` is provided, also check it is not `np.nan`, as this is not supported.
+    - If `padding_indicator` is provided, also check it is not `np.nan`, as this is not supported.
     """
     if array.ndim != 3:
         raise ValueError(EXCEPTION_MESSAGES.expected_array3d)
     if array.shape[2] == 0:
         raise ValueError("Dim 2 (-1) is the feature dimension and must not be of size 0")
     if padding_indicator is not None and np.isnan(padding_indicator):
         raise ValueError(EXCEPTION_MESSAGES.padding_indicator_nan_not_supported)
 
 
 def get_seq_lengths_timeseries_array3d(array: np.ndarray, padding_indicator: Any = None) -> List[int]:
-    """Given a 3D numpy ``array`` that represents timeseries like ``(sample, timestep, feature)``, and optionally a
-    ``padding_indicator`` to indicate padding, get the length (number of [non-padding] timesteps) for each sample.
+    """Given a 3D numpy `array` that represents timeseries like `(sample, timestep, feature)`, and optionally a
+    `padding_indicator` to indicate padding, get the length (number of [non-padding] timesteps) for each sample.
 
     Example:
-        >>> import numpy as np
-        >>> from tempor.data.utils import *
-        >>>
-        >>> pad = 999.0
-        >>> array = np.asarray(  # Array with two samples, with two timeseries features.
-        ...     [
-        ...         # Sample 1:
-        ...         [
-        ...             [11, 12, 13, 14, pad],
-        ...             [1.1, 1.2, 1.3, 1.4, pad],
-        ...         ],
-        ...         # Sample 2:
-        ...         [
-        ...             [21, 22, pad, pad, pad],
-        ...             [2.1, 2.2, pad, pad, pad],
-        ...         ],
-        ...     ]
-        ... )
-        >>> array = np.transpose(array, (0, 2, 1))
-        >>> get_seq_lengths_timeseries_array3d(array, padding_indicator=pad)
-        [4, 2]
+    >>> import numpy as np
+    >>> pad = 999.0
+    >>> array = np.asarray(  # Array with two samples, with two timeseries features.
+    ...     [
+    ...         # Sample 1:
+    ...         [
+    ...             [11, 12, 13, 14, pad],
+    ...             [1.1, 1.2, 1.3, 1.4, pad],
+    ...         ],
+    ...         # Sample 2:
+    ...         [
+    ...             [21, 22, pad, pad, pad],
+    ...             [2.1, 2.2, pad, pad, pad],
+    ...         ],
+    ...     ]
+    ... )
+    >>> array = np.transpose(array, (0, 2, 1))
+    >>> get_seq_lengths_timeseries_array3d(array, padding_indicator=pad)
+    [4, 2]
     """
     validate_timeseries_array3d(array, padding_indicator)
     is_padded = padding_indicator is not None
     if is_padded:
         lengths = []
         for array_sample in array:
             array_sample_padding = array_sample == padding_indicator
@@ -231,44 +204,42 @@
             lengths.append(n_timesteps)
         return lengths
     else:
         return [array.shape[1]] * array.shape[0]
 
 
 def unpad_timeseries_array3d(array: np.ndarray, padding_indicator: Any) -> List[np.ndarray]:
-    """Given a 3D numpy ``array`` that represents timeseries like ``(sample, timestep, feature)``, and optionally a
-    ``padding_indicator`` to indicate padding, return a list of length ``num_samples``, which contains arrays for each
-    sample like ``(timestep, feature)``, with the padding removed.
+    """Given a 3D numpy `array` that represents timeseries like `(sample, timestep, feature)`, and optionally a
+    `padding_indicator` to indicate padding, return a list of length `num_samples`, which contains arrays for each sample
+    like `(timestep, feature)`, with the padding removed.
     """
     validate_timeseries_array3d(array, padding_indicator)
     lengths = get_seq_lengths_timeseries_array3d(array, padding_indicator)
     arrays_unpadded = []
     for sample_i, length in enumerate(lengths):
         arrays_unpadded.append(array[sample_i, :length, :])
     return arrays_unpadded
 
 
 def make_sample_time_index_tuples(
     sample_index: data_typing.SampleIndex, time_indexes: data_typing.TimeIndexList
 ) -> data_typing.SampleTimeIndexTuples:
-    """Given a list of elements ``sample_index`` representing sample IDs and a list (of same length) of lists each
+    """Given a list of elements `sample_index` representing sample IDs and a list (of same length) of lists each
     representing the timesteps for the corresponding sample, return a list of tuples like
-    ``[(<sample ID>, <timestep>), ...]``.
+    `[(<sample ID>, <timestep>), ...]`.
 
     Example:
-        >>> from tempor.data.utils import *
-        >>>
-        >>> sample_index = ["s1", "s2"]
-        >>> time_indexes = [[1, 2, 3], [1, 5, 9, 10]]
-        >>> make_sample_time_index_tuples(sample_index, time_indexes)
-        [('s1', 1), ('s1', 2), ('s1', 3), ('s2', 1), ('s2', 5), ('s2', 9), ('s2', 10)]
+    >>> sample_index = ["s1", "s2"]
+    >>> time_indexes = [[1, 2, 3], [1, 5, 9, 10]]
+    >>> make_sample_time_index_tuples(sample_index, time_indexes)
+    [('s1', 1), ('s1', 2), ('s1', 3), ('s2', 1), ('s2', 5), ('s2', 9), ('s2', 10)]
     """
     if len(sample_index) != len(time_indexes):
         raise ValueError("Expected the same number of elements in `sample_index` and `time_indexes`")
-    sample_indexes_copied = [[si] * len(tis) for si, tis in zip(sample_index, time_indexes)]  # type: ignore[arg-type]
+    sample_indexes_copied = [[si] * len(tis) for si, tis in zip(sample_index, time_indexes)]
     sample_indexes_flattened = list(itertools.chain.from_iterable(sample_indexes_copied))
     time_indexes_flattened = list(itertools.chain.from_iterable(time_indexes))
     pairs = [(si, ti) for si, ti in zip(sample_indexes_flattened, time_indexes_flattened)]
     return pairs  # type: ignore
 
 
 @pydantic.validate_arguments(config={"arbitrary_types_allowed": True, "smart_union": True})
@@ -276,184 +247,37 @@
     array: np.ndarray,
     *,
     sample_index: data_typing.SampleIndex,
     time_indexes: data_typing.TimeIndexList,
     feature_index: data_typing.FeatureIndex,
     padding_indicator: Any = None,
 ) -> pd.DataFrame:
-    """Given a 3D timeseries ``array``, ``sample_index``, ``time_indexes``, ``feature_index``, and a
-    ``padding_indicator``, build a 2-level multiindex (sample, timestep) `pandas.DataFrame`.
+    """Given a 3D timeseries `array`, `sample_index`, `time_indexes`, `feature_index`, and a `padding_indicator`, build
+    a 2-level multiindex (sample, timestep) `pandas.DataFrame`.
 
-    Padding values of ``padding_indicator`` can be set inside the array to pad out the length of arrays of different
+    Padding values of `padding_indicator` can be set inside the array to pad out the length of arrays of different
     samples in case they differ. Padding needs to go at the end of the timesteps (dim 1). Padding must be the same
     across the feature dimension (dim 2) for each sample.
 
     Raises:
         ValueError: if data or padding format is unexpected.
 
     Args:
-        array (np.ndarray):
-            3D numpy `array` that represents timeseries like ``(sample, timestep, feature)``.
-        sample_index (List[<sample element>):
-            List of sample IDs (should be the same length as dim 0 of `array`).
-        time_indexes (List[List[<timestep element>]]):
-            List of lists containing timesteps for each sample (outer list should be the same length as dim 0 of
-            `array`, inner list should contain as many elements as each sample has timesteps).
-        feature_index (List[<feature element>]):
-            List of feature names.
-        padding_indicator (Any, optional):
-            Padding indicator used in `array` to indicate padding. Defaults to None.
+        array (np.ndarray): 3D numpy `array` that represents timeseries like `(sample, timestep, feature)`.
+        sample_index (List[<sample element>): List of sample IDs (should be the same length as dim 0 of `array`).
+        time_indexes (List[List[<timestep element>]]): List of lists containing timesteps for each sample (outer list
+        should be the same length as dim 0 of `array`, inner list should contain as many elements as each sample has
+        timesteps).
+        feature_index (List[<feature element>]): List of feature names.
+        padding_indicator (Any, optional): Padding indicator used in `array` to indicate padding. Defaults to None.
 
     Returns:
         pd.DataFrame: Resultant dataframe.
     """
     validate_timeseries_array3d(array, padding_indicator)
     unpadded_arrays = unpad_timeseries_array3d(array, padding_indicator)
     data = np.concatenate(unpadded_arrays)
     return pd.DataFrame(
         data,
         index=pd.MultiIndex.from_tuples(make_sample_time_index_tuples(sample_index, time_indexes)),
         columns=feature_index,
     )
-
-
-# --- List of dataframes --> Multiindex timeseries dataframe. ---
-
-
-@pydantic.validate_arguments(config={"arbitrary_types_allowed": True, "smart_union": True})
-def list_of_dataframes_to_multiindex_timeseries_dataframe(
-    list_of_dataframes: List[pd.DataFrame],
-    *,
-    sample_index: data_typing.SampleIndex,
-    time_indexes: Optional[data_typing.TimeIndexList] = None,
-    feature_index: Optional[data_typing.FeatureIndex] = None,
-) -> pd.DataFrame:
-    dfs: List[pd.DataFrame] = list_of_dataframes
-
-    if time_indexes is not None and len(list_of_dataframes) != len(time_indexes):
-        raise ValueError(
-            "Expected `list_of_dataframes` and `time_indexes` to be of same length but was "
-            f"{len(list_of_dataframes)} and {len(time_indexes)} respectively"
-        )
-
-    if time_indexes is not None:
-        for idx, df in enumerate(list_of_dataframes):
-            dfs[idx] = df.set_index(
-                keys=pd.Index(time_indexes[idx], name=df.index.name),  # pyright: ignore
-                drop=True,
-                verify_integrity=True,
-            )
-    else:
-        time_indexes = [list(df.index) for df in dfs]
-
-    df_concat = pd.concat(dfs, axis=0, ignore_index=False)
-
-    multiindex = pd.MultiIndex.from_tuples(make_sample_time_index_tuples(sample_index, time_indexes))
-    df_concat.set_index(
-        keys=multiindex,
-        drop=True,
-        verify_integrity=True,
-        inplace=True,  # pyright: ignore
-    )
-    df_concat.index.set_names(
-        [settings.DATA_SETTINGS.sample_index_name, settings.DATA_SETTINGS.time_index_name], inplace=True
-    )
-    if feature_index is not None:
-        df_concat = set_df_column_names_inplace(df_concat, feature_index)
-
-    return df_concat
-
-
-def multiindex_timeseries_dataframe_to_list_of_dataframes(df: pd.DataFrame) -> List[pd.DataFrame]:
-    """Returns a list of dataframes where each dataframe has the data for each sample. That is, each of the dataframes
-    has a unique level ``0`` index value.
-
-    Args:
-        df (pd.DataFrame): Input multiindex dataframe.
-
-    Returns:
-        List[pd.DataFrame]: Output list of dataframes.
-    """
-    sample_index = get_df_index_level0_unique(df)
-    return [df.loc[(si, slice(None)), :] for si in sample_index]
-
-
-# --- [(event_times, event_values), ...] --> DataFrame compatible with EventSamples. ---
-
-
-@pydantic.validate_arguments(config={"arbitrary_types_allowed": False, "smart_union": True})
-def event_time_value_pairs_to_event_dataframe(
-    event_time_value_pairs: Sequence[Tuple[data_typing.TimeIndex, List[bool]]],
-    sample_index: data_typing.SampleIndex,
-    feature_index: Optional[data_typing.FeatureIndex] = None,
-) -> pd.DataFrame:
-    """Convert a sequence like ``[(event_times, event_values), ...]`` to a `pandas.DataFrame` whose columns contain
-    elements like tuples ``(event_time, event_value)``.
-
-    Args:
-        event_time_value_pairs (Sequence[Tuple[data_typing.TimeIndex, List[bool]]]):
-            A sequence where each item corresponds to an event feature and is a tuple of form
-            ``(event_times, event_values)`` (e.g. ``([1.1, 1.2, 1.3], [True, True, False])``).
-        sample_index (data_typing.SampleIndex):
-            List of sample IDs, to be set as dataframe row index.
-        feature_index (Optional[data_typing.FeatureIndex]):
-            List of feature names, to be set as dataframe column names.
-
-    Example:
-        >>> from tempor.data.utils import *
-        >>>
-        >>> sample_index = ["s1", "s2", "s3"]
-        >>> feature_names = ["feature_1", "feature_2"]
-        >>> event_feature_1 = ([1.1, 1.2, 1.3], [True, True, False])
-        >>> event_feature_2 = ([2.1, 2.2, 2.3], [False, True, False])
-        >>> event_time_value_pairs = [event_feature_1, event_feature_2]
-        >>> df = event_time_value_pairs_to_event_dataframe(
-        ...     event_time_value_pairs, sample_index=sample_index, feature_index=feature_names
-        ... )
-        >>> df.shape
-        (3, 2)
-
-    Returns:
-        pd.DataFrame: `pandas.DataFrame` compatible with `EventSamples`.
-    """
-    series_list = [pd.Series(zip(t, v)) for t, v in event_time_value_pairs]
-    data_input = pd.DataFrame(data=series_list).T.to_numpy()
-    df = pd.DataFrame(data=data_input, index=sample_index)
-    if feature_index is not None:
-        df = set_df_column_names_inplace(df, feature_index)
-    return df
-
-
-# --- Date-time time index -related ---
-
-
-@pydantic.validate_arguments(config={"arbitrary_types_allowed": True, "smart_union": True})
-def datetime_time_index_to_float(time_index: Union[data_typing.TimeIndex, pd.Index, pd.Series]) -> np.ndarray:
-    """Convert a date-time ``time_index`` to floats. The conversion is done by calling
-    ``<time_index as a numpy array>.astype(float)``.
-
-    Args:
-        time_index (Union[data_typing.TimeIndex, pd.Index, pd.Series]):
-            The input time index.
-
-    Returns:
-        np.ndarray:
-            NumPy array containing the time index converted to `float` s.
-    """
-    if isinstance(time_index, (pd.Index, pd.Series)):
-        time_index_pd_type = time_index
-    else:
-        time_index_pd_type = pd.Series(time_index)
-    return time_index_pd_type.to_numpy().astype(float)
-
-
-# --- Miscellaneous. ---
-
-
-def ensure_pd_iloc_key_returns_df(key):
-    if isinstance(key, slice):
-        key_: Any = key
-    elif tempor.core.utils.is_iterable(key):
-        key_ = key
-    else:
-        key_ = [key]
-    return key_
```

## tempor/exc/__init__.py

```diff
@@ -1,10 +1,2 @@
 class DataValidationException(ValueError):
     pass
-
-
-class UnsupportedSetupException(RuntimeError):
-    """Raise this exception when an TemporAI estimator (model) encounters an unsupported situation,
-    e.g. incompatible data format.
-    """
-
-    pass  # pylint: disable=unnecessary-pass
```

## tempor/log/_custom_logger.py

```diff
@@ -1,14 +1,13 @@
 import logging
 import os
 import sys
-from typing import Any, Callable, Dict, Union
+from typing import Any, Callable, Dict, Literal, Union
 
 from loguru import logger
-from typing_extensions import Literal
 
 import tempor.config as conf
 
 _LogFormatType = Literal["print-like", "log-like"]
 
 logger.level("INFO", color="")  # Make INFO level format not bold.
```

## tempor/plugins/_plugin_loader.py

```diff
@@ -1,13 +1,10 @@
 import tempor.plugins.core as plugins
 
-from . import prediction, preprocessing, time_to_event, treatments
+from . import preprocessing
 
 plugin_loader = plugins.PluginLoader()
 
 
 __all__ = [
-    "prediction",
     "preprocessing",
-    "time_to_event",
-    "treatments",
 ]
```

## tempor/plugins/core/_base_estimator.py

```diff
@@ -1,31 +1,30 @@
 import abc
 import dataclasses
 from typing import TYPE_CHECKING, Any, ClassVar, Dict, List, Optional, Type
 
 import omegaconf
 import pydantic
 import rich.pretty
-from typing_extensions import Self
 
-from tempor.core import pydantic_utils, utils
+import tempor.core.utils
 from tempor.data import dataset
 from tempor.log import logger
 
 from ._params import Params
 from ._plugin import Plugin
 
 
 @dataclasses.dataclass
 class EmptyParamsDefinition:
     pass
 
 
 class BaseEstimator(Plugin, abc.ABC):
-    ParamsDefinition: ClassVar[Type] = EmptyParamsDefinition
+    PARAMS_DEFINITION: ClassVar[Type] = EmptyParamsDefinition
     _fitted: bool
 
     class _InitArgsValidator(pydantic.BaseModel):
         params: Optional[Dict[str, Any]]
         ParamsDefinitionClass: Type
 
         # Output:
@@ -36,36 +35,35 @@
             params = values.get("params", dict())
             ParamsDefinitionClass = values.get("ParamsDefinitionClass")
 
             if TYPE_CHECKING:  # pragma: no cover
                 assert ParamsDefinitionClass is not None  # nosec B101
 
             try:
-                if not pydantic_utils.is_pydantic_dataclass(ParamsDefinitionClass):
-                    ParamsDefinitionClass = pydantic_utils.make_pydantic_dataclass(ParamsDefinitionClass)
-                defined_params = omegaconf.OmegaConf.structured(dataclasses.asdict(ParamsDefinitionClass(**params)))
+                defined_params = omegaconf.OmegaConf.structured(ParamsDefinitionClass(**params))
             except Exception as ex:
-                name = utils.get_class_full_name(ex)
+                name = tempor.core.utils.get_class_full_name(ex)
                 sep = "\n" + "-" * (len(name) + 1) + "\n"
                 raise ValueError(
-                    f"Model parameters could not be validated as defined by `{ParamsDefinitionClass.__name__}`, "
-                    f"cause: {sep}{name}:\n{ex}{sep}"
+                    "Model parameters could not be converted to OmegaConf Structured Config "
+                    f"as defined by `{ParamsDefinitionClass.__name__}`, cause: {sep}{name}:\n{ex}{sep}"
                 ) from ex
 
             values["params_processed"] = defined_params
             return values
 
         class Config:
             arbitrary_types_allowed = True
 
     def __init__(self, **params) -> None:
         Plugin.__init__(self)
         self._fitted = False
-        args_validator = self._InitArgsValidator(params=params, ParamsDefinitionClass=self.ParamsDefinition)
+        args_validator = self._InitArgsValidator(params=params, ParamsDefinitionClass=self.PARAMS_DEFINITION)
         params_processed = args_validator.params_processed
+        print(params_processed)
         if TYPE_CHECKING:  # pragma: no cover
             assert isinstance(params_processed, omegaconf.DictConfig)  # nosec B101
         self.params = params_processed
 
     @property
     def is_fitted(self) -> bool:
         """Check if the model was trained"""
@@ -75,46 +73,40 @@
         yield "name", self.name
         yield "category", self.category
         yield "params", omegaconf.OmegaConf.to_container(self.params)
 
     def __repr__(self) -> str:
         return rich.pretty.pretty_repr(self)
 
-    @pydantic.validate_arguments(config=dict(arbitrary_types_allowed=True))
     def fit(
         self,
-        data: dataset.BaseDataset,
+        data: dataset.Dataset,
         *args,
         **kwargs,
-    ) -> Self:
-        if not data.fit_ready:
-            raise ValueError(
-                f"The dataset was not fit-ready, check that all necessary data components are present:\n{data}"
-            )
-
+    ) -> "BaseEstimator":
         logger.debug(f"Calling _fit() implementation on {self.__class__.__name__}")
         fitted_model = self._fit(data, *args, **kwargs)
 
         self._fitted = True
         return fitted_model
 
     @abc.abstractmethod
-    def _fit(self, data: dataset.BaseDataset, *args, **kwargs) -> Self:
+    def _fit(self, data: dataset.Dataset, *args, **kwargs) -> "BaseEstimator":  # pragma: no cover
         ...
 
     @staticmethod
     @abc.abstractmethod
     def hyperparameter_space(*args: Any, **kwargs: Any) -> List[Params]:  # pragma: no cover
         """The hyperparameter search domain, used for tuning."""
         ...  # pylint: disable=unnecessary-ellipsis
 
     @classmethod
-    def sample_hyperparameters(cls, *args: Any, **kwargs: Any) -> Dict[str, Any]:
+    def sample_hyperparameters(cls, trial: Any, *args: Any, **kwargs: Any) -> Dict[str, Any]:
         """Sample hyperparameters."""
         param_space = cls.hyperparameter_space(*args, **kwargs)
 
         results = {}
 
         for hp in param_space:
-            results[hp.name] = hp.sample()
+            results[hp.name] = hp.sample(trial)
 
         return results
```

## tempor/plugins/core/_base_predictor.py

```diff
@@ -1,82 +1,36 @@
 import abc
 from typing import Any
 
-import pydantic
-
 from tempor.data import dataset
 from tempor.log import logger
 
 from . import _base_estimator as estimator
 
 
 class BasePredictor(estimator.BaseEstimator):
     def __init__(self, **params) -> None:  # pylint: disable=useless-super-delegation
         super().__init__(**params)
 
     def predict(
         self,
-        data: dataset.PredictiveDataset,
+        data: dataset.Dataset,
         *args,
         **kwargs,
     ) -> Any:  # TODO: Narrow down output formats later.
-        if not data.predict_ready:
-            raise ValueError(
-                f"The dataset was not predict-ready, check that all necessary data components are present:\n{data}"
-            )
-
         logger.debug(f"Calling _predict() implementation on {self.__class__.__name__}")
         prediction = self._predict(data, *args, **kwargs)
 
         return prediction
 
-    def predict_proba(
-        self,
-        data: dataset.PredictiveDataset,
-        *args,
-        **kwargs,
-    ) -> Any:  # TODO: Narrow down output formats later.
-        if not data.predict_ready:
-            raise ValueError(
-                f"The dataset was not predict-ready, check that all necessary data components are present:\n{data}"
-            )
-
-        logger.debug(f"Calling _predict_proba() implementation on {self.__class__.__name__}")
-        prediction = self._predict_proba(data, *args, **kwargs)
-
-        return prediction
-
-    def predict_counterfactuals(
-        self,
-        data: dataset.PredictiveDataset,
-        *args,
-        **kwargs,
-    ) -> Any:  # TODO: Narrow down output formats later.
-        if not data.predict_ready:
-            raise ValueError(
-                f"The dataset was not predict-ready, check that all necessary data components are present:\n{data}"
-            )
-
-        logger.debug(f"Calling _predict_counterfactuals() implementation on {self.__class__.__name__}")
-        prediction = self._predict_counterfactuals(data, *args, **kwargs)
-
-        return prediction
-
-    @pydantic.validate_arguments(config=dict(arbitrary_types_allowed=True))
     def fit_predict(
         self,
-        data: dataset.PredictiveDataset,
+        data: dataset.Dataset,
         *args,
         **kwargs,
     ) -> Any:
         self.fit(data, *args, **kwargs)
         return self.predict(data, *args, **kwargs)
 
     @abc.abstractmethod
-    def _predict(self, data: dataset.PredictiveDataset, *args, **kwargs) -> Any:  # pragma: no cover
+    def _predict(self, data: dataset.Dataset, *args, **kwargs) -> Any:  # pragma: no cover
         ...
-
-    def _predict_proba(self, data: dataset.PredictiveDataset, *args, **kwargs) -> Any:
-        raise NotImplementedError("`predict_proba` is supported only for classification tasks")
-
-    def _predict_counterfactuals(self, data: dataset.PredictiveDataset, *args, **kwargs) -> Any:
-        raise NotImplementedError("`predict_counterfactuals` is supported only for treatments tasks")
```

## tempor/plugins/core/_base_transformer.py

```diff
@@ -1,39 +1,36 @@
 import abc
 from typing import Any
 
-import pydantic
-
 from tempor.data import dataset
 from tempor.log import logger
 
 from . import _base_estimator as estimator
 
 
 class BaseTransformer(estimator.BaseEstimator):
     def __init__(self, **params) -> None:  # pylint: disable=useless-super-delegation
         super().__init__(**params)
 
     def transform(
         self,
-        data: dataset.BaseDataset,
+        data: dataset.Dataset,
         *args,
         **kwargs,
     ) -> Any:
         logger.debug(f"Calling _transform() implementation on {self.__class__.__name__}")
         transformed_data = self._transform(data, *args, **kwargs)
 
         return transformed_data
 
-    @pydantic.validate_arguments(config=dict(arbitrary_types_allowed=True))
     def fit_transform(
         self,
-        data: dataset.BaseDataset,
+        data: dataset.Dataset,
         *args,
         **kwargs,
-    ) -> dataset.BaseDataset:
+    ) -> Any:
         self.fit(data, *args, **kwargs)
         return self.transform(data, *args, **kwargs)
 
     @abc.abstractmethod
-    def _transform(self, data: dataset.BaseDataset, *args, **kwargs) -> dataset.BaseDataset:  # pragma: no cover
+    def _transform(self, data: dataset.Dataset, *args, **kwargs) -> Any:  # pragma: no cover
         ...
```

## tempor/plugins/core/_params.py

```diff
@@ -1,77 +1,20 @@
 import abc
-import random
 from typing import Any, List, Tuple
 
 
 class Params(abc.ABC):
-    """Helper for describing the hyperparameters for each estimator."""
+    """
+    Helper for describing the hyperparameters for each estimator.
+    """
 
     def __init__(self, name: str, bounds: Tuple[Any, Any]) -> None:
         self.name = name
         self.bounds = bounds
 
     @abc.abstractmethod
     def get(self) -> List[Any]:
         ...
 
     @abc.abstractmethod
-    def sample(self) -> Any:
+    def sample(self, trial: Any) -> Any:
         ...
-
-
-class CategoricalParams(Params):
-    """Sample from a categorical distribution."""
-
-    def __init__(self, name: str, choices: List[Any]) -> None:
-        super().__init__(name, (min(choices), max(choices)))
-        self.name = name
-        self.choices = choices
-
-    def get(self) -> List[Any]:
-        return [self.name, self.choices]
-
-    def sample(self) -> Any:
-        return random.SystemRandom().choice(self.choices)
-
-
-class FloatParams(Params):
-    """Sample from a float distribution."""
-
-    def __init__(self, name: str, low: float, high: float) -> None:
-        low = float(low)
-        high = float(high)
-
-        super().__init__(name, (low, high))
-        self.name = name
-        self.low = low
-        self.high = high
-
-    def get(self) -> List[Any]:
-        return [self.name, self.low, self.high]
-
-    def sample(self) -> Any:
-        return random.uniform(self.low, self.high)  # nosec
-
-
-class IntegerParams(Params):
-    """Sample from an integer distribution."""
-
-    def __init__(self, name: str, low: int, high: int, step: int = 1) -> None:
-        self.low = low
-        self.high = high
-        self.step = step
-
-        super().__init__(name, (low, high))
-        self.name = name
-        self.low = low
-        self.high = high
-        self.step = step
-        self.choices = [val for val in range(low, high + 1, step)]
-
-    def get(self) -> List[Any]:
-        return [self.name, self.low, self.high, self.step]
-
-    def sample(self) -> Any:
-        return random.SystemRandom().choice(
-            self.choices,
-        )
```

## tempor/plugins/core/_plugin.py

```diff
@@ -1,29 +1,21 @@
+import functools
 import glob
-import importlib
 import importlib.abc
 import importlib.util
-import os
 import os.path
-import sys
-from typing import TYPE_CHECKING, Any, Callable, ClassVar, Dict, List, Type, TypeVar
+from typing import Any, ClassVar, Dict, List, Type
 
-from typing_extensions import ParamSpec
-
-import tempor
 from tempor.log import logger
 
 from . import utils
 
 PLUGIN_NAME_NOT_SET = "NOT_SET"
 PLUGIN_CATEGORY_NOT_SET = "NOT_SET"
 
-P = ParamSpec("P")
-T = TypeVar("T")
-
 
 class Plugin:
     name: ClassVar[str] = PLUGIN_NAME_NOT_SET
     category: ClassVar[str] = PLUGIN_CATEGORY_NOT_SET
 
     @classmethod
     def fqn(cls) -> str:
@@ -57,26 +49,15 @@
     # Not a bullet proof check but should suffice for practical purposes.
     return (
         class_1.__name__ == class_2.__name__ and class_1.__module__.split(".")[-1] == class_2.__module__.split(".")[-1]
     )
 
 
 def register_plugin(name: str, category: str):
-    def class_decorator(cls: Callable[P, T]) -> Callable[P, T]:
-        # NOTE:
-        # The Callable[<ParamSpec>, <TypeVar>] approach allows to preserve the type annotation of the parameters of the
-        # wrapped class (its __init__ method, specifically). See resources:
-        #     * https://stackoverflow.com/a/74080156
-        #     * https://docs.python.org/3/library/typing.html#typing.ParamSpec
-
-        if TYPE_CHECKING:  # pragma: no cover
-            # Note that cls is in fact `Type[Plugin]`, but this allows to
-            # silence static type-checker warnings inside this function.
-            assert isinstance(cls, Plugin)  # nosec B101
-
+    def inner(cls: Type[Plugin]):
         logger.debug(f"Registering plugin of class {cls}")
         cls.name = name
         cls.category = category
 
         if cls.category not in PLUGIN_CATEGORY_REGISTRY:
             raise TypeError(
                 f"Found plugin category {cls.category} which has not been registered with "
@@ -94,27 +75,30 @@
                 raise TypeError(
                     f"Plugin with fully-qualified name {cls.fqn()} already registered (as class "
                     f"{PLUGIN_REGISTRY[cls.fqn()]})"
                 )
             else:
                 # The same class is being reimported, do not raise error.
                 pass
-
         PLUGIN_REGISTRY[cls.fqn()] = cls
 
-        return cls
+        @functools.wraps(cls)
+        def wrapper(*args, **kwargs):
+            return cls(*args, **kwargs)
 
-    return class_decorator
+        # To access the class directly if required:
+        wrapper.cls = cls  # type: ignore
+
+        return wrapper
+
+    return inner
 
 
 class PluginLoader:
     def __init__(self) -> None:
-        self._refresh()
-
-    def _refresh(self):
         self._plugin_registry: Dict[str, Type[Plugin]] = PLUGIN_REGISTRY
 
         name_by_category: Dict = dict()
         for plugin_class in self._plugin_registry.values():
             name_by_category = utils.append_by_dot_path(
                 name_by_category, key_path=plugin_class.category, value=plugin_class.name
             )
@@ -124,58 +108,44 @@
         for plugin_class in self._plugin_registry.values():
             class_by_category = utils.append_by_dot_path(
                 class_by_category, key_path=plugin_class.category, value=plugin_class
             )
         self._plugin_class_by_category = class_by_category
 
     def list(self) -> Dict:
-        self._refresh()
         return self._plugin_name_by_category
 
     def list_fqns(self) -> List[str]:
-        self._refresh()
         return list(self._plugin_registry.keys())
 
     def list_classes(self) -> Dict:
-        self._refresh()
         return self._plugin_class_by_category
 
-    def list_categories(self) -> Dict[str, Type[Plugin]]:
-        self._refresh()
-        return PLUGIN_CATEGORY_REGISTRY
-
     def _raise_plugin_does_not_exist_error(self, name: str):
         if name not in self._plugin_registry:
             raise ValueError(f"Plugin {name} does not exist.")
 
     def get(self, name: str, *args, **kwargs) -> Any:
-        self._refresh()
         self._raise_plugin_does_not_exist_error(name)
         return self._plugin_registry[name](*args, **kwargs)
 
     def get_class(self, name: str) -> Type:
-        self._refresh()
         self._raise_plugin_does_not_exist_error(name)
         return self._plugin_registry[name]
 
 
 PLUGIN_FILENAME_PREFIX = "plugin_"
 
 
 def _glob_plugin_paths(package_dir: str) -> List[str]:
     return [f for f in glob.glob(os.path.join(package_dir, f"{PLUGIN_FILENAME_PREFIX}*.py")) if os.path.isfile(f)]
 
 
 def _module_name_from_path(path: str) -> str:
-    path = os.path.normpath(path)
-    split = path[path.rfind(f"{tempor.import_name}{os.sep}") :].split(os.sep)
-    if split[-1][-3:] != ".py":
-        raise ValueError(f"Path `{path}` is not a python file.")
-    split[-1] = split[-1].replace(".py", "")
-    return ".".join(split)
+    return os.path.basename(path)[:-3]
 
 
 class importing:  # Functions as namespace, for clarity.
     @staticmethod
     def import_plugins(init_file: str) -> None:
         package_dir = os.path.dirname(init_file)
         logger.debug(f"Importing all plugin modules inside {package_dir}")
@@ -183,16 +153,15 @@
         logger.trace(f"Found plugin module paths to import:\n{paths}")
         for f in paths:
             module_name = _module_name_from_path(f)
             logger.debug(f"Importing plugin module: {module_name}")
             spec = importlib.util.spec_from_file_location(module_name, f)
             if spec is None or not isinstance(spec.loader, importlib.abc.Loader):
                 raise RuntimeError(f"Import failed for {module_name}")
-            module = importlib.util.module_from_spec(spec)
-            sys.modules[module_name] = module
-            spec.loader.exec_module(module)
+            mod = importlib.util.module_from_spec(spec)
+            spec.loader.exec_module(mod)
 
     @staticmethod
     def gather_modules_names(package_init_file: str) -> List[str]:
         package_dir = os.path.dirname(package_init_file)
         paths = _glob_plugin_paths(package_dir=package_dir)
         return [_module_name_from_path(f) for f in paths]
```

## tempor/plugins/core/utils.py

```diff
@@ -1,8 +1,9 @@
-"""Module with utilities that support plugin functionality."""
+"""Module with utilities that support plugin functionality.
+"""
 
 from typing import Any, Dict, List
 
 # Helpers for organizing the plugin registry.
 
 
 def add_by_list_of_keys(dictionary: Dict, key_path: List[Any], value: Any) -> Dict:
```

## tempor/plugins/preprocessing/__init__.py

```diff
@@ -1,7 +1,6 @@
-from . import imputation, nop, scaling
+from . import imputation, scaling
 
 __all__ = [
     "imputation",
-    "nop",
     "scaling",
 ]
```

## tempor/plugins/preprocessing/imputation/__init__.py

```diff
@@ -1,8 +1,16 @@
-from . import static, temporal
-from ._base import BaseImputer
+import tempor.plugins.core as plugins
 
-__all__ = [
+
+class BaseImputer(plugins.BaseTransformer):
+    def __init__(self, **params) -> None:  # pylint: disable=useless-super-delegation
+        super().__init__(**params)
+
+
+plugins.register_plugin_category("preprocessing.imputation", BaseImputer)
+
+plugins.importing.import_plugins(__file__)
+
+__all__ = [  # pyright: ignore
+    *plugins.importing.gather_modules_names(__file__),
     "BaseImputer",
-    "static",
-    "temporal",
 ]
```

## tempor/plugins/preprocessing/scaling/__init__.py

```diff
@@ -1,8 +1,16 @@
-from . import static, temporal
-from ._base import BaseScaler
+import tempor.plugins.core as plugins
 
-__all__ = [
+
+class BaseScaler(plugins.BaseTransformer):
+    def __init__(self, **params) -> None:  # pylint: disable=useless-super-delegation
+        super().__init__(**params)
+
+
+plugins.register_plugin_category("preprocessing.scaling", BaseScaler)
+
+plugins.importing.import_plugins(__file__)
+
+__all__ = [  # pyright: ignore
+    *plugins.importing.gather_modules_names(__file__),
     "BaseScaler",
-    "static",
-    "temporal",
 ]
```

## Comparing `tempor/plugins/preprocessing/nop/__init__.py` & `tempor/plugins/preprocessing/scaling/plugin_nop.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,17 @@
-from typing_extensions import Self
+from typing import Any
 
 import tempor.plugins.core as plugins
 from tempor.data import dataset
+from tempor.plugins.preprocessing.scaling import BaseScaler
 
-plugins.register_plugin_category("preprocessing.nop", plugins.BaseTransformer)
 
-
-@plugins.register_plugin(name="nop_transformer", category="preprocessing.nop")
-class NopTransformer(plugins.BaseTransformer):
+@plugins.register_plugin(name="nop_scaler", category="preprocessing.scaling")
+class NopScaler(BaseScaler):
     def __init__(self, **params) -> None:  # pylint: disable=useless-super-delegation
         super().__init__(**params)
 
-    def _fit(
-        self,
-        data: dataset.BaseDataset,
-        *args,
-        **kwargs,
-    ) -> Self:
+    def _fit(self, data: dataset.Dataset, *args, **kwargs) -> "NopScaler":
         return self
 
-    def _transform(self, data: dataset.BaseDataset, *args, **kwargs) -> dataset.BaseDataset:
+    def _transform(self, data: dataset.Dataset, *args, **kwargs) -> Any:
         return data
-
-    @staticmethod
-    def hyperparameter_space(*args, **kwargs):
-        return []
-
-
-__all__ = [
-    "NopTransformer",
-]
```

## Comparing `temporai-0.0.1.dist-info/LICENSE.txt` & `temporai-0.0.1.dev0.dist-info/LICENSE.txt`

 * *Files identical despite different names*


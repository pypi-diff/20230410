# Comparing `tmp/pyreal-0.3.2.tar.gz` & `tmp/pyreal-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreal-0.3.2.tar", max compression
+gzip compressed data, was "pyreal-0.4.0.tar", max compression
```

## Comparing `pyreal-0.3.2.tar` & `pyreal-0.4.0.tar`

### file list

```diff
@@ -1,125 +1,138 @@
--rw-r--r--   0        0        0      165 2023-02-13 19:17:44.961326 pyreal-0.3.2/AUTHORS.rst
--rw-r--r--   0        0        0        9 2023-02-13 19:17:44.961326 pyreal-0.3.2/HISTORY.md
--rw-r--r--   0        0        0     1075 2023-02-13 19:17:44.961326 pyreal-0.3.2/LICENSE
--rw-r--r--   0        0        0     5260 2023-02-13 19:17:44.961326 pyreal-0.3.2/README.md
--rw-r--r--   0        0        0     1901 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      165 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/__init__.py
--rw-r--r--   0        0        0        0 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/applications/__init__.py
--rw-r--r--   0        0        0    60300 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/applications/data/data.csv
--rw-r--r--   0        0        0      977 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/applications/data/model.pkl
--rw-r--r--   0        0        0     2006 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/applications/data/transformers.pkl
--rw-r--r--   0        0        0     2581 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/applications/titanic.py
--rw-r--r--   0        0        0        0 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/__init__.py
--rw-r--r--   0        0        0        0 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/challenges/__init__.py
--rw-r--r--   0        0        0     3042 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/challenges/explainer_challenge.py
--rw-r--r--   0        0        0        0 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/challenges/gfi/__init__.py
--rw-r--r--   0        0        0      436 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/challenges/gfi/global_feature_importance_challenge.py
--rw-r--r--   0        0        0      430 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/challenges/gfi/shap_feature_importance_challenge.py
--rw-r--r--   0        0        0        0 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/challenges/lfc/__init__.py
--rw-r--r--   0        0        0      439 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/challenges/lfc/local_feature_contribution_challenge.py
--rw-r--r--   0        0        0      436 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/challenges/lfc/shap_feature_contribution_challenge.py
--rw-r--r--   0        0        0     1623 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/dataset.py
--rw-r--r--   0        0        0      610 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/download_datasets_script.py
--rw-r--r--   0        0        0     5213 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/main.py
--rw-r--r--   0        0        0    15073 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/models/Bioresponse_logistic_regression.pkl
--rw-r--r--   0        0        0     1100 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/models/PhishingWebsites_logistic_regression.pkl
--rw-r--r--   0        0        0     1652 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/models/adult_logistic_regression.pkl
--rw-r--r--   0        0        0     3108 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/models/analcatdata_authorship_logistic_regression.pkl
--rw-r--r--   0        0        0     1244 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/models/analcatdata_dmft_logistic_regression.pkl
--rw-r--r--   0        0        0      941 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/models/balance-scale_logistic_regression.pkl
--rw-r--r--   0        0        0      892 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/models/banknote-authentication_logistic_regression.pkl
--rw-r--r--   0        0        0      892 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/models/blood-transfusion-service-center_logistic_regression.pkl
--rw-r--r--   0        0        0      881 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/models/breast-w_logistic_regression.pkl
--rw-r--r--   0        0        0     1116 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/models/cmc_logistic_regression.pkl
--rw-r--r--   0        0        0    62681 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/models/cnae-9_logistic_regression.pkl
--rw-r--r--   0        0        0     1180 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/models/credit-approval_logistic_regression.pkl
--rw-r--r--   0        0        0     1300 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/models/credit-g_logistic_regression.pkl
--rw-r--r--   0        0        0      873 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/models/diabetes_logistic_regression.pkl
--rw-r--r--   0        0        0      873 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/models/electricity_logistic_regression.pkl
--rw-r--r--   0        0        0     4528 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/models/eucalyptus_logistic_regression.pkl
--rw-r--r--   0        0        0     3423 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/models/first-order-theorem-proving_logistic_regression.pkl
--rw-r--r--   0        0        0      948 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/models/ilpd_logistic_regression.pkl
--rw-r--r--   0        0        0   129793 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/isolet_logistic_regression.pkl
--rw-r--r--   0        0        0     1028 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/jm1_logistic_regression.pkl
--rw-r--r--   0        0        0     1028 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/kc1_logistic_regression.pkl
--rw-r--r--   0        0        0      977 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/kc2_logistic_regression.pkl
--rw-r--r--   0        0        0     1396 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/kr-vs-kp_logistic_regression.pkl
--rw-r--r--   0        0        0     4636 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/letter_logistic_regression.pkl
--rw-r--r--   0        0        0     4865 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/madelon_logistic_regression.pkl
--rw-r--r--   0        0        0    18351 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/mfeat-factors_logistic_regression.pkl
--rw-r--r--   0        0        0     7151 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/mfeat-fourier_logistic_regression.pkl
--rw-r--r--   0        0        0     6191 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/mfeat-karhunen_logistic_regression.pkl
--rw-r--r--   0        0        0     1551 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/mfeat-morphological_logistic_regression.pkl
--rw-r--r--   0        0        0     4831 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/mfeat-zernike_logistic_regression.pkl
--rw-r--r--   0        0        0    63793 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/mnist_784_logistic_regression.pkl
--rw-r--r--   0        0        0     1807 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/nomao_logistic_regression.pkl
--rw-r--r--   0        0        0     6191 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/optdigits_logistic_regression.pkl
--rw-r--r--   0        0        0     1439 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/ozone-level-8hr_logistic_regression.pkl
--rw-r--r--   0        0        0     1028 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/pc1_logistic_regression.pkl
--rw-r--r--   0        0        0     1159 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/pc3_logistic_regression.pkl
--rw-r--r--   0        0        0     1159 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/pc4_logistic_regression.pkl
--rw-r--r--   0        0        0     2351 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/pendigits_logistic_regression.pkl
--rw-r--r--   0        0        0      900 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/phoneme_logistic_regression.pkl
--rw-r--r--   0        0        0     1191 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/qsar-biodeg_logistic_regression.pkl
--rw-r--r--   0        0        0     2703 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/satimage_logistic_regression.pkl
--rw-r--r--   0        0        0    21553 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/semeion_logistic_regression.pkl
--rw-r--r--   0        0        0     1228 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/sick_logistic_regression.pkl
--rw-r--r--   0        0        0     1319 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/spambase_logistic_regression.pkl
--rw-r--r--   0        0        0     7738 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/splice_logistic_regression.pkl
--rw-r--r--   0        0        0     1025 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/tic-tac-toe_logistic_regression.pkl
--rw-r--r--   0        0        0     1444 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/vehicle_logistic_regression.pkl
--rw-r--r--   0        0        0     3384 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/vowel_logistic_regression.pkl
--rw-r--r--   0        0        0     1695 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/wall-robot-navigation_logistic_regression.pkl
--rw-r--r--   0        0        0     1100 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/models/wdbc_logistic_regression.pkl
--rw-r--r--   0        0        0      145 2023-02-13 19:17:44.965326 pyreal-0.3.2/pyreal/benchmark/models.py
--rw-r--r--   0        0        0    10056 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/results/20210916-115944/GlobalFeatureImportanceChallenge
--rw-r--r--   0        0        0    10104 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/results/20210916-115944/LocalFeatureContributionChallenge
--rw-r--r--   0        0        0    10111 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/results/20210916-115944/ShapFeatureContributionChallenge
--rw-r--r--   0        0        0    10072 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/results/20210916-115944/ShapFeatureImportanceChallenge
--rw-r--r--   0        0        0    10069 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/results/20210924-133808/GlobalFeatureImportanceChallenge
--rw-r--r--   0        0        0    10073 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/results/20210924-133808/ShapFeatureImportanceChallenge
--rw-r--r--   0        0        0     1186 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/benchmark/task.py
--rw-r--r--   0        0        0     1879 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/__init__.py
--rw-r--r--   0        0        0    18115 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/base.py
--rw-r--r--   0        0        0        0 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/dte/__init__.py
--rw-r--r--   0        0        0     3018 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/dte/base.py
--rw-r--r--   0        0        0     6168 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/dte/decision_tree_explainer.py
--rw-r--r--   0        0        0     2871 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/dte/surrogate_decision_tree.py
--rw-r--r--   0        0        0     7766 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/generic_explainer.py
--rw-r--r--   0        0        0        0 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/gfi/__init__.py
--rw-r--r--   0        0        0     3863 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/gfi/base.py
--rw-r--r--   0        0        0     5810 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/gfi/global_feature_importance.py
--rw-r--r--   0        0        0     1866 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/gfi/permutation_feature_importance.py
--rw-r--r--   0        0        0     3505 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/gfi/shap_feature_importance.py
--rw-r--r--   0        0        0        0 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/lfc/__init__.py
--rw-r--r--   0        0        0     4482 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/lfc/base.py
--rw-r--r--   0        0        0     6282 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/lfc/local_feature_contribution.py
--rw-r--r--   0        0        0     4057 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/lfc/shap_feature_contribution.py
--rw-r--r--   0        0        0     2955 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/lfc/simple_counterfactual_contribution.py
--rw-r--r--   0        0        0      372 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/time_series/__init__.py
--rw-r--r--   0        0        0        0 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/time_series/saliency/__init__.py
--rw-r--r--   0        0        0     4228 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/time_series/saliency/base.py
--rw-r--r--   0        0        0     5092 2023-02-13 19:17:44.969326 pyreal-0.3.2/pyreal/explainers/time_series/saliency/univariate_lime_saliency.py
--rw-r--r--   0        0        0     5285 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/explainers/time_series/saliency/univariate_occlusion_saliency.py
--rw-r--r--   0        0        0     1756 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/transformers/__init__.py
--rw-r--r--   0        0        0    16967 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/transformers/base.py
--rw-r--r--   0        0        0     5189 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/transformers/feature_select.py
--rw-r--r--   0        0        0     2719 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/transformers/impute.py
--rw-r--r--   0        0        0    15368 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/transformers/one_hot_encode.py
--rw-r--r--   0        0        0     2164 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/transformers/pad.py
--rw-r--r--   0        0        0     6565 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/transformers/sax.py
--rw-r--r--   0        0        0    16093 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/transformers/time_series_formatter.py
--rw-r--r--   0        0        0     1337 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/transformers/wrappers.py
--rw-r--r--   0        0        0        0 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/types/__init__.py
--rw-r--r--   0        0        0        0 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/types/explanations/__init__.py
--rw-r--r--   0        0        0      898 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/types/explanations/base.py
--rw-r--r--   0        0        0      987 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/types/explanations/decision_tree.py
--rw-r--r--   0        0        0     3651 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/types/explanations/feature_based.py
--rw-r--r--   0        0        0      646 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/types/explanations/time_series_saliency.py
--rw-r--r--   0        0        0        0 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/utils/__init__.py
--rw-r--r--   0        0        0     7792 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/utils/_plot_tree.py
--rw-r--r--   0        0        0     1968 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/utils/dataloader.py
--rw-r--r--   0        0        0     1821 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/utils/model_utils.py
--rw-r--r--   0        0        0    11417 2023-02-13 19:17:44.973326 pyreal-0.3.2/pyreal/utils/visualize.py
--rw-r--r--   0        0        0     7037 1970-01-01 00:00:00.000000 pyreal-0.3.2/setup.py
--rw-r--r--   0        0        0     6567 1970-01-01 00:00:00.000000 pyreal-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      165 2023-04-10 15:12:35.216516 pyreal-0.4.0/AUTHORS.rst
+-rw-r--r--   0        0        0        9 2023-04-10 15:12:35.216516 pyreal-0.4.0/HISTORY.md
+-rw-r--r--   0        0        0     1075 2023-04-10 15:12:35.216516 pyreal-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4238 2023-04-10 15:12:35.216516 pyreal-0.4.0/README.md
+-rw-r--r--   0        0        0     1856 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      240 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/challenges/__init__.py
+-rw-r--r--   0        0        0     3042 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/challenges/explainer_challenge.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/challenges/gfi/__init__.py
+-rw-r--r--   0        0        0      436 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/challenges/gfi/global_feature_importance_challenge.py
+-rw-r--r--   0        0        0      430 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/challenges/gfi/shap_feature_importance_challenge.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/challenges/lfc/__init__.py
+-rw-r--r--   0        0        0      439 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/challenges/lfc/local_feature_contribution_challenge.py
+-rw-r--r--   0        0        0      436 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/challenges/lfc/shap_feature_contribution_challenge.py
+-rw-r--r--   0        0        0     1623 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/dataset.py
+-rw-r--r--   0        0        0      610 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/download_datasets_script.py
+-rw-r--r--   0        0        0     5213 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/main.py
+-rw-r--r--   0        0        0    15073 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/Bioresponse_logistic_regression.pkl
+-rw-r--r--   0        0        0     1100 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/PhishingWebsites_logistic_regression.pkl
+-rw-r--r--   0        0        0     1652 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/adult_logistic_regression.pkl
+-rw-r--r--   0        0        0     3108 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/analcatdata_authorship_logistic_regression.pkl
+-rw-r--r--   0        0        0     1244 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/analcatdata_dmft_logistic_regression.pkl
+-rw-r--r--   0        0        0      941 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/balance-scale_logistic_regression.pkl
+-rw-r--r--   0        0        0      892 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/banknote-authentication_logistic_regression.pkl
+-rw-r--r--   0        0        0      892 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/blood-transfusion-service-center_logistic_regression.pkl
+-rw-r--r--   0        0        0      881 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/breast-w_logistic_regression.pkl
+-rw-r--r--   0        0        0     1116 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models/cmc_logistic_regression.pkl
+-rw-r--r--   0        0        0    62681 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/cnae-9_logistic_regression.pkl
+-rw-r--r--   0        0        0     1180 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/credit-approval_logistic_regression.pkl
+-rw-r--r--   0        0        0     1300 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/credit-g_logistic_regression.pkl
+-rw-r--r--   0        0        0      873 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/diabetes_logistic_regression.pkl
+-rw-r--r--   0        0        0      873 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/electricity_logistic_regression.pkl
+-rw-r--r--   0        0        0     4528 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/eucalyptus_logistic_regression.pkl
+-rw-r--r--   0        0        0     3423 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/first-order-theorem-proving_logistic_regression.pkl
+-rw-r--r--   0        0        0      948 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/ilpd_logistic_regression.pkl
+-rw-r--r--   0        0        0   129793 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/isolet_logistic_regression.pkl
+-rw-r--r--   0        0        0     1028 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/jm1_logistic_regression.pkl
+-rw-r--r--   0        0        0     1028 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/kc1_logistic_regression.pkl
+-rw-r--r--   0        0        0      977 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/kc2_logistic_regression.pkl
+-rw-r--r--   0        0        0     1396 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/kr-vs-kp_logistic_regression.pkl
+-rw-r--r--   0        0        0     4636 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/letter_logistic_regression.pkl
+-rw-r--r--   0        0        0     4865 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/madelon_logistic_regression.pkl
+-rw-r--r--   0        0        0    18351 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/mfeat-factors_logistic_regression.pkl
+-rw-r--r--   0        0        0     7151 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/mfeat-fourier_logistic_regression.pkl
+-rw-r--r--   0        0        0     6191 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/mfeat-karhunen_logistic_regression.pkl
+-rw-r--r--   0        0        0     1551 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/mfeat-morphological_logistic_regression.pkl
+-rw-r--r--   0        0        0     4831 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/mfeat-zernike_logistic_regression.pkl
+-rw-r--r--   0        0        0    63793 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/mnist_784_logistic_regression.pkl
+-rw-r--r--   0        0        0     1807 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/nomao_logistic_regression.pkl
+-rw-r--r--   0        0        0     6191 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/optdigits_logistic_regression.pkl
+-rw-r--r--   0        0        0     1439 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/ozone-level-8hr_logistic_regression.pkl
+-rw-r--r--   0        0        0     1028 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/pc1_logistic_regression.pkl
+-rw-r--r--   0        0        0     1159 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/pc3_logistic_regression.pkl
+-rw-r--r--   0        0        0     1159 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/pc4_logistic_regression.pkl
+-rw-r--r--   0        0        0     2351 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/pendigits_logistic_regression.pkl
+-rw-r--r--   0        0        0      900 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/phoneme_logistic_regression.pkl
+-rw-r--r--   0        0        0     1191 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/qsar-biodeg_logistic_regression.pkl
+-rw-r--r--   0        0        0     2703 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/satimage_logistic_regression.pkl
+-rw-r--r--   0        0        0    21553 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/semeion_logistic_regression.pkl
+-rw-r--r--   0        0        0     1228 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/sick_logistic_regression.pkl
+-rw-r--r--   0        0        0     1319 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/spambase_logistic_regression.pkl
+-rw-r--r--   0        0        0     7738 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/splice_logistic_regression.pkl
+-rw-r--r--   0        0        0     1025 2023-04-10 15:12:35.224516 pyreal-0.4.0/pyreal/benchmark/models/tic-tac-toe_logistic_regression.pkl
+-rw-r--r--   0        0        0     1444 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/models/vehicle_logistic_regression.pkl
+-rw-r--r--   0        0        0     3384 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/models/vowel_logistic_regression.pkl
+-rw-r--r--   0        0        0     1695 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/models/wall-robot-navigation_logistic_regression.pkl
+-rw-r--r--   0        0        0     1100 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/models/wdbc_logistic_regression.pkl
+-rw-r--r--   0        0        0      145 2023-04-10 15:12:35.220516 pyreal-0.4.0/pyreal/benchmark/models.py
+-rw-r--r--   0        0        0    10056 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/results/20210916-115944/GlobalFeatureImportanceChallenge
+-rw-r--r--   0        0        0    10104 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/results/20210916-115944/LocalFeatureContributionChallenge
+-rw-r--r--   0        0        0    10111 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/results/20210916-115944/ShapFeatureContributionChallenge
+-rw-r--r--   0        0        0    10072 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/results/20210916-115944/ShapFeatureImportanceChallenge
+-rw-r--r--   0        0        0    10069 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/results/20210924-133808/GlobalFeatureImportanceChallenge
+-rw-r--r--   0        0        0    10073 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/results/20210924-133808/ShapFeatureImportanceChallenge
+-rw-r--r--   0        0        0     1186 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/benchmark/task.py
+-rw-r--r--   0        0        0     1879 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/__init__.py
+-rw-r--r--   0        0        0    18048 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/base.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/dte/__init__.py
+-rw-r--r--   0        0        0     3018 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/dte/base.py
+-rw-r--r--   0        0        0     6168 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/dte/decision_tree_explainer.py
+-rw-r--r--   0        0        0     3071 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/dte/surrogate_decision_tree.py
+-rw-r--r--   0        0        0     7766 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/generic_explainer.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/gfi/__init__.py
+-rw-r--r--   0        0        0     3982 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/gfi/base.py
+-rw-r--r--   0        0        0     5985 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/gfi/global_feature_importance.py
+-rw-r--r--   0        0        0     1866 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/gfi/permutation_feature_importance.py
+-rw-r--r--   0        0        0     3505 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/gfi/shap_feature_importance.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/lfc/__init__.py
+-rw-r--r--   0        0        0     4671 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/lfc/base.py
+-rw-r--r--   0        0        0     6452 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/lfc/local_feature_contribution.py
+-rw-r--r--   0        0        0     4057 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/lfc/shap_feature_contribution.py
+-rw-r--r--   0        0        0     2955 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/lfc/simple_counterfactual_contribution.py
+-rw-r--r--   0        0        0      372 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/time_series/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/time_series/saliency/__init__.py
+-rw-r--r--   0        0        0     4376 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/time_series/saliency/base.py
+-rw-r--r--   0        0        0     5102 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/time_series/saliency/univariate_lime_saliency.py
+-rw-r--r--   0        0        0     5489 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/explainers/time_series/saliency/univariate_occlusion_saliency.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/realapp/__init__.py
+-rw-r--r--   0        0        0    17709 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/realapp/realapp.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/sample_applications/__init__.py
+-rw-r--r--   0        0        0     8996 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/sample_applications/ames_housing.py
+-rw-r--r--   0        0        0     1769 2023-04-10 15:12:35.228516 pyreal-0.4.0/pyreal/sample_applications/california_housing.py
+-rw-r--r--   0        0        0   460673 2023-04-10 15:12:35.232516 pyreal-0.4.0/pyreal/sample_applications/data_ames_housing/data.csv
+-rw-r--r--   0        0        0    13637 2023-04-10 15:12:35.232516 pyreal-0.4.0/pyreal/sample_applications/data_ames_housing/data_description.txt
+-rw-r--r--   0        0        0     3431 2023-04-10 15:12:35.232516 pyreal-0.4.0/pyreal/sample_applications/data_ames_housing/feature_descriptions.csv
+-rw-r--r--   0        0        0    14681 2023-04-10 15:12:35.232516 pyreal-0.4.0/pyreal/sample_applications/data_cal_housing/cal_cities_lat_long.csv
+-rw-r--r--   0        0        0  1217129 2023-04-10 15:12:35.236516 pyreal-0.4.0/pyreal/sample_applications/data_cal_housing/california.csv
+-rw-r--r--   0        0        0    68558 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/sample_applications/data_student/data.csv
+-rw-r--r--   0        0        0     1514 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/sample_applications/data_student/students.csv
+-rw-r--r--   0        0        0    60300 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/sample_applications/data_titanic/data.csv
+-rw-r--r--   0        0        0     4569 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/sample_applications/student_performance.py
+-rw-r--r--   0        0        0     3233 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/sample_applications/titanic.py
+-rw-r--r--   0        0        0     1756 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/transformers/__init__.py
+-rw-r--r--   0        0        0    16940 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/transformers/base.py
+-rw-r--r--   0        0        0     5376 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/transformers/feature_select.py
+-rw-r--r--   0        0        0     2719 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/transformers/impute.py
+-rw-r--r--   0        0        0    15375 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/transformers/one_hot_encode.py
+-rw-r--r--   0        0        0     2164 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/transformers/pad.py
+-rw-r--r--   0        0        0     6565 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/transformers/sax.py
+-rw-r--r--   0        0        0    16093 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/transformers/time_series_formatter.py
+-rw-r--r--   0        0        0     1337 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/transformers/wrappers.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/types/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/types/explanations/__init__.py
+-rw-r--r--   0        0        0     4137 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/types/explanations/base.py
+-rw-r--r--   0        0        0      987 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/types/explanations/decision_tree.py
+-rw-r--r--   0        0        0     5184 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/types/explanations/feature_based.py
+-rw-r--r--   0        0        0      646 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/types/explanations/time_series_saliency.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/utils/__init__.py
+-rw-r--r--   0        0        0     7810 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/utils/_plot_tree.py
+-rw-r--r--   0        0        0     1968 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/utils/dataloader.py
+-rw-r--r--   0        0        0     1821 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/utils/model_utils.py
+-rw-r--r--   0        0        0      520 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/visualize/__init__.py
+-rw-r--r--   0        0        0    14256 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/visualize/feature_based_vis.py
+-rw-r--r--   0        0        0     2576 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/visualize/time_series_vis.py
+-rw-r--r--   0        0        0     2687 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/visualize/tree_vis.py
+-rw-r--r--   0        0        0      870 2023-04-10 15:12:35.240516 pyreal-0.4.0/pyreal/visualize/visualize_config.py
+-rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 pyreal-0.4.0/PKG-INFO
```

### Comparing `pyreal-0.3.2/LICENSE` & `pyreal-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyproject.toml` & `pyreal-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 maintainers = [
   "MIT Data To AI Lab <dailabmit@gmail.com>",
 ]
 
 description = "Library for evaluating and deploying human readable machine learning explanations."
 name = "pyreal"
-version = "0.3.2"
+version = "0.4.0"
 
 license = ""
 
 readme = "README.md"
 
 documentation = "https://sibyl-dev.github.io/pyreal"
 homepage = "https://sibyl-ml.dev/"
@@ -33,25 +33,23 @@
 # Library Requirements
 [tool.poetry.dependencies]
 
 # Main Python Requirements
 python = "^3.8, <3.11"
 
 #Library Dependencies
-eli5 = ">=0.11,<0.14"
 matplotlib = "^3.6.0"
 numpy = "^1.23.3"
 pandas = "^1.5.0"
 scikit-learn = "^1.1.2"
 numba = "^0.56.2" # Explicit numba (required by shap) forces recent version
-shap = "=0.40.0"
+shap = "=0.40.0" # Explicit shap prevents break with newer versions
 lime = "^0.2.0.1"
 
 # Example Dependencies
-tensorflow = {version = "^2.6.0,<=2.10.0", optional = true}
 lightgbm = {version = "^3.3.2", optional = true}
 
 # Development Requirements
 seaborn = "^0.12.2"
 [tool.poetry.dev-dependencies]
 
 # Testing Dependencies
@@ -75,15 +73,15 @@
 ipython = ">=8.5.0"
 m2r2 = ">=0.3.3"
 nbsphinx = ">=0.8.8"
 pydata-sphinx-theme = ">=0.10.1"
 
 # Extra Dependency Bundles
 [tool.poetry.extras]
-examples = ["tensorflow", "lightgbm"]
+examples = ["lightgbm"]
 
 [tool.black]
 line-length = 99
 preview = true
 
 [tool.isort]
 profile = "black"
```

### Comparing `pyreal-0.3.2/pyreal/applications/data/data.csv` & `pyreal-0.4.0/pyreal/sample_applications/data_titanic/data.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/applications/titanic.py` & `pyreal-0.4.0/pyreal/sample_applications/titanic.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 import os
 import pickle
 from urllib.parse import urljoin
 
 import pandas as pd
-from sklearn.linear_model import LogisticRegression
+from lightgbm import LGBMClassifier
 
+from pyreal import RealApp
 from pyreal.transformers import (
     ColumnDropTransformer,
     MultiTypeImputer,
     OneHotEncoder,
     fit_transformers,
     run_transformers,
 )
 
-DATA_DIR = os.path.join(os.path.dirname(__file__), "data")
+DATA_DIR = os.path.join(os.path.dirname(__file__), "data_titanic")
 DATA_FILE = os.path.join(DATA_DIR, "data.csv")
 MODEL_FILE = os.path.join(DATA_DIR, "model.pkl")
 TRANSFORMER_FILE = os.path.join(DATA_DIR, "transformers.pkl")
 AWS_BASE_URL = "https://pyreal-data.s3.amazonaws.com/"
 
 
-def load_titanic_data():
+def load_data(n_rows=None, include_targets=False):
     if os.path.exists(DATA_FILE):
         df = pd.read_csv(DATA_FILE)
     else:
         url = urljoin(AWS_BASE_URL, "titanic.csv")
         df = pd.read_csv(url)
 
         if not os.path.isdir(DATA_DIR):
             os.mkdir(DATA_DIR)
         df.to_csv(DATA_FILE, index=False)
     y = df["target"].rename("Survived")
     x_orig = df.drop("target", axis="columns")
-    return x_orig, y
+
+    if n_rows is not None and include_targets:
+        return x_orig[:n_rows], y[:n_rows]
+    elif n_rows is not None:
+        return x_orig[:n_rows]
+    elif include_targets:
+        return x_orig, y
+    else:
+        return x_orig
 
 
 def load_feature_descriptions():
     return {
         "PassengerId": "Passenger ID",
         "Pclass": "Ticket Class",
         "SibSp": "Number of siblings/spouses aboard",
@@ -44,41 +53,57 @@
         "Ticket": "Ticket Number",
         "Fare": "Passenger Fare",
         "Cabin": "Cabin Number",
         "Embarked": "Port of Embarkment",
     }
 
 
-def load_titanic_model():
+def load_model():
     if os.path.exists(MODEL_FILE):
         return pickle.load(open(os.path.join(DATA_DIR, "model.pkl"), "rb"))
     else:
-        transformers = load_titanic_transformers()
-        x_orig, y = load_titanic_data()
+        transformers = load_transformers()
+        x_orig, y = load_data(include_targets=True)
         x_model = run_transformers(transformers, x_orig)
-        model = LogisticRegression(max_iter=500)
+        # model = LogisticRegression(max_iter=500)
+        model = LGBMClassifier()
         model.fit(x_model, y)
 
         if not os.path.isdir(DATA_DIR):
             os.mkdir(DATA_DIR)
         with open(MODEL_FILE, "wb") as f:
             pickle.dump(model, f)
         return model
 
 
-def load_titanic_transformers():
+def load_transformers():
     if os.path.exists(TRANSFORMER_FILE):
         return pickle.load(open(os.path.join(DATA_DIR, "transformers.pkl"), "rb"))
     else:
-        x_orig, y = load_titanic_data()
+        x_orig, y = load_data(include_targets=True)
         column_drop = ColumnDropTransformer(["PassengerId", "Name", "Ticket", "Cabin"])
         imputer = MultiTypeImputer()
         one_hot_encoder = OneHotEncoder(["Sex", "Embarked"])
 
         transformers = [column_drop, imputer, one_hot_encoder]
         fit_transformers(transformers, x_orig)
 
         if not os.path.isdir(DATA_DIR):
             os.mkdir(DATA_DIR)
         with open(TRANSFORMER_FILE, "wb") as f:
             pickle.dump(transformers, f)
         return transformers
+
+
+def load_app():
+    x_train_orig, y = load_data(include_targets=True)
+    model = load_model()
+    transformers = load_transformers()
+    feature_descriptions = load_feature_descriptions()
+
+    return RealApp(
+        model,
+        x_train_orig,
+        y_orig=y,
+        transformers=transformers,
+        feature_descriptions=feature_descriptions,
+    )
```

### Comparing `pyreal-0.3.2/pyreal/benchmark/challenges/explainer_challenge.py` & `pyreal-0.4.0/pyreal/benchmark/challenges/explainer_challenge.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/dataset.py` & `pyreal-0.4.0/pyreal/benchmark/dataset.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/download_datasets_script.py` & `pyreal-0.4.0/pyreal/benchmark/download_datasets_script.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/main.py` & `pyreal-0.4.0/pyreal/benchmark/main.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/Bioresponse_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/Bioresponse_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/PhishingWebsites_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/PhishingWebsites_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/adult_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/adult_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/analcatdata_authorship_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/analcatdata_authorship_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/analcatdata_dmft_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/analcatdata_dmft_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/balance-scale_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/balance-scale_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/banknote-authentication_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/banknote-authentication_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/blood-transfusion-service-center_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/blood-transfusion-service-center_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/breast-w_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/breast-w_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/cmc_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/cmc_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/cnae-9_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/cnae-9_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/credit-approval_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/credit-approval_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/credit-g_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/credit-g_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/diabetes_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/diabetes_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/electricity_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/electricity_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/eucalyptus_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/eucalyptus_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/first-order-theorem-proving_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/first-order-theorem-proving_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/ilpd_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/ilpd_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/isolet_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/isolet_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/jm1_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/jm1_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/kc1_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/kc1_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/kc2_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/kc2_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/kr-vs-kp_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/kr-vs-kp_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/letter_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/letter_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/madelon_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/madelon_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/mfeat-factors_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/mfeat-factors_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/mfeat-fourier_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/mfeat-fourier_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/mfeat-karhunen_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/mfeat-karhunen_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/mfeat-morphological_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/mfeat-morphological_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/mfeat-zernike_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/mfeat-zernike_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/mnist_784_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/mnist_784_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/nomao_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/nomao_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/optdigits_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/optdigits_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/ozone-level-8hr_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/ozone-level-8hr_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/pc1_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/pc1_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/pc3_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/pc3_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/pc4_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/pc4_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/pendigits_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/pendigits_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/phoneme_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/phoneme_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/qsar-biodeg_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/qsar-biodeg_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/satimage_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/satimage_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/semeion_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/semeion_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/sick_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/sick_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/spambase_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/spambase_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/splice_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/splice_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/tic-tac-toe_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/tic-tac-toe_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/vehicle_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/vehicle_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/vowel_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/vowel_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/wall-robot-navigation_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/wall-robot-navigation_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/models/wdbc_logistic_regression.pkl` & `pyreal-0.4.0/pyreal/benchmark/models/wdbc_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/results/20210916-115944/GlobalFeatureImportanceChallenge` & `pyreal-0.4.0/pyreal/benchmark/results/20210916-115944/GlobalFeatureImportanceChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/results/20210916-115944/LocalFeatureContributionChallenge` & `pyreal-0.4.0/pyreal/benchmark/results/20210916-115944/LocalFeatureContributionChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/results/20210916-115944/ShapFeatureContributionChallenge` & `pyreal-0.4.0/pyreal/benchmark/results/20210916-115944/ShapFeatureContributionChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/results/20210916-115944/ShapFeatureImportanceChallenge` & `pyreal-0.4.0/pyreal/benchmark/results/20210916-115944/ShapFeatureImportanceChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/results/20210924-133808/GlobalFeatureImportanceChallenge` & `pyreal-0.4.0/pyreal/benchmark/results/20210924-133808/GlobalFeatureImportanceChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/results/20210924-133808/ShapFeatureImportanceChallenge` & `pyreal-0.4.0/pyreal/benchmark/results/20210924-133808/ShapFeatureImportanceChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/benchmark/task.py` & `pyreal-0.4.0/pyreal/benchmark/task.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/explainers/__init__.py` & `pyreal-0.4.0/pyreal/explainers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/explainers/base.py` & `pyreal-0.4.0/pyreal/explainers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import pandas as pd
 from sklearn.base import is_classifier
 from sklearn.metrics import get_scorer
 
 from pyreal.transformers import BreakingTransformError
 from pyreal.transformers import fit_transformers as fit_transformers_func
 from pyreal.transformers import run_transformers
+from pyreal.types.explanations.base import Explanation
 from pyreal.utils import model_utils
 
 log = logging.getLogger(__name__)
 
 
 def _check_transformers(transformers):
     """
@@ -276,36 +277,37 @@
         i_transformers = _get_transformers(self.transformers, interpret=True)
         return run_transformers(i_transformers, x_orig)
 
     def transform_explanation(self, explanation, x_orig=None):
         """
         Transform the explanation into its interpretable form, by running the e_transformer's
         "inverse_transform_explanation" and i_transformers "transform_explanation" functions.
-        If an `x_orig` argument is added, also convert x_orig with the same transformers. This
-        function will result in x_orig in the same feature space as the final explanation
+        If an `x_orig` is provided, also convert `x_orig` with the same
+        transformers. This function will result in `values` in the Explanation object
+        in the same feature space as the final explanation
 
         Args:
             explanation (type varies by subclass):
                 The raw explanation to transform
-            x_orig (DataFrame of shape (n_instances, x_orig_feature_count) or None):
-                Input data used to generate explanation. Optional argument
+            x_orig (DataFrame of shape (n_instances, n_features) or None)
+                Data to transform to final space
 
         Returns:
-            type varies by subclass
+            Explanation
                 The interpretable form of the explanation
-            DataFrame of shape (n_instances, x_orig_feature_count)
-                If `x_orig` is not None, return `x_orig` transformed to the state of the final
-                explanation. Not returned if `x_orig` is None.
         """
+        if not isinstance(explanation, Explanation):
+            raise ValueError("explanation is not a valid Explanation object")
+
         convert_x = x_orig is not None
         if self.return_original_explanation:
             if convert_x:
-                return explanation, self.transform_to_x_algorithm(x_orig)
-            else:
-                return explanation
+                explanation = explanation.update_values(self.transform_to_x_algorithm(x_orig))
+            return explanation
+
         x = None
         if convert_x:
             x = x_orig.copy()
 
         a_transformers = _get_transformers(self.transformers, algorithm=True, interpret=False)
         i_transformers = _get_transformers(self.transformers, interpret=True)
 
@@ -319,35 +321,35 @@
                     "Transformer class %s does not have the required inverse explanation "
                     "transform and is set to break, stopping transform process"
                     % type(t).__name__
                 )
                 break_point = len(a_transformers) - i
                 if convert_x:
                     x = run_transformers(a_transformers[0:break_point], x)
-                    return explanation, x
+                    return explanation.update_values(x)
                 else:
                     return explanation
         # Iterate through interpret transformers
         for t in i_transformers:
             if not t.algorithm:
                 try:
                     explanation = t.transform_explanation(explanation)
                 except BreakingTransformError:
                     log.warning(
                         "Transformer class %s does not have the required explanation "
                         "transform and is set to break, stopping transform process"
                         % type(t).__name__
                     )
                     if convert_x:
-                        return explanation, x
+                        return explanation.update_values(x)
                     return explanation
             if convert_x:
                 x = t.transform(x)
         if convert_x:
-            return explanation, x
+            return explanation.update_values(x)
         return explanation
 
     def model_predict(self, x_orig):
         """
         Predict on x_orig using the model and return the result
 
         Args:
@@ -394,22 +396,23 @@
         return self.feature_descriptions[feature_name]
 
     def convert_columns_to_interpretable(self, df):
         """
         Returns df with columns (or index, for series) converted to the interpretable descriptions
 
         Args:
-            df (DataFrame of shape (n_instances, x_orig_feature_count) or Series):
+            df (DataFrame):
 
         Returns:
             string
                  Description of feature
         """
         if self.feature_descriptions is None:
             return df
+
         if isinstance(df, pd.Series):
             return df.rename(self.feature_descriptions)
         return df.rename(self.feature_descriptions, axis="columns")
 
     def convert_data_to_interpretable(self, x_orig):
         """
         Convert data in its original form to an interpretable form, with interpretable features
```

### Comparing `pyreal-0.3.2/pyreal/explainers/dte/base.py` & `pyreal-0.4.0/pyreal/explainers/dte/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/explainers/dte/decision_tree_explainer.py` & `pyreal-0.4.0/pyreal/explainers/dte/decision_tree_explainer.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/explainers/dte/surrogate_decision_tree.py` & `pyreal-0.4.0/pyreal/explainers/dte/surrogate_decision_tree.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import pandas as pd
 from sklearn import tree
 
 from pyreal.explainers import DecisionTreeExplainerBase
+from pyreal.types.explanations.decision_tree import DecisionTreeExplanation
+from pyreal.types.explanations.feature_based import FeatureImportanceExplanation
 
 
 class SurrogateDecisionTree(DecisionTreeExplainerBase):
     """
     SurrogateDecisionTree object.
 
     A SurrogateDecisionTree object gets feature explanation using the surrogate
@@ -52,19 +54,19 @@
 
         Returns:
             An explanation class in the form of a decision tree model
         """
 
         if self.explainer is None:
             raise AttributeError(
-                "Instance has no explainer. Please fit the explainer             before producing"
+                "Instance has no explainer. Please fit the explainer before producing"
                 " explanations."
             )
 
-        return self.explainer
+        return DecisionTreeExplanation(self.explainer)
 
     def produce_importances(self):
         """
         Produce the explanation in terms of feature importances.
 
         Returns:
             The feature importances of the decision tree explainer.
@@ -73,8 +75,8 @@
             raise AttributeError(
                 "Instance has no explainer. Please fit the explainer             before producing"
                 " explanations."
             )
 
         features = self.return_features()
         importances = pd.DataFrame(self.explainer.feature_importances_[None, :], columns=features)
-        return importances
+        return FeatureImportanceExplanation(importances)
```

### Comparing `pyreal-0.3.2/pyreal/explainers/generic_explainer.py` & `pyreal-0.4.0/pyreal/explainers/generic_explainer.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/explainers/gfi/base.py` & `pyreal-0.4.0/pyreal/explainers/gfi/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,20 +46,22 @@
         Returns:
             DataFrame of shape (n_features,)
                 Importance of each feature for the model
         """
         # Importance for a given model stays constant, so can be saved and re-returned
         if self.importance is not None:
             return self.importance
-        importance = self.get_importance()
-        importance = self.transform_explanation(importance).get()
+        explanation = self.get_importance()
+        explanation = self.transform_explanation(explanation)
         if self.interpretable_features:
-            return self.convert_columns_to_interpretable(importance)
-        self.importance = importance
-        return importance
+            explanation.update_explanation(
+                self.convert_columns_to_interpretable(explanation.get()), inplace=True
+            )
+        self.importance = explanation
+        return explanation
 
     @abstractmethod
     def get_importance(self):
         """
         Gets the raw explanation.
 
         Returns:
@@ -92,9 +94,11 @@
                 The variation of this Explainer's explanations
         """
         if explanations is None:
             explanations = []
             for i in range(n_iterations - 1):
                 if with_fit:
                     self.fit()
-                explanations.append(self.produce(self._x_train_orig.iloc[0:n_rows]).to_numpy())
+                explanations.append(
+                    self.produce(self._x_train_orig.iloc[0:n_rows]).get().to_numpy()
+                )
         return np.max(np.var(explanations, axis=0))
```

### Comparing `pyreal-0.3.2/pyreal/explainers/gfi/global_feature_importance.py` & `pyreal-0.4.0/pyreal/explainers/gfi/global_feature_importance.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,27 +114,29 @@
     Currently, only SHAP is supported.
 
     Args:
         model (string filepath or model object):
            Filepath to the pickled model to explain, or model object with .predict() function
         x_train_orig (dataframe of shape (n_instances, x_orig_feature_count)):
            The training set for the explainer
-        e_algorithm (string, one of ["shap"]):
+        e_algorithm (string, one of ["shap", "permutation"]):
            Explanation algorithm to use. If none, one will be chosen automatically based on model
            type
+        shap_type (string, one of ["kernel", "linear"]):
+            Type of shap algorithm to use, if e_algorithm="shap".
         **kwargs: see LocalFeatureContributionsBase args
     """
 
-    def __init__(self, model, x_train_orig, e_algorithm=None, **kwargs):
+    def __init__(self, model, x_train_orig, e_algorithm=None, shap_type=None, **kwargs):
         if e_algorithm is None:
             e_algorithm = choose_algorithm()
         self.base_global_feature_importance = None
         if e_algorithm == "shap":
             self.base_global_feature_importance = ShapFeatureImportance(
-                model, x_train_orig, **kwargs
+                model, x_train_orig, shap_type=shap_type, **kwargs
             )
         if e_algorithm == "permutation":
             self.base_global_feature_importance = PermutationFeatureImportance(
                 model, x_train_orig, **kwargs
             )
         if self.base_global_feature_importance is None:
             raise ValueError("Invalid algorithm type %s" % e_algorithm)
```

### Comparing `pyreal-0.3.2/pyreal/explainers/gfi/permutation_feature_importance.py` & `pyreal-0.4.0/pyreal/explainers/gfi/permutation_feature_importance.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/explainers/gfi/shap_feature_importance.py` & `pyreal-0.4.0/pyreal/explainers/gfi/shap_feature_importance.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/explainers/lfc/base.py` & `pyreal-0.4.0/pyreal/explainers/lfc/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,24 +52,26 @@
         series = False
         name = None
         if isinstance(x_orig, pd.Series):
             name = x_orig.name
             series = True
             x_orig = x_orig.to_frame().T
         contributions = self.get_contributions(x_orig)
-        contributions, x_interpret = self.transform_explanation(contributions, x_orig)
+        explanation = self.transform_explanation(contributions, x_orig)
+        x_interpret = explanation.get_values()
         if series:
             x_interpret = x_interpret.squeeze()
             x_interpret.name = name
-        contributions = contributions.get()
+        contributions = explanation.get()
         if self.interpretable_features:
-            return self.convert_columns_to_interpretable(
-                contributions
-            ), self.convert_columns_to_interpretable(x_interpret)
-        return contributions, x_interpret
+            contributions = self.convert_columns_to_interpretable(contributions)
+            x_interpret = self.convert_columns_to_interpretable(x_interpret)
+        explanation.update_values(x_interpret, inplace=True)
+        explanation.update_explanation(contributions, inplace=True)
+        return explanation
 
     @abstractmethod
     def get_contributions(self, x_orig):
         """
         Gets the raw explanation.
         Args:
             x_orig (DataFrame of shape (n_instances, n_features):
@@ -105,10 +107,12 @@
                 The variation of this Explainer's explanations
         """
         if explanations is None:
             explanations = []
             for i in range(n_iterations - 1):
                 if with_fit:
                     self.fit()
-                explanations.append(self.produce(self._x_train_orig.iloc[0:n_rows])[0].to_numpy())
+                explanations.append(
+                    self.produce(self._x_train_orig.iloc[0:n_rows]).get().to_numpy()
+                )
 
         return np.max(np.var(explanations, axis=0))
```

### Comparing `pyreal-0.3.2/pyreal/explainers/lfc/local_feature_contribution.py` & `pyreal-0.4.0/pyreal/explainers/lfc/local_feature_contribution.py`

 * *Files 9% similar despite different names*

```diff
@@ -118,27 +118,29 @@
     Currently, only SHAP is supported.
 
     Args:
         model (string filepath or model object):
            Filepath to the pickled model to explain, or model object with .predict() function
         x_train_orig (dataframe of shape (n_instances, x_orig_feature_count)):
            The training set for the explainer
-        e_algorithm (string, one of ["shap"]):
+        e_algorithm (string, one of ["shap", "simple"]):
            Explanation algorithm to use. If none, one will be chosen automatically based on model
            type
+        shap_type (string, one of ["kernel", "linear"]):
+            Type of shap algorithm to use, if e_algorithm="shap".
         **kwargs: see LocalFeatureContributionsBase args
     """
 
-    def __init__(self, model, x_train_orig, e_algorithm=None, **kwargs):
+    def __init__(self, model, x_train_orig, e_algorithm=None, shap_type=None, **kwargs):
         if e_algorithm is None:
             e_algorithm = choose_algorithm()
         self.base_local_feature_contribution = None
         if e_algorithm == "shap":
             self.base_local_feature_contribution = ShapFeatureContribution(
-                model, x_train_orig, **kwargs
+                model, x_train_orig, shap_type=shap_type, **kwargs
             )
         elif e_algorithm == "simple":
             self.base_local_feature_contribution = SimpleCounterfactualContribution(
                 model, x_train_orig, **kwargs
             )
         if self.base_local_feature_contribution is None:
             raise ValueError("Invalid algorithm type %s" % e_algorithm)
```

### Comparing `pyreal-0.3.2/pyreal/explainers/lfc/shap_feature_contribution.py` & `pyreal-0.4.0/pyreal/explainers/lfc/shap_feature_contribution.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/explainers/lfc/simple_counterfactual_contribution.py` & `pyreal-0.4.0/pyreal/explainers/lfc/simple_counterfactual_contribution.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/explainers/time_series/saliency/base.py` & `pyreal-0.4.0/pyreal/explainers/time_series/saliency/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,24 +49,26 @@
         series = False
         name = None
         if isinstance(x_orig, pd.Series):
             name = x_orig.name
             series = True
             x_orig = x_orig.to_frame().T
         contributions = self.get_contributions(x_orig)
-        contributions, x_interpret = self.transform_explanation(contributions, x_orig)
+        explanation = self.transform_explanation(contributions, x_orig)
+        x_interpret = explanation.get_values()
         if series:
             x_interpret = x_interpret.squeeze()
             x_interpret.name = name
-        contributions = contributions.get()
+        contributions = explanation.get()
         if self.interpretable_features:
-            return self.convert_columns_to_interpretable(
-                contributions
-            ), self.convert_columns_to_interpretable(x_interpret)
-        return contributions, x_interpret
+            contributions = self.convert_columns_to_interpretable(contributions)
+            x_interpret = self.convert_columns_to_interpretable(x_interpret)
+        explanation.update_values(x_interpret, inplace=True)
+        explanation.update_explanation(contributions, inplace=True)
+        return explanation
 
     @abstractmethod
     def get_contributions(self, x_orig):
         """
         Get the raw explanation.
         Args:
             x_orig (DataFrame of shape (n_instances, length of series):
```

### Comparing `pyreal-0.3.2/pyreal/explainers/time_series/saliency/univariate_lime_saliency.py` & `pyreal-0.4.0/pyreal/explainers/time_series/saliency/univariate_lime_saliency.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from contextlib import ExitStack
 
 import numpy as np
 import pandas as pd
 from lime import lime_tabular
 
 from pyreal.explainers.time_series import SaliencyBase
-from pyreal.types.explanations.feature_based import FeatureContributionExplanation
+from pyreal.types.explanations.feature_based import ClassFeatureContributionExplanation
 
 
 class UnivariateLimeSaliency(SaliencyBase):
     """
     UnivariateLimeSaliency object.
 
     An UnivariateLimeSaliency object judges the relative importance or saliency of each timestep
@@ -123,8 +123,8 @@
             )
 
         if isinstance(x_algo, pd.DataFrame):
             importances_df = pd.DataFrame(importances, index=x_algo.columns).T
         else:
             importances_df = pd.DataFrame(importances).T
 
-        return FeatureContributionExplanation(importances_df)
+        return ClassFeatureContributionExplanation(importances_df)
```

### Comparing `pyreal-0.3.2/pyreal/explainers/time_series/saliency/univariate_occlusion_saliency.py` & `pyreal-0.4.0/pyreal/explainers/time_series/saliency/univariate_occlusion_saliency.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import numpy as np
 import pandas as pd
 
 from pyreal.explainers.time_series import SaliencyBase
-from pyreal.types.explanations.feature_based import FeatureContributionExplanation
+from pyreal.types.explanations.feature_based import (
+    ClassFeatureContributionExplanation,
+    FeatureContributionExplanation,
+)
 
 
 class UnivariateOcclusionSaliency(SaliencyBase):
     """
     UnivariateOcclusionSaliency object.
 
     An OcclusionSaliency object judges the relative importance or saliency of each timestep
@@ -41,14 +44,15 @@
             num_classes (int):
                 Required if regression=False and classes=None
             **kwargs: see base Explainer args
         """
         self.width = width
         self.k = k
         self.num_classes = num_classes
+        self.regression = regression
         if regression:
             self.num_classes = 1
         super(UnivariateOcclusionSaliency, self).__init__(model, x_train_orig, **kwargs)
         if self.num_classes is None and self.classes is None:
             raise ValueError(
                 "Must provide classes or num_classes parameter when regression is False"
             )
@@ -103,15 +107,18 @@
         importance = v / self.width
 
         if isinstance(x_algo, pd.DataFrame):
             importances_df = pd.DataFrame(importance, index=x_algo.columns).T
         else:
             importances_df = pd.DataFrame(importance).T
 
-        return FeatureContributionExplanation(importances_df)
+        if self.regression:
+            return FeatureContributionExplanation(importances_df)
+        else:
+            return ClassFeatureContributionExplanation(importances_df)
 
     def _occlude_once(self, sig, win_min, win_max, k):
         """
         Occlude one window and return the resulting model prediction
         """
         occ_test_signal = np.copy(sig)
         if self.k == "avg":
```

### Comparing `pyreal-0.3.2/pyreal/transformers/__init__.py` & `pyreal-0.4.0/pyreal/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/transformers/base.py` & `pyreal-0.4.0/pyreal/transformers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,14 @@
             Explanation:
                 The transformed explanation
         Raises:
             ValueError
                 If `explanation` is not of a supported ExplanationType
 
         """
-        print(explanation)
         if isinstance(explanation, AdditiveFeatureContributionExplanation):
             return self.transform_explanation_additive_feature_contribution(explanation)
         if isinstance(explanation, AdditiveFeatureImportanceExplanation):
             return self.transform_explanation_additive_feature_importance(explanation)
         if isinstance(explanation, FeatureContributionExplanation):
             return self.transform_explanation_feature_contribution(explanation)
         if isinstance(explanation, FeatureImportanceExplanation):
```

### Comparing `pyreal-0.3.2/pyreal/transformers/feature_select.py` & `pyreal-0.4.0/pyreal/transformers/feature_select.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         Args:
             columns (dataframe column label type or list of dataframe column label type):
                 Label of column to select, or an ordered list of column labels to select
         """
         if columns is not None and not isinstance(columns, (list, tuple, np.ndarray, pd.Index)):
             columns = [columns]
         self.columns = columns
+        self.column_order = None
         self.dropped_columns = []
         super().__init__(**kwargs)
 
     def fit(self, x, **params):
         """
         Saves the columns being dropped
 
@@ -34,15 +35,16 @@
             x (DataFrame of shape (n_instances, n_features)):
                 The dataset to fit on
         Returns:
             None
 
         """
         self.dropped_columns = list(set(x.columns) - set(self.columns))
-        super().fit(x)
+        self.column_order = x.columns
+        return super().fit(x)
 
     def data_transform(self, x):
         """
         Reorders and selects the features in x
 
         Args:
             x (DataFrame of shape (n_instances, n_features)):
@@ -64,15 +66,15 @@
             FeatureBased:
                 The transformed explanation
 
         """
         explanation_df = explanation.get()
         for col in self.dropped_columns:
             explanation_df[col] = 0
-        return FeatureBased(explanation_df)
+        return FeatureBased(explanation_df[self.column_order])
 
     def transform_explanation_feature_based(self, explanation):
         """
         Selects the desired columns
         Args:
             explanation (FeatureBased):
                 The explanation to be transformed
@@ -111,27 +113,29 @@
         Args:
             columns (dataframe column label type or list of dataframe column label type):
                 Label of column to select, or an ordered list of column labels to select
         """
         if columns is not None and not isinstance(columns, Sequence):
             columns = [columns]
         self.dropped_columns = columns
+        self.column_order = None
         super().__init__(**kwargs)
 
     def data_transform(self, x):
         """
         Reorders and selects the features in x
 
         Args:
             x (DataFrame of shape (n_instances, n_features)):
                 The data to transform
         Returns:
             DataFrame of shape (n_instances, len(columns)):
                 The data with features selected and reordered
         """
+        self.column_order = x.columns
         return x.drop(self.dropped_columns, axis=1)
 
     def inverse_transform_explanation_feature_based(self, explanation):
         """
         Sets the contribution of dropped features to 0
         Args:
             explanation (FeatureBased):
@@ -141,15 +145,15 @@
             FeatureBased:
                 The transformed explanation
 
         """
         explanation_df = explanation.get()
         for col in self.dropped_columns:
             explanation_df[col] = 0
-        return FeatureBased(explanation_df)
+        return FeatureBased(explanation_df[self.column_order])
 
     def transform_explanation_feature_based(self, explanation):
         """
         Drops columns from an explanation
         Args:
             explanation (FeatureBased):
                 The explanation to be transformed
```

### Comparing `pyreal-0.3.2/pyreal/transformers/impute.py` & `pyreal-0.4.0/pyreal/transformers/impute.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/transformers/one_hot_encode.py` & `pyreal-0.4.0/pyreal/transformers/one_hot_encode.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         """
         Initializes the base one-hot encoder
 
         Args:
             columns (dataframe column label type or list of dataframe column label type):
                 Label of column to select, or an ordered list of column labels to select
         """
-        self.ohe = SklearnOneHotEncoder(sparse=False)
+        self.ohe = SklearnOneHotEncoder(sparse_output=False)
         if columns is not None and not isinstance(columns, (list, tuple, np.ndarray, pd.Index)):
             columns = [columns]
         self.columns = columns
         super().__init__(**kwargs)
 
     def fit(self, x, **params):
         """
```

### Comparing `pyreal-0.3.2/pyreal/transformers/pad.py` & `pyreal-0.4.0/pyreal/transformers/pad.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/transformers/sax.py` & `pyreal-0.4.0/pyreal/transformers/sax.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/transformers/time_series_formatter.py` & `pyreal-0.4.0/pyreal/transformers/time_series_formatter.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/transformers/wrappers.py` & `pyreal-0.4.0/pyreal/transformers/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/types/explanations/decision_tree.py` & `pyreal-0.4.0/pyreal/types/explanations/decision_tree.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/types/explanations/feature_based.py` & `pyreal-0.4.0/pyreal/types/explanations/feature_based.py`

 * *Files 19% similar despite different names*

```diff
@@ -79,14 +79,31 @@
             None
         Raises:
             AssertionException
                 if `self.explanation` is invalid
         """
         super().validate()
 
+    def validate_values(self):
+        """
+        Validate that self.values are valid values for this Explanation.
+
+        Returns:
+            None
+        Raises:
+            AssertionException
+                if `self.values` is invalid
+        """
+        super().validate_values()
+        if self.values.shape != self.explanation.shape:
+            raise AssertionError(
+                "FeatureContributions expects one value per contribution. Contributions shape: %s,"
+                " values shape: %s" % (self.explanation.shape, self.values.shape)
+            )
+
 
 class AdditiveFeatureContributionExplanation(FeatureContributionExplanation):
     """
     A type wrapper for local feature contribution DataFrame type outputs from explanation
     algorithms. Local feature contribution explanations give one numeric value per instance
     per feature, representing that feature's contribution to the model's prediction
     for this instance. Contribution values can be added together with meaningful effect
@@ -100,7 +117,39 @@
         Returns:
             None
         Raises:
             AssertionException
                 if `self.explanation` is invalid
         """
         super().validate()
+
+
+class ClassFeatureContributionExplanation(FeatureBased):
+    """
+    A type wrapper for local feature contribution DataFrame type outputs from explanation
+    algorithms. Classification Local feature contribution explanations give one numeric value
+    per instance per feature per class, representing that feature's contribution to the
+    model's prediction for this instance and class.
+    """
+
+    def validate(self):
+        """
+        Validate that `self.explanation` is a valid `DataFrame`
+        Returns:
+            None
+        Raises:
+            AssertionException
+                if `self.explanation` is invalid
+        """
+        super().validate()
+
+    def validate_values(self):
+        """
+        Validate that self.values are valid values for this Explanation.
+
+        Returns:
+            None
+        Raises:
+            AssertionException
+                if `self.values` is invalid
+        """
+        super().validate_values()
```

### Comparing `pyreal-0.3.2/pyreal/types/explanations/time_series_saliency.py` & `pyreal-0.4.0/pyreal/types/explanations/time_series_saliency.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/utils/_plot_tree.py` & `pyreal-0.4.0/pyreal/utils/_plot_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             node_val = tree.value[node_id][0, :] / tree.weighted_n_node_samples[node_id]
             if tree.n_classes[0] == 1:
                 # Regression
                 node_val = tree.value[node_id][0, :]
         else:
             # If multi-output color node by impurity
             node_val = -tree.impurity[node_id]
-        return self.get_color(node_val)
+        return self.get_color(node_val).replace(" ", "0")
 
     # TODO: edit the following functions to change the sizes of the elements
     # in the plot
 
     # def export(self, decision_tree, ax=None):
     #     import matplotlib.pyplot as plt
     #     from matplotlib.text import Annotation
```

### Comparing `pyreal-0.3.2/pyreal/utils/dataloader.py` & `pyreal-0.4.0/pyreal/utils/dataloader.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/pyreal/utils/model_utils.py` & `pyreal-0.4.0/pyreal/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.3.2/PKG-INFO` & `pyreal-0.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreal
-Version: 0.3.2
+Version: 0.4.0
 Summary: Library for evaluating and deploying human readable machine learning explanations.
 Home-page: https://sibyl-ml.dev/
 Keywords: pyreal,Pyreal
 Author: Alexandra Zytek
 Author-email: zyteka@mit.edu
 Maintainer: MIT Data To AI Lab
 Maintainer-email: dailabmit@gmail.com
@@ -12,25 +12,23 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: examples
-Requires-Dist: eli5 (>=0.11,<0.14)
 Requires-Dist: lightgbm (>=3.3.2,<4.0.0) ; extra == "examples"
 Requires-Dist: lime (>=0.2.0.1,<0.3.0.0)
 Requires-Dist: matplotlib (>=3.6.0,<4.0.0)
 Requires-Dist: numba (>=0.56.2,<0.57.0)
 Requires-Dist: numpy (>=1.23.3,<2.0.0)
 Requires-Dist: pandas (>=1.5.0,<2.0.0)
 Requires-Dist: scikit-learn (>=1.1.2,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: shap (==0.40.0)
-Requires-Dist: tensorflow (>=2.6.0,<=2.10.0) ; extra == "examples"
 Project-URL: Documentation, https://sibyl-dev.github.io/pyreal
 Project-URL: Repository, https://github.com/DAI-Lab/pyreal
 Description-Content-Type: text/markdown
 
 <p align="left">
 <img width=15% src="https://dai.lids.mit.edu/wp-content/uploads/2018/06/Logo_DAI_highres.png" alt=“DAI-Lab” />
 <i>An open source project from Data to AI Lab at MIT.</i>
@@ -49,17 +47,16 @@
 - License: MIT
 - Documentation: https://pyreal.gitbook.io/pyreal
 - API Documentation: https://sibyl-ml.dev/pyreal/api_reference/index.html
 - Homepage: https://sibyl-ml.dev/
 
 # Overview
 
-**Pyreal** wraps the complete machine learning explainability pipeline into Explainer objects. Explainer objects
-handle all the transforming logic, in order to provide a human-interpretable explanation from any original
-data form.
+**Pyreal** wraps the complete machine learning explainability pipeline into RealApp objects, which seamlessly
+provide usable explanations in a low-code manner.
 
 # Install
 
 ## Requirements
 
 **Pyreal** has been developed and tested on [Python 3.8, 3.9, and 3.10](https://www.python.org/downloads/)
 The library uses Poetry for package management.
@@ -69,108 +66,82 @@
 We recommend using
 [pip](https://pip.pypa.io/en/stable/) in order to install **Pyreal**:
 
 ```
 pip install pyreal
 ```
 
-This will pull and install the latest stable release from [PyPI](https://pypi.org/).
+This will pull and install the latest stable release from [PyPI](https://pypi.org/project/pyreal/).
 
 ## Install from source
 If you do not have **poetry** installed, please head to [poetry installation guide](https://python-poetry.org/docs/#installation)
 and install poetry according to the instructions.\
 Run the following command to make sure poetry is activated. You may need to close and reopen the terminal.
 
 ```
 poetry --version
 ```
 
 Finally, you can clone this repository and install it from
-source by running `poetry install`:
+source by running `poetry install`, with the optional `examples` extras if you'd like to run our tutorial scripts.
 
 ```
 git clone git@github.com:DAI-Lab/pyreal.git
 cd pyreal
-poetry install
+poetry install -E examples
 ```
 
 ## Install for Development
 
 If you want to contribute to the project, a few more steps are required to make the project ready
 for development.
 
-Please head to the [Contributing Guide](https://sibyl-dev.github.io/pyreal/developer_guides/contributing.html)
+Please head to the [Contributing Guide](https://dtail.gitbook.io/pyreal/developer-guides/contributing-to-pyreal)
 for more details about this process.
 
 # Quickstart
 
 In this short tutorial we will guide you through a series of steps that will help you
 getting started with **Pyreal**. We will get an explanation for a prediction on whether a
 passenger on the Titanic would have survived.
 
- For a more detailed version of this tutorial, see
-`examples.titanic.titanic_lfc.ipynb`
+ For a more detailed version of this tutorial, see [our documentation](https://dtail.gitbook.io/pyreal/getting-started/quickstart).
 
-#### Load in demo dataset, pre-fit model, and transformers
+#### Load in the demo data and application
 ```
->>> import pyreal.applications.titanic as titanic
->>> from pyreal.transformers import ColumnDropTransformer, MultiTypeImputer
+>>> import pyreal.sample_applications.titanic as titanic
 
-# Load in data
->>> x_train_orig, y = titanic.load_titanic_data()
-
-# Load in feature descriptions -> dict(feature_name: feature_description, ...)
->>> feature_descriptions = titanic.load_feature_descriptions()
-
-# Load in model
->>> model = titanic.load_titanic_model()
-
-# Load in list of transformers
->>> transformers = titanic.load_titanic_transformers()
-
-# Create and fit LocalFeatureContribution Explainer object
->>> from pyreal.explainers import LocalFeatureContribution
->>> lfc = LocalFeatureContribution(model=model, x_train_orig=x_train_orig,
-...                                transformers=transformers,
-...                                feature_descriptions=feature_descriptions,
-...                                fit_on_init=True)
-
-# Make predictions on an input
->>> input_to_explain = x_train_orig.iloc[0]
->>> prediction = lfc.model_predict(input_to_explain) # Prediction: [0]
-
-# Explain an input
->>> contributions = lfc.produce(input_to_explain)
-
-# Visualize the explanation
->>> from pyreal.utils import visualize
->>> x_interpret = lfc.convert_data_to_interpretable(input_to_explain)
+>>> real_app = titanic.load_app()
+>>> sample_data = titanic.load_data(n_rows=300)
 
 ```
+#### Predict and produce explanation
+```
+>>> predictions = real_app.predict(sample_data)
 
-<!--## Install for Development
-
-TODO: Running tests should not bring up a window. Refactor into the above docstring, not actually spawning the subsequent window-->
+>>> explanation = real_app.produce_feature_contributions(sample_data)
 
-##### Plot a bar plot of top contributing features, by absolute value
 ```
-visualize.plot_top_contributors(contributions, select_by="absolute", values=x_interpret)
+#### Visualize explanation for one passenger
 ```
+passenger_id = 1
+plot_top_contributors(explanation[passenger_id], prediction=predictions[passenger_id], show=False)
 
+```
 
 The output will be a bar plot showing the most contributing features, by absolute value.
 
-![Quickstart](docs/images/quickstart.png)
+![Quickstart](docs/images/titanic.png)
 
 We can see here that the input passenger's predicted chance of survival was greatly reduced
 because of their sex (male) and ticket class (3rd class).
 
 ### Terminology
 Pyreal introduces specific terms and naming schemes to refer to different feature spaces and
 transformations. The [Terminology User Guide](https://sibyl-ml.dev/pyreal/user_guides/transformer_workflow.html#terminology) provides an introduction to these terms.
 
 # What's next?
 
 For more details about **Pyreal** and all its possibilities
 and features, please check the [documentation site](
-https://sibyl-dev.github.io/pyreal/).
+https://dtail.gitbook.io/pyreal/).
```

